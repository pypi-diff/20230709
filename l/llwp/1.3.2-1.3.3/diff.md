# Comparing `tmp/llwp-1.3.2.tar.gz` & `tmp/llwp-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llwp-1.3.2.tar", last modified: Wed May 10 08:29:59 2023, max compression
+gzip compressed data, was "llwp-1.3.3.tar", last modified: Sun Jul  9 15:15:17 2023, max compression
```

## Comparing `llwp-1.3.2.tar` & `llwp-1.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:29:59.709115 llwp-1.3.2/
--rw-rw-rw-   0        0        0      832 2023-04-18 13:31:13.000000 llwp-1.3.2/LICENSE
--rw-rw-rw-   0        0        0       21 2023-03-29 19:59:21.000000 llwp-1.3.2/MANIFEST.in
--rw-rw-rw-   0        0        0      981 2023-05-10 08:29:59.709115 llwp-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-03-29 18:29:00.000000 llwp-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 08:29:59.677865 llwp-1.3.2/llwp/
--rw-rw-rw-   0        0        0   230232 2023-05-09 18:07:29.000000 llwp-1.3.2/llwp/LLWP.py
--rw-rw-rw-   0        0        0     1193 2022-09-29 19:12:05.000000 llwp-1.3.2/llwp/LLWP.svg
--rw-rw-rw-   0        0        0       20 2023-03-29 18:18:08.000000 llwp-1.3.2/llwp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:29:59.709115 llwp-1.3.2/llwp.egg-info/
--rw-rw-rw-   0        0        0      981 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      807 2023-05-10 08:19:00.000000 llwp-1.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 08:29:59.709115 llwp-1.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 15:15:17.438122 llwp-1.3.3/
+-rw-rw-rw-   0        0        0      832 2023-04-18 13:31:13.000000 llwp-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-03-29 19:59:21.000000 llwp-1.3.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      981 2023-07-09 15:15:17.438122 llwp-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-03-29 18:29:00.000000 llwp-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-09 15:15:17.423565 llwp-1.3.3/llwp/
+-rw-rw-rw-   0        0        0   230270 2023-06-27 14:16:48.000000 llwp-1.3.3/llwp/LLWP.py
+-rw-rw-rw-   0        0        0     1193 2022-09-29 19:12:05.000000 llwp-1.3.3/llwp/LLWP.svg
+-rw-rw-rw-   0        0        0       20 2023-03-29 18:18:08.000000 llwp-1.3.3/llwp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 15:15:17.438122 llwp-1.3.3/llwp.egg-info/
+-rw-rw-rw-   0        0        0      981 2023-07-09 15:15:17.000000 llwp-1.3.3/llwp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-09 15:15:17.000000 llwp-1.3.3/llwp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 15:15:17.000000 llwp-1.3.3/llwp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-09 15:15:17.000000 llwp-1.3.3/llwp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2023-07-09 15:15:17.000000 llwp-1.3.3/llwp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-09 15:15:17.000000 llwp-1.3.3/llwp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      807 2023-07-09 15:11:29.000000 llwp-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 15:15:17.438122 llwp-1.3.3/setup.cfg
```

### Comparing `llwp-1.3.2/LICENSE` & `llwp-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llwp-1.3.2/PKG-INFO` & `llwp-1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llwp
-Version: 1.3.2
+Version: 1.3.3
 Summary: LLWP is a fast, efficient and easy solution for exploring and assigning spectra - relying on Loomis-Wood plots.
 Author-email: Luis Bonah <bonah@ph1.uni-koeln.de>
 Project-URL: Homepage, https://llwp.astro.uni-koeln.de/
 Keywords: LLWP,Loomis-Wood Plots,Spectroscopy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `llwp-1.3.2/llwp/LLWP.py` & `llwp-1.3.3/llwp/LLWP.py`

 * *Files 1% similar despite different names*

```diff
@@ -3016,19 +3016,19 @@
 		if tmp_min:
 			condition.append(f"{tmp_min} <= x")
 		if tmp_max:
 			condition.append(f"x <= {tmp_max}")
 
 		tmp_condition = []
 		if main.config["seriesfinderwindow_atype"]:
-			tmp_condition.append(f"(abs(qnu2-qnl2) == 0 and abs(qnu3-qnl3) == 1)")
+			tmp_condition.append(f"(abs(qnu2-qnl2) % 2 == 0 and abs(qnu3-qnl3) % 2 == 1)")
 		if main.config["seriesfinderwindow_btype"]:
-			tmp_condition.append(f"(abs(qnu2-qnl2) == 1 and abs(qnu3-qnl3) == 1)")
+			tmp_condition.append(f"(abs(qnu2-qnl2) % 2 == 1 and abs(qnu3-qnl3) % 2 == 1)")
 		if main.config["seriesfinderwindow_ctype"]:
-			tmp_condition.append(f"(abs(qnu2-qnl2) == 1 and abs(qnu3-qnl3) == 0)")
+			tmp_condition.append(f"(abs(qnu2-qnl2) % 2 == 1 and abs(qnu3-qnl3) % 2 == 0)")
 		if tmp_condition:
 			condition.append(" or ".join(tmp_condition))
 		condition = " and ".join([f"({x})" for x  in condition])
 
 		tmp_cat_df = main.get_visible_data("cat")
 
 		if condition:
@@ -3050,15 +3050,15 @@
 
 			tmp_cat_df = pd.merge(tmp_cat_df, tmp_lin_df, how="outer", on=qns_visible)
 			tmp_cat_df = tmp_cat_df[tmp_cat_df.DROP != True]
 			unassigned = "without already assigned lines"
 		else:
 			unassigned = "with already assigned lines"
 
-		tmp_cat_df["y"] = np.log(tmp_cat_df["y"])/np.log(10)
+		tmp_cat_df["y"] = np.log10(tmp_cat_df["y"])
 		tmp_cat_df = tmp_cat_df.nlargest(nor, "y")
 
 		if tmp_min and tmp_max:
 			xrange = f"in the range from {tmp_min} to {tmp_max}"
 		else:
 			xrange = "in the total range"
 		message = f"The {nor} most intense predicted transitions {unassigned} {xrange} are shown below."
@@ -3104,14 +3104,15 @@
 		super().__init__(id, parent)
 		self.setWindowTitle("Assign Blend")
 
 		self.init_gui()
 		self.update_gui(entries, dict_, index)
 
 	def update_gui(self, entries, dict_, index):
+		self.noq = main.config["series_qns"]
 		self.entries = entries.reset_index(drop=True)
 		self.xmiddle = dict_["x"]
 		self.index = index
 		self.error = dict_["error"]
 
 		self.label.setText(f"Assigning Blend for position {self.xmiddle}.")
 
@@ -3150,15 +3151,14 @@
 	def init_gui(self):
 		layout = QVBoxLayout()
 		self.setLayout(layout)
 
 		self.label = QQ(QLabel)
 		layout.addWidget(self.label)
 
-		self.noq = main.config["series_qns"]
 		self.table = QTableWidget()
 		self.cols = ["x", "y", "dist"] + [f"qn{ul}{i+1}" for ul in ("u", "l") for i in range(6)] + ["filename"]
 		self.table.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
 		self.table.setRowCount(0)
 		self.table.setColumnCount(len(self.cols)+1)
 		self.table.setHorizontalHeaderLabels(["Y/N", "x", "log. y", "Dist"] +  [f"{ul}{i+1}" for ul in ("U", "L") for i in range(6)] + ["Filename"])
 		layout.addWidget(self.table)
@@ -3203,15 +3203,14 @@
 			for i in range(6):
 				tmp_dict[f"qnu{i+1}"] = pyckett.SENTINEL
 				tmp_dict[f"qnl{i+1}"] = pyckett.SENTINEL
 
 			for i in range(self.noq):
 				tmp_dict[f"qnu{i+1}"] = row[f"qnu{i+1}"]
 				tmp_dict[f"qnl{i+1}"] = row[f"qnl{i+1}"]
-
 			main.plotwidget.assign(None, tmp_dict)
 
 		main.plotwidget.set_data()
 		self.close()
 
 class PipeWindow(EQWidget):
 	def __init__(self, id, parent=None):
@@ -4758,16 +4757,16 @@
 				table.setItem(currRowCount, j+1, QTableWidgetItem(val))
 			tmpd = {key: row[key] for key in qns_visible}
 			tmpd["xpre"] = row["x"]
 			table.setCellWidget(currRowCount, 0, QQ(QPushButton, text="Assign", change=lambda x, tmpd=tmpd: self.table_save(tmpd)))
 
 		
 		for i in range(6):
-			table.setColumnHidden(i+ len(tmp) + 2, i>=noq)
-			table.setColumnHidden(i+ len(tmp) + 8, i>=noq)
+			table.setColumnHidden(i+ len(tmp) + 1, i>=noq)
+			table.setColumnHidden(i+ len(tmp) + 7, i>=noq)
 
 		table.resizeColumnsToContents()
 		layout.addWidget(table)
 
 		buttons = QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
 		buttonBox = QDialogButtonBox(buttons)
 		buttonBox.accepted.connect(lambda: self.selector_save(1))
@@ -5893,15 +5892,15 @@
 
 		while i < len(cells):
 			tmp = []
 			row = cells[i].row()
 			while i < len(cells) and cells[i].row() == row:
 				tmp.append(cells[i].data())
 				i += 1
-			output.append("\t".join(tmp))
+			output.append("\t".join(map(str, tmp)))
 		output = "\n".join(output)
 		QApplication.clipboard().setText(output)
 
 	elif event.key() == Qt.Key.Key_V and (event.modifiers() == Qt.KeyboardModifier.ControlModifier):
 		if QAbstractItemView.EditTrigger.NoEditTriggers == self.editTriggers():
 			return
 		cells = sorted(self.selectedIndexes())
@@ -6060,15 +6059,15 @@
 		gauss = gauss/(2*np.sqrt(2*np.log(2)))
 		lorentz = lorentz/2
 		if gauss == 0 and lorentz == 0:
 			return [0 if i!=x_0 else np.inf for i in x]
 		ys = special.voigt_profile(x-x_0, gauss, lorentz)
 
 	for i in range(0, int(derivative)):
-		ys = np.gradient(ys)
+		ys = np.gradient(ys, edge_order=2)
 	if derivative%2 == 0 and derivative != 0 and derivative%4 != 0:
 		ys = -ys
 	ymax = np.max(ys) if np.isfinite(ys).any() else 1
 	if not np.isfinite(ymax) or ymax == 0:
 		ymax = 1
 	ys = amp*ys/ymax
 	return(ys)
```

### Comparing `llwp-1.3.2/llwp/LLWP.svg` & `llwp-1.3.3/llwp/LLWP.svg`

 * *Files identical despite different names*

### Comparing `llwp-1.3.2/llwp.egg-info/PKG-INFO` & `llwp-1.3.3/llwp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llwp
-Version: 1.3.2
+Version: 1.3.3
 Summary: LLWP is a fast, efficient and easy solution for exploring and assigning spectra - relying on Loomis-Wood plots.
 Author-email: Luis Bonah <bonah@ph1.uni-koeln.de>
 Project-URL: Homepage, https://llwp.astro.uni-koeln.de/
 Keywords: LLWP,Loomis-Wood Plots,Spectroscopy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `llwp-1.3.2/pyproject.toml` & `llwp-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llwp"
-version = "1.3.2"
+version = "1.3.3"
 authors = [
   { name="Luis Bonah", email="bonah@ph1.uni-koeln.de" },
 ]
 description = "LLWP is a fast, efficient and easy solution for exploring and assigning spectra - relying on Loomis-Wood plots."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = ['numpy', 'pandas', 'matplotlib', 'wrapt', 'pyckett', 'scipy', 'PyQt6']
```

