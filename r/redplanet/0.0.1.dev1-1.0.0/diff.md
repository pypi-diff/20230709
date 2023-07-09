# Comparing `tmp/redplanet-0.0.1.dev1.tar.gz` & `tmp/redplanet-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redplanet-0.0.1.dev1.tar", last modified: Sun Jul  9 17:42:29 2023, max compression
+gzip compressed data, was "redplanet-1.0.0.tar", last modified: Sun Jul  9 18:02:56 2023, max compression
```

## Comparing `redplanet-0.0.1.dev1.tar` & `redplanet-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.573420 redplanet-0.0.1.dev1/
--rw-rw-rw-   0        0        0    35821 2023-06-23 07:09:38.000000 redplanet-0.0.1.dev1/LICENSE.txt
--rw-rw-rw-   0        0        0    46226 2023-07-09 17:42:29.573420 redplanet-0.0.1.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     3791 2023-07-09 17:40:53.000000 redplanet-0.0.1.dev1/README.md
--rw-rw-rw-   0        0        0     3348 2023-07-09 17:41:36.000000 redplanet-0.0.1.dev1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-09 17:42:29.573420 redplanet-0.0.1.dev1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.528037 redplanet-0.0.1.dev1/src/
-drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.534127 redplanet-0.0.1.dev1/src/redplanet/
-drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.568437 redplanet-0.0.1.dev1/src/redplanet/Crust/
--rw-rw-rw-   0        0        0    30071 2023-07-09 04:30:43.000000 redplanet-0.0.1.dev1/src/redplanet/Crust/Crust.py
--rw-rw-rw-   0        0        0     5800 2023-07-09 04:44:31.000000 redplanet-0.0.1.dev1/src/redplanet/Crust/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.571608 redplanet-0.0.1.dev1/src/redplanet/GRS/
--rw-rw-rw-   0        0        0    23508 2023-07-09 04:07:45.000000 redplanet-0.0.1.dev1/src/redplanet/GRS/GRS.py
--rw-rw-rw-   0        0        0     3226 2023-07-09 04:04:41.000000 redplanet-0.0.1.dev1/src/redplanet/GRS/__init__.py
--rw-rw-rw-   0        0        0     4529 2023-07-09 04:39:11.000000 redplanet-0.0.1.dev1/src/redplanet/__init__.py
--rw-rw-rw-   0        0        0     4733 2023-07-09 04:36:21.000000 redplanet-0.0.1.dev1/src/redplanet/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-09 17:42:29.565474 redplanet-0.0.1.dev1/src/redplanet.egg-info/
--rw-rw-rw-   0        0        0    46226 2023-07-09 17:42:29.000000 redplanet-0.0.1.dev1/src/redplanet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-07-09 17:42:29.000000 redplanet-0.0.1.dev1/src/redplanet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 17:42:29.000000 redplanet-0.0.1.dev1/src/redplanet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-07-09 17:42:29.000000 redplanet-0.0.1.dev1/src/redplanet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-09 17:42:29.000000 redplanet-0.0.1.dev1/src/redplanet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-09 18:02:56.113208 redplanet-1.0.0/
+-rw-rw-rw-   0        0        0    35821 2023-06-23 07:09:38.000000 redplanet-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    46431 2023-07-09 18:02:56.112351 redplanet-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3989 2023-07-09 17:59:51.000000 redplanet-1.0.0/README.md
+-rw-rw-rw-   0        0        0     3355 2023-07-09 18:01:55.000000 redplanet-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-09 18:02:56.113208 redplanet-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-09 18:02:56.082167 redplanet-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-09 18:02:56.088153 redplanet-1.0.0/src/redplanet/
+drwxrwxrwx   0        0        0        0 2023-07-09 18:02:56.108220 redplanet-1.0.0/src/redplanet/Crust/
+-rw-rw-rw-   0        0        0    30071 2023-07-09 04:30:43.000000 redplanet-1.0.0/src/redplanet/Crust/Crust.py
+-rw-rw-rw-   0        0        0     5800 2023-07-09 04:44:31.000000 redplanet-1.0.0/src/redplanet/Crust/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:02:56.110212 redplanet-1.0.0/src/redplanet/GRS/
+-rw-rw-rw-   0        0        0    23508 2023-07-09 04:07:45.000000 redplanet-1.0.0/src/redplanet/GRS/GRS.py
+-rw-rw-rw-   0        0        0     3226 2023-07-09 04:04:41.000000 redplanet-1.0.0/src/redplanet/GRS/__init__.py
+-rw-rw-rw-   0        0        0     4529 2023-07-09 04:39:11.000000 redplanet-1.0.0/src/redplanet/__init__.py
+-rw-rw-rw-   0        0        0     4733 2023-07-09 04:36:21.000000 redplanet-1.0.0/src/redplanet/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-09 18:02:56.106223 redplanet-1.0.0/src/redplanet.egg-info/
+-rw-rw-rw-   0        0        0    46431 2023-07-09 18:02:56.000000 redplanet-1.0.0/src/redplanet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-09 18:02:56.000000 redplanet-1.0.0/src/redplanet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-09 18:02:56.000000 redplanet-1.0.0/src/redplanet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-07-09 18:02:56.000000 redplanet-1.0.0/src/redplanet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-09 18:02:56.000000 redplanet-1.0.0/src/redplanet.egg-info/top_level.txt
```

### Comparing `redplanet-0.0.1.dev1/LICENSE.txt` & `redplanet-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev1/PKG-INFO` & `redplanet-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redplanet
-Version: 0.0.1.dev1
+Version: 1.0.0
 Summary: User-friendly access (i.e. APIs) for various Mars datasets and derived geophysics quantities. Create publication-ready plots on the fly or access the underlying data for more involved calculations.
 Author-email: Zain Eris Kamal <zain.eris.kamal@rutgers.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,15 +676,15 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://github.com/Humboldt-Penguin/redplanet
 Project-URL: Author, https://github.com/Humboldt-Penguin
 Keywords: mars,geophysics,grs,crust,heat flow
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -711,16 +711,18 @@
 Access/visualize chemical abundance maps derived from the 2001 Mars Odyssey Gamma Ray Spectrometer. The original data is defined in 5 degree bins, but this module allows you to programmatically estimate values at exact coordinates by interpolating between points. Concentrations can be extracted for both the shallow subsurface (raw data) and bulk crustal composition (normalized to volatile-free basis, i.e. zero H2O/Cl/Si).
 
 &nbsp;
 
 - Example 1: Iron concentrations in Arabia Terra. Data is normalized to a volatile-free basis (H2O/Cl/Si free), so it is representative of the bulk crustal composition rather than shallow subsurface. 
 
 <p align="center">
-  <!-- <img width="600" src="docs/figures/GRS_fe_norm_ArabiaTerra.png"> -->
-  <img width="600" src="https://files.catbox.moe/irjxsp.png">
+  <a href="https://files.catbox.moe/irjxsp.png">
+    <!-- <img width="600" src="docs/figures/GRS_fe_norm_ArabiaTerra.png"> -->
+    <img width="600" src="https://files.catbox.moe/irjxsp.png">
+  </a>
 </p>
 
 
 
 Recreate with: 
 ```python
 from redplanet import GRS
@@ -744,16 +746,18 @@
 Access/visualize maps of topography, Moho, crustal thickness, and crustal density from spherical harmonics. We offer ~22,000 models of the crust-mantle interface parameterized by reference interior models, crustal thickness at the InSight landing, and homogeneous/inhomogeneous crustal densities across the dichotomy. 
 
 &nbsp;
 
 - Example 1: Topography, Moho, and crustal thickness of the Valles Marineris region. Model parameters are 41 km crustal thickness at the InSight landing, 2,900 kg/m^3 crustal density in the North, and 2,700 kg/m^3 crustal density in the South.
 
 <p align="center">
-  <!-- <img src="docs/figures/Crust_various_VallesMarineris.png"> -->
-  <img src="https://files.catbox.moe/tnk9io.png">
+  <a href="https://files.catbox.moe/tnk9io.png">
+    <!-- <img src="docs/figures/Crust_various_VallesMarineris.png"> -->
+    <img src="https://files.catbox.moe/tnk9io.png">
+  </a>
 </p>
 
 
 Recreate with:
 ```python
 from redplanet import Crust
 lons = (-100,-20)
@@ -765,16 +769,18 @@
 ```
 
 &nbsp;
 
 - Example 2: Crustal thickness profile of Henry Crater with various crust-mantle interface models.
 
 <p align="center">
-  <!-- <img src="docs/figures/Crust_thick-profile_Henry.png"> -->
-  <img src="https://files.catbox.moe/nnnm3l.png">
+  <a href="https://files.catbox.moe/nnnm3l.png">
+    <!-- <img src="docs/figures/Crust_thick-profile_Henry.png"> -->
+    <img width="700" src="https://files.catbox.moe/nnnm3l.png">
+  </a>
 </p>
 
 
 Recreate with: See section 2.2 in [demo.ipynb](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/notebooks/demo/demo.ipynb).
 
 &nbsp;
```

### Comparing `redplanet-0.0.1.dev1/README.md` & `redplanet-1.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -57,181 +57,194 @@
 00000380: 2c20 736f 2069 7420 6973 2072 6570 7265  , so it is repre
 00000390: 7365 6e74 6174 6976 6520 6f66 2074 6865  sentative of the
 000003a0: 2062 756c 6b20 6372 7573 7461 6c20 636f   bulk crustal co
 000003b0: 6d70 6f73 6974 696f 6e20 7261 7468 6572  mposition rather
 000003c0: 2074 6861 6e20 7368 616c 6c6f 7720 7375   than shallow su
 000003d0: 6273 7572 6661 6365 2e20 0d0a 0d0a 3c70  bsurface. ....<p
 000003e0: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-000003f0: 0d0a 2020 3c21 2d2d 203c 696d 6720 7769  ..  <!-- <img wi
-00000400: 6474 683d 2236 3030 2220 7372 633d 2264  dth="600" src="d
-00000410: 6f63 732f 6669 6775 7265 732f 4752 535f  ocs/figures/GRS_
-00000420: 6665 5f6e 6f72 6d5f 4172 6162 6961 5465  fe_norm_ArabiaTe
-00000430: 7272 612e 706e 6722 3e20 2d2d 3e0d 0a20  rra.png"> -->.. 
-00000440: 203c 696d 6720 7769 6474 683d 2236 3030   <img width="600
-00000450: 2220 7372 633d 2268 7474 7073 3a2f 2f66  " src="https://f
-00000460: 696c 6573 2e63 6174 626f 782e 6d6f 652f  iles.catbox.moe/
-00000470: 6972 6a78 7370 2e70 6e67 223e 0d0a 3c2f  irjxsp.png">..</
-00000480: 703e 0d0a 0d0a 0d0a 0d0a 5265 6372 6561  p>........Recrea
-00000490: 7465 2077 6974 683a 200d 0a60 6060 7079  te with: ..```py
-000004a0: 7468 6f6e 0d0a 6672 6f6d 2072 6564 706c  thon..from redpl
-000004b0: 616e 6574 2069 6d70 6f72 7420 4752 530d  anet import GRS.
-000004c0: 0a47 5253 2e76 6973 7561 6c69 7a65 280d  .GRS.visualize(.
-000004d0: 0a20 2065 6c65 6d65 6e74 5f6e 616d 653d  .  element_name=
-000004e0: 2766 6527 2c20 0d0a 2020 6e6f 726d 616c  'fe', ..  normal
-000004f0: 697a 653d 5472 7565 2c20 0d0a 2020 6c6f  ize=True, ..  lo
-00000500: 6e5f 626f 756e 6473 3d28 352c 3430 292c  n_bounds=(5,40),
-00000510: 200d 0a20 206c 6174 5f62 6f75 6e64 733d   ..  lat_bounds=
-00000520: 282d 3130 2c33 3029 2c20 0d0a 2020 6772  (-10,30), ..  gr
-00000530: 6964 5f73 7061 6369 6e67 3d30 2e31 2c20  id_spacing=0.1, 
-00000540: 0d0a 2020 6f76 6572 6c61 793d 5472 7565  ..  overlay=True
-00000550: 0d0a 290d 0a60 6060 0d0a 0d0a 266e 6273  ..)..```....&nbs
-00000560: 703b 0d0a 0d0a 2d2d 2d2d 0d0a 0d0a 2323  p;....----....##
-00000570: 2043 7275 7374 0d0a 0d0a 0d0a 4163 6365   Crust......Acce
-00000580: 7373 2f76 6973 7561 6c69 7a65 206d 6170  ss/visualize map
-00000590: 7320 6f66 2074 6f70 6f67 7261 7068 792c  s of topography,
-000005a0: 204d 6f68 6f2c 2063 7275 7374 616c 2074   Moho, crustal t
-000005b0: 6869 636b 6e65 7373 2c20 616e 6420 6372  hickness, and cr
-000005c0: 7573 7461 6c20 6465 6e73 6974 7920 6672  ustal density fr
-000005d0: 6f6d 2073 7068 6572 6963 616c 2068 6172  om spherical har
-000005e0: 6d6f 6e69 6373 2e20 5765 206f 6666 6572  monics. We offer
-000005f0: 207e 3232 2c30 3030 206d 6f64 656c 7320   ~22,000 models 
-00000600: 6f66 2074 6865 2063 7275 7374 2d6d 616e  of the crust-man
-00000610: 746c 6520 696e 7465 7266 6163 6520 7061  tle interface pa
-00000620: 7261 6d65 7465 7269 7a65 6420 6279 2072  rameterized by r
-00000630: 6566 6572 656e 6365 2069 6e74 6572 696f  eference interio
-00000640: 7220 6d6f 6465 6c73 2c20 6372 7573 7461  r models, crusta
-00000650: 6c20 7468 6963 6b6e 6573 7320 6174 2074  l thickness at t
-00000660: 6865 2049 6e53 6967 6874 206c 616e 6469  he InSight landi
-00000670: 6e67 2c20 616e 6420 686f 6d6f 6765 6e65  ng, and homogene
-00000680: 6f75 732f 696e 686f 6d6f 6765 6e65 6f75  ous/inhomogeneou
-00000690: 7320 6372 7573 7461 6c20 6465 6e73 6974  s crustal densit
-000006a0: 6965 7320 6163 726f 7373 2074 6865 2064  ies across the d
-000006b0: 6963 686f 746f 6d79 2e20 0d0a 0d0a 266e  ichotomy. ....&n
-000006c0: 6273 703b 0d0a 0d0a 2d20 4578 616d 706c  bsp;....- Exampl
-000006d0: 6520 313a 2054 6f70 6f67 7261 7068 792c  e 1: Topography,
-000006e0: 204d 6f68 6f2c 2061 6e64 2063 7275 7374   Moho, and crust
-000006f0: 616c 2074 6869 636b 6e65 7373 206f 6620  al thickness of 
-00000700: 7468 6520 5661 6c6c 6573 204d 6172 696e  the Valles Marin
-00000710: 6572 6973 2072 6567 696f 6e2e 204d 6f64  eris region. Mod
-00000720: 656c 2070 6172 616d 6574 6572 7320 6172  el parameters ar
-00000730: 6520 3431 206b 6d20 6372 7573 7461 6c20  e 41 km crustal 
-00000740: 7468 6963 6b6e 6573 7320 6174 2074 6865  thickness at the
-00000750: 2049 6e53 6967 6874 206c 616e 6469 6e67   InSight landing
-00000760: 2c20 322c 3930 3020 6b67 2f6d 5e33 2063  , 2,900 kg/m^3 c
-00000770: 7275 7374 616c 2064 656e 7369 7479 2069  rustal density i
-00000780: 6e20 7468 6520 4e6f 7274 682c 2061 6e64  n the North, and
-00000790: 2032 2c37 3030 206b 672f 6d5e 3320 6372   2,700 kg/m^3 cr
-000007a0: 7573 7461 6c20 6465 6e73 6974 7920 696e  ustal density in
-000007b0: 2074 6865 2053 6f75 7468 2e0d 0a0d 0a3c   the South.....<
-000007c0: 7020 616c 6967 6e3d 2263 656e 7465 7222  p align="center"
-000007d0: 3e0d 0a20 203c 212d 2d20 3c69 6d67 2073  >..  <!-- <img s
-000007e0: 7263 3d22 646f 6373 2f66 6967 7572 6573  rc="docs/figures
-000007f0: 2f43 7275 7374 5f76 6172 696f 7573 5f56  /Crust_various_V
-00000800: 616c 6c65 734d 6172 696e 6572 6973 2e70  allesMarineris.p
-00000810: 6e67 223e 202d 2d3e 0d0a 2020 3c69 6d67  ng"> -->..  <img
-00000820: 2073 7263 3d22 6874 7470 733a 2f2f 6669   src="https://fi
-00000830: 6c65 732e 6361 7462 6f78 2e6d 6f65 2f74  les.catbox.moe/t
-00000840: 6e6b 3969 6f2e 706e 6722 3e0d 0a3c 2f70  nk9io.png">..</p
-00000850: 3e0d 0a0d 0a0d 0a52 6563 7265 6174 6520  >......Recreate 
-00000860: 7769 7468 3a0d 0a60 6060 7079 7468 6f6e  with:..```python
-00000870: 0d0a 6672 6f6d 2072 6564 706c 616e 6574  ..from redplanet
-00000880: 2069 6d70 6f72 7420 4372 7573 740d 0a6c   import Crust..l
-00000890: 6f6e 7320 3d20 282d 3130 302c 2d32 3029  ons = (-100,-20)
-000008a0: 0d0a 6c61 7473 203d 2028 2d36 302c 3430  ..lats = (-60,40
-000008b0: 290d 0a43 7275 7374 2e6c 6f61 645f 6d6f  )..Crust.load_mo
-000008c0: 6465 6c28 5249 4d3d 274b 6861 6e32 3032  del(RIM='Khan202
-000008d0: 3227 2c20 696e 7369 6768 745f 7468 6963  2', insight_thic
-000008e0: 6b6e 6573 733d 3431 2c20 7268 6f5f 6e6f  kness=41, rho_no
-000008f0: 7274 683d 3239 3030 2c20 7268 6f5f 736f  rth=2900, rho_so
-00000900: 7574 683d 3237 3030 290d 0a43 7275 7374  uth=2700)..Crust
-00000910: 2e76 6973 7561 6c69 7a65 2871 7561 6e74  .visualize(quant
-00000920: 6974 793d 2774 6f70 6f27 2c20 6c6f 6e5f  ity='topo', lon_
-00000930: 626f 756e 6473 3d6c 6f6e 732c 206c 6174  bounds=lons, lat
-00000940: 5f62 6f75 6e64 733d 6c61 7473 2c20 6772  _bounds=lats, gr
-00000950: 6964 5f73 7061 6369 6e67 3d30 2e31 290d  id_spacing=0.1).
-00000960: 0a43 7275 7374 2e76 6973 7561 6c69 7a65  .Crust.visualize
-00000970: 2871 7561 6e74 6974 793d 276d 6f68 6f27  (quantity='moho'
-00000980: 2c20 6c6f 6e5f 626f 756e 6473 3d6c 6f6e  , lon_bounds=lon
-00000990: 732c 206c 6174 5f62 6f75 6e64 733d 6c61  s, lat_bounds=la
-000009a0: 7473 2c20 6f76 6572 6c61 793d 5472 7565  ts, overlay=True
-000009b0: 2c20 6772 6964 5f73 7061 6369 6e67 3d30  , grid_spacing=0
-000009c0: 2e33 290d 0a43 7275 7374 2e76 6973 7561  .3)..Crust.visua
-000009d0: 6c69 7a65 2871 7561 6e74 6974 793d 2774  lize(quantity='t
-000009e0: 6869 636b 272c 206c 6f6e 5f62 6f75 6e64  hick', lon_bound
-000009f0: 733d 6c6f 6e73 2c20 6c61 745f 626f 756e  s=lons, lat_boun
-00000a00: 6473 3d6c 6174 732c 206f 7665 726c 6179  ds=lats, overlay
-00000a10: 3d54 7275 652c 2067 7269 645f 7370 6163  =True, grid_spac
-00000a20: 696e 673d 302e 3329 0d0a 6060 600d 0a0d  ing=0.3)..```...
-00000a30: 0a26 6e62 7370 3b0d 0a0d 0a2d 2045 7861  .&nbsp;....- Exa
-00000a40: 6d70 6c65 2032 3a20 4372 7573 7461 6c20  mple 2: Crustal 
-00000a50: 7468 6963 6b6e 6573 7320 7072 6f66 696c  thickness profil
-00000a60: 6520 6f66 2048 656e 7279 2043 7261 7465  e of Henry Crate
-00000a70: 7220 7769 7468 2076 6172 696f 7573 2063  r with various c
-00000a80: 7275 7374 2d6d 616e 746c 6520 696e 7465  rust-mantle inte
-00000a90: 7266 6163 6520 6d6f 6465 6c73 2e0d 0a0d  rface models....
-00000aa0: 0a3c 7020 616c 6967 6e3d 2263 656e 7465  .<p align="cente
-00000ab0: 7222 3e0d 0a20 203c 212d 2d20 3c69 6d67  r">..  <!-- <img
-00000ac0: 2073 7263 3d22 646f 6373 2f66 6967 7572   src="docs/figur
-00000ad0: 6573 2f43 7275 7374 5f74 6869 636b 2d70  es/Crust_thick-p
-00000ae0: 726f 6669 6c65 5f48 656e 7279 2e70 6e67  rofile_Henry.png
-00000af0: 223e 202d 2d3e 0d0a 2020 3c69 6d67 2073  "> -->..  <img s
-00000b00: 7263 3d22 6874 7470 733a 2f2f 6669 6c65  rc="https://file
-00000b10: 732e 6361 7462 6f78 2e6d 6f65 2f6e 6e6e  s.catbox.moe/nnn
-00000b20: 6d33 6c2e 706e 6722 3e0d 0a3c 2f70 3e0d  m3l.png">..</p>.
-00000b30: 0a0d 0a0d 0a52 6563 7265 6174 6520 7769  .....Recreate wi
-00000b40: 7468 3a20 5365 6520 7365 6374 696f 6e20  th: See section 
-00000b50: 322e 3220 696e 205b 6465 6d6f 2e69 7079  2.2 in [demo.ipy
-00000b60: 6e62 5d28 6874 7470 733a 2f2f 6769 7468  nb](https://gith
-00000b70: 7562 2e63 6f6d 2f48 756d 626f 6c64 742d  ub.com/Humboldt-
-00000b80: 5065 6e67 7569 6e2f 7265 6470 6c61 6e65  Penguin/redplane
-00000b90: 742f 626c 6f62 2f6d 6169 6e2f 646f 6373  t/blob/main/docs
-00000ba0: 2f6e 6f74 6562 6f6f 6b73 2f64 656d 6f2f  /notebooks/demo/
-00000bb0: 6465 6d6f 2e69 7079 6e62 292e 0d0a 0d0a  demo.ipynb).....
-00000bc0: 266e 6273 703b 0d0a 0d0a 2d2d 2d0d 0a0d  &nbsp;....---...
-00000bd0: 0a23 2044 6f63 756d 656e 7461 7469 6f6e  .# Documentation
-00000be0: 0d0a 0d0a 3c21 2d2d 2046 6f72 2061 206d  ....<!-- For a m
-00000bf0: 6f72 6520 696e 2d64 6570 7468 2074 7574  ore in-depth tut
-00000c00: 6f72 6961 6c20 696e 2069 6e74 6572 6163  orial in interac
-00000c10: 7469 7665 206e 6f74 6562 6f6f 6b20 666f  tive notebook fo
-00000c20: 726d 6174 2c20 7365 6520 5b64 6f63 732f  rmat, see [docs/
-00000c30: 6e6f 7465 626f 6f6b 732f 6465 6d6f 2f64  notebooks/demo/d
-00000c40: 656d 6f2e 6970 796e 625d 2864 6f63 732f  emo.ipynb](docs/
-00000c50: 6e6f 7465 626f 6f6b 732f 6465 6d6f 2f64  notebooks/demo/d
-00000c60: 656d 6f2e 6970 796e 6229 2e20 2d2d 3e0d  emo.ipynb). -->.
-00000c70: 0a46 6f72 2061 206d 6f72 6520 696e 2d64  .For a more in-d
-00000c80: 6570 7468 2074 7574 6f72 6961 6c20 696e  epth tutorial in
-00000c90: 2069 6e74 6572 6163 7469 7665 206e 6f74   interactive not
-00000ca0: 6562 6f6f 6b20 666f 726d 6174 2c20 7365  ebook format, se
-00000cb0: 6520 5b64 656d 6f2e 6970 796e 625d 2868  e [demo.ipynb](h
-00000cc0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000cd0: 6d2f 4875 6d62 6f6c 6474 2d50 656e 6775  m/Humboldt-Pengu
-00000ce0: 696e 2f72 6564 706c 616e 6574 2f62 6c6f  in/redplanet/blo
-00000cf0: 622f 6d61 696e 2f64 6f63 732f 6e6f 7465  b/main/docs/note
-00000d00: 626f 6f6b 732f 6465 6d6f 2f64 656d 6f2e  books/demo/demo.
-00000d10: 6970 796e 6229 2e0d 0a0d 0a26 6e62 7370  ipynb).....&nbsp
-00000d20: 3b0d 0a0d 0a2d 2d2d 0d0a 0d0a 2320 4c69  ;....---....# Li
-00000d30: 6e6b 730d 0a0d 0a2d 2044 6f6e 2774 2068  nks....- Don't h
-00000d40: 6573 6974 6174 6520 746f 2072 6561 6368  esitate to reach
-00000d50: 206f 7574 3a20 5b7a 6169 6e2e 6572 6973   out: [zain.eris
-00000d60: 2e6b 616d 616c 4072 7574 6765 7273 2e65  .kamal@rutgers.e
-00000d70: 6475 5d28 6d61 696c 746f 3a7a 6169 6e2e  du](mailto:zain.
-00000d80: 6572 6973 2e6b 616d 616c 4072 7574 6765  eris.kamal@rutge
-00000d90: 7273 2e65 6475 290d 0a2d 2041 636b 6e6f  rs.edu)..- Ackno
-00000da0: 776c 6564 6765 6d65 6e74 733a 205b 646f  wledgements: [do
-00000db0: 6373 2f74 6861 6e6b 732e 7478 745d 2868  cs/thanks.txt](h
-00000dc0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000dd0: 6d2f 4875 6d62 6f6c 6474 2d50 656e 6775  m/Humboldt-Pengu
-00000de0: 696e 2f72 6564 706c 616e 6574 2f62 6c6f  in/redplanet/blo
-00000df0: 622f 6d61 696e 2f64 6f63 732f 7468 616e  b/main/docs/than
-00000e00: 6b73 2e74 7874 290d 0a2d 2052 6566 6572  ks.txt)..- Refer
-00000e10: 656e 6365 733a 205b 646f 6373 2f72 6566  ences: [docs/ref
-00000e20: 6572 656e 6365 732e 7478 745d 2868 7474  erences.txt](htt
-00000e30: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000e40: 4875 6d62 6f6c 6474 2d50 656e 6775 696e  Humboldt-Penguin
-00000e50: 2f72 6564 706c 616e 6574 2f62 6c6f 622f  /redplanet/blob/
-00000e60: 6d61 696e 2f64 6f63 732f 7265 6665 7265  main/docs/refere
-00000e70: 6e63 6573 2e74 7874 290d 0a2d 204f 7468  nces.txt)..- Oth
-00000e80: 6572 2077 6f72 6b3a 205b 6769 7468 7562  er work: [github
-00000e90: 2e63 6f6d 2f48 756d 626f 6c64 742d 5065  .com/Humboldt-Pe
-00000ea0: 6e67 7569 6e5d 2868 7474 7073 3a2f 2f67  nguin](https://g
-00000eb0: 6974 6875 622e 636f 6d2f 4875 6d62 6f6c  ithub.com/Humbol
-00000ec0: 6474 2d50 656e 6775 696e 290d 0a0d 0a    dt-Penguin)....
+000003f0: 0d0a 2020 3c61 2068 7265 663d 2268 7474  ..  <a href="htt
+00000400: 7073 3a2f 2f66 696c 6573 2e63 6174 626f  ps://files.catbo
+00000410: 782e 6d6f 652f 6972 6a78 7370 2e70 6e67  x.moe/irjxsp.png
+00000420: 223e 0d0a 2020 2020 3c21 2d2d 203c 696d  ">..    <!-- <im
+00000430: 6720 7769 6474 683d 2236 3030 2220 7372  g width="600" sr
+00000440: 633d 2264 6f63 732f 6669 6775 7265 732f  c="docs/figures/
+00000450: 4752 535f 6665 5f6e 6f72 6d5f 4172 6162  GRS_fe_norm_Arab
+00000460: 6961 5465 7272 612e 706e 6722 3e20 2d2d  iaTerra.png"> --
+00000470: 3e0d 0a20 2020 203c 696d 6720 7769 6474  >..    <img widt
+00000480: 683d 2236 3030 2220 7372 633d 2268 7474  h="600" src="htt
+00000490: 7073 3a2f 2f66 696c 6573 2e63 6174 626f  ps://files.catbo
+000004a0: 782e 6d6f 652f 6972 6a78 7370 2e70 6e67  x.moe/irjxsp.png
+000004b0: 223e 0d0a 2020 3c2f 613e 0d0a 3c2f 703e  ">..  </a>..</p>
+000004c0: 0d0a 0d0a 0d0a 0d0a 5265 6372 6561 7465  ........Recreate
+000004d0: 2077 6974 683a 200d 0a60 6060 7079 7468   with: ..```pyth
+000004e0: 6f6e 0d0a 6672 6f6d 2072 6564 706c 616e  on..from redplan
+000004f0: 6574 2069 6d70 6f72 7420 4752 530d 0a47  et import GRS..G
+00000500: 5253 2e76 6973 7561 6c69 7a65 280d 0a20  RS.visualize(.. 
+00000510: 2065 6c65 6d65 6e74 5f6e 616d 653d 2766   element_name='f
+00000520: 6527 2c20 0d0a 2020 6e6f 726d 616c 697a  e', ..  normaliz
+00000530: 653d 5472 7565 2c20 0d0a 2020 6c6f 6e5f  e=True, ..  lon_
+00000540: 626f 756e 6473 3d28 352c 3430 292c 200d  bounds=(5,40), .
+00000550: 0a20 206c 6174 5f62 6f75 6e64 733d 282d  .  lat_bounds=(-
+00000560: 3130 2c33 3029 2c20 0d0a 2020 6772 6964  10,30), ..  grid
+00000570: 5f73 7061 6369 6e67 3d30 2e31 2c20 0d0a  _spacing=0.1, ..
+00000580: 2020 6f76 6572 6c61 793d 5472 7565 0d0a    overlay=True..
+00000590: 290d 0a60 6060 0d0a 0d0a 266e 6273 703b  )..```....&nbsp;
+000005a0: 0d0a 0d0a 2d2d 2d2d 0d0a 0d0a 2323 2043  ....----....## C
+000005b0: 7275 7374 0d0a 0d0a 0d0a 4163 6365 7373  rust......Access
+000005c0: 2f76 6973 7561 6c69 7a65 206d 6170 7320  /visualize maps 
+000005d0: 6f66 2074 6f70 6f67 7261 7068 792c 204d  of topography, M
+000005e0: 6f68 6f2c 2063 7275 7374 616c 2074 6869  oho, crustal thi
+000005f0: 636b 6e65 7373 2c20 616e 6420 6372 7573  ckness, and crus
+00000600: 7461 6c20 6465 6e73 6974 7920 6672 6f6d  tal density from
+00000610: 2073 7068 6572 6963 616c 2068 6172 6d6f   spherical harmo
+00000620: 6e69 6373 2e20 5765 206f 6666 6572 207e  nics. We offer ~
+00000630: 3232 2c30 3030 206d 6f64 656c 7320 6f66  22,000 models of
+00000640: 2074 6865 2063 7275 7374 2d6d 616e 746c   the crust-mantl
+00000650: 6520 696e 7465 7266 6163 6520 7061 7261  e interface para
+00000660: 6d65 7465 7269 7a65 6420 6279 2072 6566  meterized by ref
+00000670: 6572 656e 6365 2069 6e74 6572 696f 7220  erence interior 
+00000680: 6d6f 6465 6c73 2c20 6372 7573 7461 6c20  models, crustal 
+00000690: 7468 6963 6b6e 6573 7320 6174 2074 6865  thickness at the
+000006a0: 2049 6e53 6967 6874 206c 616e 6469 6e67   InSight landing
+000006b0: 2c20 616e 6420 686f 6d6f 6765 6e65 6f75  , and homogeneou
+000006c0: 732f 696e 686f 6d6f 6765 6e65 6f75 7320  s/inhomogeneous 
+000006d0: 6372 7573 7461 6c20 6465 6e73 6974 6965  crustal densitie
+000006e0: 7320 6163 726f 7373 2074 6865 2064 6963  s across the dic
+000006f0: 686f 746f 6d79 2e20 0d0a 0d0a 266e 6273  hotomy. ....&nbs
+00000700: 703b 0d0a 0d0a 2d20 4578 616d 706c 6520  p;....- Example 
+00000710: 313a 2054 6f70 6f67 7261 7068 792c 204d  1: Topography, M
+00000720: 6f68 6f2c 2061 6e64 2063 7275 7374 616c  oho, and crustal
+00000730: 2074 6869 636b 6e65 7373 206f 6620 7468   thickness of th
+00000740: 6520 5661 6c6c 6573 204d 6172 696e 6572  e Valles Mariner
+00000750: 6973 2072 6567 696f 6e2e 204d 6f64 656c  is region. Model
+00000760: 2070 6172 616d 6574 6572 7320 6172 6520   parameters are 
+00000770: 3431 206b 6d20 6372 7573 7461 6c20 7468  41 km crustal th
+00000780: 6963 6b6e 6573 7320 6174 2074 6865 2049  ickness at the I
+00000790: 6e53 6967 6874 206c 616e 6469 6e67 2c20  nSight landing, 
+000007a0: 322c 3930 3020 6b67 2f6d 5e33 2063 7275  2,900 kg/m^3 cru
+000007b0: 7374 616c 2064 656e 7369 7479 2069 6e20  stal density in 
+000007c0: 7468 6520 4e6f 7274 682c 2061 6e64 2032  the North, and 2
+000007d0: 2c37 3030 206b 672f 6d5e 3320 6372 7573  ,700 kg/m^3 crus
+000007e0: 7461 6c20 6465 6e73 6974 7920 696e 2074  tal density in t
+000007f0: 6865 2053 6f75 7468 2e0d 0a0d 0a3c 7020  he South.....<p 
+00000800: 616c 6967 6e3d 2263 656e 7465 7222 3e0d  align="center">.
+00000810: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000820: 733a 2f2f 6669 6c65 732e 6361 7462 6f78  s://files.catbox
+00000830: 2e6d 6f65 2f74 6e6b 3969 6f2e 706e 6722  .moe/tnk9io.png"
+00000840: 3e0d 0a20 2020 203c 212d 2d20 3c69 6d67  >..    <!-- <img
+00000850: 2073 7263 3d22 646f 6373 2f66 6967 7572   src="docs/figur
+00000860: 6573 2f43 7275 7374 5f76 6172 696f 7573  es/Crust_various
+00000870: 5f56 616c 6c65 734d 6172 696e 6572 6973  _VallesMarineris
+00000880: 2e70 6e67 223e 202d 2d3e 0d0a 2020 2020  .png"> -->..    
+00000890: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000008a0: 2f2f 6669 6c65 732e 6361 7462 6f78 2e6d  //files.catbox.m
+000008b0: 6f65 2f74 6e6b 3969 6f2e 706e 6722 3e0d  oe/tnk9io.png">.
+000008c0: 0a20 203c 2f61 3e0d 0a3c 2f70 3e0d 0a0d  .  </a>..</p>...
+000008d0: 0a0d 0a52 6563 7265 6174 6520 7769 7468  ...Recreate with
+000008e0: 3a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  :..```python..fr
+000008f0: 6f6d 2072 6564 706c 616e 6574 2069 6d70  om redplanet imp
+00000900: 6f72 7420 4372 7573 740d 0a6c 6f6e 7320  ort Crust..lons 
+00000910: 3d20 282d 3130 302c 2d32 3029 0d0a 6c61  = (-100,-20)..la
+00000920: 7473 203d 2028 2d36 302c 3430 290d 0a43  ts = (-60,40)..C
+00000930: 7275 7374 2e6c 6f61 645f 6d6f 6465 6c28  rust.load_model(
+00000940: 5249 4d3d 274b 6861 6e32 3032 3227 2c20  RIM='Khan2022', 
+00000950: 696e 7369 6768 745f 7468 6963 6b6e 6573  insight_thicknes
+00000960: 733d 3431 2c20 7268 6f5f 6e6f 7274 683d  s=41, rho_north=
+00000970: 3239 3030 2c20 7268 6f5f 736f 7574 683d  2900, rho_south=
+00000980: 3237 3030 290d 0a43 7275 7374 2e76 6973  2700)..Crust.vis
+00000990: 7561 6c69 7a65 2871 7561 6e74 6974 793d  ualize(quantity=
+000009a0: 2774 6f70 6f27 2c20 6c6f 6e5f 626f 756e  'topo', lon_boun
+000009b0: 6473 3d6c 6f6e 732c 206c 6174 5f62 6f75  ds=lons, lat_bou
+000009c0: 6e64 733d 6c61 7473 2c20 6772 6964 5f73  nds=lats, grid_s
+000009d0: 7061 6369 6e67 3d30 2e31 290d 0a43 7275  pacing=0.1)..Cru
+000009e0: 7374 2e76 6973 7561 6c69 7a65 2871 7561  st.visualize(qua
+000009f0: 6e74 6974 793d 276d 6f68 6f27 2c20 6c6f  ntity='moho', lo
+00000a00: 6e5f 626f 756e 6473 3d6c 6f6e 732c 206c  n_bounds=lons, l
+00000a10: 6174 5f62 6f75 6e64 733d 6c61 7473 2c20  at_bounds=lats, 
+00000a20: 6f76 6572 6c61 793d 5472 7565 2c20 6772  overlay=True, gr
+00000a30: 6964 5f73 7061 6369 6e67 3d30 2e33 290d  id_spacing=0.3).
+00000a40: 0a43 7275 7374 2e76 6973 7561 6c69 7a65  .Crust.visualize
+00000a50: 2871 7561 6e74 6974 793d 2774 6869 636b  (quantity='thick
+00000a60: 272c 206c 6f6e 5f62 6f75 6e64 733d 6c6f  ', lon_bounds=lo
+00000a70: 6e73 2c20 6c61 745f 626f 756e 6473 3d6c  ns, lat_bounds=l
+00000a80: 6174 732c 206f 7665 726c 6179 3d54 7275  ats, overlay=Tru
+00000a90: 652c 2067 7269 645f 7370 6163 696e 673d  e, grid_spacing=
+00000aa0: 302e 3329 0d0a 6060 600d 0a0d 0a26 6e62  0.3)..```....&nb
+00000ab0: 7370 3b0d 0a0d 0a2d 2045 7861 6d70 6c65  sp;....- Example
+00000ac0: 2032 3a20 4372 7573 7461 6c20 7468 6963   2: Crustal thic
+00000ad0: 6b6e 6573 7320 7072 6f66 696c 6520 6f66  kness profile of
+00000ae0: 2048 656e 7279 2043 7261 7465 7220 7769   Henry Crater wi
+00000af0: 7468 2076 6172 696f 7573 2063 7275 7374  th various crust
+00000b00: 2d6d 616e 746c 6520 696e 7465 7266 6163  -mantle interfac
+00000b10: 6520 6d6f 6465 6c73 2e0d 0a0d 0a3c 7020  e models.....<p 
+00000b20: 616c 6967 6e3d 2263 656e 7465 7222 3e0d  align="center">.
+00000b30: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000b40: 733a 2f2f 6669 6c65 732e 6361 7462 6f78  s://files.catbox
+00000b50: 2e6d 6f65 2f6e 6e6e 6d33 6c2e 706e 6722  .moe/nnnm3l.png"
+00000b60: 3e0d 0a20 2020 203c 212d 2d20 3c69 6d67  >..    <!-- <img
+00000b70: 2073 7263 3d22 646f 6373 2f66 6967 7572   src="docs/figur
+00000b80: 6573 2f43 7275 7374 5f74 6869 636b 2d70  es/Crust_thick-p
+00000b90: 726f 6669 6c65 5f48 656e 7279 2e70 6e67  rofile_Henry.png
+00000ba0: 223e 202d 2d3e 0d0a 2020 2020 3c69 6d67  "> -->..    <img
+00000bb0: 2077 6964 7468 3d22 3730 3022 2073 7263   width="700" src
+00000bc0: 3d22 6874 7470 733a 2f2f 6669 6c65 732e  ="https://files.
+00000bd0: 6361 7462 6f78 2e6d 6f65 2f6e 6e6e 6d33  catbox.moe/nnnm3
+00000be0: 6c2e 706e 6722 3e0d 0a20 203c 2f61 3e0d  l.png">..  </a>.
+00000bf0: 0a3c 2f70 3e0d 0a0d 0a0d 0a52 6563 7265  .</p>......Recre
+00000c00: 6174 6520 7769 7468 3a20 5365 6520 7365  ate with: See se
+00000c10: 6374 696f 6e20 322e 3220 696e 205b 6465  ction 2.2 in [de
+00000c20: 6d6f 2e69 7079 6e62 5d28 6874 7470 733a  mo.ipynb](https:
+00000c30: 2f2f 6769 7468 7562 2e63 6f6d 2f48 756d  //github.com/Hum
+00000c40: 626f 6c64 742d 5065 6e67 7569 6e2f 7265  boldt-Penguin/re
+00000c50: 6470 6c61 6e65 742f 626c 6f62 2f6d 6169  dplanet/blob/mai
+00000c60: 6e2f 646f 6373 2f6e 6f74 6562 6f6f 6b73  n/docs/notebooks
+00000c70: 2f64 656d 6f2f 6465 6d6f 2e69 7079 6e62  /demo/demo.ipynb
+00000c80: 292e 0d0a 0d0a 266e 6273 703b 0d0a 0d0a  ).....&nbsp;....
+00000c90: 2d2d 2d0d 0a0d 0a23 2044 6f63 756d 656e  ---....# Documen
+00000ca0: 7461 7469 6f6e 0d0a 0d0a 3c21 2d2d 2046  tation....<!-- F
+00000cb0: 6f72 2061 206d 6f72 6520 696e 2d64 6570  or a more in-dep
+00000cc0: 7468 2074 7574 6f72 6961 6c20 696e 2069  th tutorial in i
+00000cd0: 6e74 6572 6163 7469 7665 206e 6f74 6562  nteractive noteb
+00000ce0: 6f6f 6b20 666f 726d 6174 2c20 7365 6520  ook format, see 
+00000cf0: 5b64 6f63 732f 6e6f 7465 626f 6f6b 732f  [docs/notebooks/
+00000d00: 6465 6d6f 2f64 656d 6f2e 6970 796e 625d  demo/demo.ipynb]
+00000d10: 2864 6f63 732f 6e6f 7465 626f 6f6b 732f  (docs/notebooks/
+00000d20: 6465 6d6f 2f64 656d 6f2e 6970 796e 6229  demo/demo.ipynb)
+00000d30: 2e20 2d2d 3e0d 0a46 6f72 2061 206d 6f72  . -->..For a mor
+00000d40: 6520 696e 2d64 6570 7468 2074 7574 6f72  e in-depth tutor
+00000d50: 6961 6c20 696e 2069 6e74 6572 6163 7469  ial in interacti
+00000d60: 7665 206e 6f74 6562 6f6f 6b20 666f 726d  ve notebook form
+00000d70: 6174 2c20 7365 6520 5b64 656d 6f2e 6970  at, see [demo.ip
+00000d80: 796e 625d 2868 7474 7073 3a2f 2f67 6974  ynb](https://git
+00000d90: 6875 622e 636f 6d2f 4875 6d62 6f6c 6474  hub.com/Humboldt
+00000da0: 2d50 656e 6775 696e 2f72 6564 706c 616e  -Penguin/redplan
+00000db0: 6574 2f62 6c6f 622f 6d61 696e 2f64 6f63  et/blob/main/doc
+00000dc0: 732f 6e6f 7465 626f 6f6b 732f 6465 6d6f  s/notebooks/demo
+00000dd0: 2f64 656d 6f2e 6970 796e 6229 2e0d 0a0d  /demo.ipynb)....
+00000de0: 0a26 6e62 7370 3b0d 0a0d 0a2d 2d2d 0d0a  .&nbsp;....---..
+00000df0: 0d0a 2320 4c69 6e6b 730d 0a0d 0a2d 2044  ..# Links....- D
+00000e00: 6f6e 2774 2068 6573 6974 6174 6520 746f  on't hesitate to
+00000e10: 2072 6561 6368 206f 7574 3a20 5b7a 6169   reach out: [zai
+00000e20: 6e2e 6572 6973 2e6b 616d 616c 4072 7574  n.eris.kamal@rut
+00000e30: 6765 7273 2e65 6475 5d28 6d61 696c 746f  gers.edu](mailto
+00000e40: 3a7a 6169 6e2e 6572 6973 2e6b 616d 616c  :zain.eris.kamal
+00000e50: 4072 7574 6765 7273 2e65 6475 290d 0a2d  @rutgers.edu)..-
+00000e60: 2041 636b 6e6f 776c 6564 6765 6d65 6e74   Acknowledgement
+00000e70: 733a 205b 646f 6373 2f74 6861 6e6b 732e  s: [docs/thanks.
+00000e80: 7478 745d 2868 7474 7073 3a2f 2f67 6974  txt](https://git
+00000e90: 6875 622e 636f 6d2f 4875 6d62 6f6c 6474  hub.com/Humboldt
+00000ea0: 2d50 656e 6775 696e 2f72 6564 706c 616e  -Penguin/redplan
+00000eb0: 6574 2f62 6c6f 622f 6d61 696e 2f64 6f63  et/blob/main/doc
+00000ec0: 732f 7468 616e 6b73 2e74 7874 290d 0a2d  s/thanks.txt)..-
+00000ed0: 2052 6566 6572 656e 6365 733a 205b 646f   References: [do
+00000ee0: 6373 2f72 6566 6572 656e 6365 732e 7478  cs/references.tx
+00000ef0: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
+00000f00: 622e 636f 6d2f 4875 6d62 6f6c 6474 2d50  b.com/Humboldt-P
+00000f10: 656e 6775 696e 2f72 6564 706c 616e 6574  enguin/redplanet
+00000f20: 2f62 6c6f 622f 6d61 696e 2f64 6f63 732f  /blob/main/docs/
+00000f30: 7265 6665 7265 6e63 6573 2e74 7874 290d  references.txt).
+00000f40: 0a2d 204f 7468 6572 2077 6f72 6b3a 205b  .- Other work: [
+00000f50: 6769 7468 7562 2e63 6f6d 2f48 756d 626f  github.com/Humbo
+00000f60: 6c64 742d 5065 6e67 7569 6e5d 2868 7474  ldt-Penguin](htt
+00000f70: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000f80: 4875 6d62 6f6c 6474 2d50 656e 6775 696e  Humboldt-Penguin
+00000f90: 290d 0a0d 0a                             )....
```

### Comparing `redplanet-0.0.1.dev1/pyproject.toml` & `redplanet-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 
 #######################################################################
 [project]
 
 name = "redplanet" 
-version = "0.0.1.dev1" 
+version = "1.0.0" 
 
 description = "User-friendly access (i.e. APIs) for various Mars datasets and derived geophysics quantities. Create publication-ready plots on the fly or access the underlying data for more involved calculations." 
 readme = "README.md"
 
 authors = [{name = "Zain Eris Kamal", email = "zain.eris.kamal@rutgers.edu" }]
 
 requires-python = ">=3.7"
@@ -62,15 +62,15 @@
 
 
 keywords = ["mars", "geophysics", "grs", "crust", "heat flow"] 
 
 
 # For a list of valid classifiers, see https://pypi.org/classifiers/
 classifiers = [ 
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 5 - Production/Stable",
 
   "Operating System :: OS Independent",
 
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
 
   "Intended Audience :: Developers",
```

### Comparing `redplanet-0.0.1.dev1/src/redplanet/Crust/Crust.py` & `redplanet-1.0.0/src/redplanet/Crust/Crust.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev1/src/redplanet/Crust/__init__.py` & `redplanet-1.0.0/src/redplanet/Crust/__init__.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev1/src/redplanet/GRS/GRS.py` & `redplanet-1.0.0/src/redplanet/GRS/GRS.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev1/src/redplanet/GRS/__init__.py` & `redplanet-1.0.0/src/redplanet/GRS/__init__.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev1/src/redplanet/__init__.py` & `redplanet-1.0.0/src/redplanet/__init__.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev1/src/redplanet/utils.py` & `redplanet-1.0.0/src/redplanet/utils.py`

 * *Files identical despite different names*

### Comparing `redplanet-0.0.1.dev1/src/redplanet.egg-info/PKG-INFO` & `redplanet-1.0.0/src/redplanet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redplanet
-Version: 0.0.1.dev1
+Version: 1.0.0
 Summary: User-friendly access (i.e. APIs) for various Mars datasets and derived geophysics quantities. Create publication-ready plots on the fly or access the underlying data for more involved calculations.
 Author-email: Zain Eris Kamal <zain.eris.kamal@rutgers.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -676,15 +676,15 @@
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: Homepage, https://github.com/Humboldt-Penguin/redplanet
 Project-URL: Author, https://github.com/Humboldt-Penguin
 Keywords: mars,geophysics,grs,crust,heat flow
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
@@ -711,16 +711,18 @@
 Access/visualize chemical abundance maps derived from the 2001 Mars Odyssey Gamma Ray Spectrometer. The original data is defined in 5 degree bins, but this module allows you to programmatically estimate values at exact coordinates by interpolating between points. Concentrations can be extracted for both the shallow subsurface (raw data) and bulk crustal composition (normalized to volatile-free basis, i.e. zero H2O/Cl/Si).
 
 &nbsp;
 
 - Example 1: Iron concentrations in Arabia Terra. Data is normalized to a volatile-free basis (H2O/Cl/Si free), so it is representative of the bulk crustal composition rather than shallow subsurface. 
 
 <p align="center">
-  <!-- <img width="600" src="docs/figures/GRS_fe_norm_ArabiaTerra.png"> -->
-  <img width="600" src="https://files.catbox.moe/irjxsp.png">
+  <a href="https://files.catbox.moe/irjxsp.png">
+    <!-- <img width="600" src="docs/figures/GRS_fe_norm_ArabiaTerra.png"> -->
+    <img width="600" src="https://files.catbox.moe/irjxsp.png">
+  </a>
 </p>
 
 
 
 Recreate with: 
 ```python
 from redplanet import GRS
@@ -744,16 +746,18 @@
 Access/visualize maps of topography, Moho, crustal thickness, and crustal density from spherical harmonics. We offer ~22,000 models of the crust-mantle interface parameterized by reference interior models, crustal thickness at the InSight landing, and homogeneous/inhomogeneous crustal densities across the dichotomy. 
 
 &nbsp;
 
 - Example 1: Topography, Moho, and crustal thickness of the Valles Marineris region. Model parameters are 41 km crustal thickness at the InSight landing, 2,900 kg/m^3 crustal density in the North, and 2,700 kg/m^3 crustal density in the South.
 
 <p align="center">
-  <!-- <img src="docs/figures/Crust_various_VallesMarineris.png"> -->
-  <img src="https://files.catbox.moe/tnk9io.png">
+  <a href="https://files.catbox.moe/tnk9io.png">
+    <!-- <img src="docs/figures/Crust_various_VallesMarineris.png"> -->
+    <img src="https://files.catbox.moe/tnk9io.png">
+  </a>
 </p>
 
 
 Recreate with:
 ```python
 from redplanet import Crust
 lons = (-100,-20)
@@ -765,16 +769,18 @@
 ```
 
 &nbsp;
 
 - Example 2: Crustal thickness profile of Henry Crater with various crust-mantle interface models.
 
 <p align="center">
-  <!-- <img src="docs/figures/Crust_thick-profile_Henry.png"> -->
-  <img src="https://files.catbox.moe/nnnm3l.png">
+  <a href="https://files.catbox.moe/nnnm3l.png">
+    <!-- <img src="docs/figures/Crust_thick-profile_Henry.png"> -->
+    <img width="700" src="https://files.catbox.moe/nnnm3l.png">
+  </a>
 </p>
 
 
 Recreate with: See section 2.2 in [demo.ipynb](https://github.com/Humboldt-Penguin/redplanet/blob/main/docs/notebooks/demo/demo.ipynb).
 
 &nbsp;
```

