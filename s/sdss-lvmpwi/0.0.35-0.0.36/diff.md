# Comparing `tmp/sdss_lvmpwi-0.0.35.tar.gz` & `tmp/sdss_lvmpwi-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmpwi-0.0.35.tar", max compression
+gzip compressed data, was "sdss_lvmpwi-0.0.36.tar", max compression
```

## Comparing `sdss_lvmpwi-0.0.35.tar` & `sdss_lvmpwi-0.0.36.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0     1515 2023-03-11 18:52:13.751863 sdss_lvmpwi-0.0.35/LICENSE
--rw-r--r--   0        0        0     4446 2023-03-11 18:52:13.751863 sdss_lvmpwi-0.0.35/README.md
--rw-r--r--   0        0        0       97 2023-03-11 18:52:13.751863 sdss_lvmpwi-0.0.35/config/80-arduino_0666.rules
--rw-r--r--   0        0        0       97 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/80-planewave_0666.rules
--rw-r--r--   0        0        0     1330 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/2021-11-18-working-on-pier-after-tuning.pxp
--rw-r--r--   0        0        0     1201 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/20211118-modell.pxp
--rw-r--r--   0        0        0    21754 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/2022-10-25-2143-only-new-stars.pxp
--rw-r--r--   0        0        0    26507 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/2022-10-25-2223-35stars-8arcsec-rms.pxp
--rw-r--r--   0        0        0    30710 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/2022-12-12.pxp
--rw-r--r--   0        0        0     1371 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/20221010-modell.pxp
--rw-r--r--   0        0        0    16656 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/20221016-2330-48stars.pxp
--rw-r--r--   0        0        0    17397 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/20221016-2342-56stars.pxp
--rw-r--r--   0        0        0    18717 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/20221017-0045-63stars.pxp
--rw-r--r--   0        0        0     1581 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-1.pxp
--rw-r--r--   0        0        0     1959 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-3.pxp
--rw-r--r--   0        0        0     2147 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-4.pxp
--rw-r--r--   0        0        0     2336 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-5.pxp
--rw-r--r--   0        0        0     2527 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-6.pxp
--rw-r--r--   0        0        0     2716 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-7.pxp
--rw-r--r--   0        0        0     1394 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw.pxp
--rw-r--r--   0        0        0      586 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/Settings/GUI.cfg
--rw-r--r--   0        0        0      186 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/Settings/LMount.cfg
--rw-r--r--   0        0        0     1055 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/Settings/PWI4.cfg
--rw-r--r--   0        0        0      195 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/config/planewave/pwi/Settings/Telemetry.cfg
--rw-r--r--   0        0        0       97 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/container/80-planewave_0666.rules
--rw-r--r--   0        0        0     3084 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/container/Dockerfile
--rw-r--r--   0        0        0     5318 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/container/__init__.py
--rw-r--r--   0        0        0      759 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/container/container-lvm-hostname-pwi.service
--rw-r--r--   0        0        0      773 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/container/container-lvm-sci-pwi.service
--rw-r--r--   0        0        0      778 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/container/container-lvm-skye-pwi.service
--rw-r--r--   0        0        0      778 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/container/container-lvm-skyw-pwi.service
--rw-r--r--   0        0        0      778 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/container/container-lvm-spec-pwi.service
--rwxr-xr-x   0        0        0     5561 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/container/novnc_server
--rwxr-xr-x   0        0        0     2673 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/container/run-pwi.sh
--rw-r--r--   0        0        0     4940 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/container/xrdp.ini
--rw-r--r--   0        0        0     2585 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/pyproject.toml
--rw-r--r--   0        0        0      720 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/python/lvmpwi/__init__.py
--rw-r--r--   0        0        0     1532 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/python/lvmpwi/__main__.py
--rw-r--r--   0        0        0      191 2023-03-11 18:52:13.755864 sdss_lvmpwi-0.0.35/python/lvmpwi/actor/__init__.py
--rw-r--r--   0        0        0     5560 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/actor/actor.py
--rw-r--r--   0        0        0     1449 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/actor/commands/__init__.py
--rw-r--r--   0        0        0    19523 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/actor/commands/mount.py
--rw-r--r--   0        0        0     6627 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/actor/commands/pointing_model.py
--rw-r--r--   0        0        0      772 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/actor/commands/site.py
--rw-r--r--   0        0        0     2885 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/actor/commands/status.py
--rw-r--r--   0        0        0      944 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/actor/exceptions.py
--rw-r--r--   0        0        0      280 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/etc/lvm.pwi.yml
--rw-r--r--   0        0        0      222 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/pwi/__init__.py
--rw-r--r--   0        0        0     2509 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/pwi/platesolve.py
--rw-r--r--   0        0        0     3694 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/pwi/pwi4_build_model.py
--rw-r--r--   0        0        0    31538 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/pwi/pwi4_client.py
--rw-r--r--   0        0        0      908 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/python/lvmpwi/pwi/pwi4_client_demo.py
--rw-r--r--   0        0        0      220 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/tests/__init__.py
--rw-r--r--   0        0        0     1244 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/tests/conftest.py
--rw-r--r--   0        0        0      403 2023-03-11 18:52:13.759864 sdss_lvmpwi-0.0.35/tests/test_00_container.py
--rw-r--r--   0        0        0     5793 1970-01-01 00:00:00.000000 sdss_lvmpwi-0.0.35/PKG-INFO
+-rw-r--r--   0        0        0     1515 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/LICENSE
+-rw-r--r--   0        0        0     4446 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/README.md
+-rw-r--r--   0        0        0       97 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/80-arduino_0666.rules
+-rw-r--r--   0        0        0       97 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/80-planewave_0666.rules
+-rw-r--r--   0        0        0     1330 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/2021-11-18-working-on-pier-after-tuning.pxp
+-rw-r--r--   0        0        0     1201 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/20211118-modell.pxp
+-rw-r--r--   0        0        0    21754 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/2022-10-25-2143-only-new-stars.pxp
+-rw-r--r--   0        0        0    26507 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/2022-10-25-2223-35stars-8arcsec-rms.pxp
+-rw-r--r--   0        0        0    30710 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/2022-12-12.pxp
+-rw-r--r--   0        0        0     1371 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/20221010-modell.pxp
+-rw-r--r--   0        0        0    16656 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/20221016-2330-48stars.pxp
+-rw-r--r--   0        0        0    17397 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/20221016-2342-56stars.pxp
+-rw-r--r--   0        0        0    18717 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/20221017-0045-63stars.pxp
+-rw-r--r--   0        0        0     1581 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-1.pxp
+-rw-r--r--   0        0        0     1959 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-3.pxp
+-rw-r--r--   0        0        0     2147 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-4.pxp
+-rw-r--r--   0        0        0     2336 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-5.pxp
+-rw-r--r--   0        0        0     2527 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-6.pxp
+-rw-r--r--   0        0        0     2716 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-7.pxp
+-rw-r--r--   0        0        0     1394 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw.pxp
+-rw-r--r--   0        0        0      586 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/Settings/GUI.cfg
+-rw-r--r--   0        0        0      186 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/Settings/LMount.cfg
+-rw-r--r--   0        0        0     1055 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/Settings/PWI4.cfg
+-rw-r--r--   0        0        0      195 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/config/planewave/pwi/Settings/Telemetry.cfg
+-rw-r--r--   0        0        0       97 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/container/80-planewave_0666.rules
+-rw-r--r--   0        0        0     3084 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/container/Dockerfile
+-rw-r--r--   0        0        0     5318 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/container/__init__.py
+-rw-r--r--   0        0        0      759 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/container/container-lvm-hostname-pwi.service
+-rw-r--r--   0        0        0      773 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/container/container-lvm-sci-pwi.service
+-rw-r--r--   0        0        0      778 2023-07-09 16:24:17.748306 sdss_lvmpwi-0.0.36/container/container-lvm-skye-pwi.service
+-rw-r--r--   0        0        0      778 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/container/container-lvm-skyw-pwi.service
+-rw-r--r--   0        0        0      778 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/container/container-lvm-spec-pwi.service
+-rwxr-xr-x   0        0        0     5561 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/container/novnc_server
+-rwxr-xr-x   0        0        0     2673 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/container/run-pwi.sh
+-rw-r--r--   0        0        0     4940 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/container/xrdp.ini
+-rw-r--r--   0        0        0     2585 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/pyproject.toml
+-rw-r--r--   0        0        0      720 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/__init__.py
+-rw-r--r--   0        0        0     1532 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/__main__.py
+-rw-r--r--   0        0        0      191 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/actor/__init__.py
+-rw-r--r--   0        0        0     5560 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/actor/actor.py
+-rw-r--r--   0        0        0     1449 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/actor/commands/__init__.py
+-rw-r--r--   0        0        0    19045 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/actor/commands/mount.py
+-rw-r--r--   0        0        0     6627 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/actor/commands/pointing_model.py
+-rw-r--r--   0        0        0      772 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/actor/commands/site.py
+-rw-r--r--   0        0        0     2885 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/actor/commands/status.py
+-rw-r--r--   0        0        0      944 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/actor/exceptions.py
+-rw-r--r--   0        0        0      280 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/etc/lvm.pwi.yml
+-rw-r--r--   0        0        0      222 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/pwi/__init__.py
+-rw-r--r--   0        0        0     2509 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/pwi/platesolve.py
+-rw-r--r--   0        0        0     3694 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/pwi/pwi4_build_model.py
+-rw-r--r--   0        0        0    31538 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/pwi/pwi4_client.py
+-rw-r--r--   0        0        0      908 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/python/lvmpwi/pwi/pwi4_client_demo.py
+-rw-r--r--   0        0        0      220 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/tests/__init__.py
+-rw-r--r--   0        0        0     1244 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/tests/conftest.py
+-rw-r--r--   0        0        0      403 2023-07-09 16:24:17.752306 sdss_lvmpwi-0.0.36/tests/test_00_container.py
+-rw-r--r--   0        0        0     5642 1970-01-01 00:00:00.000000 sdss_lvmpwi-0.0.36/PKG-INFO
```

### Comparing `sdss_lvmpwi-0.0.35/LICENSE` & `sdss_lvmpwi-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/README.md` & `sdss_lvmpwi-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/2021-11-18-working-on-pier-after-tuning.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/2021-11-18-working-on-pier-after-tuning.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/20211118-modell.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/20211118-modell.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/2022-10-25-2143-only-new-stars.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/2022-10-25-2143-only-new-stars.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/2022-10-25-2223-35stars-8arcsec-rms.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/2022-10-25-2223-35stars-8arcsec-rms.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/2022-12-12.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/2022-12-12.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/20221010-modell.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/20221010-modell.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/20221016-2330-48stars.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/20221016-2330-48stars.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/20221016-2342-56stars.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/20221016-2342-56stars.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/20221017-0045-63stars.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/20221017-0045-63stars.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-1.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-1.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-3.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-3.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-4.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-4.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-5.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-5.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-6.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-6.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw-7.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw-7.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/2023-02-16-lco-skyw.pxp` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/2023-02-16-lco-skyw.pxp`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/Settings/GUI.cfg` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/Settings/GUI.cfg`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/config/planewave/pwi/Settings/PWI4.cfg` & `sdss_lvmpwi-0.0.36/config/planewave/pwi/Settings/PWI4.cfg`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/container/Dockerfile` & `sdss_lvmpwi-0.0.36/container/Dockerfile`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/container/__init__.py` & `sdss_lvmpwi-0.0.36/container/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/container/container-lvm-hostname-pwi.service` & `sdss_lvmpwi-0.0.36/container/container-lvm-hostname-pwi.service`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/container/container-lvm-sci-pwi.service` & `sdss_lvmpwi-0.0.36/container/container-lvm-sci-pwi.service`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/container/container-lvm-skye-pwi.service` & `sdss_lvmpwi-0.0.36/container/container-lvm-skye-pwi.service`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/container/container-lvm-skyw-pwi.service` & `sdss_lvmpwi-0.0.36/container/container-lvm-skyw-pwi.service`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/container/container-lvm-spec-pwi.service` & `sdss_lvmpwi-0.0.36/container/container-lvm-spec-pwi.service`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/container/novnc_server` & `sdss_lvmpwi-0.0.36/container/novnc_server`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/container/run-pwi.sh` & `sdss_lvmpwi-0.0.36/container/run-pwi.sh`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/container/xrdp.ini` & `sdss_lvmpwi-0.0.36/container/xrdp.ini`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/pyproject.toml` & `sdss_lvmpwi-0.0.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmpwi"
-version = "0.0.35"
+version = "0.0.36"
 description = "Lvm Pwi4 Actor"
 authors = ["Florian Briegel <briegel@mpia.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmpwi"
 repository = "https://github.com/sdss/lvmpwi"
 documentation = "https://sdss-lvmpwi.readthedocs.org"
```

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/__init__.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/__main__.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/actor/actor.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/actor/commands/__init__.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/actor/commands/mount.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/actor/commands/mount.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,165 +4,165 @@
 # @Date: 2021-07-06
 # @Filename: mount.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 
 from __future__ import annotations
 
+import asyncio
 from math import nan
 
 import click
-import asyncio
 from clu.command import Command
 
-from lvmpwi.actor.exceptions import *
 from lvmpwi.actor.commands import parser
+from lvmpwi.actor.exceptions import *
 from lvmpwi.pwi import PWI4
 
 
 async def statusPWI(pwi: PWI4, lock: asyncio.Lock):
-
     async with lock:
         return pwi.status()
 
-async def statusTick(actor, pwi: PWI4, delta_time):
 
+async def statusTick(actor, pwi: PWI4, delta_time):
     lock = actor.statusLock
 
     while True:
         try:
             if not lock.locked():
                 status = await statusPWI(pwi, lock)
 
                 actor.write(
-                        "i",
-                        {
-                            "is_slewing": status.mount.is_slewing,
-                            'is_enabled': status.mount.axis0.is_enabled,
-                            "is_tracking": status.mount.is_tracking,
-                            "ra_j2000_hours": status.mount.ra_j2000_hours,
-                            "dec_j2000_degs": status.mount.dec_j2000_degs,
-                            "ra_apparent_hours": status.mount.ra_apparent_hours,
-                            "dec_apparent_degs": status.mount.dec_apparent_degs,
-                            "altitude_degs": status.mount.altitude_degs,
-                            "azimuth_degs": status.mount.azimuth_degs,
-                            "field_angle_here_degs": status.mount.field_angle_here_degs,
-                            "field_angle_rate_at_target_degs_per_sec": status.mount.field_angle_rate_at_target_degs_per_sec,
-                            "field_angle_at_target_degs": status.mount.field_angle_at_target_degs,
-                            "axis0": {
-                                'position_degs': status.mount.axis0.position_degs,
-                                'position_timestamp': status.mount.axis0.position_timestamp_str,
-                            },
-                            "axis1": {
-                                'position_degs': status.mount.axis1.position_degs,
-                                'position_timestamp': status.mount.axis1.position_timestamp_str,
-                            },
-                        }
+                    "i",
+                    {
+                        "is_slewing": status.mount.is_slewing,
+                        "is_enabled": status.mount.axis0.is_enabled,
+                        "is_tracking": status.mount.is_tracking,
+                        "ra_j2000_hours": status.mount.ra_j2000_hours,
+                        "dec_j2000_degs": status.mount.dec_j2000_degs,
+                        "ra_apparent_hours": status.mount.ra_apparent_hours,
+                        "dec_apparent_degs": status.mount.dec_apparent_degs,
+                        "altitude_degs": status.mount.altitude_degs,
+                        "azimuth_degs": status.mount.azimuth_degs,
+                        "field_angle_here_degs": status.mount.field_angle_here_degs,
+                        "field_angle_rate_at_target_degs_per_sec": status.mount.field_angle_rate_at_target_degs_per_sec,
+                        "field_angle_at_target_degs": status.mount.field_angle_at_target_degs,
+                        "axis0": {
+                            "position_degs": status.mount.axis0.position_degs,
+                            "position_timestamp": status.mount.axis0.position_timestamp_str,
+                        },
+                        "axis1": {
+                            "position_degs": status.mount.axis1.position_degs,
+                            "position_timestamp": status.mount.axis1.position_timestamp_str,
+                        },
+                    },
+                    internal=True,
                 )
 
         except Exception as e:
-
             actor.write("i", {"error": e})
 
         await asyncio.sleep(delta_time)
 
+
 @parser.command("setConnected")
 @click.argument("enable", type=bool)
-#@click.option("--statusTick", type=float, default=1)
-async def setConnected(command: Command, pwi: PWI4, enable:bool):
-    """set mount connected true/false """
+# @click.option("--statusTick", type=float, default=1)
+async def setConnected(command: Command, pwi: PWI4, enable: bool):
+    """set mount connected true/false"""
 
     try:
         task = command.actor.statusTask
         if task:
             task.cancel()
 
         if enable:
             status = pwi.mount_connect()
-#            if statustick > 0.0:
-#                command.actor.statusTask = command.actor.loop.create_task(statusTick(command.actor, pwi, statustick))
+        #            if statustick > 0.0:
+        #                command.actor.statusTask = command.actor.loop.create_task(statusTick(command.actor, pwi, statustick))
         else:
             status = pwi.mount_disconnect()
 
-        return command.finish(
-            is_connected = status.mount.is_connected
-        )
+        return command.finish(is_connected=status.mount.is_connected)
 
     except Exception as ex:
         return command.fail(error=ex)
 
 
 @parser.command("setEnabled")
 @click.argument("enable", type=bool)
 @click.option("--axis0", type=bool, default=True)
 @click.option("--axis1", type=bool, default=True)
-async def setEnabled(command: Command, pwi: PWI4, enable:bool, axis0:bool, axis1:bool):
+async def setEnabled(
+    command: Command, pwi: PWI4, enable: bool, axis0: bool, axis1: bool
+):
     """mount enable/disable axis"""
 
     try:
         if axis0:
             pwi.mount_enable(0) if enable else pwi.mount_disable(0)
         if axis1:
             pwi.mount_enable(1) if enable else pwi.mount_disable(1)
-            
+
         await asyncio.sleep(0.1)
 
         status = await statusPWI(pwi, command.actor.statusLock)
         return command.finish(
-            is_enabled = status.mount.axis1.is_enabled & status.mount.axis0.is_enabled,
-            axis0 = {
-                'is_enabled': status.mount.axis0.is_enabled,
+            is_enabled=status.mount.axis1.is_enabled & status.mount.axis0.is_enabled,
+            axis0={
+                "is_enabled": status.mount.axis0.is_enabled,
             },
-            axis1 = {
-                'is_enabled': status.mount.axis1.is_enabled,
+            axis1={
+                "is_enabled": status.mount.axis1.is_enabled,
             },
-    )
+        )
 
     except Exception as ex:
         return command.fail(error=ex)
 
 
 @parser.command("setTracking")
 @click.argument("enable", type=bool)
-async def setTracking(command: Command, pwi: PWI4, enable:bool):
+async def setTracking(command: Command, pwi: PWI4, enable: bool):
     """mount enable/disable tracking"""
 
     try:
         status = pwi.mount_tracking_on() if enable else pwi.mount_tracking_off()
 
         await asyncio.sleep(0.1)
 
         status = await statusPWI(pwi, command.actor.statusLock)
         return command.finish(
-            is_tracking = status.mount.is_tracking,
+            is_tracking=status.mount.is_tracking,
         )
-    
+
     except Exception as ex:
         return command.fail(error=ex)
 
 
 @parser.command()
 async def stop(command: Command, pwi: PWI4):
     """mount stop"""
 
     try:
         status = pwi.mount_stop()
-    
+
         await asyncio.sleep(0.1)
         status = await statusPWI(pwi, command.actor.statusLock)
-        
+
         return command.finish(
             is_slewing=status.mount.is_slewing,
             is_tracking=status.mount.is_tracking,
-            is_enabled = status.mount.axis0.is_enabled and status.mount.axis1.is_enabled,
-            axis0 = {
-                'is_enabled': status.mount.axis0.is_enabled,
+            is_enabled=status.mount.axis0.is_enabled and status.mount.axis1.is_enabled,
+            axis0={
+                "is_enabled": status.mount.axis0.is_enabled,
             },
-            axis1 = {
-                'is_enabled': status.mount.axis1.is_enabled,
+            axis1={
+                "is_enabled": status.mount.axis1.is_enabled,
             },
         )
 
     except Exception as ex:
         return command.fail(error=ex)
 
 
@@ -171,116 +171,110 @@
 async def setSlewTimeConstant(command: Command, pwi: PWI4, time: int):
     """mount set_slew_time_constant"""
 
     try:
         status = pwi.mount_set_slew_time_constant()
 
         return command.finish(
-            is_enabled = status.mount.axis0.is_enabled and status.mount.axis1.is_enabled,
-            axis0 = {
-                'is_enabled': status.mount.axis0.is_enabled,
+            is_enabled=status.mount.axis0.is_enabled and status.mount.axis1.is_enabled,
+            axis0={
+                "is_enabled": status.mount.axis0.is_enabled,
             },
-            axis1 = {
-                'is_enabled': status.mount.axis1.is_enabled,
+            axis1={
+                "is_enabled": status.mount.axis1.is_enabled,
             },
         )
-    
+
     except Exception as ex:
         return command.fail(error=ex)
 
 
 def checkIfMountCanMove(status):
-        if not status.mount.is_connected:
-            raise PwiActorMountNotConnected()
+    if not status.mount.is_connected:
+        raise PwiActorMountNotConnected()
 
-        if not (status.mount.axis0.is_enabled & status.mount.axis1.is_enabled):
-            raise PwiActorMountAxisNotEnabled()
+    if not (status.mount.axis0.is_enabled & status.mount.axis1.is_enabled):
+        raise PwiActorMountAxisNotEnabled()
 
 
 async def waitUntilEndOfSlew(command: Command, pwi: PWI4):
     await asyncio.sleep(0.05)
-    while(True):
+    while True:
         status = await statusPWI(pwi, command.actor.statusLock)
-        
+
         command.info(
             is_slewing=status.mount.is_slewing,
-            
             ra_j2000_hours=status.mount.ra_j2000_hours,
             dec_j2000_degs=status.mount.dec_j2000_degs,
-            
             ra_apparent_hours=status.mount.ra_apparent_hours,
             dec_apparent_degs=status.mount.dec_apparent_degs,
-            
             altitude_degs=status.mount.altitude_degs,
             azimuth_degs=status.mount.azimuth_degs,
-            
             field_angle_here_degs=status.mount.field_angle_here_degs,
             field_angle_rate_at_target_degs_per_sec=status.mount.field_angle_rate_at_target_degs_per_sec,
             field_angle_at_target_degs=status.mount.field_angle_at_target_degs,
-            
-            axis0 = {
-                'dist_to_target_arcsec': status.mount.axis0.dist_to_target_arcsec,
-                'position_degs': status.mount.axis0.position_degs,
-                'rms_error_arcsec': status.mount.axis0.rms_error_arcsec,
-                'servo_error_arcsec': status.mount.axis0.servo_error_arcsec,
-            },
-            
-            axis1 = {
-                'dist_to_target_arcsec': status.mount.axis1.dist_to_target_arcsec,
-                'position_degs': status.mount.axis1.position_degs,
-                'rms_error_arcsec': status.mount.axis1.rms_error_arcsec,
-                'servo_error_arcsec': status.mount.axis1.servo_error_arcsec,
+            axis0={
+                "dist_to_target_arcsec": status.mount.axis0.dist_to_target_arcsec,
+                "position_degs": status.mount.axis0.position_degs,
+                "rms_error_arcsec": status.mount.axis0.rms_error_arcsec,
+                "servo_error_arcsec": status.mount.axis0.servo_error_arcsec,
+            },
+            axis1={
+                "dist_to_target_arcsec": status.mount.axis1.dist_to_target_arcsec,
+                "position_degs": status.mount.axis1.position_degs,
+                "rms_error_arcsec": status.mount.axis1.rms_error_arcsec,
+                "servo_error_arcsec": status.mount.axis1.servo_error_arcsec,
             },
         )
         for i in range(5):
             status = await statusPWI(pwi, command.actor.statusLock)
             if not status.mount.is_slewing:
                 return
             await asyncio.sleep(0.1)
-            
-        
+
+
 @parser.command("gotoRaDecJ2000")
 @click.argument("RA_H", type=float)
 @click.argument("DEG_D", type=float)
 async def gotoRaDecJ2000(command: Command, pwi: PWI4, ra_h: float, deg_d: float):
     """mount goto_ra_dec_j2000"""
 
     try:
         status = pwi.mount_goto_ra_dec_j2000(ra_h, deg_d)
         checkIfMountCanMove(status)
-        
+
         await waitUntilEndOfSlew(command, pwi)
-    
+
         status = await statusPWI(pwi, command.actor.statusLock)
         return command.finish(
-            ra_j2000_hours = status.mount.ra_j2000_hours,
-            dec_j2000_degs = status.mount.dec_j2000_degs,
+            ra_j2000_hours=status.mount.ra_j2000_hours,
+            dec_j2000_degs=status.mount.dec_j2000_degs,
         )
     except Exception as ex:
         return command.fail(error=ex)
 
 
 @parser.command("gotoRaDecApparent")
 @click.argument("RA_H", type=float)
 @click.argument("DEG_D", type=float)
 async def gotoRaDecApparent(command: Command, pwi: PWI4, ra_h: float, deg_d: float):
-    """mount goto_ra_dec_apparent """
+    """mount goto_ra_dec_apparent"""
 
     try:
         status = pwi.mount_goto_ra_dec_apparent(ra_h, deg_d)
         checkIfMountCanMove(status)
 
         await waitUntilEndOfSlew(command, pwi)
-    
+
         status = await statusPWI(pwi, command.actor.statusLock)
         return command.finish(
-            ra_apparent_hours = status.mount.ra_apparent_hours,
-            dec_apparent_degs = status.mount.dec_apparent_degs,
+            ra_apparent_hours=status.mount.ra_apparent_hours,
+            dec_apparent_degs=status.mount.dec_apparent_degs,
         )
-    
+
     except Exception as ex:
         return command.fail(error=ex)
 
 
 @parser.command("gotoAltAzJ2000")
 @click.argument("ALT_D", type=float)
 @click.argument("AZ_D", type=float)
@@ -288,47 +282,47 @@
     """mount goto_alt_az_j2000"""
 
     try:
         status = pwi.mount_goto_alt_az(alt_d, az_d)
         checkIfMountCanMove(status)
 
         await waitUntilEndOfSlew(command, pwi)
-    
+
         status = await statusPWI(pwi, command.actor.statusLock)
         return command.finish(
-            altitude_degs = status.mount.altitude_degs,
-            azimuth_degs = status.mount.azimuth_degs,
+            altitude_degs=status.mount.altitude_degs,
+            azimuth_degs=status.mount.azimuth_degs,
         )
-    
+
     except Exception as ex:
         return command.fail(error=ex)
 
 
 @parser.command("findHome")
 async def findHome(command: Command, pwi: PWI4):
     """mount find_home"""
 
     try:
         status = pwi.mount_find_home()
         checkIfMountCanMove(status)
-    
+
         await waitUntilEndOfSlew(command, pwi)
 
         status = await statusPWI(pwi, command.actor.statusLock)
         return command.finish(
-            dec_j2000_degs = status.mount.dec_j2000_degs,
-            ra_j2000_hours = status.mount.ra_j2000_hours,
-            axis0 = {
-                'position_degs': status.mount.axis0.position_degs,
+            dec_j2000_degs=status.mount.dec_j2000_degs,
+            ra_j2000_hours=status.mount.ra_j2000_hours,
+            axis0={
+                "position_degs": status.mount.axis0.position_degs,
             },
-            axis1 = {
-                'position_degs': status.mount.axis1.position_degs,
+            axis1={
+                "position_degs": status.mount.axis1.position_degs,
             },
         )
-    
+
     except Exception as ex:
         return command.fail(error=ex)
 
 
 @parser.command()
 async def park(command: Command, pwi: PWI4):
     """mount park"""
@@ -337,97 +331,93 @@
         status = pwi.mount_park()
         checkIfMountCanMove(status)
 
         await waitUntilEndOfSlew(command, pwi)
 
         status = await statusPWI(pwi, command.actor.statusLock)
         return command.finish(
-            dec_j2000_degs = status.mount.dec_j2000_degs,
-            ra_j2000_hours = status.mount.ra_j2000_hours,
-            axis0 = {
-                'position_degs': status.mount.axis0.position_degs,
+            dec_j2000_degs=status.mount.dec_j2000_degs,
+            ra_j2000_hours=status.mount.ra_j2000_hours,
+            axis0={
+                "position_degs": status.mount.axis0.position_degs,
             },
-            axis1 = {
-                'position_degs': status.mount.axis1.position_degs,
+            axis1={
+                "position_degs": status.mount.axis1.position_degs,
             },
         )
-    
+
     except Exception as ex:
         return command.fail(error=ex)
 
 
-
 # pwi4 command: mount_set_park_here(self):
 
+
 @parser.command("parkHere")
 async def parkHere(command: Command, pwi: PWI4):
     """mount park"""
 
     try:
         status = pwi.mount_park_here()
         checkIfMountCanMove(status)
 
         await waitUntilEndOfSlew(command, pwi)
 
         status = await statusPWI(pwi, command.actor.statusLock)
         return command.finish(
-            dec_j2000_degs = status.mount.dec_j2000_degs,
-            ra_j2000_hours = status.mount.ra_j2000_hours,
-            axis0 = {
-                'position_degs': status.mount.axis0.position_degs,
+            dec_j2000_degs=status.mount.dec_j2000_degs,
+            ra_j2000_hours=status.mount.ra_j2000_hours,
+            axis0={
+                "position_degs": status.mount.axis0.position_degs,
             },
-            axis1 = {
-                'position_degs': status.mount.axis1.position_degs,
+            axis1={
+                "position_degs": status.mount.axis1.position_degs,
             },
         )
-    
+
     except Exception as ex:
         return command.fail(error=ex)
 
 
 async def waitUntilAxisErrorIsBelowLimit(command: Command, pwi: PWI4, axis_error=0.4):
-    while(True):
+    while True:
         for i in range(5):
             status = await statusPWI(pwi, command.actor.statusLock)
-            if status.mount.axis0.rms_error_arcsec < axis_error and status.mount.axis1.rms_error_arcsec < axis_error:
+            if (
+                status.mount.axis0.rms_error_arcsec < axis_error
+                and status.mount.axis1.rms_error_arcsec < axis_error
+            ):
                 return
             await asyncio.sleep(0.1)
 
         command.info(
             is_slewing=status.mount.is_slewing,
-            
             ra_j2000_hours=status.mount.ra_j2000_hours,
             dec_j2000_degs=status.mount.dec_j2000_degs,
-            
             ra_apparent_hours=status.mount.ra_apparent_hours,
             dec_apparent_degs=status.mount.dec_apparent_degs,
-            
             altitude_degs=status.mount.altitude_degs,
             azimuth_degs=status.mount.azimuth_degs,
-            
             field_angle_here_degs=status.mount.field_angle_here_degs,
             field_angle_rate_at_target_degs_per_sec=status.mount.field_angle_rate_at_target_degs_per_sec,
             field_angle_at_target_degs=status.mount.field_angle_at_target_degs,
-            
-            axis0 = {
-                'dist_to_target_arcsec': status.mount.axis0.dist_to_target_arcsec,
-                'position_degs': status.mount.axis0.position_degs,
-                'rms_error_arcsec': status.mount.axis0.rms_error_arcsec,
-                'servo_error_arcsec': status.mount.axis0.servo_error_arcsec,
-            },
-            
-            axis1 = {
-                'dist_to_target_arcsec': status.mount.axis1.dist_to_target_arcsec,
-                'position_degs': status.mount.axis1.position_degs,
-                'rms_error_arcsec': status.mount.axis1.rms_error_arcsec,
-                'servo_error_arcsec': status.mount.axis1.servo_error_arcsec,
+            axis0={
+                "dist_to_target_arcsec": status.mount.axis0.dist_to_target_arcsec,
+                "position_degs": status.mount.axis0.position_degs,
+                "rms_error_arcsec": status.mount.axis0.rms_error_arcsec,
+                "servo_error_arcsec": status.mount.axis0.servo_error_arcsec,
+            },
+            axis1={
+                "dist_to_target_arcsec": status.mount.axis1.dist_to_target_arcsec,
+                "position_degs": status.mount.axis1.position_degs,
+                "rms_error_arcsec": status.mount.axis1.rms_error_arcsec,
+                "servo_error_arcsec": status.mount.axis1.servo_error_arcsec,
             },
         )
-            
-        
+
 
 @parser.command()
 # AXIS_reset
 @click.option("--ra_reset", type=float, default=nan)
 @click.option("--dec_reset", type=float, default=nan)
 @click.option("--axis0_reset", type=float, default=nan)
 @click.option("--axis1_reset", type=float, default=nan)
@@ -454,78 +444,69 @@
 @click.option("--axis1_set_rate_arcsec_per_sec", type=float, default=nan)
 @click.option("--path_set_rate_arcsec_per_sec", type=float, default=nan)
 @click.option("--transverse_set_rate_arcsec_per_sec", type=float, default=nan)
 # Tolerated axis error (option)
 @click.option("--axis_error", type=float, default=0.4)
 async def offset(command: Command, pwi: PWI4, **kwargs):
     """mount offset
-     
-        One or more of the following offsets can be specified as a keyword argument:
-        AXIS_reset: Clear all position and rate offsets for this axis. Set this to any value to issue the command.
-        AXIS_stop_rate: Set any active offset rate to zero. Set this to any value to issue the command.
-        AXIS_add_arcsec: Increase the current position offset by the specified amount
-        AXIS_set_rate_arcsec_per_sec: Continually increase the offset at the specified rate
-        Where AXIS can be one of:
-        ra: Offset the target Right Ascension coordinate
-        dec: Offset the target Declination coordinate
-        axis0: Offset the mount's primary axis position 
-               (roughly Azimuth on an Alt-Az mount, or RA on In equatorial mount)
-        axis1: Offset the mount's secondary axis position 
-               (roughly Altitude on an Alt-Az mount, or Dec on an equatorial mount)
-        path: Offset along the direction of travel for a moving target
-        transverse: Offset perpendicular to the direction of travel for a moving target
-        For example, to offset axis0 by -30 arcseconds and have it continually increase at 1
-        arcsec/sec, and to also clear any existing offset in the transverse direction,
-        you could call the method like this:
-        mount_offset(axis0_add_arcsec=-30, axis0_set_rate_arcsec_per_sec=1, transverse_reset=0)
-        """
 
-    
+    One or more of the following offsets can be specified as a keyword argument:
+    AXIS_reset: Clear all position and rate offsets for this axis. Set this to any value to issue the command.
+    AXIS_stop_rate: Set any active offset rate to zero. Set this to any value to issue the command.
+    AXIS_add_arcsec: Increase the current position offset by the specified amount
+    AXIS_set_rate_arcsec_per_sec: Continually increase the offset at the specified rate
+    Where AXIS can be one of:
+    ra: Offset the target Right Ascension coordinate
+    dec: Offset the target Declination coordinate
+    axis0: Offset the mount's primary axis position
+           (roughly Azimuth on an Alt-Az mount, or RA on In equatorial mount)
+    axis1: Offset the mount's secondary axis position
+           (roughly Altitude on an Alt-Az mount, or Dec on an equatorial mount)
+    path: Offset along the direction of travel for a moving target
+    transverse: Offset perpendicular to the direction of travel for a moving target
+    For example, to offset axis0 by -30 arcseconds and have it continually increase at 1
+    arcsec/sec, and to also clear any existing offset in the transverse direction,
+    you could call the method like this:
+    mount_offset(axis0_add_arcsec=-30, axis0_set_rate_arcsec_per_sec=1, transverse_reset=0)
+    """
 
     try:
-        status = pwi.mount_offset(**{key: value for key, value in kwargs.items() if value is not nan})
+        status = pwi.mount_offset(
+            **{key: value for key, value in kwargs.items() if value is not nan}
+        )
         checkIfMountCanMove(status)
-        
+
         await waitUntilAxisErrorIsBelowLimit(command, pwi, kwargs["axis_error"])
-        
+
         status = await statusPWI(pwi, command.actor.statusLock)
         return command.finish(
             is_tracking=status.mount.is_tracking,
             is_connected=status.mount.is_connected,
             is_slewing=status.mount.is_slewing,
             is_enabled=status.mount.axis0.is_enabled & status.mount.axis1.is_enabled,
-            
             ra_j2000_hours=status.mount.ra_j2000_hours,
             dec_j2000_degs=status.mount.dec_j2000_degs,
-
             ra_apparent_hours=status.mount.ra_apparent_hours,
             dec_apparent_degs=status.mount.dec_apparent_degs,
-
             altitude_degs=status.mount.altitude_degs,
             azimuth_degs=status.mount.azimuth_degs,
-
             field_angle_rate_at_target_degs_per_sec=status.mount.field_angle_rate_at_target_degs_per_sec,
             field_angle_at_target_degs=status.mount.field_angle_at_target_degs,
             field_angle_here_degs=status.mount.field_angle_here_degs,
-
-            axis0 = {
-                'dist_to_target_arcsec': status.mount.axis0.dist_to_target_arcsec,
-                'is_enabled': status.mount.axis0.is_enabled,
-                'position_degs': status.mount.axis0.position_degs,
-                'rms_error_arcsec': status.mount.axis0.rms_error_arcsec,
-                'servo_error_arcsec': status.mount.axis0.servo_error_arcsec,
-            },
-
-            axis1 = {
-                'dist_to_target_arcsec': status.mount.axis1.dist_to_target_arcsec,
-                'is_enabled': status.mount.axis1.is_enabled,
-                'position_degs': status.mount.axis1.position_degs,
-                'rms_error_arcsec': status.mount.axis1.rms_error_arcsec,
-                'servo_error_arcsec': status.mount.axis1.servo_error_arcsec,
+            axis0={
+                "dist_to_target_arcsec": status.mount.axis0.dist_to_target_arcsec,
+                "is_enabled": status.mount.axis0.is_enabled,
+                "position_degs": status.mount.axis0.position_degs,
+                "rms_error_arcsec": status.mount.axis0.rms_error_arcsec,
+                "servo_error_arcsec": status.mount.axis0.servo_error_arcsec,
+            },
+            axis1={
+                "dist_to_target_arcsec": status.mount.axis1.dist_to_target_arcsec,
+                "is_enabled": status.mount.axis1.is_enabled,
+                "position_degs": status.mount.axis1.position_degs,
+                "rms_error_arcsec": status.mount.axis1.rms_error_arcsec,
+                "servo_error_arcsec": status.mount.axis1.servo_error_arcsec,
             },
         )
 
-
     except Exception as ex:
         return command.fail(error=ex)
-
-
```

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/actor/commands/pointing_model.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/actor/commands/pointing_model.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/actor/commands/site.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/actor/commands/site.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/actor/commands/status.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/actor/exceptions.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/actor/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/pwi/platesolve.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/pwi/platesolve.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/pwi/pwi4_build_model.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/pwi/pwi4_build_model.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/pwi/pwi4_client.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/pwi/pwi4_client.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/python/lvmpwi/pwi/pwi4_client_demo.py` & `sdss_lvmpwi-0.0.36/python/lvmpwi/pwi/pwi4_client_demo.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/tests/conftest.py` & `sdss_lvmpwi-0.0.36/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmpwi-0.0.35/PKG-INFO` & `sdss_lvmpwi-0.0.36/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmpwi
-Version: 0.0.35
+Version: 0.0.36
 Summary: Lvm Pwi4 Actor
 Home-page: https://github.com/sdss/lvmpwi
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: Florian Briegel
 Author-email: briegel@mpia.de
 Requires-Python: >=3.8,<4.0
@@ -13,17 +13,14 @@
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
 Provides-Extra: docs
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: daemonocle (>=1.1.1,<2.0.0)
 Requires-Dist: sdss-clu (>=2.0.0)
 Requires-Dist: sdss-cluplus (>=0.5.0)
```

