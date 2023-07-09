# Comparing `tmp/jamexp-0.1.7.tar.gz` & `tmp/jamexp-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jamexp-0.1.7.tar", max compression
+gzip compressed data, was "jamexp-0.1.8.tar", max compression
```

## Comparing `jamexp-0.1.7.tar` & `jamexp-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      429 2023-03-09 22:36:29.783388 jamexp-0.1.7/README.md
--rw-r--r--   0        0        0       22 2023-03-09 22:36:29.783388 jamexp-0.1.7/jamexp/__init__.py
--rw-r--r--   0        0        0      489 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/cli/helper.py
--rw-r--r--   0        0        0     2415 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/cli/jckill.py
--rw-r--r--   0        0        0     1425 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/cli/jcp_template.py
--rw-r--r--   0        0        0      945 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/cli/jhyd_clean.py
--rw-r--r--   0        0        0     2935 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/cli/jlink.py
--rw-r--r--   0        0        0     1250 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/cli/jnb_clean.py
--rw-r--r--   0        0        0     1099 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/cli/jpin.py
--rw-r--r--   0        0        0     1185 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/cli/jwb_check_running.py
--rw-r--r--   0        0        0      768 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/cli/jwb_clean.py
--rw-r--r--   0        0        0    12075 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/cli/ngc_shell.py
--rw-r--r--   0        0        0     1131 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/cli/star_file.py
--rw-r--r--   0        0        0      113 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/hyd/__init__.py
--rw-r--r--   0        0        0     2935 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/hyd/folder.py
--rw-r--r--   0        0        0     2037 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/template_data/.gitignore
--rw-r--r--   0        0        0     1207 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/template_data/.pre-commit-config.yaml
--rw-r--r--   0        0        0       31 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/utils/__init__.py
--rw-r--r--   0        0        0      323 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/utils/os_shell.py
--rw-r--r--   0        0        0      386 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/utils/timer.py
--rw-r--r--   0        0        0      471 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/wandb_clean/__init__.py
--rw-r--r--   0        0        0      817 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/wandb_clean/filters.py
--rw-r--r--   0        0        0     2260 2023-03-09 22:36:29.784388 jamexp-0.1.7/jamexp/wandb_clean/utils.py
--rw-r--r--   0        0        0     1340 2023-03-09 22:36:31.302482 jamexp-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 jamexp-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      429 2023-07-09 03:11:06.220896 jamexp-0.1.8/README.md
+-rw-r--r--   0        0        0       22 2023-07-09 03:11:06.220896 jamexp-0.1.8/jamexp/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-09 03:11:06.220896 jamexp-0.1.8/jamexp/cli/helper.py
+-rw-r--r--   0        0        0     2415 2023-07-09 03:11:06.220896 jamexp-0.1.8/jamexp/cli/jckill.py
+-rw-r--r--   0        0        0     1425 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/cli/jcp_template.py
+-rw-r--r--   0        0        0      945 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/cli/jhyd_clean.py
+-rw-r--r--   0        0        0     2935 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/cli/jlink.py
+-rw-r--r--   0        0        0     1250 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/cli/jnb_clean.py
+-rw-r--r--   0        0        0     1099 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/cli/jpin.py
+-rw-r--r--   0        0        0     1185 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/cli/jwb_check_running.py
+-rw-r--r--   0        0        0      768 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/cli/jwb_clean.py
+-rw-r--r--   0        0        0    12214 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/cli/ngc_shell.py
+-rw-r--r--   0        0        0     1131 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/cli/star_file.py
+-rw-r--r--   0        0        0      113 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/hyd/__init__.py
+-rw-r--r--   0        0        0     2935 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/hyd/folder.py
+-rw-r--r--   0        0        0     2037 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/template_data/.gitignore
+-rw-r--r--   0        0        0     1207 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/template_data/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       31 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/utils/__init__.py
+-rw-r--r--   0        0        0      323 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/utils/os_shell.py
+-rw-r--r--   0        0        0      386 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/utils/timer.py
+-rw-r--r--   0        0        0      471 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/wandb_clean/__init__.py
+-rw-r--r--   0        0        0      817 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/wandb_clean/filters.py
+-rw-r--r--   0        0        0     2260 2023-07-09 03:11:06.221896 jamexp-0.1.8/jamexp/wandb_clean/utils.py
+-rw-r--r--   0        0        0     1340 2023-07-09 03:11:07.327894 jamexp-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 jamexp-0.1.8/PKG-INFO
```

### Comparing `jamexp-0.1.7/jamexp/cli/jckill.py` & `jamexp-0.1.8/jamexp/cli/jckill.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/cli/jcp_template.py` & `jamexp-0.1.8/jamexp/cli/jcp_template.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/cli/jhyd_clean.py` & `jamexp-0.1.8/jamexp/cli/jhyd_clean.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/cli/jlink.py` & `jamexp-0.1.8/jamexp/cli/jlink.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/cli/jnb_clean.py` & `jamexp-0.1.8/jamexp/cli/jnb_clean.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/cli/jpin.py` & `jamexp-0.1.8/jamexp/cli/jpin.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/cli/jwb_check_running.py` & `jamexp-0.1.8/jamexp/cli/jwb_check_running.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/cli/jwb_clean.py` & `jamexp-0.1.8/jamexp/cli/jwb_clean.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/cli/ngc_shell.py` & `jamexp-0.1.8/jamexp/cli/ngc_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,21 +121,23 @@
         print("#"*10 + f" {status}  Total {len(jobs):<10}" + "#"*10)
         if jobs:
             df = pd.DataFrame([job.get_ls_kv() for job in jobs]).sort_values(
                 sort_keys.get(status, 'id'), ascending=False
             )
             print(df.to_string(index=False))
 
-def collect_job(is_dir, key, ace=2):
-    loc = {
-        1: 'nv-us-east',
-        2: 'nv-us-west',
-        3: 'nv-us-west',
+def collect_job(is_dir, key, ace='w2'):
+    ace = {
+        'w1': 'nv-us-west-1',
+        'w2': 'nv-us-west-2',
+        'w3': 'nv-us-west-3',
+        'e1': 'nv-us-east-1',
+        'e2': 'nv-us-east-2',
+        'e3': 'nv-us-east-3',
     }[ace]
-    ace = f"{loc}-{ace}"
     team = 'deep-imagination' if is_dir else 'lpr-imagine'
     stdout, stderr = run_simple_command(f'ngc batch list --format_type json --team {team} --ace {ace}')
     if stderr:
         print('ngc batch list error')
         print(stderr)
     else:
         list_job = json.loads(stdout)
@@ -144,25 +146,25 @@
         if key:
             parsed_jobs = {k: [job for job in v if key in job.job_name] for k, v in parsed_jobs.items()}
     return parsed_jobs
 
 def _ngc_list(
     is_dir : bool = typer.Option(False, "-t/-T", help="defualt use lpr-imagine, otherwise use deep-imagination"),
     key : str = typer.Option('ml', help='filter key, only show jobs whose names contain the key'),
-    ace : int = typer.Option(2, help='ace number, default 2'),
+    ace : str = typer.Option("w2", help='ace number, default nv-us-west-2'),
     status : str = typer.Option('none', help='filter status, only show jobs whose status is the status'),
 ):
     status = None if status.lower() == 'none' else status
     parsed_jobs = collect_job(is_dir, key, ace)
     ls_print_jobs(parsed_jobs, status)
 
 def _ngc_result(
     is_dir : bool = typer.Option(False, "-t/-T", help="defualt use lpr-imagine, otherwise use deep-imagination"),
     key : str = typer.Option('ml', help='filter key, only show jobs whose names contain the key'),
-    ace : int = typer.Option(2, help='ace number, default 2'),
+    ace : str = typer.Option("w2", help='ace number, default nv-us-west-2'),
     is_fzf : bool = typer.Option(False, "-i/-I", help="use iteractive fzf to select job, default false -> use latest job"),
 ):
     parsed_jobs = collect_job(is_dir, key, ace)
     # parsed_jobs = {k: v if k in [] for k, v in parsed_jobs.items()}
     if 'QUEUED' in parsed_jobs:
         del parsed_jobs['QUEUED']
     if 'STARTING' in parsed_jobs:
@@ -204,15 +206,15 @@
     dir_list = os.listdir(f"{save_dir}/{select_run.job_id}")
     for file_name in dir_list:
         logger.info(f"{save_dir}/{select_run.job_id}/{file_name}")
 
 def _ngc_bash(
     is_dir : bool = typer.Option(False, "-t/-T", help="defualt use lpr-imagine, otherwise use deep-imagination"),
     key : str = typer.Option('ml', help='filter key, only show jobs whose names contain the key'),
-    ace : int = typer.Option(2, help='ace number, default 2'),
+    ace : str = typer.Option("w2", help='ace number, default nv-us-west-2'),
     is_fzf : bool = typer.Option(False, "-i/-I", help="use iteractive fzf to select job, default false -> use latest job"),
 ):
     parsed_jobs = collect_job(is_dir, key, ace)
     all_jobs = []
     for k, v in parsed_jobs.items():
         if k in ['QUEUED', 'STARTING', 'RUNNING']:
             all_jobs.extend(v)
@@ -249,15 +251,15 @@
             time.sleep(5)
         else:
             break
 
 def _ngc_kill(
     is_dir : bool = typer.Option(False, "-t/-T", help="defualt use lpr-imagine, otherwise use deep-imagination"),
     key : str = typer.Option('ml', help='filter key, only show jobs whose names contain the key'),
-    ace : int = typer.Option(2, help='ace number, default 2'),
+    ace : str = typer.Option("w2", help='ace number, default nv-us-west-2'),
     is_fzf : bool = typer.Option(True, "-i/-I", help="use iteractive fzf to select job, default true. otherwise delete all jobs"),
     confirm : bool = typer.Option(False, "-c/-C", help="confirm to kill job, default false -> only print"),
 ):
     parsed_jobs = collect_job(is_dir, key, ace)
     all_jobs = []
     for k, v in parsed_jobs.items():
         if k in ['QUEUED', 'STARTING', 'RUNNING']:
```

### Comparing `jamexp-0.1.7/jamexp/cli/star_file.py` & `jamexp-0.1.8/jamexp/cli/star_file.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/hyd/folder.py` & `jamexp-0.1.8/jamexp/hyd/folder.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/template_data/.gitignore` & `jamexp-0.1.8/jamexp/template_data/.gitignore`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/template_data/.pre-commit-config.yaml` & `jamexp-0.1.8/jamexp/template_data/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/wandb_clean/filters.py` & `jamexp-0.1.8/jamexp/wandb_clean/filters.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/jamexp/wandb_clean/utils.py` & `jamexp-0.1.8/jamexp/wandb_clean/utils.py`

 * *Files identical despite different names*

### Comparing `jamexp-0.1.7/pyproject.toml` & `jamexp-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jamexp"
-version = "0.1.7"
+version = "0.1.8"
 description = "Jam Experiment helper"
 authors = ["Qinsheng <qsh.zh27@gmail.com>"]
 readme = "README.md"
 keywords = ["jam", "experiment"]
 license = "MIT"
 packages = [
     {include = "jamexp"},
```

### Comparing `jamexp-0.1.7/PKG-INFO` & `jamexp-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jamexp
-Version: 0.1.7
+Version: 0.1.8
 Summary: Jam Experiment helper
 License: MIT
 Keywords: jam,experiment
 Author: Qinsheng
 Author-email: qsh.zh27@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

