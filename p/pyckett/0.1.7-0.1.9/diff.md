# Comparing `tmp/pyckett-0.1.7.tar.gz` & `tmp/pyckett-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyckett-0.1.7.tar", last modified: Sun Apr 23 10:00:48 2023, max compression
+gzip compressed data, was "pyckett-0.1.9.tar", last modified: Sun Jul  9 15:18:38 2023, max compression
```

## Comparing `pyckett-0.1.7.tar` & `pyckett-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 10:00:48.322937 pyckett-0.1.7/
--rw-rw-rw-   0        0        0     1055 2023-02-26 19:47:50.000000 pyckett-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     3221 2023-04-23 10:00:48.322937 pyckett-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     2718 2023-04-23 09:56:22.000000 pyckett-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 10:00:48.300938 pyckett-0.1.7/pyckett/
--rw-rw-rw-   0        0        0       23 2023-03-09 18:14:18.000000 pyckett-0.1.7/pyckett/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:00:48.320937 pyckett-0.1.7/pyckett/clitools/
--rw-rw-rw-   0        0        0      176 2023-03-16 20:38:05.000000 pyckett-0.1.7/pyckett/clitools/__init__.py
--rw-rw-rw-   0        0        0     7730 2023-04-02 19:00:27.000000 pyckett-0.1.7/pyckett/clitools/addparameters.py
--rw-rw-rw-   0        0        0     7722 2023-04-04 09:42:11.000000 pyckett-0.1.7/pyckett/clitools/automaticfit.py
--rw-rw-rw-   0        0        0     2625 2023-04-02 18:07:15.000000 pyckett-0.1.7/pyckett/clitools/omitparameters.py
--rw-rw-rw-   0        0        0     2892 2023-03-09 18:36:05.000000 pyckett-0.1.7/pyckett/clitools/partitionfunction.py
--rw-rw-rw-   0        0        0     4569 2023-04-04 09:37:24.000000 pyckett-0.1.7/pyckett/clitools/separatefits.py
--rw-rw-rw-   0        0        0     2388 2023-04-05 08:23:32.000000 pyckett-0.1.7/pyckett/clitools/uncertainties.py
--rw-rw-rw-   0        0        0    30442 2023-04-16 12:03:16.000000 pyckett-0.1.7/pyckett/pyckett.py
-drwxrwxrwx   0        0        0        0 2023-04-23 10:00:48.313937 pyckett-0.1.7/pyckett.egg-info/
--rw-rw-rw-   0        0        0     3221 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      495 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      326 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-23 10:00:48.000000 pyckett-0.1.7/pyckett.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      989 2023-04-23 10:00:23.000000 pyckett-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-23 10:00:48.322937 pyckett-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 15:18:38.951298 pyckett-0.1.9/
+-rw-rw-rw-   0        0        0     1055 2023-02-26 19:47:50.000000 pyckett-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     3221 2023-07-09 15:18:38.951298 pyckett-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2718 2023-04-23 09:56:22.000000 pyckett-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 15:18:38.916864 pyckett-0.1.9/pyckett/
+-rw-rw-rw-   0        0        0       23 2023-03-09 18:14:18.000000 pyckett-0.1.9/pyckett/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:18:38.949300 pyckett-0.1.9/pyckett/clitools/
+-rw-rw-rw-   0        0        0      176 2023-03-16 20:38:05.000000 pyckett-0.1.9/pyckett/clitools/__init__.py
+-rw-rw-rw-   0        0        0     7752 2023-06-27 12:09:50.000000 pyckett-0.1.9/pyckett/clitools/addparameters.py
+-rw-rw-rw-   0        0        0     7722 2023-04-04 09:42:11.000000 pyckett-0.1.9/pyckett/clitools/automaticfit.py
+-rw-rw-rw-   0        0        0     2625 2023-04-02 18:07:15.000000 pyckett-0.1.9/pyckett/clitools/omitparameters.py
+-rw-rw-rw-   0        0        0     2892 2023-03-09 18:36:05.000000 pyckett-0.1.9/pyckett/clitools/partitionfunction.py
+-rw-rw-rw-   0        0        0     4630 2023-06-13 19:39:14.000000 pyckett-0.1.9/pyckett/clitools/separatefits.py
+-rw-rw-rw-   0        0        0     2388 2023-04-05 08:23:32.000000 pyckett-0.1.9/pyckett/clitools/uncertainties.py
+-rw-rw-rw-   0        0        0    31151 2023-06-12 18:42:24.000000 pyckett-0.1.9/pyckett/pyckett.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:18:38.937487 pyckett-0.1.9/pyckett.egg-info/
+-rw-rw-rw-   0        0        0     3221 2023-07-09 15:18:38.000000 pyckett-0.1.9/pyckett.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2023-07-09 15:18:38.000000 pyckett-0.1.9/pyckett.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 15:18:38.000000 pyckett-0.1.9/pyckett.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      326 2023-07-09 15:18:38.000000 pyckett-0.1.9/pyckett.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-07-09 15:18:38.000000 pyckett-0.1.9/pyckett.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-09 15:18:38.000000 pyckett-0.1.9/pyckett.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      989 2023-07-09 15:17:34.000000 pyckett-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 15:18:38.951298 pyckett-0.1.9/setup.cfg
```

### Comparing `pyckett-0.1.7/LICENSE` & `pyckett-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyckett-0.1.7/PKG-INFO` & `pyckett-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyckett
-Version: 0.1.7
+Version: 0.1.9
 Summary: A wrapper around Pickett's SPFIT and SPCAT
 Author-email: Luis Bonah <bonah@ph1.uni-koeln.de>
 Project-URL: Homepage, https://github.com/Ltotheois/Pyckett/
 Keywords: pickett,spectroscopy,spfit,spcat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyckett-0.1.7/README.md` & `pyckett-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyckett-0.1.7/pyckett/clitools/addparameters.py` & `pyckett-0.1.9/pyckett/clitools/addparameters.py`

 * *Files 5% similar despite different names*

```diff
@@ -138,19 +138,19 @@
 		interstates.update([tuple(sorted((v1, v2))) for v1 in newinteraction for v2 in newinteraction if v1 != v2])
 
 	for v2, v1 in interstates:
 		ud = {"v1": v1, "v2": v2}
 		interstate_cands.update(update_base_states(ud, pyckett.INITIAL_PARAMS_INTERACTION))
 
 	rotational_cands = rotational_cands - present_params
-	get_comment = lambda id: ROTATIONAL_PARAMS[pyckett.format_param_id(pyckett.parse_param_id(id, VIB_DIGITS), 0)][0]
+	get_comment = lambda id: ROTATIONAL_PARAMS.get(pyckett.format_param_id(pyckett.parse_param_id(id, VIB_DIGITS), 0), ("",))[0]
 	rotational_cands = [(id, get_comment(id)) for id in rotational_cands]
 	
 	interstate_cands = interstate_cands - present_params
-	get_comment = lambda id: INTERSTATE_PARAMS[pyckett.format_param_id(pyckett.parse_param_id(id, VIB_DIGITS), 0)][0]
+	get_comment = lambda id: INTERSTATE_PARAMS.get(pyckett.format_param_id(pyckett.parse_param_id(id, VIB_DIGITS), 0), ("",))[0]
 	interstate_cands = [(id, get_comment(id)) for id in interstate_cands]	
 	
 	candidates = []
 	if not skiprotational:
 		candidates.extend(rotational_cands)
 	if not skipinterstate:
 		candidates.extend(interstate_cands)
```

### Comparing `pyckett-0.1.7/pyckett/clitools/automaticfit.py` & `pyckett-0.1.9/pyckett/clitools/automaticfit.py`

 * *Files identical despite different names*

### Comparing `pyckett-0.1.7/pyckett/clitools/omitparameters.py` & `pyckett-0.1.9/pyckett/clitools/omitparameters.py`

 * *Files identical despite different names*

### Comparing `pyckett-0.1.7/pyckett/clitools/partitionfunction.py` & `pyckett-0.1.9/pyckett/clitools/partitionfunction.py`

 * *Files identical despite different names*

### Comparing `pyckett-0.1.7/pyckett/clitools/separatefits.py` & `pyckett-0.1.9/pyckett/clitools/separatefits.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,16 @@
 		tmp_lin = lin.query(f"{qnu} in @states and {qnl} in @states").copy()
 	
 		filter_states = lambda x: (x[0] in states and x[1] in states) or (x[0] == ALL_STATES and  x[1] == ALL_STATES) 
 		tmp_params = [x[-1].copy() for x in params if filter_states(x)]
 		tmp_par = par.copy()
 		
 		if not args.keepqns:
-			tmp_par['NVIB'] = max(2, len(states))
+			sign_nvib = -1 if tmp_par['NVIB'] < 0 else 1
+			tmp_par['NVIB'] = max(2, len(states)) * sign_nvib
 			new_vib_digits = pyckett.get_vib_digits(tmp_par) 
 			new_all_states = pyckett.get_all_states(new_vib_digits)
 			
 			translation_dict = {v: i for i, v in enumerate(states)}
 			translation_dict[ALL_STATES] = new_all_states
 			
 			tmp_lin[qnu] = tmp_lin[qnu].replace(translation_dict)
```

### Comparing `pyckett-0.1.7/pyckett/clitools/uncertainties.py` & `pyckett-0.1.9/pyckett/clitools/uncertainties.py`

 * *Files identical despite different names*

### Comparing `pyckett-0.1.7/pyckett/pyckett.py` & `pyckett-0.1.9/pyckett/pyckett.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,34 +20,36 @@
 ZEROTHRESHOLD = 1E-30
 ZERO = 1E-37
 
 SPFIT_PATH = os.environ.get("PYCKETT_SPFIT_PATH")
 SPCAT_PATH = os.environ.get("PYCKETT_SPCAT_PATH")
 
 QNLABELS = ['qnu1', 'qnu2', 'qnu3', 'qnu4', 'qnu5', 'qnu6', 'qnl1', 'qnl2', 'qnl3', 'qnl4', 'qnl5', 'qnl6']
+QNLABELS_ENERGY = ['qn1', 'qn2', 'qn3', 'qn4', 'qn5', 'qn6']
 
 class pickett_int(np.int64):
 	def __new__(cls, value):
-		if np.issubdtype(type(value), np.integer):
+		if type(value) is np.int64:
 			return(value)
 		
 		value = value.strip()
-		
 		if not value:
 			return(SENTINEL)
 
+		init_char = value[0]
+		if init_char.isnumeric():
+			return np.int64(value)
+		
+		elif init_char.isalpha():
+			return np.int64(str(ord(init_char.upper())-55) + value[1:])
+			
 		# Special case for ERHAM cat files
 		# ERHAM writes ** for quantum numbers higher than 99
-		if all([x == "*" for x in value]):
-			return(99)
-
-		if value[0].isalpha():
-			value = str(ord(value[0].upper())-55)+value[1:]
-		
-		return super().__new__(cls, value)
+		elif all([x == "*" for x in value]):
+			return(np.int64(99))
 
 
 cat_dtypes = {
 	'x':		np.float64,
 	'error':	np.float64,
 	'y':		np.float64,
 	'degfreed':	pickett_int,
@@ -393,15 +395,15 @@
 			qn = row[qnlabel]
 			if qn == SENTINEL:
 				qnsstring += "  "
 			else:
 				qnsstring += format_(row[qnlabel], "2d")
 
 		lines.append(f"{freq}{error}{intens}{dof}{elower}{usd}{tag}{qnfmt}{qnsstring}")
-	lines.append("\n")
+	lines.append("")
 	
 	return("\n".join(lines))
 
 def df_to_lin(df):
 	lines = []
 
 	for index, row in df.iterrows():
@@ -433,14 +435,38 @@
 	data = data.drop(columns=[':'])
 	data["filename"] = str(fname)
 	
 	if sort:
 		data.sort_values("egy", inplace=True)
 	return(data)
 
+def df_to_egy(df):
+	lines = []
+
+	for index, row in df.iterrows():
+		iblk = format_(row["iblk"], "5d")
+		indx = format_(row["indx"], "5d")
+		egy  = format_(row["egy"], "18.6f")
+		err  = format_(row["err"], "18.6f")
+		pmix = format_(row["pmix"], "11.6f")
+		we   = format_(row["we"], "5d")
+
+		qnsstring = ""
+		for qnlabel in QNLABELS_ENERGY:
+			qn = row[qnlabel]
+			if qn == SENTINEL:
+				qnsstring += "   "
+			else:
+				qnsstring += format_(row[qnlabel], "3d")
+
+		lines.append(f" {iblk}{indx}{egy}{err}{pmix}{we}:{qnsstring}")
+	lines.append("")
+	
+	return("\n".join(lines))
+
 def parvar_to_dict(fname):
 	result = {}
 	tmp_file = open(fname, "r") if not isinstance(fname, io.StringIO) else fname
 	with tmp_file as file:
 		result["TITLE"] = file.readline().replace("\n", "")
 		
 		keys = ['NPAR', 'NLINE', 'NITR', 'NXPAR', 'THRESH', 'ERRTST', 'FRAC', 'CAL']
```

### Comparing `pyckett-0.1.7/pyckett.egg-info/PKG-INFO` & `pyckett-0.1.9/pyckett.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyckett
-Version: 0.1.7
+Version: 0.1.9
 Summary: A wrapper around Pickett's SPFIT and SPCAT
 Author-email: Luis Bonah <bonah@ph1.uni-koeln.de>
 Project-URL: Homepage, https://github.com/Ltotheois/Pyckett/
 Keywords: pickett,spectroscopy,spfit,spcat
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyckett-0.1.7/pyproject.toml` & `pyckett-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyckett"
-version = "0.1.7"
+version = "0.1.9"
 authors = [
   { name="Luis Bonah", email="bonah@ph1.uni-koeln.de" },
 ]
 description = "A wrapper around Pickett's SPFIT and SPCAT"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ['numpy', 'pandas', 'matplotlib']
```

