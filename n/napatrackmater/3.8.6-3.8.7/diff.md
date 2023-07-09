# Comparing `tmp/napatrackmater-3.8.6.tar.gz` & `tmp/napatrackmater-3.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napatrackmater-3.8.6.tar", last modified: Sat Jul  8 14:46:43 2023, max compression
+gzip compressed data, was "napatrackmater-3.8.7.tar", last modified: Sun Jul  9 20:44:21 2023, max compression
```

## Comparing `napatrackmater-3.8.6.tar` & `napatrackmater-3.8.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-08 14:46:43.778390 napatrackmater-3.8.6/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.8.6/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-08 14:46:43.774301 napatrackmater-3.8.6/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.8.6/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-08 14:46:43.578786 napatrackmater-3.8.6/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.8.6/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.8.6/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   112940 2023-07-08 14:17:00.000000 napatrackmater-3.8.6/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.8.6/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.8.6/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    14304 2023-07-08 08:48:33.000000 napatrackmater-3.8.6/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.8.6/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.8.6/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.8.6/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-08 14:46:07.000000 napatrackmater-3.8.6/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-08 14:46:43.743924 napatrackmater-3.8.6/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-08 14:46:42.000000 napatrackmater-3.8.6/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-07-08 14:46:43.000000 napatrackmater-3.8.6/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-08 14:46:42.000000 napatrackmater-3.8.6/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-07-08 14:46:42.000000 napatrackmater-3.8.6/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-07-08 14:46:42.000000 napatrackmater-3.8.6/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-07-08 14:46:42.000000 napatrackmater-3.8.6/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-08 14:46:43.779774 napatrackmater-3.8.6/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1410 2023-07-03 08:06:08.000000 napatrackmater-3.8.6/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 20:44:21.718738 napatrackmater-3.8.7/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.8.7/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-09 20:44:21.714128 napatrackmater-3.8.7/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.8.7/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 20:44:21.279941 napatrackmater-3.8.7/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.8.7/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.8.7/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   113135 2023-07-09 20:43:25.000000 napatrackmater-3.8.7/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16426 2023-06-15 20:52:31.000000 napatrackmater-3.8.7/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.8.7/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    14304 2023-07-08 08:48:33.000000 napatrackmater-3.8.7/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.8.7/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.8.7/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.8.7/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-07-09 20:43:32.000000 napatrackmater-3.8.7/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-07-09 20:44:21.656952 napatrackmater-3.8.7/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-07-09 20:44:20.000000 napatrackmater-3.8.7/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-07-09 20:44:20.000000 napatrackmater-3.8.7/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-07-09 20:44:20.000000 napatrackmater-3.8.7/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-07-09 20:44:20.000000 napatrackmater-3.8.7/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-07-09 20:44:20.000000 napatrackmater-3.8.7/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-07-09 20:44:20.000000 napatrackmater-3.8.7/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-07-09 20:44:21.725269 napatrackmater-3.8.7/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1410 2023-07-03 08:06:08.000000 napatrackmater-3.8.7/setup.py
```

### Comparing `napatrackmater-3.8.6/LICENSE` & `napatrackmater-3.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.6/PKG-INFO` & `napatrackmater-3.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.8.6
+Version: 3.8.7
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.8.6/README.md` & `napatrackmater-3.8.7/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.6/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.8.7/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.6/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.8.7/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.6/napatrackmater/Trackmate.py` & `napatrackmater-3.8.7/napatrackmater/Trackmate.py`

 * *Files 1% similar despite different names*

```diff
@@ -6309,751 +6309,763 @@
 00018a40: 286d 6974 6f74 6963 5f64 6973 705f 7829  (mitotic_disp_x)
 00018a50: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
 00018a60: 2020 2020 2020 2073 656c 662e 6d69 746f         self.mito
 00018a70: 7469 635f 7661 725f 6469 7370 5f78 2e61  tic_var_disp_x.a
 00018a80: 7070 656e 6428 6e70 2e73 7464 286d 6974  ppend(np.std(mit
 00018a90: 6f74 6963 5f64 6973 705f 7829 290d 0a0d  otic_disp_x))...
 00018aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018ab0: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00018ac0: 635f 6d65 616e 5f72 6164 6975 732e 6170  c_mean_radius.ap
-00018ad0: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-00018ae0: 6f74 6963 5f72 6164 6975 7329 290d 0a20  otic_radius)).. 
-00018af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b00: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00018b10: 7661 725f 7261 6469 7573 2e61 7070 656e  var_radius.appen
-00018b20: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
-00018b30: 5f72 6164 6975 7329 290d 0a20 2020 2020  _radius))..     
-00018b40: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00018b50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018b60: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00018b70: 635f 6d65 616e 5f73 7065 6564 2e61 7070  c_mean_speed.app
-00018b80: 656e 6428 6e70 2e6d 6561 6e28 6d69 746f  end(np.mean(mito
-00018b90: 7469 635f 7370 6565 6429 290d 0a20 2020  tic_speed))..   
-00018ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018bb0: 2073 656c 662e 6d69 746f 7469 635f 7661   self.mitotic_va
-00018bc0: 725f 7370 6565 642e 6170 7065 6e64 286e  r_speed.append(n
-00018bd0: 702e 7374 6428 6d69 746f 7469 635f 7370  p.std(mitotic_sp
-00018be0: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
-00018bf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018c00: 662e 6d69 746f 7469 635f 6d65 616e 5f61  f.mitotic_mean_a
-00018c10: 6363 2e61 7070 656e 6428 6e70 2e6d 6561  cc.append(np.mea
-00018c20: 6e28 6d69 746f 7469 635f 6163 6329 290d  n(mitotic_acc)).
-00018c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018c40: 2020 2020 2073 656c 662e 6d69 746f 7469       self.mitoti
-00018c50: 635f 7661 725f 6163 632e 6170 7065 6e64  c_var_acc.append
-00018c60: 286e 702e 7374 6428 6d69 746f 7469 635f  (np.std(mitotic_
-00018c70: 6163 6329 290d 0a0d 0a20 2020 2020 2020  acc))....       
-00018c80: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018c90: 662e 6d69 746f 7469 635f 6d65 616e 5f64  f.mitotic_mean_d
-00018ca0: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00018cb0: 652e 6170 7065 6e64 286e 702e 6d65 616e  e.append(np.mean
-00018cc0: 286d 6974 6f74 6963 5f64 6972 6563 7469  (mitotic_directi
-00018cd0: 6f6e 616c 5f63 6861 6e67 6529 290d 0a20  onal_change)).. 
-00018ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cf0: 2020 2073 656c 662e 6d69 746f 7469 635f     self.mitotic_
-00018d00: 7661 725f 6469 7265 6374 696f 6e61 6c5f  var_directional_
-00018d10: 6368 616e 6765 2e61 7070 656e 6428 6e70  change.append(np
-00018d20: 2e73 7464 286d 6974 6f74 6963 5f64 6972  .std(mitotic_dir
-00018d30: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
-00018d40: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00018d50: 2020 2020 2020 2020 2073 656c 662e 6d69           self.mi
-00018d60: 746f 7469 635f 6d65 616e 5f64 6973 7461  totic_mean_dista
-00018d70: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00018d80: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
-00018d90: 6f74 6963 5f64 6973 7461 6e63 655f 6365  otic_distance_ce
-00018da0: 6c6c 5f6d 6173 6b29 290d 0a20 2020 2020  ll_mask))..     
-00018db0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00018dc0: 656c 662e 6d69 746f 7469 635f 7661 725f  elf.mitotic_var_
-00018dd0: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00018de0: 736b 2e61 7070 656e 6428 6e70 2e73 7464  sk.append(np.std
-00018df0: 286d 6974 6f74 6963 5f64 6973 7461 6e63  (mitotic_distanc
-00018e00: 655f 6365 6c6c 5f6d 6173 6b29 290d 0a0d  e_cell_mask))...
-00018e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018e20: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-00018e30: 746f 7469 635f 6d65 616e 5f64 6973 705f  totic_mean_disp_
-00018e40: 7a2e 6170 7065 6e64 286e 702e 6d65 616e  z.append(np.mean
-00018e50: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-00018e60: 705f 7a29 290d 0a20 2020 2020 2020 2020  p_z))..         
-00018e70: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00018e80: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-00018e90: 6469 7370 5f7a 2e61 7070 656e 6428 6e70  disp_z.append(np
-00018ea0: 2e73 7464 286e 6f6e 5f6d 6974 6f74 6963  .std(non_mitotic
-00018eb0: 5f64 6973 705f 7a29 290d 0a0d 0a20 2020  _disp_z))....   
-00018ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ed0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
-00018ee0: 635f 6d65 616e 5f64 6973 705f 792e 6170  c_mean_disp_y.ap
-00018ef0: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
-00018f00: 5f6d 6974 6f74 6963 5f64 6973 705f 7929  _mitotic_disp_y)
-00018f10: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018f20: 2020 2020 2020 2073 656c 662e 6e6f 6e5f         self.non_
-00018f30: 6d69 746f 7469 635f 7661 725f 6469 7370  mitotic_var_disp
-00018f40: 5f79 2e61 7070 656e 6428 6e70 2e73 7464  _y.append(np.std
-00018f50: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6973  (non_mitotic_dis
-00018f60: 705f 7929 290d 0a0d 0a20 2020 2020 2020  p_y))....       
-00018f70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00018f80: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00018f90: 616e 5f64 6973 705f 782e 6170 7065 6e64  an_disp_x.append
-00018fa0: 286e 702e 6d65 616e 286e 6f6e 5f6d 6974  (np.mean(non_mit
-00018fb0: 6f74 6963 5f64 6973 705f 7829 290d 0a20  otic_disp_x)).. 
-00018fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018fd0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
-00018fe0: 7469 635f 7661 725f 6469 7370 5f78 2e61  tic_var_disp_x.a
-00018ff0: 7070 656e 6428 6e70 2e73 7464 286e 6f6e  ppend(np.std(non
-00019000: 5f6d 6974 6f74 6963 5f64 6973 705f 7829  _mitotic_disp_x)
-00019010: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-00019020: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00019030: 6e5f 6d69 746f 7469 635f 6d65 616e 5f72  n_mitotic_mean_r
-00019040: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-00019050: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-00019060: 5f72 6164 6975 7329 290d 0a20 2020 2020  _radius))..     
-00019070: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00019080: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
-00019090: 7661 725f 7261 6469 7573 2e61 7070 656e  var_radius.appen
-000190a0: 6428 6e70 2e73 7464 286e 6f6e 5f6d 6974  d(np.std(non_mit
-000190b0: 6f74 6963 5f72 6164 6975 7329 290d 0a0d  otic_radius))...
-000190c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000190d0: 2020 2020 2073 656c 662e 6e6f 6e5f 6d69       self.non_mi
-000190e0: 746f 7469 635f 6d65 616e 5f73 7065 6564  totic_mean_speed
-000190f0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00019100: 6e6f 6e5f 6d69 746f 7469 635f 7370 6565  non_mitotic_spee
-00019110: 6429 290d 0a20 2020 2020 2020 2020 2020  d))..           
-00019120: 2020 2020 2020 2020 2073 656c 662e 6e6f           self.no
-00019130: 6e5f 6d69 746f 7469 635f 7661 725f 7370  n_mitotic_var_sp
-00019140: 6565 642e 6170 7065 6e64 286e 702e 7374  eed.append(np.st
-00019150: 6428 6e6f 6e5f 6d69 746f 7469 635f 7370  d(non_mitotic_sp
-00019160: 6565 6429 290d 0a0d 0a20 2020 2020 2020  eed))....       
-00019170: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019180: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00019190: 616e 5f61 6363 2e61 7070 656e 6428 6e70  an_acc.append(np
-000191a0: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
-000191b0: 635f 6163 6329 290d 0a20 2020 2020 2020  c_acc))..       
-000191c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000191d0: 662e 6e6f 6e5f 6d69 746f 7469 635f 7661  f.non_mitotic_va
-000191e0: 725f 6163 632e 6170 7065 6e64 286e 702e  r_acc.append(np.
-000191f0: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
-00019200: 6163 6329 290d 0a0d 0a20 2020 2020 2020  acc))....       
-00019210: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019220: 662e 6e6f 6e5f 6d69 746f 7469 635f 6d65  f.non_mitotic_me
-00019230: 616e 5f64 6972 6563 7469 6f6e 616c 5f63  an_directional_c
-00019240: 6861 6e67 652e 6170 7065 6e64 286e 702e  hange.append(np.
-00019250: 6d65 616e 286e 6f6e 5f6d 6974 6f74 6963  mean(non_mitotic
-00019260: 5f64 6972 6563 7469 6f6e 616c 5f63 6861  _directional_cha
-00019270: 6e67 6529 290d 0a20 2020 2020 2020 2020  nge))..         
-00019280: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00019290: 6e6f 6e5f 6d69 746f 7469 635f 7661 725f  non_mitotic_var_
-000192a0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
-000192b0: 6765 2e61 7070 656e 6428 6e70 2e73 7464  ge.append(np.std
-000192c0: 286e 6f6e 5f6d 6974 6f74 6963 5f64 6972  (non_mitotic_dir
-000192d0: 6563 7469 6f6e 616c 5f63 6861 6e67 6529  ectional_change)
-000192e0: 2920 0d0a 0d0a 2020 2020 2020 2020 2020  ) ....          
-000192f0: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00019300: 6f6e 5f6d 6974 6f74 6963 5f6d 6561 6e5f  on_mitotic_mean_
-00019310: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00019320: 736b 2e61 7070 656e 6428 6e70 2e6d 6561  sk.append(np.mea
-00019330: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
-00019340: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-00019350: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00019360: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
-00019370: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
-00019380: 7461 6e63 655f 6365 6c6c 5f6d 6173 6b2e  tance_cell_mask.
-00019390: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
-000193a0: 6e5f 6d69 746f 7469 635f 6469 7374 616e  n_mitotic_distan
-000193b0: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
-000193c0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-000193d0: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-000193e0: 5f6d 6561 6e5f 6469 7370 5f7a 2e61 7070  _mean_disp_z.app
-000193f0: 656e 6428 6e70 2e6d 6561 6e28 616c 6c5f  end(np.mean(all_
-00019400: 6469 7370 5f7a 2929 0d0a 2020 2020 2020  disp_z))..      
-00019410: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019420: 6c66 2e61 6c6c 5f76 6172 5f64 6973 705f  lf.all_var_disp_
-00019430: 7a2e 6170 7065 6e64 286e 702e 7374 6428  z.append(np.std(
-00019440: 616c 6c5f 6469 7370 5f7a 2929 0d0a 0d0a  all_disp_z))....
-00019450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019460: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00019470: 6e5f 6469 7370 5f79 2e61 7070 656e 6428  n_disp_y.append(
-00019480: 6e70 2e6d 6561 6e28 616c 6c5f 6469 7370  np.mean(all_disp
-00019490: 5f79 2929 0d0a 2020 2020 2020 2020 2020  _y))..          
-000194a0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-000194b0: 6c6c 5f76 6172 5f64 6973 705f 792e 6170  ll_var_disp_y.ap
-000194c0: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
-000194d0: 6469 7370 5f79 2929 0d0a 0d0a 2020 2020  disp_y))....    
-000194e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000194f0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-00019500: 7370 5f78 2e61 7070 656e 6428 6e70 2e6d  sp_x.append(np.m
-00019510: 6561 6e28 616c 6c5f 6469 7370 5f78 2929  ean(all_disp_x))
-00019520: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019530: 2020 2020 2020 7365 6c66 2e61 6c6c 5f76        self.all_v
-00019540: 6172 5f64 6973 705f 782e 6170 7065 6e64  ar_disp_x.append
-00019550: 286e 702e 7374 6428 616c 6c5f 6469 7370  (np.std(all_disp
-00019560: 5f78 2929 0d0a 0d0a 2020 2020 2020 2020  _x))....        
-00019570: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019580: 2e61 6c6c 5f6d 6561 6e5f 7261 6469 7573  .all_mean_radius
-00019590: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-000195a0: 616c 6c5f 7261 6469 7573 2929 0d0a 2020  all_radius))..  
-000195b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195c0: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f72    self.all_var_r
-000195d0: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
-000195e0: 7374 6428 616c 6c5f 7261 6469 7573 2929  std(all_radius))
-000195f0: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-00019600: 2020 2020 2020 2020 7365 6c66 2e61 6c6c          self.all
-00019610: 5f6d 6561 6e5f 7370 6565 642e 6170 7065  _mean_speed.appe
-00019620: 6e64 286e 702e 6d65 616e 2861 6c6c 5f73  nd(np.mean(all_s
-00019630: 7065 6564 2929 0d0a 2020 2020 2020 2020  peed))..        
-00019640: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019650: 2e61 6c6c 5f76 6172 5f73 7065 6564 2e61  .all_var_speed.a
-00019660: 7070 656e 6428 6e70 2e73 7464 2861 6c6c  ppend(np.std(all
-00019670: 5f73 7065 6564 2929 0d0a 0d0a 2020 2020  _speed))....    
-00019680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019690: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6163  self.all_mean_ac
-000196a0: 632e 6170 7065 6e64 286e 702e 6d65 616e  c.append(np.mean
-000196b0: 2861 6c6c 5f61 6363 2929 0d0a 2020 2020  (all_acc))..    
-000196c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000196d0: 7365 6c66 2e61 6c6c 5f76 6172 5f61 6363  self.all_var_acc
-000196e0: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
-000196f0: 6c6c 5f61 6363 2929 0d0a 0d0a 0d0a 0d0a  ll_acc))........
-00019700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019710: 2020 2020 7365 6c66 2e61 6c6c 5f6d 6561      self.all_mea
-00019720: 6e5f 6469 7265 6374 696f 6e61 6c5f 6368  n_directional_ch
-00019730: 616e 6765 2e61 7070 656e 6428 6e70 2e6d  ange.append(np.m
-00019740: 6561 6e28 616c 6c5f 6469 7265 6374 696f  ean(all_directio
-00019750: 6e61 6c5f 6368 616e 6765 2929 0d0a 2020  nal_change))..  
-00019760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019770: 2020 7365 6c66 2e61 6c6c 5f76 6172 5f64    self.all_var_d
-00019780: 6972 6563 7469 6f6e 616c 5f63 6861 6e67  irectional_chang
-00019790: 652e 6170 7065 6e64 286e 702e 7374 6428  e.append(np.std(
-000197a0: 616c 6c5f 6469 7265 6374 696f 6e61 6c5f  all_directional_
-000197b0: 6368 616e 6765 2929 0d0a 0d0a 2020 2020  change))....    
-000197c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197d0: 7365 6c66 2e61 6c6c 5f6d 6561 6e5f 6469  self.all_mean_di
-000197e0: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
-000197f0: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
-00019800: 616c 6c5f 6469 7374 616e 6365 5f63 656c  all_distance_cel
-00019810: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
-00019820: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019830: 6c66 2e61 6c6c 5f76 6172 5f64 6973 7461  lf.all_var_dista
-00019840: 6e63 655f 6365 6c6c 5f6d 6173 6b2e 6170  nce_cell_mask.ap
-00019850: 7065 6e64 286e 702e 7374 6428 616c 6c5f  pend(np.std(all_
-00019860: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
-00019870: 736b 2929 0d0a 2020 2020 2020 2020 2020  sk))..          
+00018ab0: 2020 2020 206d 6173 6b20 3d20 6d69 746f       mask = mito
+00018ac0: 7469 635f 7261 6469 7573 203d 3d20 4e6f  tic_radius == No
+00018ad0: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
+00018ae0: 2020 2020 2020 2020 7365 6c66 2e6d 6974          self.mit
+00018af0: 6f74 6963 5f6d 6561 6e5f 7261 6469 7573  otic_mean_radius
+00018b00: 2e61 7070 656e 6428 6e70 2e6d 6561 6e28  .append(np.mean(
+00018b10: 6d69 746f 7469 635f 7261 6469 7573 5b7e  mitotic_radius[~
+00018b20: 6d61 736b 5d29 290d 0a20 2020 2020 2020  mask]))..       
+00018b30: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018b40: 662e 6d69 746f 7469 635f 7661 725f 7261  f.mitotic_var_ra
+00018b50: 6469 7573 2e61 7070 656e 6428 6e70 2e73  dius.append(np.s
+00018b60: 7464 286d 6974 6f74 6963 5f72 6164 6975  td(mitotic_radiu
+00018b70: 735b 7e6d 6173 6b5d 2929 0d0a 2020 2020  s[~mask]))..    
+00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018ba0: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00018bb0: 6963 5f6d 6561 6e5f 7370 6565 642e 6170  ic_mean_speed.ap
+00018bc0: 7065 6e64 286e 702e 6d65 616e 286d 6974  pend(np.mean(mit
+00018bd0: 6f74 6963 5f73 7065 6564 2929 0d0a 2020  otic_speed))..  
+00018be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bf0: 2020 7365 6c66 2e6d 6974 6f74 6963 5f76    self.mitotic_v
+00018c00: 6172 5f73 7065 6564 2e61 7070 656e 6428  ar_speed.append(
+00018c10: 6e70 2e73 7464 286d 6974 6f74 6963 5f73  np.std(mitotic_s
+00018c20: 7065 6564 2929 0d0a 0d0a 2020 2020 2020  peed))....      
+00018c30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018c40: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00018c50: 6163 632e 6170 7065 6e64 286e 702e 6d65  acc.append(np.me
+00018c60: 616e 286d 6974 6f74 6963 5f61 6363 2929  an(mitotic_acc))
+00018c70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018c80: 2020 2020 2020 7365 6c66 2e6d 6974 6f74        self.mitot
+00018c90: 6963 5f76 6172 5f61 6363 2e61 7070 656e  ic_var_acc.appen
+00018ca0: 6428 6e70 2e73 7464 286d 6974 6f74 6963  d(np.std(mitotic
+00018cb0: 5f61 6363 2929 0d0a 0d0a 2020 2020 2020  _acc))....      
+00018cc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018cd0: 6c66 2e6d 6974 6f74 6963 5f6d 6561 6e5f  lf.mitotic_mean_
+00018ce0: 6469 7265 6374 696f 6e61 6c5f 6368 616e  directional_chan
+00018cf0: 6765 2e61 7070 656e 6428 6e70 2e6d 6561  ge.append(np.mea
+00018d00: 6e28 6d69 746f 7469 635f 6469 7265 6374  n(mitotic_direct
+00018d10: 696f 6e61 6c5f 6368 616e 6765 2929 0d0a  ional_change))..
+00018d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d30: 2020 2020 7365 6c66 2e6d 6974 6f74 6963      self.mitotic
+00018d40: 5f76 6172 5f64 6972 6563 7469 6f6e 616c  _var_directional
+00018d50: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
+00018d60: 702e 7374 6428 6d69 746f 7469 635f 6469  p.std(mitotic_di
+00018d70: 7265 6374 696f 6e61 6c5f 6368 616e 6765  rectional_change
+00018d80: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00018d90: 2020 2020 2020 2020 2020 7365 6c66 2e6d            self.m
+00018da0: 6974 6f74 6963 5f6d 6561 6e5f 6469 7374  itotic_mean_dist
+00018db0: 616e 6365 5f63 656c 6c5f 6d61 736b 2e61  ance_cell_mask.a
+00018dc0: 7070 656e 6428 6e70 2e6d 6561 6e28 6d69  ppend(np.mean(mi
+00018dd0: 746f 7469 635f 6469 7374 616e 6365 5f63  totic_distance_c
+00018de0: 656c 6c5f 6d61 736b 2929 0d0a 2020 2020  ell_mask))..    
+00018df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018e00: 7365 6c66 2e6d 6974 6f74 6963 5f76 6172  self.mitotic_var
+00018e10: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+00018e20: 6173 6b2e 6170 7065 6e64 286e 702e 7374  ask.append(np.st
+00018e30: 6428 6d69 746f 7469 635f 6469 7374 616e  d(mitotic_distan
+00018e40: 6365 5f63 656c 6c5f 6d61 736b 2929 0d0a  ce_cell_mask))..
+00018e50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00018e60: 2020 2020 2020 7365 6c66 2e6e 6f6e 5f6d        self.non_m
+00018e70: 6974 6f74 6963 5f6d 6561 6e5f 6469 7370  itotic_mean_disp
+00018e80: 5f7a 2e61 7070 656e 6428 6e70 2e6d 6561  _z.append(np.mea
+00018e90: 6e28 6e6f 6e5f 6d69 746f 7469 635f 6469  n(non_mitotic_di
+00018ea0: 7370 5f7a 2929 0d0a 2020 2020 2020 2020  sp_z))..        
+00018eb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018ec0: 2e6e 6f6e 5f6d 6974 6f74 6963 5f76 6172  .non_mitotic_var
+00018ed0: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
+00018ee0: 702e 7374 6428 6e6f 6e5f 6d69 746f 7469  p.std(non_mitoti
+00018ef0: 635f 6469 7370 5f7a 2929 0d0a 0d0a 2020  c_disp_z))....  
+00018f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f10: 2020 7365 6c66 2e6e 6f6e 5f6d 6974 6f74    self.non_mitot
+00018f20: 6963 5f6d 6561 6e5f 6469 7370 5f79 2e61  ic_mean_disp_y.a
+00018f30: 7070 656e 6428 6e70 2e6d 6561 6e28 6e6f  ppend(np.mean(no
+00018f40: 6e5f 6d69 746f 7469 635f 6469 7370 5f79  n_mitotic_disp_y
+00018f50: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00018f60: 2020 2020 2020 2020 7365 6c66 2e6e 6f6e          self.non
+00018f70: 5f6d 6974 6f74 6963 5f76 6172 5f64 6973  _mitotic_var_dis
+00018f80: 705f 792e 6170 7065 6e64 286e 702e 7374  p_y.append(np.st
+00018f90: 6428 6e6f 6e5f 6d69 746f 7469 635f 6469  d(non_mitotic_di
+00018fa0: 7370 5f79 2929 0d0a 0d0a 2020 2020 2020  sp_y))....      
+00018fb0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00018fc0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f6d  lf.non_mitotic_m
+00018fd0: 6561 6e5f 6469 7370 5f78 2e61 7070 656e  ean_disp_x.appen
+00018fe0: 6428 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69  d(np.mean(non_mi
+00018ff0: 746f 7469 635f 6469 7370 5f78 2929 0d0a  totic_disp_x))..
+00019000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019010: 2020 2020 7365 6c66 2e6e 6f6e 5f6d 6974      self.non_mit
+00019020: 6f74 6963 5f76 6172 5f64 6973 705f 782e  otic_var_disp_x.
+00019030: 6170 7065 6e64 286e 702e 7374 6428 6e6f  append(np.std(no
+00019040: 6e5f 6d69 746f 7469 635f 6469 7370 5f78  n_mitotic_disp_x
+00019050: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+00019060: 2020 2020 2020 2020 2020 6d61 736b 203d            mask =
+00019070: 206e 6f6e 5f6d 6974 6f74 6963 5f72 6164   non_mitotic_rad
+00019080: 6975 7320 3d3d 204e 6f6e 650d 0a20 2020  ius == None..   
+00019090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190a0: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+000190b0: 635f 6d65 616e 5f72 6164 6975 732e 6170  c_mean_radius.ap
+000190c0: 7065 6e64 286e 702e 6d65 616e 286e 6f6e  pend(np.mean(non
+000190d0: 5f6d 6974 6f74 6963 5f72 6164 6975 735b  _mitotic_radius[
+000190e0: 7e6d 6173 6b5d 2929 0d0a 2020 2020 2020  ~mask]))..      
+000190f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019100: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00019110: 6172 5f72 6164 6975 732e 6170 7065 6e64  ar_radius.append
+00019120: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
+00019130: 7469 635f 7261 6469 7573 5b7e 6d61 736b  tic_radius[~mask
+00019140: 5d29 290d 0a0d 0a20 2020 2020 2020 2020  ]))....         
+00019150: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019160: 6e6f 6e5f 6d69 746f 7469 635f 6d65 616e  non_mitotic_mean
+00019170: 5f73 7065 6564 2e61 7070 656e 6428 6e70  _speed.append(np
+00019180: 2e6d 6561 6e28 6e6f 6e5f 6d69 746f 7469  .mean(non_mitoti
+00019190: 635f 7370 6565 6429 290d 0a20 2020 2020  c_speed))..     
+000191a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000191b0: 656c 662e 6e6f 6e5f 6d69 746f 7469 635f  elf.non_mitotic_
+000191c0: 7661 725f 7370 6565 642e 6170 7065 6e64  var_speed.append
+000191d0: 286e 702e 7374 6428 6e6f 6e5f 6d69 746f  (np.std(non_mito
+000191e0: 7469 635f 7370 6565 6429 290d 0a0d 0a20  tic_speed)).... 
+000191f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019200: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00019210: 7469 635f 6d65 616e 5f61 6363 2e61 7070  tic_mean_acc.app
+00019220: 656e 6428 6e70 2e6d 6561 6e28 6e6f 6e5f  end(np.mean(non_
+00019230: 6d69 746f 7469 635f 6163 6329 290d 0a20  mitotic_acc)).. 
+00019240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019250: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+00019260: 7469 635f 7661 725f 6163 632e 6170 7065  tic_var_acc.appe
+00019270: 6e64 286e 702e 7374 6428 6e6f 6e5f 6d69  nd(np.std(non_mi
+00019280: 746f 7469 635f 6163 6329 290d 0a0d 0a20  totic_acc)).... 
+00019290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000192a0: 2020 2073 656c 662e 6e6f 6e5f 6d69 746f     self.non_mito
+000192b0: 7469 635f 6d65 616e 5f64 6972 6563 7469  tic_mean_directi
+000192c0: 6f6e 616c 5f63 6861 6e67 652e 6170 7065  onal_change.appe
+000192d0: 6e64 286e 702e 6d65 616e 286e 6f6e 5f6d  nd(np.mean(non_m
+000192e0: 6974 6f74 6963 5f64 6972 6563 7469 6f6e  itotic_direction
+000192f0: 616c 5f63 6861 6e67 6529 290d 0a20 2020  al_change))..   
+00019300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019310: 2073 656c 662e 6e6f 6e5f 6d69 746f 7469   self.non_mitoti
+00019320: 635f 7661 725f 6469 7265 6374 696f 6e61  c_var_directiona
+00019330: 6c5f 6368 616e 6765 2e61 7070 656e 6428  l_change.append(
+00019340: 6e70 2e73 7464 286e 6f6e 5f6d 6974 6f74  np.std(non_mitot
+00019350: 6963 5f64 6972 6563 7469 6f6e 616c 5f63  ic_directional_c
+00019360: 6861 6e67 6529 2920 0d0a 0d0a 2020 2020  hange)) ....    
+00019370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019380: 7365 6c66 2e6e 6f6e 5f6d 6974 6f74 6963  self.non_mitotic
+00019390: 5f6d 6561 6e5f 6469 7374 616e 6365 5f63  _mean_distance_c
+000193a0: 656c 6c5f 6d61 736b 2e61 7070 656e 6428  ell_mask.append(
+000193b0: 6e70 2e6d 6561 6e28 6e6f 6e5f 6d69 746f  np.mean(non_mito
+000193c0: 7469 635f 6469 7374 616e 6365 5f63 656c  tic_distance_cel
+000193d0: 6c5f 6d61 736b 2929 0d0a 2020 2020 2020  l_mask))..      
+000193e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000193f0: 6c66 2e6e 6f6e 5f6d 6974 6f74 6963 5f76  lf.non_mitotic_v
+00019400: 6172 5f64 6973 7461 6e63 655f 6365 6c6c  ar_distance_cell
+00019410: 5f6d 6173 6b2e 6170 7065 6e64 286e 702e  _mask.append(np.
+00019420: 7374 6428 6e6f 6e5f 6d69 746f 7469 635f  std(non_mitotic_
+00019430: 6469 7374 616e 6365 5f63 656c 6c5f 6d61  distance_cell_ma
+00019440: 736b 2929 0d0a 0d0a 0d0a 2020 2020 2020  sk))......      
+00019450: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019460: 6c66 2e61 6c6c 5f6d 6561 6e5f 6469 7370  lf.all_mean_disp
+00019470: 5f7a 2e61 7070 656e 6428 6e70 2e6d 6561  _z.append(np.mea
+00019480: 6e28 616c 6c5f 6469 7370 5f7a 2929 0d0a  n(all_disp_z))..
+00019490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194a0: 2020 2020 7365 6c66 2e61 6c6c 5f76 6172      self.all_var
+000194b0: 5f64 6973 705f 7a2e 6170 7065 6e64 286e  _disp_z.append(n
+000194c0: 702e 7374 6428 616c 6c5f 6469 7370 5f7a  p.std(all_disp_z
+000194d0: 2929 0d0a 0d0a 2020 2020 2020 2020 2020  ))....          
+000194e0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000194f0: 6c6c 5f6d 6561 6e5f 6469 7370 5f79 2e61  ll_mean_disp_y.a
+00019500: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+00019510: 6c5f 6469 7370 5f79 2929 0d0a 2020 2020  l_disp_y))..    
+00019520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019530: 7365 6c66 2e61 6c6c 5f76 6172 5f64 6973  self.all_var_dis
+00019540: 705f 792e 6170 7065 6e64 286e 702e 7374  p_y.append(np.st
+00019550: 6428 616c 6c5f 6469 7370 5f79 2929 0d0a  d(all_disp_y))..
+00019560: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019570: 2020 2020 2020 7365 6c66 2e61 6c6c 5f6d        self.all_m
+00019580: 6561 6e5f 6469 7370 5f78 2e61 7070 656e  ean_disp_x.appen
+00019590: 6428 6e70 2e6d 6561 6e28 616c 6c5f 6469  d(np.mean(all_di
+000195a0: 7370 5f78 2929 0d0a 2020 2020 2020 2020  sp_x))..        
+000195b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000195c0: 2e61 6c6c 5f76 6172 5f64 6973 705f 782e  .all_var_disp_x.
+000195d0: 6170 7065 6e64 286e 702e 7374 6428 616c  append(np.std(al
+000195e0: 6c5f 6469 7370 5f78 2929 0d0a 0d0a 2020  l_disp_x))....  
+000195f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019600: 2020 6d61 736b 203d 2061 6c6c 5f72 6164    mask = all_rad
+00019610: 6975 7320 3d3d 204e 6f6e 650d 0a20 2020  ius == None..   
+00019620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019630: 2073 656c 662e 616c 6c5f 6d65 616e 5f72   self.all_mean_r
+00019640: 6164 6975 732e 6170 7065 6e64 286e 702e  adius.append(np.
+00019650: 6d65 616e 2861 6c6c 5f72 6164 6975 735b  mean(all_radius[
+00019660: 7e6d 6173 6b5d 2929 0d0a 2020 2020 2020  ~mask]))..      
+00019670: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019680: 6c66 2e61 6c6c 5f76 6172 5f72 6164 6975  lf.all_var_radiu
+00019690: 732e 6170 7065 6e64 286e 702e 7374 6428  s.append(np.std(
+000196a0: 616c 6c5f 7261 6469 7573 5b7e 6d61 736b  all_radius[~mask
+000196b0: 5d29 290d 0a0d 0a20 2020 2020 2020 2020  ]))....         
+000196c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000196d0: 616c 6c5f 6d65 616e 5f73 7065 6564 2e61  all_mean_speed.a
+000196e0: 7070 656e 6428 6e70 2e6d 6561 6e28 616c  ppend(np.mean(al
+000196f0: 6c5f 7370 6565 6429 290d 0a20 2020 2020  l_speed))..     
+00019700: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00019710: 656c 662e 616c 6c5f 7661 725f 7370 6565  elf.all_var_spee
+00019720: 642e 6170 7065 6e64 286e 702e 7374 6428  d.append(np.std(
+00019730: 616c 6c5f 7370 6565 6429 290d 0a0d 0a20  all_speed)).... 
+00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019750: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+00019760: 5f61 6363 2e61 7070 656e 6428 6e70 2e6d  _acc.append(np.m
+00019770: 6561 6e28 616c 6c5f 6163 6329 290d 0a20  ean(all_acc)).. 
+00019780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019790: 2020 2073 656c 662e 616c 6c5f 7661 725f     self.all_var_
+000197a0: 6163 632e 6170 7065 6e64 286e 702e 7374  acc.append(np.st
+000197b0: 6428 616c 6c5f 6163 6329 290d 0a0d 0a0d  d(all_acc)).....
+000197c0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+000197d0: 2020 2020 2020 2073 656c 662e 616c 6c5f         self.all_
+000197e0: 6d65 616e 5f64 6972 6563 7469 6f6e 616c  mean_directional
+000197f0: 5f63 6861 6e67 652e 6170 7065 6e64 286e  _change.append(n
+00019800: 702e 6d65 616e 2861 6c6c 5f64 6972 6563  p.mean(all_direc
+00019810: 7469 6f6e 616c 5f63 6861 6e67 6529 290d  tional_change)).
+00019820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019830: 2020 2020 2073 656c 662e 616c 6c5f 7661       self.all_va
+00019840: 725f 6469 7265 6374 696f 6e61 6c5f 6368  r_directional_ch
+00019850: 616e 6765 2e61 7070 656e 6428 6e70 2e73  ange.append(np.s
+00019860: 7464 2861 6c6c 5f64 6972 6563 7469 6f6e  td(all_direction
+00019870: 616c 5f63 6861 6e67 6529 290d 0a0d 0a20  al_change)).... 
 00019880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019890: 2020 0d0a 2020 2020 2020 2020 0d0a 6465    ..        ..de
-000198a0: 6620 626f 756e 6461 7279 5f70 6f69 6e74  f boundary_point
-000198b0: 7328 6d61 736b 2c20 7863 616c 6962 7261  s(mask, xcalibra
-000198c0: 7469 6f6e 2c20 7963 616c 6962 7261 7469  tion, ycalibrati
-000198d0: 6f6e 2c20 7a63 616c 6962 7261 7469 6f6e  on, zcalibration
-000198e0: 293a 0d0a 0d0a 2020 2020 6e64 696d 203d  ):....    ndim =
-000198f0: 206c 656e 286d 6173 6b2e 7368 6170 6529   len(mask.shape)
-00019900: 0d0a 2020 2020 7469 6d65 645f 6d61 736b  ..    timed_mask
-00019910: 203d 207b 7d0d 0a20 2020 206d 6173 6b20   = {}..    mask 
-00019920: 3d20 6d61 736b 203e 2030 0d0a 2020 2020  = mask > 0..    
-00019930: 6d61 736b 203d 206d 6173 6b2e 6173 7479  mask = mask.asty
-00019940: 7065 2827 7569 6e74 3827 290d 0a20 2020  pe('uint8')..   
-00019950: 2023 2059 5820 7368 6170 6564 206f 626a   # YX shaped obj
-00019960: 6563 740d 0a20 2020 2069 6620 6e64 696d  ect..    if ndim
-00019970: 203d 3d20 323a 0d0a 2020 2020 2020 2020   == 2:..        
-00019980: 0d0a 2020 2020 2020 2020 626f 756e 6461  ..        bounda
-00019990: 7279 203d 2066 696e 645f 626f 756e 6461  ry = find_bounda
-000199a0: 7269 6573 286d 6173 6b29 0d0a 2020 2020  ries(mask)..    
-000199b0: 2020 2020 7265 6769 6f6e 6365 6e74 726f      regioncentro
-000199c0: 6964 203d 2028 302c 2920 2b20 636f 6d70  id = (0,) + comp
-000199d0: 7574 655f 6365 6e74 726f 6964 2862 6f75  ute_centroid(bou
-000199e0: 6e64 6172 7929 200d 0a20 2020 2020 2020  ndary) ..       
-000199f0: 2069 6e64 6963 6573 203d 206e 702e 7768   indices = np.wh
-00019a00: 6572 6528 626f 756e 6461 7279 203e 2030  ere(boundary > 0
-00019a10: 290d 0a20 2020 2020 2020 2072 6561 6c5f  )..        real_
-00019a20: 696e 6469 6365 7320 3d20 6e70 2e74 7261  indices = np.tra
-00019a30: 6e73 706f 7365 286e 702e 6173 6172 7261  nspose(np.asarra
-00019a40: 7928 696e 6469 6365 732c 2064 7479 7065  y(indices, dtype
-00019a50: 3d6e 702e 666c 6f61 7433 3229 292e 636f  =np.float32)).co
-00019a60: 7079 2829 0d0a 0d0a 2020 2020 2020 2020  py()....        
-00019a70: 666f 7220 6a20 696e 2072 616e 6765 2830  for j in range(0
-00019a80: 2c20 6c65 6e28 7265 616c 5f69 6e64 6963  , len(real_indic
-00019a90: 6573 2929 3a0d 0a0d 0a20 2020 2020 2020  es)):....       
-00019aa0: 2020 2020 2072 6561 6c5f 696e 6469 6365       real_indice
-00019ab0: 735b 6a5d 5b30 5d20 3d20 7265 616c 5f69  s[j][0] = real_i
-00019ac0: 6e64 6963 6573 5b6a 5d5b 305d 202a 2079  ndices[j][0] * y
-00019ad0: 6361 6c69 6272 6174 696f 6e0d 0a20 2020  calibration..   
-00019ae0: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-00019af0: 6469 6365 735b 6a5d 5b31 5d20 3d20 7265  dices[j][1] = re
-00019b00: 616c 5f69 6e64 6963 6573 5b6a 5d5b 315d  al_indices[j][1]
-00019b10: 202a 2078 6361 6c69 6272 6174 696f 6e0d   * xcalibration.
-00019b20: 0a0d 0a20 2020 2020 2020 2074 7265 6520  ...        tree 
-00019b30: 3d20 7370 6174 6961 6c2e 634b 4454 7265  = spatial.cKDTre
-00019b40: 6528 7265 616c 5f69 6e64 6963 6573 290d  e(real_indices).
-00019b50: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
-00019b60: 6f62 6a65 6374 2063 6f6e 7461 696e 7320  object contains 
-00019b70: 6c69 7374 206f 6620 616c 6c20 7468 6520  list of all the 
-00019b80: 706f 696e 7473 2066 6f72 2061 6c6c 2074  points for all t
-00019b90: 6865 206c 6162 656c 7320 696e 2074 6865  he labels in the
-00019ba0: 204d 6173 6b20 696d 6167 6520 7769 7468   Mask image with
-00019bb0: 2074 6865 206c 6162 656c 2069 6420 616e   the label id an
-00019bc0: 6420 766f 6c75 6d65 206f 6620 6561 6368  d volume of each
-00019bd0: 206c 6162 656c 0d0a 2020 2020 2020 2020   label..        
-00019be0: 7469 6d65 645f 6d61 736b 5b73 7472 2830  timed_mask[str(0
-00019bf0: 295d 203d 205b 7472 6565 2c20 696e 6469  )] = [tree, indi
-00019c00: 6365 732c 2072 6567 696f 6e63 656e 7472  ces, regioncentr
-00019c10: 6f69 645d 0d0a 0d0a 2020 2020 2320 5459  oid]....    # TY
-00019c20: 5820 7368 6170 6564 206f 626a 6563 740d  X shaped object.
-00019c30: 0a20 2020 2069 6620 6e64 696d 203d 3d20  .    if ndim == 
-00019c40: 333a 0d0a 0d0a 0d0a 2020 2020 2020 2020  3:......        
-00019c50: 666f 7220 6920 696e 2074 7164 6d28 7261  for i in tqdm(ra
-00019c60: 6e67 6528 302c 206d 6173 6b2e 7368 6170  nge(0, mask.shap
-00019c70: 655b 305d 2929 3a0d 0a20 2020 2020 2020  e[0])):..       
-00019c80: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00019c90: 2020 2020 2020 2020 2020 2062 6f75 6e64             bound
-00019ca0: 6172 7920 3d20 6669 6e64 5f62 6f75 6e64  ary = find_bound
-00019cb0: 6172 6965 7328 6d61 736b 5b69 2c3a 5d29  aries(mask[i,:])
-00019cc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019cd0: 2020 7265 6769 6f6e 6365 6e74 726f 6964    regioncentroid
-00019ce0: 203d 2028 302c 2920 2b20 636f 6d70 7574   = (0,) + comput
-00019cf0: 655f 6365 6e74 726f 6964 2862 6f75 6e64  e_centroid(bound
-00019d00: 6172 7929 200d 0a20 2020 2020 2020 2020  ary) ..         
-00019d10: 2020 2020 2020 2069 6e64 6963 6573 203d         indices =
-00019d20: 206e 702e 7768 6572 6528 626f 756e 6461   np.where(bounda
-00019d30: 7279 203e 2030 290d 0a20 2020 2020 2020  ry > 0)..       
-00019d40: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
-00019d50: 6469 6365 7320 3d20 6e70 2e74 7261 6e73  dices = np.trans
-00019d60: 706f 7365 286e 702e 6173 6172 7261 7928  pose(np.asarray(
-00019d70: 696e 6469 6365 732c 2064 7479 7065 3d6e  indices, dtype=n
-00019d80: 702e 666c 6f61 7433 3229 292e 636f 7079  p.float32)).copy
-00019d90: 2829 0d0a 0d0a 2020 2020 2020 2020 2020  ()....          
-00019da0: 2020 2020 2020 666f 7220 6a20 696e 2072        for j in r
-00019db0: 616e 6765 2830 2c20 6c65 6e28 7265 616c  ange(0, len(real
-00019dc0: 5f69 6e64 6963 6573 2929 3a0d 0a0d 0a20  _indices)):.... 
-00019dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019de0: 2020 2072 6561 6c5f 696e 6469 6365 735b     real_indices[
-00019df0: 6a5d 5b30 5d20 3d20 7265 616c 5f69 6e64  j][0] = real_ind
-00019e00: 6963 6573 5b6a 5d5b 305d 202a 2079 6361  ices[j][0] * yca
-00019e10: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-00019e20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00019e30: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
-00019e40: 5d20 3d20 7265 616c 5f69 6e64 6963 6573  ] = real_indices
-00019e50: 5b6a 5d5b 315d 202a 2078 6361 6c69 6272  [j][1] * xcalibr
-00019e60: 6174 696f 6e0d 0a0d 0a20 2020 2020 2020  ation....       
-00019e70: 2020 2020 2020 2020 2074 7265 6520 3d20           tree = 
-00019e80: 7370 6174 6961 6c2e 634b 4454 7265 6528  spatial.cKDTree(
-00019e90: 7265 616c 5f69 6e64 6963 6573 290d 0a0d  real_indices)...
-00019ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019eb0: 2074 696d 6564 5f6d 6173 6b5b 7374 7228   timed_mask[str(
-00019ec0: 6929 5d20 3d20 5b74 7265 652c 2069 6e64  i)] = [tree, ind
-00019ed0: 6963 6573 2c20 7265 6769 6f6e 6365 6e74  ices, regioncent
-00019ee0: 726f 6964 5d0d 0a20 2020 2020 2020 2020  roid]..         
-00019ef0: 2020 200d 0a20 2020 2023 2054 5a59 5820     ..    # TZYX 
-00019f00: 7368 6170 6564 206f 626a 6563 740d 0a20  shaped object.. 
-00019f10: 2020 2069 6620 6e64 696d 203d 3d20 343a     if ndim == 4:
-00019f20: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00019f30: 274d 616b 696e 6720 6d61 736b 2069 6e20  'Making mask in 
-00019f40: 3444 2729 0d0a 2020 2020 2020 2020 626f  4D')..        bo
-00019f50: 756e 6461 7279 203d 206e 702e 7a65 726f  undary = np.zero
-00019f60: 7328 0d0a 2020 2020 2020 2020 2020 2020  s(..            
-00019f70: 5b6d 6173 6b2e 7368 6170 655b 305d 2c20  [mask.shape[0], 
-00019f80: 6d61 736b 2e73 6861 7065 5b31 5d2c 206d  mask.shape[1], m
-00019f90: 6173 6b2e 7368 6170 655b 325d 2c20 6d61  ask.shape[2], ma
-00019fa0: 736b 2e73 6861 7065 5b33 5d5d 2c20 6474  sk.shape[3]], dt
-00019fb0: 7970 653d 6e70 2e75 696e 7438 0d0a 2020  ype=np.uint8..  
-00019fc0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00019fd0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00019fe0: 302c 206d 6173 6b2e 7368 6170 655b 305d  0, mask.shape[0]
-00019ff0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0001a000: 0d0a 2020 2020 2020 2020 2020 2020 626f  ..            bo
-0001a010: 756e 6461 7279 5b69 2c3a 5d20 3d20 6669  undary[i,:] = fi
-0001a020: 6e64 5f62 6f75 6e64 6172 6965 7328 6d61  nd_boundaries(ma
-0001a030: 736b 5b69 2c3a 5d29 0d0a 2020 2020 2020  sk[i,:])..      
-0001a040: 2020 2020 2020 7265 6769 6f6e 6365 6e74        regioncent
-0001a050: 726f 6964 203d 2063 6f6d 7075 7465 5f63  roid = compute_c
-0001a060: 656e 7472 6f69 6428 626f 756e 6461 7279  entroid(boundary
-0001a070: 5b69 2c3a 5d29 200d 0a20 2020 2020 2020  [i,:]) ..       
-0001a080: 2020 2020 2069 6e64 6963 6573 203d 206e       indices = n
-0001a090: 702e 7768 6572 6528 626f 756e 6461 7279  p.where(boundary
-0001a0a0: 5b69 2c3a 5d20 3e20 3029 0d0a 2020 2020  [i,:] > 0)..    
-0001a0b0: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
-0001a0c0: 6963 6573 203d 206e 702e 7472 616e 7370  ices = np.transp
-0001a0d0: 6f73 6528 6e70 2e61 7361 7272 6179 2869  ose(np.asarray(i
-0001a0e0: 6e64 6963 6573 2c20 6474 7970 653d 6e70  ndices, dtype=np
-0001a0f0: 2e66 6c6f 6174 3332 2929 2e63 6f70 7928  .float32)).copy(
-0001a100: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
-0001a110: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-0001a120: 302c 206c 656e 2872 6561 6c5f 696e 6469  0, len(real_indi
-0001a130: 6365 7329 293a 0d0a 0d0a 2020 2020 2020  ces)):....      
-0001a140: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0001a150: 616c 5f69 6e64 6963 6573 5b6a 5d5b 305d  al_indices[j][0]
-0001a160: 203d 2072 6561 6c5f 696e 6469 6365 735b   = real_indices[
-0001a170: 6a5d 5b30 5d20 2a20 7a63 616c 6962 7261  j][0] * zcalibra
-0001a180: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-0001a190: 2020 2020 2020 2020 2020 7265 616c 5f69            real_i
-0001a1a0: 6e64 6963 6573 5b6a 5d5b 315d 203d 2072  ndices[j][1] = r
-0001a1b0: 6561 6c5f 696e 6469 6365 735b 6a5d 5b31  eal_indices[j][1
-0001a1c0: 5d20 2a20 7963 616c 6962 7261 7469 6f6e  ] * ycalibration
-0001a1d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a1e0: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
-0001a1f0: 6573 5b6a 5d5b 325d 203d 2072 6561 6c5f  es[j][2] = real_
-0001a200: 696e 6469 6365 735b 6a5d 5b32 5d20 2a20  indices[j][2] * 
-0001a210: 7863 616c 6962 7261 7469 6f6e 0d0a 0d0a  xcalibration....
-0001a220: 2020 2020 2020 2020 2020 2020 7472 6565              tree
-0001a230: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
-0001a240: 6565 2872 6561 6c5f 696e 6469 6365 7329  ee(real_indices)
-0001a250: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-0001a260: 6d65 645f 6d61 736b 5b73 7472 2869 295d  med_mask[str(i)]
-0001a270: 203d 205b 7472 6565 2c20 696e 6469 6365   = [tree, indice
-0001a280: 732c 2072 6567 696f 6e63 656e 7472 6f69  s, regioncentroi
-0001a290: 645d 0d0a 2020 2020 7072 696e 7428 2743  d]..    print('C
-0001a2a0: 6f6d 7075 7465 6420 7468 6520 626f 756e  omputed the boun
-0001a2b0: 6461 7279 2070 6f69 6e74 7327 290d 0a0d  dary points')...
-0001a2c0: 0a20 2020 2072 6574 7572 6e20 7469 6d65  .    return time
-0001a2d0: 645f 6d61 736b 2c20 626f 756e 6461 7279  d_mask, boundary
-0001a2e0: 2020 2020 2020 2020 0d0a 0d0a 6465 6620          ....def 
-0001a2f0: 636f 6d70 7574 655f 6365 6e74 726f 6964  compute_centroid
-0001a300: 2862 696e 6172 795f 696d 6167 6529 3a0d  (binary_image):.
-0001a310: 0a20 2020 2023 2045 6e73 7572 6520 6269  .    # Ensure bi
-0001a320: 6e61 7279 2069 6d61 6765 2069 7320 6120  nary image is a 
-0001a330: 4e75 6d50 7920 6172 7261 790d 0a20 2020  NumPy array..   
-0001a340: 2062 696e 6172 795f 696d 6167 6520 3d20   binary_image = 
-0001a350: 6e70 2e61 7272 6179 2862 696e 6172 795f  np.array(binary_
-0001a360: 696d 6167 6529 0d0a 0d0a 2020 2020 7768  image)....    wh
-0001a370: 6974 655f 7069 7865 6c73 203d 206e 702e  ite_pixels = np.
-0001a380: 7768 6572 6528 6269 6e61 7279 5f69 6d61  where(binary_ima
-0001a390: 6765 203d 3d20 3129 0d0a 2020 2020 6e75  ge == 1)..    nu
-0001a3a0: 6d5f 7069 7865 6c73 203d 206c 656e 2877  m_pixels = len(w
-0001a3b0: 6869 7465 5f70 6978 656c 735b 305d 290d  hite_pixels[0]).
-0001a3c0: 0a0d 0a20 2020 2023 2043 6f6d 7075 7465  ...    # Compute
-0001a3d0: 2074 6865 2063 656e 7472 6f69 6420 6f66   the centroid of
-0001a3e0: 2074 6865 2077 6869 7465 2070 6978 656c   the white pixel
-0001a3f0: 7320 696e 2074 6865 2062 6f75 6e64 6172  s in the boundar
-0001a400: 7920 696d 6167 650d 0a20 2020 2063 656e  y image..    cen
-0001a410: 7472 6f69 6420 3d20 6e70 2e7a 6572 6f73  troid = np.zeros
-0001a420: 2862 696e 6172 795f 696d 6167 652e 6e64  (binary_image.nd
-0001a430: 696d 290d 0a20 2020 2066 6f72 2064 696d  im)..    for dim
-0001a440: 2069 6e20 7261 6e67 6528 6269 6e61 7279   in range(binary
-0001a450: 5f69 6d61 6765 2e6e 6469 6d29 3a0d 0a20  _image.ndim):.. 
-0001a460: 2020 2020 2020 2063 656e 7472 6f69 645b         centroid[
-0001a470: 6469 6d5d 203d 2077 6869 7465 5f70 6978  dim] = white_pix
-0001a480: 656c 735b 6469 6d5d 2e73 756d 2829 202f  els[dim].sum() /
-0001a490: 206e 756d 5f70 6978 656c 730d 0a0d 0a20   num_pixels.... 
-0001a4a0: 2020 2072 6574 7572 6e20 6365 6e74 726f     return centro
-0001a4b0: 6964 0d0a 0d0a 0d0a 0d0a 200d 0a0d 0a64  id........ ....d
-0001a4c0: 6566 2067 6574 5f63 7376 5f64 6174 6128  ef get_csv_data(
-0001a4d0: 6373 7629 3a0d 0a0d 0a20 2020 2020 2020  csv):....       
-0001a4e0: 2064 6174 6173 6574 203d 2070 642e 7265   dataset = pd.re
-0001a4f0: 6164 5f63 7376 280d 0a20 2020 2020 2020  ad_csv(..       
-0001a500: 2020 2020 2063 7376 2c20 6465 6c69 6d69       csv, delimi
-0001a510: 7465 723d 222c 222c 2065 6e63 6f64 696e  ter=",", encodin
-0001a520: 673d 2275 6e69 636f 6465 5f65 7363 6170  g="unicode_escap
-0001a530: 6522 2c20 6c6f 775f 6d65 6d6f 7279 3d46  e", low_memory=F
-0001a540: 616c 7365 0d0a 2020 2020 2020 2020 295b  alse..        )[
-0001a550: 333a 5d0d 0a20 2020 2020 2020 2064 6174  3:]..        dat
-0001a560: 6173 6574 5f69 6e64 6578 203d 2064 6174  aset_index = dat
-0001a570: 6173 6574 2e69 6e64 6578 0d0a 2020 2020  aset.index..    
-0001a580: 2020 2020 7265 7475 726e 2064 6174 6173      return datas
-0001a590: 6574 2c20 6461 7461 7365 745f 696e 6465  et, dataset_inde
-0001a5a0: 780d 0a20 2020 200d 0a64 6566 2067 6574  x..    ..def get
-0001a5b0: 5f73 706f 745f 6461 7461 7365 7428 7370  _spot_dataset(sp
-0001a5c0: 6f74 5f64 6174 6173 6574 2c20 7472 6163  ot_dataset, trac
-0001a5d0: 6b5f 616e 616c 7973 6973 5f73 706f 745f  k_analysis_spot_
-0001a5e0: 6b65 7973 2c20 7863 616c 6962 7261 7469  keys, xcalibrati
-0001a5f0: 6f6e 2c20 7963 616c 6962 7261 7469 6f6e  on, ycalibration
-0001a600: 2c20 7a63 616c 6962 7261 7469 6f6e 2c20  , zcalibration, 
-0001a610: 4174 7472 6962 7574 6542 6f78 6e61 6d65  AttributeBoxname
-0001a620: 2c20 6465 7465 6374 696f 6e63 6861 6e6e  , detectionchann
-0001a630: 656c 293a 0d0a 2020 2020 2020 2020 416c  el):..        Al
-0001a640: 6c56 616c 7565 7320 3d20 7b7d 0d0a 2020  lValues = {}..  
-0001a650: 2020 2020 2020 706f 7369 7820 3d20 7472        posix = tr
-0001a660: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-0001a670: 745f 6b65 7973 5b22 706f 7369 7822 5d0d  t_keys["posix"].
-0001a680: 0a20 2020 2020 2020 2070 6f73 6979 203d  .        posiy =
-0001a690: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
-0001a6a0: 7370 6f74 5f6b 6579 735b 2270 6f73 6979  spot_keys["posiy
-0001a6b0: 225d 0d0a 2020 2020 2020 2020 706f 7369  "]..        posi
-0001a6c0: 7a20 3d20 7472 6163 6b5f 616e 616c 7973  z = track_analys
-0001a6d0: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
-0001a6e0: 7369 7a22 5d0d 0a20 2020 2020 2020 2066  siz"]..        f
-0001a6f0: 7261 6d65 203d 2074 7261 636b 5f61 6e61  rame = track_ana
-0001a700: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-0001a710: 2266 7261 6d65 225d 0d0a 2020 2020 2020  "frame"]..      
-0001a720: 2020 0d0a 2020 2020 2020 2020 4c6f 6361    ..        Loca
-0001a730: 7469 6f6e 5820 3d20 280d 0a20 2020 2020  tionX = (..     
-0001a740: 2020 2020 2020 2073 706f 745f 6461 7461         spot_data
-0001a750: 7365 745b 706f 7369 785d 2e61 7374 7970  set[posix].astyp
-0001a760: 6528 2266 6c6f 6174 2229 202f 2078 6361  e("float") / xca
-0001a770: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-0001a780: 2020 2029 2e61 7374 7970 6528 2269 6e74     ).astype("int
-0001a790: 2229 0d0a 2020 2020 2020 2020 4c6f 6361  ")..        Loca
-0001a7a0: 7469 6f6e 5920 3d20 280d 0a20 2020 2020  tionY = (..     
-0001a7b0: 2020 2020 2020 2073 706f 745f 6461 7461         spot_data
-0001a7c0: 7365 745b 706f 7369 795d 2e61 7374 7970  set[posiy].astyp
-0001a7d0: 6528 2266 6c6f 6174 2229 202f 2079 6361  e("float") / yca
-0001a7e0: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-0001a7f0: 2020 2029 2e61 7374 7970 6528 2269 6e74     ).astype("int
-0001a800: 2229 0d0a 2020 2020 2020 2020 4c6f 6361  ")..        Loca
-0001a810: 7469 6f6e 5a20 3d20 280d 0a20 2020 2020  tionZ = (..     
-0001a820: 2020 2020 2020 2073 706f 745f 6461 7461         spot_data
-0001a830: 7365 745b 706f 7369 7a5d 2e61 7374 7970  set[posiz].astyp
-0001a840: 6528 2266 6c6f 6174 2229 202f 207a 6361  e("float") / zca
-0001a850: 6c69 6272 6174 696f 6e0d 0a20 2020 2020  libration..     
-0001a860: 2020 2029 2e61 7374 7970 6528 2269 6e74     ).astype("int
-0001a870: 2229 0d0a 2020 2020 2020 2020 4c6f 6361  ")..        Loca
-0001a880: 7469 6f6e 5420 3d20 2873 706f 745f 6461  tionT = (spot_da
-0001a890: 7461 7365 745b 6672 616d 655d 2e61 7374  taset[frame].ast
-0001a8a0: 7970 6528 2266 6c6f 6174 2229 292e 6173  ype("float")).as
-0001a8b0: 7479 7065 2822 696e 7422 290d 0a20 2020  type("int")..   
-0001a8c0: 2020 2020 200d 0a0d 0a20 2020 2020 2020       ....       
-0001a8d0: 2069 676e 6f72 655f 7661 6c75 6573 203d   ignore_values =
-0001a8e0: 205b 7472 6163 6b5f 616e 616c 7973 6973   [track_analysis
-0001a8f0: 5f73 706f 745f 6b65 7973 5b22 6d65 616e  _spot_keys["mean
-0001a900: 5f69 6e74 656e 7369 7479 225d 2c74 7261  _intensity"],tra
-0001a910: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
-0001a920: 5f6b 6579 735b 2274 6f74 616c 5f69 6e74  _keys["total_int
-0001a930: 656e 7369 7479 225d 5d0d 0a20 2020 2020  ensity"]]..     
-0001a940: 2020 2066 6f72 2028 6b2c 7629 2069 6e20     for (k,v) in 
-0001a950: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
-0001a960: 706f 745f 6b65 7973 2e69 7465 6d73 2829  pot_keys.items()
-0001a970: 3a0d 0a0d 0a20 2020 2020 2020 2020 2020  :....           
-0001a980: 2020 2020 2069 6620 6465 7465 6374 696f       if detectio
-0001a990: 6e63 6861 6e6e 656c 203d 3d20 313a 0d0a  nchannel == 1:..
-0001a9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a9b0: 2020 2020 2069 6620 6b20 3d3d 2022 6d65       if k == "me
-0001a9c0: 616e 5f69 6e74 656e 7369 7479 5f63 6832  an_intensity_ch2
-0001a9d0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-0001a9e0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-0001a9f0: 616c 7565 203d 2074 7261 636b 5f61 6e61  alue = track_ana
-0001aa00: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
-0001aa10: 226d 6561 6e5f 696e 7465 6e73 6974 7922  "mean_intensity"
-0001aa20: 5d0d 0a20 2020 2020 2020 2020 2020 2020  ]..             
-0001aa30: 2020 2020 2020 2020 2020 2020 2020 416c                Al
-0001aa40: 6c56 616c 7565 735b 7661 6c75 655d 203d  lValues[value] =
-0001aa50: 2073 706f 745f 6461 7461 7365 745b 765d   spot_dataset[v]
-0001aa60: 2e61 7374 7970 6528 2266 6c6f 6174 2229  .astype("float")
-0001aa70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001aa80: 2020 2020 2020 2069 6620 6b20 3d3d 2022         if k == "
-0001aa90: 746f 7461 6c5f 696e 7465 6e73 6974 795f  total_intensity_
-0001aaa0: 6368 3222 3a0d 0a20 2020 2020 2020 2020  ch2":..         
-0001aab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aac0: 2020 7661 6c75 6520 3d20 7472 6163 6b5f    value = track_
-0001aad0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001aae0: 7973 5b22 746f 7461 6c5f 696e 7465 6e73  ys["total_intens
-0001aaf0: 6974 7922 5d0d 0a20 2020 2020 2020 2020  ity"]..         
-0001ab00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab10: 2020 416c 6c56 616c 7565 735b 7661 6c75    AllValues[valu
-0001ab20: 655d 203d 2073 706f 745f 6461 7461 7365  e] = spot_datase
-0001ab30: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
-0001ab40: 6174 2229 2020 2020 2020 200d 0a0d 0a20  at")       .... 
-0001ab50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001ab60: 6620 7620 6e6f 7420 696e 2069 676e 6f72  f v not in ignor
-0001ab70: 655f 7661 6c75 6573 3a0d 0a20 2020 2020  e_values:..     
-0001ab80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ab90: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0001aba0: 2020 2020 2020 2020 2020 2041 6c6c 5661             AllVa
-0001abb0: 6c75 6573 5b76 5d20 3d20 7370 6f74 5f64  lues[v] = spot_d
-0001abc0: 6174 6173 6574 5b76 5d2e 6173 7479 7065  ataset[v].astype
-0001abd0: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
-0001abe0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0001abf0: 0d0a 2020 2020 2020 2020 416c 6c56 616c  ..        AllVal
-0001ac00: 7565 735b 706f 7369 785d 203d 2072 6f75  ues[posix] = rou
-0001ac10: 6e64 284c 6f63 6174 696f 6e58 2c33 290d  nd(LocationX,3).
-0001ac20: 0a20 2020 2020 2020 2041 6c6c 5661 6c75  .        AllValu
-0001ac30: 6573 5b70 6f73 6979 5d20 3d20 726f 756e  es[posiy] = roun
-0001ac40: 6428 4c6f 6361 7469 6f6e 592c 3329 0d0a  d(LocationY,3)..
-0001ac50: 2020 2020 2020 2020 416c 6c56 616c 7565          AllValue
-0001ac60: 735b 706f 7369 7a5d 203d 2072 6f75 6e64  s[posiz] = round
-0001ac70: 284c 6f63 6174 696f 6e5a 2c33 290d 0a20  (LocationZ,3).. 
-0001ac80: 2020 2020 2020 2041 6c6c 5661 6c75 6573         AllValues
-0001ac90: 5b66 7261 6d65 5d20 3d20 726f 756e 6428  [frame] = round(
-0001aca0: 4c6f 6361 7469 6f6e 542c 3329 0d0a 2020  LocationT,3)..  
-0001acb0: 2020 2020 2020 4174 7472 6962 7574 6569        Attributei
-0001acc0: 6473 203d 205b 5d0d 0a20 2020 2020 2020  ds = []..       
-0001acd0: 2041 7474 7269 6275 7465 6964 732e 6170   Attributeids.ap
-0001ace0: 7065 6e64 2841 7474 7269 6275 7465 426f  pend(AttributeBo
-0001acf0: 786e 616d 6529 0d0a 2020 2020 2020 2020  xname)..        
-0001ad00: 666f 7220 6174 7472 6962 7574 656e 616d  for attributenam
-0001ad10: 6520 696e 2041 6c6c 5661 6c75 6573 2e6b  e in AllValues.k
-0001ad20: 6579 7328 293a 0d0a 2020 2020 2020 2020  eys():..        
-0001ad30: 2020 2020 2020 4174 7472 6962 7574 6569        Attributei
-0001ad40: 6473 2e61 7070 656e 6428 6174 7472 6962  ds.append(attrib
-0001ad50: 7574 656e 616d 6529 2020 2020 0d0a 2020  utename)    ..  
-0001ad60: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0001ad70: 2020 2020 0d0a 2020 2020 2020 2020 7265      ..        re
-0001ad80: 7475 726e 2041 7474 7269 6275 7465 6964  turn Attributeid
-0001ad90: 732c 2041 6c6c 5661 6c75 6573 2020 2020  s, AllValues    
-0001ada0: 200d 0a20 2020 200d 0a64 6566 2067 6574   ..    ..def get
-0001adb0: 5f74 7261 636b 5f64 6174 6173 6574 2874  _track_dataset(t
-0001adc0: 7261 636b 5f64 6174 6173 6574 2c20 7472  rack_dataset, tr
-0001add0: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-0001ade0: 745f 6b65 7973 2c20 7472 6163 6b5f 616e  t_keys, track_an
-0001adf0: 616c 7973 6973 5f74 7261 636b 5f6b 6579  alysis_track_key
-0001ae00: 732c 2054 7261 636b 4174 7472 6962 7574  s, TrackAttribut
-0001ae10: 6542 6f78 6e61 6d65 293a 0d0a 0d0a 2020  eBoxname):....  
-0001ae20: 2020 2020 2020 416c 6c54 7261 636b 5661        AllTrackVa
-0001ae30: 6c75 6573 203d 207b 7d0d 0a20 2020 2020  lues = {}..     
-0001ae40: 2020 2074 7261 636b 5f69 6420 3d20 7472     track_id = tr
-0001ae50: 6163 6b5f 616e 616c 7973 6973 5f73 706f  ack_analysis_spo
-0001ae60: 745f 6b65 7973 5b22 7472 6163 6b5f 6964  t_keys["track_id
-0001ae70: 225d 0d0a 2020 2020 2020 2020 5469 6420  "]..        Tid 
-0001ae80: 3d20 7472 6163 6b5f 6461 7461 7365 745b  = track_dataset[
-0001ae90: 7472 6163 6b5f 6964 5d2e 6173 7479 7065  track_id].astype
-0001aea0: 2822 666c 6f61 7422 290d 0a20 2020 2020  ("float")..     
-0001aeb0: 2020 0d0a 2020 2020 2020 2020 416c 6c54    ..        AllT
-0001aec0: 7261 636b 5661 6c75 6573 5b74 7261 636b  rackValues[track
-0001aed0: 5f69 645d 203d 2054 6964 0d0a 2020 2020  _id] = Tid..    
-0001aee0: 2020 0d0a 2020 2020 2020 2020 666f 7220    ..        for 
-0001aef0: 286b 2c20 7629 2069 6e20 7472 6163 6b5f  (k, v) in track_
-0001af00: 616e 616c 7973 6973 5f74 7261 636b 5f6b  analysis_track_k
-0001af10: 6579 732e 6974 656d 7328 293a 0d0a 0d0a  eys.items():....
-0001af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af30: 7820 3d20 7472 6163 6b5f 6461 7461 7365  x = track_datase
-0001af40: 745b 765d 2e61 7374 7970 6528 2266 6c6f  t[v].astype("flo
-0001af50: 6174 2229 0d0a 2020 2020 2020 2020 2020  at")..          
-0001af60: 2020 2020 2020 6d69 6e76 616c 203d 206d        minval = m
-0001af70: 696e 2878 290d 0a20 2020 2020 2020 2020  in(x)..         
-0001af80: 2020 2020 2020 206d 6178 7661 6c20 3d20         maxval = 
-0001af90: 6d61 7828 7829 0d0a 0d0a 2020 2020 2020  max(x)....      
-0001afa0: 2020 2020 2020 2020 2020 6966 206d 696e            if min
-0001afb0: 7661 6c20 3e20 3020 616e 6420 6d61 7876  val > 0 and maxv
-0001afc0: 616c 203c 3d20 313a 0d0a 0d0a 2020 2020  al <= 1:....    
-0001afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001afe0: 7820 3d20 7820 2b20 310d 0a0d 0a20 2020  x = x + 1....   
-0001aff0: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
-0001b000: 5472 6163 6b56 616c 7565 735b 6b5d 203d  TrackValues[k] =
-0001b010: 2072 6f75 6e64 2878 2c20 3329 0d0a 0d0a   round(x, 3)....
-0001b020: 2020 2020 2020 2020 5472 6163 6b41 7474          TrackAtt
-0001b030: 7269 6275 7465 6964 7320 3d20 5b5d 0d0a  ributeids = []..
-0001b040: 2020 2020 2020 2020 5472 6163 6b41 7474          TrackAtt
-0001b050: 7269 6275 7465 6964 732e 6170 7065 6e64  ributeids.append
-0001b060: 2854 7261 636b 4174 7472 6962 7574 6542  (TrackAttributeB
-0001b070: 6f78 6e61 6d65 290d 0a20 2020 2020 2020  oxname)..       
-0001b080: 2066 6f72 2061 7474 7269 6275 7465 6e61   for attributena
-0001b090: 6d65 2069 6e20 7472 6163 6b5f 616e 616c  me in track_anal
-0001b0a0: 7973 6973 5f74 7261 636b 5f6b 6579 732e  ysis_track_keys.
-0001b0b0: 6b65 7973 2829 3a0d 0a20 2020 2020 2020  keys():..       
-0001b0c0: 2020 2020 2054 7261 636b 4174 7472 6962       TrackAttrib
-0001b0d0: 7574 6569 6473 2e61 7070 656e 6428 6174  uteids.append(at
-0001b0e0: 7472 6962 7574 656e 616d 6529 2020 2020  tributename)    
-0001b0f0: 0d0a 2020 2020 0d0a 2020 2020 2020 2020  ..    ..        
-0001b100: 7265 7475 726e 2054 7261 636b 4174 7472  return TrackAttr
-0001b110: 6962 7574 6569 6473 2c20 416c 6c54 7261  ibuteids, AllTra
-0001b120: 636b 5661 6c75 6573 0d0a 2020 2020 0d0a  ckValues..    ..
-0001b130: 6465 6620 6765 745f 6564 6765 735f 6461  def get_edges_da
-0001b140: 7461 7365 7428 6564 6765 735f 6461 7461  taset(edges_data
-0001b150: 7365 742c 2065 6467 6573 5f64 6174 6173  set, edges_datas
-0001b160: 6574 5f69 6e64 6578 2c20 7472 6163 6b5f  et_index, track_
-0001b170: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
-0001b180: 7973 2c20 7472 6163 6b5f 616e 616c 7973  ys, track_analys
-0001b190: 6973 5f65 6467 6573 5f6b 6579 7329 3a0d  is_edges_keys):.
-0001b1a0: 0a0d 0a20 2020 2020 2020 2041 6c6c 4564  ...        AllEd
-0001b1b0: 6765 7356 616c 7565 7320 3d20 7b7d 0d0a  gesValues = {}..
-0001b1c0: 2020 2020 2020 2020 7472 6163 6b5f 6964          track_id
-0001b1d0: 203d 2074 7261 636b 5f61 6e61 6c79 7369   = track_analysi
-0001b1e0: 735f 7370 6f74 5f6b 6579 735b 2274 7261  s_spot_keys["tra
-0001b1f0: 636b 5f69 6422 5d0d 0a20 2020 2020 2020  ck_id"]..       
-0001b200: 2054 6964 203d 2065 6467 6573 5f64 6174   Tid = edges_dat
-0001b210: 6173 6574 5b74 7261 636b 5f69 645d 2e61  aset[track_id].a
-0001b220: 7374 7970 6528 2266 6c6f 6174 2229 0d0a  stype("float")..
-0001b230: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
-0001b240: 3d20 6e70 2e77 6865 7265 2854 6964 203d  = np.where(Tid =
-0001b250: 3d20 3029 0d0a 2020 2020 2020 2020 6d61  = 0)..        ma
-0001b260: 7874 7261 636b 5f69 6420 3d20 6d61 7828  xtrack_id = max(
-0001b270: 5469 6429 0d0a 2020 2020 2020 2020 636f  Tid)..        co
-0001b280: 6e64 6974 696f 6e5f 696e 6469 6365 7320  ndition_indices 
-0001b290: 3d20 6564 6765 735f 6461 7461 7365 745f  = edges_dataset_
-0001b2a0: 696e 6465 785b 696e 6469 6365 735d 0d0a  index[indices]..
-0001b2b0: 2020 2020 2020 2020 5469 645b 636f 6e64          Tid[cond
-0001b2c0: 6974 696f 6e5f 696e 6469 6365 735d 203d  ition_indices] =
-0001b2d0: 206d 6178 7472 6163 6b5f 6964 202b 2031   maxtrack_id + 1
-0001b2e0: 0d0a 2020 2020 2020 2020 416c 6c45 6467  ..        AllEdg
-0001b2f0: 6573 5661 6c75 6573 5b74 7261 636b 5f69  esValues[track_i
-0001b300: 645d 203d 2054 6964 0d0a 0d0a 2020 2020  d] = Tid....    
-0001b310: 2020 2020 666f 7220 6b20 696e 2074 7261      for k in tra
-0001b320: 636b 5f61 6e61 6c79 7369 735f 6564 6765  ck_analysis_edge
-0001b330: 735f 6b65 7973 2e76 616c 7565 7328 293a  s_keys.values():
-0001b340: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
-0001b350: 6966 206b 2021 3d20 7472 6163 6b5f 6964  if k != track_id
-0001b360: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001b370: 2020 2078 203d 2065 6467 6573 5f64 6174     x = edges_dat
-0001b380: 6173 6574 5b6b 5d2e 6173 7479 7065 2822  aset[k].astype("
-0001b390: 666c 6f61 7422 290d 0a0d 0a20 2020 2020  float")....     
-0001b3a0: 2020 2020 2020 2020 2020 2041 6c6c 4564             AllEd
-0001b3b0: 6765 7356 616c 7565 735b 6b5d 203d 2078  gesValues[k] = x
-0001b3c0: 2020 200d 0a20 2020 2020 2020 2020 0d0a     ..         ..
-0001b3d0: 2020 2020 2020 2020 7265 7475 726e 2041          return A
-0001b3e0: 6c6c 4564 6765 7356 616c 7565 7320 2020  llEdgesValues   
-0001b3f0: 0d0a 2020 2020 0d0a 2020 2020 2020 200d  ..    ..       .
-0001b400: 0a20 2020 200d 0a64 6566 2073 6361 6c65  .    ..def scale
-0001b410: 5f76 616c 7565 2878 2c20 7363 616c 6520  _value(x, scale 
-0001b420: 3d20 3235 3520 2a20 3235 3529 3a0d 0a0d  = 255 * 255):...
-0001b430: 0a0d 0a20 2020 2020 7265 7475 726e 2078  ...     return x
-0001b440: 202a 2073 6361 6c65 2020 200d 0a20 2020   * scale   ..   
-0001b450: 200d 0a0d 0a0d 0a64 6566 2070 726f 625f   ......def prob_
-0001b460: 7369 676d 6f69 6428 7829 3a0d 0a20 2020  sigmoid(x):..   
-0001b470: 2072 6574 7572 6e20 3120 2d20 6d61 7468   return 1 - math
-0001b480: 2e65 7870 282d 7829 0d0a 0d0a 0d0a 6465  .exp(-x)......de
-0001b490: 6620 616e 6775 6c61 725f 6368 616e 6765  f angular_change
-0001b4a0: 2876 6563 5f30 2c20 7665 635f 3129 3a0d  (vec_0, vec_1):.
-0001b4b0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-0001b4c0: 2020 2076 6563 5f30 203d 2076 6563 5f30     vec_0 = vec_0
-0001b4d0: 202f 206e 702e 6c69 6e61 6c67 2e6e 6f72   / np.linalg.nor
-0001b4e0: 6d28 7665 635f 3029 0d0a 2020 2020 2020  m(vec_0)..      
-0001b4f0: 2020 7665 635f 3120 3d20 7665 635f 3120    vec_1 = vec_1 
-0001b500: 2f20 6e70 2e6c 696e 616c 672e 6e6f 726d  / np.linalg.norm
-0001b510: 2876 6563 5f31 290d 0a20 2020 2020 2020  (vec_1)..       
-0001b520: 2061 6e67 6c65 203d 206e 702e 6172 6363   angle = np.arcc
-0001b530: 6f73 286e 702e 636c 6970 286e 702e 646f  os(np.clip(np.do
-0001b540: 7428 7665 635f 302c 2076 6563 5f31 292c  t(vec_0, vec_1),
-0001b550: 202d 312e 302c 2031 2e30 2929 0d0a 2020   -1.0, 1.0))..  
-0001b560: 2020 2020 2020 616e 676c 6520 3d20 616e        angle = an
-0001b570: 676c 6520 2a20 3138 3020 2f20 6e70 2e70  gle * 180 / np.p
-0001b580: 690d 0a20 2020 2020 2020 2072 6574 7572  i..        retur
-0001b590: 6e20 616e 676c 650d 0a20 2020 2020 0d0a  n angle..     ..
-0001b5a0: 0d0a 6465 6620 6576 616c 5f62 6f6f 6c28  ..def eval_bool(
-0001b5b0: 7661 6c75 6529 3a0d 0a20 2020 2020 2020  value):..       
-0001b5c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0001b5d0: 2020 2020 2069 6620 7661 6c75 6520 203d       if value  =
-0001b5e0: 3d20 2754 7275 6527 3a20 0d0a 2020 2020  = 'True': ..    
-0001b5f0: 2020 2020 2020 2020 2020 2020 6469 765f              div_
-0001b600: 6b65 7920 3d20 5472 7565 0d0a 2020 2020  key = True..    
-0001b610: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0001b620: 2020 2020 2020 2020 2020 2064 6976 5f6b             div_k
-0001b630: 6579 203d 2046 616c 7365 200d 0a0d 0a20  ey = False .... 
-0001b640: 2020 2020 2020 2072 6574 7572 6e20 6469         return di
-0001b650: 765f 6b65 7920 2020 2020 2020 2020 2020  v_key           
-0001b660: 2020 2020 200d 0a0d 0a64 6566 2063 6865       ....def che
-0001b670: 636b 5f61 6e64 5f75 7064 6174 655f 6d61  ck_and_update_ma
-0001b680: 736b 286d 6173 6b2c 696d 6167 6529 3a0d  sk(mask,image):.
-0001b690: 0a20 2020 2020 2020 0d0a 2020 2020 2020  .       ..      
-0001b6a0: 2020 6966 206c 656e 286d 6173 6b2e 7368    if len(mask.sh
-0001b6b0: 6170 6529 203c 206c 656e 2869 6d61 6765  ape) < len(image
-0001b6c0: 2e73 6861 7065 293a 0d0a 2020 2020 2020  .shape):..      
-0001b6d0: 2020 2020 2020 7570 6461 7465 5f6d 6173        update_mas
-0001b6e0: 6b20 3d20 6e70 2e7a 6572 6f73 280d 0a20  k = np.zeros(.. 
-0001b6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b700: 2020 2020 2020 2020 2020 205b 0d0a 2020             [..  
-0001b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b720: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0001b730: 6167 652e 7368 6170 655b 305d 2c0d 0a20  age.shape[0],.. 
-0001b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b750: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001b760: 6d61 6765 2e73 6861 7065 5b31 5d2c 0d0a  mage.shape[1],..
-0001b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b790: 696d 6167 652e 7368 6170 655b 325d 2c0d  image.shape[2],.
-0001b7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b7c0: 2069 6d61 6765 2e73 6861 7065 5b33 5d2c   image.shape[3],
-0001b7d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b7e0: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-0001b7f0: 2064 7479 7065 3d22 7569 6e74 3822 0d0a   dtype="uint8"..
-0001b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b810: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0001b820: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-0001b830: 7261 6e67 6528 302c 2075 7064 6174 655f  range(0, update_
-0001b840: 6d61 736b 2e73 6861 7065 5b30 5d29 3a0d  mask.shape[0]):.
-0001b850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b860: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-0001b870: 302c 2075 7064 6174 655f 6d61 736b 2e73  0, update_mask.s
-0001b880: 6861 7065 5b31 5d29 3a0d 0a0d 0a20 2020  hape[1]):....   
-0001b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8a0: 2075 7064 6174 655f 6d61 736b 5b69 2c20   update_mask[i, 
-0001b8b0: 6a2c 203a 2c20 3a5d 203d 206d 6173 6b5b  j, :, :] = mask[
-0001b8c0: 692c 203a 2c20 3a5d 0d0a 2020 2020 2020  i, :, :]..      
-0001b8d0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
-0001b8e0: 2020 2020 2020 2020 2075 7064 6174 655f           update_
-0001b8f0: 6d61 736b 203d 206d 6173 6b0d 0a0d 0a20  mask = mask.... 
-0001b900: 2020 2020 2020 2072 6574 7572 6e20 7570         return up
-0001b910: 6461 7465 5f6d 6173 6b20 2020 2020 2020  date_mask       
-0001b920: 200d 0a20 2020 2020 2020 0d0a             ..       ..
+00019890: 2020 2073 656c 662e 616c 6c5f 6d65 616e     self.all_mean
+000198a0: 5f64 6973 7461 6e63 655f 6365 6c6c 5f6d  _distance_cell_m
+000198b0: 6173 6b2e 6170 7065 6e64 286e 702e 6d65  ask.append(np.me
+000198c0: 616e 2861 6c6c 5f64 6973 7461 6e63 655f  an(all_distance_
+000198d0: 6365 6c6c 5f6d 6173 6b29 290d 0a20 2020  cell_mask))..   
+000198e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198f0: 2073 656c 662e 616c 6c5f 7661 725f 6469   self.all_var_di
+00019900: 7374 616e 6365 5f63 656c 6c5f 6d61 736b  stance_cell_mask
+00019910: 2e61 7070 656e 6428 6e70 2e73 7464 2861  .append(np.std(a
+00019920: 6c6c 5f64 6973 7461 6e63 655f 6365 6c6c  ll_distance_cell
+00019930: 5f6d 6173 6b29 290d 0a20 2020 2020 2020  _mask))..       
+00019940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019950: 2020 2020 200d 0a20 2020 2020 2020 200d       ..        .
+00019960: 0a64 6566 2062 6f75 6e64 6172 795f 706f  .def boundary_po
+00019970: 696e 7473 286d 6173 6b2c 2078 6361 6c69  ints(mask, xcali
+00019980: 6272 6174 696f 6e2c 2079 6361 6c69 6272  bration, ycalibr
+00019990: 6174 696f 6e2c 207a 6361 6c69 6272 6174  ation, zcalibrat
+000199a0: 696f 6e29 3a0d 0a0d 0a20 2020 206e 6469  ion):....    ndi
+000199b0: 6d20 3d20 6c65 6e28 6d61 736b 2e73 6861  m = len(mask.sha
+000199c0: 7065 290d 0a20 2020 2074 696d 6564 5f6d  pe)..    timed_m
+000199d0: 6173 6b20 3d20 7b7d 0d0a 2020 2020 6d61  ask = {}..    ma
+000199e0: 736b 203d 206d 6173 6b20 3e20 300d 0a20  sk = mask > 0.. 
+000199f0: 2020 206d 6173 6b20 3d20 6d61 736b 2e61     mask = mask.a
+00019a00: 7374 7970 6528 2775 696e 7438 2729 0d0a  stype('uint8')..
+00019a10: 2020 2020 2320 5958 2073 6861 7065 6420      # YX shaped 
+00019a20: 6f62 6a65 6374 0d0a 2020 2020 6966 206e  object..    if n
+00019a30: 6469 6d20 3d3d 2032 3a0d 0a20 2020 2020  dim == 2:..     
+00019a40: 2020 200d 0a20 2020 2020 2020 2062 6f75     ..        bou
+00019a50: 6e64 6172 7920 3d20 6669 6e64 5f62 6f75  ndary = find_bou
+00019a60: 6e64 6172 6965 7328 6d61 736b 290d 0a20  ndaries(mask).. 
+00019a70: 2020 2020 2020 2072 6567 696f 6e63 656e         regioncen
+00019a80: 7472 6f69 6420 3d20 2830 2c29 202b 2063  troid = (0,) + c
+00019a90: 6f6d 7075 7465 5f63 656e 7472 6f69 6428  ompute_centroid(
+00019aa0: 626f 756e 6461 7279 2920 0d0a 2020 2020  boundary) ..    
+00019ab0: 2020 2020 696e 6469 6365 7320 3d20 6e70      indices = np
+00019ac0: 2e77 6865 7265 2862 6f75 6e64 6172 7920  .where(boundary 
+00019ad0: 3e20 3029 0d0a 2020 2020 2020 2020 7265  > 0)..        re
+00019ae0: 616c 5f69 6e64 6963 6573 203d 206e 702e  al_indices = np.
+00019af0: 7472 616e 7370 6f73 6528 6e70 2e61 7361  transpose(np.asa
+00019b00: 7272 6179 2869 6e64 6963 6573 2c20 6474  rray(indices, dt
+00019b10: 7970 653d 6e70 2e66 6c6f 6174 3332 2929  ype=np.float32))
+00019b20: 2e63 6f70 7928 290d 0a0d 0a20 2020 2020  .copy()....     
+00019b30: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
+00019b40: 6528 302c 206c 656e 2872 6561 6c5f 696e  e(0, len(real_in
+00019b50: 6469 6365 7329 293a 0d0a 0d0a 2020 2020  dices)):....    
+00019b60: 2020 2020 2020 2020 7265 616c 5f69 6e64          real_ind
+00019b70: 6963 6573 5b6a 5d5b 305d 203d 2072 6561  ices[j][0] = rea
+00019b80: 6c5f 696e 6469 6365 735b 6a5d 5b30 5d20  l_indices[j][0] 
+00019b90: 2a20 7963 616c 6962 7261 7469 6f6e 0d0a  * ycalibration..
+00019ba0: 2020 2020 2020 2020 2020 2020 7265 616c              real
+00019bb0: 5f69 6e64 6963 6573 5b6a 5d5b 315d 203d  _indices[j][1] =
+00019bc0: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+00019bd0: 5b31 5d20 2a20 7863 616c 6962 7261 7469  [1] * xcalibrati
+00019be0: 6f6e 0d0a 0d0a 2020 2020 2020 2020 7472  on....        tr
+00019bf0: 6565 203d 2073 7061 7469 616c 2e63 4b44  ee = spatial.cKD
+00019c00: 5472 6565 2872 6561 6c5f 696e 6469 6365  Tree(real_indice
+00019c10: 7329 0d0a 2020 2020 2020 2020 2320 5468  s)..        # Th
+00019c20: 6973 206f 626a 6563 7420 636f 6e74 6169  is object contai
+00019c30: 6e73 206c 6973 7420 6f66 2061 6c6c 2074  ns list of all t
+00019c40: 6865 2070 6f69 6e74 7320 666f 7220 616c  he points for al
+00019c50: 6c20 7468 6520 6c61 6265 6c73 2069 6e20  l the labels in 
+00019c60: 7468 6520 4d61 736b 2069 6d61 6765 2077  the Mask image w
+00019c70: 6974 6820 7468 6520 6c61 6265 6c20 6964  ith the label id
+00019c80: 2061 6e64 2076 6f6c 756d 6520 6f66 2065   and volume of e
+00019c90: 6163 6820 6c61 6265 6c0d 0a20 2020 2020  ach label..     
+00019ca0: 2020 2074 696d 6564 5f6d 6173 6b5b 7374     timed_mask[st
+00019cb0: 7228 3029 5d20 3d20 5b74 7265 652c 2069  r(0)] = [tree, i
+00019cc0: 6e64 6963 6573 2c20 7265 6769 6f6e 6365  ndices, regionce
+00019cd0: 6e74 726f 6964 5d0d 0a0d 0a20 2020 2023  ntroid]....    #
+00019ce0: 2054 5958 2073 6861 7065 6420 6f62 6a65   TYX shaped obje
+00019cf0: 6374 0d0a 2020 2020 6966 206e 6469 6d20  ct..    if ndim 
+00019d00: 3d3d 2033 3a0d 0a0d 0a0d 0a20 2020 2020  == 3:......     
+00019d10: 2020 2066 6f72 2069 2069 6e20 7471 646d     for i in tqdm
+00019d20: 2872 616e 6765 2830 2c20 6d61 736b 2e73  (range(0, mask.s
+00019d30: 6861 7065 5b30 5d29 293a 0d0a 2020 2020  hape[0])):..    
+00019d40: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+00019d50: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+00019d60: 756e 6461 7279 203d 2066 696e 645f 626f  undary = find_bo
+00019d70: 756e 6461 7269 6573 286d 6173 6b5b 692c  undaries(mask[i,
+00019d80: 3a5d 290d 0a20 2020 2020 2020 2020 2020  :])..           
+00019d90: 2020 2020 2072 6567 696f 6e63 656e 7472       regioncentr
+00019da0: 6f69 6420 3d20 2830 2c29 202b 2063 6f6d  oid = (0,) + com
+00019db0: 7075 7465 5f63 656e 7472 6f69 6428 626f  pute_centroid(bo
+00019dc0: 756e 6461 7279 2920 0d0a 2020 2020 2020  undary) ..      
+00019dd0: 2020 2020 2020 2020 2020 696e 6469 6365            indice
+00019de0: 7320 3d20 6e70 2e77 6865 7265 2862 6f75  s = np.where(bou
+00019df0: 6e64 6172 7920 3e20 3029 0d0a 2020 2020  ndary > 0)..    
+00019e00: 2020 2020 2020 2020 2020 2020 7265 616c              real
+00019e10: 5f69 6e64 6963 6573 203d 206e 702e 7472  _indices = np.tr
+00019e20: 616e 7370 6f73 6528 6e70 2e61 7361 7272  anspose(np.asarr
+00019e30: 6179 2869 6e64 6963 6573 2c20 6474 7970  ay(indices, dtyp
+00019e40: 653d 6e70 2e66 6c6f 6174 3332 2929 2e63  e=np.float32)).c
+00019e50: 6f70 7928 290d 0a0d 0a20 2020 2020 2020  opy()....       
+00019e60: 2020 2020 2020 2020 2066 6f72 206a 2069           for j i
+00019e70: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
+00019e80: 6561 6c5f 696e 6469 6365 7329 293a 0d0a  eal_indices)):..
+00019e90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019ea0: 2020 2020 2020 7265 616c 5f69 6e64 6963        real_indic
+00019eb0: 6573 5b6a 5d5b 305d 203d 2072 6561 6c5f  es[j][0] = real_
+00019ec0: 696e 6469 6365 735b 6a5d 5b30 5d20 2a20  indices[j][0] * 
+00019ed0: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
+00019ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ef0: 2020 7265 616c 5f69 6e64 6963 6573 5b6a    real_indices[j
+00019f00: 5d5b 315d 203d 2072 6561 6c5f 696e 6469  ][1] = real_indi
+00019f10: 6365 735b 6a5d 5b31 5d20 2a20 7863 616c  ces[j][1] * xcal
+00019f20: 6962 7261 7469 6f6e 0d0a 0d0a 2020 2020  ibration....    
+00019f30: 2020 2020 2020 2020 2020 2020 7472 6565              tree
+00019f40: 203d 2073 7061 7469 616c 2e63 4b44 5472   = spatial.cKDTr
+00019f50: 6565 2872 6561 6c5f 696e 6469 6365 7329  ee(real_indices)
+00019f60: 0d0a 0d0a 2020 2020 2020 2020 2020 2020  ....            
+00019f70: 2020 2020 7469 6d65 645f 6d61 736b 5b73      timed_mask[s
+00019f80: 7472 2869 295d 203d 205b 7472 6565 2c20  tr(i)] = [tree, 
+00019f90: 696e 6469 6365 732c 2072 6567 696f 6e63  indices, regionc
+00019fa0: 656e 7472 6f69 645d 0d0a 2020 2020 2020  entroid]..      
+00019fb0: 2020 2020 2020 0d0a 2020 2020 2320 545a        ..    # TZ
+00019fc0: 5958 2073 6861 7065 6420 6f62 6a65 6374  YX shaped object
+00019fd0: 0d0a 2020 2020 6966 206e 6469 6d20 3d3d  ..    if ndim ==
+00019fe0: 2034 3a0d 0a20 2020 2020 2020 2070 7269   4:..        pri
+00019ff0: 6e74 2827 4d61 6b69 6e67 206d 6173 6b20  nt('Making mask 
+0001a000: 696e 2034 4427 290d 0a20 2020 2020 2020  in 4D')..       
+0001a010: 2062 6f75 6e64 6172 7920 3d20 6e70 2e7a   boundary = np.z
+0001a020: 6572 6f73 280d 0a20 2020 2020 2020 2020  eros(..         
+0001a030: 2020 205b 6d61 736b 2e73 6861 7065 5b30     [mask.shape[0
+0001a040: 5d2c 206d 6173 6b2e 7368 6170 655b 315d  ], mask.shape[1]
+0001a050: 2c20 6d61 736b 2e73 6861 7065 5b32 5d2c  , mask.shape[2],
+0001a060: 206d 6173 6b2e 7368 6170 655b 335d 5d2c   mask.shape[3]],
+0001a070: 2064 7479 7065 3d6e 702e 7569 6e74 380d   dtype=np.uint8.
+0001a080: 0a20 2020 2020 2020 2029 0d0a 2020 2020  .        )..    
+0001a090: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
+0001a0a0: 6765 2830 2c20 6d61 736b 2e73 6861 7065  ge(0, mask.shape
+0001a0b0: 5b30 5d29 3a0d 0a20 2020 2020 2020 2020  [0]):..         
+0001a0c0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0001a0d0: 2062 6f75 6e64 6172 795b 692c 3a5d 203d   boundary[i,:] =
+0001a0e0: 2066 696e 645f 626f 756e 6461 7269 6573   find_boundaries
+0001a0f0: 286d 6173 6b5b 692c 3a5d 290d 0a20 2020  (mask[i,:])..   
+0001a100: 2020 2020 2020 2020 2072 6567 696f 6e63           regionc
+0001a110: 656e 7472 6f69 6420 3d20 636f 6d70 7574  entroid = comput
+0001a120: 655f 6365 6e74 726f 6964 2862 6f75 6e64  e_centroid(bound
+0001a130: 6172 795b 692c 3a5d 2920 0d0a 2020 2020  ary[i,:]) ..    
+0001a140: 2020 2020 2020 2020 696e 6469 6365 7320          indices 
+0001a150: 3d20 6e70 2e77 6865 7265 2862 6f75 6e64  = np.where(bound
+0001a160: 6172 795b 692c 3a5d 203e 2030 290d 0a20  ary[i,:] > 0).. 
+0001a170: 2020 2020 2020 2020 2020 2072 6561 6c5f             real_
+0001a180: 696e 6469 6365 7320 3d20 6e70 2e74 7261  indices = np.tra
+0001a190: 6e73 706f 7365 286e 702e 6173 6172 7261  nspose(np.asarra
+0001a1a0: 7928 696e 6469 6365 732c 2064 7479 7065  y(indices, dtype
+0001a1b0: 3d6e 702e 666c 6f61 7433 3229 292e 636f  =np.float32)).co
+0001a1c0: 7079 2829 0d0a 0d0a 2020 2020 2020 2020  py()....        
+0001a1d0: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+0001a1e0: 6765 2830 2c20 6c65 6e28 7265 616c 5f69  ge(0, len(real_i
+0001a1f0: 6e64 6963 6573 2929 3a0d 0a0d 0a20 2020  ndices)):....   
+0001a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a210: 2072 6561 6c5f 696e 6469 6365 735b 6a5d   real_indices[j]
+0001a220: 5b30 5d20 3d20 7265 616c 5f69 6e64 6963  [0] = real_indic
+0001a230: 6573 5b6a 5d5b 305d 202a 207a 6361 6c69  es[j][0] * zcali
+0001a240: 6272 6174 696f 6e0d 0a20 2020 2020 2020  bration..       
+0001a250: 2020 2020 2020 2020 2020 2020 2072 6561               rea
+0001a260: 6c5f 696e 6469 6365 735b 6a5d 5b31 5d20  l_indices[j][1] 
+0001a270: 3d20 7265 616c 5f69 6e64 6963 6573 5b6a  = real_indices[j
+0001a280: 5d5b 315d 202a 2079 6361 6c69 6272 6174  ][1] * ycalibrat
+0001a290: 696f 6e0d 0a20 2020 2020 2020 2020 2020  ion..           
+0001a2a0: 2020 2020 2020 2020 2072 6561 6c5f 696e           real_in
+0001a2b0: 6469 6365 735b 6a5d 5b32 5d20 3d20 7265  dices[j][2] = re
+0001a2c0: 616c 5f69 6e64 6963 6573 5b6a 5d5b 325d  al_indices[j][2]
+0001a2d0: 202a 2078 6361 6c69 6272 6174 696f 6e0d   * xcalibration.
+0001a2e0: 0a0d 0a20 2020 2020 2020 2020 2020 2074  ...            t
+0001a2f0: 7265 6520 3d20 7370 6174 6961 6c2e 634b  ree = spatial.cK
+0001a300: 4454 7265 6528 7265 616c 5f69 6e64 6963  DTree(real_indic
+0001a310: 6573 290d 0a20 2020 2020 2020 2020 2020  es)..           
+0001a320: 2074 696d 6564 5f6d 6173 6b5b 7374 7228   timed_mask[str(
+0001a330: 6929 5d20 3d20 5b74 7265 652c 2069 6e64  i)] = [tree, ind
+0001a340: 6963 6573 2c20 7265 6769 6f6e 6365 6e74  ices, regioncent
+0001a350: 726f 6964 5d0d 0a20 2020 2070 7269 6e74  roid]..    print
+0001a360: 2827 436f 6d70 7574 6564 2074 6865 2062  ('Computed the b
+0001a370: 6f75 6e64 6172 7920 706f 696e 7473 2729  oundary points')
+0001a380: 0d0a 0d0a 2020 2020 7265 7475 726e 2074  ....    return t
+0001a390: 696d 6564 5f6d 6173 6b2c 2062 6f75 6e64  imed_mask, bound
+0001a3a0: 6172 7920 2020 2020 2020 200d 0a0d 0a64  ary        ....d
+0001a3b0: 6566 2063 6f6d 7075 7465 5f63 656e 7472  ef compute_centr
+0001a3c0: 6f69 6428 6269 6e61 7279 5f69 6d61 6765  oid(binary_image
+0001a3d0: 293a 0d0a 2020 2020 2320 456e 7375 7265  ):..    # Ensure
+0001a3e0: 2062 696e 6172 7920 696d 6167 6520 6973   binary image is
+0001a3f0: 2061 204e 756d 5079 2061 7272 6179 0d0a   a NumPy array..
+0001a400: 2020 2020 6269 6e61 7279 5f69 6d61 6765      binary_image
+0001a410: 203d 206e 702e 6172 7261 7928 6269 6e61   = np.array(bina
+0001a420: 7279 5f69 6d61 6765 290d 0a0d 0a20 2020  ry_image)....   
+0001a430: 2077 6869 7465 5f70 6978 656c 7320 3d20   white_pixels = 
+0001a440: 6e70 2e77 6865 7265 2862 696e 6172 795f  np.where(binary_
+0001a450: 696d 6167 6520 3d3d 2031 290d 0a20 2020  image == 1)..   
+0001a460: 206e 756d 5f70 6978 656c 7320 3d20 6c65   num_pixels = le
+0001a470: 6e28 7768 6974 655f 7069 7865 6c73 5b30  n(white_pixels[0
+0001a480: 5d29 0d0a 0d0a 2020 2020 2320 436f 6d70  ])....    # Comp
+0001a490: 7574 6520 7468 6520 6365 6e74 726f 6964  ute the centroid
+0001a4a0: 206f 6620 7468 6520 7768 6974 6520 7069   of the white pi
+0001a4b0: 7865 6c73 2069 6e20 7468 6520 626f 756e  xels in the boun
+0001a4c0: 6461 7279 2069 6d61 6765 0d0a 2020 2020  dary image..    
+0001a4d0: 6365 6e74 726f 6964 203d 206e 702e 7a65  centroid = np.ze
+0001a4e0: 726f 7328 6269 6e61 7279 5f69 6d61 6765  ros(binary_image
+0001a4f0: 2e6e 6469 6d29 0d0a 2020 2020 666f 7220  .ndim)..    for 
+0001a500: 6469 6d20 696e 2072 616e 6765 2862 696e  dim in range(bin
+0001a510: 6172 795f 696d 6167 652e 6e64 696d 293a  ary_image.ndim):
+0001a520: 0d0a 2020 2020 2020 2020 6365 6e74 726f  ..        centro
+0001a530: 6964 5b64 696d 5d20 3d20 7768 6974 655f  id[dim] = white_
+0001a540: 7069 7865 6c73 5b64 696d 5d2e 7375 6d28  pixels[dim].sum(
+0001a550: 2920 2f20 6e75 6d5f 7069 7865 6c73 0d0a  ) / num_pixels..
+0001a560: 0d0a 2020 2020 7265 7475 726e 2063 656e  ..    return cen
+0001a570: 7472 6f69 640d 0a0d 0a0d 0a0d 0a20 0d0a  troid........ ..
+0001a580: 0d0a 6465 6620 6765 745f 6373 765f 6461  ..def get_csv_da
+0001a590: 7461 2863 7376 293a 0d0a 0d0a 2020 2020  ta(csv):....    
+0001a5a0: 2020 2020 6461 7461 7365 7420 3d20 7064      dataset = pd
+0001a5b0: 2e72 6561 645f 6373 7628 0d0a 2020 2020  .read_csv(..    
+0001a5c0: 2020 2020 2020 2020 6373 762c 2064 656c          csv, del
+0001a5d0: 696d 6974 6572 3d22 2c22 2c20 656e 636f  imiter=",", enco
+0001a5e0: 6469 6e67 3d22 756e 6963 6f64 655f 6573  ding="unicode_es
+0001a5f0: 6361 7065 222c 206c 6f77 5f6d 656d 6f72  cape", low_memor
+0001a600: 793d 4661 6c73 650d 0a20 2020 2020 2020  y=False..       
+0001a610: 2029 5b33 3a5d 0d0a 2020 2020 2020 2020   )[3:]..        
+0001a620: 6461 7461 7365 745f 696e 6465 7820 3d20  dataset_index = 
+0001a630: 6461 7461 7365 742e 696e 6465 780d 0a20  dataset.index.. 
+0001a640: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
+0001a650: 7461 7365 742c 2064 6174 6173 6574 5f69  taset, dataset_i
+0001a660: 6e64 6578 0d0a 2020 2020 0d0a 6465 6620  ndex..    ..def 
+0001a670: 6765 745f 7370 6f74 5f64 6174 6173 6574  get_spot_dataset
+0001a680: 2873 706f 745f 6461 7461 7365 742c 2074  (spot_dataset, t
+0001a690: 7261 636b 5f61 6e61 6c79 7369 735f 7370  rack_analysis_sp
+0001a6a0: 6f74 5f6b 6579 732c 2078 6361 6c69 6272  ot_keys, xcalibr
+0001a6b0: 6174 696f 6e2c 2079 6361 6c69 6272 6174  ation, ycalibrat
+0001a6c0: 696f 6e2c 207a 6361 6c69 6272 6174 696f  ion, zcalibratio
+0001a6d0: 6e2c 2041 7474 7269 6275 7465 426f 786e  n, AttributeBoxn
+0001a6e0: 616d 652c 2064 6574 6563 7469 6f6e 6368  ame, detectionch
+0001a6f0: 616e 6e65 6c29 3a0d 0a20 2020 2020 2020  annel):..       
+0001a700: 2041 6c6c 5661 6c75 6573 203d 207b 7d0d   AllValues = {}.
+0001a710: 0a20 2020 2020 2020 2070 6f73 6978 203d  .        posix =
+0001a720: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001a730: 7370 6f74 5f6b 6579 735b 2270 6f73 6978  spot_keys["posix
+0001a740: 225d 0d0a 2020 2020 2020 2020 706f 7369  "]..        posi
+0001a750: 7920 3d20 7472 6163 6b5f 616e 616c 7973  y = track_analys
+0001a760: 6973 5f73 706f 745f 6b65 7973 5b22 706f  is_spot_keys["po
+0001a770: 7369 7922 5d0d 0a20 2020 2020 2020 2070  siy"]..        p
+0001a780: 6f73 697a 203d 2074 7261 636b 5f61 6e61  osiz = track_ana
+0001a790: 6c79 7369 735f 7370 6f74 5f6b 6579 735b  lysis_spot_keys[
+0001a7a0: 2270 6f73 697a 225d 0d0a 2020 2020 2020  "posiz"]..      
+0001a7b0: 2020 6672 616d 6520 3d20 7472 6163 6b5f    frame = track_
+0001a7c0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001a7d0: 7973 5b22 6672 616d 6522 5d0d 0a20 2020  ys["frame"]..   
+0001a7e0: 2020 2020 200d 0a20 2020 2020 2020 204c       ..        L
+0001a7f0: 6f63 6174 696f 6e58 203d 2028 0d0a 2020  ocationX = (..  
+0001a800: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+0001a810: 6174 6173 6574 5b70 6f73 6978 5d2e 6173  ataset[posix].as
+0001a820: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+0001a830: 7863 616c 6962 7261 7469 6f6e 0d0a 2020  xcalibration..  
+0001a840: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+0001a850: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+0001a860: 6f63 6174 696f 6e59 203d 2028 0d0a 2020  ocationY = (..  
+0001a870: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+0001a880: 6174 6173 6574 5b70 6f73 6979 5d2e 6173  ataset[posiy].as
+0001a890: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+0001a8a0: 7963 616c 6962 7261 7469 6f6e 0d0a 2020  ycalibration..  
+0001a8b0: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+0001a8c0: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+0001a8d0: 6f63 6174 696f 6e5a 203d 2028 0d0a 2020  ocationZ = (..  
+0001a8e0: 2020 2020 2020 2020 2020 7370 6f74 5f64            spot_d
+0001a8f0: 6174 6173 6574 5b70 6f73 697a 5d2e 6173  ataset[posiz].as
+0001a900: 7479 7065 2822 666c 6f61 7422 2920 2f20  type("float") / 
+0001a910: 7a63 616c 6962 7261 7469 6f6e 0d0a 2020  zcalibration..  
+0001a920: 2020 2020 2020 292e 6173 7479 7065 2822        ).astype("
+0001a930: 696e 7422 290d 0a20 2020 2020 2020 204c  int")..        L
+0001a940: 6f63 6174 696f 6e54 203d 2028 7370 6f74  ocationT = (spot
+0001a950: 5f64 6174 6173 6574 5b66 7261 6d65 5d2e  _dataset[frame].
+0001a960: 6173 7479 7065 2822 666c 6f61 7422 2929  astype("float"))
+0001a970: 2e61 7374 7970 6528 2269 6e74 2229 0d0a  .astype("int")..
+0001a980: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+0001a990: 2020 2020 6967 6e6f 7265 5f76 616c 7565      ignore_value
+0001a9a0: 7320 3d20 5b74 7261 636b 5f61 6e61 6c79  s = [track_analy
+0001a9b0: 7369 735f 7370 6f74 5f6b 6579 735b 226d  sis_spot_keys["m
+0001a9c0: 6561 6e5f 696e 7465 6e73 6974 7922 5d2c  ean_intensity"],
+0001a9d0: 7472 6163 6b5f 616e 616c 7973 6973 5f73  track_analysis_s
+0001a9e0: 706f 745f 6b65 7973 5b22 746f 7461 6c5f  pot_keys["total_
+0001a9f0: 696e 7465 6e73 6974 7922 5d5d 0d0a 2020  intensity"]]..  
+0001aa00: 2020 2020 2020 666f 7220 286b 2c76 2920        for (k,v) 
+0001aa10: 696e 2074 7261 636b 5f61 6e61 6c79 7369  in track_analysi
+0001aa20: 735f 7370 6f74 5f6b 6579 732e 6974 656d  s_spot_keys.item
+0001aa30: 7328 293a 0d0a 0d0a 2020 2020 2020 2020  s():....        
+0001aa40: 2020 2020 2020 2020 6966 2064 6574 6563          if detec
+0001aa50: 7469 6f6e 6368 616e 6e65 6c20 3d3d 2031  tionchannel == 1
+0001aa60: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001aa70: 2020 2020 2020 2020 6966 206b 203d 3d20          if k == 
+0001aa80: 226d 6561 6e5f 696e 7465 6e73 6974 795f  "mean_intensity_
+0001aa90: 6368 3222 3a0d 0a20 2020 2020 2020 2020  ch2":..         
+0001aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aab0: 2020 7661 6c75 6520 3d20 7472 6163 6b5f    value = track_
+0001aac0: 616e 616c 7973 6973 5f73 706f 745f 6b65  analysis_spot_ke
+0001aad0: 7973 5b22 6d65 616e 5f69 6e74 656e 7369  ys["mean_intensi
+0001aae0: 7479 225d 0d0a 2020 2020 2020 2020 2020  ty"]..          
+0001aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab00: 2041 6c6c 5661 6c75 6573 5b76 616c 7565   AllValues[value
+0001ab10: 5d20 3d20 7370 6f74 5f64 6174 6173 6574  ] = spot_dataset
+0001ab20: 5b76 5d2e 6173 7479 7065 2822 666c 6f61  [v].astype("floa
+0001ab30: 7422 290d 0a20 2020 2020 2020 2020 2020  t")..           
+0001ab40: 2020 2020 2020 2020 2020 6966 206b 203d            if k =
+0001ab50: 3d20 2274 6f74 616c 5f69 6e74 656e 7369  = "total_intensi
+0001ab60: 7479 5f63 6832 223a 0d0a 2020 2020 2020  ty_ch2":..      
+0001ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab80: 2020 2020 2076 616c 7565 203d 2074 7261       value = tra
+0001ab90: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001aba0: 5f6b 6579 735b 2274 6f74 616c 5f69 6e74  _keys["total_int
+0001abb0: 656e 7369 7479 225d 0d0a 2020 2020 2020  ensity"]..      
+0001abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001abd0: 2020 2020 2041 6c6c 5661 6c75 6573 5b76       AllValues[v
+0001abe0: 616c 7565 5d20 3d20 7370 6f74 5f64 6174  alue] = spot_dat
+0001abf0: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
+0001ac00: 666c 6f61 7422 2920 2020 2020 2020 0d0a  float")       ..
+0001ac10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ac20: 2020 6966 2076 206e 6f74 2069 6e20 6967    if v not in ig
+0001ac30: 6e6f 7265 5f76 616c 7565 733a 0d0a 2020  nore_values:..  
+0001ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ac50: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0001ac60: 2020 2020 2020 2020 2020 2020 2020 416c                Al
+0001ac70: 6c56 616c 7565 735b 765d 203d 2073 706f  lValues[v] = spo
+0001ac80: 745f 6461 7461 7365 745b 765d 2e61 7374  t_dataset[v].ast
+0001ac90: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
+0001aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001acb0: 200d 0a0d 0a20 2020 2020 2020 2041 6c6c   ....        All
+0001acc0: 5661 6c75 6573 5b70 6f73 6978 5d20 3d20  Values[posix] = 
+0001acd0: 726f 756e 6428 4c6f 6361 7469 6f6e 582c  round(LocationX,
+0001ace0: 3329 0d0a 2020 2020 2020 2020 416c 6c56  3)..        AllV
+0001acf0: 616c 7565 735b 706f 7369 795d 203d 2072  alues[posiy] = r
+0001ad00: 6f75 6e64 284c 6f63 6174 696f 6e59 2c33  ound(LocationY,3
+0001ad10: 290d 0a20 2020 2020 2020 2041 6c6c 5661  )..        AllVa
+0001ad20: 6c75 6573 5b70 6f73 697a 5d20 3d20 726f  lues[posiz] = ro
+0001ad30: 756e 6428 4c6f 6361 7469 6f6e 5a2c 3329  und(LocationZ,3)
+0001ad40: 0d0a 2020 2020 2020 2020 416c 6c56 616c  ..        AllVal
+0001ad50: 7565 735b 6672 616d 655d 203d 2072 6f75  ues[frame] = rou
+0001ad60: 6e64 284c 6f63 6174 696f 6e54 2c33 290d  nd(LocationT,3).
+0001ad70: 0a20 2020 2020 2020 2041 7474 7269 6275  .        Attribu
+0001ad80: 7465 6964 7320 3d20 5b5d 0d0a 2020 2020  teids = []..    
+0001ad90: 2020 2020 4174 7472 6962 7574 6569 6473      Attributeids
+0001ada0: 2e61 7070 656e 6428 4174 7472 6962 7574  .append(Attribut
+0001adb0: 6542 6f78 6e61 6d65 290d 0a20 2020 2020  eBoxname)..     
+0001adc0: 2020 2066 6f72 2061 7474 7269 6275 7465     for attribute
+0001add0: 6e61 6d65 2069 6e20 416c 6c56 616c 7565  name in AllValue
+0001ade0: 732e 6b65 7973 2829 3a0d 0a20 2020 2020  s.keys():..     
+0001adf0: 2020 2020 2020 2020 2041 7474 7269 6275           Attribu
+0001ae00: 7465 6964 732e 6170 7065 6e64 2861 7474  teids.append(att
+0001ae10: 7269 6275 7465 6e61 6d65 2920 2020 200d  ributename)    .
+0001ae20: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0001ae30: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001ae40: 2072 6574 7572 6e20 4174 7472 6962 7574   return Attribut
+0001ae50: 6569 6473 2c20 416c 6c56 616c 7565 7320  eids, AllValues 
+0001ae60: 2020 2020 0d0a 2020 2020 0d0a 6465 6620      ..    ..def 
+0001ae70: 6765 745f 7472 6163 6b5f 6461 7461 7365  get_track_datase
+0001ae80: 7428 7472 6163 6b5f 6461 7461 7365 742c  t(track_dataset,
+0001ae90: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001aea0: 7370 6f74 5f6b 6579 732c 2074 7261 636b  spot_keys, track
+0001aeb0: 5f61 6e61 6c79 7369 735f 7472 6163 6b5f  _analysis_track_
+0001aec0: 6b65 7973 2c20 5472 6163 6b41 7474 7269  keys, TrackAttri
+0001aed0: 6275 7465 426f 786e 616d 6529 3a0d 0a0d  buteBoxname):...
+0001aee0: 0a20 2020 2020 2020 2041 6c6c 5472 6163  .        AllTrac
+0001aef0: 6b56 616c 7565 7320 3d20 7b7d 0d0a 2020  kValues = {}..  
+0001af00: 2020 2020 2020 7472 6163 6b5f 6964 203d        track_id =
+0001af10: 2074 7261 636b 5f61 6e61 6c79 7369 735f   track_analysis_
+0001af20: 7370 6f74 5f6b 6579 735b 2274 7261 636b  spot_keys["track
+0001af30: 5f69 6422 5d0d 0a20 2020 2020 2020 2054  _id"]..        T
+0001af40: 6964 203d 2074 7261 636b 5f64 6174 6173  id = track_datas
+0001af50: 6574 5b74 7261 636b 5f69 645d 2e61 7374  et[track_id].ast
+0001af60: 7970 6528 2266 6c6f 6174 2229 0d0a 2020  ype("float")..  
+0001af70: 2020 2020 200d 0a20 2020 2020 2020 2041       ..        A
+0001af80: 6c6c 5472 6163 6b56 616c 7565 735b 7472  llTrackValues[tr
+0001af90: 6163 6b5f 6964 5d20 3d20 5469 640d 0a20  ack_id] = Tid.. 
+0001afa0: 2020 2020 200d 0a20 2020 2020 2020 2066       ..        f
+0001afb0: 6f72 2028 6b2c 2076 2920 696e 2074 7261  or (k, v) in tra
+0001afc0: 636b 5f61 6e61 6c79 7369 735f 7472 6163  ck_analysis_trac
+0001afd0: 6b5f 6b65 7973 2e69 7465 6d73 2829 3a0d  k_keys.items():.
+0001afe0: 0a0d 0a20 2020 2020 2020 2020 2020 2020  ...             
+0001aff0: 2020 2078 203d 2074 7261 636b 5f64 6174     x = track_dat
+0001b000: 6173 6574 5b76 5d2e 6173 7479 7065 2822  aset[v].astype("
+0001b010: 666c 6f61 7422 290d 0a20 2020 2020 2020  float")..       
+0001b020: 2020 2020 2020 2020 206d 696e 7661 6c20           minval 
+0001b030: 3d20 6d69 6e28 7829 0d0a 2020 2020 2020  = min(x)..      
+0001b040: 2020 2020 2020 2020 2020 6d61 7876 616c            maxval
+0001b050: 203d 206d 6178 2878 290d 0a0d 0a20 2020   = max(x)....   
+0001b060: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0001b070: 6d69 6e76 616c 203e 2030 2061 6e64 206d  minval > 0 and m
+0001b080: 6178 7661 6c20 3c3d 2031 3a0d 0a0d 0a20  axval <= 1:.... 
+0001b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0a0: 2020 2078 203d 2078 202b 2031 0d0a 0d0a     x = x + 1....
+0001b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0c0: 416c 6c54 7261 636b 5661 6c75 6573 5b6b  AllTrackValues[k
+0001b0d0: 5d20 3d20 726f 756e 6428 782c 2033 290d  ] = round(x, 3).
+0001b0e0: 0a0d 0a20 2020 2020 2020 2054 7261 636b  ...        Track
+0001b0f0: 4174 7472 6962 7574 6569 6473 203d 205b  Attributeids = [
+0001b100: 5d0d 0a20 2020 2020 2020 2054 7261 636b  ]..        Track
+0001b110: 4174 7472 6962 7574 6569 6473 2e61 7070  Attributeids.app
+0001b120: 656e 6428 5472 6163 6b41 7474 7269 6275  end(TrackAttribu
+0001b130: 7465 426f 786e 616d 6529 0d0a 2020 2020  teBoxname)..    
+0001b140: 2020 2020 666f 7220 6174 7472 6962 7574      for attribut
+0001b150: 656e 616d 6520 696e 2074 7261 636b 5f61  ename in track_a
+0001b160: 6e61 6c79 7369 735f 7472 6163 6b5f 6b65  nalysis_track_ke
+0001b170: 7973 2e6b 6579 7328 293a 0d0a 2020 2020  ys.keys():..    
+0001b180: 2020 2020 2020 2020 5472 6163 6b41 7474          TrackAtt
+0001b190: 7269 6275 7465 6964 732e 6170 7065 6e64  ributeids.append
+0001b1a0: 2861 7474 7269 6275 7465 6e61 6d65 2920  (attributename) 
+0001b1b0: 2020 200d 0a20 2020 200d 0a20 2020 2020     ..    ..     
+0001b1c0: 2020 2072 6574 7572 6e20 5472 6163 6b41     return TrackA
+0001b1d0: 7474 7269 6275 7465 6964 732c 2041 6c6c  ttributeids, All
+0001b1e0: 5472 6163 6b56 616c 7565 730d 0a20 2020  TrackValues..   
+0001b1f0: 200d 0a64 6566 2067 6574 5f65 6467 6573   ..def get_edges
+0001b200: 5f64 6174 6173 6574 2865 6467 6573 5f64  _dataset(edges_d
+0001b210: 6174 6173 6574 2c20 6564 6765 735f 6461  ataset, edges_da
+0001b220: 7461 7365 745f 696e 6465 782c 2074 7261  taset_index, tra
+0001b230: 636b 5f61 6e61 6c79 7369 735f 7370 6f74  ck_analysis_spot
+0001b240: 5f6b 6579 732c 2074 7261 636b 5f61 6e61  _keys, track_ana
+0001b250: 6c79 7369 735f 6564 6765 735f 6b65 7973  lysis_edges_keys
+0001b260: 293a 0d0a 0d0a 2020 2020 2020 2020 416c  ):....        Al
+0001b270: 6c45 6467 6573 5661 6c75 6573 203d 207b  lEdgesValues = {
+0001b280: 7d0d 0a20 2020 2020 2020 2074 7261 636b  }..        track
+0001b290: 5f69 6420 3d20 7472 6163 6b5f 616e 616c  _id = track_anal
+0001b2a0: 7973 6973 5f73 706f 745f 6b65 7973 5b22  ysis_spot_keys["
+0001b2b0: 7472 6163 6b5f 6964 225d 0d0a 2020 2020  track_id"]..    
+0001b2c0: 2020 2020 5469 6420 3d20 6564 6765 735f      Tid = edges_
+0001b2d0: 6461 7461 7365 745b 7472 6163 6b5f 6964  dataset[track_id
+0001b2e0: 5d2e 6173 7479 7065 2822 666c 6f61 7422  ].astype("float"
+0001b2f0: 290d 0a20 2020 2020 2020 2069 6e64 6963  )..        indic
+0001b300: 6573 203d 206e 702e 7768 6572 6528 5469  es = np.where(Ti
+0001b310: 6420 3d3d 2030 290d 0a20 2020 2020 2020  d == 0)..       
+0001b320: 206d 6178 7472 6163 6b5f 6964 203d 206d   maxtrack_id = m
+0001b330: 6178 2854 6964 290d 0a20 2020 2020 2020  ax(Tid)..       
+0001b340: 2063 6f6e 6469 7469 6f6e 5f69 6e64 6963   condition_indic
+0001b350: 6573 203d 2065 6467 6573 5f64 6174 6173  es = edges_datas
+0001b360: 6574 5f69 6e64 6578 5b69 6e64 6963 6573  et_index[indices
+0001b370: 5d0d 0a20 2020 2020 2020 2054 6964 5b63  ]..        Tid[c
+0001b380: 6f6e 6469 7469 6f6e 5f69 6e64 6963 6573  ondition_indices
+0001b390: 5d20 3d20 6d61 7874 7261 636b 5f69 6420  ] = maxtrack_id 
+0001b3a0: 2b20 310d 0a20 2020 2020 2020 2041 6c6c  + 1..        All
+0001b3b0: 4564 6765 7356 616c 7565 735b 7472 6163  EdgesValues[trac
+0001b3c0: 6b5f 6964 5d20 3d20 5469 640d 0a0d 0a20  k_id] = Tid.... 
+0001b3d0: 2020 2020 2020 2066 6f72 206b 2069 6e20         for k in 
+0001b3e0: 7472 6163 6b5f 616e 616c 7973 6973 5f65  track_analysis_e
+0001b3f0: 6467 6573 5f6b 6579 732e 7661 6c75 6573  dges_keys.values
+0001b400: 2829 3a0d 0a0d 0a20 2020 2020 2020 2020  ():....         
+0001b410: 2020 2069 6620 6b20 213d 2074 7261 636b     if k != track
+0001b420: 5f69 643a 0d0a 2020 2020 2020 2020 2020  _id:..          
+0001b430: 2020 2020 2020 7820 3d20 6564 6765 735f        x = edges_
+0001b440: 6461 7461 7365 745b 6b5d 2e61 7374 7970  dataset[k].astyp
+0001b450: 6528 2266 6c6f 6174 2229 0d0a 0d0a 2020  e("float")....  
+0001b460: 2020 2020 2020 2020 2020 2020 2020 416c                Al
+0001b470: 6c45 6467 6573 5661 6c75 6573 5b6b 5d20  lEdgesValues[k] 
+0001b480: 3d20 7820 2020 0d0a 2020 2020 2020 2020  = x   ..        
+0001b490: 200d 0a20 2020 2020 2020 2072 6574 7572   ..        retur
+0001b4a0: 6e20 416c 6c45 6467 6573 5661 6c75 6573  n AllEdgesValues
+0001b4b0: 2020 200d 0a20 2020 200d 0a20 2020 2020     ..    ..     
+0001b4c0: 2020 0d0a 2020 2020 0d0a 6465 6620 7363    ..    ..def sc
+0001b4d0: 616c 655f 7661 6c75 6528 782c 2073 6361  ale_value(x, sca
+0001b4e0: 6c65 203d 2032 3535 202a 2032 3535 293a  le = 255 * 255):
+0001b4f0: 0d0a 0d0a 0d0a 2020 2020 2072 6574 7572  ......     retur
+0001b500: 6e20 7820 2a20 7363 616c 6520 2020 0d0a  n x * scale   ..
+0001b510: 2020 2020 0d0a 0d0a 0d0a 6465 6620 7072      ......def pr
+0001b520: 6f62 5f73 6967 6d6f 6964 2878 293a 0d0a  ob_sigmoid(x):..
+0001b530: 2020 2020 7265 7475 726e 2031 202d 206d      return 1 - m
+0001b540: 6174 682e 6578 7028 2d78 290d 0a0d 0a0d  ath.exp(-x).....
+0001b550: 0a64 6566 2061 6e67 756c 6172 5f63 6861  .def angular_cha
+0001b560: 6e67 6528 7665 635f 302c 2076 6563 5f31  nge(vec_0, vec_1
+0001b570: 293a 0d0a 2020 2020 2020 2020 0d0a 2020  ):..        ..  
+0001b580: 2020 2020 2020 7665 635f 3020 3d20 7665        vec_0 = ve
+0001b590: 635f 3020 2f20 6e70 2e6c 696e 616c 672e  c_0 / np.linalg.
+0001b5a0: 6e6f 726d 2876 6563 5f30 290d 0a20 2020  norm(vec_0)..   
+0001b5b0: 2020 2020 2076 6563 5f31 203d 2076 6563       vec_1 = vec
+0001b5c0: 5f31 202f 206e 702e 6c69 6e61 6c67 2e6e  _1 / np.linalg.n
+0001b5d0: 6f72 6d28 7665 635f 3129 0d0a 2020 2020  orm(vec_1)..    
+0001b5e0: 2020 2020 616e 676c 6520 3d20 6e70 2e61      angle = np.a
+0001b5f0: 7263 636f 7328 6e70 2e63 6c69 7028 6e70  rccos(np.clip(np
+0001b600: 2e64 6f74 2876 6563 5f30 2c20 7665 635f  .dot(vec_0, vec_
+0001b610: 3129 2c20 2d31 2e30 2c20 312e 3029 290d  1), -1.0, 1.0)).
+0001b620: 0a20 2020 2020 2020 2061 6e67 6c65 203d  .        angle =
+0001b630: 2061 6e67 6c65 202a 2031 3830 202f 206e   angle * 180 / n
+0001b640: 702e 7069 0d0a 2020 2020 2020 2020 7265  p.pi..        re
+0001b650: 7475 726e 2061 6e67 6c65 0d0a 2020 2020  turn angle..    
+0001b660: 200d 0a0d 0a64 6566 2065 7661 6c5f 626f   ....def eval_bo
+0001b670: 6f6c 2876 616c 7565 293a 0d0a 2020 2020  ol(value):..    
+0001b680: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0001b690: 2020 2020 2020 2020 6966 2076 616c 7565          if value
+0001b6a0: 2020 3d3d 2027 5472 7565 273a 200d 0a20    == 'True': .. 
+0001b6b0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+0001b6c0: 6976 5f6b 6579 203d 2054 7275 650d 0a20  iv_key = True.. 
+0001b6d0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0001b6e0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+0001b6f0: 765f 6b65 7920 3d20 4661 6c73 6520 0d0a  v_key = False ..
+0001b700: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001b710: 2064 6976 5f6b 6579 2020 2020 2020 2020   div_key        
+0001b720: 2020 2020 2020 2020 0d0a 0d0a 6465 6620          ....def 
+0001b730: 6368 6563 6b5f 616e 645f 7570 6461 7465  check_and_update
+0001b740: 5f6d 6173 6b28 6d61 736b 2c69 6d61 6765  _mask(mask,image
+0001b750: 293a 0d0a 2020 2020 2020 200d 0a20 2020  ):..       ..   
+0001b760: 2020 2020 2069 6620 6c65 6e28 6d61 736b       if len(mask
+0001b770: 2e73 6861 7065 2920 3c20 6c65 6e28 696d  .shape) < len(im
+0001b780: 6167 652e 7368 6170 6529 3a0d 0a20 2020  age.shape):..   
+0001b790: 2020 2020 2020 2020 2075 7064 6174 655f           update_
+0001b7a0: 6d61 736b 203d 206e 702e 7a65 726f 7328  mask = np.zeros(
+0001b7b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b7c0: 2020 2020 2020 2020 2020 2020 2020 5b0d                [.
+0001b7d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b7f0: 2069 6d61 6765 2e73 6861 7065 5b30 5d2c   image.shape[0],
+0001b800: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b820: 2020 696d 6167 652e 7368 6170 655b 315d    image.shape[1]
+0001b830: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b850: 2020 2069 6d61 6765 2e73 6861 7065 5b32     image.shape[2
+0001b860: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+0001b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b880: 2020 2020 696d 6167 652e 7368 6170 655b      image.shape[
+0001b890: 335d 2c0d 0a20 2020 2020 2020 2020 2020  3],..           
+0001b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b8b0: 205d 2c20 6474 7970 653d 2275 696e 7438   ], dtype="uint8
+0001b8c0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
+0001b8d0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+0001b8e0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+0001b8f0: 696e 2072 616e 6765 2830 2c20 7570 6461  in range(0, upda
+0001b900: 7465 5f6d 6173 6b2e 7368 6170 655b 305d  te_mask.shape[0]
+0001b910: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001b920: 2020 2020 666f 7220 6a20 696e 2072 616e      for j in ran
+0001b930: 6765 2830 2c20 7570 6461 7465 5f6d 6173  ge(0, update_mas
+0001b940: 6b2e 7368 6170 655b 315d 293a 0d0a 0d0a  k.shape[1]):....
+0001b950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b960: 2020 2020 7570 6461 7465 5f6d 6173 6b5b      update_mask[
+0001b970: 692c 206a 2c20 3a2c 203a 5d20 3d20 6d61  i, j, :, :] = ma
+0001b980: 736b 5b69 2c20 3a2c 203a 5d0d 0a20 2020  sk[i, :, :]..   
+0001b990: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+0001b9a0: 2020 2020 2020 2020 2020 2020 7570 6461              upda
+0001b9b0: 7465 5f6d 6173 6b20 3d20 6d61 736b 0d0a  te_mask = mask..
+0001b9c0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001b9d0: 2075 7064 6174 655f 6d61 736b 2020 2020   update_mask    
+0001b9e0: 2020 2020 0d0a 2020 2020 2020 200d 0a        ..       ..
```

### Comparing `napatrackmater-3.8.6/napatrackmater/Trackvector.py` & `napatrackmater-3.8.7/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.6/napatrackmater/__init__.py` & `napatrackmater-3.8.7/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.6/napatrackmater/clustering.py` & `napatrackmater-3.8.7/napatrackmater/clustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.6/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.8.7/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.6/napatrackmater/fate_mapping.py` & `napatrackmater-3.8.7/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.6/napatrackmater/pretrained.py` & `napatrackmater-3.8.7/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.6/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.8.7/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.8.6
+Version: 3.8.7
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.8.6/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.8.7/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.8.6/setup.py` & `napatrackmater-3.8.7/setup.py`

 * *Files identical despite different names*

