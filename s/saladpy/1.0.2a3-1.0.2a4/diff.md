# Comparing `tmp/saladpy-1.0.2a3.tar.gz` & `tmp/saladpy-1.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saladpy-1.0.2a3.tar", last modified: Sun Jul  9 13:15:52 2023, max compression
+gzip compressed data, was "saladpy-1.0.2a4.tar", last modified: Sun Jul  9 14:38:28 2023, max compression
```

## Comparing `saladpy-1.0.2a3.tar` & `saladpy-1.0.2a4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:15:52.253825 saladpy-1.0.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 13:15:52.253825 saladpy-1.0.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:15:52.249825 saladpy-1.0.2a3/saladpy/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:15:52.249825 saladpy-1.0.2a3/saladpy/methods/
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/methods/User.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:15:52.253825 saladpy-1.0.2a3/saladpy/methods/types/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/methods/types/BaseClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/methods/types/UserTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/saladpy/methods/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 13:15:52.249825 saladpy-1.0.2a3/saladpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 13:15:52.000000 saladpy-1.0.2a3/saladpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-09 13:15:52.000000 saladpy-1.0.2a3/saladpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 13:15:52.000000 saladpy-1.0.2a3/saladpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 13:15:52.000000 saladpy-1.0.2a3/saladpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 13:15:52.000000 saladpy-1.0.2a3/saladpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 13:15:52.253825 saladpy-1.0.2a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-09 13:15:40.000000 saladpy-1.0.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/saladpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/saladpy/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/methods/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/saladpy/methods/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/methods/types/BaseClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/methods/types/UserTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/saladpy/methods/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/saladpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-09 14:38:28.000000 saladpy-1.0.2a4/saladpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-09 14:38:28.000000 saladpy-1.0.2a4/saladpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 14:38:28.000000 saladpy-1.0.2a4/saladpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 14:38:28.000000 saladpy-1.0.2a4/saladpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 14:38:28.000000 saladpy-1.0.2a4/saladpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 14:38:28.305175 saladpy-1.0.2a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-09 14:38:18.000000 saladpy-1.0.2a4/setup.py
```

### Comparing `saladpy-1.0.2a3/LICENSE` & `saladpy-1.0.2a4/LICENSE`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a3/PKG-INFO` & `saladpy-1.0.2a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saladpy
-Version: 1.0.2a3
+Version: 1.0.2a4
 Summary: A Python wrapper for the Salad Web API
 Home-page: https://github.com/Coddo-Python/SaladPy
 Author: Coddo-Python
 Author-email: Coddo <coddobusiness@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015-present Coddo-Python
```

### Comparing `saladpy-1.0.2a3/README.md` & `saladpy-1.0.2a4/README.md`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a3/pyproject.toml` & `saladpy-1.0.2a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saladpy"
-version = "1.0.2-a.3"
+version = "1.0.2-a.4"
 description = "A Python wrapper for the Salad Web API"
 readme = "README.md"
 authors = [{ name = "Coddo", email = "coddobusiness@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `saladpy-1.0.2a3/saladpy/client.py` & `saladpy-1.0.2a4/saladpy/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -114,17 +114,19 @@
                     text = await r.json()
                     raise SaladPyException(
                         f"Error {r.status} during OTP verification! {text}"
                     )
                 else:
                     return True
 
-    async def _req(self, api_url : str, method: str, endpoint: str, params: Optional[dict] = None):
+    async def _req(self, api_url : str, method: str, endpoint: str, params: Optional[dict] = None, token: Optional[str] = None, *args, **kwargs):
         headers = {}
-        if self.token:
+        if token:
+            headers["Authorization"] = f"Bearer {token}"
+        elif self.token:
             headers["Authorization"] = f"Bearer {self.token}"
         async with self.http.request(
             method, f"{api_url}{endpoint}", params=params, headers=headers
         ) as r:
             text = await r.text()
             try:
                 assert r.status == 200
@@ -149,18 +151,18 @@
             print(r.status)
             text = await r.text()
             print(text)
             if r.status == 200:
                 self.http.cookie_jar.update_cookies(r.cookies)
                 self.http.cookie_jar.save(self.cachePath)
 
-    async def _get(self, api_url: str, endpoint: str, params: Optional[dict] = None):
-        resp = await self._req(api_url, "GET", endpoint, params)
+    async def _get(self, api_url: str, endpoint: str, params: Optional[dict] = None, **kwargs):
+        resp = await self._req(api_url, "GET", endpoint, params, **kwargs)
         if resp == 404:
             return resp
         return json.loads(resp)
 
-    async def _post(self, api_url: str, endpoint: str, params: Optional[dict] = None):
-        resp = await self._req(api_url, "POST", endpoint, params)
+    async def _post(self, api_url: str, endpoint: str, params: Optional[dict] = None, **kwargs):
+        resp = await self._req(api_url, "POST", endpoint, params, **kwargs)
         if resp == 404:
             return resp
         return json.loads(resp)
```

### Comparing `saladpy-1.0.2a3/saladpy/methods/User.py` & `saladpy-1.0.2a4/saladpy/methods/User.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,123 +3,123 @@
 
 from .types import *
 
 
 class UserMethods(BaseClient):
     """A class containing all the User API endpoints"""
 
-    async def profile(self) -> ProfileResponse:
+    async def profile(self, **kwargs) -> ProfileResponse:
         """Gets a User's Profile
 
         Returns:
             ProfileResponse: Info about the User's profile
         """
-        return ProfileResponse(**await self._get(self.V1_API_URL, "profile"))
+        return ProfileResponse(**await self._get(self.V1_API_URL, "profile", **kwargs))
 
-    async def balance(self) -> BalanceResponse:
+    async def balance(self, **kwargs) -> BalanceResponse:
         """Gets a User's Balance
 
         Returns:
             BalanceResponse: The user's currentBalance and lifetimeBalance
         """
-        return BalanceResponse(**await self._get(self.V1_API_URL, "profile/balance"))
+        return BalanceResponse(**await self._get(self.V1_API_URL, "profile/balance", **kwargs))
 
-    async def xp(self) -> int:
+    async def xp(self, **kwargs) -> int:
         """Gets a User's xp
 
         Returns:
             int: Lifetime Xp
         """
-        return (await self._get(self.V1_API_URL, "profile/xp"))["lifetimeXp"]
+        return (await self._get(self.V1_API_URL, "profile/xp", **kwargs))["lifetimeXp"]
 
-    async def referral_code(self) -> str:
+    async def referral_code(self, **kwargs) -> str:
         """Gets a User's referral code
 
         Returns:
             str: User's referral code
         """
-        return (await self._get(self.V1_API_URL, "profile/referral-code"))["code"]
+        return (await self._get(self.V1_API_URL, "profile/referral-code", **kwargs))["code"]
 
-    async def referrals(self) -> List[ReferralsResponse]:
+    async def referrals(self, **kwargs) -> List[ReferralsResponse]:
         """Gets a list of users that have used a User's code
 
         Returns:
             List[ReferralsResponse]: List of users that have used your referral code
         """
-        result = await self._get(self.V1_API_URL, "profile/referrals")
+        result = await self._get(self.V1_API_URL, "profile/referrals", **kwargs)
         response = []
         for resp in result:
             ref_def = ReferralDefinition(**resp["referralDefinition"])
             resp.pop("referralDefinition", None)
             response.append(ReferralsResponse(referralDefinition=ref_def, **resp))
         return response
 
-    async def redemptions(self) -> List[RedemptionsResponse]:
+    async def redemptions(self, **kwargs) -> List[RedemptionsResponse]:
         """Gets a User's Redemptions
 
         Returns:
             List[RedemptionsResponse]: A list of a user's redemptions, will be empty if there are none
         """
-        result = await self._get(self.V1_API_URL, "reward-vault")
+        result = await self._get(self.V1_API_URL, "reward-vault", **kwargs)
         response = []
         for resp in result:
             if "code" not in resp:
                 resp["code"] = ""
             response.append(RedemptionsResponse(**resp))
         return response
 
-    async def one_day_earning_history(self) -> Dict[str, float]:
+    async def one_day_earning_history(self, **kwargs) -> Dict[str, float]:
         """Gets a User's 1 day earning history
 
         Returns:
             Dict[str, float]: 1 Day earning history, where the key is a time and the value is a float, empty if no earning history
         """
-        return await self._get(self.V2_API_URL, "reports/1-day-earning-history")  # type: ignore
+        return await self._get(self.V2_API_URL, "reports/1-day-earning-history", **kwargs)  # type: ignore
 
-    async def seven_day_earning_history(self) -> Dict[str, float]:
+    async def seven_day_earning_history(self, **kwargs) -> Dict[str, float]:
         """Gets a User's 7 day earning history
 
         Returns:
             Dict[str, float]: 7 Day earning history, where the key is a time and the value is a float, empty if no earning history
         """
-        return await self._get(self.V2_API_URL, "reports/7-day-earning-history")  # type: ignore
+        return await self._get(self.V2_API_URL, "reports/7-day-earning-history", **kwargs)  # type: ignore
 
-    async def thirty_day_earning_history(self) -> Dict[str, float]:
+    async def thirty_day_earning_history(self, **kwargs) -> Dict[str, float]:
         """Gets a User's 30 day earning history
 
         Returns:
             Dict[str, float]: 30 Day earning history, where the key is a time and the value is a float, empty if no earning history
         """
-        return await self._get(self.V2_API_URL, "reports/30-day-earning-history")  # type: ignore
+        return await self._get(self.V2_API_URL, "reports/30-day-earning-history", **kwargs)  # type: ignore
 
-    async def avatars(self) -> List[AvatarsResponse]:
+    async def avatars(self, **kwargs) -> List[AvatarsResponse]:
         """Gets a User's unlocked avatars
 
         Returns:
             List[AvatarsResponse]: List of unlocked avatars
         """
-        return [AvatarsResponse(**resp) for resp in await self._get(self.V2_API_URL, "avatars")]  # type: ignore
+        return [AvatarsResponse(**resp) for resp in await self._get(self.V2_API_URL, "avatars", **kwargs)]  # type: ignore
 
-    async def selected_avatar(self) -> Union[SelectedAvatarResponse, None]:
+    async def selected_avatar(self, **kwargs) -> Union[SelectedAvatarResponse, None]:
         """Gets a User's currently selected avatar
 
         Returns:
             SelectedAvatarResponse: Currently selected avatar
             None: If using the default avatar
         """
-        resp = await self._get(self.V2_API_URL, "avatars/selected")  # type: ignore
+        resp = await self._get(self.V2_API_URL, "avatars/selected", **kwargs)  # type: ignore
         if resp == 404:
             return None
         return SelectedAvatarResponse(**resp)
 
-    async def bonuses(self) -> Union[list, None]:
+    async def bonuses(self, **kwargs) -> Union[list, None]:
         """Gets a User's unclaimed bonuses
 
         Returns:
         TODO: Test what a list of bonuses would look like
             List: List of unclaimed bonuses
             None: If there are no unclaimed bonuses
         """
-        resp = await self._get(self.V2_API_URL, "bonuses")  # type: ignore
+        resp = await self._get(self.V2_API_URL, "bonuses", **kwargs)  # type: ignore
         if resp == []:
             return None
         return resp
```

### Comparing `saladpy-1.0.2a3/saladpy/methods/types/BaseClient.py` & `saladpy-1.0.2a4/saladpy/methods/types/BaseClient.py`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a3/saladpy/methods/types/UserTypes.py` & `saladpy-1.0.2a4/saladpy/methods/types/UserTypes.py`

 * *Files identical despite different names*

### Comparing `saladpy-1.0.2a3/saladpy.egg-info/PKG-INFO` & `saladpy-1.0.2a4/saladpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saladpy
-Version: 1.0.2a3
+Version: 1.0.2a4
 Summary: A Python wrapper for the Salad Web API
 Home-page: https://github.com/Coddo-Python/SaladPy
 Author: Coddo-Python
 Author-email: Coddo <coddobusiness@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2015-present Coddo-Python
```

### Comparing `saladpy-1.0.2a3/setup.py` & `saladpy-1.0.2a4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     author='Coddo-Python',
     url='https://github.com/Coddo-Python/SaladPy',
     project_urls={
         'Github': 'https://github.com/Coddo-Python/SaladPy',
         'Issue tracker': 'https://github.com/Coddo-Python/SaladPy/issues',
         'Docs': 'https://saladpy.gitbook.io/saladpy-docs/'
     },
-    version="1.0.2-a.3",
+    version="1.0.2-a.4",
     license='MIT',
     description='A Python wrapper for the Salad Web API',
     long_description=readme,
     packages=["saladpy", "saladpy.methods", "saladpy.methods.types"],
     install_requires=requirements,
     python_requires='>=3.8.0',
     classifiers=[
```

