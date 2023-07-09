# Comparing `tmp/mo_sql_parsing-9.410.23165-py2.py3-none-any.whl.zip` & `tmp/mo_sql_parsing-9.422.23190-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 38381 bytes, number of entries: 13
+Zip file size: 38385 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     2597 b- defN 22-Dec-18 22:41 mo_sql_parsing/__init__.py
 -rw-rw-rw-  2.0 fat    22449 b- defN 23-Jun-10 00:48 mo_sql_parsing/formatting.py
 -rw-rw-rw-  2.0 fat    10666 b- defN 23-Jun-10 00:27 mo_sql_parsing/keywords.py
--rw-rw-rw-  2.0 fat    33839 b- defN 23-Jun-14 00:23 mo_sql_parsing/sql_parser.py
+-rw-rw-rw-  2.0 fat    33848 b- defN 23-Jul-09 13:13 mo_sql_parsing/sql_parser.py
 -rw-rw-rw-  2.0 fat     7321 b- defN 23-Mar-26 12:53 mo_sql_parsing/types.py
 -rw-rw-rw-  2.0 fat    22999 b- defN 23-May-24 01:38 mo_sql_parsing/utils.py
 -rw-rw-rw-  2.0 fat     2987 b- defN 23-Mar-26 12:53 mo_sql_parsing/windows.py
--rw-rw-rw-  2.0 fat    15922 b- defN 23-Jun-14 00:23 mo_sql_parsing-9.410.23165.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9345 b- defN 23-Jun-14 00:23 mo_sql_parsing-9.410.23165.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jun-14 00:23 mo_sql_parsing-9.410.23165.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jun-14 00:23 mo_sql_parsing-9.410.23165.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-14 00:23 mo_sql_parsing-9.410.23165.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1134 b- defN 23-Jun-14 00:23 mo_sql_parsing-9.410.23165.dist-info/RECORD
-13 files, 129386 bytes uncompressed, 36475 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat    15922 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9345 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/zip-safe
+?rw-rw-r--  2.0 fat     1134 b- defN 23-Jul-09 13:13 mo_sql_parsing-9.422.23190.dist-info/RECORD
+13 files, 129395 bytes uncompressed, 36479 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mo_sql_parsing/utils.py
 Comment: 
 
 Filename: mo_sql_parsing/windows.py
 Comment: 
 
-Filename: mo_sql_parsing-9.410.23165.dist-info/LICENSE
+Filename: mo_sql_parsing-9.422.23190.dist-info/LICENSE
 Comment: 
 
-Filename: mo_sql_parsing-9.410.23165.dist-info/METADATA
+Filename: mo_sql_parsing-9.422.23190.dist-info/METADATA
 Comment: 
 
-Filename: mo_sql_parsing-9.410.23165.dist-info/WHEEL
+Filename: mo_sql_parsing-9.422.23190.dist-info/WHEEL
 Comment: 
 
-Filename: mo_sql_parsing-9.410.23165.dist-info/top_level.txt
+Filename: mo_sql_parsing-9.422.23190.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_sql_parsing-9.410.23165.dist-info/zip-safe
+Filename: mo_sql_parsing-9.422.23190.dist-info/zip-safe
 Comment: 
 
-Filename: mo_sql_parsing-9.410.23165.dist-info/RECORD
+Filename: mo_sql_parsing-9.422.23190.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_sql_parsing/sql_parser.py

```diff
@@ -64,15 +64,15 @@
 
         white.add_ignore(Literal("--") + rest_of_line)
         white.add_ignore(Literal("#") + rest_of_line)
         white.add_ignore(Literal("/*") + SkipTo("*/", include=True))
 
         with whitespaces.NO_WHITESPACE:
             identifier = ~RESERVED + ident
-        function_name = ~(UNION | FROM | WHERE) + ident
+        function_name = ~(UNION | FROM | WHERE | SELECT) + ident
 
         # EXPRESSIONS
         expression = Forward()
         (column_type, column_definition, column_def_references, column_option,) = get_column_type(
             expression, identifier, literal_string
         )
 
@@ -285,15 +285,15 @@
         ) | Group(expression)("params")
 
         # https://cloud.google.com/bigquery/docs/reference/standard-sql/aggregate-function-calls
         call_function = (
             function_name("op")
             + LB
             + Optional(flag("distinct"))
-            + Optional(Group(query)("params") | delimited_list(one_param))
+            + Optional(delimited_list(one_param) | Group(query)("params"))
             + Optional((keyword("respect") | keyword("ignore"))("nulls") + keyword("nulls").suppress())
             + Optional(ORDER_BY + delimited_list(Group(sort_column))("orderby"))
             + Optional(assign("limit", expression))
             + RB
         ) / to_json_call
 
         dynamic_accessor = LK + expression + RK
```

## Comparing `mo_sql_parsing-9.410.23165.dist-info/LICENSE` & `mo_sql_parsing-9.422.23190.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_sql_parsing-9.410.23165.dist-info/METADATA` & `mo_sql_parsing-9.422.23190.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.410.23165
+Version: 9.422.23190
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots (==9.408.23161)
-Requires-Dist: mo-future (==7.401.23144)
-Requires-Dist: mo-imports (==7.408.23161)
-Requires-Dist: mo-parsing (==8.408.23161)
+Requires-Dist: mo-dots (==9.417.23168)
+Requires-Dist: mo-future (==7.416.23168)
+Requires-Dist: mo-imports (==7.416.23168)
+Requires-Dist: mo-parsing (==8.421.23188)
 Provides-Extra: dev
 Provides-Extra: tests
 Requires-Dist: mo-testing ; extra == 'tests'
 Requires-Dist: mo-threads ; extra == 'tests'
 Requires-Dist: mo-files ; extra == 'tests'
 Requires-Dist: mo-streams ; extra == 'tests'
 Requires-Dist: zstandard ; extra == 'tests'
```

## Comparing `mo_sql_parsing-9.410.23165.dist-info/RECORD` & `mo_sql_parsing-9.422.23190.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mo_sql_parsing/__init__.py,sha256=qu67hMKaz6Rn_c0idUNZ9e_BvFuxXsDZRuwQmmGYqpI,2597
 mo_sql_parsing/formatting.py,sha256=tItgfyUsmHx8iyL-mf2MnS9vAcCrpbUxqIRZTPRYKC4,22449
 mo_sql_parsing/keywords.py,sha256=4huuey_x1Q2ervkRWMqj4woMsmmSlDDCFhKCViN5jDs,10666
-mo_sql_parsing/sql_parser.py,sha256=bXhsDz7kM73u8mtfKUS4kOVBF2K9H-rVBDOzUwCULeI,33839
+mo_sql_parsing/sql_parser.py,sha256=Jr7WkLQNX1nrLOhthysWiu30iLM49w6fj-Pl7c_1LtA,33848
 mo_sql_parsing/types.py,sha256=4nnewHeuD_q3W7muesXsSS4JW73TM17YgBjlxQkOfpo,7321
 mo_sql_parsing/utils.py,sha256=1vVp9zi1uqq04Y9K0Y4yAfrqMyPhyXr7U06s4NXiqrc,22999
 mo_sql_parsing/windows.py,sha256=DNYTT34qFS8lfaDEg4oXigmYoSA72_LyHLgIQjBSpWI,2987
-mo_sql_parsing-9.410.23165.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
-mo_sql_parsing-9.410.23165.dist-info/METADATA,sha256=nXhUgoXOZDJegUAeDHD0PEHHflHR9lN63GBOcxnMagM,9345
-mo_sql_parsing-9.410.23165.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-mo_sql_parsing-9.410.23165.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
-mo_sql_parsing-9.410.23165.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-mo_sql_parsing-9.410.23165.dist-info/RECORD,,
+mo_sql_parsing-9.422.23190.dist-info/LICENSE,sha256=YCIsKMGn9qksffmOXF9EWeYk5uKF4Lm5RGevX2qzND0,15922
+mo_sql_parsing-9.422.23190.dist-info/METADATA,sha256=3aZMXKcxfoVPiF34bQuQ1ysjkG5-TftNgKWFn1DDC8c,9345
+mo_sql_parsing-9.422.23190.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+mo_sql_parsing-9.422.23190.dist-info/top_level.txt,sha256=P9tODVsRxMEL1jG7yBYiLD3rRo_rjSKa_r-F6cbnfgA,15
+mo_sql_parsing-9.422.23190.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+mo_sql_parsing-9.422.23190.dist-info/RECORD,,
```

