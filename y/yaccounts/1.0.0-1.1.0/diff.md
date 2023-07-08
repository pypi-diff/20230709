# Comparing `tmp/yaccounts-1.0.0.tar.gz` & `tmp/yaccounts-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaccounts-1.0.0.tar", last modified: Fri Jul  7 21:31:50 2023, max compression
+gzip compressed data, was "yaccounts-1.1.0.tar", last modified: Sat Jul  8 21:48:11 2023, max compression
```

## Comparing `yaccounts-1.0.0.tar` & `yaccounts-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-07 21:31:50.834701 yaccounts-1.0.0/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-07 21:31:50.834701 yaccounts-1.0.0/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-07 21:31:50.834701 yaccounts-1.0.0/setup.cfg
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      385 2023-07-07 21:28:10.000000 yaccounts-1.0.0/setup.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-07 21:31:50.834701 yaccounts-1.0.0/yaccounts/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-07 21:28:10.000000 yaccounts-1.0.0/yaccounts/__init__.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1510 2023-07-07 21:28:10.000000 yaccounts-1.0.0/yaccounts/analyzer.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1245 2023-07-07 21:28:10.000000 yaccounts-1.0.0/yaccounts/config.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     9410 2023-07-07 21:28:10.000000 yaccounts-1.0.0/yaccounts/operating_unit.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      290 2023-07-07 21:28:10.000000 yaccounts-1.0.0/yaccounts/utils.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1068 2023-07-07 21:28:10.000000 yaccounts-1.0.0/yaccounts/workbook.py
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2493 2023-07-07 21:28:10.000000 yaccounts-1.0.0/yaccounts/worksheet.py
-drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-07 21:31:50.834701 yaccounts-1.0.0/yaccounts.egg-info/
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-07 21:31:50.000000 yaccounts-1.0.0/yaccounts.egg-info/PKG-INFO
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      328 2023-07-07 21:31:50.000000 yaccounts-1.0.0/yaccounts.egg-info/SOURCES.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-07-07 21:31:50.000000 yaccounts-1.0.0/yaccounts.egg-info/dependency_links.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-07 21:31:50.000000 yaccounts-1.0.0/yaccounts.egg-info/requires.txt
--rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       10 2023-07-07 21:31:50.000000 yaccounts-1.0.0/yaccounts.egg-info/top_level.txt
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-08 21:48:11.477444 yaccounts-1.1.0/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-08 21:48:11.477444 yaccounts-1.1.0/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-08 21:48:11.477444 yaccounts-1.1.0/setup.cfg
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      385 2023-07-08 21:29:14.000000 yaccounts-1.1.0/setup.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-08 21:48:11.477444 yaccounts-1.1.0/test/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      655 2023-07-08 21:20:04.000000 yaccounts-1.1.0/test/test.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-08 21:48:11.477444 yaccounts-1.1.0/yaccounts/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-07 06:17:46.000000 yaccounts-1.1.0/yaccounts/__init__.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     3087 2023-07-08 21:17:41.000000 yaccounts-1.1.0/yaccounts/analyzer.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1741 2023-07-08 19:41:53.000000 yaccounts-1.1.0/yaccounts/config.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)    10112 2023-07-08 21:24:22.000000 yaccounts-1.1.0/yaccounts/operating_unit.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      290 2023-07-07 06:17:46.000000 yaccounts-1.1.0/yaccounts/utils.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     1097 2023-07-07 07:06:47.000000 yaccounts-1.1.0/yaccounts/workbook.py
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)     2975 2023-07-07 07:56:06.000000 yaccounts-1.1.0/yaccounts/worksheet.py
+drwxr-xr-x   0 jgoeders  (1000) jgoeders  (1000)        0 2023-07-08 21:48:11.477444 yaccounts-1.1.0/yaccounts.egg-info/
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      226 2023-07-08 21:48:11.000000 yaccounts-1.1.0/yaccounts.egg-info/PKG-INFO
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)      341 2023-07-08 21:48:11.000000 yaccounts-1.1.0/yaccounts.egg-info/SOURCES.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)        1 2023-07-08 21:48:11.000000 yaccounts-1.1.0/yaccounts.egg-info/dependency_links.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       38 2023-07-08 21:48:11.000000 yaccounts-1.1.0/yaccounts.egg-info/requires.txt
+-rw-r--r--   0 jgoeders  (1000) jgoeders  (1000)       10 2023-07-08 21:48:11.000000 yaccounts-1.1.0/yaccounts.egg-info/top_level.txt
```

### Comparing `yaccounts-1.0.0/yaccounts/operating_unit.py` & `yaccounts-1.1.0/yaccounts/operating_unit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 import calendar
 from collections import defaultdict
+import datetime
 import re
 import numpy as np
 
 import pandas as pd
 
 from .config import *
 
 
 class OperatingUnit:
-    def __init__(self, worksheet, operating_unit, name=None, previous_expenditures=0) -> None:
+    def __init__(
+        self,
+        worksheet,
+        operating_unit,
+        year,
+        name=None,
+        rolling_budget=None,
+        previous_expenditures=0,
+    ) -> None:
         self.worksheet = worksheet
         self.operating_unit = operating_unit
         self.name = name
         self.previous_expenditures = previous_expenditures
+        self.year = year
+
+        if rolling_budget is None:
+            self.rolling_budget = operating_unit.startswith("R")
+        else:
+            self.rolling_budget = rolling_budget
 
         # Create a new dataframe with months of the year as column headers
         self.df_gen = pd.DataFrame(
             columns=("Type", *[calendar.month_abbr[i] for i in range(1, 13)])
         )
 
         self.row_colors = {}
@@ -29,16 +44,31 @@
         self.df = None
 
     def set_options(self, hide_student_wages=False):
         self.hide_student_wages = hide_student_wages
 
     def run(self, df):
         self.df = df
+        if self.year:
+            # Filter df on 'Fiscal Year' column
+            self.df = self.df[self.df["Fiscal Year"] == self.year]
 
-        print("Running Operating Unit:", self.operating_unit)
+        print(
+            f"Running Operating Unit:{self.operating_unit} {('(' + str(self.year) + ')') if self.year else ''}",
+        )
+
+        if self.rolling_budget:
+            self.previous_expenditures_total = (
+                (
+                    self.previous_expenditures.total_expenses
+                    + self.previous_expenditures.previous_expenditures_total
+                )
+                if isinstance(self.previous_expenditures, OperatingUnit)
+                else self.previous_expenditures
+            )
 
         # Add student wage data
         self.add_row("Student Wages", CODES_STUDENT_WAGES, color=COLOR_STUDENT_WAGES)
         self.create_student_wages()
         self.add_row("Student Benefits", CODES_STUDENT_BENEFITS, color=COLOR_STUDENT_BENEFITS)
         self.add_row("Student Tuition", CODES_STUDENT_TUITION, color=COLOR_STUDENT_TUITION)
         self.add_row("Faculty Spr/Sum", CODES_FACULTY_SPRING_SUMMER, color=COLOR_FACULTY)
@@ -51,22 +81,21 @@
         )
         self.add_empty_row()
 
         self.add_row("Interest", CODES_INTEREST, actuals_coeff=-1)
         self.add_row(
             "Budget (New/Carryover)",
             [],
-            budgets_account_codes=CODES_BALANCE_FORWARD,
             budgets_coeff=1,
-            actuals_coeff=-1,
+            actuals_coeff=0,
         )
+        self.add_row("Transfers", CODES_INCOME, actuals_coeff=-1)
         self.row_total_income = self.add_row(
             "Total Income",
-            CODES_INTEREST,
-            budgets_account_codes=CODES_BALANCE_FORWARD,
+            CODES_INTEREST + CODES_INCOME,
             color=COLOR_TOTAL_INCOME,
             budgets_coeff=1,
             actuals_coeff=-1,
         )
 
         self.add_empty_row()
 
@@ -75,19 +104,20 @@
 
         # Calculate the sum for rows where 'Type' column is not empty
         columns_to_sum = self.df_gen.columns[1:]  # Get all columns starting from the second column
         self.df_gen.loc[self.df_gen["Type"] != "", "Sum"] = self.df_gen.loc[
             self.df_gen["Type"] != "", columns_to_sum
         ].sum(axis=1)
 
+        # Save total expenses, which is found in the self.row_total_expenses, "Sum" column
+        self.total_expenses = self.df_gen.iloc[self.row_total_expenses]["Sum"]
+
         self.add_balance_row()
         self.add_empty_row()
 
-        self.check_unhandled_codes()
-
         # self.df_gen["Sum"] = self.df_gen.apply(
         #     lambda row: row["Value"] if row["Type"] else None, axis=1
         # )
 
         # Add extra row to top of df_gen called "Students"
         # header_row = ["Students"] + [""] * (num_students)
         # df_gen = pd.concat((header_row, df_gen), ignore_index=True)
@@ -102,14 +132,16 @@
         # formattedWorksheet = FormattedWorksheet(sheet, workbook, df_gen, hasIndex=True)
 
         # sheet.insert_row(header_row, 0)
         # sheet.write_row(1, 1, header_row)
         title_name = self.operating_unit
         if self.name:
             title_name = f"{self.name} ({title_name})"
+        if self.year:
+            title_name = f"{title_name} - {self.year}"
         self.worksheet.write_to_sheet(self.df_gen, title_name, self.hidden_rows, self.row_colors)
 
         # sheet.set_row(student_total_row, cell_format=blue_fill_format)
 
     def add_empty_row(self):
         # Add an empty row of None values
         # self.df_gen = pd.concat((self.df_gen, pd.DataFrame([[""] * 13])), ignore_index=True)
@@ -125,16 +157,15 @@
         # )
 
         # self.df_gen = pd.concat((self.df_gen, pd.DataFrame([[""] * 13])), ignore_index=True)
 
     def add_row(
         self,
         row_name,
-        actuals_account_codes,
-        budgets_account_codes=[],
+        account_codes,
         budgets_coeff=0,
         actuals_coeff=1,
         color=None,
     ):
         """Sum the values in the 'Amount' column for each month in the given account codes.
         If actual=True, then only actual values will be summed.
         Otherwise budgeted (account income) values will be summed."""
@@ -150,15 +181,15 @@
                             & (self.df["JRNL Line Ledger"] == "BUDGETS")
                         ][COL_NAME_AMOUNT].sum()
                     )
                     + actuals_coeff
                     * (
                         self.df.loc[
                             (self.df["Accounting Period"] == month)
-                            & self.df["Account"].isin(actuals_account_codes)
+                            & self.df["Account"].isin(account_codes)
                             & (self.df["JRNL Line Ledger"] == "ACTUALS")
                         ][COL_NAME_AMOUNT].sum()
                     )
                 ]
                 for month in range(1, 13)
             },
         }
@@ -168,32 +199,38 @@
 
         if color:
             self.row_colors[len(self.df_gen)] = color
 
         return self.df_gen.tail(1).index[0]
 
     def add_balance_row(self):
-        self.df_gen.loc[len(self.df_gen)] = {
-            "Type": "Previous Expenditures",
-            calendar.month_abbr[1]: self.previous_expenditures,
-        }
+        if self.rolling_budget:
+            self.df_gen.loc[len(self.df_gen)] = {
+                "Type": "Previous Expenditures",
+                calendar.month_abbr[1]: self.previous_expenditures_total,
+            }
 
         self.df_gen.loc[len(self.df_gen)] = {"Type": "Balance (end of month)"}
 
         # # Iterate through columns and calcuate the balance, which is the total income minus the total expenses
         for month in range(1, 13):
-            self.df_gen.iloc[len(self.df_gen) - 1, month] = (
-                self.df_gen.iloc[self.row_total_income][month]
-                - self.df_gen.iloc[self.row_total_expenses][month]
-                + (
-                    self.df_gen.iloc[len(self.df_gen) - 1, month - 1]
-                    if month > 1
-                    else -self.df_gen.iloc[len(self.df_gen) - 2, month]
-                )
-            )
+            income = self.df_gen.iloc[self.row_total_income][month]
+            expenses = self.df_gen.iloc[self.row_total_expenses][month]
+
+            if month > 1:
+                prev_balance = self.df_gen.iloc[len(self.df_gen) - 1, month - 1]
+            elif self.rolling_budget:
+                prev_balance = -self.df_gen.iloc[len(self.df_gen) - 2, month]
+            else:
+                prev_balance = 0
+
+            balance = income - expenses + prev_balance
+            self.df_gen.iloc[len(self.df_gen) - 1, month] = balance
+            if month == 12:
+                self.balance = balance
 
         self.row_colors[len(self.df_gen)] = "yellow"
 
     def create_student_wages(self):
         # Filter to only student wages ('Account' column in STUDENT_WAGES)
         df_students = self.df[
             (self.df["Account"].isin(CODES_STUDENT_WAGES))
@@ -227,21 +264,7 @@
         self.df_gen = pd.concat((self.df_gen, pd.DataFrame(student_data)), ignore_index=True)
 
         # Add new row index to hidden rows
         if self.hide_student_wages:
             self.hidden_rows.extend(
                 range(len(self.df_gen) - len(student_data["Type"]) + 1, len(self.df_gen) + 1)
             )
-
-    def check_unhandled_codes(self):
-        # Get all account codes that were not handled
-        unhandled_codes = self.df[
-            (~self.df["Account"].isin(all_handled_codes()))
-            & (self.df["JRNL Line Ledger"] == "ACTUALS")
-        ]["Account"].unique()
-
-        # TODO: Add to spreadsheet instead of raising exception
-
-        if unhandled_codes.size > 0:
-            raise Exception(
-                f"Unhandled account codes: {','.join([str(c) for c in unhandled_codes])}.  See https://finserve.byu.edu/account-revenue-expense"
-            )
```

### Comparing `yaccounts-1.0.0/yaccounts/workbook.py` & `yaccounts-1.1.0/yaccounts/workbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from .utils import filter_df_on_operating_units
 from .worksheet import Worksheet
 
 
 class Workbook:
     def __init__(self, path) -> None:
+        self.analyzer = None
         self.path = path
 
         self.writer = pd.ExcelWriter(path, engine="xlsxwriter")
         self.workbook = self.writer.book
 
         self.worksheets = []
```

### Comparing `yaccounts-1.0.0/yaccounts/worksheet.py` & `yaccounts-1.1.0/yaccounts/worksheet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import matplotlib
 from .utils import ensure_tuple, filter_df_on_operating_units
 from .operating_unit import OperatingUnit
 
 
 class Worksheet:
     def __init__(self, workbook, sheet) -> None:
@@ -10,17 +11,30 @@
         self.sheet = sheet
         self.next_start_row = 0
 
         # self.name = name
         # if name is None:
         #     self.name = ",".join([ou.operating_unit for ou in self.operating_units])
 
-    def add_operating_unit(self, operating_unit, name=None, previous_expenditures=0):
-        operating_unit_obj = OperatingUnit(self, operating_unit, name, previous_expenditures)
-        self.operating_units.append(operating_unit_obj)
+    def add_operating_unit(self, operating_unit, name=None, year=None, previous_expenditures=0):
+        if year is None:
+            # Get all years for this operating unit from the dataframe
+            years = sorted(
+                self.workbook.analyzer.df[
+                    self.workbook.analyzer.df["Operating Unit"] == operating_unit
+                ]["Fiscal Year"].unique()
+            )
+        else:
+            years = ensure_tuple(year)
+
+        prev = previous_expenditures
+        for year in years:
+            prev = OperatingUnit(self, operating_unit, year, name=name, previous_expenditures=prev)
+            self.operating_units.append(prev)
+        # return operating_unit_obj
 
     def format_cell(self, row, col, format):
         self.sheet.conditional_format(row, col, row, col, {"type": "no_errors", "format": format})
 
     def format_row(self, row, format):
         self.sheet.conditional_format(row, 0, row, 13, {"type": "no_errors", "format": format})
         #     sheet.write_blank(row, i, sheet[row, i].value, color)
```

