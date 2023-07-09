# Comparing `tmp/sdss_lvmtan-0.2.3.tar.gz` & `tmp/sdss_lvmtan-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmtan-0.2.3.tar", max compression
+gzip compressed data, was "sdss_lvmtan-0.2.4.tar", max compression
```

## Comparing `sdss_lvmtan-0.2.3.tar` & `sdss_lvmtan-0.2.4.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1504 2023-03-14 03:33:59.194747 sdss_lvmtan-0.2.3/LICENSE.md
--rw-r--r--   0        0        0     3835 2023-03-14 03:33:59.194977 sdss_lvmtan-0.2.3/README.md
--rw-r--r--   0        0        0      874 2023-03-14 03:33:59.195197 sdss_lvmtan-0.2.3/build.py
--rw-r--r--   0        0        0     2202 2023-03-14 03:33:59.198089 sdss_lvmtan-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       75 2023-03-14 03:33:59.198558 sdss_lvmtan-0.2.3/python/lvmtan/.coverage
--rw-r--r--   0        0        0     6135 2023-03-14 03:33:59.198977 sdss_lvmtan-0.2.3/python/lvmtan/BasdaCluPythonServiceWorker.py
--rw-r--r--   0        0        0     6171 2023-03-14 03:33:59.199322 sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaBaseCluPythonServiceWorker.py
--rw-r--r--   0        0        0     9382 2023-03-14 03:33:59.199677 sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaCluPythonServiceWorker.py
--rw-r--r--   0        0        0    10614 2023-03-14 03:33:59.199963 sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaTrajCluPythonServiceWorker.py
--rw-r--r--   0        0        0     1495 2023-03-14 03:33:59.200278 sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaWheelCluPythonServiceWorker.py
--rw-r--r--   0        0        0     2404 2023-03-14 03:33:59.200554 sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaXCluPythonServiceWorker.py
--rw-r--r--   0        0        0    12681 2023-03-14 03:33:59.200815 sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaXYCluPythonServiceWorker.py
--rw-r--r--   0        0        0     1074 2023-03-14 03:33:59.201085 sdss_lvmtan-0.2.3/python/lvmtan/__init__.py
--rw-r--r--   0        0        0      759 2023-03-14 03:33:59.201504 sdss_lvmtan-0.2.3/python/lvmtan/config/alias.cfg
--rw-r--r--   0        0        0     8229 2023-03-14 03:33:59.201994 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/common/PI_M413.12S_datasheet.conf
--rw-r--r--   0        0        0     8200 2023-03-14 03:33:59.202235 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/common/PI_MICOS_datasheet.conf
--rw-r--r--   0        0        0     8200 2023-03-14 03:33:59.202457 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/common/PI_WHEEL_datasheet.conf
--rw-r--r--   0        0        0     9189 2023-03-14 03:33:59.202678 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/common/datasheetServo.conf
--rw-r--r--   0        0        0     8487 2023-03-14 03:33:59.202892 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/common/datasheetStepper.conf
--rw-r--r--   0        0        0      828 2023-03-14 03:33:59.203098 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.all-sim.conf
--rw-r--r--   0        0        0     1546 2023-03-14 03:33:59.203423 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.all-svr.conf
--rw-r--r--   0        0        0     2860 2023-03-14 03:33:59.203652 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.all.ui
--rw-r--r--   0        0        0      833 2023-03-14 03:33:59.203884 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.moe-mpia.conf
--rw-r--r--   0        0        0      828 2023-03-14 03:33:59.204105 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.moe-sim.conf
--rw-r--r--   0        0        0     1560 2023-03-14 03:33:59.204322 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.moe-svr.conf
--rw-r--r--   0        0        0     6768 2023-03-14 03:33:59.204798 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-dev.conf
--rw-r--r--   0        0        0      277 2023-03-14 03:33:59.205046 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-sim.conf
--rw-r--r--   0        0        0      848 2023-03-14 03:33:59.205312 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-svc.conf
--rw-r--r--   0        0        0      846 2023-03-14 03:33:59.205514 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-svr.conf
--rw-r--r--   0        0        0     7057 2023-03-14 03:33:59.205799 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/km/lvm.sci.km-dev.conf
--rw-r--r--   0        0        0     2144 2023-03-14 03:33:59.206021 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/km/lvm.sci.km-svc.conf
--rw-r--r--   0        0        0     1286 2023-03-14 03:33:59.206255 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/km/lvm.sci.km-svr.conf
--rw-r--r--   0        0        0      335 2023-03-14 03:33:59.206463 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/lvm.sci-sim.conf
--rw-r--r--   0        0        0      912 2023-03-14 03:33:59.206694 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/lvm.sci-svr.conf
--rw-r--r--   0        0        0     6769 2023-03-14 03:33:59.207208 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-dev.conf
--rw-r--r--   0        0        0      278 2023-03-14 03:33:59.207426 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-sim.conf
--rw-r--r--   0        0        0      965 2023-03-14 03:33:59.207645 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-svc.conf
--rw-r--r--   0        0        0      849 2023-03-14 03:33:59.207859 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-svr.conf
--rw-r--r--   0        0        0     7057 2023-03-14 03:33:59.208142 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/km/lvm.skye.km-dev.conf
--rw-r--r--   0        0        0     2161 2023-03-14 03:33:59.208342 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/km/lvm.skye.km-svc.conf
--rw-r--r--   0        0        0     1286 2023-03-14 03:33:59.208539 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/km/lvm.skye.km-svr.conf
--rw-r--r--   0        0        0      335 2023-03-14 03:33:59.208737 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/lvm.skye-sim.conf
--rw-r--r--   0        0        0      917 2023-03-14 03:33:59.208990 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/lvm.skye-svr.conf
--rw-r--r--   0        0        0     6770 2023-03-14 03:33:59.209443 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-dev.conf
--rw-r--r--   0        0        0      269 2023-03-14 03:33:59.209708 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-sim.conf
--rw-r--r--   0        0        0      830 2023-03-14 03:33:59.209953 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-svc.conf
--rw-r--r--   0        0        0      849 2023-03-14 03:33:59.210208 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-svr.conf
--rw-r--r--   0        0        0     7057 2023-03-14 03:33:59.210500 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-dev.conf
--rw-r--r--   0        0        0     2165 2023-03-14 03:33:59.210717 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-svc.conf
--rw-r--r--   0        0        0     1286 2023-03-14 03:33:59.210976 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-svr.conf
--rw-r--r--   0        0        0      335 2023-03-14 03:33:59.211237 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/lvm.skyw-sim.conf
--rw-r--r--   0        0        0      917 2023-03-14 03:33:59.211476 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/lvm.skyw-svr.conf
--rw-r--r--   0        0        0     4743 2023-03-14 03:33:59.211930 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-dev.conf
--rw-r--r--   0        0        0      866 2023-03-14 03:33:59.212183 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-svc.conf
--rw-r--r--   0        0        0      859 2023-03-14 03:33:59.212428 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-svr.conf
--rw-r--r--   0        0        0     6769 2023-03-14 03:33:59.212744 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-dev.conf
--rw-r--r--   0        0        0      269 2023-03-14 03:33:59.213031 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-sim.conf
--rw-r--r--   0        0        0      830 2023-03-14 03:33:59.213255 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-svc.conf
--rw-r--r--   0        0        0      845 2023-03-14 03:33:59.213479 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-svr.conf
--rw-r--r--   0        0        0      352 2023-03-14 03:33:59.213682 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/lvm.spec-sim.conf
--rw-r--r--   0        0        0      917 2023-03-14 03:33:59.213892 sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/lvm.spec-svr.conf
--rw-r--r--   0        0        0     7847 2023-03-14 03:33:59.214254 sdss_lvmtan-0.2.3/python/lvmtan/config/test/derot/test.derot.km-dev.conf
--rw-r--r--   0        0        0      265 2023-03-14 03:33:59.214458 sdss_lvmtan-0.2.3/python/lvmtan/config/test/derot/test.derot.km-sim.conf
--rw-r--r--   0        0        0     2222 2023-03-14 03:33:59.214653 sdss_lvmtan-0.2.3/python/lvmtan/config/test/derot/test.derot.km-svc.conf
--rw-r--r--   0        0        0     1503 2023-03-14 03:33:59.214970 sdss_lvmtan-0.2.3/python/lvmtan/config/test/derot/test.derot.km-svr.conf
--rw-r--r--   0        0        0      269 2023-03-14 03:33:59.215165 sdss_lvmtan-0.2.3/python/lvmtan/config/test/derot/test.derot.km_lab-sim.conf
--rw-r--r--   0        0        0     1738 2023-03-14 03:33:59.215358 sdss_lvmtan-0.2.3/python/lvmtan/config/test/derot/test.derot.km_lab-svr.conf
--rw-r--r--   0        0        0     6431 2023-03-14 03:33:59.215638 sdss_lvmtan-0.2.3/python/lvmtan/config/test/first/test.first.focus_stage-dev.conf
--rw-r--r--   0        0        0      298 2023-03-14 03:33:59.215851 sdss_lvmtan-0.2.3/python/lvmtan/config/test/first/test.first.focus_stage-sim.conf
--rw-r--r--   0        0        0     1081 2023-03-14 03:33:59.216058 sdss_lvmtan-0.2.3/python/lvmtan/config/test/first/test.first.focus_stage-svc.conf
--rw-r--r--   0        0        0      863 2023-03-14 03:33:59.216260 sdss_lvmtan-0.2.3/python/lvmtan/config/test/first/test.first.focus_stage-svr.conf
--rw-r--r--   0        0        0     8229 2023-03-14 03:33:59.216466 sdss_lvmtan-0.2.3/python/lvmtan/config/test/first/test.first.focus_stage_X_datasheet.conf
--rw-r--r--   0        0        0     8229 2023-03-14 03:33:59.216822 sdss_lvmtan-0.2.3/python/lvmtan/config/test/xy/test.xy.stage-datasheet.conf
--rw-r--r--   0        0        0     9377 2023-03-14 03:33:59.217084 sdss_lvmtan-0.2.3/python/lvmtan/config/test/xy/test.xy.stage-dev.conf
--rw-r--r--   0        0        0      274 2023-03-14 03:33:59.217324 sdss_lvmtan-0.2.3/python/lvmtan/config/test/xy/test.xy.stage-sim.conf
--rw-r--r--   0        0        0      947 2023-03-14 03:33:59.217591 sdss_lvmtan-0.2.3/python/lvmtan/config/test/xy/test.xy.stage-svc.conf
--rw-r--r--   0        0        0      843 2023-03-14 03:33:59.217849 sdss_lvmtan-0.2.3/python/lvmtan/config/test/xy/test.xy.stage-svr.conf
--rw-r--r--   0        0        0      493 2023-03-14 03:33:59.218059 sdss_lvmtan-0.2.3/python/lvmtan/exceptions.py
--rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 sdss_lvmtan-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-09 16:26:43.883782 sdss_lvmtan-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0     3835 2023-07-09 16:26:43.883999 sdss_lvmtan-0.2.4/README.md
+-rw-r--r--   0        0        0      874 2023-07-09 16:26:43.884205 sdss_lvmtan-0.2.4/build.py
+-rw-r--r--   0        0        0     2202 2023-07-09 16:26:43.886642 sdss_lvmtan-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-07-09 16:26:43.887081 sdss_lvmtan-0.2.4/python/lvmtan/.coverage
+-rw-r--r--   0        0        0     6135 2023-07-09 16:26:43.887417 sdss_lvmtan-0.2.4/python/lvmtan/BasdaCluPythonServiceWorker.py
+-rw-r--r--   0        0        0     6171 2023-07-09 16:26:43.887670 sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaBaseCluPythonServiceWorker.py
+-rw-r--r--   0        0        0     9382 2023-07-09 16:26:43.887997 sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaCluPythonServiceWorker.py
+-rw-r--r--   0        0        0    10590 2023-07-09 16:26:43.888245 sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaTrajCluPythonServiceWorker.py
+-rw-r--r--   0        0        0     1495 2023-07-09 16:26:43.888491 sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaWheelCluPythonServiceWorker.py
+-rw-r--r--   0        0        0     2404 2023-07-09 16:26:43.888716 sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaXCluPythonServiceWorker.py
+-rw-r--r--   0        0        0    12681 2023-07-09 16:26:43.888926 sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaXYCluPythonServiceWorker.py
+-rw-r--r--   0        0        0     1074 2023-07-09 16:26:43.889130 sdss_lvmtan-0.2.4/python/lvmtan/__init__.py
+-rw-r--r--   0        0        0      759 2023-07-09 16:26:43.889458 sdss_lvmtan-0.2.4/python/lvmtan/config/alias.cfg
+-rw-r--r--   0        0        0     8229 2023-07-09 16:26:43.889935 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/common/PI_M413.12S_datasheet.conf
+-rw-r--r--   0        0        0     8200 2023-07-09 16:26:43.890210 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/common/PI_MICOS_datasheet.conf
+-rw-r--r--   0        0        0     8200 2023-07-09 16:26:43.890462 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/common/PI_WHEEL_datasheet.conf
+-rw-r--r--   0        0        0     9189 2023-07-09 16:26:43.890720 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/common/datasheetServo.conf
+-rw-r--r--   0        0        0     8487 2023-07-09 16:26:43.890990 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/common/datasheetStepper.conf
+-rw-r--r--   0        0        0      828 2023-07-09 16:26:43.891232 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.all-sim.conf
+-rw-r--r--   0        0        0     1546 2023-07-09 16:26:43.891476 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.all-svr.conf
+-rw-r--r--   0        0        0     2860 2023-07-09 16:26:43.891756 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.all.ui
+-rw-r--r--   0        0        0      833 2023-07-09 16:26:43.891998 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.moe-mpia.conf
+-rw-r--r--   0        0        0      828 2023-07-09 16:26:43.892206 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.moe-sim.conf
+-rw-r--r--   0        0        0     1560 2023-07-09 16:26:43.892430 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.moe-svr.conf
+-rw-r--r--   0        0        0     6768 2023-07-09 16:26:43.892872 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-dev.conf
+-rw-r--r--   0        0        0      277 2023-07-09 16:26:43.893100 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-sim.conf
+-rw-r--r--   0        0        0      848 2023-07-09 16:26:43.893308 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-svc.conf
+-rw-r--r--   0        0        0      846 2023-07-09 16:26:43.893623 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-svr.conf
+-rw-r--r--   0        0        0     7057 2023-07-09 16:26:43.893931 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/km/lvm.sci.km-dev.conf
+-rw-r--r--   0        0        0     2144 2023-07-09 16:26:43.894182 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/km/lvm.sci.km-svc.conf
+-rw-r--r--   0        0        0     1286 2023-07-09 16:26:43.894410 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/km/lvm.sci.km-svr.conf
+-rw-r--r--   0        0        0      335 2023-07-09 16:26:43.894625 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/lvm.sci-sim.conf
+-rw-r--r--   0        0        0      912 2023-07-09 16:26:43.894840 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/lvm.sci-svr.conf
+-rw-r--r--   0        0        0     6769 2023-07-09 16:26:43.895228 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-dev.conf
+-rw-r--r--   0        0        0      278 2023-07-09 16:26:43.895455 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-sim.conf
+-rw-r--r--   0        0        0      965 2023-07-09 16:26:43.895683 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-svc.conf
+-rw-r--r--   0        0        0      849 2023-07-09 16:26:43.895904 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-svr.conf
+-rw-r--r--   0        0        0     7057 2023-07-09 16:26:43.896185 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/km/lvm.skye.km-dev.conf
+-rw-r--r--   0        0        0     2161 2023-07-09 16:26:43.896407 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/km/lvm.skye.km-svc.conf
+-rw-r--r--   0        0        0     1286 2023-07-09 16:26:43.896613 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/km/lvm.skye.km-svr.conf
+-rw-r--r--   0        0        0      335 2023-07-09 16:26:43.896820 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/lvm.skye-sim.conf
+-rw-r--r--   0        0        0      917 2023-07-09 16:26:43.897125 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/lvm.skye-svr.conf
+-rw-r--r--   0        0        0     6770 2023-07-09 16:26:43.897506 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-dev.conf
+-rw-r--r--   0        0        0      269 2023-07-09 16:26:43.897722 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-sim.conf
+-rw-r--r--   0        0        0      830 2023-07-09 16:26:43.897933 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-svc.conf
+-rw-r--r--   0        0        0      849 2023-07-09 16:26:43.898151 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-svr.conf
+-rw-r--r--   0        0        0     7057 2023-07-09 16:26:43.898441 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-dev.conf
+-rw-r--r--   0        0        0     2165 2023-07-09 16:26:43.898646 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-svc.conf
+-rw-r--r--   0        0        0     1286 2023-07-09 16:26:43.898882 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-svr.conf
+-rw-r--r--   0        0        0      335 2023-07-09 16:26:43.899147 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/lvm.skyw-sim.conf
+-rw-r--r--   0        0        0      917 2023-07-09 16:26:43.899354 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/lvm.skyw-svr.conf
+-rw-r--r--   0        0        0     4743 2023-07-09 16:26:43.899740 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-dev.conf
+-rw-r--r--   0        0        0      866 2023-07-09 16:26:43.899961 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-svc.conf
+-rw-r--r--   0        0        0      859 2023-07-09 16:26:43.900184 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-svr.conf
+-rw-r--r--   0        0        0     6769 2023-07-09 16:26:43.900467 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-dev.conf
+-rw-r--r--   0        0        0      269 2023-07-09 16:26:43.900683 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-sim.conf
+-rw-r--r--   0        0        0      830 2023-07-09 16:26:43.900895 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-svc.conf
+-rw-r--r--   0        0        0      845 2023-07-09 16:26:43.901099 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-svr.conf
+-rw-r--r--   0        0        0      352 2023-07-09 16:26:43.901295 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/lvm.spec-sim.conf
+-rw-r--r--   0        0        0      917 2023-07-09 16:26:43.901504 sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/lvm.spec-svr.conf
+-rw-r--r--   0        0        0     7847 2023-07-09 16:26:43.902293 sdss_lvmtan-0.2.4/python/lvmtan/config/test/derot/test.derot.km-dev.conf
+-rw-r--r--   0        0        0      265 2023-07-09 16:26:43.902550 sdss_lvmtan-0.2.4/python/lvmtan/config/test/derot/test.derot.km-sim.conf
+-rw-r--r--   0        0        0     2222 2023-07-09 16:26:43.902951 sdss_lvmtan-0.2.4/python/lvmtan/config/test/derot/test.derot.km-svc.conf
+-rw-r--r--   0        0        0     1503 2023-07-09 16:26:43.903361 sdss_lvmtan-0.2.4/python/lvmtan/config/test/derot/test.derot.km-svr.conf
+-rw-r--r--   0        0        0      269 2023-07-09 16:26:43.903610 sdss_lvmtan-0.2.4/python/lvmtan/config/test/derot/test.derot.km_lab-sim.conf
+-rw-r--r--   0        0        0     1738 2023-07-09 16:26:43.903898 sdss_lvmtan-0.2.4/python/lvmtan/config/test/derot/test.derot.km_lab-svr.conf
+-rw-r--r--   0        0        0     6431 2023-07-09 16:26:43.904610 sdss_lvmtan-0.2.4/python/lvmtan/config/test/first/test.first.focus_stage-dev.conf
+-rw-r--r--   0        0        0      298 2023-07-09 16:26:43.904868 sdss_lvmtan-0.2.4/python/lvmtan/config/test/first/test.first.focus_stage-sim.conf
+-rw-r--r--   0        0        0     1081 2023-07-09 16:26:43.905299 sdss_lvmtan-0.2.4/python/lvmtan/config/test/first/test.first.focus_stage-svc.conf
+-rw-r--r--   0        0        0      863 2023-07-09 16:26:43.905553 sdss_lvmtan-0.2.4/python/lvmtan/config/test/first/test.first.focus_stage-svr.conf
+-rw-r--r--   0        0        0     8229 2023-07-09 16:26:43.905787 sdss_lvmtan-0.2.4/python/lvmtan/config/test/first/test.first.focus_stage_X_datasheet.conf
+-rw-r--r--   0        0        0     8229 2023-07-09 16:26:43.906458 sdss_lvmtan-0.2.4/python/lvmtan/config/test/xy/test.xy.stage-datasheet.conf
+-rw-r--r--   0        0        0     9377 2023-07-09 16:26:43.906756 sdss_lvmtan-0.2.4/python/lvmtan/config/test/xy/test.xy.stage-dev.conf
+-rw-r--r--   0        0        0      274 2023-07-09 16:26:43.907077 sdss_lvmtan-0.2.4/python/lvmtan/config/test/xy/test.xy.stage-sim.conf
+-rw-r--r--   0        0        0      947 2023-07-09 16:26:43.907301 sdss_lvmtan-0.2.4/python/lvmtan/config/test/xy/test.xy.stage-svc.conf
+-rw-r--r--   0        0        0      843 2023-07-09 16:26:43.907499 sdss_lvmtan-0.2.4/python/lvmtan/config/test/xy/test.xy.stage-svr.conf
+-rw-r--r--   0        0        0      493 2023-07-09 16:26:43.907704 sdss_lvmtan-0.2.4/python/lvmtan/exceptions.py
+-rw-r--r--   0        0        0     4956 1970-01-01 00:00:00.000000 sdss_lvmtan-0.2.4/PKG-INFO
```

### Comparing `sdss_lvmtan-0.2.3/LICENSE.md` & `sdss_lvmtan-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/README.md` & `sdss_lvmtan-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/build.py` & `sdss_lvmtan-0.2.4/build.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/pyproject.toml` & `sdss_lvmtan-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmtan"
-version = "0.2.3"
+version = "0.2.4"
 description = "Lvm Tan Clu Wrapper"
 authors = ["Florian Briegel <briegel@mpia.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmtan"
 repository = "https://github.com/sdss/lvmtan"
 documentation = "https://sdss-lvmtan.readthedocs.org"
```

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/BasdaCluPythonServiceWorker.py` & `sdss_lvmtan-0.2.4/python/lvmtan/BasdaCluPythonServiceWorker.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaBaseCluPythonServiceWorker.py` & `sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaBaseCluPythonServiceWorker.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaCluPythonServiceWorker.py` & `sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaCluPythonServiceWorker.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaTrajCluPythonServiceWorker.py` & `sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaTrajCluPythonServiceWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # -*- coding: utf-8 -*-
 #
 # @Author: Florian Briegel (briegel@mpia.de)
 # @Date: 2021-06-15
 # @Filename: BasdaMoccaTrajCluPythonServiceWorker.py
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
+import asyncio
 import datetime
+import math
 
+import astropy.coordinates
+import astropy.time
+import astropy.units as u
 import BasdaMoccaException
 import BasdaMoccaTraj
 import BasdaService
 import Nice
+import numpy
 import numpy as np
-
-from Nice import I_LOG, N_LOG, U8_LOG, A_LOG, F_LOG, E_LOG
+from astropy.utils import iers
+from lvmtipo.fiber import Fiber
+from lvmtipo.siderostat import Siderostat
+from lvmtipo.site import Site
+from lvmtipo.target import Target
+from Nice import A_LOG, E_LOG, F_LOG, I_LOG, N_LOG, U8_LOG
 
 from .BasdaMoccaXCluPythonServiceWorker import *
 from .exceptions import LvmTanOutOfRange
 
-import asyncio
-import math
-import numpy
-import astropy.coordinates
-import astropy.time
-import astropy.units as u
-
-from lvmtipo.site import Site
-from lvmtipo.siderostat import Siderostat
-from lvmtipo.fiber import Fiber
-from lvmtipo.target import Target
 
-from astropy.utils import iers
 iers.conf.auto_download = False
 
 class BasdaMoccaTrajCluPythonServiceWorker(BasdaMoccaXCluPythonServiceWorker):
     "python clu worker"
 
     def __init__(self, _svcName):
         BasdaMoccaXCluPythonServiceWorker.__init__(self, _svcName)
@@ -72,15 +70,15 @@
         self.derot_dist = 7
         self.backlashInSteps = 1000
         self.homeIsWest = False
 
         I_LOG(f"site: {self.site}, homeOffset: {self.homeOffset}, homeIsWest: {self.homeIsWest}, azang: {azang}, medSign {medSign}")
 
     def _status(self, reachable=True):
-        return {**BasdaMoccaXCluPythonServiceWorker._status(self), 
+        return {**BasdaMoccaXCluPythonServiceWorker._status(self),
                 "CurrentTime": self.service.getCurrentTime() if reachable else "Unknown",
                 "Simulate": self.simulate,
                 "SkyPA": self.service.getDeviceEncoderPosition("SKY"),
                }
 
     def _sid_mpiaMocon(self, target, polyN=1, delta_time=1, time=None):
         if not time:
@@ -102,35 +100,35 @@
             try:
                 position = self._sid_mpiaMocon(target, delta_time=delta_time)[0][2]
 
                 U8_LOG(f"field angle {position} steps")
                 self.service.moveAbsolute(position, "STEPS")
 
                 command.actor.write(
-                     "i", 
-                     { 
+                     "i",
+                     {
                         "Position": self.service.getPosition(),
                         "SkyPA": self.service.getDeviceEncoderPosition("SKY"),
                         "DeviceEncoder": {"Position": self.service.getDeviceEncoderPosition("STEPS"), "Unit": "STEPS"},
                         "Velocity": self.service.getVelocity(),
                         "AtHome": self.service.isAtHome(),
                         "AtLimit": self.service.isAtLimit(),
                         "Simulate": self.simulate,
                      }
                 )
-                     
+
             except Exception as e:
                  E_LOG(f"{e}")
                  command.fail(error=e)
 
             await asyncio.sleep(delta_time)
 
 
     async def _slewTickMocon(self, command, target, delta_time):
-        
+
         try:
             async def setSegment(parent, idx, t0, t1=None):
                 cmd = f"{idx%parent.derot_buffer} {t0[0]} {t0[1]} {t0[2]}"
                 U8_LOG (cmd)
                 await parent._chat(1, 221, parent.device_module, 0, cmd)
                 if t1:
                     cmd = f"{(idx+1)%parent.derot_buffer} 0 0 {t1[2]}"
@@ -184,15 +182,16 @@
                             {
                                 "Position": self.service.getPosition(),
                                 "SkyPA": self.service.getDeviceEncoderPosition("SKY"),
                                 "DeviceEncoder": {"Position": self.service.getDeviceEncoderPosition("STEPS"), "Unit": "STEPS"},
                                 "Velocity": self.service.getVelocity(),
                                 "AtHome": self.service.isAtHome(),
                                 "AtLimit": self.service.isAtLimit(),
-                            }
+                            },
+                            internal=True
                         )
                     await asyncio.sleep(0.3)
 
                 except Exception as ex:
                     E_LOG(ex)
                     break
 
@@ -288,24 +287,23 @@
 
 
         except Exception as e:
             command.fail(error=e)
 
         I_LOG(f"done")
         return command.finish(**self._status(self.service.isReachable()))
-            
-            
+
+
 
     @command_parser.command("slewStop")
     @BasdaCluPythonServiceWorker.wrapper
     async def slewStop(
         self,
         command: Command
     ):
         """Stop slew"""
 
         await self._slewStop()
 
         U8_LOG("done")
 
         return command.finish(**self._status(self.service.isReachable()))
-
```

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaWheelCluPythonServiceWorker.py` & `sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaWheelCluPythonServiceWorker.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaXCluPythonServiceWorker.py` & `sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaXCluPythonServiceWorker.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/BasdaMoccaXYCluPythonServiceWorker.py` & `sdss_lvmtan-0.2.4/python/lvmtan/BasdaMoccaXYCluPythonServiceWorker.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/__init__.py` & `sdss_lvmtan-0.2.4/python/lvmtan/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/alias.cfg` & `sdss_lvmtan-0.2.4/python/lvmtan/config/alias.cfg`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/common/PI_M413.12S_datasheet.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/common/PI_M413.12S_datasheet.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/common/PI_MICOS_datasheet.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/common/PI_MICOS_datasheet.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/common/PI_WHEEL_datasheet.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/common/PI_WHEEL_datasheet.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/common/datasheetServo.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/common/datasheetServo.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/common/datasheetStepper.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/common/datasheetStepper.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.all-sim.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.all-sim.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.all-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.all-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.all.ui` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.all.ui`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.moe-mpia.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.moe-mpia.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.moe-sim.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.moe-sim.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/lvm.moe-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/lvm.moe-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-dev.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-dev.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-svc.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-svc.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/foc/lvm.sci.foc-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/km/lvm.sci.km-dev.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/km/lvm.sci.km-dev.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/km/lvm.sci.km-svc.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/km/lvm.sci.km-svc.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/km/lvm.sci.km-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/km/lvm.sci.km-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/sci/lvm.sci-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/sci/lvm.sci-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-dev.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-dev.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-svc.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-svc.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/foc/lvm.skye.foc-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/km/lvm.skye.km-dev.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/km/lvm.skye.km-dev.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/km/lvm.skye.km-svc.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/km/lvm.skye.km-svc.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/km/lvm.skye.km-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/km/lvm.skye.km-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skye/lvm.skye-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skye/lvm.skye-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-dev.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-dev.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-svc.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-svc.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/foc/lvm.skyw.foc-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-dev.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-dev.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-svc.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-svc.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/km/lvm.skyw.km-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/skyw/lvm.skyw-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/skyw/lvm.skyw-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-dev.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-dev.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-svc.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-svc.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/fibsel/lvm.spec.fibsel-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-dev.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-dev.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-svc.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-svc.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/foc/lvm.spec.foc-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/lvm/spec/lvm.spec-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/lvm/spec/lvm.spec-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/derot/test.derot.km-dev.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/derot/test.derot.km-dev.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/derot/test.derot.km-svc.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/derot/test.derot.km-svc.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/derot/test.derot.km-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/derot/test.derot.km-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/derot/test.derot.km_lab-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/derot/test.derot.km_lab-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/first/test.first.focus_stage-dev.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/first/test.first.focus_stage-dev.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/first/test.first.focus_stage-svc.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/first/test.first.focus_stage-svc.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/first/test.first.focus_stage-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/first/test.first.focus_stage-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/first/test.first.focus_stage_X_datasheet.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/first/test.first.focus_stage_X_datasheet.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/xy/test.xy.stage-datasheet.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/xy/test.xy.stage-datasheet.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/xy/test.xy.stage-dev.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/xy/test.xy.stage-dev.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/xy/test.xy.stage-svc.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/xy/test.xy.stage-svc.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/python/lvmtan/config/test/xy/test.xy.stage-svr.conf` & `sdss_lvmtan-0.2.4/python/lvmtan/config/test/xy/test.xy.stage-svr.conf`

 * *Files identical despite different names*

### Comparing `sdss_lvmtan-0.2.3/PKG-INFO` & `sdss_lvmtan-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmtan
-Version: 0.2.3
+Version: 0.2.4
 Summary: Lvm Tan Clu Wrapper
 Home-page: https://github.com/sdss/lvmtan
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: Florian Briegel
 Author-email: briegel@mpia.de
 Requires-Python: >=3.8,<4
@@ -13,15 +13,14 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: sdss-clu (>=2.0.0)
 Requires-Dist: sdss-cluplus (>=0.0.1)
 Requires-Dist: sdss-lvmtipo (>=0.0.36)
 Requires-Dist: sdsstools (>=0.4.0)
 Project-URL: Documentation, https://sdss-lvmtan.readthedocs.org
```

