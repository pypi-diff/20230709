# Comparing `tmp/sybil-scorer-0.2.0.tar.gz` & `tmp/sybil-scorer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sybil-scorer-0.2.0.tar", last modified: Thu Jun 29 10:43:45 2023, max compression
+gzip compressed data, was "sybil-scorer-0.2.1.tar", last modified: Sun Jul  9 20:37:18 2023, max compression
```

## Comparing `sybil-scorer-0.2.0.tar` & `sybil-scorer-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.883710 sybil-scorer-0.2.0/
--rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     9689 2023-06-29 10:43:45.884708 sybil-scorer-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     7755 2023-05-05 09:28:10.000000 sybil-scorer-0.2.0/README.md
--rw-rw-rw-   0        0        0     1142 2023-06-29 10:38:40.000000 sybil-scorer-0.2.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.821710 sybil-scorer-0.2.0/sbscorer/
-drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.836711 sybil-scorer-0.2.0/sbscorer/sbdata/
--rw-rw-rw-   0        0        0    22880 2023-05-08 09:36:36.000000 sybil-scorer-0.2.0/sbscorer/sbdata/FlipsideApi.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.2.0/sbscorer/sbdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.843711 sybil-scorer-0.2.0/sbscorer/sblegos/
--rw-rw-rw-   0        0        0    27938 2023-06-29 10:33:57.000000 sybil-scorer-0.2.0/sbscorer/sblegos/TransactionAnalyser.py
--rw-rw-rw-   0        0        0     9373 2023-06-09 19:15:54.000000 sybil-scorer-0.2.0/sbscorer/sblegos/TransactionAnalyserTest.py
--rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.2.0/sbscorer/sblegos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.847711 sybil-scorer-0.2.0/sbscorer/sbutils/
--rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.2.0/sbscorer/sbutils/LoadData.py
--rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.2.0/sbscorer/sbutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 10:43:45.881708 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/
--rw-rw-rw-   0        0        0     9689 2023-06-29 10:43:45.000000 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-06-29 10:43:45.000000 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 10:43:45.000000 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2023-06-29 10:43:45.000000 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-06-29 10:43:45.000000 sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      748 2023-06-29 10:43:45.894711 sybil-scorer-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.475887 sybil-scorer-0.2.1/
+-rw-rw-rw-   0        0        0     1084 2023-01-29 12:58:09.000000 sybil-scorer-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     9689 2023-07-09 20:37:18.475887 sybil-scorer-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7755 2023-05-05 09:28:10.000000 sybil-scorer-0.2.1/README.md
+-rw-rw-rw-   0        0        0     1142 2023-07-09 20:36:13.000000 sybil-scorer-0.2.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.393647 sybil-scorer-0.2.1/sbscorer/
+drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.415215 sybil-scorer-0.2.1/sbscorer/sbdata/
+-rw-rw-rw-   0        0        0    24311 2023-07-08 21:12:35.000000 sybil-scorer-0.2.1/sbscorer/sbdata/FlipsideApi.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.2.1/sbscorer/sbdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.436217 sybil-scorer-0.2.1/sbscorer/sblegos/
+-rw-rw-rw-   0        0        0    30118 2023-07-08 20:54:57.000000 sybil-scorer-0.2.1/sbscorer/sblegos/TransactionAnalyser.py
+-rw-rw-rw-   0        0        0     9373 2023-06-09 19:15:54.000000 sybil-scorer-0.2.1/sbscorer/sblegos/TransactionAnalyserTest.py
+-rw-rw-rw-   0        0        0        0 2023-01-21 08:46:58.000000 sybil-scorer-0.2.1/sbscorer/sblegos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.446552 sybil-scorer-0.2.1/sbscorer/sbutils/
+-rw-rw-rw-   0        0        0     5318 2023-01-30 19:57:35.000000 sybil-scorer-0.2.1/sbscorer/sbutils/LoadData.py
+-rw-rw-rw-   0        0        0        0 2023-01-17 19:51:41.000000 sybil-scorer-0.2.1/sbscorer/sbutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 20:37:18.473887 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/
+-rw-rw-rw-   0        0        0     9689 2023-07-09 20:37:18.000000 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-07-09 20:37:18.000000 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 20:37:18.000000 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2023-07-09 20:37:18.000000 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-09 20:37:18.000000 sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      748 2023-07-09 20:37:18.477886 sybil-scorer-0.2.1/setup.cfg
```

### Comparing `sybil-scorer-0.2.0/LICENSE` & `sybil-scorer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.2.0/PKG-INFO` & `sybil-scorer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil-scorer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A sybil scoring tool
 Home-page: https://github.com/poupou-web3/cluster-scorer
 Author: Poupou
 Author-email: Poupou <poupou-web3@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Poupou
```

### Comparing `sybil-scorer-0.2.0/README.md` & `sybil-scorer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.2.0/pyproject.toml` & `sybil-scorer-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0.0', "wheel"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "sybil-scorer"
-version = "0.2.0"
+version = "0.2.1"
 description = "A sybil scoring tool"
 readme = "README.md"
 authors = [{ name = "Poupou", email = "poupou-web3@protonmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `sybil-scorer-0.2.0/sbscorer/sbdata/FlipsideApi.py` & `sybil-scorer-0.2.1/sbscorer/sbdata/FlipsideApi.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,14 +143,44 @@
 
         """
         list_network = ["ethereum", "polygon",
                         "arbitrum", "avalanche", "gnosis", "optimism"]
         for network in list_network:
             self.extract_transactions_net(extract_dir, array_address, network)
 
+    def extract_data_flipside(self, array_address, sql_template):
+
+        q, r = divmod(len(array_address), self.MAX_ADDRESS)
+        if r != 0:
+            q += 1
+        list_df = []
+        for i in range(q):
+            start_index = i * self.MAX_ADDRESS
+            end_index = (i + 1) * self.MAX_ADDRESS
+            print(
+                f"Extracting for address: {start_index} - {end_index}")
+            array_address_slice = array_address[start_index:end_index]
+            str_address_slice = self.get_string_address(array_address_slice)
+            sql = sql_template % (str_address_slice, str_address_slice)
+            df = self.execute_query(sql=sql)
+
+            if df.shape[0] == 0 or df.shape == self.MAX_ROWS:  # retry with smaller query timeout or max rows
+                self.extract_data_flipside_rec(array_address, sql_template, start_index, end_index)
+            else:
+                list_df.append(df)
+        df = pd.concat(list_df)
+        return df
+
+    def extract_data_flipside_rec(self, array_address, sql_template, start_index, end_index):
+        end_first_slice = (start_index + end_index) // 2
+        print("Retrying with smaller query")
+        list_df = [self.extract_data_flipside(array_address[:end_first_slice], sql_template),
+                   self.extract_data_flipside(array_address[end_first_slice:], sql_template)]
+        return pd.concat(list_df)
+
     def extract_transactions_net(self, extract_dir, array_address, network):
         """
         Extract the transactions contained in array_address for the network and save them to csv in the extract_dir
         Each csv is named as eoa_tx.csv and is stored in a folder named after the network
 
         Parameters
         ----------
```

### Comparing `sybil-scorer-0.2.0/sbscorer/sblegos/TransactionAnalyser.py` & `sybil-scorer-0.2.1/sbscorer/sblegos/TransactionAnalyser.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,106 +13,145 @@
 
 class TransactionAnalyser(object):
     """
     This class is used to analyse transactions of an address.
     It has methods that allows to perform on chain analysis of an address.
     """
 
-    def __init__(self, df_transactions, df_address):
+    def __init__(self, df_transactions, array_address):
         """
         This class is used to analyse transactions of an address.
         It has methods that allows to perform on chain analysis of an address.
 
         It is initialized with a df_transactions containing all the transactions made by a list of addresses that
         should match the df_transactions
         Parameters
         ----------
         df_transactions : pd.DataFrame
             The dataframe containing all the transactions of the addresses
-        df_address : pd.DataFrame
-            The dataframe containing a 'address' column 
+        array_address : np.ndarray
+            The ndarray containing a list of addresses
         """
         assert isinstance(df_transactions, pd.DataFrame), "The df_transactions should be a pd.DataFrame"
-        assert isinstance(df_address, pd.DataFrame), "The df_address should be a pd.DataFrame"
-        assert 'address' in df_address.columns, "The df_address should contain a column 'address'"
+        assert isinstance(array_address, np.ndarray), "The df_address should be a numpy array"
 
         self.gb_EOA_sorted = None
         self.df_seed_wallet_naive = None
         self.df_seed_wallet = None
         self.details_first_incoming_transaction = None
         self.details_first_outgoing_transaction = None
-        self.df_transactions = df_transactions
+        self.array_address = np.intersect1d(array_address, df_transactions['EOA'].unique())
+        self.df_transactions = df_transactions[df_transactions['EOA'].isin(array_address)]
 
         # store the array of string transactions
         self.dict_add_interacted = None
         self.dict_add_string_tx = None
         self.dict_add_value_string_tx = None
 
         # set objects
         self.set_group_by_sorted_EOA()
         self.set_seed_wallet_naive()
         self.set_seed_wallet()
-        self.df_address = df_address
         self.set_details_first_incoming_transaction()
         self.set_details_first_outgoing_transaction()
 
     def has_same_seed_naive(self, address):
         """
         Return if the address has the same seed wallet as one of the seed wallet of the df_transactions
 
-        If the df_seed_wallet is not set, it will set it
-        Note df_transaction could contain transactions from multiple network but the seed wallet of the address is
+        Note
+        1. You should consider using count_same_seed_naive and applying a vectorized operation.
+        2. df_transaction could contain transactions from multiple network but the seed wallet of the address is
         filtered which prevent unexpected raise of the boolean.
 
         Parameters
         ----------
         address : str
             The address to check
 
         Returns
         -------
         has_same_seed : bool
             True if the address has the same seed wallet as one of the seed wallet of the df_transactions
         """
 
-        if self.df_seed_wallet_naive is None:
-            self.set_seed_wallet_naive()
+        return self.count_same_seed_naive(address) > 0
+
+    def count_same_seed_naive(self, address):
+        """
+        Return if the address has the same seed wallet as one of the seed wallet of the df_transactions
+
+        If the df_seed_wallet is not set, it will set it
+        Note df_transaction could contain transactions from multiple network but the seed wallet of the address is
+        filtered which prevent unexpected raise of the boolean.
+
+        Parameters
+        ----------
+        address : str
+            The address to check
+
+        Returns
+        -------
+        count_same_seed : int
+            The number of addresses having the same seed wallet
+        """
+
         df_same_seed = self.get_address_same_seed(self.df_seed_wallet_naive, address)
-        return df_same_seed.shape[0] > 0
+        return df_same_seed.shape[0]
 
     def has_same_seed(self, address):
         """
         Return if the address has the same seed wallet as one of the seed wallet of the df_transactions
         using a non-naive algorithm.
         For some address the first transaction is not the incoming funding transaction.
         It is possible to interact with a smart contract even before receiving any fund.
         This algorithm takes that into account.
 
-        If the df_seed_wallet is not set, it will set it
-        Note df_transaction could contain transactions from multiple network but the seed wallet of the address is
+        1. You should consider using count_same_seed_naive and applying a vectorized operation.
+        2. df_transaction could contain transactions from multiple network but the seed wallet of the address is
         filtered which prevent unexpected raise of the boolean.
 
         Parameters
         ----------
         address : str
             The address to check
 
         Returns
         -------
         has_same_seed : bool
             True if the address has the same seed wallet as one of the seed wallet of the df_transactions
         """
 
-        if self.df_seed_wallet is None:
-            self.set_seed_wallet()
-        if address in self.df_seed_wallet.to_address.values:
+        return self.count_same_seed(address)
+
+    def count_same_seed(self, address):
+        """
+        Return the number of address having the same seed wallet as one of the seed wallet of the df_transactions
+        using a non-naive algorithm.
+        For some address the first transaction is not the incoming funding transaction.
+        It is possible to interact with a smart contract even before receiving any fund.
+        This algorithm takes that into account. Note that it does not retrieve the true funder through the internal
+        transaction but the first incoming transaction.
+
+        Parameters
+        ----------
+        address : str
+            The address to check
+
+        Returns
+        -------
+        count_same_seed : int
+            The number of addresses having the same seed wallet as one of the seed wallet of the df_transactions
+        """
+
+        if address in self.df_seed_wallet.to_address.values:  # check that there normal incoming transactions
             df_same_seed = self.get_address_same_seed(self.df_seed_wallet, address)
-            return df_same_seed.shape[0] > 0
+            return df_same_seed.shape[0]
         else:
-            return False
+            return 0
 
     @staticmethod
     def get_address_same_seed(df, address):
         """
         Return a df of address that have the same seed wallet as the address given in parameter.
         Parameters
         ----------
@@ -409,18 +448,16 @@
         else:
             Exception("algo_type not supported")
 
         shape_target = self.get_address_transactions(address).shape[0]
         min_shape = max(1, shape_target / 4)
         max_shape = max(shape_target, shape_target * 3)
 
-        if self.df_address.columns != ['address']:
-            self.df_address.columns = ['address']
         list_lcs = []
-        for add in self.df_address['address']:
+        for add in self.array_address:
             if add != address:
                 shape_other = self.get_address_transactions(add).shape[0]
                 if min_shape < shape_other < max_shape:  # Heuristic to avoid comparing addresses with too different shapes
                     if algo_type == "address_only":
                         str_transactions_other = self.dict_add_string_tx.get(add)
                     else:
                         str_transactions_other = self.dict_add_value_string_tx.get(add)
@@ -431,15 +468,15 @@
             else:
                 list_lcs.append(0)
 
         if minimum_sim_tx == -1:
             mask = np.array(list_lcs) > max(3, min(10, shape_target / 4))
         else:
             mask = np.array(list_lcs) > minimum_sim_tx
-        df_similar_address = self.df_address.loc[mask, :].copy()
+        df_similar_address = pd.DataFrame(self.array_address[mask], columns=['address'])
         df_similar_address['lcs'] = np.array(list_lcs)[mask]
         len_tx = len(str_transactions_target) / 2  # Divide by 2 because we have from_address and to_address
         df_similar_address['score'] = df_similar_address.loc[:, 'lcs'].apply(
             lambda x: min(x / len_tx, 1))
         return df_similar_address.set_index('address')
 
     @staticmethod
@@ -581,19 +618,26 @@
     @staticmethod
     def get_max_score_lcs(lcs):
         if lcs.shape[0] == 0:
             return 0
         else:
             return lcs.reset_index()['score'].max()
 
+    def get_df_seeder_count(self):
+        return self.df_seed_wallet.groupby('from_address').count().sort_values(by='to_address',
+                                                                               ascending=False).reset_index().drop(
+            columns=['to_address']).rename(columns={'from_address': 'seeder', 'EOA': 'count_seed'})
+
     def get_df_features(self):
         df_features = self.gb_EOA_sorted['tx_hash'].count().reset_index().rename(columns={'tx_hash': 'count_tx'})
-        df_features['less_10_tx'] = df_features['count_tx'].apply(lambda x: x < 10)
-        df_features['same_seed'] = df_features['EOA'].apply(lambda x: self.has_same_seed(x))
-        df_features['same_seed_naive'] = df_features['EOA'].apply(lambda x: self.has_same_seed_naive(x))
+        df_features['less_10_tx'] = df_features['count_tx'] <= 10
+        df_features['count_same_seed'] = df_features['EOA'].apply(lambda x: self.count_same_seed(x))
+        df_features['count_same_seed_naive'] = df_features['EOA'].apply(lambda x: self.count_same_seed_naive(x))
+        df_features['same_seed'] = df_features['count_same_seed'] > 0
+        df_features['same_seed_naive'] = df_features['count_same_seed_naive'] > 0
         df_features['seed_suspicious'] = df_features.loc[:, 'same_seed'].ne(df_features.loc[:, 'same_seed_naive'])
         df_features['count_interact_other_ctbt'] = df_features['EOA'].apply(
             lambda x: self.count_interaction_with_other_contributor(x))
 
         details_first_incoming_transaction = self.details_first_incoming_transaction
         details_first_outgoing_transaction = self.details_first_outgoing_transaction
 
@@ -615,32 +659,37 @@
         merge = df_features.merge(details_first_incoming_transaction, on='EOA', how='left')
         merge = merge.merge(details_first_outgoing_transaction, on='EOA', how='left')
 
         return merge
 
     def get_df_features_vectorized(self):
         df_features = self.gb_EOA_sorted['tx_hash'].count().reset_index().rename(columns={'tx_hash': 'count_tx'})
-        df_features['less_10_tx'] = np.vectorize(lambda x: x < 10)(df_features['count_tx'])
-        df_features['same_seed'] = np.vectorize(self.has_same_seed)(df_features['EOA'])
-        df_features['same_seed_naive'] = np.vectorize(self.has_same_seed_naive)(df_features['EOA'])
+        df_features['less_10_tx'] = df_features['count_tx'] <= 10
+
+        df_features['count_same_seed'] = np.vectorize(self.count_same_seed)(df_features['EOA'])
+        df_features['count_same_seed_naive'] = np.vectorize(self.count_same_seed_naive)(df_features['EOA'])
+        df_features['same_seed'] = df_features['count_same_seed'] > 0
+        df_features['same_seed_naive'] = df_features['count_same_seed_naive'] > 0
         df_features['seed_suspicious'] = df_features.loc[:, 'same_seed'].ne(df_features.loc[:, 'same_seed_naive'])
+
         df_features['count_interact_other_ctbt'] = np.vectorize(self.count_interaction_with_other_contributor)(
             df_features['EOA'])
 
         details_first_incoming_transaction = self.details_first_incoming_transaction
         details_first_outgoing_transaction = self.details_first_outgoing_transaction
 
         df_features['lcs'] = 0
         df_features['cluster_size_lcs'] = 0
         df_features['mean_score_lcs'] = 0
         df_features['max_score_lcs'] = 0
 
         df_bool_less_10_tx = df_features['less_10_tx']
         if df_bool_less_10_tx.sum() > 0:
-            r = np.vectorize(self.transaction_similitude_pylcs)(df_features.loc[df_bool_less_10_tx, 'EOA'])
+            r = df_features.loc[df_bool_less_10_tx, 'EOA'].apply(
+                lambda x: self.transaction_similitude_pylcs(x, minimum_sim_tx=3))
             df_features.loc[df_bool_less_10_tx, 'cluster_size_lcs'] = np.vectorize(len)(r)
             df_features.loc[df_bool_less_10_tx, 'mean_score_lcs'] = np.vectorize(self.get_mean_score_lcs)(r)
             df_features.loc[df_bool_less_10_tx, 'max_score_lcs'] = np.vectorize(self.get_max_score_lcs)(r)
 
         df_features['has_lcs'] = df_features['cluster_size_lcs'] > 0
 
         merge = df_features.merge(details_first_incoming_transaction, on='EOA', how='left')
```

### Comparing `sybil-scorer-0.2.0/sbscorer/sblegos/TransactionAnalyserTest.py` & `sybil-scorer-0.2.1/sbscorer/sblegos/TransactionAnalyserTest.py`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.2.0/sbscorer/sbutils/LoadData.py` & `sybil-scorer-0.2.1/sbscorer/sbutils/LoadData.py`

 * *Files identical despite different names*

### Comparing `sybil-scorer-0.2.0/sbscorer/sybil_scorer.egg-info/PKG-INFO` & `sybil-scorer-0.2.1/sbscorer/sybil_scorer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sybil-scorer
-Version: 0.2.0
+Version: 0.2.1
 Summary: A sybil scoring tool
 Home-page: https://github.com/poupou-web3/cluster-scorer
 Author: Poupou
 Author-email: Poupou <poupou-web3@protonmail.com>
 License: MIT License
         
         Copyright (c) 2023 Poupou
```

### Comparing `sybil-scorer-0.2.0/setup.cfg` & `sybil-scorer-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 7962 696c 2d73 636f 7265 720d   = sybil-scorer.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e32 2e30  .version = 0.2.0
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e32 2e31  .version = 0.2.1
 00000030: 0d0a 6175 7468 6f72 203d 2050 6f75 706f  ..author = Poupo
 00000040: 750d 0a61 7574 686f 725f 656d 6169 6c20  u..author_email 
 00000050: 3d20 706f 7570 6f75 2d77 6562 3340 7072  = poupou-web3@pr
 00000060: 6f74 6f6e 6d61 696c 2e63 6f6d 0d0a 6465  otonmail.com..de
 00000070: 7363 7269 7074 696f 6e20 3d20 4120 7379  scription = A sy
 00000080: 6269 6c20 7363 6f72 696e 6720 746f 6f6c  bil scoring tool
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

