# Comparing `tmp/weblodge-0.1.0.tar.gz` & `tmp/weblodge-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weblodge-0.1.0.tar", max compression
+gzip compressed data, was "weblodge-0.1.2.tar", max compression
```

## Comparing `weblodge-0.1.0.tar` & `weblodge-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,25 @@
--rw-r--r--   0        0        0      390 2023-06-28 15:43:09.062457 weblodge-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       12 2023-06-18 17:16:45.083902 weblodge-0.1.0/README.md
--rw-r--r--   0        0        0       30 2023-06-28 15:44:21.520164 weblodge-0.1.0/weblodge/__main__.py
--rw-r--r--   0        0        0      234 2023-06-27 07:17:59.497866 weblodge-0.1.0/weblodge/_azure/__init__.py
--rw-r--r--   0        0        0     2699 2023-06-28 09:43:31.952087 weblodge-0.1.0/weblodge/_azure/appservice.py
--rw-r--r--   0        0        0     1092 2023-06-27 06:05:46.079859 weblodge-0.1.0/weblodge/_azure/cli.py
--rw-r--r--   0        0        0     1945 2023-06-28 09:55:55.074141 weblodge-0.1.0/weblodge/_azure/resource_group.py
--rw-r--r--   0        0        0      934 2023-06-28 09:43:40.188174 weblodge-0.1.0/weblodge/_azure/subscription.py
--rw-r--r--   0        0        0     2906 2023-06-28 09:43:49.993220 weblodge-0.1.0/weblodge/_azure/web_app.py
--rw-r--r--   0        0        0       22 2023-06-28 15:44:02.050886 weblodge-0.1.0/weblodge/cli/__init__.py
--rw-r--r--   0        0        0      360 2023-06-28 15:43:55.924970 weblodge-0.1.0/weblodge/cli/main.py
--rw-r--r--   0        0        0       40 2023-06-27 06:05:46.082167 weblodge-0.1.0/weblodge/config/__init__.py
--rw-r--r--   0        0        0     1791 2023-06-27 06:05:46.082167 weblodge-0.1.0/weblodge/config/config.py
--rw-r--r--   0        0        0       27 2023-06-27 06:05:46.082167 weblodge-0.1.0/weblodge/web_app/__init__.py
--rw-r--r--   0        0        0     2669 2023-06-28 08:33:52.027932 weblodge-0.1.0/weblodge/web_app/build.py
--rw-r--r--   0        0        0     2741 2023-06-28 08:33:48.109258 weblodge-0.1.0/weblodge/web_app/deploy.py
--rw-r--r--   0        0        0      966 2023-06-28 08:34:17.679026 weblodge-0.1.0/weblodge/web_app/web_app.py
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 weblodge-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-06 14:06:29.155692 weblodge-0.1.2/LICENSE
+-rw-r--r--   0        0        0      595 2023-07-08 15:13:03.051883 weblodge-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5597 2023-07-08 15:09:42.600637 weblodge-0.1.2/README.md
+-rw-r--r--   0        0        0       98 2023-07-06 14:06:29.174572 weblodge-0.1.2/weblodge/__main__.py
+-rw-r--r--   0        0        0      349 2023-07-06 14:06:29.174572 weblodge-0.1.2/weblodge/_azure/__init__.py
+-rw-r--r--   0        0        0     3431 2023-07-06 14:06:29.175573 weblodge-0.1.2/weblodge/_azure/appservice.py
+-rw-r--r--   0        0        0     2076 2023-07-06 14:06:29.176571 weblodge-0.1.2/weblodge/_azure/cli.py
+-rw-r--r--   0        0        0     2209 2023-07-06 14:06:29.177571 weblodge-0.1.2/weblodge/_azure/resource_group.py
+-rw-r--r--   0        0        0     1123 2023-07-06 14:06:29.177571 weblodge-0.1.2/weblodge/_azure/subscription.py
+-rw-r--r--   0        0        0     4137 2023-07-08 14:52:51.005316 weblodge-0.1.2/weblodge/_azure/web_app.py
+-rw-r--r--   0        0        0      147 2023-07-06 14:06:29.178571 weblodge-0.1.2/weblodge/cli/__init__.py
+-rw-r--r--   0        0        0     3013 2023-07-08 14:53:30.288516 weblodge-0.1.2/weblodge/cli/main.py
+-rw-r--r--   0        0        0      175 2023-07-06 14:06:29.179570 weblodge-0.1.2/weblodge/config/__init__.py
+-rw-r--r--   0        0        0      877 2023-07-06 14:06:29.180572 weblodge-0.1.2/weblodge/config/item.py
+-rw-r--r--   0        0        0       82 2023-07-06 14:06:29.180572 weblodge-0.1.2/weblodge/parameters/__init__.py
+-rw-r--r--   0        0        0     2399 2023-07-08 12:35:00.012463 weblodge-0.1.2/weblodge/parameters/parameters.py
+-rw-r--r--   0        0        0      165 2023-07-06 14:06:29.182572 weblodge-0.1.2/weblodge/state/__init__.py
+-rw-r--r--   0        0        0      748 2023-07-06 14:06:29.182572 weblodge-0.1.2/weblodge/state/state.py
+-rw-r--r--   0        0        0      202 2023-07-08 12:33:03.246479 weblodge-0.1.2/weblodge/web_app/__init__.py
+-rw-r--r--   0        0        0     4683 2023-07-08 13:35:49.466210 weblodge-0.1.2/weblodge/web_app/build.py
+-rw-r--r--   0        0        0     1320 2023-07-06 14:06:29.184570 weblodge-0.1.2/weblodge/web_app/delete.py
+-rw-r--r--   0        0        0     3329 2023-07-06 14:06:29.184570 weblodge-0.1.2/weblodge/web_app/deploy.py
+-rw-r--r--   0        0        0      726 2023-07-08 12:43:17.432229 weblodge-0.1.2/weblodge/web_app/logs.py
+-rw-r--r--   0        0        0     1692 2023-07-08 12:32:53.895619 weblodge-0.1.2/weblodge/web_app/web_app.py
+-rw-r--r--   0        0        0     7313 1970-01-01 00:00:00.000000 weblodge-0.1.2/PKG-INFO
```

### Comparing `weblodge-0.1.0/weblodge/_azure/appservice.py` & `weblodge-0.1.2/weblodge/_azure/appservice.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,31 @@
-from typing import List
+"""
+Azure AppService Plan abstraction.
+
+Allow to CRUD on Azure AppService Plan.
+"""
+from typing import Dict, List
 from dataclasses import dataclass
 
 from .cli import Cli
 from .resource_group import ResourceGroupModel, ResourceGroup
 
 
 @dataclass(frozen=True)
 class AppServiceModel:
     """
     Azure AppService Plan representation.
     """
-    id: str
+    id: str  # pylint: disable=invalid-name
     name: str
     number_of_sites: int
     sku: str
     location: str
     resource_group: ResourceGroupModel
+    tags: Dict[str, str]
 
 
 class AppService:
     """
     Helper class to manage Azure AppServices Plan.
     """
     def __init__(self, cli: Cli()) -> None:
@@ -31,48 +37,77 @@
         List all AppServices Plan.
         """
         if force_reload:
             self._resources.clear()
 
         if not self._resources:
             appservices = self._cli.invoke('appservice plan list')
-            for s in appservices:
-                a = AppServiceModel(
-                    id=s['id'],
-                    name=s['name'],
-                    number_of_sites=int(s['numberOfSites']),
-                    sku=s['sku']['name'],
-                    resource_group=ResourceGroup(self._cli).get(s['resourceGroup']),
-                    location=s['location']
+            for asp in appservices:
+                self._resources.append(
+                    AppServiceModel(
+                        id=asp['id'],
+                        name=asp['name'],
+                        number_of_sites=int(asp['numberOfSites']),
+                        sku=asp['sku']['name'],
+                        resource_group=ResourceGroup(self._cli).get(asp['resourceGroup']),
+                        location=asp['location'],
+                        tags=asp['tags']
+                    )
                 )
-                self._resources.append(a)
 
         return self._resources
-    
-    def get(self, name: str = None, resource_group: ResourceGroupModel = None, id_: str = None, force_reload=True) -> AppServiceModel:
+
+    def get(
+            self,
+            name: str = None,
+            resource_group: ResourceGroupModel = None,
+            id_: str = None,
+            force_reload=True
+        ) -> AppServiceModel:
         """
         Return an appservice by its name or its id.
         If resource_group is provided, it will used with the name based search.
         """
-        for s in self.list(force_reload=force_reload):
-            if s.id == id_:
-                return s
-            if s.name == name:
-                if resource_group is None or s.resource_group.name == resource_group.name:
-                    return s
+        for asp in self.list(force_reload=force_reload):
+            if asp.id == id_:
+                return asp
+            if asp.name == name:
+                if resource_group is None or asp.resource_group.name == resource_group.name:
+                    return asp
 
-        raise Exception(f"AppService '{name}' not found.")
+        raise Exception(f"AppService '{name}' not found.")  # pylint: disable=broad-exception-raised
 
     def delete(self, asp: AppServiceModel) -> List[AppServiceModel]:
         """
         Delete an AppService Plan.
         """
-        self._cli.invoke(f'appservice plan delete --name {asp.name} --resource-group {asp.resource_group.name} --yes', to_json=False)
+        asp_name = asp.name
+        rg_name = asp.resource_group.name
+
+        self._cli.invoke(
+            f'appservice plan delete --name {asp_name} --resource-group {rg_name} --yes',
+            to_json=False
+        )
+
         return self.list(force_reload=True)
 
-    def create(self, name: str, sku: str, resource_group: ResourceGroupModel, location: str = None) -> AppServiceModel:
+    # pylint: disable=too-many-arguments
+    def create(
+            self,
+            name: str,
+            sku: str,
+            resource_group: ResourceGroupModel,
+            location: str = None,
+            tags: Dict[str, str] = None
+        ) -> AppServiceModel:
         """
         Create a Linux AppService Plan.
         """
+        tags = tags or resource_group.tags
         location = location or resource_group.location
-        self._cli.invoke(f'appservice plan create --name {name} --sku {sku} --resource-group {resource_group.name} --location {location} --is-linux')
+
+        self._cli.invoke(
+            f'appservice plan create --name {name} --sku {sku} --resource-group {resource_group.name} --location {location} --is-linux',  # pylint: disable=line-too-long
+            tags=tags
+        )
+
         return self.get(name=name, resource_group=resource_group, force_reload=True)
```

### Comparing `weblodge-0.1.0/weblodge/_azure/subscription.py` & `weblodge-0.1.2/weblodge/_azure/subscription.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,45 @@
+"""
+Azure Subscription representation.
+"""
 from typing import List
 from dataclasses import dataclass
 
 from .cli import Cli
 
 
 @dataclass(frozen=True)
 class SubscriptionModel:
     """
     Azure Subscription representation.
     """
-    id: str
+    id: str  # pylint: disable=invalid-name
     name: str
 
 
 class Subscription:
     """
     Helper class to manage Azure subscriptions.
     """
     def __init__(self, cli: Cli()) -> None:
         self._cli = cli
         self._resources = []
 
     def list(self) -> List[SubscriptionModel]:
+        """
+        Return the list of subscriptions.
+        """
         if not self._resources:
             subscription = self._cli.invoke('account list')
             self._resources = [SubscriptionModel(id=s['id'], name=s['name']) for s in subscription]
 
         return self._resources
 
     def get(self, name: str) -> SubscriptionModel:
         """
         Return a subscription by its name.
         """
-        for s in self.list():
-            if s.name == name:
-                return s
+        for sub in self.list():
+            if sub.name == name:
+                return sub
 
-        raise Exception(f"Subscription '{name}' not found.")
+        raise Exception(f"Subscription '{name}' not found.")  # pylint: disable=broad-exception-raised
```

### Comparing `weblodge-0.1.0/weblodge/_azure/web_app.py` & `weblodge-0.1.2/weblodge/_azure/web_app.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
+"""
+Azure Web App representation.
+"""
+from typing import List, Dict
 from dataclasses import dataclass
-from typing import List
 
 from .cli import Cli
 from .resource_group import ResourceGroupModel, ResourceGroup
 from .appservice import AppServiceModel, AppService
 
 
 @dataclass(frozen=True)
-class WebAppModel:
+class WebAppModel:  # pylint: disable=too-many-instance-attributes
     """
     Azure WebApp representation.
     """
     name: str
     kind: str
     location: str
     host_names: List[str]
     linux_fx_version: str
     app_service: AppServiceModel
     resource_group: ResourceGroupModel
+    tags: Dict[str, str]
 
 
 class WebApp:
     """
     Helper class to manage Azure WebApps.
     """
     def __init__(self, cli: Cli()) -> None:
@@ -34,59 +38,97 @@
         """
         if force_reload:
             self._resources.clear()
 
         if not self._resources:
             web_apps = self._cli.invoke('webapp list')
             resource_group_helper = ResourceGroup(self._cli)
-            
-            for w in web_apps:
-                web_app = WebAppModel(
-                    name=w['name'],
-                    host_names=w['hostNames'],
-                    kind=w['kind'],
-                    location=w['location'],
-                    linux_fx_version=w['siteConfig']['linuxFxVersion'],
-                    app_service=AppService(self._cli).get(id_=w['appServicePlanId']),
-                    resource_group=resource_group_helper.get(w['resourceGroup']),
+
+            for web_app in web_apps:
+                self._resources.append(
+                    WebAppModel(
+                        name=web_app['name'],
+                        host_names=web_app['hostNames'],
+                        kind=web_app['kind'],
+                        location=web_app['location'],
+                        linux_fx_version=web_app['siteConfig']['linuxFxVersion'],
+                        app_service=AppService(self._cli).get(id_=web_app['appServicePlanId']),
+                        resource_group=resource_group_helper.get(web_app['resourceGroup']),
+                        tags=web_app['tags']
+                    )
                 )
-                self._resources.append(web_app)
 
         return self._resources
 
     def get(self, name: str, force_reload=False) -> WebAppModel:
         """
         Return a WebApp by its name.
         """
-        for s in self.list(force_reload=force_reload):
-            if s.name == name:
-                return s
+        for webapp in self.list(force_reload=force_reload):
+            if webapp.name == name:
+                return webapp
 
-        raise Exception(f"WebApp '{name}' not found.")
+        raise Exception(f"WebApp '{name}' not found.")  # pylint: disable=broad-exception-raised
 
     def delete(self, webapp: WebAppModel) -> List[WebAppModel]:
         """
         Delete a WebApp.
         """
-        self._cli.invoke(f'webapp delete -g {webapp.resource_group.name} -n {webapp.name}', to_json=False)
+        self._cli.invoke(
+            f'webapp delete -g {webapp.resource_group.name} -n {webapp.name}',
+            to_json=False
+        )
         return self.list(force_reload=True)
 
-    def create(self, name: str, app_service: AppServiceModel, resource_group: ResourceGroupModel = None, python_version: str = '3.10') -> WebAppModel:
+    # pylint: disable=too-many-arguments
+    def create(
+            self,
+            name: str,
+            app_service: AppServiceModel,
+            resource_group: ResourceGroupModel = None,
+            python_version: str = '3.10',
+            tags: Dict[str, str] = None
+        ) -> WebAppModel:
         """
         Create a new WebApp.
+
+        Settings enabled:
+        - WebSockets
+        - HTTP/2
+        - Always On
         """
         rg_name = resource_group.name if resource_group else app_service.resource_group.name
+
+        self._cli.invoke(
+            f'webapp create -g {rg_name} -p {app_service.id} -n {name} --runtime PYTHON:{python_version}',  # pylint: disable=line-too-long
+            tags=tags
+        )
         self._cli.invoke(
-            f'webapp create -g {rg_name} -p {app_service.id} -n {name} --runtime PYTHON:{python_version}'
+            ' '.join((
+                f'webapp config set --resource-group {rg_name} --name {name}',
+                '--web-sockets-enabled true',
+                '--http20-enabled',
+                '--always-on true'
+            ))
         )
         return self.get(name, force_reload=True)
-    
+
     def deploy(self, webapp: WebAppModel, src: str) -> None:
         """
         Deploy an application zipped to the WebApp.
         """
-        rg = webapp.resource_group.name
-        wa = webapp.name
+        self._cli.invoke(
+            ' '.join((
+                'webapp deployment source config-zip',
+                f'-g {webapp.resource_group.name} -n {webapp.name}',
+                f'--src {src}'
+            ))
+        )
 
+    def logs(self, webapp: WebAppModel) -> None:
+        """
+        Stream WebApp logs.
+        This is a blocking operation. User must run CTRL+C to stop the process.
+        """
         self._cli.invoke(
-            f'webapp deployment source config-zip -g {rg} -n {wa} --src {src}'
+            f'webapp log tail -g {webapp.resource_group.name} -n {webapp.name}'
         )
```

### Comparing `weblodge-0.1.0/weblodge/web_app/deploy.py` & `weblodge-0.1.2/weblodge/web_app/deploy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,79 +1,103 @@
+"""
+Create the infrastructure that will host the application.
+
+The infrastructure is composed of:
+- Resource Group
+- App Service Plan
+- Web App
+
+All that infrastructure is created in the same Azure region and in the same Azure
+Resource Group.
+"""
 import os
 import random
 import string
 from typing import List
 from dataclasses import dataclass, field
 
-from weblodge.config import ConfigField
+from weblodge.config import Item as ConfigItem
 from weblodge._azure import Cli, ResourceGroup, AppService, WebApp
 
 
 @dataclass
 class Deploy:
+    """
+    Facade to the deployment process.
+
+    Create the infrastructure that will host the application.
+    If not provide, a random name will be generated to allow user to deploy an application
+    without providing any input.
+    """
     # Application name.
     # This name must be unique across all of Azure WebApplication.
     # It will be used as the URL of the application and for created Azure resources.
     app_name: str = ''.join(random.choice(string.ascii_uppercase) for _ in range(20))
     # Application SKU (https://azure.microsoft.com/en-us/pricing/details/app-service/linux/).
     sku: str = 'F1'
     # Application location.
     location: str = 'northeurope'
     # Application environment.
     environment: str = 'development'
     # Dist directory containing the application zipped.
     dist: str = 'dist'
 
+    # Infrastructure tags.
+    tags: dict = field(default_factory=dict)
+
     @classmethod
-    def config(cls) -> List[ConfigField]:
+    @property
+    def config(cls) -> List[ConfigItem]:
         """
-        Configure the application.
+        Configure the deployment.
         """
         return [
-            ConfigField(
-                name='app-name',
-                description='The unique name of the application. If not provide, a random name will be generated.',
-                example='my-app',
-                default=cls.app_name
+            ConfigItem(
+                name='app_name',
+                description='Unique name of the application within Azure. If not provide, a random name is used.',  # pylint: disable=line-too-long
             ),
-            ConfigField(
+            ConfigItem(
                 name='sku',
-                description='The application SLU (https://azure.microsoft.com/en-us/pricing/details/app-service/linux/).',
-                example='F1, B1',
+                description='The application computational power (https://azure.microsoft.com/en-us/pricing/details/app-service/linux/).',  # pylint: disable=line-too-long
                 default=cls.sku
             ),
-            ConfigField(
+            ConfigItem(
                 name='location',
                 description='The physical application location.',
-                example='northeurope, westeurope',
                 default=cls.location
             ),
-            ConfigField(
+            ConfigItem(
                 name='environment',
                 description='The environment of your application.',
-                example='production, staging, development',
                 default=cls.environment
             ),
-            ConfigField(
+            ConfigItem(
                 name='dist',
                 description='Folder containing the application zipped.',
-                example='dist',
                 default=cls.dist
             ),
         ]
 
-    def deploy(self, package_name: str='azwebapp.zip') -> None:
+    def deploy(self, package_name: str='azwebapp.zip') -> str:
         """
-        Deploy the application to Azure.
+        Deploy the application to Azure and return its URL.
         """
         default_name = f'{self.app_name}-{self.environment}-{self.location}'
+
         cli = Cli()
-        rg = ResourceGroup(cli)
-        wa = WebApp(cli)
-        ap = AppService(cli)
-
-        _rg = rg.create(f'rg-{default_name}', self.location)
-        _ap = ap.create(f'asp-{default_name}', self.sku, _rg)
-        _wa = wa.create(self.app_name, _ap)
+        web_app_cls = WebApp(cli)
+
+        web_app = web_app_cls.create(
+            self.app_name,
+            AppService(cli).create(
+                f'asp-{default_name}',
+                self.sku,
+                ResourceGroup(cli).create(
+                    f'rg-{default_name}',
+                    self.location,
+                    tags=self.tags
+                )
+            )
+        )
 
-        wa.deploy(_wa, os.path.join(self.dist, package_name))
-        return _wa.host_names[0]
+        web_app_cls.deploy(web_app, os.path.join(self.dist, package_name))
+        return web_app.host_names[0]
```

