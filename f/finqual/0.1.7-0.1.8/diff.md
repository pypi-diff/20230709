# Comparing `tmp/finqual-0.1.7.tar.gz` & `tmp/finqual-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "finqual-0.1.8.tar", last modified: Sun Jul  9 17:38:33 2023, max compression
```

## Comparing `finqual-0.1.7.tar` & `finqual-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finqual-0.1.7/finqual/__init__.py
--rw-r--r--   0        0        0   118812 2020-02-02 00:00:00.000000 finqual-0.1.7/finqual/finqual.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 finqual-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 finqual-0.1.7/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 finqual-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 finqual-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-09 17:38:33.263412 finqual-0.1.8/
+-rw-rw-rw-   0        0        0     1091 2023-05-30 17:24:17.000000 finqual-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     2483 2023-07-09 17:38:33.263412 finqual-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1945 2023-06-08 21:03:22.000000 finqual-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 17:38:33.257397 finqual-0.1.8/finqual/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:28:31.000000 finqual-0.1.8/finqual/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:38:33.261910 finqual-0.1.8/finqual/data/
+-rw-rw-rw-   0        0        0   434839 2023-06-14 22:18:44.000000 finqual-0.1.8/finqual/data/sec_sic.csv
+-rw-rw-rw-   0        0        0   120205 2023-07-09 17:37:48.000000 finqual-0.1.8/finqual/finqual.py
+drwxrwxrwx   0        0        0        0 2023-07-09 17:38:33.260909 finqual-0.1.8/finqual.egg-info/
+-rw-rw-rw-   0        0        0     2483 2023-07-09 17:38:33.000000 finqual-0.1.8/finqual.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-09 17:38:33.000000 finqual-0.1.8/finqual.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 17:38:33.000000 finqual-0.1.8/finqual.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-09 17:38:33.000000 finqual-0.1.8/finqual.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-09 17:38:33.263412 finqual-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      790 2023-07-09 17:12:09.000000 finqual-0.1.8/setup.py
```

### Comparing `finqual-0.1.7/finqual/finqual.py` & `finqual-0.1.8/finqual/finqual.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Import packages
 import pandas as pd
 import numpy as np
 import requests
 import ratelimit
+import datetime
 
 # Node class and respective functions
 """
 Tree class
 """
 
 class Node():
@@ -30,58 +31,120 @@
         self.children.append(obj)
         obj.parent = self
 
     def getRootParent(self):
         """
         Returns the root parent node of a given node
         """
-
         while (self.parent != None):
             self = self.parent
 
         return self
 
     def getChildrenNames(self):
-        children = []
-        for i in self.children:
-            children.append(i.name)
-        return children
+        return [child.name for child in self.children]
 
     def getChildrenNodes(self):
-        children = []
-        for i in self.children:
-            children.append(i)
-        return children
+        return self.children
 
     def dfs(self, visited):
         """
         A depth-first search function that takes in a Node class and an empty list "visited", returning a list of all the children of that Node
         """
+        visited.append(self.name)
 
-        children = self.getChildrenNodes()
-
-        for i in children:  # For each child in node
-            if i not in visited:  # If child is not in visited, then append to visited
-                visited.append(i.name)
-                for i in children:  # If child is in visited, then go into that branch
-                    i.dfs(visited)
+        for child in self.children:
+            child.dfs(visited)
 
         return visited
 
 
 # API connection class
 
 class Ticker():
 
     def __init__(self, ticker):
         self.ticker = ticker
+        self.cik = self.CIK()
         self.data = self.SEC()
+        #self.fiscal = self.fiscal_year()
+
+    def CIK(self):
+        headers = {"Accept": "application/json, text/plain, */*", "Accept-Encoding": "gzip, deflate, br",
+                   "Accept-Language": "en-US,en;q=0.9",
+                   "Origin": "https://www.nasdaq.com",
+                   "Referer": "https://www.nasdaq.com",
+                   "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36"}
+
+        source = requests.get(url="https://www.sec.gov/files/company_tickers.json", headers=headers, verify=True)
+        cik = source.json()
+        cik = pd.DataFrame(cik)
+        cik = cik.transpose()
+
+        value = str(cik.loc[cik["ticker"] == self.ticker]["cik_str"][0])
+
+        # Making sure the CIK is of right length
+        value = value.zfill(10)
+
+        return value
+
+    def is_date_between(self, date, q):
+
+        start_date = q[0]
+        end_date = q[1]
+
+        date_month = date.month
+        date_day = date.day
+
+        start_month = start_date.month
+        start_day = start_date.day
+
+        end_month = end_date.month
+        end_day = end_date.day
+
+        if start_month < end_month:
+            return (start_month, start_day) <= (date_month, date_day) <= (end_month, end_day)
+        elif start_month > end_month:
+            return (start_month, start_day) <= (date_month, date_day) or (date_month, date_day) <= (end_month, end_day)
+        else:  # start_month == end_month
+            if start_day <= end_day:
+                return (start_month, start_day) <= (date_month, date_day) <= (end_month, end_day)
+            else:  # Handle wraparound from end of year to start of year
+                return (start_month, start_day) <= (date_month, date_day) or (date_month, date_day) <= (
+                    end_month, end_day)
+
+    def date_quarter(self, date, q1, q2, q3, q4):
+        quarter_list = [(q1, 1), (q2, 2), (q3, 3), (q4, 4)]
+        for quarter, quarter_num in quarter_list:
+            if self.is_date_between(date, quarter):
+                return quarter_num
+        return None
+
+    def fiscal_year(self):
+
+        headers = {"Accept": "application/json, text/plain, */*", "Accept-Encoding": "gzip, deflate, br",
+                   "Accept-Language": "en-US,en;q=0.9",
+                   "Origin": "https://www.nasdaq.com",
+                   "Referer": "https://www.nasdaq.com",
+                   "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36"}
+
+        source = requests.get(url="https://data.sec.gov/submissions/CIK" + self.cik + ".json", headers=headers, verify=True)
+        data = source.json()
+        end = data["fiscalYearEnd"]
+        fiscal_end = datetime.datetime.strptime(end, "%m%d")
+
+        q4 = [fiscal_end + datetime.timedelta(days=-14), fiscal_end + datetime.timedelta(days=14)]
+        q1 = [q4[0] + datetime.timedelta(days=76), q4[1] + datetime.timedelta(days=104)]
+        q2 = [q1[0] + datetime.timedelta(days=76), q1[1] + datetime.timedelta(days=104)]
+        q3 = [q2[0] + datetime.timedelta(days=76), q2[1] + datetime.timedelta(days=104)]
+
+        return q1, q2, q3, q4
 
     @ratelimit.sleep_and_retry
-    @ratelimit.limits(calls = 9, period = 1)
+    @ratelimit.limits(calls = 10, period = 1)
     def SEC(self):
         """
         Function to get a Pandas dataframe from the SEC API of a chosen ticker
         """
         # Defining the headers for access
         headers = {"Accept": "application/json, text/plain, */*", "Accept-Encoding": "gzip, deflate, br",
                    "Accept-Language": "en-US,en;q=0.9",
@@ -94,321 +157,283 @@
         cik = source.json()
         cik = pd.DataFrame(cik)
         cik = cik.transpose()
 
         value = str(cik.loc[cik["ticker"] == self.ticker]["cik_str"][0])
 
         # Making sure the CIK is of right length
-        append = 10 - len(value)
-
-        for i in range(append):
-            value = "0" + value
+        value = value.zfill(10)
 
         url = 'https://data.sec.gov/api/xbrl/companyfacts/CIK' + value + '.json'
 
         # Getting the Pandas dataframe of chosen ticker
         source = requests.get(url=url, headers=headers, verify=True)
         data = source.json()
         data = pd.DataFrame(data)
 
-        return data
+        return data["facts"]
 
-    def lookup(self, node, year, category, quarter=None):
+    def lookup(self, node, year, category, quarter = None):
         """
         Looks up items that are under the "us-gaap" taxonomy and are in USD units, this has to be done year by year or quarter
         by quarter as companies may change what they file certain items under
         """
         item = node.name
         data = self.data
 
         if (category == "income"):
             """
             Creating search term
             """
-            search = "CY" + str(year)
-            if (quarter != None):
-                search = search + "Q" + str(quarter)
-            """
-            Getting the desired item value
-            """
+
             try:
+                df = pd.DataFrame(data["us-gaap"][item]["units"]["USD"])
+                df.dropna(inplace = True)
+                df["frame"] = df["frame"].str.replace('I', '')
 
-                df = pd.DataFrame(data["facts"]["us-gaap"][item]["units"]["USD"])
-                df = df.dropna()
-                return df[df["frame"] == search]["val"].iloc[0]
+                if (quarter != None):
+                    # If looking at quarter then:
+                    search = "CY" + str(year) + "Q" + str(quarter)
+                else:
+                    search = "CY" + str(year)
 
-            except:
+                return df["val"].to_numpy()[df["frame"].to_numpy() == search][0]
 
+            except:
                 return False
 
         if (category == "balance"):
 
             """
             Getting the desired item value
             """
             try:
 
-                df = pd.DataFrame(data["facts"]["us-gaap"][item]["units"]["USD"])
-                df = df.dropna()
+                df = pd.DataFrame(data["us-gaap"][item]["units"]["USD"])
+                df.dropna(inplace = True)
                 df["frame"] = df["frame"].str.replace('I', '')
                 fy = df[df["fp"] == "FY"].iloc[-1][7][-2:]
 
                 if (quarter == None):
                     search = "CY" + str(year) + fy
                 else:
                     search = "CY" + str(year) + "Q" + str(quarter)
 
-                return df[df["frame"] == search]["val"].iloc[0]
+                return df["val"].to_numpy()[df["frame"].to_numpy() == search][0]
 
             except:
 
                 return False
 
         if (category == "cashflow"):
-
             try:
-                df = pd.DataFrame(data["facts"]["us-gaap"][item]["units"]["USD"])
-                df = df.dropna()
-                df["frame"] = df["frame"].str.replace('I', '')
+                df = pd.DataFrame(data["us-gaap"][item]["units"]["USD"])
+            except:
+                return False
 
+            if (df.shape[1] == 8):
                 try:
-                    fy = df[df["fp"] == "FY"].iloc[-1][7][-2:]
+                    df.drop_duplicates(subset=["end", "val"], inplace=True, keep="last")
+                    df['end'] = pd.to_datetime(df["end"], format='%Y-%m-%d')
+
+                    df["year"] = df['end'].dt.year
+                    df["quarter"] = df["end"].dt.quarter
+                    df["quarter_frame"] = df["year"].astype(str) + "Q" + df["quarter"].astype(str)
+
+                    if (quarter == None):
+                        search = str(year) + "Q" + str(4)
+                        try:
+                            return df["val"].to_numpy()[df["quarter_frame"].to_numpy() == search][0]
+                        except:
+                            return False
+                    else:
+                        search = str(year) + "Q" + str(quarter)
+                        try:
+                            return df["val"].to_numpy()[df["quarter_frame"].to_numpy() == search][0]
+                        except:
+                            return False
                 except:
-                    fy = None
+                    pass
 
-                if (quarter != None):
-                    # If looking at quarter then:
-                    search = "CY" + str(year) + "Q" + str(quarter)
-                    return df[df["frame"] == search]["val"].iloc[0]
+            else:
+                df['end'] = pd.to_datetime(df["end"], format='%Y-%m-%d')
+                df['start'] = pd.to_datetime(df["start"], format='%Y-%m-%d')
+                df.drop_duplicates(subset=['start', "end"], inplace=True, keep="last")
+
+                df["difference_days"] = (df["end"] - df["start"]).dt.days
+                df["flag"] = df["difference_days"].between(76, 104)
+
+                df["year"] = df['end'].dt.year
+                df["quarter"] = df['end'].dt.quarter
+                df["quarter_frame"] = df["year"].astype(str) + "Q" + df["quarter"].astype(str)
+
+                df['frame'] = np.where(df['difference_days'].between(350, 380), df['year'].astype(str), np.nan)
+                df.sort_values(['year', 'quarter', "end", "difference_days"], inplace=True)
+                df.drop_duplicates(subset=['year', "quarter"], inplace=True, keep="last")
+
+                """
+                #Calculating the quarter_vals
+                """
+                df.loc[~df['flag'], 'quarter_val'] = df.groupby('start')['val'].diff(periods=1)
+                df.loc[df['quarter_val'].isnull(), 'quarter_val'] = df['val']
+                df["quarter_val"] = df["quarter_val"].astype(np.int64)
+                df.reset_index(drop=True, inplace=True)
 
-                else:
+                if (quarter == None):
+                    search = str(year)
                     try:
-                        search = "CY" + str(year)
-                        return df[df["frame"] == search]["val"].iloc[0]
-
+                        return df["val"].to_numpy()[df["frame"].to_numpy() == search][0]
                     except:
-                        pass
-
+                        return False
+                else:
+                    search = str(year) + "Q" + str(quarter)
                     try:
-                        search = "CY" + str(year) + fy
-                        return df[df["frame"] == search]["val"].iloc[0]
-
+                        return df["quarter_val"].to_numpy()[df["quarter_frame"].to_numpy() == search][0]
                     except:
                         return False
-            except:
-                return False
 
-    def tree_item(self, node, year, values, attributes, category, quarter=None):
+    def tree_item(self, node, year, values, attributes, category, quarter = None):
         """
         Returns the value of a chosen node at a certain point in time, using a tree-based node system and summing where needed
         """
         check = self.lookup(node, year, category, quarter)
-        # print(node.name + str(check))
 
         if (check != False):
             values.append(check)
             attributes.append(node.attribute)
 
         else:
-
             [self.tree_item(i, year, values, attributes, category, quarter) for i in node.getChildrenNodes()]
 
         # This is done after checking all the nodes
-
         df = pd.DataFrame(zip(values, attributes), columns=["USD", "Attribute"])
 
         # Sum credits and subtract credits
-
         parent_attribute = node.attribute
 
         if (parent_attribute == "debit"):
             value = df.loc[df["Attribute"] == "debit"]["USD"].sum() - df.loc[df["Attribute"] == "credit"]["USD"].sum()
 
         else:
             value = df.loc[df["Attribute"] == "credit"]["USD"].sum() - df.loc[df["Attribute"] == "debit"]["USD"].sum()
 
         return value
 
-    def year_tree_item(self, node, start, end, category, quarter=None):
+    def year_tree_item(self, node, start, end, category, quarter = None):
         """
         Returns a given tree_item over a timeframe
         """
-
         year_list = [i for i in np.arange(end, start - 1, -1)]
-
         values = []
 
         if quarter != None:
-
             values = [self.tree_item(node, i, [], [], category, j) for i in year_list for j in np.arange(4, 0, -1)]
 
         else:
-
             values = [self.tree_item(node, i, [], [], category) for i in year_list]
 
         return values
 
-    def income(self, start, end, quarter=None, readable=None, category="cashflow"):
-
-        if quarter != None and readable != None:
-            df = self.income1(start, end, quarter=True, readable=True, category="cashflow")
-        elif quarter != None and readable == None:
-            df = self.income1(start, end, quarter=True, readable=None, category="cashflow")
-        elif quarter == None and readable != None:
-            df = self.income1(start, end, quarter=None, readable=None, category="cashflow")
-        else:
-            df = self.income1(start, end, quarter=None, readable=None, category="cashflow")
+    def income(self, start, end, category = "income", quarter = None, readable = None):
 
+        df = self.income_helper(start, end, category, quarter, readable)
         df = df.drop(["Cost and Expenses", "Interest Expense", "Depreciation and Amortization"])
 
         return df
 
-    def income1(self, start, end, quarter=None, readable=None, category="cashflow"):
+    def income_helper(self, start, end, category, quarter = None, readable = None):
         """
         Creating list of years and quarters for columns
         """
         year_list = [i for i in np.arange(end, start - 2, -1)]
-
         quarter_list = [str(i) + "Q" + str(j) for i in year_list for j in np.arange(4, 0, -1)]
-
         """
         Creating list of income statement items and their names
         """
-        nodes = [rev, cor, gp, opex, ce, oi, noi, pti, tax, ni, cce5_2, ide1_1]
-
+        nodes = [rev, cor, gp, opex, ce,
+                 oi,
+                 noi, pti, tax, ni, cce5_2,
+                 ide1_1]
         node_names = ["Revenues", "Cost of Revenue", "Gross Profit", "Operating Expenses", "Cost and Expenses",
                       "Operating Profit"
-            , "Non-Operating Income/Expense", "Pretax Profit", "Tax", "Net Profit", "Depreciation and Amortization"
-            , "Interest Expense"]
-
+                     ,"Non-Operating Income/Expense", "Pretax Profit", "Tax", "Net Profit", "Depreciation and Amortization"
+                     ,"Interest Expense"]
         """
         Appending each node values for each year to a data
         """
         if quarter == True:
-            data = [self.year_tree_item(i, start - 1, end, quarter=True, category="cashflow") for i in nodes]
-            df = pd.DataFrame(data, index=[node_names], columns=[quarter_list])
-
-            df.columns = df.columns.get_level_values(0)
-            df.index = df.index.get_level_values(0)
+            data = [self.year_tree_item(i, start - 1, end, category, quarter) for i in nodes]
+            df = pd.DataFrame(data, index = [node_names], columns = [quarter_list])
 
             """
             Get the missing quarter stuff, some zeros will be replaced at sense-checking stage, the zeros will signify the quarter that the company reports in
             """
-
             for i in np.arange(start, end + 1):
-
                 df1 = df.filter(regex=str(i))  # Filtering for only a year i's items
-
                 try:
                     position = [True if self.MissingQuarter(df1, i) > 3 else False for i in df1.columns].index(True)
-
                     label = df1.columns[position]  # Getting the column name of the label
-                    # Getting the last four quarters from label backwards, using the original dataframe
                     idx = df.columns.get_loc(label)
-                    idx_list = [x for x in np.arange(idx, idx + 4)]
+                    idx_list = [x for x in np.arange(idx, idx + 4)]   # Getting the last four quarters from label backwards by index
                     df1 = df.iloc[:, idx_list]  # Getting the dataframe for the chosen four quarters
-                    totals = [df1.loc[i].sum() for i in
-                              df1.index]  # Summing across income statement items for a given year's quarters
 
+                    totals = df1.sum(axis = 1).values  # Summing across income statement items for a given year's quarters
                     """
                     Getting the annual figures for comparison into an "actual" list
                     """
                     if readable == True:
-                        annual = [int(x.replace(',', '')) for x in
-                                  self.income1(i, i, quarter=False, readable=True, category="cashflow")[i]]
+                        annual = [int(x.replace(',', '')) for x in self.income_helper(i, i, category = "income", quarter = False, readable = True)[i]]
                     else:
-                        annual = list(self.income1(i, i, quarter=False, readable=False, category="cashflow")[i])
+                        annual = list(self.income_helper(i, i, category = "income", quarter = False, readable = False)[i])
 
-                    changed = list(
-                        df.loc[:, label])  # The list of values that are to be changed, i.e. the incorrect column
+                    changed = list(df.loc[:, label])  # The list of values that are to be changed, i.e. the incorrect column
 
-                    diff = [a - b + c for a, b, c in
-                            zip(annual, totals, changed)]  # Reconcile discrepancies and the actual figures
+                    diff = [a - b + c for a, b, c in zip(annual, totals, changed)]  # Reconcile discrepancies and the actual figures
                     df.loc[:, label] = diff
 
-
                 except:
 
                     continue
 
-            """
-            Sense-checking
-            """
-
-            df.loc["Cost of Revenue"] = [
-                df.loc["Revenues"][str(i) + "Q" + str(j)] - df.loc["Gross Profit"][str(i) + "Q" + str(j)] for i in
-                np.arange(end, start - 2, -1) for j in np.arange(4, 0, -1)]
-
-            df.loc["Operating Expenses"] = [
-                df.loc["Gross Profit"][str(i) + "Q" + str(j)] - df.loc["Operating Profit"][str(i) + "Q" + str(j)] for i
-                in np.arange(end, start - 2, -1) for j in np.arange(4, 0, -1)]
-
-            df.loc["Non-Operating Income/Expense"] = [
-                df.loc["Pretax Profit"][str(i) + "Q" + str(j)] - df.loc["Operating Profit"][str(i) + "Q" + str(j)] for i
-                in np.arange(end, start - 2, -1) for j in np.arange(4, 0, -1)]
-
-            df.loc["EBIT"] = [df.loc["Net Profit"][str(i) + "Q" + str(j)] + df.loc["Tax"][str(i) + "Q" + str(j)] +
-                              df.loc["Interest Expense"][str(i) + "Q" + str(j)] for i in np.arange(end, start - 2, -1)
-                              for j in np.arange(4, 0, -1)]
-
-            df.loc["EBITDA"] = [
-                df.loc["EBIT"][str(i) + "Q" + str(j)] + df.loc["Depreciation and Amortization"][str(i) + "Q" + str(j)]
-                for i in np.arange(end, start - 2, -1) for j in np.arange(4, 0, -1)]
-
         else:
 
-            data = [self.year_tree_item(i, start - 1, end, category="cashflow") for i in nodes]
+            data = [self.year_tree_item(i, start - 1, end, category = "income") for i in nodes]
             df = pd.DataFrame(data, index=[node_names], columns=[year_list])
 
-            df.columns = df.columns.get_level_values(0)
-            df.index = df.index.get_level_values(0)
-
-            """
-            Sense-checking
-            """
-
-            df.loc["Cost of Revenue"] = [df.loc["Revenues"][i] - df.loc["Gross Profit"][i] for i in
-                                         np.arange(end, start - 2, -1)]
+        df.columns = df.columns.get_level_values(0)
+        df.index = df.index.get_level_values(0)
 
-            for i in df.columns:
-                if (df.loc["Cost of Revenue", i] == 0 and df.loc["Cost and Expenses", i] != 0 and df.loc[
-                    "Operating Expenses", i] != 0):
-                    df.loc["Cost of Revenue", i] = df.loc["Cost and Expenses", i] - df.loc["Operating Expenses", i]
-
-            df.loc["Gross Profit"] = [df.loc["Revenues"][i] - df.loc["Cost of Revenue"][i] for i in
-                                      np.arange(end, start - 2, -1)]
+        """
+        Sense-checking
+        """
 
-            for i in df.columns:
-                if (df.loc["Operating Profit", i] == 0 and df.loc["Operating Expenses", i] != 0 and df.loc[
-                    "Gross Profit", i] != 0):
-                    df.loc["Operating Profit", i] = df.loc["Gross Profit", i] - df.loc["Operating Expenses", i]
+        df.loc["Cost of Revenue"] = df.loc["Revenues"] - df.loc["Gross Profit"]
 
-            df.loc["Operating Expenses"] = [df.loc["Gross Profit"][i] - df.loc["Operating Profit"][i] for i in
-                                            np.arange(end, start - 2, -1)]
+        mask = (df.loc["Cost of Revenue"] == 0) & (df.loc["Cost and Expenses"] != 0) & (df.loc["Operating Expenses"] != 0)
+        df.loc["Cost of Revenue", mask] = df.loc["Cost and Expenses", mask] - df.loc["Operating Expenses", mask]
 
-            df.loc["Non-Operating Income/Expense"] = [df.loc["Pretax Profit"][i] - df.loc["Operating Profit"][i] for i
-                                                      in np.arange(end, start - 2, -1)]
+        df.loc["Gross Profit"] = df.loc["Revenues"] - df.loc["Cost of Revenue"]
 
-            df.loc["EBIT"] = [df.loc["Net Profit"][i] + df.loc["Tax"][i] + df.loc["Interest Expense"][i] for i in
-                              np.arange(end, start - 2, -1)]
+        mask = (df.loc["Operating Profit"] == 0) & (df.loc["Operating Expenses"] != 0) & (df.loc["Gross Profit"] != 0)
+        df.loc["Operating Profit", mask] = df.loc["Gross Profit", mask] - df.loc["Operating Expenses", mask]
 
-            df.loc["EBITDA"] = [df.loc["EBIT"][i] + df.loc["Depreciation and Amortization"][i] for i in
-                                np.arange(end, start - 2, -1)]
+        df.loc["Operating Expenses"] = df.loc["Gross Profit"] - df.loc["Operating Profit"]
+        df.loc["Non-Operating Income/Expense"] = df.loc["Pretax Profit"] - df.loc["Operating Profit"]
+        df.loc["EBIT"] = df.loc["Net Profit"] + df.loc["Tax"] + df.loc["Interest Expense"]
+        df.loc["EBITDA"] = df.loc["EBIT"] + df.loc["Depreciation and Amortization"]
 
         if readable == True:
-
             df = df.applymap(lambda x: '{:,}'.format(x))
             df = df.loc[:, (df != 0).any(axis=0)]
-            df = df[df.columns.drop(list(df.filter(regex=str(start - 1))))]
+            df.drop(df.filter(regex=str(start - 1)).columns, axis=1, inplace=True)
             return df
 
         else:
-
-            # df = df.loc[:, (df != 0).any(axis=0)]
-            df = df[df.columns.drop(list(df.filter(regex=str(start - 1))))]
+            df = df.loc[:, (df != 0).any(axis=0)] #Remove columns that have all zeros
+            df.drop(df.filter(regex=str(start - 1)).columns, axis=1, inplace=True)
             return df
 
     def MissingQuarter(self, df, column):
         """
         Returns the number of times 0 appears in a column
         """
         try:
@@ -417,114 +442,63 @@
             return 0
 
     def cashflow(self, start, end, quarter=None, readable=None, category="cashflow"):
         """
         Creating list of years and quarters for columns
         """
         year_list = [i for i in np.arange(end, start - 1, -1)]
-
         quarter_list = [str(i) + "Q" + str(j) for i in year_list for j in np.arange(4, 0, -1)]
-
         """
         Creating list of income statement items and their names
         """
-
         nodes = [cce2_3, cce2_4, cce2_5, cce1_1, cce1, cce4_8]
 
         node_names = ["Operating Cash Flow", "Investing Cash Flow", "Financing Cash Flow",
                       "Effect of Exchange Rate on Cash", "End Cash Position", "Capital Expenditures"]
-
         """
         Appending each node values for each year to a data
         """
         if quarter == True:
-            data = [self.year_tree_item(i, start, end, quarter=True, category="cashflow") for i in nodes]
-            df = pd.DataFrame(data, index=[node_names], columns=[quarter_list])
-
-            df.columns = df.columns.get_level_values(0)
-            df.index = df.index.get_level_values(0)
-
-            for i in np.arange(start, end + 1):
-
-                df1 = df.filter(regex=str(i))  # Filtering for only a year i's items
-
-                totals = [df1.loc[i].sum() for i in
-                          df1.index]  # Summing across income statement items for a given year's quarters
-
-                try:
-                    position = [True if self.MissingQuarter(df1, i) > 3 else False for i in df1.columns].index(True)
-
-                    label = df1.columns[position]  # Getting the column name of the label
-
-                    """
-                    Getting the annual figures for comparison into an "actual" list
-                    """
-                    if readable == True:
-                        annual = [int(x.replace(',', '')) for x in
-                                  self.cashflow(i, i, quarter=False, readable=True, category="cashflow")[i]]
-                    else:
-                        annual = list(self.cashflow(i, i, quarter=False, readable=False, category="cashflow")[i])
-
-                    changed = list(
-                        df1.iloc[:, position])  # The list of values that are to be changed, i.e. the incorrect column
-
-                    diff = [a - b - c for a, b, c in
-                            zip(annual, totals, changed)]  # Reconcile discrepancies and the actual figures
-
-                    df.loc[:, label] = diff
-
-                except:
-
-                    continue
-
-            df.loc["Free Cash Flow"] = [
-                df.loc["Operating Cash Flow"][str(i) + "Q" + str(j)] - df.loc["Capital Expenditures"][
-                    str(i) + "Q" + str(j)] for i in np.arange(end, start - 1, -1) for j in np.arange(4, 0, -1)]
+            data = [self.year_tree_item(i, start, end, quarter = True, category = "cashflow") for i in nodes]
+            df = pd.DataFrame(data, index = [node_names], columns = [quarter_list])
 
         else:
+            data = [self.year_tree_item(i, start, end, category = "cashflow") for i in nodes]
+            df = pd.DataFrame(data, index = [node_names], columns = [year_list])
 
-            data = [self.year_tree_item(i, start, end, category="cashflow") for i in nodes]
-            df = pd.DataFrame(data, index=[node_names], columns=[year_list])
-
-            df.columns = df.columns.get_level_values(0)
-            df.index = df.index.get_level_values(0)
+        df.columns = df.columns.get_level_values(0)
+        df.index = df.index.get_level_values(0)
 
-            df.loc["Free Cash Flow"] = [df.loc["Operating Cash Flow"][i] - df.loc["Capital Expenditures"][i] for i in
-                                        np.arange(end, start - 1, -1)]
+        df.loc["Free Cash Flow"] = df.loc["Operating Cash Flow"] - df.loc["Capital Expenditures"]
+        df.drop(["Capital Expenditures"], inplace=True)
+        df = df.loc[:, (df != 0).any(axis=0)]
 
         if readable == True:
-
             df = df.applymap(lambda x: '{:,}'.format(x))
-            df = df.loc[:, (df != 0).any(axis=0)]
-            df = df.drop(["Capital Expenditures"])
             return df
-
         else:
-
-            df = df.loc[:, (df != 0).any(axis=0)]
-            df = df.drop(["Capital Expenditures"])
             return df
 
-    def balance(self, start, end, quarter=None, readable=None):
+    def balance(self, start, end, quarter = None, readable = None):
         """
         Creating list of years and quarters for columns
         """
         year_list = [i for i in np.arange(end, start - 1, -1)]
-
         quarter_list = [str(i) + "Q" + str(j) for i in year_list for j in np.arange(4, 0, -1)]
 
         """
         Creating list of income statement items and their names
         """
 
         nodes = [ca2_1, ca2_2, ca1_4, ca2_12, ca1_34, ca,
                  nca1_13, nca1_19, nca1_36, nca,
                  cl2_1, cl2_2, cl1_2, cl1_3, cl1_27, cl,
                  ncl1_1, ncl1_2, ncl,
-                 se2_3, se2_8, se2_12, se2_14, se1_1, se1_2,
+                 se2_3, se2_8, se2_12, se2_14,
+                 se1_1, se1_2,
                  a, l, se]
 
         node_names = ["Cash and Cash Equivalents", "Short-term Investments", "Accounts Receivable, Net", "Inventories",
                       "Other Current Assets", "Total Current Assets",
                       "Property Plant and Equipment", "Intangibles", "Other Non-Current Assets",
                       "Total Non-Current Assets",
                       "Accounts Payable", "Accrued Liabilities", "Deferred Revenue", "Short-term Borrowings",
@@ -534,96 +508,159 @@
                       "Stockholder's Equity", "Minority Interest",
                       "Total Assets", "Total Liabilities", "Total Equity"]
 
         """
         Appending each node values for each year to a data
         """
         if quarter == True:
-            data = [self.year_tree_item(i, start, end, category="balance", quarter=True) for i in
-                    nodes]  # Fetching the data
-            df = pd.DataFrame(data, index=[node_names], columns=[
-                quarter_list])  # Creating the dataframe with columns and index according to the list
-
-            df.columns = df.columns.get_level_values(0)  # Resetting to flat index
-            df.index = df.index.get_level_values(0)  # Resetting to flat index
-
-            """
-            Sense-checking
-            """
-            df.loc["Total Non-Current Assets"] = [
-                df.loc["Total Assets"][str(i) + "Q" + str(j)] - df.loc["Total Current Assets"][str(i) + "Q" + str(j)]
-                for i in np.arange(end, start - 1, -1) for j in np.arange(4, 0, -1)]
-            df.loc["Other Current Assets"] = [
-                df.loc["Total Current Assets"][str(i) + "Q" + str(j)] - df.iloc[0:4][str(i) + "Q" + str(j)].sum() for i
-                in np.arange(end, start - 1, -1) for j in np.arange(4, 0, -1)]
-            df.loc["Other Non-Current Assets"] = [
-                df.loc["Total Non-Current Assets"][str(i) + "Q" + str(j)] - df.iloc[6:7][str(i) + "Q" + str(j)].sum()
-                for i in np.arange(end, start - 1, -1) for j in np.arange(4, 0, -1)]
-
-            df.loc["Other Current Liabilities"] = [
-                df.loc["Total Current Liabilities"][str(i) + "Q" + str(j)] - df.iloc[11:15][str(i) + "Q" + str(j)].sum()
-                for i in np.arange(end, start - 1, -1) for j in np.arange(4, 0, -1)]
-            df.loc["Total Non-Current Liabilities"] = [
-                df.loc["Total Liabilities"][str(i) + "Q" + str(j)] - df.loc["Total Current Liabilities"][
-                    str(i) + "Q" + str(j)].sum() for i in np.arange(end, start - 1, -1) for j in np.arange(4, 0, -1)]
-            df.loc["Non-Debt Long Term Liabilities"] = [
-                df.loc["Total Non-Current Liabilities"][str(i) + "Q" + str(j)] - df.loc["Long-Term Debt"][
-                    str(i) + "Q" + str(j)].sum() for i in np.arange(end, start - 1, -1) for j in np.arange(4, 0, -1)]
-
-            df.loc["Accumulated Other Change"] = [
-                df.loc["Stockholder's Equity"][str(i) + "Q" + str(j)] - df.iloc[21:24][str(i) + "Q" + str(j)].sum() for
-                i in np.arange(end, start - 1, -1) for j in np.arange(4, 0, -1)]
-            df.loc["Minority Interest"] = [
-                df.loc["Total Equity"][str(i) + "Q" + str(j)] - df.loc["Stockholder's Equity"][
-                    str(i) + "Q" + str(j)].sum() for i in np.arange(end, start - 1, -1) for j in np.arange(4, 0, -1)]
+            data = [self.year_tree_item(i, start, end, category = "balance", quarter=True) for i in nodes]  # Fetching the data
+            df = pd.DataFrame(data, index=[node_names], columns=[quarter_list])  # Creating the dataframe with columns and index according to the list
 
         else:
+            data = [self.year_tree_item(i, start, end, category = "balance") for i in nodes]
+            df = pd.DataFrame(data, index=[node_names], columns=[year_list])
 
-            data = [self.year_tree_item(i, start, end, category="balance") for i in nodes]
+        df.columns = df.columns.get_level_values(0)
+        df.index = df.index.get_level_values(0)
 
-            df = pd.DataFrame(data, index=[node_names], columns=[year_list])
+        """
+        Sense-checking
+        """
+        df.loc["Total Non-Current Assets"] = df.loc["Total Assets"] - df.loc["Total Current Assets"]
+        df.loc["Other Current Assets"] = df.loc["Total Current Assets"] - df.iloc[0:4].sum()
+        df.loc["Other Non-Current Assets"] = df.loc["Total Non-Current Assets"] - df.iloc[6:7].sum()
 
-            df.columns = df.columns.get_level_values(0)
-            df.index = df.index.get_level_values(0)
+        df.loc["Other Current Liabilities"] = df.loc["Total Current Liabilities"] - df.iloc[11:15].sum()
+        df.loc["Total Non-Current Liabilities"] = df.loc["Total Liabilities"] - df.loc["Total Current Liabilities"]
+        df.loc["Non-Debt Long Term Liabilities"] = df.loc["Total Non-Current Liabilities"] - df.loc["Long-Term Debt"]
 
-            """
-            Sense-checking
-            """
-            df.loc["Total Non-Current Assets"] = [df.loc["Total Assets"][i] - df.loc["Total Current Assets"][i] for i in
-                                                  np.arange(end, start - 1, -1)]
-            df.loc["Other Current Assets"] = [df.loc["Total Current Assets"][i] - df.iloc[0:4][i].sum() for i in
-                                              np.arange(end, start - 1, -1)]
-            df.loc["Other Non-Current Assets"] = [df.loc["Total Non-Current Assets"][i] - df.iloc[6:7][i].sum() for i in
-                                                  np.arange(end, start - 1, -1)]
-
-            df.loc["Other Current Liabilities"] = [df.loc["Total Current Liabilities"][i] - df.iloc[11:15][i].sum() for
-                                                   i in np.arange(end, start - 1, -1)]
-            df.loc["Total Non-Current Liabilities"] = [
-                df.loc["Total Liabilities"][i] - df.loc["Total Current Liabilities"][i].sum() for i in
-                np.arange(end, start - 1, -1)]
-            df.loc["Non-Debt Long Term Liabilities"] = [
-                df.loc["Total Non-Current Liabilities"][i] - df.loc["Long-Term Debt"][i].sum() for i in
-                np.arange(end, start - 1, -1)]
-
-            df.loc["Accumulated Other Change"] = [df.loc["Stockholder's Equity"][i] - df.iloc[19:22][i].sum() for i in
-                                                  np.arange(end, start - 1, -1)]
-            df.loc["Minority Interest"] = [df.loc["Total Equity"][i] - df.loc["Stockholder's Equity"][i].sum() for i in
-                                           np.arange(end, start - 1, -1)]
+        df.loc["Accumulated Other Change"] = df.loc["Stockholder's Equity"] - df.iloc[19:22].sum()
+        df.loc["Minority Interest"] = df.loc["Total Equity"] - df.loc["Stockholder's Equity"]
 
         if readable == True:
 
             df = df.applymap(lambda x: '{:,}'.format(x))
             df = df.loc[:, (df != 0).any(axis=0)]
             return df
 
         else:
 
             df = df.loc[:, (df != 0).any(axis=0)]
             return df
 
+    def comparables(self, n, level = None):
+
+        if level == None:
+            level = 4
+
+        sic = pd.read_csv('data/sec_sic.csv', index_col=0)
+        sic = sic.dropna()
+
+        sic["SIC"] = sic["SIC"].astype(int)
+        sic["SIC"] = sic["SIC"].astype(str)
+        sic['SIC'] = sic['SIC'].apply(lambda x: x[:level])
+        sic["SIC"] = sic["SIC"].astype(int)
+
+        sic_code = sic[sic["ticker"] == self.ticker]["SIC"].values[0]
+        company_list = sic[sic["SIC"] == sic_code].copy()
+        company_list.drop(["cik_str"], axis=1, inplace=True)
+        company_list.reset_index(drop=True, inplace=True)
+
+        sic_index = company_list[company_list['ticker'] == self.ticker].index[0]  # Getting index of desired row
+
+        n_above = n // 2
+        n_below = n - n_above
+
+        start_row = max(0, sic_index - n_above)  # Getting the index
+        end_row = min(sic_index + n_below, len(company_list) - 1)
+
+        surronding_companies = company_list.iloc[start_row:end_row + 1]
+
+        if len(surronding_companies) < (n + 1):
+            n_below = n - len(surronding_companies) + 1
+            end_row = min(end_row + n_below, len(company_list) - 1)
+            surronding_companies = company_list.iloc[start_row:end_row + 1]
+
+        if len(surronding_companies) < (n + 1):
+            n_above = n - len(surronding_companies) + 1
+            start_row = max(0, start_row - n_above)
+            surronding_companies = company_list.iloc[start_row:end_row + 1]
+
+        surronding_companies = surronding_companies.rename(columns={'ticker': 'Ticker', 'title': 'Name'})
+
+        return surronding_companies
+
+    def ratios(self, start, end):
+
+        df = self.data
+
+        balance_r = self.balance(start - 1, end)
+        income_r = self.income(start, end)
+        cash_r = self.cashflow(start, end)
+
+        year_list = [i for i in np.arange(end, start - 1, -1)]
+
+        cap_df = pd.DataFrame(df["dei"]["EntityPublicFloat"]["units"]["USD"])
+        cap_df["fy"] = cap_df["frame"].str[2:6]
+
+        cap = []
+        for i in year_list:
+            try:
+                cap.append(cap_df.loc[cap_df['fy'] == str(i), 'val'].iloc[0])
+            except:
+                cap.append(None)
+
+        cap = pd.Series(cap, index=year_list)
+
+        ebitda = income_r.loc["EBITDA"]
+        ebit = income_r.loc["EBIT"]
+        net_profit = income_r.loc["Net Profit"]
+        operating_profit = income_r.loc["Operating Profit"]
+        tax = income_r.loc["Tax"]
+
+        current_assets = balance_r.loc["Total Current Assets"]
+        total_assets = balance_r.loc["Total Assets"]
+        current_liabilities = balance_r.loc["Total Current Liabilities"]
+        total_liabilities = balance_r.loc["Total Liabilities"]
+        total_se = balance_r.loc["Stockholder's Equity"]
+        total_equity = balance_r.loc["Total Equity"]
+        inventory = balance_r.loc["Inventories"]
+        cash = balance_r.loc["Cash and Cash Equivalents"]
+
+        fcf = cash_r.loc["Free Cash Flow"]
+
+        nwc = (current_assets - current_liabilities).diff(-1)
+
+        d_a = pd.Series(self.year_tree_item(cce5_2, start, end, "income"), index=year_list)
+        capex = pd.Series(self.year_tree_item(cce4_8, start, end, "cashflow"), index=year_list)
+        ufcf = operating_profit + tax - capex + d_a - nwc
+
+        cap = cap + total_liabilities - cash
+
+        ratio_df = pd.DataFrame(columns=year_list)
+
+        ratio_df.loc["Current Ratio"] = (current_assets / current_liabilities)
+        ratio_df.loc["Quick Ratio"] = ((current_assets - inventory) / current_liabilities)
+
+        ratio_df.loc["Debt-to-Equity Ratio"] = (total_liabilities / total_se)
+
+        ratio_df.loc["Return on Equity"] = (net_profit / total_se)
+        ratio_df.loc["Return on Assets"] = (net_profit / total_assets)
+        ratio_df.loc["Return on Capital Employed"] = ebit / (total_assets - current_liabilities)
+        ratio_df.loc["Return on Invested Capital"] = (operating_profit + tax) / (total_liabilities + total_equity)
+
+        ratio_df.loc["FCFF Yield"] = ufcf / (cap)
+
+        ratio_df.loc["EV/EBITDA"] = (cap / ebitda)
+
+        ratio_df.dropna(axis=1, how='all', inplace=True)
+
+        ratio_df["Mean"] = ratio_df.mean(axis=1)
+
+        return ratio_df
 
 """
 Net Income
 """
 ni = Node("NetIncomeLoss", attribute="credit")
 
 # Level 1
@@ -1980,41 +2017,36 @@
              parent=se3_8)
 se4_2 = Node("DefinedBenefitPlanAccumulatedOtherComprehensiveIncomeNetPriorServiceCostCreditAfterTax",
              attribute="debit", parent=se3_8)
 se4_3 = Node("DefinedBenefitPlanAccumulatedOtherComprehensiveIncomeNetTransitionAssetsObligationsAfterTax",
              attribute="credit", parent=se3_8)
 
 """
-Cash and Cash Equivalents
+Cash and Cash Equivalents - Cashflow
 """
 # Level 0
 cce = Node("CashAndCashEquivalentsPeriodIncreaseDecrease", attribute="debit")
 
+
 # End-cash position
 cce1 = Node("CashCashEquivalentsRestrictedCashAndRestrictedCashEquivalents", attribute="debit")
-cce2 = Node(
-    "CashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsIncludingDisposalGroupAndDiscontinuedOperations",
-    attribute="debit", parent=cce1)
+cce2 = Node("CashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsIncludingDisposalGroupAndDiscontinuedOperations", attribute="debit", parent=cce1)
+cce3 = Node("CashAndCashEquivalentsAtCarryingValue", attribute="debit", parent=cce2)
 
 # Level 1
 
-cce1_1 = Node(
-    "EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsIncludingDisposalGroupAndDiscontinuedOperations",
-    attribute="debit", parent=cce)
+cce1_1 = Node("EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsIncludingDisposalGroupAndDiscontinuedOperations", attribute="debit", parent=cce)
 cce1_3 = Node("EffectOfExchangeRateOnCashAndCashEquivalents", attribute="debit", parent=cce1_1)
 
 cce1_2 = Node("CashAndCashEquivalentsPeriodIncreaseDecreaseExcludingExchangeRateEffect", attribute="debit", parent=cce)
 
 # Level 2
 
-cce2_1 = Node("EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalents", attribute="debit",
-              parent=cce1_3)
-cce2_2 = Node(
-    "EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsDisposalGroupIncludingDiscontinuedOperations",
-    attribute="debit", parent=cce2_1)
+cce2_1 = Node("EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalents", attribute="debit", parent=cce1_3)
+cce2_2 = Node("EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsDisposalGroupIncludingDiscontinuedOperations", attribute="debit", parent=cce2_1)
 
 cce2_3 = Node("NetCashProvidedByUsedInOperatingActivities", attribute="debit", parent=cce1_2)
 cce2_4 = Node("NetCashProvidedByUsedInInvestingActivities", attribute="debit", parent=cce1_2)
 cce2_5 = Node("NetCashProvidedByUsedInFinancingActivities", attribute="debit", parent=cce1_2)
 
 # Level 3
 
@@ -2033,16 +2065,15 @@
 
 # Level 4
 
 cce4_1 = Node("IncomeLossIncludingPortionAttributableToNoncontrollingInterest", attribute="credit", parent=cce3_1)
 cce4_2 = Node("IncomeTaxExpenseBenefitContinuingOperationsDiscontinuedOperationsExtraordinaryItems", attribute="debit",
               parent=cce3_1)
 
-cce4_3 = Node("AdjustmentsNoncashItemsToReconcileNetIncomeLossToCashProvidedByUsedInOperatingActivities",
-              attribute="debit", parent=cce3_2)
+cce4_3 = Node("AdjustmentsNoncashItemsToReconcileNetIncomeLossToCashProvidedByUsedInOperatingActivities", attribute="debit", parent=cce3_2)
 cce4_4 = Node("PaymentsForProceedsFromTenantAllowance", attribute="credit", parent=cce3_2)
 cce4_5 = Node("PaymentsForProceedsFromOtherDeposits", attribute="credit", parent=cce3_2)
 cce4_6 = Node("IncreaseDecreaseInOperatingCapital", attribute="credit", parent=cce3_2)
 cce4_7 = Node("OtherOperatingActivitiesCashFlowStatement", attribute="debit", parent=cce3_2)
 
 cce4_8 = Node("PaymentsForProceedsFromProductiveAssets", attribute="credit", parent=cce3_3)
```

### Comparing `finqual-0.1.7/LICENSE.txt` & `finqual-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finqual-0.1.7/README.md` & `finqual-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `finqual-0.1.7/PKG-INFO` & `finqual-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-Metadata-Version: 2.1
-Name: finqual
-Version: 0.1.7
-Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet and cashflow statement directly from the SEC with no request caps and fast request rate limits
-Author: Myztika
-License-File: LICENSE.txt
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
-# finqual
-
-This is a work in progress package that enables users to programmatically access the SEC EDGAR API database to retrieve financial information such as income statement, balance sheet or cash flow statement.
-
-## Features
-Ability to call the income statement, balance sheet or cash flow statement for any company on the within EDGAR, the SEC's Electronic Data Gathering, Analysis, and Retrieval system.
-
-This has two key features that enable better programmatic access compared to other providers:
-- Ability to call up to 10 requests per second, with built-in rate limiter
-- No restriction on the number of calls within a certain timeframe
-
-## Functionality
-
-First, ensure that the required packages are installed (see the "Dependencies" section). Import the package using:
-```
-from finqual import finqual as fq
-```
-
-From there, use a "Ticker" class to call the desired stock and the desired financial statement. For example:
-```
-fq.Ticker("TSLA").income(2020,2022)
-fq.Ticker("TSLA").balance(2020,2022, quarter = True)
-fq.Ticker("TSLA").cashflow(2020,2022)
-```
-
-Note that the financial statement function takes a mandatory timeframe input and then an optional input to return the quarterly results within that timeframe (default to annual results if not inputted).
-
-## Dependencies
-
-Only four packages are required, with the following versions confirmed to be working:
-
-| Package   | Version  |
-|-----------|----------|
-| pandas    | ≥ 2.0.2  |
-| numpy     | ≥ 1.24.3 |
-| requests  | ≥ 2.31.0 |
-| ratelimit | ≥ 2.2.1  |
-
-## Limitations
-Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
-
-- Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database, and quite prevalent for quarterly reports as well
-- More comprehensive mappings from known tags
+Metadata-Version: 2.1
+Name: finqual
+Version: 0.1.8
+Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet, and cash flow statement directly from the SEC with no request caps and fast request rate limits.
+Author: Myztika
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# finqual
+
+This is a work in progress package that enables users to programmatically access the SEC EDGAR API database to retrieve financial information such as income statement, balance sheet or cash flow statement.
+
+## Features
+Ability to call the income statement, balance sheet or cash flow statement for any company on the within EDGAR, the SEC's Electronic Data Gathering, Analysis, and Retrieval system.
+
+This has two key features that enable better programmatic access compared to other providers:
+- Ability to call up to 10 requests per second, with built-in rate limiter
+- No restriction on the number of calls within a certain timeframe
+
+## Functionality
+
+First, ensure that the required packages are installed (see the "Dependencies" section). Import the package using:
+```
+from finqual import finqual as fq
+```
+
+From there, use a "Ticker" class to call the desired stock and the desired financial statement. For example:
+```
+fq.Ticker("TSLA").income(2020,2022)
+fq.Ticker("TSLA").balance(2020,2022, quarter = True)
+fq.Ticker("TSLA").cashflow(2020,2022)
+```
+
+Note that the financial statement function takes a mandatory timeframe input and then an optional input to return the quarterly results within that timeframe (default to annual results if not inputted).
+
+## Dependencies
+
+Only four packages are required, with the following versions confirmed to be working:
+
+| Package   | Version  |
+|-----------|----------|
+| pandas    | â‰¥ 2.0.2  |
+| numpy     | â‰¥ 1.24.3 |
+| requests  | â‰¥ 2.31.0 |
+| ratelimit | â‰¥ 2.2.1  |
+
+## Limitations
+Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
+
+- Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database, and quite prevalent for quarterly reports as well
+- More comprehensive mappings from known tags
```

