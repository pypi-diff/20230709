# Comparing `tmp/assistant_improve_toolkit-1.4.0.tar.gz` & `tmp/assistant_improve_toolkit-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistant_improve_toolkit-1.4.0.tar", last modified: Fri Jun 30 14:33:41 2023, max compression
+gzip compressed data, was "assistant_improve_toolkit-1.4.1.tar", last modified: Sat Jul  8 22:45:04 2023, max compression
```

## Comparing `assistant_improve_toolkit-1.4.0.tar` & `assistant_improve_toolkit-1.4.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.132699 assistant_improve_toolkit-1.4.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10174 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-30 14:33:41.132699 assistant_improve_toolkit-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-30 14:33:41.132699 assistant_improve_toolkit-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.124699 assistant_improve_toolkit-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.128699 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47406 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/computation_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/cos_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/fetch_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/version.py
--rw-r--r--   0 runner    (1001) docker     (123)   109055 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/visualize_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/watson_assistant_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.128699 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-30 14:33:41.000000 assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.128699 assistant_improve_toolkit-1.4.0/src/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:33:41.132699 assistant_improve_toolkit-1.4.0/src/main/python/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46395 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/computation_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/cos_op.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/export_csv_for_intent_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/fetch_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)   107935 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/visualize_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/watson_assistant_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-30 14:16:32.000000 assistant_improve_toolkit-1.4.0/src/main/python/watson_assistant_func_skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:45:04.502125 assistant_improve_toolkit-1.4.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10174 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-08 22:45:04.502125 assistant_improve_toolkit-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-08 22:45:04.502125 assistant_improve_toolkit-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:45:04.498125 assistant_improve_toolkit-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:45:04.502125 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47427 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/computation_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/cos_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/fetch_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109166 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/visualize_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13709 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/watson_assistant_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:45:04.502125 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-08 22:45:04.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-08 22:45:04.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:45:04.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 22:45:04.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-08 22:45:04.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 22:45:04.000000 assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:45:04.502125 assistant_improve_toolkit-1.4.1/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 22:45:04.502125 assistant_improve_toolkit-1.4.1/src/main/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/main/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46395 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/main/python/computation_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/main/python/cos_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/main/python/export_csv_for_intent_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/main/python/fetch_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107935 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/main/python/visualize_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/main/python/watson_assistant_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-07-08 22:30:24.000000 assistant_improve_toolkit-1.4.1/src/main/python/watson_assistant_func_skip.py
```

### Comparing `assistant_improve_toolkit-1.4.0/LICENSE` & `assistant_improve_toolkit-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/PKG-INFO` & `assistant_improve_toolkit-1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant_improve_toolkit
-Version: 1.4.0
+Version: 1.4.1
 Summary: Assistant Improve Toolkit
 Home-page: https://github.com/watson-developer-cloud/assistant-improve-recommendations-notebook
 Author: IBM Watson
 Author-email: watdevex@us.ibm.com
 Maintainer: Zhe Zhang
 Maintainer-email: zhangzhe@us.ibm.com
 License: Apache 2.0
```

### Comparing `assistant_improve_toolkit-1.4.0/README.md` & `assistant_improve_toolkit-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/setup.py` & `assistant_improve_toolkit-1.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # Learn more about it at: http://github.com/fabiommendes/python-boilerplate/
 #
 
 import setuptools
 from os import path
 
-__version__ = '1.3.9'
+__version__ = '1.4.0'
 
 # read contents of README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as file:
     readme_file = file.read()
 
 setuptools.setup(
```

### Comparing `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/__init__.py` & `assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/computation_func.py` & `assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/computation_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,17 +290,19 @@
     print('Extracting context and output ...')
     df2 = pd.concat([df1.drop(['response_context', 'response_output'], axis=1),
                      df1['response_context'].apply(pd.Series).add_prefix('response_context_'),
                      pd.DataFrame(df1['response_output'].tolist()).add_prefix('response_')],
                     axis=1)  # type: pd.DataFrame
     
     # Add context_system fields
-    df3 = pd.concat([df2.drop(['response_context_system'], axis=1),
-                     df2['response_context_system'].apply(pd.Series).add_prefix('response_')],
-                    axis=1)  # type: pd.DataFrame
+    # df3 = pd.concat([df2.drop(['response_context_system'], axis=1),
+    #                  df2['response_context_system'].apply(pd.Series).add_prefix('response_')],
+    #                 axis=1)  # type: pd.DataFrame
+
+    df3 = df2
 
     if 'response_context_skills' in df3:
         df3['response_context_skills'] = df3['response_context_skills'].fillna({i: {} for i in df3.index})
         df3['response_context_response_context_IntentStarted'] = df3['response_context_skills'].apply(lambda x: extract_intent_started(x))
         df3['response_context_response_context_IntentCompleted'] = df3['response_context_skills'].apply(lambda x: extract_intent_completed(x))
 
     if 'response_context_response_context_IntentStarted' in df3.columns \
```

### Comparing `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/cos_op.py` & `assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/cos_op.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py` & `assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/fetch_logs.py` & `assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/visualize_func.py` & `assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/visualize_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,66 +365,67 @@
         coverage_grp = covered_counts.groupby(level=0).apply(lambda x: round(100 * x / float(x.sum()), 2)).rename(
             columns={'Covered': 'Coverage'}).reset_index()
         covered_counts.columns = ['Count']
         covered_counts = covered_counts.reset_index()
         coverage_grp = coverage_grp.merge(covered_counts, how='left', on=['response_datetime_interval', 'Covered'])
         coverage_time = coverage_grp[coverage_grp['Covered']==True].reset_index(drop=True)
 
-        start_datetime = coverage_time.response_datetime_interval.iloc[0]
-        end_datetime = coverage_time.response_datetime_interval.iloc[-1]
-        if start_datetime == end_datetime:
-            start_datetime -= delta
-            end_datetime += delta
-            time_index_df = pd.DataFrame([dt for dt in [start_datetime] + coverage_time.response_datetime_interval.tolist() + [end_datetime]],
-                                         columns=['response_datetime_interval'])
-        else:
-            time_index_df = pd.DataFrame([dt for dt in coverage_time.response_datetime_interval.tolist()],
-                             columns=['response_datetime_interval'])
-
-        coverage_data = time_index_df.merge(coverage_time, how='left', on=['response_datetime_interval'])
-        coverage_data['Count'] = coverage_data['Count'].fillna(0)
-        coverage_data['Coverage'] = coverage_data['Coverage'].fillna(0)
-
-        output_notebook(hide_banner=True)
-
-        p = figure(plot_width=950, plot_height=350, x_axis_type="datetime",
-                   x_range=(start_datetime, end_datetime),
-                   y_range=(max(np.floor(coverage_data['Coverage'].min()) - 10, 0),
-                            min(np.floor(coverage_data['Coverage'].max()) + 10, 100)), title='Coverage over time')
-
-        p.line(x='response_datetime_interval', y='Coverage', source=coverage_data, line_width=1.5, color='#4fa8f6')
-
-        p.xaxis.formatter = DatetimeTickFormatter(
-            seconds=["%Y-%m-%d %H:%M:%S"],
-            minsec=["%Y-%m-%d %H:%M:%S"],
-            minutes=["%Y-%m-%d %H:%M:%S"],
-            hourmin=["%Y-%m-%d %H:%M:%S"],
-            hours=["%Y-%m-%d %H:%M:%S"],
-            days=["%Y-%m-%d %H:%M:%S"],
-            months=["%Y-%m-%d %H:%M:%S"],
-            years=["%Y-%m-%d %H:%M:%S"],
-        )
-        p.xaxis.major_label_orientation = 0.5
-        p.yaxis.axis_label = 'Coverage %'
+        if len(coverage_time) > 0:
+            start_datetime = coverage_time.response_datetime_interval.iloc[0]
+            end_datetime = coverage_time.response_datetime_interval.iloc[-1]
+            if start_datetime == end_datetime:
+                start_datetime -= delta
+                end_datetime += delta
+                time_index_df = pd.DataFrame([dt for dt in [start_datetime] + coverage_time.response_datetime_interval.tolist() + [end_datetime]],
+                                            columns=['response_datetime_interval'])
+            else:
+                time_index_df = pd.DataFrame([dt for dt in coverage_time.response_datetime_interval.tolist()],
+                                columns=['response_datetime_interval'])
 
-        hover = HoverTool(
-            tooltips=[
-                ("Datetime", "@response_datetime_interval{%Y-%m-%d %H:%M:%S}"),
-                ("Count", "@Count"),
-                ("Coverage", "@Coverage{0.00}%")
-            ],
-            formatters={
-                '@response_datetime_interval': 'datetime'
-            },
-        )
-        p.add_tools(hover)
-        p.title.align = 'center'
-        p.title.text_font_size = '12pt'
-        p.axis.major_label_text_font_size = "10pt"
-        show(p)
+            coverage_data = time_index_df.merge(coverage_time, how='left', on=['response_datetime_interval'])
+            coverage_data['Count'] = coverage_data['Count'].fillna(0)
+            coverage_data['Coverage'] = coverage_data['Coverage'].fillna(0)
+
+            output_notebook(hide_banner=True)
+
+            p = figure(width=950, height=350, x_axis_type="datetime",
+                    x_range=(start_datetime, end_datetime),
+                    y_range=(max(np.floor(coverage_data['Coverage'].min()) - 10, 0),
+                                min(np.floor(coverage_data['Coverage'].max()) + 10, 100)), title='Coverage over time')
+
+            p.line(x='response_datetime_interval', y='Coverage', source=coverage_data, line_width=1.5, color='#4fa8f6')
+
+            p.xaxis.formatter = DatetimeTickFormatter(
+                seconds=["%Y-%m-%d %H:%M:%S"],
+                minsec=["%Y-%m-%d %H:%M:%S"],
+                minutes=["%Y-%m-%d %H:%M:%S"],
+                hourmin=["%Y-%m-%d %H:%M:%S"],
+                hours=["%Y-%m-%d %H:%M:%S"],
+                days=["%Y-%m-%d %H:%M:%S"],
+                months=["%Y-%m-%d %H:%M:%S"],
+                years=["%Y-%m-%d %H:%M:%S"],
+            )
+            p.xaxis.major_label_orientation = 0.5
+            p.yaxis.axis_label = 'Coverage %'
+
+            hover = HoverTool(
+                tooltips=[
+                    ("Datetime", "@response_datetime_interval{%Y-%m-%d %H:%M:%S}"),
+                    ("Count", "@Count"),
+                    ("Coverage", "@Coverage{0.00}%")
+                ],
+                formatters={
+                    '@response_datetime_interval': 'datetime'
+                },
+            )
+            p.add_tools(hover)
+            p.title.align = 'center'
+            p.title.text_font_size = '12pt'
+            p.axis.major_label_text_font_size = "10pt"
+            show(p)
 
 
 def show_top_node_effort(disambiguation_utterances, top=10, assistant_nodes=None):
     node_title_map = dict()
     if assistant_nodes is not None:
         for idx, node in assistant_nodes.iterrows():
             if str(node['title']) != 'nan':
@@ -452,15 +453,15 @@
         else:
             dialog_node_effort_overall_df.at[idx, 'selected_dialog_node_name'] = item.selected_dialog_node
 
     output_notebook(hide_banner=True)
 
     source = ColumnDataSource(dialog_node_effort_overall_df.head(top))
 
-    p = figure(plot_width=950, plot_height=350,
+    p = figure(width=950, height=350,
                y_range=dialog_node_effort_overall_df.head(top)['selected_dialog_node_name'].iloc[::-1],
                x_range=DataRange1d(start=0), title='Nodes yield the highest customer effort')
 
     p.hbar(y='selected_dialog_node_name', left='effort_score', source=source, height=0.4, fill_color='#BFC5CD',
            line_color='#BFC5CD', hover_fill_color='#1C679A', hover_line_color='#1C679A')
 
     hover = HoverTool(
@@ -608,15 +609,15 @@
         node_effort_df = time_index_df[['request_datetime_interval', 'effort_score_{}'.format(default_node_name)]]
         node_effort_df.columns = ['request_datetime_interval', 'effort_score']
         output_notebook(hide_banner=True)
 
         source = ColumnDataSource(node_effort_df)
         source_all = ColumnDataSource(time_index_df)
 
-        p = figure(plot_width=950, plot_height=350, x_axis_type="datetime",
+        p = figure(width=950, height=350, x_axis_type="datetime",
                    x_range=(start_datetime - start_delta, end_datetime + end_delta),
                    y_range=DataRange1d(start=0), title='Dialog node: "{}"'.format(default_node_name))
 
         p.vbar(x='request_datetime_interval', top='effort_score', source=source, width=bar_width, fill_color='#BFC5CD',
                line_color='#BFC5CD', hover_fill_color='#1C679A', hover_line_color='#1C679A')
 
         p.xaxis.formatter = DatetimeTickFormatter(
@@ -778,15 +779,15 @@
         node_effort_df = time_index_df[['request_datetime_interval', 'effort_score_0']]
         node_effort_df.columns = ['request_datetime_interval', 'effort_score']
         output_notebook(hide_banner=True)
 
         source = ColumnDataSource(node_effort_df)
         source_all = ColumnDataSource(time_index_df)
 
-        p = figure(plot_width=950, plot_height=350, x_axis_type="datetime",
+        p = figure(width=950, height=350, x_axis_type="datetime",
                    x_range=(start_datetime - start_delta, end_datetime + end_delta),
                    y_range=DataRange1d(start=0), title='Utterance: "{}"'.format(input_effort_options[0]))
 
         p.vbar(x='request_datetime_interval', top='effort_score', source=source, width=bar_width, fill_color='#BFC5CD',
                line_color='#BFC5CD', hover_fill_color='#1C679A', hover_line_color='#1C679A')
 
         p.xaxis.formatter = DatetimeTickFormatter(
@@ -956,15 +957,15 @@
         colors = tuple(
             [(int(255 * (0.1 + 0.7 * (1 - i * 0.2))), int(255 * (0.4 + 0.4 * (1 - i * 0.2))), int(255 * 0.8), 0.8) for i
              in
              range(5)])
 
         output_notebook(hide_banner=True)
 
-        p = figure(plot_width=950, plot_height=350, x_axis_type="datetime",
+        p = figure(width=950, height=350, x_axis_type="datetime",
                    x_range=(start_datetime - start_delta, end_datetime + end_delta),
                    y_range=DataRange1d(start=0), title='Disambiguation click distribution over time')
         p.grid.minor_grid_line_color = '#eeeeee'
         names = ["click_on_%d" % i for i in range(1, 6)]
         legend_names = ["Click-%d" % i for i in range(1, 6)]
 
         p.vbar_stack(names, x='request_datetime_interval', color=colors, source=vis_df, width=bar_width,
@@ -1115,15 +1116,15 @@
         column_names.extend([i for i in range(5)])
         vis_df = select_rank_df[column_names].copy()
         vis_df.columns = ['request_datetime_interval'] + ["click_on_%d" % i for i in range(1, 6)]
         vis_df['total'] = vis_df[["click_on_%d" % i for i in range(1, 6)]].sum(axis=1)
 
         output_notebook(hide_banner=True)
 
-        p = figure(plot_width=950, plot_height=350, x_axis_type="datetime",
+        p = figure(width=950, height=350, x_axis_type="datetime",
                    x_range=(start_datetime - start_delta, end_datetime + end_delta),
                    y_range=DataRange1d(start=0), title='More options click distribution over time')
         p.grid.minor_grid_line_color = '#eeeeee'
         names = ["click_on_%d" % i for i in range(1, 6)]
         legend_names = ["Click-%d" % i for i in range(1, 6)]
 
         colors = tuple(
@@ -1186,15 +1187,15 @@
     cooccurrence_matrix.index.name = 'Node B'
 
     df = pd.DataFrame(cooccurrence_matrix.stack(), columns=['count']).reset_index()
     source = ColumnDataSource(df)
     mapper = LinearColorMapper(palette=tuple(reversed(brewer['Blues'][256])), low=df['count'].min(),
                                high=df['count'].max())
     num_elements = cooccurrence_matrix.shape[0]
-    p = figure(plot_width=700 + 8 * num_elements, plot_height=600 + 8 * num_elements, title="Node Co-occurrence Map",
+    p = figure(width=700 + 8 * num_elements, height=600 + 8 * num_elements, title="Node Co-occurrence Map",
                x_range=list(cooccurrence_matrix.index), y_range=list(reversed(cooccurrence_matrix.columns)),
                toolbar_location=None, tools="hover")
 
     p.rect(x="Node A", y="Node B", width=0.9, height=0.9, fill_alpha=1, source=source,
            line_color=None, fill_color=transform('count', mapper), hover_line_color="#08306b")
 
     color_bar = ColorBar(color_mapper=mapper, location=(0, 0),
@@ -1421,15 +1422,15 @@
         output_notebook(hide_banner=True)
 
         colors = tuple(
             [(int(255 * (0.1 + 0.7 * (1 - i * 0.2))), int(255 * (0.4 + 0.4 * (1 - i * 0.2))), int(255 * 0.8), 0.8) for i
              in
              range(3)])
 
-        p = figure(plot_width=950, plot_height=350, x_axis_type="datetime",
+        p = figure(width=950, height=350, x_axis_type="datetime",
                    x_range=(start_datetime - start_delta, end_datetime + end_delta),
                    y_range=(0, effort_data['effort_score_sum'].max() * 1.3),
                    title='Customer effort vs clicks over time')
         p.yaxis.axis_label = 'Customer Effort'
 
         # Setting the second y axis range name and range
 
@@ -1770,15 +1771,15 @@
         half_axis_sum = effort_data['effort_score_sum'].max() * 1.1 // 2
         legend_position = 'top_right'
         if min_sum < half_axis_sum:
             legend_position = 'bottom_right'
 
         output_notebook(hide_banner=True)
 
-        p = figure(plot_width=950, plot_height=350, x_axis_type="datetime",
+        p = figure(width=950, height=350, x_axis_type="datetime",
                    x_range=(start_datetime, end_datetime),
                    y_range=(0, effort_data['effort_score_sum'].max() * 1.1), title='Total customer effort over time')
         p.yaxis.axis_label = 'Total Customer Effort'
 
         p.extra_y_ranges["effort_score_mean"] = Range1d(start=0, end=effort_data['effort_score_mean'].max() * 1.1)
 
         p.grid.minor_grid_line_color = '#eeeeee'
@@ -2192,15 +2193,15 @@
         df_comb = pd.concat([df_time_interval, df_comb], axis=1)
         df_comb.columns = ['request_datetime_interval', 'Disambiguation', 'Single', 'dis_h', 'single_h', 'dis_l',
                            'single_l']
 
         df_comb['Total'] = df_comb['Disambiguation'] + df_comb['Single']
         output_notebook(hide_banner=True)
 
-        p = figure(plot_width=950, plot_height=350, x_axis_type="datetime",
+        p = figure(width=950, height=350, x_axis_type="datetime",
                    x_range=(start_datetime - start_delta, end_datetime + end_delta), title='Disambiguation vs single answer over time')
 
         source = ColumnDataSource(df_comb)
         p.vbar(x='request_datetime_interval', bottom=0, top='dis_h', width=bar_width, source=source, color='#4b86b4',
                legend_label='Disambiguation')
         p.vbar(x='request_datetime_interval', bottom='dis_h', top=1, width=bar_width, source=source, color='#adcbe3',
                legend_label='Single Answer')
```

### Comparing `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit/watson_assistant_func.py` & `assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit/watson_assistant_func.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,21 +213,21 @@
                 return load_logs_from_file(filename, None)
             else:
                 file_exist = True
     else:
         print('Please provide a valid filename.')
         return None
 
-    # adding default filters based on assistant_id and workspace_id
-    if assistant_id is not None and len(assistant_id) > 0:
-        filters.append('request.context.system.assistant_id::{}'.format(assistant_id))
-    if skill_id is not None and len(skill_id) > 0:
-        filters.append('workspace_id::{}'.format(skill_id))
-
     if version == 1:
+        # adding default filters based on assistant_id and workspace_id
+        if assistant_id is not None and len(assistant_id) > 0:
+            filters.append('request.context.system.assistant_id::{}'.format(assistant_id))
+        if skill_id is not None and len(skill_id) > 0:
+            filters.append('workspace_id::{}'.format(skill_id))
+        
         logs = _get_logs_from_v1_api(sdk_object=sdk_v1_object,
                                      workspace_id=workspace_id,
                                      log_filter=','.join(filters),
                                      num_logs=num_logs)
     elif version == 2:
         logs = _get_logs_from_v2_api(sdk_object=sdk_v2_object,
                                      environment_id=environment_id,
```

### Comparing `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/PKG-INFO` & `assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant-improve-toolkit
-Version: 1.4.0
+Version: 1.4.1
 Summary: Assistant Improve Toolkit
 Home-page: https://github.com/watson-developer-cloud/assistant-improve-recommendations-notebook
 Author: IBM Watson
 Author-email: watdevex@us.ibm.com
 Maintainer: Zhe Zhang
 Maintainer-email: zhangzhe@us.ibm.com
 License: Apache 2.0
```

### Comparing `assistant_improve_toolkit-1.4.0/src/assistant_improve_toolkit.egg-info/SOURCES.txt` & `assistant_improve_toolkit-1.4.1/src/assistant_improve_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/main/python/__init__.py` & `assistant_improve_toolkit-1.4.1/src/main/python/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/main/python/computation_func.py` & `assistant_improve_toolkit-1.4.1/src/main/python/computation_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/main/python/cos_op.py` & `assistant_improve_toolkit-1.4.1/src/main/python/cos_op.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/main/python/export_csv_for_intent_recommendation.py` & `assistant_improve_toolkit-1.4.1/src/main/python/export_csv_for_intent_recommendation.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/main/python/fetch_logs.py` & `assistant_improve_toolkit-1.4.1/src/main/python/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/main/python/visualize_func.py` & `assistant_improve_toolkit-1.4.1/src/main/python/visualize_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/main/python/watson_assistant_func.py` & `assistant_improve_toolkit-1.4.1/src/main/python/watson_assistant_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.4.0/src/main/python/watson_assistant_func_skip.py` & `assistant_improve_toolkit-1.4.1/src/main/python/watson_assistant_func_skip.py`

 * *Files identical despite different names*

