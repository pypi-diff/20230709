# Comparing `tmp/sdss_lvmcam-0.3.3.tar.gz` & `tmp/sdss_lvmcam-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmcam-0.3.3.tar", max compression
+gzip compressed data, was "sdss_lvmcam-0.3.5.tar", max compression
```

## Comparing `sdss_lvmcam-0.3.3.tar` & `sdss_lvmcam-0.3.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1504 2023-03-11 16:03:19.543551 sdss_lvmcam-0.3.3/LICENSE.md
--rw-r--r--   0        0        0      976 2023-03-11 16:03:19.543891 sdss_lvmcam-0.3.3/README.md
--rw-r--r--   0        0        0     2433 2023-03-11 16:03:19.555130 sdss_lvmcam-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      465 2023-03-11 16:03:19.555617 sdss_lvmcam-0.3.3/python/lvmcam/__init__.py
--rw-r--r--   0        0        0     1706 2023-03-11 16:03:19.555945 sdss_lvmcam-0.3.3/python/lvmcam/__main__.py
--rw-r--r--   0        0        0       67 2023-03-11 16:03:19.556325 sdss_lvmcam-0.3.3/python/lvmcam/actor/__init__.py
--rw-r--r--   0        0        0     6879 2023-03-11 16:03:19.556672 sdss_lvmcam-0.3.3/python/lvmcam/actor/actor.py
--rw-r--r--   0        0        0     1477 2023-03-11 16:03:19.557208 sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/__init__.py
--rwxr-xr-x   0        0        0     1775 2023-03-11 16:03:19.557589 sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/area.py
--rwxr-xr-x   0        0        0     1609 2023-03-11 16:03:19.557937 sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/binning.py
--rwxr-xr-x   0        0        0     9166 2023-03-11 16:03:19.558291 sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/expose.py
--rw-r--r--   0        0        0      316 2023-03-11 16:03:19.558647 sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/foo.py
--rw-r--r--   0        0        0     1517 2023-03-11 16:03:19.558964 sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/gain.py
--rwxr-xr-x   0        0        0     2440 2023-03-11 16:03:19.559323 sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/reconnect.py
--rwxr-xr-x   0        0        0     1966 2023-03-11 16:03:19.559641 sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/shutter.py
--rw-r--r--   0        0        0     1461 2023-03-11 16:03:19.560096 sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/status.py
--rwxr-xr-x   0        0        0     2040 2023-03-11 16:03:19.560488 sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/temperature.py
--rw-r--r--   0        0        0     1151 2023-03-11 16:03:19.560919 sdss_lvmcam-0.3.3/python/lvmcam/etc/lvm.camera_param.agcam.yml
--rw-r--r--   0        0        0     1258 2023-03-11 16:03:19.561273 sdss_lvmcam-0.3.3/python/lvmcam/etc/lvm.sci.agcam.yml
--rw-r--r--   0        0        0     1021 2023-03-11 16:03:19.561601 sdss_lvmcam-0.3.3/python/lvmcam/etc/lvm.skye.agcam.yml
--rw-r--r--   0        0        0     1251 2023-03-11 16:03:19.561939 sdss_lvmcam-0.3.3/python/lvmcam/etc/lvm.skyw.agcam.yml
--rw-r--r--   0        0        0     1043 2023-03-11 16:03:19.562271 sdss_lvmcam-0.3.3/python/lvmcam/etc/lvm.spec.agcam.yml
--rw-r--r--   0        0        0      464 2023-03-11 16:03:19.562620 sdss_lvmcam-0.3.3/python/lvmcam/exceptions.py
--rw-r--r--   0        0        0       87 2023-03-11 16:03:19.563112 sdss_lvmcam-0.3.3/python/lvmcam/models/__init__.py
--rw-r--r--   0        0        0     1489 2023-03-11 16:03:19.563455 sdss_lvmcam-0.3.3/python/lvmcam/models/camera.py
--rw-r--r--   0        0        0     1360 2023-03-11 16:03:19.563801 sdss_lvmcam-0.3.3/python/lvmcam/models/genicam.py
--rw-r--r--   0        0        0     5184 2023-03-11 16:03:19.564180 sdss_lvmcam-0.3.3/python/lvmcam/models/scraper.py
--rw-r--r--   0        0        0     2158 2023-03-11 16:03:19.564506 sdss_lvmcam-0.3.3/python/lvmcam/models/wcs.py
--rw-r--r--   0        0        0     2272 1970-01-01 00:00:00.000000 sdss_lvmcam-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-09 16:15:57.219075 sdss_lvmcam-0.3.5/LICENSE.md
+-rw-r--r--   0        0        0      976 2023-07-09 16:15:57.219498 sdss_lvmcam-0.3.5/README.md
+-rw-r--r--   0        0        0     2497 2023-07-09 16:15:57.231353 sdss_lvmcam-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      465 2023-07-09 16:15:57.231942 sdss_lvmcam-0.3.5/python/lvmcam/__init__.py
+-rw-r--r--   0        0        0     1706 2023-07-09 16:15:57.232347 sdss_lvmcam-0.3.5/python/lvmcam/__main__.py
+-rw-r--r--   0        0        0       67 2023-07-09 16:15:57.232924 sdss_lvmcam-0.3.5/python/lvmcam/actor/__init__.py
+-rw-r--r--   0        0        0     7070 2023-07-09 16:15:57.233372 sdss_lvmcam-0.3.5/python/lvmcam/actor/actor.py
+-rw-r--r--   0        0        0     1477 2023-07-09 16:15:57.233868 sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/__init__.py
+-rwxr-xr-x   0        0        0     1775 2023-07-09 16:15:57.234305 sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/area.py
+-rwxr-xr-x   0        0        0     1609 2023-07-09 16:15:57.234670 sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/binning.py
+-rwxr-xr-x   0        0        0     9294 2023-07-09 16:15:57.235034 sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/expose.py
+-rw-r--r--   0        0        0      316 2023-07-09 16:15:57.235382 sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/foo.py
+-rw-r--r--   0        0        0     1517 2023-07-09 16:15:57.235720 sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/gain.py
+-rwxr-xr-x   0        0        0     2440 2023-07-09 16:15:57.236061 sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/reconnect.py
+-rwxr-xr-x   0        0        0     1966 2023-07-09 16:15:57.236428 sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/shutter.py
+-rw-r--r--   0        0        0     1461 2023-07-09 16:15:57.236774 sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/status.py
+-rwxr-xr-x   0        0        0     2040 2023-07-09 16:15:57.237169 sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/temperature.py
+-rw-r--r--   0        0        0     1151 2023-07-09 16:15:57.237578 sdss_lvmcam-0.3.5/python/lvmcam/etc/lvm.camera_param.agcam.yml
+-rw-r--r--   0        0        0     1363 2023-07-09 16:15:57.237916 sdss_lvmcam-0.3.5/python/lvmcam/etc/lvm.sci.agcam.yml
+-rw-r--r--   0        0        0     1085 2023-07-09 16:15:57.238240 sdss_lvmcam-0.3.5/python/lvmcam/etc/lvm.skye.agcam.yml
+-rw-r--r--   0        0        0     1315 2023-07-09 16:15:57.238569 sdss_lvmcam-0.3.5/python/lvmcam/etc/lvm.skyw.agcam.yml
+-rw-r--r--   0        0        0     1296 2023-07-09 16:15:57.238900 sdss_lvmcam-0.3.5/python/lvmcam/etc/lvm.spec.agcam.yml
+-rw-r--r--   0        0        0      464 2023-07-09 16:15:57.239239 sdss_lvmcam-0.3.5/python/lvmcam/exceptions.py
+-rw-r--r--   0        0        0       87 2023-07-09 16:15:57.239702 sdss_lvmcam-0.3.5/python/lvmcam/models/__init__.py
+-rw-r--r--   0        0        0     1640 2023-07-09 16:15:57.240205 sdss_lvmcam-0.3.5/python/lvmcam/models/camera.py
+-rw-r--r--   0        0        0     1360 2023-07-09 16:15:57.240606 sdss_lvmcam-0.3.5/python/lvmcam/models/genicam.py
+-rw-r--r--   0        0        0     5184 2023-07-09 16:15:57.240994 sdss_lvmcam-0.3.5/python/lvmcam/models/scraper.py
+-rw-r--r--   0        0        0     2194 2023-07-09 16:15:57.241348 sdss_lvmcam-0.3.5/python/lvmcam/models/wcs.py
+-rw-r--r--   0        0        0     2186 1970-01-01 00:00:00.000000 sdss_lvmcam-0.3.5/PKG-INFO
```

### Comparing `sdss_lvmcam-0.3.3/LICENSE.md` & `sdss_lvmcam-0.3.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/README.md` & `sdss_lvmcam-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/pyproject.toml` & `sdss_lvmcam-0.3.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "sdss-lvmcam"
-version = "0.3.3"
+version = "0.3.5"
 description = "The package for lvmcam"
-authors = ["Mingyu Jeon <mgjeon@khu.ac.kr>", "Sumin Lee <lxmark888@khu.ac.kr>"]
+authors = ["Florian Briegel <briegel@mpia.de>"]
+maintainers = ["Florian Briegel <briegel@mpia.de>", "José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmcam"
 repository = "https://github.com/sdss/lvmcam"
 documentation = "https://sdss-lvmcam.readthedocs.org"
 keywords = ["astronomy", "software"]
 classifiers = [
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/__main__.py` & `sdss_lvmcam-0.3.5/python/lvmcam/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/actor/actor.py` & `sdss_lvmcam-0.3.5/python/lvmcam/actor/actor.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,20 @@
         self.exposure_state = {}
         self.log.debug(f"{config.get('scraper', [])}")
         self.scraper_store = ScraperDataStore(self, config.get("scraper", {}))
 
         self.site = Site(name=config.get("site", "LCO"))
         self.log.info(f"Site: {config.get('site', 'LCO')}")
 
+        act_cfg = config.get("actor")
+        if act_cfg is None:
+            self.bench = ""
+        else:
+            self.bench = act_cfg["name"]
+
         # but south-> north at LCO
         if self.site.lat > 40.0:
             azang = 180  # MPIA
         else:
             azang = 0  # LCO, APO, KHU
 
         medSign = -1
@@ -160,15 +166,17 @@
             try:
                 cam = await self.camera_system.add_camera(name=camera, actor=self)
                 self.log.debug(f"camname {camera}")
                 self.log.debug(f"basename {self.basename}")
                 self.log.debug(f"dirname {self.dirname}")
 
                 cam.image_namer = ImageNamer(
-                    basename=self.basename, dirname=self.dirname, camera=cam
+                    basename=self.basename,
+                    dirname=self.dirname,
+                    camera=cam,
                 )
                 cam.fits_model = FITSModel(
                     [
                         Extension(
                             data="raw",
                             header_model=header_model,
                             compressed=None,
```

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/__init__.py` & `sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/area.py` & `sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/area.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/binning.py` & `sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/binning.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/expose.py` & `sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/expose.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,21 @@
     "-s",
     type=int,
     default=1,
     show_default=True,
     help="Number of images to stack.",
 )
 @click.option(
+    "-n",
+    "--num",
+    type=int,
+    default=None,
+    help="Sequence number for this exposure filename.",
+)
+@click.option(
     "--no-postprocess",
     is_flag=True,
     help="Skip the post-process step, if defined.",
 )
 @click.option(
     "--ra_h",
     type=float,
@@ -289,15 +296,15 @@
                         stack,
                         filename,
                         no_postprocess,
                         **exposure_kwargs,
                     )
                 )
             )
-            await asyncio.sleep(0.100)  # dirty 1G fix
+            # await asyncio.sleep(0.1)  # dirty 1G fix
 
         results = await asyncio.gather(*jobs)
         command.actor.listener.remove_callback(report_exposure_state_partial)
 
         status = {}
         for camera in cameras:
             state = command.actor.exposure_state[camera.name].get("state", "NA")
```

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/gain.py` & `sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/gain.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/reconnect.py` & `sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/reconnect.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/shutter.py` & `sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/shutter.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/status.py` & `sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/actor/commands/temperature.py` & `sdss_lvmcam-0.3.5/python/lvmcam/actor/commands/temperature.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/etc/lvm.camera_param.agcam.yml` & `sdss_lvmcam-0.3.5/python/lvmcam/etc/lvm.camera_param.agcam.yml`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/etc/lvm.sci.agcam.yml` & `sdss_lvmcam-0.3.5/python/lvmcam/etc/lvm.sci.agcam.yml`

 * *Files 20% similar despite different names*

```diff
@@ -22,43 +22,47 @@
   lvm.tel:
     temperature: bentemp
     humidity: benhum
     pressure: benpress
 
 cameras:
   east:
+    telescope: sci
     descr: 'Guider Camera Science East'
 
     # araviscam
     uid: 19283186
     ip: 10.8.38.111
 
     genicam_params:
       bool:
-        ReverseX: True
+        ReverseX: False
+        ReverseY: True
 
     # skymakercam
     instpar: lvm_age_cam
 
-  center:
-    descr: 'Guider Camera Science Center'
-    # araviscam
-    uid: 22126027
-    ip: 10.8.38.119
-
-    pixsize: 4.5
+  # center:
+  #   telescope: sci
+  #   descr: 'Guider Camera Science Center'
+  #   # araviscam
+  #   uid: 22126027
+  #   ip: 10.8.38.119
+
+  #   pixsize: 4.5
+
+  #   genicam_params:
+  #     string:
+  #       PixelFormat: 'BayerGB16'
 
-    genicam_params:
-      string:
-        PixelFormat: 'BayerGB16'
-
-    # skymakercam
-    instpar: lvm_agc_cam
+  #   # skymakercam
+  #   instpar: lvm_agc_cam
 
   west:
+    telescope: sci
     descr: 'Guider Camera Science West'
 
     # araviscam
     uid: 19283169
     ip: 10.8.38.112
 
     genicam_params:
```

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/etc/lvm.skye.agcam.yml` & `sdss_lvmcam-0.3.5/python/lvmcam/etc/lvm.skye.agcam.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,28 +22,31 @@
   lvm.tel:
     temperature: bentemp
     humidity: benhum
     pressure: benpress
 
 cameras:
   east:
+    telescope: skye
     descr: 'Guider Camera Skye East'
 
     # araviscam
     uid: 19283198
     ip: 10.8.38.113
 
     genicam_params:
       bool:
-        ReverseX: True
+        ReverseX: False
+        ReverseY: True
 
     # skymakercam
     instpar: lvm_age_cam
 
   west:
+    telescope: skye
     descr: 'Guider Camera Skye West'
 
     # araviscam
     uid: 19283179
     ip: 10.8.38.114
 
     genicam_params:
```

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/etc/lvm.skyw.agcam.yml` & `sdss_lvmcam-0.3.5/python/lvmcam/etc/lvm.skyw.agcam.yml`

 * *Files 15% similar despite different names*

```diff
@@ -26,27 +26,30 @@
     lvm.tel:
       temperature: bentempi
       temperature_enclosure: bentempo
       humidity_enclosure: benhumo
 
 cameras:
   east:
+    telescope: skyw
     descr: 'Guider Camera SkyW East'
 
     # araviscam
     uid: 19283195
     ip: 10.8.38.115
 
     genicam_params:
       bool:
-        ReverseX: True
+        ReverseX: False
+        ReverseY: True
 
     # skymakercam
     instpar: lvm_age_cam
   west:
+    telescope: skyw
     descr: 'Guider Camera SkyW West'
 
     # araviscam
     uid: 19283190
     ip: 10.8.38.116
 
     genicam_params:
```

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/etc/lvm.spec.agcam.yml` & `sdss_lvmcam-0.3.5/python/lvmcam/etc/lvm.spec.agcam.yml`

 * *Files 26% similar despite different names*

```diff
@@ -15,36 +15,43 @@
     axis0.position_timestamp: axis0_position_timestamp_s
     axis1.position_degs: axis1_position_d
     axis1.position_timestamp: axis1_position_timestamp_s
 
   lvm.spec.foc:
     Position: foc_dt
 
+  # Note the following is virtual: there is no km on this bench
   lvm.spec.km:
     Position: km_d
     DeviceEncoder.Position: km_s
 
   lvm.tel:
     temperature: bentempi
     temperature_enclosure: bentempo
     humidity_enclosure: benhumo
 
 cameras:
   east:
+    telescope: spec
     descr: 'Guider Camera Spec East'
 
     # araviscam
     uid: 19283200
     ip: 10.8.38.117
 
     genicam_params:
       bool:
-        ReverseX: True
+        ReverseX: False
+        ReverseY: True
 
     # skymakercam
     instpar: lvm_age_cam
 
+  # There is no west camera on this bench.
+  # Early CAD documentation of late 2021 shew the camera
+  # as a 'west', but as build it is 'east'.
+
 actor:
   name: lvm.spec.agcam
   host: localhost
   port: 5672
   log_dir: '/data/logs/lvm.spec.agcam'
```

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/models/camera.py` & `sdss_lvmcam-0.3.5/python/lvmcam/models/camera.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,21 @@
 from __future__ import annotations
 
 from basecam.models import Card, CardGroup
 
 
 CameraCards = CardGroup(
     [
-        Card("OBSERVAT", "{__camera__.actor.site}", "Observatory", default=""),
-        Card("INSTRUME", "LVM", "SDSS-V Local Volume Mapper"),
+        Card("OBSERVAT", value="LCO", comment="Observatory"),
+        Card(
+            "TELESCOP",
+            value="{__exposure__.camera.telescope}",
+            comment="Telescope that took the image",
+        ),
+        Card("INSTRUME", value="LVM", comment="SDSS-V Local Volume Mapper"),
         Card("GAIN", value="{__exposure__.camera.gain}", comment="[ct] Camera gain"),
         Card(
             "BINX",
             value="{__exposure__.camera.binning[0]}",
             comment="[pix] Binning along axis 1",
         ),
         Card(
```

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/models/genicam.py` & `sdss_lvmcam-0.3.5/python/lvmcam/models/genicam.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/models/scraper.py` & `sdss_lvmcam-0.3.5/python/lvmcam/models/scraper.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmcam-0.3.3/python/lvmcam/models/wcs.py` & `sdss_lvmcam-0.3.5/python/lvmcam/models/wcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
         wcs = exposure.camera.actor.sid.to_wcs(
             exposure.camera.actor.site,
             target,
             None,
             exposure.camera.actor.ambi,
             exposure.scraper_store.get("km_s", 0.0),
-            exposure.camera.name,
+            exposure.camera.actor.bench + " " + exposure.camera.name,
             config_get(
                 exposure.camera.camera_params,
                 "genicam_params.bool.ReverseX",
                 False,
             ),
             config_get(
                 exposure.camera.camera_params,
```

### Comparing `sdss_lvmcam-0.3.3/PKG-INFO` & `sdss_lvmcam-0.3.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: sdss-lvmcam
-Version: 0.3.3
+Version: 0.3.5
 Summary: The package for lvmcam
 Home-page: https://github.com/sdss/lvmcam
 License: BSD-3-Clause
 Keywords: astronomy,software
-Author: Mingyu Jeon
-Author-email: mgjeon@khu.ac.kr
+Author: Florian Briegel
+Author-email: briegel@mpia.de
+Maintainer: Florian Briegel
+Maintainer-email: briegel@mpia.de
 Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: sdss-araviscam (>=0.1.91)
 Requires-Dist: sdss-basecam (>=0.7.1,<0.8.0)
 Requires-Dist: sdss-cluplus (>=0.2.10)
 Requires-Dist: sdss-skymakercam (>=0.0.6)
 Project-URL: Documentation, https://sdss-lvmcam.readthedocs.org
```

