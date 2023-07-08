# Comparing `tmp/qtmetabolabpy-0.8.7.tar.gz` & `tmp/qtmetabolabpy-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtmetabolabpy-0.8.7.tar", last modified: Mon Feb  6 00:14:15 2023, max compression
+gzip compressed data, was "qtmetabolabpy-0.8.9.tar", last modified: Thu Feb 16 14:19:26 2023, max compression
```

## Comparing `qtmetabolabpy-0.8.7.tar` & `qtmetabolabpy-0.8.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-06 00:14:15.296360 qtmetabolabpy-0.8.7/
--rw-r--r--   0 ludwigc    (501) staff       (20)    35149 2022-10-18 16:45:07.000000 qtmetabolabpy-0.8.7/LICENSE
--rw-r--r--   0 ludwigc    (501) staff       (20)      311 2022-10-18 18:34:32.000000 qtmetabolabpy-0.8.7/MANIFEST.in
--rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-02-06 00:14:15.295351 qtmetabolabpy-0.8.7/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)     2977 2022-10-18 16:44:50.000000 qtmetabolabpy-0.8.7/README.rst
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-06 00:14:14.845093 qtmetabolabpy-0.8.7/qtmetabolabpy/
--rw-r--r--   0 ludwigc    (501) staff       (20)      210 2022-12-12 19:03:28.000000 qtmetabolabpy-0.8.7/qtmetabolabpy/__init__.py
--rwxr-xr-x   0 ludwigc    (501) staff       (20)   367930 2023-01-25 00:13:58.000000 qtmetabolabpy-0.8.7/qtmetabolabpy/__main__.py
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-06 00:14:14.906978 qtmetabolabpy-0.8.7/qtmetabolabpy/mlStarter/
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-06 00:14:14.913668 qtmetabolabpy-0.8.7/qtmetabolabpy/mlStarter/Contents/
--rw-r--r--   0 ludwigc    (501) staff       (20)      884 2022-10-18 18:24:17.000000 qtmetabolabpy-0.8.7/qtmetabolabpy/mlStarter/Contents/Info.plist
--rw-r--r--   0 ludwigc    (501) staff       (20)        9 2022-10-18 18:19:22.000000 qtmetabolabpy-0.8.7/qtmetabolabpy/mlStarter/Contents/PkgInfo
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-06 00:14:14.917766 qtmetabolabpy-0.8.7/qtmetabolabpy/mlStarter/Contents/Resources/
--rw-r--r--   0 ludwigc    (501) staff       (20)   173336 2022-10-18 18:19:22.000000 qtmetabolabpy-0.8.7/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
--rw-r--r--   0 ludwigc    (501) staff       (20)        0 2022-10-18 18:19:22.000000 qtmetabolabpy-0.8.7/qtmetabolabpy/mlStarter/Icon
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-06 00:14:15.284504 qtmetabolabpy-0.8.7/qtmetabolabpy/ui/
--rw-r--r--   0 ludwigc    (501) staff       (20)   231298 2022-12-05 19:14:54.000000 qtmetabolabpy-0.8.7/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
-drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-06 00:14:14.906593 qtmetabolabpy-0.8.7/qtmetabolabpy.egg-info/
--rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-02-06 00:14:14.000000 qtmetabolabpy-0.8.7/qtmetabolabpy.egg-info/PKG-INFO
--rw-r--r--   0 ludwigc    (501) staff       (20)      545 2023-02-06 00:14:14.000000 qtmetabolabpy-0.8.7/qtmetabolabpy.egg-info/SOURCES.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)        1 2023-02-06 00:14:14.000000 qtmetabolabpy-0.8.7/qtmetabolabpy.egg-info/dependency_links.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       62 2023-02-06 00:14:14.000000 qtmetabolabpy-0.8.7/qtmetabolabpy.egg-info/entry_points.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)      119 2023-02-06 00:14:14.000000 qtmetabolabpy-0.8.7/qtmetabolabpy.egg-info/requires.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       14 2023-02-06 00:14:14.000000 qtmetabolabpy-0.8.7/qtmetabolabpy.egg-info/top_level.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)      321 2022-11-17 22:52:22.000000 qtmetabolabpy-0.8.7/requirements.txt
--rw-r--r--   0 ludwigc    (501) staff       (20)       38 2023-02-06 00:14:15.296562 qtmetabolabpy-0.8.7/setup.cfg
--rw-r--r--   0 ludwigc    (501) staff       (20)     3912 2022-10-18 18:11:50.000000 qtmetabolabpy-0.8.7/setup.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.473433 qtmetabolabpy-0.8.9/
+-rw-r--r--   0 ludwigc    (501) staff       (20)    35149 2022-10-18 16:45:07.000000 qtmetabolabpy-0.8.9/LICENSE
+-rw-r--r--   0 ludwigc    (501) staff       (20)      311 2022-10-18 18:34:32.000000 qtmetabolabpy-0.8.9/MANIFEST.in
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-02-16 14:19:26.473235 qtmetabolabpy-0.8.9/PKG-INFO
+-rw-r--r--   0 ludwigc    (501) staff       (20)     2977 2022-10-18 16:44:50.000000 qtmetabolabpy-0.8.9/README.rst
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.464948 qtmetabolabpy-0.8.9/qtmetabolabpy/
+-rw-r--r--   0 ludwigc    (501) staff       (20)      210 2022-12-12 19:03:28.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/__init__.py
+-rwxr-xr-x   0 ludwigc    (501) staff       (20)   370456 2023-02-16 14:09:43.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/__main__.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.467090 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.469274 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/
+-rw-r--r--   0 ludwigc    (501) staff       (20)      884 2022-10-18 18:24:17.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/Info.plist
+-rw-r--r--   0 ludwigc    (501) staff       (20)        9 2022-10-18 18:19:22.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/PkgInfo
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.469778 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/Resources/
+-rw-r--r--   0 ludwigc    (501) staff       (20)   173336 2022-10-18 18:19:22.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns
+-rw-r--r--   0 ludwigc    (501) staff       (20)        0 2022-10-18 18:19:22.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Icon
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.472853 qtmetabolabpy-0.8.9/qtmetabolabpy/ui/
+-rw-r--r--   0 ludwigc    (501) staff       (20)   241807 2023-02-12 22:56:40.000000 qtmetabolabpy-0.8.9/qtmetabolabpy/ui/metabolabpy_mainwindow.ui
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-02-16 14:19:26.466951 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3745 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/PKG-INFO
+-rw-r--r--   0 ludwigc    (501) staff       (20)      545 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)        1 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       62 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/entry_points.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)      119 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/requires.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       14 2023-02-16 14:19:26.000000 qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/top_level.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)      321 2022-11-17 22:52:22.000000 qtmetabolabpy-0.8.9/requirements.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       38 2023-02-16 14:19:26.473482 qtmetabolabpy-0.8.9/setup.cfg
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3912 2022-10-18 18:11:50.000000 qtmetabolabpy-0.8.9/setup.py
```

### Comparing `qtmetabolabpy-0.8.7/LICENSE` & `qtmetabolabpy-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.8.7/PKG-INFO` & `qtmetabolabpy-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.8.7
+Version: 0.8.9
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.8.7/README.rst` & `qtmetabolabpy-0.8.9/README.rst`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.8.7/qtmetabolabpy/__main__.py` & `qtmetabolabpy-0.8.9/qtmetabolabpy/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,16 @@
     import PySide2  # pragma: no cover
     import qtmodern.styles  # pragma: no cover
     from PySide2.QtGui import QPixmap
 except:
     pass
 
 import darkdetect
+import webbrowser
+import pandas as pd
 #import matplotlib.pyplot as pl  # pragma: no cover
 
 if "linux" in sys.platform:  # pragma: no cover
     gui_env = ['TkAgg', 'GTKAgg', 'Qt5Agg', 'WXAgg']  # pragma: no cover
 elif sys.platform == "darwin":  # pragma: no cover
     try:  # pragma: no cover
         gui_env = ['Qt5Agg']  # pragma: no cover
@@ -336,15 +338,15 @@
         self.w.tsaButton.clicked.connect(self.set_pqn_tsa_scaling)
         self.w.addSplineBaselineButton.clicked.connect(self.ginput_spline_baseline)
         self.w.clearSplineBaselineButton.clicked.connect(self.clear_spline_points)
         self.w.resetSplineBaselineButton.clicked.connect(self.reset_spline_points)
         self.w.correctAllButton.clicked.connect(self.corr_spline_baseline)
         self.w.plotBaselineButton.clicked.connect(self.plot_spline_baseline)
         self.w.averagePoints.textChanged.connect(self.get_spline_average_points)
-        self.w.linearSplinePoints.textChanged.connect(self.set_linear_spline_points)
+        self.w.linearSplinePoints.textChanged.connect(self.get_linear_spline_points)
         self.w.fitUpToBonds.currentIndexChanged.connect(self.set_up_to_bonds)
         self.w.autoScaling.clicked.connect(self.set_variance_stabilisation_options)
         self.w.paretoScaling.clicked.connect(self.set_variance_stabilisation_options)
         self.w.gLogTransform.clicked.connect(self.set_variance_stabilisation_options)
         self.w.varianceStabilisation.stateChanged.connect(self.set_variance_stabilisation)
         self.w.exportDataSet.stateChanged.connect(self.set_export_data_set)
         self.w.excludeRegionTW.cellChanged.connect(self.set_exclude_pre_proc)
@@ -513,14 +515,15 @@
         self.w.hsqcAssignedMetabolites.clicked.connect(self.set_hsqc_assigned_metabolite)
         self.w.mlSaveButton.clicked.connect(self.save_ml_info)
         self.w.mlResetButton.clicked.connect(self.reset_ml_info)
         self.w.deleteAssignedHsqc.clicked.connect(self.remove_assigned_metabolite)
         self.w.maFitButton.clicked.connect(self.ma_fit_hsqc_1d)
         # self.w.helpComboBox.currentIndexChanged.connect(self.set_help)
         self.w.helpComboBox.activated.connect(self.set_help)
+        self.w.tutorialComboBox.activated.connect(self.set_tutorial)
         # Quit Button
         self.w.quitButton.clicked.connect(self.quit_app)
         self.w.saveButton.clicked.connect(self.save_button)
         self.w.loadButton.clicked.connect(self.load_button)
         self.w.exportPathSelectButton.clicked.connect(self.set_export_table)
         self.w.actionQuit.triggered.connect(self.quit_app)
         self.w.dispPlotButton.clicked.connect(self.plot_spc_disp)
@@ -1406,15 +1409,15 @@
         self.fill_spline_baseline_tw()
         self.plot_spc(True)
         # end clear_spline_points
 
     def reset_spline_points(self):
         for k in range(len(self.nd.nmrdat[self.nd.s])):
             if self.nd.nmrdat[self.nd.s][k].display.display_spc or k == self.nd.e:
-                self.nd.nmrdat[self.nd.s][k].proc_spc1d()
+                self.nd.nmrdat[self.nd.s][k].proc_spc1d(reset_spline=True)
                 self.nd.nmrdat[self.nd.s][k].add_baseline_points()
 
         self.plot_spc(True)
         # end clear_spline_points
 
     def cnst(self, index=-1):
         if index == -1:
@@ -1520,14 +1523,51 @@
 
         f.close()
         subprocess.os.system('pip install pylnk3')
         subprocess.os.system('pylnk3 create ' + ml_bat + ' ' + link_file + ' -m Minimized --icon ' + icon_file)
         subprocess.os.system('pip uninstall pylnk3 --yes')
         # end create_icon_win
 
+    def create_titles(self, excel_name='', dataset_label='', pos_label='', rack_label='', replace_title=False):
+        if dataset_label == '' or pos_label == '' or rack_label == '':
+            print(f'Usage: create_titles(dataset_label="dataset_label", pos_label="pos_label", rack_label="rack_label", replace_title=False)')
+            return
+
+        if excel_name == '':
+            answer = QFileDialog.getOpenFileName(None, 'Load Excel File', '', '*.xlsx')
+            if answer[0] == '':
+                return
+            else:
+                excel_name = answer[0]
+
+        else:
+            if not os.path.isfile(excel_name):
+                return
+
+        xls = pd.read_excel(excel_name).fillna('')
+        something_not_found = False
+        if len(np.where(xls.columns.str.contains(dataset_label))[0]) == 0:
+            something_not_found = True
+            print(f'dataset_label: {dataset_label} not found.')
+
+        if len(np.where(xls.columns.str.contains(pos_label))[0]) == 0:
+            something_not_found = True
+            print(f'pos_label: {pos_label} not found.')
+
+        if len(np.where(xls.columns.str.contains(rack_label))[0]) == 0:
+            something_not_found = True
+            print(f'rack_label: {rack_label} not found.')
+
+        if something_not_found:
+            return
+
+        self.nd.create_titles(xls, dataset_label, pos_label, rack_label, replace_title, excel_name)
+        self.update_gui()
+        # end create_titles
+
     def d(self, index=-1):
         if index > len(self.nd.nmrdat[self.nd.s][self.nd.e].acq.delay) - 1 or index < -1:
             index = -1
 
         if index == -1:
             print(f'd = {self.nd.nmrdat[self.nd.s][self.nd.e].acq.delay}')
         else:
@@ -4129,39 +4169,56 @@
         # self.w.isotopomerMultiplet.canvas.axes.spines['bottom'].set_color(fg)
         # self.w.isotopomerMultiplet.canvas.axes.spines['top'].set_color(fg)
         # self.w.isotopomerMultiplet.canvas.axes.spines['left'].set_color(fg)
         # self.w.isotopomerMultiplet.canvas.axes.spines['right'].set_color(fg)
         # end load_light_mode
 
     def ma_fit_hsqc_1d(self):
+        if self.cf.mode == 'dark' or (self.cf.mode == 'system' and darkdetect.isDark()):
+            txt_col = QColor.fromRgbF(1.0, 1.0, 1.0, 1.0)
+            err_col = QColor.fromRgbF(1.0, 0.5, 0.5, 1.0)
+        else:
+            txt_col = QColor.fromRgbF(0.0, 0.0, 0.0, 1.0)
+            err_col = QColor.fromRgbF(1.0, 0.0, 0.0, 1.0)
+
+        code_out = io.StringIO()
+        code_err = io.StringIO()
+        sys.stdout = code_out
+        sys.stderr = code_err
+        print('fitting multiplet...')
         fit_again_counter = 0
         auto_scale = self.w.maAutoScale.isChecked()
         if self.w.maAutoScale.isChecked():
             self.w.maAutoScale.setChecked(False)
 
         hsqc = self.nd.nmrdat[self.nd.s][self.nd.e].hsqc
         if hsqc.hsqc_data[hsqc.cur_metabolite].spin_systems[hsqc.cur_peak - 1]['contribution'][0] == 100.0:
             self.nd.nmrdat[self.nd.s][self.nd.e].fit_hsqc_1d()
 
         self.nd.nmrdat[self.nd.s][self.nd.e].fit_hsqc_1d()
         while self.nd.nmrdat[self.nd.s][self.nd.e].fit_hsqc_again:
             if fit_again_counter < 3:
                 fit_again_counter += 1
-                print("self.nd.nmrdat[self.nd.s][self.nd.e].fit_hsqc_again[iteration: {}]: {}".format(fit_again_counter,
-                                                                                                      self.nd.nmrdat[
-                                                                                                          self.nd.s][
-                                                                                                          self.nd.e].fit_hsqc_again))
+                print(f'self.nd.nmrdat[{self.nd.s}][{self.nd.e}].fit_hsqc_again[iteration: {fit_again_counter}]: '
+                      f'{self.nd.nmrdat[self.nd.s][self.nd.e].fit_hsqc_again}')
                 self.nd.nmrdat[self.nd.s][self.nd.e].fit_hsqc_again = False
                 self.nd.nmrdat[self.nd.s][self.nd.e].fit_hsqc_1d()
             else:
                 self.nd.nmrdat[self.nd.s][self.nd.e].fit_hsqc_again = False
 
         # self.hsqc_spin_sys_change()
         self.w.maAutoScale.setChecked(auto_scale)
         self.ma_sim_hsqc_1d()
+        self.w.console.setTextColor(txt_col)
+        self.w.console.append(code_out.getvalue())
+        sys.stdout = sys.__stdout__
+        sys.stderr = sys.__stderr__
+        code_out.close()
+        code_err.close()
+        self.w.console.verticalScrollBar().setValue(self.w.console.verticalScrollBar().maximum())
         # end ma_fit_hsqc_1d
 
     def ma_sim_hsqc_1d(self):
         if self.nd.hsqc_spin_sys_connected == True:
             self.w.hsqcSpinSys.cellChanged.disconnect()
             self.nd.hsqc_spin_sys_connected = False
 
@@ -4981,22 +5038,23 @@
                     else:
                         neg_col = d.neg_col
 
                     pos_col = matplotlib.colors.to_hex(pos_col)
                     neg_col = matplotlib.colors.to_hex(neg_col)
                     self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][k].ppm1,
                                                       self.nd.nmrdat[s][k].spc[0].real, color=pos_col)
+
                     if self.w.splinebaseline.isChecked():
-                        print("isChecked1")
-                        self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][k].spline_baseline.baseline_points,
-                                                          self.nd.nmrdat[s][k].spline_baseline.baseline_values, 'o', color="lightgreen")
-                        if plot_spline_baseline:
-                            self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][k].ppm1,
-                                                              self.nd.nmrdat[s][k].calc_spline_baseline(),
-                                                              color="lightgreen")
+                        if len(self.nd.nmrdat[s][k].spline_baseline.baseline_points) > 0:
+                            self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][k].spline_baseline.baseline_points,
+                                                              self.nd.nmrdat[s][k].spline_baseline.baseline_values, 'o', color="lightgreen")
+                            if plot_spline_baseline:
+                                self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][k].ppm1,
+                                                                  self.nd.nmrdat[s][k].calc_spline_baseline(),
+                                                                  color="lightgreen")
 
             d = self.nd.nmrdat[s][e].display
             if (d.pos_col == "RGB"):
                 pos_col = d.pos_col_rgb
             else:
                 pos_col = d.pos_col
 
@@ -5016,19 +5074,20 @@
                                                              self.nd.nmrdat[s][e].end_peak[k],
                                                              alpha=self.nd.pp.alpha, color=self.nd.pp.colour)
 
             self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[self.nd.s][self.nd.e].ppm1,
                                               self.nd.nmrdat[self.nd.s][self.nd.e].spc[0].real, color=pos_col)
 
             if self.w.splinebaseline.isChecked():
-                self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][e].spline_baseline.baseline_points,
-                                                  self.nd.nmrdat[s][e].spline_baseline.baseline_values, 'o', color="lightgreen")
-                if plot_spline_baseline:
-                    baseline = self.nd.nmrdat[s][e].calc_spline_baseline()
-                    self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][e].ppm1, baseline, color="lightgreen")
+                if len(self.nd.nmrdat[s][k].spline_baseline.baseline_points) > 0:
+                    self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][e].spline_baseline.baseline_points,
+                                                      self.nd.nmrdat[s][e].spline_baseline.baseline_values, 'o', color="lightgreen")
+                    if plot_spline_baseline:
+                        baseline = self.nd.nmrdat[s][e].calc_spline_baseline()
+                        self.w.MplWidget.canvas.axes.plot(self.nd.nmrdat[s][e].ppm1, baseline, color="lightgreen")
 
             self.w.MplWidget.canvas.axes.set_xlabel(xlabel)
             self.w.MplWidget.canvas.axes.autoscale()
             self.w.MplWidget.canvas.axes.invert_xaxis()
             if (self.keep_zoom == True):
                 self.w.MplWidget.canvas.axes.set_xlim(xlim)
                 self.w.MplWidget.canvas.axes.set_ylim(ylim)
@@ -5751,15 +5810,15 @@
 
     def get_linear_spline_points(self):
         try:
             self.nd.nmrdat[self.nd.s][self.nd.e].spline_baseline.linear_spline = int(self.w.linearSplinePoints.text())
         except:
             self.nd.nmrdat[self.nd.s][self.nd.e].spline_baseline.linear_spline = 200
 
-        for k in len(self.nd.nmrdat[self.nd.s]):
+        for k in range(len(self.nd.nmrdat[self.nd.s])):
             if self.nd.nmrdat[self.nd.s][k].display.display_spc:
                 self.nd.nmrdat[self.nd.s][k].spline_baseline.linear_spline = self.nd.nmrdat[self.nd.s][
                     self.nd.e].spline_baseline.linear_spline
 
         self.set_spline_average_points()
         # end set_spline_average_points
 
@@ -6599,14 +6658,22 @@
         url.append("https://www.genome.jp/kegg/pathway.html#metabolism")
         url.append("https://nmrshiftdb.nmr.uni-koeln.de")
         url.append("https://sdbs.db.aist.go.jp/sdbs/cgi-bin/cre_index.cgi")
         url.append("http://dmar.riken.jp/spincouple/")
         self.w.helpView.setUrl(url[idx])
         # end set_help
 
+    def set_tutorial(self):
+        url = []
+        idx = self.w.tutorialComboBox.currentIndex()
+        url.append("https://youtu.be/uUNRintjUIo")
+        url.append("https://youtu.be/AeEoq0bwLJg")
+        webbrowser.open(url[idx], new=2)
+        # end set_help
+
     def set_hsqc_pars1(self):
         self.w.h1Range.setText(str(self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.range_h))
         # end set_hsqc_pars1
 
     def set_hsqc_pars2(self):
         self.w.c13Range.setText(str(self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.range_c))
         # end set_hsqc_pars2
@@ -7111,21 +7178,20 @@
             self.set_hsqc_metabolite()
         except:
             pass
 
         # end set_hsqc_assigned_metabolite
 
     def set_hsqc_metabolite(self):
-        print("set_hsqc_metabolite")
+        #print("set_hsqc_metabolite")
         my_autosim = self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.autosim
         self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.autosim = False
         self.w.openWeb.clear()
         idx = self.w.hsqcMetabolites.currentIndex().row()
         if idx == -1:
-            print("/////////////")
             return
 
         if self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.j_scale == -1:
             self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.j_scale = self.nd.nmrdat[self.nd.s][self.nd.e].acq.cnst[18]
 
         metabolite_name = self.w.hsqcMetabolites.currentIndex().data()
         cur_peak = self.nd.nmrdat[self.nd.s][self.nd.e].hsqc.cur_peak
```

### Comparing `qtmetabolabpy-0.8.7/qtmetabolabpy/mlStarter/Contents/Info.plist` & `qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.8.7/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns` & `qtmetabolabpy-0.8.9/qtmetabolabpy/mlStarter/Contents/Resources/AppIcon.icns`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.8.7/qtmetabolabpy/ui/metabolabpy_mainwindow.ui` & `qtmetabolabpy-0.8.9/qtmetabolabpy/ui/metabolabpy_mainwindow.ui`

 * *Files 8% similar despite different names*

#### Comparing `qtmetabolabpy-0.8.7/qtmetabolabpy/ui/metabolabpy_mainwindow.ui` & `qtmetabolabpy-0.8.9/qtmetabolabpy/ui/metabolabpy_mainwindow.ui`

```diff
@@ -418,15 +418,15 @@
                             <property name="lineWidth">
                               <number>2</number>
                             </property>
                             <property name="midLineWidth">
                               <number>0</number>
                             </property>
                             <property name="currentIndex">
-                              <number>1</number>
+                              <number>0</number>
                             </property>
                             <widget class="QWidget" name="selectClassTab">
                               <layout class="QHBoxLayout" name="horizontalLayout_42">
                                 <item>
                                   <layout class="QVBoxLayout" name="verticalLayout_12">
                                     <item>
                                       <spacer name="verticalSpacer_3">
@@ -847,14 +847,17 @@
                                       </widget>
                                     </item>
                                     <item>
                                       <widget class="QSpinBox" name="segAlignRefSpc">
                                         <property name="minimum">
                                           <number>-1</number>
                                         </property>
+                                        <property name="value">
+                                          <number>1</number>
+                                        </property>
                                       </widget>
                                     </item>
                                     <item>
                                       <spacer name="verticalSpacer_8">
                                         <property name="orientation">
                                           <enum>Qt::Vertical</enum>
                                         </property>
@@ -881,15 +884,15 @@
                                       </widget>
                                     </item>
                                   </layout>
                                 </item>
                                 <item row="0" column="1">
                                   <widget class="QTableWidget" name="segAlignTW">
                                     <property name="rowCount">
-                                      <number>100</number>
+                                      <number>500</number>
                                     </property>
                                     <row>
                                       <property name="text">
                                         <string/>
                                       </property>
                                     </row>
                                     <row>
@@ -1063,14 +1066,414 @@
                                     <row/>
                                     <row/>
                                     <row/>
                                     <row/>
                                     <row/>
                                     <row/>
                                     <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
+                                    <row/>
                                     <column>
                                       <property name="text">
                                         <string>PPM Start</string>
                                       </property>
                                     </column>
                                     <column>
                                       <property name="text">
@@ -6003,27 +6406,54 @@
               </layout>
             </widget>
             <widget class="QWidget" name="helpTab">
               <attribute name="title">
                 <string>Help</string>
               </attribute>
               <layout class="QGridLayout" name="gridLayout_27">
-                <item row="1" column="4">
+                <item row="1" column="5">
                   <widget class="QCheckBox" name="autoUnzip">
                     <property name="text">
                       <string>Auto-unzip downloaded zip files</string>
                     </property>
                     <property name="checked">
                       <bool>true</bool>
                     </property>
                   </widget>
                 </item>
-                <item row="0" column="0" colspan="5">
+                <item row="1" column="3">
+                  <widget class="QPushButton" name="stopNotebookButton">
+                    <property name="text">
+                      <string>Stop Notebook Server</string>
+                    </property>
+                  </widget>
+                </item>
+                <item row="1" column="2">
+                  <widget class="QPushButton" name="startNotebookButton">
+                    <property name="text">
+                      <string>(Re-)Start Notebook Server</string>
+                    </property>
+                  </widget>
+                </item>
+                <item row="0" column="0" colspan="6">
                   <widget class="QWebEngineView2" name="helpView" native="true"/>
                 </item>
+                <item row="1" column="4">
+                  <spacer name="horizontalSpacer_24">
+                    <property name="orientation">
+                      <enum>Qt::Horizontal</enum>
+                    </property>
+                    <property name="sizeHint" stdset="0">
+                      <size>
+                        <width>1208</width>
+                        <height>20</height>
+                      </size>
+                    </property>
+                  </spacer>
+                </item>
                 <item row="1" column="0">
                   <widget class="QComboBox" name="helpComboBox">
                     <item>
                       <property name="text">
                         <string>Help</string>
                       </property>
                     </item>
@@ -6065,39 +6495,26 @@
                     <item>
                       <property name="text">
                         <string>SpinCouple</string>
                       </property>
                     </item>
                   </widget>
                 </item>
-                <item row="1" column="3">
-                  <spacer name="horizontalSpacer_24">
-                    <property name="orientation">
-                      <enum>Qt::Horizontal</enum>
-                    </property>
-                    <property name="sizeHint" stdset="0">
-                      <size>
-                        <width>1208</width>
-                        <height>20</height>
-                      </size>
-                    </property>
-                  </spacer>
-                </item>
                 <item row="1" column="1">
-                  <widget class="QPushButton" name="startNotebookButton">
-                    <property name="text">
-                      <string>(Re-)Start Notebook Server</string>
-                    </property>
-                  </widget>
-                </item>
-                <item row="1" column="2">
-                  <widget class="QPushButton" name="stopNotebookButton">
-                    <property name="text">
-                      <string>Stop Notebook Server</string>
-                    </property>
+                  <widget class="QComboBox" name="tutorialComboBox">
+                    <item>
+                      <property name="text">
+                        <string>Tutorial 1</string>
+                      </property>
+                    </item>
+                    <item>
+                      <property name="text">
+                        <string>Tutorial 2</string>
+                      </property>
+                    </item>
                   </widget>
                 </item>
               </layout>
             </widget>
           </widget>
         </item>
       </layout>
```

### Comparing `qtmetabolabpy-0.8.7/qtmetabolabpy.egg-info/PKG-INFO` & `qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtmetabolabpy
-Version: 0.8.7
+Version: 0.8.9
 Summary: Python package for data processing of NMR 1D and 2D metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/qtmetabolabpy
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `qtmetabolabpy-0.8.7/qtmetabolabpy.egg-info/SOURCES.txt` & `qtmetabolabpy-0.8.9/qtmetabolabpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qtmetabolabpy-0.8.7/setup.py` & `qtmetabolabpy-0.8.9/setup.py`

 * *Files identical despite different names*

