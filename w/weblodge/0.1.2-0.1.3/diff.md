# Comparing `tmp/weblodge-0.1.2.tar.gz` & `tmp/weblodge-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weblodge-0.1.2.tar", max compression
+gzip compressed data, was "weblodge-0.1.3.tar", max compression
```

## Comparing `weblodge-0.1.2.tar` & `weblodge-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1074 2023-07-06 14:06:29.155692 weblodge-0.1.2/LICENSE
--rw-r--r--   0        0        0      595 2023-07-08 15:13:03.051883 weblodge-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5597 2023-07-08 15:09:42.600637 weblodge-0.1.2/README.md
--rw-r--r--   0        0        0       98 2023-07-06 14:06:29.174572 weblodge-0.1.2/weblodge/__main__.py
--rw-r--r--   0        0        0      349 2023-07-06 14:06:29.174572 weblodge-0.1.2/weblodge/_azure/__init__.py
--rw-r--r--   0        0        0     3431 2023-07-06 14:06:29.175573 weblodge-0.1.2/weblodge/_azure/appservice.py
--rw-r--r--   0        0        0     2076 2023-07-06 14:06:29.176571 weblodge-0.1.2/weblodge/_azure/cli.py
--rw-r--r--   0        0        0     2209 2023-07-06 14:06:29.177571 weblodge-0.1.2/weblodge/_azure/resource_group.py
--rw-r--r--   0        0        0     1123 2023-07-06 14:06:29.177571 weblodge-0.1.2/weblodge/_azure/subscription.py
--rw-r--r--   0        0        0     4137 2023-07-08 14:52:51.005316 weblodge-0.1.2/weblodge/_azure/web_app.py
--rw-r--r--   0        0        0      147 2023-07-06 14:06:29.178571 weblodge-0.1.2/weblodge/cli/__init__.py
--rw-r--r--   0        0        0     3013 2023-07-08 14:53:30.288516 weblodge-0.1.2/weblodge/cli/main.py
--rw-r--r--   0        0        0      175 2023-07-06 14:06:29.179570 weblodge-0.1.2/weblodge/config/__init__.py
--rw-r--r--   0        0        0      877 2023-07-06 14:06:29.180572 weblodge-0.1.2/weblodge/config/item.py
--rw-r--r--   0        0        0       82 2023-07-06 14:06:29.180572 weblodge-0.1.2/weblodge/parameters/__init__.py
--rw-r--r--   0        0        0     2399 2023-07-08 12:35:00.012463 weblodge-0.1.2/weblodge/parameters/parameters.py
--rw-r--r--   0        0        0      165 2023-07-06 14:06:29.182572 weblodge-0.1.2/weblodge/state/__init__.py
--rw-r--r--   0        0        0      748 2023-07-06 14:06:29.182572 weblodge-0.1.2/weblodge/state/state.py
--rw-r--r--   0        0        0      202 2023-07-08 12:33:03.246479 weblodge-0.1.2/weblodge/web_app/__init__.py
--rw-r--r--   0        0        0     4683 2023-07-08 13:35:49.466210 weblodge-0.1.2/weblodge/web_app/build.py
--rw-r--r--   0        0        0     1320 2023-07-06 14:06:29.184570 weblodge-0.1.2/weblodge/web_app/delete.py
--rw-r--r--   0        0        0     3329 2023-07-06 14:06:29.184570 weblodge-0.1.2/weblodge/web_app/deploy.py
--rw-r--r--   0        0        0      726 2023-07-08 12:43:17.432229 weblodge-0.1.2/weblodge/web_app/logs.py
--rw-r--r--   0        0        0     1692 2023-07-08 12:32:53.895619 weblodge-0.1.2/weblodge/web_app/web_app.py
--rw-r--r--   0        0        0     7313 1970-01-01 00:00:00.000000 weblodge-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-06 14:06:29.155692 weblodge-0.1.3/LICENSE
+-rw-r--r--   0        0        0      614 2023-07-08 22:46:33.768180 weblodge-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5597 2023-07-08 22:19:02.551640 weblodge-0.1.3/README.md
+-rw-r--r--   0        0        0       98 2023-07-06 14:06:29.174572 weblodge-0.1.3/weblodge/__main__.py
+-rw-r--r--   0        0        0      349 2023-07-06 14:06:29.174572 weblodge-0.1.3/weblodge/_azure/__init__.py
+-rw-r--r--   0        0        0     3431 2023-07-06 14:06:29.175573 weblodge-0.1.3/weblodge/_azure/appservice.py
+-rw-r--r--   0        0        0     2483 2023-07-08 22:20:03.474586 weblodge-0.1.3/weblodge/_azure/cli.py
+-rw-r--r--   0        0        0     2209 2023-07-06 14:06:29.177571 weblodge-0.1.3/weblodge/_azure/resource_group.py
+-rw-r--r--   0        0        0     1123 2023-07-06 14:06:29.177571 weblodge-0.1.3/weblodge/_azure/subscription.py
+-rw-r--r--   0        0        0     4275 2023-07-08 22:43:38.841236 weblodge-0.1.3/weblodge/_azure/web_app.py
+-rw-r--r--   0        0        0      147 2023-07-06 14:06:29.178571 weblodge-0.1.3/weblodge/cli/__init__.py
+-rw-r--r--   0        0        0     3261 2023-07-08 22:20:03.486153 weblodge-0.1.3/weblodge/cli/main.py
+-rw-r--r--   0        0        0      175 2023-07-06 14:06:29.179570 weblodge-0.1.3/weblodge/config/__init__.py
+-rw-r--r--   0        0        0      877 2023-07-06 14:06:29.180572 weblodge-0.1.3/weblodge/config/item.py
+-rw-r--r--   0        0        0       92 2023-07-08 22:20:03.486153 weblodge-0.1.3/weblodge/parameters/__init__.py
+-rw-r--r--   0        0        0     2466 2023-07-08 22:20:03.486153 weblodge-0.1.3/weblodge/parameters/parameters.py
+-rw-r--r--   0        0        0      165 2023-07-06 14:06:29.182572 weblodge-0.1.3/weblodge/state/__init__.py
+-rw-r--r--   0        0        0      748 2023-07-06 14:06:29.182572 weblodge-0.1.3/weblodge/state/state.py
+-rw-r--r--   0        0        0      202 2023-07-08 22:19:02.555640 weblodge-0.1.3/weblodge/web_app/__init__.py
+-rw-r--r--   0        0        0     4728 2023-07-08 22:43:56.400491 weblodge-0.1.3/weblodge/web_app/build.py
+-rw-r--r--   0        0        0     1320 2023-07-06 14:06:29.184570 weblodge-0.1.3/weblodge/web_app/delete.py
+-rw-r--r--   0        0        0     4561 2023-07-08 22:29:44.849936 weblodge-0.1.3/weblodge/web_app/deploy.py
+-rw-r--r--   0        0        0      696 2023-07-08 22:19:02.556642 weblodge-0.1.3/weblodge/web_app/logs.py
+-rw-r--r--   0        0        0     1692 2023-07-08 12:32:53.895619 weblodge-0.1.3/weblodge/web_app/web_app.py
+-rw-r--r--   0        0        0     7353 1970-01-01 00:00:00.000000 weblodge-0.1.3/PKG-INFO
```

### Comparing `weblodge-0.1.2/LICENSE` & `weblodge-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.2/pyproject.toml` & `weblodge-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weblodge"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Vuillemot Florian <vuillemot.florian@outlook.fr>"]
 
 repository = "https://github.com/florian-vuillemot/weblodge"
 homepage = "https://github.com/florian-vuillemot/weblodge"
 
 readme = ["README.md", "LICENSE"]
@@ -12,14 +12,15 @@
 
 [tool.poetry.scripts]
 weblodge = "weblodge.cli:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 azure-cli = "2.49"
+urllib3 = "^2.0.3"
 
 [tool.poetry.group.linter.dependencies]
 pylint = ">=2.17,<=3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `weblodge-0.1.2/README.md` & `weblodge-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.2/weblodge/_azure/appservice.py` & `weblodge-0.1.3/weblodge/_azure/appservice.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.2/weblodge/_azure/cli.py` & `weblodge-0.1.3/weblodge/_azure/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Interface to the Azure CLI.
 """
 import json
+import time
 from io import StringIO
 import logging
 from typing import Dict, Union
 
 from azure.cli.core import get_default_cli
 
 
@@ -26,27 +27,35 @@
             to_json=True,
             tags: Dict[str, str] = None
         ) -> Union[str, Dict]:
         """
         Execute an Azure CLI command and return its output.
         If `to_json` is True, the output is converted to a JSON object.
         """
-
         if self._first_invoke:
             self._first_invoke = False
 
             try:
                 return self._invoke(command, to_json=to_json, tags=tags)
             except Exception:  # pylint: disable=broad-exception-caught
                 # Command may fail if the user is not logged in.
                 logger.info('Previous command failed, try login to Azure CLI...')
                 self._invoke('login', False, None)
                 logger.info('Login successful, retry previous command...')
 
-        return self._invoke(command, to_json=to_json, tags=tags)
+        try:
+            return self._invoke(command, to_json=to_json, tags=tags)
+        except Exception:  # pylint: disable=broad-exception-caught
+            logger.info(
+                'The previous command failed.\n'
+                'This may be due to simultaneous asynchronous operations.\n'
+                'Will try again in 30 seconds...'
+            )
+            time.sleep(30)
+            return self._invoke(command, to_json=to_json, tags=tags)
 
     def _invoke(self, command: str, to_json: bool, tags) -> Union[str, Dict]:
         # Convert the string command to a array of arguments.
         cmd = command.split()
         # Create a file-like object to store the output.
         out_fd = StringIO()
```

### Comparing `weblodge-0.1.2/weblodge/_azure/resource_group.py` & `weblodge-0.1.3/weblodge/_azure/resource_group.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.2/weblodge/_azure/subscription.py` & `weblodge-0.1.3/weblodge/_azure/subscription.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.2/weblodge/_azure/web_app.py` & `weblodge-0.1.3/weblodge/_azure/web_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,28 +90,30 @@
         ) -> WebAppModel:
         """
         Create a new WebApp.
 
         Settings enabled:
         - WebSockets
         - HTTP/2
-        - Always On
+        - Always On: If the SKU is not F1.
+        - Startup file: weblodge.startup
         """
         rg_name = resource_group.name if resource_group else app_service.resource_group.name
 
         self._cli.invoke(
             f'webapp create -g {rg_name} -p {app_service.id} -n {name} --runtime PYTHON:{python_version}',  # pylint: disable=line-too-long
             tags=tags
         )
         self._cli.invoke(
             ' '.join((
                 f'webapp config set --resource-group {rg_name} --name {name}',
                 '--web-sockets-enabled true',
                 '--http20-enabled',
-                '--always-on true'
+                '--startup-file weblodge.startup',
+                f'--always-on {app_service.sku != "F1"}',
             ))
         )
         return self.get(name, force_reload=True)
 
     def deploy(self, webapp: WebAppModel, src: str) -> None:
         """
         Deploy an application zipped to the WebApp.
```

### Comparing `weblodge-0.1.2/weblodge/cli/main.py` & `weblodge-0.1.3/weblodge/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,16 +71,21 @@
         config = build(config)
 
     logger.info('Deploying...')
     config = parameters.load(
         web_app.deploy_config(),
         config
     )
-    webapp_url = web_app.deploy(config)
-    logger.info(f"Successfully deployed at 'https://{webapp_url}'.")
+    if webapp_url := web_app.deploy(config):
+        logger.info(f"The application will soon be available on: https://{webapp_url}")
+    else:
+        logger.critical(
+            'The application may not be deployed, but the infrastructure may be' \
+            f" partially created. You can delete it by running: '{parameters.CLI_NAME} delete'"
+        )
     return config
 
 
 def delete(config: Dict[str, str]) -> Dict[str, str]:
     """
     Delete the application.
     """
```

### Comparing `weblodge-0.1.2/weblodge/config/item.py` & `weblodge-0.1.3/weblodge/config/item.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.2/weblodge/parameters/parameters.py` & `weblodge-0.1.3/weblodge/parameters/parameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """
 User inputs can be provided by command line.
 This package contains the logic to parse the command line arguments for internal
 components based on the configuration items. but also the global arguments that are
 hard coded.
 """
+import sys
 import argparse
 from dataclasses import dataclass
 from typing import Dict, List
 
 from weblodge.config import Item as ConfigItem
 
 
+# Command Line Interface name.
+CLI_NAME = sys.argv[0]
+
+
 @dataclass(frozen=True)
 class Global:
     """
     Global and pre defined configuration.
     """
     # The action to perform.
     action: str
```

### Comparing `weblodge-0.1.2/weblodge/state/state.py` & `weblodge-0.1.3/weblodge/state/state.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.2/weblodge/web_app/build.py` & `weblodge-0.1.3/weblodge/web_app/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     app: str = 'app'
 
     # Zip file that contains the user application code.
     package: str = 'azwebapp.zip'
     # Kudu deployment config file.
     kudu_config: str = '.deployment'
     # Startup file.
-    startup_file: str = 'startup.txt'
+    # Set in the deployment config too.
+    startup_file: str = 'weblodge.startup'
 
     @property
     def package_path(self) -> str:
         """
         Return the package path.
         """
         return os.path.join(self.dist, self.package)
```

### Comparing `weblodge-0.1.2/weblodge/web_app/delete.py` & `weblodge-0.1.3/weblodge/web_app/delete.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.2/weblodge/web_app/deploy.py` & `weblodge-0.1.3/weblodge/web_app/deploy.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,21 +8,27 @@
 
 All that infrastructure is created in the same Azure region and in the same Azure
 Resource Group.
 """
 import os
 import random
 import string
-from typing import List
+import logging
+from typing import List, Optional
 from dataclasses import dataclass, field
 
+from urllib3 import Retry, request
+
 from weblodge.config import Item as ConfigItem
 from weblodge._azure import Cli, ResourceGroup, AppService, WebApp
 
 
+logger = logging.getLogger('weblodge')
+
+
 @dataclass
 class Deploy:
     """
     Facade to the deployment process.
 
     Create the infrastructure that will host the application.
     If not provide, a random name will be generated to allow user to deploy an application
@@ -50,14 +56,15 @@
         """
         Configure the deployment.
         """
         return [
             ConfigItem(
                 name='app_name',
                 description='Unique name of the application within Azure. If not provide, a random name is used.',  # pylint: disable=line-too-long
+                default=cls.app_name
             ),
             ConfigItem(
                 name='sku',
                 description='The application computational power (https://azure.microsoft.com/en-us/pricing/details/app-service/linux/).',  # pylint: disable=line-too-long
                 default=cls.sku
             ),
             ConfigItem(
@@ -73,31 +80,57 @@
             ConfigItem(
                 name='dist',
                 description='Folder containing the application zipped.',
                 default=cls.dist
             ),
         ]
 
-    def deploy(self, package_name: str='azwebapp.zip') -> str:
+    def deploy(self, package_name: str='azwebapp.zip') -> Optional[str]:
         """
         Deploy the application to Azure and return its URL.
         """
         default_name = f'{self.app_name}-{self.environment}-{self.location}'
 
         cli = Cli()
         web_app_cls = WebApp(cli)
 
+        logger.info('The infrastructure is being created or updated...')
         web_app = web_app_cls.create(
             self.app_name,
             AppService(cli).create(
                 f'asp-{default_name}',
                 self.sku,
                 ResourceGroup(cli).create(
                     f'rg-{default_name}',
                     self.location,
                     tags=self.tags
                 )
             )
         )
+        logger.info('The infrastructure has been created or updated.')
+
+        logger.info('Waiting the infrastructure to be running...')
+        if not self.ping(web_app):
+            logger.info('The infrastructure is not yet running. Retrying...')
+            if not self.ping(web_app):
+                logger.critical('The infrastructure is not yet running.\nPlease retry later.')
+                return None
+        logger.info('The infrastructure is running.')
 
+        logger.info('Uploading the application...')
         web_app_cls.deploy(web_app, os.path.join(self.dist, package_name))
+        logger.info('The application has been uploaded.')
         return web_app.host_names[0]
+
+    def ping(self, web_app: WebApp) -> bool:
+        """
+        Ping the application to warm it up.
+        Return True if the application is up and running.
+        """
+        try:
+            return request(
+                "GET",
+                web_app.host_names[0],
+                retries=Retry(total=10, backoff_factor=5)
+            ).status < 400
+        except:  # pylint: disable=bare-except
+            return False
```

### Comparing `weblodge-0.1.2/weblodge/web_app/logs.py` & `weblodge-0.1.3/weblodge/web_app/logs.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-"""
-Stream logs from an Azure Web App in the user console.
-"""
-from typing import List, Dict
-
-from weblodge.config import Item as ConfigItem
-from weblodge._azure import Cli, WebApp
-
-
-def config() -> List[ConfigItem]:
-    """
-    Getting logs from the application configuration.
-    """
-    return [
-        ConfigItem(
-            name='app_name',
-            description='The application name.'
-        )
-    ]
-
-def logs(config_: Dict[str, str]):
-    """
-    Stream logs from the application.
-    This function is blocking and never returns.
-    User must run CTRL+C to stop the process.
-    """
-    web_app = WebApp(Cli())
-
-    # Stream logs.
-    web_app.logs(web_app.get(config_['app_name']))
+"""
+Stream logs from an Azure Web App in the user console.
+"""
+from typing import List, Dict
+
+from weblodge.config import Item as ConfigItem
+from weblodge._azure import Cli, WebApp
+
+
+def config() -> List[ConfigItem]:
+    """
+    Getting logs from the application configuration.
+    """
+    return [
+        ConfigItem(
+            name='app_name',
+            description='The application name.'
+        )
+    ]
+
+def logs(config_: Dict[str, str]):
+    """
+    Stream logs from the application.
+    This function is blocking and never returns.
+    User must run CTRL+C to stop the process.
+    """
+    web_app = WebApp(Cli())
+
+    # Stream logs.
+    web_app.logs(web_app.get(config_['app_name']))
```

### Comparing `weblodge-0.1.2/weblodge/web_app/web_app.py` & `weblodge-0.1.3/weblodge/web_app/web_app.py`

 * *Files identical despite different names*

### Comparing `weblodge-0.1.2/PKG-INFO` & `weblodge-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: weblodge
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/florian-vuillemot/weblodge
 Keywords: deployment,azure
 Author: Vuillemot Florian
 Author-email: vuillemot.florian@outlook.fr
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: azure-cli (==2.49)
+Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Project-URL: Repository, https://github.com/florian-vuillemot/weblodge
 Description-Content-Type: text/markdown
 
 # WebLodge
 
 **WebLodge** is a command line aiming to provide anyone with deployment and cloud management capabilities.
```

