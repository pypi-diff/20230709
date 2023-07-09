# Comparing `tmp/finops_crawler-0.1.8.tar.gz` & `tmp/finops_crawler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finops_crawler-0.1.8.tar", max compression
+gzip compressed data, was "finops_crawler-0.1.9.tar", max compression
```

## Comparing `finops_crawler-0.1.8.tar` & `finops_crawler-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1076 2023-06-11 11:15:47.781457 finops_crawler-0.1.8/LICENSE
--rwxr-xr-x   0        0        0     2283 2023-07-01 15:16:28.232353 finops_crawler-0.1.8/README.md
--rwxr-xr-x   0        0        0      789 2023-07-01 15:18:27.715046 finops_crawler-0.1.8/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-06-08 15:33:10.101196 finops_crawler-0.1.8/src/finops_crawler/__init__.py
--rwxr-xr-x   0        0        0     6951 2023-06-29 19:45:07.140846 finops_crawler-0.1.8/src/finops_crawler/aws/README.md
--rwxr-xr-x   0        0        0       37 2023-06-21 18:23:16.839560 finops_crawler-0.1.8/src/finops_crawler/aws/__init__.py
--rwxr-xr-x   0        0        0     6732 2023-06-27 21:37:29.561570 finops_crawler-0.1.8/src/finops_crawler/aws/api.py
--rwxr-xr-x   0        0        0      414 2023-06-29 17:04:38.710868 finops_crawler-0.1.8/src/finops_crawler/aws/example.py
--rwxr-xr-x   0        0        0     4597 2023-06-29 19:45:38.260975 finops_crawler-0.1.8/src/finops_crawler/azure/README.md
--rwxr-xr-x   0        0        0       39 2023-06-21 18:23:06.251734 finops_crawler-0.1.8/src/finops_crawler/azure/__init__.py
--rwxr-xr-x   0        0        0     5976 2023-07-01 11:53:30.533644 finops_crawler-0.1.8/src/finops_crawler/azure/api.py
--rwxr-xr-x   0        0        0      694 2023-07-01 11:52:51.970184 finops_crawler-0.1.8/src/finops_crawler/azure/example.py
--rwxr-xr-x   0        0        0      227 2023-06-11 19:45:00.017416 finops_crawler-0.1.8/src/finops_crawler/base.py
--rwxr-xr-x   0        0        0     2245 2023-06-30 19:22:06.313656 finops_crawler-0.1.8/src/finops_crawler/openai/README.md
--rwxr-xr-x   0        0        0       40 2023-06-27 18:55:36.826379 finops_crawler-0.1.8/src/finops_crawler/openai/__init__.py
--rwxr-xr-x   0        0        0     3565 2023-06-27 21:30:19.118798 finops_crawler-0.1.8/src/finops_crawler/openai/api.py
--rwxr-xr-x   0        0        0      365 2023-06-30 19:16:33.672634 finops_crawler-0.1.8/src/finops_crawler/openai/example.py
--rw-r--r--   0        0        0     3187 2023-07-01 15:18:41.866128 finops_crawler-0.1.8/setup.py
--rw-r--r--   0        0        0     2991 2023-07-01 15:18:41.866421 finops_crawler-0.1.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1076 2023-06-11 11:15:47.781457 finops_crawler-0.1.9/LICENSE
+-rwxr-xr-x   0        0        0     2439 2023-07-01 15:28:05.588871 finops_crawler-0.1.9/README.md
+-rwxr-xr-x   0        0        0      789 2023-07-01 15:28:20.892527 finops_crawler-0.1.9/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-06-08 15:33:10.101196 finops_crawler-0.1.9/src/finops_crawler/__init__.py
+-rwxr-xr-x   0        0        0     6951 2023-06-29 19:45:07.140846 finops_crawler-0.1.9/src/finops_crawler/aws/README.md
+-rwxr-xr-x   0        0        0       37 2023-06-21 18:23:16.839560 finops_crawler-0.1.9/src/finops_crawler/aws/__init__.py
+-rwxr-xr-x   0        0        0     6732 2023-06-27 21:37:29.561570 finops_crawler-0.1.9/src/finops_crawler/aws/api.py
+-rwxr-xr-x   0        0        0      414 2023-06-29 17:04:38.710868 finops_crawler-0.1.9/src/finops_crawler/aws/example.py
+-rwxr-xr-x   0        0        0     4597 2023-06-29 19:45:38.260975 finops_crawler-0.1.9/src/finops_crawler/azure/README.md
+-rwxr-xr-x   0        0        0       39 2023-06-21 18:23:06.251734 finops_crawler-0.1.9/src/finops_crawler/azure/__init__.py
+-rwxr-xr-x   0        0        0     5976 2023-07-01 11:53:30.533644 finops_crawler-0.1.9/src/finops_crawler/azure/api.py
+-rwxr-xr-x   0        0        0      694 2023-07-01 11:52:51.970184 finops_crawler-0.1.9/src/finops_crawler/azure/example.py
+-rwxr-xr-x   0        0        0      227 2023-06-11 19:45:00.017416 finops_crawler-0.1.9/src/finops_crawler/base.py
+-rwxr-xr-x   0        0        0     2245 2023-06-30 19:22:06.313656 finops_crawler-0.1.9/src/finops_crawler/openai/README.md
+-rwxr-xr-x   0        0        0       40 2023-06-27 18:55:36.826379 finops_crawler-0.1.9/src/finops_crawler/openai/__init__.py
+-rwxr-xr-x   0        0        0     3565 2023-06-27 21:30:19.118798 finops_crawler-0.1.9/src/finops_crawler/openai/api.py
+-rwxr-xr-x   0        0        0      365 2023-06-30 19:16:33.672634 finops_crawler-0.1.9/src/finops_crawler/openai/example.py
+-rw-r--r--   0        0        0     3343 2023-07-01 15:29:04.083043 finops_crawler-0.1.9/setup.py
+-rw-r--r--   0        0        0     3147 2023-07-01 15:29:04.083343 finops_crawler-0.1.9/PKG-INFO
```

### Comparing `finops_crawler-0.1.8/LICENSE` & `finops_crawler-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `finops_crawler-0.1.8/README.md` & `finops_crawler-0.1.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 The result, for now, is a Python variable as returned by the API or SDK.
 
 ### Platform-specific documentation
 
 Each platform is different and has a separate guide on how to set up an entity with minimum permissions to read the cost data. Specific code snippets to get started are included.
 
-- [Azure](./src/finops_crawler/azure/README.md)
-- [AWS](./src/finops_crawler/aws/README.md)
-- [OpenAI](./src/finops_crawler/openai/README.md)
+- [Azure](https://github.com/finops-fitness-club/finops-crawler/tree/main/src/finops_crawler/azure)
+- [AWS](https://github.com/finops-fitness-club/finops-crawler/tree/main/src/finops_crawler/aws)
+- [OpenAI](https://github.com/finops-fitness-club/finops-crawler/tree/main/src/finops_crawler/openai)
 
 
 ### Overview of the flow
 
 1. Set up a user (technical user/service principal) for querying the data
 2. Set up permissions for that user
 3. Set environment variables to be used by the package
```

### Comparing `finops_crawler-0.1.8/pyproject.toml` & `finops_crawler-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=0.12"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "finops_crawler"
-version = "0.1.8"
+version = "0.1.9"
 description = "It's a package for importing cost and usage data from various cloud platforms and SaaS tools"
 authors = ["Lauri Koobas <laurikoobas@gmail.com>", "FinOps Fitness Club <finops.fitness.club@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
```

### Comparing `finops_crawler-0.1.8/src/finops_crawler/aws/README.md` & `finops_crawler-0.1.9/src/finops_crawler/aws/README.md`

 * *Files identical despite different names*

### Comparing `finops_crawler-0.1.8/src/finops_crawler/aws/api.py` & `finops_crawler-0.1.9/src/finops_crawler/aws/api.py`

 * *Files identical despite different names*

### Comparing `finops_crawler-0.1.8/src/finops_crawler/azure/README.md` & `finops_crawler-0.1.9/src/finops_crawler/azure/README.md`

 * *Files identical despite different names*

### Comparing `finops_crawler-0.1.8/src/finops_crawler/azure/api.py` & `finops_crawler-0.1.9/src/finops_crawler/azure/api.py`

 * *Files identical despite different names*

### Comparing `finops_crawler-0.1.8/src/finops_crawler/azure/example.py` & `finops_crawler-0.1.9/src/finops_crawler/azure/example.py`

 * *Files identical despite different names*

### Comparing `finops_crawler-0.1.8/src/finops_crawler/openai/README.md` & `finops_crawler-0.1.9/src/finops_crawler/openai/README.md`

 * *Files identical despite different names*

### Comparing `finops_crawler-0.1.8/src/finops_crawler/openai/api.py` & `finops_crawler-0.1.9/src/finops_crawler/openai/api.py`

 * *Files identical despite different names*

### Comparing `finops_crawler-0.1.8/setup.py` & `finops_crawler-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 {'': ['*']}
 
 install_requires = \
 ['boto3==1.26.156', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'finops-crawler',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': "It's a package for importing cost and usage data from various cloud platforms and SaaS tools",
-    'long_description': '# finops-crawler\n\nThis project is active. Development is ongoing, and contributions are welcome (see below).\n\n## Basic Usage\n\nThis package is designed to fetch cost/usage data from various platforms (Azure, AWS, OpenAI, and more to follow).\n\n**The main principle is to have as simple an approach as possible along with the absolute minimum set of permissions required**. Thus, the quickstart part of each guide is presented as CLI commands.\n\nThe result, for now, is a Python variable as returned by the API or SDK.\n\n### Platform-specific documentation\n\nEach platform is different and has a separate guide on how to set up an entity with minimum permissions to read the cost data. Specific code snippets to get started are included.\n\n- [Azure](./src/finops_crawler/azure/README.md)\n- [AWS](./src/finops_crawler/aws/README.md)\n- [OpenAI](./src/finops_crawler/openai/README.md)\n\n\n### Overview of the flow\n\n1. Set up a user (technical user/service principal) for querying the data\n2. Set up permissions for that user\n3. Set environment variables to be used by the package\n4. Use the package\n\n### Resulting data\n\nEach platform has its own format. Also, the same date range might produce different results depending on the platform. Some might include the last day, some may not.\n\nThere is an open data specification being developed by FinOps Foundation ([FOCUS](https://focus.finops.org/)). At this point, it\'s still very new and not adopted by the industry. We will keep a close eye on it and support it as soon as feasible.\n\n*Note*: querying long time periods might trigger paginated results. AWS currently handles it correctly, very soon Azure will as well. Have not tested yet with OpenAI.\n\n### Plans\n\nIncrease breath by expanding to various other tools and platforms (Databricks, GCP, etc.)\n\nIncrease depth by implementing `save_to_postgres` or similar functionality to actually store it.\n\n### Contributing\n\nGot ideas for improvements? We\'d love your input!\n\n1. Fork and clone this repository.\n2. Optionally, choose an issue labeled as "help wanted" or "good first issue".\n3. Submit a pull request with your changes and a clear description.\n\nRemember, all contributions from bug fixes to documentation updates are greatly appreciated!\n\nEnjoy :)\n\nEmail: finops.fitness.club@gmail.com\n',
+    'long_description': '# finops-crawler\n\nThis project is active. Development is ongoing, and contributions are welcome (see below).\n\n## Basic Usage\n\nThis package is designed to fetch cost/usage data from various platforms (Azure, AWS, OpenAI, and more to follow).\n\n**The main principle is to have as simple an approach as possible along with the absolute minimum set of permissions required**. Thus, the quickstart part of each guide is presented as CLI commands.\n\nThe result, for now, is a Python variable as returned by the API or SDK.\n\n### Platform-specific documentation\n\nEach platform is different and has a separate guide on how to set up an entity with minimum permissions to read the cost data. Specific code snippets to get started are included.\n\n- [Azure](https://github.com/finops-fitness-club/finops-crawler/tree/main/src/finops_crawler/azure)\n- [AWS](https://github.com/finops-fitness-club/finops-crawler/tree/main/src/finops_crawler/aws)\n- [OpenAI](https://github.com/finops-fitness-club/finops-crawler/tree/main/src/finops_crawler/openai)\n\n\n### Overview of the flow\n\n1. Set up a user (technical user/service principal) for querying the data\n2. Set up permissions for that user\n3. Set environment variables to be used by the package\n4. Use the package\n\n### Resulting data\n\nEach platform has its own format. Also, the same date range might produce different results depending on the platform. Some might include the last day, some may not.\n\nThere is an open data specification being developed by FinOps Foundation ([FOCUS](https://focus.finops.org/)). At this point, it\'s still very new and not adopted by the industry. We will keep a close eye on it and support it as soon as feasible.\n\n*Note*: querying long time periods might trigger paginated results. AWS currently handles it correctly, very soon Azure will as well. Have not tested yet with OpenAI.\n\n### Plans\n\nIncrease breath by expanding to various other tools and platforms (Databricks, GCP, etc.)\n\nIncrease depth by implementing `save_to_postgres` or similar functionality to actually store it.\n\n### Contributing\n\nGot ideas for improvements? We\'d love your input!\n\n1. Fork and clone this repository.\n2. Optionally, choose an issue labeled as "help wanted" or "good first issue".\n3. Submit a pull request with your changes and a clear description.\n\nRemember, all contributions from bug fixes to documentation updates are greatly appreciated!\n\nEnjoy :)\n\nEmail: finops.fitness.club@gmail.com\n',
     'author': 'Lauri Koobas',
     'author_email': 'laurikoobas@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `finops_crawler-0.1.8/PKG-INFO` & `finops_crawler-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finops-crawler
-Version: 0.1.8
+Version: 0.1.9
 Summary: It's a package for importing cost and usage data from various cloud platforms and SaaS tools
 Author: Lauri Koobas
 Author-email: laurikoobas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: boto3 (==1.26.156)
@@ -26,17 +26,17 @@
 
 The result, for now, is a Python variable as returned by the API or SDK.
 
 ### Platform-specific documentation
 
 Each platform is different and has a separate guide on how to set up an entity with minimum permissions to read the cost data. Specific code snippets to get started are included.
 
-- [Azure](./src/finops_crawler/azure/README.md)
-- [AWS](./src/finops_crawler/aws/README.md)
-- [OpenAI](./src/finops_crawler/openai/README.md)
+- [Azure](https://github.com/finops-fitness-club/finops-crawler/tree/main/src/finops_crawler/azure)
+- [AWS](https://github.com/finops-fitness-club/finops-crawler/tree/main/src/finops_crawler/aws)
+- [OpenAI](https://github.com/finops-fitness-club/finops-crawler/tree/main/src/finops_crawler/openai)
 
 
 ### Overview of the flow
 
 1. Set up a user (technical user/service principal) for querying the data
 2. Set up permissions for that user
 3. Set environment variables to be used by the package
```

