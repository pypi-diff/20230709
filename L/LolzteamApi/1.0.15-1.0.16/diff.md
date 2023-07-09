# Comparing `tmp/LolzteamApi-1.0.15.tar.gz` & `tmp/LolzteamApi-1.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LolzteamApi-1.0.15.tar", last modified: Sat Jul  8 17:31:43 2023, max compression
+gzip compressed data, was "LolzteamApi-1.0.16.tar", last modified: Sun Jul  9 10:42:00 2023, max compression
```

## Comparing `LolzteamApi-1.0.15.tar` & `LolzteamApi-1.0.16.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 17:31:43.994810 LolzteamApi-1.0.15/
--rw-rw-rw-   0        0        0     1089 2023-07-07 23:34:42.000000 LolzteamApi-1.0.15/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-08 17:31:43.961329 LolzteamApi-1.0.15/LolzteamApi/
--rw-rw-rw-   0        0        0   162555 2023-07-08 16:47:32.000000 LolzteamApi-1.0.15/LolzteamApi/LolzteamApi.py
--rw-rw-rw-   0        0        0      111 2023-07-08 01:36:03.000000 LolzteamApi-1.0.15/LolzteamApi/__init__.py
--rw-rw-rw-   0        0        0     1121 2023-07-08 01:42:28.000000 LolzteamApi-1.0.15/LolzteamApi/check_updates.py
-drwxrwxrwx   0        0        0        0 2023-07-08 17:31:43.990794 LolzteamApi-1.0.15/LolzteamApi.egg-info/
--rw-rw-rw-   0        0        0     2260 2023-07-08 17:31:43.000000 LolzteamApi-1.0.15/LolzteamApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-07-08 17:31:43.000000 LolzteamApi-1.0.15/LolzteamApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 17:31:43.000000 LolzteamApi-1.0.15/LolzteamApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-08 17:31:43.000000 LolzteamApi-1.0.15/LolzteamApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-08 17:31:43.000000 LolzteamApi-1.0.15/LolzteamApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2260 2023-07-08 17:31:43.990794 LolzteamApi-1.0.15/PKG-INFO
--rw-rw-rw-   0        0        0     1859 2023-07-07 23:34:42.000000 LolzteamApi-1.0.15/README.md
--rw-rw-rw-   0        0        0       42 2023-07-08 17:31:43.994810 LolzteamApi-1.0.15/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-07-08 16:48:36.000000 LolzteamApi-1.0.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-09 10:42:00.142315 LolzteamApi-1.0.16/
+-rw-rw-rw-   0        0        0     1089 2023-07-08 18:11:39.000000 LolzteamApi-1.0.16/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-09 10:42:00.114534 LolzteamApi-1.0.16/LolzteamApi/
+-rw-rw-rw-   0        0        0   164017 2023-07-09 10:35:34.000000 LolzteamApi-1.0.16/LolzteamApi/LolzteamApi.py
+-rw-rw-rw-   0        0        0      111 2023-07-08 01:36:03.000000 LolzteamApi-1.0.16/LolzteamApi/__init__.py
+-rw-rw-rw-   0        0        0     1121 2023-07-08 01:42:28.000000 LolzteamApi-1.0.16/LolzteamApi/check_updates.py
+drwxrwxrwx   0        0        0        0 2023-07-09 10:42:00.138999 LolzteamApi-1.0.16/LolzteamApi.egg-info/
+-rw-rw-rw-   0        0        0     2260 2023-07-09 10:42:00.000000 LolzteamApi-1.0.16/LolzteamApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-07-09 10:42:00.000000 LolzteamApi-1.0.16/LolzteamApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 10:42:00.000000 LolzteamApi-1.0.16/LolzteamApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-09 10:42:00.000000 LolzteamApi-1.0.16/LolzteamApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-09 10:42:00.000000 LolzteamApi-1.0.16/LolzteamApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2260 2023-07-09 10:42:00.138999 LolzteamApi-1.0.16/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2023-07-08 18:11:39.000000 LolzteamApi-1.0.16/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-09 10:42:00.142829 LolzteamApi-1.0.16/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-07-09 09:09:11.000000 LolzteamApi-1.0.16/setup.py
```

### Comparing `LolzteamApi-1.0.15/LICENSE` & `LolzteamApi-1.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.15/LolzteamApi/LolzteamApi.py` & `LolzteamApi-1.0.16/LolzteamApi/LolzteamApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 import requests
 import time
 import json
 
 
 class LolzteamApi:
-    def __init__(self, token: str, bypass_429: bool = True):
+    def __init__(self, token: str, bypass_429: bool = True, language: str = "RU"):
         """
         :param token: Your token. You can get in there -> https://zelenka.guru/account/api
         :param bypass_429: Bypass status code 429 by sleep
+        :param language: Language for your api responses. Pass "en" if you want to get responses in english or pass "ru" if you want to get responses in russian.
         """
 
         self.__token = token
+        self.__headers = {'Authorization': f"bearer {self.__token}"}
+
         self.__bypass_429 = bypass_429
         self.__auto_delay_time = time.time() - 3
-        self.__headers = {'Authorization': f"bearer {self.__token}"}
+        self.__locale = language
+        self.__token_user_id = self.__set_user_id()
 
-        self.market = self.__Market(self)
+        self.market = self.__Market(self, self.__token_user_id)
         self.forum = self.__Forum(self)
 
-    def send_request(self, method: str, url: str, params=None, data=None, files=None):
+    def send_request(self, method: str, url: str, params: dict = None, data=None, files=None):
         method = method.upper()
         LolzteamApi.__auto_delay(self)
+
+        if params is None:
+            params = {}
+        params["locale"] = self.__locale
+
         match method:
             case "GET":
                 response = requests.get(url=url, params=params, data=data, files=files, headers=self.__headers)
             case "POST":
                 response = requests.post(url=url, params=params, data=data, files=files, headers=self.__headers)
             case "PUT":
                 response = requests.put(url=url, params=params, data=data, files=files, headers=self.__headers)
@@ -34,27 +43,36 @@
                 response = {"error": "Создатель либы где-то проебался. Отпиши @AS7RID в тг, он починит"}
         self.__auto_delay_time = time.time()
         try:
             return response.json()
         except requests.exceptions.JSONDecodeError:
             return response.text
 
+    def __set_user_id(self):
+        url = "https://api.lzt.market/me"
+        response = LolzteamApi.send_request(self=self, method="GET", url=url)
+        try:
+            return response["user"]["user_id"]
+        except KeyError:
+            return None
+
     def __auto_delay(self):
         """
         Sleep for time difference between the last call and current call if it's less than 3 seconds
         """
         if self.__bypass_429:
             current_time = time.time()
             time_diff = current_time - self.__auto_delay_time
             if time_diff < 3.0:  # if difference between current and last call > 3 seconds we will sleep the rest of the time
 
                 time.sleep(3.003 - time_diff)
 
     def change_token(self, new_token: str):
         self.__token = new_token
+        self.__token_user_id = self.__set_user_id()
         self.__headers = {'Authorization': f"bearer {self.__token}"}
 
     class __Forum:
         def __init__(self, api_self):
             self.__api = api_self  # Passing main self to sub all classes
 
             #  Sections definitions
@@ -2140,15 +2158,14 @@
                     "client_id": client_id,
                     "client_secret": client_secret,
                     "twitter_uri": twitter_url,
                     "twitter_auth": twitter_auth
                 }
                 return LolzteamApi.send_request(self=self.__api, method="POST", url=url, params=params)
 
-
             def google(self, client_id: int, client_secret: str, google_token: str):
                 """
                 POST https://api.zelenka.guru/oauth/token/google
 
                 Request API access token using Google access token.
 
                 Required scopes: None
@@ -2249,20 +2266,21 @@
             :return: json server response
             """
 
             url = f"https://api.zelenka.guru/batch"
             return LolzteamApi.send_request(self=self.__api, method="POST", url=url, data=json.dumps(request_body))
 
     class __Market:
-        def __init__(self, api_self):
+        def __init__(self, api_self, token_user_id):
             self.__api = api_self
-            self.profile = self.__Profile(self.__api)
-            self.payments = self.__Payments(self.__api)
-            self.accounts = self.__Accounts(self.__api)
-            self.list = self.__List(self.__api)
+            self.__token_user_id = token_user_id
+
+            self.profile = self.__Profile(self.__api, self.__token_user_id)
+            self.payments = self.__Payments(self.__api, self.__token_user_id)
+            self.list = self.__List(self.__api, self.__token_user_id)
             self.publishing = self.__Publishing(self.__api)
             self.purchasing = self.__Purchasing(self.__api)
             self.managing = self.__Managing(self.__api)
             self.proxy = self.__Proxy(self.__api)
 
         def batch(self, request_body: list[dict]):
             """
@@ -2285,16 +2303,17 @@
             :return: json server response
             """
 
             url = f"https://api.lzt.market/batch"
             return LolzteamApi.send_request(self=self.__api, method="POST", url=url, data=json.dumps(request_body))
 
         class __Profile:
-            def __init__(self, api_self):
+            def __init__(self, api_self, token_user_id):
                 self.__api = api_self
+                self.__token_user_id = token_user_id
 
             def get(self):
                 """
                 GET https://api.lzt.market/me
 
                 Displays info about your profile.
 
@@ -2332,15 +2351,16 @@
                     "max_discount_percent": max_discount_percent,
                     "allow_accept_accounts": allow_accept_accounts,
                     "hide_favourites": hide_favourites,
                     "vk_ua": vk_ua
                 }
                 return LolzteamApi.send_request(self=self.__api, method="PUT", url=url, params=params)
 
-            def owned(self, user_id: int, category_id: int = None, pmin: int = None, pmax: int = None,
+            # Copy of __List.owned
+            def owned(self, user_id: int = None, category_id: int = None, pmin: int = None, pmax: int = None,
                       title: str = None):
                 """
                 GET https://api.lzt.market/user/user_id/items
 
                 Displays a list of owned accounts.
 
                 Category id-names list:
@@ -2400,25 +2420,28 @@
                 :param pmin: Minimal price of account (Inclusive)
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
 
                 :return: json server response
 
                 """
+                if user_id is None:  # Tweak
+                    user_id = self.__token_user_id
                 url = f"https://api.lzt.market/user/{user_id}/items"
                 params = {
                     "user_id": user_id,
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
                     "title": title
                 }
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
-            def purchased(self, user_id: int, category_id: int = None, pmin: int = None, pmax: int = None,
+            # Copy of __List.purchased
+            def purchased(self, user_id: int = None, category_id: int = None, pmin: int = None, pmax: int = None,
                           title: str = None):
                 """
                 GET https://api.lzt.market/user/user_id/orders
 
                 Displays a list of purchased accounts.
 
                 Category id-names list:
@@ -2478,23 +2501,26 @@
                 :param pmin: Minimal price of account (Inclusive)
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
 
                 :return: json server response
 
                 """
-                url = f"https://api.lzt.market/user/{user_id}/orders"
                 params = {
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
                     "title": title
                 }
+                if user_id is None:  # Tweak
+                    user_id = self.__token_user_id
+                url = f"https://api.lzt.market/user/{user_id}/orders"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
+            # Copy of __List.favorite
             def favorite(self, page: int = None):
                 """
                 GET https://api.lzt.market/fave
 
                 Displays a list of favourites accounts.
 
                 Required scopes: market
@@ -2506,14 +2532,15 @@
                 """
                 url = "https://api.lzt.market/fave"
                 params = {
                     "page": page
                 }
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
+            # Copy of __List.viewed
             def viewed(self, page: int = None):
                 """
                 GET https://api.lzt.market/viewed
 
                 Displays a list of viewed accounts.
 
                 Required scopes: market
@@ -2526,16 +2553,18 @@
                 url = "https://api.lzt.market/viewed"
                 params = {
                     "page": page
                 }
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
         class __List:
-            def __init__(self, api_self):
+            def __init__(self, api_self, token_user_id):
                 self.__api = api_self
+                self.__token_user_id = token_user_id
+
                 self.categories = self.__Category_Market(self.__api)
 
             class __Category_Market:  # лежит в List
                 def __init__(self, api_self):
                     self.__api = api_self
 
                 def categories(self, top_queries: bool = None):
@@ -2785,15 +2814,15 @@
                 """
                 url = "https://api.lzt.market/"
                 params = {
                     "page": page
                 }
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
-            def owned(self, user_id: int, category_id: int = None, pmin: int = None, pmax: int = None,
+            def owned(self, user_id: int = None, category_id: int = None, pmin: int = None, pmax: int = None,
                       title: str = None):
                 """
                 GET https://api.lzt.market/user/user_id/items
 
                 Displays a list of owned accounts.
 
                 Category id-names list:
@@ -2853,25 +2882,27 @@
                 :param pmin: Minimal price of account (Inclusive)
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
 
                 :return: json server response
 
                 """
-                url = f"https://api.lzt.market/user/{user_id}/items"
                 params = {
                     "user_id": user_id,
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
                     "title": title
                 }
+                if user_id is None:  # Tweak
+                    user_id = self.__token_user_id
+                url = f"https://api.lzt.market/user/{user_id}/items"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
-            def purchased(self, user_id: int, category_id: int = None, pmin: int = None, pmax: int = None,
+            def purchased(self, user_id: int = None, category_id: int = None, pmin: int = None, pmax: int = None,
                           title: str = None):
                 """
                 GET https://api.lzt.market/user/user_id/orders
 
                 Displays a list of purchased accounts.
 
                 Category id-names list:
@@ -2931,21 +2962,23 @@
                 :param pmin: Minimal price of account (Inclusive)
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
 
                 :return: json server response
 
                 """
-                url = f"https://api.lzt.market/user/{user_id}/orders"
                 params = {
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
                     "title": title
                 }
+                if user_id is None:  # Tweak
+                    user_id = self.__token_user_id
+                url = f"https://api.lzt.market/user/{user_id}/orders"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             def favorite(self, page: int = None):
                 """
                 GET https://api.lzt.market/fave
 
                 Displays a list of favourites accounts.
@@ -3001,25 +3034,18 @@
                 if steam_preview:
                     url = f"https://api.lzt.market/{item_id}/steam-preview"
                 params = {
                     "type": preview_type
                 }
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
-        class __Accounts:
-            def __init__(self, api_self):
-                self.__api = api_self
-                self.list = ''
-                self.managing = ''
-                self.purchasing = ''
-                self.publishing = ''
-
         class __Payments:
-            def __init__(self, api_self):
+            def __init__(self, api_self, token_user_id):
                 self.__api = api_self
+                self.__token_user_id = token_user_id
 
             def history(self, user_id: int, operation_type: str = None, pmin: int = None, pmax: int = None,
                         page: int = None,
                         operation_id_lt: int = None, receiver: str = None, sender: str = None, start_date: str = None,
                         end_date: str = None, wallet: str = None, comment: str = None, is_hold: bool = None,
                         show_payments_stats: bool = None):
                 """
@@ -3043,15 +3069,14 @@
                 :param comment: Comment for money transfers
                 :param is_hold: Display hold operations
                 :param show_payments_stats: Display payment stats for selected period (outgoing value, incoming value)
 
                 :return: json server response
 
                 """
-                url = f"https://api.lzt.market/user/{user_id}/payments"
                 if True:  # Костыль, пока не пофиксят недочет #43
                     if is_hold:
                         is_hold = 1
                     else:
                         is_hold = 0
                     if show_payments_stats:
                         show_payments_stats = 1
@@ -3069,14 +3094,17 @@
                     "start_date": start_date,
                     "end_date": end_date,
                     "wallet": wallet,
                     "comment": comment,
                     "is_hold": is_hold,
                     "show_payments_stats": show_payments_stats
                 }
+                if user_id is None:  # Tweak
+                    user_id = self.__token_user_id
+                url = f"https://api.lzt.market/user/{user_id}/payments"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             def transfer(self, amount: int, secret_answer: str, currency: str = "rub", user_id: int = None,
                          username: str = None, comment: str = None, transfer_hold: bool = None,
                          hold_length_option: str = None,
                          hold_length_value: int = None):
                 """
@@ -3771,14 +3799,15 @@
                     "login_password": login_password
                 }
                 for key, value in extra:
                     es = f"extra[{key}]"
                     params[es] = value
                 return LolzteamApi.send_request(self=self.__api, method="POST", url=url, params=params)
 
+            # Copy of __Managing.edit
             def edit(self, item_id: int, price: int = None, currency: str = None, item_origin: str = None,
                      title: str = None, title_en: str = None, description: str = None, information: str = None,
                      email_login_data: str = None, email_type: str = None, allow_ask_discount: bool = None,
                      proxy_id: int = None):
                 """
                 POST https://api.lzt.market/item_id/edit
 
@@ -3812,14 +3841,15 @@
                 :param email_login_data: Required if a category is one of list of Required email login data categories. Email login data (login:pass format).
                 :param email_type: Email type. Allowed values: native, autoreg.
                 :param allow_ask_discount: Allow users to ask discount for this account.
                 :param proxy_id: Using proxy id for account checking.
 
                 :return: json server response
                 """
+
                 url = f"https://api.lzt.market/{item_id}/edit"
                 params = {
                     "price": price,
                     "currency": currency,
                     "item_origin": item_origin,
                     "title": title,
                     "title_en": title_en,
```

### Comparing `LolzteamApi-1.0.15/LolzteamApi/check_updates.py` & `LolzteamApi-1.0.16/LolzteamApi/check_updates.py`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.15/LolzteamApi.egg-info/PKG-INFO` & `LolzteamApi-1.0.16/LolzteamApi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.15
+Version: 1.0.16
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.15 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.16 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.15/PKG-INFO` & `LolzteamApi-1.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.15
+Version: 1.0.16
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.15 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.16 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
```

### Comparing `LolzteamApi-1.0.15/README.md` & `LolzteamApi-1.0.16/README.md`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.15/setup.py` & `LolzteamApi-1.0.16/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = ["requests", "beautifulsoup4"]
 
 setuptools.setup(
     name="LolzteamApi",
-    version="1.0.15",
+    version="1.0.16",
     author="AS7RID",
     author_email="as7ridwork@gmail.com",
     description="A library that contains all the methods of the Lolzteam API (Market/Forum)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AS7RIDENIED/Lolzteam_Python_Api",
     packages=setuptools.find_packages(),
```

