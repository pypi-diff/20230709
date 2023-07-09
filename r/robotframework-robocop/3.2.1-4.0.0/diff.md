# Comparing `tmp/robotframework-robocop-3.2.1.tar.gz` & `tmp/robotframework-robocop-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-robocop-3.2.1.tar", last modified: Fri Jun 16 15:20:37 2023, max compression
+gzip compressed data, was "robotframework-robocop-4.0.0.tar", last modified: Sun Jul  9 18:38:53 2023, max compression
```

## Comparing `robotframework-robocop-3.2.1.tar` & `robotframework-robocop-4.0.0.tar`

### file list

```diff
@@ -1,43 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:20:37.845709 robotframework-robocop-3.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-16 15:20:37.845709 robotframework-robocop-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:20:37.841709 robotframework-robocop-3.2.1/robocop/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:20:37.841709 robotframework-robocop-3.2.1/robocop/checkers/
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17339 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/duplications.py
--rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    27361 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/lengths.py
--rw-r--r--   0 runner    (1001) docker     (123)    41796 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    44284 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/naming.py
--rw-r--r--   0 runner    (1001) docker     (123)    33524 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/checkers/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    24721 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    18783 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    14683 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:20:37.845709 robotframework-robocop-3.2.1/robocop/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/disablers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/file_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12577 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/run_keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/utils/version_matching.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/robocop/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 15:20:37.845709 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-16 15:20:37.000000 robotframework-robocop-3.2.1/robotframework_robocop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 15:20:37.845709 robotframework-robocop-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-16 15:20:27.000000 robotframework-robocop-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.237940 robotframework-robocop-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-07-09 18:38:53.237940 robotframework-robocop-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12529 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.233940 robotframework-robocop-4.0.0/robocop/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.233940 robotframework-robocop-4.0.0/robocop/checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17812 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/duplications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29873 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/lengths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51778 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47251 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/naming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34167 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15657 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/checkers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25154 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.233940 robotframework-robocop-4.0.0/robocop/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/compare_runs_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/file_stats_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/json_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/return_status_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/robocop_version_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/rules_by_id_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/rules_by_severity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/sarif_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/time_taken_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/reports/timestamp_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16146 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.233940 robotframework-robocop-4.0.0/robocop/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/disablers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/file_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/run_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/utils/version_matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/robocop/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 18:38:53.237940 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14103 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-09 18:38:53.000000 robotframework-robocop-4.0.0/robotframework_robocop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 18:38:53.237940 robotframework-robocop-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-09 18:38:41.000000 robotframework-robocop-4.0.0/setup.py
```

### Comparing `robotframework-robocop-3.2.1/LICENSE` & `robotframework-robocop-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.1/PKG-INFO` & `robotframework-robocop-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 3.2.1
+Version: 4.0.0
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-3.2.1/README.md` & `robotframework-robocop-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.1/robocop/checkers/comments.py` & `robotframework-robocop-4.0.0/robocop/checkers/comments.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,41 +30,42 @@
         ),
         rule_id="0701",
         name="todo-in-comment",
         msg="Found a marker '{{ marker }}' in the comments",
         severity=RuleSeverity.WARNING,
         docs="""
         Report occurrences of the configured, case-insensitive marker in the comments.
-        By default, it reports TODO and FIXME markers.
+        By default, it reports ``TODO`` and ``FIXME`` markers.
 
         Example::
 
             # TODO: Refactor this code
             # fixme
 
         Configuration example::
 
             robocop --configure "todo-in-comment:markers:todo,Remove me,Fix this!"
 
         """,
+        added_in_version="1.0.0",
     ),
     "0702": Rule(
         RuleParam(
             name="block",
             default="^###",
             converter=regex,
             desc="Block comment regex pattern.",
         ),
         rule_id="0702",
         name="missing-space-after-comment",
         msg="Missing blank space after comment character",
         severity=RuleSeverity.WARNING,
         docs="""
-        Make sure to have one blank space after '#' comment character.
-        Configured regex for block comment should take into account the first character is `#`.
+        Make sure to have one blank space after ``#`` comment character.
+        Configured regex for block comment should take into account the first character is ``#``.
 
         Example::
 
             #bad
             # good
             ### good block
 
@@ -79,14 +80,15 @@
                 # Important topics here!
                 #
                 #*****
                 or
                 #* Headers *#
 
         """,
+        added_in_version="1.0.0",
     ),
     "0703": Rule(
         rule_id="0703",
         name="invalid-comment",
         msg="Invalid comment. '#' needs to be first character in the cell. "
         "For block comments you can use '*** Comments ***' section",
         severity=RuleSeverity.ERROR,
@@ -98,51 +100,54 @@
         Example::
 
             # good
              # bad
               # third cell so it's good
 
         """,
+        added_in_version="1.0.0",
     ),
     "0704": Rule(
         rule_id="0704",
         name="ignored-data",
         msg="Ignored data found in file",
         severity=RuleSeverity.WARNING,
         docs="""
         All lines before first test data section
         (`ref <https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#test-data-sections>`_)
-        are ignored. It's recommended to add `*** Comments ***` section header for lines that should be ignored.
+        are ignored. It's recommended to add ``*** Comments ***`` section header for lines that should be ignored.
 
         Missing section header::
 
             Resource   file.resource  # it looks like *** Settings *** but section header is missing - line is ignored
 
             *** Keywords ***
             Keyword Name
                No Operation
 
-        Comment lines that should be inside `*** Comments ***`::
+        Comment lines that should be inside ``*** Comments ***``::
 
             Deprecated Test
                 Keyword
                 Keyword 2
 
             *** Test Cases ***
 
         """,
+        added_in_version="1.3.0",
     ),
     "0705": Rule(
         rule_id="0705",
         name="bom-encoding-in-file",
         msg="This file contains BOM (Byte Order Mark) encoding not supported by Robot Framework",
         severity=RuleSeverity.WARNING,
         docs="""
         Some code editors can save Robot file using BOM encoding. Ensure that file is saved in UTF-8 encoding.
         """,
+        added_in_version="1.7.0",
     ),
 }
 
 
 class CommentChecker(VisitorChecker):
     """Checker for comments content. It detects invalid comments or leftovers like `todo` or `fixme` in the code."""
```

### Comparing `robotframework-robocop-3.2.1/robocop/checkers/documentation.py` & `robotframework-robocop-4.0.0/robocop/checkers/documentation.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
             Keyword
                 [Documentation]  Keyword documentation
                 Keyword Step
                 Other Step
 
         """,
+        added_in_version="1.0.0",
     ),
     "0202": Rule(
         RuleParam(
             name="ignore_templated",
             default="True",
             converter=str2bool,
             show_type="bool",
@@ -37,51 +38,55 @@
         rule_id="0202",
         name="missing-doc-test-case",
         msg="Missing documentation in '{{ name }}' test case",
         severity=RuleSeverity.WARNING,
         docs="""
         You can add documentation to test case using following syntax::
 
+            *** Test Cases ***
             Test
                 [Documentation]  Test documentation
                 Keyword Step
                 Other Step
 
         The rule by default ignores templated test cases but it can be configured with::
 
             robocop --configure missing-doc-test-case:ignore_templated:False
 
-        Possible values are: Yes / 1 / True (default) or No / False / 0.
+        Possible values are: ``Yes`` / ``1`` / ``True`` (default) or ``No`` / ``False`` / ``0``.
         """,
+        added_in_version="1.0.0",
     ),
     "0203": Rule(
         rule_id="0203",
         name="missing-doc-suite",
         msg="Missing documentation in suite",
         severity=RuleSeverity.WARNING,
         docs="""
         You can add documentation to suite using following syntax::
 
             *** Settings ***
             Documentation    Suite documentation
 
         """,
+        added_in_version="1.0.0",
     ),
     "0204": Rule(
         rule_id="0204",
         name="missing-doc-resource-file",
         msg="Missing documentation in resource file",
         severity=RuleSeverity.WARNING,
         docs="""
         You can add documentation to resource file using following syntax::
 
             *** Settings ***
             Documentation    Resource file documentation
 
         """,
+        added_in_version="2.8.0",
     ),
 }
 
 
 class MissingDocumentationChecker(VisitorChecker):
     """Checker for missing documentation."""
 
@@ -91,23 +96,23 @@
         "missing-doc-suite",
         "missing-doc-resource-file",
     )
 
     def visit_Keyword(self, node):  # noqa
         if node.name.lstrip().startswith("#"):
             return
-        self.check_if_docs_are_present(node, "missing-doc-keyword")
+        self.check_if_docs_are_present(node, "missing-doc-keyword", extend_disablers=True)
 
     def visit_TestCase(self, node):  # noqa
         if self.param("missing-doc-test-case", "ignore_templated") and self.templated_suite:
             return
-        self.check_if_docs_are_present(node, "missing-doc-test-case")
+        self.check_if_docs_are_present(node, "missing-doc-test-case", extend_disablers=True)
 
     def visit_SettingSection(self, node):  # noqa
-        self.check_if_docs_are_present(node, "missing-doc-suite")
+        self.check_if_docs_are_present(node, "missing-doc-suite", extend_disablers=False)
 
     def visit_File(self, node):  # noqa
         for section in node.sections:
             if isinstance(section, SettingSection):
                 break
         else:
             source = node.source if node.source else self.source
@@ -117,16 +122,23 @@
                     self.report("missing-doc-resource-file", node=node, lineno=1, col=1)
                 else:
                     self.report("missing-doc-suite", node=node, lineno=1, col=1)
             else:
                 self.report("missing-doc-suite", node=node, lineno=1, col=1)
         super().visit_File(node)
 
-    def check_if_docs_are_present(self, node, msg):
+    def check_if_docs_are_present(self, node, msg, extend_disablers):
         for statement in node.body:
             if isinstance(statement, Documentation):
                 break
         else:
+            extended_disablers = (node.lineno, node.end_lineno) if extend_disablers else None
             if hasattr(node, "name"):
-                self.report(msg, name=node.name, node=node, end_col=node.col_offset + len(node.name) + 1)
+                self.report(
+                    msg,
+                    name=node.name,
+                    node=node,
+                    end_col=node.col_offset + len(node.name) + 1,
+                    extended_disablers=extended_disablers,
+                )
             else:
-                self.report(msg, node=node, end_col=node.end_col_offset)
+                self.report(msg, node=node, end_col=node.end_col_offset, extended_disablers=extended_disablers)
```

### Comparing `robotframework-robocop-3.2.1/robocop/checkers/duplications.py` & `robotframework-robocop-4.0.0/robocop/checkers/duplications.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
             *** Test Cases ***
             Test with name
                 No Operation
             
             test_with Name  # it is a duplicate of 'Test with name'
                 No Operation
         """,
+        added_in_version="1.0.0",
     ),
     "0802": Rule(
         rule_id="0802",
         name="duplicated-keyword",
         msg="Multiple keywords with name '{{ name }}' (first occurrence in line {{ first_occurrence_line }})",
         severity=RuleSeverity.ERROR,
         docs="""
@@ -67,14 +68,15 @@
             keyword
                 No Operation
             
             K_eywor d
                 No Operation
             
         """,
+        added_in_version="1.0.0",
     ),
     "0803": Rule(
         rule_id="0803",
         name="duplicated-variable",
         msg="Multiple variables with name '{{ name }}' in Variables section (first occurrence in line "
         "{{ first_occurrence_line }}). "
         "Note that Robot Framework is case-insensitive",
@@ -87,20 +89,22 @@
             ${variable}    1
             ${VARIAble}    a
             @{variable}    a  b
             ${v ariabl e}  c
             ${v_ariable}   d
 
         """,
+        added_in_version="1.0.0",
     ),
     "0804": Rule(
         rule_id="0804",
         name="duplicated-resource",
         msg="Multiple resource imports with path '{{ name }}' (first occurrence in line {{ first_occurrence_line }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0805": Rule(
         rule_id="0805",
         name="duplicated-library",
         msg="Multiple library imports with name '{{ name }}' and identical arguments (first occurrence in line "
         "{{ first_occurrence_line }})",
         severity=RuleSeverity.WARNING,
@@ -108,26 +112,29 @@
         If you need to reimport library use alias::
         
             *** Settings ***
             Library  RobotLibrary
             Library  RobotLibrary  AS  OtherRobotLibrary
 
         """,
+        added_in_version="1.0.0",
     ),
     "0806": Rule(
         rule_id="0806",
         name="duplicated-metadata",
         msg="Duplicated metadata '{{ name }}' (first occurrence in line {{ first_occurrence_line }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0807": Rule(
         rule_id="0807",
         name="duplicated-variables-import",
         msg="Duplicated variables import with path '{{ name }}' (first occurrence in line {{ first_occurrence_line }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0808": Rule(
         rule_id="0808",
         name="section-already-defined",
         msg="'{{ section_name }}' section header already defined in file (first occurrence in line "
         "{{ first_occurrence_line }})",
         severity=RuleSeverity.WARNING,
@@ -146,30 +153,31 @@
                 No Operation
             
             *** Test Cases ***  # duplicate
             Other Test
                 Keyword
 
         """,
+        added_in_version="1.0.0",
     ),
     "0809": Rule(
         RuleParam(
             name="sections_order",
             default="settings,variables,testcases,keywords",
             converter=configure_sections_order,
             show_type="str",
             desc="order of sections in comma-separated list",
         ),
         rule_id="0809",
         name="section-out-of-order",
         msg="'{{ section_name }}' section header is defined in wrong order: {{ recommended_order }}",
         severity=RuleSeverity.WARNING,
         docs="""
-        Sections should be defined in order set by `sections_order` 
-        parameter (default: `settings,variables,testcases,keywords`).
+        Sections should be defined in order set by ``sections_order``
+        parameter (default: ``settings,variables,testcases,keywords``).
         
         To change the default order use following option::
         
             robocop --configure section-out-of-order:sections_order:comma,separated,list,of,sections
         
         where section should be case-insensitive name from the list: comments, settings, variables, testcases, keywords. 
         Order of not configured sections is ignored.
@@ -179,28 +187,30 @@
             *** Settings ***
             
             *** Keywords ***
             
             *** Test Cases ***  # it will report issue because Test Cases should be defined before Keywords
 
         """,
+        added_in_version="1.0.0",
     ),
     "0810": Rule(
         rule_id="0810",
         name="both-tests-and-tasks",
         msg="Both Task(s) and Test Case(s) section headers defined in file",
         severity=RuleSeverity.ERROR,
         docs="""
-        The file contains both Test Case and Task sections. Use only one of them. ::
+        The file contains both ``*** Test Cases ***`` and ``*** Tasks ***`` sections. Use only one of them. ::
         
             *** Test Cases ***
             
             *** Tasks ***
 
         """,
+        added_in_version="1.0.0",
     ),
     "0811": Rule(
         rule_id="0811",
         name="duplicated-argument-name",
         msg="Argument name '{{ argument_name }}' is already used",
         severity=RuleSeverity.ERROR,
         docs="""
@@ -209,14 +219,15 @@
         
             *** Keywords ***
             Keyword
                 [Arguments]    ${var}  ${VAR}  ${v_ar}  ${v ar}
                 Other Keyword
 
         """,
+        added_in_version="1.11.0",
     ),
     "0812": Rule(
         rule_id="0812",
         name="duplicated-assigned-var-name",
         msg="Assigned variable name '{{ variable_name }}' is already used",
         severity=RuleSeverity.INFO,
         docs="""
@@ -224,14 +235,15 @@
         are duplicates::
         
             *** Test Cases ***
             Test
                 ${var}  ${VAR}  ${v_ar}  ${v ar}  Keyword
         
         """,
+        added_in_version="1.12.0",
     ),
     "0813": Rule(
         rule_id="0813",
         name="duplicated-setting",
         msg="{{ error_msg }}",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -239,14 +251,15 @@
         Example::
         
             *** Settings ***
             Force Tags        F1
             Force Tags        F2  # this setting will be ignored
         
         """,
+        added_in_version="2.0.0",
     ),
 }
 
 
 class DuplicationsChecker(VisitorChecker):
     """Checker for duplicated names."""
```

### Comparing `robotframework-robocop-3.2.1/robocop/checkers/errors.py` & `robotframework-robocop-4.0.0/robocop/checkers/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 try:
     from robot.api.parsing import If
 except ImportError:
     If = None
 
 from robocop.checkers import VisitorChecker
 from robocop.rules import Rule, RuleSeverity
-from robocop.utils import ROBOT_VERSION, find_robot_vars
+from robocop.utils import ROBOT_VERSION, find_robot_vars, get_errors
 
 rules = {
     "0401": Rule(
         rule_id="0401",
         name="parsing-error",
         msg="Robot Framework syntax error: {{ error_msg }}",
         severity=RuleSeverity.ERROR,
+        added_in_version="1.0.0",
     ),
     "0402": Rule(
         rule_id="0402",
         name="not-enough-whitespace-after-setting",
         msg="Provide at least two spaces after '{{ setting_name }}' setting",
         severity=RuleSeverity.ERROR,
         docs="""
@@ -37,14 +38,15 @@
             *** Keywords ***
             Keyword
                 [Documentation]  This is doc
                 [Arguments] ${var}  # only one space after [Arguments]
                 Should Be True  ${var}
             
         """,
+        added_in_version="1.0.0",
     ),
     "0403": Rule(
         rule_id="0403",
         name="missing-keyword-name",
         msg="Missing keyword name when calling some values",
         severity=RuleSeverity.ERROR,
         docs="""
@@ -52,14 +54,15 @@
         
             *** Keywords ***
             Keyword
                 ${var}
                 ${one}      ${two}
 
         """,
+        added_in_version="1.8.0",
     ),
     "0404": Rule(
         rule_id="0404",
         name="variables-import-with-args",
         msg="YAML variable files do not take arguments",
         severity=RuleSeverity.ERROR,
         docs="""
@@ -67,14 +70,15 @@
         
             *** Settings ***
             Variables    vars.yaml        arg1
             Variables    variables.yml    arg2
             Variables    module           arg3  # valid from RF > 5
         
         """,
+        added_in_version="1.11.0",
     ),
     "0405": Rule(
         rule_id="0405",
         name="invalid-continuation-mark",
         msg="Invalid continuation mark '{{ mark }}'. It should be '...'",
         severity=RuleSeverity.ERROR,
         docs="""
@@ -82,14 +86,15 @@
         
             Keyword
             ..  ${var}  # .. instead of ...
             ...  1
             ....  2  # .... instead of ...
 
         """,
+        added_in_version="1.11.0",
     ),
     # there is not-enough-whitespace-after-newline-marker for keyword calls already
     "0406": Rule(
         rule_id="0406",
         name="not-enough-whitespace-after-newline-marker",
         msg="Provide at least two spaces after '...' marker",
         severity=RuleSeverity.ERROR,
@@ -97,52 +102,56 @@
         Example of rule violation::
         
             @{LIST}  1
             ... 2  # not enough whitespace
             ...  3
 
         """,
+        added_in_version="1.11.0",
     ),
     "0407": Rule(
         rule_id="0407",
         name="invalid-argument",
         msg="{{ error_msg }}",
         severity=RuleSeverity.ERROR,
         version=">=4.0",
         docs="""
-        Argument names should follow variable naming syntax: start with identifier (`$`, `@` or `&`) and enclosed in 
-        curly brackets (`{}`).
+        Argument names should follow variable naming syntax: start with identifier (``$``, ``@`` or ``&``) and enclosed in 
+        curly brackets (``{}``).
         
         Valid names::
         
             Keyword
                 [Arguments]    ${var}    @{args}    &{config}    ${var}=default
         
         Invalid names::
         
             Keyword
                 [Arguments]    {var}    @args}    var=default
         
         """,
+        added_in_version="1.11.0",
     ),
     "0408": Rule(
         rule_id="0408",
         name="non-existing-setting",
         msg="{{ error_msg }}",
         severity=RuleSeverity.ERROR,
         docs="""
         Non-existing setting can't be used in the code.
         
-        Rule violation example::
+        Example of rule violation::
         
-           *** Test Case ***
+           *** Test Cases ***
+           My Test Case
                [Not Existing]  arg
                [Arguments]  ${arg}
     
         """,
+        added_in_version="1.11.0",
     ),
     "0409": Rule(
         rule_id="0409",
         name="setting-not-supported",
         msg="Setting '[{{ setting_name }}]' is not supported in {{ test_or_keyword }}. "
         "Allowed are: {{ allowed_settings }}",
         severity=RuleSeverity.ERROR,
@@ -162,28 +171,30 @@
             [Tags]	         Used for specifying user keyword tags.
             [Arguments]	     Used for specifying user keyword arguments.
             [Return]	     Used for specifying user keyword return values.
             [Teardown]	     Used for specifying user keyword teardown.
             [Timeout]	     Used for specifying a user keyword timeout.
         
         """,
+        added_in_version="1.11.0",
     ),
     "0410": Rule(
         rule_id="0410",
         name="not-enough-whitespace-after-variable",
         msg="Provide at least two spaces after '{{ variable_name }}' variable name",
         severity=RuleSeverity.ERROR,
         version=">=4.0",
         docs="""
         Example of rule violation::
         
             ${variable} 1  # not enough whitespace
             ${other_var}  2
         
         """,
+        added_in_version="1.11.0",
     ),
     "0411": Rule(
         rule_id="0411",
         name="not-enough-whitespace-after-suite-setting",
         msg="Provide at least two spaces after '{{ setting_name }}' setting",
         severity=RuleSeverity.ERROR,
         docs="""
@@ -192,45 +203,71 @@
             *** Settings ***
             Library Collections  # not enough whitespace
             Force Tags  tag
             ...  tag2
             Suite Setup Keyword  # not enough whitespace
         
         """,
+        added_in_version="1.11.0",
     ),
     "0412": Rule(
         rule_id="0412",
         name="invalid-for-loop",
         msg="Invalid for loop syntax: {{ error_msg }}",
         severity=RuleSeverity.ERROR,
         version=">=4.0",
+        added_in_version="1.11.0",
     ),
     "0413": Rule(
         rule_id="0413",
         name="invalid-if",
         msg="Invalid IF syntax: {{ error_msg }}",
         severity=RuleSeverity.ERROR,
         version=">=4.0",
+        added_in_version="1.11.0",
     ),
     "0414": Rule(
         rule_id="0414",
         name="return-in-test-case",
         msg="RETURN can only be used inside a user keyword",
         severity=RuleSeverity.ERROR,
         version=">=5.0",
+        added_in_version="2.0.0",
     ),
     "0415": Rule(
         rule_id="0415",
         name="invalid-section-in-resource",
         msg="Resource file can't contain '{{ section_name }}' section",
         docs="""
         The higher-level structure of resource files is the same as that of test case files,
         but they can't contain Test Cases or Tasks sections.
         """,
         severity=RuleSeverity.ERROR,
+        added_in_version="3.1.0",
+    ),
+    "0416": Rule(
+        rule_id="0416",
+        name="invalid-setting-in-resource",
+        msg="Settings section in resource file can't contain '{{ section_name }}' setting",
+        docs="""
+        The Setting section in resource files can contain only import settings (``Library``,
+        ``Resource``, ``Variables``), ``Documentation`` and ``Keyword Tags``.
+        """,
+        severity=RuleSeverity.ERROR,
+        added_in_version="3.3.0",
+    ),
+    "0417": Rule(
+        rule_id="0417",
+        name="unsupported-setting-in-init-file",
+        msg="Setting '{{ setting }}' is not supported in initialization files",
+        severity=RuleSeverity.ERROR,
+        docs="""
+        Settings ``Default Tags`` and ``Test Template`` are not supported in initialization files.
+        """,
+        added_in_version="3.3.0",
     ),
 }
 
 
 class ParsingErrorChecker(VisitorChecker):
     """Checker that parses Robot Framework DataErrors."""
 
@@ -243,14 +280,16 @@
         "setting-not-supported",
         "not-enough-whitespace-after-variable",
         "not-enough-whitespace-after-suite-setting",
         "invalid-for-loop",
         "invalid-if",
         "return-in-test-case",
         "invalid-section-in-resource",
+        "invalid-setting-in-resource",
+        "unsupported-setting-in-init-file",
     )
 
     keyword_only_settings = {"Arguments", "Return"}
     keyword_settings = [
         "[Documentation]",
         "[Tags]",
         "[Arguments]",
@@ -352,15 +391,19 @@
         elif "IF" in error or ("ELSE" in error and If and isinstance(self.in_block, If)):
             self.handle_invalid_block(node, error, "invalid-if")
         elif "FOR loop" in error:
             self.handle_invalid_block(node, error, "invalid-for-loop")
         elif "Non-default argument after default arguments" in error or "Only last argument can be kwargs" in error:
             self.handle_positional_after_named(node, error_index)
         elif "Resource file with" in error:
-            self.handle_invalid_section_in_resource(node, error)
+            self.handle_invalid_section_in_resource(node)
+        elif "is not allowed in resource file" in error:
+            self.handle_invalid_setting_in_resource_file(node, error)
+        elif "is not allowed in suite initialization file" in error:
+            self.handle_unsupported_settings_in_init_file(node, error)
         else:
             error = error.replace("\n   ", "")
             token = node.header if hasattr(node, "header") else node
             end_col = token.col_offset + len(node.name) + 1 if hasattr(node, "name") else token.end_col_offset + 1
             # TODO: 'col' location here can be specified more precisely
             self.report("parsing-error", error_msg=error, node=node, col=token.col_offset + 1, end_col=end_col)
 
@@ -512,14 +555,26 @@
                 self.report(
                     "not-enough-whitespace-after-newline-marker",
                     node=node,
                     col=col,
                     end_col=col + 3,
                 )
 
+    def handle_unsupported_settings_in_init_file(self, node, error):
+        setting_node = node.data_tokens[0]
+        setting_name = setting_node.value
+        self.report(
+            "unsupported-setting-in-init-file",
+            setting=setting_name,
+            node=setting_node,
+            col=setting_node.col_offset + 1,
+            end_col=setting_node.col_offset + 1 + len(setting_name),
+            lineno=setting_node.lineno,
+        )
+
     @staticmethod
     def is_var_positional(value):
         if not value:
             return False
         if value.startswith("&") or "=" in value:
             return True
         return False
@@ -542,24 +597,34 @@
             "parsing-error",
             error_msg=f"Positional argument '{token.value}' follows named argument",
             node=token,
             col=token.col_offset + 1,
             end_col=token.end_col_offset + 1,
         )
 
-    def handle_invalid_section_in_resource(self, node, error):
+    def handle_invalid_section_in_resource(self, node):
         error_token = node.tokens[0]
         section_name = error_token.value
         self.report(
             "invalid-section-in-resource",
             section_name=section_name,
             node=node,
             end_col=node.col_offset + len(section_name) + 1,
         )
 
+    def handle_invalid_setting_in_resource_file(self, node, error):
+        setting_error = re.search("Setting '(.*)' is not allowed in resource file", error)
+        self.report(
+            "invalid-setting-in-resource",
+            section_name=setting_error.group(1),
+            node=node,
+            lineno=node.lineno,
+            end_col=node.end_col_offset + 1,
+        )
+
 
 class TwoSpacesAfterSettingsChecker(VisitorChecker):
     """Checker for not enough whitespaces after [Setting] header."""
 
     reports = ("not-enough-whitespace-after-setting",)
 
     def __init__(self):
```

### Comparing `robotframework-robocop-3.2.1/robocop/checkers/lengths.py` & `robotframework-robocop-4.0.0/robocop/checkers/lengths.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,223 +24,281 @@
 from robocop.rules import Rule, RuleParam, RuleSeverity, SeverityThreshold
 from robocop.utils import get_section_name, normalize_robot_name, pattern_type, str2bool
 
 rules = {
     "0501": Rule(
         RuleParam(name="max_len", default=40, converter=int, desc="number of lines allowed in a keyword"),
         RuleParam(name="ignore_docs", default=False, converter=str2bool, show_type="bool", desc="Ignore documentation"),
-        SeverityThreshold("max_len", compare_method="greater"),
+        SeverityThreshold("max_len", compare_method="greater", substitute_value="allowed_length"),
         rule_id="0501",
         name="too-long-keyword",
         msg="Keyword '{{ keyword_name }}' is too long ({{ keyword_length }}/{{ allowed_length}})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0502": Rule(
         RuleParam(name="min_calls", default=1, converter=int, desc="number of keyword calls required in a keyword"),
-        SeverityThreshold("min_calls", compare_method="less"),
+        SeverityThreshold("min_calls", compare_method="less", substitute_value="min_allowed_count"),
         rule_id="0502",
         name="too-few-calls-in-keyword",
         msg="Keyword '{{ keyword_name }}' has too few keywords inside ({{ keyword_count }}/{{ min_allowed_count }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0503": Rule(
         RuleParam(name="max_calls", default=10, converter=int, desc="number of keyword calls allowed in a keyword"),
-        SeverityThreshold("max_calls", compare_method="greater"),
+        SeverityThreshold("max_calls", compare_method="greater", substitute_value="max_allowed_count"),
         rule_id="0503",
         name="too-many-calls-in-keyword",
         msg="Keyword '{{ keyword_name }}' has too many keywords inside ({{ keyword_count }}/{{ max_allowed_count }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0504": Rule(
         RuleParam(name="max_len", default=20, converter=int, desc="number of lines allowed in a test case"),
         RuleParam(name="ignore_docs", default=False, converter=str2bool, show_type="bool", desc="Ignore documentation"),
-        SeverityThreshold("max_len", compare_method="greater"),
+        SeverityThreshold("max_len", compare_method="greater", substitute_value="allowed_length"),
         rule_id="0504",
         name="too-long-test-case",
         msg="Test case '{{ test_name }}' is too long ({{ test_length }}/{{ allowed_length }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0505": Rule(
         RuleParam(name="max_calls", default=10, converter=int, desc="number of keyword calls allowed in a test case"),
         RuleParam(
             name="ignore_templated", default=False, converter=str2bool, show_type="bool", desc="Ignore templated tests"
         ),
-        SeverityThreshold("max_calls", compare_method="greater"),
+        SeverityThreshold("max_calls", compare_method="greater", substitute_value="max_allowed_count"),
         rule_id="0505",
         name="too-many-calls-in-test-case",
         msg="Test case '{{ test_name }}' has too many keywords inside ({{ keyword_count }}/{{ max_allowed_count }})",
         docs="Redesign the test and move complex logic to separate keywords to increase readability.",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0506": Rule(
         RuleParam(name="max_lines", default=400, converter=int, desc="number of lines allowed in a file"),
-        SeverityThreshold("max_lines", compare_method="greater"),
+        SeverityThreshold("max_lines", compare_method="greater", substitute_value="max_allowed_count"),
         rule_id="0506",
         name="file-too-long",
         msg="File has too many lines ({{ lines_count }}/{{max_allowed_count }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0507": Rule(
         RuleParam(name="max_args", default=5, converter=int, desc="number of lines allowed in a file"),
-        SeverityThreshold("max_args", compare_method="greater"),
+        SeverityThreshold("max_args", compare_method="greater", substitute_value="max_allowed_count"),
         rule_id="0507",
         name="too-many-arguments",
         msg="Keyword '{{ keyword_name }}' has too many arguments ({{ arguments_count }}/{{ max_allowed_count }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0508": Rule(
         RuleParam(name="line_length", default=120, converter=int, desc="number of characters allowed in line"),
         RuleParam(
             name="ignore_pattern",
             default=re.compile(r"https?://\S+"),
             converter=pattern_type,
             show_type="regex",
             desc="ignore lines that contain configured pattern",
         ),
-        SeverityThreshold("line_length"),
+        SeverityThreshold("line_length", substitute_value="allowed_length"),
         rule_id="0508",
         name="line-too-long",
         msg="Line is too long ({{ line_length }}/{{ allowed_length }})",
         severity=RuleSeverity.WARNING,
         docs="""
         It is possible to ignore lines that match regex pattern. Configure it using following option::
 
             robocop --configure line-too-long:ignore_pattern:pattern
 
         The default pattern is ``https?://\S+`` that ignores the lines that look like an URL.
 
         """,
+        added_in_version="1.0.0",
     ),
     "0509": Rule(
-        rule_id="0509", name="empty-section", msg="Section '{{ section_name }}' is empty", severity=RuleSeverity.WARNING
+        rule_id="0509",
+        name="empty-section",
+        msg="Section '{{ section_name }}' is empty",
+        severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0510": Rule(
         RuleParam(
             name="max_returns", default=4, converter=int, desc="allowed number of returned values from a keyword"
         ),
-        SeverityThreshold("max_returns", compare_method="greater"),
+        SeverityThreshold("max_returns", compare_method="greater", substitute_value="max_allowed_count"),
         rule_id="0510",
         name="number-of-returned-values",
         msg="Too many return values ({{ return_count }}/{{ max_allowed_count }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0511": Rule(
         rule_id="0511",
         name="empty-metadata",
         msg="Metadata settings does not have any value set",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0512": Rule(
         rule_id="0512",
         name="empty-documentation",
         msg="Documentation of {{ block_name }} is empty",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
+    ),
+    "0513": Rule(
+        rule_id="0513",
+        name="empty-force-tags",
+        msg="Force Tags are empty",
+        severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
-    "0513": Rule(rule_id="0513", name="empty-force-tags", msg="Force Tags are empty", severity=RuleSeverity.WARNING),
     "0514": Rule(
-        rule_id="0514", name="empty-default-tags", msg="Default Tags are empty", severity=RuleSeverity.WARNING
+        rule_id="0514",
+        name="empty-default-tags",
+        msg="Default Tags are empty",
+        severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0515": Rule(
-        rule_id="0515", name="empty-variables-import", msg="Import variables path is empty", severity=RuleSeverity.ERROR
+        rule_id="0515",
+        name="empty-variables-import",
+        msg="Import variables path is empty",
+        severity=RuleSeverity.ERROR,
+        added_in_version="1.0.0",
     ),
     "0516": Rule(
-        rule_id="0516", name="empty-resource-import", msg="Import resource path is empty", severity=RuleSeverity.ERROR
+        rule_id="0516",
+        name="empty-resource-import",
+        msg="Import resource path is empty",
+        severity=RuleSeverity.ERROR,
+        added_in_version="1.0.0",
     ),
     "0517": Rule(
-        rule_id="0517", name="empty-library-import", msg="Import library path is empty", severity=RuleSeverity.ERROR
+        rule_id="0517",
+        name="empty-library-import",
+        msg="Import library path is empty",
+        severity=RuleSeverity.ERROR,
+        added_in_version="1.0.0",
     ),
     "0518": Rule(
         rule_id="0518",
         name="empty-setup",
         msg="Setup of {{ block_name }} does not have any keywords",
         severity=RuleSeverity.ERROR,
+        added_in_version="1.0.0",
     ),
     "0519": Rule(
         rule_id="0519",
         name="empty-suite-setup",
         msg="Suite Setup does not have any keywords",
         severity=RuleSeverity.ERROR,
+        added_in_version="1.0.0",
     ),
     "0520": Rule(
         rule_id="0520",
         name="empty-test-setup",
         msg="Test Setup does not have any keywords",
         severity=RuleSeverity.ERROR,
+        added_in_version="1.0.0",
     ),
     "0521": Rule(
         rule_id="0521",
         name="empty-teardown",
         msg="Teardown of {{ block_name }} does not have any keywords",
         severity=RuleSeverity.ERROR,
+        added_in_version="1.0.0",
     ),
     "0522": Rule(
         rule_id="0522",
         name="empty-suite-teardown",
         msg="Suite Teardown does not have any keywords",
         severity=RuleSeverity.ERROR,
+        added_in_version="1.0.0",
     ),
     "0523": Rule(
         rule_id="0523",
         name="empty-test-teardown",
         msg="Test Teardown does not have any keywords",
         severity=RuleSeverity.ERROR,
+        added_in_version="1.0.0",
     ),
     "0524": Rule(
-        rule_id="0524", name="empty-timeout", msg="Timeout of {{ block_name }} is empty", severity=RuleSeverity.WARNING
+        rule_id="0524",
+        name="empty-timeout",
+        msg="Timeout of {{ block_name }} is empty",
+        severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
+    ),
+    "0525": Rule(
+        rule_id="0525",
+        name="empty-test-timeout",
+        msg="Test Timeout is empty",
+        severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
-    "0525": Rule(rule_id="0525", name="empty-test-timeout", msg="Test Timeout is empty", severity=RuleSeverity.WARNING),
     "0526": Rule(
         rule_id="0526",
         name="empty-arguments",
         msg="Arguments of {{ block_name }} are empty",
         severity=RuleSeverity.ERROR,
+        added_in_version="1.0.0",
     ),
     "0527": Rule(
         RuleParam(name="max_testcases", default=50, converter=int, desc="number of test cases allowed in a suite"),
         RuleParam(
             name="max_templated_testcases",
             default=100,
             converter=int,
             desc="number of test cases allowed in a templated suite",
         ),
-        SeverityThreshold("max_testcases or max_templated_testcases"),
+        SeverityThreshold("max_testcases or max_templated_testcases", substitute_value="max_allowed_count"),
         rule_id="0527",
         name="too-many-test-cases",
         msg="Too many test cases ({{ test_count }}/{{ max_allowed_count }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.10.0",
     ),
     "0528": Rule(
         RuleParam(name="min_calls", default=1, converter=int, desc="number of keyword calls required in a test case"),
         RuleParam(
             name="ignore_templated", default=False, converter=str2bool, show_type="bool", desc="Ignore templated tests"
         ),
         rule_id="0528",
         name="too-few-calls-in-test-case",
         msg="Test case '{{ test_name }}' has too few keywords inside ({{ keyword_count }}/{{ min_allowed_count }})",
         docs="""
-        Test without keywords will fail. Add more keywords or set results using Fail, Pass, Skip keywords::
+        Test without keywords will fail. Add more keywords or set results using ``Fail``, ``Pass Execution`` or
+        ``Skip`` keywords::
 
             *** Test Cases ***
             Test case
                 [Tags]    smoke
                 Skip    Test case draft
 
         """,
         severity=RuleSeverity.ERROR,
+        added_in_version="2.4.0",
     ),
     "0529": Rule(
         rule_id="0529",
         name="empty-test-template",
         msg="Test Template is empty",
         docs="""
         ``Test Template`` sets the template to all tests in a suite. Empty value is considered an error
         because it leads the users to wrong impression on how the suite operates.
         Without value, the setting is ignored and the tests are not templated.
         """,
         severity=RuleSeverity.ERROR,
+        added_in_version="3.1.0",
     ),
     "0530": Rule(
         rule_id="0530",
         name="empty-template",
         msg="Template of {{ block_name }} is empty. "
         "To overwrite suite Test Template use more explicit [Template]  NONE",
         docs="""
@@ -258,14 +316,23 @@
                 argument
             
             Not templated test
                 [Template]    NONE
 
         """,
         severity=RuleSeverity.WARNING,
+        added_in_version="3.1.0",
+    ),
+    "0531": Rule(
+        rule_id="0531",
+        name="empty-keyword-tags",
+        msg="Keyword Tags are empty",
+        severity=RuleSeverity.WARNING,
+        version=">=6",
+        added_in_version="3.3.0",
     ),
 }
 
 
 def is_data_statement(node):
     return not isinstance(node, (EmptyLine, Comment))
 
@@ -332,72 +399,76 @@
                     self.report(
                         "too-many-arguments",
                         keyword_name=node.name,
                         arguments_count=args_number,
                         max_allowed_count=self.param("too-many-arguments", "max_args"),
                         node=node,
                         end_col=node.col_offset + len(node.name) + 1,
+                        extended_disablers=(node.lineno, node.end_lineno),
                         sev_threshold_value=args_number,
                     )
                 break
         length, node_end_line = check_node_length(node, ignore_docs=self.param("too-long-keyword", "ignore_docs"))
         if length > self.param("too-long-keyword", "max_len"):
             self.report(
                 "too-long-keyword",
                 keyword_name=node.name,
                 keyword_length=length,
                 allowed_length=self.param("too-long-keyword", "max_len"),
                 node=node,
                 end_col=node.col_offset + len(node.name) + 1,
-                ext_disablers=(node.lineno, node_end_line),
+                extended_disablers=(node.lineno, node_end_line),
                 sev_threshold_value=length,
             )
             return
         key_calls = LengthChecker.count_keyword_calls(node)
         if key_calls < self.param("too-few-calls-in-keyword", "min_calls"):
             self.report(
                 "too-few-calls-in-keyword",
                 keyword_name=node.name,
                 keyword_count=key_calls,
                 min_allowed_count=self.param("too-few-calls-in-keyword", "min_calls"),
                 node=node,
                 end_col=node.col_offset + len(node.name) + 1,
+                extended_disablers=(node.lineno, node.end_lineno),
                 sev_threshold_value=key_calls,
             )
         elif key_calls > self.param("too-many-calls-in-keyword", "max_calls"):
             self.report(
                 "too-many-calls-in-keyword",
                 keyword_name=node.name,
                 keyword_count=key_calls,
                 max_allowed_count=self.param("too-many-calls-in-keyword", "max_calls"),
                 node=node,
                 end_col=node.col_offset + len(node.name) + 1,
+                extended_disablers=(node.lineno, node.end_lineno),
                 sev_threshold_value=key_calls,
             )
 
     def test_is_templated(self, node):
         if self.templated_suite:
             return True
         if not node.body:
             return False
         for statement in node.body:
             if isinstance(statement, Template):
                 return True
         return False
 
     def visit_TestCase(self, node):  # noqa
-        length, _ = check_node_length(node, ignore_docs=self.param("too-long-test-case", "ignore_docs"))
+        length, node_end_line = check_node_length(node, ignore_docs=self.param("too-long-test-case", "ignore_docs"))
         if length > self.param("too-long-test-case", "max_len"):
             self.report(
                 "too-long-test-case",
                 test_name=node.name,
                 test_length=length,
                 allowed_length=self.param("too-long-test-case", "max_len"),
                 node=node,
                 end_col=node.col_offset + len(node.name) + 1,
+                extended_disablers=(node.lineno, node_end_line),
                 sev_threshold_value=length,
             )
         test_is_templated = self.test_is_templated(node)
         skip_too_many = test_is_templated and self.param("too-many-calls-in-test-case", "ignore_templated")
         skip_too_few = test_is_templated and self.param("too-few-calls-in-test-case", "ignore_templated")
         if skip_too_few and skip_too_many:
             return
@@ -406,24 +477,26 @@
             self.report(
                 "too-many-calls-in-test-case",
                 test_name=node.name,
                 keyword_count=key_calls,
                 max_allowed_count=self.param("too-many-calls-in-test-case", "max_calls"),
                 node=node,
                 sev_threshold_value=key_calls,
+                extended_disablers=(node.lineno, node.end_lineno),
                 end_col=node.col_offset + len(node.name) + 1,
             )
         elif not skip_too_few and (key_calls < self.param("too-few-calls-in-test-case", "min_calls")):
             self.report(
                 "too-few-calls-in-test-case",
                 test_name=node.name,
                 keyword_count=key_calls,
                 min_allowed_count=self.param("too-few-calls-in-test-case", "min_calls"),
                 node=node,
                 sev_threshold_value=key_calls,
+                extended_disablers=(node.lineno, node.end_lineno),
                 end_col=node.col_offset + len(node.name) + 1,
             )
 
     @staticmethod
     def count_keyword_calls(node):
         # ReturnStatement is imported and evaluates to true in RF 5.0+, we don't need to also check Break/Continue
         if (
@@ -540,14 +613,15 @@
         "empty-suite-teardown",
         "empty-test-teardown",
         "empty-timeout",
         "empty-test-timeout",
         "empty-template",
         "empty-test-template",
         "empty-arguments",
+        "empty-keyword-tags",
     )
 
     def __init__(self):
         self.parent_node_name = ""
         super().__init__()
 
     def visit_SettingSection(self, node):  # noqa
@@ -586,14 +660,18 @@
         if not node.values:
             self.report("empty-force-tags", node=node, col=node.col_offset + 1, end_col=node.end_col_offset)
 
     def visit_DefaultTags(self, node):  # noqa
         if not node.values:
             self.report("empty-default-tags", node=node, col=node.col_offset + 1, end_col=node.end_col_offset)
 
+    def visit_KeywordTags(self, node):  # noqa
+        if not node.values:
+            self.report("empty-keyword-tags", node=node, col=node.col_offset + 1, end_col=node.end_col_offset)
+
     def visit_VariablesImport(self, node):  # noqa
         if not node.name:
             self.report("empty-variables-import", node=node, col=node.col_offset + 1, end_col=node.end_col_offset)
 
     def visit_ResourceImport(self, node):  # noqa
         if not node.name:
             self.report("empty-resource-import", node=node, col=node.col_offset + 1)
```

### Comparing `robotframework-robocop-3.2.1/robocop/checkers/misc.py` & `robotframework-robocop-4.0.0/robocop/checkers/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 Miscellaneous checkers
 """
-from collections import namedtuple
 from dataclasses import dataclass
 from pathlib import Path
 
 from robot.api import Token
 from robot.errors import VariableError
 from robot.parsing.model.blocks import TestCaseSection
 from robot.parsing.model.statements import Arguments, KeywordCall, Return, Teardown
@@ -59,24 +58,26 @@
 
             Keyword
                 Step
                 ${variable}    Other Step
                 [Return]    ${variable}
 
         """,
+        added_in_version="1.0.0",
     ),
     "0903": Rule(
         rule_id="0903",
         name="empty-return",
         msg="[Return] is empty",
         severity=RuleSeverity.WARNING,
         docs="""
         ``[Return]`` statement is used to define variables returned from keyword. If you don't return anything from
         keyword,  don't use ``[Return]``.
         """,
+        added_in_version="1.0.0",
     ),
     "0907": Rule(
         rule_id="0907",
         name="nested-for-loop",
         msg="Nested for loops are not supported. You can use keyword with for loop instead",
         severity=RuleSeverity.ERROR,
         version="<4.0",
@@ -86,24 +87,26 @@
             FOR    ${var}    IN RANGE    10
                 FOR   ${other_var}   IN    a  b
                     # Nesting supported from Robot Framework 4.0+
                 END
             END
 
         """,
+        added_in_version="1.0.0",
     ),
     "0908": Rule(
         rule_id="0908",
         name="if-can-be-used",
         msg="'{{ run_keyword }}' can be replaced with IF block since Robot Framework 4.0",
         severity=RuleSeverity.INFO,
         version="==4.*",
         docs="""
-        Starting from Robot Framework 4.0 `Run Keyword If` and `Run Keyword Unless` can be replaced by IF block.
+        Starting from Robot Framework 4.0 ``Run Keyword If`` and ``Run Keyword Unless`` can be replaced by IF block.
         """,
+        added_in_version="1.4.0",
     ),
     "0909": Rule(
         RuleParam(
             name="assignment_sign_type",
             default="autodetect",
             converter=parse_assignment_sign_type,
             show_type="assignment sign type",
@@ -130,18 +133,19 @@
                 ${var}  ${var2}  Some Keyword  # this assignment doesn't use equal sign while the previous one uses ' ='
 
         By default Robocop looks for most popular assignment sign in the file. It is possible to define expected
         assignment sign by running::
 
             robocop --configure inconsistent-assignment:assignment_sign_type:equal_sign
 
-        You can choose between following signs: 'autodetect' (default), 'none' (''), 'equal_sign' ('=') or
-        space_and_equal_sign (' =').
+        You can choose between following signs: 'autodetect' (default), 'none', 'equal_sign' (``=``) or
+        space_and_equal_sign (`` =``).
 
         """,
+        added_in_version="1.7.0",
     ),
     "0910": Rule(
         RuleParam(
             name="assignment_sign_type",
             default="autodetect",
             converter=parse_assignment_sign_type,
             show_type="assignment sign type",
@@ -161,23 +165,24 @@
             *** Variables ***
             ${var} =    1
             ${var2}=    2
             ${var3} =   3
             ${var4}     a
             ${var5}     b
 
-        By default Robocop looks for most popular assignment sign in the file. It is possible to define expected
+        By default, Robocop looks for the most popular assignment sign in the file. It is possible to define expected
         assignment sign by running::
 
             robocop --configure inconsistent-assignment-in-variables:assignment_sign_type:equal_sign
 
-        You can choose between following signs: 'autodetect' (default), 'none' (''), 'equal_sign' ('=') or
-        space_and_equal_sign (' =').
+        You can choose between following signs: 'autodetect' (default), 'none', 'equal_sign' (``=``) or
+        space_and_equal_sign (`` =``).
 
         """,
+        added_in_version="1.7.0",
     ),
     "0911": Rule(
         rule_id="0911",
         name="wrong-import-order",
         msg="BuiltIn library import '{{ builtin_import }}' should be placed before '{{ custom_import }}'",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -185,14 +190,15 @@
 
             *** Settings ***
             Library    Collections
             Library    CustomLibrary
             Library    OperatingSystem  # BuiltIn library defined after custom CustomLibrary
 
         """,
+        added_in_version="1.7.0",
     ),
     "0912": Rule(
         rule_id="0912",
         name="empty-variable",
         msg="Use built-in variable {{ var_type }}{EMPTY} instead of leaving variable without value or using backslash",
         severity=RuleSeverity.INFO,
         docs="""
@@ -203,74 +209,78 @@
             ${VAR_WITH_EMPTY}       ${EMPTY}
             @{MULTILINE_FIRST_EMPTY}
             ...                               # missing value
             ...  value
             ${EMPTY_WITH_BACKSLASH}  \        # used backslash
 
         """,
+        added_in_version="1.10.0",
     ),
     "0913": Rule(
         rule_id="0913",
         name="can-be-resource-file",
         msg="No tests in '{{ file_name }}' file, consider renaming to '{{ file_name_stem }}.resource'",
         severity=RuleSeverity.INFO,
         docs="""
-        If the Robot file contains only keywords or variables it's a good practice to use `.resource` extension.
+        If the Robot file contains only keywords or variables, it's a good practice to use ``.resource`` extension.
         """,
+        added_in_version="1.10.0",
     ),
     "0914": Rule(
         rule_id="0914",
         name="if-can-be-merged",
         msg="IF statement can be merged with previous IF (defined in line {{ line }})",
         severity=RuleSeverity.INFO,
         version=">=4.0",
         docs="""
-        IF statement follows another IF with identical conditions. It can be possibly merged into one.
+        ``IF`` statement follows another ``IF`` with identical conditions. It can be possibly merged into one.
 
         Example of rule violation::
 
             IF  ${var} == 4
                 Keyword
             END
             # comments are ignored
             IF  ${var}  == 4
                 Keyword 2
             END
 
-        IF statement is considered identical only if all branches have identical conditions.
+        ``IF`` statement is considered identical only if all branches have identical conditions.
 
-        Similar but not identical IF::
+        Similar but not identical ``IF``::
 
             IF  ${variable}
                 Keyword
             ELSE
                 Other Keyword
             END
             IF  ${variable}
                 Keyword
             END
 
         """,
+        added_in_version="2.0.0",
     ),
     "0915": Rule(
         rule_id="0915",
         name="statement-outside-loop",
         msg="{{ name }} {{ statement_type }} used outside a loop",
         severity=RuleSeverity.ERROR,
         version=">=5.0",
         docs="""
         Following keywords and statements should only be used inside loop (``WHILE`` or ``FOR``):
-            - ``Exit For Loop``,
-            - ``Exit For Loop If``,
-            - ``Continue For Loop``,
+            - ``Exit For Loop``
+            - ``Exit For Loop If``
+            - ``Continue For Loop``
             - ``Continue For Loop If``
-            - ``CONTINUE``,
+            - ``CONTINUE``
             - ``BREAK``
 
         """,
+        added_in_version="2.0.0",
     ),
     "0916": Rule(
         RuleParam(
             name="max_width",
             default=80,
             converter=int,
             desc="maximum width of IF (in characters) below which it will be recommended to use inline IF",
@@ -278,36 +288,37 @@
         SeverityThreshold("max_width", compare_method="less"),
         rule_id="0916",
         name="inline-if-can-be-used",
         msg="IF can be replaced with inline IF",
         severity=RuleSeverity.INFO,
         version=">=5.0",
         docs="""
-        Short and simple IFs can be replaced with inline IF.
+        Short and simple ``IF`` statements can be replaced with ``inline IF``.
 
-        Following IF::
+        Following ``IF``::
 
             IF    $condition
                 BREAK
             END
 
         can be replaced with::
 
             IF    $condition    BREAK
 
         """,
+        added_in_version="2.0.0",
     ),
     "0917": Rule(
         rule_id="0917",
         name="unreachable-code",
         msg="Unreachable code after {{ statement }} statement",
         severity=RuleSeverity.WARNING,
         version=">=5.0",
         docs="""
-        Detect the unreachable code after RETURN, BREAK or CONTINUE statements.
+        Detect the unreachable code after ``RETURN``, ``BREAK`` or ``CONTINUE`` statements.
 
         For example::
 
             Example Keyword
                 FOR    ${animal}    IN    cat    dog
                     IF    '${animal}' == 'cat'
                         CONTINUE
@@ -316,42 +327,44 @@
                     BREAK
                     Log    Unreachable log
                 END
                 RETURN
                 Log    Unreachable log
 
         """,
+        added_in_version="3.1.0",
     ),
     "0918": Rule(
         rule_id="0918",
         name="multiline-inline-if",
         msg="Avoid splitting inline IF to multiple lines",
         severity=RuleSeverity.WARNING,
         version=">=5.0",
         docs="""
-        It's allowed to create inline IF that spans multiple lines, but it should be avoided,
-        since it decreases readability. Try to use normal IF/ELSE instead.
+        It's allowed to create ``inline IF`` that spans multiple lines, but it should be avoided,
+        since it decreases readability. Try to use normal ``IF``/``ELSE`` instead.
 
         Bad::
 
             IF  ${condition}  Log  hello
             ...    ELSE       Log  hi!
 
         Good::
 
             IF  ${condition}    Log  hello     ELSE    Log  hi!
 
-        or::
+        or also good::
 
             IF  ${condition}
                 Log  hello
             ELSE
                 Log  hi!
             END
         """,
+        added_in_version="3.1.0",
     ),
     "0919": Rule(
         rule_id="0919",
         name="unused-argument",
         msg="Keyword argument '{{ name }}' is not used",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -365,14 +378,15 @@
                     Log    Escaped syntax is supported.
                 END
 
             Keyword with ${embedded} and ${not_used}  # will report ${not_used}
                 Log    ${embedded}
 
         """,
+        added_in_version="3.2.0",
     ),
     "0920": Rule(
         rule_id="0920",
         name="unused-variable",
         msg="Variable '{{ name }}' is assigned but not used",
         severity=RuleSeverity.INFO,
         docs="""
@@ -391,14 +405,15 @@
             Process Value 10 Times
                 [Arguments]    ${value}
                 FOR    ${_}   IN RANGE    10
                     Process Value    ${value}
                 END
 
     """,
+        added_in_version="3.2.0",
     ),
     "0921": Rule(
         rule_id="0921",
         name="argument-overwritten-before-usage",
         msg="Keyword argument '{{ name }}' is overwritten before usage",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -406,38 +421,165 @@
         
             *** Keywords ***
             Overwritten Argument
                 [Arguments]    ${overwritten}  # we do not use ${overwritten} value at all
                 ${overwritten}    Set Variable    value  # we only overwrite it
 
         """,
+        added_in_version="3.2.0",
     ),
     "0922": Rule(
         rule_id="0922",
         name="variable-overwritten-before-usage",
         msg="Local variable '{{ name }}' is overwritten before usage",
         severity=RuleSeverity.WARNING,
         docs="""
         Local variable in Keyword, Test Case or Task is overwritten before it is used::
 
             *** Keywords ***
             Overwritten Variable
                 ${value}    Keyword
                 ${value}    Keyword
 
-        In case the value of the variable is not important, it is possible to use `${_}` name::
+        In case the value of the variable is not important, it is possible to use ``${_}`` name::
         
             *** Test Cases ***
             Call keyword and ignore some return values
                 ${_}    ${item}    Unpack List    @{LIST}
                 FOR    ${_}    IN RANGE  10
                     Log    Run this code 10 times.
                 END
 
         """,
+        added_in_version="3.2.0",
+    ),
+    "0923": Rule(
+        rule_id="0923",
+        name="unnecessary-string-conversion",
+        msg="Variable '{{ name }}' in '{{ block_name }}' condition has unnecessary string conversion",
+        severity=RuleSeverity.INFO,
+        version=">=4.0",
+        docs="""
+        Expressions in Robot Framework are evaluated using Python's eval function. When a variable is used
+        in the expression using the normal ``${variable}`` syntax, its value is replaced before the expression
+        is evaluated. For example, with the following expression::
+        
+            *** Test Cases ***
+            Check if schema was uploaded
+                Upload Schema    schema.avsc
+                Check If File Exist In SFTP    schema.avsc
+        
+            *** Keywords ***
+            Upload Schema
+                [Arguments]    ${filename}
+                IF    ${filename} == 'default'
+                    ${filename}    Get Default Upload Path
+                END
+                Send File To SFTP Root   ${filename}
+        
+        "${filename}" will be replaced by "schema.avsc"::
+        
+            IF    schema.avsc == 'default'
+        
+        "schema.avsc" will not be recognized as Python variable. That's why you need to quote it::
+        
+            IF    '${filename}' == 'default'
+        
+        However it introduces unnecessary string conversion and can mask difference in the type. For example::
+        
+            ${numerical}    Set Variable    10  # ${numerical} is actually string 10, not integer 10
+            IF    "${numerical}" == "10"
+
+        You can use  ``$variable`` syntax instead::
+        
+            IF    $numerical == 10
+        
+        It will put the actual variable in the evaluated expression without converting it to string.
+        """,
+        added_in_version="4.0.0",
+    ),
+    "0924": Rule(
+        rule_id="0924",
+        name="expression-can-be-simplified",
+        msg="'{{ block_name }}' condition can be simplified",
+        severity=RuleSeverity.INFO,
+        version=">=4.0",
+        docs="""
+        Evaluated expression can be simplified. For example::
+        
+            *** Keywords ***
+            Click On Element
+                [Arguments]    ${locator}
+                IF    ${is_element_visible}==${TRUE}    RETURN
+                ${is_element_enabled}    Set Variable    ${TRUE}
+                WHILE    ${is_element_enabled} != ${TRUE}
+                    ${is_element_enabled}    Get Element Status    ${locator}
+                END
+                Click    ${locator}
+        
+        can be rewritten to::
+        
+            *** Keywords ***
+            Click On Element
+                [Arguments]    ${locator}
+                IF    ${is_element_visible}    RETURN
+                ${is_element_enabled}    Set Variable    ${FALSE}
+                WHILE    not ${is_element_enabled}
+                    ${is_element_enabled}    Get Element Status    ${locator}
+                END
+                Click    ${locator}
+
+        Comparisons to empty sequences (lists, dicts, sets), empty string or ``0`` can be also simplified::
+        
+            *** Test Cases ***
+            Check conditions
+                Should Be True     ${list} == []  # equivalent of 'not ${list}'
+                Should Be True     ${string} != ""  # equivalent of '${string}'
+                Should Be True     len(${sequence}))  # equivalent of '${sequence}'
+
+        """,
+        added_in_version="4.0.0",
+    ),
+    "0925": Rule(
+        rule_id="0925",
+        name="misplaced-negative-condition",
+        msg="'{{ block_name }}' condition '{{ original_condition }}' can be rewritten to '{{ proposed_condition }}'",
+        severity=RuleSeverity.INFO,
+        version=">=4.0",
+        docs="""
+        Position of not operator can be changed for better readability.
+        
+        For example::
+        
+            *** Keywords ***
+            Check Unmapped Codes
+                ${codes}    Get Codes From API
+                IF    not ${codes} is None
+                    FOR    ${code}    IN    @{codes}
+                        Validate Single Code    ${code}
+                    END
+                ELSE
+                    Fail    Did not receive codes from API.
+                END
+        
+        Can be rewritten to::
+        
+            *** Keywords ***
+            Check Unmapped Codes
+                ${codes}    Get Codes From API
+                IF    ${codes} is not None
+                    FOR    ${code}    IN    @{codes}
+                        Validate Single Code    ${code}
+                    END
+                ELSE
+                    Fail    Did not receive codes from API.
+                END
+
+        """,
+        added_in_version="4.0.0",
     ),
 }
 
 
 class ReturnChecker(VisitorChecker):
     """Checker for [Return] and Return From Keyword violations."""
 
@@ -963,15 +1105,15 @@
 
     def visit_If(self, node):  # noqa
         if node.header.errors:
             return node
         for token in node.header.get_tokens(Token.ARGUMENT):
             self.find_not_nested_variable(token.value, is_var=False)
         for token in node.header.get_tokens(Token.ASSIGN):
-            self.handle_assign_variable(token, remove_equal=True)
+            self.handle_assign_variable(token)
         self.variables.append({})
         for item in node.body:
             self.visit(item)
         self.variables.pop()
         if node.orelse:
             self.visit(node.orelse)
 
@@ -996,72 +1138,72 @@
         if getattr(node.header, "errors", None):
             return node
         self.in_loop = True
         self.ignore_overwriting = True
         for token in node.header.get_tokens(Token.ARGUMENT):
             self.find_not_nested_variable(token.value, is_var=False)
         for token in node.header.get_tokens(Token.VARIABLE):
-            self.handle_assign_variable(token, remove_equal=False)
+            self.handle_assign_variable(token)
         self.generic_visit(node)
         self.ignore_overwriting = False
         self.in_loop = False
         self.clear_variables_after_loop()
 
     visit_ForLoop = visit_For
 
     def visit_Try(self, node):  # noqa
         if node.errors or node.header.errors:
             return node
         if node.variable is not None:
             error_var = node.header.get_token(Token.VARIABLE)
             if error_var is not None:
-                self.handle_assign_variable(error_var, remove_equal=False)
+                self.handle_assign_variable(error_var)
         return self.generic_visit(node)
 
     def visit_KeywordCall(self, node):  # noqa
         for token in node.get_tokens(Token.ARGUMENT, Token.KEYWORD):  # argument can be used in keyword name
             self.find_not_nested_variable(token.value, is_var=False)
         for token in node.get_tokens(Token.ASSIGN):  # we first check args, then assign for used and then overwritten
-            self.handle_assign_variable(token, remove_equal=True)
+            self.handle_assign_variable(token)
 
     def visit_Return(self, node):  # noqa
         for token in node.get_tokens(Token.ARGUMENT):
             self.find_not_nested_variable(token.value, is_var=False)
 
     visit_ReturnStatement = visit_Teardown = visit_Timeout = visit_Return
 
     def visit_TemplateArguments(self, node):  # noqa
         for argument in node.data_tokens:
             self.find_not_nested_variable(argument.value, is_var=False)
 
-    def handle_assign_variable(self, token, remove_equal):
+    def handle_assign_variable(self, token):
         """Check if assign does not overwrite arguments or variables.
 
         Store assign variables for future overwriting checks."""
         value = token.value
-        if remove_equal:
-            value = value.rstrip("=").strip()  # remove possible '=' and ' ='
-        normalized = normalize_robot_var_name(value)  # remove ${ } and normalize
+        variable_match = search_variable(value, ignore_errors=True)
+        normalized = normalize_robot_name(variable_match.base)
         if not normalized:  # ie. "${_}" -> ""
             return
         arg = self.arguments.pop(normalized, None)
         if arg is not None:
             self.report_arg_or_var_rule("argument-overwritten-before-usage", arg.token)
         is_used = False
-        for variable_scope in self.variables[::-1]:
-            if normalized in variable_scope:
-                is_used = variable_scope[normalized].is_used or is_used
-                if not variable_scope[normalized].is_used and not self.ignore_overwriting:
-                    self.report_arg_or_var_rule(
-                        "variable-overwritten-before-usage", variable_scope[normalized].token, value
-                    )
+        if not variable_match.items:  # not item assignment like ${var}[1] =
+            for variable_scope in self.variables[::-1]:
+                if normalized in variable_scope:
+                    is_used = variable_scope[normalized].is_used or is_used
+                    if not variable_scope[normalized].is_used and not self.ignore_overwriting:
+                        self.report_arg_or_var_rule(
+                            "variable-overwritten-before-usage", variable_scope[normalized].token, variable_match.name
+                        )
         if self.in_loop:
-            variable = CachedVariable(value, token, is_used)
+            variable = CachedVariable(variable_match.name, token, is_used)
         else:
-            variable = CachedVariable(value, token, False)
+            variable = CachedVariable(variable_match.name, token, False)
         self.variables[-1][normalized] = variable
 
     def find_not_nested_variable(self, value, is_var):
         """Find and process not nested variable.
 
         Search `value` string until there is ${variable} without other variables inside. Unescaped escaped syntax
         ($var or \\${var}). If variable does exist in assign variables or arguments, it is removed to denote it was
@@ -1132,7 +1274,108 @@
         for attr_access in (".", "[", "(", "%", "+", "-", "*", "/"):  # ${arg.attr}
             if attr_access in variable_name:
                 name, _ = variable_name.split(attr_access, maxsplit=1)
                 name = name.strip()
                 if name in variable_scope:
                     variable_scope[name].is_used = True
                     return
+
+
+class ExpressionsChecker(VisitorChecker):
+    reports = ("unnecessary-string-conversion", "expression-can-be-simplified", "misplaced-negative-condition")
+    QUOTE_CHARS = {"'", '"'}
+    CONDITION_KEYWORDS = {"passexecutionif", "setvariableif", "shouldbetrue", "shouldnotbetrue", "skipif"}
+    COMPARISON_SIGNS = {"==", "!="}
+    EMPTY_COMPARISON = {"${true}", "${false}", "true", "false", "[]", "{}", "set()", "list()", "dict()", "0"}
+
+    def visit_If(self, node):  # noqa
+        condition_token = node.header.get_token(Token.ARGUMENT)
+        self.check_condition(node.header.type, condition_token, node.condition)
+        self.generic_visit(node)
+
+    visit_While = visit_If
+
+    def visit_KeywordCall(self, node):  # noqa
+        normalized_name = normalize_robot_name(node.keyword, remove_prefix="builtin.")
+        if normalized_name not in self.CONDITION_KEYWORDS:
+            return
+        condition_token = node.get_token(Token.ARGUMENT)
+        self.check_condition(node.keyword, condition_token, condition_token.value)
+        if normalized_name == "setvariableif":
+            arguments = node.get_tokens(Token.ARGUMENT)
+            if len(arguments) < 4:
+                return
+            for condition_token in arguments[2::2]:
+                self.check_condition(node.keyword, condition_token, condition_token.value)
+
+    def check_condition(self, node_name, condition_token, condition):
+        if not condition:
+            return
+        try:
+            variables = list(VariableIterator(condition))
+        except VariableError:  # for example ${variable which wasn't closed properly
+            return
+        position = condition_token.col_offset + 1
+        for before, variable, remaining in variables:
+            position += len(before)
+            self.check_for_misplaced_not(condition_token, node_name, before, variable, remaining)
+            self.check_for_complex_condition(condition_token, node_name, before, variable, remaining, position)
+            if not before or not remaining:
+                continue
+            if before[-1] in self.QUOTE_CHARS and before[-1] == remaining[0]:
+                self.report(
+                    "unnecessary-string-conversion",
+                    name=variable,
+                    block_name=node_name,
+                    node=condition_token,
+                    col=position,
+                    end_col=position + len(variable),
+                )
+
+    def check_for_misplaced_not(self, condition_token, node_name, left_side, variable, right_side):
+        """Check if the condition contains misplaced not.
+
+        An example of misplaced condition would be 'not ${variable} is None'.
+        """
+        if not (left_side.endswith("not ") and right_side.startswith(" is ")):
+            return
+        right_tokens = right_side.split(" ")
+        orig_right_side = " ".join(right_tokens[1:3])
+        original_condition = f"not {variable} {orig_right_side}"
+        proposed_condition = f"{variable} is not {right_tokens[2]}"
+        self.report(
+            "misplaced-negative-condition",
+            block_name=node_name,
+            original_condition=original_condition,
+            proposed_condition=proposed_condition,
+            node=condition_token,
+            col=condition_token.col_offset + 1,
+            end_col=condition_token.end_col_offset + 1,
+        )
+
+    def check_for_complex_condition(self, condition_token, node_name, left_side, variable, right_side, position):
+        """Check if right side of the equation can be simplified."""
+        if not right_side:
+            return
+        normalized = right_side.lower().lstrip()  # ' == ${TRUE}' -> '== ${true}'
+        if len(normalized) < 3:
+            if normalized == ")" and left_side.endswith("len("):
+                self.report(
+                    "expression-can-be-simplified",
+                    block_name=node_name,
+                    node=condition_token,
+                    col=position - len("len("),
+                    end_col=position + len(variable) + 1,
+                )
+            return
+        equation = normalized[:2]  # '=='
+        compared_value = normalized[2:].lstrip()  # '${true}'
+        if equation not in self.COMPARISON_SIGNS:
+            return
+        if compared_value in self.EMPTY_COMPARISON:
+            self.report(
+                "expression-can-be-simplified",
+                block_name=node_name,
+                node=condition_token,
+                col=position,
+                end_col=position + len(variable) + len(right_side),
+            )
```

### Comparing `robotframework-robocop-3.2.1/robocop/checkers/naming.py` & `robotframework-robocop-4.0.0/robocop/checkers/naming.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 import string
 from collections import defaultdict
 from pathlib import Path
 
 from robot.api import Token
 from robot.errors import VariableError
+from robot.parsing.model.blocks import TestCaseSection
 from robot.parsing.model.statements import Arguments
 from robot.variables import VariableIterator
 from robot.variables.search import search_variable
 
 from robocop.checkers import VisitorChecker
 from robocop.rules import Rule, RuleParam, RuleSeverity
 from robocop.utils import (
@@ -37,22 +38,23 @@
             desc="pattern defining characters (not) allowed in a name",
         ),
         rule_id="0301",
         name="not-allowed-char-in-name",
         msg="Not allowed character '{{ character }}' found in {{ block_name }} name",
         severity=RuleSeverity.WARNING,
         docs="""
-        Reports not allowed pattern found in Test Case or Keyword names. By default it's dot (`.`). You can
+        Reports not allowed pattern found in Test Case or Keyword names. By default it's dot (``.``). You can
         configure what patterns are reported by calling::
 
              robocop --configure not-allowed-char-in-name:pattern:regex_pattern
 
-        `regex_pattern` should define regex pattern not allowed in names. For example `[@\[]` pattern
-        reports any occurrence of `@[` characters.
+        ``regex_pattern`` should define regex pattern not allowed in names. For example ``[@\[]`` pattern
+        reports any occurrence of ``@[`` characters.
         """,
+        added_in_version="1.0.0",
     ),
     "0302": Rule(
         RuleParam(
             name="convention",
             default="each_word_capitalized",
             converter=str,
             desc="possible values: 'each_word_capitalized' (default) or 'first_word_capitalized'",
@@ -64,14 +66,15 @@
             show_type="regex",
             desc="pattern for accepted words in keyword",
         ),
         rule_id="0302",
         name="wrong-case-in-keyword-name",
         msg="Keyword name '{{ keyword_name }}' does not follow case convention",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "0303": Rule(
         rule_id="0303",
         name="keyword-name-is-reserved-word",
         msg="'{{ keyword_name }}' is a reserved keyword{{ error_msg }}",
         severity=RuleSeverity.ERROR,
         docs="""
@@ -85,14 +88,15 @@
           - WHILE
           - CONTINUE
           - RETURN
           - TRY
           - EXCEPT
 
         """,
+        added_in_version="1.0.0",
     ),
     "0305": Rule(
         rule_id="0305",
         name="underscore-in-keyword-name",
         msg="Underscores in keyword name '{{ keyword_name }}' can be replaced with spaces",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -101,14 +105,15 @@
             # bad
             keyword_with_underscores
 
             # good
             Keyword Without Underscores
 
         """,
+        added_in_version="1.0.0",
     ),
     "0306": Rule(
         rule_id="0306",
         name="setting-name-not-in-title-case",
         msg="Setting name '{{ setting_name }}' should use title or upper case",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -129,14 +134,15 @@
 
              *** Test Cases ***
              Test
                  [documentation]  Some documentation
                  Step
 
         """,
+        added_in_version="1.0.0",
     ),
     "0307": Rule(
         rule_id="0307",
         name="section-name-invalid",
         msg="Section name should be in format '{{ section_title_case }}' or '{{ section_upper_case }}'",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -146,26 +152,29 @@
             *** Keywords ***
 
         Bad::
 
             *** keywords ***
 
         """,
+        added_in_version="1.0.0",
     ),
     "0308": Rule(
         rule_id="0308",
         name="not-capitalized-test-case-title",
         msg="Test case '{{ test_name }}' title should start with capital letter",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.4.0",
     ),
     "0309": Rule(
         rule_id="0309",
         name="section-variable-not-uppercase",
         msg="Section variable '{{ variable_name }}' name should be uppercase",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.4.0",
     ),
     "0310": Rule(
         rule_id="0310",
         name="non-local-variables-should-be-uppercase",
         msg="Test, suite and global variables should be uppercase",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -180,32 +189,36 @@
 
             Set Task Variable    ${my_var}           1
             Set Suite Variable   ${My Var}           1
             Set Test Variable    ${myvar}            1
             Set Global Variable  ${my_var${NESTED}}  1
 
         """,
+        added_in_version="1.4.0",
     ),
     "0311": Rule(
         rule_id="0311",
         name="else-not-upper-case",
         msg="ELSE and ELSE IF should be upper case",
         severity=RuleSeverity.ERROR,
+        added_in_version="1.5.0",
     ),
     "0312": Rule(
         rule_id="0312",
         name="keyword-name-is-empty",
         msg="Keyword name should not be empty",
         severity=RuleSeverity.ERROR,
+        added_in_version="1.8.0",
     ),
     "0313": Rule(
         rule_id="0313",
         name="test-case-name-is-empty",
         msg="Test case name should not be empty",
         severity=RuleSeverity.ERROR,
+        added_in_version="1.8.0",
     ),
     "0314": Rule(
         rule_id="0314",
         name="empty-library-alias",
         msg="Library alias should not be empty",
         severity=RuleSeverity.ERROR,
         docs="""
@@ -218,65 +231,69 @@
 
         Bad::
 
              *** Settings ***
              Library  CustomLibrary  AS
 
         """,
+        added_in_version="1.10.0",
     ),
     "0315": Rule(
         rule_id="0315",
         name="duplicated-library-alias",
         msg="Library alias should not be the same as original name",
         severity=RuleSeverity.WARNING,
         docs="""
         Example of rule violation::
 
              *** Settings ***
-             Library  CustomLibrary  AS  CustomLibrary  # same as library name
+             Library  CustomLibrary  AS  CustomLibrary   # same as library name
              Library  CustomLibrary  AS  Custom Library  # same as library name (spaces are ignored)
 
         """,
+        added_in_version="1.10.0",
     ),
     "0316": Rule(
         rule_id="0316",
         name="possible-variable-overwriting",
         msg="Variable '{{ variable_name }}' may overwrite similar variable inside '{{ block_name }}' {{ block_type }}. "
         "Note that variables are case-insensitive, and also spaces and underscores are ignored.",
         severity=RuleSeverity.INFO,
         docs="""
         Following assignments overwrite the same variable::
-        
+
             *** Keywords ***
             Keyword
-                ${variable}    Keyword Call
-                ${VARIABLE}    Keyword Call
+                ${variable}      Keyword Call
+                ${VARIABLE}      Keyword Call
                 ${vari_ab le}    Keyword Call
-        
+
         Use consistent variable naming guidelines to avoid unintended variable overwriting.
         Remember that variable names in Robot Framework are case-insensitive and
         underscores and whitespaces are ignored.
         """,
+        added_in_version="1.10.0",
     ),
     "0317": Rule(
         rule_id="0317",
         name="hyphen-in-variable-name",
         msg="Use underscore in variable name '{{ variable_name }}' instead of hyphens to "
         "avoid treating them like minus sign",
         severity=RuleSeverity.INFO,
         docs="""
         Robot Framework supports evaluation of Python code inside ${ } brackets. For example::
 
-             ${var2}  Set Variable  ${${var}-${var2}}
+            ${var2}  Set Variable  ${${var}-${var2}}
 
         That's why there is possibility that hyphen in name is not recognized as part of name but as minus sign.
         Better to use underscore (if it's intended)::
 
-        ${var2}  Set Variable  ${ ${var}_${var2}}
+            ${var2}  Set Variable  ${${var}_${var2}}
         """,
+        added_in_version="1.10.0",
     ),
     "0318": Rule(
         rule_id="0318",
         name="bdd-without-keyword-call",
         msg="BDD reserved keyword '{{ keyword_name }}' not followed by any keyword{{ error_msg }}",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -293,21 +310,23 @@
 
             Given
             When User Log In
             Then User Should See Welcome Page
 
         Since those words are used for BDD style it's also recommended not to use them within the keyword name.
         """,
+        added_in_version="1.11.0",
     ),
     "0319": Rule(
         rule_id="0319",
         name="deprecated-statement",
         msg="'{{ statement_name }}' is deprecated since Robot Framework version "
         "{{ version }}, use '{{ alternative }}' instead",
         severity=RuleSeverity.WARNING,
+        added_in_version="2.0.0",
     ),
     "0320": Rule(
         RuleParam(
             name="pattern",
             default=re.compile(r"[\.\?]"),
             converter=pattern_type,
             show_type="regex",
@@ -319,17 +338,18 @@
         severity=RuleSeverity.WARNING,
         docs="""
         Reports not allowed pattern found in Suite names. By default it's dot (`.`). You can
         configure what characters are reported by calling::
 
              robocop --configure not-allowed-char-in-filename:pattern:regex_pattern
 
-        `regex_pattern` should define regex pattern for characters not allowed in names. For example `[@\[]` pattern
-        reports any occurrence of `@[` characters.
+        ``regex_pattern`` should define regex pattern for characters not allowed in names. For example `[@\[]` pattern
+        reports any occurrence of ``@[`` characters.
         """,
+        added_in_version="2.1.0",
     ),
     "0321": Rule(
         rule_id="0321",
         name="deprecated-with-name",
         msg=(
             "'WITH NAME' alias marker is deprecated since Robot Framework 6.0 version "
             "and will be removed in the future release. Use 'AS' instead"
@@ -347,26 +367,28 @@
 
         Code with the supported marker::
 
             *** Settings ***
             Library    Collections    AS    AliasedName
 
         """,
+        added_in_version="2.5.0",
     ),
     "0322": Rule(
         rule_id="0322",
         name="deprecated-singular-header",
         msg="'{{ singular_header }}' singular header form is deprecated since RF 6.0 and "
         "will be removed in the future releases. Use '{{ plural_header }}' instead",
         severity=RuleSeverity.WARNING,
         version=">=6.0",
         docs="""
         Robot Framework 6.0 starts deprecation period for singular headers forms. The rationale behind this change
         is available at https://github.com/robotframework/robotframework/issues/4431 .
         """,
+        added_in_version="2.6.0",
     ),
     "0323": Rule(
         rule_id="0323",
         name="inconsistent-variable-name",
         msg="Variable '{{ name }}' has inconsistent naming. First used as '{{ first_use }}'",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -382,47 +404,62 @@
                 ${variable}    Keyword Call
                 IF    ${ARGUMENT}  # inconsistent name with ${argument}
                     Should Be True    ${vari_able}  # inconsistent name with ${variable}
                 END
                 Log    ${variable}  # consistent name
 
         """,
+        added_in_version="3.2.0",
     ),
     "0324": Rule(
         rule_id="0324",
         name="overwriting-reserved-variable",
         msg="{{ var_or_arg }} '{{ variable_name }}' overwrites reserved variable '{{ reserved_variable }}'",
         severity=RuleSeverity.WARNING,
         docs="""
         Overwriting reserved variables may bring unexpected results.
         For example, overwriting variable with name ``${LOG_LEVEL}`` can break Robot Framework logging.
         See full list of reserved variables at
         `Robot Framework User Guide <https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#automatic-variables>`_
         """,
+        added_in_version="3.2.0",
     ),
     "0325": Rule(
         rule_id="0325",
         name="invalid-section",
-        msg="Invalid section '{{ invalid_section }}'. Consider using --language parameter if the file is defined with different language.",
+        msg="Invalid section '{{ invalid_section }}'. Consider using --language parameter if the file is defined with different language",
         severity=RuleSeverity.ERROR,
         version=">=6.1",
         docs="""
-            Robot Framework 6.1 detects unrecognized sections based on the language defined for the specific files.
-            Consider using --language parameter if the file is defined with different language.
-            
-            It is also possible to configure language in the file:
+        Robot Framework 6.1 detects unrecognized sections based on the language defined for the specific files.
+        Consider using ``--language`` parameter if the file is defined with different language.
+        
+        It is also possible to configure language in the file::
             
-            ```
             language: pl
             
             *** Przypadki Testowe ***
             Test case
                 Step
-            ```
-            """,
+
+        """,
+        added_in_version="3.2.0",
+    ),
+    "0326": Rule(
+        rule_id="0326",
+        name="mixed-task-test-settings",
+        msg="Use {{ task_or_test }}-related setting '{{ setting }}' if {{ tasks_or_tests }} section is used",
+        severity=RuleSeverity.WARNING,
+        docs="""
+        If ``*** Tasks ***`` section is present in the file, use task-related settings like ``Task Setup``,
+        ``Task Teardown``, ``Task Template``, ``Task Tags`` and ``Task Timeout`` instead of their `Test` variants.
+
+        Similarly, use test-related settings when using ``*** Test Cases ***`` section.
+        """,
+        added_in_version="3.3.0",
     ),
 }
 
 SET_VARIABLE_VARIANTS = {
     "settaskvariable",
     "settestvariable",
     "setsuitevariable",
@@ -629,21 +666,23 @@
 
     reports = (
         "setting-name-not-in-title-case",
         "section-name-invalid",
         "empty-library-alias",
         "duplicated-library-alias",
         "invalid-section",
+        "mixed-task-test-settings",
     )
     ALIAS_TOKENS = [Token.WITH_NAME] if ROBOT_VERSION.major < 5 else [Token.WITH_NAME, "AS"]
     # Separating alias values since RF 3 uses WITH_NAME instead of WITH NAME
     ALIAS_TOKENS_VALUES = ["WITH NAME"] if ROBOT_VERSION.major < 5 else [Token.WITH_NAME, "AS"]
 
     def __init__(self):
         self.section_name_pattern = re.compile(r"\*\*\*\s.+\s\*\*\*")
+        self.task_section = False
         super().__init__()
 
     def visit_InvalidSection(self, node):  # noqa
         name = node.header.data_tokens[0].value
         invalid_header = node.header.get_token(Token.INVALID_HEADER)
         if "Resource file with" in invalid_header.error:
             return
@@ -664,26 +703,44 @@
                 "section-name-invalid",
                 section_title_case=valid_name,
                 section_upper_case=valid_name.upper(),
                 node=node,
                 end_col=node.col_offset + len(name) + 1,
             )
 
+    def visit_File(self, node):  # noqa
+        for section in node.sections:
+            if isinstance(section, TestCaseSection):
+                if (ROBOT_VERSION.major < 6 and "task" in section.header.name.lower()) or (
+                    ROBOT_VERSION.major >= 6 and section.header.type == Token.TASK_HEADER
+                ):
+                    self.task_section = True
+            else:
+                self.task_section = False
+        super().visit_File(node)
+
     def visit_Setup(self, node):  # noqa
         self.check_setting_name(node.data_tokens[0].value, node)
+        self.check_settings_consistency(node.data_tokens[0].value, node)
 
     visit_SuiteSetup = (
         visit_TestSetup
     ) = (
         visit_Teardown
     ) = (
         visit_SuiteTeardown
     ) = (
         visit_TestTeardown
     ) = (
+        visit_TestTimeout
+    ) = (
+        visit_TestTemplate
+    ) = (
+        visit_TestTags
+    ) = (
         visit_ForceTags
     ) = (
         visit_DefaultTags
     ) = (
         visit_ResourceImport
     ) = (
         visit_VariablesImport
@@ -716,14 +773,32 @@
     def check_setting_name(self, name, node):
         if not (name.istitle() or name.isupper()):
             col = node.tokens[0].end_col_offset if node.tokens[0].type == "SEPARATOR" else node.col_offset
             self.report(
                 "setting-name-not-in-title-case", setting_name=name, node=node, col=col + 1, end_col=col + len(name) + 1
             )
 
+    def check_settings_consistency(self, name, node):
+        if "test" in name.lower() and self.task_section:
+            self.report(
+                "mixed-task-test-settings",
+                setting="Task " + name.split()[1],
+                task_or_test="task",
+                tasks_or_tests="Tasks",
+                node=node,
+            )
+        elif "task" in name.lower() and not self.task_section:
+            self.report(
+                "mixed-task-test-settings",
+                setting="Test " + name.split()[1],
+                task_or_test="test",
+                tasks_or_tests="Test Cases",
+                node=node,
+            )
+
 
 class TestCaseNamingChecker(VisitorChecker):
     """Checker for test case naming violations."""
 
     reports = (
         "not-capitalized-test-case-title",
         "test-case-name-is-empty",
@@ -795,27 +870,19 @@
             self.report(
                 "section-variable-not-uppercase",
                 variable_name=token.value.strip(),
                 lineno=token.lineno,
                 col=token.col_offset + 1,
                 end_col=token.col_offset + len(token.value) + 1,
             )
-        self.check_for_reserved_naming(token, "Variable")
+        self.check_for_reserved_naming_or_hyphen(token, "Variable")
 
     def visit_KeywordCall(self, node):  # noqa
         for token in node.get_tokens(Token.ASSIGN):
-            if "-" in token.value:
-                self.report(
-                    "hyphen-in-variable-name",
-                    variable_name=token.value,
-                    lineno=token.lineno,
-                    col=token.col_offset + 1,
-                    end_col=token.end_col_offset + 1,
-                )
-            self.check_for_reserved_naming(token, "Variable")
+            self.check_for_reserved_naming_or_hyphen(token, "Variable", is_assign=True)
 
         if not node.keyword:
             return
         if normalize_robot_name(node.keyword, remove_prefix="builtin.") in SET_VARIABLE_VARIANTS:
             if len(node.data_tokens) < 2:
                 return
             token = node.data_tokens[1]
@@ -836,50 +903,58 @@
                     node=node,
                     col=token.col_offset + 1,
                     end_col=token.end_col_offset + 1,
                 )
 
     def visit_If(self, node):  # noqa
         for token in node.header.get_tokens(Token.ASSIGN):
-            self.check_for_reserved_naming(token, "Variable")
+            self.check_for_reserved_naming_or_hyphen(token, "Variable")
         self.generic_visit(node)
 
     def visit_Arguments(self, node):  # noqa
         for arg in node.get_tokens(Token.ARGUMENT):
-            self.check_for_reserved_naming(arg, "Argument")
+            self.check_for_reserved_naming_or_hyphen(arg, "Argument")
 
     def parse_embedded_arguments(self, name_token):
         """Store embedded arguments from keyword name. Ignore embedded variables patterns like (${var:pattern})."""
         try:
             for token in name_token.tokenize_variables():
                 if token.type == Token.VARIABLE:
-                    self.check_for_reserved_naming(token, "Embedded argument", has_pattern=True)
+                    self.check_for_reserved_naming_or_hyphen(token, "Embedded argument", has_pattern=True)
         except VariableError:
             pass
 
-    def check_for_reserved_naming(self, token, var_or_arg, has_pattern=False):
-        """Check if variable name is a reserved Robot Framework name."""
-        name, *_ = token.value.split("=", maxsplit=1)
-        name = name.rstrip()
+    def check_for_reserved_naming_or_hyphen(self, token, var_or_arg, has_pattern=False, is_assign=False):
+        """Check if variable name is a reserved Robot Framework name or uses hyphen in the name."""
+        variable_match = search_variable(token.value, ignore_errors=True)
+        name = variable_match.base
         if has_pattern:
-            name, *pattern = name.split(":", maxsplit=1)
-            if pattern:
-                name += "}"  # recreate, so it handles ${variable:pattern} -> ${variable} matching
-        normalized_name = normalize_robot_var_name(name)
+            name, *_ = name.split(":", maxsplit=1)  # var:pattern -> var
+        if is_assign and "-" in variable_match.base:
+            self.report(
+                "hyphen-in-variable-name",
+                variable_name=token.value,
+                lineno=token.lineno,
+                col=token.col_offset + 1,
+                end_col=token.end_col_offset + 1,
+            )
+        if variable_match.items:  # item assignments ${dict}[key] =
+            return
+        normalized_name = normalize_robot_name(name)
         if normalized_name in self.RESERVED_VARIABLES:
             reserved_variable = self.RESERVED_VARIABLES[normalized_name]
             self.report(
                 "overwriting-reserved-variable",
                 var_or_arg=var_or_arg,
-                variable_name=name,
+                variable_name=variable_match.match,
                 reserved_variable=reserved_variable,
                 node=token,
                 lineno=token.lineno,
                 col=token.col_offset + 1,
-                end_col=token.col_offset + len(name) + 1,
+                end_col=token.col_offset + len(variable_match.match) + 1,
             )
 
 
 class SimilarVariableChecker(VisitorChecker):
     """Checker for finding same variables with similar names."""
 
     reports = ("possible-variable-overwriting", "inconsistent-variable-name")
```

### Comparing `robotframework-robocop-3.2.1/robocop/checkers/spacing.py` & `robotframework-robocop-4.0.0/robocop/checkers/spacing.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,62 +23,68 @@
 
 rules = {
     "1001": Rule(
         rule_id="1001",
         name="trailing-whitespace",
         msg="Trailing whitespace at the end of line",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "1002": Rule(
         rule_id="1002",
         name="missing-trailing-blank-line",
         msg="Missing trailing blank line at the end of file",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "1003": Rule(
         RuleParam(
             name="empty_lines",
             default=2,
             converter=int,
             desc="number of empty lines required between sections",
         ),
         rule_id="1003",
         name="empty-lines-between-sections",
         msg="Invalid number of empty lines between sections ({{ empty_lines }}/{{ allowed_empty_lines }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "1004": Rule(
         RuleParam(
             name="empty_lines",
             default=1,
             converter=int,
             desc="number of empty lines required between test cases",
         ),
         rule_id="1004",
         name="empty-lines-between-test-cases",
         msg="Invalid number of empty lines between test cases ({{ empty_lines }}/{{ allowed_empty_lines }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "1005": Rule(
         RuleParam(
             name="empty_lines",
             default=1,
             converter=int,
             desc="number of empty lines required between keywords",
         ),
         rule_id="1005",
         name="empty-lines-between-keywords",
         msg="Invalid number of empty lines between keywords ({{ empty_lines }}/{{ allowed_empty_lines }})",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.0.0",
     ),
     "1006": Rule(
         rule_id="1006",
         name="mixed-tabs-and-spaces",
         msg="Inconsistent use of tabs and spaces in file",
         severity=RuleSeverity.WARNING,
+        added_in_version="1.1.0",
     ),
     "1008": Rule(
         RuleParam(  # TODO: unused, remove in the next release
             name="strict",
             default=False,
             converter=str2bool,
             desc="Strict checking of the indentation",
@@ -111,44 +117,47 @@
                 IF    $condition    RETURN
                Keyword Call  # line is under-intended by two spaces
 
         The correct indentation is determined by the most common indentation in the current block. Although,
         it allows for more flexible indentation by specifying the ``indent`` parameter for checking if the
         indentation is the multiple of ``indent`` spaces (default -1, which makes this parameter being ignored).
         """,
+        added_in_version="3.0.0",
     ),
     "1009": Rule(
         RuleParam(
             name="empty_lines",
             default=0,
             converter=int,
             desc="number of empty lines allowed after section header",
         ),
-        SeverityThreshold("empty_lines"),
+        SeverityThreshold("empty_lines", substitute_value="allowed_empty_lines"),
         rule_id="1009",
         name="empty-line-after-section",
         msg="Too many empty lines after '{{ section_name }}' section header "
         "({{ empty_lines }}/{{ allowed_empty_lines }})",
         severity=RuleSeverity.WARNING,
         docs="""
         Empty lines after the section header are not allowed by default. Example of rule violation::
 
              *** Test Cases ***
 
              Resource  file.resource
 
-        It can be configured using `empty_lines` parameter.
+        It can be configured using ``empty_lines`` parameter.
         """,
+        added_in_version="1.2.0",
     ),
     "1010": Rule(
         rule_id="1010",
         name="too-many-trailing-blank-lines",
         msg="Too many blank lines at the end of file",
         severity=RuleSeverity.WARNING,
         docs="""There should be exactly one blank line at the end of the file""",
+        added_in_version="1.4.0",
     ),
     "1011": Rule(
         rule_id="1011",
         name="misaligned-continuation",
         msg="Continuation marker should be aligned with starting row",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -159,37 +168,39 @@
 
                 *** Test Cases ***
                 Example
                     Do X    first argument    second argument    third argument
                   ...    fourth argument    fifth argument    sixth argument
 
         """,
+        added_in_version="1.6.0",
     ),
     "1012": Rule(
         RuleParam(
             name="empty_lines",
             default=1,
             converter=int,
             desc="number of allowed consecutive empty lines",
         ),
-        SeverityThreshold("empty_lines", compare_method="greater"),
+        SeverityThreshold("empty_lines", compare_method="greater", substitute_value="allowed_empty_lines"),
         rule_id="1012",
         name="consecutive-empty-lines",
         msg="Too many consecutive empty lines ({{ empty_lines }}/{{ allowed_empty_lines }})",
         severity=RuleSeverity.WARNING,
         docs="""
         Example of rule violation::
 
             Keyword
                 Step 1
 
 
                 Step 2
 
         """,
+        added_in_version="1.8.0",
     ),
     "1013": Rule(
         rule_id="1013",
         name="empty-lines-in-statement",
         msg="Multi-line statement with empty lines",
         severity=RuleSeverity.WARNING,
         docs="""
@@ -197,14 +208,15 @@
 
              Keyword
              ...  1
              # empty line in-between multiline statement
              ...  2
 
         """,
+        added_in_version="1.8.0",
     ),
     "1014": Rule(
         rule_id="1014",
         name="variable-should-be-left-aligned",
         msg="Variable in Variable section should be left aligned",
         severity=RuleSeverity.ERROR,
         version=">=4.0",
@@ -212,14 +224,15 @@
         Example of rule violation::
 
             *** Variables ***
              ${VAR}  1
               ${VAR2}  2
 
         """,
+        added_in_version="1.8.0",
     ),
     "1015": Rule(
         RuleParam(name="ignore_docs", default=True, converter=str2bool, show_type="bool", desc="Ignore documentation"),
         rule_id="1015",
         name="misaligned-continuation-row",
         msg="Each next continuation line should be aligned with the previous one",
         severity=RuleSeverity.WARNING,
@@ -233,14 +246,15 @@
 
             *** Test Cases ***
             My Test
                 My Keyword
                 ...    arg1
                 ...   arg2  # misaligned
         """,
+        added_in_version="1.11.0",
     ),
     "1016": Rule(
         rule_id="1016",
         name="suite-setting-should-be-left-aligned",
         msg="Setting in Settings section should be left aligned",
         severity=RuleSeverity.ERROR,
         version=">=4.0",
@@ -249,32 +263,34 @@
 
             *** Settings ***
                 Library  Collections
                 Resource  data.resource
                 Variables  vars.robot
 
         """,
+        added_in_version="2.4.0",
     ),
     "1017": Rule(
         rule_id="1017",
         name="bad-block-indent",
         msg="Indent expected. Provide 2 or more spaces of indentation for statements inside block",
         severity=RuleSeverity.ERROR,
         docs="""
         If the indentation is less than two spaces than current block parent element
-        (such as FOR/IF/WHILE/TRY header) the indentation is invalid and the rule reports an error::
+        (such as ``FOR``/``IF``/``WHILE``/``TRY`` header) the indentation is invalid and the rule reports an error::
 
             *** Keywords ***
             Some Keyword
                 FOR  ${elem}  IN  ${list}
                     Log  ${elem}  # this is fine
                Log  stuff    # this is bad indent
             # bad comment
                 END
         """,
+        added_in_version="3.0.0",
     ),
 }
 
 
 class InvalidSpacingChecker(RawFileChecker):
     """Checker for trailing spaces and lines."""
```

### Comparing `robotframework-robocop-3.2.1/robocop/checkers/tags.py` & `robotframework-robocop-4.0.0/robocop/checkers/tags.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,151 +12,206 @@
     "0601": Rule(
         rule_id="0601",
         name="tag-with-space",
         msg="Tag '{{ tag }}' should not contain spaces",
         severity=RuleSeverity.WARNING,
         docs="""
         Example of rule violation::
-        
+
             Test
                 [Tags]  ${tag with space}
-        
+
         """,
+        added_in_version="1.0.0",
     ),
     "0602": Rule(
         rule_id="0602",
         name="tag-with-or-and",
         msg="Tag '{{ tag }}' with reserved word OR/AND."
         " Hint: make sure to include this tag using lowercase name to avoid issues",
         severity=RuleSeverity.INFO,
         docs="""
-        OR and AND words are used to combine tags when selecting tests to be run in Robot Framework. Using following 
+        ``OR`` and ``AND`` words are used to combine tags when selecting tests to be run in Robot Framework. Using following 
         configuration::
-        
+
             robot --include tagANDtag2
-        
-        Robot Framework will only execute tests that contain `tag` and `tag2`. That's why it's best to avoid AND and OR 
+
+        Robot Framework will only execute tests that contain ``tag`` and ``tag2``. That's why it's best to avoid ``AND`` and ``OR``
         in tag names. See 
-        `docs <https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#tag-patterns>`_ 
+        `docs <https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#tag-patterns>`_
         for more information.
-        
-        Tag matching is case-insensitive. If your tag contains OR or AND you can use lowercase to match it.
-        For example, if your tag is `PORT` you can match it with `port`.
+
+        Tag matching is case-insensitive. If your tag contains ``OR`` or ``AND`` you can use lowercase to match it.
+        For example, if your tag is ``PORT``, you can match it with ``port``.
         """,
+        added_in_version="1.0.0",
     ),
     "0603": Rule(
         rule_id="0603",
         name="tag-with-reserved-word",
         msg="Tag '{{ tag }}' prefixed with reserved word `robot:`",
         severity=RuleSeverity.WARNING,
         docs="""
-        This prefix is used by Robot Framework special tags. More details 
+        ``robot:`` prefix is used by Robot Framework special tags. More details 
         `here <https://robotframework.org/robotframework/latest/RobotFrameworkUserGuide.html#reserved-tags>`_.
         Special tags currently in use:
-        
+
             - robot:exit
+            - robot:flatten
             - robot:no-dry-run
             - robot:continue-on-failure 
             - robot:recursive-continue-on-failure
             - robot:skip
             - robot:skip-on-failure
             - robot:stop-on-failure
             - robot:exclude
             - robot:private
 
         """,
+        added_in_version="1.0.0",
     ),
     "0605": Rule(
         rule_id="0605",
         name="could-be-test-tags",
         msg="All tests in suite share these tags: '{{ tags }}'. "
         "You can define them in 'Test Tags' in suite settings instead",
         severity=RuleSeverity.INFO,
         docs="""
         Example::
-        
+
             *** Test Cases ***
             Test
-                [Tag]  featureX  smoke
+                [Tags]  featureX  smoke
                 Step
-            
+
             Test 2
-                [Tag]  featureX
+                [Tags]  featureX
                 Step
-        
-        In this example all tests share one common tag `featureX`. It can be declared just once using ``Test Tags``
+
+        In this example all tests share one common tag ``featureX``. It can be declared just once using ``Test Tags``
         or ``Task Tags``.
+        This rule was renamed from ``could-be-force-tags`` to ``could-be-test-tags`` in Robocop 2.6.0.
         """,
+        added_in_version="1.0.0",
     ),
     "0606": Rule(
         rule_id="0606",
         name="tag-already-set-in-test-tags",
         msg="Tag '{{ tag }}' is already set by {{ test_force_tags }} in suite settings",
         severity=RuleSeverity.INFO,
         docs="""
-        Avoid repeating same tags in tests when the tag is already declared in ``Test Tags`` or ``Force Tags``.
+        Avoid repeating the same tags in tests when the tag is already declared in ``Test Tags`` or ``Force Tags``.
         Example of rule violation::
-        
-            *** Setting ***
-            Test Tags  common-tag
-            
+
+            *** Settings ***
+            Test Tags  common_tag
+
             *** Test Cases ***
             Test
-                [Tag]  sanity  common-tag
-        
+                [Tags]  sanity  common_tag
+                Some Keyword
+
+        This rule was renamed from ``tag-already-set-in-force-tags`` to ``tag-already-set-in-test-tags`` in
+        Robocop 2.6.0.
         """,
+        added_in_version="1.0.0",
     ),
     "0607": Rule(
         rule_id="0607",
         name="unnecessary-default-tags",
         msg="Tags defined in Default Tags are always overwritten",
         severity=RuleSeverity.INFO,
         docs="""
         Example of rule violation::
-        
+
             *** Settings ***
             Default Tags  tag1  tag2
-            
+
             *** Test Cases ***
             Test
                 [Tags]  tag3
                 Step
-            
+
             Test 2
                 [Tags]  tag4
                 Step
-        
-        Since `Test` and `Test 2` have `[Tags]` section, `Default Tags` setting is never used.
+
+        Since ``Test`` and ``Test 2`` have ``[Tags]`` section, ``Default Tags`` setting is never used.
         """,
+        added_in_version="1.0.0",
     ),
     "0608": Rule(
         rule_id="0608",
         name="empty-tags",
         msg="[Tags] setting without values{{ optional_warning }}",
         severity=RuleSeverity.WARNING,
         docs="""
-        If you want to use empty `[Tags]` (for example to overwrite `Default Tags`) then use `NONE` value 
+        If you want to use empty ``[Tags]`` (for example to overwrite ``Default Tags``) then use ``NONE`` value 
         to be explicit.
         """,
+        added_in_version="2.0.0",
     ),
     "0609": Rule(
         rule_id="0609",
         name="duplicated-tags",
         msg="Multiple tags with name '{{ name }}' (first occurrence at line {{ line }} column {{ column }})",
         severity=RuleSeverity.WARNING,
         docs="""
         Tags are free text, but they are normalized so that they are converted to lowercase and all spaces are removed.
         Only first tag is used, other occurrences are ignored.
-        
+
         Example of duplicated tags::
         
             Test
                 [Tags]    Tag    TAG    tag    t a g
 
         """,
+        added_in_version="2.0.0",
+    ),
+    "0610": Rule(
+        rule_id="0610",
+        name="could-be-keyword-tags",
+        msg="All keywords in suite share these tags: '{{ tags }}'. "
+        "You can define them in 'Keyword Tags' in suite settings instead",
+        severity=RuleSeverity.INFO,
+        version=">=6",
+        docs="""
+        Example::
+
+            *** Keywords ***
+            Keyword
+                [Tags]  featureX  smoke
+                Step
+
+            Keyword 2
+                [Tags]  featureX
+                Step
+
+        In this example all keywords share one common tag ``featureX``. It can be declared just once using ``Keyword Tags``.
+        """,
+        added_in_version="3.3.0",
+    ),
+    "0611": Rule(
+        rule_id="0611",
+        name="tag-already-set-in-keyword-tags",
+        msg="Tag '{{ tag }}' is already set by {{ keyword_tags }} in suite settings",
+        severity=RuleSeverity.INFO,
+        version=">=6",
+        docs="""
+        Avoid repeating the same tags in keywords when the tag is already declared in ``Keyword Tags``.
+        Example of rule violation::
+
+            *** Settings ***
+            Keyword Tags  common_tag
+
+            *** Keywords ***
+            Keyword
+                [Tags]  sanity  common_tag
+        """,
+        added_in_version="3.3.0",
     ),
 }
 
 
 class TagNameChecker(VisitorChecker):
     """Checker for tag names. It scans for tags with spaces or Robot Framework reserved words."""
 
@@ -166,14 +221,15 @@
         "tag-with-reserved-word",
         "duplicated-tags",
     )
 
     is_keyword = False
     reserved_tags = {
         "robot:exit",
+        "robot:flatten",
         "robot:no-dry-run",
         "robot:continue-on-failure",
         "robot:recursive-continue-on-failure",
         "robot:skip",
         "robot:skip-on-failure",
         "robot:stop-on-failure",
         "robot:exclude",
@@ -326,20 +382,89 @@
             self.report(
                 "empty-tags",
                 optional_warning=suffix,
                 node=node,
                 col=node.data_tokens[0].col_offset + 1,
                 end_col=node.end_col_offset,
             )
-        self.tags.append([tag.value for tag in node.data_tokens[1:]])
+        if not self.in_keywords:
+            self.tags.append([tag.value for tag in node.data_tokens[1:]])
         for tag in node.data_tokens[1:]:
-            if tag.value not in self.test_tags:
+            if self.in_keywords or tag.value not in self.test_tags:
                 continue
             test_force_tags = self.test_tags_node.data_tokens[0].value
             self.report(
                 "tag-already-set-in-test-tags",
                 tag=tag.value,
                 test_force_tags=test_force_tags,
                 node=node,
                 lineno=tag.lineno,
                 col=tag.col_offset + 1,
             )
+
+
+class KeywordTagsChecker(VisitorChecker):
+    """Checker for keyword tags."""
+
+    reports = (
+        "could-be-keyword-tags",
+        "tag-already-set-in-keyword-tags",
+    )
+
+    def __init__(self):
+        self.tags_in_keywords = []
+        self.keyword_tags = set()
+        self.keyword_tags_node = None
+        self.keywords_count = 0
+        self.in_keywords = False
+        super().__init__()
+
+    def visit_File(self, node):  # noqa
+        self.tags_in_keywords = []
+        self.keyword_tags = set()
+        self.keyword_tags_node = None
+        self.keywords_count = 0
+        super().visit_File(node)
+        if not self.tags_in_keywords:
+            return
+        if len(self.tags_in_keywords) != self.keywords_count:
+            return
+        if self.keywords_count < 2:
+            return
+        common_keyword_tags = set.intersection(*[set(tags) for tags in self.tags_in_keywords])
+        common_keyword_tags = common_keyword_tags - self.keyword_tags
+        if common_keyword_tags:
+            report_node = node if self.keyword_tags_node is None else self.keyword_tags_node
+            self.report(
+                "could-be-keyword-tags",
+                tags=", ".join(common_keyword_tags),
+                node=report_node,
+            )
+
+    def visit_Keyword(self, node):  # noqa
+        self.keywords_count += 1
+        self.generic_visit(node)
+
+    def visit_KeywordTags(self, node):  # noqa
+        self.keyword_tags = {token.value for token in node.data_tokens[1:]}
+        self.keyword_tags_node = node
+
+    def visit_KeywordSection(self, node):  # noqa
+        self.in_keywords = True
+        self.generic_visit(node)
+        self.in_keywords = False
+
+    def visit_Tags(self, node):  # noqa
+        if self.in_keywords:
+            self.tags_in_keywords.append([tag.value for tag in node.data_tokens[1:]])
+        for tag in node.data_tokens[1:]:
+            if not self.in_keywords or tag.value not in self.keyword_tags:
+                continue
+            keyword_tags = self.keyword_tags_node.data_tokens[0].value
+            self.report(
+                "tag-already-set-in-keyword-tags",
+                tag=tag.value,
+                keyword_tags=keyword_tags,
+                node=node,
+                lineno=tag.lineno,
+                col=tag.col_offset + 1,
+            )
```

### Comparing `robotframework-robocop-3.2.1/robocop/config.py` & `robotframework-robocop-4.0.0/robocop/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,15 @@
         self.language = []
         self.list = ""
         self.list_configurables = ""
         self.list_reports = ""
         self.output = None
         self.recursive = True
         self.verbose = False
+        self.persistent = False
         self.config_from = ""
         self.root = find_project_root(root, ["."])
         self.parse()
 
     def remove_severity(self):
         self.include = {self.replace_severity_values(rule) for rule in self.include}
         self.exclude = {self.replace_severity_values(rule) for rule in self.exclude}
@@ -285,16 +286,17 @@
             "-r",
             "--reports",
             action=ParseDelimitedArgAction,
             default=self.reports,
             help="Generate reports after scan.\n"
             "You can enable reports by listing them in comma-separated list:\n"
             "--reports rules_by_id,rules_by_error_type,scan_timer\n"
-            "To enable all reports use all:\n"
-            "--reports all",
+            "To enable all default reports use 'all':\n"
+            "--reports all\n"
+            "List available reports with --list-reports option.",
         )
         optional.add_argument(
             "-f",
             "--format",
             type=str,
             default=self.format,
             help="Format of output message. "
@@ -394,14 +396,20 @@
         optional.add_argument(
             "--language",
             "--lang",
             action=ParseDelimitedArgAction,
             default=self.language,
             help="Parse Robot Framework files using additional languages.",
         )
+        optional.add_argument(
+            "--persistent",
+            action="store_true",
+            default=self.persistent,
+            help="Use this flag to save Robocop reports in cache directory for later comparison.",
+        )
         optional.add_argument("-h", "--help", action="help", help="Print this help message and exit.")
         optional.add_argument(
             "-v",
             "--version",
             action="version",
             version=__version__,
             help="Display Robocop version.",
@@ -557,15 +565,15 @@
         if self.include or self.include_patterns:  # if any include pattern, it must match with something
             if rule.rule_id in self.include or rule.name in self.include:
                 return True
             for pattern in self.include_patterns:
                 if pattern.match(rule.rule_id) or pattern.match(rule.name):
                     return True
             return False
-        return True
+        return rule.enabled
 
     def is_rule_disabled(self, rule):
         if not rule.enabled_in_version:
             return True
         if rule.severity < self.threshold:
             return True
         if rule.rule_id in self.exclude or rule.name in self.exclude:
@@ -620,10 +628,12 @@
                 self.threshold = RuleSeverity(value)
             elif key == "output":
                 self.output = open(value, "w")
             elif key == "no_recursive":
                 self.recursive = not value
             elif key == "verbose":
                 self.verbose = value
+            elif key == "persistent":
+                self.persistent = value
             else:
                 raise InvalidArgumentError(f"Option '{key}' is not supported in pyproject.toml configuration file.")
         return True
```

### Comparing `robotframework-robocop-3.2.1/robocop/exceptions.py` & `robotframework-robocop-4.0.0/robocop/exceptions.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.1/robocop/files.py` & `robotframework-robocop-4.0.0/robocop/files.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.1/robocop/rules.py` & `robotframework-robocop-4.0.0/robocop/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from textwrap import dedent
 from typing import Any, Callable, Dict, Optional, Pattern, Union
 
 from jinja2 import Template
 
 import robocop.exceptions
 from robocop.utils import ROBOT_VERSION
+from robocop.utils.misc import str2bool
 from robocop.utils.version_matching import VersionSpecifier
 
 
 @total_ordering
 class RuleSeverity(Enum):
     """
     Rule severity.
@@ -156,19 +157,20 @@
     When adding support for ``SeverityThreshold`` to ``Rule``, the value of the param
     needs to be passed to self.report() call as ``sev_threshold_value``.
 
     ``compare_method`` is used to determine how to compare parameter value
     with threshold ranges.
     """
 
-    def __init__(self, param_name, compare_method="greater"):
+    def __init__(self, param_name, compare_method="greater", substitute_value=None):
         self.name = "severity_threshold"
         self.param_name = param_name
         self.thresholds = None
         self.compare_method = compare_method
+        self.substitute_value = substitute_value
 
     @property
     def value(self):
         """Property syntax is used to match with RuleParam converting logic."""
         return self.thresholds
 
     @value.setter
@@ -216,14 +218,26 @@
         if self.thresholds is None:
             return None
         for severity, threshold in self.thresholds:
             if self.check_condition(value, threshold):
                 return severity
         return None
 
+    def get_matching_threshold(self, value):
+        """
+        Find first threshold that passes the condition with passed value.
+
+        It's useful to get rule message updated with the threshold value that triggered rule.
+        """
+        if value is None:
+            return None
+        for severity, threshold in self.thresholds:
+            if self.check_condition(value, threshold):
+                return threshold
+
     def __str__(self):
         return self.name
 
 
 class Rule:
     """
     Robocop linter rule.
@@ -238,52 +252,70 @@
         *params: Union[RuleParam, SeverityThreshold],
         rule_id: str,
         name: str,
         msg: str,
         severity: RuleSeverity,
         version: str = None,
         docs: str = "",
+        added_in_version: Optional[str] = None,
+        enabled: bool = True,
     ):
         """
         :param params: RuleParam() or SeverityThreshold() instances
         :param rule_id: id of the rule
         :param name: name of the rule
         :param msg: message printed when rule breach is detected
         :param severity: severity of the rule (ie: RuleSeverity.INFO)
         :param version: supported Robot Framework version (ie: >=4.0)
         :param docs: Full documentation of the rule (rst supported)
         description of the rule
+        :param added_in_version: Version of the Robocop when the Rule was created
         """
         self.rule_id = rule_id
         self.name = name
         self.msg = msg
         self.msg_template = self.get_template(msg)
         self.default_severity = severity
         self.docs = dedent(docs)
         self.config = {
             "severity": RuleParam(
-                "severity",
-                severity,
-                RuleSeverity.parser,
+                name="severity",
+                default=severity,
+                converter=RuleSeverity.parser,
                 desc="Rule severity (E = Error, W = Warning, I = Info)",
                 show_type="severity",
-            )
+            ),
+            "enabled": RuleParam(
+                name="enabled",
+                default=enabled,
+                converter=str2bool,
+                desc="Rule default enable status",
+                show_type="bool",
+            ),
         }
         self.severity_threshold = None
         for param in params:
             self.config[param.name] = param
-        self.enabled = True
         self.supported_version = version if version else "All"
         self.enabled_in_version = self.supported_in_rf_version(version)
+        self.added_in_version = added_in_version
 
     @property
     def severity(self):
         return self.config["severity"].value
 
     @property
+    def enabled(self):
+        return self.config["enabled"].value
+
+    @enabled.setter
+    def enabled(self, value):
+        self.config["enabled"].value = value
+
+    @property
     def description(self):
         desc = ""
         if not (self.msg.startswith("{{") and self.msg.endswith("}}")):
             desc += f"{self.msg}."
         if self.docs:
             desc += "\n"
             desc += self.docs
@@ -336,35 +368,49 @@
                 f"Provided param '{param}' for rule '{self.name}' does not exist. "
                 f"Available configurable{'' if count == 1 else 's'} for this rule:\n"
                 f"    {configurables_text}"
             )
         self.config[param].value = value
 
     def available_configurables(self, include_severity: bool = True):
-        params = [str(param) for param in self.config.values() if param.name != "severity" or include_severity]
+        params = []
+        for param in self.config.values():
+            if (param.name == "severity" and not include_severity) or param.name == "enabled":
+                continue
+            params.append(str(param))
         if not params:
             return 0, ""
         count = len(params)
         text = "\n    ".join(params)
         return count, text
 
     def prepare_message(
-        self, source, node, lineno, col, end_lineno, end_col, ext_disablers, sev_threshold_value, severity, **kwargs
+        self,
+        source,
+        node,
+        lineno,
+        col,
+        end_lineno,
+        end_col,
+        extended_disablers,
+        sev_threshold_value,
+        severity,
+        **kwargs,
     ):
         msg = self.get_message(**kwargs)
         return Message(
             rule=self,
             msg=msg,
             source=source,
             node=node,
             lineno=lineno,
             col=col,
             end_col=end_col,
             end_lineno=end_lineno,
-            ext_disablers=ext_disablers,
+            extended_disablers=extended_disablers,
             sev_threshold_value=sev_threshold_value,
             overwrite_severity=severity,
         )
 
     def matches_pattern(self, pattern: Union[str, Pattern]):
         """check if this rule matches given pattern"""
         if isinstance(pattern, str):
@@ -379,15 +425,15 @@
         msg,
         source,
         node,
         lineno,
         col,
         end_lineno,
         end_col,
-        ext_disablers=None,
+        extended_disablers=None,
         sev_threshold_value=None,
         overwrite_severity=None,
     ):
         self.enabled = rule.enabled
         self.rule_id = rule.rule_id
         self.name = rule.name
         self.severity = self.get_severity(overwrite_severity, rule, sev_threshold_value)
@@ -397,15 +443,15 @@
         if node is not None and node.lineno > -1:
             self.line = node.lineno
         if lineno is not None:
             self.line = lineno
         self.col = 1 if col is None else col
         self.end_line = self.line if end_lineno is None else end_lineno
         self.end_col = self.col if end_col is None else end_col
-        self.ext_disablers = ext_disablers if ext_disablers else []
+        self.extended_disablers = extended_disablers if extended_disablers else []
 
     def __lt__(self, other):
         return (self.line, self.col, self.rule_id) < (
             other.line,
             other.col,
             other.rule_id,
         )
@@ -419,13 +465,15 @@
     def get_fullname(self) -> str:
         return f"{self.severity.value}{self.rule_id} ({self.name})"
 
     def to_json(self) -> Dict:
         return {
             "source": self.source,
             "line": self.line,
+            "end_line": self.end_line,
             "column": self.col,
+            "end_column": self.end_col,
             "severity": self.severity.value,
             "rule_id": self.rule_id,
             "description": self.desc,
             "rule_name": self.name,
         }
```

### Comparing `robotframework-robocop-3.2.1/robocop/run.py` & `robotframework-robocop-4.0.0/robocop/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from robot.api import get_resource_model
 from robot.errors import DataError
 
 import robocop.exceptions
 from robocop import checkers, reports
 from robocop.config import Config
 from robocop.files import get_files
+from robocop.reports import is_report_comparable, load_reports_result_from_cache, save_reports_result_to_cache
 from robocop.rules import Message
 from robocop.utils import DisablersFinder, FileType, FileTypeChecker, RecommendationFinder, is_suite_templated
 from robocop.utils.file_types import check_model_type, get_resource_with_lang
 
 
 class Robocop:
     """
@@ -44,15 +45,15 @@
         self.checkers = []
         self.rules = {}
         self.reports = {}
         self.root = os.getcwd()
         self.config = Config(from_cli=from_cli) if config is None else config
         self.from_cli = from_cli
         if not from_cli:
-            self.config.reports.append("json_report")
+            self.config.reports.append("internal_json_report")
         self.out = self.set_output()
 
     def set_output(self):
         """Set output for printing to file if configured. Else use standard output"""
         return self.config.output or None
 
     def write_line(self, line):
@@ -75,15 +76,15 @@
         self.run_checks()
         self.make_reports()
         if self.config.output and not self.out.closed:
             self.out.close()
         if self.from_cli:
             sys.exit(self.reports["return_status"].return_status)
         else:
-            return self.reports["json_report"].issues
+            return self.reports["internal_json_report"].issues
 
     def recognize_file_types(self):
         """
         Pre-parse files to recognize their types. If the filename is `__init__.*`, the type is `INIT`.
         Files with .resource extension are `RESOURCE` type.
         If the file is imported somewhere then file type is `RESOURCE`. Otherwise, file type is `GENERAL`.
         These types are important since they are used to define parsing class for robot API.
@@ -121,15 +122,15 @@
             found_issues.sort()
             for issue in found_issues:
                 self.report(issue)
         if "file_stats" in self.reports:
             self.reports["file_stats"].files_count = len(self.files)
 
     def run_check(self, ast_model, filename, source=None):
-        disablers = DisablersFinder(filename=filename, source=source)
+        disablers = DisablersFinder(ast_model)
         if disablers.file_disabled:
             return []
         found_issues = []
         templated = is_suite_templated(ast_model)
         for checker in self.checkers:
             if checker.disabled:
                 continue
@@ -221,21 +222,33 @@
     def check_for_disabled_rules(self):
         """Check checker configuration to disable rules."""
         for checker in self.checkers:
             if not self.any_rule_enabled(checker):
                 checker.disabled = True
 
     def make_reports(self):
+        report_results = {}
+        prev_results = load_reports_result_from_cache()
+        prev_results = prev_results.get(str(self.root)) if prev_results is not None else None
         for report in self.reports.values():
             if report.name == "sarif":
                 output = report.get_report(self.config, self.rules)
+            elif is_report_comparable(report):
+                prev_result = prev_results.get(report.name) if prev_results is not None else None
+                output = report.get_report(prev_result)
             else:
                 output = report.get_report()
             if output is not None:
                 self.write_line(output)
+            if self.config.persistent and is_report_comparable(report):
+                result = report.persist_result()
+                if result is not None:
+                    report_results[report.name] = result
+        if self.config.persistent:
+            save_reports_result_to_cache(str(self.root), report_results)
 
     def any_rule_enabled(self, checker) -> bool:
         for name, rule in checker.rules.items():
             rule.enabled = self.config.is_rule_enabled(rule)
             checker.rules[name] = rule
         return any(msg.enabled for msg in checker.rules.values())
```

### Comparing `robotframework-robocop-3.2.1/robocop/utils/__init__.py` & `robotframework-robocop-4.0.0/robocop/utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,14 @@
     RecommendationFinder,
     find_robot_vars,
     get_errors,
     get_section_name,
     is_suite_templated,
     issues_to_lsp_diagnostic,
     keyword_col,
-    modules_from_path,
-    modules_from_paths,
-    modules_in_current_dir,
     normalize_robot_name,
     normalize_robot_var_name,
     parse_assignment_sign_type,
     pattern_type,
     remove_robot_vars,
     str2bool,
     token_col,
```

### Comparing `robotframework-robocop-3.2.1/robocop/utils/file_types.py` & `robotframework-robocop-4.0.0/robocop/utils/file_types.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.1/robocop/utils/misc.py` & `robotframework-robocop-4.0.0/robocop/utils/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,40 @@
 import ast
 import difflib
-import importlib.util
 import re
 import token
 import tokenize
 from collections import Counter, defaultdict
-from importlib import import_module
 from io import StringIO
 from pathlib import Path
 from tokenize import generate_tokens
 from typing import Dict, List, Optional, Pattern, Tuple
 
+import platformdirs
 from robot.api import Token
 
 try:
     from robot.api.parsing import Variable
 except ImportError:
     from robot.parsing.model.statements import Variable
 
-from robot.variables.search import VariableIterator
+from robot.variables.search import VariableIterator, search_variable
 from robot.version import VERSION as RF_VERSION
 
-from robocop.exceptions import InvalidExternalCheckerError
 from robocop.utils.version_matching import Version
 from robocop.version import __version__
 
 ROBOT_VERSION = Version(RF_VERSION)
 ROBOT_WITH_LANG = Version("6.0")
 
 
 def rf_supports_lang():
     return ROBOT_VERSION >= ROBOT_WITH_LANG
 
 
-def modules_in_current_dir(path, module_name):
-    """Yield modules inside `path` parent directory"""
-    yield from modules_from_path(Path(path).parent, module_name)
-
-
-def modules_from_paths(paths):
-    for path in paths:
-        path_object = Path(path)
-        if path_object.exists():
-            if path_object.is_dir():
-                yield from modules_from_paths(
-                    [file for file in path_object.iterdir() if "__pycache__" not in str(file)]
-                )
-            else:
-                spec = importlib.util.spec_from_file_location(path_object.stem, path_object)
-                mod = importlib.util.module_from_spec(spec)
-
-                spec.loader.exec_module(mod)
-                yield mod
-        else:
-            # if it's not physical path, try to import from installed modules
-            try:
-                parent_name, *lib_name = path.rsplit(".", 1)
-                if lib_name:
-                    parent = __import__(parent_name, fromlist=lib_name)
-                    mod = getattr(parent, "".join(lib_name))
-                else:
-                    mod = __import__(parent_name, None)
-                yield mod
-            except ImportError:
-                raise InvalidExternalCheckerError(path) from None
-
-
-def modules_from_path(path, module_name=None, relative="."):
-    """Traverse current directory and yield python files imported as module"""
-    if path.is_file():
-        yield import_module(relative + path.stem, module_name)
-    elif path.is_dir():
-        for file in path.iterdir():
-            if "__pycache__" in str(file):
-                continue
-            if file.suffix == ".py" and file.stem != "__init__":
-                yield from modules_from_path(file, module_name, relative)
-
-
 def normalize_robot_name(name: str, remove_prefix: Optional[str] = None) -> str:
     name = name.replace(" ", "").replace("_", "").lower() if name else ""
     if remove_prefix:
         return name[name.startswith(remove_prefix) and len(remove_prefix) :]
     return name
 
 
@@ -175,15 +128,16 @@
             var_token = child.get_token(Token.VARIABLE)
             sign = self.get_assignment_sign(var_token.value)
             self.variables_sign_counter[sign] += 1
         return node
 
     @staticmethod
     def get_assignment_sign(token_value):
-        return token_value[token_value.find("}") + 1 :]
+        variable = search_variable(token_value, ignore_errors=True)
+        return variable.after
 
 
 def parse_assignment_sign_type(value: str) -> str:
     types = {
         "none": "",
         "equal_sign": "=",
         "space_and_equal_sign": " =",
@@ -349,15 +303,15 @@
 def get_errors(node):
     if ROBOT_VERSION.major == 3:
         return [node.error] if node.error else []
     return node.errors
 
 
 def find_escaped_variables(string):
-    """Return list of $escaped or \${escaped} variables from the string.
+    r"""Return list of $escaped or \${escaped} variables from the string.
 
     We are tokenizing the string using Python ast modules. This allows us to find valid Python-like names and check
     if they are escaped Robot Framework variables.
     """
     variable_started = False
     variables = []
     try:
@@ -367,7 +321,18 @@
                     variables.append(tokval)
                 variable_started = False
             if toknum == token.ERRORTOKEN and tokval == "$":
                 variable_started = True
     except tokenize.TokenError:
         pass
     return variables
+
+
+def get_robocop_cache_directory(ensure_exists):
+    return Path(platformdirs.user_cache_dir("robocop", ensure_exists=ensure_exists))
+
+
+def get_string_diff(prev_count, count):
+    """Get +0, -10 string."""
+    diff = count - prev_count
+    prefix = "+" if diff >= 0 else ""
+    return prefix + str(diff)
```

### Comparing `robotframework-robocop-3.2.1/robocop/utils/run_keywords.py` & `robotframework-robocop-4.0.0/robocop/utils/run_keywords.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.1/robocop/utils/version_matching.py` & `robotframework-robocop-4.0.0/robocop/utils/version_matching.py`

 * *Files identical despite different names*

### Comparing `robotframework-robocop-3.2.1/robotframework_robocop.egg-info/PKG-INFO` & `robotframework-robocop-4.0.0/robotframework_robocop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-robocop
-Version: 3.2.1
+Version: 4.0.0
 Summary: Static code analysis tool (linter) for Robot Framework
 Home-page: https://github.com/MarketSquare/robotframework-robocop
 Download-URL: https://pypi.org/project/robotframework-robocop
 Author: Bartlomiej Hirsz, Mateusz Nojek
 Author-email: bartek.hirsz@gmail.com, matnojek@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://robocop.readthedocs.io/en/stable
```

### Comparing `robotframework-robocop-3.2.1/setup.py` & `robotframework-robocop-4.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,25 +53,29 @@
     install_requires=[
         "jinja2>=3.0,<4.0",
         "robotframework>=3.2.2",
         "pathspec>=0.9,<0.12",
         "tomli>=2.0.0",
         "pytz>=2022.7",
         "python-dateutil>=2.8.2",
+        "platformdirs>=3.2.0,<3.9.0",
     ],
     extras_require={
         "dev": [
             "black",
             "coverage",
             "pytest",
             "pyyaml",
             "pytest-benchmark",
             "nox",
         ],
         "doc": [
             "furo",
             "sphinx",
             "sphinx_design",
+            "sphinx-copybutton",
+            "sphinxemoji",
+            "pygments",
         ],
     },
     entry_points={"console_scripts": ["robocop=robocop:run_robocop"]},
 )
```

