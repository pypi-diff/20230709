# Comparing `tmp/napatrackmater-3.8.8.tar.gz` & `tmp/napatrackmater-3.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-3.8.8.tar", last modified: Sun Jul  9 21:00:23 2023, max compression
+gzip compressed data, was "napatrackmater-3.8.9.tar", last modified: Sun Jul  9 21:11:55 2023, max compression
```

## Comparing `napatrackmater-3.8.8.tar` & `napatrackmater-3.8.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 21:00:23.276116 napatrackmater-3.8.8/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.8.8/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-09 21:00:23.270034 napatrackmater-3.8.8/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.8.8/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 21:00:23.059672 napatrackmater-3.8.8/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.8.8/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.8.8/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   113387 2023-07-09 20:59:41.000000 napatrackmater-3.8.8/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.8.8/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.8.8/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    14304 2023-07-08 08:48:33.000000 napatrackmater-3.8.8/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.8.8/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.8.8/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.8.8/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-09 20:59:50.000000 napatrackmater-3.8.8/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 21:00:23.234546 napatrackmater-3.8.8/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-09 21:00:22.000000 napatrackmater-3.8.8/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-07-09 21:00:22.000000 napatrackmater-3.8.8/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-09 21:00:22.000000 napatrackmater-3.8.8/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-07-09 21:00:22.000000 napatrackmater-3.8.8/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-07-09 21:00:22.000000 napatrackmater-3.8.8/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-07-09 21:00:22.000000 napatrackmater-3.8.8/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-09 21:00:23.277630 napatrackmater-3.8.8/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1410 2023-07-03 08:06:08.000000 napatrackmater-3.8.8/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 21:11:55.135350 napatrackmater-3.8.9/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.8.9/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-09 21:11:55.129768 napatrackmater-3.8.9/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.8.9/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 21:11:54.863864 napatrackmater-3.8.9/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.8.9/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.8.9/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   113282 2023-07-09 21:10:58.000000 napatrackmater-3.8.9/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.8.9/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.8.9/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    14304 2023-07-08 08:48:33.000000 napatrackmater-3.8.9/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.8.9/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.8.9/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.8.9/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-09 21:11:04.000000 napatrackmater-3.8.9/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 21:11:55.090648 napatrackmater-3.8.9/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-07-09 21:11:54.000000 napatrackmater-3.8.9/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-09 21:11:55.138307 napatrackmater-3.8.9/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1410 2023-07-03 08:06:08.000000 napatrackmater-3.8.9/setup.py
```

### Comparing `napatrackmater-3.8.8/LICENSE` & `napatrackmater-3.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.8/PKG-INFO` & `napatrackmater-3.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.8.8
+Version: 3.8.9
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.8.8/README.md` & `napatrackmater-3.8.9/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.8/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.8.9/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.8/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.8.9/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.8/napatrackmater/Trackmate.py` & `napatrackmater-3.8.9/napatrackmater/Trackmate.py`

 * *Files 1% similar despite different names*

```diff
@@ -6309,779 +6309,773 @@
 00018a40: 286d 6974 6f74 6963 5f64 6973 705f 7829  (mitotic_disp_x)
 00018a50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00018a60: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
 00018a70: 7469 635f 7661 725f 6469 7370 5f78 2e61  tic_var_disp_x.a
 00018a80: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
 00018a90: 6f74 6963 5f64 6973 705f 7829 290d 0a0d  otic_disp_x))...
 00018aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ab0: 2020 2020 206d 6173 6b20 3d20 6d69 746f       mask = mito
-00018ac0: 7469 635f 7261 6469 7573 203d 3d20 4e6f  tic_radius == No
-00018ad0: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-00018ae0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00018af0: 6f74 6963 5f6d 6561 6e5f 7261 6469 7573  otic_mean_radius
-00018b00: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00018b10: 6d69 746f 7469 635f 7261 6469 7573 5b7e  mitotic_radius[~
-00018b20: 6d61 736b 5d29 290d 0a20 2020 2020 2020  mask]))..       
-00018b30: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00018b40: 7465 7265 645f 7661 6c75 6573 203d 205b  tered_values = [
-00018b50: 7661 6c20 666f 7220 7661 6c20 696e 206d  val for val in m
-00018b60: 6974 6f74 6963 5f72 6164 6975 7320 6966  itotic_radius if
-00018b70: 2076 616c 2069 7320 6e6f 7420 4e6f 6e65   val is not None
-00018b80: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-00018b90: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
-00018ba0: 7469 635f 7661 725f 7261 6469 7573 2e61  tic_var_radius.a
-00018bb0: 7070 656e 6428 6e70 2e73 7464 2866 696c  ppend(np.std(fil
-00018bc0: 7465 7265 645f 7661 6c75 6573 2929 0d0a  tered_values))..
-00018bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018be0: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-00018bf0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00018c00: 6974 6f74 6963 5f6d 6561 6e5f 7370 6565  itotic_mean_spee
-00018c10: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
-00018c20: 286d 6974 6f74 6963 5f73 7065 6564 2929  (mitotic_speed))
-00018c30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018c40: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
-00018c50: 6963 5f76 6172 5f73 7065 6564 2e61 7070  ic_var_speed.app
-00018c60: 656e 6428 6e70 2e73 7464 286d 6974 6f74  end(np.std(mitot
-00018c70: 6963 5f73 7065 6564 2929 0d0a 0d0a 2020  ic_speed))....  
-00018c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c90: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00018ca0: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
-00018cb0: 702e 6d65 616e 286d 6974 6f74 6963 5f61  p.mean(mitotic_a
-00018cc0: 6363 2929 0d0a 2020 2020 2020 2020 2020  cc))..          
-00018cd0: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
-00018ce0: 6974 6f74 6963 5f76 6172 5f61 6363 2e61  itotic_var_acc.a
-00018cf0: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
-00018d00: 6f74 6963 5f61 6363 2929 0d0a 0d0a 2020  otic_acc))....  
-00018d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d20: 2020 7365 6c66 2e6d 6974 6f74 6963 5f6d    self.mitotic_m
-00018d30: 6561 6e5f 6469 7265 6374 696f 6e61 6c5f  ean_directional_
-00018d40: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
-00018d50: 2e6d 6561 6e28 6d69 746f 7469 635f 6469  .mean(mitotic_di
-00018d60: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00018d70: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00018d80: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
-00018d90: 6f74 6963 5f76 6172 5f64 6972 6563 7469  otic_var_directi
-00018da0: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
-00018db0: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
-00018dc0: 635f 6469 7265 6374 696f 6e61 6c5f 6368  c_directional_ch
-00018dd0: 616e 6765 2929 0d0a 0d0a 2020 2020 2020  ange))....      
-00018de0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018df0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
-00018e00: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018e10: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
-00018e20: 6e28 6d69 746f 7469 635f 6469 7374 616e  n(mitotic_distan
-00018e30: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
-00018e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e50: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
-00018e60: 5f76 6172 5f64 6973 7461 6e63 655f 6365  _var_distance_ce
-00018e70: 6c6c 5f6d 6173 6b2e 6170 7065 6e64 286e  ll_mask.append(n
-00018e80: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
-00018e90: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00018ea0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-00018eb0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00018ec0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00018ed0: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
-00018ee0: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-00018ef0: 635f 6469 7370 5f7a 2929 0d0a 2020 2020  c_disp_z))..    
-00018f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f10: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-00018f20: 5f76 6172 5f64 6973 705f 7a2e 6170 7065  _var_disp_z.appe
-00018f30: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
-00018f40: 746f 7469 635f 6469 7370 5f7a 2929 0d0a  totic_disp_z))..
-00018f50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00018f60: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-00018f70: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
-00018f80: 5f79 2e61 7070 656e 6428 6e70 2e6d 6561  _y.append(np.mea
-00018f90: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
-00018fa0: 7370 5f79 2929 0d0a 2020 2020 2020 2020  sp_y))..        
-00018fb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00018fc0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
-00018fd0: 5f64 6973 705f 792e 6170 7065 6e64 286e  _disp_y.append(n
-00018fe0: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
-00018ff0: 635f 6469 7370 5f79 2929 0d0a 0d0a 2020  c_disp_y))....  
-00019000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019010: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
-00019020: 6963 5f6d 6561 6e5f 6469 7370 5f78 2e61  ic_mean_disp_x.a
-00019030: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-00019040: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
-00019050: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00019060: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00019070: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00019080: 705f 782e 6170 7065 6e64 286e 702e 7374  p_x.append(np.st
-00019090: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
-000190a0: 7370 5f78 2929 0d0a 0d0a 2020 2020 2020  sp_x))....      
-000190b0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-000190c0: 736b 203d 206e 6f6e 5f6d 6974 6f74 6963  sk = non_mitotic
-000190d0: 5f72 6164 6975 7320 3d3d 204e 6f6e 650d  _radius == None.
-000190e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000190f0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00019100: 746f 7469 635f 6d65 616e 5f72 6164 6975  totic_mean_radiu
-00019110: 732e 6170 7065 6e64 286e 702e 6d65 616e  s.append(np.mean
-00019120: 286e 6f6e 5f6d 6974 6f74 6963 5f72 6164  (non_mitotic_rad
-00019130: 6975 735b 7e6d 6173 6b5d 2929 0d0a 2020  ius[~mask]))..  
-00019140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019150: 2020 6669 6c74 6572 6564 5f76 616c 7565    filtered_value
-00019160: 7320 3d20 5b76 616c 2066 6f72 2076 616c  s = [val for val
-00019170: 2069 6e20 6e6f 6e5f 6d69 746f 7469 635f   in non_mitotic_
-00019180: 7261 6469 7573 2069 6620 7661 6c20 6973  radius if val is
-00019190: 206e 6f74 204e 6f6e 655d 0d0a 2020 2020   not None]..    
-000191a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191b0: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
-000191c0: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
-000191d0: 6e64 286e 702e 7374 6428 6669 6c74 6572  nd(np.std(filter
-000191e0: 6564 5f76 616c 7565 7329 290d 0a0d 0a20  ed_values)).... 
-000191f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019200: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00019210: 7469 635f 6d65 616e 5f73 7065 6564 2e61  tic_mean_speed.a
-00019220: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
-00019230: 6e5f 6d69 746f 7469 635f 7370 6565 6429  n_mitotic_speed)
-00019240: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00019250: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00019260: 6d69 746f 7469 635f 7661 725f 7370 6565  mitotic_var_spee
-00019270: 642e 6170 7065 6e64 286e 702e 7374 6428  d.append(np.std(
-00019280: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
-00019290: 6429 290d 0a0d 0a20 2020 2020 2020 2020  d))....         
-000192a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000192b0: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-000192c0: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
-000192d0: 6561 6e28 6e6f 6e5f 6d69 746f 7469 635f  ean(non_mitotic_
-000192e0: 6163 6329 290d 0a20 2020 2020 2020 2020  acc))..         
-000192f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019300: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00019310: 6163 632e 6170 7065 6e64 286e 702e 7374  acc.append(np.st
-00019320: 6428 6e6f 6e5f 6d69 746f 7469 635f 6163  d(non_mitotic_ac
-00019330: 6329 290d 0a0d 0a20 2020 2020 2020 2020  c))....         
-00019340: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019350: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
-00019360: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00019370: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
-00019380: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
-00019390: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-000193a0: 6529 290d 0a20 2020 2020 2020 2020 2020  e))..           
-000193b0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-000193c0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
-000193d0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-000193e0: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
-000193f0: 6f6e 5f6d 6974 6f74 6963 5f64 6972 6563  on_mitotic_direc
-00019400: 7469 6f6e 616c 5f63 6861 6e67 6529 2920  tional_change)) 
-00019410: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00019420: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00019430: 5f6d 6974 6f74 6963 5f6d 6561 6e5f 6469  _mitotic_mean_di
-00019440: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00019450: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00019460: 6e6f 6e5f 6d69 746f 7469 635f 6469 7374  non_mitotic_dist
-00019470: 616e 6365 5f63 656c 6c5f 6d61 736b 2929  ance_cell_mask))
-00019480: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019490: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
-000194a0: 6974 6f74 6963 5f76 6172 5f64 6973 7461  itotic_var_dista
-000194b0: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-000194c0: 7065 6e64 286e 702e 7374 6428 6e6f 6e5f  pend(np.std(non_
-000194d0: 6d69 746f 7469 635f 6469 7374 616e 6365  mitotic_distance
-000194e0: 5f63 656c 6c5f 6d61 736b 2929 0d0a 0d0a  _cell_mask))....
-000194f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019500: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
-00019510: 6561 6e5f 6469 7370 5f7a 2e61 7070 656e  ean_disp_z.appen
-00019520: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
-00019530: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
-00019540: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019550: 2e61 6c6c 5f76 6172 5f64 6973 705f 7a2e  .all_var_disp_z.
-00019560: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
-00019570: 6c5f 6469 7370 5f7a 2929 0d0a 0d0a 2020  l_disp_z))....  
-00019580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019590: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
-000195a0: 6469 7370 5f79 2e61 7070 656e 6428 6e70  disp_y.append(np
-000195b0: 2e6d 6561 6e28 616c 6c5f 6469 7370 5f79  .mean(all_disp_y
-000195c0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-000195d0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-000195e0: 5f76 6172 5f64 6973 705f 792e 6170 7065  _var_disp_y.appe
-000195f0: 6e64 286e 702e 7374 6428 616c 6c5f 6469  nd(np.std(all_di
-00019600: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
-00019610: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019620: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
-00019630: 5f78 2e61 7070 656e 6428 6e70 2e6d 6561  _x.append(np.mea
-00019640: 6e28 616c 6c5f 6469 7370 5f78 2929 0d0a  n(all_disp_x))..
-00019650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019660: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
-00019670: 5f64 6973 705f 782e 6170 7065 6e64 286e  _disp_x.append(n
-00019680: 702e 7374 6428 616c 6c5f 6469 7370 5f78  p.std(all_disp_x
-00019690: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
-000196a0: 2020 2020 2020 2020 2020 6d61 736b 203d            mask =
-000196b0: 2061 6c6c 5f72 6164 6975 7320 3d3d 204e   all_radius == N
-000196c0: 6f6e 650d 0a20 2020 2020 2020 2020 2020  one..           
-000196d0: 2020 2020 2020 2020 2073 656c 662e 616c           self.al
-000196e0: 6c5f 6d65 616e 5f72 6164 6975 732e 6170  l_mean_radius.ap
-000196f0: 7065 6e64 286e 702e 6d65 616e 2861 6c6c  pend(np.mean(all
-00019700: 5f72 6164 6975 735b 7e6d 6173 6b5d 2929  _radius[~mask]))
-00019710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019720: 2020 2020 2020 6669 6c74 6572 6564 5f76        filtered_v
-00019730: 616c 7565 7320 3d20 5b76 616c 2066 6f72  alues = [val for
-00019740: 2076 616c 2069 6e20 616c 6c5f 7261 6469   val in all_radi
-00019750: 7573 2069 6620 7661 6c20 6973 206e 6f74  us if val is not
-00019760: 204e 6f6e 655d 0d0a 2020 2020 2020 2020   None]..        
-00019770: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019780: 2e61 6c6c 5f76 6172 5f72 6164 6975 732e  .all_var_radius.
-00019790: 6170 7065 6e64 286e 702e 7374 6428 6669  append(np.std(fi
-000197a0: 6c74 6572 6564 5f76 616c 7565 7329 290d  ltered_values)).
-000197b0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
-000197c0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
-000197d0: 6d65 616e 5f73 7065 6564 2e61 7070 656e  mean_speed.appen
-000197e0: 6428 6e70 2e6d 6561 6e28 616c 6c5f 7370  d(np.mean(all_sp
-000197f0: 6565 6429 290d 0a20 2020 2020 2020 2020  eed))..         
-00019800: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019810: 616c 6c5f 7661 725f 7370 6565 642e 6170  all_var_speed.ap
-00019820: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
-00019830: 7370 6565 6429 290d 0a0d 0a20 2020 2020  speed))....     
-00019840: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019850: 656c 662e 616c 6c5f 6d65 616e 5f61 6363  elf.all_mean_acc
-00019860: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00019870: 616c 6c5f 6163 6329 290d 0a20 2020 2020  all_acc))..     
-00019880: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019890: 656c 662e 616c 6c5f 7661 725f 6163 632e  elf.all_var_acc.
-000198a0: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
-000198b0: 6c5f 6163 6329 290d 0a0d 0a0d 0a0d 0a20  l_acc))........ 
-000198c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000198d0: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
-000198e0: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-000198f0: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
-00019900: 616e 2861 6c6c 5f64 6972 6563 7469 6f6e  an(all_direction
-00019910: 616c 5f63 6861 6e67 6529 290d 0a20 2020  al_change))..   
-00019920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019930: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
-00019940: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
-00019950: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
-00019960: 6c6c 5f64 6972 6563 7469 6f6e 616c 5f63  ll_directional_c
-00019970: 6861 6e67 6529 290d 0a0d 0a20 2020 2020  hange))....     
-00019980: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019990: 656c 662e 616c 6c5f 6d65 616e 5f64 6973  elf.all_mean_dis
-000199a0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-000199b0: 6170 7065 6e64 286e 702e 6d65 616e 2861  append(np.mean(a
-000199c0: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
-000199d0: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
-000199e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000199f0: 662e 616c 6c5f 7661 725f 6469 7374 616e  f.all_var_distan
-00019a00: 6365 5f63 656c 6c5f 6d61 736b 2e61 7070  ce_cell_mask.app
-00019a10: 656e 6428 6e70 2e73 7464 2861 6c6c 5f64  end(np.std(all_d
-00019a20: 6973 7461 6e63 655f 6365 6c6c 5f6d 6173  istance_cell_mas
-00019a30: 6b29 290d 0a20 2020 2020 2020 2020 2020  k))..           
-00019a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a50: 200d 0a20 2020 2020 2020 200d 0a64 6566   ..        ..def
-00019a60: 2062 6f75 6e64 6172 795f 706f 696e 7473   boundary_points
-00019a70: 286d 6173 6b2c 2078 6361 6c69 6272 6174  (mask, xcalibrat
-00019a80: 696f 6e2c 2079 6361 6c69 6272 6174 696f  ion, ycalibratio
-00019a90: 6e2c 207a 6361 6c69 6272 6174 696f 6e29  n, zcalibration)
-00019aa0: 3a0d 0a0d 0a20 2020 206e 6469 6d20 3d20  :....    ndim = 
-00019ab0: 6c65 6e28 6d61 736b 2e73 6861 7065 290d  len(mask.shape).
-00019ac0: 0a20 2020 2074 696d 6564 5f6d 6173 6b20  .    timed_mask 
-00019ad0: 3d20 7b7d 0d0a 2020 2020 6d61 736b 203d  = {}..    mask =
-00019ae0: 206d 6173 6b20 3e20 300d 0a20 2020 206d   mask > 0..    m
-00019af0: 6173 6b20 3d20 6d61 736b 2e61 7374 7970  ask = mask.astyp
-00019b00: 6528 2775 696e 7438 2729 0d0a 2020 2020  e('uint8')..    
-00019b10: 2320 5958 2073 6861 7065 6420 6f62 6a65  # YX shaped obje
-00019b20: 6374 0d0a 2020 2020 6966 206e 6469 6d20  ct..    if ndim 
-00019b30: 3d3d 2032 3a0d 0a20 2020 2020 2020 200d  == 2:..        .
-00019b40: 0a20 2020 2020 2020 2062 6f75 6e64 6172  .        boundar
-00019b50: 7920 3d20 6669 6e64 5f62 6f75 6e64 6172  y = find_boundar
-00019b60: 6965 7328 6d61 736b 290d 0a20 2020 2020  ies(mask)..     
-00019b70: 2020 2072 6567 696f 6e63 656e 7472 6f69     regioncentroi
-00019b80: 6420 3d20 2830 2c29 202b 2063 6f6d 7075  d = (0,) + compu
-00019b90: 7465 5f63 656e 7472 6f69 6428 626f 756e  te_centroid(boun
-00019ba0: 6461 7279 2920 0d0a 2020 2020 2020 2020  dary) ..        
-00019bb0: 696e 6469 6365 7320 3d20 6e70 2e77 6865  indices = np.whe
-00019bc0: 7265 2862 6f75 6e64 6172 7920 3e20 3029  re(boundary > 0)
-00019bd0: 0d0a 2020 2020 2020 2020 7265 616c 5f69  ..        real_i
-00019be0: 6e64 6963 6573 203d 206e 702e 7472 616e  ndices = np.tran
-00019bf0: 7370 6f73 6528 6e70 2e61 7361 7272 6179  spose(np.asarray
-00019c00: 2869 6e64 6963 6573 2c20 6474 7970 653d  (indices, dtype=
-00019c10: 6e70 2e66 6c6f 6174 3332 2929 2e63 6f70  np.float32)).cop
-00019c20: 7928 290d 0a0d 0a20 2020 2020 2020 2066  y()....        f
-00019c30: 6f72 206a 2069 6e20 7261 6e67 6528 302c  or j in range(0,
-00019c40: 206c 656e 2872 6561 6c5f 696e 6469 6365   len(real_indice
-00019c50: 7329 293a 0d0a 0d0a 2020 2020 2020 2020  s)):....        
-00019c60: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
-00019c70: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
-00019c80: 6469 6365 735b 6a5d 5b30 5d20 2a20 7963  dices[j][0] * yc
-00019c90: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
-00019ca0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-00019cb0: 6963 6573 5b6a 5d5b 315d 203d 2072 6561  ices[j][1] = rea
-00019cc0: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
-00019cd0: 2a20 7863 616c 6962 7261 7469 6f6e 0d0a  * xcalibration..
-00019ce0: 0d0a 2020 2020 2020 2020 7472 6565 203d  ..        tree =
-00019cf0: 2073 7061 7469 616c 2e63 4b44 5472 6565   spatial.cKDTree
-00019d00: 2872 6561 6c5f 696e 6469 6365 7329 0d0a  (real_indices)..
-00019d10: 2020 2020 2020 2020 2320 5468 6973 206f          # This o
-00019d20: 626a 6563 7420 636f 6e74 6169 6e73 206c  bject contains l
-00019d30: 6973 7420 6f66 2061 6c6c 2074 6865 2070  ist of all the p
-00019d40: 6f69 6e74 7320 666f 7220 616c 6c20 7468  oints for all th
-00019d50: 6520 6c61 6265 6c73 2069 6e20 7468 6520  e labels in the 
-00019d60: 4d61 736b 2069 6d61 6765 2077 6974 6820  Mask image with 
-00019d70: 7468 6520 6c61 6265 6c20 6964 2061 6e64  the label id and
-00019d80: 2076 6f6c 756d 6520 6f66 2065 6163 6820   volume of each 
-00019d90: 6c61 6265 6c0d 0a20 2020 2020 2020 2074  label..        t
-00019da0: 696d 6564 5f6d 6173 6b5b 7374 7228 3029  imed_mask[str(0)
-00019db0: 5d20 3d20 5b74 7265 652c 2069 6e64 6963  ] = [tree, indic
-00019dc0: 6573 2c20 7265 6769 6f6e 6365 6e74 726f  es, regioncentro
-00019dd0: 6964 5d0d 0a0d 0a20 2020 2023 2054 5958  id]....    # TYX
-00019de0: 2073 6861 7065 6420 6f62 6a65 6374 0d0a   shaped object..
-00019df0: 2020 2020 6966 206e 6469 6d20 3d3d 2033      if ndim == 3
-00019e00: 3a0d 0a0d 0a0d 0a20 2020 2020 2020 2066  :......        f
-00019e10: 6f72 2069 2069 6e20 7471 646d 2872 616e  or i in tqdm(ran
-00019e20: 6765 2830 2c20 6d61 736b 2e73 6861 7065  ge(0, mask.shape
-00019e30: 5b30 5d29 293a 0d0a 2020 2020 2020 2020  [0])):..        
-00019e40: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00019e50: 2020 2020 2020 2020 2020 626f 756e 6461            bounda
-00019e60: 7279 203d 2066 696e 645f 626f 756e 6461  ry = find_bounda
-00019e70: 7269 6573 286d 6173 6b5b 692c 3a5d 290d  ries(mask[i,:]).
-00019e80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019e90: 2072 6567 696f 6e63 656e 7472 6f69 6420   regioncentroid 
-00019ea0: 3d20 2830 2c29 202b 2063 6f6d 7075 7465  = (0,) + compute
-00019eb0: 5f63 656e 7472 6f69 6428 626f 756e 6461  _centroid(bounda
-00019ec0: 7279 2920 0d0a 2020 2020 2020 2020 2020  ry) ..          
-00019ed0: 2020 2020 2020 696e 6469 6365 7320 3d20        indices = 
-00019ee0: 6e70 2e77 6865 7265 2862 6f75 6e64 6172  np.where(boundar
-00019ef0: 7920 3e20 3029 0d0a 2020 2020 2020 2020  y > 0)..        
-00019f00: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-00019f10: 6963 6573 203d 206e 702e 7472 616e 7370  ices = np.transp
-00019f20: 6f73 6528 6e70 2e61 7361 7272 6179 2869  ose(np.asarray(i
-00019f30: 6e64 6963 6573 2c20 6474 7970 653d 6e70  ndices, dtype=np
-00019f40: 2e66 6c6f 6174 3332 2929 2e63 6f70 7928  .float32)).copy(
-00019f50: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00019f60: 2020 2020 2066 6f72 206a 2069 6e20 7261       for j in ra
-00019f70: 6e67 6528 302c 206c 656e 2872 6561 6c5f  nge(0, len(real_
-00019f80: 696e 6469 6365 7329 293a 0d0a 0d0a 2020  indices)):....  
-00019f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019fa0: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
-00019fb0: 5d5b 305d 203d 2072 6561 6c5f 696e 6469  ][0] = real_indi
-00019fc0: 6365 735b 6a5d 5b30 5d20 2a20 7963 616c  ces[j][0] * ycal
-00019fd0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-00019fe0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00019ff0: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
-0001a000: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
-0001a010: 6a5d 5b31 5d20 2a20 7863 616c 6962 7261  j][1] * xcalibra
-0001a020: 7469 6f6e 0d0a 0d0a 2020 2020 2020 2020  tion....        
-0001a030: 2020 2020 2020 2020 7472 6565 203d 2073          tree = s
-0001a040: 7061 7469 616c 2e63 4b44 5472 6565 2872  patial.cKDTree(r
-0001a050: 6561 6c5f 696e 6469 6365 7329 0d0a 0d0a  eal_indices)....
-0001a060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a070: 7469 6d65 645f 6d61 736b 5b73 7472 2869  timed_mask[str(i
-0001a080: 295d 203d 205b 7472 6565 2c20 696e 6469  )] = [tree, indi
-0001a090: 6365 732c 2072 6567 696f 6e63 656e 7472  ces, regioncentr
-0001a0a0: 6f69 645d 0d0a 2020 2020 2020 2020 2020  oid]..          
-0001a0b0: 2020 0d0a 2020 2020 2320 545a 5958 2073    ..    # TZYX s
-0001a0c0: 6861 7065 6420 6f62 6a65 6374 0d0a 2020  haped object..  
-0001a0d0: 2020 6966 206e 6469 6d20 3d3d 2034 3a0d    if ndim == 4:.
-0001a0e0: 0a20 2020 2020 2020 2070 7269 6e74 2827  .        print('
-0001a0f0: 4d61 6b69 6e67 206d 6173 6b20 696e 2034  Making mask in 4
-0001a100: 4427 290d 0a20 2020 2020 2020 2062 6f75  D')..        bou
-0001a110: 6e64 6172 7920 3d20 6e70 2e7a 6572 6f73  ndary = np.zeros
-0001a120: 280d 0a20 2020 2020 2020 2020 2020 205b  (..            [
-0001a130: 6d61 736b 2e73 6861 7065 5b30 5d2c 206d  mask.shape[0], m
-0001a140: 6173 6b2e 7368 6170 655b 315d 2c20 6d61  ask.shape[1], ma
-0001a150: 736b 2e73 6861 7065 5b32 5d2c 206d 6173  sk.shape[2], mas
-0001a160: 6b2e 7368 6170 655b 335d 5d2c 2064 7479  k.shape[3]], dty
-0001a170: 7065 3d6e 702e 7569 6e74 380d 0a20 2020  pe=np.uint8..   
-0001a180: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0001a190: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
-0001a1a0: 2c20 6d61 736b 2e73 6861 7065 5b30 5d29  , mask.shape[0])
-0001a1b0: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
-0001a1c0: 0a20 2020 2020 2020 2020 2020 2062 6f75  .            bou
-0001a1d0: 6e64 6172 795b 692c 3a5d 203d 2066 696e  ndary[i,:] = fin
-0001a1e0: 645f 626f 756e 6461 7269 6573 286d 6173  d_boundaries(mas
-0001a1f0: 6b5b 692c 3a5d 290d 0a20 2020 2020 2020  k[i,:])..       
-0001a200: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
-0001a210: 6f69 6420 3d20 636f 6d70 7574 655f 6365  oid = compute_ce
-0001a220: 6e74 726f 6964 2862 6f75 6e64 6172 795b  ntroid(boundary[
-0001a230: 692c 3a5d 2920 0d0a 2020 2020 2020 2020  i,:]) ..        
-0001a240: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
-0001a250: 2e77 6865 7265 2862 6f75 6e64 6172 795b  .where(boundary[
-0001a260: 692c 3a5d 203e 2030 290d 0a20 2020 2020  i,:] > 0)..     
-0001a270: 2020 2020 2020 2072 6561 6c5f 696e 6469         real_indi
-0001a280: 6365 7320 3d20 6e70 2e74 7261 6e73 706f  ces = np.transpo
-0001a290: 7365 286e 702e 6173 6172 7261 7928 696e  se(np.asarray(in
-0001a2a0: 6469 6365 732c 2064 7479 7065 3d6e 702e  dices, dtype=np.
-0001a2b0: 666c 6f61 7433 3229 292e 636f 7079 2829  float32)).copy()
-0001a2c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001a2d0: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
-0001a2e0: 2c20 6c65 6e28 7265 616c 5f69 6e64 6963  , len(real_indic
-0001a2f0: 6573 2929 3a0d 0a0d 0a20 2020 2020 2020  es)):....       
-0001a300: 2020 2020 2020 2020 2020 2020 2072 6561               rea
-0001a310: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
-0001a320: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
-0001a330: 5d5b 305d 202a 207a 6361 6c69 6272 6174  ][0] * zcalibrat
-0001a340: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
-0001a350: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-0001a360: 6469 6365 735b 6a5d 5b31 5d20 3d20 7265  dices[j][1] = re
-0001a370: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
-0001a380: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
-0001a390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a3a0: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-0001a3b0: 735b 6a5d 5b32 5d20 3d20 7265 616c 5f69  s[j][2] = real_i
-0001a3c0: 6e64 6963 6573 5b6a 5d5b 325d 202a 2078  ndices[j][2] * x
-0001a3d0: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
-0001a3e0: 2020 2020 2020 2020 2020 2074 7265 6520             tree 
-0001a3f0: 3d20 7370 6174 6961 6c2e 634b 4454 7265  = spatial.cKDTre
-0001a400: 6528 7265 616c 5f69 6e64 6963 6573 290d  e(real_indices).
-0001a410: 0a20 2020 2020 2020 2020 2020 2074 696d  .            tim
-0001a420: 6564 5f6d 6173 6b5b 7374 7228 6929 5d20  ed_mask[str(i)] 
-0001a430: 3d20 5b74 7265 652c 2069 6e64 6963 6573  = [tree, indices
-0001a440: 2c20 7265 6769 6f6e 6365 6e74 726f 6964  , regioncentroid
-0001a450: 5d0d 0a20 2020 2070 7269 6e74 2827 436f  ]..    print('Co
-0001a460: 6d70 7574 6564 2074 6865 2062 6f75 6e64  mputed the bound
-0001a470: 6172 7920 706f 696e 7473 2729 0d0a 0d0a  ary points')....
-0001a480: 2020 2020 7265 7475 726e 2074 696d 6564      return timed
-0001a490: 5f6d 6173 6b2c 2062 6f75 6e64 6172 7920  _mask, boundary 
-0001a4a0: 2020 2020 2020 200d 0a0d 0a64 6566 2063         ....def c
-0001a4b0: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
-0001a4c0: 6269 6e61 7279 5f69 6d61 6765 293a 0d0a  binary_image):..
-0001a4d0: 2020 2020 2320 456e 7375 7265 2062 696e      # Ensure bin
-0001a4e0: 6172 7920 696d 6167 6520 6973 2061 204e  ary image is a N
-0001a4f0: 756d 5079 2061 7272 6179 0d0a 2020 2020  umPy array..    
-0001a500: 6269 6e61 7279 5f69 6d61 6765 203d 206e  binary_image = n
-0001a510: 702e 6172 7261 7928 6269 6e61 7279 5f69  p.array(binary_i
-0001a520: 6d61 6765 290d 0a0d 0a20 2020 2077 6869  mage)....    whi
-0001a530: 7465 5f70 6978 656c 7320 3d20 6e70 2e77  te_pixels = np.w
-0001a540: 6865 7265 2862 696e 6172 795f 696d 6167  here(binary_imag
-0001a550: 6520 3d3d 2031 290d 0a20 2020 206e 756d  e == 1)..    num
-0001a560: 5f70 6978 656c 7320 3d20 6c65 6e28 7768  _pixels = len(wh
-0001a570: 6974 655f 7069 7865 6c73 5b30 5d29 0d0a  ite_pixels[0])..
-0001a580: 0d0a 2020 2020 2320 436f 6d70 7574 6520  ..    # Compute 
-0001a590: 7468 6520 6365 6e74 726f 6964 206f 6620  the centroid of 
-0001a5a0: 7468 6520 7768 6974 6520 7069 7865 6c73  the white pixels
-0001a5b0: 2069 6e20 7468 6520 626f 756e 6461 7279   in the boundary
-0001a5c0: 2069 6d61 6765 0d0a 2020 2020 6365 6e74   image..    cent
-0001a5d0: 726f 6964 203d 206e 702e 7a65 726f 7328  roid = np.zeros(
-0001a5e0: 6269 6e61 7279 5f69 6d61 6765 2e6e 6469  binary_image.ndi
-0001a5f0: 6d29 0d0a 2020 2020 666f 7220 6469 6d20  m)..    for dim 
-0001a600: 696e 2072 616e 6765 2862 696e 6172 795f  in range(binary_
-0001a610: 696d 6167 652e 6e64 696d 293a 0d0a 2020  image.ndim):..  
-0001a620: 2020 2020 2020 6365 6e74 726f 6964 5b64        centroid[d
-0001a630: 696d 5d20 3d20 7768 6974 655f 7069 7865  im] = white_pixe
-0001a640: 6c73 5b64 696d 5d2e 7375 6d28 2920 2f20  ls[dim].sum() / 
-0001a650: 6e75 6d5f 7069 7865 6c73 0d0a 0d0a 2020  num_pixels....  
-0001a660: 2020 7265 7475 726e 2063 656e 7472 6f69    return centroi
-0001a670: 640d 0a0d 0a0d 0a0d 0a20 0d0a 0d0a 6465  d........ ....de
-0001a680: 6620 6765 745f 6373 765f 6461 7461 2863  f get_csv_data(c
-0001a690: 7376 293a 0d0a 0d0a 2020 2020 2020 2020  sv):....        
-0001a6a0: 6461 7461 7365 7420 3d20 7064 2e72 6561  dataset = pd.rea
-0001a6b0: 645f 6373 7628 0d0a 2020 2020 2020 2020  d_csv(..        
-0001a6c0: 2020 2020 6373 762c 2064 656c 696d 6974      csv, delimit
-0001a6d0: 6572 3d22 2c22 2c20 656e 636f 6469 6e67  er=",", encoding
-0001a6e0: 3d22 756e 6963 6f64 655f 6573 6361 7065  ="unicode_escape
-0001a6f0: 222c 206c 6f77 5f6d 656d 6f72 793d 4661  ", low_memory=Fa
-0001a700: 6c73 650d 0a20 2020 2020 2020 2029 5b33  lse..        )[3
-0001a710: 3a5d 0d0a 2020 2020 2020 2020 6461 7461  :]..        data
-0001a720: 7365 745f 696e 6465 7820 3d20 6461 7461  set_index = data
-0001a730: 7365 742e 696e 6465 780d 0a20 2020 2020  set.index..     
-0001a740: 2020 2072 6574 7572 6e20 6461 7461 7365     return datase
-0001a750: 742c 2064 6174 6173 6574 5f69 6e64 6578  t, dataset_index
-0001a760: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
-0001a770: 7370 6f74 5f64 6174 6173 6574 2873 706f  spot_dataset(spo
-0001a780: 745f 6461 7461 7365 742c 2074 7261 636b  t_dataset, track
-0001a790: 5f61 6e61 6c79 7369 735f 7370 6f74 5f6b  _analysis_spot_k
-0001a7a0: 6579 732c 2078 6361 6c69 6272 6174 696f  eys, xcalibratio
-0001a7b0: 6e2c 2079 6361 6c69 6272 6174 696f 6e2c  n, ycalibration,
-0001a7c0: 207a 6361 6c69 6272 6174 696f 6e2c 2041   zcalibration, A
-0001a7d0: 7474 7269 6275 7465 426f 786e 616d 652c  ttributeBoxname,
-0001a7e0: 2064 6574 6563 7469 6f6e 6368 616e 6e65   detectionchanne
-0001a7f0: 6c29 3a0d 0a20 2020 2020 2020 2041 6c6c  l):..        All
-0001a800: 5661 6c75 6573 203d 207b 7d0d 0a20 2020  Values = {}..   
-0001a810: 2020 2020 2070 6f73 6978 203d 2074 7261       posix = tra
-0001a820: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001a830: 5f6b 6579 735b 2270 6f73 6978 225d 0d0a  _keys["posix"]..
-0001a840: 2020 2020 2020 2020 706f 7369 7920 3d20          posiy = 
-0001a850: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001a860: 706f 745f 6b65 7973 5b22 706f 7369 7922  pot_keys["posiy"
-0001a870: 5d0d 0a20 2020 2020 2020 2070 6f73 697a  ]..        posiz
-0001a880: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
-0001a890: 735f 7370 6f74 5f6b 6579 735b 2270 6f73  s_spot_keys["pos
-0001a8a0: 697a 225d 0d0a 2020 2020 2020 2020 6672  iz"]..        fr
-0001a8b0: 616d 6520 3d20 7472 6163 6b5f 616e 616c  ame = track_anal
-0001a8c0: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-0001a8d0: 6672 616d 6522 5d0d 0a20 2020 2020 2020  frame"]..       
-0001a8e0: 200d 0a20 2020 2020 2020 204c 6f63 6174   ..        Locat
-0001a8f0: 696f 6e58 203d 2028 0d0a 2020 2020 2020  ionX = (..      
-0001a900: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
-0001a910: 6574 5b70 6f73 6978 5d2e 6173 7479 7065  et[posix].astype
-0001a920: 2822 666c 6f61 7422 2920 2f20 7863 616c  ("float") / xcal
-0001a930: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-0001a940: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
-0001a950: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
-0001a960: 696f 6e59 203d 2028 0d0a 2020 2020 2020  ionY = (..      
-0001a970: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
-0001a980: 6574 5b70 6f73 6979 5d2e 6173 7479 7065  et[posiy].astype
-0001a990: 2822 666c 6f61 7422 2920 2f20 7963 616c  ("float") / ycal
-0001a9a0: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-0001a9b0: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
-0001a9c0: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
-0001a9d0: 696f 6e5a 203d 2028 0d0a 2020 2020 2020  ionZ = (..      
-0001a9e0: 2020 2020 2020 7370 6f74 5f64 6174 6173        spot_datas
-0001a9f0: 6574 5b70 6f73 697a 5d2e 6173 7479 7065  et[posiz].astype
-0001aa00: 2822 666c 6f61 7422 2920 2f20 7a63 616c  ("float") / zcal
-0001aa10: 6962 7261 7469 6f6e 0d0a 2020 2020 2020  ibration..      
-0001aa20: 2020 292e 6173 7479 7065 2822 696e 7422    ).astype("int"
-0001aa30: 290d 0a20 2020 2020 2020 204c 6f63 6174  )..        Locat
-0001aa40: 696f 6e54 203d 2028 7370 6f74 5f64 6174  ionT = (spot_dat
-0001aa50: 6173 6574 5b66 7261 6d65 5d2e 6173 7479  aset[frame].asty
-0001aa60: 7065 2822 666c 6f61 7422 2929 2e61 7374  pe("float")).ast
-0001aa70: 7970 6528 2269 6e74 2229 0d0a 2020 2020  ype("int")..    
-0001aa80: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
-0001aa90: 6967 6e6f 7265 5f76 616c 7565 7320 3d20  ignore_values = 
-0001aaa0: 5b74 7261 636b 5f61 6e61 6c79 7369 735f  [track_analysis_
-0001aab0: 7370 6f74 5f6b 6579 735b 226d 6561 6e5f  spot_keys["mean_
-0001aac0: 696e 7465 6e73 6974 7922 5d2c 7472 6163  intensity"],trac
-0001aad0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001aae0: 6b65 7973 5b22 746f 7461 6c5f 696e 7465  keys["total_inte
-0001aaf0: 6e73 6974 7922 5d5d 0d0a 2020 2020 2020  nsity"]]..      
-0001ab00: 2020 666f 7220 286b 2c76 2920 696e 2074    for (k,v) in t
-0001ab10: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
-0001ab20: 6f74 5f6b 6579 732e 6974 656d 7328 293a  ot_keys.items():
-0001ab30: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001ab40: 2020 2020 6966 2064 6574 6563 7469 6f6e      if detection
-0001ab50: 6368 616e 6e65 6c20 3d3d 2031 3a0d 0a20  channel == 1:.. 
-0001ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab70: 2020 2020 6966 206b 203d 3d20 226d 6561      if k == "mea
-0001ab80: 6e5f 696e 7465 6e73 6974 795f 6368 3222  n_intensity_ch2"
-0001ab90: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001aba0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-0001abb0: 6c75 6520 3d20 7472 6163 6b5f 616e 616c  lue = track_anal
-0001abc0: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
-0001abd0: 6d65 616e 5f69 6e74 656e 7369 7479 225d  mean_intensity"]
-0001abe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001abf0: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
-0001ac00: 5661 6c75 6573 5b76 616c 7565 5d20 3d20  Values[value] = 
-0001ac10: 7370 6f74 5f64 6174 6173 6574 5b76 5d2e  spot_dataset[v].
-0001ac20: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
-0001ac30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ac40: 2020 2020 2020 6966 206b 203d 3d20 2274        if k == "t
-0001ac50: 6f74 616c 5f69 6e74 656e 7369 7479 5f63  otal_intensity_c
-0001ac60: 6832 223a 0d0a 2020 2020 2020 2020 2020  h2":..          
-0001ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac80: 2076 616c 7565 203d 2074 7261 636b 5f61   value = track_a
-0001ac90: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-0001aca0: 735b 2274 6f74 616c 5f69 6e74 656e 7369  s["total_intensi
-0001acb0: 7479 225d 0d0a 2020 2020 2020 2020 2020  ty"]..          
-0001acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001acd0: 2041 6c6c 5661 6c75 6573 5b76 616c 7565   AllValues[value
-0001ace0: 5d20 3d20 7370 6f74 5f64 6174 6173 6574  ] = spot_dataset
-0001acf0: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
-0001ad00: 7422 2920 2020 2020 2020 0d0a 0d0a 2020  t")       ....  
-0001ad10: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001ad20: 2076 206e 6f74 2069 6e20 6967 6e6f 7265   v not in ignore
-0001ad30: 5f76 616c 7565 733a 0d0a 2020 2020 2020  _values:..      
-0001ad40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad50: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0001ad60: 2020 2020 2020 2020 2020 416c 6c56 616c            AllVal
-0001ad70: 7565 735b 765d 203d 2073 706f 745f 6461  ues[v] = spot_da
-0001ad80: 7461 7365 745b 765d 2e61 7374 7970 6528  taset[v].astype(
-0001ad90: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
-0001ada0: 2020 2020 2020 2020 2020 2020 200d 0a0d               ...
-0001adb0: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
-0001adc0: 6573 5b70 6f73 6978 5d20 3d20 726f 756e  es[posix] = roun
-0001add0: 6428 4c6f 6361 7469 6f6e 582c 3329 0d0a  d(LocationX,3)..
-0001ade0: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
-0001adf0: 735b 706f 7369 795d 203d 2072 6f75 6e64  s[posiy] = round
-0001ae00: 284c 6f63 6174 696f 6e59 2c33 290d 0a20  (LocationY,3).. 
-0001ae10: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
-0001ae20: 5b70 6f73 697a 5d20 3d20 726f 756e 6428  [posiz] = round(
-0001ae30: 4c6f 6361 7469 6f6e 5a2c 3329 0d0a 2020  LocationZ,3)..  
-0001ae40: 2020 2020 2020 416c 6c56 616c 7565 735b        AllValues[
-0001ae50: 6672 616d 655d 203d 2072 6f75 6e64 284c  frame] = round(L
-0001ae60: 6f63 6174 696f 6e54 2c33 290d 0a20 2020  ocationT,3)..   
-0001ae70: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
-0001ae80: 7320 3d20 5b5d 0d0a 2020 2020 2020 2020  s = []..        
-0001ae90: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
-0001aea0: 656e 6428 4174 7472 6962 7574 6542 6f78  end(AttributeBox
-0001aeb0: 6e61 6d65 290d 0a20 2020 2020 2020 2066  name)..        f
-0001aec0: 6f72 2061 7474 7269 6275 7465 6e61 6d65  or attributename
-0001aed0: 2069 6e20 416c 6c56 616c 7565 732e 6b65   in AllValues.ke
-0001aee0: 7973 2829 3a0d 0a20 2020 2020 2020 2020  ys():..         
-0001aef0: 2020 2020 2041 7474 7269 6275 7465 6964       Attributeid
-0001af00: 732e 6170 7065 6e64 2861 7474 7269 6275  s.append(attribu
-0001af10: 7465 6e61 6d65 2920 2020 200d 0a20 2020  tename)    ..   
-0001af20: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0001af30: 2020 200d 0a20 2020 2020 2020 2072 6574     ..        ret
-0001af40: 7572 6e20 4174 7472 6962 7574 6569 6473  urn Attributeids
-0001af50: 2c20 416c 6c56 616c 7565 7320 2020 2020  , AllValues     
-0001af60: 0d0a 2020 2020 0d0a 6465 6620 6765 745f  ..    ..def get_
-0001af70: 7472 6163 6b5f 6461 7461 7365 7428 7472  track_dataset(tr
-0001af80: 6163 6b5f 6461 7461 7365 742c 2074 7261  ack_dataset, tra
-0001af90: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001afa0: 5f6b 6579 732c 2074 7261 636b 5f61 6e61  _keys, track_ana
-0001afb0: 6c79 7369 735f 7472 6163 6b5f 6b65 7973  lysis_track_keys
-0001afc0: 2c20 5472 6163 6b41 7474 7269 6275 7465  , TrackAttribute
-0001afd0: 426f 786e 616d 6529 3a0d 0a0d 0a20 2020  Boxname):....   
-0001afe0: 2020 2020 2041 6c6c 5472 6163 6b56 616c       AllTrackVal
-0001aff0: 7565 7320 3d20 7b7d 0d0a 2020 2020 2020  ues = {}..      
-0001b000: 2020 7472 6163 6b5f 6964 203d 2074 7261    track_id = tra
-0001b010: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001b020: 5f6b 6579 735b 2274 7261 636b 5f69 6422  _keys["track_id"
-0001b030: 5d0d 0a20 2020 2020 2020 2054 6964 203d  ]..        Tid =
-0001b040: 2074 7261 636b 5f64 6174 6173 6574 5b74   track_dataset[t
-0001b050: 7261 636b 5f69 645d 2e61 7374 7970 6528  rack_id].astype(
-0001b060: 2266 6c6f 6174 2229 0d0a 2020 2020 2020  "float")..      
-0001b070: 200d 0a20 2020 2020 2020 2041 6c6c 5472   ..        AllTr
-0001b080: 6163 6b56 616c 7565 735b 7472 6163 6b5f  ackValues[track_
-0001b090: 6964 5d20 3d20 5469 640d 0a20 2020 2020  id] = Tid..     
-0001b0a0: 200d 0a20 2020 2020 2020 2066 6f72 2028   ..        for (
-0001b0b0: 6b2c 2076 2920 696e 2074 7261 636b 5f61  k, v) in track_a
-0001b0c0: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
-0001b0d0: 7973 2e69 7465 6d73 2829 3a0d 0a0d 0a20  ys.items():.... 
-0001b0e0: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-0001b0f0: 203d 2074 7261 636b 5f64 6174 6173 6574   = track_dataset
-0001b100: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
-0001b110: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
-0001b120: 2020 2020 206d 696e 7661 6c20 3d20 6d69       minval = mi
-0001b130: 6e28 7829 0d0a 2020 2020 2020 2020 2020  n(x)..          
-0001b140: 2020 2020 2020 6d61 7876 616c 203d 206d        maxval = m
-0001b150: 6178 2878 290d 0a0d 0a20 2020 2020 2020  ax(x)....       
-0001b160: 2020 2020 2020 2020 2069 6620 6d69 6e76           if minv
-0001b170: 616c 203e 2030 2061 6e64 206d 6178 7661  al > 0 and maxva
-0001b180: 6c20 3c3d 2031 3a0d 0a0d 0a20 2020 2020  l <= 1:....     
-0001b190: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-0001b1a0: 203d 2078 202b 2031 0d0a 0d0a 2020 2020   = x + 1....    
-0001b1b0: 2020 2020 2020 2020 2020 2020 416c 6c54              AllT
-0001b1c0: 7261 636b 5661 6c75 6573 5b6b 5d20 3d20  rackValues[k] = 
-0001b1d0: 726f 756e 6428 782c 2033 290d 0a0d 0a20  round(x, 3).... 
-0001b1e0: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
-0001b1f0: 6962 7574 6569 6473 203d 205b 5d0d 0a20  ibuteids = [].. 
-0001b200: 2020 2020 2020 2054 7261 636b 4174 7472         TrackAttr
-0001b210: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
-0001b220: 5472 6163 6b41 7474 7269 6275 7465 426f  TrackAttributeBo
-0001b230: 786e 616d 6529 0d0a 2020 2020 2020 2020  xname)..        
-0001b240: 666f 7220 6174 7472 6962 7574 656e 616d  for attributenam
-0001b250: 6520 696e 2074 7261 636b 5f61 6e61 6c79  e in track_analy
-0001b260: 7369 735f 7472 6163 6b5f 6b65 7973 2e6b  sis_track_keys.k
-0001b270: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-0001b280: 2020 2020 5472 6163 6b41 7474 7269 6275      TrackAttribu
-0001b290: 7465 6964 732e 6170 7065 6e64 2861 7474  teids.append(att
-0001b2a0: 7269 6275 7465 6e61 6d65 2920 2020 200d  ributename)    .
-0001b2b0: 0a20 2020 200d 0a20 2020 2020 2020 2072  .    ..        r
-0001b2c0: 6574 7572 6e20 5472 6163 6b41 7474 7269  eturn TrackAttri
-0001b2d0: 6275 7465 6964 732c 2041 6c6c 5472 6163  buteids, AllTrac
-0001b2e0: 6b56 616c 7565 730d 0a20 2020 200d 0a64  kValues..    ..d
-0001b2f0: 6566 2067 6574 5f65 6467 6573 5f64 6174  ef get_edges_dat
-0001b300: 6173 6574 2865 6467 6573 5f64 6174 6173  aset(edges_datas
-0001b310: 6574 2c20 6564 6765 735f 6461 7461 7365  et, edges_datase
-0001b320: 745f 696e 6465 782c 2074 7261 636b 5f61  t_index, track_a
+00018ab0: 2020 2020 2066 696c 7465 7265 645f 7661       filtered_va
+00018ac0: 6c75 6573 203d 205b 7661 6c20 666f 7220  lues = [val for 
+00018ad0: 7661 6c20 696e 206d 6974 6f74 6963 5f72  val in mitotic_r
+00018ae0: 6164 6975 7320 6966 2076 616c 2069 7320  adius if val is 
+00018af0: 6e6f 7420 4e6f 6e65 5d0d 0a20 2020 2020  not None]..     
+00018b00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018b10: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00018b20: 5f72 6164 6975 732e 6170 7065 6e64 286e  _radius.append(n
+00018b30: 702e 6d65 616e 2866 696c 7465 7265 645f  p.mean(filtered_
+00018b40: 7661 6c75 6573 2929 0d0a 2020 2020 2020  values))..      
+00018b50: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00018b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b70: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018b80: 5f76 6172 5f72 6164 6975 732e 6170 7065  _var_radius.appe
+00018b90: 6e64 286e 702e 7374 6428 6669 6c74 6572  nd(np.std(filter
+00018ba0: 6564 5f76 616c 7565 7329 290d 0a20 2020  ed_values))..   
+00018bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bc0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00018bd0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00018be0: 7469 635f 6d65 616e 5f73 7065 6564 2e61  tic_mean_speed.a
+00018bf0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
+00018c00: 746f 7469 635f 7370 6565 6429 290d 0a20  totic_speed)).. 
+00018c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c20: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
+00018c30: 7661 725f 7370 6565 642e 6170 7065 6e64  var_speed.append
+00018c40: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
+00018c50: 7370 6565 6429 290d 0a0d 0a20 2020 2020  speed))....     
+00018c60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018c70: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00018c80: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
+00018c90: 6561 6e28 6d69 746f 7469 635f 6163 6329  ean(mitotic_acc)
+00018ca0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00018cb0: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
+00018cc0: 7469 635f 7661 725f 6163 632e 6170 7065  tic_var_acc.appe
+00018cd0: 6e64 286e 702e 7374 6428 6d69 746f 7469  nd(np.std(mitoti
+00018ce0: 635f 6163 6329 290d 0a0d 0a20 2020 2020  c_acc))....     
+00018cf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018d00: 656c 662e 6d69 746f 7469 635f 6d65 616e  elf.mitotic_mean
+00018d10: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00018d20: 6e67 652e 6170 7065 6e64 286e 702e 6d65  nge.append(np.me
+00018d30: 616e 286d 6974 6f74 6963 5f64 6972 6563  an(mitotic_direc
+00018d40: 7469 6f6e 616c 5f63 6861 6e67 6529 290d  tional_change)).
+00018d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018d60: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
+00018d70: 635f 7661 725f 6469 7265 6374 696f 6e61  c_var_directiona
+00018d80: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+00018d90: 6e70 2e73 7464 286d 6974 6f74 6963 5f64  np.std(mitotic_d
+00018da0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
+00018db0: 6529 290d 0a0d 0a20 2020 2020 2020 2020  e))....         
+00018dc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00018dd0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00018de0: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00018df0: 6170 7065 6e64 286e 702e 6d65 616e 286d  append(np.mean(m
+00018e00: 6974 6f74 6963 5f64 6973 7461 6e63 655f  itotic_distance_
+00018e10: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
+00018e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e30: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
+00018e40: 725f 6469 7374 616e 6365 5f63 656c 6c5f  r_distance_cell_
+00018e50: 6d61 736b 2e61 7070 656e 6428 6e70 2e73  mask.append(np.s
+00018e60: 7464 286d 6974 6f74 6963 5f64 6973 7461  td(mitotic_dista
+00018e70: 6e63 655f 6365 6c6c 5f6d 6173 6b29 290d  nce_cell_mask)).
+00018e80: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+00018e90: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
+00018ea0: 6d69 746f 7469 635f 6d65 616e 5f64 6973  mitotic_mean_dis
+00018eb0: 705f 7a2e 6170 7065 6e64 286e 702e 6d65  p_z.append(np.me
+00018ec0: 616e 286e 6f6e 5f6d 6974 6f74 6963 5f64  an(non_mitotic_d
+00018ed0: 6973 705f 7a29 290d 0a20 2020 2020 2020  isp_z))..       
+00018ee0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018ef0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+00018f00: 725f 6469 7370 5f7a 2e61 7070 656e 6428  r_disp_z.append(
+00018f10: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
+00018f20: 6963 5f64 6973 705f 7a29 290d 0a0d 0a20  ic_disp_z)).... 
+00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f40: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00018f50: 7469 635f 6d65 616e 5f64 6973 705f 792e  tic_mean_disp_y.
+00018f60: 6170 7065 6e64 286e 702e 6d65 616e 286e  append(np.mean(n
+00018f70: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00018f80: 7929 290d 0a20 2020 2020 2020 2020 2020  y))..           
+00018f90: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00018fa0: 6e5f 6d69 746f 7469 635f 7661 725f 6469  n_mitotic_var_di
+00018fb0: 7370 5f79 2e61 7070 656e 6428 6e70 2e73  sp_y.append(np.s
+00018fc0: 7464 286e 6f6e 5f6d 6974 6f74 6963 5f64  td(non_mitotic_d
+00018fd0: 6973 705f 7929 290d 0a0d 0a20 2020 2020  isp_y))....     
+00018fe0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018ff0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+00019000: 6d65 616e 5f64 6973 705f 782e 6170 7065  mean_disp_x.appe
+00019010: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
+00019020: 6974 6f74 6963 5f64 6973 705f 7829 290d  itotic_disp_x)).
+00019030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019040: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+00019050: 746f 7469 635f 7661 725f 6469 7370 5f78  totic_var_disp_x
+00019060: 2e61 7070 656e 6428 6e70 2e73 7464 286e  .append(np.std(n
+00019070: 6f6e 5f6d 6974 6f74 6963 5f64 6973 705f  on_mitotic_disp_
+00019080: 7829 290d 0a0d 0a20 2020 2020 2020 2020  x))....         
+00019090: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+000190a0: 7265 645f 7661 6c75 6573 203d 205b 7661  red_values = [va
+000190b0: 6c20 666f 7220 7661 6c20 696e 206e 6f6e  l for val in non
+000190c0: 5f6d 6974 6f74 6963 5f72 6164 6975 7320  _mitotic_radius 
+000190d0: 6966 2076 616c 2069 7320 6e6f 7420 4e6f  if val is not No
+000190e0: 6e65 5d0d 0a20 2020 2020 2020 2020 2020  ne]..           
+000190f0: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00019100: 6e5f 6d69 746f 7469 635f 6d65 616e 5f72  n_mitotic_mean_r
+00019110: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
+00019120: 6d65 616e 2866 696c 7465 7265 645f 7661  mean(filtered_va
+00019130: 6c75 6573 2929 0d0a 2020 2020 2020 2020  lues))..        
+00019140: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00019150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019160: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00019170: 6963 5f76 6172 5f72 6164 6975 732e 6170  ic_var_radius.ap
+00019180: 7065 6e64 286e 702e 7374 6428 6669 6c74  pend(np.std(filt
+00019190: 6572 6564 5f76 616c 7565 7329 290d 0a0d  ered_values))...
+000191a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000191b0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
+000191c0: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
+000191d0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+000191e0: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
+000191f0: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
+00019200: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
+00019210: 6e5f 6d69 746f 7469 635f 7661 725f 7370  n_mitotic_var_sp
+00019220: 6565 642e 6170 7065 6e64 286e 702e 7374  eed.append(np.st
+00019230: 6428 6e6f 6e5f 6d69 746f 7469 635f 7370  d(non_mitotic_sp
+00019240: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
+00019250: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019260: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00019270: 616e 5f61 6363 2e61 7070 656e 6428 6e70  an_acc.append(np
+00019280: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+00019290: 635f 6163 6329 290d 0a20 2020 2020 2020  c_acc))..       
+000192a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000192b0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
+000192c0: 725f 6163 632e 6170 7065 6e64 286e 702e  r_acc.append(np.
+000192d0: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+000192e0: 6163 6329 290d 0a0d 0a20 2020 2020 2020  acc))....       
+000192f0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019300: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
+00019310: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
+00019320: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
+00019330: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
+00019340: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
+00019350: 6e67 6529 290d 0a20 2020 2020 2020 2020  nge))..         
+00019360: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019370: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
+00019380: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00019390: 6765 2e61 7070 656e 6428 6e70 2e73 7464  ge.append(np.std
+000193a0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6972  (non_mitotic_dir
+000193b0: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
+000193c0: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
+000193d0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
+000193e0: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
+000193f0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00019400: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
+00019410: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
+00019420: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00019430: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00019440: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00019450: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+00019460: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
+00019470: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
+00019480: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
+00019490: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
+000194a0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+000194b0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+000194c0: 5f6d 6561 6e5f 6469 7370 5f7a 2e61 7070  _mean_disp_z.app
+000194d0: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
+000194e0: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
+000194f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019500: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
+00019510: 7a2e 6170 7065 6e64 286e 702e 7374 6428  z.append(np.std(
+00019520: 616c 6c5f 6469 7370 5f7a 2929 0d0a 0d0a  all_disp_z))....
+00019530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019540: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
+00019550: 6e5f 6469 7370 5f79 2e61 7070 656e 6428  n_disp_y.append(
+00019560: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7370  np.mean(all_disp
+00019570: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
+00019580: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00019590: 6c6c 5f76 6172 5f64 6973 705f 792e 6170  ll_var_disp_y.ap
+000195a0: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
+000195b0: 6469 7370 5f79 2929 0d0a 0d0a 2020 2020  disp_y))....    
+000195c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195d0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
+000195e0: 7370 5f78 2e61 7070 656e 6428 6e70 2e6d  sp_x.append(np.m
+000195f0: 6561 6e28 616c 6c5f 6469 7370 5f78 2929  ean(all_disp_x))
+00019600: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019610: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00019620: 6172 5f64 6973 705f 782e 6170 7065 6e64  ar_disp_x.append
+00019630: 286e 702e 7374 6428 616c 6c5f 6469 7370  (np.std(all_disp
+00019640: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
+00019650: 2020 2020 2020 2020 2020 2020 6669 6c74              filt
+00019660: 6572 6564 5f76 616c 7565 7320 3d20 5b76  ered_values = [v
+00019670: 616c 2066 6f72 2076 616c 2069 6e20 616c  al for val in al
+00019680: 6c5f 7261 6469 7573 2069 6620 7661 6c20  l_radius if val 
+00019690: 6973 206e 6f74 204e 6f6e 655d 0d0a 2020  is not None]..  
+000196a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000196b0: 2020 7365 6c66 2e61 6c6c 5f6d 6561 6e5f    self.all_mean_
+000196c0: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
+000196d0: 2e6d 6561 6e28 6669 6c74 6572 6564 5f76  .mean(filtered_v
+000196e0: 616c 7565 7329 290d 0a20 2020 2020 2020  alues))..       
+000196f0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
+00019700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019710: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+00019720: 7261 6469 7573 2e61 7070 656e 6428 6e70  radius.append(np
+00019730: 2e73 7464 2866 696c 7465 7265 645f 7661  .std(filtered_va
+00019740: 6c75 6573 2929 0d0a 0d0a 2020 2020 2020  lues))....      
+00019750: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019760: 6c66 2e61 6c6c 5f6d 6561 6e5f 7370 6565  lf.all_mean_spee
+00019770: 642e 6170 7065 6e64 286e 702e 6d65 616e  d.append(np.mean
+00019780: 2861 6c6c 5f73 7065 6564 2929 0d0a 2020  (all_speed))..  
+00019790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197a0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f73    self.all_var_s
+000197b0: 7065 6564 2e61 7070 656e 6428 6e70 2e73  peed.append(np.s
+000197c0: 7464 2861 6c6c 5f73 7065 6564 2929 0d0a  td(all_speed))..
+000197d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000197e0: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+000197f0: 6561 6e5f 6163 632e 6170 7065 6e64 286e  ean_acc.append(n
+00019800: 702e 6d65 616e 2861 6c6c 5f61 6363 2929  p.mean(all_acc))
+00019810: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019820: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
+00019830: 6172 5f61 6363 2e61 7070 656e 6428 6e70  ar_acc.append(np
+00019840: 2e73 7464 2861 6c6c 5f61 6363 2929 0d0a  .std(all_acc))..
+00019850: 0d0a 0d0a 0d0a 2020 2020 2020 2020 2020  ......          
+00019860: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+00019870: 6c6c 5f6d 6561 6e5f 6469 7265 6374 696f  ll_mean_directio
+00019880: 6e61 6c5f 6368 616e 6765 2e61 7070 656e  nal_change.appen
+00019890: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
+000198a0: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+000198b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000198c0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
+000198d0: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
+000198e0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
+000198f0: 702e 7374 6428 616c 6c5f 6469 7265 6374  p.std(all_direct
+00019900: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
+00019910: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019920: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00019930: 6561 6e5f 6469 7374 616e 6365 5f63 656c  ean_distance_cel
+00019940: 6c5f 6d61 736b 2e61 7070 656e 6428 6e70  l_mask.append(np
+00019950: 2e6d 6561 6e28 616c 6c5f 6469 7374 616e  .mean(all_distan
+00019960: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
+00019970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019980: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+00019990: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+000199a0: 6173 6b2e 6170 7065 6e64 286e 702e 7374  ask.append(np.st
+000199b0: 6428 616c 6c5f 6469 7374 616e 6365 5f63  d(all_distance_c
+000199c0: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
+000199d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+000199f0: 2020 0d0a 6465 6620 626f 756e 6461 7279    ..def boundary
+00019a00: 5f70 6f69 6e74 7328 6d61 736b 2c20 7863  _points(mask, xc
+00019a10: 616c 6962 7261 7469 6f6e 2c20 7963 616c  alibration, ycal
+00019a20: 6962 7261 7469 6f6e 2c20 7a63 616c 6962  ibration, zcalib
+00019a30: 7261 7469 6f6e 293a 0d0a 0d0a 2020 2020  ration):....    
+00019a40: 6e64 696d 203d 206c 656e 286d 6173 6b2e  ndim = len(mask.
+00019a50: 7368 6170 6529 0d0a 2020 2020 7469 6d65  shape)..    time
+00019a60: 645f 6d61 736b 203d 207b 7d0d 0a20 2020  d_mask = {}..   
+00019a70: 206d 6173 6b20 3d20 6d61 736b 203e 2030   mask = mask > 0
+00019a80: 0d0a 2020 2020 6d61 736b 203d 206d 6173  ..    mask = mas
+00019a90: 6b2e 6173 7479 7065 2827 7569 6e74 3827  k.astype('uint8'
+00019aa0: 290d 0a20 2020 2023 2059 5820 7368 6170  )..    # YX shap
+00019ab0: 6564 206f 626a 6563 740d 0a20 2020 2069  ed object..    i
+00019ac0: 6620 6e64 696d 203d 3d20 323a 0d0a 2020  f ndim == 2:..  
+00019ad0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00019ae0: 626f 756e 6461 7279 203d 2066 696e 645f  boundary = find_
+00019af0: 626f 756e 6461 7269 6573 286d 6173 6b29  boundaries(mask)
+00019b00: 0d0a 2020 2020 2020 2020 7265 6769 6f6e  ..        region
+00019b10: 6365 6e74 726f 6964 203d 2028 302c 2920  centroid = (0,) 
+00019b20: 2b20 636f 6d70 7574 655f 6365 6e74 726f  + compute_centro
+00019b30: 6964 2862 6f75 6e64 6172 7929 200d 0a20  id(boundary) .. 
+00019b40: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
+00019b50: 206e 702e 7768 6572 6528 626f 756e 6461   np.where(bounda
+00019b60: 7279 203e 2030 290d 0a20 2020 2020 2020  ry > 0)..       
+00019b70: 2072 6561 6c5f 696e 6469 6365 7320 3d20   real_indices = 
+00019b80: 6e70 2e74 7261 6e73 706f 7365 286e 702e  np.transpose(np.
+00019b90: 6173 6172 7261 7928 696e 6469 6365 732c  asarray(indices,
+00019ba0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00019bb0: 3229 292e 636f 7079 2829 0d0a 0d0a 2020  2)).copy()....  
+00019bc0: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
+00019bd0: 616e 6765 2830 2c20 6c65 6e28 7265 616c  ange(0, len(real
+00019be0: 5f69 6e64 6963 6573 2929 3a0d 0a0d 0a20  _indices)):.... 
+00019bf0: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
+00019c00: 696e 6469 6365 735b 6a5d 5b30 5d20 3d20  indices[j][0] = 
+00019c10: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
+00019c20: 305d 202a 2079 6361 6c69 6272 6174 696f  0] * ycalibratio
+00019c30: 6e0d 0a20 2020 2020 2020 2020 2020 2072  n..            r
+00019c40: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
+00019c50: 5d20 3d20 7265 616c 5f69 6e64 6963 6573  ] = real_indices
+00019c60: 5b6a 5d5b 315d 202a 2078 6361 6c69 6272  [j][1] * xcalibr
+00019c70: 6174 696f 6e0d 0a0d 0a20 2020 2020 2020  ation....       
+00019c80: 2074 7265 6520 3d20 7370 6174 6961 6c2e   tree = spatial.
+00019c90: 634b 4454 7265 6528 7265 616c 5f69 6e64  cKDTree(real_ind
+00019ca0: 6963 6573 290d 0a20 2020 2020 2020 2023  ices)..        #
+00019cb0: 2054 6869 7320 6f62 6a65 6374 2063 6f6e   This object con
+00019cc0: 7461 696e 7320 6c69 7374 206f 6620 616c  tains list of al
+00019cd0: 6c20 7468 6520 706f 696e 7473 2066 6f72  l the points for
+00019ce0: 2061 6c6c 2074 6865 206c 6162 656c 7320   all the labels 
+00019cf0: 696e 2074 6865 204d 6173 6b20 696d 6167  in the Mask imag
+00019d00: 6520 7769 7468 2074 6865 206c 6162 656c  e with the label
+00019d10: 2069 6420 616e 6420 766f 6c75 6d65 206f   id and volume o
+00019d20: 6620 6561 6368 206c 6162 656c 0d0a 2020  f each label..  
+00019d30: 2020 2020 2020 7469 6d65 645f 6d61 736b        timed_mask
+00019d40: 5b73 7472 2830 295d 203d 205b 7472 6565  [str(0)] = [tree
+00019d50: 2c20 696e 6469 6365 732c 2072 6567 696f  , indices, regio
+00019d60: 6e63 656e 7472 6f69 645d 0d0a 0d0a 2020  ncentroid]....  
+00019d70: 2020 2320 5459 5820 7368 6170 6564 206f    # TYX shaped o
+00019d80: 626a 6563 740d 0a20 2020 2069 6620 6e64  bject..    if nd
+00019d90: 696d 203d 3d20 333a 0d0a 0d0a 0d0a 2020  im == 3:......  
+00019da0: 2020 2020 2020 666f 7220 6920 696e 2074        for i in t
+00019db0: 7164 6d28 7261 6e67 6528 302c 206d 6173  qdm(range(0, mas
+00019dc0: 6b2e 7368 6170 655b 305d 2929 3a0d 0a20  k.shape[0])):.. 
+00019dd0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
+00019de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019df0: 2062 6f75 6e64 6172 7920 3d20 6669 6e64   boundary = find
+00019e00: 5f62 6f75 6e64 6172 6965 7328 6d61 736b  _boundaries(mask
+00019e10: 5b69 2c3a 5d29 0d0a 2020 2020 2020 2020  [i,:])..        
+00019e20: 2020 2020 2020 2020 7265 6769 6f6e 6365          regionce
+00019e30: 6e74 726f 6964 203d 2028 302c 2920 2b20  ntroid = (0,) + 
+00019e40: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
+00019e50: 2862 6f75 6e64 6172 7929 200d 0a20 2020  (boundary) ..   
+00019e60: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+00019e70: 6963 6573 203d 206e 702e 7768 6572 6528  ices = np.where(
+00019e80: 626f 756e 6461 7279 203e 2030 290d 0a20  boundary > 0).. 
+00019e90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00019ea0: 6561 6c5f 696e 6469 6365 7320 3d20 6e70  eal_indices = np
+00019eb0: 2e74 7261 6e73 706f 7365 286e 702e 6173  .transpose(np.as
+00019ec0: 6172 7261 7928 696e 6469 6365 732c 2064  array(indices, d
+00019ed0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+00019ee0: 292e 636f 7079 2829 0d0a 0d0a 2020 2020  ).copy()....    
+00019ef0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00019f00: 6a20 696e 2072 616e 6765 2830 2c20 6c65  j in range(0, le
+00019f10: 6e28 7265 616c 5f69 6e64 6963 6573 2929  n(real_indices))
+00019f20: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
+00019f30: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+00019f40: 6469 6365 735b 6a5d 5b30 5d20 3d20 7265  dices[j][0] = re
+00019f50: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
+00019f60: 202a 2079 6361 6c69 6272 6174 696f 6e0d   * ycalibration.
+00019f70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019f80: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
+00019f90: 735b 6a5d 5b31 5d20 3d20 7265 616c 5f69  s[j][1] = real_i
+00019fa0: 6e64 6963 6573 5b6a 5d5b 315d 202a 2078  ndices[j][1] * x
+00019fb0: 6361 6c69 6272 6174 696f 6e0d 0a0d 0a20  calibration.... 
+00019fc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00019fd0: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
+00019fe0: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
+00019ff0: 6573 290d 0a0d 0a20 2020 2020 2020 2020  es)....         
+0001a000: 2020 2020 2020 2074 696d 6564 5f6d 6173         timed_mas
+0001a010: 6b5b 7374 7228 6929 5d20 3d20 5b74 7265  k[str(i)] = [tre
+0001a020: 652c 2069 6e64 6963 6573 2c20 7265 6769  e, indices, regi
+0001a030: 6f6e 6365 6e74 726f 6964 5d0d 0a20 2020  oncentroid]..   
+0001a040: 2020 2020 2020 2020 200d 0a20 2020 2023           ..    #
+0001a050: 2054 5a59 5820 7368 6170 6564 206f 626a   TZYX shaped obj
+0001a060: 6563 740d 0a20 2020 2069 6620 6e64 696d  ect..    if ndim
+0001a070: 203d 3d20 343a 0d0a 2020 2020 2020 2020   == 4:..        
+0001a080: 7072 696e 7428 274d 616b 696e 6720 6d61  print('Making ma
+0001a090: 736b 2069 6e20 3444 2729 0d0a 2020 2020  sk in 4D')..    
+0001a0a0: 2020 2020 626f 756e 6461 7279 203d 206e      boundary = n
+0001a0b0: 702e 7a65 726f 7328 0d0a 2020 2020 2020  p.zeros(..      
+0001a0c0: 2020 2020 2020 5b6d 6173 6b2e 7368 6170        [mask.shap
+0001a0d0: 655b 305d 2c20 6d61 736b 2e73 6861 7065  e[0], mask.shape
+0001a0e0: 5b31 5d2c 206d 6173 6b2e 7368 6170 655b  [1], mask.shape[
+0001a0f0: 325d 2c20 6d61 736b 2e73 6861 7065 5b33  2], mask.shape[3
+0001a100: 5d5d 2c20 6474 7970 653d 6e70 2e75 696e  ]], dtype=np.uin
+0001a110: 7438 0d0a 2020 2020 2020 2020 290d 0a20  t8..        ).. 
+0001a120: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
+0001a130: 7261 6e67 6528 302c 206d 6173 6b2e 7368  range(0, mask.sh
+0001a140: 6170 655b 305d 293a 0d0a 2020 2020 2020  ape[0]):..      
+0001a150: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001a160: 2020 2020 626f 756e 6461 7279 5b69 2c3a      boundary[i,:
+0001a170: 5d20 3d20 6669 6e64 5f62 6f75 6e64 6172  ] = find_boundar
+0001a180: 6965 7328 6d61 736b 5b69 2c3a 5d29 0d0a  ies(mask[i,:])..
+0001a190: 2020 2020 2020 2020 2020 2020 7265 6769              regi
+0001a1a0: 6f6e 6365 6e74 726f 6964 203d 2063 6f6d  oncentroid = com
+0001a1b0: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
+0001a1c0: 756e 6461 7279 5b69 2c3a 5d29 200d 0a20  undary[i,:]) .. 
+0001a1d0: 2020 2020 2020 2020 2020 2069 6e64 6963             indic
+0001a1e0: 6573 203d 206e 702e 7768 6572 6528 626f  es = np.where(bo
+0001a1f0: 756e 6461 7279 5b69 2c3a 5d20 3e20 3029  undary[i,:] > 0)
+0001a200: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+0001a210: 616c 5f69 6e64 6963 6573 203d 206e 702e  al_indices = np.
+0001a220: 7472 616e 7370 6f73 6528 6e70 2e61 7361  transpose(np.asa
+0001a230: 7272 6179 2869 6e64 6963 6573 2c20 6474  rray(indices, dt
+0001a240: 7970 653d 6e70 2e66 6c6f 6174 3332 2929  ype=np.float32))
+0001a250: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
+0001a260: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+0001a270: 7261 6e67 6528 302c 206c 656e 2872 6561  range(0, len(rea
+0001a280: 6c5f 696e 6469 6365 7329 293a 0d0a 0d0a  l_indices)):....
+0001a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2a0: 2020 2020 7265 616c 5f69 6e64 6963 6573      real_indices
+0001a2b0: 5b6a 5d5b 305d 203d 2072 6561 6c5f 696e  [j][0] = real_in
+0001a2c0: 6469 6365 735b 6a5d 5b30 5d20 2a20 7a63  dices[j][0] * zc
+0001a2d0: 616c 6962 7261 7469 6f6e 0d0a 2020 2020  alibration..    
+0001a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2f0: 7265 616c 5f69 6e64 6963 6573 5b6a 5d5b  real_indices[j][
+0001a300: 315d 203d 2072 6561 6c5f 696e 6469 6365  1] = real_indice
+0001a310: 735b 6a5d 5b31 5d20 2a20 7963 616c 6962  s[j][1] * ycalib
+0001a320: 7261 7469 6f6e 0d0a 2020 2020 2020 2020  ration..        
+0001a330: 2020 2020 2020 2020 2020 2020 7265 616c              real
+0001a340: 5f69 6e64 6963 6573 5b6a 5d5b 325d 203d  _indices[j][2] =
+0001a350: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+0001a360: 5b32 5d20 2a20 7863 616c 6962 7261 7469  [2] * xcalibrati
+0001a370: 6f6e 0d0a 0d0a 2020 2020 2020 2020 2020  on....          
+0001a380: 2020 7472 6565 203d 2073 7061 7469 616c    tree = spatial
+0001a390: 2e63 4b44 5472 6565 2872 6561 6c5f 696e  .cKDTree(real_in
+0001a3a0: 6469 6365 7329 0d0a 2020 2020 2020 2020  dices)..        
+0001a3b0: 2020 2020 7469 6d65 645f 6d61 736b 5b73      timed_mask[s
+0001a3c0: 7472 2869 295d 203d 205b 7472 6565 2c20  tr(i)] = [tree, 
+0001a3d0: 696e 6469 6365 732c 2072 6567 696f 6e63  indices, regionc
+0001a3e0: 656e 7472 6f69 645d 0d0a 2020 2020 7072  entroid]..    pr
+0001a3f0: 696e 7428 2743 6f6d 7075 7465 6420 7468  int('Computed th
+0001a400: 6520 626f 756e 6461 7279 2070 6f69 6e74  e boundary point
+0001a410: 7327 290d 0a0d 0a20 2020 2072 6574 7572  s')....    retur
+0001a420: 6e20 7469 6d65 645f 6d61 736b 2c20 626f  n timed_mask, bo
+0001a430: 756e 6461 7279 2020 2020 2020 2020 0d0a  undary        ..
+0001a440: 0d0a 6465 6620 636f 6d70 7574 655f 6365  ..def compute_ce
+0001a450: 6e74 726f 6964 2862 696e 6172 795f 696d  ntroid(binary_im
+0001a460: 6167 6529 3a0d 0a20 2020 2023 2045 6e73  age):..    # Ens
+0001a470: 7572 6520 6269 6e61 7279 2069 6d61 6765  ure binary image
+0001a480: 2069 7320 6120 4e75 6d50 7920 6172 7261   is a NumPy arra
+0001a490: 790d 0a20 2020 2062 696e 6172 795f 696d  y..    binary_im
+0001a4a0: 6167 6520 3d20 6e70 2e61 7272 6179 2862  age = np.array(b
+0001a4b0: 696e 6172 795f 696d 6167 6529 0d0a 0d0a  inary_image)....
+0001a4c0: 2020 2020 7768 6974 655f 7069 7865 6c73      white_pixels
+0001a4d0: 203d 206e 702e 7768 6572 6528 6269 6e61   = np.where(bina
+0001a4e0: 7279 5f69 6d61 6765 203d 3d20 3129 0d0a  ry_image == 1)..
+0001a4f0: 2020 2020 6e75 6d5f 7069 7865 6c73 203d      num_pixels =
+0001a500: 206c 656e 2877 6869 7465 5f70 6978 656c   len(white_pixel
+0001a510: 735b 305d 290d 0a0d 0a20 2020 2023 2043  s[0])....    # C
+0001a520: 6f6d 7075 7465 2074 6865 2063 656e 7472  ompute the centr
+0001a530: 6f69 6420 6f66 2074 6865 2077 6869 7465  oid of the white
+0001a540: 2070 6978 656c 7320 696e 2074 6865 2062   pixels in the b
+0001a550: 6f75 6e64 6172 7920 696d 6167 650d 0a20  oundary image.. 
+0001a560: 2020 2063 656e 7472 6f69 6420 3d20 6e70     centroid = np
+0001a570: 2e7a 6572 6f73 2862 696e 6172 795f 696d  .zeros(binary_im
+0001a580: 6167 652e 6e64 696d 290d 0a20 2020 2066  age.ndim)..    f
+0001a590: 6f72 2064 696d 2069 6e20 7261 6e67 6528  or dim in range(
+0001a5a0: 6269 6e61 7279 5f69 6d61 6765 2e6e 6469  binary_image.ndi
+0001a5b0: 6d29 3a0d 0a20 2020 2020 2020 2063 656e  m):..        cen
+0001a5c0: 7472 6f69 645b 6469 6d5d 203d 2077 6869  troid[dim] = whi
+0001a5d0: 7465 5f70 6978 656c 735b 6469 6d5d 2e73  te_pixels[dim].s
+0001a5e0: 756d 2829 202f 206e 756d 5f70 6978 656c  um() / num_pixel
+0001a5f0: 730d 0a0d 0a20 2020 2072 6574 7572 6e20  s....    return 
+0001a600: 6365 6e74 726f 6964 0d0a 0d0a 0d0a 0d0a  centroid........
+0001a610: 200d 0a0d 0a64 6566 2067 6574 5f63 7376   ....def get_csv
+0001a620: 5f64 6174 6128 6373 7629 3a0d 0a0d 0a20  _data(csv):.... 
+0001a630: 2020 2020 2020 2064 6174 6173 6574 203d         dataset =
+0001a640: 2070 642e 7265 6164 5f63 7376 280d 0a20   pd.read_csv(.. 
+0001a650: 2020 2020 2020 2020 2020 2063 7376 2c20             csv, 
+0001a660: 6465 6c69 6d69 7465 723d 222c 222c 2065  delimiter=",", e
+0001a670: 6e63 6f64 696e 673d 2275 6e69 636f 6465  ncoding="unicode
+0001a680: 5f65 7363 6170 6522 2c20 6c6f 775f 6d65  _escape", low_me
+0001a690: 6d6f 7279 3d46 616c 7365 0d0a 2020 2020  mory=False..    
+0001a6a0: 2020 2020 295b 333a 5d0d 0a20 2020 2020      )[3:]..     
+0001a6b0: 2020 2064 6174 6173 6574 5f69 6e64 6578     dataset_index
+0001a6c0: 203d 2064 6174 6173 6574 2e69 6e64 6578   = dataset.index
+0001a6d0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001a6e0: 2064 6174 6173 6574 2c20 6461 7461 7365   dataset, datase
+0001a6f0: 745f 696e 6465 780d 0a20 2020 200d 0a64  t_index..    ..d
+0001a700: 6566 2067 6574 5f73 706f 745f 6461 7461  ef get_spot_data
+0001a710: 7365 7428 7370 6f74 5f64 6174 6173 6574  set(spot_dataset
+0001a720: 2c20 7472 6163 6b5f 616e 616c 7973 6973  , track_analysis
+0001a730: 5f73 706f 745f 6b65 7973 2c20 7863 616c  _spot_keys, xcal
+0001a740: 6962 7261 7469 6f6e 2c20 7963 616c 6962  ibration, ycalib
+0001a750: 7261 7469 6f6e 2c20 7a63 616c 6962 7261  ration, zcalibra
+0001a760: 7469 6f6e 2c20 4174 7472 6962 7574 6542  tion, AttributeB
+0001a770: 6f78 6e61 6d65 2c20 6465 7465 6374 696f  oxname, detectio
+0001a780: 6e63 6861 6e6e 656c 293a 0d0a 2020 2020  nchannel):..    
+0001a790: 2020 2020 416c 6c56 616c 7565 7320 3d20      AllValues = 
+0001a7a0: 7b7d 0d0a 2020 2020 2020 2020 706f 7369  {}..        posi
+0001a7b0: 7820 3d20 7472 6163 6b5f 616e 616c 7973  x = track_analys
+0001a7c0: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
+0001a7d0: 7369 7822 5d0d 0a20 2020 2020 2020 2070  six"]..        p
+0001a7e0: 6f73 6979 203d 2074 7261 636b 5f61 6e61  osiy = track_ana
+0001a7f0: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+0001a800: 2270 6f73 6979 225d 0d0a 2020 2020 2020  "posiy"]..      
+0001a810: 2020 706f 7369 7a20 3d20 7472 6163 6b5f    posiz = track_
+0001a820: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001a830: 7973 5b22 706f 7369 7a22 5d0d 0a20 2020  ys["posiz"]..   
+0001a840: 2020 2020 2066 7261 6d65 203d 2074 7261       frame = tra
+0001a850: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001a860: 5f6b 6579 735b 2266 7261 6d65 225d 0d0a  _keys["frame"]..
+0001a870: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001a880: 2020 4c6f 6361 7469 6f6e 5820 3d20 280d    LocationX = (.
+0001a890: 0a20 2020 2020 2020 2020 2020 2073 706f  .            spo
+0001a8a0: 745f 6461 7461 7365 745b 706f 7369 785d  t_dataset[posix]
+0001a8b0: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
+0001a8c0: 202f 2078 6361 6c69 6272 6174 696f 6e0d   / xcalibration.
+0001a8d0: 0a20 2020 2020 2020 2029 2e61 7374 7970  .        ).astyp
+0001a8e0: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
+0001a8f0: 2020 4c6f 6361 7469 6f6e 5920 3d20 280d    LocationY = (.
+0001a900: 0a20 2020 2020 2020 2020 2020 2073 706f  .            spo
+0001a910: 745f 6461 7461 7365 745b 706f 7369 795d  t_dataset[posiy]
+0001a920: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
+0001a930: 202f 2079 6361 6c69 6272 6174 696f 6e0d   / ycalibration.
+0001a940: 0a20 2020 2020 2020 2029 2e61 7374 7970  .        ).astyp
+0001a950: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
+0001a960: 2020 4c6f 6361 7469 6f6e 5a20 3d20 280d    LocationZ = (.
+0001a970: 0a20 2020 2020 2020 2020 2020 2073 706f  .            spo
+0001a980: 745f 6461 7461 7365 745b 706f 7369 7a5d  t_dataset[posiz]
+0001a990: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
+0001a9a0: 202f 207a 6361 6c69 6272 6174 696f 6e0d   / zcalibration.
+0001a9b0: 0a20 2020 2020 2020 2029 2e61 7374 7970  .        ).astyp
+0001a9c0: 6528 2269 6e74 2229 0d0a 2020 2020 2020  e("int")..      
+0001a9d0: 2020 4c6f 6361 7469 6f6e 5420 3d20 2873    LocationT = (s
+0001a9e0: 706f 745f 6461 7461 7365 745b 6672 616d  pot_dataset[fram
+0001a9f0: 655d 2e61 7374 7970 6528 2266 6c6f 6174  e].astype("float
+0001aa00: 2229 292e 6173 7479 7065 2822 696e 7422  ")).astype("int"
+0001aa10: 290d 0a20 2020 2020 2020 200d 0a0d 0a20  )..        .... 
+0001aa20: 2020 2020 2020 2069 676e 6f72 655f 7661         ignore_va
+0001aa30: 6c75 6573 203d 205b 7472 6163 6b5f 616e  lues = [track_an
+0001aa40: 616c 7973 6973 5f73 706f 745f 6b65 7973  alysis_spot_keys
+0001aa50: 5b22 6d65 616e 5f69 6e74 656e 7369 7479  ["mean_intensity
+0001aa60: 225d 2c74 7261 636b 5f61 6e61 6c79 7369  "],track_analysi
+0001aa70: 735f 7370 6f74 5f6b 6579 735b 2274 6f74  s_spot_keys["tot
+0001aa80: 616c 5f69 6e74 656e 7369 7479 225d 5d0d  al_intensity"]].
+0001aa90: 0a20 2020 2020 2020 2066 6f72 2028 6b2c  .        for (k,
+0001aaa0: 7629 2069 6e20 7472 6163 6b5f 616e 616c  v) in track_anal
+0001aab0: 7973 6973 5f73 706f 745f 6b65 7973 2e69  ysis_spot_keys.i
+0001aac0: 7465 6d73 2829 3a0d 0a0d 0a20 2020 2020  tems():....     
+0001aad0: 2020 2020 2020 2020 2020 2069 6620 6465             if de
+0001aae0: 7465 6374 696f 6e63 6861 6e6e 656c 203d  tectionchannel =
+0001aaf0: 3d20 313a 0d0a 2020 2020 2020 2020 2020  = 1:..          
+0001ab00: 2020 2020 2020 2020 2020 2069 6620 6b20             if k 
+0001ab10: 3d3d 2022 6d65 616e 5f69 6e74 656e 7369  == "mean_intensi
+0001ab20: 7479 5f63 6832 223a 0d0a 2020 2020 2020  ty_ch2":..      
+0001ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab40: 2020 2020 2076 616c 7565 203d 2074 7261       value = tra
+0001ab50: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001ab60: 5f6b 6579 735b 226d 6561 6e5f 696e 7465  _keys["mean_inte
+0001ab70: 6e73 6974 7922 5d0d 0a20 2020 2020 2020  nsity"]..       
+0001ab80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab90: 2020 2020 416c 6c56 616c 7565 735b 7661      AllValues[va
+0001aba0: 6c75 655d 203d 2073 706f 745f 6461 7461  lue] = spot_data
+0001abb0: 7365 745b 765d 2e61 7374 7970 6528 2266  set[v].astype("f
+0001abc0: 6c6f 6174 2229 0d0a 2020 2020 2020 2020  loat")..        
+0001abd0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001abe0: 6b20 3d3d 2022 746f 7461 6c5f 696e 7465  k == "total_inte
+0001abf0: 6e73 6974 795f 6368 3222 3a0d 0a20 2020  nsity_ch2":..   
+0001ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac10: 2020 2020 2020 2020 7661 6c75 6520 3d20          value = 
+0001ac20: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001ac30: 706f 745f 6b65 7973 5b22 746f 7461 6c5f  pot_keys["total_
+0001ac40: 696e 7465 6e73 6974 7922 5d0d 0a20 2020  intensity"]..   
+0001ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac60: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
+0001ac70: 735b 7661 6c75 655d 203d 2073 706f 745f  s[value] = spot_
+0001ac80: 6461 7461 7365 745b 765d 2e61 7374 7970  dataset[v].astyp
+0001ac90: 6528 2266 6c6f 6174 2229 2020 2020 2020  e("float")      
+0001aca0: 200d 0a0d 0a20 2020 2020 2020 2020 2020   ....           
+0001acb0: 2020 2020 2069 6620 7620 6e6f 7420 696e       if v not in
+0001acc0: 2069 676e 6f72 655f 7661 6c75 6573 3a0d   ignore_values:.
+0001acd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ace0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ad00: 2041 6c6c 5661 6c75 6573 5b76 5d20 3d20   AllValues[v] = 
+0001ad10: 7370 6f74 5f64 6174 6173 6574 5b76 5d2e  spot_dataset[v].
+0001ad20: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001ad30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ad40: 2020 2020 0d0a 0d0a 2020 2020 2020 2020      ....        
+0001ad50: 416c 6c56 616c 7565 735b 706f 7369 785d  AllValues[posix]
+0001ad60: 203d 2072 6f75 6e64 284c 6f63 6174 696f   = round(Locatio
+0001ad70: 6e58 2c33 290d 0a20 2020 2020 2020 2041  nX,3)..        A
+0001ad80: 6c6c 5661 6c75 6573 5b70 6f73 6979 5d20  llValues[posiy] 
+0001ad90: 3d20 726f 756e 6428 4c6f 6361 7469 6f6e  = round(Location
+0001ada0: 592c 3329 0d0a 2020 2020 2020 2020 416c  Y,3)..        Al
+0001adb0: 6c56 616c 7565 735b 706f 7369 7a5d 203d  lValues[posiz] =
+0001adc0: 2072 6f75 6e64 284c 6f63 6174 696f 6e5a   round(LocationZ
+0001add0: 2c33 290d 0a20 2020 2020 2020 2041 6c6c  ,3)..        All
+0001ade0: 5661 6c75 6573 5b66 7261 6d65 5d20 3d20  Values[frame] = 
+0001adf0: 726f 756e 6428 4c6f 6361 7469 6f6e 542c  round(LocationT,
+0001ae00: 3329 0d0a 2020 2020 2020 2020 4174 7472  3)..        Attr
+0001ae10: 6962 7574 6569 6473 203d 205b 5d0d 0a20  ibuteids = [].. 
+0001ae20: 2020 2020 2020 2041 7474 7269 6275 7465         Attribute
+0001ae30: 6964 732e 6170 7065 6e64 2841 7474 7269  ids.append(Attri
+0001ae40: 6275 7465 426f 786e 616d 6529 0d0a 2020  buteBoxname)..  
+0001ae50: 2020 2020 2020 666f 7220 6174 7472 6962        for attrib
+0001ae60: 7574 656e 616d 6520 696e 2041 6c6c 5661  utename in AllVa
+0001ae70: 6c75 6573 2e6b 6579 7328 293a 0d0a 2020  lues.keys():..  
+0001ae80: 2020 2020 2020 2020 2020 2020 4174 7472              Attr
+0001ae90: 6962 7574 6569 6473 2e61 7070 656e 6428  ibuteids.append(
+0001aea0: 6174 7472 6962 7574 656e 616d 6529 2020  attributename)  
+0001aeb0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0001aec0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0001aed0: 2020 2020 7265 7475 726e 2041 7474 7269      return Attri
+0001aee0: 6275 7465 6964 732c 2041 6c6c 5661 6c75  buteids, AllValu
+0001aef0: 6573 2020 2020 200d 0a20 2020 200d 0a64  es     ..    ..d
+0001af00: 6566 2067 6574 5f74 7261 636b 5f64 6174  ef get_track_dat
+0001af10: 6173 6574 2874 7261 636b 5f64 6174 6173  aset(track_datas
+0001af20: 6574 2c20 7472 6163 6b5f 616e 616c 7973  et, track_analys
+0001af30: 6973 5f73 706f 745f 6b65 7973 2c20 7472  is_spot_keys, tr
+0001af40: 6163 6b5f 616e 616c 7973 6973 5f74 7261  ack_analysis_tra
+0001af50: 636b 5f6b 6579 732c 2054 7261 636b 4174  ck_keys, TrackAt
+0001af60: 7472 6962 7574 6542 6f78 6e61 6d65 293a  tributeBoxname):
+0001af70: 0d0a 0d0a 2020 2020 2020 2020 416c 6c54  ....        AllT
+0001af80: 7261 636b 5661 6c75 6573 203d 207b 7d0d  rackValues = {}.
+0001af90: 0a20 2020 2020 2020 2074 7261 636b 5f69  .        track_i
+0001afa0: 6420 3d20 7472 6163 6b5f 616e 616c 7973  d = track_analys
+0001afb0: 6973 5f73 706f 745f 6b65 7973 5b22 7472  is_spot_keys["tr
+0001afc0: 6163 6b5f 6964 225d 0d0a 2020 2020 2020  ack_id"]..      
+0001afd0: 2020 5469 6420 3d20 7472 6163 6b5f 6461    Tid = track_da
+0001afe0: 7461 7365 745b 7472 6163 6b5f 6964 5d2e  taset[track_id].
+0001aff0: 6173 7479 7065 2822 666c 6f61 7422 290d  astype("float").
+0001b000: 0a20 2020 2020 2020 0d0a 2020 2020 2020  .       ..      
+0001b010: 2020 416c 6c54 7261 636b 5661 6c75 6573    AllTrackValues
+0001b020: 5b74 7261 636b 5f69 645d 203d 2054 6964  [track_id] = Tid
+0001b030: 0d0a 2020 2020 2020 0d0a 2020 2020 2020  ..      ..      
+0001b040: 2020 666f 7220 286b 2c20 7629 2069 6e20    for (k, v) in 
+0001b050: 7472 6163 6b5f 616e 616c 7973 6973 5f74  track_analysis_t
+0001b060: 7261 636b 5f6b 6579 732e 6974 656d 7328  rack_keys.items(
+0001b070: 293a 0d0a 0d0a 2020 2020 2020 2020 2020  ):....          
+0001b080: 2020 2020 2020 7820 3d20 7472 6163 6b5f        x = track_
+0001b090: 6461 7461 7365 745b 765d 2e61 7374 7970  dataset[v].astyp
+0001b0a0: 6528 2266 6c6f 6174 2229 0d0a 2020 2020  e("float")..    
+0001b0b0: 2020 2020 2020 2020 2020 2020 6d69 6e76              minv
+0001b0c0: 616c 203d 206d 696e 2878 290d 0a20 2020  al = min(x)..   
+0001b0d0: 2020 2020 2020 2020 2020 2020 206d 6178               max
+0001b0e0: 7661 6c20 3d20 6d61 7828 7829 0d0a 0d0a  val = max(x)....
+0001b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b100: 6966 206d 696e 7661 6c20 3e20 3020 616e  if minval > 0 an
+0001b110: 6420 6d61 7876 616c 203c 3d20 313a 0d0a  d maxval <= 1:..
+0001b120: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b130: 2020 2020 2020 7820 3d20 7820 2b20 310d        x = x + 1.
+0001b140: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001b150: 2020 2041 6c6c 5472 6163 6b56 616c 7565     AllTrackValue
+0001b160: 735b 6b5d 203d 2072 6f75 6e64 2878 2c20  s[k] = round(x, 
+0001b170: 3329 0d0a 0d0a 2020 2020 2020 2020 5472  3)....        Tr
+0001b180: 6163 6b41 7474 7269 6275 7465 6964 7320  ackAttributeids 
+0001b190: 3d20 5b5d 0d0a 2020 2020 2020 2020 5472  = []..        Tr
+0001b1a0: 6163 6b41 7474 7269 6275 7465 6964 732e  ackAttributeids.
+0001b1b0: 6170 7065 6e64 2854 7261 636b 4174 7472  append(TrackAttr
+0001b1c0: 6962 7574 6542 6f78 6e61 6d65 290d 0a20  ibuteBoxname).. 
+0001b1d0: 2020 2020 2020 2066 6f72 2061 7474 7269         for attri
+0001b1e0: 6275 7465 6e61 6d65 2069 6e20 7472 6163  butename in trac
+0001b1f0: 6b5f 616e 616c 7973 6973 5f74 7261 636b  k_analysis_track
+0001b200: 5f6b 6579 732e 6b65 7973 2829 3a0d 0a20  _keys.keys():.. 
+0001b210: 2020 2020 2020 2020 2020 2054 7261 636b             Track
+0001b220: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
+0001b230: 656e 6428 6174 7472 6962 7574 656e 616d  end(attributenam
+0001b240: 6529 2020 2020 0d0a 2020 2020 0d0a 2020  e)    ..    ..  
+0001b250: 2020 2020 2020 7265 7475 726e 2054 7261        return Tra
+0001b260: 636b 4174 7472 6962 7574 6569 6473 2c20  ckAttributeids, 
+0001b270: 416c 6c54 7261 636b 5661 6c75 6573 0d0a  AllTrackValues..
+0001b280: 2020 2020 0d0a 6465 6620 6765 745f 6564      ..def get_ed
+0001b290: 6765 735f 6461 7461 7365 7428 6564 6765  ges_dataset(edge
+0001b2a0: 735f 6461 7461 7365 742c 2065 6467 6573  s_dataset, edges
+0001b2b0: 5f64 6174 6173 6574 5f69 6e64 6578 2c20  _dataset_index, 
+0001b2c0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001b2d0: 706f 745f 6b65 7973 2c20 7472 6163 6b5f  pot_keys, track_
+0001b2e0: 616e 616c 7973 6973 5f65 6467 6573 5f6b  analysis_edges_k
+0001b2f0: 6579 7329 3a0d 0a0d 0a20 2020 2020 2020  eys):....       
+0001b300: 2041 6c6c 4564 6765 7356 616c 7565 7320   AllEdgesValues 
+0001b310: 3d20 7b7d 0d0a 2020 2020 2020 2020 7472  = {}..        tr
+0001b320: 6163 6b5f 6964 203d 2074 7261 636b 5f61  ack_id = track_a
 0001b330: 6e61 6c79 7369 735f 7370 6f74 5f6b 6579  nalysis_spot_key
-0001b340: 732c 2074 7261 636b 5f61 6e61 6c79 7369  s, track_analysi
-0001b350: 735f 6564 6765 735f 6b65 7973 293a 0d0a  s_edges_keys):..
-0001b360: 0d0a 2020 2020 2020 2020 416c 6c45 6467  ..        AllEdg
-0001b370: 6573 5661 6c75 6573 203d 207b 7d0d 0a20  esValues = {}.. 
-0001b380: 2020 2020 2020 2074 7261 636b 5f69 6420         track_id 
-0001b390: 3d20 7472 6163 6b5f 616e 616c 7973 6973  = track_analysis
-0001b3a0: 5f73 706f 745f 6b65 7973 5b22 7472 6163  _spot_keys["trac
-0001b3b0: 6b5f 6964 225d 0d0a 2020 2020 2020 2020  k_id"]..        
-0001b3c0: 5469 6420 3d20 6564 6765 735f 6461 7461  Tid = edges_data
-0001b3d0: 7365 745b 7472 6163 6b5f 6964 5d2e 6173  set[track_id].as
-0001b3e0: 7479 7065 2822 666c 6f61 7422 290d 0a20  type("float").. 
-0001b3f0: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
-0001b400: 206e 702e 7768 6572 6528 5469 6420 3d3d   np.where(Tid ==
-0001b410: 2030 290d 0a20 2020 2020 2020 206d 6178   0)..        max
-0001b420: 7472 6163 6b5f 6964 203d 206d 6178 2854  track_id = max(T
-0001b430: 6964 290d 0a20 2020 2020 2020 2063 6f6e  id)..        con
-0001b440: 6469 7469 6f6e 5f69 6e64 6963 6573 203d  dition_indices =
-0001b450: 2065 6467 6573 5f64 6174 6173 6574 5f69   edges_dataset_i
-0001b460: 6e64 6578 5b69 6e64 6963 6573 5d0d 0a20  ndex[indices].. 
-0001b470: 2020 2020 2020 2054 6964 5b63 6f6e 6469         Tid[condi
-0001b480: 7469 6f6e 5f69 6e64 6963 6573 5d20 3d20  tion_indices] = 
-0001b490: 6d61 7874 7261 636b 5f69 6420 2b20 310d  maxtrack_id + 1.
-0001b4a0: 0a20 2020 2020 2020 2041 6c6c 4564 6765  .        AllEdge
-0001b4b0: 7356 616c 7565 735b 7472 6163 6b5f 6964  sValues[track_id
-0001b4c0: 5d20 3d20 5469 640d 0a0d 0a20 2020 2020  ] = Tid....     
-0001b4d0: 2020 2066 6f72 206b 2069 6e20 7472 6163     for k in trac
-0001b4e0: 6b5f 616e 616c 7973 6973 5f65 6467 6573  k_analysis_edges
-0001b4f0: 5f6b 6579 732e 7661 6c75 6573 2829 3a0d  _keys.values():.
-0001b500: 0a0d 0a20 2020 2020 2020 2020 2020 2069  ...            i
-0001b510: 6620 6b20 213d 2074 7261 636b 5f69 643a  f k != track_id:
-0001b520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b530: 2020 7820 3d20 6564 6765 735f 6461 7461    x = edges_data
-0001b540: 7365 745b 6b5d 2e61 7374 7970 6528 2266  set[k].astype("f
-0001b550: 6c6f 6174 2229 0d0a 0d0a 2020 2020 2020  loat")....      
-0001b560: 2020 2020 2020 2020 2020 416c 6c45 6467            AllEdg
-0001b570: 6573 5661 6c75 6573 5b6b 5d20 3d20 7820  esValues[k] = x 
-0001b580: 2020 0d0a 2020 2020 2020 2020 200d 0a20    ..         .. 
-0001b590: 2020 2020 2020 2072 6574 7572 6e20 416c         return Al
-0001b5a0: 6c45 6467 6573 5661 6c75 6573 2020 200d  lEdgesValues   .
-0001b5b0: 0a20 2020 200d 0a20 2020 2020 2020 0d0a  .    ..       ..
-0001b5c0: 2020 2020 0d0a 6465 6620 7363 616c 655f      ..def scale_
-0001b5d0: 7661 6c75 6528 782c 2073 6361 6c65 203d  value(x, scale =
-0001b5e0: 2032 3535 202a 2032 3535 293a 0d0a 0d0a   255 * 255):....
-0001b5f0: 0d0a 2020 2020 2072 6574 7572 6e20 7820  ..     return x 
-0001b600: 2a20 7363 616c 6520 2020 0d0a 2020 2020  * scale   ..    
-0001b610: 0d0a 0d0a 0d0a 6465 6620 7072 6f62 5f73  ......def prob_s
-0001b620: 6967 6d6f 6964 2878 293a 0d0a 2020 2020  igmoid(x):..    
-0001b630: 7265 7475 726e 2031 202d 206d 6174 682e  return 1 - math.
-0001b640: 6578 7028 2d78 290d 0a0d 0a0d 0a64 6566  exp(-x)......def
-0001b650: 2061 6e67 756c 6172 5f63 6861 6e67 6528   angular_change(
-0001b660: 7665 635f 302c 2076 6563 5f31 293a 0d0a  vec_0, vec_1):..
-0001b670: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001b680: 2020 7665 635f 3020 3d20 7665 635f 3020    vec_0 = vec_0 
-0001b690: 2f20 6e70 2e6c 696e 616c 672e 6e6f 726d  / np.linalg.norm
-0001b6a0: 2876 6563 5f30 290d 0a20 2020 2020 2020  (vec_0)..       
-0001b6b0: 2076 6563 5f31 203d 2076 6563 5f31 202f   vec_1 = vec_1 /
-0001b6c0: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
-0001b6d0: 7665 635f 3129 0d0a 2020 2020 2020 2020  vec_1)..        
-0001b6e0: 616e 676c 6520 3d20 6e70 2e61 7263 636f  angle = np.arcco
-0001b6f0: 7328 6e70 2e63 6c69 7028 6e70 2e64 6f74  s(np.clip(np.dot
-0001b700: 2876 6563 5f30 2c20 7665 635f 3129 2c20  (vec_0, vec_1), 
-0001b710: 2d31 2e30 2c20 312e 3029 290d 0a20 2020  -1.0, 1.0))..   
-0001b720: 2020 2020 2061 6e67 6c65 203d 2061 6e67       angle = ang
-0001b730: 6c65 202a 2031 3830 202f 206e 702e 7069  le * 180 / np.pi
-0001b740: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0001b750: 2061 6e67 6c65 0d0a 2020 2020 200d 0a0d   angle..     ...
-0001b760: 0a64 6566 2065 7661 6c5f 626f 6f6c 2876  .def eval_bool(v
-0001b770: 616c 7565 293a 0d0a 2020 2020 2020 2020  alue):..        
-0001b780: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0001b790: 2020 2020 6966 2076 616c 7565 2020 3d3d      if value  ==
-0001b7a0: 2027 5472 7565 273a 200d 0a20 2020 2020   'True': ..     
-0001b7b0: 2020 2020 2020 2020 2020 2064 6976 5f6b             div_k
-0001b7c0: 6579 203d 2054 7275 650d 0a20 2020 2020  ey = True..     
-0001b7d0: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-0001b7e0: 2020 2020 2020 2020 2020 6469 765f 6b65            div_ke
-0001b7f0: 7920 3d20 4661 6c73 6520 0d0a 0d0a 2020  y = False ....  
-0001b800: 2020 2020 2020 7265 7475 726e 2064 6976        return div
-0001b810: 5f6b 6579 2020 2020 2020 2020 2020 2020  _key            
-0001b820: 2020 2020 0d0a 0d0a 6465 6620 6368 6563      ....def chec
-0001b830: 6b5f 616e 645f 7570 6461 7465 5f6d 6173  k_and_update_mas
-0001b840: 6b28 6d61 736b 2c69 6d61 6765 293a 0d0a  k(mask,image):..
-0001b850: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001b860: 2069 6620 6c65 6e28 6d61 736b 2e73 6861   if len(mask.sha
-0001b870: 7065 2920 3c20 6c65 6e28 696d 6167 652e  pe) < len(image.
-0001b880: 7368 6170 6529 3a0d 0a20 2020 2020 2020  shape):..       
-0001b890: 2020 2020 2075 7064 6174 655f 6d61 736b       update_mask
-0001b8a0: 203d 206e 702e 7a65 726f 7328 0d0a 2020   = np.zeros(..  
-0001b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8c0: 2020 2020 2020 2020 2020 5b0d 0a20 2020            [..   
+0001b340: 735b 2274 7261 636b 5f69 6422 5d0d 0a20  s["track_id"].. 
+0001b350: 2020 2020 2020 2054 6964 203d 2065 6467         Tid = edg
+0001b360: 6573 5f64 6174 6173 6574 5b74 7261 636b  es_dataset[track
+0001b370: 5f69 645d 2e61 7374 7970 6528 2266 6c6f  _id].astype("flo
+0001b380: 6174 2229 0d0a 2020 2020 2020 2020 696e  at")..        in
+0001b390: 6469 6365 7320 3d20 6e70 2e77 6865 7265  dices = np.where
+0001b3a0: 2854 6964 203d 3d20 3029 0d0a 2020 2020  (Tid == 0)..    
+0001b3b0: 2020 2020 6d61 7874 7261 636b 5f69 6420      maxtrack_id 
+0001b3c0: 3d20 6d61 7828 5469 6429 0d0a 2020 2020  = max(Tid)..    
+0001b3d0: 2020 2020 636f 6e64 6974 696f 6e5f 696e      condition_in
+0001b3e0: 6469 6365 7320 3d20 6564 6765 735f 6461  dices = edges_da
+0001b3f0: 7461 7365 745f 696e 6465 785b 696e 6469  taset_index[indi
+0001b400: 6365 735d 0d0a 2020 2020 2020 2020 5469  ces]..        Ti
+0001b410: 645b 636f 6e64 6974 696f 6e5f 696e 6469  d[condition_indi
+0001b420: 6365 735d 203d 206d 6178 7472 6163 6b5f  ces] = maxtrack_
+0001b430: 6964 202b 2031 0d0a 2020 2020 2020 2020  id + 1..        
+0001b440: 416c 6c45 6467 6573 5661 6c75 6573 5b74  AllEdgesValues[t
+0001b450: 7261 636b 5f69 645d 203d 2054 6964 0d0a  rack_id] = Tid..
+0001b460: 0d0a 2020 2020 2020 2020 666f 7220 6b20  ..        for k 
+0001b470: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
+0001b480: 735f 6564 6765 735f 6b65 7973 2e76 616c  s_edges_keys.val
+0001b490: 7565 7328 293a 0d0a 0d0a 2020 2020 2020  ues():....      
+0001b4a0: 2020 2020 2020 6966 206b 2021 3d20 7472        if k != tr
+0001b4b0: 6163 6b5f 6964 3a0d 0a20 2020 2020 2020  ack_id:..       
+0001b4c0: 2020 2020 2020 2020 2078 203d 2065 6467           x = edg
+0001b4d0: 6573 5f64 6174 6173 6574 5b6b 5d2e 6173  es_dataset[k].as
+0001b4e0: 7479 7065 2822 666c 6f61 7422 290d 0a0d  type("float")...
+0001b4f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b500: 2041 6c6c 4564 6765 7356 616c 7565 735b   AllEdgesValues[
+0001b510: 6b5d 203d 2078 2020 200d 0a20 2020 2020  k] = x   ..     
+0001b520: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
+0001b530: 7475 726e 2041 6c6c 4564 6765 7356 616c  turn AllEdgesVal
+0001b540: 7565 7320 2020 0d0a 2020 2020 0d0a 2020  ues   ..    ..  
+0001b550: 2020 2020 200d 0a20 2020 200d 0a64 6566       ..    ..def
+0001b560: 2073 6361 6c65 5f76 616c 7565 2878 2c20   scale_value(x, 
+0001b570: 7363 616c 6520 3d20 3235 3520 2a20 3235  scale = 255 * 25
+0001b580: 3529 3a0d 0a0d 0a0d 0a20 2020 2020 7265  5):......     re
+0001b590: 7475 726e 2078 202a 2073 6361 6c65 2020  turn x * scale  
+0001b5a0: 200d 0a20 2020 200d 0a0d 0a0d 0a64 6566   ..    ......def
+0001b5b0: 2070 726f 625f 7369 676d 6f69 6428 7829   prob_sigmoid(x)
+0001b5c0: 3a0d 0a20 2020 2072 6574 7572 6e20 3120  :..    return 1 
+0001b5d0: 2d20 6d61 7468 2e65 7870 282d 7829 0d0a  - math.exp(-x)..
+0001b5e0: 0d0a 0d0a 6465 6620 616e 6775 6c61 725f  ....def angular_
+0001b5f0: 6368 616e 6765 2876 6563 5f30 2c20 7665  change(vec_0, ve
+0001b600: 635f 3129 3a0d 0a20 2020 2020 2020 200d  c_1):..        .
+0001b610: 0a20 2020 2020 2020 2076 6563 5f30 203d  .        vec_0 =
+0001b620: 2076 6563 5f30 202f 206e 702e 6c69 6e61   vec_0 / np.lina
+0001b630: 6c67 2e6e 6f72 6d28 7665 635f 3029 0d0a  lg.norm(vec_0)..
+0001b640: 2020 2020 2020 2020 7665 635f 3120 3d20          vec_1 = 
+0001b650: 7665 635f 3120 2f20 6e70 2e6c 696e 616c  vec_1 / np.linal
+0001b660: 672e 6e6f 726d 2876 6563 5f31 290d 0a20  g.norm(vec_1).. 
+0001b670: 2020 2020 2020 2061 6e67 6c65 203d 206e         angle = n
+0001b680: 702e 6172 6363 6f73 286e 702e 636c 6970  p.arccos(np.clip
+0001b690: 286e 702e 646f 7428 7665 635f 302c 2076  (np.dot(vec_0, v
+0001b6a0: 6563 5f31 292c 202d 312e 302c 2031 2e30  ec_1), -1.0, 1.0
+0001b6b0: 2929 0d0a 2020 2020 2020 2020 616e 676c  ))..        angl
+0001b6c0: 6520 3d20 616e 676c 6520 2a20 3138 3020  e = angle * 180 
+0001b6d0: 2f20 6e70 2e70 690d 0a20 2020 2020 2020  / np.pi..       
+0001b6e0: 2072 6574 7572 6e20 616e 676c 650d 0a20   return angle.. 
+0001b6f0: 2020 2020 0d0a 0d0a 6465 6620 6576 616c      ....def eval
+0001b700: 5f62 6f6f 6c28 7661 6c75 6529 3a0d 0a20  _bool(value):.. 
+0001b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b720: 200d 0a20 2020 2020 2020 2069 6620 7661   ..        if va
+0001b730: 6c75 6520 203d 3d20 2754 7275 6527 3a20  lue  == 'True': 
+0001b740: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b750: 2020 6469 765f 6b65 7920 3d20 5472 7565    div_key = True
+0001b760: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+0001b770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b780: 2064 6976 5f6b 6579 203d 2046 616c 7365   div_key = False
+0001b790: 200d 0a0d 0a20 2020 2020 2020 2072 6574   ....        ret
+0001b7a0: 7572 6e20 6469 765f 6b65 7920 2020 2020  urn div_key     
+0001b7b0: 2020 2020 2020 2020 2020 200d 0a0d 0a64             ....d
+0001b7c0: 6566 2063 6865 636b 5f61 6e64 5f75 7064  ef check_and_upd
+0001b7d0: 6174 655f 6d61 736b 286d 6173 6b2c 696d  ate_mask(mask,im
+0001b7e0: 6167 6529 3a0d 0a20 2020 2020 2020 0d0a  age):..       ..
+0001b7f0: 2020 2020 2020 2020 6966 206c 656e 286d          if len(m
+0001b800: 6173 6b2e 7368 6170 6529 203c 206c 656e  ask.shape) < len
+0001b810: 2869 6d61 6765 2e73 6861 7065 293a 0d0a  (image.shape):..
+0001b820: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+0001b830: 7465 5f6d 6173 6b20 3d20 6e70 2e7a 6572  te_mask = np.zer
+0001b840: 6f73 280d 0a20 2020 2020 2020 2020 2020  os(..           
+0001b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b860: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
+0001b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b880: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
+0001b890: 305d 2c0d 0a20 2020 2020 2020 2020 2020  0],..           
+0001b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b8b0: 2020 2020 2069 6d61 6765 2e73 6861 7065       image.shape
+0001b8c0: 5b31 5d2c 0d0a 2020 2020 2020 2020 2020  [1],..          
 0001b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8e0: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
-0001b8f0: 6765 2e73 6861 7065 5b30 5d2c 0d0a 2020  ge.shape[0],..  
+0001b8e0: 2020 2020 2020 696d 6167 652e 7368 6170        image.shap
+0001b8f0: 655b 325d 2c0d 0a20 2020 2020 2020 2020  e[2],..         
 0001b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b910: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0001b920: 6167 652e 7368 6170 655b 315d 2c0d 0a20  age.shape[1],.. 
+0001b910: 2020 2020 2020 2069 6d61 6765 2e73 6861         image.sha
+0001b920: 7065 5b33 5d2c 0d0a 2020 2020 2020 2020  pe[3],..        
 0001b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b940: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001b950: 6d61 6765 2e73 6861 7065 5b32 5d2c 0d0a  mage.shape[2],..
-0001b960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b980: 696d 6167 652e 7368 6170 655b 335d 2c0d  image.shape[3],.
-0001b990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b9a0: 2020 2020 2020 2020 2020 2020 205d 2c20               ], 
-0001b9b0: 6474 7970 653d 2275 696e 7438 220d 0a20  dtype="uint8".. 
-0001b9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b9d0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-0001b9e0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0001b9f0: 616e 6765 2830 2c20 7570 6461 7465 5f6d  ange(0, update_m
-0001ba00: 6173 6b2e 7368 6170 655b 305d 293a 0d0a  ask.shape[0]):..
-0001ba10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ba20: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
-0001ba30: 2c20 7570 6461 7465 5f6d 6173 6b2e 7368  , update_mask.sh
-0001ba40: 6170 655b 315d 293a 0d0a 0d0a 2020 2020  ape[1]):....    
-0001ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ba60: 7570 6461 7465 5f6d 6173 6b5b 692c 206a  update_mask[i, j
-0001ba70: 2c20 3a2c 203a 5d20 3d20 6d61 736b 5b69  , :, :] = mask[i
-0001ba80: 2c20 3a2c 203a 5d0d 0a20 2020 2020 2020  , :, :]..       
-0001ba90: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0001baa0: 2020 2020 2020 2020 7570 6461 7465 5f6d          update_m
-0001bab0: 6173 6b20 3d20 6d61 736b 0d0a 0d0a 2020  ask = mask....  
-0001bac0: 2020 2020 2020 7265 7475 726e 2075 7064        return upd
-0001bad0: 6174 655f 6d61 736b 2020 2020 2020 2020  ate_mask        
-0001bae0: 0d0a 2020 2020 2020 200d 0a              ..       ..
+0001b940: 2020 2020 5d2c 2064 7479 7065 3d22 7569      ], dtype="ui
+0001b950: 6e74 3822 0d0a 2020 2020 2020 2020 2020  nt8"..          
+0001b960: 2020 2020 2020 2020 2020 2020 2020 290d                ).
+0001b970: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0001b980: 2069 2069 6e20 7261 6e67 6528 302c 2075   i in range(0, u
+0001b990: 7064 6174 655f 6d61 736b 2e73 6861 7065  pdate_mask.shape
+0001b9a0: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
+0001b9b0: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
+0001b9c0: 7261 6e67 6528 302c 2075 7064 6174 655f  range(0, update_
+0001b9d0: 6d61 736b 2e73 6861 7065 5b31 5d29 3a0d  mask.shape[1]):.
+0001b9e0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001b9f0: 2020 2020 2020 2075 7064 6174 655f 6d61         update_ma
+0001ba00: 736b 5b69 2c20 6a2c 203a 2c20 3a5d 203d  sk[i, j, :, :] =
+0001ba10: 206d 6173 6b5b 692c 203a 2c20 3a5d 0d0a   mask[i, :, :]..
+0001ba20: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
+0001ba30: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+0001ba40: 7064 6174 655f 6d61 736b 203d 206d 6173  pdate_mask = mas
+0001ba50: 6b0d 0a0d 0a20 2020 2020 2020 2072 6574  k....        ret
+0001ba60: 7572 6e20 7570 6461 7465 5f6d 6173 6b20  urn update_mask 
+0001ba70: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001ba80: 0d0a                                     ..
```

### Comparing `napatrackmater-3.8.8/napatrackmater/Trackvector.py` & `napatrackmater-3.8.9/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.8/napatrackmater/__init__.py` & `napatrackmater-3.8.9/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.8/napatrackmater/clustering.py` & `napatrackmater-3.8.9/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.8/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.8.9/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.8/napatrackmater/fate_mapping.py` & `napatrackmater-3.8.9/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.8/napatrackmater/pretrained.py` & `napatrackmater-3.8.9/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.8/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.8.9/napatrackmater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.8.8
+Version: 3.8.9
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.8.8/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.8.9/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.8/setup.py` & `napatrackmater-3.8.9/setup.py`

 * *Files identical despite different names*

