# Comparing `tmp/django-qoptions-0.1.7.tar.gz` & `tmp/django-qoptions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-qoptions-0.1.7.tar", last modified: Wed Jun 12 10:42:52 2019, max compression
+gzip compressed data, was "django-qoptions-0.2.0.tar", last modified: Sun Jul  9 08:17:54 2023, max compression
```

## Comparing `django-qoptions-0.1.7.tar` & `django-qoptions-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/
--rw-rw-r--   0 vital     (1000) vital     (1000)       35 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/MANIFEST.in
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/django_qoptions.egg-info/
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2019-06-12 10:42:29.000000 django-qoptions-0.1.7/django_qoptions.egg-info/not-zip-safe
--rw-rw-r--   0 vital     (1000) vital     (1000)      828 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/django_qoptions.egg-info/PKG-INFO
--rw-rw-r--   0 vital     (1000) vital     (1000)      646 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/django_qoptions.egg-info/SOURCES.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        1 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/django_qoptions.egg-info/dependency_links.txt
--rw-rw-r--   0 vital     (1000) vital     (1000)        8 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/django_qoptions.egg-info/top_level.txt
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/options/
--rw-rw-r--   0 vital     (1000) vital     (1000)     2791 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/models.py
--rw-rw-r--   0 vital     (1000) vital     (1000)        0 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)       98 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/options_settings.py
--rwxrwxr-x   0 vital     (1000) vital     (1000)     2115 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/admin.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/options/templatetags/
--rw-rw-r--   0 vital     (1000) vital     (1000)     2496 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/templatetags/options.py
--rw-rw-r--   0 vital     (1000) vital     (1000)       75 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/templatetags/__init__.py
--rw-rw-r--   0 vital     (1000) vital     (1000)     1772 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/functions.py
--rw-rw-r--   0 vital     (1000) vital     (1000)      373 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/translation.py
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/options/locale/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/options/locale/ru/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/options/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 vital     (1000) vital     (1000)      843 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 vital     (1000) vital     (1000)     1208 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/options/locale/en/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/options/locale/en/LC_MESSAGES/
--rw-rw-r--   0 vital     (1000) vital     (1000)      508 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 vital     (1000) vital     (1000)      982 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/options/locale/lv/
-drwxrwxr-x   0 vital     (1000) vital     (1000)        0 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/options/locale/lv/LC_MESSAGES/
--rw-rw-r--   0 vital     (1000) vital     (1000)      594 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/locale/lv/LC_MESSAGES/django.mo
--rw-rw-r--   0 vital     (1000) vital     (1000)     1075 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/options/locale/lv/LC_MESSAGES/django.po
--rw-rw-r--   0 vital     (1000) vital     (1000)     1115 2019-06-12 10:41:55.000000 django-qoptions-0.1.7/setup.py
--rw-rw-r--   0 vital     (1000) vital     (1000)       59 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/setup.cfg
--rw-rw-r--   0 vital     (1000) vital     (1000)      828 2019-06-12 10:42:52.000000 django-qoptions-0.1.7/PKG-INFO
+drwxr-xr-x   0 vital     (1000) vital     (1000)        0 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/
+-rw-r--r--   0 vital     (1000) vital     (1000)       35 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/MANIFEST.in
+-rw-r--r--   0 vital     (1000) vital     (1000)      815 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/PKG-INFO
+-rw-r--r--   0 vital     (1000) vital     (1000)     1987 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/README.md
+drwxr-xr-x   0 vital     (1000) vital     (1000)        0 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/django_qoptions.egg-info/
+-rw-r--r--   0 vital     (1000) vital     (1000)      815 2023-07-09 08:17:54.000000 django-qoptions-0.2.0/django_qoptions.egg-info/PKG-INFO
+-rw-r--r--   0 vital     (1000) vital     (1000)      656 2023-07-09 08:17:54.000000 django-qoptions-0.2.0/django_qoptions.egg-info/SOURCES.txt
+-rw-r--r--   0 vital     (1000) vital     (1000)        1 2023-07-09 08:17:54.000000 django-qoptions-0.2.0/django_qoptions.egg-info/dependency_links.txt
+-rw-r--r--   0 vital     (1000) vital     (1000)        1 2023-07-09 08:17:54.000000 django-qoptions-0.2.0/django_qoptions.egg-info/not-zip-safe
+-rw-r--r--   0 vital     (1000) vital     (1000)        8 2023-07-09 08:17:54.000000 django-qoptions-0.2.0/django_qoptions.egg-info/top_level.txt
+drwxr-xr-x   0 vital     (1000) vital     (1000)        0 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/options/
+-rw-r--r--   0 vital     (1000) vital     (1000)        0 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/__init__.py
+-rwxr-xr-x   0 vital     (1000) vital     (1000)     2115 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/admin.py
+-rw-r--r--   0 vital     (1000) vital     (1000)     1772 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/functions.py
+drwxr-xr-x   0 vital     (1000) vital     (1000)        0 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/options/locale/
+drwxr-xr-x   0 vital     (1000) vital     (1000)        0 2023-07-09 08:17:54.296649 django-qoptions-0.2.0/options/locale/en/
+drwxr-xr-x   0 vital     (1000) vital     (1000)        0 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/options/locale/en/LC_MESSAGES/
+-rw-r--r--   0 vital     (1000) vital     (1000)      508 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 vital     (1000) vital     (1000)      982 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 vital     (1000) vital     (1000)        0 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/options/locale/lv/
+drwxr-xr-x   0 vital     (1000) vital     (1000)        0 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/options/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 vital     (1000) vital     (1000)      594 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0 vital     (1000) vital     (1000)     1075 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/locale/lv/LC_MESSAGES/django.po
+drwxr-xr-x   0 vital     (1000) vital     (1000)        0 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/options/locale/ru/
+drwxr-xr-x   0 vital     (1000) vital     (1000)        0 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/options/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 vital     (1000) vital     (1000)      843 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 vital     (1000) vital     (1000)     1208 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 vital     (1000) vital     (1000)     2790 2023-07-09 08:14:02.000000 django-qoptions-0.2.0/options/models.py
+-rw-r--r--   0 vital     (1000) vital     (1000)       98 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/options_settings.py
+drwxr-xr-x   0 vital     (1000) vital     (1000)        0 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/options/templatetags/
+-rw-r--r--   0 vital     (1000) vital     (1000)       75 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/templatetags/__init__.py
+-rw-r--r--   0 vital     (1000) vital     (1000)     2496 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/templatetags/options.py
+-rw-r--r--   0 vital     (1000) vital     (1000)      373 2023-07-09 08:12:35.000000 django-qoptions-0.2.0/options/translation.py
+-rw-r--r--   0 vital     (1000) vital     (1000)       38 2023-07-09 08:17:54.306649 django-qoptions-0.2.0/setup.cfg
+-rw-r--r--   0 vital     (1000) vital     (1000)     1113 2023-07-09 08:17:52.000000 django-qoptions-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-qoptions-0.1.7/django_qoptions.egg-info/PKG-INFO` & `django-qoptions-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-qoptions
-Version: 0.1.7
+Version: 0.2.0
 Summary: Options, Labels and standalone Texts for django admin. Administrator emails, phones, contact data, etc.
 Home-page: https://github.com/Brick85/options/
 Author: Vital Belikov
 Author-email: vital@qwe.lv
 License: New BSD
-Description: Options package allows you to create records in database, wich you can use in your templates and views.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Requires: django(>=1.3)
+Requires: django(>=4.0)
+
+Options package allows you to create records in database, wich you can use in your templates and views.
+
```

### Comparing `django-qoptions-0.1.7/django_qoptions.egg-info/SOURCES.txt` & `django-qoptions-0.2.0/django_qoptions.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 MANIFEST.in
+README.md
 setup.py
 django_qoptions.egg-info/PKG-INFO
 django_qoptions.egg-info/SOURCES.txt
 django_qoptions.egg-info/dependency_links.txt
 django_qoptions.egg-info/not-zip-safe
 django_qoptions.egg-info/top_level.txt
 options/__init__.py
```

### Comparing `django-qoptions-0.1.7/options/models.py` & `django-qoptions-0.2.0/options/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from django.utils.translation import get_language
 from django.core.cache import cache
 
 
 class OptionCache(object):
     langs_cache_key = 'qoptlangs'
```

### Comparing `django-qoptions-0.1.7/options/admin.py` & `django-qoptions-0.2.0/options/admin.py`

 * *Files identical despite different names*

### Comparing `django-qoptions-0.1.7/options/templatetags/options.py` & `django-qoptions-0.2.0/options/templatetags/options.py`

 * *Files identical despite different names*

### Comparing `django-qoptions-0.1.7/options/functions.py` & `django-qoptions-0.2.0/options/functions.py`

 * *Files identical despite different names*

### Comparing `django-qoptions-0.1.7/options/locale/ru/LC_MESSAGES/django.mo` & `django-qoptions-0.2.0/options/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-qoptions-0.1.7/options/locale/ru/LC_MESSAGES/django.po` & `django-qoptions-0.2.0/options/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-qoptions-0.1.7/options/locale/en/LC_MESSAGES/django.po` & `django-qoptions-0.2.0/options/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-qoptions-0.1.7/options/locale/lv/LC_MESSAGES/django.mo` & `django-qoptions-0.2.0/options/locale/lv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-qoptions-0.1.7/options/locale/lv/LC_MESSAGES/django.po` & `django-qoptions-0.2.0/options/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-qoptions-0.1.7/setup.py` & `django-qoptions-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(name='django-qoptions',
-      version='0.1.7',
+      version='0.2.0',
       description='Options, Labels and standalone Texts for django admin. Administrator emails, phones, contact data, etc.',
       long_description='Options package allows you to create records in database, wich you can use in your templates and views.',
       author='Vital Belikov',
       author_email='vital@qwe.lv',
       packages=['options', 'options.templatetags'],
       url='https://github.com/Brick85/options/',
       include_package_data=True,
       zip_safe=False,
-      requires=['django(>=1.3)'],
+      requires=['django(>=4.0)'],
       classifiers=['Development Status :: 5 - Production/Stable',
                    'Environment :: Web Environment',
                    'Framework :: Django',
                    'Intended Audience :: Developers',
                    'License :: OSI Approved :: BSD License',
                    'Natural Language :: English',
                    'Operating System :: Unix',
-                   'Programming Language :: Python :: 2.7',
+                   'Programming Language :: Python :: 3',
                    'Topic :: Utilities'],
       license='New BSD')
```

### Comparing `django-qoptions-0.1.7/PKG-INFO` & `django-qoptions-0.2.0/django_qoptions.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-qoptions
-Version: 0.1.7
+Version: 0.2.0
 Summary: Options, Labels and standalone Texts for django admin. Administrator emails, phones, contact data, etc.
 Home-page: https://github.com/Brick85/options/
 Author: Vital Belikov
 Author-email: vital@qwe.lv
 License: New BSD
-Description: Options package allows you to create records in database, wich you can use in your templates and views.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Utilities
-Requires: django(>=1.3)
+Requires: django(>=4.0)
+
+Options package allows you to create records in database, wich you can use in your templates and views.
+
```

