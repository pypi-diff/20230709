# Comparing `tmp/szh_toolbox-0.0.8.tar.gz` & `tmp/szh_toolbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "szh_toolbox-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "szh_toolbox-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `szh_toolbox-0.0.8.tar` & `szh_toolbox-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1290 2023-07-01 06:49:22.545897 szh_toolbox-0.0.8/README.md
--rw-r--r--   0        0        0      692 2023-07-03 05:38:45.662333 szh_toolbox-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4875 2023-07-01 06:45:47.550013 szh_toolbox-0.0.8/src/szh_toolbox/__init__.py
--rw-r--r--   0        0        0      349 2023-06-29 02:31:19.795188 szh_toolbox-0.0.8/src/szh_toolbox/commond.py
--rw-r--r--   0        0        0     2951 2023-07-02 06:38:49.985918 szh_toolbox-0.0.8/src/szh_toolbox/mylogger.py
--rw-r--r--   0        0        0     4563 2023-05-15 06:26:45.362456 szh_toolbox-0.0.8/src/szh_toolbox/namelist.py
--rw-r--r--   0        0        0     2793 2023-06-29 06:39:39.421182 szh_toolbox-0.0.8/src/szh_toolbox/namelistwps.py
--rw-r--r--   0        0        0     4237 2023-07-03 05:29:43.330397 szh_toolbox-0.0.8/src/szh_toolbox/noaa_download.py
--rw-r--r--   0        0        0       67 2023-06-28 07:18:07.747348 szh_toolbox-0.0.8/src/szh_toolbox/test.py
--rw-r--r--   0        0        0     1753 1970-01-01 00:00:00.000000 szh_toolbox-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1290 2023-07-01 06:49:22.545897 szh_toolbox-0.0.9/README.md
+-rw-r--r--   0        0        0      739 2023-07-08 15:17:24.200043 szh_toolbox-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4875 2023-07-01 06:45:47.550013 szh_toolbox-0.0.9/src/szh_toolbox/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-29 02:31:19.795188 szh_toolbox-0.0.9/src/szh_toolbox/commond.py
+-rw-r--r--   0        0        0     2951 2023-07-02 06:38:49.985918 szh_toolbox-0.0.9/src/szh_toolbox/mylogger.py
+-rw-r--r--   0        0        0     4563 2023-05-15 06:26:45.362456 szh_toolbox-0.0.9/src/szh_toolbox/namelist.py
+-rw-r--r--   0        0        0     2831 2023-07-08 13:38:45.373229 szh_toolbox-0.0.9/src/szh_toolbox/namelist_wps.py
+-rw-r--r--   0        0        0     8012 2023-07-08 15:16:08.390411 szh_toolbox-0.0.9/src/szh_toolbox/namelist_wps_ui.py
+-rw-r--r--   0        0        0     4237 2023-07-03 05:29:43.330397 szh_toolbox-0.0.9/src/szh_toolbox/noaa_download.py
+-rw-r--r--   0        0        0       67 2023-06-28 07:18:07.747348 szh_toolbox-0.0.9/src/szh_toolbox/test.py
+-rw-r--r--   0        0        0     1753 1970-01-01 00:00:00.000000 szh_toolbox-0.0.9/PKG-INFO
```

### Comparing `szh_toolbox-0.0.8/README.md` & `szh_toolbox-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `szh_toolbox-0.0.8/pyproject.toml` & `szh_toolbox-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["flit_core>=3.9"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "szh_toolbox"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="szh", email="suo.zh@qq.com"},
 ]
 description = "我自己的工具箱"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.scripts]
 greetc = "szh_toolbox.commond:main"
-st-wps = "szh_toolbox.namelistwps:main"
+st-wps = "szh_toolbox.namelist_wps:main"
 st-noaa = "szh_toolbox.noaa_download:commond"
+st-wpsui = "szh_toolbox.namelist_wps_ui:main"
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `szh_toolbox-0.0.8/src/szh_toolbox/__init__.py` & `szh_toolbox-0.0.9/src/szh_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `szh_toolbox-0.0.8/src/szh_toolbox/mylogger.py` & `szh_toolbox-0.0.9/src/szh_toolbox/mylogger.py`

 * *Files identical despite different names*

### Comparing `szh_toolbox-0.0.8/src/szh_toolbox/namelist.py` & `szh_toolbox-0.0.9/src/szh_toolbox/namelist.py`

 * *Files identical despite different names*

### Comparing `szh_toolbox-0.0.8/src/szh_toolbox/namelistwps.py` & `szh_toolbox-0.0.9/src/szh_toolbox/namelist_wps.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     用于计算namelist.wps中的参数计算经纬度范围
     rlat: 中心纬度
     rlon: 中心纬度
     tlat: 真实经纬度true_lat
     delta: 网格间距dx,dy你设置成不一样的，也会是一样的
     e_we: 东西方向格点数
     e_sn: 南北方向格点数
+    返回：north, west, south, east
     '''
     # 创建自定义麦卡托投影的定义字符串
     mercator_proj = f"+proj=merc +lon_0=100 +lat_ts={tlat} +x_0=0 +y_0=0 +ellps=WGS84 +units=m +no_defs"
 
     # 创建转换器实例
     tf1 = Transformer.from_crs("EPSG:4326", mercator_proj)
     tf2 = Transformer.from_crs(mercator_proj, "EPSG:4326")
```

### Comparing `szh_toolbox-0.0.8/src/szh_toolbox/noaa_download.py` & `szh_toolbox-0.0.9/src/szh_toolbox/noaa_download.py`

 * *Files identical despite different names*

### Comparing `szh_toolbox-0.0.8/PKG-INFO` & `szh_toolbox-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: szh_toolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: 我自己的工具箱
 Author-email: szh <suo.zh@qq.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

