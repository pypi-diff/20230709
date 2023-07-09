# Comparing `tmp/fastmvc-0.1.2.tar.gz` & `tmp/fastmvc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmvc-0.1.2.tar", max compression
+gzip compressed data, was "fastmvc-0.1.3.tar", max compression
```

## Comparing `fastmvc-0.1.2.tar` & `fastmvc-0.1.3.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0       21 2023-03-02 02:02:53.603068 fastmvc-0.1.2/fastmvc/__init__.py
--rw-r--r--   0        0        0     1915 2023-02-09 12:33:33.962086 fastmvc-0.1.2/fastmvc/extras/flickr.py
--rw-r--r--   0        0        0    12912 2023-03-02 02:08:02.692479 fastmvc-0.1.2/fastmvc/generator.py
--rw-r--r--   0        0        0     2777 2023-03-01 02:13:17.970286 fastmvc-0.1.2/fastmvc/main.py
--rw-r--r--   0        0        0     1549 2023-02-27 18:19:18.475856 fastmvc-0.1.2/fastmvc/models/database/_base.py
--rw-r--r--   0        0        0     1622 2023-02-27 18:19:36.826922 fastmvc-0.1.2/fastmvc/models/database/deta.py
--rw-r--r--   0        0        0     1917 2023-02-27 18:19:08.218798 fastmvc-0.1.2/fastmvc/models/database/firestore.py
--rw-r--r--   0        0        0      193 2023-02-26 14:42:47.054219 fastmvc-0.1.2/fastmvc/models/html.py
--rw-r--r--   0        0        0      185 2023-03-01 02:16:21.356500 fastmvc-0.1.2/fastmvc/templates/core/.env
--rw-r--r--   0        0        0       14 2023-02-28 16:12:11.577451 fastmvc-0.1.2/fastmvc/templates/core/.gitignore
--rw-r--r--   0        0        0      120 2023-02-28 21:16:04.642352 fastmvc-0.1.2/fastmvc/templates/core/app.yaml
--rw-r--r--   0        0        0      570 2023-03-01 01:52:59.493150 fastmvc-0.1.2/fastmvc/templates/core/ignore/service-account-file.json
--rw-r--r--   0        0        0      381 2023-03-02 01:43:36.488810 fastmvc-0.1.2/fastmvc/templates/core/main.py
--rw-r--r--   0        0        0      202 2023-03-01 01:36:11.808802 fastmvc-0.1.2/fastmvc/templates/core/requirements.txt
--rw-r--r--   0        0        0      355 2023-02-26 17:21:55.878811 fastmvc-0.1.2/fastmvc/templates/core/static_pages/router.py
--rw-r--r--   0        0        0     1034 2023-03-01 17:14:46.411838 fastmvc-0.1.2/fastmvc/templates/core/static_pages/static/css/core.css
--rw-r--r--   0        0        0       19 2022-05-30 03:31:54.000000 fastmvc-0.1.2/fastmvc/templates/core/static_pages/static/css/stylesheet.css
--rw-r--r--   0        0        0     2300 2023-03-01 17:24:15.001077 fastmvc-0.1.2/fastmvc/templates/core/static_pages/static/img/logo.svg
--rw-r--r--   0        0        0        0 2022-07-17 19:58:48.000000 fastmvc-0.1.2/fastmvc/templates/core/static_pages/static/js/application.js
--rw-r--r--   0        0        0     1928 2023-02-26 14:48:59.198397 fastmvc-0.1.2/fastmvc/templates/core/static_pages/static/js/color-modes.js
--rw-r--r--   0        0        0     3934 2023-02-26 15:10:33.818704 fastmvc-0.1.2/fastmvc/templates/core/static_pages/templates/_base.html
--rw-r--r--   0        0        0     1854 2023-02-08 02:02:33.691677 fastmvc-0.1.2/fastmvc/templates/core/static_pages/templates/_color_mode.html
--rw-r--r--   0        0        0      282 2023-02-26 17:14:24.019385 fastmvc-0.1.2/fastmvc/templates/core/static_pages/templates/_navlinks.html
--rw-r--r--   0        0        0     2482 2023-02-08 02:04:17.706030 fastmvc-0.1.2/fastmvc/templates/core/static_pages/templates/_svg_symbols.html
--rw-r--r--   0        0        0      535 2023-02-26 15:11:54.245011 fastmvc-0.1.2/fastmvc/templates/core/static_pages/templates/index.html
--rw-r--r--   0        0        0      187 2023-03-01 13:31:47.552403 fastmvc-0.1.2/fastmvc/templates/scaffold/model.py
--rw-r--r--   0        0        0     1933 2023-02-26 14:57:01.653403 fastmvc-0.1.2/fastmvc/templates/scaffold/router.py
--rw-r--r--   0        0        0      951 2023-02-26 14:54:22.688256 fastmvc-0.1.2/fastmvc/templates/scaffold/templates/form.html
--rw-r--r--   0        0        0      800 2023-02-26 14:54:12.351525 fastmvc-0.1.2/fastmvc/templates/scaffold/templates/index.html
--rw-r--r--   0        0        0      821 2023-02-26 14:54:46.340756 fastmvc-0.1.2/fastmvc/templates/scaffold/templates/view.html
--rw-r--r--   0        0        0      378 2023-02-26 14:59:03.174712 fastmvc-0.1.2/fastmvc/templates/scaffold_helpers/bool.html
--rw-r--r--   0        0        0      196 2023-02-26 14:59:37.540256 fastmvc-0.1.2/fastmvc/templates/scaffold_helpers/float.html
--rw-r--r--   0        0        0      182 2023-02-26 15:00:07.003389 fastmvc-0.1.2/fastmvc/templates/scaffold_helpers/int.html
--rw-r--r--   0        0        0      164 2023-02-26 15:01:06.978628 fastmvc-0.1.2/fastmvc/templates/scaffold_helpers/scaffold_navlink.html
--rw-r--r--   0        0        0      205 2023-02-26 15:01:26.765723 fastmvc-0.1.2/fastmvc/templates/scaffold_helpers/str.html
--rw-r--r--   0        0        0      174 2023-02-26 15:01:46.975976 fastmvc-0.1.2/fastmvc/templates/scaffold_helpers/text.html
--rw-r--r--   0        0        0      231 2023-02-10 00:42:21.840062 fastmvc-0.1.2/fastmvc/templates/scaffold_helpers/trix_meta_content.html
--rw-r--r--   0        0        0      537 2023-02-26 15:03:14.452811 fastmvc-0.1.2/fastmvc/templates/scaffold_helpers/user_login.html
--rw-r--r--   0        0        0      261 2023-02-26 15:03:48.395485 fastmvc-0.1.2/fastmvc/templates/scaffold_helpers/wysiwyg.html
--rw-r--r--   0        0        0     2529 2023-03-01 13:33:29.248691 fastmvc-0.1.2/fastmvc/templates/users/model.py
--rw-r--r--   0        0        0     3241 2023-02-26 14:45:44.598398 fastmvc-0.1.2/fastmvc/templates/users/router.py
--rw-r--r--   0        0        0      604 2023-02-26 15:06:44.370207 fastmvc-0.1.2/fastmvc/templates/users/templates/dashboard.html
--rw-r--r--   0        0        0     2088 2023-02-26 15:07:35.756143 fastmvc-0.1.2/fastmvc/templates/users/templates/login.html
--rw-r--r--   0        0        0      670 2023-02-26 14:39:07.527008 fastmvc-0.1.2/fastmvc/templates/users/templates/not_authenticated.html
--rw-r--r--   0        0        0     3254 2023-02-26 15:07:28.995215 fastmvc-0.1.2/fastmvc/templates/users/templates/signup.html
--rw-r--r--   0        0        0     3694 2023-02-26 15:08:27.822779 fastmvc-0.1.2/fastmvc/templates/users/utils.py
--rw-r--r--   0        0        0       27 2022-06-02 02:11:06.000000 fastmvc-0.1.2/fastmvc/user_config.json
--rw-r--r--   0        0        0     1168 2023-03-01 13:23:38.656587 fastmvc-0.1.2/fastmvc/utilities.py
--rw-r--r--   0        0        0      604 2023-03-02 02:03:08.669211 fastmvc-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1313 2023-03-02 02:17:48.947896 fastmvc-0.1.2/README.md
--rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 fastmvc-0.1.2/setup.py
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 fastmvc-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-07-09 14:02:40.343890 fastmvc-0.1.3/fastmvc/__init__.py
+-rw-r--r--   0        0        0     1915 2023-02-09 12:33:33.962086 fastmvc-0.1.3/fastmvc/extras/flickr.py
+-rw-r--r--   0        0        0    12771 2023-07-09 15:27:56.870587 fastmvc-0.1.3/fastmvc/generator.py
+-rw-r--r--   0        0        0     3149 2023-07-09 15:39:12.147182 fastmvc-0.1.3/fastmvc/main.py
+-rw-r--r--   0        0        0     1466 2023-07-09 19:07:38.248982 fastmvc-0.1.3/fastmvc/models/database/_base.py
+-rw-r--r--   0        0        0     1622 2023-02-27 18:19:36.826922 fastmvc-0.1.3/fastmvc/models/database/deta.py
+-rw-r--r--   0        0        0     1888 2023-07-09 19:07:18.891660 fastmvc-0.1.3/fastmvc/models/database/firestore.py
+-rw-r--r--   0        0        0      193 2023-02-26 14:42:47.054219 fastmvc-0.1.3/fastmvc/models/html.py
+-rw-r--r--   0        0        0      185 2023-03-01 02:16:21.356500 fastmvc-0.1.3/fastmvc/templates/core/.env
+-rw-r--r--   0        0        0       66 2023-07-09 02:39:17.318832 fastmvc-0.1.3/fastmvc/templates/core/.gitignore
+-rw-r--r--   0        0        0      334 2023-07-08 20:46:10.189370 fastmvc-0.1.3/fastmvc/templates/core/app.yaml
+-rw-r--r--   0        0        0      570 2023-03-01 01:52:59.493150 fastmvc-0.1.3/fastmvc/templates/core/ignore/service-account-file.json
+-rw-r--r--   0        0        0      381 2023-03-02 01:43:36.488810 fastmvc-0.1.3/fastmvc/templates/core/main.py
+-rw-r--r--   0        0        0      202 2023-03-01 01:36:11.808802 fastmvc-0.1.3/fastmvc/templates/core/requirements.txt
+-rw-r--r--   0        0        0      355 2023-02-26 17:21:55.878811 fastmvc-0.1.3/fastmvc/templates/core/static_pages/router.py
+-rw-r--r--   0        0        0     1034 2023-03-01 17:14:46.411838 fastmvc-0.1.3/fastmvc/templates/core/static_pages/static/css/core.css
+-rw-r--r--   0        0        0       19 2022-05-30 03:31:54.000000 fastmvc-0.1.3/fastmvc/templates/core/static_pages/static/css/stylesheet.css
+-rw-r--r--   0        0        0     2300 2023-03-01 17:24:15.001077 fastmvc-0.1.3/fastmvc/templates/core/static_pages/static/img/logo.svg
+-rw-r--r--   0        0        0        0 2022-07-17 19:58:48.000000 fastmvc-0.1.3/fastmvc/templates/core/static_pages/static/js/application.js
+-rw-r--r--   0        0        0     1928 2023-02-26 14:48:59.198397 fastmvc-0.1.3/fastmvc/templates/core/static_pages/static/js/color-modes.js
+-rw-r--r--   0        0        0     3926 2023-07-04 01:06:21.191892 fastmvc-0.1.3/fastmvc/templates/core/static_pages/templates/_base.html
+-rw-r--r--   0        0        0     1854 2023-02-08 02:02:33.691677 fastmvc-0.1.3/fastmvc/templates/core/static_pages/templates/_color_mode.html
+-rw-r--r--   0        0        0      282 2023-02-26 17:14:24.019385 fastmvc-0.1.3/fastmvc/templates/core/static_pages/templates/_navlinks.html
+-rw-r--r--   0        0        0     2482 2023-02-08 02:04:17.706030 fastmvc-0.1.3/fastmvc/templates/core/static_pages/templates/_svg_symbols.html
+-rw-r--r--   0        0        0      535 2023-02-26 15:11:54.245011 fastmvc-0.1.3/fastmvc/templates/core/static_pages/templates/index.html
+-rw-r--r--   0        0        0      255 2023-07-09 19:10:05.928473 fastmvc-0.1.3/fastmvc/templates/scaffold/model.py
+-rw-r--r--   0        0        0     1933 2023-02-26 14:57:01.653403 fastmvc-0.1.3/fastmvc/templates/scaffold/router.py
+-rw-r--r--   0        0        0      951 2023-02-26 14:54:22.688256 fastmvc-0.1.3/fastmvc/templates/scaffold/templates/form.html
+-rw-r--r--   0        0        0      800 2023-02-26 14:54:12.351525 fastmvc-0.1.3/fastmvc/templates/scaffold/templates/index.html
+-rw-r--r--   0        0        0      821 2023-02-26 14:54:46.340756 fastmvc-0.1.3/fastmvc/templates/scaffold/templates/view.html
+-rw-r--r--   0        0        0      378 2023-02-26 14:59:03.174712 fastmvc-0.1.3/fastmvc/templates/scaffold_helpers/bool.html
+-rw-r--r--   0        0        0      196 2023-02-26 14:59:37.540256 fastmvc-0.1.3/fastmvc/templates/scaffold_helpers/float.html
+-rw-r--r--   0        0        0      182 2023-02-26 15:00:07.003389 fastmvc-0.1.3/fastmvc/templates/scaffold_helpers/int.html
+-rw-r--r--   0        0        0      164 2023-02-26 15:01:06.978628 fastmvc-0.1.3/fastmvc/templates/scaffold_helpers/scaffold_navlink.html
+-rw-r--r--   0        0        0      205 2023-02-26 15:01:26.765723 fastmvc-0.1.3/fastmvc/templates/scaffold_helpers/str.html
+-rw-r--r--   0        0        0      174 2023-02-26 15:01:46.975976 fastmvc-0.1.3/fastmvc/templates/scaffold_helpers/text.html
+-rw-r--r--   0        0        0      231 2023-02-10 00:42:21.840062 fastmvc-0.1.3/fastmvc/templates/scaffold_helpers/trix_meta_content.html
+-rw-r--r--   0        0        0      537 2023-02-26 15:03:14.452811 fastmvc-0.1.3/fastmvc/templates/scaffold_helpers/user_login.html
+-rw-r--r--   0        0        0      261 2023-02-26 15:03:48.395485 fastmvc-0.1.3/fastmvc/templates/scaffold_helpers/wysiwyg.html
+-rw-r--r--   0        0        0     2529 2023-03-01 13:33:29.248691 fastmvc-0.1.3/fastmvc/templates/users/model.py
+-rw-r--r--   0        0        0     3241 2023-02-26 14:45:44.598398 fastmvc-0.1.3/fastmvc/templates/users/router.py
+-rw-r--r--   0        0        0      604 2023-02-26 15:06:44.370207 fastmvc-0.1.3/fastmvc/templates/users/templates/dashboard.html
+-rw-r--r--   0        0        0     2088 2023-02-26 15:07:35.756143 fastmvc-0.1.3/fastmvc/templates/users/templates/login.html
+-rw-r--r--   0        0        0      670 2023-02-26 14:39:07.527008 fastmvc-0.1.3/fastmvc/templates/users/templates/not_authenticated.html
+-rw-r--r--   0        0        0     3254 2023-02-26 15:07:28.995215 fastmvc-0.1.3/fastmvc/templates/users/templates/signup.html
+-rw-r--r--   0        0        0     3694 2023-02-26 15:08:27.822779 fastmvc-0.1.3/fastmvc/templates/users/utils.py
+-rw-r--r--   0        0        0       27 2022-06-02 02:11:06.000000 fastmvc-0.1.3/fastmvc/user_config.json
+-rw-r--r--   0        0        0     1166 2023-07-09 15:19:24.455152 fastmvc-0.1.3/fastmvc/utilities.py
+-rw-r--r--   0        0        0     1083 2022-10-28 02:06:58.000000 fastmvc-0.1.3/LICENSE
+-rw-r--r--   0        0        0      604 2023-07-08 22:11:13.602211 fastmvc-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1280 2023-03-07 00:39:21.692090 fastmvc-0.1.3/README.md
+-rw-r--r--   0        0        0     2724 1970-01-01 00:00:00.000000 fastmvc-0.1.3/setup.py
+-rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 fastmvc-0.1.3/PKG-INFO
```

### Comparing `fastmvc-0.1.2/fastmvc/extras/flickr.py` & `fastmvc-0.1.3/fastmvc/extras/flickr.py`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/generator.py` & `fastmvc-0.1.3/fastmvc/generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,56 +8,56 @@
 
 """
 HELPERS
 """
 
 
 def __builder(
-    project_path: str, 
-    generator_path:str, 
-    format_attrs: dict, 
+    project_path: str,
+    generator_path:str,
+    format_attrs: dict,
     scaffold_obj_name='',
     ignore_list: list or None = None
 ) -> None:
     """Build a project scaffold from a generator template.
-    
+
     Args:
-        project_path (str): The path to the directory where the project scaffold should be created.  
-        generator_path (str): The path to the directory containing the generator template files.  
-        format_attrs (dict): A dictionary of attributes to be used in formatting the generator template files.  
-        scaffold_obj_name (str, optional): The name of the object being scaffolded. Defaults to an empty string.  
+        project_path (str): The path to the directory where the project scaffold should be created.
+        generator_path (str): The path to the directory containing the generator template files.
+        format_attrs (dict): A dictionary of attributes to be used in formatting the generator template files.
+        scaffold_obj_name (str, optional): The name of the object being scaffolded. Defaults to an empty string.
     """
     project_path = Path(project_path)
     generator_path = Path(__file__).parent.resolve() / generator_path
     for (dirpath, _, filenames) in walk(generator_path):
-        np = (Path(scaffold_obj_name) / project_path 
+        np = (Path(scaffold_obj_name) / project_path
               if scaffold_obj_name else project_path)
         new_path = dirpath.replace(str(generator_path), str(np))
         if '__pycache__' in str(dirpath):
             continue
         makedirs(new_path, exist_ok=True)
         for filename in filenames:
             if any([filename in igf for igf in ignore_list or list()]):
                 continue
             full_path = Path(dirpath) / filename
             print(f">> {Path(new_path) / filename}")
             with open(full_path, 'r') as c:
-                content = c.read()          
-            
+                content = c.read()
+
             with open(Path(new_path) / filename, 'w+') as o:
                 o.write(__format(content, format_attrs))
 
 
 def __format(doc: str, attr_dict: dict) -> str:
     """Format a document with the specified attribute dictionary.
-    
+
     Args:
-        doc (str): The document to be formatted.  
-        attr_dict (dict): A dictionary of attributes to be used in the formatting.  
-        
+        doc (str): The document to be formatted.
+        attr_dict (dict): A dictionary of attributes to be used in the formatting.
+
     Returns:
         str: The formatted string.
     """
     env = Environment(
         variable_start_string='^{',
         variable_end_string='}^',
         block_start_string='^%',
@@ -66,54 +66,54 @@
         lstrip_blocks=True)
     template = env.from_string(doc)
     return template.render(**attr_dict)
 
 
 def __get_object_attrs(attributes: list) -> dict:
     """Get a dictionary of object attributes from a list of attribute strings.
-    
+
     Args:
-        attributes (list): A list of strings representing object attributes in the form "name:type".  
-        
+        attributes (list): A list of strings representing object attributes in the form "name:type".
+
     Returns:
-        dict: A dictionary of object attributes, 
+        dict: A dictionary of object attributes,
             where the keys are the attribute names and the values are the attribute types.
     """
     obj_attrs = dict()
     for a in attributes:
         if not a:
             continue
         s = a.split(':')
         obj_attrs[s[0]] = 'str' if len(s) == 1 else s[1].lower()
     return obj_attrs
 
 
 def __prepare_model_attrs(obj_attrs: dict) -> str:
-    """Provides attributes for the DetaModel  
+    """Provides attributes for the DetaModel
 
     Args:
-        obj_attrs (dict): attributes dictionary  
+        obj_attrs (dict): attributes dictionary
 
     Returns:
         str: prepared attributes as string
     """
     model_attrs = [
-        f"{k}: {'str' if v in ('text', 'wysiwyg') else v}" 
+        f"{k}: {'str' if v in ('text', 'wysiwyg') else v}"
         for k, v in obj_attrs.items()]
     return '\n    '.join(model_attrs)
 
 
 def __create_form_attrs(attributes: dict, helpers_path: str) -> str:
-    """Create form field HTML for the specified attributes.  
-    
+    """Create form field HTML for the specified attributes.
+
     Args:
-        attributes (dict): A dictionary of form field attributes, 
-            where the keys are the field names and the values are the field types.   
-        helpers_path (str): The path to the directory containing form field helper templates.  
-        
+        attributes (dict): A dictionary of form field attributes,
+            where the keys are the field names and the values are the field types.
+        helpers_path (str): The path to the directory containing form field helper templates.
+
     Returns:
         str: The HTML for the form fields.
     """
     helpers_path = Path(__file__).parent.resolve() / helpers_path
     form_fields = list()
     for f, t in attributes.items():
         field_helper = helpers_path / f'{t}.html'
@@ -124,70 +124,70 @@
         format_attrs = {'f': f, 'F': f.title()}
         form_fields.append(__format(content, format_attrs))
     return '\n'.join(form_fields)
 
 
 def __add_wysiwyg_meta(take_action: bool):
     if take_action:
-        with open(Path(__file__).parent.resolve() 
-                  / 'templates/scaffold_helpers/trix_meta_content.html', 
+        with open(Path(__file__).parent.resolve()
+                  / 'templates/scaffold_helpers/trix_meta_content.html',
                   'r') as o:
             return o.read()
 
 
 def __get_import_placement(main_py: list) -> int:
-    """Get the index at which to insert an import statement in the main Python script.  
-    
+    """Get the index at which to insert an import statement in the main Python script.
+
     Args:
-        main_py (list): A list of lines in the main Python script.  
-        
+        main_py (list): A list of lines in the main Python script.
+
     Returns:
-        int: The index at which to insert an import statement.  
+        int: The index at which to insert an import statement.
     """
     imp_placement = 0
     for i, line in enumerate(main_py):
         if '_router' in line and 'import' in line:
             imp_placement = i + 1
     return imp_placement
 
 
 """
 GENERATORS
 """
 
 
 def build_base(p: str, project_name: str, platform: Platform) -> None:
-    """Builds a base for the new project.  
+    """Builds a base for the new project.
 
-    Currently supports two platforms: Google App Engine and Deta.  
-    See templates/core/ or templates/mkdocs_core/ to see the files 
+    Currently supports two platforms: Google App Engine and Deta.
+    See templates/core/ or templates/mkdocs_core/ to see the files
     which will be generated through the `__builder` method
 
     Args:
-        p (str): the current working directory  
-        project_name (str): name of the new project  
-        platform (Platform): platform to build for.  
+        p (str): the current working directory
+        project_name (str): name of the new project
+        platform (Platform): platform to build for.
     """
     makedirs(p)
     content_attrs = {
         'Obj': project_name.title(),
         'project_key': config('project_key') or '',
         'platform': platform.name }
 
     ignore_list = list()
     if platform != Platform.GOOGLE_APP_ENGINE:
         ignore_list.append('app.yaml')
         ignore_list.append('service-account-file.json')
 
     __builder(
-        project_path=p, 
-        generator_path=f'templates/core', 
+        project_path=p,
+        generator_path=f'templates/core',
         format_attrs=content_attrs,
         ignore_list=ignore_list)
-    
+
 
 def __build_platform_specific_info():
     platform = dict()
     plat = get_project_platform()
     if plat == Platform.DETA:
         platform = {
             'data_model_import': 'deta import DetaBase',
@@ -199,195 +199,197 @@
             'data_model': 'Firestore'
         }
     return platform
 
 
 
 def gen_scaffold(p: str, obj: str, attributes: list) -> None:
-    """Generates Model, View, and Controller for a new Object.  
+    """Generates Model, View, and Controller for a new Object.
 
     Args:
-        p (str): the current working directory  
-        obj (str): the name of the new object to be created  
+        p (str): the current working directory
+        obj (str): the name of the new object to be created
         attributes (list): the attributes of the new object
     """
     obj_attrs = __get_object_attrs(attributes)
     format_attrs = {
         'proj': Path.cwd().name,
-        'obj': obj, 
-        'Obj': obj.title(), 
-        'model_attrs': __prepare_model_attrs(obj_attrs), 
+        'obj': obj,
+        'Obj': obj.title(),
+        'model_attrs': __prepare_model_attrs(obj_attrs),
         'form_attrs': __create_form_attrs(
-            attributes=obj_attrs, 
+            attributes=obj_attrs,
             helpers_path='templates/scaffold_helpers'),
         'wysiwyg': __add_wysiwyg_meta('wysiwyg' in obj_attrs.values()),
         'platform': __build_platform_specific_info()}
-    
+
     __builder(
-        project_path=p, 
-        generator_path='templates/scaffold', 
+        project_path=p,
+        generator_path='templates/scaffold',
         format_attrs=format_attrs,
         scaffold_obj_name=obj)
     update(add_to_main(p, obj))
 
-    with open(Path(__file__).parent.resolve() 
-              / 'templates/scaffold_helpers/scaffold_navlink.html', 
+    with open(Path(__file__).parent.resolve()
+              / 'templates/scaffold_helpers/scaffold_navlink.html',
               'r') as o:
         scaffold_link = __format(o.read(), format_attrs)
 
     update(add_to_navlinks(
         p,
         content=scaffold_link))
 
 
 def gen_authlib(p: str) -> None:
     """Generates a minimal authorization framework.
 
     Based on AuthLib library, the generate authorization framework
-    allows users to login with Google. See AuthLib library for 
-    other potential Open ID providers.  
+    allows users to login with Google. See AuthLib library for
+    other potential Open ID providers.
 
     Args:
-        p (str): the current working directory  
-    """   
+        p (str): the current working directory
+    """
     obj = 'user'
     format_attrs = {
         'proj': Path.cwd().name,
-        'obj': obj, 
+        'obj': obj,
         'Obj': obj.title(),
         'platform': __build_platform_specific_info() }
 
     __builder(
-        project_path=p, 
-        generator_path='templates/users', 
+        project_path=p,
+        generator_path='templates/users',
         format_attrs=format_attrs,
         scaffold_obj_name=obj)
     update(add_to_main(
-        p, 
-        obj, 
+        p,
+        obj,
         extra_imports=[
             'from starlette.middleware.sessions import SessionMiddleware\n',
             'from os import environ\n'],
         extra_includes=[
             '\napp.add_middleware(SessionMiddleware, secret_key=environ.get("APP_SECRET"))']))
     update(add_to_requirements(
         p,
         reqs=['itsdangerous', 'httpx', 'Authlib', 'pyjwt', 'passlib[bcrypt]']))
     update(add_to_env(
         p,
         APP_SECRET=format_attrs['proj'][0] + token_urlsafe(16),
         GOOGLE_CLIENT_ID="",
         GOOGLE_CLIENT_SECRET=""))
-    
+
     with open(Path(__file__).parent.resolve() / 'templates/scaffold_helpers/user_login.html', 'r') as o:
         user_links = o.read()
 
     update(add_to_navlinks(
         p,
         content=user_links))
 
 
 """
 UPDATERS
 """
-@dataclass 
+@dataclass
 class File:
-    filepath: str 
+    filepath: str
     content: str
     mode: str = 'w'
 
 
 def update(file: File):
-    with open(file.filepath, file.mode) as m:
-        m.write(file.content)
+    if file:
+        with open(file.filepath, file.mode) as m:
+            m.write(file.content)
 
 
 def add_to_main(
-    p: str, 
+    p: str,
     name: str,
-    extra_imports: list or None = None, 
+    extra_imports: list or None = None,
     extra_includes: list or None = None
 ) -> File:
-    """Adds provided data to the main router with the scaffold router imports.  
+    """Adds provided data to the main router with the scaffold router imports.
 
     When a new scaffolded MVC is added to the project, the router for
-    it should be added to main.py. This method will import the router 
+    it should be added to main.py. This method will import the router
     and include the router in the main `app`, along with the appropriate
-    prefix. Extra imports and app additions may be appended as well.  
+    prefix. Extra imports and app additions may be appended as well.
 
     Args:
-        p (str): The path to the directory containing the main file.  
-        name (str): name of the router to include.  
-        extra_imports (listorNone, optional): additional imports to include. Defaults to None.  
+        p (str): The path to the directory containing the main file.
+        name (str): name of the router to include.
+        extra_imports (listorNone, optional): additional imports to include. Defaults to None.
         extra_includes (listorNone, optional): additional lines of code to include. Defaults to None.
-    
+
     Return:
         File: the updated file and metadata
     """
     main_file = Path(p) / 'main.py'
     with open(main_file, 'r') as m:
         main = m.readlines()
     imprt = [f'from {name}.router import {name}_router\n']
     incld = [f'\napp.include_router({name}_router, tags=["{name}"], prefix="/{name}")']
     imprt += extra_imports or list()
     incld += extra_includes or list()
     main.insert(
-        __get_import_placement(main), 
+        __get_import_placement(main),
         ''.join(imprt))
     main.append(''.join(incld))
     return File(
-        filepath=main_file, 
-        content=''.join(main), 
+        filepath=main_file,
+        content=''.join(main),
         mode='w')
 
 
 def add_to_requirements(p: str, reqs: list) -> File:
-    """Adds provided data to the requirements file at the specified path with the provided requirements.  
+    """Adds provided data to the requirements file at the specified path with the provided requirements.
 
     Args:
-        p (str): The path to the directory containing the requirements file.  
-        reqs (list): A list of requirements to be added to the requirements 
-        
+        p (str): The path to the directory containing the requirements file.
+        reqs (list): A list of requirements to be added to the requirements
+
     Return:
         File: the updated file and metadata
     """
     req_file = Path(p) / 'requirements.txt'
     with open(req_file, 'r') as m:
         file_reqs = m.readlines()
-    
+
     file_reqs.insert(0, '\n'.join(reqs) + '\n')
     return File(
-        filepath=req_file, 
-        content=''.join(file_reqs), 
+        filepath=req_file,
+        content=''.join(file_reqs),
         mode='w')
 
 
 def add_to_env(p: str, **kwargs) -> File:
-    """Adds provided data to the env file at the specified path with the provided variables.  
+    """Adds provided data to the env file at the specified path with the provided variables.
 
     Args:
-        p (str): The path to the directory containing the env file.  
-        kwargs: key and value for each entry 
-        
+        p (str): The path to the directory containing the env file.
+        kwargs: key and value for each entry
+
     Return:
         File: the updated file and metadata
     """
     env_file = Path(p) / '.env'
     with open(env_file, 'r') as e:
         file_env = e.readlines()
     file_env += [
         f"{k}={v}"
         for k, v in kwargs.items()]
     return File(
-        filepath=env_file, 
-        content='\n'.join(file_env) + '\n', 
+        filepath=env_file,
+        content='\n'.join(file_env) + '\n',
         mode='w')
 
 
 def add_to_navlinks(p: str, content: str):
     navlink_file = Path(p) / 'static_pages' / 'templates' / '_navlinks.html'
-    with open(navlink_file, 'r') as e:
-        file_navlink = e.read()
-    return File(
-        filepath=navlink_file,
-        content=file_navlink + '\n\n' + content,
-        mode='w')
+    if Path.exists(navlink_file):
+        with open(navlink_file, 'r') as e:
+            file_navlink = e.read()
+        return File(
+            filepath=navlink_file,
+            content=file_navlink + '\n\n' + content,
+            mode='w')
```

### Comparing `fastmvc-0.1.2/fastmvc/main.py` & `fastmvc-0.1.3/fastmvc/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,23 +32,23 @@
 
 @app.command()
 def new(project: str, platform: str or None = None):
     """ create a new project """
     plat = __choose_platform(platform)
     if not plat:
         return
-    
+
     new_folder = os.path.join(os.curdir, project)
-    try:      
+    try:
         typer.secho(f"\nBuilding new project: {project}\n", fg='green')
         build_base(new_folder, project, plat)
         typer.echo(f"\n{project} was created.\n")
     except FileExistsError:
         typer.secho(f"'{project}' already exists in this folder.\n", fg='red')
-    
+
 
 @app.command()
 def server():
     """ run the app locally """
     utils.run_server()
 
 
@@ -89,7 +89,18 @@
 
 
 @app.command()
 def view_config():
     """ view your development configurations """
     conf = utils.config()
     typer.echo(conf)
+
+
+@app.command()
+def help(subject: str):
+    if subject == 'gcloud':
+        typer.echo("""
+        GCLOUD COMMANDS:\n
+        gcloud init              -- choose your configuration file for gcloud
+        gcloud app create        -- create a new app in configured gcloud
+        gcloud app deploy        -- upload files and create a new version of app in cloud.
+        """)
```

### Comparing `fastmvc-0.1.2/fastmvc/models/database/_base.py` & `fastmvc-0.1.3/fastmvc/models/database/_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,63 @@
 import pydantic
 import re
 
 
-class DBModelMetaClass(pydantic.main.ModelMetaclass):
+class DBModelMetaClass(pydantic.main._model_construction.ModelMetaclass):
     def __new__(mcs, name, bases, dct):
         cls = super().__new__(mcs, name, bases, dct)
-        cls.Config.arbitrary_types_allowed = True  # but, be careful if you use them!
-        if getattr(cls.Config, "table_name", None):
-            cls.__db_name__ = cls.Config.table_name
-        else:
-            cls.__db_name__ = re.sub(r"(?<!^)(?=[A-Z])", "_", name).lower()
+        cls.model_config['arbitrary_types_allowed'] = True   # but, be careful if you use them!
+        cls.__db_name__ = cls.model_config.get(
+            'table_name',
+            re.sub(r"(?<!^)(?=[A-Z])", "_", name).lower())
+
         cls._db = None
 
         for name, field in cls.__fields__.items():
             setattr(cls, name, field)
         return cls
 
     @property
     def __db__(cls):
         return cls.handle_db_property(cls)
 
     @staticmethod
     def handle_db_property(cls):
         """Return the database client with model collection"""
         pass
-    
+
 
 class BaseDataModel(pydantic.BaseModel):
 
-    key: str = None
-    
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.key = self.key or None    
+        self.key = self.key or None
 
-    @classmethod 
+    @classmethod
     def db(cls):
         return cls.__db__
 
     @classmethod
     def get(cls, key):
         pass
-    
+
     @classmethod
     def get_all(cls):
         pass
-    
+
     @classmethod
     def delete_key(cls, key):
         pass
 
-    @classmethod 
+    @classmethod
     def query(cls, statement):
         pass
 
     def update(self, update_data: dict):
         pass
-    
+
     def save(self):
         pass
-    
+
     def get_attribute_value(self, index=1):
         d = self.__dict__
         return list(d.values())[index]
```

### Comparing `fastmvc-0.1.2/fastmvc/models/database/deta.py` & `fastmvc-0.1.3/fastmvc/models/database/deta.py`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/models/database/firestore.py` & `fastmvc-0.1.3/fastmvc/models/database/firestore.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,65 +6,65 @@
 
     @staticmethod
     def handle_db_property(cls):
         if cls._db:
             return cls._db
         cls._db = firestore.Client().collection(cls.__db_name__)
         return cls._db
-    
+
 
 class Firestore(BaseDataModel, metaclass=FirestoreModelMeta):
-    
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     @classmethod
     def __parsed(cls, record):
         r = record.to_dict()
         r.update({'key': record.id})
-        return cls.parse_obj(r)
+        return cls.model_validate(r)
 
     @classmethod
     def get(cls, key):
         doc_ref = cls.__db__.document(key)
         doc = doc_ref.get()
         if doc.exists:
             return cls.__parsed(doc)
         else:
             return None
-    
+
     @classmethod
     def get_all(cls):
         for record in cls.__db__.get():
             yield cls.__parsed(record)
-    
+
     @classmethod
     def delete_key(cls, key):
         cls.__db__.document(key).delete()
 
-    @classmethod 
+    @classmethod
     def query(cls, statement: dict):
         query = cls.__db__
         for k, v in statement.items():
             query = query.where(k, '==', v)
         for record in query.stream():
             yield cls.__parsed(record)
-            
+
     @classmethod
     def _edit(cls, key, data):
         doc_ref = cls.__db__.document(key)
         return doc_ref.update(data)
 
     def update(self, update_data: dict):
         result = self._edit(key=self.key, data=update_data)
 
-    @classmethod 
+    @classmethod
     def _put(cls, key, data):
         doc_ref = cls.__db__.document(key)
         doc_ref.set(data)
         return doc_ref.id
-    
+
     def save(self):
         data = self.dict()
         key = data.pop('key', None)
         new_doc_id = self._put(key, data)
         self.key = new_doc_id
```

### Comparing `fastmvc-0.1.2/fastmvc/templates/core/ignore/service-account-file.json` & `fastmvc-0.1.3/fastmvc/templates/core/ignore/service-account-file.json`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/core/static_pages/static/css/core.css` & `fastmvc-0.1.3/fastmvc/templates/core/static_pages/static/css/core.css`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/core/static_pages/static/img/logo.svg` & `fastmvc-0.1.3/fastmvc/templates/core/static_pages/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/core/static_pages/static/js/color-modes.js` & `fastmvc-0.1.3/fastmvc/templates/core/static_pages/static/js/color-modes.js`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/core/static_pages/templates/_base.html` & `fastmvc-0.1.3/fastmvc/templates/core/static_pages/templates/_base.html`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width,initial-scale=1">
     <link rel="icon" href="{{ url_for('static', path='/img/logo.svg') }}" />
     <meta name="theme-color" content="#ffffff">
     <title>{% block page_title %}{% endblock %}^{Obj}^</title>
     <meta name="robots" content="{% block meta_robots %}index, follow{% endblock %}">
-    <meta name="description" content="{% block meta_description %}^{Obj}^ was built with DetaMVC - the fastest way to get to production!{% endblock %}">
+    <meta name="description" content="{% block meta_description %}^{Obj}^ was built with FastMVC - the fastest way to get to production!{% endblock %}">
     <meta property="og:url" content="{{ request.url }}">
     <meta property="og:title" content="{{ self.page_title() }}">
     <meta property="og:description" content="{{ self.meta_description() }}">
     <meta property="og:image" content="{% block meta_shared_image %}{{ url_for('static', path='/img/logo.svg') }}{% endblock %}">
     <meta name="twitter:card" content="summary_large_image">
     <link rel="canonical" href="{{ request.url }}">
 
@@ -21,29 +21,29 @@
     {% block meta_additions %}{% endblock %}
   </head>
   <body>
     {% include 'static_pages/templates/_svg_symbols.html' %}
 
     <header class="navbar navbar-expand-lg dmvc-navbar sticky-top">
       <nav aria-label="Main navigation" class="container-xxl flex-wrap flex-lg-nowrap">
-  
+
           <a class="navbar-brand p-0 me-0 me-lg-2" href="/">
               <img height="40"  class="me-2" src="{{ url_for('static', path='/img/logo.svg') }}">
               <span class="align-middle">^{Obj}^</span>
           </a>
-  
+
           <button aria-controls="dmvcNavbar" aria-label="Toggle navigation"
                   class="navbar-toggler d-flex d-lg-none order-3 p-2" data-bs-target="#dmvcNavbar"
                   data-bs-toggle="offcanvas" type="button">
               <svg class="bi" height="24"width="24" xmlns="http://www.w3.org/2000/svg">
                   <use href="#sandwich">
                   </use>
               </svg>
           </button>
-  
+
           <div aria-labelledby="dmvcNavbarOffcanvasLabel" class="offcanvas-lg offcanvas-end flex-grow-1"
                data-bs-scroll="true" id="dmvcNavbar" tabindex="-1">
               <div class="offcanvas-header px-4 pb-0">
                   <h5 class="offcanvas-title" id="dmvcNavbarOffcanvasLabel">
                   ^{Obj}^
                   </h5>
                   <button aria-label="Close" class="btn-close" type="button"
@@ -51,19 +51,19 @@
                   </button>
               </div>
               <div class="offcanvas-body p-4 pt-0 p-lg-0 justify-content-end">
                   <hr class="d-lg-none"/>
                   <ul class="navbar-nav flex-row flex-wrap">
                       {% include 'static_pages/templates/_navlinks.html' %}
                   </ul>
-  
+
                   {% include 'static_pages/templates/_color_mode.html' %}
               </div>
           </div>
-  
+
       </nav>
     </header>
 
     {% if alert %}
     <div class="alert alert-{{alert.type or 'danger'}} alert-dismissible fade show" role="alert">
         {{ alert.message | safe or alert | safe }}
         <button type="button" class="btn-close" data-bs-dismiss="alert" aria-label="Close"></button>
@@ -72,8 +72,8 @@
 
     {% block content %}
     {% endblock %}
 
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/js/bootstrap.bundle.min.js" crossorigin="anonymous"></script>
     <script src="{{ url_for('static', path='/js/application.js?v=1.0.0') }}"></script>
   </body>
-</html>
+</html>
```

### Comparing `fastmvc-0.1.2/fastmvc/templates/core/static_pages/templates/_color_mode.html` & `fastmvc-0.1.3/fastmvc/templates/core/static_pages/templates/_color_mode.html`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/core/static_pages/templates/_svg_symbols.html` & `fastmvc-0.1.3/fastmvc/templates/core/static_pages/templates/_svg_symbols.html`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/core/static_pages/templates/index.html` & `fastmvc-0.1.3/fastmvc/templates/core/static_pages/templates/index.html`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/scaffold/router.py` & `fastmvc-0.1.3/fastmvc/templates/scaffold/router.py`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/scaffold/templates/form.html` & `fastmvc-0.1.3/fastmvc/templates/scaffold/templates/form.html`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/scaffold/templates/index.html` & `fastmvc-0.1.3/fastmvc/templates/scaffold/templates/index.html`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/scaffold/templates/view.html` & `fastmvc-0.1.3/fastmvc/templates/scaffold/templates/view.html`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/scaffold_helpers/user_login.html` & `fastmvc-0.1.3/fastmvc/templates/scaffold_helpers/user_login.html`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/users/model.py` & `fastmvc-0.1.3/fastmvc/templates/users/model.py`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/users/router.py` & `fastmvc-0.1.3/fastmvc/templates/users/router.py`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/users/templates/dashboard.html` & `fastmvc-0.1.3/fastmvc/templates/users/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/users/templates/login.html` & `fastmvc-0.1.3/fastmvc/templates/users/templates/login.html`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/users/templates/not_authenticated.html` & `fastmvc-0.1.3/fastmvc/templates/users/templates/not_authenticated.html`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/users/templates/signup.html` & `fastmvc-0.1.3/fastmvc/templates/users/templates/signup.html`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/templates/users/utils.py` & `fastmvc-0.1.3/fastmvc/templates/users/utils.py`

 * *Files identical despite different names*

### Comparing `fastmvc-0.1.2/fastmvc/utilities.py` & `fastmvc-0.1.3/fastmvc/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import json 
+import json
 from pathlib import Path
 import os
 import enum
 
 CONFIG_PATH = Path(__file__).parent.resolve() / 'user_config.json'
 
 
@@ -29,15 +29,15 @@
 def __fetch_config():
     with open(CONFIG_PATH, 'r') as j:
         return json.loads(j.read())
 
 
 def set_project_key(project_key: str):
     conf = __fetch_config()
-    conf['project_key'] = project_key 
+    conf['project_key'] = project_key
     with open(CONFIG_PATH, 'w') as j:
         j.write(json.dumps(conf, indent=4))
 
 
 def clear_project_key():
     set_project_key("")
```

### Comparing `fastmvc-0.1.2/pyproject.toml` & `fastmvc-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "FastMVC"
-version = "0.1.2"
+version = "0.1.3"
 description = "Rapid application development built for the cloud."
 authors = ["MBeebe <pyn-sol@beebe.dev>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 fastmvc = "fastmvc.main:app"
```

### Comparing `fastmvc-0.1.2/README.md` & `fastmvc-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ![FastMVC](https://live.staticflickr.com/65535/52719951542_f745d984cc_o.png)  
 
 # FastMVC
-FastMVC is a modern, fast (high-performance), web framework for building Web Applications
+FastMVC is a web framework for building Web Applications
 with the MVC structure (Model - View - Controller) and effortlessly deploying them to cloud platforms. 
 
 - Model is interchangeable depending on the cloud platform you would like to use.
 - View uses Jinja2 to create front end pages
 - Controller is written using FastAPI
```

### Comparing `fastmvc-0.1.2/setup.py` & `fastmvc-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,17 @@
  'typer[all]']
 
 entry_points = \
 {'console_scripts': ['fastmvc = fastmvc.main:app']}
 
 setup_kwargs = {
     'name': 'fastmvc',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'Rapid application development built for the cloud.',
-    'long_description': '![FastMVC](https://live.staticflickr.com/65535/52719951542_f745d984cc_o.png)  \n\n# FastMVC\nFastMVC is a modern, fast (high-performance), web framework for building Web Applications\nwith the MVC structure (Model - View - Controller) and effortlessly deploying them to cloud platforms. \n\n- Model is interchangeable depending on the cloud platform you would like to use.\n- View uses Jinja2 to create front end pages\n- Controller is written using FastAPI\n\n\n## FastMVC CLI\n`fastmvc new [PROJECT_NAME]`  \nCreates a new project. Will ask which platform to build towards (GOOGLE_APP_ENGINE, or DETA) and set up the base of the project accordingly.  \n\nOptionally, you can pass the flag `--platform` and provide one of the options above.  \n\n`fastmvc scaffold [MODEL_NAME] [ATTRIBUTE]:[DATA_TYPE]`  \nScaffold out a Model, View, and Controller for your object. For example:  \n\nfastmvc scaffold post title:str content:wysiwyg draft:bool  \n\n`fastmvc auth`  \nBuilds an Authentication Framework to easily integrate user sign in for your application.  \n\n`fastmvc s`  \nAlias for `uvicorn main:app --reload` to run your application locally  \n\n## Supported Cloud Platforms\n__Built__\n- Google App Engine (using Firestore database)\n- Deta (using DetaBase)\n\n__Coming Soon__\n- AWS Elastic Beanstalk\n\n\n',
+    'long_description': '![FastMVC](https://live.staticflickr.com/65535/52719951542_f745d984cc_o.png)  \n\n# FastMVC\nFastMVC is a web framework for building Web Applications\nwith the MVC structure (Model - View - Controller) and effortlessly deploying them to cloud platforms. \n\n- Model is interchangeable depending on the cloud platform you would like to use.\n- View uses Jinja2 to create front end pages\n- Controller is written using FastAPI\n\n\n## FastMVC CLI\n`fastmvc new [PROJECT_NAME]`  \nCreates a new project. Will ask which platform to build towards (GOOGLE_APP_ENGINE, or DETA) and set up the base of the project accordingly.  \n\nOptionally, you can pass the flag `--platform` and provide one of the options above.  \n\n`fastmvc scaffold [MODEL_NAME] [ATTRIBUTE]:[DATA_TYPE]`  \nScaffold out a Model, View, and Controller for your object. For example:  \n\nfastmvc scaffold post title:str content:wysiwyg draft:bool  \n\n`fastmvc auth`  \nBuilds an Authentication Framework to easily integrate user sign in for your application.  \n\n`fastmvc s`  \nAlias for `uvicorn main:app --reload` to run your application locally  \n\n## Supported Cloud Platforms\n__Built__\n- Google App Engine (using Firestore database)\n- Deta (using DetaBase)\n\n__Coming Soon__\n- AWS Elastic Beanstalk\n\n\n',
     'author': 'MBeebe',
     'author_email': 'pyn-sol@beebe.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fastmvc-0.1.2/PKG-INFO` & `fastmvc-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmvc
-Version: 0.1.2
+Version: 0.1.3
 Summary: Rapid application development built for the cloud.
 Author: MBeebe
 Author-email: pyn-sol@beebe.dev
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,15 +22,15 @@
 Requires-Dist: python-multipart
 Requires-Dist: typer[all]
 Description-Content-Type: text/markdown
 
 ![FastMVC](https://live.staticflickr.com/65535/52719951542_f745d984cc_o.png)  
 
 # FastMVC
-FastMVC is a modern, fast (high-performance), web framework for building Web Applications
+FastMVC is a web framework for building Web Applications
 with the MVC structure (Model - View - Controller) and effortlessly deploying them to cloud platforms. 
 
 - Model is interchangeable depending on the cloud platform you would like to use.
 - View uses Jinja2 to create front end pages
 - Controller is written using FastAPI
```

