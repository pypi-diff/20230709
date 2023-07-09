# Comparing `tmp/sabledocs-0.4.198.tar.gz` & `tmp/sabledocs-0.5.202.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.4.198.tar", last modified: Tue Jun 27 21:35:32 2023, max compression
+gzip compressed data, was "sabledocs-0.5.202.dev0.tar", last modified: Sun Jul  9 15:59:27 2023, max compression
```

## Comparing `sabledocs-0.4.198.tar` & `sabledocs-0.5.202.dev0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:35:32.634014 sabledocs-0.4.198/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-06-27 21:35:19.000000 sabledocs-0.4.198/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-06-27 21:35:19.000000 sabledocs-0.4.198/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2023-06-27 21:35:32.634014 sabledocs-0.4.198/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4261 2023-06-27 21:35:19.000000 sabledocs-0.4.198/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-27 21:35:19.000000 sabledocs-0.4.198/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-06-27 21:35:32.638015 sabledocs-0.4.198/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:35:32.630015 sabledocs-0.4.198/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:35:32.634014 sabledocs-0.4.198/src/sabledocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/lunr_search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13934 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:35:32.634014 sabledocs-0.4.198/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:35:32.634014 sabledocs-0.4.198/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5751 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/templates/_default/search.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      823 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:35:32.634014 sabledocs-0.4.198/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   261187 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2023-06-27 21:35:19.000000 sabledocs-0.4.198/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 21:35:32.634014 sabledocs-0.4.198/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4801 2023-06-27 21:35:32.000000 sabledocs-0.4.198/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-06-27 21:35:32.000000 sabledocs-0.4.198/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-27 21:35:32.000000 sabledocs-0.4.198/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-27 21:35:32.000000 sabledocs-0.4.198/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-06-27 21:35:32.000000 sabledocs-0.4.198/src/sabledocs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-27 21:35:32.000000 sabledocs-0.4.198/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-09 15:59:27.502191 sabledocs-0.5.202.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-07-09 15:59:27.502191 sabledocs-0.5.202.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4261 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-07-09 15:59:27.502191 sabledocs-0.5.202.dev0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-09 15:59:27.498191 sabledocs-0.5.202.dev0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-09 15:59:27.498191 sabledocs-0.5.202.dev0/src/sabledocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3379 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/lunr_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13934 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-09 15:59:27.498191 sabledocs-0.5.202.dev0/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-09 15:59:27.502191 sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5751 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2599 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/search.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1060 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-09 15:59:27.502191 sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   261187 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      849 2023-07-09 15:59:09.000000 sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-09 15:59:27.502191 sabledocs-0.5.202.dev0/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4806 2023-07-09 15:59:27.000000 sabledocs-0.5.202.dev0/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-07-09 15:59:27.000000 sabledocs-0.5.202.dev0/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-09 15:59:27.000000 sabledocs-0.5.202.dev0/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-09 15:59:27.000000 sabledocs-0.5.202.dev0/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-07-09 15:59:27.000000 sabledocs-0.5.202.dev0/src/sabledocs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-07-09 15:59:27.000000 sabledocs-0.5.202.dev0/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.4.198/LICENSE` & `sabledocs-0.5.202.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/PKG-INFO` & `sabledocs-0.5.202.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.4.198
+Version: 0.5.202.dev0
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.4.198/README.md` & `sabledocs-0.5.202.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/pyproject.toml` & `sabledocs-0.5.202.dev0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sabledocs"
-version = "0.4"
+version = "0.5"
 authors = [
   { name="Mark Vincze", email="mrk.vincze@gmail.com" },
 ]
 description = "Static documentation generator for Protobuf and gRPC"
 readme = "README.md"
 requires-python = ">=3.11.0"
 dependencies = [
```

### Comparing `sabledocs-0.4.198/src/sabledocs/__main__.py` & `sabledocs-0.5.202.dev0/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/src/sabledocs/lunr_search.py` & `sabledocs-0.5.202.dev0/src/sabledocs/lunr_search.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.5.202.dev0/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/src/sabledocs/proto_model.py` & `sabledocs-0.5.202.dev0/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/src/sabledocs/sable_config.py` & `sabledocs-0.5.202.dev0/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/src/sabledocs/templates/_default/base.html` & `sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/enum.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-<h5 class="title is-5 type-heading" id="enum-{{ enum.full_name }}">
+<h4 class="title is-4 type-heading" id="enum-{{ enum.full_name }}">
   <a href="#enum-{{ enum.full_name }}" title="{{ enum.full_name }}">enum {{ enum.name }}</a>
   {% if enum.repository_url %}
     <a class="type-source-link" href="{{ enum.repository_url }}">{{ enum.source_file_path }}</a>
   {% endif %}
-</h5>
+</h4>
 
 <div class="block content">
   <p>{{ enum.description_html | safe }}</p>
 </div>
 
 <table class="table is-fullwidth is-hoverable is-bordered">
   <thead>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-** enum_{{_enum.name_}} {% if enum.repository_url %} {{_enum.source_file_path
-}} {% endif %} **
+*** enum_{{_enum.name_}} {% if enum.repository_url %} {{_enum.source_file_path
+}} {% endif %} ***
 {{ enum.description_html | safe }}
 Name                  Number                  Description
 {{ enum_value.name }} {{ enum_value.number }} {{ enum_value.description_html |
                                               safe }}
```

### Comparing `sabledocs-0.4.198/src/sabledocs/templates/_default/index.html` & `sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/src/sabledocs/templates/_default/message.html` & `sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/message.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 {% import "type_name.html" as common %}
 
-<h5 class="title is-5 type-heading" id="message-{{ message.full_name }}">
+<h4 class="title is-4 type-heading" id="message-{{ message.full_name }}">
   <span>
     <a href="#message-{{ message.full_name }}" title="{{ message.full_name }}">message {{ message.name }}</a>
   {% if message.parent_message %}
     <span style="font-size: 0.7em; font-weight: normal">(Nested in {{ common.type_name(message.parent_message) }})</span>
   {% endif %}
   </span>
   {% if message.repository_url %}
     <a class="type-source-link" href="{{ message.repository_url }}">{{ message.source_file_path }}</a>
   {% endif %}
-</h5>
+</h4>
 
 <div class="block content">
   {{ message.description_html | safe }}
 </div>
 
 <table class="table is-fullwidth is-hoverable is-bordered">
   <thead>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% import "type_name.html" as common %}
-**  message_{{_message.name_}} {% if message.parent_message %} (Nested in {
+***  message_{{_message.name_}} {% if message.parent_message %} (Nested in {
 { common.type_name(message.parent_message) }}) {% endif %}  {% if
-message.repository_url %} {{_message.source_file_path_}} {% endif %} **
+message.repository_url %} {{_message.source_file_path_}} {% endif %} ***
 {{ message.description_html | safe }}
              Field      Type             Description            Default Value
                         {% if
                         field.label !=
                         "" and
 {            {          field.label !=   {                      {
 {            {          "optional" %} {  {                      {
```

### Comparing `sabledocs-0.4.198/src/sabledocs/templates/_default/package.html` & `sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/package.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 {% extends "base.html" %}
 {% block content %}
   <p class="mb-2">
     <a style="font-size: 0.9em" href="index.html">← Back to packages</a>
   </p>
-  <h4 class="title is-4">
+  <h3 class="title is-3">
     {% if package.name %}
     Package <code>{{ package.name }}</code>
     {% else %}
     Default package
     {% endif %}
-  </h4>
+  </h3>
 
   <div class="block">
     {% for service in package.services %}
     <p>
       <a href="#service-{{ service.full_name }}">
         <span class="tag" style="min-width: 6em">Service</span>
         <code>{{ service.name }}</code> 
@@ -45,48 +45,48 @@
   <div class="block">
       {{ package.description | safe }}
   </div>
 
   {% if package.services %}
 
   <div class="block">
-    <h4 class="title is-4">
+    <h3 class="title is-3">
       Services
-    </h4>
+    </h3>
 
     {% for service in package.services %}
     <div>
       {% include 'service.html' %} 
     </div>
     {% endfor %}
   </div>
 
   {% endif %}
 
   {% if package.messages %}
 
-    <h4 class="title is-4">
+    <h3 class="title is-3">
       Messages
-    </h4>
+    </h3>
 
     {% for message in package.messages %}
       {% if not message.is_map_entry %}
       <div class="block">
         {% include 'message.html' %} 
       </div>
       {% endif %}
     {% endfor %}
 
   {% endif %}
 
   {% if package.enums %}
 
-    <h4 class="title is-4">
+    <h3 class="title is-3">
       Enums
-    </h4>
+    </h3>
 
     {% for enum in package.enums %}
     <div class="block">
       {% include 'enum.html' %} 
     </div>
     {% endfor %}
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
 {% extends "base.html" %} {% block content %}
 â_Back_to_packages
-*** {% if package.name %} Package {{ package.name }} {% else %} Default package
-{% endif %} ***
+**** {% if package.name %} Package {{ package.name }} {% else %} Default
+package {% endif %} ****
 {% for service in package.services %}
 Service_{{_service.name_}}
 {% endfor %} {% for message in package.messages %} {% if not
 message.is_map_entry %}
 Message_{{_message.name_}}
 {% endif %} {% endfor %} {% for enum in package.enums %}
 Enum_{{_enum.name_}}
 {% endfor %}
 {{ package.description | safe }}
 {% if package.services %}
-*** Services ***
+**** Services ****
 {% for service in package.services %}
 {% include 'service.html' %}
 {% endfor %}
 {% endif %} {% if package.messages %}
-*** Messages ***
+**** Messages ****
 {% for message in package.messages %} {% if not message.is_map_entry %}
 {% include 'message.html' %}
 {% endif %} {% endfor %} {% endif %} {% if package.enums %}
-*** Enums ***
+**** Enums ****
 {% for enum in package.enums %}
 {% include 'enum.html' %}
 {% endfor %} {% endif %} {% endblock %}
```

### Comparing `sabledocs-0.4.198/src/sabledocs/templates/_default/search.html` & `sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/search.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.5.202.dev0/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.4.198/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.5.202.dev0/src/sabledocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.4.198
+Version: 0.5.202.dev0
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.4.198/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.5.202.dev0/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

