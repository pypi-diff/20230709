# Comparing `tmp/wiliot-testers-4.0.14.tar.gz` & `tmp/wiliot-testers-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiliot-testers-4.0.14.tar", last modified: Sun Jul  9 07:12:32 2023, max compression
+gzip compressed data, was "wiliot-testers-4.0.6.tar", last modified: Tue Apr 25 08:52:33 2023, max compression
```

## Comparing `wiliot-testers-4.0.14.tar` & `wiliot-testers-4.0.6.tar`

### file list

```diff
@@ -1,111 +1,108 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.456645 wiliot-testers-4.0.14/
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     7231 2023-07-09 07:12:32.456645 wiliot-testers-4.0.14/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6726 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/README.md
--rw-rw-rw-   0 root         (0) root         (0)     7595 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-09 07:12:32.456645 wiliot-testers-4.0.14/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2087 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/unittests.dockerfile
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.448645 wiliot-testers-4.0.14/wiliot_testers/
--rw-rw-rw-   0 root         (0) root         (0)    10654 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/API_README.md
--rw-rw-rw-   0 root         (0) root         (0)     4005 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.448645 wiliot-testers-4.0.14/wiliot_testers/calibration_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/calibration_test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20959 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/calibration_test/calibration_test.py
--rw-rw-rw-   0 root         (0) root         (0)    25345 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/calibration_test/calibration_test_by_tbp.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.448645 wiliot-testers-4.0.14/wiliot_testers/config/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/config/equipment_config.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.448645 wiliot-testers-4.0.14/wiliot_testers/docs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    72970 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/docs/tester_api_flow.pdf
--rw-rw-rw-   0 root         (0) root         (0)     4818 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/docs/wiliot_logo.png
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.448645 wiliot-testers-4.0.14/wiliot_testers/examples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7410 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/examples/wiliot_tester_example.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.452645 wiliot-testers-4.0.14/wiliot_testers/offline/
--rw-rw-rw-   0 root         (0) root         (0)     7114 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/README.md
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/barcode_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.452645 wiliot-testers-4.0.14/wiliot_testers/offline/configs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/configs/test_configs.json
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/configs/tests_suites.json
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.452645 wiliot-testers-4.0.14/wiliot_testers/offline/docs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    37001 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/docs/example_of_timing_diagram.jpg
--rw-rw-rw-   0 root         (0) root         (0)     9764 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png
--rw-rw-rw-   0 root         (0) root         (0)    44358 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/docs/offline_tester_run_gui.png
--rw-rw-rw-   0 root         (0) root         (0)    20401 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/docs/offline_tester_start_gui.png
--rw-rw-rw-   0 root         (0) root         (0)    81030 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/docs/r2r_communication_diagram.jpg
--rw-rw-rw-   0 root         (0) root         (0)     4386 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG
--rw-rw-rw-   0 root         (0) root         (0)     4818 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/docs/wiliot_logo.png
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/env_install.bat
--rw-rw-rw-   0 root         (0) root         (0)     9005 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/env_install.py
--rw-rw-rw-   0 root         (0) root         (0)   161481 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/offline_tester.py
--rw-rw-rw-   0 root         (0) root         (0)    57849 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/offline_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/run_barcode_testing.bat
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/run_offline_tester.bat
--rw-rw-rw-   0 root         (0) root         (0)     7447 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/offline/tadbik_r2r_controller.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.452645 wiliot-testers-4.0.14/wiliot_testers/sample/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42258 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/com_connect.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.452645 wiliot-testers-4.0.14/wiliot_testers/sample/configs/
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/configs/.default_surfaces.json
--rw-rw-rw-   0 root         (0) root         (0)     1418 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/configs/.default_test_configs.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12210 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/configs_gui.py
--rw-rw-rw-   0 root         (0) root         (0)     4426 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/get_temperature_sensor_name.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/sample_test.bat
--rw-rw-rw-   0 root         (0) root         (0)    83154 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/sample_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.456645 wiliot-testers-4.0.14/wiliot_testers/sample/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22413 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/utils/com_connect.ui
--rw-rw-rw-   0 root         (0) root         (0)     1153 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/utils/comm.gif
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/utils/configs.gif
--rw-rw-rw-   0 root         (0) root         (0)    24482 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/utils/configs.ui
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/utils/edit.gif
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/utils/refresh.gif
--rw-rw-rw-   0 root         (0) root         (0)     3213 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/utils/reset.png
--rw-rw-rw-   0 root         (0) root         (0)    26613 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/utils/sample_test.ui
--rw-rw-rw-   0 root         (0) root         (0)      323 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/utils/save.png
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/sample/utils/wiliot3.gif
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.456645 wiliot-testers-4.0.14/wiliot_testers/system_test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/system_test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    45287 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/system_test/harvester_test.py
--rw-rw-rw-   0 root         (0) root         (0)    73298 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/system_test/system_test_example.py
--rw-rw-rw-   0 root         (0) root         (0)    39503 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/test_equipment.py
--rw-rw-rw-   0 root         (0) root         (0)    66705 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/tester_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      274 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/upload_testers_data.bat
--rw-rw-rw-   0 root         (0) root         (0)    15772 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/upload_testers_data_to_cloud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.456645 wiliot-testers-4.0.14/wiliot_testers/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6048 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/utils/get_version.py
--rw-rw-rw-   0 root         (0) root         (0)    10956 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/utils/upload_to_cloud_api.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-09 07:12:32.000000 wiliot-testers-4.0.14/wiliot_testers/version.py
--rw-rw-rw-   0 root         (0) root         (0)     9672 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/wiliot_tester_log.py
--rw-rw-rw-   0 root         (0) root         (0)    17264 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/wiliot_tester_tag_result.py
--rw-rw-rw-   0 root         (0) root         (0)    62590 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/wiliot_tester_tag_test.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.456645 wiliot-testers-4.0.14/wiliot_testers/yield/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/yield/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.456645 wiliot-testers-4.0.14/wiliot_testers/yield/arduino_counter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/yield/arduino_counter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      809 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/yield/arduino_counter/arduino_counter.ino
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.456645 wiliot-testers-4.0.14/wiliot_testers/yield/configs/
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/yield/configs/.default_configs.json
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/yield/configs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1394 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/yield/configs/inlay_data.py
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/yield/run_yield_tester.bat
--rw-rw-rw-   0 root         (0) root         (0)    31593 2023-07-09 07:12:22.000000 wiliot-testers-4.0.14/wiliot_testers/yield/yield_tester.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-09 07:12:32.448645 wiliot-testers-4.0.14/wiliot_testers.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     7231 2023-07-09 07:12:32.000000 wiliot-testers-4.0.14/wiliot_testers.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-07-09 07:12:32.000000 wiliot-testers-4.0.14/wiliot_testers.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-09 07:12:32.000000 wiliot-testers-4.0.14/wiliot_testers.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-09 07:12:32.000000 wiliot-testers-4.0.14/wiliot_testers.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-07-09 07:12:32.000000 wiliot-testers-4.0.14/wiliot_testers.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-09 07:12:32.000000 wiliot-testers-4.0.14/wiliot_testers.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     5765 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5261 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     7247 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2086 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/unittests.dockerfile
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.100857 wiliot-testers-4.0.6/wiliot_testers/
+-rw-rw-rw-   0 root         (0) root         (0)    10654 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/API_README.md
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/calibration_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/calibration_test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20959 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    25345 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test_by_tbp.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/config/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/config/equipment_config.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/docs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/docs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    72970 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/docs/tester_api_flow.pdf
+-rw-rw-rw-   0 root         (0) root         (0)     4818 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/docs/wiliot_logo.png
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/examples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7410 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/examples/wiliot_tester_example.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/offline/
+-rw-rw-rw-   0 root         (0) root         (0)     7114 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers/offline/configs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/configs/test_configs.json
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/configs/tests_suites.json
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/offline/docs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37001 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/example_of_timing_diagram.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     9764 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png
+-rw-rw-rw-   0 root         (0) root         (0)    44358 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_run_gui.png
+-rw-rw-rw-   0 root         (0) root         (0)    20401 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_start_gui.png
+-rw-rw-rw-   0 root         (0) root         (0)    81030 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/r2r_communication_diagram.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     4386 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG
+-rw-rw-rw-   0 root         (0) root         (0)     4818 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/docs/wiliot_logo.png
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/env_install.bat
+-rw-rw-rw-   0 root         (0) root         (0)     9005 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/env_install.py
+-rw-rw-rw-   0 root         (0) root         (0)   155011 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/offline_tester.py
+-rw-rw-rw-   0 root         (0) root         (0)    63768 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/offline_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/run_offline_tester.bat
+-rw-rw-rw-   0 root         (0) root         (0)     7447 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/offline/tadbik_r2r_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/sample/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    41938 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/com_connect.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/sample/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs/.default_surfaces.json
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs/.default_test_configs.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12551 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/configs_gui.py
+-rw-rw-rw-   0 root         (0) root         (0)     4426 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/get_temperature_sensor_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/sample_test.bat
+-rw-rw-rw-   0 root         (0) root         (0)    74858 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/sample_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/sample/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22413 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/com_connect.ui
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/comm.gif
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.gif
+-rw-rw-rw-   0 root         (0) root         (0)    24482 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.ui
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/edit.gif
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/refresh.gif
+-rw-rw-rw-   0 root         (0) root         (0)     3213 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/reset.png
+-rw-rw-rw-   0 root         (0) root         (0)    26613 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/sample_test.ui
+-rw-rw-rw-   0 root         (0) root         (0)      323 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/save.png
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/sample/utils/wiliot3.gif
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/system_test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/system_test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42625 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/system_test/harvester_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    73298 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/system_test/system_test_example.py
+-rw-rw-rw-   0 root         (0) root         (0)    31248 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/test_equipment.py
+-rw-rw-rw-   0 root         (0) root         (0)    75770 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/tester_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/upload_testers_data.bat
+-rw-rw-rw-   0 root         (0) root         (0)    14651 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/upload_testers_data_to_cloud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.108857 wiliot-testers-4.0.6/wiliot_testers/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6048 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/utils/get_version.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     8865 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_log.py
+-rw-rw-rw-   0 root         (0) root         (0)    16346 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_result.py
+-rw-rw-rw-   0 root         (0) root         (0)    61986 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_test.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/wiliot_testers/yield/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/arduino_counter.ino
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.112857 wiliot-testers-4.0.6/wiliot_testers/yield/configs/
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/configs/.default_configs.json
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/configs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1394 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/configs/inlay_data.py
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/run_yield_tester.bat
+-rw-rw-rw-   0 root         (0) root         (0)    22306 2023-04-25 08:52:21.000000 wiliot-testers-4.0.6/wiliot_testers/yield/yield_tester.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-25 08:52:33.104857 wiliot-testers-4.0.6/wiliot_testers.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     5765 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3451 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-04-25 08:52:32.000000 wiliot-testers-4.0.6/wiliot_testers.egg-info/top_level.txt
```

### Comparing `wiliot-testers-4.0.14/.gitignore` & `wiliot-testers-4.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/LICENSE` & `wiliot-testers-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/PKG-INFO` & `wiliot-testers-4.0.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-testers
-Version: 4.0.14
+Version: 4.0.6
 Summary: A library for interacting with Wiliot's Testers app
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -56,62 +56,15 @@
 * [Sample Test](wiliot_testers/sample/sample_test.py)
 * [Yield Tester](wiliot_testers/yield/yield_tester.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
-Version 4.0.14:
------------------
-* sample tester:
-    * add fail bin for the whole test
-    * add the option to construct specific tests including number of tested tags and the parameters for the test to pass/fail
-* upload data to cloud:
-    * supports also dev env
-    * reduce the max size of a big file
-* test equipment:
-    * improve scanner configuration
-    * add logging
-* tester sdk:
-    * add more fail bins    
-    
-
-Version 4.0.12:
------------------
-* offline tester:
-    * add responded yield to gui
-    * add the option to change the max number of bad QR
-    * fix bug in test format
-    * fix bug when working with two gw
-    * add pop up when upload failed
-    * change default line selection to True
-    * improve code for printing GUI - production and test
-* improve harvester test
-* improve function to upload tester data to cloud including big files (>15Mb)
-* tester sdk:
-    * add more function to the tester log
-    * fix bug when stop event is not specified
-* yield:
-    * add more logging including progress data
 
-Version 4.0.11:
------------------
-* offline tester:
-    * fix bug when several tags under test and test status is still pass
-    * support 8 characters barcode label
-    * Support label scanner for both barcode and QR
-    * check printer communication during the run
-    
-* upload data:
-    * fix .bat file for upload data to the cloud
-    
-* sample test:
-    * fix script error when installing on a clean environment
-    
-    
 Version 4.0.6:
 -----------------
 * offline tester:
     *  update test suite.
     *  enable line selection using text communication with the printing (currently available only if printing offset > 0 and no QR check.
     *  add tag reel location to packet data csv (i.e. the location on the reel even if multiple runs were done on the same reel)
     *  check gw trigger (optic sensor signal) and apply printing validation, right after a trigger was received (or missing label was decided)
```

### Comparing `wiliot-testers-4.0.14/bitbucket-pipelines.yml` & `wiliot-testers-4.0.6/bitbucket-pipelines.yml`

 * *Files 3% similar despite different names*

```diff
@@ -65,35 +65,30 @@
             #print current version:
             - python3 wiliot_testers/utils/get_version.py
             #Update patch version by git tag:
             - version="`python3 wiliot_testers/utils/get_version.py next_patch`" && echo $version && git tag -a -m "[skip ci] build number $BITBUCKET_BUILD_NUMBER set the library patch version to $version." $version  && git push origin $version
             #print new version
             - python3 wiliot_testers/utils/get_version.py
 
-    publish-full-version-into-new-codearfact:
+    publish-full-version-into-codearfact:
       - step:
           name: Build and publish full version py-wilot into codeartifact
-          image:
-            name: 096303741971.dkr.ecr.us-east-2.amazonaws.com/ci:0.0.1-alpine
-            aws:
-              access-key: $CLOUD_AWS_ACCESS_KEY_ID
-              secret-key: $CLOUD_AWS_SECRET_ACCESS_KEY
+          <<: *wiliot-ci-image
           script:
-            - pip3 install setuptools_scm wheel twine
+            - pip3 install setuptools_scm
             - pip3 install gitpython
             # get updated version number:
             - version="`python3 wiliot_testers/utils/get_version.py`"
             # update minor version:
             - python3 setup.py sdist bdist_wheel
             #update version.py with new minor version and build number (first step is done by setup as well- but we want to add build number as well):
             - echo "__version__ = '$version'" > wiliot_testers/version.py
             - echo "build_number = '$BITBUCKET_BUILD_NUMBER'" >> wiliot_testers/version.py
-            - export AWS_ACCESS_KEY_ID=$CLOUD_AWS_ACCESS_KEY_ID AWS_SECRET_ACCESS_KEY=$CLOUD_AWS_SECRET_ACCESS_KEY
-            - aws codeartifact login --region us-east-2 --tool twine --domain wiliot-cloud --domain-owner 096303741971 --repository pypi
-            - twine upload --verbose --repository codeartifact dist/*
+            - aws codeartifact login --tool twine --domain wiliot-cloud --domain-owner 142654642153 --repository pypi
+            - twine upload --repository codeartifact dist/*
 
     publish-slim-version-into-pypi:
       - step:
           name: Build and publish slim version py-wilot into pypi
           <<: *wiliot-ci-image
           script:
             - pip3 install setuptools_scm
```

### Comparing `wiliot-testers-4.0.14/setup.py` & `wiliot-testers-4.0.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,15 +37,15 @@
                      'pyqtgraph',
                      'PySimpleGUI',
                      'matplotlib',
                      'PyQt5',
                      'pygubu==0.16',
                      'appdirs',
                      'pillow',
-                     'wiliot-api>=4.1.2',
-                     'wiliot-core>=4.0.13',
-                     'wiliot-tools>=4.0.5'
+                     'wiliot-api==4.1.0',
+                     'wiliot-core==4.0.8',
+                     'wiliot-tools==4.0.4'
                  ],
                  zip_safe=False,
                  python_requires='>=3.6',
                  include_package_data=True,
                  )
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/API_README.md` & `wiliot-testers-4.0.6/wiliot_testers/API_README.md`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/__init__.py` & `wiliot-testers-4.0.6/wiliot_testers/__init__.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/calibration_test/calibration_test.py` & `wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/calibration_test/calibration_test_by_tbp.py` & `wiliot-testers-4.0.6/wiliot_testers/calibration_test/calibration_test_by_tbp.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/docs/tester_api_flow.pdf` & `wiliot-testers-4.0.6/wiliot_testers/docs/tester_api_flow.pdf`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/docs/wiliot_logo.png` & `wiliot-testers-4.0.6/wiliot_testers/docs/wiliot_logo.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/examples/wiliot_tester_example.py` & `wiliot-testers-4.0.6/wiliot_testers/examples/wiliot_tester_example.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/README.md` & `wiliot-testers-4.0.6/wiliot_testers/offline/README.md`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/configs/tests_suites.json` & `wiliot-testers-4.0.6/wiliot_testers/offline/configs/tests_suites.json`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/docs/example_of_timing_diagram.jpg` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/example_of_timing_diagram.jpg`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_print_sgtin_gui.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/docs/offline_tester_run_gui.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_run_gui.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/docs/offline_tester_start_gui.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/offline_tester_start_gui.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/docs/r2r_communication_diagram.jpg` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/r2r_communication_diagram.jpg`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/upload_to_cloud_gui.PNG`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/docs/wiliot_logo.png` & `wiliot-testers-4.0.6/wiliot_testers/offline/docs/wiliot_logo.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/env_install.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/env_install.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/offline_tester.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/offline_tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,30 +66,28 @@
 from PyQt5.QtGui import *
 import pyqtgraph as pg
 from wiliot_testers.test_equipment import BarcodeScanner
 from numpy import mean
 from wiliot_testers.wiliot_tester_tag_test import *
 from wiliot_testers.wiliot_tester_log import *
 from wiliot_testers.tester_utils import *
-from wiliot_testers.utils.upload_to_cloud_api import *
 from wiliot_testers.offline.offline_utils import *
-from wiliot_core import WiliotDir, check_user_config_is_ok, csv_to_dict, InlayTypes, DualGWMode, WiliotGateway
+from wiliot_core import WiliotDir, check_user_config_is_ok, csv_to_dict, InlayTypes, DualGWMode
 from wiliot_testers.utils.get_version import get_version
 from wiliot_core import WiliotGateway, DualGWMode
 from appdirs import user_data_dir
 from queue import Queue
 import socket
 
 # a global variable which will be in the log_file name that says the R2R code version
 n_tag_counter_position = 4  # 4 characters on the esternal id indicate tag counter in the reel
 R2R_code_version = '13'
 # running parameters
 tested = 0
 passed = 0
-responded = 0
 under_threshold = 0
 missing_labels = 0
 black_list_size = 0
 last_pass_string = 'No tag has passed yet :('
 
 desired_pass_num = 999999999  # this will be set to the desired pass that we want to stop after
 desired_tags_num = 999999999  # this will be set to the desired tags that we want to stop after
@@ -102,60 +100,37 @@
 run_start_time_ = datetime.datetime.now()
 qr_que_list = []
 external_id_for_printer = 999999999
 yield_over_time = 0
 calculate_interval = 10
 calculate_on = 50
 
-MIN_TEST_TIME = 1.5  # seconds
-TIME_BTWN_PRINTER_REQUESTS = 0.25  # seconds
-PRINTER_SOCKET_TIMEOUT = 1  # seconds
+MIN_TEST_TIME = 0.3  # seconds
 
 lock_print = threading.Lock()
 
 
 class QRThread(threading.Thread):
-    def __init__(self, events, ports_and_guis, print=False):
+    def __init__(self, events, ports_and_guis):
         threading.Thread.__init__(self)
         self.events = events
-        self.is_print = print
         self.ports_and_guis = ports_and_guis
         self.qr_comport = self.ports_and_guis.Tag_Value['QRcomport']
         self.max_wrong_readouts_in_row = int(self.ports_and_guis.Tag_Value['maxQRWrongTags'])
-        self.qr_timeout = str(self.ports_and_guis.Tag_Value['QRtimeout'])
-
-        try:
-            if self.is_print:
-                self.scanner = BarcodeScanner(com_port='COM{}'.format(self.qr_comport), log_type='LOG', write_to_log=False, timeout=self.qr_timeout, log_name=self.ports_and_guis.my_logger.results_logger.name)
-            else:
-                self.scanner = BarcodeScanner(com_port='COM{}'.format(self.qr_comport), log_type='LOG', write_to_log=True, timeout=self.qr_timeout, log_name=self.ports_and_guis.my_logger.results_logger.name)
-
-            self.ports_and_guis.my_logger.logger.info('Connected to scanner at port COM{}'.format(self.qr_comport))
-
-        except Exception as e:
-            self.ports_and_guis.my_logger.logger.info('No barcode scanner found')
-            raise Exception(f'could not connect to bracode scanner {e}')
-
+        self.scanner = BarcodeScanner(com='COM{}'.format(self.qr_comport), log_type='LOG')
         self.read_out_attempts = 5
         self.failed_qr_list = []
         self.qr_max_bad_tags = 10
-        if 'qr_max_bad_tags' in self.ports_and_guis.Tag_Value:
-            try:
-                self.qr_max_bad_tags = int(self.ports_and_guis.Tag_Value['qr_max_bad_tags'])
-            except Exception as e:
-                self.ports_and_guis.my_logger.logger.warning(f'Could not convert the qr_max_bad_tags to number, '
-                                                             f'the default value would be {self.qr_max_bad_tags}: {e}')
         self.wrong_readout = 0
         self.wrong_readout_in_row = 0
 
     def run(self):
 
         def success_read():
             self.ports_and_guis.my_logger.logger.info("QR code validated successfully")
-            self.events.qr_val.set()
             self.events.qr_read_success.set()
             self.success = True
             self.wrong_readout_in_row = 0
 
         die = False
 
         while not die:
@@ -163,80 +138,63 @@
             self.events.start_compare.wait(timeout=10)
             if not self.events.start_compare.is_set():
                 if self.events.done_to_tag_thread.is_set() or self.events.done_to_r2r_thread.is_set():
                     die = True
                     break
                 continue
 
-            if not self.is_print:
+            if not self.events.qr_queue.empty():
                 self.events.start_compare.clear()
-                self.events.qr_val.clear()
+                try:
+                    self.tag_comparted = self.events.qr_queue.get(block=False, timeout=0.1)
+                except Exception:
+                    die = True
+                    break
                 self.success = False
+                self.ports_and_guis.my_logger.logger.info('Comparing {}'.format(self.tag_comparted))
                 for i in range(self.read_out_attempts):
                     self.qr_tag = self.scanner.scan_ext_id()
-                    self.ports_and_guis.my_logger.logger.info('Scanned {}'.format(self.qr_tag))
-                self.events.qr_val.set()
-                self.events.qr_read_success.set()
-
-
-            else:
-                if not self.events.qr_queue.empty():
-                    self.events.start_compare.clear()
-                    self.events.qr_val.clear()
-                    try:
-                        self.tag_comparted = self.events.qr_queue.get(block=False, timeout=0.1)
-                    except Exception:
-                        die = True
-                        break
-                    self.success = False
-                    self.ports_and_guis.my_logger.logger.info('Comparing {}'.format(self.tag_comparted))
-                    for i in range(self.read_out_attempts):
-                        self.qr_tag = self.scanner.scan_ext_id()
-                        self.ports_and_guis.my_logger.logger.info(
-                            f'--- SCANNING: expected ex id: {self.tag_comparted["externalID"]}, '
-                            f'read ex id: {self.qr_tag[0]} ---')
-                        if self.qr_tag[1] is not None:
-                            if self.tag_comparted['status'] == 'Pass':
-                                if self.tag_comparted['externalID'][-4:] == self.qr_tag[1]:
-                                    success_read()
-                                    break
-
-                        else:
-                            if self.tag_comparted['status'] == 'Fail':
+                    time.sleep(0.05)
+                    if self.qr_tag[1] is not None:
+                        if self.tag_comparted['status'] == 'Pass':
+                            if self.tag_comparted['externalID'][-4:] == self.qr_tag[1]:
                                 success_read()
                                 break
 
-                        self.ports_and_guis.my_logger.logger.info(
-                            "Scanning failed, trying again attempt {}/{}".format(i, self.read_out_attempts))
-
-                    if not self.success:
-                        self.ports_and_guis.my_logger.logger.warning('Scan failed for tag {}'.format(self.tag_comparted))
-                        self.wrong_readout += 1
-                        self.wrong_readout_in_row += 1
-                        if self.wrong_readout < self.qr_max_bad_tags and \
-                                self.wrong_readout_in_row < self.max_wrong_readouts_in_row:
-                            self.events.qr_val.clear()
-                            self.events.qr_read_success.set()
-
-                if self.wrong_readout >= self.qr_max_bad_tags:
-                    die = True
-                    self.ports_and_guis.my_logger.logger.warning('Maximum bad tags comparing reached')
-                    break
+                    else:
+                        if self.tag_comparted['status'] == 'Fail':
+                            success_read()
+                            break
 
-                if self.wrong_readout_in_row >= self.max_wrong_readouts_in_row:
-                    self.ports_and_guis.my_logger.logger.warning('Maximum bad tags comparing in row reached')
-                    die = True
-                    break
+                    self.ports_and_guis.my_logger.logger.info(
+                        "Scanning failed, trying again attempt {}/{}".format(i, self.read_out_attempts))
 
-                if self.events.done_to_tag_thread.is_set() or self.events.done_to_r2r_thread.is_set():
-                    die = True
-                    break
+                if not self.success:
+                    self.ports_and_guis.my_logger.logger.warning('Scan failed for tag {}'.format(self.tag_comparted))
+                    self.wrong_readout += 1
+                    self.wrong_readout_in_row += 1
+                    if self.wrong_readout < self.qr_max_bad_tags and \
+                            self.wrong_readout_in_row < self.max_wrong_readouts_in_row:
+                        self.events.qr_read_success.set()
+
+            if self.wrong_readout >= self.qr_max_bad_tags:
+                die = True
+                self.ports_and_guis.my_logger.logger.warning('Maximum bad tags comparing reached')
+                break
+
+            if self.wrong_readout_in_row >= self.max_wrong_readouts_in_row:
+                self.ports_and_guis.my_logger.logger.warning('Maximum bad tags comparing in row reached')
+                die = True
+                break
+
+            if self.events.done_to_tag_thread.is_set() or self.events.done_to_r2r_thread.is_set():
+                die = True
+                break
 
         if die:
-            self.scanner.close_port()
             msg = 'Pausing run because QR comparing went wrong or run end'
             printing_func(msg, 'QRThread', lock_print, logger_type='warning',
                           logger_name=self.ports_and_guis.my_logger.logger.name)
             self.events.done_to_tag_thread.set()
             self.events.stop_to_r2r_thread.set()
 
 
@@ -313,15 +271,14 @@
             self.start_value = start_value
             self.cur_value = 0
             self.pass_job_name = pass_job_name
             self.fail_job_name = self.ports_and_guis.Tag_Printing_Value['failJobName']
             self.pass_job_num = self.ports_and_guis.Tag_Printing_Value['passJobNum']
             self.fail_job_num = 1
 
-
             # open the socket & config the printer
             self.initialization()
 
         except Exception:
             exception_details = sys.exc_info()
             self.exception_queue.put(exception_details)
 
@@ -358,15 +315,15 @@
 
             cmds = ['CAF\r\n',
                     'CQI\r\n',
                     f'CLN|{self.fail_job_num}|\r\n',
                     f'CLN|{self.pass_job_num}|\r\n',
                     f'LAS|{self.pass_job_name}|{self.pass_job_num}|' + job_fields_str]
             if self.fail_job_name == self.pass_job_name:
-                cmds.append(f'LAS|{self.pass_job_name}|{self.fail_job_num}|' + job_fields_str)
+                cmds.append(f'LAS|{self.pass_job_name}|{self.pass_job_num}|' + job_fields_str)
             else:
                 cmds.append(f'LAS|{self.fail_job_name}|{self.fail_job_num}|\r\n')
 
             if self.enable_line_selection:
                 cmds.append(self.get_line_selection_cmd(self.fail_job_name))  # select line
             for cmd in cmds:
                 value = self.query(cmd)
@@ -476,15 +433,15 @@
                                 try:
                                     self.printer_status()
                                     break
                                 except Exception as e:
                                     self.ports_and_guis.my_logger.logger.info(f'got exception from printer, '
                                                                               f'try again ({e})')
                                     dt = (datetime.datetime.now() - t_i).total_seconds()
-                                    time.sleep(TIME_BTWN_PRINTER_REQUESTS)
+                                    time.sleep(0.010)
                             if self.enable_line_selection:
                                 self.set_printing_type()  # set the printing type for the next tag #TODO need to enable it for QR as well
 
                 except Exception:
                     do_the_thread_again = False
                     exception_details = sys.exc_info()
                     self.exception_queue.put(exception_details)
@@ -665,16 +622,14 @@
         """
         if print_and_log:
             msg = "Sent command to printer: " + cmd.strip('\r\n')
             printing_func(msg, 'PrinterThread', lock_print, logger_type='debug',
                           logger_name=self.ports_and_guis.my_logger.logger.name)
         self.ports_and_guis.Printer_socket.send(cmd.encode())
         data = self.ports_and_guis.Printer_socket.recv(int(self.TCP_BUFFER))
-        if len(data) == 0:
-            raise PrinterNeedsResetException(f'The printer did not ack to the following cmd :{cmd}')
         value = data.decode("utf-8")
         # Cut the last character as the device returns a null terminated string
         value = value[:-1]
         if print_and_log:
             msg = "Received answer from printer: " + str(value.strip('\r\n'))
             printing_func(msg, 'PrinterThread', lock_print, logger_type='debug',
                           logger_name=self.ports_and_guis.my_logger.logger.name)
@@ -705,15 +660,14 @@
             time.sleep(1)  # to make sure the socket is closed when we start the reopen
             self.initialization()
         except Exception:
             printing_func('reopen_sock() failed, please end this run', 'PrinterThread',
                           lock_print, logger_type='warning', logger_name=self.ports_and_guis.my_logger.logger.name)
             raise (PrinterNeedsResetException('reopen_sock() failed'))
 
-    # UNUSED FUNCTION
     def line_assigment(self, job_name, line_number, field_name, field_value):
         """
         builds the command to send to printer for configuration of the printing format
         @param job_name: (string) what is the job name (should be the same as in the printer)
         @param line_number: what is the line to assign to (2 = pass, 1 = fail)
         @param field_name: field name in the printer
         @param field_value: what to put in this field
@@ -721,15 +675,14 @@
         """
         # Send Line Assignment Command: job name + line number+starting value
         cmd = 'LAS|' + str(job_name) + '|' + str(line_number) + '|' + str(field_name) + '=' + str(
             field_value) + '|\r\n'
         # changing to bytes
         return cmd
 
-    # UNUSED FUNCTION
     def clear_line(self, line_number):
         """
         builds the command to send to printer for clearing a line
         @param line_number: the line to clear
         @return: the cmd to send to printer
         """
         # On success, returns the default success response (ACK). On failure, returns the default failure response (ERR)
@@ -746,15 +699,14 @@
         3 Running
         4 Offline
         @return: the cmd to send to printer
         """
         cmd = 'SST|' + str(desired_state) + '|\r\n'
         return cmd
 
-    # UNUSED FUNCTION
     def get_job_name(self):
         """
         gets the last job that were used by the printer
         @return: the name of the current job in the printer in the following format:
             JOB|<job name>|<line number>|<CR>
         """
         cmd = 'GJN\r\n'
@@ -882,15 +834,15 @@
              'packet_status', 'adv_address', 'selected_tag', 'is_test_pass', 'status_offline', 'fail_bin',
              'fail_bin_str',
              'test_status', 'num_packets', 'num_cycles', 'sprinkler_counter_mean', 'sprinkler_counter_std',
              'sprinkler_counter_min', 'sprinkler_counter_max', 'tbp_mean', 'tbp_std', 'tbp_min', 'tbp_max',
              'tbp_num_vals',
              'per_mean', 'per_std', 'rssi_mean', 'rssi_std', 'rssi_min', 'rssi_max', 'ttfp', 'rx_rate_normalized',
              'rx_rate', 'total_test_duration', 'total_location_duration', 'test_start_time', 'trigger_time',
-             'test_end_time', 'label_validated_at_loc', 'rx_channel', 'energizing_pattern', 'time_profile',
+             'test_end_time', 'qr_validated', 'rx_channel', 'energizing_pattern', 'time_profile',
              'decrypted_packet_type',
              'group_id', 'flow_ver', 'test_mode', 'en', 'type', 'data_uid', 'nonce', 'enc_uid', 'mic', 'enc_payload',
              'gw_packet', 'stat_param', 'temperature_sensor']
 
         try:
             self.GwObj, self.t = self.config()
 
@@ -942,40 +894,25 @@
                     self.ports_and_guis.my_logger.logger.info('Sent start to test QR')
                 else:
                     self.events.qr_read_success.set()
                     self.ports_and_guis.my_logger.logger.info('Queue not full yet')
 
             else:
                 self.events.start_compare.set()
-        elif self.qr_enable == 'Yes' and not self.ports_and_guis.print_test:
-            self.events.printer_validation_success.clear()
-            self.events.qr_read_success.clear()
-            self.events.start_compare.set()
 
     def check_printer_validation(self):
         if self.to_print and not self.ports_and_guis.print_test:
             self.events.validation_success.wait(timeout=5)
             if not self.events.validation_success.isSet():
                 self.ports_and_guis.my_logger.logger.warning(
                     "QR Validation didn't succeed or Printer counter is not right")
                 self.events.stop_to_r2r_thread.set()
                 self.events.done_to_tag_thread.set()
             else:
-                self.ports_and_guis.my_logger.logger.info('Validation criteria is ok')
-            self.events.printer_validation_success.clear()
-            self.events.qr_read_success.clear()
-
-    def check_qr_validation(self):
-        if self.qr_enable == 'Yes' and not self.to_print:
-            self.events.validation_success.wait(timeout=5)
-            if not self.events.validation_success.isSet():
-                self.ports_and_guis.my_logger.logger.warning(
-                    "QR Validation didn't succeed or Printer counter is not right")
-            else:
-                self.ports_and_guis.my_logger.logger.info('Validation criteria is ok')
+                self.ports_and_guis.my_logger.logger.info('Validation is ok')
             self.events.printer_validation_success.clear()
             self.events.qr_read_success.clear()
 
     @pyqtSlot()
     def run(self):
         """
         runs the thread
@@ -1010,15 +947,15 @@
                 if self.events.done_to_tag_thread.is_set():
                     self.ports_and_guis.my_logger.logger.warning('TagThread recieved - Job is done')
                     die = True
                     break
                 else:  # the r2r_ready event happened , done_or_printer_event.wait will happen after start GW
                     # start of tags loop ###########################
                     # the long timer (will cause +1 missing label)
-                    global tested, passed, missing_labels, black_list_size, responded
+                    global tested, passed, missing_labels, black_list_size
                     global last_pass_string, reel_name
                     self.events.r2r_ready.clear()
                     self.r2r_response_times_up = False
                     self.start_GW_happened = False
                     # will wait 10 seconds after the tag timer should have ended
                     # and then will enforce a start_r2r & fail_r2r
 
@@ -1103,29 +1040,24 @@
                         except Exception:
                             self.ports_and_guis.my_logger.logger.warning('Problem with temperature sensor detection')
                             pass
                         self.ports_and_guis.my_logger.logger.debug('Temperature is: {}'.format(str(temperature_sensor)))
                     else:
                         temperature_sensor = float(-1)
 
-                    if self.qr_enable == 'Yes' and not self.to_print:
-                        self.check_qr_validation()
-
                     self.test_data['tag_run_location'] = self.tag_location
                     self.test_data['tag_reel_location'] = int(self.tag_reel_location) + int(self.tag_location)
                     self.test_data['temperature_sensor'] = temperature_sensor
                     if self.events.done_to_tag_thread.is_set():
                         break
                     # printing processes:
                     if self.to_print and not self.ports_and_guis.print_test:
                         self.test_data['external_id'] = self.printed_external_id
                         self.ports_and_guis.my_logger.logger.info('Making sure printer or QR doesnt have failures')
                         self.check_printer_validation()
-                    elif self.to_print and self.ports_and_guis.print_test:
-                        self.test_data['external_id'] = self.printed_external_id
 
 
                     try:
                         if self.events.done_to_tag_thread.is_set():
                             break
                         tested += 1
                         if self.tester_res.is_results_empty():
@@ -1138,15 +1070,15 @@
                             self.test_data['is_test_pass'] = False
                             self.ports_and_guis.my_logger.logger.warning(
                                 'Tag location: {} failed - Missing Label'.format(str(self.tag_location)))
                             self.events.start_to_r2r_thread.set()
 
                             total_loc_time = datetime.datetime.now() - self.start_time
                             self.test_data['total_location_duration'] = total_loc_time.total_seconds()
-                            self.test_data['label_validated_at_loc'] = self.events.qr_val.is_set()
+
                             # add packets to packet_data.csv:
                             self.update_packet_data(packets_data_path=self.ports_and_guis.my_logger.packets_data_path,
                                                     test_data=self.test_data)
                             # update run_data:
                             self.update_run_data(run_data_path=self.ports_and_guis.my_logger.run_data_path,
                                                  run_data=self.run_data)
                             if self.to_print and not self.ports_and_guis.print_test:
@@ -1177,15 +1109,15 @@
 
                             if self.ttfp_num:
                                 self.run_data['ttfp_avg'] = self.ttfp_sum / self.ttfp_num
 
                             selected_tag = self.tester_res.check_and_get_selected_tag_id()
                             if selected_tag == '':
                                 # Didnt understand who is talking in different stages or the case no tag was selected
-                                # responded += 1
+
                                 try:
                                     self.ports_and_guis.my_logger.logger.warning(
                                         'Tag location: {} failed - {}'.format(self.tag_location,
                                                                               self.tester_res.get_total_fail_bin(
                                                                                   as_name=True)))
                                 except Exception:
                                     pass
@@ -1201,16 +1133,15 @@
                                 if selected_tag in self.all_selected_tags:
                                     # Duplication
                                     self.tester_res.set_total_fail_bin(FailureCodes.DUPLICATION_OFFLINE)
                                     self.tester_res.set_total_test_status(status=False)
                                     black_list_size += 1
                                     self.black_list.append(selected_tag)
                                     self.ports_and_guis.my_logger.logger.warning(
-                                        'Tag location: {} has been already seen in the run before'.format(
-                                            str(self.tag_location)))
+                                        'Tag location: {} has been already seen in the run before'.format(str(self.tag_location)))
                                     self.tester_res.set_packet_status(adv_address=selected_tag,
                                                                       status='duplication')
                                     if self.to_print and not self.ports_and_guis.print_test:
                                         self.events.qr_queue.put({'externalID': selected_tag, 'status': 'Fail'})
                                         if self.enable_line_selection:
                                             self.events.tag_status_queue.put('fail')
 
@@ -1218,15 +1149,14 @@
                                         self.WiliotTester.add_to_blacklist(selected_tag)
                                         self.ports_and_guis.my_logger.logger.warning(
                                             'Tag {} in location {} has reached max appearance in black list'.format(
                                                 selected_tag, self.tag_location))
                                     self.events.fail_to_r2r_thread.set()
 
                                 else:
-                                    responded += 1
                                     # Tag pass or fail but with respond
                                     self.missing_labels_in_a_row = 0
                                     self.all_selected_tags.append(selected_tag)
                                     if self.tester_res.is_all_tests_passed():
                                         # Pass
                                         passed += 1
                                         if self.to_print and not self.ports_and_guis.print_test:
@@ -1251,26 +1181,14 @@
                                             if self.enable_line_selection:
                                                 self.events.tag_status_queue.put('pass')
                                             self.ports_and_guis.my_logger.logger.info(
                                                 'Added tag {} to que as pass'.format(self.printed_external_id))
                                             self.externalId += 1
                                         else:
                                             last_pass_string = f'Tag Location:  {str(self.tag_location)}'
-                                            self.printed_external_id, is_OK = get_printed_value(
-                                                self.printing_value['stringBeforeCounter'],
-                                                self.printing_value['digitsInCounter'],
-                                                str(self.externalId),
-                                                self.value['printingFormat'])
-                                            self.next_printed_external_id, is_OK = get_printed_value(
-                                                self.printing_value['stringBeforeCounter'],
-                                                self.printing_value['digitsInCounter'],
-                                                str(int(self.externalId) + 1),
-                                                self.value['printingFormat'])
-                                            self.test_data['external_id'] = self.printed_external_id
-                                            self.externalId += 1
                                         self.events.pass_to_r2r_thread.set()
                                     else:
                                         # Tag failed statistics
                                         self.ports_and_guis.my_logger.logger.warning(
                                             'Tag location: {} failed - {}'.format(str(self.tag_location), str(
                                                 self.tester_res.get_total_fail_bin(as_name=True))))
                                         if self.to_print and not self.ports_and_guis.print_test:
@@ -1282,27 +1200,26 @@
                                                 'Tag added as fail, failed during test')
                                         self.events.fail_to_r2r_thread.set()
                             self.all_tags += self.tester_res.get_test_unique_adva()
                             self.all_tags = list(set(self.all_tags))
                             self.run_data['total_run_responding_tags'] = len(self.all_tags)
                             total_loc_time = datetime.datetime.now() - self.start_time
                             self.test_data['total_location_duration'] = total_loc_time.total_seconds()
-                            self.test_data['label_validated_at_loc'] = self.events.qr_val.is_set()
                             # add packets to packet_data.csv:
                             self.update_packet_data(res=self.tester_res,
                                                     packets_data_path=self.ports_and_guis.my_logger.packets_data_path,
                                                     test_data=self.test_data)
                             # update run_data:
                             self.update_run_data(run_data_path=self.ports_and_guis.my_logger.run_data_path,
                                                  run_data=self.run_data, res=self.tester_res)
                         self.tag_location += 1
-                        # Check the diff criteria
+                        # Check the diff critiria
                         if self.pass_response_diff is not None:
                             if len(self.all_tags) > self.pass_response_diff_offset:
-                                if (passed * 100) / len(self.all_tags) < 100 - int(self.pass_response_diff):
+                                if (passed*100)/len(self.all_tags) < 100-int(self.pass_response_diff):
                                     self.ports_and_guis.my_logger.logger.warning(
                                         'Problem with setup, stop criteria for responsive tags and pass tags diff is '
                                         'lower then threshold please check setup or change the value')
                                     self.events.done_to_r2r_thread.set()
                                     self.events.done_to_tag_thread.set()
                                     if self.to_print:
                                         self.events.done_to_printer_thread.set()
@@ -1480,34 +1397,32 @@
 
         if self.ports_and_guis.auto_attenuator_enable:
             attn_pwr = int(self.ports_and_guis.Tag_Value['attnval']) - 5
             self.ports_and_guis.my_logger.results_logger.info('Setting ATTN to {}'.format(attn_pwr))
             set_attn_status = self.ports_and_guis.attenuator.Setattn(attn_pwr)
             time.sleep(2)
             if set_attn_status:
-                self.ports_and_guis.my_logger.results_logger.info(
-                    'Attenuation in dB set to {}'.format(self.ports_and_guis.attenuator.Getattn()))
+                self.ports_and_guis.my_logger.results_logger.info('Attenuation in dB set to {}'.format(self.ports_and_guis.attenuator.Getattn()))
 
         self.ttfp_num = 0
         self.ttfp_sum = 0
         return self.GwObj, t
 
     def start_energizer(self):
         if self.ports_and_guis.energizerGW:
-            self.ports_and_guis.energizerGW.write('!gateway_app')
+            self.ports_and_guis.energizerGW.write('!gateway_app', with_ack=True)
 
     def stop_energizer(self):
         if self.ports_and_guis.energizerGW:
             self.ports_and_guis.energizerGW.write('!cancel')
             self.ports_and_guis.energizerGW.reset_buffer()
 
     def get_curr_timestamp_in_sec(self):
         return (datetime.datetime.now() - self.start_time).total_seconds()
 
-    # UNUSED FUNCTION
     def is_gw_respond_with_stat_param_zero(self, chosen_tag_packets):
         chosen_tag_packets_df = chosen_tag_packets.get_df()
         return len(chosen_tag_packets_df[chosen_tag_packets_df['stat_param'] == 0]) > 1
 
     def closure_fn(self):
         """
            turn off the GW (reset) and closes the GW Comport
@@ -1515,32 +1430,44 @@
                'User pressed Stop!'
            """
         if self.black_list.__len__() > 0:
             self.ports_and_guis.my_logger.logger.warning('Black list tags: {}'.format(list(set(self.black_list))))
         if not self.did_closure_fn_run:
             self.run_data['reel_run_end_time'] = datetime.datetime.now()
             self.run_data['upload_date'] = datetime.datetime.now()
-            dict_to_csv(self.run_data, path=self.ports_and_guis.my_logger.run_data_path)
+            self.dict_to_csv(self.run_data, path=self.ports_and_guis.my_logger.run_data_path)
             self.WiliotTester.exit_tag_test()
             printing_func("TagThread is done", 'TagThread',
                           lock_print, logger_type='warning', logger_name=self.ports_and_guis.my_logger.logger.name)
             self.did_closure_fn_run = True
 
-    # TODO, MAYBE ONE FUNCTION OR OFFLINE AND YIELD?
+    def dict_to_csv(self, dict_in, path, append=False, only_titles=False):
+        if append:
+            method = 'a'
+        else:
+            method = 'w'
+        with open(path, method, newline='') as f:
+            dict_writer = DictWriter(f, fieldnames=dict_in.keys())
+            if not append:
+                dict_writer.writeheader()
+            if not only_titles:
+                dict_writer.writerow(dict_in)
+            f.close()
+
     def update_run_data(self, run_data_path, run_data, res=None, save_to_csv=True):
         if res is not None:
             run_data['total_run_tested'] += 1
             run_data['total_run_passed_offline'] += res.get_total_test_status()
             run_data['run_responsive_tags_yield'] = \
                 (run_data['total_run_responding_tags'] / run_data['total_run_tested']) * 100
             run_data['run_offline_yield'] = \
                 (run_data['total_run_passed_offline'] / run_data['total_run_tested']) * 100
 
         if save_to_csv:
-            dict_to_csv(dict_in=run_data, path=run_data_path)
+            self.dict_to_csv(dict_in=run_data, path=run_data_path)
 
     def update_packet_data(self, packets_data_path, res=None, test_data=None, only_titles=False):
 
         def save_default_packet_data(summary=None):
             default_data = {'raw_packet': None, 'adv_address': None, 'decrypted_packet_type': None,
                             'group_id': None, 'flow_ver': None,
                             'test_mode': None, 'en': None, 'type': None, 'data_uid': None, 'nonce': None,
@@ -1550,15 +1477,15 @@
                             'tag_run_location': test_data['tag_run_location'],
                             'tag_reel_location': test_data['tag_reel_location'],
                             'total_test_duration': test_data['total_test_duration'],
                             'total_location_duration': test_data['total_location_duration'],
                             'status_offline': test_data['status_offline'],
                             'fail_bin': test_data['fail_bin'], 'fail_bin_str': test_data['fail_bin_str'],
                             'external_id': None,
-                            'label_validated_at_loc': test_data['label_validated_at_loc'], 'test_num': test_data['test_num'],
+                            'qr_validated': test_data['qr_validated'], 'test_num': test_data['test_num'],
                             'trigger_time': test_data['trigger_time'], 'packet_status': None,
                             'temperature_sensor': float(-1)}
             if summary is None:
                 default_sum = {'is_test_pass': None, 'selected_tag': None, 'test_start_time': None,
                                'test_end_time': None, 'test_status': None, 'rx_channel': None,
                                'energizing_pattern': None, 'time_profile': None, 'num_packets': 0,
                                'num_cycles': 0, 'sprinkler_counter_mean': None, 'sprinkler_counter_std': None,
@@ -1569,21 +1496,21 @@
                                'rx_rate': None}
             else:
                 default_sum = summary
 
             default_packet_att = {'is_valid_packet': None, 'inlay_type': None}
             default_dict = {**default_data, **default_sum, **default_packet_att}
             default_ordered_dict = {k: default_dict[k] for k in self.packet_headers_default}
-            dict_to_csv(dict_in=default_ordered_dict, path=packets_data_path, append=(not only_titles),
-                        only_titles=only_titles)
+            self.dict_to_csv(dict_in=default_ordered_dict, path=packets_data_path, append=(not only_titles),
+                             only_titles=only_titles)
 
         if res is not None:
             test_data['status_offline'] = int(res.get_total_test_status())
             if test_data['status_offline'] == 0:
-                test_data['external_id'] = ''
+                test_data['external_id'] = None
             test_data['total_test_duration'] = res.get_total_test_duration()
             test_data['fail_bin'] = res.get_total_fail_bin()
             test_data['fail_bin_str'] = res.get_total_fail_bin(as_name=True)
             test_data['trigger_time'] = res.get_trigger_time()
             for i, r in enumerate(res):
                 test_data['test_num'] = i
                 r_sum = r.get_summary()
@@ -1606,15 +1533,15 @@
 
     def run_data_init(self):
         global run_start_time, common_run_name, tested
         if self.value['toPrint'] == 'Yes':
 
             self.init_external_id = self.printing_value['firstPrintingValue']
             self.string_before_counter = self.printing_value['stringBeforeCounter']
-            printing_format = self.ports_and_guis.Tag_Value['printingFormat']
+            printing_format = self.printing_value['printingFormat']
             print_pass_job_name = self.printing_value['passJobName']
             self.printed_external_id, is_ok = get_printed_value(string_before_the_counter=self.string_before_counter,
                                                                 digits_in_counter=4,
                                                                 first_counter=self.init_external_id,
                                                                 printing_format=printing_format)
 
         else:
@@ -1640,29 +1567,28 @@
                          'conversion_type': ConversionTypes(self.ports_and_guis.Tag_Value['conversion']).name,
                          'inlay': InlayTypes(self.ports_and_guis.Tag_Value['inlay']).name,
                          'test_suite': self.ports_and_guis.Tag_Value['inlayType'],
                          'test_suite_dict': self.ports_and_guis.tests_suite,
                          'surface': SurfaceTypes(self.ports_and_guis.Tag_Value['surface']).name,
                          'to_print': self.ports_and_guis.Tag_Value['toPrint'],
                          'qr_validation': self.ports_and_guis.Tag_Value['QRRead'],
-                         'qr_offset': self.ports_and_guis.Tag_Value['QRoffset'],
                          'print_pass_job_name': print_pass_job_name, 'printing_format': printing_format,
                          'external_id_prefix': self.string_before_counter,
                          'external_id_suffix_init_value': self.init_external_id,
                          'coupler_partnumber': '',
                          'gw_version': self.ports_and_guis.ver, 'py_wiliot_version': get_version(), 'upload_date': None,
                          'owner_id': 'wiliot-ops', 'temperature_sensor_enable': self.ports_and_guis.temperature_enabled,
                          'ttfp_avg': float('nan')}
 
         self.test_data = {'common_run_name': common_run_name, 'tag_run_location': tested,
                           'total_location_duration': None, 'total_test_duration': None,
                           'status_offline': False, 'fail_bin': FailureCodes.NONE.value,
                           'fail_bin_str': FailureCodes.NONE.name,
                           'external_id': self.printed_external_id,
-                          'label_validated_at_loc': self.events.qr_val.is_set(), 'trigger_time': None,
+                          'qr_validated': self.qr_enable, 'trigger_time': None,
                           'test_num': 0, 'temperature_sensor': float(-1), 'tag_reel_location': self.tag_reel_location}
 
 
 class R2RThread(threading.Thread):
     """
     Thread that controls R2R machine
 
@@ -1856,15 +1782,14 @@
         # both printer and tag thread will wait on it. only printer will .clear() it (in printing mode)
         self.r2r_ready = threading.Event()
         # start qr read_out
         self.qr_queue = Queue()
         self.tag_status_queue = Queue()
         self.start_compare = threading.Event()
         self.qr_read_success = threading.Event()
-        self.qr_val = threading.Event()
         # printer events
         self.was_pass_to_printer = threading.Event()
         self.was_fail_to_printer = threading.Event()
         self.printer_success = threading.Event()
         self.printer_error = threading.Event()
         self.printer_event = or_event_set(self.printer_success, self.printer_error)
         self.printer_validation_success = threading.Event()
@@ -1983,16 +1908,15 @@
 
         self.auto_attenuator_enable = self.Tag_Value['externalAttenuator']
         if self.auto_attenuator_enable:
             try:
                 if self.Tag_Value['attnComport'].upper() == 'AUTO':
                     self.attenuator = Attenuator('API').GetActiveTE()
                 else:
-                    self.attenuator = Attenuator('API',
-                                                 comport='COM' + str(self.Tag_Value['attnComport'])).GetActiveTE()
+                    self.attenuator = Attenuator('API',comport = 'COM'+str(self.Tag_Value['attnComport'])).GetActiveTE()
                 current_attn = self.attenuator.Getattn()
             except Exception as e:
                 raise EquipmentError('Attenuator Error - Verify Attenuator connection')
 
         self.config_equipment(temperature_sensor=True)
 
         # check if the system variable exist
@@ -2003,51 +1927,43 @@
         # serial for GW
         self.GwObj = WiliotGateway(auto_connect=True, logger_name=self.my_logger.gw_logger.name,
                                    is_multi_processes=True, log_dir_for_multi_processes=os.path.join(self.new_path,
                                                                                                      common_run_name))
         self.ver, _ = self.GwObj.get_gw_version()
 
         if 'additionalGW' in self.tests_suite:
-            self.energizerGW = WiliotGateway(logger_name=self.my_logger.gw_logger.name,
-                                             port=self.tests_suite['additionalGW']['port'])
+            self.energizerGW = WiliotGateway(logger_name=self.my_logger.gw_logger.name, port=self.tests_suite['additionalGW']['port'])
             if self.energizerGW.connected:
                 self.energizerGW.reset_gw()
-                sleep(5)
-                self.energizerGW.write('!listen_to_tag_only 1')
-                sleep(1)
-                self.energizerGW.write('!set_tester_mode 1')
-                sleep(1)
-                self.energizerGW.write('!pl_gw_config 0')
                 sleep(1)
-                self.energizerGW.write('!sub1g_sync 1')
+                self.energizerGW.write('!listen_to_tag_only 1', with_ack=True)
+                self.energizerGW.write('!set_tester_mode 1', with_ack=True)
+                self.energizerGW.write('!pl_gw_config 0', with_ack=True)
+                self.energizerGW.write('!sub1g_sync 1', with_ack=True)
 
                 try:
                     self.additional_gw_mode = DualGWMode(self.tests_suite['additionalGW']['mode'])
                 except Exception as e:
                     raise Exception('no mode in additionalGW dict in test suite or invalid mode: {}'.format(e))
 
-                self.energizerGW.config_gw(received_channel=self.tests_suite['additionalGW']['rxChannel'],
-                                           energy_pattern_val=self.tests_suite['additionalGW']['energizingPattern'],
-                                           time_profile_val=self.tests_suite['additionalGW']['timeProfile'],
-                                           output_power_val=self.tests_suite['additionalGW']['gw_output_power'],
-                                           bypass_pa_val=self.tests_suite['additionalGW']['bypass_pa'], with_ack=False,
+                self.energizerGW.config_gw(energy_pattern_val=self.tests_suite['additionalGW']['energizingPattern'],
+                                         time_profile_val=self.tests_suite['additionalGW']['timeProfile'],
+                                         output_power_val=self.tests_suite['additionalGW']['gw_output_power'],
+                                         bypass_pa_val=self.tests_suite['additionalGW']['bypass_pa'],with_ack=True,
                                            start_gw_app=False)
                 if 'sub1g_power' in self.tests_suite['additionalGW']:
-                    sleep(1)  # sometimes when commands sends one after another the uart failed
                     self.energizerGW.config_gw(sub1g_output_power_val=self.tests_suite['additionalGW']['sub1g_power'],
-                                               start_gw_app=False)
+                                               with_ack=True, start_gw_app=False)
 
                 if 'gw_commands' in self.tests_suite['additionalGW']:
                     if len(self.tests_suite['additionalGW']['gw_commands']) > 0:
                         for command in self.tests_suite['additionalGW']['gw_commands']:
-                            sleep(1)  # sometimes when commands sends one after another the uart failed
-                            self.energizerGW.write(command)
+                            self.energizerGW.write(command, with_ack=True)
                 if self.additional_gw_mode == DualGWMode.STATIC:
-                    sleep(1)  # sometimes when commands sends one after another the uart failed
-                    self.energizerGW.write('!gateway_app')
+                    self.energizerGW.write('!gateway_app', with_ack=True)
 
         else:
             self.energizerGW = False
 
 
 
         # for Printer thread ###########
@@ -2071,15 +1987,14 @@
         self.R2R_myGPIO = R2rGpio()
 
     def open_printer_socket(self):
         """
         opens the printer socket
         """
         self.Printer_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self.Printer_socket.settimeout(PRINTER_SOCKET_TIMEOUT)
         self.Printer_socket.connect((self.configs_for_printer_values['TCP_IP'],
                                      int(self.configs_for_printer_values['TCP_PORT'])))
 
     def update_printer_gui_inputs(self):
         """
         save the last pass value for crash support.
         passed global variable will be updated at tag Thread and should be correct here
@@ -2380,30 +2295,29 @@
 
             if (self.printer is not None and not self.printer.exception_queue.empty()) or \
                     not self.tag_checker_thread.exception_queue.empty() or not self.r2r_thread.exception_queue.empty():
                 self.events.stop_to_r2r_thread.set()
                 self.handle_r2r_exception()
                 self.init_ok = False
 
+            if self.to_scan == 'Yes':
+                self.tag_comparing_qr = QRThread(self.events, self.ports_and_guis)
+
             self.events.tag_thread_is_ready_to_main.wait()
             self.events.tag_thread_is_ready_to_main.clear()
 
             self.pass_job_name = self.tag_checker_thread.printing_value['passJobName']  # will be set inside config
             self.to_print = self.tag_checker_thread.to_print
             self.start_value = int(self.tag_checker_thread.printing_value['firstPrintingValue'])
 
             # printer set-up ####################################################################
             # happens here so we will wait less until the printer will start up (will happen in the background)
             if self.to_print:
                 self.printer = Printer(self.start_value, self.pass_job_name, self.events, self.ports_and_guis)
                 self.look_for_exceptions()
-
-            if self.to_scan == 'Yes':
-                self.tag_comparing_qr = QRThread(self.events, self.ports_and_guis, print=self.to_print)
-
             self.gw_version = self.ports_and_guis.ver
             self.wiliot_ver = get_version()
             self.open_ui()  # starts recurring_timer() that starts look_for_exceptions()
             if self.init_ok:
                 self.r2r_thread.start()
                 self.tag_checker_thread.start()
                 self.events.tag_thread_is_ready_to_main.wait()
@@ -2417,17 +2331,14 @@
                         self.printer.start()
                     self.events.printer_event.wait()
                     if self.events.printer_success.isSet():
                         self.events.printer_success.clear()
                         msg = 'Printer is ready to start'
                         printing_func(msg, 'MainWindow', lock_print, logger_type='debug',
                                       logger_name=self.ports_and_guis.my_logger.logger.name)
-                else:
-                    if self.to_scan == 'Yes':
-                        self.tag_comparing_qr.start()
 
                 self.events.start_to_r2r_thread.set()
         except Exception:
             exception_details = sys.exc_info()
             msg = 'Exception detected during initialization:'
             try:
                 printing_func(msg, 'MainWindow', lock_print, logger_type='warning',
@@ -2537,15 +2448,15 @@
     def stop_fn(self):
         """
         will be triggered by the Stop button and will end the run.
         will upload run's data to cloud and close the threads.
         """
         self.final_close = True
         self.events.done_to_r2r_thread.set()
-        global tested, passed, missing_labels, responded
+        global tested, passed, missing_labels
         global last_pass_string, under_threshold, problem_in_locations_hist, fail_bin_list
         global reel_name
         if tested == 0:
             yield_ = -1.0
         else:
             if tested > 1:
                 # if tested > passed:
@@ -2615,15 +2526,15 @@
         env_dirs = WiliotDir()
         WILIOT_DIR = env_dirs.get_wiliot_root_app_dir()
         machine_dir = join(WILIOT_DIR, 'offline')
         local_config_dir = join(machine_dir, 'configs')
 
         if self.to_print:
             self.events.done_to_printer_thread.set()
-            printing_format = self.ports_and_guis.Tag_Value['printingFormat']
+            printing_format = self.tag_checker_thread.value['printingFormat']
             if printing_format == 'Test':
                 filename = 'gui_printer_inputs_4_Test_do_not_delete.json'
             else:
                 filename = 'gui_printer_inputs_4_SGTIN_do_not_delete.json'
 
             app_dir = os.path.abspath(os.path.dirname(__file__))
             self.folder_path = join(app_dir, 'configs')
@@ -2652,33 +2563,23 @@
 
         res = None
         if values['upload'] == 'Yes':
             if tested > 0:
                 try:
                     res = upload_to_cloud_api(batch_name=reel_name, tester_type='offline-test',
                                               run_data_csv_name=self.ports_and_guis.my_logger.run_data_path,
-                                              packets_data_csv_name=self.ports_and_guis.my_logger.packets_data_path,
-                                              env=self.ports_and_guis.env,
-                                              owner_id=self.ports_and_guis.Tag_Value['OwnerId'],
+                                              tags_data_csv_name=self.ports_and_guis.my_logger.packets_data_path,
+                                              to_logging=True, env=self.ports_and_guis.env,
                                               logger_=self.ports_and_guis.my_logger.gw_logger.name, is_path=True,
-                                              client=self.client)
+                                              client=self.client, packets_instead_tags=True)
                     sleep(2)
                 except Exception:
                     exception_details = sys.exc_info()
                     print_exception(exception_details=exception_details, printing_lock=lock_print)
                     res = False
-
-                if not res:
-                    SimGUI.popup_ok("Run upload failed. Check exception error at the console and check Internet connection is available and upload logs manually",
-                                    title='Upload Error',
-                                    font='Calibri',
-                                    keep_on_top=True,
-                                    auto_close=False,
-                                    no_titlebar=True)
-
             else:
                 self.ports_and_guis.my_logger.results_logger.warning(
                     'tested value is incorrect, please check run_data file')
                 res = False
 
             if not res:
                 msg = 'Upload to cloud failed!!!!!!!!!\ngot an error while uploading to cloud'
@@ -2688,22 +2589,18 @@
                 self.ports_and_guis.my_logger.results_logger.info('Uploaded to cloud ' + str(res))
         else:
             self.ports_and_guis.my_logger.results_logger.info('Uploaded to cloud? No')
 
         if res is not None and not self.no_gui:
             upload_conclusion(failed_tags=None, succeeded_csv_uploads=res)
         try:
-            try:
-                responded_yield = (responded * 100)/tested
-            except Exception:
-                responded_yield = -1
             msg = "Stopped by the operator.\n" + 'Reels yield_over_time is: |' + str(self.yield_over_time) + \
                   '| interval: |' + str(self.calculate_interval) + '|, on: |' + str(self.calculate_on) + \
                   '\nLast words: ' + values['comments'] + '\nTested = ' + str(tested) + ', Passed = ' + str(passed) + \
-                  'Responded Yield = ' + str(responded_yield) + '%, Yield = ' + str(yield_) + '%' + ', Missing labels = ' + str(missing_labels)
+                  ', Yield = ' + str(yield_) + '%' + ', Missing labels = ' + str(missing_labels)
             printing_func(msg, 'MainWindow', lock_print, logger_type='info',
                           logger_name=self.ports_and_guis.my_logger.results_logger.name)
         except Exception:
             self.ports_and_guis.my_logger.results_logger.warning('User finished the run from GUI')
         try:
             self.ports_and_guis.GwObj.exit_gw_api()
         except:
@@ -2715,25 +2612,23 @@
         time.sleep(1)
         sys.exit(0)
 
     def recurring_timer(self):
         """
         update the runs main GUI, checks that the other threads are OK (no exceptions)
         """
-        global tested, passed, missing_labels, black_list_size, responded
+        global tested, passed, missing_labels, black_list_size
         global last_pass_string, reel_name
 
         if tested == 0:
             yield_ = -1.0
-            responded_yield = -1
             self.reel_label.setText("Reel Name: " + reel_name)
         else:
             yield_ = passed / tested * 100
-            responded_yield = responded/tested*100
-        self.tested.setText('Tested = ' + str(tested) + ', Passed = ' + str(passed) + ', Responded Yield = ' + str(responded_yield) + '%, Yield = ' +
+        self.tested.setText('Tested = ' + str(tested) + ', Passed = ' + str(passed) + ', Yield = ' +
                             '{0:.4g}'.format(yield_) + '%' + '\nMissing labels = ' + str(missing_labels) +
                             ', black list size = ' + str(black_list_size))
         self.last_pass.setText(last_pass_string)
         # update the graph, if there was change in the tested amount
         # because passed and tested are been updated in different times
         # we will check the passed of the prev tag => tested -1
         if tested > self.last_tested_num:
@@ -2951,14 +2846,17 @@
                     run_dict_list = [{k: v[0] for k, v in run_dict.items()}]
                     with open(self.ports_and_guis.my_logger.run_data_path, 'w', newline='') as f:
                         csv_writer = csv.DictWriter(f, run_dict.keys())
                         csv_writer.writeheader()
                         csv_writer.writerows(run_dict_list)
                         f.close()
 
+
+
+
 def set_attn_power_offline(attn_obj, attn_power, simulation=False):
     """
     configure Attenuator to a specific value
     gets:
         attn_obj:       Attenuator obj
         attn_power:     value to set attn
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/offline_utils.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/offline_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,35 +105,34 @@
                                        'batchName': 'test_reel',
                                        'tagGen': 'N/A',
                                        'inlayType': 'Ble_Test_Only', 'inlay': InlayTypes.TEO_086.value,
                                        'desiredTags': '9999999', 'desiredPass': '9999999',
                                        'surface': SurfaceTypes.AIR.value,
                                        'conversion': ConversionTypes.STANDARD.value, 'blackListAfter': '2',
                                        'Environment': 'production', 'OwnerId': 'wiliot-ops', 'operator': '',
-                                       'QRRead': 'No', 'QRcomport': 'COM3', 'QRoffset': '2', 'maxQRWrongTags': '1',
-                                       'QRtimeout': '200',
+                                       'QRRead': 'No', 'QRcomport': 'COM3', 'QRoffset': '2', 'maxQRWrongTags': '2',
                                        'comments': '', 'maxFailStop': '50', 'maxYieldStop': '40'}
         elif gui_type == 'Test':
             self.default_gui_values = {'passJobName': 'SGTIN_QR', 'passJobNum': 2, 'sgtin': 'test_test_test_test_X_',
                                        'stringBeforeCounter': 'test',
                                        'reelNumManually': 'test', 'firstPrintingValue': '0', 'tagLocation': '0',
                                        'tag_reel_location': '0',
-                                       'enableLineSelection': 'Yes'}
+                                       'enableLineSelection': 'No'}
         elif gui_type == 'SGTIN':
             self.default_gui_values = {'passJobName': 'SGTIN_QR', 'passJobNum': 2, 'sgtin': '(01)00850027865010(21)',
                                        'stringBeforeCounter': '',
                                        'reelNumManually': '', 'firstPrintingValue': '0', 'tagLocation': '0',
                                        'tag_reel_location': '0',
-                                       'enableLineSelection': 'Yes'}
+                                       'enableLineSelection': 'No'}
         elif gui_type == 'Barcode':
             self.default_gui_values = {'passJobName': 'BARCODE_8', 'passJobNum': 3, 'sgtin': '',
                                        'stringBeforeCounter': '',
                                        'reelNumManually': '', 'firstPrintingValue': '0', 'tagLocation': '0',
                                        'tag_reel_location': '0',
-                                       'enableLineSelection': 'Yes'}
+                                       'enableLineSelection': 'No'}
         else:
             self.default_gui_values = {}
 
 
 def simple_calibration_gui():
     """
     open pop up window
@@ -253,15 +252,15 @@
         pathlib.Path(dir_config).mkdir(parents=True, exist_ok=True)
         with open(configuration_dir, 'w') as output:
             configuration = default_calibration()
             json.dump(configuration, output, indent=2, separators=(", ", ": "), sort_keys=False)
 
     wiliot_logo = join('docs', 'wiliot_logo.png')
     wiliot_logo_image = Image.open(wiliot_logo)
-    wiliot_logo_image = wiliot_logo_image.resize((128, 50), Image.LANCZOS)
+    wiliot_logo_image = wiliot_logo_image.resize((128, 50), Image.ANTIALIAS)
     wiliot_logo_image.save(wiliot_logo, format="png")
 
     folder_name = 'configs'
     file_name = 'gui_inputs_do_not_delete.json'
     gui_inputs_values = open_json(folder_path=folder_name, file_path=os.path.join(folder_name, file_name),
                                   default_values=DefaultGUIValues(gui_type='Main').default_gui_values)
     for key in DefaultGUIValues(gui_type='Main').default_gui_values.keys():
@@ -271,58 +270,57 @@
     EXTEND_KEY = '-SECTION-'
     SimGUI.theme('GreenTan')
     inlay_group = tuple(list(InlayTypes._value2member_map_))
     conversion_group = tuple(list(ConversionTypes._value2member_map_))
     surface_group = tuple(list(SurfaceTypes._value2member_map_))
 
     main_data_tab = [[SimGUI.Text('Reel_name:', size=(40, 1)), SimGUI.InputText(gui_inputs_values['batchName'],
-                                                                                key='batchName')],
-                     [SimGUI.Text('Operator:', size=(40, 1)), SimGUI.InputText(gui_inputs_values['operator'],
-                                                                               key='operator')],
-                     [SimGUI.InputCombo(('D'), visible=False, default_value='D3', key='tagGen')],
-                     [SimGUI.Text('Test suite:', size=(40, 1)),
-                      SimGUI.InputCombo(inlay_type_list, default_value=gui_inputs_values['inlayType'],
-                                        key='inlayType')],
-                     [SimGUI.Text('Environment', size=(40, 1), visible=True),
-                      SimGUI.InputCombo((tuple(['test', 'production'])), default_value=gui_inputs_values['Environment'],
-                                        key='Environment', visible=True)],
-                     [SimGUI.Text('Owner Id', size=(40, 1), visible=True),
-                      SimGUI.InputCombo((tuple(['wiliot-ops'])), default_value=gui_inputs_values['OwnerId'],
-                                        key='OwnerId', visible=True)],
+                                                                             key='batchName')],
+                  [SimGUI.Text('Operator:', size=(40, 1)), SimGUI.InputText(gui_inputs_values['operator'],
+                                                                             key='operator')],
+                  [SimGUI.InputCombo(('D'), visible=False, default_value='D3', key='tagGen')],
+                  [SimGUI.Text('Test suite:', size=(40, 1)),
+                   SimGUI.InputCombo(inlay_type_list, default_value=gui_inputs_values['inlayType'],
+                                     key='inlayType')],
+                 [SimGUI.Text('Environment', size=(40, 1), visible=True),
+                  SimGUI.InputCombo((tuple(['test', 'production'])), default_value=gui_inputs_values['Environment'],
+                                    key='Environment', visible=True)],
+                [SimGUI.Text('Owner Id', size=(40, 1), visible=True),
+                  SimGUI.InputCombo((tuple(['wiliot-ops'])), default_value=gui_inputs_values['OwnerId'],
+                                    key='OwnerId', visible=True)],
                      [SimGUI.Text('', size=(40, 1))],
                      [SimGUI.Text('', size=(40, 1))],
-                     [SimGUI.Text('Comments:', size=(40, 1)), SimGUI.InputText(gui_inputs_values['comments'],
-                                                                               key='comments')]]
+                  [SimGUI.Text('Comments:', size=(40, 1)), SimGUI.InputText(gui_inputs_values['comments'],
+                                                                            key='comments')]]
 
     reel_tab = [[SimGUI.Text('Inlay serial number (3 digits):', size=(40, 1), visible=True),
                  SimGUI.InputCombo(inlay_group, default_value=gui_inputs_values['inlay'], key='inlay', visible=True)],
                 [SimGUI.Text('Surface:', size=(40, 1), visible=True),
                  SimGUI.InputCombo((surface_group),
                                    default_value=gui_inputs_values['surface'], key='surface',
                                    visible=True)],
                 [SimGUI.Text('Conversion', size=(40, 1), visible=True),
                  SimGUI.InputCombo((conversion_group), default_value=gui_inputs_values['conversion'],
                                    key='conversion', visible=True)],
                 [SimGUI.Text('External attenuator', size=(40, 1)),
                  SimGUI.Checkbox('', default=False, key='externalAttenuator',
                                  disabled=False, visible=True)],
                 [SimGUI.Text('QR ComPort: ', size=(40, 1), visible=True),
-                 SimGUI.Spin(values=['Auto', 1, 2, 3, 4, 5, 6, 7, 8, 10, 11, 12, 13, 14, 15, 16, 17, 18],
-                             initial_value=('Auto'),
+                 SimGUI.Spin(values=['Auto',1,2,3,4,5,6,7,8,10,11,12,13,14,15,16,17,18], initial_value=('Auto'),
                              size=(6, 1), key='attnComport')],
                 [SimGUI.Text('Attenuation value:', size=(40, 1)),
                  SimGUI.Spin(values=[i for i in range(5, 20)], key='attnval',
                              initial_value=5,
                              size=(6, 1))]]
 
     print_tab = [[SimGUI.Text('To print?', size=(40, 1)),
                   SimGUI.InputCombo(('Yes', 'No'), default_value=gui_inputs_values['toPrint'], key='toPrint')],
                  [SimGUI.Text('What is the printing job format?', size=(40, 1)),
                   SimGUI.InputCombo(('Test', 'SGTIN', 'Barcode'), default_value=gui_inputs_values['printingFormat']
-                                    if gui_inputs_values['printingFormat'] != 'Test' else 'SGTIN', key='printingFormat')],
+                  if gui_inputs_values['printingFormat'] != 'Test' else 'SGTIN', key='printingFormat')],
                  [SimGUI.Text('printing offset', size=(40, 1)),
                   SimGUI.Spin(values=[i for i in range(0, 5)], initial_value=int(gui_inputs_values['printOffset']),
                               size=(6, 1), key='printOffset')],
                  [SimGUI.Text('QR Validation:', size=(40, 1)),
                   SimGUI.InputCombo(('Yes', 'No'), visible=True, default_value=gui_inputs_values["QRRead"],
                                     key='QRRead')],
                  [SimGUI.Text('Max QR wrong readouts in row:', size=(40, 1)),
@@ -332,18 +330,14 @@
                   SimGUI.Spin(values=[i for i in range(1, 15)], initial_value=(
                       int(gui_inputs_values['QRcomport'][-1]) if len(str(gui_inputs_values['QRcomport'])) > 1 else int(
                           gui_inputs_values['QRcomport'])),
                               size=(6, 1), key='QRcomport')],
                  [SimGUI.Text('QR offset (tags between GW and QR scanner):', size=(40, 1), visible=True),
                   SimGUI.Spin(values=[i for i in range(1, 10)], initial_value=int(gui_inputs_values['QRoffset']),
                               size=(6, 1), key='QRoffset')],
-                 [SimGUI.Text('QR Timeout:', size=(40, 1), visible=True),
-                  SimGUI.Spin(values=[i for i in range(100, 1000, 100)],
-                              initial_value=int(gui_inputs_values['QRtimeout']),
-                              size=(6, 1), key='QRtimeout')],
                  [SimGUI.Text('Max appears before entering black list (min=2)',
                               size=(40, 1)),
                   SimGUI.Spin(values=[i for i in range(1, 100)],
                               initial_value=int(
                                   gui_inputs_values['blackListAfter']),
                               size=(6, 1), key='blackListAfter')]]
 
@@ -372,24 +366,25 @@
                                         size=(40, 2)),
                             SimGUI.InputText(gui_inputs_values['desiredTags'], key='desiredTags')],
                            [SimGUI.Text('Desired amount of pass\n(will stop the run after this amount of passes):',
                                         size=(40, 2)),
                             SimGUI.InputText(gui_inputs_values['desiredPass'], key='desiredPass')]]
 
     layout = [
-        [SimGUI.Image(wiliot_logo)],
-        [SimGUI.TabGroup(
-            [[
-                SimGUI.Tab('Main Run Data', main_data_tab),
-                SimGUI.Tab('Reel Data', reel_tab),
-                SimGUI.Tab('Stop Condition', stop_conditiona_tab),
-                SimGUI.Tab('Printing', print_tab)]])],
-        [SimGUI.Submit(button_color=('white', '#0e6251')), SimGUI.Button('Simple Calibration'),
-         SimGUI.Button('Advanced Calibration'),
-         SimGUI.Text('version: {}'.format(get_version()), font='Helvetica 10 bold')]]
+                [SimGUI.Image(wiliot_logo)],
+                    [SimGUI.TabGroup(
+                    [[
+                       SimGUI.Tab('Main Run Data', main_data_tab),
+                       SimGUI.Tab('Reel Data', reel_tab),
+                       SimGUI.Tab('Stop Condition', stop_conditiona_tab),
+                       SimGUI.Tab('Printing', print_tab)]])],
+              [SimGUI.Submit(button_color=('white', '#0e6251')), SimGUI.Button('Simple Calibration'),
+               SimGUI.Button('Advanced Calibration'),
+               SimGUI.Text('version: {}'.format(get_version()), font='Helvetica 10 bold')]]
+
 
     window = SimGUI.Window('Offline Tester', layout, font='Calibri')
     calib_val = False
     while True:
         event, values = window.read()
 
         if event is None:
@@ -406,20 +401,20 @@
             # make sure user input is legit
             reel_name_ver = False
             if int(values['printOffset']) != int(gui_inputs_values['printOffset']):
                 # popup warning message:
                 change_in_printing_offset = \
                     SimGUI.popup_ok_cancel('Are you sure you want to change the printing offset?\n'
                                            '(old value:{}, new value: {})?\n'.format(gui_inputs_values['printOffset'],
-                                                                                     values['printOffset']),
+                                                                       values['printOffset']),
                                            keep_on_top=True, font=('normal', 20))
                 if change_in_printing_offset.lower() == 'cancel':
                     values['printOffset'] = gui_inputs_values['printOffset']
                     SimGUI.popup('printing offset was NOT change and equals to {}'.format(values['printOffset']),
-                                 button_type='ok', font=14)
+                                      button_type='ok', font=14)
 
             if ' ' in values['batchName'] or '/' in values['batchName'] or '\\' in values['batchName']:
                 print("Reel name could not contain spaces, '\\' or '/'\nplease fix it and press Submit")
                 continue
 
             else:
                 try:
@@ -432,24 +427,23 @@
                     print("the following values should be numbers (integer): maxMissingLabels, packetThreshold,"
                           "desiredTags, desiredPass, blackListAfter (and should not be smaller than 2")
                     continue
                 yes_no = ['Yes', 'No']
                 if values['toPrint'] not in yes_no:
                     print("the following values should be 'Yes' or 'No': toPrint")
                     continue
-                if values['Environment'] == 'production' and values['toPrint'].lower() == 'yes':
+                if values['Environment'] == 'production' and  values['toPrint'].lower() == 'yes':
                     reel_name_ver = check_structure(values['batchName'])
                 else:
                     reel_name_ver = True
 
                 if reel_name_ver:
                     break
                 else:
-                    SimGUI.popup('Reel name error \n Reel name should be: <6 uppercase alphanumeric chars>.'
-                                 '<2 integers minimum 01 maximum 25>_<upper case char minimum A maximum F>',
+                    SimGUI.popup('Reel name error \n Reel name should be: <6 uppercase alphanumeric chars>.<2 integers minimum 01 maximum 25>_<upper case char minimum A maximum F>'.format(values['printOffset']),
                                  button_type='ok', font=14)
 
         elif event == 'Advanced Calibration':
             # calib_val = True
             # break
             window.hide()
             calib_values = open_calibration_config()
@@ -506,207 +500,219 @@
                 # add the first counter number by order to the string
                 first_print += str(first_counter)
                 break
         is_ok = True
     return first_print, is_ok
 
 
-def gui_inputs_values_for_test_and_sgtin(printing_format):
+def printing_test_window():
     """
-    A function that sends the GUI's input
+    opens the GUI for user input for test print
+    :return: dictionary of user inputs
     """
+    printing_format = 'Test'
     folder_name = 'configs'
-    if printing_format in ('SGTIN', 'Barcode'):
-        file_name = 'gui_printer_inputs_4_SGTIN_do_not_delete.json'
-    else:
-        file_name = 'gui_printer_inputs_4_Test_do_not_delete.json'
+    file_name = 'gui_printer_inputs_4_Test_do_not_delete.json'
     gui_inputs_values = open_json_cache(folder_path=folder_name, file_path=os.path.join(folder_name, file_name),
                                         default_values=DefaultGUIValues(printing_format).default_gui_values)
-    return gui_inputs_values
 
+    # If the JSON file is empty, get those values from the default
+    if gui_inputs_values['reelNumManually'] == "":
+        reel_num = 'test_test_test_test_X_test'
+        gui_inputs_values['sgtin'] = reel_num[:22]
+        gui_inputs_values['reelNumManually'] = reel_num[22:]
+        gui_inputs_values['firstPrintingValue'] = '0'
+        gui_inputs_values['tagLocation'] = '0'
+        gui_inputs_values['tag_reel_location'] = '0'
 
-def printing_process_of_test_and_sgtin(window, printing_format, gui_inputs_values, env='', owner_id='wiliot-ops'):
-    """
-    A function that does all the work of the printing process
-    """
-    read_only = False
-    reel_number = ''
+    # Define the window's contents
+    layout = [[SimGUI.Text('Job to print for pass and fail:'),
+               SimGUI.InputCombo(('SGTIN_only', 'SGTIN_QR', 'BARCODE_8', 'devkit_TEO', 'devkit_TIKI', 'empty'),
+                                 default_value=gui_inputs_values['passJobName'], key='passJobName')],
+              [SimGUI.Text('pass line number:'),
+               SimGUI.Input(gui_inputs_values['passJobNum'], key='passJobNum')],
+              [SimGUI.Text("What is the first counter number?")],
+              [SimGUI.Input(gui_inputs_values['firstPrintingValue'], key='firstPrintingValue')],
+              [SimGUI.Checkbox('Insert reel number manually?', default=False, key='isManually')],
+              [SimGUI.Text("For manual mode only - what is the sgtin number?", key='sgtinNumManuallyText'),
+               SimGUI.Input(gui_inputs_values['sgtin'], key='sgtinNumManually')],
+              [SimGUI.Text("For manual mode only - what is the reel number?", key='reelNumManuallyText'),
+               SimGUI.Input(gui_inputs_values['reelNumManually'], key='reelNumManually')],
+              [SimGUI.Text(size=(60, 3), key='-OUTPUT-')],
+              [SimGUI.Text("*Tags in this run will not be serialized")],
+              [SimGUI.Button('Check first print'), SimGUI.Button('Submit', button_color=('white', '#0e6251'))]]
+
+    # Create the window
+    window = SimGUI.Window('Printing Test', layout, keep_on_top=True)
+
+    # Display and interact with the Window using an Event Loop
     tag_digits_num = 4
     pass_job_name = None
+    reel_number = ''
     is_ok = True
     while True:
         event, values = window.read()
         should_submit = True
-        if printing_format != 'Test':
-            pass_job_name = values['passJobName']
+        # See if user wants to quit or window was closed
         if event == SimGUI.WINDOW_CLOSED or event is None:
             is_ok = False
             break
         if event == 'Submit':
+            # check if the first counter number is int
             try:
-                printing_value = 'First counter number is too big for counter digits number!!\n''Please enter a new first counter number'
-                if (printing_format != 'Test' and not values['isNewReel']) or (
-                        printing_format == 'Test' and not values['isManually']):
+                # to check if it is int as it should
+                tmp = int(values['firstPrintingValue'])
+                # automatic insert
+                if not values['isManually']:
                     pass_job_name = values['passJobName']
                     first_counter = values['firstPrintingValue']
-                    if printing_format == 'Test':
-                        window['sgtinNumManually'].update('test_test_test_test_X_')
-                        window['reelNumManually'].update('test')
+                    window['sgtinNumManually'].update('test_test_test_test_X_')
+                    window['reelNumManually'].update('test')
+                    # Output a message to the window
                     if len(str(values['firstPrintingValue'])) > tag_digits_num:
-                        if printing_format != 'Test':
-                            printing_value += 'you entered: ' + str(
-                                values['firstPrintingValue'] + ' in length of: ' + len(
-                                    str(values['firstPrintingValue'])))
-                        window['-OUTPUT-'].update(printing_value)
+                        window['-OUTPUT-'].update(
+                            'First counter number is too big for counter digits number!!\n'
+                            'Please enter a new first counter number')
                         should_submit = False
                     else:
                         should_submit = True
-                        if printing_format != 'Test':
-                            reel_number = str(gui_inputs_values['sgtin']) + str(gui_inputs_values['reelNumManually'])
-                            first_print, is_ok = get_printed_value(reel_number, tag_digits_num, first_counter,
-                                                                   printing_format)
-                            print('The first tag printing value will be: ' + first_print)
-                elif (printing_format != 'Test' and values['isNewReel']) or (
-                        printing_format == 'Test' and values['isManually']):
+
+                # manual input
+                elif values['isManually']:
                     if len(str(values['firstPrintingValue'])) > tag_digits_num:
-                        if printing_format != 'Test':
-                            printing_value += 'you entered: ' + str(
-                                values['firstPrintingValue'] + ' in length of: ' + len(
-                                    str(values['firstPrintingValue'])))
-                        window['-OUTPUT-'].update(printing_value)
+                        window['-OUTPUT-'].update(
+                            'First counter number is too big for counter digits number!!\n'
+                            'Please enter a new first counter number')
                         should_submit = False
-                    elif (printing_format == 'SGTIN' or 'SGTIN' in values['passJobName']) and not len(
-                            str(values['sgtinNumManually'])) == 22:
+
+                    elif 'SGTIN' in values['passJobName'] and not len(str(values['sgtinNumManually'])) == 22:
                         window['-OUTPUT-'].update(
                             'SGTIN number is not equal to 22 chars!!\n'
-                            'Please enter correct SGTIN, its length is: ' + str(len(str(values['sgtinNumManually']))))
+                            'Please enter correct SGTIN, length: ' + str(len(str(values['sgtinNumManually']))))
                         should_submit = False
-                    elif (printing_format == 'SGTIN' or 'SGTIN' in values['passJobName']) and not len(
-                            str(values['reelNumManually'])) == 4:
+
+                    elif 'SGTIN' in values['passJobName'] and not len(str(values['reelNumManually'])) == 4:
                         window['-OUTPUT-'].update(
                             'Reel number is not equal to 4 chars!!\n'
                             'Please enter correct Reel number')
                         should_submit = False
-                    elif (printing_format == 'Barcode' or 'Barcode' in values['passJobName']) and len(
-                            values['reelNumManually']) != 3:
+
+                    elif 'Barcode' in values['passJobName'] and len(values['reelNumManually']) != 3:
                         window['-OUTPUT-'].update(
                             'Reel number is not equal to 3 chars!!\n'
                             'Please enter correct Reel number')
-                        if printing_format == 'Barcode':
-                            should_submit = False
+
                     else:
                         pass_job_name = values['passJobName']
-                        reel_number = str(values['sgtinNumManually']) + str(values['reelNumManually'])
+                        reel_number = values['sgtinNumManually'] + values['reelNumManually']
                         first_counter = values['firstPrintingValue']
                         first_print, is_ok = get_printed_value(reel_number, tag_digits_num,
                                                                first_counter, printing_format)
-                        if printing_format == 'Test':
-                            window['-OUTPUT-'].update('The first tag printing value will be:\n' + first_print)
-                        else:
-                            print('The first tag printing value will be: ' + first_print)
+                        # Output a message to the window
+                        window['-OUTPUT-'].update('The first tag printing value will be:\n' + first_print)
                         should_submit = True
-
             except Exception:
-
                 window['-OUTPUT-'].update(
-
                     'First counter is not a number!!\nPlease enter a new first counter number')
-
                 should_submit = False
 
             if should_submit:
                 break
-    if (printing_format != 'Test' and is_ok) or (printing_format == 'Test'):
-        v = {'passJobName': pass_job_name, 'digitsInCounter': tag_digits_num, 'passJobNum': values['passJobNum'],
-             'firstPrintingValue': values['firstPrintingValue'], 'tagLocation': values['firstPrintingValue'],
-             'tag_reel_location': gui_inputs_values['tag_reel_location'],
-             'enableLineSelection': gui_inputs_values['enableLineSelection']}
 
-        data_to_save = {'passJobName': pass_job_name,
-                        'passJobNum': values['passJobNum'],
-                        'sgtin': values['sgtinNumManually'],
-                        'reelNumManually': values['reelNumManually'],
-                        'enableLineSelection': gui_inputs_values['enableLineSelection'],
-                        'firstPrintingValue': values['firstPrintingValue'],
-                        'tagLocation': values['firstPrintingValue'],
-                        'tag_reel_location': gui_inputs_values['tag_reel_location']}
+        if event == 'Check first print':
+            try:
+                tmp = int(values['firstPrintingValue'])
+                # automatic input
+                if not values['isManually']:
+
+                    window['sgtinNumManually'].update('test_test_test_test_X_')
+                    window['reelNumManually'].update('test')
+                    reel_number = values['sgtinNumManually'] + values['reelNumManually']
+                    first_counter = values['firstPrintingValue']
+                    first_print, is_ok = get_printed_value(reel_number, tag_digits_num,
+                                                           first_counter, printing_format)
 
-        if printing_format != 'Test':
-            v['stringBeforeCounter'] = reel_number
-            v['failJobName'] = 'line_'
-            v['printingFormat'] = printing_format
-            data_to_save['stringBeforeCounter'] = reel_number
-            data_to_save['printingFormat'] = printing_format
-        elif printing_format == 'Test':
-            v['stringBeforeCounter'] = values['sgtinNumManually'] + values['reelNumManually']
-            v['failJobName'] = pass_job_name
-        folder_name = 'configs'
-        file_name = 'gui_printer_inputs_4_SGTIN_do_not_delete.json'
-        f = open(os.path.join(folder_name, file_name), "w")
-        json.dump(data_to_save, f)
-        f.close()
-        return v, is_ok
+                    # Output a message to the window
+                    if len(str(values['firstPrintingValue'])) > tag_digits_num:
+                        window['-OUTPUT-'].update('First counter number is too big for counter digits number!!\n'
+                                                  'Please enter a new first counter number')
+                    else:
+                        window['-OUTPUT-'].update('The first tag printing value will be:\n' + first_print)
+                        print('The first tag printing value will be: ' + first_print)
 
-    return gui_inputs_values, is_ok
 
+                # manual input
+                elif values['isManually']:
+                    if len(str(values['firstPrintingValue'])) > tag_digits_num:
+                        window['-OUTPUT-'].update('First counter number is too big for counter digits number!!\n'
+                                                  'Please enter a new first counter number')
 
-def printing_test_window():
-    """
-    opens the GUI for user input for test print
-    :return: dictionary of user inputs
-    """
-    printing_format = 'Test'
-    gui_inputs_values = gui_inputs_values_for_test_and_sgtin(printing_format)
+                    elif 'SGTIN' in values['passJobName'] and not len(str(values['sgtinNumManually'])) == 22:
+                        window['-OUTPUT-'].update(
+                            'SGTIN number is not equal to 22 chars!!\n'
+                            'Please enter correct SGTIN, its length is: ' + str(len(str(values['sgtinNumManually']))))
 
-    if gui_inputs_values['reelNumManually'] == "":
-        reel_num = 'test_test_test_test_X_test'
-        gui_inputs_values['sgtin'] = reel_num[:22]
-        gui_inputs_values['reelNumManually'] = reel_num[22:]
-        gui_inputs_values['firstPrintingValue'] = '0'
-        gui_inputs_values['tagLocation'] = '0'
-        gui_inputs_values['tag_reel_location'] = '0'
+                    elif 'SGTIN' in values['passJobName'] and not len(str(values['reelNumManually'])) == 4:
+                        window['-OUTPUT-'].update(
+                            'Reel number is not equal to 4 chars!!\n'
+                            'Please enter correct Reel number')
 
-    layout = [[SimGUI.Text('Job to print for pass and fail:'),
-               SimGUI.InputCombo(('SGTIN_only', 'SGTIN_QR', 'BARCODE_8', 'devkit_TEO', 'devkit_TIKI', 'empty'),
-                                 default_value=gui_inputs_values['passJobName'], key='passJobName')],
-              [SimGUI.Text('pass line number:'),
-               SimGUI.Input(gui_inputs_values['passJobNum'], key='passJobNum')],
-              [SimGUI.Text("What is the first counter number?")],
-              [SimGUI.Input(gui_inputs_values['firstPrintingValue'], key='firstPrintingValue')],
-              [SimGUI.Checkbox('Insert reel number manually?', default=False, key='isManually')],
-              [SimGUI.Text("For manual mode only - what is the sgtin number?", key='sgtinNumManuallyText'),
-               SimGUI.Input(gui_inputs_values['sgtin'], key='sgtinNumManually')],
-              [SimGUI.Text("For manual mode only - what is the reel number?", key='reelNumManuallyText'),
-               SimGUI.Input(gui_inputs_values['reelNumManually'], key='reelNumManually')],
-              [SimGUI.Text(size=(60, 3), key='-OUTPUT-')],
-              [SimGUI.Text("*Tags in this run will not be serialized")],
-              [SimGUI.Button('Check first print'), SimGUI.Button('Submit', button_color=('white', '#0e6251'))]]
-    window = SimGUI.Window('Printing Test', layout, keep_on_top=True)
-    wanted_v, wanted_is_ok = printing_process_of_test_and_sgtin(window, printing_format, gui_inputs_values)
+                    elif 'Barcode' in values['passJobName'] and len(values['reelNumManually']) != 3:
+                        window['-OUTPUT-'].update(
+                            'Reel number is not equal to 3 chars!!\n'
+                            'Please enter correct Reel number')
+
+                    else:
+                        pass_job_name = values['passJobName']
+                        reel_number = values['sgtinNumManually'] + values['reelNumManually']
+                        first_counter = values['firstPrintingValue']
+                        first_print, is_ok = get_printed_value(reel_number, tag_digits_num,
+                                                               first_counter, printing_format)
+                        # Output a message to the window
+                        window['-OUTPUT-'].update('The first tag printing value will be:\n' + first_print)
+            except Exception:
+                window['-OUTPUT-'].update(
+                    'First counter is not a number!!\nPlease enter a new first counter number')
+
+    # Finish up by removing from the screen
     window.close()
-    return wanted_v, wanted_is_ok
+    v = {'passJobName': pass_job_name, 'passJobNum': values['passJobNum'],
+         'stringBeforeCounter': values['sgtinNumManually']+values['reelNumManually'],
+         'digitsInCounter': tag_digits_num, 'enableLineSelection': gui_inputs_values['enableLineSelection'],
+         'firstPrintingValue': values['firstPrintingValue'], 'failJobName': pass_job_name,
+         'tagLocation': values['firstPrintingValue'], 'tag_reel_location': gui_inputs_values['tag_reel_location']}
+
+    data_to_save = {'passJobName': pass_job_name, 'passJobNum': values['passJobNum'],
+                    'sgtin': values['sgtinNumManually'], 'reelNumManually': values['reelNumManually'],
+                    'enableLineSelection': gui_inputs_values['enableLineSelection'],
+                    'firstPrintingValue': values['firstPrintingValue'], 'tagLocation': values['firstPrintingValue'],
+                    'tag_reel_location': gui_inputs_values['tag_reel_location']}
+    f = open(os.path.join(folder_name, file_name), "w")
+    json.dump(data_to_save, f)
+    f.close()
+    return v, is_ok
 
 
 def printing_sgtin_window(env='', owner_id='wiliot-ops', printing_format='SGTIN'):
     """
     opens the GUI for user input for SGTIN print
     :return: dictionary of user inputs
     """
     read_only = False
-    gui_inputs_values = gui_inputs_values_for_test_and_sgtin(printing_format)
-
-    # Checking if it's a new reel run and updating the GUI inputs according to this
+    folder_name = 'configs'
+    file_name = 'gui_printer_inputs_4_SGTIN_do_not_delete.json'
+    gui_inputs_values = open_json_cache(folder_path=folder_name, file_path=os.path.join(folder_name, file_name),
+                                        default_values=DefaultGUIValues(printing_format).default_gui_values)
     new_run = SimGUI.popup_yes_no('    New Reel?    \n', keep_on_top=True, font=('normal', 20))
     if new_run == 'Yes':
         gui_inputs_values['tagLocation'] = '0'
         gui_inputs_values['tag_reel_location'] = '0'
         try:
             logging.info('Receiving data from the cloud, please wait')
             reel_num = get_reel_name_from_cloud_api(env, owner_id, printing_format)
-            print(reel_num)
         except Exception:
             logging.warning('Problem with receiving data from cloud')
             raise Exception
         gui_inputs_values['firstPrintingValue'] = '0000'
         if 'data' in reel_num:
             reel_number = reel_num['data']
             if printing_format == 'SGTIN':
@@ -737,23 +743,125 @@
               [SimGUI.Text("SGTIN number", key='sgtinNumManuallyText'),
                SimGUI.Input(gui_inputs_values['sgtin'], key='sgtinNumManually', readonly=read_only)],
               [SimGUI.Text("Reel number", key='reelNumManuallyText'),
                SimGUI.Input(gui_inputs_values['reelNumManually'], key='reelNumManually', readonly=read_only)],
               [SimGUI.Text(size=(60, 3), key='-OUTPUT-')],
               [SimGUI.Text('Tag Location: {}'.format(gui_inputs_values['tagLocation']))],
               [SimGUI.Button('Submit', button_color=('white', '#0e6251'))]]
-    window = SimGUI.Window('Printing Test', layout, keep_on_top=True)
-    wanted_v, wanted_is_ok = printing_process_of_test_and_sgtin(window, printing_format, gui_inputs_values, env,
-                                                                owner_id)
+    window = SimGUI.Window('Printing SGTIN', layout, keep_on_top=True)
+
+    # Display and interact with the Window using an Event Loop
+    # window['-OUTPUT-'].update(
+    tag_digits_num = 4
+    while True:
+        event, values = window.read()
+        should_submit = True
+        pass_job_name = values['passJobName']
+        # See if user wants to quit or window was closed
+        if event == SimGUI.WINDOW_CLOSED or event is None:
+            is_ok = False
+            break
+        if event == 'Submit':
+            # check if the first counter number is int
+            try:
+                # to check if it is int as it should
+                tmp = int(values['firstPrintingValue'])
+                # automatic input
+                if not values['isNewReel']:
+                    # window['sgtinNumManually'].update(readonly=read_only)
+                    pass_job_name = values['passJobName']
+                    first_counter = values['firstPrintingValue']
+                    # Output a message to the window
+                    if len(str(values['firstPrintingValue'])) > tag_digits_num:
+                        window['-OUTPUT-'].update(
+                            'First counter number is too big for counter digits number!!\n'
+                            'Please enter a new first counter number you entered: ' + str(
+                                values['firstPrintingValue'] + ' in length of: ' + len(
+                                    str(values['firstPrintingValue']))))
+                        should_submit = False
+                    else:
+                        reel_number = str(gui_inputs_values['sgtin']) + str(gui_inputs_values['reelNumManually'])
+                        first_print, is_ok = get_printed_value(reel_number, tag_digits_num, first_counter,
+                                                               printing_format)
+                        print('The first tag printing value will be: ' + first_print)
+                        should_submit = True
+
+                # manual input
+                else:
+                    if len(str(values['firstPrintingValue'])) > tag_digits_num:
+                        window['-OUTPUT-'].update(
+                            'First counter number is too big for counter digits number!!\n'
+                            'Please enter a new first counter number you entered: ' + str(
+                                values['firstPrintingValue'] + ' in length of: ' + len(
+                                    str(values['firstPrintingValue']))))
+
+                        should_submit = False
+
+                    elif printing_format == 'SGTIN' and not len(values['sgtinNumManually']) == 22:
+                        window['-OUTPUT-'].update(
+                            'SGTIN number is not equal to 22 chars!!\n'
+                            'Please enter correct SGTIN, its length is: ' + str(len(str(values['sgtinNumManually']))))
+                        should_submit = False
+
+                    elif printing_format == 'SGTIN' and len(values['reelNumManually']) != 4:
+                        window['-OUTPUT-'].update(
+                            'Reel number is not equal to 4 chars!!\n'
+                            'Please enter correct Reel number')
+                        should_submit = False
+
+                    elif printing_format == 'Barcode' and len(values['reelNumManually']) != 3:
+                        window['-OUTPUT-'].update(
+                            'Reel number is not equal to 3 chars!!\n'
+                            'Please enter correct Reel number')
+                        should_submit = False
+
+                    else:
+                        pass_job_name = values['passJobName']
+                        reel_number = str(values['sgtinNumManually']) + str(values['reelNumManually'])
+                        first_counter = values['firstPrintingValue']
+                        first_print, is_ok = get_printed_value(reel_number, tag_digits_num,
+                                                               first_counter, printing_format)
+                        # Output a message to the window
+                        print('The first tag printing value will be: ' + first_print)
+                        should_submit = True
+            except Exception:
+                window['-OUTPUT-'].update(
+                    'First counter is not a number!!\nPlease enter a new first counter number')
+                should_submit = False
+
+            if should_submit:
+                break
+
+    # Finish up by removing from the screen
     window.close()
-    return wanted_v, wanted_is_ok
+    if is_ok:
+        v = {'passJobName': pass_job_name, 'passJobNum': values['passJobNum'], 'stringBeforeCounter': reel_number,
+             'digitsInCounter': tag_digits_num, 'firstPrintingValue': values['firstPrintingValue'],
+             'failJobName': 'line_', 'tagLocation': values['firstPrintingValue'],
+             'tag_reel_location': gui_inputs_values['tag_reel_location'],
+             'enableLineSelection': gui_inputs_values['enableLineSelection'],
+             'printingFormat': printing_format}
+        data_to_save = {'passJobName': pass_job_name, 'passJobNum': values['passJobNum'],
+                        'sgtin': values['sgtinNumManually'], 'reelNumManually': values['reelNumManually'],
+                        'firstPrintingValue': values['firstPrintingValue'], 'stringBeforeCounter': reel_number,
+                        'tagLocation': values['firstPrintingValue'],
+                        'printingFormat': printing_format,
+                        'enableLineSelection': gui_inputs_values['enableLineSelection'],
+                        'tag_reel_location': gui_inputs_values['tag_reel_location']}
+
+        f = open(os.path.join(folder_name, file_name), "w")
+        json.dump(data_to_save, f)
+        f.close()
+        return v, is_ok
+    else:
+        return gui_inputs_values, is_ok
 
 
 def save_screen(tested, passed, yield_, missing_labels, problem_in_locations_hist_val, ttfgp_avg,
-                default_upload_value=None, responded = None):
+                default_upload_value=None):
     """
     open last GUI
     :type tested: int
     :param tested: amount of tested tags
     :type passed: int
     :param passed: amount of passed tags
     :type yield_: float
@@ -780,15 +888,14 @@
     if default_upload_value is not None:
         def_upload = default_upload_value
     else:
         def_upload = "Yes"
 
     layout = [
         [SimGUI.Text('Tags tested = ' + str(tested), size=(21, 1)),
-         SimGUI.Text('Tags responded = ' + str(responded if responded is not None else 0), size=(21, 1)),
          SimGUI.Text('Tags passed = ' + str(passed), size=(21, 1))],
         [SimGUI.Text('Yield = ' + '{0:.4g}'.format(yield_) + '%', size=(21, 2)),
          SimGUI.Text('Missing labels = ' + str(missing_labels), size=(21, 2))],
         ttfgp_avg_line,
         [SimGUI.Text('Would you like to upload this log to the cloud?'),
          SimGUI.InputCombo(('Yes', 'No'), default_value=def_upload, key='upload')],
         [SimGUI.Text('Post run comments:')],
@@ -1104,32 +1211,30 @@
         try:
             # Attempt to open a connection to the specified comport
             self.s = serial.Serial(self.comport, self.baud_rate, timeout=0, write_timeout=0)
             logging.info(f'Connection to Arduino on {self.comport} restablished.')
             reconnect_success = True
 
         except serial.serialutil.SerialException:
-            logging.warning(
-                f'Connection to {self.comport} failed. Attempting to close the connection and detect Arduino...')
+            logging.warning(f'Connection to {self.comport} failed. Attempting to close the connection and detect Arduino...')
             try:
                 self.s.close()
                 time.sleep(1)
                 self.s = serial.Serial(self.comport, self.baud_rate, timeout=0, write_timeout=0)
                 logging.info(f'Connection to Arduino on {self.comport} restablished.')
                 reconnect_success = True
 
             except Exception as e:
                 logging.warning(f"Failed to close connection to {self.comport} {e} - Please restart connection")
                 return
 
         if reconnect_success:
             response = self.query("*IDN?")
             if ("Williot R2R GPIO" in response):
-                logging.info(
-                    'Connection was restablished on COM{} with version {}'.format(response, self.query("SER?")))
+                logging.info('Connection was restablished on COM{} with version {}'.format(response,self.query("SER?")))
                 self.s.flushInput()
             else:
                 self.s.close()
                 logging.warning(f"Failed to close connection to {self.comport} - Please restart connection")
 
 
 if __name__ == '__main__':
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/offline/tadbik_r2r_controller.py` & `wiliot-testers-4.0.6/wiliot_testers/offline/tadbik_r2r_controller.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/com_connect.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/com_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 from os.path import abspath
 from json import dump
 from os.path import join, dirname
 from wiliot_testers.test_equipment import *
 from wiliot_core import WiliotGateway, ActionType, DataType
 from configs_gui import CONFIGS_DIR
 
+logger = logging.getLogger('sample')
+
 barcodeMutex = threading.Lock()
 
 CONNECT_HW = 'Connect HW'
 GO = 'Go'
 CONTINUE = 'Continue'
 READ = 'Read'
 FINISH = 'Finish'
@@ -128,159 +130,154 @@
     barcode_error = []
     chambers_to_close = []
     gw_latest_version = ['']
     gw_update_status = 'disabled'
     start_time = 0
     temperature_sensor_readings = []
     all_sensors = []
-    ttk = None
-
-    def __init__(self, top_builder=None, new_tag_func=None, update_go=None, default_dict=None, logger=None):
+    
+    def __init__(self, top_builder=None, new_tag_func=None, update_go=None, default_dict=None):
         '''
         Constructor
         '''
         self.gateway = WiliotGateway(logger_name='sample')
         self.top_builder = top_builder
         self.add_tag_to_test = new_tag_func
         self.update_go_state = update_go
         self.default_dict = default_dict
-        if logger is None:
-            self.logger = logging.getLogger('sample')
-        else:
-            self.logger = logger
-
+    
     def __del__(self):
         if self.gateway is not None and self.is_gw_serial_open():
             self.gateway.close_port()
-
+        
         for com_port, barcode in self.barcodes_serials.items():
             if barcode is not None and barcode.is_open():
                 barcode.close_port()
-
+        
         for com_port, chamber in self.chambers_serials.items():
             if chamber is not None and chamber.is_connected():
                 chamber.open_chamber()
                 chamber.close_port()
-
+        
         # for com_port, atten in self.atten_serials.items():
         #     if atten!=None and 'serial' in atten.keys() and atten['serial']!=None and atten:
         #         atten.disconnect()
-
+    
     def gui(self, ttk_frame=None):
         self.builder = builder = pygubu.Builder()
         ui_file = join(abspath(dirname(__file__)), 'utils', 'com_connect.ui')
         self.builder.add_from_file(ui_file)
-
+        
         img_path = join(abspath(dirname(__file__)), '')
         builder.add_resource_path(img_path)
         img_path = join(abspath(dirname(__file__)), 'utils')
         builder.add_resource_path(img_path)
-
+        
         self.ttk = ttk_frame
-
+        
         self.ttk.title("ComConnect")
-
+        
         self.mainwindow = self.builder.get_object('mainwindow', self.ttk)
-
+        
         self.builder.connect_callbacks(self)
         self.isGui = True
         self.find_com_ports()
         self.set_gui_defaults()
-
+        
         self.ttk.protocol("WM_DELETE_WINDOW", self.close)
         self.ttk.lift()
         self.ttk.attributes("-topmost", True)
         self.ttk.attributes("-topmost", False)
-
+        
         # self.set_gui_defaults()
-
+        
         self.ttk.mainloop()
-
+    
     def find_com_ports(self, *args):
         com_ports = serial_ports()
         available_ports = [com_port for com_port in com_ports if com_port not in self.used_ports]
-
+        
         self.update_com_gui(available_ports, com_ports)
-
+    
     def set_gui_defaults(self):
-
+        
         if self.serials_connected(CHAMBERS):
             self.builder.get_object('connect_chambers').configure(text='Disconnect')
             self.builder.get_object('chosenChambers')['state'] = 'disabled'
             self.builder.get_object('availableChambers')['state'] = 'disabled'
             self.builder.get_object('chambers_up')['state'] = 'disabled'
             self.builder.get_object('chambers_down')['state'] = 'disabled'
             self.builder.get_object('addChambers')['state'] = 'disabled'
         else:
             self.builder.get_object('connect_chambers').configure(text='Connect')
-
+        
         ble_atten = ''
         lora_atten = ''
         for com_port, atten in self.atten_serials.items():
             ble_atten = com_port if atten['type'] == BLE else ble_atten
             lora_atten = com_port if atten['type'] == LORA else lora_atten
-
+        
         self.builder.get_object('attenComBle').set(ble_atten)
         self.builder.get_object('attenComLoRa').set(lora_atten)
         if self.serials_connected(ATTENUATORS):
             self.builder.get_object('connect_atten').configure(text='Disconnect')
             self.builder.get_object('attenComBle')['state'] = 'disabled'
             self.builder.get_object('attenComLoRa')['state'] = 'disabled'
         else:
             self.builder.get_object('connect_atten').configure(text='Connect')
         pass
-
+    
     def update_com_gui(self, available_ports, com_ports):
         self.builder.get_object('gwCom')['values'] = available_ports + ['']
         self.builder.get_object('attenComBle')['values'] = available_ports + ['']
         self.builder.get_object('attenComLoRa')['values'] = available_ports + ['']
         self.update_multi_serials(available_ports, BARCODES)
         self.update_multi_serials(available_ports, CHAMBERS)
-
+        
         self.missing_com_port = False
-
+        
         self.check_chosen_ports(com_ports)
         self.check_opened_ports()
-
+    
     def check_chosen_ports(self, com_ports):
         if len(self.gw_com_port) == 0 or self.gw_com_port[0] not in com_ports:
             self.gw_com_port = ['']
             self.builder.get_object('gwCom').set('')
             self.missing_com_port = True
-
+        
         i = 0
         while i < len(self.atten_serials.keys()):
             port = list(self.atten_serials.keys())[i]
             atten = list(self.atten_serials.values())[i]
             if port != '' and port not in com_ports:
                 self.atten_serials.pop(port)
                 self.builder.get_object(f"attenCom{atten['type']}").set('')
                 self.missing_com_port = True
                 continue
             i += 1
-
+        
         self.check_multi_coms(BARCODES, com_ports)
         self.check_multi_coms(CHAMBERS, com_ports)
-
+    
     def check_multi_coms(self, obj, com_ports):
         self.builder.get_object(f'chosen{obj}').delete(0, END)
         ports = getattr(self, f'{obj.lower()}_serials')
         for port in ports.keys():
             if port in com_ports:
                 self.builder.get_object(f'chosen{obj}').insert(END, port)
             else:
                 self.missing_com_port = True
-
+    
     def check_opened_ports(self):
         if self.is_gui_opened():
             self.check_gw_open()
             self.check_multi_open(BARCODES)
             self.check_multi_open(CHAMBERS)
             self.check_atten_open()
-
+    
     def check_multi_open(self, obj):
         if self.serials_connected(obj):
             self.builder.get_object(f'connect_{obj.lower()}').configure(text='Disconnect')
             self.builder.get_object(f'chosen{obj}')['state'] = 'disabled'
             self.builder.get_object(f'available{obj}')['state'] = 'disabled'
             self.builder.get_object(f'{obj.lower()}_up')['state'] = 'disabled'
             self.builder.get_object(f'{obj.lower()}_down')['state'] = 'disabled'
@@ -288,15 +285,15 @@
         else:
             self.builder.get_object(f'connect_{obj.lower()}').configure(text='Connect')
             self.builder.get_object(f'chosen{obj}')['state'] = 'normal'
             self.builder.get_object(f'available{obj}')['state'] = 'normal'
             self.builder.get_object(f'{obj.lower()}_up')['state'] = 'normal'
             self.builder.get_object(f'{obj.lower()}_down')['state'] = 'normal'
             self.builder.get_object(f'add{obj}')['state'] = 'normal'
-
+    
     def check_gw_open(self):
         if len(self.gw_com_port) > 0 and self.gw_com_port[0] != '':
             self.builder.get_object('gwCom').set(self.gw_com_port[0])
         if self.is_gw_serial_open():
             self.builder.get_object('connect_gw').configure(text='Disconnect')
             self.builder.get_object('gwCom')['state'] = 'disabled'
             self.builder.get_object('version').configure(text=GW_VERSION + self.gwVersion[0])
@@ -304,35 +301,34 @@
             self.builder.get_object('update_gw')['state'] = self.gw_update_status
         else:
             self.builder.get_object('connect_gw').configure(text='Connect')
             self.builder.get_object('gwCom')['state'] = 'normal'
             self.builder.get_object('version').configure(text=GW_VERSION)
             self.builder.get_object('latestVersion').configure(text=GW_AVAILABLE_VERSION)
             self.builder.get_object('update_gw')['state'] = 'disabled'
-
+    
     def check_atten_open(self):
         connected = False
         for com, atten in self.atten_serials.items():
             if atten['serial'] is not None and atten['serial'].GetActiveTE().is_open():
                 connected = True
         if connected:
             self.builder.get_object(f'connect_atten').configure(text='Disconnect')
             self.builder.get_object(f'attenComLoRa')['state'] = 'disabled'
             self.builder.get_object(f'attenComBle')['state'] = 'disabled'
         else:
             self.builder.get_object(f'connect_atten').configure(text='Connect')
             self.builder.get_object(f'attenComLoRa')['state'] = 'normal'
             self.builder.get_object(f'attenComBle')['state'] = 'normal'
 
-    def choose_com_ports(self):
-        default_dict = self.default_dict
+    def choose_com_ports(self, default_dict):
         com_ports = [s.device for s in tools.list_ports.comports()]
         if len(com_ports) == 0:
             com_ports = [s.name for s in tools.list_ports.comports()]
-
+        
         if 'gw' in default_dict.keys() and default_dict['gw'] in com_ports:
             self.gw_com_port = [default_dict['gw']]
             self.used_ports.append(default_dict['gw'])
         else:
             self.gw_com_port = ['']
             self.missing_com_port = True
         if 'atten' in default_dict.keys() and BLE in default_dict['atten'].keys() and default_dict['atten'][BLE] \
@@ -349,123 +345,123 @@
             self.atten_serials[default_dict['atten'][LORA]] = {}
             self.atten_serials[default_dict['atten'][LORA]]['type'] = LORA
             self.atten_serials[default_dict['atten'][LORA]]['serial'] = None
             self.used_ports.append(default_dict['atten'][LORA])
         elif 'atten' in default_dict.keys() and LORA in default_dict['atten'].keys() \
                 and default_dict['atten'][LORA].strip() != '':
             self.missing_com_port = True
-
+        
         if 'barcodes' in default_dict.keys():
             self.barcodes_serials = dict.fromkeys([barcode for barcode in default_dict['barcodes'] if barcode
                                                    in com_ports], None)
             self.used_ports += list(self.barcodes_serials.keys())
-
+        
         if 'chambers' in default_dict.keys():
             self.chambers_serials = dict.fromkeys([chamber for chamber in default_dict['chambers'] if chamber
                                                    in com_ports], None)
             self.used_ports += list(self.chambers_serials.keys())
 
         if 'temperature_sensors' in default_dict.keys():
             self.sensors_serials = dict.fromkeys([sensor for sensor in default_dict['temperature_sensors']], None)
-
+        
         missing_barcodes = []
         missing_chambers = []
         if 'barcodes' in default_dict.keys():
             missing_barcodes = [barcode for barcode in default_dict['barcodes'] if barcode not in com_ports]
         if 'chambers' in default_dict.keys():
             missing_chambers = [chamber for chamber in default_dict['chambers'] if chamber not in com_ports]
         if any(missing_barcodes + missing_chambers):
             self.missing_com_port = True
-
+        
         return self.missing_com_port
-
+    
     def choose_gw(self, *args):
         if len(self.gw_com_port) > 0 and self.gw_com_port[0] != '':
             self.used_ports.pop(self.used_ports.index(self.gw_com_port[0]))
         self.gw_com_port = [self.builder.get_object('gwCom').get()]
         self.used_ports.append(self.gw_com_port[0])
-
+    
     def choose_ble_atten(self, *args):
         ble_com = self.builder.get_object('attenComBle').get()
         ble_last_com = [com for com, item in self.atten_serials.items() if item['type'] == BLE]
         if len(ble_last_com) > 0:
             self.atten_serials.pop(ble_last_com[0])
             self.used_ports.pop(self.used_ports.index(ble_last_com[0]))
         if ble_com.strip() != '':
             self.atten_serials[ble_com] = {}
             self.atten_serials[ble_com]['type'] = BLE
             self.atten_serials[ble_com]['serial'] = None
             self.used_ports.append(ble_com)
-
+    
     def choose_lora_atten(self, *args):
         lora_com = self.builder.get_object('attenComLoRa').get()
         lora_last_com = [com for com, item in self.atten_serials.items() if item['type'] == LORA]
         if len(lora_last_com) > 0:
             self.atten_serials.pop(lora_last_com[0])
             self.used_ports.pop(self.used_ports.index(lora_last_com[0]))
         if lora_com.strip() != '':
             self.atten_serials[lora_com] = {}
             self.atten_serials[lora_com]['type'] = LORA
             self.atten_serials[lora_com]['serial'] = None
             self.used_ports.append(lora_com)
-
+    
     def connect_all(self, gui=True):
         if not self.is_gw_serial_open():
             success = self.connect_gw(gui)
             if not success:
                 return
         if not self.serials_connected(ATTENUATORS):
             self.connect_atten(gui)
         if not self.serials_connected(BARCODES):
             self.connect_barcodes(gui)
         if not self.serials_connected(CHAMBERS):
             self.connect_chambers(gui)
         self.connect_temperature_sensor()
         self.hwConnected = True
-
+    
     def connect_gw(self, gui=True, disconnect=False):
         if not self.is_gw_serial_open() and not disconnect:
             if len(self.gw_com_port) == 0 or self.gw_com_port[0].strip() == '':
-                self.popup_message('No default com port for GW, please choose GW com port.', title='Error', log='error')
+                popup_message('No default com port for GW, please choose GW com port.', title='Error', log='error')
                 return False
             com_port = self.gw_com_port[0]
             self.gateway.open_port(port=com_port, baud=921600)
             if self.is_gw_serial_open():
                 self.start_listener(not_print_str=True)
-                self.logger.info(f'GW is connected on port: {com_port}.')
+                logger.info(f'GW is connected on port: {com_port}.')
                 self.gateway.reset_gw()
                 sleep(1)
                 version = self.gateway.get_gw_version()
                 self.gwVersion = version
                 self.gw_latest_version = latest_version = self.gateway.get_latest_version_number()
                 cur_version = int(version[0].replace('.', ''))
                 self.gw_update_status = 'normal' if cur_version < int(latest_version[0].replace('.', '')) \
                     else 'disabled'
                 if cur_version >= int(GW_TBP_VERSION.replace('.', '')):
                     self.cur_gw_tbp_version = True
             else:
-                self.logger.error(f'Error connecting to GW on port: {com_port}.')
+                logger.error(f'Error connecting to GW on port: {com_port}.')
                 return False
         else:
             self.gateway.close_port()
             self.builder.get_object('connect_gw').configure(text='Connect')
             self.builder.get_object('version').configure(text=GW_VERSION)
             self.builder.get_object('latestVersion').configure(text=GW_AVAILABLE_VERSION)
             self.builder.get_object('gwCom')['state'] = 'normal'
         if gui:
             self.check_gw_open()
-
+        
         return True
-
+    
     def connect_barcodes(self, gui=True):
         self.connect_multi_serials(BARCODES, gui=gui)
-
+    
     def connect_chambers(self, gui=True):
         self.connect_multi_serials(CHAMBERS, gui=gui)
-
+    
     def connect_atten(self, gui=True):
         is_connected = self.connect_multi_serials(ATTENUATORS, gui=gui)
         if gui:
             atten_state = 'disabled' if is_connected else 'normal'
             self.builder.get_object('attenComLoRa')['state'] = atten_state
             self.builder.get_object('attenComBle')['state'] = atten_state
 
@@ -474,22 +470,22 @@
         self.temperature_sensor_readings = []
         for sensor_name in self.sensors_serials.keys():
             self.temperature_sensor_readings.append([])
             try:
                 sensor_temp = YoctoTemperatureSensor()
                 is_connected = sensor_temp.connect(target=sensor_name)
                 if is_connected:
-                    self.logger.info('Temperature Sensor {} is connected'.format(sensor_temp.get_sensor_name()))
+                    logger.info('Temperature Sensor {} is connected'.format(sensor_temp.get_sensor_name()))
                     self.all_sensors.append(sensor_temp)
                 else:
-                    self.logger.info('Could not connect to Temperature Sensor according to '
-                                     'the following name: {}'.format(sensor_name))
+                    logger.info('Could not connect to Temperature Sensor according to '
+                                'the following name: {}'.format(sensor_name))
                     self.all_sensors.append(None)
             except Exception as e:
-                self.logger.info('while connecting to the Temperature Sensor the following error occurs : {}'.format(e))
+                logger.info('while connecting to the Temperature Sensor the following error occurs : {}'.format(e))
                 self.all_sensors.append(None)
 
     def read_temperature_sensor(self):
         for i, sensor in enumerate(self.all_sensors):
             if sensor is not None:
                 self.temperature_sensor_readings[i].append(sensor.get_temperature())
 
@@ -517,22 +513,22 @@
                     self.builder.get_object(f'add{obj}')['state'] = 'disabled'
                 except:
                     pass
         if gui:
             self.find_com_ports()
         # self.update_go_state()
         return is_connected
-
+    
     def open_serials(self, obj, serials):
         threads = []
         for com_port, com_serial in serials.items():
             if 'barcode' in obj.lower():
                 if com_serial is not None and com_serial.is_open():
                     continue
-                com_serial = BarcodeScanner(com_port=com_port, log_type='LOG_NL')
+                com_serial = BarcodeScanner(com=com_port, log_type='LOG_NL')
                 if com_serial.is_open():
                     # self.used_ports.append(com_port)
                     serials[com_port] = com_serial
             elif 'chamber' in obj.lower():
                 if com_serial is not None and com_serial.is_connected():
                     continue
                 temp_thread = Thread(target=self.connect_chamber, args=([com_port, serials]))
@@ -543,166 +539,163 @@
                     # 8 if serial['serial']!=None and
                     # serial['serial'].GetActiveTE().s.is_open():
                     continue
                 com_serial = Attenuator('API', comport=com_port)
                 if com_serial.GetActiveTE().is_open():
                     # self.used_ports.append(com_port)
                     serials[com_port]['serial'] = com_serial
-
+        
         for thread in threads:
             thread.join()
-
+    
     def close(self):
         if self.is_gw_serial_open() and self.serials_connected(ATTENUATORS) and self.serials_connected(BARCODES):
             self.hwConnected = True
             self.enable_hw_connected()
         if self.isGui:
             self.isGui = False
             self.ttk.destroy()
         return self.hwConnected
-
+    
     def save(self):
         # default_dict = {}
         # if isfile(join(CONFIGS_DIR, '.defaults.json')):
         #     with open(join(CONFIGS_DIR, '.defaults.json'), 'r') as defaultComs:
         #         default_dict = load(defaultComs)
         self.default_dict['gw'] = self.gw_com_port[0]
         self.default_dict['atten'] = {}
         for com_port, atten in self.atten_serials.items():
             self.default_dict['atten'][atten['type']] = com_port
         self.default_dict['barcodes'] = list(self.barcodes_serials.keys())
         self.default_dict['chambers'] = list(self.chambers_serials.keys())
         with open(join(CONFIGS_DIR, '.defaults.json'), 'w+') as defaultComs:
             dump(dict(self.default_dict), defaultComs, indent=4)
-
-        self.logger.info(f'Com ports saved successfully.')
-
+        
+        logger.info(f'Com ports saved successfully.')
+    
     def focus_barcode_available(self, *args):
         self.focus_available(BARCODES)
-
+    
     def focus_barcode_chosen(self, *args):
         self.focus_chosen(BARCODES)
-
+    
     def focus_chamber_available(self, *args):
         self.focus_available(CHAMBERS)
-
+    
     def focus_chamber_chosen(self, *args):
         self.focus_chosen(CHAMBERS)
-
+    
     def focus_available(self, obj):
         self.builder.get_object(f'add{obj}').configure(text='>')
         setattr(self, f'{obj.lower()}_state', ADD)
-
+    
     def focus_chosen(self, obj):
         self.builder.get_object(f'add{obj}').configure(text='<')
         setattr(self, f'{obj.lower()}_state', REMOVE)
         setattr(self, f'{obj.lower()}_move_com', '')
-
+    
     def add_barcode(self):
         if getattr(self, f'{BARCODES.lower()}_state') == ADD:
             com_chosen = self.builder.get_object(f'available{BARCODES}').get(ACTIVE)
-            try:
-                temp_barcode = BarcodeScanner(com_port=com_chosen)
-            except Exception as e:
-                self.popup_message(f'Could NOT connect. {e}', title='Error', log='error')
+            temp_barcode = BarcodeScanner()
+            if not temp_barcode.check_com_port(com_chosen):
+                popup_message(f'{com_chosen} is not barcode scanner', title='Error', log='error')
         self.add(BARCODES)
         self.find_com_ports()
-
+    
     def add_chamber(self):
         self.add(CHAMBERS)
         self.find_com_ports()
-
+    
     def add(self, obj):
         if getattr(self, f'{obj.lower()}_state') == ADD:
             sending = self.builder.get_object(f'available{obj}')
             receiving = self.builder.get_object(f'chosen{obj}')
         else:
             sending = self.builder.get_object(f'chosen{obj}')
             receiving = self.builder.get_object(f'available{obj}')
-
+        
         com_list = list(sending.get(0, END))
         com_chosen = sending.get(ACTIVE)
         receiving.insert(END, com_chosen)
         com_index = com_list.index(com_chosen)
         sending.delete(com_index, com_index)
-
+        
         serials = getattr(self, f'{obj.lower()}_serials')
         com_ports = self.builder.get_object(f'chosen{obj}').get(0, END)
         old_ports = [port for port in serials.keys() if port not in com_ports]
         new_serials = dict(zip(com_ports, [None] * len(com_ports)))
         self.used_ports = [port for port in self.used_ports if port not in old_ports] + list(com_ports)
         setattr(self, f'{obj.lower()}_serials', new_serials)
-
+    
     def chamber_up(self):
         self.up(CHAMBERS)
-
+    
     def chamber_down(self):
         self.down(CHAMBERS)
-
+    
     def barcode_up(self):
         self.up(BARCODES)
-
+    
     def barcode_down(self):
         self.down(BARCODES)
-
+    
     def up(self, obj):
         com_list = list(self.builder.get_object(f'chosen{obj}').get(0, END))
         if getattr(self, f'{obj.lower()}_move_com') == '':
             chosen_com = self.builder.get_object(f'chosen{obj}').get(ACTIVE)
             setattr(self, f'{obj.lower()}_move_com', chosen_com)
         else:
             chosen_com = getattr(self, f'{obj.lower()}_move_com')
-        if chosen_com != '':
-            com_index = com_list.index(chosen_com)
-            if com_index > 0:
-                com_list.pop(com_list.index(chosen_com))
-                com_list.insert(com_index - 1, chosen_com)
-                self.builder.get_object(f'chosen{obj}').delete(0, END)
-                for com in com_list:
-                    self.builder.get_object(f'chosen{obj}').insert(END, com)
-                self.builder.get_object(f'chosen{obj}').select_set(com_index - 1)
-
+        com_index = com_list.index(chosen_com)
+        if com_index > 0:
+            com_list.pop(com_list.index(chosen_com))
+            com_list.insert(com_index - 1, chosen_com)
+            self.builder.get_object(f'chosen{obj}').delete(0, END)
+            for com in com_list:
+                self.builder.get_object(f'chosen{obj}').insert(END, com)
+            self.builder.get_object(f'chosen{obj}').select_set(com_index - 1)
+    
     def down(self, obj):
         com_list = list(self.builder.get_object(f'chosen{obj}').get(0, END))
         if getattr(self, f'{obj.lower()}_move_com') == '':
             chosen_com = self.builder.get_object(f'chosen{obj}').get(ACTIVE)
             setattr(self, f'{obj.lower()}_move_com', chosen_com)
         else:
             chosen_com = getattr(self, f'{obj.lower()}_move_com')
-        if chosen_com != '':
-            com_index = com_list.index(chosen_com)
-            if com_index < (len(com_list) - 1):
-                com_list.pop(com_list.index(chosen_com))
-                com_list.insert(com_index + 1, chosen_com)
-                self.builder.get_object(f'chosen{obj}').delete(0, END)
-                for com in com_list:
-                    self.builder.get_object(f'chosen{obj}').insert(END, com)
-                self.builder.get_object(f'chosen{obj}').select_set(com_index + 1)
-
+        com_index = com_list.index(chosen_com)
+        if com_index < (len(com_list) - 1):
+            com_list.pop(com_list.index(chosen_com))
+            com_list.insert(com_index + 1, chosen_com)
+            self.builder.get_object(f'chosen{obj}').delete(0, END)
+            for com in com_list:
+                self.builder.get_object(f'chosen{obj}').insert(END, com)
+            self.builder.get_object(f'chosen{obj}').select_set(com_index + 1)
+    
     def update_multi_serials(self, available_ports, obj):
         self.builder.get_object(f'available{obj}').delete(0, END)
         for port in available_ports:
             if port not in self.used_ports:
                 self.builder.get_object(f'available{obj}').insert(END, port)
-
+    
     def update_atten_serials(self, available_ports):
         for com, item in self.atten_serials.items():
             if item['serial'] is None or not item['serial'].is_open():
                 self.builder.get_object(f'attenCom{item["type"]}')['values'] = available_ports
             else:
                 self.builder.get_object(f'attenCom{item["type"]}').set(com)
-
+    
     def connect_chamber(self, com_port, serials):
         com_serial = Tescom(com_port)
         if com_serial.is_connected():
             # self.used_ports.append(com_port)
             serials[com_port] = com_serial
             if not com_serial.is_door_open():
                 com_serial.open_chamber()
-
+    
     def close_serials(self, obj, serials):
         if 'atten' in obj.lower():
             for serial in serials.values():
                 # serial['serial'].GetActiveTE.s.close_port()
                 if serial['serial'] is not None and serial['serial'].GetActiveTE().is_open():
                     serial['serial'].GetActiveTE().close_port()
                 serial['serial'] = None
@@ -710,15 +703,15 @@
         else:
             for com_serial in serials.values():
                 if 'chamber' in obj.lower():
                     com_serial.open_chamber()
                 com_serial.close_port()
                 # self.used_ports.remove(com_port)
                 # serials.pop(com_port)
-
+    
     def serials_connected(self, obj):
         serials = getattr(self, f'{obj.lower()}_serials')
         if 'atten' in obj.lower():
             serials = dict(zip(serials.keys(), [atten['serial'] for atten in serials.values()]))
         connected_serials = 0
         for com_port, com_serial in serials.items():
             if com_serial is not None:
@@ -730,246 +723,236 @@
                     connected_serials += 1
             # if com_port.strip()=='':
             #     connected_serials += 1
         if connected_serials > 0 and connected_serials == len(serials.keys()):
             return True
         else:
             return False
-
+    
     def get_data(self, actionType=ActionType.ALL_SAMPLE, dataType=DataType.PACKET_LIST):
         return self.gateway.get_packets(action_type=actionType, data_type=dataType)
-
-    def read_barcode(self, scanner_index=0, close_chamber=False, add_to_test=False, n_try=5):
-        if len(list(self.barcodes_serials.values())) == 0:
-            self.logger.error('Trying to read barcode but no scanner were connected')
-            return None, None
+    
+    def read_barcode(self, scanner_index=0, close_chamber=False, add_to_test=False):
         scanner = list(self.barcodes_serials.values())[scanner_index]
-        for i in range(n_try):
-            full_data, cur_id, reel_id, gtin = scanner.scan_ext_id()
-            if full_data is None and cur_id is None and reel_id is None and full_data is None:
-                continue
-            break
-
+        full_data, cur_id, reel_id, gtin = scanner.scan_ext_id(scanDur=5)
+        
         cur_id = cur_id if cur_id is not None else full_data
         reel_id = reel_id if reel_id is not None else full_data
         gtin = gtin if gtin is not None else ''
         if reel_id is not None:
             self.reel_id = reel_id
             self.gtin = gtin
         if cur_id is None:
             barcodeMutex.acquire()
             if close_chamber:
                 self.barcode_error.append(scanner_index)
             barcodeMutex.release()
             return None, None
-
+        
         if not close_chamber:
             reel_id_obj = self.top_builder.tkvariables.get('reelId')
             reel_id_obj.set(self.reel_id)
-
+        
         else:
             success = self.add_tag_to_test(cur_id, reel_id, scanner_index=scanner_index, add_to_test=add_to_test)
             if success:
                 self.chambers_to_close.append(scanner_index)
-
+        
         return cur_id, reel_id
-
+    
     def read_scanners_barcodes(self, indexes=()):
         if len(indexes) == 0:
             indexes = list(range(len(self.barcodes_serials.values())))
         scanner_threads = []
         self.barcode_error = []
         self.chambers_to_close = []
-
+        
         for i in indexes:
             t = threading.Thread(target=self.read_barcode, args=(i, True, True))
             scanner_threads.append(t)
             t.start()
         for i in range(len(scanner_threads)):
             t = scanner_threads[i]
             t.join()
-
+        
         read_message = ''
         title = 'Warning'
         font = 18
         if len(self.barcode_error) > 0:
             read_message += f'Error reading external ID from chambers {self.barcode_error}, try repositioning the tags.\n'
             title = 'Error'
             font = 16
-
+        
         if len(self.chambers_to_close) > 0:
             read_message += f'Chambers are closing!!\nWatch your hands!!!'
-
-        popupThread = threading.Thread(target=self.popup_message,
+        
+        popupThread = threading.Thread(target=popup_message,
                                        args=(read_message, title, ("Helvetica", font), title.lower()))
         popupThread.start()
         popupThread.join()
-
+        
         if len(self.chambers_to_close) > 0:
             self.close_chambers(self.chambers_to_close)
-
+        
         self.update_go_state()
-
+    
     def enable_hw_connected(self):
         self.top_builder.get_object('read_qr')['state'] = 'normal'
         self.top_builder.get_object('reelId')['state'] = 'normal'
         if self.top_builder.tkvariables.get('go').get() == CONNECT_HW:
             self.top_builder.tkvariables.get('go').set(READ)
             self.top_builder.get_object('go')['state'] = 'disabled'
-
+    
     def send_gw_app(self, params):
         str_rsp = []
         self.gateway.reset_buffer()
         self.gateway.clear_rsp_str_input_q()
-
+        
         self.gateway.reset_start_time()
-
+        
         for param, value in params.items():
             if param.startswith(ATTENUATION):
                 for com_port, atten in self.atten_serials.items():
                     if param.lower().endswith(atten['type'].lower()):
                         try:
                             attenuation = atten['serial'].GetActiveTE().Setattn(float(value))
-                            self.logger.info(f"{atten['type']} Attenuation set to: {str(attenuation).strip()}")
-                        except Exception as e:
-                            self.logger.error(f"{atten['type']} Attenuator error: try reconnect the attenuator [{e}].")
+                            logger.info(f"{atten['type']} Attenuation set to: {str(attenuation).strip()}")
+                        except:
+                            logger.error(f"{atten['type']} Attenuator error: try reconnect the attenuator.")
                             return False
-
+        
         self.start_time = time()
         try:
-            str_rsp.append(self.gateway.write('!sub1g_sync 1', with_ack=True))
             str_rsp.append(self.gateway.write('!listen_to_tag_only 1', with_ack=True))
             str_rsp.append(self.gateway.write('!set_tester_mode 1', with_ack=True))
             if 'EmulateSurfaceValue' in params.keys():
                 str_rsp.append(self.gateway.write('!set_sub_1_ghz_energizing_frequency {}'.format(
                     params['EmulateSurfaceValue']), with_ack=True))
             _, gw_ans = self.gateway.config_gw(effective_output_power_val=22, sub1g_output_power_val=29,
                                                energy_pattern_val=params['pattern'], received_channel=params['channel'],
                                                time_profile_val=[params['tOn'], params['tTotal']], start_gw_app=True,
                                                filter_val=False, pacer_val=0,
                                                with_ack=True)
             for rsp in gw_ans:
                 str_rsp.append(rsp)
-
-        except Exception as e:
-            self.logger.error(f'Gateway error: try reconnect the gateway [{e}].')
+        
+        except:
+            logger.error(f'Gateway error: try reconnect the gateway.')
             self.cancel_gw_commands()
             return False
-
+        
         for command in str_rsp:
             if "Command Complete Event" not in command['raw'] and "Energizing" not in command['raw']:
-                self.logger.error(f'Gateway response: {command["raw"]}')
+                logger.error(f'Gateway response: {command["raw"]}')
                 self.cancel_gw_commands()
                 return False
-
+        
         return True
-
+    
     def connect_and_close(self):
         self.connect_all()
         self.close()
-
+    
     def get_reel_id(self):
         return self.reel_id
-
+    
     def get_gtin(self):
         return self.gtin
-
+    
     def get_reel_external(self):
         return self.gtin + self.reel_id
-
+    
     def is_gw_serial_open(self):
         serial_open, _, _ = self.gateway.get_connection_status()
         return serial_open
-
+    
     def is_gw_data_available(self):
         return self.gateway.is_data_available()
-
+    
     def is_gui_opened(self):
         return self.isGui
-
+    
     def get_gw_version(self):
         return self.gwVersion[0]
-
+    
     def update_gw(self):
         self.gateway.update_version()
-
+    
     def get_gw_time(self):
         return self.start_time
-
+    
     def cancel_gw_commands(self):
         # self.gateway.write(GW_CANCEL)
         self.gateway.reset_gw()
         # self.gateway.stop_continuous_listener()
         # self.gateway.reset_buffer()
         sleep(0.1)
-
+    
     def start_listener(self, not_print_str=True):
         # self.gateway.start_continuous_listener(not_print_str)
         self.gateway.start_continuous_listener()
-
+    
     def is_hw_connected(self):
         return self.hwConnected
-
+    
     def get_chambers(self):
         return list(self.chambers_serials.values())
-
+    
     def open_chambers(self, indexes=()):
         chambers_threads = []
         chambers = list(self.chambers_serials.values())
         if len(indexes) == 0:
             indexes = list(range(len(chambers)))
         for index in indexes:
             if len(chambers) > index and chambers[index] is not None:
                 temp_thread = Thread(target=chambers[index].open_chamber, args=())
                 temp_thread.start()
                 chambers_threads.append(temp_thread)
-
+        
         for thread in chambers_threads:
             thread.join()
-
+    
     def close_chambers(self, indexes=()):
         chambers = list(self.chambers_serials.values())
         chambers_threads = []
         if len(indexes) == 0:
             indexes = list(range(len(chambers)))
         for index in indexes:
             if len(chambers) > index and chambers[index] is not None:
                 t = threading.Thread(target=chambers[index].close_chamber, args=())
                 chambers_threads.append(t)
                 t.start()
         for thread in chambers_threads:
             thread.join()
-
+    
     def get_num_of_barcode_scanners(self):
         return len(self.barcodes_serials.keys())
-
+    
     def get_error_barcode(self):
         return self.barcode_error
-
+    
     def gw_tbp_version(self):
         return self.cur_gw_tbp_version
-
+    
     def gw_get_packets(self):
         self.gateway.get_packets(action_type=ActionType.ALL_SAMPLE, data_type=DataType.PROCESSED)
-
+    
     def get_default_dict(self):
         return self.default_dict
 
-    def popup_message(self, msg, title='Error', font=("Helvetica", 10), log='info', bg=None, tk_frame=None):
-        if tk_frame:
-            popup = Toplevel(tk_frame)
-        else:
-            popup = Tk()
-        popup.eval('tk::PlaceWindow . center')
-        popup.wm_title(title)
-        if bg is not None:
-            popup.configure(bg=bg)
-        getattr(self.logger, log)(f'{title} - {msg}')
-
-        def popup_exit():
-            popup.destroy()
-
-        label = Label(popup, text=msg, font=font)
-        label.pack(side="top", fill="x", padx=10, pady=10)
-        b1 = Button(popup, text="Okay", command=popup_exit)
-        b1.pack(padx=10, pady=10)
-        popup.mainloop()
+
+def popup_message(msg, title='Error', font=("Helvetica", 10), log='info', bg=None):
+    popup = Tk()
+    popup.eval('tk::PlaceWindow . center')
+    popup.wm_title(title)
+    if bg is not None:
+        popup.configure(bg=bg)
+    getattr(logger, log)(f'{title} - {msg}')
+    
+    def popup_exit():
+        popup.destroy()
+    
+    label = Label(popup, text=msg, font=font)
+    label.pack(side="top", fill="x", padx=10, pady=10)
+    b1 = Button(popup, text="Okay", command=popup_exit)
+    b1.pack(padx=10, pady=10)
+    popup.mainloop()
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/configs/.default_test_configs.json` & `wiliot-testers-4.0.6/wiliot_testers/sample/configs/.default_test_configs.json`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/configs_gui.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/configs_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,23 +67,24 @@
 from wiliot_core import WiliotDir
 from wiliot_testers.utils.get_version import get_version
 
 VER = get_version()
 MEASURED = {'button': 'Measured', 'label': '[meter]'}
 MANUAL = {'button': 'Manual', 'label': '[db]'}
 DEFAULT_EMULATED_SURFACE = 'no simulation'
+logger = logging.getLogger('sample')
 
 wiliot_env = WiliotDir()
-sample_test_dir = abspath(join(wiliot_env.get_common_dir(), 'sample_test'))
-OUTPUT_DIR = abspath(join(sample_test_dir, 'logs'))
-CONFIGS_DIR = abspath(join(sample_test_dir, 'configs'))
-if not isdir(abspath(join(OUTPUT_DIR))):
-    makedirs(abspath(join(OUTPUT_DIR)))
-if not isdir(abspath(join(CONFIGS_DIR))):
-    makedirs(abspath(join(CONFIGS_DIR)))
+sample_test_dir = join(wiliot_env.get_common_dir(), 'sample_test')
+OUTPUT_DIR = join(sample_test_dir, 'logs')
+CONFIGS_DIR = join(sample_test_dir, 'configs')
+if not isdir(join(OUTPUT_DIR)):
+    makedirs(join(OUTPUT_DIR))
+if not isdir(join(CONFIGS_DIR)):
+    makedirs(join(CONFIGS_DIR))
 
 
 class ConfigsGui(object):
     '''
     classdocs
     '''
     isGui = False
@@ -97,38 +98,38 @@
     all_configs_fields = []
     
     def __init__(self, top_builder=None):
         '''
         Constructor
         '''
         self.top_builder = top_builder
-        self.config_path = abspath(join(dirname(__file__), 'configs', '.default_test_configs.json'))
+        self.config_path = join(dirname(__file__), 'configs', '.default_test_configs.json')
         if isfile(self.config_path):
             with open(self.config_path, 'r') as jsonFile:
                 self.configsDict = load(jsonFile)
                 if len(self.configsDict):
                     self.all_configs_fields = list(self.configsDict[next(iter(self.configsDict))].keys())
             self.fix_antenna_type()
 
-        with open(abspath(join(dirname(__file__), 'configs', '.default_surfaces.json')), 'r') as jsonFile:
+        with open(join(dirname(__file__), 'configs', '.default_surfaces.json'), 'r') as jsonFile:
             self.defaultSurfacesDict = load(jsonFile)
 
         self.copy_config_file()
 
     def copy_config_file(self):
-        copyfile(self.config_path, abspath(join(CONFIGS_DIR, f'.default_test_configs(ViewOnly)_{VER}.json')))
+        copyfile(self.config_path, join(CONFIGS_DIR, f'.default_test_configs(ViewOnly)_{VER}.json'))
 
     def gui(self, ttk_frame=None):
         self.builder = builder = pygubu.Builder()
-        ui_file = abspath(join(abspath(dirname(__file__)), 'utils', 'configs.ui'))
+        ui_file = join(abspath(dirname(__file__)), 'utils', 'configs.ui')
         self.builder.add_from_file(ui_file)
         
-        img_path = abspath(join(abspath(dirname(__file__)), ''))
+        img_path = join(abspath(dirname(__file__)), '')
         builder.add_resource_path(img_path)
-        img_path = abspath(join(abspath(dirname(__file__)), 'utils'))
+        img_path = join(abspath(dirname(__file__)), 'utils')
         builder.add_resource_path(img_path)
         
         self.ttk = ttk_frame
         
         self.ttk.title("Sample Test Configs")
         
         self.mainwindow = self.builder.get_object('mainwindow', self.ttk)
@@ -176,14 +177,21 @@
         ble_label = self.builder.tkvariables.get('attenBleLabel')
         ble_label.set(ble_label.get().split()[0] + ' ' + self.atten_cur_mode['label'])
         lora_label = self.builder.tkvariables.get('attenLoRaLabel')
         lora_label.set(lora_label.get().split()[0] + ' ' + self.atten_cur_mode['label'])
     
     def close(self):
         self.isGui = False
+        for param in self.all_configs_fields:
+            if self.builder.tkvariables.get(param) is not None:
+                value = self.builder.tkvariables.get(param).get()
+                self.paramDict[param] = value
+                self.configsDict[self.config][param] = value
+                if param == 'EmulateSurface':
+                    self.paramDict['EmulateSurfaceValue'] = self.defaultSurfacesDict['EmulateSurface'][value]
         self.ttk.destroy()
     
     def is_gui_opened(self):
         return self.isGui
     
     def get_params(self):
         return self.paramDict
@@ -238,17 +246,16 @@
         self.top_builder.get_object('test_config')['values'] = [key for key, item in self.configsDict.items()
                                                                 if isinstance(item, dict)]
         self.top_builder.get_object('test_config').set(config)
         
         with open(self.config_path, 'w+') as jsonFile:
             dump(self.configsDict, jsonFile, indent=4)
         self.copy_config_file()
-
-        self.set_params(config)
-        print(f'{config} configuration saved successfully.')
+        
+        logger.info(f'{config} configuration saved successfully.')
     
     def reset(self):
         def_dict = deepcopy(self.defaultConfigsDict)
         self.configsDict.update(def_dict)
         self.set_gui_defaults()
     
     def test_time_update(self, *args):
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/get_temperature_sensor_name.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/get_temperature_sensor_name.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/sample_test.py` & `wiliot-testers-4.0.6/wiliot_testers/sample/sample_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,28 +67,37 @@
 import pygubu
 from threading import Thread, Lock
 from time import sleep
 import time
 import csv
 import datetime
 from wiliot_testers.sample.configs_gui import ConfigsGui, OUTPUT_DIR, CONFIGS_DIR
-from wiliot_testers.sample.com_connect import ComConnect, GO, CONTINUE, CONNECT_HW, READ, SEND
+from wiliot_testers.sample.com_connect import ComConnect, GO, CONTINUE, CONNECT_HW, READ, SEND, \
+    popup_message
 from traceback import print_exc
 from json import load, dump
 import argparse
 import sys
 from os.path import isfile, abspath, dirname, join, isdir, exists
 from wiliot_testers.utils.get_version import get_version
+# sys.path.append(abspath(dirname(join('..', '..', '..', '..', 'pywiliot_internal'))))
 from wiliot_testers.tester_utils \
     import setLogger, changeFileHandler, removeFileHandler, CsvLog, HeaderType, TesterName, StreamToLogger
 from wiliot_core import TagCollection, PacketList
-from wiliot_core import check_user_config_is_ok, InlayTypes, WiliotDir
+from wiliot_core import check_user_config_is_ok, InlayTypes
 from wiliot_api import ManufacturingClient
-from wiliot_testers.utils.upload_to_cloud_api import *
-from enum import Enum
+from wiliot_testers.tester_utils import upload_to_cloud_api
+
+LOG_LEVEL = 'INFO'
+
+# default_log_file = join(abspath(dirname(__file__)), 'SampleTest.log')
+default_log_file = join(OUTPUT_DIR, 'SampleTest.log')
+logger = setLogger('sample', LOG_LEVEL, outputFile=default_log_file, file_mode='a+')
+sys.stdout = StreamToLogger(logger, logging.INFO)
+sys.stderr = StreamToLogger(logger, logging.ERROR)
 
 addToDictMutex = Lock()
 calibMutex = Lock()
 recvDataMutex = Lock()
 timerMutex = Lock()
 mutex = Lock()
 
@@ -101,28 +110,18 @@
 DEF_NUM_OF_TAGS = 2
 
 CLOUD_TIMEOUT_POST = 10
 CLOUD_TIMEOUT_RESOLVE = 2
 
 SGTIN_PREFIX_DEFAULT = '(01)00850027865010(21)'
 
-
 class SampleException(Exception):
     pass
 
 
-class FailureCodeSampleTest(Enum):
-    NONE = 0
-    PASS = 1  # Pass
-    NO_RESPONSE = 3
-    NO_TBP = 5
-    HIGH_TBP_AVG = 7
-    NOT_COMPLETED = 9
-
-
 class SampleTest(object):
     goButtonState = CONNECT_HW
     stopButtonState = STOP
     client = None
     comConnect = None
     configsGui = None
     comTtk = None
@@ -137,15 +136,14 @@
     post_data = True
     wiliotTags = False
     forceCloseRequested = False
     closeRequested = False
     testGo = False
     stopTimer = False
     closeListener = False
-    is_test_pass = False
     testConfig = ''
     reel_id = ''
     gtin = ''
     testDir = ''
     owner = ''
     station_name = ''
     pywiliot_version = ''
@@ -169,108 +167,87 @@
     add_to_dict_threads = []
     unknown_packets = PacketList()
     antenna = ''
     low = 0
     high = 0
     step = 1
     n_repetitions = 1
-    logger = logging.getLogger('sample')
-
+    
     # numOfTags = ''
     multiTag = TagCollection()
     
     def __init__(self, calib=None, environment='', post_data=True, offline=False):
-
-        self.set_logger()
+        
         self.calib = calib
         self.offline = offline
         self.offline_tag_index = 0
         self.environment = environment
         self.post_data = post_data
         if self.offline:
             self.post_data = False
 
         self.pywiliot_version = get_version()
-        self.logger.info(f'PyWiliot version: {self.pywiliot_version}')
+        logger.info(f'PyWiliot version: {self.pywiliot_version}')
         
-        if isfile(abspath(join(CONFIGS_DIR, '.defaults.json'))):
-            with open(abspath(join(CONFIGS_DIR, '.defaults.json')), 'r') as defaultComs:
+        if isfile(join(CONFIGS_DIR, '.defaults.json')):
+            with open(join(CONFIGS_DIR, '.defaults.json'), 'r') as defaultComs:
                 self.defaultDict = load(defaultComs)
 
         self.popup_login()
         
         self.builder = builder = pygubu.Builder()
         
         self.comConnect = ComConnect(top_builder=builder, new_tag_func=self.add_tag_to_test,
-                                     update_go=self.update_go_state, default_dict=self.defaultDict, logger=self.logger)
+                                     update_go=self.update_go_state, default_dict=self.defaultDict)
         self.update_data()
         if not self.offline:
             _, api_key, is_success = check_user_config_is_ok(env='prod', owner_id=self.owner)
             if not is_success:
-                self.logger.warning('invalid User credential')
+                logger.warning('invalid User credential')
                 return
             self.client = ManufacturingClient(api_key=api_key, logger_='root')
         self.configsGui = ConfigsGui(top_builder=builder)
-        self.logger.info(f'Sample test is up and running')
-
-    def set_logger(self):
-        formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s: %(message)s', '%Y-%m-%d %H:%M:%S')
-        stream_handler = logging.StreamHandler()
-        stream_handler.setLevel(logging.DEBUG)
-        stream_handler.setFormatter(formatter)
-        wiliot_dir = WiliotDir()
-        logger_path = abspath(join(wiliot_dir.get_wiliot_root_app_dir(), 'sample_test'))
-        if not isdir(logger_path):
-            os.mkdir(logger_path)
-        logger_path = abspath(join(logger_path, 'logs'))
-        if not isdir(logger_path):
-            os.mkdir(logger_path)
-        logger_name = 'sample_test_{}.log'.format(datetime.datetime.now().strftime('%Y%m%d_%H%M%S'))
-        self.logger_path = abspath(join(logger_path, logger_name))
-        file_handler = logging.FileHandler(self.logger_path, mode='a')
-        file_formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S')
-        file_handler.setFormatter(file_formatter)
-        self.logger.addHandler(file_handler)
-        self.logger.addHandler(stream_handler)
-        self.logger.setLevel(logging.INFO)
-
+    
     def gui(self):
-        self.logger.info(f'Sample test setting the GUI')
         self.set_gui()
-        self.logger.info(f'Sample test GUI is running')
+        
         self.ttk.mainloop()
     
     def set_gui(self):
-        uifile = abspath(join(abspath(dirname(__file__)), 'utils', 'sample_test.ui'))
+        uifile = join(abspath(dirname(__file__)), 'utils', 'sample_test.ui')
         self.builder.add_from_file(uifile)
-
-        img_path = abspath(join(abspath(dirname(__file__)), ''))
+        
+        img_path = join(abspath(dirname(__file__)), '')
         self.builder.add_resource_path(img_path)
-        img_path = abspath(join(abspath(dirname(__file__)), 'utils'))
+        img_path = join(abspath(dirname(__file__)), 'utils')
         self.builder.add_resource_path(img_path)
-
+        
+        missing_com_port = self.comConnect.choose_com_ports(self.defaultDict)
+        
+        if missing_com_port:
+            popup_message('All or some of the default com ports are not available, '
+                          'please check connections.', title='Warning', log='warning')
+        
         self.ttk = Tk()
 
         self.ttk.title("Wiliot Sample Test")
         self.mainWindow = self.builder.get_object('mainwindow', self.ttk)
         self.ttk.protocol("WM_DELETE_WINDOW", self.close)
         self.builder.connect_callbacks(self)
-
+        
         self.builder.get_object('reelId').bind("<Key>", self.get_reel_id)
         list_box = self.builder.get_object('scanned')
         scrollbar = self.builder.get_object('scrollbar1')
         list_box.configure(yscrollcommand=scrollbar.set)
         scrollbar.configure(command=list_box.yview)
         self.builder.get_object('scrollbar1').set(self.builder.get_object('scanned').index(ACTIVE),
                                                   self.builder.get_object('scanned').index(END))
-        self.logger.info(f'checking available serial connection')
-        self.comConnect.choose_com_ports()
-        self.logger.info(f'setting up gui defaults')
+        
         self.set_gui_defaults()
-
+    
     def choose_param(self, *args):
         var = args[0].widget['style'].split('.')[0]
         if self.builder.tkvariables.get(var) is not None:
             value = self.builder.get_object(var).get()
             if var not in self.defaultDict.keys():
                 self.defaultDict[var] = []
             if value in self.defaultDict[var]:
@@ -310,60 +287,60 @@
             self.advas_dict = {}
             self.builder.tkvariables.get('stop').set(STOP)
             self.stopButtonState = STOP
             # self.numOfTags = int(self.builder.tkvariables.get('numTags').get())
             self.testId = testId = time.time()
             self.testName = testName = self.builder.get_object('testName').get()
             # self.operator = operator = self.builder.get_object('operator').get()
-            if not isdir(abspath(join(OUTPUT_DIR, testName))):
-                makedirs(abspath(join(OUTPUT_DIR, testName)))
+            if not isdir(join(OUTPUT_DIR, testName)):
+                makedirs(join(OUTPUT_DIR, testName))
             self.testDir = testDir = datetime.datetime.fromtimestamp(testId).strftime('%d%m%y_%H%M%S')
-            mkdir(abspath(join(OUTPUT_DIR, testName, testDir)))
+            mkdir(join(OUTPUT_DIR, testName, testDir))
             self.common_run_name = common_run_name = self.reel_id + '_' + testDir
-            self.test_log_file = abspath(join(OUTPUT_DIR, testName, testDir, f'{common_run_name}.log'))
-            changeFileHandler(self.logger, self.test_log_file, append_handler=True)
-            self.logger.info(f'Starts new test: {common_run_name}')
-            removeFileHandler(self.logger, self.logger_path)
+            self.test_log_file = join(OUTPUT_DIR, testName, testDir, f'{common_run_name}.log')
+            changeFileHandler(logger, self.test_log_file, append_handler=True)
+            logger.info(f'Starts new test: {common_run_name}')
+            removeFileHandler(logger, default_log_file)
             self.update_params()
             self.testStartTime = time.time()
             self.comConnect.read_temperature_sensor()  # read temperature
             if self.calib:
                 self.calibModeThread = Thread(target=self.calib_thread, args=())
                 self.calibModeThread.start()
                 self.calibModeThread.join()
                 self.calibModeThread = Thread(target=self.calib_mode, args=())
                 self.calibModeThread.start()
             else:
                 self.sendCommandThread = Thread(target=self.send_gw_commands, args=())
                 self.sendCommandThread.start()
-
+        
         elif goButtonState == CONTINUE:
             self.builder.tkvariables.get('stop').set(STOP)
             self.stopButtonState = STOP
             self.total_bad_advas.extend(x for x in self.bad_advas if x not in self.total_bad_advas)
             self.bad_advas = []
             self.advas_dict = {}
             self.sendCommandThread = Thread(target=self.send_gw_commands, args=())
             self.sendCommandThread.start()
-
+    
     def calib_thread(self):
         self.popup_calib()
-
+    
     def read_scanners_barcodes(self, indexes):
         self.comConnect.read_scanners_barcodes(indexes)
         # self.update_params_state(state='normal', group=CONTINUE)
-
+    
     def connect_all(self, gui=True):
         self.comConnect.connect_all(gui=gui)
         self.builder.tkvariables.get('go').set(READ)
         # self.update_params_state(state='normal', group=READ)
         self.builder.get_object('read_qr')['state'] = 'normal'
         self.builder.get_object('reelId')['state'] = 'normal'
         self.builder.get_object('connect')['state'] = 'normal'
-
+    
     def add_tag_to_test(self, cur_id, reel_id, scanner_index=0, add_to_test=False):
         mutex.acquire()
         if cur_id not in self.test_barcodes.keys() and cur_id not in self.barcodes_read.keys() and add_to_test:
             self.barcodes_read[cur_id] = {'chamber': scanner_index,
                                           'packets': [],
                                           'reel': self.reel_id,
                                           'ext ID': cur_id,
@@ -373,42 +350,42 @@
                                           'adv_address': [],
                                           'packetList': PacketList()}
             # self.test_barcodes[cur_id] = scanner_index
             self.builder.get_object('scanned').insert(END, f'{cur_id}, {scanner_index}')
             mutex.release()
         else:
             mutex.release()
-            self.comConnect.popup_message(f'Tag {cur_id} in chamber {scanner_index} already read.', title='Warning', log='warning')
+            popup_message(f'Tag {cur_id} in chamber {scanner_index} already read.', title='Warning', log='warning')
             return False
 
         if self.reel_id != '' and self.reel_id != reel_id and self.wiliotTags:
-            self.comConnect.popup_message('Tag reel different from test reel.', title='Warning', log='error')
-
+            popup_message('Tag reel different from test reel.', title='Warning', log='error')
+        
         return True
-
+    
     def update_go_state(self, force_go=False):
         if (self.comConnect.get_num_of_barcode_scanners() == len(self.barcodes_read.keys()) or force_go) and \
                 len(self.test_barcodes.keys()) > 0:
             self.builder.tkvariables.get('go').set(CONTINUE)
             self.update_params_state(state='normal', group=CONTINUE)
         elif self.comConnect.get_num_of_barcode_scanners() == len(self.barcodes_read.keys()) or force_go:
             self.builder.tkvariables.get('go').set(GO)
             self.update_params_state(state='normal', group=GO)
         else:
             self.builder.tkvariables.get('go').set(READ)
             self.update_params_state(state='normal', group=READ)
         # self.top_builder.get_object('go')['state'] = 'normal'
-
+    
     def get_missing_ids_chambers(self):
         indexes = list(range(self.comConnect.get_num_of_barcode_scanners()))
         if len(self.barcodes_read.keys()) > 0:
             used_indexes = [barcode['chamber'] for barcode in self.barcodes_read.values()]
             indexes = [index for index in indexes if index not in used_indexes]
         return indexes
-
+    
     def force_go(self):
         """
         enable go in the GUI even if some of the chambers are empty
         """
         if self.builder.get_variable('forceGo').get() == '1':
             self.builder.get_object('forceGo')['state'] = 'disabled'
             self.builder.get_object('stop')['state'] = 'disabled'
@@ -417,23 +394,23 @@
             self.builder.get_object('remove')['state'] = 'disabled'
             if self.closeChambersThread is not None and self.closeChambersThread.is_alive():
                 self.closeChambersThread.join()
             self.closeChambersThread = Thread(target=self.force_go_close_chambers, args=())
             self.closeChambersThread.start()
         else:
             self.update_go_state()
-
+    
     def force_go_close_chambers(self):
         indexes = self.get_missing_ids_chambers()
         self.comConnect.close_chambers(indexes)
         self.update_go_state(force_go=True)
         self.builder.get_object('forceGo')['state'] = 'normal'
         self.builder.get_object('stop')['state'] = 'normal'
         self.builder.get_object('go')['state'] = 'normal'
-
+    
     def calib_mode(self):
         self.testFinished = False
         attenuations = numpy.arange(float(self.low), float(self.high) + float(self.step), float(self.step))
         n_rep = int(self.n_repetitions)
         for i in attenuations:
             for j in range(n_rep):
                 calibMutex.acquire()
@@ -456,44 +433,43 @@
 
                 self.sendCommandThread = Thread(target=self.send_gw_commands, args=())
                 self.sendCommandThread.start()
                 self.sendCommandThread.join()
                 sleep(5)
                 if self.forceCloseRequested:
                     break
-
+        
         calibMutex.acquire()
         self.calib_mode_post_process()
         self.comConnect.open_chambers()
         # self.builder.tkvariables.get('numTags').set(0)
         # self.builder.tkvariables.get('go').set(READ)
         # self.test_barcodes = {}
         # self.builder.get_object('connect')['state'] = 'normal'
         # self.builder.get_object('read_qr')['state'] = 'normal'
         calibMutex.release()
         self.finish_test(post_data=False, reset_tester=True, post_process=False)
-        self.comConnect.popup_message('Sample Test - Calib Mode Finished running.', title='Info', log='info')
-
+        popup_message('Sample Test - Calib Mode Finished running.', title='Info', log='info')
+    
     def calib_mode_post_process(self):
         common_run_name = self.reel_id + '_' + self.testDir
         unique_valid = []
-        full_test_dir = abspath(join(OUTPUT_DIR, self.testName, self.testDir))
+        full_test_dir = join(OUTPUT_DIR, self.testName, self.testDir)
         is_first = True
         for atten, runData in self.packets_dict.items():
             for extId, data in runData.items():
                 if data['packetList'].size() > 0:
                     packet_df = data['packetList'].get_df(add_sprinkler_info=True)
                     packet_df.insert(loc=len(packet_df.columns), column='status', value='PASSED')
                     packet_df.insert(loc=len(packet_df.columns), column='attenuation', value=float(atten.split('_')[0]))
                     packet_df.insert(loc=len(packet_df.columns), column='test_num', value=int(atten.split('_')[1]))
                     packet_df.insert(loc=len(packet_df.columns), column='external_id', value=extId)
                     packet_df.insert(loc=len(packet_df.columns), column='chamber', value=data['chamber'])
                     data['packetList'].export_packet_df(
-                        packet_df=packet_df,
-                        path=abspath(join(full_test_dir, f'{common_run_name}@packets_data_calib_mode.csv')),
+                        packet_df=packet_df, path=join(full_test_dir, f'{common_run_name}@packets_data_calib_mode.csv'),
                         append=not is_first)
                     is_first = False
                 
                 unique_valid.append({
                     'adv_address': data['adv_address'],
                     'tbp': data['tbp'],
                     'ttfp': data['ttfp'],
@@ -501,16 +477,15 @@
                     'reel': data['reel'],
                     'attenuation': float(atten.split('_')[0]),
                     'test_num': int(atten.split('_')[1]),
                     'chamber': data['chamber']
                 })
         
         if len(unique_valid):
-            with open(abspath(join(full_test_dir, f'{common_run_name}@unique_data.csv')), 'w+',
-                      newline='') as new_tagsCsv:
+            with open(join(full_test_dir, f'{common_run_name}@unique_data.csv'), 'w+', newline='') as new_tagsCsv:
                 writer = csv.DictWriter(new_tagsCsv, fieldnames=list(unique_valid[0].keys()))
                 writer.writeheader()
                 writer.writerows(unique_valid)
         
         self.barcodes_read = {}
         self.test_barcodes = {}
         self.builder.get_object('scanned').delete(0, END)
@@ -525,37 +500,26 @@
     
     def stop(self):
         """
         stop the test and run post process
         """
         if self.stopButtonState == STOP:
             self.forceCloseRequested = True
-
+        
         elif self.stopButtonState == FINISH:
             # self.numOfTags = len(self.test_barcodes.keys())
             # self.finishThread = Thread(target=self.iteration_finished, args=([True]))
             # self.finishThread.start()
             self.builder.get_object('scanned').delete(0, END)
             self.builder.tkvariables.get('stop').set(SEND)
             self.stopButtonState = SEND
             for barcode in list(self.test_barcodes.keys()):
                 self.builder.get_object('scanned').insert(END, barcode)
         
         elif self.stopButtonState == SEND:
-            if not self.is_test_completed() and 'controlLimits' in self.defaultDict.keys():
-                control_limits = self.defaultDict['controlLimits'][self.defaultDict['controlLimitsTestNum']]
-                self.update_values_for_control_limits(control_limits=control_limits)
-                is_pass, fail_str, complete_sub_test, fail_bin = self.check_control_limits()
-                self.reset_values_for_control_limits(control_limits=control_limits)
-                if not is_pass or not complete_sub_test:
-                    send_anyway = popup_yes_no(f'Test was FAILED!! are you sure you want to finish the test and '
-                                               f'send data to the cloud?')
-                    if not send_anyway:
-                        self.logger.info('User decide to keep testing')
-                        return
             self.builder.get_object('go')['state'] = 'disabled'
             self.builder.get_object('stop')['state'] = 'disabled'
             self.builder.get_object('forceGo')['state'] = 'disabled'
             self.builder.get_object('add')['state'] = 'disabled'
             self.builder.get_object('remove')['state'] = 'disabled'
             self.finishThread = Thread(target=self.finish, args=())
             self.finishThread.start()
@@ -572,32 +536,31 @@
             if self.builder.tkvariables.get('stop').get() == SEND:
                 self.builder.get_object('scanned').delete(0, END)
                 self.remove_barcodes()
                 self.stopButtonState = FINISH
                 self.builder.tkvariables.get('stop').set(FINISH)
             
             if len(new_tag.split(',')) < 2:
-                self.comConnect.popup_message(f'Missing chamber index, add chamber index after a comma.', title='Error', log='error')
+                popup_message(f'Missing chamber index, add chamber index after a comma.', title='Error', log='error')
                 return
             cur_id = new_tag.split(',')[0].strip()
             scan_index = int(new_tag.split(',')[1].strip())
             if 0 < self.comConnect.get_num_of_barcode_scanners() < (scan_index + 1):
-                self.comConnect.popup_message(f'Chamber number {scan_index} not exists.', title='Error', log='error')
+                popup_message(f'Chamber number {scan_index} not exists.', title='Error', log='error')
                 return
             
             barcodes = self.builder.get_object('scanned').get(0, END)
             if any([barcode for barcode in barcodes if int(barcode.split()[1].strip()) == scan_index]):
-                self.comConnect.popup_message(f'Chamber {scan_index} tag already scanned.', title='Error', log='error')
+                popup_message(f'Chamber {scan_index} tag already scanned.', title='Error', log='error')
                 return
             # logger.info(scan_index)
             
             self.builder.tkvariables.get('addTag').set('')
-            popup_thread = Thread(target=self.comConnect.popup_message,
-                                  args=('Chambers are closing!!\nWatch your hands!!!',
-                                        'Warning', ("Helvetica", 18), 'warning'))
+            popup_thread = Thread(target=popup_message, args=('Chambers are closing!!\nWatch your hands!!!',
+                                                              'Warning', ("Helvetica", 18), 'warning'))
             popup_thread.start()
             popup_thread.join()
             self.add_tag_to_test(cur_id, self.reel_id, scan_index, add_to_test=True)
             chambers = self.comConnect.get_chambers()
             if len(chambers) > scan_index and chambers[scan_index] is not None:
                 chambers[scan_index].close_chamber()
             self.update_go_state()
@@ -700,15 +663,15 @@
         self.builder.get_variable('isCalib').set(str(int(self.calib)))
         self.builder.get_variable('isOffline').set(str(int(self.offline)))
         self.builder.get_variable('isTestEnv').set(str(int(self.environment == 'test')))
         
         if 'config' in self.defaultDict.keys():
             self.testConfig = self.defaultDict['config']
         else:
-            self.testConfig = ''
+            self.testConfig = []
         self.builder.get_object('test_config').set(self.testConfig)
         self.configsGui.set_default_config(self.testConfig)
         self.configsGui.set_params(self.testConfig)
     
     def open_configs(self):
         """
         open Configs GUI
@@ -732,15 +695,15 @@
             self.comTtk = Toplevel(self.ttk)
             self.ttk.eval(f'tk::PlaceWindow {str(self.comTtk)} center')
             self.comConnect.gui(self.comTtk)
     
     def read_qr(self):
         barcode, reel = self.comConnect.read_barcode()
         if barcode is None:
-            read_qr_thread = Thread(target=self.comConnect.popup_message, args=(
+            read_qr_thread = Thread(target=popup_message, args=(
                 [f'Error reading external ID, try repositioning the tag.', 'Error', ("Helvetica", 10), 'error']))
             read_qr_thread.start()
             read_qr_thread.join()
             if not self.calib:
                 return
         
         if reel is not None:
@@ -803,21 +766,14 @@
         self.runDataDict['timeProfile'] = '[{}, {}]'.format(params['tOn'], params['tTotal'])
         self.runDataDict['txPower'] = 'max'
         self.runDataDict['controlLimits'] = 'tagTbpRange: [{},{}], testTbpRange: [{},{}], respondingThr[%]: {}, ' \
                                             'validTbpThr[%]: {}'.format(params['tag_tbp_min'], params['tag_tbp_max'],
                                                                         params['test_tbp_min'], params['test_tbp_max'],
                                                                         params['test_responding_min'],
                                                                         params['test_valid_tbp'])
-        if 'controlLimits' in self.defaultDict.keys():
-            self.logger.info('reset control limits')
-            self.runDataDict['controlLimits'] = self.defaultDict['controlLimits'].copy()
-            self.defaultDict['controlLimitsTestNum'] = 0
-            self.params['tag_tbp_min'] = self.defaultDict['controlLimits'][0]['tag_tbp_min']
-            self.params['tag_tbp_max'] = self.defaultDict['controlLimits'][0]['tag_tbp_max']
-
         self.runDataDict['hwVersion'] = self.defaultDict['tester_hw']['version'] \
             if 'tester_hw' in self.defaultDict.keys() else ''
         self.runDataDict['sub1gFrequency'] = params['EmulateSurfaceValue']
 
     def send_gw_commands(self):
         """
         send commands to the GW and start the packet listener
@@ -834,18 +790,18 @@
     def stop_state(self):
         self.builder.get_object('stop')['state'] = 'normal'
     
     def recv_data_from_gw(self):
         self.tagsFinished = {}
         self.testGo = True
         self.startTime = self.comConnect.get_gw_time()
-        self.logger.info(f'Tags in the test: {",".join(list(self.barcodes_read.keys()))}')
+        logger.info(f'Tags in the test: {",".join(list(self.barcodes_read.keys()))}')
         gw_passed = self.comConnect.send_gw_app(self.params)
         if not gw_passed:
-            self.comConnect.popup_message(f'Error sending GW commands.', 'Error', ("Helvetica", 10), 'error')
+            popup_message(f'Error sending GW commands.', 'Error', ("Helvetica", 10), 'error')
             self.update_params_state(state='normal', group=CONTINUE)
             return
         self.gatewayDataThread = Thread(target=self.stop_state(), args=())
         self.gatewayDataThread.start()
         last_time = time.time()
         self.targetTime = last_time + self.testTime
         if self.timerThread is not None:
@@ -856,15 +812,15 @@
         self.sync_thread.start()
         packets_list = PacketList()
         recvDataMutex.acquire()
         while True:
             sleep(0.001)
             try:
                 if self.closeListener:
-                    self.logger.info("DataHandlerProcess Stop")
+                    logger.info("DataHandlerProcess Stop")
                     break
                 
                 if self.comConnect.is_gw_data_available():
                     
                     gw_data = self.comConnect.get_data()
                     
                     packets_list.__add__(gw_data)
@@ -962,37 +918,37 @@
                 print(packet.get_packet_string())
                 full_data, success = self.get_packet_ext_id(packet)
 
                 if not success:
                     if not post_run:
                         self.unknown_packets.append(packet)
                         if adv_address not in self.advas_dict.keys():
-                            self.logger.error(
+                            logger.error(
                                 f'Could not get external ID for adv_address {adv_address} '
                                 f'from the cloud - saving data for post process')
                         self.advas_dict[adv_address] = None
                     else:
-                        self.logger.error(
+                        logger.error(
                             f'Could not get external ID for adv_address {adv_address} '
                             f'from the cloud - dumping packet')
                     continue
 
                 ext_id = full_data['barcode'] if full_data['barcode'] in self.barcodes_read.keys() else full_data[
                     'cur_id']
                 if ext_id is not None and ext_id not in self.barcodes_read.keys():
-                    self.logger.info(
+                    logger.info(
                         f'Tag with adv_address {adv_address} and external ID {full_data["cur_id"]} '
                         f'detected but not belong to the test.')
                     self.bad_advas.append(adv_address)
                     continue
 
                 self.advas_dict[adv_address] = ext_id
 
                 if adv_address not in self.barcodes_read[ext_id]['adv_address']:
-                    self.logger.info(
+                    logger.info(
                         f'New Tag detected with adv_address {adv_address} and external ID {full_data["cur_id"]}.')
                     self.barcodes_read[ext_id]['adv_address'].append(adv_address)
             
             self.barcodes_read[ext_id]['packets'].append(packet.get_packet_string())
             self.barcodes_read[ext_id]['packetList'].append(packet.copy())
             
             if self.barcodes_read[ext_id]['packetList'].get_statistics()['sprinkler_counter_max'] > 3 and not post_run:
@@ -1024,21 +980,21 @@
         
         self.finish_test()
         
         # read_tags = ''
         # if self.tagsCount < self.numOfTags and not force_finish:
         read_tags = '\nReplace tags and click on "Read"'
         
-        finishThread = Thread(target=self.comConnect.popup_message, args=(f'{serial_warning}'
-                                                                          f'{stat}'
-                                                                          f'{read_tags}',
-                                                                          'info',
-                                                                          ("Helvetica", 10),
-                                                                          'info',
-                                                                          bg_color))
+        finishThread = Thread(target=popup_message, args=(f'{serial_warning}'
+                                                          f'{stat}'
+                                                          f'{read_tags}',
+                                                          'info',
+                                                          ("Helvetica", 10),
+                                                          'info',
+                                                          bg_color))
         finishThread.start()
         finishThread.join()
         
         self.update_params_state(state='normal', group=READ)
         
         self.builder.tkvariables.get('numTags').set(len(self.test_barcodes.keys()))
         self.builder.tkvariables.get('addTag').set('')
@@ -1063,15 +1019,15 @@
         self.remove_barcodes()
         self.finish_test(True, True)
         # self.finishTestThread = Thread(target=self.finish_test, args=([True, True]))
         # self.finishTestThread.start()
     
     def handle_unknown_packets(self):
         if self.unknown_packets.size() > 0:
-            self.logger.info(f'Start handling unknown packets.')
+            logger.info(f'Start handling unknown packets.')
             self.process_packets(self.unknown_packets, post_run=True)
     
     def post_process_iteration(self):
         tbp_count = 0
         ttfp_count = 0
         ttfp_avg = 0
         tbp_avg = 0
@@ -1089,169 +1045,81 @@
                 ttfp_avg = ((ttfp_avg * ttfp_count) + ttfp) / (ttfp_count + 1)
                 self.barcodes_read[extId]['tbp'] = int(tbp)
                 self.barcodes_read[extId]['ttfp'] = ttfp
                 
                 self.barcodes_read[extId]['rssi'] = float(stat["rssi_mean"])
         
         return tbp_avg, ttfp_avg
-
-    def update_values_for_control_limits(self, control_limits):
-        self.params['test_tbp_min'] = control_limits['test_tbp_min']
-        self.params['test_tbp_max'] = control_limits['test_tbp_max']
-        self.params['test_responding_min'] = control_limits['test_responding_min']
-        self.params['test_valid_tbp'] = control_limits['test_valid_tbp']
-
-
-    def reset_values_for_control_limits(self, control_limits):
-        self.params['tag_tbp_min'] = control_limits['tag_tbp_min']
-        self.params['tag_tbp_max'] = control_limits['tag_tbp_max']
-        self.params['test_tbp_min'] = ''
-        self.params['test_tbp_max'] = ''
-        self.params['test_responding_min'] = ''
-        self.params['test_valid_tbp'] = ''
-
-    def update_control_limits(self, reset_test=False):
-        next_test = False
-        if 'controlLimits' in self.defaultDict.keys():
-            self.logger.info(f'Check control limits for pre-defined phased-test:'
-                             f'\nnumber of tested:{self.dataBaseDict["tested"]}')
-            if reset_test and self.defaultDict['controlLimitsTestNum'] < len(self.defaultDict['controlLimits']) - 1:
-                self.defaultDict['controlLimitsTestNum'] += 1
-                self.logger.info(f'move to the next test: {self.defaultDict["controlLimitsTestNum"]}')
-
-            control_limits = self.defaultDict['controlLimits'][self.defaultDict['controlLimitsTestNum']]
-
-            if reset_test:
-                self.reset_values_for_control_limits(control_limits=control_limits)
-
-            elif self.dataBaseDict['tested'] >= int(control_limits['n_tags']):
-                self.update_values_for_control_limits(control_limits=control_limits)
-                next_test = True
-        return next_test
-
-    def is_test_completed(self):
-        completed = True
-        if 'controlLimits' in self.defaultDict.keys():
-            control_limits = self.defaultDict['controlLimits'][-1]
-            if self.dataBaseDict['tested'] < int(control_limits['n_tags']):
-                completed = False
-        return completed
-
+    
     def check_control_limits(self):
-        complete_sub_test = self.update_control_limits(reset_test=False)
         is_pass = True
         fail_str = ''
-        fail_bin = FailureCodeSampleTest.PASS
 
+        if self.params['test_tbp_min'] != '' and self.params['test_tbp_max'] != '':
+            if not int(self.params['test_tbp_min']) < float(
+                    self.runDataDict['tbpAvg']) < int(self.params['test_tbp_max']):
+                is_pass = False
+                fail_str += 'Failed tbp avg test. '
         if self.params['test_responding_min'] != '':
-            if float(self.dataBaseDict['responding[%]'].replace('%', '')) < float(self.params['test_responding_min']):
+            if int(self.dataBaseDict['responding[%]'].replace('%', '')) < int(self.params['test_responding_min']):
                 is_pass = False
                 fail_str += 'Failed % responding test. '
-                if fail_bin == FailureCodeSampleTest.PASS:
-                    fail_bin = FailureCodeSampleTest.NO_RESPONSE
         if self.params['test_valid_tbp'] != '':
-            if float(self.dataBaseDict['passed[%]'].replace('%', '')) < float(self.params['test_valid_tbp']):
+            if int(self.dataBaseDict['passed[%]'].replace('%', '')) < int(self.params['test_valid_tbp']):
                 is_pass = False
                 fail_str += 'Failed % tags with valid tbp avg test. '
-                if fail_bin == FailureCodeSampleTest.PASS:
-                    fail_bin = FailureCodeSampleTest.NO_TBP
-        if self.params['test_tbp_min'] != '' and self.params['test_tbp_max'] != '':
-            if not int(self.params['test_tbp_min']) < float(
-                    self.runDataDict['tbpAvg']) < int(self.params['test_tbp_max']):
-                is_pass = False
-                fail_str += 'Failed tbp avg test. '
-                if fail_bin == FailureCodeSampleTest.PASS:
-                    fail_bin = FailureCodeSampleTest.HIGH_TBP_AVG
-
-
-        return is_pass, fail_str, complete_sub_test, fail_bin
+        return is_pass, fail_str
 
     def finish_test(self, post_data=False, reset_tester=False, post_process=True):
+        pass_fail, fail_str, serial_warning, bg_color = ['', '', '', '']
         if post_process:
             pass_barcodes = self.post_process()
-            pass_fail, fail_str, complete_sub_test, fail_bin = self.check_control_limits()
-            if complete_sub_test and not pass_fail:
-                self.update_control_limits(reset_test=True)
-
+            
             dup_adva = [extId for extId, tag in self.test_barcodes.items() if len(tag['adv_address']) > 1]
-
+            
+            pass_fail, fail_str = self.check_control_limits()
+            self.runDataDict['testStatus'] = pass_fail
             all_answered = all([False for ext_id in self.test_barcodes.values() if len(ext_id['packets']) == 0])
             serial_warning = (not all_answered) and len(self.total_bad_advas) != 0
             adva_warning = len(dup_adva) > 0
             serial_warning = '' if not serial_warning else 'Serialization warning!\n'
             serial_warning = serial_warning \
                 if not adva_warning else serial_warning + f'ADVA warning in tags: {dup_adva}\n'
-            bg_color = 'green'
-            if 'controlLimits' not in self.defaultDict.keys():
-                bg_color = 'green' if not (serial_warning or adva_warning) else 'yellow'
+            bg_color = 'green' if not (serial_warning or adva_warning) else 'yellow'
             bg_color = bg_color if pass_fail else 'red'
-            pass_fail_str = 'Passed' if pass_fail else 'Failed'
-
-            if 'controlLimits' in self.defaultDict.keys():
-                if reset_tester and not complete_sub_test:
-                    # user click on finish but test was not completed:
-                    if fail_bin == FailureCodeSampleTest.PASS:
-                        fail_bin = FailureCodeSampleTest.NOT_COMPLETED
-                        pass_fail = False
-                        pass_fail_str = 'Failed'
-                        bg_color = 'red'
-                if complete_sub_test and not reset_tester:
-                    new_test_pass_str = 'SUCCESSFULLY COMPLETED THE TEST! please move to the next reel'
-                    last_stage = self.is_test_completed()
-                    new_test_fail_str = 'FAILED CURRENT TEST STAGE,' + \
-                                        ' failed the reel' if last_stage else ' please continue to test the reel'
-                    if not last_stage and not pass_fail:
-                        bg_color = 'yellow'
-                    self.comConnect.popup_message(f'Test {self.common_run_name} has {pass_fail_str}\n' +
-                                                  f'{fail_str}\n' +
-                                                  f'{new_test_pass_str if pass_fail else new_test_fail_str}'
-                                                  f'\n' +
-                                                  f'{serial_warning}'
-                                                  f'Fail bin: {fail_bin.value}:{fail_bin.name}', title='Finished test',
-                                                  bg=bg_color,
-                                                  log='info')
-            self.is_test_pass = pass_fail
-        
-            if reset_tester:
-                self.comConnect.popup_message(f'Test {self.common_run_name} has {pass_fail_str}\n' +
-                                              f'{fail_str}\n' +
-                                              f'{serial_warning}' +
-                                              f'Fail bin: {fail_bin.value}:{fail_bin.name}\n' +
-                                              f'Average TTFP: {self.dataBaseDict["ttfpAvg"]} [sec]\n' +
-                                              f'Average TBP: {self.dataBaseDict["tbpAvg"]} [msec]\n' +
-                                              f'STD TBP: {self.dataBaseDict["tbpStd"]} [msec]\n' +
-                                              f'Yield: {self.dataBaseDict["responding[%]"]}', title='Finished test',
-                                              bg=bg_color,
-                                              log='info')
-                self.update_control_limits(reset_test=True)
-
-            # log data:
-            self.runDataDict['testStatus'] = pass_fail
-            self.runDataDict['failBin'] = str(fail_bin.value) + str(self.defaultDict['controlLimitsTestNum']) \
-                if 'controlLimitsTestNum' in self.defaultDict.keys() else ''
-            self.runDataDict['failBinStr'] = fail_bin.name
-
+            pass_fail = 'Passed' if pass_fail else 'Failed'
+            
             self.files_and_cloud(post_data)
         
+        if reset_tester and post_process:
+            popup_message(f'Test {self.common_run_name} has {pass_fail}\n' +
+                          f'{fail_str}\n' +
+                          f'{serial_warning}' +
+                          f'Average TTFP: {self.dataBaseDict["ttfpAvg"]} [sec]\n' +
+                          f'Average TBP: {self.dataBaseDict["tbpAvg"]} [msec]\n' +
+                          f'STD TBP: {self.dataBaseDict["tbpStd"]} [msec]\n' +
+                          f'Yield: {self.dataBaseDict["responding[%]"]}', title='Finished test', bg=bg_color,
+                          log='info')
+        
         if reset_tester:
             # self.tagsCount = 0
             self.builder.get_object('reelId').bind("<Key>", self.get_reel_id)
             self.builder.tkvariables.get('numTags').set(0)
             self.builder.tkvariables.get('go').set(READ)
             self.testFinished = True
             self.packets_dict = {}
             self.test_barcodes = {}
             self.barcodes_read = {}
             self.reel_id = ''
             self.gtin = ''
             self.builder.tkvariables.get('reelId').set('')
             
-            changeFileHandler(self.logger, self.logger_path, file_mode='a+', append_handler=True)
-            self.logger.info(f'Test {self.common_run_name} ended.')
-            removeFileHandler(self.logger, self.test_log_file)
+            changeFileHandler(logger, default_log_file, file_mode='a+', append_handler=True)
+            logger.info(f'Test {self.common_run_name} ended.')
+            removeFileHandler(logger, self.test_log_file)
             self.update_params_state(state='normal', group=READ)
             self.builder.tkvariables.get('stop').set(STOP)
             self.builder.get_object('stop')['state'] = 'disabled'
 
         if self.offline:
             self.offline_tag_index = 0
 
@@ -1295,22 +1163,22 @@
                                    'adv_address': data['adv_address'],
                                    'state(tbp_exists:0,no_tbp:-1,no_ttfp:-2,dup_adv_address:-3)': tag_state,
                                    'status': data['status'], 'chamber': data['chamber'],
                                    'temperature_from_sensor': temperature_from_sensor
                                    }
                         
                         packets_csv.append_dict_as_row([tag_row])
-
-        with open(abspath(join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@configs_data.csv')),
+        
+        with open(join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@configs_data.csv'),
                   'w+', newline='') as newCsv:
             writer = csv.DictWriter(newCsv, fieldnames=self.dataBaseDict.keys())
             writer.writeheader()
             writer.writerows([self.dataBaseDict])
-
-        with open(abspath(join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@tags_data.csv')),
+        
+        with open(join(OUTPUT_DIR, self.testName, self.testDir, f'{self.common_run_name}@tags_data.csv'),
                   'w+', newline='') as newCsv:
             ids_dict = self.test_barcodes
             tags = []
             for extId, tag in ids_dict.items():
                 if tag['chamber'] < len(self.comConnect.temperature_sensor_readings):
                     all_reading_temp = self.comConnect.temperature_sensor_readings[tag['chamber']]
                 else:
@@ -1337,18 +1205,18 @@
             writer = csv.DictWriter(newCsv, fieldnames=tags[0].keys())
             writer.writeheader()
             writer.writerows(tags)
         
         if post_data and self.post_data:
             post_success = self.post_to_cloud(run_data_path, tags_data_path, environment=self.environment)
             if not post_success:
-                self.comConnect.popup_message(f'Failed uploading run and/or tags data, Upload manually:\n' +
-                                              f'{self.common_run_name}@run_data.csv\n' +
-                                              f'{self.common_run_name}@packets_data.csv', log='warning')
-    
+                popup_message(f'Failed uploading run and/or tags data, Upload manually:\n' +
+                              f'{self.common_run_name}@run_data.csv\n' +
+                              f'{self.common_run_name}@packets_data.csv', log='warning')
+
     def get_packet_ext_id(self, packet):
         """
         get external ID of a tag by sending an example packet to the cloud.
         :type packet: Packet
         :param packet: contains the raw and time of the packet.
         :return: external ID of the tag, and the external ID parsed when it's wiliot tag.
         """
@@ -1411,24 +1279,17 @@
             if not first_iter:
                 try_again = popup_yes_no(f'Could not post data to cloud, try again?')
                 if not try_again:
                     return False
             
             success = upload_to_cloud_api(batch_name=self.reel_id, tester_type='sample-test',
                                           run_data_csv_name=run_data_file_path,
-                                          packets_data_csv_name=packets_data_file_path,
-                                          is_path=True,
-                                          env=environment,
-                                          owner_id=self.owner,
-                                          logger_='sample')
+                                          tags_data_csv_name=packets_data_file_path, env=environment, is_path=True,
+                                          client=self.client, packets_instead_tags=True)
             first_iter = False
-
-        if not success:
-            self.comConnect.popup_message(f'Run upload failed. Check exception error at the console and check Internet connection is available and upload logs manually.', title='Upload Error',
-                                          log='error')
         
         return success
 
     def post_process(self):
         tbp_arr = []
         ttfp_arr = []
         rssi_arr = []
@@ -1459,17 +1320,17 @@
         num_of_answered = len(ttfp_arr)
         num_of_pass = len(pass_barcodes)
         self.dataBaseDict['packets'] = self.numOfPackets
         self.dataBaseDict['tested'] = self.runDataDict['tested'] = tested_barcodes
         self.dataBaseDict['responded'] = self.runDataDict['responded'] = num_of_answered
         self.dataBaseDict['passed'] = self.runDataDict['passed'] = num_of_pass
         self.dataBaseDict['responding[%]'] = self.runDataDict['responding[%]'] = self.runDataDict['yield'] = \
-            f'{float((num_of_answered / tested_barcodes) * 100) if tested_barcodes > 0 else 0}%'
+            f'{int((num_of_answered / tested_barcodes) * 100) if tested_barcodes > 0 else 0}%'
         self.dataBaseDict['passed[%]'] = self.runDataDict[
-            'passed[%]'] = f'{float((num_of_pass / tested_barcodes) * 100 if tested_barcodes > 0 else 0)}%'
+            'passed[%]'] = f'{int((num_of_pass / tested_barcodes) * 100 if tested_barcodes > 0 else 0)}%'
         # calc ttfp
         avg_ttfp = sum(ttfp_arr) / len(ttfp_arr) if len(ttfp_arr) > 0 else -1
         ttfp_arr = ttfp_arr if len(ttfp_arr) > 0 else [-1]
         
         self.dataBaseDict['ttfpStd'] = f'{numpy.std(ttfp_arr):.3f}'
         self.runDataDict['ttfpAvg'] = self.dataBaseDict['ttfpAvg'] = f'{avg_ttfp:.3f}'
         self.dataBaseDict['ttfpMin'] = f'{min(ttfp_arr):.3f}'
@@ -1531,16 +1392,16 @@
         temp_coms = self.comConnect.get_default_dict()
         if self.station_name.strip() != '':
             temp_coms['stationName'] = self.station_name
         if self.testConfig != '':
             temp_coms['config'] = self.testConfig
         if self.calib:
             temp_coms[f'{self.antenna}_calib'] = {'low': self.low, 'high': self.high, 'step': self.step}
-
-        with open(abspath(join(CONFIGS_DIR, '.defaults.json')), 'w+') as defaultComs:
+        
+        with open(join(CONFIGS_DIR, '.defaults.json'), 'w+') as defaultComs:
             dump(temp_coms, defaultComs, indent=4)
     
     def popup_login(self):
         """
         popup to insert fusion auth credentials, and choosing owner.
         """
         default_font = ("Helvetica", 10)
@@ -1587,24 +1448,24 @@
 
         popup.mainloop()
 
         if self.owner not in owner_id_list:
             owner_id_list.append(self.owner)
             owner_id_list = [o for o in owner_id_list if o != '']
             self.defaultDict['owner'] = owner_id_list
-            with open(abspath(join(CONFIGS_DIR, '.defaults.json')), 'w+') as defaultComs:
+            with open(join(CONFIGS_DIR, '.defaults.json'), 'w+') as defaultComs:
                 dump(self.defaultDict, defaultComs, indent=4)
     
     def popup_calib(self):
         """
         popup to choose calib mode parameters
         """
         default_font = ("Helvetica", 10)
         popup = Tk()
-        # popup.eval('tk::PlaceWindow . center')
+        popup.eval('tk::PlaceWindow . center')
         popup.wm_title('Login')
         
         # defaultDict = {}
         # if isfile(join(CONFIGS_DIR, '.defaults.json')):
         #     with open(join(CONFIGS_DIR, '.defaults.json'), 'r') as defaultComs:
         #         defaultDict = load(defaultComs)
         
@@ -1629,15 +1490,15 @@
                 e3.delete(0, END)
                 e4.delete(0, END)
                 e5.delete(0, END)
                 e2.insert(0, antennaDict['low'])
                 e3.insert(0, antennaDict['high'])
                 e4.insert(0, antennaDict['step'])
                 e5.insert(0, 1)
-
+        
         l1 = Label(popup, text='Enter calibration parameters:', font=default_font)
         l1.grid(row=1, column=0, padx=10, pady=10, columnspan=3)
         l2 = Label(popup, text='Antenna Type:', font=default_font)
         l2.grid(row=2, column=0, padx=10, pady=10)
         c2 = ttk.Combobox(popup, values=['BLE', 'LoRa'])
         c2.grid(row=2, column=1, padx=10, pady=10)
         c2.bind("<FocusOut>", update_antenna_params)
@@ -1665,36 +1526,32 @@
         
         popup.mainloop()
         
         # return antenna, low, high, step
 
     def on_send_to_cloud(self):
         self.post_data = bool(int(self.builder.get_variable('sendToCloud').get()))
-        self.logger.info(f'send to cloud was changed to {self.post_data}')
+        logger.info(f'send to cloud was changed to {self.post_data}')
 
     def on_power_calib(self):
         self.calib = bool(int(self.builder.get_variable('isCalib').get()))
-        self.logger.info(f'calibration mode was changed to {self.calib}')
+        logger.info(f'calibration mode was changed to {self.calib}')
 
     def on_offline(self):
         self.offline = bool(int(self.builder.get_variable('isOffline').get()))
-        self.logger.info(f'offline mode was changed to {self.offline}')
+        logger.info(f'offline mode was changed to {self.offline}')
 
     def on_test_env(self):
         self.environment = 'test' if bool(int(self.builder.get_variable('isTestEnv').get())) else ''
         env_for_printing = self.environment if self.environment != '' else 'production'
-        self.logger.info(f'sending data to {env_for_printing} environment')
+        logger.info(f'sending data to {env_for_printing} environment')
 
 
-def popup_yes_no(question, tk_frame=None):
-    if tk_frame is None:
-        root = Tk()
-        root.eval(f'tk::PlaceWindow {str(root)} center')
-    else:
-        root = tk_frame
+def popup_yes_no(question):
+    root = Tk()
     root.wm_withdraw()
     result = messagebox.askquestion("Sample Test", question, icon='warning')
     root.destroy()
     if result == 'yes':
         return True
     else:
         return False
@@ -1724,17 +1581,17 @@
     post_data = args.post_data
     offline = args.offline
     
     # Run the UI
     # calib = True
     # offline = True
     if calib:
-        print(f'Sample Test - calibration mode active.')
+        logger.warning(f'Sample Test - calibration mode active.')
     if offline:
-        print(f'Sample Test - offline mode active.')
+        logger.warning(f'Sample Test - offline mode active.')
     app_folder = abspath(join(dirname(__file__), '../wiliot_testers'))
     try:
         sampleTest = SampleTest(calib=calib, environment=args.environment, post_data=post_data,
                                 offline=offline)
         sampleTest.gui()
     except BaseException:
         print_exc()
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/utils/com_connect.ui` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/com_connect.ui`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/utils/comm.gif` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/comm.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/utils/configs.gif` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/utils/configs.ui` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/configs.ui`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/utils/reset.png` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/reset.png`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/utils/sample_test.ui` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/sample_test.ui`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/sample/utils/wiliot3.gif` & `wiliot-testers-4.0.6/wiliot_testers/sample/utils/wiliot3.gif`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/system_test/harvester_test.py` & `wiliot-testers-4.0.6/wiliot_testers/system_test/harvester_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -57,49 +57,54 @@
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
 '''
 Eduard Tatievski
 '''
 
+
 import matplotlib.pyplot as plt
-from wiliot_testers.calibration_test.calibration_test_by_tbp import *
-from wiliot_core.packet_data import packet_list, packet, tag_collection
-from wiliot_testers.test_equipment import Attenuator, EquipmentError
-from wiliot_testers.wiliot_tester_log import *
 import PySimpleGUI as SimGUI
 import os
 import pathlib
 import datetime
 import csv
-import pandas as pd
 import collections
+import sys
+import threading
+import pandas as pd
+from wiliot_testers.test_equipment import Attenuator, EquipmentError
+from wiliot_testers.wiliot_tester_log import *
+from wiliot_core import WiliotGateway, ActionType, DataType
+from wiliot_core import PacketList, TagCollection
+from wiliot_testers.wiliot_tester_tag_test import *
+from wiliot_core import DecryptedPacketList, DecryptedTagCollection
 
 
 class Harvester(object):
 
     def __init__(self):
         # Getting all wanted values
         self.num_of_chambers = 1  # Number of chambers connected
         self.min_tags_answering = 1
         self.gui_values = self.init_gui()
         # Create log folder if not exist and build new name
         self.init_name_path()
         # Create log class
         self.my_logger = WiliotTesterLog(self.run_name_date)
-        self.my_logger.set_logger(self.log_path, tester_name='Harvester')
+        self.my_logger.set_logger(self.log_path, tester_name='harvester')
         # Connect to GW and Attenuator if selected
         self.init_hw()
         # Build new power list according to gui inputs
-        # self.power_range = self.build_range()
-        self.power = re.split('(d)', self.gui_values['power'])[0]
-        self.my_logger.results_logger.info('Starting scan on power: {}'.format(self.power))
-        self.frequency_range = list(range(int(self.gui_values['start_freq']), int(self.gui_values['stop_freq']) + 1,
-                                          int(self.gui_values['step'])))
-        self.all_results = pd.DataFrame({'Adva': [], 'Frequency': [], 'TBP': [], 'BB': []})
+        self.power_range = self.build_range()
+        self.my_logger.results_logger.info('Starting scan on powers: {}'.format(self.power_range))
+        if self.sub1g_enable:
+            self.frequency_range = list(range(850, 940, 1))
+        else:
+            self.frequency_range = list(range(2402, 2481, 2))
         self.scan()
 
     def calibrate_bb(self):
         if self.gw_obj.connected:
             self.gw_obj.reset_buffer()
             self.gw_obj.start_continuous_listener()
         for bb_val in reversed(self.bb_list):
@@ -185,15 +190,14 @@
 
     def init_hw(self):
 
         try:
             self.gw_obj = WiliotGateway(auto_connect=True, logger_name=self.my_logger.gw_logger.name, verbose=False)
             time.sleep(1)
             if self.gw_obj.connected:
-                self.gw_obj.reset_gw()
                 self.gw_obj.reset_buffer()
                 time.sleep(1.5)
                 self.gw_obj.start_continuous_listener()
                 self.gw_obj.write('!set_tester_mode 1', with_ack=True)
                 self.gw_obj.write('!pl_gw_config 1', with_ack=True)
                 self.gw_obj.write('!enable_brg_mgmt 0', with_ack=True)
                 self.gw_obj.write('!listen_to_tag_only 1', with_ack=True)
@@ -203,39 +207,35 @@
                 raise EquipmentError('Gateway Error - Verify WiliotGateway connection')
         except Exception as e:
             self.my_logger.gw_logger.warning(e)
             raise EquipmentError('Gateway Error - Verify WiliotGateway connection')
             self.gw_obj.close_port()
 
         if self.attn_enable:
-            self.attntype = self.gui_values['attntype']
-            self.attnval = int(self.gui_values['attnval'])
-
             try:
-                self.attn_obj = Attenuator(str(self.attntype)).GetActiveTE()
+                self.attn_obj = Attenuator('API').GetActiveTE()
                 current_attn = self.attn_obj.Getattn()
-                self.my_logger.gw_logger.info('Current attenuator values: {}'.format(current_attn))
             except Exception:
                 raise EquipmentError('Attenuator Error - Verify Attenuator connection')
 
     def init_name_path(self):
         self.log_path = os.path.join('', 'logs')
         if not os.path.exists(self.log_path):
             pathlib.Path(self.log_path).mkdir(parents=True, exist_ok=True)
         self.time_start = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
         self.run_name_date = str(self.gui_values['testName']) + '_' + str(self.time_start)
         self.full_name_path = os.path.join(self.log_path, self.run_name_date)
-        self.packets_csv_path = os.path.join(self.full_name_path, self.run_name_date + '.csv')
-        self.test_csv_path = os.path.join(self.full_name_path, self.run_name_date + '_tests.csv')
+        self.packets_csv_path =  os.path.join(self.full_name_path, self.run_name_date + '.csv')
+        self.test_csv_path =  os.path.join(self.full_name_path, self.run_name_date + '_tests.csv')
 
     def init_gui(self):
 
         # self.bb_list = [0, 2, 7, 12, 19, 20, 21, 22, 23, 24, 25, 27, 29, 30, 31, 32, 33, 36, 40]
-        self.bb_list = [40, 36, 33, 32, 31, 30, 29, 27, 25, 24, 23, 22, 21, 20, 19, 12, 7, 2, 0]
-        # self.bb_list = [12, 7, 2, 0]
+        # self.bb_list = [40, 36, 33, 32, 31, 30, 29, 27, 25, 24, 23, 22, 21, 20, 19, 12, 7, 2, 0]
+        self.bb_list = [12, 7, 2, 0]
 
         self.valid_sub1g_output_power = ['17dBm', '18dBm', '19dBm', '20dBm', '21dBm', '22dBm',
                                          '23dBm', '24dBm', '25dBm', '26dBm', '27dBm', '28dBm', '29dBm']
 
         self.valid_attn_sub1g_output_power = ['-10dBm', '-9dBm', '-8dBm', '-7dBm', '-6dBm', '-5dBm',
                                               '-4dBm', '-3dBm', '-2dBm', '-1dBm', '0dBm', '1dBm',
                                               '2dBm', '3dBm', '4dBm', '5dBm', '6dBm', '7dBm', '8dBm',
@@ -278,168 +278,119 @@
             {'abs_power': 21, 'gw_output_power': 'pos2dBm', 'bypass_pa': '0'},
             {'abs_power': 22, 'gw_output_power': 'pos3dBm', 'bypass_pa': '0'}]
 
         SimGUI.theme('GreenTan')
         layout = [[SimGUI.Text('Test Name', auto_size_text=True)],
                   [SimGUI.Input(key='testName', readonly=False, size=(30, 1))],
                   [SimGUI.Text('Num of tags'),
-                   SimGUI.Input(key='tagsNum', readonly=False, default_text=self.min_tags_answering, size=(4, 1))],
+                  SimGUI.Input(key='tagsNum', readonly=False, default_text=self.min_tags_answering, size=(4, 1))],
                   [SimGUI.Text('Test Time'),
                    SimGUI.Input(key='testTime', default_text='10', size=(7, 1))],
-                  # [SimGUI.Text('Which TBP requested?'),
-                  #  SimGUI.Input(key='requestedTBP', default_text='250', size=(7, 1))],
-                  [SimGUI.Text('Frequency range: Start [MHz]:'),
-                   SimGUI.Input(key='start_freq', default_text='2402', size=(5, 1)),
-                   SimGUI.Text('Stop [MHz]:'),
-                   SimGUI.Input(key='stop_freq', default_text='2480', size=(5, 1)),
-                   SimGUI.Text('Step [MHz]'),
-                   SimGUI.Input(key='step', default_text='2', size=(4, 1))],
-                  [SimGUI.Text('Energy : ', size=(14, 1)),
-                   SimGUI.InputCombo(tuple(self.abs_power_list), default_value=self.abs_power_list[0], key='power')],
-                  # SimGUI.InputCombo(tuple(self.abs_power_list),
-                  #                   default_value=self.abs_power_list[0], key='lowerPower'),
-                  # SimGUI.InputCombo(tuple(self.abs_power_list),
-                  #                   default_value=self.abs_power_list[-1], key='higherPower')],
-                  [SimGUI.Text('Beacons backoff', size=(14, 1)),
-                   SimGUI.InputCombo(tuple(self.bb_list),
-                                     default_value=self.bb_list[0], key='lowerBB'),
-                   SimGUI.InputCombo(tuple(self.bb_list),
-                                     default_value=self.bb_list[-1], key='higherBB')],
+                  [SimGUI.Text('Which TBP requested?'),
+                   SimGUI.Input(key='requestedTBP', default_text='100', size=(7, 1))],
                   [SimGUI.Button('2.4Ghz', button_color=('white', '#158225'), key='2.4mode', size=(10, 1)),
                    SimGUI.Button('Sub1G', button_color=('white', '#821515'), key='sub1gmode', size=(10, 1))],
                   [SimGUI.Text('Time profile - On:'),
                    SimGUI.Input(key='onTime', default_text='5', size=(3, 1)),
                    SimGUI.Text('Off:'),
                    SimGUI.Input(key='totalTime', default_text='15', size=(3, 1))],
                   [SimGUI.Button('Enable Attenuator', button_color=('white', '#158225'), key='attn', size=(20, 1))],
                   [SimGUI.Text('Attenuator Disabled', size=(40, 1), key='-ATTN-', text_color='Dark Red')],
-                  [SimGUI.Text('Attenuator type: ', size=(14, 1), visible=False, key='attntypeen'),
-                   SimGUI.InputCombo(('API', 'MCDI', 'MCDI-USB'),
-                                     default_value='API', key='attntype', visible=False)],
-                  [SimGUI.Text('Attenuation in dBm', visible=False, key='attnvalen'),
-                   SimGUI.Input(key='attnval', visible=False, default_text='0', size=(4, 1))],
+                  [SimGUI.Text('Energy boundaries', size=(14, 1)),
+                   SimGUI.InputCombo(tuple(self.abs_power_list),
+                                     default_value=self.abs_power_list[0], key='lowerPower'),
+                   SimGUI.InputCombo(tuple(self.abs_power_list),
+                                     default_value=self.abs_power_list[-1], key='higherPower')],
+
                   [SimGUI.Text(size=(40, 1), key='-OUTPUT-', text_color='red', font='bold')],
                   [SimGUI.Button('Submit', button_color=('white', '#0e6251'))]]
 
         window = SimGUI.Window('Harvester Test', layout, auto_size_text=True, auto_size_buttons=False)
         self.attn_enable = False
         self.sub1g_enable = False
         while True:
             event, values = window.read()
             # See if user wants to quit or window was closed
             if event == 'sub1gmode':
                 self.sub1g_enable = True
                 window['2.4mode'].update(button_color=('white', '#821515'))
                 window['sub1gmode'].update(button_color=('white', '#158225'))
-                window['power'].update(values=tuple(self.valid_sub1g_output_power),
-                                       value=self.valid_sub1g_output_power[0])
-                window['start_freq'].update(value='850')
-                window['stop_freq'].update(value='940')
-                # if self.attn_enable:
-                #     window['lowerPower'].update(value=self.valid_attn_sub1g_output_power[0],
-                #                                 values=tuple(self.valid_attn_sub1g_output_power))
-                #     window['higherPower'].update(values=tuple(self.valid_attn_sub1g_output_power),
-                #                                  value=self.valid_attn_sub1g_output_power[-1])
-                # else:
-                #     window['lowerPower'].update(values=tuple(self.valid_sub1g_output_power),
-                #                                 value=self.valid_sub1g_output_power[0])
-                #     window['higherPower'].update(values=tuple(self.valid_sub1g_output_power),
-                #                                  value=self.valid_sub1g_output_power[-1])
+                if self.attn_enable:
+                    window['lowerPower'].update(value=self.valid_attn_sub1g_output_power[0],
+                                                values=tuple(self.valid_attn_sub1g_output_power))
+                    window['higherPower'].update(values=tuple(self.valid_attn_sub1g_output_power),
+                                                 value=self.valid_attn_sub1g_output_power[-1])
+                else:
+                    window['lowerPower'].update(values=tuple(self.valid_sub1g_output_power),
+                                                value=self.valid_sub1g_output_power[0])
+                    window['higherPower'].update(values=tuple(self.valid_sub1g_output_power),
+                                                 value=self.valid_sub1g_output_power[-1])
 
             if event == '2.4mode':
                 self.sub1g_enable = False
                 window['2.4mode'].update(button_color=('white', '#158225'))
                 window['sub1gmode'].update(button_color=('white', '#821515'))
-                window['power'].update(values=tuple(self.abs_power_list),
-                                       value=self.abs_power_list[0])
-                window['start_freq'].update(value='2402')
-                window['stop_freq'].update(value='2480')
-                # if self.attn_enable:
-                #     window['lowerPower'].update(value=self.abs_att_power_list[0],
-                #                                 values=tuple(self.abs_att_power_list))
-                #     window['higherPower'].update(values=tuple(self.abs_att_power_list),
-                #                                  value=self.abs_att_power_list[-1])
-                # else:
-                #     window['lowerPower'].update(values=tuple(self.abs_power_list),
-                #                                 value=self.abs_power_list[0])
-                #     window['higherPower'].update(values=tuple(self.abs_power_list),
-                #                                  value=self.abs_power_list[-1])
+                if self.attn_enable:
+                    window['lowerPower'].update(value=self.abs_att_power_list[0],
+                                                values=tuple(self.abs_att_power_list))
+                    window['higherPower'].update(values=tuple(self.abs_att_power_list),
+                                                 value=self.abs_att_power_list[-1])
+                else:
+                    window['lowerPower'].update(values=tuple(self.abs_power_list),
+                                                value=self.abs_power_list[0])
+                    window['higherPower'].update(values=tuple(self.abs_power_list),
+                                                 value=self.abs_power_list[-1])
 
             if event == 'attn':
                 self.attn_enable = not self.attn_enable
                 if self.attn_enable:
                     window['-ATTN-'].update('Attenuator Enabled', text_color='Dark Green')
                     window['attn'].update('Disable Attenuator', button_color=('white', '#821515'))
-                    window['attntype'].update(visible=True)
-                    window['attntypeen'].update(visible=True)
-                    window['attnval'].update(visible=True)
-                    window['attnvalen'].update(visible=True)
-                    # if self.sub1g_enable:
-                    #     window['lowerPower'].update(value=self.valid_attn_sub1g_output_power[0],
-                    #                                 values=tuple(self.valid_attn_sub1g_output_power))
-                    #     window['higherPower'].update(values=tuple(self.valid_attn_sub1g_output_power),
-                    #                                  value=self.valid_attn_sub1g_output_power[-1])
-                    # else:
-                    #     window['lowerPower'].update(value=self.abs_att_power_list[0],
-                    #                                 values=tuple(self.abs_att_power_list))
-                    #     window['higherPower'].update(values=tuple(self.abs_att_power_list),
-                    #                                  value=self.abs_att_power_list[-1])
+                    if self.sub1g_enable:
+                        window['lowerPower'].update(value=self.valid_attn_sub1g_output_power[0],
+                                                    values=tuple(self.valid_attn_sub1g_output_power))
+                        window['higherPower'].update(values=tuple(self.valid_attn_sub1g_output_power),
+                                                     value=self.valid_attn_sub1g_output_power[-1])
+                    else:
+                        window['lowerPower'].update(value=self.abs_att_power_list[0],
+                                                    values=tuple(self.abs_att_power_list))
+                        window['higherPower'].update(values=tuple(self.abs_att_power_list),
+                                                     value=self.abs_att_power_list[-1])
 
                 else:
                     window['-ATTN-'].update('Attenuator Disabled', text_color='Dark Red')
                     window['attn'].update('Enable Attenuator', button_color=('white', '#158225'))
-                    window['attntype'].update(visible=False)
-                    window['attntypeen'].update(visible=False)
-                    window['attnval'].update(visible=False)
-                    window['attnvalen'].update(visible=False)
-                    # if self.sub1g_enable:
-                    #     window['lowerPower'].update(values=tuple(self.valid_sub1g_output_power),
-                    #                                 value=self.valid_sub1g_output_power[0])
-                    #     window['higherPower'].update(values=tuple(self.valid_sub1g_output_power),
-                    #                                  value=self.valid_sub1g_output_power[-1])
-                    # else:
-                    #     window['lowerPower'].update(values=tuple(self.abs_power_list),
-                    #                                 value=self.abs_power_list[0])
-                    #     window['higherPower'].update(values=tuple(self.abs_power_list),
-                    #                                  value=self.abs_power_list[-1])
+                    if self.sub1g_enable:
+                        window['lowerPower'].update(values=tuple(self.valid_sub1g_output_power),
+                                                    value=self.valid_sub1g_output_power[0])
+                        window['higherPower'].update(values=tuple(self.valid_sub1g_output_power),
+                                                     value=self.valid_sub1g_output_power[-1])
+                    else:
+                        window['lowerPower'].update(values=tuple(self.abs_power_list),
+                                                    value=self.abs_power_list[0])
+                        window['higherPower'].update(values=tuple(self.abs_power_list),
+                                                     value=self.abs_power_list[-1])
 
             if event == SimGUI.WINDOW_CLOSED or event is None:
                 print('User exited program')
                 sys.exit(0)
             if event == 'Submit':
                 if ' ' in values['testName'] or '/' in values['testName'] or '\\' in values['testName'] or values[
                     'testName'] == '':
                     window['-OUTPUT-'].update('Please enter valid run name without / or spaces')
                     continue
                 else:
                     try:
-                        # requestedTBP = int(values['requestedTBP'])
+                        requestedTBP = int(values['requestedTBP'])
                         onTime = int(values['onTime'])
                         totalTime = int(values['totalTime'])
-                        start_f = int(values['start_freq'])
-                        stop_f = int(values['stop_freq'])
-                        step_f = int(values['step'])
                         self.min_tags_answering = int(values['tagsNum'])
-                        start_index = self.bb_list.index(values['lowerBB'])
-                        end_index = self.bb_list.index(values['higherBB'])
-                        direction = -1 if start_index > end_index else 1
-                        self.new_bb_list = self.bb_list[start_index:end_index + direction:direction]
-                        if self.sub1g_enable:
-                            if start_f not in range(849, 941) or stop_f not in range(849, 941):
-                                window['-OUTPUT-'].update(
-                                    'Please enter valid Frequency range for Sub1G')
-                                continue
-                        else:
-                            if start_f not in range(2400, 2490) or stop_f not in range(2400, 2490):
-                                window['-OUTPUT-'].update(
-                                    'Please enter valid Frequency range for 2.4GHz')
-                                continue
                         break
                     except Exception:
-                        window['-OUTPUT-'].update('Please enter valid Time Profile/ Test Time / Frequency values')
+                        window['-OUTPUT-'].update('Please enter valid TBP/ Time Profile/ Test Time values')
                         continue
 
         window.close()
         return values
 
     def packet_filter(self, packet_list, filter_param='rssi', param_limits=None):
         """
@@ -488,33 +439,35 @@
     def init_timer(self):
         self.timeout = False
         self.success = False
         self.clean_gw()
         self.timer = threading.Timer(int(self.gui_values['testTime']), self.time_expire)
 
     def start_analyze(self, power=None, freq=None, bb=None):
+
+        def update_custom_data(packet_list, key, value):
+            if key in packet_list.list_custom_data.keys():
+                packet_list.list_custom_data[key].append(value)
+            else:
+                packet_list.list_custom_data[key] = [value]
+
         tbp = None
         for tag_adva in self.all_tags.tags:
             if self.is_gw_fetal_error(self.all_tags.tags[tag_adva]):
                 self.my_logger.gw_logger.warning('gw fetal error was detected')
                 self.gw_reset_and_config()
             for packet in self.all_tags.tags[tag_adva].packet_list:
                 self.all_tests.append(packet)
             try:
                 tbp = self.all_tags.get_avg_tbp_by_id(tag_adva)
                 packets_sum = self.all_tags.get_statistics_by_id(tag_adva)['num_packets']
             except Exception as e:
-                self.my_logger.logger.info(
-                    'Exception receiving TBP or Packets num on tag {}, exception {}'.format(tag_adva, e))
+                self.my_logger.logger.info('Exception receiving TBP or Packets num on tag {}, exception {}'.format(tag_adva, e))
                 tbp = None
-            new_row = {'Adva': tag_adva, 'Frequency': freq, 'TBP': tbp, 'BB': bb}
-            new_df = pd.DataFrame(new_row, index=[0])
-            self.all_results = pd.concat([self.all_results, new_df], ignore_index=True)
-            details = {'Test Num': self.test_num, 'BB': bb, 'Frequency': freq, 'Power': power, 'Packets': packets_sum,
-                       'TBP': tbp}
+            details = {'Test Num': self.test_num, 'BB': bb, 'Frequency': freq, 'Power': power, 'Packets': packets_sum, 'TBP': tbp}
             if self.all_tests.tags[tag_adva].list_custom_data.__len__() == 0:
                 self.all_tests.tags[tag_adva].list_custom_data['Data'] = []
             self.all_tests.tags[tag_adva].list_custom_data['Data'].append(details)
 
     def get_packets(self, filter_param='rssi', filter_value=100, power=None, freq=None, bb=None):
         """
         receive packets from the gw (via the listener) and filter them according to packet_filter()
@@ -532,22 +485,23 @@
             packets_received_list = self.gw_obj.get_packets(action_type=ActionType.ALL_SAMPLE,
                                                             data_type=DataType.PACKET_LIST)
         if packets_received_list:
             for packet in packets_received_list:
                 packet_param_list = int(packet.get_average_rssi())
                 if filter_value >= packet_param_list:
                     self.my_logger.logger.info('got packet {}'.format(packet.packet_data['raw_packet']))
-                    self.all_tags.append(packet=packet.copy())
                 else:
                     self.my_logger.logger.info(
                         'got packet {} but with high rssi {}'.format(packet.packet_data['raw_packet'],
                                                                      packet_param_list))
                     continue
 
-                if self.all_tags.tags.__len__() > 0:  # self.num_of_chambers:  # If we got more then X chamber tags and at least X chambers * 4 packets for each tag
+                self.all_tags.append(packet=packet.copy())
+
+                if self.all_tags.tags.__len__() > 0: #self.num_of_chambers:  # If we got more then X chamber tags and at least X chambers * 4 packets for each tag
                     for packet_list in self.all_tags.tags:
                         try:
                             avg_tbp = self.all_tags.tags[packet_list].get_avg_tbp()
                             if avg_tbp > 0:
                                 self.num_good_tags += 1
                         except Exception:
                             pass
@@ -556,21 +510,22 @@
                             self.success = True
                         else:
                             continue
                 if self.success:
                     self.my_logger.logger.info(
                         'Found {} tags\n{} tags TBP was calculated\n{} tags TBP wasnt calculated\nStarting analyzing'.format(
                             self.all_tags.tags.__len__(), self.num_good_tags, self.num_bad_tags))
+
                     break
 
         if self.success:
             self.timer.cancel()
             self.gw_obj.stop_gw_app()
-            self.clean_gw()
             self.gw_obj.stop_continuous_listener()
+            self.clean_gw()
             self.start_analyze(power, freq, bb)
 
     def is_gw_fetal_error(self, packet_list):
         """
         check if the gw reset itself for some reason
         :param packet_list: the received packets list
         :type packet_list: PacketList
@@ -595,70 +550,88 @@
     def get_result(self):
         return self.all_tests
 
     def time_expire(self):
         self.timeout = True
         self.timer.cancel()
         # self.gw_obj.stop_gw_app()
-        self.my_logger.results_logger.info(
-            'Timeout - found {} tags but didnt received enough packets to calculate TBP for all, calculated only for {} tags'.format(
-                self.all_tags.tags.__len__(), self.num_good_tags))
+        self.my_logger.results_logger.info('Timeout - found {} tags but didnt received enough packets to calculate TBP for all, calculated only for {} tags'.format(self.all_tags.tags.__len__(),self.num_good_tags))
 
     def gw_reset_and_config(self):
         self.gw_obj.reset_gw()
         time.sleep(2)
         self.gw_obj.write('!set_tester_mode 1', with_ack=True)
         self.gw_obj.write('!enable_brg_mgmt 0', with_ack=True)
         self.gw_obj.write('!listen_to_tag_only 1', with_ack=True)
         self.gw_obj.write('!energizing_prob_set 100', with_ack=True)
 
     def clean_gw(self):
-        self.gw_obj.reset_buffer()
         self.gw_obj.reset_listener()
 
-    def data_read_analyze(self, dict=None):
+    def data_read_analyze(self, dict = None):
+        self.analyzed_dict = {}
+        min_tbp = int(self.gui_values['requestedTBP'])
+        power = ''
+        for freq in self.frequency_range:
+            if not self.analyzed_dict:
+                self.analyzed_dict['Default'] = {freq: {min_tbp:power}}
+            else:
+                self.analyzed_dict['Default'][freq] = {min_tbp:power}
 
-        # Get unique BB values
-        self.all_results = self.all_results.dropna(subset=['TBP'])
+        self.analyzed_data = {'Frequency': '', 'TBP': '', 'Power': ''}
+        data = pd.read_csv(self.test_csv_path)
+        data.set_index(x for x in data['Adva'])
+        for index in data.index:
+            row = data.iloc[index]
+            if row['Adva'] in self.analyzed_dict.keys():
+                if row['Frequency'] in self.analyzed_dict[row['Adva']].keys():
+                    if abs(min_tbp - int(list(self.analyzed_dict[row['Adva']][row['Frequency']])[0])) < abs(min_tbp - int(row['TBP'])) or int(row['TBP']) < 1 or int(row['TBP']) > 1000:
+                        continue
+                self.analyzed_dict[row['Adva']][row['Frequency']] = {row['TBP']: row['Power']}
+            else:
+                if int(row['TBP']) < 1 or int(row['TBP']) > 1000:
+                    continue
+                self.analyzed_dict[row['Adva']] = {row['Frequency']:{row['TBP']: row['Power']}}
 
-        unique_bbs = self.all_results['BB'].unique()
 
-        # Set up subplots
-        fig, axes = plt.subplots(nrows=1, ncols=unique_bbs.size, figsize=(10, 4))
-
-        # Loop over unique BB values and plot graphs
-        for i, bb in enumerate(unique_bbs):
-            # Get data for current BB value
-            bb_df = self.all_results[self.all_results['BB'] == bb]
-            # Get unique Adva names for current BB value
-            unique_adv = bb_df['Adva'].unique()
-
-            # Plot graph for current BB value on the appropriate subplot
-            ax = axes[i]
-            ax.set_title(f"Beacon Backoff = {bb}")
-            freq_ticks = sorted(self.all_results['Frequency'].unique())
-            ax.set_xticks(self.x_grid, rotation=90)
-            ax.set_xlabel("Frequency")
-            ax.set_ylabel("TBP")
-            for adv in unique_adv:
-                adv_df = bb_df[bb_df['Adva'] == adv]
-                ax.plot(adv_df['Frequency'], adv_df['TBP'], label=adv)
-            ax.legend()
 
-        # Show the plot
+        # for adva in self.analyzed_dict.keys():
+        #     for freq in self.frequency_range:
+        #         if freq not in self.analyzed_dict[adva].keys():
+        #             self.analyzed_dict[adva][freq] = {0 : 0}
+
+        for val in self.analyzed_dict.keys():
+            print('Adva: ' + val)
+            for freq in self.analyzed_dict[val].keys():
+                try:
+                    tbp = list(self.analyzed_dict[val][freq])[0]
+                    print('Frequency {} : TBP {} : Power {}'.format(freq, tbp, self.analyzed_dict[val][freq][tbp]))
+                except Exception:
+                    print('Issue')
+
+        for adva in self.analyzed_dict.keys():
+            new_dict = collections.OrderedDict(sorted(self.analyzed_dict[adva].items()))
+            (keys, values_dict) = zip(*new_dict.items())
+            values = tuple([list(k)[0] for k in values_dict])
+            if any(values):
+                plt.plot(keys, values,'o-', label=adva)
+
+        # naming the x axis
+        plt.xlabel('Frequency')
+        # naming the y axis
+        plt.ylabel('TBP')
+        # giving a title to my graph
+        plt.title('Harvester Test')
+        # show a legend on the plot
+        plt.legend()
+        # function to show the plot
         plt.show()
 
     def finish(self):
         # Start writing all data to file
-        self.all_results = self.all_results.groupby('Adva').apply(
-            lambda x: x.sort_values(by=['Frequency', 'BB'], ascending=[True, False])).reset_index(drop=True)
-
-        self.my_logger.results_logger.info(self.all_results)
-        for i in self.all_results:
-            self.my_logger.results_logger.info(i)
         self.all_packet_list = self.all_tests.to_packet_list()
         all_data = []
         custom_data = {'Test Num': '', 'Adva': '', 'BeaconBackoff': '', 'Frequency': '', 'Power': '', 'Packets': '',
                        'TBP': ''}
         for packet_list in self.all_tests.tags:
             for custom in self.all_tests.tags[packet_list].list_custom_data['Data']:
                 p_list_data = {'Test Num': '', 'Adva': '', 'BeaconBackoff': '', 'Frequency': '', 'Power': '',
@@ -683,146 +656,151 @@
         try:
             self.all_tests.to_csv(path=self.packets_csv_path, val='adv_address')
         except Exception:
             self.my_logger.logger.warning('Empty list')
         # Read data from file organized with pandas
 
         # Draw graphs according to post process correlated to TBP requested
-        if len(self.frequency_range) > 8:
-            self.x_grid = self.frequency_range[::3]
-            if len(self.frequency_range) > 15:
-                self.x_grid = self.frequency_range[::4]
-                if len(self.frequency_range) > 28:
-                    self.x_grid = self.frequency_range[::5]
-        else:
-            self.x_grid = self.frequency_range
+        self.x_grid = self.frequency_range
         self.data_read_analyze()
+
+        self.my_logger.logger.info('Results: {}'.format(self.results))
         # The End
         self.my_logger.logger.info('Finished')
 
     def config_gw(self, power, freq, bb):
         if not self.sub1g_enable:
             # ---------------------------------------------------------------------------------------------------------------------
             # 2.4 + Attenuator
             if self.attn_enable:
-                # abs_power_val, abs_attn_val = self.convert_power(power, sub1g=False)
-                # for list_power_val in self.valid_output_power_vals:
-                #     if abs_power_val == list_power_val['abs_power']:
-                #         gw_out_power = list_power_val['gw_output_power']
+                abs_power_val, abs_attn_val = self.convert_power(power, sub1g=False)
+                for list_power_val in self.valid_output_power_vals:
+                    if abs_power_val == list_power_val['abs_power']:
+                        gw_out_power = list_power_val['gw_output_power']
                 self.my_logger.logger.info(
-                    'Setting GW power: {}, Attenuation value: {} Frequency {} Beacaon Backoff val {}'.format(
-                        power, self.attnval, freq, bb))
-                self.attn_obj.Setattn(self.attnval)
+                    'Setting GW power: {}, Attenuation value: {} Frequency {} Becaon Backoff val {}'.format(
+                        power, abs_attn_val, freq, bb))
+                self.attn_obj.Setattn(abs_attn_val)
                 self.gw_obj.config_gw(energy_pattern_val=18,
                                       time_profile_val=[self.gui_values['onTime'],
                                                         self.gui_values['totalTime']],
                                       beacons_backoff_val=bb,
                                       received_channel='37',
-                                      effective_output_power_val=int(power),
+                                      output_power_val=gw_out_power,
                                       start_gw_app=True,
                                       with_ack=True)
             # ---------------------------------------------------------------------------------------------------------------------
             # 2.4 + No Attenuator
             else:
-                # abs_power_val, abs_attn_val = self.convert_power(power, sub1g=False)
-                # if int(abs_power_val) > 5:
-                #     bypass_pa_val = 0
-                # else:
-                #     bypass_pa_val = 1
-                # for list_power_val in self.valid_output_power_vals:
-                #     if abs_power_val == int(list_power_val['abs_power']):
-                #         gw_out_power = list_power_val['gw_output_power']
+                abs_power_val, abs_attn_val = self.convert_power(power, sub1g=False)
+                if int(abs_power_val) > 5:
+                    bypass_pa_val = 0
+                else:
+                    bypass_pa_val = 1
+                for list_power_val in self.valid_output_power_vals:
+                    if abs_power_val == int(list_power_val['abs_power']):
+                        gw_out_power = list_power_val['gw_output_power']
                 self.my_logger.logger.info(
-                    'Setting GW power: {}, No attenuation Frequency {} Beacaon Backoff val {}'.format(
+                    'Setting GW power: {}, No attenuation Frequency {} Becaon Backoff val {}'.format(
                         power, freq, bb))
                 self.gw_obj.config_gw(energy_pattern_val=18,
                                       time_profile_val=[self.gui_values['onTime'],
                                                         self.gui_values['totalTime']],
                                       beacons_backoff_val=bb,
                                       received_channel='37',
-                                      effective_output_power_val=int(power),
+                                      bypass_pa_val = bypass_pa_val,
+                                      output_power_val=gw_out_power,
                                       start_gw_app=True,
                                       with_ack=True)
         # ---------------------------------------------------------------------------------------------------------------------
         # Sub1G
         else:
             # ---------------------------------------------------------------------------------------------------------------------
             # Sub1G + Attenuator
             if self.attn_enable:
-                # abs_power_val, abs_attn_val = self.convert_power(power, sub1g=True)
+                abs_power_val, abs_attn_val = self.convert_power(power, sub1g=True)
                 self.my_logger.logger.info(
-                    'Setting Sub1G GW power: {}, Attenuation value: {} Frequency {} Beacaon Backoff val {}'.format(
-                        power, self.attnval, freq, bb))
-                self.attn_obj.Setattn(self.attnval)
+                    'Setting Sub1G GW power: {}, Attenuation value: {} Frequency {} Becaon Backoff val {}'.format(
+                        power, abs_attn_val, freq, bb))
+                self.attn_obj.Setattn(abs_attn_val)
                 self.gw_obj.config_gw(energy_pattern_val=50,
                                       time_profile_val=[self.gui_values['onTime'],
                                                         self.gui_values['totalTime']],
                                       beacons_backoff_val=bb,
                                       received_channel='37',
-                                      effective_output_power_val=22,
-                                      sub1g_output_power_val=power,
+                                      sub1g_output_power_val=abs_power_val,
                                       start_gw_app=True,
                                       with_ack=True)
             # ---------------------------------------------------------------------------------------------------------------------
             # Sub1G + No Attenuator
             else:
-                # abs_power_val, abs_attn_val = self.convert_power(power, sub1g=True)
+                abs_power_val, abs_attn_val = self.convert_power(power, sub1g=True)
                 self.my_logger.logger.info(
-                    'Setting Sub1G GW power: {}, No attenuation value Frequency {} Beacaon Backoff val {}'.format(
+                    'Setting Sub1G GW power: {}, No attenuation value Frequency {} Becaon Backoff val {}'.format(
                         power, freq, bb))
+                self.attn_obj.Setattn(abs_attn_val)
                 self.gw_obj.config_gw(energy_pattern_val=50,
                                       time_profile_val=[self.gui_values['onTime'],
                                                         self.gui_values['totalTime']],
                                       beacons_backoff_val=bb,
                                       received_channel='37',
-                                      effective_output_power_val=22,
-                                      sub1g_output_power_val=power,
+                                      sub1g_output_power_val=abs_power_val,
                                       start_gw_app=True,
                                       with_ack=True)
         # ---------------------------------------------------------------------------------------------------------------------
         if self.sub1g_enable:
             self.gw_obj.write('!set_dyn_energizing_pattern 6 1 0 0', with_ack=True)
             self.gw_obj.write('!set_beacons_pattern 550 3 2402 2426 2480', with_ack=True)
-            self.gw_obj.write('!set_sub_1_ghz_energizing_frequency {}'.format(freq), with_ack=True)
-
         else:
             self.gw_obj.write('!set_dyn_energizing_pattern 6 0 1 {}'.format(freq), with_ack=True)
             self.gw_obj.write('!set_beacons_pattern 550 3 2402 2426 2480', with_ack=True)
 
     def scan(self):
         self.all_tests = TagCollection()
         self.test_num = 0
         self.results = []
         # Scan power
-        power = self.power
-        self.my_logger.logger.info('Sweeping freq {}'.format(self.frequency_range))
-        # Scan frequency
-        for freq in self.frequency_range:
-            # Scan beacon backoff
-            for index, bb in enumerate(self.new_bb_list):
-                self.test_num += 1
-                # 2.4Ghz
-                self.all_tags = TagCollection()
-                self.gw_obj.start_continuous_listener()
-                self.init_timer()  # Init timeout flag and reset success flag
-                self.timer.start()  # Start timer thread
-                self.my_logger.results_logger.info(
-                    '-' * 30 + 'New Test - Power {} Frequency {} Beacon Backoff {}'.format(power, freq,
-                                                                                           bb) + '-' * 30)
-
-                self.config_gw(power=power, freq=freq, bb=bb)
-
-                # Start receiving packets
-                while not self.timeout and not self.success:  # While function to work until timeout or success test
-                    time.sleep(0.01)
-                    self.get_packets(power=power, freq=freq,
-                                     bb=bb)  # Will start to get packets, then analyze them and add to self.all_tests with custom data of which test it came from
+        for power in self.power_range:
+            self.bb_list = [12, 7, 2, 0]
+            # Scan frequency
+            for freq in self.frequency_range:
+                # Scan beacon backoff
+                for index,bb in enumerate(self.bb_list):
+                    self.test_num +=1
+                    # 2.4Ghz
+                    self.all_tags = TagCollection()
+                    self.gw_obj.start_continuous_listener()
+                    self.init_timer()  # Init timeout flag and reset success flag
+                    self.timer.start()  # Start timer thread
+                    self.my_logger.results_logger.info(
+                        '-' * 30 + 'New test power {} frequency {} beacon backoff {}'.format(power, freq,
+                                                                                             bb) + '-' * 30)
+
+                    self.config_gw(power = power, freq=freq, bb=bb)
+
+                    # Start receiving packets
+                    while not self.timeout and not self.success:  # While function to work until timeout or success test
+                        time.sleep(0.01)
+                        self.get_packets(power=power, freq=freq,
+                                         bb=bb)  # Will start to get packets, then analyze them and add to self.all_tests with custom data of which test it came from
+
+                    if self.success:
+                        if len(self.bb_list) > 1:
+                            try:
+                                temp = self.bb_list[index + 1]
+                            except IndexError:
+                                temp = self.bb_list[index]
+                            self.results.append({'Power': power, 'BB':temp})
+                            self.bb_list.clear()
+                            self.bb_list.append(temp)
+                            self.my_logger.results_logger.info('Beacon Backoff value selected the value: {}'.format(self.bb_list[0]))
+
+                        self.success = False
 
-                self.clean_gw()  # clear the buffers
-                time.sleep(0.5)
+                    self.clean_gw()  # clear the buffers
 
         self.gw_obj.close_port(is_reset=True)
         self.gw_obj.stop_continuous_listener()
         self.finish()
 
 
 if __name__ == '__main__':
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/system_test/system_test_example.py` & `wiliot-testers-4.0.6/wiliot_testers/system_test/system_test_example.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/test_equipment.py` & `wiliot-testers-4.0.6/wiliot_testers/test_equipment.py`

 * *Files 23% similar despite different names*

```diff
@@ -236,2234 +236,1718 @@
 00000eb0: 4d41 4745 532c 204c 4f53 5345 532c 204f  MAGES, LOSSES, O
 00000ec0: 5220 434f 5354 533b 2041 4e44 0a20 2020  R COSTS; AND.   
 00000ed0: 2843 2920 4556 454e 2049 4620 414e 5920  (C) EVEN IF ANY 
 00000ee0: 5245 4d45 4459 2046 4149 4c53 204f 4620  REMEDY FAILS OF 
 00000ef0: 4954 5320 4553 5345 4e54 4941 4c20 5055  ITS ESSENTIAL PU
 00000f00: 5250 4f53 452e 0a22 2222 0a66 726f 6d20  RPOSE..""".from 
 00000f10: 7469 6d65 2069 6d70 6f72 7420 7469 6d65  time import time
-00000f20: 2c20 736c 6565 702c 2070 6572 665f 636f  , sleep, perf_co
-00000f30: 756e 7465 725f 6e73 0a66 726f 6d20 7374  unter_ns.from st
-00000f40: 6174 6973 7469 6373 2069 6d70 6f72 7420  atistics import 
-00000f50: 6d6f 6465 0a69 6d70 6f72 7420 6c6f 6767  mode.import logg
-00000f60: 696e 670a 696d 706f 7274 2073 7973 0a69  ing.import sys.i
-00000f70: 6d70 6f72 7420 7365 7269 616c 0a69 6d70  mport serial.imp
-00000f80: 6f72 7420 7365 7269 616c 2e74 6f6f 6c73  ort serial.tools
-00000f90: 2e6c 6973 745f 706f 7274 730a 6672 6f6d  .list_ports.from
-00000fa0: 2079 6f63 746f 7075 6365 2e79 6f63 746f   yoctopuce.yocto
-00000fb0: 5f74 656d 7065 7261 7475 7265 2069 6d70  _temperature imp
-00000fc0: 6f72 7420 5941 5049 2c20 5952 6566 5061  ort YAPI, YRefPa
-00000fd0: 7261 6d2c 2059 5465 6d70 6572 6174 7572  ram, YTemperatur
-00000fe0: 650a 696d 706f 7274 206f 730a 6672 6f6d  e.import os.from
-00000ff0: 2064 6174 6574 696d 6520 696d 706f 7274   datetime import
-00001000: 2064 6174 6574 696d 650a 6672 6f6d 2077   datetime.from w
-00001010: 696c 696f 745f 636f 7265 2069 6d70 6f72  iliot_core impor
-00001020: 7420 5769 6c69 6f74 4469 720a 0a63 6c61  t WiliotDir..cla
-00001030: 7373 2045 7175 6970 6d65 6e74 4572 726f  ss EquipmentErro
-00001040: 7228 4578 6365 7074 696f 6e29 3a0a 0a20  r(Exception):.. 
-00001050: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00001060: 7365 6c66 2c20 2a61 7267 7329 3a0a 2020  self, *args):.  
-00001070: 2020 2020 2020 6966 2061 7267 733a 0a20        if args:. 
-00001080: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001090: 6d65 7373 6167 6520 3d20 6172 6773 5b30  message = args[0
-000010a0: 5d0a 2020 2020 2020 2020 656c 7365 3a0a  ].        else:.
-000010b0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000010c0: 2e6d 6573 7361 6765 203d 204e 6f6e 650a  .message = None.
-000010d0: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
-000010e0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000010f0: 2320 7072 696e 7428 2763 616c 6c69 6e67  # print('calling
-00001100: 2073 7472 2729 0a20 2020 2020 2020 2069   str').        i
-00001110: 6620 7365 6c66 2e6d 6573 7361 6765 3a0a  f self.message:.
-00001120: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001130: 726e 2027 4571 7569 706d 656e 7445 7272  rn 'EquipmentErr
-00001140: 6f72 3a20 7b6d 7367 7d27 2e66 6f72 6d61  or: {msg}'.forma
-00001150: 7428 6d73 673d 7365 6c66 2e6d 6573 7361  t(msg=self.messa
-00001160: 6765 290a 2020 2020 2020 2020 656c 7365  ge).        else
-00001170: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00001180: 7475 726e 2027 4571 7569 706d 656e 7445  turn 'EquipmentE
-00001190: 7272 6f72 2068 6173 2062 6565 6e20 7261  rror has been ra
-000011a0: 6973 6564 270a 0a0a 6465 6620 7365 7269  ised'...def seri
-000011b0: 616c 5f70 6f72 7473 2829 3a0a 2020 2020  al_ports():.    
-000011c0: 2222 2220 4c69 7374 7320 7365 7269 616c  """ Lists serial
-000011d0: 2070 6f72 7420 6e61 6d65 730a 0a20 2020   port names..   
-000011e0: 2020 2020 203a 7261 6973 6573 2045 6e76       :raises Env
-000011f0: 6972 6f6e 6d65 6e74 4572 726f 723a 0a20  ironmentError:. 
-00001200: 2020 2020 2020 2020 2020 204f 6e20 756e             On un
-00001210: 7375 7070 6f72 7465 6420 6f72 2075 6e6b  supported or unk
-00001220: 6e6f 776e 2070 6c61 7466 6f72 6d73 0a20  nown platforms. 
-00001230: 2020 2020 2020 203a 7265 7475 726e 733a         :returns:
-00001240: 0a20 2020 2020 2020 2020 2020 2041 206c  .            A l
-00001250: 6973 7420 6f66 2074 6865 2073 6572 6961  ist of the seria
-00001260: 6c20 706f 7274 7320 6176 6169 6c61 626c  l ports availabl
-00001270: 6520 6f6e 2074 6865 2073 7973 7465 6d0a  e on the system.
-00001280: 2020 2020 2222 220a 2020 2020 6176 6169      """.    avai
-00001290: 6c61 626c 655f 706f 7274 7320 3d20 5b73  lable_ports = [s
-000012a0: 2e64 6576 6963 6520 666f 7220 7320 696e  .device for s in
-000012b0: 2073 6572 6961 6c2e 746f 6f6c 732e 6c69   serial.tools.li
-000012c0: 7374 5f70 6f72 7473 2e63 6f6d 706f 7274  st_ports.comport
-000012d0: 7328 295d 0a20 2020 2069 6620 6c65 6e28  s()].    if len(
-000012e0: 6176 6169 6c61 626c 655f 706f 7274 7329  available_ports)
-000012f0: 203d 3d20 303a 0a20 2020 2020 2020 2061   == 0:.        a
-00001300: 7661 696c 6162 6c65 5f70 6f72 7473 203d  vailable_ports =
-00001310: 205b 732e 6e61 6d65 2066 6f72 2073 2069   [s.name for s i
-00001320: 6e20 7365 7269 616c 2e74 6f6f 6c73 2e6c  n serial.tools.l
-00001330: 6973 745f 706f 7274 732e 636f 6d70 6f72  ist_ports.compor
-00001340: 7473 2829 5d0a 2020 2020 2020 2020 6966  ts()].        if
-00001350: 206c 656e 2861 7661 696c 6162 6c65 5f70   len(available_p
-00001360: 6f72 7473 2920 3d3d 2030 3a0a 2020 2020  orts) == 0:.    
-00001370: 2020 2020 2020 2020 7072 696e 7428 226e          print("n
-00001380: 6f20 7365 7269 616c 2070 6f72 7473 2077  o serial ports w
-00001390: 6572 6520 666f 756e 642e 2070 6c65 6173  ere found. pleas
-000013a0: 6520 6368 6563 6b20 796f 7572 2063 6f6e  e check your con
-000013b0: 6e65 6374 696f 6e73 2229 0a20 2020 2072  nections").    r
-000013c0: 6574 7572 6e20 6176 6169 6c61 626c 655f  eturn available_
-000013d0: 706f 7274 730a 0a0a 636c 6173 7320 4174  ports...class At
-000013e0: 7465 6e75 6174 6f72 286f 626a 6563 7429  tenuator(object)
-000013f0: 3a0a 2020 2020 2727 270a 2020 2020 5375  :.    '''.    Su
-00001400: 7070 6f72 7420 616c 6c20 6174 746e 2063  pport all attn c
-00001410: 6c61 7373 6573 2066 6f72 3a0a 2020 2020  lasses for:.    
-00001420: 2727 270a 0a20 2020 2064 6566 205f 5f69  '''..    def __i
-00001430: 6e69 745f 5f28 7365 6c66 2c20 4154 544e  nit__(self, ATTN
-00001440: 5f74 7970 652c 2063 6f6d 706f 7274 3d27  _type, comport='
-00001450: 4155 544f 2729 3a0a 2020 2020 2020 2020  AUTO'):.        
-00001460: 6966 2027 4d43 4449 2d55 5342 2720 696e  if 'MCDI-USB' in
-00001470: 2041 5454 4e5f 7479 7065 3a0a 2020 2020   ATTN_type:.    
-00001480: 2020 2020 2020 2020 7365 6c66 2e5f 6163          self._ac
-00001490: 7469 7665 5f54 4520 3d20 4174 7465 6e75  tive_TE = Attenu
-000014a0: 6174 6f72 2e4d 4344 495f 5553 4228 290a  ator.MCDI_USB().
-000014b0: 2020 2020 2020 2020 656c 6966 2027 4d43          elif 'MC
-000014c0: 4449 2720 696e 2041 5454 4e5f 7479 7065  DI' in ATTN_type
-000014d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000014e0: 6c66 2e5f 6163 7469 7665 5f54 4520 3d20  lf._active_TE = 
-000014f0: 4174 7465 6e75 6174 6f72 2e4d 4344 4928  Attenuator.MCDI(
-00001500: 290a 2020 2020 2020 2020 656c 6966 2027  ).        elif '
-00001510: 4150 4927 2069 6e20 4154 544e 5f74 7970  API' in ATTN_typ
-00001520: 6520 6f72 2027 5765 696e 7363 6865 6c27  e or 'Weinschel'
-00001530: 2069 6e20 4154 544e 5f74 7970 653a 0a20   in ATTN_type:. 
-00001540: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001550: 5f61 6374 6976 655f 5445 203d 2041 7474  _active_TE = Att
-00001560: 656e 7561 746f 722e 4150 4928 636f 6d70  enuator.API(comp
-00001570: 6f72 7429 0a0a 2020 2020 2020 2020 656c  ort)..        el
-00001580: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00001590: 7061 7373 0a0a 2020 2020 6465 6620 4765  pass..    def Ge
-000015a0: 7441 6374 6976 6554 4528 7365 6c66 293a  tActiveTE(self):
-000015b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000015c0: 7365 6c66 2e5f 6163 7469 7665 5f54 450a  self._active_TE.
-000015d0: 0a20 2020 2063 6c61 7373 204d 4344 4928  .    class MCDI(
-000015e0: 6f62 6a65 6374 293a 0a0a 2020 2020 2020  object):..      
-000015f0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
-00001600: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
-00001610: 2020 646f 746e 6574 203d 2046 616c 7365    dotnet = False
-00001620: 0a20 2020 2020 2020 2020 2020 2075 7469  .            uti
-00001630: 6c73 5f64 6972 203d 206f 732e 7061 7468  ls_dir = os.path
-00001640: 2e6a 6f69 6e28 6f73 2e70 6174 682e 6469  .join(os.path.di
-00001650: 726e 616d 6528 5f5f 6669 6c65 5f5f 292c  rname(__file__),
-00001660: 2027 7574 696c 7327 290a 2020 2020 2020   'utils').      
-00001670: 2020 2020 2020 7379 732e 7061 7468 2e61        sys.path.a
-00001680: 7070 656e 6428 7574 696c 735f 6469 7229  ppend(utils_dir)
-00001690: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000016a0: 646f 746e 6574 203d 3d20 5472 7565 3a0a  dotnet == True:.
-000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016c0: 696d 706f 7274 2063 6c72 2020 2320 7079  import clr  # py
-000016d0: 7468 6f6e 6e65 742c 206d 616e 7561 6c6c  thonnet, manuall
-000016e0: 7920 696e 7374 616c 6c65 6420 7769 7468  y installed with
-000016f0: 2061 2064 6f77 6e6c 6f61 6465 6420 7768   a downloaded wh
-00001700: 6565 6c20 616e 6420 7069 700a 2020 2020  eel and pip.    
-00001710: 2020 2020 2020 2020 2020 2020 696d 706f              impo
-00001720: 7274 2063 7479 7065 7320 2023 206d 6f64  rt ctypes  # mod
-00001730: 756c 6520 746f 206f 7065 6e20 7574 696c  ule to open util
-00001740: 7320 6669 6c65 730a 2020 2020 2020 2020  s files.        
-00001750: 2020 2020 2020 2020 636c 722e 4164 6452          clr.AddR
-00001760: 6566 6572 656e 6365 2822 5379 7374 656d  eference("System
-00001770: 2e49 4f22 290a 2020 2020 2020 2020 2020  .IO").          
-00001780: 2020 2020 2020 696d 706f 7274 2053 7973        import Sys
-00001790: 7465 6d2e 494f 0a20 2020 2020 2020 2020  tem.IO.         
-000017a0: 2020 2020 2020 2053 7973 7465 6d2e 494f         System.IO
-000017b0: 2e44 6972 6563 746f 7279 2e53 6574 4375  .Directory.SetCu
-000017c0: 7272 656e 7444 6972 6563 746f 7279 2875  rrentDirectory(u
-000017d0: 7469 6c73 5f64 6972 290a 2020 2020 2020  tils_dir).      
-000017e0: 2020 2020 2020 2020 2020 636c 722e 4164            clr.Ad
-000017f0: 6452 6566 6572 656e 6365 2827 6d63 6c5f  dReference('mcl_
-00001800: 5255 4441 545f 4e45 5434 3527 290a 2020  RUDAT_NET45').  
-00001810: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-00001820: 6f6d 206d 636c 5f52 5544 4154 5f4e 4554  om mcl_RUDAT_NET
-00001830: 3435 2069 6d70 6f72 7420 5553 425f 5255  45 import USB_RU
-00001840: 4441 540a 2020 2020 2020 2020 2020 2020  DAT.            
-00001850: 2020 2020 7365 6c66 2e44 6576 6963 6520      self.Device 
-00001860: 3d20 5553 425f 5255 4441 5428 290a 2020  = USB_RUDAT().  
-00001870: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00001880: 6c66 2e44 6576 6963 652e 436f 6e6e 6563  lf.Device.Connec
-00001890: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-000018a0: 2020 2020 696e 666f 203d 2073 656c 662e      info = self.
-000018b0: 4465 7669 6365 496e 666f 2829 0a20 2020  DeviceInfo().   
-000018c0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000018d0: 6e74 2827 466f 756e 6420 4174 7465 6e75  nt('Found Attenu
-000018e0: 6174 6f72 3a20 4d6f 6465 6c20 7b7d 2c20  ator: Model {}, 
-000018f0: 7b7d 202c 7b7d 2027 2e66 6f72 6d61 7428  {} ,{} '.format(
-00001900: 696e 666f 5b30 5d2c 2069 6e66 6f5b 315d  info[0], info[1]
-00001910: 2c20 696e 666f 5b32 5d29 290a 2020 2020  , info[2])).    
-00001920: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00001930: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-00001940: 6f6d 2055 5342 5f52 5544 4154 2069 6d70  om USB_RUDAT imp
-00001950: 6f72 7420 5553 4244 4154 0a20 2020 2020  ort USBDAT.     
-00001960: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001970: 4465 7669 6365 203d 2055 5342 4441 5428  Device = USBDAT(
-00001980: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00001990: 2020 696e 666f 203d 2073 656c 662e 4465    info = self.De
-000019a0: 7669 6365 496e 666f 2829 0a20 2020 2020  viceInfo().     
-000019b0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-000019c0: 2827 466f 756e 6420 4174 7465 6e75 6174  ('Found Attenuat
-000019d0: 6f72 3a20 4d6f 6465 6c20 7b7d 2c20 7b7d  or: Model {}, {}
-000019e0: 202c 7b7d 2027 2e66 6f72 6d61 7428 696e   ,{} '.format(in
-000019f0: 666f 5b30 5d2c 2069 6e66 6f5b 315d 2c20  fo[0], info[1], 
-00001a00: 696e 666f 5b32 5d29 290a 0a20 2020 2020  info[2]))..     
-00001a10: 2020 2064 6566 2044 6576 6963 6549 6e66     def DeviceInf
-00001a20: 6f28 7365 6c66 293a 0a20 2020 2020 2020  o(self):.       
-00001a30: 2020 2020 2063 6d64 203d 2022 3a4d 4e3f       cmd = ":MN?
-00001a40: 220a 2020 2020 2020 2020 2020 2020 6d6f  ".            mo
-00001a50: 6465 6c5f 6e61 6d65 203d 2073 656c 662e  del_name = self.
-00001a60: 4465 7669 6365 2e53 656e 645f 5343 5049  Device.Send_SCPI
-00001a70: 2863 6d64 2c20 2222 290a 2020 2020 2020  (cmd, "").      
-00001a80: 2020 2020 2020 636d 6420 3d20 223a 534e        cmd = ":SN
-00001a90: 3f22 0a20 2020 2020 2020 2020 2020 2073  ?".            s
-00001aa0: 6572 6961 6c20 3d20 7365 6c66 2e44 6576  erial = self.Dev
-00001ab0: 6963 652e 5365 6e64 5f53 4350 4928 636d  ice.Send_SCPI(cm
-00001ac0: 642c 2022 2229 0a20 2020 2020 2020 2020  d, "").         
-00001ad0: 2020 2063 6d64 203d 2022 3a46 4952 4d57     cmd = ":FIRMW
-00001ae0: 4152 453f 220a 2020 2020 2020 2020 2020  ARE?".          
-00001af0: 2020 6677 203d 2073 656c 662e 4465 7669    fw = self.Devi
-00001b00: 6365 2e53 656e 645f 5343 5049 2863 6d64  ce.Send_SCPI(cmd
-00001b10: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-00001b20: 2020 2320 7265 7475 726e 205b 6d6f 6465    # return [mode
-00001b30: 6c5f 6e61 6d65 5b31 5d2c 2073 6572 6961  l_name[1], seria
-00001b40: 6c5b 315d 2c20 6677 5b31 5d5d 2020 2364  l[1], fw[1]]  #d
-00001b50: 6f74 6e65 740a 2020 2020 2020 2020 2020  otnet.          
-00001b60: 2020 7265 7475 726e 205b 6d6f 6465 6c5f    return [model_
-00001b70: 6e61 6d65 2c20 7365 7269 616c 2c20 6677  name, serial, fw
-00001b80: 5d0a 0a20 2020 2020 2020 2064 6566 2053  ]..        def S
-00001b90: 6574 6174 746e 2873 656c 662c 2061 7474  etattn(self, att
-00001ba0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-00001bb0: 636d 6420 3d20 223a 5345 5441 5454 3a22  cmd = ":SETATT:"
-00001bc0: 202b 2073 7472 2861 7474 6e29 0a20 2020   + str(attn).   
-00001bd0: 2020 2020 2020 2020 2073 7461 7475 7320           status 
-00001be0: 3d20 696e 7428 7365 6c66 2e44 6576 6963  = int(self.Devic
-00001bf0: 652e 5365 6e64 5f53 4350 4928 636d 642c  e.Send_SCPI(cmd,
-00001c00: 2022 2229 290a 2020 2020 2020 2020 2020   "")).          
-00001c10: 2020 6966 2073 7461 7475 7320 3d3d 2030    if status == 0
-00001c20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001c30: 2020 7072 696e 7428 2743 6f6d 6d61 6e64    print('Command
-00001c40: 2066 6169 6c65 6420 6f72 2069 6e76 616c   failed or inval
-00001c50: 6964 2061 7474 656e 7561 7469 6f6e 2073  id attenuation s
-00001c60: 6574 2729 0a20 2020 2020 2020 2020 2020  et').           
-00001c70: 2065 6c69 6620 7374 6174 7573 203d 3d20   elif status == 
-00001c80: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-00001c90: 2020 2023 2070 7269 6e74 2827 436f 6d6d     # print('Comm
-00001ca0: 616e 6420 636f 6d70 6c65 7465 6420 7375  and completed su
-00001cb0: 6363 6573 7366 756c 6c79 2729 0a20 2020  ccessfully').   
-00001cc0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00001cd0: 6e74 2827 4174 7465 6e75 6174 696f 6e20  nt('Attenuation 
-00001ce0: 7365 7420 746f 2020 7b7d 5b64 425d 272e  set to  {}[dB]'.
-00001cf0: 666f 726d 6174 2866 6c6f 6174 2873 656c  format(float(sel
-00001d00: 662e 4765 7461 7474 6e28 2929 2929 0a20  f.Getattn()))). 
-00001d10: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00001d20: 7374 6174 7573 203d 3d20 323a 0a20 2020  status == 2:.   
-00001d30: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00001d40: 6e74 280a 2020 2020 2020 2020 2020 2020  nt(.            
-00001d50: 2020 2020 2020 2020 2752 6571 7565 7374          'Request
-00001d60: 6564 2061 7474 656e 7561 7469 6f6e 2077  ed attenuation w
-00001d70: 6173 2068 6967 6865 7220 7468 616e 2074  as higher than t
-00001d80: 6865 2061 6c6c 6f77 6564 2072 616e 6765  he allowed range
-00001d90: 2c20 7468 6520 6174 7465 6e75 6174 696f  , the attenuatio
-00001da0: 6e20 7761 7320 7365 7420 746f 2074 6865  n was set to the
-00001db0: 2064 6576 6963 65ef bfbd 7320 6d61 7869   device...s maxi
-00001dc0: 6d75 6d20 616c 6c6f 7765 6420 7661 6c75  mum allowed valu
-00001dd0: 6527 290a 2020 2020 2020 2020 2020 2020  e').            
-00001de0: 2320 7072 696e 7428 7374 6174 7573 290a  # print(status).
-00001df0: 0a20 2020 2020 2020 2064 6566 2047 6574  .        def Get
-00001e00: 6174 746e 2873 656c 6629 3a0a 2020 2020  attn(self):.    
-00001e10: 2020 2020 2020 2020 636d 6420 3d20 223a          cmd = ":
-00001e20: 4154 543f 220a 2020 2020 2020 2020 2020  ATT?".          
-00001e30: 2020 5265 7370 203d 2066 6c6f 6174 2873    Resp = float(s
-00001e40: 656c 662e 4465 7669 6365 2e53 656e 645f  elf.Device.Send_
-00001e50: 5343 5049 2863 6d64 2c20 2222 2929 0a20  SCPI(cmd, "")). 
-00001e60: 2020 2020 2020 2020 2020 2023 2070 7269             # pri
-00001e70: 6e74 2852 6573 7029 0a20 2020 2020 2020  nt(Resp).       
-00001e80: 2020 2020 2023 2069 6620 7374 6174 7573       # if status
-00001e90: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-00001ea0: 2020 2023 2020 2020 2070 7269 6e74 2827     #     print('
-00001eb0: 436f 6d6d 616e 6420 6661 696c 6564 206f  Command failed o
-00001ec0: 7220 696e 7661 6c69 6420 6174 7465 6e75  r invalid attenu
-00001ed0: 6174 696f 6e20 7365 7427 290a 2020 2020  ation set').    
-00001ee0: 2020 2020 2020 2020 2320 656c 6966 2073          # elif s
-00001ef0: 7461 7475 7320 3d3d 2031 3a0a 2020 2020  tatus == 1:.    
-00001f00: 2020 2020 2020 2020 2320 2020 2020 7072          #     pr
-00001f10: 696e 7428 2743 6f6d 6d61 6e64 2063 6f6d  int('Command com
-00001f20: 706c 6574 6564 2073 7563 6365 7373 6675  pleted successfu
-00001f30: 6c6c 7927 290a 2020 2020 2020 2020 2020  lly').          
-00001f40: 2020 7265 7475 726e 2052 6573 700a 0a20    return Resp.. 
-00001f50: 2020 2063 6c61 7373 204d 4344 495f 5553     class MCDI_US
-00001f60: 4228 6f62 6a65 6374 293a 0a20 2020 2020  B(object):.     
-00001f70: 2020 2023 2036 3420 6269 7420 6172 7261     # 64 bit arra
-00001f80: 7920 746f 2073 656e 6420 746f 2055 5342  y to send to USB
-00001f90: 0a20 2020 2020 2020 2063 6d64 3120 3d20  .        cmd1 = 
-00001fa0: 5b30 2c20 302c 2030 2c20 302c 2030 2c20  [0, 0, 0, 0, 0, 
-00001fb0: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
-00001fc0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-00001fd0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
-00001fe0: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
-00001ff0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-00002000: 2030 2c20 302c 2030 2c0a 2020 2020 2020   0, 0, 0,.      
-00002010: 2020 2020 2020 2020 2020 302c 2030 2c20            0, 0, 
-00002020: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
-00002030: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
-00002040: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
-00002050: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
-00002060: 2c20 302c 2030 2c20 302c 2030 2c0a 2020  , 0, 0, 0, 0,.  
-00002070: 2020 2020 2020 2020 2020 2020 2020 305d                0]
-00002080: 2020 2320 3634 2062 6974 2061 7272 6179    # 64 bit array
-00002090: 2074 6f20 7365 6e64 2074 6f20 5553 420a   to send to USB.
-000020a0: 0a20 2020 2020 2020 2064 6566 205f 5f69  .        def __i
-000020b0: 6e69 745f 5f28 7365 6c66 293a 0a20 2020  nit__(self):.   
-000020c0: 2020 2020 2020 2020 2023 2066 696e 6420           # find 
-000020d0: 7468 6520 6465 7669 6365 0a20 2020 2020  the device.     
-000020e0: 2020 2020 2020 2073 656c 662e 6465 7620         self.dev 
-000020f0: 3d20 7573 622e 636f 7265 2e66 696e 6428  = usb.core.find(
-00002100: 6964 5665 6e64 6f72 3d30 7832 3063 652c  idVendor=0x20ce,
-00002110: 2069 6450 726f 6475 6374 3d30 7830 3032   idProduct=0x002
-00002120: 3329 0a20 2020 2020 2020 2020 2020 2023  3).            #
-00002130: 2077 6173 2069 7420 666f 756e 643f 0a20   was it found?. 
-00002140: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00002150: 6c66 2e64 6576 2069 7320 4e6f 6e65 3a0a  lf.dev is None:.
-00002160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002170: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00002180: 2827 4465 7669 6365 206e 6f74 2066 6f75  ('Device not fou
-00002190: 6e64 2729 0a20 2020 2020 2020 2020 2020  nd').           
-000021a0: 2023 2073 6574 2074 6865 2061 6374 6976   # set the activ
-000021b0: 6520 636f 6e66 6967 7572 6174 696f 6e2e  e configuration.
-000021c0: 2077 6974 6820 6e6f 2061 7267 7320 7765   with no args we
-000021d0: 2075 7365 2066 6972 7374 2063 6f6e 6669   use first confi
-000021e0: 672e 0a20 2020 2020 2020 2020 2020 2023  g..            #
-000021f0: 2020 666f 7220 4c69 6e75 7820 6f6e 6c79    for Linux only
-00002200: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002210: 7379 732e 706c 6174 666f 726d 203d 3d20  sys.platform == 
-00002220: 276c 696e 7578 273a 0a0a 2020 2020 2020  'linux':..      
-00002230: 2020 2020 2020 2020 2020 666f 7220 636f            for co
-00002240: 6e66 6967 7572 6174 696f 6e20 696e 2073  nfiguration in s
-00002250: 656c 662e 6465 763a 0a20 2020 2020 2020  elf.dev:.       
-00002260: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00002270: 2069 6e74 6572 6661 6365 2069 6e20 636f   interface in co
-00002280: 6e66 6967 7572 6174 696f 6e3a 0a20 2020  nfiguration:.   
-00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022a0: 2020 2020 2069 666e 756d 203d 2069 6e74       ifnum = int
-000022b0: 6572 6661 6365 2e62 496e 7465 7266 6163  erface.bInterfac
-000022c0: 654e 756d 6265 720a 2020 2020 2020 2020  eNumber.        
-000022d0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000022e0: 6f74 2073 656c 662e 6465 762e 6973 5f6b  ot self.dev.is_k
-000022f0: 6572 6e65 6c5f 6472 6976 6572 5f61 6374  ernel_driver_act
-00002300: 6976 6528 6966 6e75 6d29 3a0a 2020 2020  ive(ifnum):.    
-00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
-00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002340: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00002350: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00002360: 7072 696e 7420 2264 6574 6163 6820 6b65  print "detach ke
-00002370: 726e 656c 2064 7269 7665 7220 6672 6f6d  rnel driver from
-00002380: 2064 6576 6963 6520 2573 3a20 696e 7465   device %s: inte
-00002390: 7266 6163 6520 2573 2220 2520 2864 6576  rface %s" % (dev
-000023a0: 2c20 6966 6e75 6d29 0a20 2020 2020 2020  , ifnum).       
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 2073 656c 662e 6465 762e 6465 7461 6368   self.dev.detach
-000023d0: 5f6b 6572 6e65 6c5f 6472 6976 6572 2869  _kernel_driver(i
-000023e0: 666e 756d 290a 2020 2020 2020 2020 2020  fnum).          
-000023f0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00002400: 2075 7362 2e63 6f72 652e 5553 4245 7272   usb.core.USBErr
-00002410: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-00002420: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-00002430: 0a0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00002440: 6c66 2e64 6576 2e73 6574 5f63 6f6e 6669  lf.dev.set_confi
-00002450: 6775 7261 7469 6f6e 2829 0a20 2020 2020  guration().     
-00002460: 2020 2020 2020 2073 656c 662e 636d 6431         self.cmd1
-00002470: 5b30 5d20 3d20 3431 0a20 2020 2020 2020  [0] = 41.       
-00002480: 2020 2020 2073 656c 662e 6465 762e 7772       self.dev.wr
-00002490: 6974 6528 3078 3031 2c20 7365 6c66 2e63  ite(0x01, self.c
-000024a0: 6d64 3129 2020 2320 534e 0a20 2020 2020  md1)  # SN.     
-000024b0: 2020 2020 2020 2073 203d 2073 656c 662e         s = self.
-000024c0: 6465 762e 7265 6164 2830 7838 312c 2036  dev.read(0x81, 6
-000024d0: 3429 0a20 2020 2020 2020 2020 2020 2073  4).            s
-000024e0: 656c 662e 5365 7269 616c 4e75 6d62 6572  elf.SerialNumber
-000024f0: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
-00002500: 2020 6920 3d20 310a 2020 2020 2020 2020    i = 1.        
-00002510: 2020 2020 7768 696c 6520 2873 5b69 5d20      while (s[i] 
-00002520: 3e20 3029 3a0a 2020 2020 2020 2020 2020  > 0):.          
-00002530: 2020 2020 2020 7365 6c66 2e53 6572 6961        self.Seria
-00002540: 6c4e 756d 6265 7220 3d20 7365 6c66 2e53  lNumber = self.S
-00002550: 6572 6961 6c4e 756d 6265 7220 2b20 6368  erialNumber + ch
-00002560: 7228 735b 695d 290a 2020 2020 2020 2020  r(s[i]).        
-00002570: 2020 2020 2020 2020 6920 3d20 6920 2b20          i = i + 
-00002580: 310a 2020 2020 2020 2020 2020 2020 7365  1.            se
-00002590: 6c66 2e63 6d64 315b 305d 203d 2034 300a  lf.cmd1[0] = 40.
-000025a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000025b0: 2e64 6576 2e77 7269 7465 2830 7830 312c  .dev.write(0x01,
-000025c0: 2073 656c 662e 636d 6431 2920 2023 204d   self.cmd1)  # M
-000025d0: 6f64 656c 0a20 2020 2020 2020 2020 2020  odel.           
-000025e0: 2073 203d 2073 656c 662e 6465 762e 7265   s = self.dev.re
-000025f0: 6164 2830 7838 312c 2036 3429 0a20 2020  ad(0x81, 64).   
-00002600: 2020 2020 2020 2020 2073 656c 662e 4d6f           self.Mo
-00002610: 6465 6c4e 616d 6520 3d20 2222 0a20 2020  delName = "".   
-00002620: 2020 2020 2020 2020 2069 203d 2031 0a20           i = 1. 
-00002630: 2020 2020 2020 2020 2020 2077 6869 6c65             while
-00002640: 2028 735b 695d 203e 2030 293a 0a20 2020   (s[i] > 0):.   
-00002650: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00002660: 662e 4d6f 6465 6c4e 616d 6520 3d20 7365  f.ModelName = se
-00002670: 6c66 2e4d 6f64 656c 4e61 6d65 202b 2063  lf.ModelName + c
-00002680: 6872 2873 5b69 5d29 0a20 2020 2020 2020  hr(s[i]).       
-00002690: 2020 2020 2020 2020 2069 203d 2069 202b           i = i +
-000026a0: 2031 0a0a 2020 2020 2020 2020 2020 2020   1..            
-000026b0: 7365 6c66 2e4d 6178 696d 756d 5f41 7474  self.Maximum_Att
-000026c0: 6e20 3d20 666c 6f61 7428 7365 6c66 2e4d  n = float(self.M
-000026d0: 6f64 656c 4e61 6d65 5b31 313a 5d29 0a20  odelName[11:]). 
-000026e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000026f0: 636d 6431 5b30 5d20 3d20 3939 0a20 2020  cmd1[0] = 99.   
-00002700: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-00002710: 762e 7772 6974 6528 3078 3031 2c20 7365  v.write(0x01, se
-00002720: 6c66 2e63 6d64 3129 2020 2320 4657 0a20  lf.cmd1)  # FW. 
-00002730: 2020 2020 2020 2020 2020 2073 203d 2073             s = s
-00002740: 656c 662e 6465 762e 7265 6164 2830 7838  elf.dev.read(0x8
-00002750: 312c 2036 3429 0a20 2020 2020 2020 2020  1, 64).         
-00002760: 2020 2073 656c 662e 4657 203d 2022 220a     self.FW = "".
-00002770: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002780: 2e46 5720 3d20 6368 7228 735b 355d 2920  .FW = chr(s[5]) 
-00002790: 2b20 6368 7228 735b 365d 290a 2020 2020  + chr(s[6]).    
-000027a0: 2020 2020 2020 2020 7365 6c66 2e73 7461          self.sta
-000027b0: 7475 735f 6d65 7373 6167 6520 3d20 2746  tus_message = 'F
-000027c0: 6f75 6e64 2041 7474 656e 7561 746f 723a  ound Attenuator:
-000027d0: 204d 6f64 656c 207b 7d2c 2053 4e3a 207b   Model {}, SN: {
-000027e0: 7d20 2c20 4657 3a20 7b7d 2c20 4d61 7869  } , FW: {}, Maxi
-000027f0: 6d75 6d20 6174 7465 6e75 6174 696f 6e3a  mum attenuation:
-00002800: 207b 7d64 4220 272e 666f 726d 6174 280a   {}dB '.format(.
-00002810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002820: 7374 7228 7365 6c66 2e4d 6f64 656c 4e61  str(self.ModelNa
-00002830: 6d65 292c 2073 7472 2873 656c 662e 5365  me), str(self.Se
-00002840: 7269 616c 4e75 6d62 6572 292c 2073 7472  rialNumber), str
-00002850: 2873 656c 662e 4657 292c 2073 7472 2873  (self.FW), str(s
-00002860: 656c 662e 4d61 7869 6d75 6d5f 4174 746e  elf.Maximum_Attn
-00002870: 2929 0a20 2020 2020 2020 2020 2020 2070  )).            p
-00002880: 7269 6e74 2873 656c 662e 7374 6174 7573  rint(self.status
-00002890: 5f6d 6573 7361 6765 290a 0a20 2020 2020  _message)..     
-000028a0: 2020 2064 6566 2052 6561 6453 4e28 7365     def ReadSN(se
-000028b0: 6c66 293a 0a20 2020 2020 2020 2020 2020  lf):.           
-000028c0: 2072 6574 7572 6e20 7374 7228 7365 6c66   return str(self
-000028d0: 2e53 6572 6961 6c4e 756d 6265 7229 0a0a  .SerialNumber)..
-000028e0: 2020 2020 2020 2020 6465 6620 5265 6164          def Read
-000028f0: 4d4e 2873 656c 6629 3a0a 2020 2020 2020  MN(self):.      
-00002900: 2020 2020 2020 7265 7475 726e 2073 7472        return str
-00002910: 2873 656c 662e 4d6f 6465 6c4e 616d 6529  (self.ModelName)
-00002920: 0a0a 2020 2020 2020 2020 6465 6620 5265  ..        def Re
-00002930: 6164 4657 2873 656c 6629 3a0a 2020 2020  adFW(self):.    
-00002940: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002950: 7472 2873 656c 662e 4657 290a 0a20 2020  tr(self.FW)..   
-00002960: 2020 2020 2064 6566 2052 6561 644d 6178       def ReadMax
-00002970: 5261 6e67 6528 7365 6c66 293a 0a20 2020  Range(self):.   
-00002980: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00002990: 7365 6c66 2e4d 6178 696d 756d 5f41 7474  self.Maximum_Att
-000029a0: 6e0a 0a20 2020 2020 2020 2064 6566 2053  n..        def S
-000029b0: 6574 6174 746e 2873 656c 662c 2041 7474  etattn(self, Att
-000029c0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-000029d0: 7365 6c66 2e63 6d64 315b 305d 203d 2031  self.cmd1[0] = 1
-000029e0: 390a 2020 2020 2020 2020 2020 2020 7365  9.            se
-000029f0: 6c66 2e63 6d64 315b 315d 203d 2069 6e74  lf.cmd1[1] = int
-00002a00: 2841 7474 6e29 0a20 2020 2020 2020 2020  (Attn).         
-00002a10: 2020 2073 656c 662e 636d 6431 5b32 5d20     self.cmd1[2] 
-00002a20: 3d20 696e 7428 2841 7474 6e20 2d20 696e  = int((Attn - in
-00002a30: 7428 4174 746e 2929 202a 2034 290a 2020  t(Attn)) * 4).  
-00002a40: 2020 2020 2020 2020 2020 6966 2041 7474            if Att
-00002a50: 6e20 3e20 7365 6c66 2e4d 6178 696d 756d  n > self.Maximum
-00002a60: 5f41 7474 6e3a 0a20 2020 2020 2020 2020  _Attn:.         
-00002a70: 2020 2020 2020 2070 7269 6e74 2827 4174         print('At
-00002a80: 7465 6e75 6174 696f 6e20 6e6f 7420 696e  tenuation not in
-00002a90: 2052 616e 6765 2c73 6574 7469 6e67 206d   Range,setting m
-00002aa0: 6178 696d 756d 203d 207b 7d20 272e 666f  aximum = {} '.fo
-00002ab0: 726d 6174 2873 7472 2873 656c 662e 4d61  rmat(str(self.Ma
-00002ac0: 7869 6d75 6d5f 4174 746e 2929 290a 2020  ximum_Attn))).  
-00002ad0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00002ae0: 6c66 2e63 6d64 315b 315d 203d 2069 6e74  lf.cmd1[1] = int
-00002af0: 2873 656c 662e 4d61 7869 6d75 6d5f 4174  (self.Maximum_At
-00002b00: 746e 290a 2020 2020 2020 2020 2020 2020  tn).            
-00002b10: 2020 2020 7365 6c66 2e63 6d64 315b 325d      self.cmd1[2]
-00002b20: 203d 2069 6e74 2828 7365 6c66 2e4d 6178   = int((self.Max
-00002b30: 696d 756d 5f41 7474 6e20 2d20 696e 7428  imum_Attn - int(
-00002b40: 7365 6c66 2e4d 6178 696d 756d 5f41 7474  self.Maximum_Att
-00002b50: 6e29 2920 2a20 3429 0a20 2020 2020 2020  n)) * 4).       
-00002b60: 2020 2020 2023 2073 656c 662e 6465 762e       # self.dev.
-00002b70: 7365 745f 636f 6e66 6967 7572 6174 696f  set_configuratio
-00002b80: 6e28 290a 0a20 2020 2020 2020 2020 2020  n()..           
-00002b90: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00002ba0: 2020 2020 2020 7365 6c66 2e64 6576 2e77        self.dev.w
-00002bb0: 7269 7465 2830 7830 312c 2073 656c 662e  rite(0x01, self.
-00002bc0: 636d 6431 2920 2023 2053 6574 2061 7474  cmd1)  # Set att
-00002bd0: 656e 7561 7469 6f6e 0a20 2020 2020 2020  enuation.       
-00002be0: 2020 2020 2020 2020 2073 203d 2073 656c           s = sel
-00002bf0: 662e 6465 762e 7265 6164 2830 7838 312c  f.dev.read(0x81,
-00002c00: 2036 3429 0a20 2020 2020 2020 2020 2020   64).           
-00002c10: 2020 2020 2073 656c 662e 6e65 775f 6174       self.new_at
-00002c20: 7420 3d20 2753 6574 7469 6e67 2041 7474  t = 'Setting Att
-00002c30: 656e 7561 7469 6f6e 203d 207b 7d64 4220  enuation = {}dB 
-00002c40: 272e 666f 726d 6174 2873 7472 2873 5b31  '.format(str(s[1
-00002c50: 5d20 2b20 735b 325d 202f 2034 2929 0a20  ] + s[2] / 4)). 
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00002c70: 7269 6e74 2873 656c 662e 6e65 775f 6174  rint(self.new_at
-00002c80: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-00002c90: 2020 2072 6574 7572 6e20 735b 315d 202b     return s[1] +
-00002ca0: 2073 5b32 5d20 2f20 340a 2020 2020 2020   s[2] / 4.      
-00002cb0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-00002cc0: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
-00002cd0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00002ce0: 6e74 2865 290a 2020 2020 2020 2020 2020  nt(e).          
-00002cf0: 2020 2020 2020 7365 6c66 2e6e 6577 5f61        self.new_a
-00002d00: 7474 203d 2065 0a20 2020 2020 2020 2020  tt = e.         
-00002d10: 2020 2020 2020 2072 6574 7572 6e20 730a         return s.
-00002d20: 0a20 2020 2020 2020 2064 6566 2047 6574  .        def Get
-00002d30: 6174 746e 2873 656c 6629 3a0a 2020 2020  attn(self):.    
-00002d40: 2020 2020 2020 2020 2320 7365 6c66 2e64          # self.d
-00002d50: 6576 2e73 6574 5f63 6f6e 6669 6775 7261  ev.set_configura
-00002d60: 7469 6f6e 2829 0a20 2020 2020 2020 2020  tion().         
-00002d70: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
-00002d80: 2020 2020 2020 2020 7365 6c66 2e63 6d64          self.cmd
-00002d90: 315b 305d 203d 2031 380a 2020 2020 2020  1[0] = 18.      
-00002da0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-00002db0: 6576 2e77 7269 7465 2830 7830 312c 2073  ev.write(0x01, s
-00002dc0: 656c 662e 636d 6431 2920 2023 2047 6574  elf.cmd1)  # Get
-00002dd0: 2061 7474 656e 7561 7474 696f 6e0a 2020   attenuattion.  
-00002de0: 2020 2020 2020 2020 2020 2020 2020 7320                s 
-00002df0: 3d20 7365 6c66 2e64 6576 2e72 6561 6428  = self.dev.read(
-00002e00: 3078 3831 2c20 3634 290a 2020 2020 2020  0x81, 64).      
-00002e10: 2020 2020 2020 2020 2020 7365 6c66 2e6e            self.n
-00002e20: 6577 5f61 7474 203d 2027 4375 7272 656e  ew_att = 'Curren
-00002e30: 7420 4174 7465 6e75 6174 696f 6e20 3d20  t Attenuation = 
-00002e40: 7b7d 6442 2027 2e66 6f72 6d61 7428 7374  {}dB '.format(st
-00002e50: 7228 735b 315d 202b 2073 5b32 5d20 2f20  r(s[1] + s[2] / 
-00002e60: 3429 290a 2020 2020 2020 2020 2020 2020  4)).            
-00002e70: 2020 2020 7072 696e 7428 7365 6c66 2e6e      print(self.n
-00002e80: 6577 5f61 7474 290a 2020 2020 2020 2020  ew_att).        
-00002e90: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002ea0: 5b31 5d20 2b20 735b 325d 202f 2034 0a20  [1] + s[2] / 4. 
-00002eb0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-00002ec0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-00002ed0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002ee0: 2020 7072 696e 7428 6529 0a20 2020 2020    print(e).     
-00002ef0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00002f00: 6e65 775f 6174 7420 3d20 650a 2020 2020  new_att = e.    
-00002f10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002f20: 726e 2073 0a0a 2020 2020 2020 2020 6465  rn s..        de
-00002f30: 6620 5365 6e64 5f53 4350 4928 7365 6c66  f Send_SCPI(self
-00002f40: 2c20 5343 5049 636d 642c 2074 6d70 293a  , SCPIcmd, tmp):
-00002f50: 0a20 2020 2020 2020 2020 2020 2023 2073  .            # s
-00002f60: 656e 6420 5343 5049 2063 6f6d 6d61 6e64  end SCPI command
-00002f70: 7320 2874 6f20 7375 7070 6f72 7465 6420  s (to supported 
-00002f80: 6669 726d 7761 7265 206f 6e6c 7921 290a  firmware only!).
-00002f90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00002fa0: 2e63 6d64 315b 305d 203d 2034 320a 2020  .cmd1[0] = 42.  
-00002fb0: 2020 2020 2020 2020 2020 6c31 203d 2030            l1 = 0
-00002fc0: 0a20 2020 2020 2020 2020 2020 206c 3120  .            l1 
-00002fd0: 3d20 6c65 6e28 5343 5049 636d 6429 0a20  = len(SCPIcmd). 
-00002fe0: 2020 2020 2020 2020 2020 2069 6e64 7820             indx 
-00002ff0: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00003000: 7768 696c 6520 2869 6e64 7820 3c3d 206c  while (indx <= l
-00003010: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-00003020: 2020 2020 7365 6c66 2e63 6d64 315b 696e      self.cmd1[in
-00003030: 6478 5d20 3d20 6f72 6428 5343 5049 636d  dx] = ord(SCPIcm
-00003040: 645b 696e 6478 202d 2031 5d29 0a20 2020  d[indx - 1]).   
-00003050: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
-00003060: 7820 3d20 696e 6478 202b 2031 0a20 2020  x = indx + 1.   
-00003070: 2020 2020 2020 2020 2073 656c 662e 636d           self.cm
-00003080: 6431 5b69 6e64 785d 203d 2030 0a20 2020  d1[indx] = 0.   
-00003090: 2020 2020 2020 2020 2073 656c 662e 6465           self.de
-000030a0: 762e 7772 6974 6528 3078 3031 2c20 7365  v.write(0x01, se
-000030b0: 6c66 2e63 6d64 3129 2020 2320 5343 5020  lf.cmd1)  # SCP 
-000030c0: 436f 6d6d 616e 6420 7570 2074 6f20 3630  Command up to 60
-000030d0: 2063 6861 7273 3b0a 2020 2020 2020 2020   chars;.        
-000030e0: 2020 2020 7320 3d20 7365 6c66 2e64 6576      s = self.dev
-000030f0: 2e72 6561 6428 3078 3831 2c20 3634 290a  .read(0x81, 64).
-00003100: 2020 2020 2020 2020 2020 2020 6920 3d20              i = 
-00003110: 310a 2020 2020 2020 2020 2020 2020 5265  1.            Re
-00003120: 7453 7472 203d 2022 220a 2020 2020 2020  tStr = "".      
-00003130: 2020 2020 2020 7768 696c 6520 2873 5b69        while (s[i
-00003140: 5d20 3e20 3029 3a0a 2020 2020 2020 2020  ] > 0):.        
-00003150: 2020 2020 2020 2020 5265 7453 7472 203d          RetStr =
-00003160: 2052 6574 5374 7220 2b20 6368 7228 735b   RetStr + chr(s[
-00003170: 695d 290a 2020 2020 2020 2020 2020 2020  i]).            
-00003180: 2020 2020 6920 3d20 6920 2b20 310a 2020      i = i + 1.  
-00003190: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000031a0: 2073 7472 2852 6574 5374 7229 0a0a 2020   str(RetStr)..  
-000031b0: 2020 636c 6173 7320 4150 4928 6f62 6a65    class API(obje
-000031c0: 6374 293a 0a0a 2020 2020 2020 2020 6465  ct):..        de
-000031d0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-000031e0: 2063 6f6d 706f 7274 3d22 4155 544f 2229   comport="AUTO")
-000031f0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00003200: 6c66 2e62 6175 6472 6174 6520 3d20 3936  lf.baudrate = 96
-00003210: 3030 0a20 2020 2020 2020 2020 2020 2069  00.            i
-00003220: 6620 636f 6d70 6f72 7420 3d3d 2022 4155  f comport == "AU
-00003230: 544f 223a 0a20 2020 2020 2020 2020 2020  TO":.           
-00003240: 2020 2020 2070 6f72 7473 5f6c 6973 7420       ports_list 
-00003250: 3d20 7365 7269 616c 5f70 6f72 7473 2829  = serial_ports()
-00003260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003270: 2066 6f72 2070 6f72 7420 696e 2070 6f72   for port in por
-00003280: 7473 5f6c 6973 743a 0a20 2020 2020 2020  ts_list:.       
-00003290: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000032a0: 662e 636f 6d70 6f72 7420 3d20 706f 7274  f.comport = port
-000032b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000032c0: 2020 2020 2073 656c 662e 7320 3d20 7365       self.s = se
-000032d0: 7269 616c 2e53 6572 6961 6c28 7365 6c66  rial.Serial(self
-000032e0: 2e63 6f6d 706f 7274 2c20 7365 6c66 2e62  .comport, self.b
-000032f0: 6175 6472 6174 652c 2074 696d 656f 7574  audrate, timeout
-00003300: 3d30 2e35 290a 2020 2020 2020 2020 2020  =0.5).          
-00003310: 2020 2020 2020 2020 2020 736c 6565 7028            sleep(
-00003320: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-00003330: 2020 2020 2020 2073 656c 662e 732e 666c         self.s.fl
-00003340: 7573 6849 6e70 7574 2829 0a20 2020 2020  ushInput().     
-00003350: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003360: 656c 662e 732e 666c 7573 684f 7574 7075  elf.s.flushOutpu
-00003370: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00003380: 2020 2020 2020 2020 736c 6565 7028 302e          sleep(0.
-00003390: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-000033a0: 2020 2020 2020 2023 2054 7572 6e20 7468         # Turn th
-000033b0: 6520 636f 6e73 6f6c 6520 6f66 660a 2020  e console off.  
-000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033d0: 2020 7365 6c66 2e73 2e77 7269 7465 2822    self.s.write("
-000033e0: 434f 4e53 4f4c 4520 4449 5341 424c 455c  CONSOLE DISABLE\
-000033f0: 725c 6e22 2e65 6e63 6f64 6528 2929 0a20  r\n".encode()). 
-00003400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003410: 2020 2023 2046 6c75 7368 2074 6865 2062     # Flush the b
-00003420: 7566 6665 7273 0a20 2020 2020 2020 2020  uffers.         
-00003430: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
-00003440: 2830 2e31 290a 2020 2020 2020 2020 2020  (0.1).          
-00003450: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-00003460: 2e66 6c75 7368 2829 0a20 2020 2020 2020  .flush().       
-00003470: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003480: 662e 732e 666c 7573 6849 6e70 7574 2829  f.s.flushInput()
-00003490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000034a0: 2020 2020 2073 656c 662e 732e 666c 7573       self.s.flus
-000034b0: 684f 7574 7075 7428 290a 2020 2020 2020  hOutput().      
-000034c0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000034d0: 6c66 2e73 2e77 7269 7465 2822 2a49 444e  lf.s.write("*IDN
-000034e0: 3f5c 725c 6e22 2e65 6e63 6f64 6528 2929  ?\r\n".encode())
-000034f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003500: 2020 2020 2073 6c65 6570 2830 2e31 290a       sleep(0.1).
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 2020 6966 2073 656c 662e 732e 696e      if self.s.in
-00003530: 5f77 6169 7469 6e67 203e 2031 3a0a 2020  _waiting > 1:.  
+00000f20: 2c20 736c 6565 700a 6672 6f6d 2073 7461  , sleep.from sta
+00000f30: 7469 7374 6963 7320 696d 706f 7274 206d  tistics import m
+00000f40: 6f64 650a 696d 706f 7274 2073 7973 0a69  ode.import sys.i
+00000f50: 6d70 6f72 7420 7365 7269 616c 0a69 6d70  mport serial.imp
+00000f60: 6f72 7420 7365 7269 616c 2e74 6f6f 6c73  ort serial.tools
+00000f70: 2e6c 6973 745f 706f 7274 730a 6672 6f6d  .list_ports.from
+00000f80: 2079 6f63 746f 7075 6365 2e79 6f63 746f   yoctopuce.yocto
+00000f90: 5f74 656d 7065 7261 7475 7265 2069 6d70  _temperature imp
+00000fa0: 6f72 7420 5941 5049 2c20 5952 6566 5061  ort YAPI, YRefPa
+00000fb0: 7261 6d2c 2059 5465 6d70 6572 6174 7572  ram, YTemperatur
+00000fc0: 650a 696d 706f 7274 206f 730a 0a0a 636c  e.import os...cl
+00000fd0: 6173 7320 4571 7569 706d 656e 7445 7272  ass EquipmentErr
+00000fe0: 6f72 2845 7863 6570 7469 6f6e 293a 0a0a  or(Exception):..
+00000ff0: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+00001000: 2873 656c 662c 202a 6172 6773 293a 0a20  (self, *args):. 
+00001010: 2020 2020 2020 2069 6620 6172 6773 3a0a         if args:.
+00001020: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001030: 2e6d 6573 7361 6765 203d 2061 7267 735b  .message = args[
+00001040: 305d 0a20 2020 2020 2020 2065 6c73 653a  0].        else:
+00001050: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001060: 662e 6d65 7373 6167 6520 3d20 4e6f 6e65  f.message = None
+00001070: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
+00001080: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00001090: 2023 2070 7269 6e74 2827 6361 6c6c 696e   # print('callin
+000010a0: 6720 7374 7227 290a 2020 2020 2020 2020  g str').        
+000010b0: 6966 2073 656c 662e 6d65 7373 6167 653a  if self.message:
+000010c0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000010d0: 7572 6e20 2745 7175 6970 6d65 6e74 4572  urn 'EquipmentEr
+000010e0: 726f 723a 207b 6d73 677d 272e 666f 726d  ror: {msg}'.form
+000010f0: 6174 286d 7367 3d73 656c 662e 6d65 7373  at(msg=self.mess
+00001100: 6167 6529 0a20 2020 2020 2020 2065 6c73  age).        els
+00001110: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00001120: 6574 7572 6e20 2745 7175 6970 6d65 6e74  eturn 'Equipment
+00001130: 4572 726f 7220 6861 7320 6265 656e 2072  Error has been r
+00001140: 6169 7365 6427 0a0a 0a64 6566 2073 6572  aised'...def ser
+00001150: 6961 6c5f 706f 7274 7328 293a 0a20 2020  ial_ports():.   
+00001160: 2022 2222 204c 6973 7473 2073 6572 6961   """ Lists seria
+00001170: 6c20 706f 7274 206e 616d 6573 0a0a 2020  l port names..  
+00001180: 2020 2020 2020 3a72 6169 7365 7320 456e        :raises En
+00001190: 7669 726f 6e6d 656e 7445 7272 6f72 3a0a  vironmentError:.
+000011a0: 2020 2020 2020 2020 2020 2020 4f6e 2075              On u
+000011b0: 6e73 7570 706f 7274 6564 206f 7220 756e  nsupported or un
+000011c0: 6b6e 6f77 6e20 706c 6174 666f 726d 730a  known platforms.
+000011d0: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
+000011e0: 3a0a 2020 2020 2020 2020 2020 2020 4120  :.            A 
+000011f0: 6c69 7374 206f 6620 7468 6520 7365 7269  list of the seri
+00001200: 616c 2070 6f72 7473 2061 7661 696c 6162  al ports availab
+00001210: 6c65 206f 6e20 7468 6520 7379 7374 656d  le on the system
+00001220: 0a20 2020 2022 2222 0a20 2020 2061 7661  .    """.    ava
+00001230: 696c 6162 6c65 5f70 6f72 7473 203d 205b  ilable_ports = [
+00001240: 732e 6465 7669 6365 2066 6f72 2073 2069  s.device for s i
+00001250: 6e20 7365 7269 616c 2e74 6f6f 6c73 2e6c  n serial.tools.l
+00001260: 6973 745f 706f 7274 732e 636f 6d70 6f72  ist_ports.compor
+00001270: 7473 2829 5d0a 2020 2020 6966 206c 656e  ts()].    if len
+00001280: 2861 7661 696c 6162 6c65 5f70 6f72 7473  (available_ports
+00001290: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
+000012a0: 6176 6169 6c61 626c 655f 706f 7274 7320  available_ports 
+000012b0: 3d20 5b73 2e6e 616d 6520 666f 7220 7320  = [s.name for s 
+000012c0: 696e 2073 6572 6961 6c2e 746f 6f6c 732e  in serial.tools.
+000012d0: 6c69 7374 5f70 6f72 7473 2e63 6f6d 706f  list_ports.compo
+000012e0: 7274 7328 295d 0a20 2020 2020 2020 2069  rts()].        i
+000012f0: 6620 6c65 6e28 6176 6169 6c61 626c 655f  f len(available_
+00001300: 706f 7274 7329 203d 3d20 303a 0a20 2020  ports) == 0:.   
+00001310: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00001320: 6e6f 2073 6572 6961 6c20 706f 7274 7320  no serial ports 
+00001330: 7765 7265 2066 6f75 6e64 2e20 706c 6561  were found. plea
+00001340: 7365 2063 6865 636b 2079 6f75 7220 636f  se check your co
+00001350: 6e6e 6563 7469 6f6e 7322 290a 2020 2020  nnections").    
+00001360: 7265 7475 726e 2061 7661 696c 6162 6c65  return available
+00001370: 5f70 6f72 7473 0a0a 0a63 6c61 7373 2041  _ports...class A
+00001380: 7474 656e 7561 746f 7228 6f62 6a65 6374  ttenuator(object
+00001390: 293a 0a20 2020 2027 2727 0a20 2020 2053  ):.    '''.    S
+000013a0: 7570 706f 7274 2061 6c6c 2061 7474 6e20  upport all attn 
+000013b0: 636c 6173 7365 7320 666f 723a 0a20 2020  classes for:.   
+000013c0: 2027 2727 0a0a 2020 2020 6465 6620 5f5f   '''..    def __
+000013d0: 696e 6974 5f5f 2873 656c 662c 2041 5454  init__(self, ATT
+000013e0: 4e5f 7479 7065 2c20 636f 6d70 6f72 743d  N_type, comport=
+000013f0: 2741 5554 4f27 293a 0a20 2020 2020 2020  'AUTO'):.       
+00001400: 2069 6620 274d 4344 492d 5553 4227 2069   if 'MCDI-USB' i
+00001410: 6e20 4154 544e 5f74 7970 653a 0a20 2020  n ATTN_type:.   
+00001420: 2020 2020 2020 2020 2073 656c 662e 5f61           self._a
+00001430: 6374 6976 655f 5445 203d 2041 7474 656e  ctive_TE = Atten
+00001440: 7561 746f 722e 4d43 4449 5f55 5342 2829  uator.MCDI_USB()
+00001450: 0a20 2020 2020 2020 2065 6c69 6620 274d  .        elif 'M
+00001460: 4344 4927 2069 6e20 4154 544e 5f74 7970  CDI' in ATTN_typ
+00001470: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00001480: 656c 662e 5f61 6374 6976 655f 5445 203d  elf._active_TE =
+00001490: 2041 7474 656e 7561 746f 722e 4d43 4449   Attenuator.MCDI
+000014a0: 2829 0a20 2020 2020 2020 2065 6c69 6620  ().        elif 
+000014b0: 2741 5049 2720 696e 2041 5454 4e5f 7479  'API' in ATTN_ty
+000014c0: 7065 206f 7220 2757 6569 6e73 6368 656c  pe or 'Weinschel
+000014d0: 2720 696e 2041 5454 4e5f 7479 7065 3a0a  ' in ATTN_type:.
+000014e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000014f0: 2e5f 6163 7469 7665 5f54 4520 3d20 4174  ._active_TE = At
+00001500: 7465 6e75 6174 6f72 2e41 5049 2863 6f6d  tenuator.API(com
+00001510: 706f 7274 290a 0a20 2020 2020 2020 2065  port)..        e
+00001520: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00001530: 2070 6173 730a 0a20 2020 2064 6566 2047   pass..    def G
+00001540: 6574 4163 7469 7665 5445 2873 656c 6629  etActiveTE(self)
+00001550: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00001560: 2073 656c 662e 5f61 6374 6976 655f 5445   self._active_TE
+00001570: 0a0a 2020 2020 636c 6173 7320 4d43 4449  ..    class MCDI
+00001580: 286f 626a 6563 7429 3a0a 0a20 2020 2020  (object):..     
+00001590: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
+000015a0: 7365 6c66 293a 0a20 2020 2020 2020 2020  self):.         
+000015b0: 2020 2064 6f74 6e65 7420 3d20 4661 6c73     dotnet = Fals
+000015c0: 650a 2020 2020 2020 2020 2020 2020 7574  e.            ut
+000015d0: 696c 735f 6469 7220 3d20 6f73 2e70 6174  ils_dir = os.pat
+000015e0: 682e 6a6f 696e 286f 732e 7061 7468 2e64  h.join(os.path.d
+000015f0: 6972 6e61 6d65 285f 5f66 696c 655f 5f29  irname(__file__)
+00001600: 2c20 2775 7469 6c73 2729 0a20 2020 2020  , 'utils').     
+00001610: 2020 2020 2020 2073 7973 2e70 6174 682e         sys.path.
+00001620: 6170 7065 6e64 2875 7469 6c73 5f64 6972  append(utils_dir
+00001630: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00001640: 2064 6f74 6e65 7420 3d3d 2054 7275 653a   dotnet == True:
+00001650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001660: 2069 6d70 6f72 7420 636c 7220 2023 2070   import clr  # p
+00001670: 7974 686f 6e6e 6574 2c20 6d61 6e75 616c  ythonnet, manual
+00001680: 6c79 2069 6e73 7461 6c6c 6564 2077 6974  ly installed wit
+00001690: 6820 6120 646f 776e 6c6f 6164 6564 2077  h a downloaded w
+000016a0: 6865 656c 2061 6e64 2070 6970 0a20 2020  heel and pip.   
+000016b0: 2020 2020 2020 2020 2020 2020 2069 6d70               imp
+000016c0: 6f72 7420 6374 7970 6573 2020 2320 6d6f  ort ctypes  # mo
+000016d0: 6475 6c65 2074 6f20 6f70 656e 2075 7469  dule to open uti
+000016e0: 6c73 2066 696c 6573 0a20 2020 2020 2020  ls files.       
+000016f0: 2020 2020 2020 2020 2063 6c72 2e41 6464           clr.Add
+00001700: 5265 6665 7265 6e63 6528 2253 7973 7465  Reference("Syste
+00001710: 6d2e 494f 2229 0a20 2020 2020 2020 2020  m.IO").         
+00001720: 2020 2020 2020 2069 6d70 6f72 7420 5379         import Sy
+00001730: 7374 656d 2e49 4f0a 2020 2020 2020 2020  stem.IO.        
+00001740: 2020 2020 2020 2020 5379 7374 656d 2e49          System.I
+00001750: 4f2e 4469 7265 6374 6f72 792e 5365 7443  O.Directory.SetC
+00001760: 7572 7265 6e74 4469 7265 6374 6f72 7928  urrentDirectory(
+00001770: 7574 696c 735f 6469 7229 0a20 2020 2020  utils_dir).     
+00001780: 2020 2020 2020 2020 2020 2063 6c72 2e41             clr.A
+00001790: 6464 5265 6665 7265 6e63 6528 276d 636c  ddReference('mcl
+000017a0: 5f52 5544 4154 5f4e 4554 3435 2729 0a20  _RUDAT_NET45'). 
+000017b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000017c0: 726f 6d20 6d63 6c5f 5255 4441 545f 4e45  rom mcl_RUDAT_NE
+000017d0: 5434 3520 696d 706f 7274 2055 5342 5f52  T45 import USB_R
+000017e0: 5544 4154 0a20 2020 2020 2020 2020 2020  UDAT.           
+000017f0: 2020 2020 2073 656c 662e 4465 7669 6365       self.Device
+00001800: 203d 2055 5342 5f52 5544 4154 2829 0a20   = USB_RUDAT(). 
+00001810: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001820: 656c 662e 4465 7669 6365 2e43 6f6e 6e65  elf.Device.Conne
+00001830: 6374 2829 0a20 2020 2020 2020 2020 2020  ct().           
+00001840: 2020 2020 2069 6e66 6f20 3d20 7365 6c66       info = self
+00001850: 2e44 6576 6963 6549 6e66 6f28 290a 2020  .DeviceInfo().  
+00001860: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001870: 696e 7428 2746 6f75 6e64 2041 7474 656e  int('Found Atten
+00001880: 7561 746f 723a 204d 6f64 656c 207b 7d2c  uator: Model {},
+00001890: 207b 7d20 2c7b 7d20 272e 666f 726d 6174   {} ,{} '.format
+000018a0: 2869 6e66 6f5b 305d 2c20 696e 666f 5b31  (info[0], info[1
+000018b0: 5d2c 2069 6e66 6f5b 325d 2929 0a20 2020  ], info[2])).   
+000018c0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+000018d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000018e0: 726f 6d20 5553 425f 5255 4441 5420 696d  rom USB_RUDAT im
+000018f0: 706f 7274 2055 5342 4441 540a 2020 2020  port USBDAT.    
+00001900: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00001910: 2e44 6576 6963 6520 3d20 5553 4244 4154  .Device = USBDAT
+00001920: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00001930: 2020 2069 6e66 6f20 3d20 7365 6c66 2e44     info = self.D
+00001940: 6576 6963 6549 6e66 6f28 290a 2020 2020  eviceInfo().    
+00001950: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00001960: 7428 2746 6f75 6e64 2041 7474 656e 7561  t('Found Attenua
+00001970: 746f 723a 204d 6f64 656c 207b 7d2c 207b  tor: Model {}, {
+00001980: 7d20 2c7b 7d20 272e 666f 726d 6174 2869  } ,{} '.format(i
+00001990: 6e66 6f5b 305d 2c20 696e 666f 5b31 5d2c  nfo[0], info[1],
+000019a0: 2069 6e66 6f5b 325d 2929 0a0a 2020 2020   info[2]))..    
+000019b0: 2020 2020 6465 6620 4465 7669 6365 496e      def DeviceIn
+000019c0: 666f 2873 656c 6629 3a0a 2020 2020 2020  fo(self):.      
+000019d0: 2020 2020 2020 636d 6420 3d20 223a 4d4e        cmd = ":MN
+000019e0: 3f22 0a20 2020 2020 2020 2020 2020 206d  ?".            m
+000019f0: 6f64 656c 5f6e 616d 6520 3d20 7365 6c66  odel_name = self
+00001a00: 2e44 6576 6963 652e 5365 6e64 5f53 4350  .Device.Send_SCP
+00001a10: 4928 636d 642c 2022 2229 0a20 2020 2020  I(cmd, "").     
+00001a20: 2020 2020 2020 2063 6d64 203d 2022 3a53         cmd = ":S
+00001a30: 4e3f 220a 2020 2020 2020 2020 2020 2020  N?".            
+00001a40: 7365 7269 616c 203d 2073 656c 662e 4465  serial = self.De
+00001a50: 7669 6365 2e53 656e 645f 5343 5049 2863  vice.Send_SCPI(c
+00001a60: 6d64 2c20 2222 290a 2020 2020 2020 2020  md, "").        
+00001a70: 2020 2020 636d 6420 3d20 223a 4649 524d      cmd = ":FIRM
+00001a80: 5741 5245 3f22 0a20 2020 2020 2020 2020  WARE?".         
+00001a90: 2020 2066 7720 3d20 7365 6c66 2e44 6576     fw = self.Dev
+00001aa0: 6963 652e 5365 6e64 5f53 4350 4928 636d  ice.Send_SCPI(cm
+00001ab0: 642c 2022 2229 0a20 2020 2020 2020 2020  d, "").         
+00001ac0: 2020 2023 2072 6574 7572 6e20 5b6d 6f64     # return [mod
+00001ad0: 656c 5f6e 616d 655b 315d 2c20 7365 7269  el_name[1], seri
+00001ae0: 616c 5b31 5d2c 2066 775b 315d 5d20 2023  al[1], fw[1]]  #
+00001af0: 646f 746e 6574 0a20 2020 2020 2020 2020  dotnet.         
+00001b00: 2020 2072 6574 7572 6e20 5b6d 6f64 656c     return [model
+00001b10: 5f6e 616d 652c 2073 6572 6961 6c2c 2066  _name, serial, f
+00001b20: 775d 0a0a 2020 2020 2020 2020 6465 6620  w]..        def 
+00001b30: 5365 7461 7474 6e28 7365 6c66 2c20 6174  Setattn(self, at
+00001b40: 746e 293a 0a20 2020 2020 2020 2020 2020  tn):.           
+00001b50: 2063 6d64 203d 2022 3a53 4554 4154 543a   cmd = ":SETATT:
+00001b60: 2220 2b20 7374 7228 6174 746e 290a 2020  " + str(attn).  
+00001b70: 2020 2020 2020 2020 2020 7374 6174 7573            status
+00001b80: 203d 2069 6e74 2873 656c 662e 4465 7669   = int(self.Devi
+00001b90: 6365 2e53 656e 645f 5343 5049 2863 6d64  ce.Send_SCPI(cmd
+00001ba0: 2c20 2222 2929 0a20 2020 2020 2020 2020  , "")).         
+00001bb0: 2020 2069 6620 7374 6174 7573 203d 3d20     if status == 
+00001bc0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
+00001bd0: 2020 2070 7269 6e74 2827 436f 6d6d 616e     print('Comman
+00001be0: 6420 6661 696c 6564 206f 7220 696e 7661  d failed or inva
+00001bf0: 6c69 6420 6174 7465 6e75 6174 696f 6e20  lid attenuation 
+00001c00: 7365 7427 290a 2020 2020 2020 2020 2020  set').          
+00001c10: 2020 656c 6966 2073 7461 7475 7320 3d3d    elif status ==
+00001c20: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+00001c30: 2020 2020 2320 7072 696e 7428 2743 6f6d      # print('Com
+00001c40: 6d61 6e64 2063 6f6d 706c 6574 6564 2073  mand completed s
+00001c50: 7563 6365 7373 6675 6c6c 7927 290a 2020  uccessfully').  
+00001c60: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001c70: 696e 7428 2741 7474 656e 7561 7469 6f6e  int('Attenuation
+00001c80: 2073 6574 2074 6f20 207b 7d5b 6442 5d27   set to  {}[dB]'
+00001c90: 2e66 6f72 6d61 7428 666c 6f61 7428 7365  .format(float(se
+00001ca0: 6c66 2e47 6574 6174 746e 2829 2929 290a  lf.Getattn()))).
+00001cb0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00001cc0: 2073 7461 7475 7320 3d3d 2032 3a0a 2020   status == 2:.  
+00001cd0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00001ce0: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+00001cf0: 2020 2020 2020 2020 2027 5265 7175 6573           'Reques
+00001d00: 7465 6420 6174 7465 6e75 6174 696f 6e20  ted attenuation 
+00001d10: 7761 7320 6869 6768 6572 2074 6861 6e20  was higher than 
+00001d20: 7468 6520 616c 6c6f 7765 6420 7261 6e67  the allowed rang
+00001d30: 652c 2074 6865 2061 7474 656e 7561 7469  e, the attenuati
+00001d40: 6f6e 2077 6173 2073 6574 2074 6f20 7468  on was set to th
+00001d50: 6520 6465 7669 6365 efbf bd73 206d 6178  e device...s max
+00001d60: 696d 756d 2061 6c6c 6f77 6564 2076 616c  imum allowed val
+00001d70: 7565 2729 0a20 2020 2020 2020 2020 2020  ue').           
+00001d80: 2023 2070 7269 6e74 2873 7461 7475 7329   # print(status)
+00001d90: 0a0a 2020 2020 2020 2020 6465 6620 4765  ..        def Ge
+00001da0: 7461 7474 6e28 7365 6c66 293a 0a20 2020  tattn(self):.   
+00001db0: 2020 2020 2020 2020 2063 6d64 203d 2022           cmd = "
+00001dc0: 3a41 5454 3f22 0a20 2020 2020 2020 2020  :ATT?".         
+00001dd0: 2020 2052 6573 7020 3d20 666c 6f61 7428     Resp = float(
+00001de0: 7365 6c66 2e44 6576 6963 652e 5365 6e64  self.Device.Send
+00001df0: 5f53 4350 4928 636d 642c 2022 2229 290a  _SCPI(cmd, "")).
+00001e00: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
+00001e10: 696e 7428 5265 7370 290a 2020 2020 2020  int(Resp).      
+00001e20: 2020 2020 2020 2320 6966 2073 7461 7475        # if statu
+00001e30: 7320 3d3d 2030 3a0a 2020 2020 2020 2020  s == 0:.        
+00001e40: 2020 2020 2320 2020 2020 7072 696e 7428      #     print(
+00001e50: 2743 6f6d 6d61 6e64 2066 6169 6c65 6420  'Command failed 
+00001e60: 6f72 2069 6e76 616c 6964 2061 7474 656e  or invalid atten
+00001e70: 7561 7469 6f6e 2073 6574 2729 0a20 2020  uation set').   
+00001e80: 2020 2020 2020 2020 2023 2065 6c69 6620           # elif 
+00001e90: 7374 6174 7573 203d 3d20 313a 0a20 2020  status == 1:.   
+00001ea0: 2020 2020 2020 2020 2023 2020 2020 2070           #     p
+00001eb0: 7269 6e74 2827 436f 6d6d 616e 6420 636f  rint('Command co
+00001ec0: 6d70 6c65 7465 6420 7375 6363 6573 7366  mpleted successf
+00001ed0: 756c 6c79 2729 0a20 2020 2020 2020 2020  ully').         
+00001ee0: 2020 2072 6574 7572 6e20 5265 7370 0a0a     return Resp..
+00001ef0: 2020 2020 636c 6173 7320 4d43 4449 5f55      class MCDI_U
+00001f00: 5342 286f 626a 6563 7429 3a0a 2020 2020  SB(object):.    
+00001f10: 2020 2020 2320 3634 2062 6974 2061 7272      # 64 bit arr
+00001f20: 6179 2074 6f20 7365 6e64 2074 6f20 5553  ay to send to US
+00001f30: 420a 2020 2020 2020 2020 636d 6431 203d  B.        cmd1 =
+00001f40: 205b 302c 2030 2c20 302c 2030 2c20 302c   [0, 0, 0, 0, 0,
+00001f50: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00001f60: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
+00001f70: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
+00001f80: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00001f90: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
+00001fa0: 2c20 302c 2030 2c20 302c 0a20 2020 2020  , 0, 0, 0,.     
+00001fb0: 2020 2020 2020 2020 2020 2030 2c20 302c             0, 0,
+00001fc0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00001fd0: 302c 2030 2c20 302c 2030 2c20 302c 2030  0, 0, 0, 0, 0, 0
+00001fe0: 2c20 302c 2030 2c20 302c 2030 2c20 302c  , 0, 0, 0, 0, 0,
+00001ff0: 2030 2c20 302c 2030 2c20 302c 2030 2c20   0, 0, 0, 0, 0, 
+00002000: 302c 2030 2c20 302c 2030 2c20 302c 0a20  0, 0, 0, 0, 0,. 
+00002010: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00002020: 5d20 2023 2036 3420 6269 7420 6172 7261  ]  # 64 bit arra
+00002030: 7920 746f 2073 656e 6420 746f 2055 5342  y to send to USB
+00002040: 0a0a 2020 2020 2020 2020 6465 6620 5f5f  ..        def __
+00002050: 696e 6974 5f5f 2873 656c 6629 3a0a 2020  init__(self):.  
+00002060: 2020 2020 2020 2020 2020 2320 6669 6e64            # find
+00002070: 2074 6865 2064 6576 6963 650a 2020 2020   the device.    
+00002080: 2020 2020 2020 2020 7365 6c66 2e64 6576          self.dev
+00002090: 203d 2075 7362 2e63 6f72 652e 6669 6e64   = usb.core.find
+000020a0: 2869 6456 656e 646f 723d 3078 3230 6365  (idVendor=0x20ce
+000020b0: 2c20 6964 5072 6f64 7563 743d 3078 3030  , idProduct=0x00
+000020c0: 3233 290a 2020 2020 2020 2020 2020 2020  23).            
+000020d0: 2320 7761 7320 6974 2066 6f75 6e64 3f0a  # was it found?.
+000020e0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000020f0: 656c 662e 6465 7620 6973 204e 6f6e 653a  elf.dev is None:
+00002100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002110: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00002120: 7228 2744 6576 6963 6520 6e6f 7420 666f  r('Device not fo
+00002130: 756e 6427 290a 2020 2020 2020 2020 2020  und').          
+00002140: 2020 2320 7365 7420 7468 6520 6163 7469    # set the acti
+00002150: 7665 2063 6f6e 6669 6775 7261 7469 6f6e  ve configuration
+00002160: 2e20 7769 7468 206e 6f20 6172 6773 2077  . with no args w
+00002170: 6520 7573 6520 6669 7273 7420 636f 6e66  e use first conf
+00002180: 6967 2e0a 2020 2020 2020 2020 2020 2020  ig..            
+00002190: 2320 2066 6f72 204c 696e 7578 206f 6e6c  #  for Linux onl
+000021a0: 790a 2020 2020 2020 2020 2020 2020 6966  y.            if
+000021b0: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
+000021c0: 2027 6c69 6e75 7827 3a0a 0a20 2020 2020   'linux':..     
+000021d0: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
+000021e0: 6f6e 6669 6775 7261 7469 6f6e 2069 6e20  onfiguration in 
+000021f0: 7365 6c66 2e64 6576 3a0a 2020 2020 2020  self.dev:.      
+00002200: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00002210: 7220 696e 7465 7266 6163 6520 696e 2063  r interface in c
+00002220: 6f6e 6669 6775 7261 7469 6f6e 3a0a 2020  onfiguration:.  
+00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002240: 2020 2020 2020 6966 6e75 6d20 3d20 696e        ifnum = in
+00002250: 7465 7266 6163 652e 6249 6e74 6572 6661  terface.bInterfa
+00002260: 6365 4e75 6d62 6572 0a20 2020 2020 2020  ceNumber.       
+00002270: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002280: 6e6f 7420 7365 6c66 2e64 6576 2e69 735f  not self.dev.is_
+00002290: 6b65 726e 656c 5f64 7269 7665 725f 6163  kernel_driver_ac
+000022a0: 7469 7665 2869 666e 756d 293a 0a20 2020  tive(ifnum):.   
+000022b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022c0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000022f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00002300: 2070 7269 6e74 2022 6465 7461 6368 206b   print "detach k
+00002310: 6572 6e65 6c20 6472 6976 6572 2066 726f  ernel driver fro
+00002320: 6d20 6465 7669 6365 2025 733a 2069 6e74  m device %s: int
+00002330: 6572 6661 6365 2025 7322 2025 2028 6465  erface %s" % (de
+00002340: 762c 2069 666e 756d 290a 2020 2020 2020  v, ifnum).      
+00002350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002360: 2020 7365 6c66 2e64 6576 2e64 6574 6163    self.dev.detac
+00002370: 685f 6b65 726e 656c 5f64 7269 7665 7228  h_kernel_driver(
+00002380: 6966 6e75 6d29 0a20 2020 2020 2020 2020  ifnum).         
+00002390: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+000023a0: 7420 7573 622e 636f 7265 2e55 5342 4572  t usb.core.USBEr
+000023b0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+000023c0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+000023d0: 730a 0a20 2020 2020 2020 2020 2020 2073  s..            s
+000023e0: 656c 662e 6465 762e 7365 745f 636f 6e66  elf.dev.set_conf
+000023f0: 6967 7572 6174 696f 6e28 290a 2020 2020  iguration().    
+00002400: 2020 2020 2020 2020 7365 6c66 2e63 6d64          self.cmd
+00002410: 315b 305d 203d 2034 310a 2020 2020 2020  1[0] = 41.      
+00002420: 2020 2020 2020 7365 6c66 2e64 6576 2e77        self.dev.w
+00002430: 7269 7465 2830 7830 312c 2073 656c 662e  rite(0x01, self.
+00002440: 636d 6431 2920 2023 2053 4e0a 2020 2020  cmd1)  # SN.    
+00002450: 2020 2020 2020 2020 7320 3d20 7365 6c66          s = self
+00002460: 2e64 6576 2e72 6561 6428 3078 3831 2c20  .dev.read(0x81, 
+00002470: 3634 290a 2020 2020 2020 2020 2020 2020  64).            
+00002480: 7365 6c66 2e53 6572 6961 6c4e 756d 6265  self.SerialNumbe
+00002490: 7220 3d20 2222 0a20 2020 2020 2020 2020  r = "".         
+000024a0: 2020 2069 203d 2031 0a20 2020 2020 2020     i = 1.       
+000024b0: 2020 2020 2077 6869 6c65 2028 735b 695d       while (s[i]
+000024c0: 203e 2030 293a 0a20 2020 2020 2020 2020   > 0):.         
+000024d0: 2020 2020 2020 2073 656c 662e 5365 7269         self.Seri
+000024e0: 616c 4e75 6d62 6572 203d 2073 656c 662e  alNumber = self.
+000024f0: 5365 7269 616c 4e75 6d62 6572 202b 2063  SerialNumber + c
+00002500: 6872 2873 5b69 5d29 0a20 2020 2020 2020  hr(s[i]).       
+00002510: 2020 2020 2020 2020 2069 203d 2069 202b           i = i +
+00002520: 2031 0a20 2020 2020 2020 2020 2020 2073   1.            s
+00002530: 656c 662e 636d 6431 5b30 5d20 3d20 3430  elf.cmd1[0] = 40
+00002540: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002550: 662e 6465 762e 7772 6974 6528 3078 3031  f.dev.write(0x01
+00002560: 2c20 7365 6c66 2e63 6d64 3129 2020 2320  , self.cmd1)  # 
+00002570: 4d6f 6465 6c0a 2020 2020 2020 2020 2020  Model.          
+00002580: 2020 7320 3d20 7365 6c66 2e64 6576 2e72    s = self.dev.r
+00002590: 6561 6428 3078 3831 2c20 3634 290a 2020  ead(0x81, 64).  
+000025a0: 2020 2020 2020 2020 2020 7365 6c66 2e4d            self.M
+000025b0: 6f64 656c 4e61 6d65 203d 2022 220a 2020  odelName = "".  
+000025c0: 2020 2020 2020 2020 2020 6920 3d20 310a            i = 1.
+000025d0: 2020 2020 2020 2020 2020 2020 7768 696c              whil
+000025e0: 6520 2873 5b69 5d20 3e20 3029 3a0a 2020  e (s[i] > 0):.  
+000025f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00002600: 6c66 2e4d 6f64 656c 4e61 6d65 203d 2073  lf.ModelName = s
+00002610: 656c 662e 4d6f 6465 6c4e 616d 6520 2b20  elf.ModelName + 
+00002620: 6368 7228 735b 695d 290a 2020 2020 2020  chr(s[i]).      
+00002630: 2020 2020 2020 2020 2020 6920 3d20 6920            i = i 
+00002640: 2b20 310a 0a20 2020 2020 2020 2020 2020  + 1..           
+00002650: 2073 656c 662e 4d61 7869 6d75 6d5f 4174   self.Maximum_At
+00002660: 746e 203d 2066 6c6f 6174 2873 656c 662e  tn = float(self.
+00002670: 4d6f 6465 6c4e 616d 655b 3131 3a5d 290a  ModelName[11:]).
+00002680: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002690: 2e63 6d64 315b 305d 203d 2039 390a 2020  .cmd1[0] = 99.  
+000026a0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000026b0: 6576 2e77 7269 7465 2830 7830 312c 2073  ev.write(0x01, s
+000026c0: 656c 662e 636d 6431 2920 2023 2046 570a  elf.cmd1)  # FW.
+000026d0: 2020 2020 2020 2020 2020 2020 7320 3d20              s = 
+000026e0: 7365 6c66 2e64 6576 2e72 6561 6428 3078  self.dev.read(0x
+000026f0: 3831 2c20 3634 290a 2020 2020 2020 2020  81, 64).        
+00002700: 2020 2020 7365 6c66 2e46 5720 3d20 2222      self.FW = ""
+00002710: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002720: 662e 4657 203d 2063 6872 2873 5b35 5d29  f.FW = chr(s[5])
+00002730: 202b 2063 6872 2873 5b36 5d29 0a20 2020   + chr(s[6]).   
+00002740: 2020 2020 2020 2020 2073 656c 662e 7374           self.st
+00002750: 6174 7573 5f6d 6573 7361 6765 203d 2027  atus_message = '
+00002760: 466f 756e 6420 4174 7465 6e75 6174 6f72  Found Attenuator
+00002770: 3a20 4d6f 6465 6c20 7b7d 2c20 534e 3a20  : Model {}, SN: 
+00002780: 7b7d 202c 2046 573a 207b 7d2c 204d 6178  {} , FW: {}, Max
+00002790: 696d 756d 2061 7474 656e 7561 7469 6f6e  imum attenuation
+000027a0: 3a20 7b7d 6442 2027 2e66 6f72 6d61 7428  : {}dB '.format(
+000027b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000027c0: 2073 7472 2873 656c 662e 4d6f 6465 6c4e   str(self.ModelN
+000027d0: 616d 6529 2c20 7374 7228 7365 6c66 2e53  ame), str(self.S
+000027e0: 6572 6961 6c4e 756d 6265 7229 2c20 7374  erialNumber), st
+000027f0: 7228 7365 6c66 2e46 5729 2c20 7374 7228  r(self.FW), str(
+00002800: 7365 6c66 2e4d 6178 696d 756d 5f41 7474  self.Maximum_Att
+00002810: 6e29 290a 2020 2020 2020 2020 2020 2020  n)).            
+00002820: 7072 696e 7428 7365 6c66 2e73 7461 7475  print(self.statu
+00002830: 735f 6d65 7373 6167 6529 0a0a 2020 2020  s_message)..    
+00002840: 2020 2020 6465 6620 5265 6164 534e 2873      def ReadSN(s
+00002850: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
+00002860: 2020 7265 7475 726e 2073 7472 2873 656c    return str(sel
+00002870: 662e 5365 7269 616c 4e75 6d62 6572 290a  f.SerialNumber).
+00002880: 0a20 2020 2020 2020 2064 6566 2052 6561  .        def Rea
+00002890: 644d 4e28 7365 6c66 293a 0a20 2020 2020  dMN(self):.     
+000028a0: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
+000028b0: 7228 7365 6c66 2e4d 6f64 656c 4e61 6d65  r(self.ModelName
+000028c0: 290a 0a20 2020 2020 2020 2064 6566 2052  )..        def R
+000028d0: 6561 6446 5728 7365 6c66 293a 0a20 2020  eadFW(self):.   
+000028e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000028f0: 7374 7228 7365 6c66 2e46 5729 0a0a 2020  str(self.FW)..  
+00002900: 2020 2020 2020 6465 6620 5265 6164 4d61        def ReadMa
+00002910: 7852 616e 6765 2873 656c 6629 3a0a 2020  xRange(self):.  
+00002920: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002930: 2073 656c 662e 4d61 7869 6d75 6d5f 4174   self.Maximum_At
+00002940: 746e 0a0a 2020 2020 2020 2020 6465 6620  tn..        def 
+00002950: 5365 7461 7474 6e28 7365 6c66 2c20 4174  Setattn(self, At
+00002960: 746e 293a 0a20 2020 2020 2020 2020 2020  tn):.           
+00002970: 2073 656c 662e 636d 6431 5b30 5d20 3d20   self.cmd1[0] = 
+00002980: 3139 0a20 2020 2020 2020 2020 2020 2073  19.            s
+00002990: 656c 662e 636d 6431 5b31 5d20 3d20 696e  elf.cmd1[1] = in
+000029a0: 7428 4174 746e 290a 2020 2020 2020 2020  t(Attn).        
+000029b0: 2020 2020 7365 6c66 2e63 6d64 315b 325d      self.cmd1[2]
+000029c0: 203d 2069 6e74 2828 4174 746e 202d 2069   = int((Attn - i
+000029d0: 6e74 2841 7474 6e29 2920 2a20 3429 0a20  nt(Attn)) * 4). 
+000029e0: 2020 2020 2020 2020 2020 2069 6620 4174             if At
+000029f0: 746e 203e 2073 656c 662e 4d61 7869 6d75  tn > self.Maximu
+00002a00: 6d5f 4174 746e 3a0a 2020 2020 2020 2020  m_Attn:.        
+00002a10: 2020 2020 2020 2020 7072 696e 7428 2741          print('A
+00002a20: 7474 656e 7561 7469 6f6e 206e 6f74 2069  ttenuation not i
+00002a30: 6e20 5261 6e67 652c 7365 7474 696e 6720  n Range,setting 
+00002a40: 6d61 7869 6d75 6d20 3d20 7b7d 2027 2e66  maximum = {} '.f
+00002a50: 6f72 6d61 7428 7374 7228 7365 6c66 2e4d  ormat(str(self.M
+00002a60: 6178 696d 756d 5f41 7474 6e29 2929 0a20  aximum_Attn))). 
+00002a70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002a80: 656c 662e 636d 6431 5b31 5d20 3d20 696e  elf.cmd1[1] = in
+00002a90: 7428 7365 6c66 2e4d 6178 696d 756d 5f41  t(self.Maximum_A
+00002aa0: 7474 6e29 0a20 2020 2020 2020 2020 2020  ttn).           
+00002ab0: 2020 2020 2073 656c 662e 636d 6431 5b32       self.cmd1[2
+00002ac0: 5d20 3d20 696e 7428 2873 656c 662e 4d61  ] = int((self.Ma
+00002ad0: 7869 6d75 6d5f 4174 746e 202d 2069 6e74  ximum_Attn - int
+00002ae0: 2873 656c 662e 4d61 7869 6d75 6d5f 4174  (self.Maximum_At
+00002af0: 746e 2929 202a 2034 290a 2020 2020 2020  tn)) * 4).      
+00002b00: 2020 2020 2020 2320 7365 6c66 2e64 6576        # self.dev
+00002b10: 2e73 6574 5f63 6f6e 6669 6775 7261 7469  .set_configurati
+00002b20: 6f6e 2829 0a0a 2020 2020 2020 2020 2020  on()..          
+00002b30: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00002b40: 2020 2020 2020 2073 656c 662e 6465 762e         self.dev.
+00002b50: 7772 6974 6528 3078 3031 2c20 7365 6c66  write(0x01, self
+00002b60: 2e63 6d64 3129 2020 2320 5365 7420 6174  .cmd1)  # Set at
+00002b70: 7465 6e75 6174 696f 6e0a 2020 2020 2020  tenuation.      
+00002b80: 2020 2020 2020 2020 2020 7320 3d20 7365            s = se
+00002b90: 6c66 2e64 6576 2e72 6561 6428 3078 3831  lf.dev.read(0x81
+00002ba0: 2c20 3634 290a 2020 2020 2020 2020 2020  , 64).          
+00002bb0: 2020 2020 2020 7365 6c66 2e6e 6577 5f61        self.new_a
+00002bc0: 7474 203d 2027 5365 7474 696e 6720 4174  tt = 'Setting At
+00002bd0: 7465 6e75 6174 696f 6e20 3d20 7b7d 6442  tenuation = {}dB
+00002be0: 2027 2e66 6f72 6d61 7428 7374 7228 735b   '.format(str(s[
+00002bf0: 315d 202b 2073 5b32 5d20 2f20 3429 290a  1] + s[2] / 4)).
+00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c10: 7072 696e 7428 7365 6c66 2e6e 6577 5f61  print(self.new_a
+00002c20: 7474 290a 2020 2020 2020 2020 2020 2020  tt).            
+00002c30: 2020 2020 7265 7475 726e 2073 5b31 5d20      return s[1] 
+00002c40: 2b20 735b 325d 202f 2034 0a20 2020 2020  + s[2] / 4.     
+00002c50: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00002c60: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+00002c70: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00002c80: 696e 7428 6529 0a20 2020 2020 2020 2020  int(e).         
+00002c90: 2020 2020 2020 2073 656c 662e 6e65 775f         self.new_
+00002ca0: 6174 7420 3d20 650a 2020 2020 2020 2020  att = e.        
+00002cb0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00002cc0: 0a0a 2020 2020 2020 2020 6465 6620 4765  ..        def Ge
+00002cd0: 7461 7474 6e28 7365 6c66 293a 0a20 2020  tattn(self):.   
+00002ce0: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00002cf0: 6465 762e 7365 745f 636f 6e66 6967 7572  dev.set_configur
+00002d00: 6174 696f 6e28 290a 2020 2020 2020 2020  ation().        
+00002d10: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00002d20: 2020 2020 2020 2020 2073 656c 662e 636d           self.cm
+00002d30: 6431 5b30 5d20 3d20 3138 0a20 2020 2020  d1[0] = 18.     
+00002d40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002d50: 6465 762e 7772 6974 6528 3078 3031 2c20  dev.write(0x01, 
+00002d60: 7365 6c66 2e63 6d64 3129 2020 2320 4765  self.cmd1)  # Ge
+00002d70: 7420 6174 7465 6e75 6174 7469 6f6e 0a20  t attenuattion. 
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00002d90: 203d 2073 656c 662e 6465 762e 7265 6164   = self.dev.read
+00002da0: 2830 7838 312c 2036 3429 0a20 2020 2020  (0x81, 64).     
+00002db0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002dc0: 6e65 775f 6174 7420 3d20 2743 7572 7265  new_att = 'Curre
+00002dd0: 6e74 2041 7474 656e 7561 7469 6f6e 203d  nt Attenuation =
+00002de0: 207b 7d64 4220 272e 666f 726d 6174 2873   {}dB '.format(s
+00002df0: 7472 2873 5b31 5d20 2b20 735b 325d 202f  tr(s[1] + s[2] /
+00002e00: 2034 2929 0a20 2020 2020 2020 2020 2020   4)).           
+00002e10: 2020 2020 2070 7269 6e74 2873 656c 662e       print(self.
+00002e20: 6e65 775f 6174 7429 0a20 2020 2020 2020  new_att).       
+00002e30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00002e40: 735b 315d 202b 2073 5b32 5d20 2f20 340a  s[1] + s[2] / 4.
+00002e50: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00002e60: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00002e70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00002e80: 2020 2070 7269 6e74 2865 290a 2020 2020     print(e).    
+00002e90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002ea0: 2e6e 6577 5f61 7474 203d 2065 0a20 2020  .new_att = e.   
+00002eb0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00002ec0: 7572 6e20 730a 0a20 2020 2020 2020 2064  urn s..        d
+00002ed0: 6566 2053 656e 645f 5343 5049 2873 656c  ef Send_SCPI(sel
+00002ee0: 662c 2053 4350 4963 6d64 2c20 746d 7029  f, SCPIcmd, tmp)
+00002ef0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00002f00: 7365 6e64 2053 4350 4920 636f 6d6d 616e  send SCPI comman
+00002f10: 6473 2028 746f 2073 7570 706f 7274 6564  ds (to supported
+00002f20: 2066 6972 6d77 6172 6520 6f6e 6c79 2129   firmware only!)
+00002f30: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002f40: 662e 636d 6431 5b30 5d20 3d20 3432 0a20  f.cmd1[0] = 42. 
+00002f50: 2020 2020 2020 2020 2020 206c 3120 3d20             l1 = 
+00002f60: 300a 2020 2020 2020 2020 2020 2020 6c31  0.            l1
+00002f70: 203d 206c 656e 2853 4350 4963 6d64 290a   = len(SCPIcmd).
+00002f80: 2020 2020 2020 2020 2020 2020 696e 6478              indx
+00002f90: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+00002fa0: 2077 6869 6c65 2028 696e 6478 203c 3d20   while (indx <= 
+00002fb0: 6c31 293a 0a20 2020 2020 2020 2020 2020  l1):.           
+00002fc0: 2020 2020 2073 656c 662e 636d 6431 5b69       self.cmd1[i
+00002fd0: 6e64 785d 203d 206f 7264 2853 4350 4963  ndx] = ord(SCPIc
+00002fe0: 6d64 5b69 6e64 7820 2d20 315d 290a 2020  md[indx - 1]).  
+00002ff0: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00003000: 6478 203d 2069 6e64 7820 2b20 310a 2020  dx = indx + 1.  
+00003010: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00003020: 6d64 315b 696e 6478 5d20 3d20 300a 2020  md1[indx] = 0.  
+00003030: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+00003040: 6576 2e77 7269 7465 2830 7830 312c 2073  ev.write(0x01, s
+00003050: 656c 662e 636d 6431 2920 2023 2053 4350  elf.cmd1)  # SCP
+00003060: 2043 6f6d 6d61 6e64 2075 7020 746f 2036   Command up to 6
+00003070: 3020 6368 6172 733b 0a20 2020 2020 2020  0 chars;.       
+00003080: 2020 2020 2073 203d 2073 656c 662e 6465       s = self.de
+00003090: 762e 7265 6164 2830 7838 312c 2036 3429  v.read(0x81, 64)
+000030a0: 0a20 2020 2020 2020 2020 2020 2069 203d  .            i =
+000030b0: 2031 0a20 2020 2020 2020 2020 2020 2052   1.            R
+000030c0: 6574 5374 7220 3d20 2222 0a20 2020 2020  etStr = "".     
+000030d0: 2020 2020 2020 2077 6869 6c65 2028 735b         while (s[
+000030e0: 695d 203e 2030 293a 0a20 2020 2020 2020  i] > 0):.       
+000030f0: 2020 2020 2020 2020 2052 6574 5374 7220           RetStr 
+00003100: 3d20 5265 7453 7472 202b 2063 6872 2873  = RetStr + chr(s
+00003110: 5b69 5d29 0a20 2020 2020 2020 2020 2020  [i]).           
+00003120: 2020 2020 2069 203d 2069 202b 2031 0a20       i = i + 1. 
+00003130: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00003140: 6e20 7374 7228 5265 7453 7472 290a 0a20  n str(RetStr).. 
+00003150: 2020 2063 6c61 7373 2041 5049 286f 626a     class API(obj
+00003160: 6563 7429 3a0a 0a20 2020 2020 2020 2064  ect):..        d
+00003170: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00003180: 2c20 636f 6d70 6f72 743d 2241 5554 4f22  , comport="AUTO"
+00003190: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+000031a0: 656c 662e 6261 7564 7261 7465 203d 2039  elf.baudrate = 9
+000031b0: 3630 300a 2020 2020 2020 2020 2020 2020  600.            
+000031c0: 6966 2063 6f6d 706f 7274 203d 3d20 2241  if comport == "A
+000031d0: 5554 4f22 3a0a 2020 2020 2020 2020 2020  UTO":.          
+000031e0: 2020 2020 2020 706f 7274 735f 6c69 7374        ports_list
+000031f0: 203d 2073 6572 6961 6c5f 706f 7274 7328   = serial_ports(
+00003200: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003210: 2020 666f 7220 706f 7274 2069 6e20 706f    for port in po
+00003220: 7274 735f 6c69 7374 3a0a 2020 2020 2020  rts_list:.      
+00003230: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003240: 6c66 2e63 6f6d 706f 7274 203d 2070 6f72  lf.comport = por
+00003250: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00003260: 2020 2020 2020 7365 6c66 2e73 203d 2073        self.s = s
+00003270: 6572 6961 6c2e 5365 7269 616c 2873 656c  erial.Serial(sel
+00003280: 662e 636f 6d70 6f72 742c 2073 656c 662e  f.comport, self.
+00003290: 6261 7564 7261 7465 2c20 7469 6d65 6f75  baudrate, timeou
+000032a0: 743d 302e 3529 0a20 2020 2020 2020 2020  t=0.5).         
+000032b0: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+000032c0: 2831 290a 2020 2020 2020 2020 2020 2020  (1).            
+000032d0: 2020 2020 2020 2020 7365 6c66 2e73 2e66          self.s.f
+000032e0: 6c75 7368 496e 7075 7428 290a 2020 2020  lushInput().    
+000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003300: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
+00003310: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+00003320: 2020 2020 2020 2020 2073 6c65 6570 2830           sleep(0
+00003330: 2e31 290a 2020 2020 2020 2020 2020 2020  .1).            
+00003340: 2020 2020 2020 2020 2320 5475 726e 2074          # Turn t
+00003350: 6865 2063 6f6e 736f 6c65 206f 6666 0a20  he console off. 
+00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003370: 2020 2073 656c 662e 732e 7772 6974 6528     self.s.write(
+00003380: 2243 4f4e 534f 4c45 2044 4953 4142 4c45  "CONSOLE DISABLE
+00003390: 5c72 5c6e 222e 656e 636f 6465 2829 290a  \r\n".encode()).
+000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033b0: 2020 2020 2320 466c 7573 6820 7468 6520      # Flush the 
+000033c0: 6275 6666 6572 730a 2020 2020 2020 2020  buffers.        
+000033d0: 2020 2020 2020 2020 2020 2020 736c 6565              slee
+000033e0: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
+000033f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003400: 732e 666c 7573 6828 290a 2020 2020 2020  s.flush().      
+00003410: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003420: 6c66 2e73 2e66 6c75 7368 496e 7075 7428  lf.s.flushInput(
+00003430: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003440: 2020 2020 2020 7365 6c66 2e73 2e66 6c75        self.s.flu
+00003450: 7368 4f75 7470 7574 2829 0a20 2020 2020  shOutput().     
+00003460: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003470: 656c 662e 732e 7772 6974 6528 222a 4944  elf.s.write("*ID
+00003480: 4e3f 5c72 5c6e 222e 656e 636f 6465 2829  N?\r\n".encode()
+00003490: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000034a0: 2020 2020 2020 736c 6565 7028 302e 3129        sleep(0.1)
+000034b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000034c0: 2020 2020 2069 6620 7365 6c66 2e73 2e69       if self.s.i
+000034d0: 6e5f 7761 6974 696e 6720 3e20 313a 0a20  n_waiting > 1:. 
+000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000034f0: 2020 2020 2020 2072 6573 7020 3d20 7365         resp = se
+00003500: 6c66 2e73 2e72 6561 646c 696e 6528 292e  lf.s.readline().
+00003510: 6465 636f 6465 2822 7574 662d 3822 290a  decode("utf-8").
+00003520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003530: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
 00003540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003550: 2020 2020 2020 7265 7370 203d 2073 656c        resp = sel
-00003560: 662e 732e 7265 6164 6c69 6e65 2829 2e64  f.s.readline().d
-00003570: 6563 6f64 6528 2275 7466 2d38 2229 0a20  ecode("utf-8"). 
-00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003590: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000035a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035b0: 2072 6573 7020 3d20 2727 0a20 2020 2020   resp = ''.     
-000035c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000035d0: 656c 662e 6d6f 6465 6c20 3d20 7265 7370  elf.model = resp
-000035e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000035f0: 2020 2020 2069 6620 2822 4165 726f 666c       if ("Aerofl
-00003600: 6578 2220 696e 2072 6573 7029 3a0a 2020  ex" in resp):.  
-00003610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003620: 2020 2020 2020 7072 696e 7428 2746 6f75        print('Fou
-00003630: 6e64 2027 202b 2072 6573 702e 7374 7269  nd ' + resp.stri
-00003640: 7028 275c 725c 6e27 2920 2b20 2720 6f6e  p('\r\n') + ' on
-00003650: 2070 6f72 743a 2027 202b 2070 6f72 7429   port: ' + port)
-00003660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003670: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-00003680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003690: 2020 2065 6c69 6620 2738 3331 3127 2069     elif '8311' i
-000036a0: 6e20 7265 7370 206f 7220 2738 3333 3127  n resp or '8331'
-000036b0: 2069 6e20 7265 7370 3a0a 2020 2020 2020   in resp:.      
-000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036d0: 2020 7072 696e 7428 2746 6f75 6e64 2027    print('Found '
-000036e0: 202b 2072 6573 702e 7374 7269 7028 275c   + resp.strip('\
-000036f0: 725c 6e27 2920 2b20 2720 6f6e 2070 6f72  r\n') + ' on por
-00003700: 743a 2027 202b 2070 6f72 7429 0a20 2020  t: ' + port).   
-00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003720: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00003730: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00003740: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-00003750: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00003760: 2020 2020 2020 7365 6c66 2e73 203d 2073        self.s = s
-00003770: 6572 6961 6c2e 5365 7269 616c 2863 6f6d  erial.Serial(com
-00003780: 706f 7274 2c20 7365 6c66 2e62 6175 6472  port, self.baudr
-00003790: 6174 652c 2074 696d 656f 7574 3d30 2e35  ate, timeout=0.5
-000037a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000037b0: 2020 736c 6565 7028 3129 0a20 2020 2020    sleep(1).     
-000037c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000037d0: 732e 7772 6974 6528 2243 4f4e 534f 4c45  s.write("CONSOLE
-000037e0: 2044 4953 4142 4c45 5c72 5c6e 222e 656e   DISABLE\r\n".en
-000037f0: 636f 6465 2829 290a 2020 2020 2020 2020  code()).        
-00003800: 2020 2020 2020 2020 2320 466c 7573 6820          # Flush 
-00003810: 7468 6520 6275 6666 6572 730a 2020 2020  the buffers.    
-00003820: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003830: 2e73 2e66 6c75 7368 2829 0a20 2020 2020  .s.flush().     
-00003840: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003850: 732e 666c 7573 6849 6e70 7574 2829 0a20  s.flushInput(). 
-00003860: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003870: 656c 662e 732e 666c 7573 684f 7574 7075  elf.s.flushOutpu
-00003880: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00003890: 2020 2020 7365 6c66 2e51 7565 7279 2822      self.Query("
-000038a0: 2a49 444e 3f5c 725c 6e22 290a 2020 2020  *IDN?\r\n").    
-000038b0: 2020 2020 2020 2020 2020 2020 7265 7370              resp
-000038c0: 203d 2073 656c 662e 5175 6572 7928 222a   = self.Query("*
-000038d0: 4944 4e3f 5c72 5c6e 2229 0a20 2020 2020  IDN?\r\n").     
-000038e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000038f0: 6d6f 6465 6c20 3d20 7265 7370 0a20 2020  model = resp.   
-00003900: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00003910: 2822 4165 726f 666c 6578 2220 696e 2072  ("Aeroflex" in r
-00003920: 6573 7029 206f 7220 2822 3432 3035 2220  esp) or ("4205" 
-00003930: 696e 2072 6573 7029 3a0a 2020 2020 2020  in resp):.      
-00003940: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00003950: 696e 7428 2746 6f75 6e64 2027 202b 2072  int('Found ' + r
-00003960: 6573 702e 7374 7269 7028 275c 725c 6e27  esp.strip('\r\n'
-00003970: 2920 2b20 2720 6f6e 2070 6f72 743a 2027  ) + ' on port: '
-00003980: 202b 2063 6f6d 706f 7274 290a 2020 2020   + comport).    
-00003990: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000039a0: 2027 3833 3131 2720 696e 2072 6573 7020   '8311' in resp 
-000039b0: 6f72 2027 3833 3331 2720 696e 2072 6573  or '8331' in res
-000039c0: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-000039d0: 2020 2020 2020 2070 7269 6e74 2827 466f         print('Fo
-000039e0: 756e 6420 2720 2b20 7265 7370 2e73 7472  und ' + resp.str
-000039f0: 6970 2827 5c72 5c6e 2729 202b 2027 206f  ip('\r\n') + ' o
-00003a00: 6e20 706f 7274 3a20 2720 2b20 636f 6d70  n port: ' + comp
-00003a10: 6f72 7429 0a20 2020 2020 2020 2020 2020  ort).           
-00003a20: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00003a30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003a40: 656c 662e 636c 6f73 655f 706f 7274 2829  elf.close_port()
-00003a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003a60: 2020 2020 2070 7269 6e74 2827 4165 726f       print('Aero
-00003a70: 666c 6578 2041 7474 656e 7561 746f 7220  flex Attenuator 
-00003a80: 6e6f 7420 666f 756e 6420 6f6e 2073 656c  not found on sel
-00003a90: 6563 7465 6420 706f 7274 2c20 6368 6563  ected port, chec
-00003aa0: 6b20 636f 6e6e 6563 7469 6f6e 272c 2066  k connection', f
-00003ab0: 696c 653d 7379 732e 7374 6465 7272 290a  ile=sys.stderr).
-00003ac0: 0a20 2020 2020 2020 2064 6566 2057 7269  .        def Wri
-00003ad0: 7465 2873 656c 662c 2063 6d64 2c20 7761  te(self, cmd, wa
-00003ae0: 6974 3d46 616c 7365 293a 0a20 2020 2020  it=False):.     
-00003af0: 2020 2020 2020 2022 2222 5365 6e64 2074         """Send t
-00003b00: 6865 2069 6e70 7574 2063 6d64 2073 7472  he input cmd str
-00003b10: 696e 6720 7669 6120 434f 4d20 536f 636b  ing via COM Sock
-00003b20: 6574 2222 220a 2020 2020 2020 2020 2020  et""".          
-00003b30: 2020 6966 2073 656c 662e 732e 6973 4f70    if self.s.isOp
-00003b40: 656e 2829 3a0a 2020 2020 2020 2020 2020  en():.          
-00003b50: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
-00003b60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00003b70: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003b80: 662e 732e 6f70 656e 2829 0a20 2020 2020  f.s.open().     
-00003b90: 2020 2020 2020 2073 656c 662e 732e 666c         self.s.fl
-00003ba0: 7573 6849 6e70 7574 2829 0a20 2020 2020  ushInput().     
-00003bb0: 2020 2020 2020 2073 6c65 6570 2831 290a         sleep(1).
-00003bc0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00003bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003be0: 2073 656c 662e 732e 7772 6974 6528 7374   self.s.write(st
-00003bf0: 722e 656e 636f 6465 2863 6d64 2929 0a20  r.encode(cmd)). 
-00003c00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00003c10: 6c65 6570 2830 2e31 2920 2023 2043 6f6d  leep(0.1)  # Com
-00003c20: 6d61 6e64 7320 6d61 7920 6265 206c 6f73  mands may be los
-00003c30: 7420 7768 656e 2077 7269 7469 6e67 2074  t when writing t
-00003c40: 6f6f 2066 6173 740a 0a20 2020 2020 2020  oo fast..       
-00003c50: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-00003c60: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00003c70: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
-00003c80: 7365 6c66 2e73 2e63 6c6f 7365 2829 0a0a  self.s.close()..
-00003c90: 2020 2020 2020 2020 6465 6620 5175 6572          def Quer
-00003ca0: 7928 7365 6c66 2c20 636d 6429 3a0a 2020  y(self, cmd):.  
-00003cb0: 2020 2020 2020 2020 2020 2222 2253 656e            """Sen
-00003cc0: 6420 7468 6520 696e 7075 7420 636d 6420  d the input cmd 
-00003cd0: 7374 7269 6e67 2076 6961 2043 4f4d 2053  string via COM S
-00003ce0: 6f63 6b65 7420 616e 6420 7265 7475 726e  ocket and return
-00003cf0: 2074 6865 2072 6570 6c79 2073 7472 696e   the reply strin
-00003d00: 6722 2222 0a20 2020 2020 2020 2020 2020  g""".           
-00003d10: 2069 6620 7365 6c66 2e73 2e69 734f 7065   if self.s.isOpe
-00003d20: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
-00003d30: 2020 2020 2070 6173 730a 2020 2020 2020       pass.      
-00003d40: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00003d50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003d60: 2e73 2e6f 7065 6e28 290a 2020 2020 2020  .s.open().      
-00003d70: 2020 2020 2020 2020 2020 736c 6565 7028            sleep(
-00003d80: 302e 3129 0a20 2020 2020 2020 2020 2020  0.1).           
-00003d90: 2023 2073 656c 662e 732e 666c 7573 6849   # self.s.flushI
-00003da0: 6e70 7574 2829 0a20 2020 2020 2020 2020  nput().         
-00003db0: 2020 2073 6c65 6570 2831 290a 2020 2020     sleep(1).    
-00003dc0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00003dd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003de0: 662e 732e 7772 6974 6528 636d 642e 656e  f.s.write(cmd.en
-00003df0: 636f 6465 2829 290a 2020 2020 2020 2020  code()).        
-00003e00: 2020 2020 2020 2020 736c 6565 7028 302e          sleep(0.
-00003e10: 3129 0a20 2020 2020 2020 2020 2020 2020  1).             
-00003e20: 2020 2069 6620 7365 6c66 2e73 2e69 6e5f     if self.s.in_
-00003e30: 7761 6974 696e 6720 3e20 303a 0a20 2020  waiting > 0:.   
-00003e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e50: 2064 6174 6120 3d20 7365 6c66 2e73 2e72   data = self.s.r
-00003e60: 6561 646c 696e 6528 292e 6465 636f 6465  eadline().decode
-00003e70: 2822 7574 662d 3822 290a 2020 2020 2020  ("utf-8").      
-00003e80: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00003e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ea0: 2020 2020 6461 7461 203d 2027 270a 2020      data = ''.  
-00003eb0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-00003ec0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00003ed0: 2020 6461 7461 203d 2027 270a 2020 2020    data = ''.    
-00003ee0: 2020 2020 2020 2020 2320 7365 6c66 2e73          # self.s
-00003ef0: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
-00003f00: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
-00003f10: 0a0a 2020 2020 2020 2020 6465 6620 636c  ..        def cl
-00003f20: 6f73 655f 706f 7274 2873 656c 6629 3a0a  ose_port(self):.
-00003f30: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00003f40: 656c 662e 7320 6973 206e 6f74 204e 6f6e  elf.s is not Non
-00003f50: 6520 616e 6420 7365 6c66 2e73 2e69 734f  e and self.s.isO
-00003f60: 7065 6e28 293a 0a20 2020 2020 2020 2020  pen():.         
-00003f70: 2020 2020 2020 2073 656c 662e 732e 636c         self.s.cl
-00003f80: 6f73 6528 290a 0a20 2020 2020 2020 2064  ose()..        d
-00003f90: 6566 2069 735f 6f70 656e 2873 656c 662c  ef is_open(self,
-00003fa0: 2063 6865 636b 5f70 6f72 743d 4661 6c73   check_port=Fals
-00003fb0: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00003fc0: 6966 2073 656c 662e 7320 6973 206e 6f74  if self.s is not
-00003fd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00003fe0: 2020 2020 2020 2069 6620 6368 6563 6b5f         if check_
-00003ff0: 706f 7274 3a0a 2020 2020 2020 2020 2020  port:.          
-00004000: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
-00004010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004020: 2020 2020 2020 2073 656c 662e 5175 6572         self.Quer
-00004030: 7928 222a 4944 4e3f 5c72 5c6e 2229 0a20  y("*IDN?\r\n"). 
-00004040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004050: 2020 2020 2020 2072 6573 7020 3d20 7365         resp = se
-00004060: 6c66 2e51 7565 7279 2822 2a49 444e 3f5c  lf.Query("*IDN?\
-00004070: 725c 6e22 290a 2020 2020 2020 2020 2020  r\n").          
-00004080: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004090: 6c66 2e6d 6f64 656c 203d 2072 6573 700a  lf.model = resp.
+00003550: 2020 7265 7370 203d 2027 270a 2020 2020    resp = ''.    
+00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003570: 7365 6c66 2e6d 6f64 656c 203d 2072 6573  self.model = res
+00003580: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
+00003590: 2020 2020 2020 6966 2028 2241 6572 6f66        if ("Aerof
+000035a0: 6c65 7822 2069 6e20 7265 7370 293a 0a20  lex" in resp):. 
+000035b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035c0: 2020 2020 2020 2070 7269 6e74 2827 466f         print('Fo
+000035d0: 756e 6420 2720 2b20 7265 7370 2e73 7472  und ' + resp.str
+000035e0: 6970 2827 5c72 5c6e 2729 202b 2027 206f  ip('\r\n') + ' o
+000035f0: 6e20 706f 7274 3a20 2720 2b20 706f 7274  n port: ' + port
+00003600: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003610: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003630: 2020 2020 656c 6966 2027 3833 3131 2720      elif '8311' 
+00003640: 696e 2072 6573 7020 6f72 2027 3833 3331  in resp or '8331
+00003650: 2720 696e 2072 6573 703a 0a20 2020 2020  ' in resp:.     
+00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003670: 2020 2070 7269 6e74 2827 466f 756e 6420     print('Found 
+00003680: 2720 2b20 7265 7370 2e73 7472 6970 2827  ' + resp.strip('
+00003690: 5c72 5c6e 2729 202b 2027 206f 6e20 706f  \r\n') + ' on po
+000036a0: 7274 3a20 2720 2b20 706f 7274 290a 2020  rt: ' + port).  
+000036b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036e0: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+000036f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00003700: 2020 2020 2020 2073 656c 662e 7320 3d20         self.s = 
+00003710: 7365 7269 616c 2e53 6572 6961 6c28 636f  serial.Serial(co
+00003720: 6d70 6f72 742c 2073 656c 662e 6261 7564  mport, self.baud
+00003730: 7261 7465 2c20 7469 6d65 6f75 743d 302e  rate, timeout=0.
+00003740: 3529 0a20 2020 2020 2020 2020 2020 2020  5).             
+00003750: 2020 2073 6c65 6570 2831 290a 2020 2020     sleep(1).    
+00003760: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003770: 2e73 2e77 7269 7465 2822 434f 4e53 4f4c  .s.write("CONSOL
+00003780: 4520 4449 5341 424c 455c 725c 6e22 2e65  E DISABLE\r\n".e
+00003790: 6e63 6f64 6528 2929 0a20 2020 2020 2020  ncode()).       
+000037a0: 2020 2020 2020 2020 2023 2046 6c75 7368           # Flush
+000037b0: 2074 6865 2062 7566 6665 7273 0a20 2020   the buffers.   
+000037c0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000037d0: 662e 732e 666c 7573 6828 290a 2020 2020  f.s.flush().    
+000037e0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000037f0: 2e73 2e66 6c75 7368 496e 7075 7428 290a  .s.flushInput().
+00003800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003810: 7365 6c66 2e73 2e66 6c75 7368 4f75 7470  self.s.flushOutp
+00003820: 7574 2829 0a20 2020 2020 2020 2020 2020  ut().           
+00003830: 2020 2020 2073 656c 662e 5175 6572 7928       self.Query(
+00003840: 222a 4944 4e3f 5c72 5c6e 2229 0a20 2020  "*IDN?\r\n").   
+00003850: 2020 2020 2020 2020 2020 2020 2072 6573               res
+00003860: 7020 3d20 7365 6c66 2e51 7565 7279 2822  p = self.Query("
+00003870: 2a49 444e 3f5c 725c 6e22 290a 2020 2020  *IDN?\r\n").    
+00003880: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00003890: 2e6d 6f64 656c 203d 2072 6573 700a 2020  .model = resp.  
+000038a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000038b0: 2028 2241 6572 6f66 6c65 7822 2069 6e20   ("Aeroflex" in 
+000038c0: 7265 7370 2920 6f72 2028 2234 3230 3522  resp) or ("4205"
+000038d0: 2069 6e20 7265 7370 293a 0a20 2020 2020   in resp):.     
+000038e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000038f0: 7269 6e74 2827 466f 756e 6420 2720 2b20  rint('Found ' + 
+00003900: 7265 7370 2e73 7472 6970 2827 5c72 5c6e  resp.strip('\r\n
+00003910: 2729 202b 2027 206f 6e20 706f 7274 3a20  ') + ' on port: 
+00003920: 2720 2b20 636f 6d70 6f72 7429 0a20 2020  ' + comport).   
+00003930: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00003940: 6620 2738 3331 3127 2069 6e20 7265 7370  f '8311' in resp
+00003950: 206f 7220 2738 3333 3127 2069 6e20 7265   or '8331' in re
+00003960: 7370 3a0a 2020 2020 2020 2020 2020 2020  sp:.            
+00003970: 2020 2020 2020 2020 7072 696e 7428 2746          print('F
+00003980: 6f75 6e64 2027 202b 2072 6573 702e 7374  ound ' + resp.st
+00003990: 7269 7028 275c 725c 6e27 2920 2b20 2720  rip('\r\n') + ' 
+000039a0: 6f6e 2070 6f72 743a 2027 202b 2063 6f6d  on port: ' + com
+000039b0: 706f 7274 290a 2020 2020 2020 2020 2020  port).          
+000039c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039e0: 7365 6c66 2e63 6c6f 7365 5f70 6f72 7428  self.close_port(
+000039f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003a00: 2020 2020 2020 7072 696e 7428 2741 6572        print('Aer
+00003a10: 6f66 6c65 7820 4174 7465 6e75 6174 6f72  oflex Attenuator
+00003a20: 206e 6f74 2066 6f75 6e64 206f 6e20 7365   not found on se
+00003a30: 6c65 6374 6564 2070 6f72 742c 2063 6865  lected port, che
+00003a40: 636b 2063 6f6e 6e65 6374 696f 6e27 2c20  ck connection', 
+00003a50: 6669 6c65 3d73 7973 2e73 7464 6572 7229  file=sys.stderr)
+00003a60: 0a0a 2020 2020 2020 2020 6465 6620 5772  ..        def Wr
+00003a70: 6974 6528 7365 6c66 2c20 636d 642c 2077  ite(self, cmd, w
+00003a80: 6169 743d 4661 6c73 6529 3a0a 2020 2020  ait=False):.    
+00003a90: 2020 2020 2020 2020 2222 2253 656e 6420          """Send 
+00003aa0: 7468 6520 696e 7075 7420 636d 6420 7374  the input cmd st
+00003ab0: 7269 6e67 2076 6961 2043 4f4d 2053 6f63  ring via COM Soc
+00003ac0: 6b65 7422 2222 0a20 2020 2020 2020 2020  ket""".         
+00003ad0: 2020 2069 6620 7365 6c66 2e73 2e69 734f     if self.s.isO
+00003ae0: 7065 6e28 293a 0a20 2020 2020 2020 2020  pen():.         
+00003af0: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
+00003b00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00003b10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003b20: 6c66 2e73 2e6f 7065 6e28 290a 2020 2020  lf.s.open().    
+00003b30: 2020 2020 2020 2020 7365 6c66 2e73 2e66          self.s.f
+00003b40: 6c75 7368 496e 7075 7428 290a 2020 2020  lushInput().    
+00003b50: 2020 2020 2020 2020 736c 6565 7028 3129          sleep(1)
+00003b60: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00003b70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003b80: 2020 7365 6c66 2e73 2e77 7269 7465 2873    self.s.write(s
+00003b90: 7472 2e65 6e63 6f64 6528 636d 6429 290a  tr.encode(cmd)).
+00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bb0: 736c 6565 7028 302e 3129 2020 2320 436f  sleep(0.1)  # Co
+00003bc0: 6d6d 616e 6473 206d 6179 2062 6520 6c6f  mmands may be lo
+00003bd0: 7374 2077 6865 6e20 7772 6974 696e 6720  st when writing 
+00003be0: 746f 6f20 6661 7374 0a0a 2020 2020 2020  too fast..      
+00003bf0: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
+00003c00: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00003c10: 7373 0a20 2020 2020 2020 2020 2020 2023  ss.            #
+00003c20: 2073 656c 662e 732e 636c 6f73 6528 290a   self.s.close().
+00003c30: 0a20 2020 2020 2020 2064 6566 2051 7565  .        def Que
+00003c40: 7279 2873 656c 662c 2063 6d64 293a 0a20  ry(self, cmd):. 
+00003c50: 2020 2020 2020 2020 2020 2022 2222 5365             """Se
+00003c60: 6e64 2074 6865 2069 6e70 7574 2063 6d64  nd the input cmd
+00003c70: 2073 7472 696e 6720 7669 6120 434f 4d20   string via COM 
+00003c80: 536f 636b 6574 2061 6e64 2072 6574 7572  Socket and retur
+00003c90: 6e20 7468 6520 7265 706c 7920 7374 7269  n the reply stri
+00003ca0: 6e67 2222 220a 2020 2020 2020 2020 2020  ng""".          
+00003cb0: 2020 6966 2073 656c 662e 732e 6973 4f70    if self.s.isOp
+00003cc0: 656e 2829 3a0a 2020 2020 2020 2020 2020  en():.          
+00003cd0: 2020 2020 2020 7061 7373 0a20 2020 2020        pass.     
+00003ce0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00003cf0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00003d00: 662e 732e 6f70 656e 2829 0a20 2020 2020  f.s.open().     
+00003d10: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+00003d20: 2830 2e31 290a 2020 2020 2020 2020 2020  (0.1).          
+00003d30: 2020 2320 7365 6c66 2e73 2e66 6c75 7368    # self.s.flush
+00003d40: 496e 7075 7428 290a 2020 2020 2020 2020  Input().        
+00003d50: 2020 2020 736c 6565 7028 3129 0a20 2020      sleep(1).   
+00003d60: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
+00003d70: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00003d80: 6c66 2e73 2e77 7269 7465 2863 6d64 2e65  lf.s.write(cmd.e
+00003d90: 6e63 6f64 6528 2929 0a20 2020 2020 2020  ncode()).       
+00003da0: 2020 2020 2020 2020 2073 6c65 6570 2830           sleep(0
+00003db0: 2e31 290a 2020 2020 2020 2020 2020 2020  .1).            
+00003dc0: 2020 2020 6966 2073 656c 662e 732e 696e      if self.s.in
+00003dd0: 5f77 6169 7469 6e67 203e 2030 3a0a 2020  _waiting > 0:.  
+00003de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003df0: 2020 6461 7461 203d 2073 656c 662e 732e    data = self.s.
+00003e00: 7265 6164 6c69 6e65 2829 2e64 6563 6f64  readline().decod
+00003e10: 6528 2275 7466 2d38 2229 0a20 2020 2020  e("utf-8").     
+00003e20: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00003e30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003e40: 2020 2020 2064 6174 6120 3d20 2727 0a20       data = ''. 
+00003e50: 2020 2020 2020 2020 2020 2065 7863 6570             excep
+00003e60: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00003e70: 2020 2064 6174 6120 3d20 2727 0a20 2020     data = ''.   
+00003e80: 2020 2020 2020 2020 2023 2073 656c 662e           # self.
+00003e90: 732e 636c 6f73 6528 290a 2020 2020 2020  s.close().      
+00003ea0: 2020 2020 2020 7265 7475 726e 2064 6174        return dat
+00003eb0: 610a 0a20 2020 2020 2020 2064 6566 2063  a..        def c
+00003ec0: 6c6f 7365 5f70 6f72 7428 7365 6c66 293a  lose_port(self):
+00003ed0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003ee0: 7365 6c66 2e73 2069 7320 6e6f 7420 4e6f  self.s is not No
+00003ef0: 6e65 2061 6e64 2073 656c 662e 732e 6973  ne and self.s.is
+00003f00: 4f70 656e 2829 3a0a 2020 2020 2020 2020  Open():.        
+00003f10: 2020 2020 2020 2020 7365 6c66 2e73 2e63          self.s.c
+00003f20: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
+00003f30: 6465 6620 6973 5f6f 7065 6e28 7365 6c66  def is_open(self
+00003f40: 2c20 6368 6563 6b5f 706f 7274 3d46 616c  , check_port=Fal
+00003f50: 7365 293a 0a20 2020 2020 2020 2020 2020  se):.           
+00003f60: 2069 6620 7365 6c66 2e73 2069 7320 6e6f   if self.s is no
+00003f70: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00003f80: 2020 2020 2020 2020 6966 2063 6865 636b          if check
+00003f90: 5f70 6f72 743a 0a20 2020 2020 2020 2020  _port:.         
+00003fa0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00003fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003fc0: 2020 2020 2020 2020 7365 6c66 2e51 7565          self.Que
+00003fd0: 7279 2822 2a49 444e 3f5c 725c 6e22 290a  ry("*IDN?\r\n").
+00003fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ff0: 2020 2020 2020 2020 7265 7370 203d 2073          resp = s
+00004000: 656c 662e 5175 6572 7928 222a 4944 4e3f  elf.Query("*IDN?
+00004010: 5c72 5c6e 2229 0a20 2020 2020 2020 2020  \r\n").         
+00004020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004030: 656c 662e 6d6f 6465 6c20 3d20 7265 7370  elf.model = resp
+00004040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004050: 2020 2020 2020 2020 2069 6620 2822 4165           if ("Ae
+00004060: 726f 666c 6578 2220 696e 2072 6573 7029  roflex" in resp)
+00004070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004080: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00004090: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
 000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040b0: 2020 2020 2020 2020 6966 2028 2241 6572          if ("Aer
-000040c0: 6f66 6c65 7822 2069 6e20 7265 7370 293a  oflex" in resp):
-000040d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000040e0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000040f0: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
-00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004110: 2065 6c69 6620 2738 3331 3127 2069 6e20   elif '8311' in 
-00004120: 7265 7370 206f 7220 2738 3333 3127 2069  resp or '8331' i
-00004130: 6e20 7265 7370 3a0a 2020 2020 2020 2020  n resp:.        
-00004140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004150: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+000040b0: 2020 656c 6966 2027 3833 3131 2720 696e    elif '8311' in
+000040c0: 2072 6573 7020 6f72 2027 3833 3331 2720   resp or '8331' 
+000040d0: 696e 2072 6573 703a 0a20 2020 2020 2020  in resp:.       
+000040e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040f0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00004100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004110: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004130: 2020 2020 2073 656c 662e 636c 6f73 655f       self.close_
+00004140: 706f 7274 2829 0a20 2020 2020 2020 2020  port().         
+00004150: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
 00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004170: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
-00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004190: 2020 2020 7365 6c66 2e63 6c6f 7365 5f70      self.close_p
-000041a0: 6f72 7428 290a 2020 2020 2020 2020 2020  ort().          
-000041b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041d0: 7265 7475 726e 2073 656c 662e 732e 6973  return self.s.is
-000041e0: 4f70 656e 2829 0a20 2020 2020 2020 2020  Open().         
-000041f0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00004200: 0a20 2020 2020 2020 2064 6566 2053 6574  .        def Set
-00004210: 6174 746e 2873 656c 662c 2061 7474 6e29  attn(self, attn)
-00004220: 3a0a 2020 2020 2020 2020 2020 2020 636d  :.            cm
-00004230: 6420 3d20 2241 5454 4e20 7b3a 2e32 667d  d = "ATTN {:.2f}
-00004240: 5c72 5c6e 222e 666f 726d 6174 2861 7474  \r\n".format(att
-00004250: 6e29 0a20 2020 2020 2020 2020 2020 2073  n).            s
-00004260: 656c 662e 5772 6974 6528 636d 6429 0a20  elf.Write(cmd). 
-00004270: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00004280: 203d 2073 656c 662e 4765 7461 7474 6e28   = self.Getattn(
-00004290: 290a 2020 2020 2020 2020 2020 2020 7661  ).            va
-000042a0: 6c75 6520 3d20 666c 6f61 7428 7661 6c75  lue = float(valu
-000042b0: 6529 0a20 2020 2020 2020 2020 2020 2069  e).            i
-000042c0: 6620 7661 6c75 6520 213d 2061 7474 6e3a  f value != attn:
-000042d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000042e0: 2070 7269 6e74 2866 2745 7272 6f72 2073   print(f'Error s
-000042f0: 6574 7469 6e67 2061 7474 656e 7561 7469  etting attenuati
-00004300: 6f6e 3a20 6e65 7720 3a20 7b61 7474 6e7d  on: new : {attn}
-00004310: 2063 7572 7265 6e74 3a20 7b76 616c 7565   current: {value
-00004320: 7d27 290a 2020 2020 2020 2020 2020 2020  }').            
-00004330: 7265 7475 726e 2076 616c 7565 0a0a 2020  return value..  
-00004340: 2020 2020 2020 6465 6620 4765 7461 7474        def Getatt
-00004350: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-00004360: 2020 2020 2063 6d64 203d 2022 4154 544e       cmd = "ATTN
-00004370: 3f5c 725c 6e22 0a20 2020 2020 2020 2020  ?\r\n".         
-00004380: 2020 2076 616c 7565 203d 2073 656c 662e     value = self.
-00004390: 5175 6572 7928 636d 6429 0a20 2020 2020  Query(cmd).     
-000043a0: 2020 2020 2020 2072 6574 7572 6e20 7661         return va
-000043b0: 6c75 650a 0a0a 636c 6173 7320 5465 7363  lue...class Tesc
-000043c0: 6f6d 3a0a 2020 2020 2222 220a 2020 2020  om:.    """.    
-000043d0: 436f 6e74 726f 6c20 5445 5343 4f4d 2074  Control TESCOM t
-000043e0: 6573 7469 6e67 2063 6861 6d62 6572 730a  esting chambers.
-000043f0: 2020 2020 2222 220a 2020 2020 6f70 656e      """.    open
-00004400: 5f63 6d64 203d 2062 274f 5045 4e5c 7227  _cmd = b'OPEN\r'
-00004410: 0a20 2020 2063 6c6f 7365 5f63 6d64 203d  .    close_cmd =
-00004420: 2062 2743 4c4f 5345 5c72 270a 2020 2020   b'CLOSE\r'.    
-00004430: 636f 6d5f 706f 7274 5f6f 626a 203d 204e  com_port_obj = N
-00004440: 6f6e 650a 2020 2020 6d6f 6465 6c73 5f6c  one.    models_l
-00004450: 6973 7420 3d20 5b27 5443 2d35 3036 3443  ist = ['TC-5064C
-00004460: 272c 2027 5441 2d37 3031 3141 5027 2c20  ', 'TA-7011AP', 
-00004470: 2754 432d 3530 3633 4127 2c20 2754 432d  'TC-5063A', 'TC-
-00004480: 3539 3730 4350 275d 0a0a 2020 2020 6465  5970CP']..    de
-00004490: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-000044a0: 2070 6f72 743d 4e6f 6e65 293a 0a20 2020   port=None):.   
-000044b0: 2020 2020 2073 656c 662e 706f 7274 203d       self.port =
-000044c0: 2070 6f72 740a 2020 2020 2020 2020 7472   port.        tr
-000044d0: 793a 0a20 2020 2020 2020 2020 2020 2069  y:.            i
-000044e0: 6620 706f 7274 2069 7320 6e6f 7420 4e6f  f port is not No
-000044f0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00004500: 2020 2020 7365 6c66 2e63 6f6e 6e65 6374      self.connect
-00004510: 2870 6f72 7429 0a0a 2020 2020 2020 2020  (port)..        
-00004520: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00004530: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-00004540: 2020 2070 7269 6e74 2865 290a 2020 2020     print(e).    
-00004550: 2020 2020 2020 2020 7072 696e 7428 2254          print("T
-00004560: 6573 636f 6d20 2d20 436f 6e6e 6563 7469  escom - Connecti
-00004570: 6f6e 2066 6169 6c65 6422 290a 0a20 2020  on failed")..   
-00004580: 2064 6566 2063 6f6e 6e65 6374 2873 656c   def connect(sel
-00004590: 662c 2070 6f72 7429 3a0a 2020 2020 2020  f, port):.      
-000045a0: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-000045b0: 6172 616d 2070 6f72 743a 2063 6f6d 2070  aram port: com p
-000045c0: 6f72 7420 746f 2063 6f6e 6e65 6374 0a20  ort to connect. 
-000045d0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-000045e0: 636f 6d20 706f 7274 206f 626a 0a20 2020  com port obj.   
-000045f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00004600: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00004610: 2020 636f 6d5f 706f 7274 5f6f 626a 203d    com_port_obj =
-00004620: 2073 656c 662e 636f 6d5f 706f 7274 5f6f   self.com_port_o
-00004630: 626a 203d 2073 6572 6961 6c2e 5365 7269  bj = serial.Seri
-00004640: 616c 2870 6f72 743d 706f 7274 2c20 6261  al(port=port, ba
-00004650: 7564 7261 7465 3d39 3630 302c 2074 696d  udrate=9600, tim
-00004660: 656f 7574 3d31 290a 2020 2020 2020 2020  eout=1).        
-00004670: 2020 2020 6966 2063 6f6d 5f70 6f72 745f      if com_port_
-00004680: 6f62 6a20 6973 206e 6f74 204e 6f6e 653a  obj is not None:
-00004690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000046a0: 2073 656c 662e 646f 6f72 5f63 6d64 203d   self.door_cmd =
-000046b0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-000046c0: 2020 2020 2020 7365 6c66 2e63 6f6d 5f70        self.com_p
-000046d0: 6f72 745f 6f62 6a2e 7772 6974 6528 6227  ort_obj.write(b'
-000046e0: 4d4f 4445 4c3f 5c72 2729 0a20 2020 2020  MODEL?\r').     
-000046f0: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
-00004700: 2830 2e31 290a 2020 2020 2020 2020 2020  (0.1).          
-00004710: 2020 2020 2020 6d6f 6465 6c20 3d20 7374        model = st
-00004720: 7228 7365 6c66 2e63 6f6d 5f70 6f72 745f  r(self.com_port_
-00004730: 6f62 6a2e 7265 6164 2831 3429 290a 2020  obj.read(14)).  
-00004740: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00004750: 7274 7320 3d20 5b70 2066 6f72 2070 2069  rts = [p for p i
-00004760: 6e20 6d6f 6465 6c2e 7370 6c69 7428 2227  n model.split("'
-00004770: 2229 5d0a 2020 2020 2020 2020 2020 2020  ")].            
-00004780: 2020 2020 7061 7274 7320 3d20 5b70 2066      parts = [p f
-00004790: 6f72 2070 2069 6e20 7061 7274 735b 315d  or p in parts[1]
-000047a0: 2e73 706c 6974 2822 2022 295d 0a20 2020  .split(" ")].   
-000047b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000047c0: 662e 6d6f 6465 6c20 3d20 7061 7274 735b  f.model = parts[
-000047d0: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
-000047e0: 2020 2069 6620 6c65 6e28 7365 6c66 2e6d     if len(self.m
-000047f0: 6f64 656c 2920 3e20 303a 0a20 2020 2020  odel) > 0:.     
-00004800: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00004810: 7269 6e74 2822 5246 2063 6861 6d62 6572  rint("RF chamber
-00004820: 2063 6f6e 6e65 6374 6564 2074 6f20 706f   connected to po
-00004830: 7274 2022 202b 2073 7472 2870 6f72 7429  rt " + str(port)
-00004840: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004850: 2020 2020 2020 7072 696e 7428 2254 6573        print("Tes
-00004860: 636f 6d20 2d20 4368 616d 6265 7220 6d6f  com - Chamber mo
-00004870: 6465 6c3a 222c 2073 656c 662e 6d6f 6465  del:", self.mode
-00004880: 6c29 0a20 2020 2020 2020 2020 2020 2020  l).             
-00004890: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000048a0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000048b0: 6e74 2822 5465 7363 6f6d 202d 2045 7272  nt("Tescom - Err
-000048c0: 6f72 2120 4e6f 2063 6861 6d62 6572 2066  or! No chamber f
-000048d0: 6f75 6e64 2229 0a20 2020 2020 2020 2020  ound").         
-000048e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000048f0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00004900: 2020 6966 2073 656c 662e 6d6f 6465 6c20    if self.model 
-00004910: 696e 2073 656c 662e 6d6f 6465 6c73 5f6c  in self.models_l
-00004920: 6973 743a 0a20 2020 2020 2020 2020 2020  ist:.           
-00004930: 2020 2020 2020 2020 2073 656c 662e 646f           self.do
-00004940: 6f72 5f63 6d64 203d 2062 2744 4f4f 523f  or_cmd = b'DOOR?
-00004950: 5c72 270a 2020 2020 2020 2020 2020 2020  \r'.            
-00004960: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00004970: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00004980: 6c66 2e64 6f6f 725f 636d 6420 3d20 6227  lf.door_cmd = b'
-00004990: 4c49 443f 5c72 270a 2020 2020 2020 2020  LID?\r'.        
-000049a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000049b0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000049c0: 4578 6365 7074 696f 6e0a 2020 2020 2020  Exception.      
-000049d0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-000049e0: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-000049f0: 2020 2020 2023 2070 7269 6e74 2865 290a       # print(e).
-00004a00: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00004a10: 7428 2822 5465 7363 6f6d 202d 2043 6f75  t(("Tescom - Cou
-00004a20: 6c64 206e 6f74 2063 6f6e 6e65 6374 2074  ld not connect t
-00004a30: 6f20 706f 7274 2022 202b 2070 6f72 7429  o port " + port)
-00004a40: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00004a50: 7475 726e 204e 6f6e 650a 0a20 2020 2064  turn None..    d
-00004a60: 6566 2063 6c6f 7365 5f70 6f72 7428 7365  ef close_port(se
-00004a70: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00004a80: 0a20 2020 2020 2020 2063 6c6f 7365 7320  .        closes 
-00004a90: 636f 6d20 706f 7274 0a20 2020 2020 2020  com port.       
-00004aa0: 2022 2222 0a20 2020 2020 2020 2074 7279   """.        try
-00004ab0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00004ac0: 6c66 2e63 6f6d 5f70 6f72 745f 6f62 6a2e  lf.com_port_obj.
-00004ad0: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
-00004ae0: 2020 2020 7072 696e 7428 2252 4620 6368      print("RF ch
-00004af0: 616d 6265 7220 6469 7363 6f6e 6e65 6374  amber disconnect
-00004b00: 6564 2066 726f 6d20 706f 7274 3a20 2220  ed from port: " 
-00004b10: 2b20 7374 7228 7365 6c66 2e70 6f72 7429  + str(self.port)
-00004b20: 290a 2020 2020 2020 2020 6578 6365 7074  ).        except
-00004b30: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00004b40: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00004b50: 6e74 2822 436f 756c 6420 6e6f 7420 6469  nt("Could not di
-00004b60: 7363 6f6e 6e65 6374 2229 0a0a 2020 2020  sconnect")..    
-00004b70: 6465 6620 6f70 656e 5f63 6861 6d62 6572  def open_chamber
-00004b80: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00004b90: 2222 220a 2020 2020 2020 2020 6f70 656e  """.        open
-00004ba0: 7320 6368 616d 6265 720a 2020 2020 2020  s chamber.      
-00004bb0: 2020 3a72 6574 7572 6e3a 2022 4f4b 2220    :return: "OK" 
-00004bc0: 6966 2063 6f6d 6d61 6e64 2077 6173 2073  if command was s
-00004bd0: 7563 6365 7373 6675 6c0a 2020 2020 2020  uccessful.      
-00004be0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-00004bf0: 2073 656c 662e 6973 5f64 6f6f 725f 6f70   self.is_door_op
-00004c00: 656e 2829 3a0a 2020 2020 2020 2020 2020  en():.          
-00004c10: 2020 7072 696e 7428 2243 6861 6d62 6572    print("Chamber
-00004c20: 2069 7320 6f70 656e 2229 0a20 2020 2020   is open").     
-00004c30: 2020 2020 2020 2072 6574 7572 6e20 274f         return 'O
-00004c40: 4b27 0a20 2020 2020 2020 2074 7279 3a0a  K'.        try:.
-00004c50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00004c60: 7428 6622 4368 616d 6265 7220 7b73 656c  t(f"Chamber {sel
-00004c70: 662e 706f 7274 7d20 6973 206f 7065 6e69  f.port} is openi
-00004c80: 6e67 2229 0a20 2020 2020 2020 2020 2020  ng").           
-00004c90: 2073 656c 662e 636f 6d5f 706f 7274 5f6f   self.com_port_o
-00004ca0: 626a 2e72 6573 6574 5f69 6e70 7574 5f62  bj.reset_input_b
-00004cb0: 7566 6665 7228 290a 2020 2020 2020 2020  uffer().        
-00004cc0: 2020 2020 7365 6c66 2e63 6f6d 5f70 6f72      self.com_por
-00004cd0: 745f 6f62 6a2e 7265 7365 745f 6f75 7470  t_obj.reset_outp
-00004ce0: 7574 5f62 7566 6665 7228 290a 2020 2020  ut_buffer().    
-00004cf0: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
-00004d00: 5f70 6f72 745f 6f62 6a2e 7772 6974 6528  _port_obj.write(
-00004d10: 7365 6c66 2e6f 7065 6e5f 636d 6429 0a20  self.open_cmd). 
-00004d20: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00004d30: 2027 270a 2020 2020 2020 2020 2020 2020   ''.            
-00004d40: 7761 6974 5f63 6f75 6e74 6572 203d 2030  wait_counter = 0
-00004d50: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
-00004d60: 6c65 2027 4f4b 2720 6e6f 7420 696e 2072  le 'OK' not in r
-00004d70: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00004d80: 2020 2020 6966 2077 6169 745f 636f 756e      if wait_coun
-00004d90: 7465 7220 3e3d 2031 353a 0a20 2020 2020  ter >= 15:.     
-00004da0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004db0: 6169 7365 2045 7863 6570 7469 6f6e 2866  aise Exception(f
-00004dc0: 2245 7272 6f72 2069 6e20 6f70 656e 696e  "Error in openin
-00004dd0: 6720 6368 616d 6265 7220 7b73 656c 662e  g chamber {self.
-00004de0: 706f 7274 7d22 290a 2020 2020 2020 2020  port}").        
-00004df0: 2020 2020 2020 2020 7265 7320 3d20 7365          res = se
-00004e00: 6c66 2e63 6f6d 5f70 6f72 745f 6f62 6a2e  lf.com_port_obj.
-00004e10: 7265 6164 2831 3429 2e64 6563 6f64 6528  read(14).decode(
-00004e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004e30: 2020 2020 2027 7574 662d 3827 292e 7570       'utf-8').up
-00004e40: 7065 7228 292e 7273 7472 6970 2827 5c72  per().rstrip('\r
-00004e50: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-00004e60: 2020 2069 6620 6c65 6e28 7374 7228 7265     if len(str(re
-00004e70: 7329 2920 3e20 303a 0a20 2020 2020 2020  s)) > 0:.       
-00004e80: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00004e90: 6e74 2866 2743 6861 6d62 6572 207b 7365  nt(f'Chamber {se
-00004ea0: 6c66 2e70 6f72 747d 2073 7461 7475 733a  lf.port} status:
-00004eb0: 2027 202b 2073 7472 2872 6573 2929 0a20   ' + str(res)). 
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00004ed0: 6169 745f 636f 756e 7465 7220 2b3d 2031  ait_counter += 1
-00004ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ef0: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
-00004f00: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-00004f10: 656c 662e 6973 5f64 6f6f 725f 6f70 656e  elf.is_door_open
-00004f20: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00004f30: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
-00004f40: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-00004f50: 2020 2020 2020 2020 2066 227b 7365 6c66           f"{self
-00004f60: 2e70 6f72 747d 2044 6f6f 7220 7374 6174  .port} Door stat
-00004f70: 7573 2064 6f65 736e 2774 206d 6174 6368  us doesn't match
-00004f80: 2063 6f6d 6d61 6e64 2073 656e 7421 2229   command sent!")
-00004f90: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00004fa0: 6e74 2866 2243 6861 6d62 6572 207b 7365  nt(f"Chamber {se
-00004fb0: 6c66 2e70 6f72 747d 2069 7320 6f70 656e  lf.port} is open
-00004fc0: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-00004fd0: 6574 7572 6e20 274f 4b27 0a20 2020 2020  eturn 'OK'.     
-00004fe0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-00004ff0: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
-00005000: 2020 2020 2020 7072 696e 7428 6529 0a20        print(e). 
-00005010: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00005020: 6e20 2246 4149 4c22 0a0a 2020 2020 6465  n "FAIL"..    de
-00005030: 6620 636c 6f73 655f 6368 616d 6265 7228  f close_chamber(
-00005040: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00005050: 2222 0a20 2020 2020 2020 2063 6c6f 7365  "".        close
-00005060: 7320 6368 616d 6265 720a 2020 2020 2020  s chamber.      
-00005070: 2020 3a72 6574 7572 6e3a 2022 4f4b 2220    :return: "OK" 
-00005080: 6966 2063 6f6d 6d61 6e64 2077 6173 2073  if command was s
-00005090: 7563 6365 7373 6675 6c0a 2020 2020 2020  uccessful.      
-000050a0: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
-000050b0: 2073 656c 662e 6973 5f64 6f6f 725f 636c   self.is_door_cl
-000050c0: 6f73 6564 2829 3a0a 2020 2020 2020 2020  osed():.        
-000050d0: 2020 2020 7072 696e 7428 2243 6861 6d62      print("Chamb
-000050e0: 6572 2063 6c6f 7365 6422 290a 2020 2020  er closed").    
-000050f0: 2020 2020 2020 2020 7265 7475 726e 2027          return '
-00005100: 4f4b 270a 2020 2020 2020 2020 7472 793a  OK'.        try:
-00005110: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00005120: 6e74 2866 2243 4841 4d42 4552 207b 7365  nt(f"CHAMBER {se
-00005130: 6c66 2e70 6f72 747d 2049 5320 434c 4f53  lf.port} IS CLOS
-00005140: 494e 472c 2043 4c45 4152 2048 414e 4453  ING, CLEAR HANDS
-00005150: 2121 2122 290a 2020 2020 2020 2020 2020  !!!").          
-00005160: 2020 736c 6565 7028 3229 0a20 2020 2020    sleep(2).     
-00005170: 2020 2020 2020 2073 656c 662e 636f 6d5f         self.com_
-00005180: 706f 7274 5f6f 626a 2e77 7269 7465 2873  port_obj.write(s
-00005190: 656c 662e 636c 6f73 655f 636d 6429 0a20  elf.close_cmd). 
-000051a0: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-000051b0: 2027 270a 2020 2020 2020 2020 2020 2020   ''.            
-000051c0: 7761 6974 5f63 6f75 6e74 6572 203d 2030  wait_counter = 0
-000051d0: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
-000051e0: 6c65 2027 5245 4144 5927 206e 6f74 2069  le 'READY' not i
-000051f0: 6e20 7265 733a 0a20 2020 2020 2020 2020  n res:.         
-00005200: 2020 2020 2020 2069 6620 7761 6974 5f63         if wait_c
-00005210: 6f75 6e74 6572 203e 3d20 3230 3a0a 2020  ounter >= 20:.  
-00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005230: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00005240: 6e28 6622 4572 726f 7220 696e 2063 6c6f  n(f"Error in clo
-00005250: 7369 6e67 2063 6861 6d62 6572 207b 7365  sing chamber {se
-00005260: 6c66 2e70 6f72 747d 2229 0a20 2020 2020  lf.port}").     
-00005270: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00005280: 2073 656c 662e 636f 6d5f 706f 7274 5f6f   self.com_port_o
-00005290: 626a 2e72 6561 6428 3134 292e 6465 636f  bj.read(14).deco
-000052a0: 6465 280a 2020 2020 2020 2020 2020 2020  de(.            
-000052b0: 2020 2020 2020 2020 2775 7466 2d38 2729          'utf-8')
-000052c0: 2e75 7070 6572 2829 2e72 7374 7269 7028  .upper().rstrip(
-000052d0: 275c 7227 290a 2020 2020 2020 2020 2020  '\r').          
-000052e0: 2020 2020 2020 6966 2027 4552 5227 2069        if 'ERR' i
-000052f0: 6e20 7265 7320 6f72 2027 5245 4144 5927  n res or 'READY'
-00005300: 2069 6e20 7265 7320 6f72 2027 4f4b 2720   in res or 'OK' 
-00005310: 696e 2072 6573 3a0a 2020 2020 2020 2020  in res:.        
-00005320: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00005330: 7428 6627 4368 616d 6265 7220 7b73 656c  t(f'Chamber {sel
-00005340: 662e 706f 7274 7d20 7374 6174 7573 3a20  f.port} status: 
-00005350: 2720 2b20 7374 7228 7265 7329 290a 2020  ' + str(res)).  
-00005360: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005370: 2027 4552 5227 2069 6e20 7265 733a 0a20   'ERR' in res:. 
-00005380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005390: 2020 2072 6574 7572 6e20 2246 4149 4c22     return "FAIL"
-000053a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000053b0: 2077 6169 745f 636f 756e 7465 7220 2b3d   wait_counter +=
-000053c0: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
-000053d0: 2020 2073 6c65 6570 2830 2e31 290a 2020     sleep(0.1).  
-000053e0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-000053f0: 2073 656c 662e 6973 5f64 6f6f 725f 636c   self.is_door_cl
-00005400: 6f73 6564 2829 3a0a 2020 2020 2020 2020  osed():.        
-00005410: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
-00005420: 6365 7074 696f 6e28 0a20 2020 2020 2020  ception(.       
-00005430: 2020 2020 2020 2020 2020 2020 2066 227b               f"{
-00005440: 7365 6c66 2e70 6f72 747d 2044 6f6f 7220  self.port} Door 
-00005450: 7374 6174 7573 2064 6f65 736e 2774 206d  status doesn't m
-00005460: 6174 6368 2063 6f6d 6d61 6e64 2073 656e  atch command sen
-00005470: 7421 2229 0a20 2020 2020 2020 2020 2020  t!").           
-00005480: 2070 7269 6e74 2866 2243 6861 6d62 6572   print(f"Chamber
-00005490: 207b 7365 6c66 2e70 6f72 747d 2063 6c6f   {self.port} clo
-000054a0: 7365 6422 290a 2020 2020 2020 2020 2020  sed").          
-000054b0: 2020 7265 7475 726e 2027 4f4b 270a 2020    return 'OK'.  
-000054c0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-000054d0: 6570 7469 6f6e 2061 7320 653a 0a20 2020  eption as e:.   
-000054e0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
-000054f0: 2245 7272 6f72 2069 6e20 636c 6f73 696e  "Error in closin
-00005500: 6720 6368 616d 6265 7220 7b73 656c 662e  g chamber {self.
-00005510: 706f 7274 7d22 290a 2020 2020 2020 2020  port}").        
-00005520: 2020 2020 7072 696e 7428 6529 0a20 2020      print(e).   
-00005530: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00005540: 2246 4149 4c22 0a0a 2020 2020 6465 6620  "FAIL"..    def 
-00005550: 6973 5f63 6f6e 6e65 6374 6564 2873 656c  is_connected(sel
-00005560: 6629 3a0a 2020 2020 2020 2020 6966 2073  f):.        if s
-00005570: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
-00005580: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00005590: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-000055a0: 7365 0a20 2020 2020 2020 2072 6574 7572  se.        retur
-000055b0: 6e20 7365 6c66 2e63 6f6d 5f70 6f72 745f  n self.com_port_
-000055c0: 6f62 6a2e 6973 4f70 656e 2829 0a0a 2020  obj.isOpen()..  
-000055d0: 2020 6465 6620 6765 745f 7374 6174 6528    def get_state(
-000055e0: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-000055f0: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
-00005600: 2e72 6573 6574 5f69 6e70 7574 5f62 7566  .reset_input_buf
-00005610: 6665 7228 290a 2020 2020 2020 2020 736c  fer().        sl
-00005620: 6565 7028 302e 3129 0a20 2020 2020 2020  eep(0.1).       
-00005630: 2073 656c 662e 636f 6d5f 706f 7274 5f6f   self.com_port_o
-00005640: 626a 2e77 7269 7465 2873 656c 662e 646f  bj.write(self.do
-00005650: 6f72 5f63 6d64 290a 2020 2020 2020 2020  or_cmd).        
-00005660: 736c 6565 7028 302e 3129 0a20 2020 2020  sleep(0.1).     
-00005670: 2020 2073 7461 7465 203d 2073 656c 662e     state = self.
-00005680: 636f 6d5f 706f 7274 5f6f 626a 2e72 6561  com_port_obj.rea
-00005690: 6428 3134 292e 6465 636f 6465 2827 7574  d(14).decode('ut
-000056a0: 662d 3827 292e 7570 7065 7228 292e 7273  f-8').upper().rs
-000056b0: 7472 6970 2827 5c72 2729 0a20 2020 2020  trip('\r').     
-000056c0: 2020 2072 6574 7572 6e20 7374 6174 650a     return state.
-000056d0: 0a20 2020 2064 6566 2069 735f 646f 6f72  .    def is_door
-000056e0: 5f6f 7065 6e28 7365 6c66 293a 0a20 2020  _open(self):.   
-000056f0: 2020 2020 2073 7461 7465 203d 2073 656c       state = sel
-00005700: 662e 6765 745f 7374 6174 6528 290a 2020  f.get_state().  
-00005710: 2020 2020 2020 6966 2027 4f50 454e 2720        if 'OPEN' 
-00005720: 696e 2073 7461 7465 3a0a 2020 2020 2020  in state:.      
-00005730: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00005740: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00005750: 2046 616c 7365 0a0a 2020 2020 6465 6620   False..    def 
-00005760: 6973 5f64 6f6f 725f 636c 6f73 6564 2873  is_door_closed(s
-00005770: 656c 6629 3a0a 2020 2020 2020 2020 7374  elf):.        st
-00005780: 6174 6520 3d20 7365 6c66 2e67 6574 5f73  ate = self.get_s
-00005790: 7461 7465 2829 0a20 2020 2020 2020 2069  tate().        i
-000057a0: 6620 2743 4c4f 5345 2720 696e 2073 7461  f 'CLOSE' in sta
-000057b0: 7465 3a0a 2020 2020 2020 2020 2020 2020  te:.            
-000057c0: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-000057d0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000057e0: 0a0a 0a63 6c61 7373 2042 6172 636f 6465  ...class Barcode
-000057f0: 5363 616e 6e65 723a 0a20 2020 2064 6566  Scanner:.    def
-00005800: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00005810: 636f 6d5f 706f 7274 3a20 7374 7220 3d20  com_port: str = 
-00005820: 4e6f 6e65 2c20 6261 7564 5f72 6174 653a  None, baud_rate:
-00005830: 2069 6e74 203d 2031 3135 3230 302c 2063   int = 115200, c
-00005840: 6f6e 6669 673a 2062 6f6f 6c20 3d20 5472  onfig: bool = Tr
-00005850: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00005860: 2020 2020 206c 6f67 5f74 7970 653a 2073       log_type: s
-00005870: 7472 203d 2027 4e4f 5f4c 4f47 272c 2077  tr = 'NO_LOG', w
-00005880: 7269 7465 5f74 6f5f 6c6f 673a 2062 6f6f  rite_to_log: boo
-00005890: 6c20 3d20 4661 6c73 652c 2074 696d 656f  l = False, timeo
-000058a0: 7574 3a20 7374 7220 3d20 2731 3030 3027  ut: str = '1000'
-000058b0: 2c20 6c6f 675f 6e61 6d65 3a20 7374 7220  , log_name: str 
-000058c0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
-000058d0: 2022 2222 0a20 2020 2020 2020 2049 6e69   """.        Ini
-000058e0: 7469 616c 697a 6520 7468 6520 5152 5363  tialize the QRSc
-000058f0: 616e 6e65 7220 6f62 6a65 6374 2e0a 2020  anner object..  
-00005900: 2020 2020 2020 4461 7461 7368 6565 743a        Datasheet:
-00005910: 0a20 2020 2020 2020 2068 7474 7073 3a2f  .        https:/
-00005920: 2f63 646e 2e72 7473 6361 6e2e 6e65 742f  /cdn.rtscan.net/
-00005930: 7770 2d63 6f6e 7465 6e74 2f75 706c 6f61  wp-content/uploa
-00005940: 6473 2f32 3032 322f 3036 2f55 7365 725f  ds/2022/06/User_
-00005950: 4d61 6e75 616c 5f52 5432 3134 5f52 5432  Manual_RT214_RT2
-00005960: 3137 5f52 5432 3335 5f52 5432 3430 5f32  17_RT235_RT240_2
-00005970: 3032 322e 3035 5f31 2e30 2e36 2e70 6466  022.05_1.0.6.pdf
-00005980: 0a20 2020 2020 2020 2046 6f72 2074 6865  .        For the
-00005990: 2066 6972 7374 2075 7365 2c20 796f 7520   first use, you 
-000059a0: 7769 6c6c 206e 6565 6420 746f 2073 6361  will need to sca
-000059b0: 6e20 3320 6261 7263 6f64 6520 746f 2069  n 3 barcode to i
-000059c0: 6e69 7469 616c 2063 6f6d 706f 7274 2063  nitial comport c
-000059d0: 6f6e 6e65 6374 696f 6e3a 0a20 2020 2020  onnection:.     
-000059e0: 2020 2068 7474 7073 3a2f 2f77 696c 696f     https://wilio
-000059f0: 742e 6174 6c61 7373 6961 6e2e 6e65 742f  t.atlassian.net/
-00005a00: 7769 6b69 2f73 7061 6365 732f 4657 2f70  wiki/spaces/FW/p
-00005a10: 6167 6573 2f32 3536 3630 3239 3430 372f  ages/2566029407/
-00005a20: 5254 7363 616e 2b42 6172 636f 6465 2b53  RTscan+Barcode+S
-00005a30: 6361 6e6e 6572 0a20 2020 2020 2020 2040  canner.        @
-00005a40: 7061 7261 6d20 636f 6d3a 0a20 2020 2020  param com:.     
-00005a50: 2020 2040 7479 7065 2063 6f6d 3a0a 2020     @type com:.  
-00005a60: 2020 2020 2020 4070 6172 616d 2062 6175        @param bau
-00005a70: 643a 0a20 2020 2020 2020 2040 7479 7065  d:.        @type
-00005a80: 2062 6175 643a 0a20 2020 2020 2020 2040   baud:.        @
-00005a90: 7061 7261 6d20 636f 6e66 6967 3a0a 2020  param config:.  
-00005aa0: 2020 2020 2020 4074 7970 6520 636f 6e66        @type conf
-00005ab0: 6967 3a0a 2020 2020 2020 2020 4070 6172  ig:.        @par
-00005ac0: 616d 206c 6f67 5f74 7970 653a 0a20 2020  am log_type:.   
-00005ad0: 2020 2020 2040 7479 7065 206c 6f67 5f74       @type log_t
-00005ae0: 7970 653a 0a20 2020 2020 2020 2040 7061  ype:.        @pa
-00005af0: 7261 6d20 7772 6974 655f 746f 5f6c 6f67  ram write_to_log
-00005b00: 3a0a 2020 2020 2020 2020 4074 7970 6520  :.        @type 
-00005b10: 7772 6974 655f 746f 5f6c 6f67 3a0a 2020  write_to_log:.  
-00005b20: 2020 2020 2020 4070 6172 616d 2074 696d        @param tim
-00005b30: 656f 7574 3a0a 2020 2020 2020 2020 4074  eout:.        @t
-00005b40: 7970 6520 7469 6d65 6f75 743a 0a20 2020  ype timeout:.   
-00005b50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005b60: 2073 656c 662e 7072 6566 6978 203d 2027   self.prefix = '
-00005b70: 7e01 3030 3030 4027 0a20 2020 2020 2020  ~.0000@'.       
-00005b80: 2073 656c 662e 7375 6666 6978 203d 2027   self.suffix = '
-00005b90: 3b03 270a 2020 2020 2020 2020 7365 6c66  ;.'.        self
-00005ba0: 2e63 6f6d 5f70 6f72 7420 3d20 636f 6d5f  .com_port = com_
-00005bb0: 706f 7274 0a20 2020 2020 2020 2073 656c  port.        sel
-00005bc0: 662e 7365 7269 616c 5f63 6f6e 6e65 6374  f.serial_connect
-00005bd0: 696f 6e20 3d20 4e6f 6e65 0a20 2020 2020  ion = None.     
-00005be0: 2020 2073 656c 662e 6465 7669 6365 5f73     self.device_s
-00005bf0: 6967 6e61 7475 7265 203d 2022 4e4c 532d  ignature = "NLS-
-00005c00: 4e31 220a 2020 2020 2020 2020 7365 6c66  N1".        self
-00005c10: 2e6c 6f67 5f74 7970 6520 3d20 6c6f 675f  .log_type = log_
-00005c20: 7479 7065 0a20 2020 2020 2020 2073 656c  type.        sel
-00005c30: 662e 7772 6974 655f 746f 5f6c 6f67 203d  f.write_to_log =
-00005c40: 2077 7269 7465 5f74 6f5f 6c6f 670a 2020   write_to_log.  
-00005c50: 2020 2020 2020 7365 6c66 2e73 6774 696e        self.sgtin
-00005c60: 5f6c 656e 6774 6820 3d20 3331 0a0a 2020  _length = 31..  
-00005c70: 2020 2020 2020 6966 206c 6f67 5f6e 616d        if log_nam
-00005c80: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-00005c90: 2020 2020 2020 2073 656c 662e 7172 5f6c         self.qr_l
-00005ca0: 6f67 6765 7220 3d20 6c6f 6767 696e 672e  ogger = logging.
-00005cb0: 6765 744c 6f67 6765 7228 2751 524c 6f67  getLogger('QRLog
-00005cc0: 6765 7227 290a 2020 2020 2020 2020 656c  ger').        el
-00005cd0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00005ce0: 7365 6c66 2e71 725f 6c6f 6767 6572 203d  self.qr_logger =
-00005cf0: 206c 6f67 6769 6e67 2e67 6574 4c6f 6767   logging.getLogg
-00005d00: 6572 286c 6f67 5f6e 616d 6529 0a0a 2020  er(log_name)..  
-00005d10: 2020 2020 2020 6966 2063 6f6d 5f70 6f72        if com_por
-00005d20: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
-00005d30: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00005d40: 6f70 656e 5f70 6f72 7428 636f 6d5f 706f  open_port(com_po
-00005d50: 7274 2c20 6261 7564 5f72 6174 653d 6261  rt, baud_rate=ba
-00005d60: 7564 5f72 6174 652c 2063 6f6e 6669 673d  ud_rate, config=
-00005d70: 636f 6e66 6967 2c20 7469 6d65 6f75 743d  config, timeout=
-00005d80: 7469 6d65 6f75 7429 0a20 2020 2020 2020  timeout).       
-00005d90: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00005da0: 2020 2073 656c 662e 6175 746f 5f63 6f6e     self.auto_con
-00005db0: 6e65 6374 2874 696d 656f 7574 3d74 696d  nect(timeout=tim
-00005dc0: 656f 7574 290a 0a20 2020 2020 2020 2069  eout)..        i
-00005dd0: 6620 7365 6c66 2e77 7269 7465 5f74 6f5f  f self.write_to_
-00005de0: 6c6f 673a 0a20 2020 2020 2020 2020 2020  log:.           
-00005df0: 2073 656c 662e 6372 6561 7465 5f6c 6f67   self.create_log
-00005e00: 5f66 696c 6528 290a 0a20 2020 2064 6566  _file()..    def
-00005e10: 2063 7265 6174 655f 6c6f 675f 6669 6c65   create_log_file
-00005e20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00005e30: 2222 220a 2020 2020 2020 2020 4372 6561  """.        Crea
-00005e40: 7465 2061 206c 6f67 2066 696c 652e 0a20  te a log file.. 
-00005e50: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00005e60: 2020 2077 696c 696f 745f 6469 7220 3d20     wiliot_dir = 
-00005e70: 5769 6c69 6f74 4469 7228 290a 2020 2020  WiliotDir().    
-00005e80: 2020 2020 7769 6c69 6f74 5f64 6972 2e63      wiliot_dir.c
-00005e90: 7265 6174 655f 6469 7228 2751 525f 7363  reate_dir('QR_sc
-00005ea0: 616e 2729 0a20 2020 2020 2020 2061 7070  an').        app
-00005eb0: 5f64 6972 203d 2077 696c 696f 745f 6469  _dir = wiliot_di
-00005ec0: 722e 6765 745f 7769 6c69 6f74 5f72 6f6f  r.get_wiliot_roo
-00005ed0: 745f 6170 705f 6469 7228 290a 2020 2020  t_app_dir().    
-00005ee0: 2020 2020 6c6f 675f 6469 7220 3d20 6f73      log_dir = os
-00005ef0: 2e70 6174 682e 6a6f 696e 2861 7070 5f64  .path.join(app_d
-00005f00: 6972 2c20 2751 525f 7363 616e 2729 0a20  ir, 'QR_scan'). 
-00005f10: 2020 2020 2020 2069 6620 6e6f 7420 6f73         if not os
-00005f20: 2e70 6174 682e 6578 6973 7473 286c 6f67  .path.exists(log
-00005f30: 5f64 6972 293a 0a20 2020 2020 2020 2020  _dir):.         
-00005f40: 2020 206f 732e 6d61 6b65 6469 7273 286c     os.makedirs(l
-00005f50: 6f67 5f64 6972 290a 0a20 2020 2020 2020  og_dir)..       
-00005f60: 2063 7572 7265 6e74 5f74 696d 6520 3d20   current_time = 
-00005f70: 6461 7465 7469 6d65 2e6e 6f77 2829 2e73  datetime.now().s
-00005f80: 7472 6674 696d 6528 2225 592d 256d 2d25  trftime("%Y-%m-%
-00005f90: 645f 2548 2d25 4d2d 2553 2229 0a20 2020  d_%H-%M-%S").   
-00005fa0: 2020 2020 2073 656c 662e 6c6f 675f 6669       self.log_fi
-00005fb0: 6c65 6e61 6d65 203d 206f 732e 7061 7468  lename = os.path
-00005fc0: 2e6a 6f69 6e28 6c6f 675f 6469 722c 2066  .join(log_dir, f
-00005fd0: 2251 525f 7265 6164 5f6c 6f67 5f7b 6375  "QR_read_log_{cu
-00005fe0: 7272 656e 745f 7469 6d65 7d2e 6c6f 6722  rrent_time}.log"
-00005ff0: 290a 2020 2020 2020 2020 7769 7468 206f  ).        with o
-00006000: 7065 6e28 7365 6c66 2e6c 6f67 5f66 696c  pen(self.log_fil
-00006010: 656e 616d 652c 2027 7727 2920 6173 2066  ename, 'w') as f
-00006020: 3a0a 2020 2020 2020 2020 2020 2020 662e  :.            f.
-00006030: 7772 6974 6528 224c 6f67 2066 696c 6520  write("Log file 
-00006040: 6372 6561 7465 642e 5c6e 2229 0a0a 2020  created.\n")..  
-00006050: 2020 6465 6620 6175 746f 5f63 6f6e 6e65    def auto_conne
-00006060: 6374 2873 656c 662c 2062 6175 645f 7261  ct(self, baud_ra
-00006070: 7465 3a20 696e 7420 3d20 3131 3532 3030  te: int = 115200
-00006080: 2c20 636f 6e66 6967 3a20 626f 6f6c 203d  , config: bool =
-00006090: 2054 7275 652c 2074 696d 656f 7574 3a20   True, timeout: 
-000060a0: 7374 7220 3d20 2731 3030 3027 293a 0a20  str = '1000'):. 
-000060b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000060c0: 2020 2041 7574 6f6d 6174 6963 616c 6c79     Automatically
-000060d0: 2063 6f6e 6e65 6374 2074 6f20 7468 6520   connect to the 
-000060e0: 434f 4d20 706f 7274 2e0a 2020 2020 2020  COM port..      
-000060f0: 2020 2222 220a 2020 2020 2020 2020 636f    """.        co
-00006100: 6d5f 706f 7274 203d 2073 656c 662e 6669  m_port = self.fi
-00006110: 6e64 5f63 6f6d 5f70 6f72 7428 6261 7564  nd_com_port(baud
-00006120: 5f72 6174 6529 0a20 2020 2020 2020 2069  _rate).        i
-00006130: 6620 636f 6d5f 706f 7274 2069 7320 6e6f  f com_port is no
-00006140: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00006150: 2020 2020 7365 6c66 2e6f 7065 6e5f 706f      self.open_po
-00006160: 7274 2863 6f6d 5f70 6f72 742c 2062 6175  rt(com_port, bau
-00006170: 645f 7261 7465 2c20 636f 6e66 6967 2c20  d_rate, config, 
-00006180: 7469 6d65 6f75 743d 7469 6d65 6f75 7429  timeout=timeout)
-00006190: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-000061a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000061b0: 7172 5f6c 6f67 6765 722e 6572 726f 7228  qr_logger.error(
-000061c0: 224e 6f20 7375 6974 6162 6c65 2043 4f4d  "No suitable COM
-000061d0: 2070 6f72 7420 666f 756e 642e 2229 0a20   port found."). 
-000061e0: 2020 2020 2020 2020 2020 2073 7973 2e65             sys.e
-000061f0: 7869 7428 3129 0a0a 2020 2020 6465 6620  xit(1)..    def 
-00006200: 6973 5f72 7473 6361 6e5f 7274 3233 3528  is_rtscan_rt235(
-00006210: 7365 6c66 2c20 636f 6d5f 706f 7274 3a20  self, com_port: 
-00006220: 7374 722c 2062 6175 645f 7261 7465 3a20  str, baud_rate: 
-00006230: 696e 7420 3d20 3131 3532 3030 2920 2d3e  int = 115200) ->
-00006240: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-00006250: 2222 0a20 2020 2020 2020 2043 6865 636b  "".        Check
-00006260: 2069 6620 7468 6520 6465 7669 6365 2069   if the device i
-00006270: 7320 5254 7363 616e 2052 5432 3335 2e0a  s RTscan RT235..
-00006280: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00006290: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000062a0: 2020 2020 2077 6974 6820 7365 7269 616c       with serial
-000062b0: 2e53 6572 6961 6c28 636f 6d5f 706f 7274  .Serial(com_port
-000062c0: 2c20 6261 7564 5f72 6174 652c 2074 696d  , baud_rate, tim
-000062d0: 656f 7574 3d31 2920 6173 2073 6572 3a0a  eout=1) as ser:.
-000062e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062f0: 7365 722e 7772 6974 6528 7374 722e 656e  ser.write(str.en
-00006300: 636f 6465 2873 656c 662e 7072 6566 6978  code(self.prefix
-00006310: 202b 2022 5152 5950 444e 2220 2b20 7365   + "QRYPDN" + se
-00006320: 6c66 2e73 7566 6669 7829 290a 2020 2020  lf.suffix)).    
-00006330: 2020 2020 2020 2020 2020 2020 736c 6565              slee
-00006340: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
-00006350: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-00006360: 3d20 7365 722e 7265 6164 5f61 6c6c 2829  = ser.read_all()
-00006370: 2e64 6563 6f64 6528 290a 2020 2020 2020  .decode().      
-00006380: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00006390: 2073 656c 662e 6465 7669 6365 5f73 6967   self.device_sig
-000063a0: 6e61 7475 7265 2069 6e20 7265 7370 6f6e  nature in respon
-000063b0: 7365 0a20 2020 2020 2020 2065 7863 6570  se.        excep
-000063c0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
-000063d0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000063e0: 6c66 2e71 725f 6c6f 6767 6572 2e65 7272  lf.qr_logger.err
-000063f0: 6f72 2866 2245 7272 6f72 2069 6e20 6973  or(f"Error in is
-00006400: 5f72 7473 6361 6e5f 7274 3233 353a 207b  _rtscan_rt235: {
-00006410: 657d 2229 0a20 2020 2020 2020 2020 2020  e}").           
-00006420: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
-00006430: 2020 2064 6566 2066 696e 645f 636f 6d5f     def find_com_
-00006440: 706f 7274 2873 656c 662c 2062 6175 645f  port(self, baud_
-00006450: 7261 7465 3a20 696e 7420 3d20 3131 3532  rate: int = 1152
-00006460: 3030 2920 2d3e 2073 7472 3a0a 2020 2020  00) -> str:.    
-00006470: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00006480: 4669 6e64 2074 6865 2043 4f4d 2070 6f72  Find the COM por
-00006490: 742e 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
-000064a0: 2020 2020 2020 2063 6f6d 5f70 6f72 7473         com_ports
-000064b0: 203d 2073 6572 6961 6c5f 706f 7274 7328   = serial_ports(
-000064c0: 290a 2020 2020 2020 2020 666f 7220 636f  ).        for co
-000064d0: 6d5f 706f 7274 2069 6e20 636f 6d5f 706f  m_port in com_po
-000064e0: 7274 733a 0a20 2020 2020 2020 2020 2020  rts:.           
-000064f0: 2069 6620 7365 6c66 2e69 735f 7274 7363   if self.is_rtsc
-00006500: 616e 5f72 7432 3335 2863 6f6d 5f70 6f72  an_rt235(com_por
-00006510: 742c 2062 6175 645f 7261 7465 293a 0a20  t, baud_rate):. 
-00006520: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00006530: 6574 7572 6e20 636f 6d5f 706f 7274 0a20  eturn com_port. 
-00006540: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00006550: 6e65 0a0a 2020 2020 6465 6620 6f70 656e  ne..    def open
-00006560: 5f70 6f72 7428 7365 6c66 2c20 636f 6d5f  _port(self, com_
-00006570: 706f 7274 3a20 7374 722c 2062 6175 645f  port: str, baud_
-00006580: 7261 7465 3a20 696e 7420 3d20 3131 3532  rate: int = 1152
-00006590: 3030 2c20 636f 6e66 6967 3a20 626f 6f6c  00, config: bool
-000065a0: 203d 2054 7275 652c 2074 696d 656f 7574   = True, timeout
-000065b0: 3a20 7374 7220 3d20 2731 3030 3027 293a  : str = '1000'):
-000065c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000065d0: 2020 2020 204f 7065 6e20 7468 6520 434f       Open the CO
-000065e0: 4d20 706f 7274 2e0a 2020 2020 2020 2020  M port..        
-000065f0: 2222 220a 2020 2020 2020 2020 7472 793a  """.        try:
-00006600: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00006610: 6e6f 7420 7365 6c66 2e69 735f 7274 7363  not self.is_rtsc
-00006620: 616e 5f72 7432 3335 2863 6f6d 5f70 6f72  an_rt235(com_por
-00006630: 742c 2062 6175 645f 7261 7465 293a 0a20  t, baud_rate):. 
-00006640: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00006650: 6169 7365 2045 7863 6570 7469 6f6e 2866  aise Exception(f
-00006660: 277b 636f 6d5f 706f 7274 7d20 6973 206e  '{com_port} is n
-00006670: 6f74 2061 2062 6172 636f 6465 2073 6361  ot a barcode sca
-00006680: 6e6e 6572 2729 0a20 2020 2020 2020 2020  nner').         
-00006690: 2020 2073 656c 662e 7365 7269 616c 5f63     self.serial_c
-000066a0: 6f6e 6e65 6374 696f 6e20 3d20 7365 7269  onnection = seri
-000066b0: 616c 2e53 6572 6961 6c28 636f 6d5f 706f  al.Serial(com_po
-000066c0: 7274 2c20 6261 7564 5f72 6174 652c 2074  rt, baud_rate, t
-000066d0: 696d 656f 7574 3d28 696e 7428 7469 6d65  imeout=(int(time
-000066e0: 6f75 7429 202b 2035 3029 2f31 3030 3029  out) + 50)/1000)
-000066f0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
-00006700: 4578 6365 7074 696f 6e20 6173 2065 3a0a  Exception as e:.
-00006710: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00006720: 2e63 6c6f 7365 5f70 6f72 7428 290a 2020  .close_port().  
-00006730: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00006740: 4578 6365 7074 696f 6e28 6627 436f 756c  Exception(f'Coul
-00006750: 6420 6e6f 7420 636f 6e6e 6563 7420 746f  d not connect to
-00006760: 207b 636f 6d5f 706f 7274 7d3a 207b 657d   {com_port}: {e}
-00006770: 2729 0a0a 2020 2020 2020 2020 6966 2073  ')..        if s
-00006780: 656c 662e 7365 7269 616c 5f63 6f6e 6e65  elf.serial_conne
-00006790: 6374 696f 6e20 6973 206e 6f74 204e 6f6e  ction is not Non
-000067a0: 6520 616e 6420 7365 6c66 2e6c 6f67 5f74  e and self.log_t
-000067b0: 7970 6520 213d 2027 4e4f 5f4c 4f47 273a  ype != 'NO_LOG':
-000067c0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000067d0: 662e 7172 5f6c 6f67 6765 722e 696e 666f  f.qr_logger.info
-000067e0: 2866 2742 6172 636f 6465 2073 6361 6e6e  (f'Barcode scann
-000067f0: 6572 2028 7b63 6f6d 5f70 6f72 747d 2920  er ({com_port}) 
-00006800: 636f 6e6e 6563 7465 642e 2729 0a20 2020  connected.').   
-00006810: 2020 2020 2065 6c69 6620 7365 6c66 2e73       elif self.s
-00006820: 6572 6961 6c5f 636f 6e6e 6563 7469 6f6e  erial_connection
-00006830: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-00006840: 2020 2020 2020 7365 6c66 2e71 725f 6c6f        self.qr_lo
-00006850: 6767 6572 2e65 7272 6f72 2866 2742 6172  gger.error(f'Bar
-00006860: 636f 6465 2073 6361 6e6e 6572 202d 2050  code scanner - P
-00006870: 726f 626c 656d 2063 6f6e 6e65 6374 696e  roblem connectin
-00006880: 6720 7b63 6f6d 5f70 6f72 747d 2729 0a20  g {com_port}'). 
-00006890: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000068a0: 6e0a 0a20 2020 2020 2020 2073 656c 662e  n..        self.
-000068b0: 636f 6d5f 706f 7274 203d 2063 6f6d 5f70  com_port = com_p
-000068c0: 6f72 740a 2020 2020 2020 2020 7365 6c66  ort.        self
-000068d0: 2e73 6572 6961 6c5f 636f 6e6e 6563 7469  .serial_connecti
-000068e0: 6f6e 2e77 7269 7465 5469 6d65 6f75 7420  on.writeTimeout 
-000068f0: 3d20 302e 3520 2023 2077 7269 7465 2074  = 0.5  # write t
-00006900: 696d 656f 7574 2e0a 2020 2020 2020 2020  imeout..        
-00006910: 6966 2063 6f6e 6669 673a 0a20 2020 2020  if config:.     
-00006920: 2020 2020 2020 2073 656c 662e 636f 6e66         self.conf
-00006930: 6967 7572 6528 7469 6d65 5f6f 7574 3d74  igure(time_out=t
-00006940: 696d 656f 7574 290a 0a20 2020 2064 6566  imeout)..    def
-00006950: 2063 6c6f 7365 5f70 6f72 7428 7365 6c66   close_port(self
-00006960: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00006970: 2020 2020 2020 2043 6c6f 7365 2074 6865         Close the
-00006980: 2043 4f4d 2070 6f72 742e 0a20 2020 2020   COM port..     
-00006990: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-000069a0: 6620 7365 6c66 2e73 6572 6961 6c5f 636f  f self.serial_co
-000069b0: 6e6e 6563 7469 6f6e 2e69 734f 7065 6e28  nnection.isOpen(
-000069c0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000069d0: 656c 662e 7365 7269 616c 5f63 6f6e 6e65  elf.serial_conne
-000069e0: 6374 696f 6e2e 636c 6f73 6528 290a 0a20  ction.close().. 
-000069f0: 2020 2064 6566 2069 735f 6f70 656e 2873     def is_open(s
-00006a00: 656c 6629 202d 3e20 626f 6f6c 3a0a 2020  elf) -> bool:.  
-00006a10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00006a20: 2020 4368 6563 6b20 6966 2074 6865 2043    Check if the C
-00006a30: 4f4d 2070 6f72 7420 6973 206f 7065 6e2e  OM port is open.
-00006a40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00006a50: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00006a60: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
-00006a70: 2e6d 616e 7561 6c5f 636f 6e66 6967 7572  .manual_configur
-00006a80: 6528 5b27 5152 5950 444e 275d 290a 2020  e(['QRYPDN']).  
-00006a90: 2020 2020 2020 2020 2020 6966 2027 4e4c            if 'NL
-00006aa0: 532d 4e31 2720 696e 2073 7472 2872 6573  S-N1' in str(res
-00006ab0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00006ac0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00006ad0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00006ae0: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-00006af0: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-00006b00: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00006b10: 0a0a 2020 2020 6465 6620 636f 6e66 6967  ..    def config
-00006b20: 7572 6528 7365 6c66 2c20 696c 6c5f 7363  ure(self, ill_sc
-00006b30: 6e3d 2731 272c 2061 6d6c 5f65 6e61 3d27  n='1', aml_ena='
-00006b40: 3127 2c20 6772 625f 656e 613d 2730 272c  1', grb_ena='0',
-00006b50: 2067 7262 5f76 6c6c 3d27 3227 2c20 6174   grb_vll='2', at
-00006b60: 735f 656e 613d 2730 272c 2061 7473 5f64  s_ena='0', ats_d
-00006b70: 7572 3d27 3336 3030 3027 2c20 7363 6e5f  ur='36000', scn_
-00006b80: 6d6f 643d 2730 272c 0a20 2020 2020 2020  mod='0',.       
-00006b90: 2020 2020 2020 2020 2020 2070 7762 5f65             pwb_e
-00006ba0: 6e61 3d27 3027 2c72 7264 725f 656e 203d  na='0',rrdr_en =
-00006bb0: 2027 3127 2c67 7264 5f65 6e61 203d 2027   '1',grd_ena = '
-00006bc0: 3027 2c20 6772 645f 6475 7220 3d20 2731  0', grd_dur = '1
-00006bd0: 272c 2074 696d 655f 6f75 743d 2731 3027  ', time_out='10'
-00006be0: 2c20 6261 645f 6d73 675f 656e 3d54 7275  , bad_msg_en=Tru
-00006bf0: 652c 2073 796d 626f 6c6f 6769 6573 3d4e  e, symbologies=N
-00006c00: 6f6e 6529 3a0a 2020 2020 2020 2020 2727  one):.        ''
-00006c10: 270a 2020 2020 2020 2020 696c 6c5f 7363  '.        ill_sc
-00006c20: 6e20 2d20 696c 6c75 6d69 6e61 7469 6f6e  n - illumination
-00006c30: 3a20 2020 2020 2020 2020 302d 6f66 662c  :         0-off,
-00006c40: 2031 2d6e 6f72 6d61 6c2c 2032 2d61 6c77   1-normal, 2-alw
-00006c50: 6179 7320 6f6e 0a20 2020 2020 2020 2061  ays on.        a
-00006c60: 6d6c 5f65 6e61 202d 2061 696d 696e 673a  ml_ena - aiming:
-00006c70: 2020 2020 2020 2020 2020 2020 2020 2030                 0
-00006c80: 2d6f 6666 2c20 312d 6e6f 726d 616c 2c20  -off, 1-normal, 
-00006c90: 322d 616c 7761 7973 206f 6e0a 2020 2020  2-always on.    
-00006ca0: 2020 2020 7077 625f 656e 6120 2d20 706f      pwb_ena - po
-00006cb0: 7765 7220 6f6e 2062 6565 7020 2020 2020  wer on beep     
-00006cc0: 2020 2020 302d 6f66 662c 2031 2d6f 6e0a      0-off, 1-on.
-00006cd0: 2020 2020 2020 2020 6772 625f 656e 6120          grb_ena 
-00006ce0: 2d20 676f 6f64 2072 6561 6420 6265 6570  - good read beep
-00006cf0: 2020 2020 2020 2020 302d 6f66 662c 2031          0-off, 1
-00006d00: 2d6f 6e0a 2020 2020 2020 2020 6772 645f  -on.        grd_
-00006d10: 656e 6120 2d20 676f 6f64 2072 6561 6420  ena - good read 
-00006d20: 656e 6162 6c65 2020 2020 2020 302d 6f66  enable      0-of
-00006d30: 662c 2031 2d6f 6e0a 2020 2020 2020 2020  f, 1-on.        
-00006d40: 6772 645f 6475 7220 2d20 676f 6f64 2072  grd_dur - good r
-00006d50: 6561 6420 6475 7261 7469 6f6e 2020 2020  ead duration    
-00006d60: 312d 3336 3030 3020 5b6d 7365 635d 0a20  1-36000 [msec]. 
-00006d70: 2020 2020 2020 2061 7473 5f65 6e61 202d         ats_ena -
-00006d80: 2061 7574 6f20 736c 6565 7020 2020 2020   auto sleep     
-00006d90: 2020 2020 2020 2030 2d64 6973 6162 6c65         0-disable
-00006da0: 2c20 312d 656e 6162 6c65 0a20 2020 2020  , 1-enable.     
-00006db0: 2020 2061 7473 5f64 7572 202d 2073 6c65     ats_dur - sle
-00006dc0: 6570 2064 7572 6174 696f 6e20 2020 2020  ep duration     
-00006dd0: 2020 2031 2d33 3630 3030 205b 7365 635d     1-36000 [sec]
-00006de0: 0a20 2020 2020 2020 2072 7264 725f 656e  .        rrdr_en
-00006df0: 202d 2052 6572 6561 6420 7265 7365 7420   - Reread reset 
-00006e00: 2020 2020 2020 2020 2030 2d6f 6666 2c20           0-off, 
-00006e10: 312d 6f6e 0a20 2020 2020 2020 2073 636e  1-on.        scn
-00006e20: 5f6d 6f64 202d 2073 6361 6e20 6d6f 6465  _mod - scan mode
-00006e30: 2020 2020 2020 2020 2020 2020 2030 2d6c               0-l
-00006e40: 6576 656c 206d 6f64 652c 2032 2d73 656e  evel mode, 2-sen
-00006e50: 7365 206d 6f64 652c 2033 2d63 6f6e 7469  se mode, 3-conti
-00006e60: 6e75 6f75 7320 6d6f 6465 2c20 372d 6261  nuous mode, 7-ba
-00006e70: 7463 6820 6d6f 6465 0a20 2020 2020 2020  tch mode.       
-00006e80: 2073 796d 626f 6c6f 6769 6573 202d 2061   symbologies - a
-00006e90: 206c 6973 7420 6f66 2073 7472 696e 6773   list of strings
-00006ea0: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
-00006eb0: 6520 7379 6d62 6f6c 6f67 6965 7320 746f  e symbologies to
-00006ec0: 2065 6e61 626c 652c 2065 2e67 2e20 5b27   enable, e.g. ['
-00006ed0: 5152 272c 2027 5044 4634 3137 272c 2027  QR', 'PDF417', '
-00006ee0: 4541 4e31 3327 5d0a 0a20 2020 2020 2020  EAN13']..       
-00006ef0: 204c 6576 656c 204d 6f64 653a 0a20 2020   Level Mode:.   
-00006f00: 2020 2020 2049 6e20 7468 6973 206d 6f64       In this mod
-00006f10: 652c 2074 6865 2073 6361 6e6e 6572 2077  e, the scanner w
-00006f20: 6169 7473 2066 6f72 2061 2074 7269 6767  aits for a trigg
-00006f30: 6572 2070 756c 6c20 746f 2061 6374 6976  er pull to activ
-00006f40: 6174 6520 6120 6465 636f 6465 2073 6573  ate a decode ses
-00006f50: 7369 6f6e 2e20 5468 6520 6465 636f 6465  sion. The decode
-00006f60: 2073 6573 7369 6f6e 2063 6f6e 7469 6e75   session continu
-00006f70: 6573 2075 6e74 696c 2061 2062 6172 636f  es until a barco
-00006f80: 6465 2069 7320 6465 636f 6465 6420 6f72  de is decoded or
-00006f90: 2079 6f75 2072 656c 6561 7365 2074 6865   you release the
-00006fa0: 2074 7269 6767 6572 2e0a 2020 2020 2020   trigger..      
-00006fb0: 2020 436f 6d6d 616e 6420 7472 6967 6765    Command trigge
-00006fc0: 7220 6d6f 6465 3a0a 2020 2020 2020 2020  r mode:.        
-00006fd0: 5468 6973 206d 6f64 6520 7265 7175 6972  This mode requir
-00006fe0: 6573 2079 6f75 2074 6f20 7365 6e64 2061  es you to send a
-00006ff0: 2063 6f6d 6d61 6e64 2028 3142 2033 3120   command (1B 31 
-00007000: 696e 2068 6578 2920 746f 2061 6374 6976  in hex) to activ
-00007010: 6174 6520 6120 6465 636f 6465 2073 6573  ate a decode ses
-00007020: 7369 6f6e 2e0a 0a20 2020 2020 2020 2053  sion...        S
-00007030: 656e 7365 204d 6f64 653a 0a20 2020 2020  ense Mode:.     
-00007040: 2020 2049 6e20 7468 6973 206d 6f64 652c     In this mode,
-00007050: 2074 6865 2073 6361 6e6e 6572 2061 6374   the scanner act
-00007060: 6976 6174 6573 2061 2064 6563 6f64 6520  ivates a decode 
-00007070: 7365 7373 696f 6e20 6576 6572 7920 7469  session every ti
-00007080: 6d65 2069 7420 6465 7465 6374 7320 6120  me it detects a 
-00007090: 6261 7263 6f64 6520 7072 6573 656e 7465  barcode presente
-000070a0: 6420 746f 2069 742e 2054 6865 2064 6563  d to it. The dec
-000070b0: 6f64 6520 7365 7373 696f 6e20 636f 6e74  ode session cont
-000070c0: 696e 7565 7320 756e 7469 6c20 6120 6261  inues until a ba
-000070d0: 7263 6f64 6520 6973 2064 6563 6f64 6564  rcode is decoded
-000070e0: 206f 7220 7468 6520 6465 636f 6465 2073   or the decode s
-000070f0: 6573 7369 6f6e 2074 696d 656f 7574 2065  ession timeout e
-00007100: 7870 6972 6573 2e20 596f 7520 6361 6e20  xpires. You can 
-00007110: 6164 6a75 7374 2074 6865 2073 656e 7369  adjust the sensi
-00007120: 7469 7669 7479 2061 6e64 2072 6572 6561  tivity and rerea
-00007130: 6420 7469 6d65 6f75 7420 746f 2061 766f  d timeout to avo
-00007140: 6964 2075 6e64 6573 6972 6564 2072 6572  id undesired rer
-00007150: 6561 6469 6e67 206f 6620 7468 6520 7361  eading of the sa
-00007160: 6d65 2062 6172 636f 6465 2069 6e20 6120  me barcode in a 
-00007170: 6769 7665 6e20 7065 7269 6f64 206f 6620  given period of 
-00007180: 7469 6d65 2e20 596f 7520 6361 6e20 616c  time. You can al
-00007190: 736f 2061 646a 7573 7420 7468 6520 696d  so adjust the im
-000071a0: 6167 6520 7374 6162 696c 697a 6174 696f  age stabilizatio
-000071b0: 6e20 7469 6d65 6f75 7420 746f 2067 6976  n timeout to giv
-000071c0: 6520 7468 6520 7363 616e 6e65 7220 7469  e the scanner ti
-000071d0: 6d65 2074 6f20 6164 6170 7420 746f 2061  me to adapt to a
-000071e0: 6d62 6965 6e74 2065 6e76 6972 6f6e 6d65  mbient environme
-000071f0: 6e74 2061 6674 6572 2069 7420 6465 636f  nt after it deco
-00007200: 6465 7320 6120 6261 7263 6f64 6520 616e  des a barcode an
-00007210: 6420 e280 9c6c 6f6f 6b73 e280 9d20 666f  d ...looks... fo
-00007220: 7220 616e 6f74 6865 722e 0a0a 2020 2020  r another...    
-00007230: 2020 2020 436f 6e74 696e 756f 7573 204d      Continuous M
-00007240: 6f64 653a 0a20 2020 2020 2020 2049 6e20  ode:.        In 
-00007250: 7468 6973 206d 6f64 652c 2074 6865 2073  this mode, the s
-00007260: 6361 6e6e 6572 2061 7574 6f6d 6174 6963  canner automatic
-00007270: 616c 6c79 2073 7461 7274 7320 6f6e 6520  ally starts one 
-00007280: 6465 636f 6465 2073 6573 7369 6f6e 2061  decode session a
-00007290: 6674 6572 2061 6e6f 7468 6572 2e20 546f  fter another. To
-000072a0: 2073 7573 7065 6e64 2f72 6573 756d 6520   suspend/resume 
-000072b0: 6261 7263 6f64 6520 7265 6164 696e 672c  barcode reading,
-000072c0: 2073 696d 706c 7920 7072 6573 7320 7468   simply press th
-000072d0: 6520 7472 6967 6765 722e 2059 6f75 2063  e trigger. You c
-000072e0: 616e 2061 646a 7573 7420 7468 6520 7265  an adjust the re
-000072f0: 7265 6164 2074 696d 656f 7574 2074 6f20  read timeout to 
-00007300: 6176 6f69 6420 756e 6465 7369 7265 6420  avoid undesired 
-00007310: 7265 7265 6164 696e 6720 6f66 2074 6865  rereading of the
-00007320: 2073 616d 6520 6261 7263 6f64 6520 696e   same barcode in
-00007330: 2061 2067 6976 656e 2070 6572 696f 6420   a given period 
-00007340: 6f66 2074 696d 652e 204e 6f74 6520 7468  of time. Note th
-00007350: 6174 2077 6865 6e20 7377 6974 6368 696e  at when switchin
-00007360: 6720 746f 2074 6869 7320 6d6f 6465 2062  g to this mode b
-00007370: 7920 7363 616e 6e69 6e67 2074 6865 2043  y scanning the C
-00007380: 6f6e 7469 6e75 6f75 7320 4d6f 6465 2062  ontinuous Mode b
-00007390: 6172 636f 6465 2c20 7468 6520 7363 616e  arcode, the scan
-000073a0: 6e65 7220 7769 6c6c 2073 746f 7020 6261  ner will stop ba
-000073b0: 7263 6f64 6520 7265 6164 696e 6720 666f  rcode reading fo
-000073c0: 7220 3320 7365 636f 6e64 7320 6265 666f  r 3 seconds befo
-000073d0: 7265 2073 7461 7274 696e 6720 7363 616e  re starting scan
-000073e0: 6e69 6e67 2063 6f6e 7469 6e75 6f75 736c  ning continuousl
-000073f0: 792e 0a0a 2020 2020 2020 2020 4261 7463  y...        Batc
-00007400: 6820 4d6f 6465 3a0a 2020 2020 2020 2020  h Mode:.        
-00007410: 496e 2074 6869 7320 6d6f 6465 2c20 6120  In this mode, a 
-00007420: 7472 6967 6765 7220 7075 6c6c 2061 6374  trigger pull act
-00007430: 6976 6174 6573 2061 2072 6f75 6e64 206f  ivates a round o
-00007440: 6620 6d75 6c74 6970 6c65 2064 6563 6f64  f multiple decod
-00007450: 6520 7365 7373 696f 6e73 2e20 5468 6520  e sessions. The 
-00007460: 726f 756e 6420 6f66 206d 756c 7469 706c  round of multipl
-00007470: 6520 7363 616e 7320 636f 6e74 696e 7565  e scans continue
-00007480: 7320 756e 7469 6c20 796f 7520 7265 6c65  s until you rele
-00007490: 6173 6520 7468 6520 7472 6967 6765 722e  ase the trigger.
-000074a0: 2052 6572 6561 6469 6e67 2074 6865 2073   Rereading the s
-000074b0: 616d 6520 6261 7263 6f64 6520 6973 206e  ame barcode is n
-000074c0: 6f74 2061 6c6c 6f77 6564 2069 6e20 7468  ot allowed in th
-000074d0: 6520 7361 6d65 2072 6f75 6e64 2e0a 2020  e same round..  
-000074e0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-000074f0: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
-00007500: 2020 2020 2070 6172 616d 7320 3d20 7b27       params = {'
-00007510: 494c 4c53 434e 273a 2069 6c6c 5f73 636e  ILLSCN': ill_scn
-00007520: 2c20 2741 4d4c 454e 4127 3a20 616d 6c5f  , 'AMLENA': aml_
-00007530: 656e 612c 2027 4752 4245 4e41 273a 2067  ena, 'GRBENA': g
-00007540: 7262 5f65 6e61 2c20 2741 5453 454e 4127  rb_ena, 'ATSENA'
-00007550: 3a20 6174 735f 656e 612c 2027 4e47 5245  : ats_ena, 'NGRE
-00007560: 4e41 273a 2027 3127 2069 6620 6261 645f  NA': '1' if bad_
-00007570: 6d73 675f 656e 2065 6c73 6520 2730 272c  msg_en else '0',
-00007580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007590: 2020 2027 4752 4256 4c4c 273a 2067 7262     'GRBVLL': grb
-000075a0: 5f76 6c6c 2c20 2741 5453 4455 5227 3a20  _vll, 'ATSDUR': 
-000075b0: 6174 735f 6475 722c 2027 5343 4e4d 4f44  ats_dur, 'SCNMOD
-000075c0: 273a 2073 636e 5f6d 6f64 2c20 2752 5244  ': scn_mod, 'RRD
-000075d0: 5245 4e27 3a20 7272 6472 5f65 6e2c 2027  REN': rrdr_en, '
-000075e0: 4752 4445 4e41 2720 3a20 6772 645f 656e  GRDENA' : grd_en
-000075f0: 612c 2027 4752 4444 5552 2720 3a20 6772  a, 'GRDDUR' : gr
-00007600: 645f 6475 722c 0a20 2020 2020 2020 2020  d_dur,.         
-00007610: 2020 2020 2020 2020 2027 5057 4245 4e41           'PWBENA
-00007620: 273a 2070 7762 5f65 6e61 2c20 274f 5254  ': pwb_ena, 'ORT
-00007630: 5345 5427 3a20 7469 6d65 5f6f 7574 7d0a  SET': time_out}.
-00007640: 2020 2020 2020 2020 7061 7261 6d73 203d          params =
-00007650: 205b 6b65 7920 2b20 7661 6c75 6520 666f   [key + value fo
-00007660: 7220 6b65 792c 2076 616c 7565 2069 6e20  r key, value in 
-00007670: 7061 7261 6d73 2e69 7465 6d73 2829 5d0a  params.items()].
-00007680: 0a20 2020 2020 2020 2069 6620 7379 6d62  .        if symb
-00007690: 6f6c 6f67 6965 7320 6973 206e 6f74 204e  ologies is not N
-000076a0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000076b0: 2066 6f72 2073 796d 626f 6c6f 6779 2069   for symbology i
-000076c0: 6e20 7379 6d62 6f6c 6f67 6965 733a 0a20  n symbologies:. 
-000076d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000076e0: 6172 616d 732e 6170 7065 6e64 2827 5359  arams.append('SY
-000076f0: 4d42 5f27 202b 2073 796d 626f 6c6f 6779  MB_' + symbology
-00007700: 202b 2027 3127 290a 0a20 2020 2020 2020   + '1')..       
-00007710: 2074 2c20 6973 5375 6363 6573 7320 3d20   t, isSuccess = 
-00007720: 7365 6c66 2e6d 616e 7561 6c5f 636f 6e66  self.manual_conf
-00007730: 6967 7572 6528 7061 7261 6d73 290a 2020  igure(params).  
-00007740: 2020 2020 2020 6966 2069 7353 7563 6365        if isSucce
-00007750: 7373 2061 6e64 2073 656c 662e 6c6f 675f  ss and self.log_
-00007760: 7479 7065 2021 3d20 274e 4f5f 4c4f 4727  type != 'NO_LOG'
-00007770: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00007780: 6c66 2e71 725f 6c6f 6767 6572 2e69 6e66  lf.qr_logger.inf
-00007790: 6f28 6627 4261 7263 6f64 6520 7363 616e  o(f'Barcode scan
-000077a0: 6e65 7220 287b 7365 6c66 2e63 6f6d 5f70  ner ({self.com_p
-000077b0: 6f72 747d 2920 636f 6e66 6967 7572 6564  ort}) configured
-000077c0: 2073 7563 6365 7373 6675 6c6c 792e 2729   successfully.')
-000077d0: 0a20 2020 2020 2020 2065 6c69 6620 6e6f  .        elif no
-000077e0: 7420 6973 5375 6363 6573 733a 0a20 2020  t isSuccess:.   
-000077f0: 2020 2020 2020 2020 2073 656c 662e 7172           self.qr
-00007800: 5f6c 6f67 6765 722e 6572 726f 7228 6627  _logger.error(f'
-00007810: 4261 7263 6f64 6520 7363 616e 6e65 7220  Barcode scanner 
-00007820: 287b 7365 6c66 2e63 6f6d 5f70 6f72 747d  ({self.com_port}
-00007830: 2920 636f 6e66 6967 7572 6174 696f 6e20  ) configuration 
-00007840: 6661 696c 6564 2e27 290a 0a20 2020 2064  failed.')..    d
-00007850: 6566 2072 6573 746f 7265 5f61 6c6c 5f66  ef restore_all_f
-00007860: 6163 746f 7279 5f64 6566 6175 6c74 7328  actory_defaults(
-00007870: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00007880: 2222 0a20 2020 2020 2020 2052 6573 746f  "".        Resto
-00007890: 7265 2061 6c6c 2066 6163 746f 7279 2064  re all factory d
-000078a0: 6566 6175 6c74 732e 0a20 2020 2020 2020  efaults..       
-000078b0: 2022 2222 0a20 2020 2020 2020 2073 6c65   """.        sle
-000078c0: 6570 2830 2e31 290a 2020 2020 2020 2020  ep(0.1).        
-000078d0: 7061 7261 6d73 203d 207b 2746 4143 4445  params = {'FACDE
-000078e0: 4627 3a20 2727 7d0a 2020 2020 2020 2020  F': ''}.        
-000078f0: 7061 7261 6d73 203d 205b 6b65 7920 2b20  params = [key + 
-00007900: 7661 6c75 6520 666f 7220 6b65 792c 2076  value for key, v
-00007910: 616c 7565 2069 6e20 7061 7261 6d73 2e69  alue in params.i
-00007920: 7465 6d73 2829 5d0a 2020 2020 2020 2020  tems()].        
-00007930: 742c 2069 7353 7563 6365 7373 203d 2073  t, isSuccess = s
-00007940: 656c 662e 6d61 6e75 616c 5f63 6f6e 6669  elf.manual_confi
-00007950: 6775 7265 2870 6172 616d 7329 0a20 2020  gure(params).   
-00007960: 2020 2020 2069 6620 6973 5375 6363 6573       if isSucces
-00007970: 7320 616e 6420 7365 6c66 2e6c 6f67 5f74  s and self.log_t
-00007980: 7970 6520 213d 2027 4e4f 5f4c 4f47 273a  ype != 'NO_LOG':
-00007990: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000079a0: 662e 7172 5f6c 6f67 6765 722e 696e 666f  f.qr_logger.info
-000079b0: 2866 2742 6172 636f 6465 2073 6361 6e6e  (f'Barcode scann
-000079c0: 6572 2028 7b73 656c 662e 636f 6d5f 706f  er ({self.com_po
-000079d0: 7274 7d29 2072 6573 746f 7265 6420 6661  rt}) restored fa
-000079e0: 6374 6f72 7920 6465 6661 756c 7420 7375  ctory default su
-000079f0: 6363 6573 7366 756c 6c79 2e27 290a 2020  ccessfully.').  
-00007a00: 2020 2020 2020 656c 6966 206e 6f74 2069        elif not i
-00007a10: 7353 7563 6365 7373 3a0a 2020 2020 2020  sSuccess:.      
-00007a20: 2020 2020 2020 7365 6c66 2e71 725f 6c6f        self.qr_lo
-00007a30: 6767 6572 2e65 7272 6f72 2866 2742 6172  gger.error(f'Bar
-00007a40: 636f 6465 2073 6361 6e6e 6572 2028 7b73  code scanner ({s
-00007a50: 656c 662e 636f 6d5f 706f 7274 7d29 2072  elf.com_port}) r
-00007a60: 6573 746f 7265 6420 6661 6374 6f72 7920  estored factory 
-00007a70: 6465 6661 756c 7420 6661 696c 6564 2e27  default failed.'
-00007a80: 290a 0a20 2020 2064 6566 206d 616e 7561  )..    def manua
-00007a90: 6c5f 636f 6e66 6967 7572 6528 7365 6c66  l_configure(self
-00007aa0: 2c20 7061 7261 6d73 293a 0a20 2020 2020  , params):.     
-00007ab0: 2020 2022 2222 0a20 2020 2020 2020 204d     """.        M
-00007ac0: 616e 7561 6c6c 7920 636f 6e66 6967 7572  anually configur
-00007ad0: 6520 7468 6520 7363 616e 6e65 722e 0a20  e the scanner.. 
-00007ae0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00007af0: 2020 2073 656c 662e 7365 7269 616c 5f63     self.serial_c
-00007b00: 6f6e 6e65 6374 696f 6e2e 666c 7573 6849  onnection.flushI
-00007b10: 6e70 7574 2829 0a20 2020 2020 2020 2073  nput().        s
-00007b20: 656c 662e 7365 7269 616c 5f63 6f6e 6e65  elf.serial_conne
-00007b30: 6374 696f 6e2e 666c 7573 684f 7574 7075  ction.flushOutpu
-00007b40: 7428 290a 2020 2020 2020 2020 736c 6565  t().        slee
-00007b50: 7028 302e 3129 0a20 2020 2020 2020 2062  p(0.1).        b
-00007b60: 6164 5f6d 7367 203d 2027 3436 3064 3061  ad_msg = '460d0a
-00007b70: 2723 3436 203d 2046 2c20 2330 6420 3d20  '#46 = F, #0d = 
-00007b80: 2f72 2023 3061 203d 202f 6e20 2d3e 206d  /r #0a = /n -> m
-00007b90: 6561 6e73 2074 6861 7420 6576 6572 7920  eans that every 
-00007ba0: 6572 726f 7220 6f72 2064 6563 6f6e 6469  error or decondi
-00007bb0: 6e67 2074 696d 656f 7574 2077 696c 6c20  ng timeout will 
-00007bc0: 7365 6e64 2074 6865 206d 6573 7361 6765  send the message
-00007bd0: 2046 2f72 2f6e 202d 3e20 7769 6c6c 2062   F/r/n -> will b
-00007be0: 6520 7472 616e 736c 6174 6564 2062 7920  e translated by 
-00007bf0: 7365 7269 616c 206c 6962 2061 7320 463c  serial lib as F<
-00007c00: 4e65 774c 696e 653e 0a20 2020 2020 2020  NewLine>.       
-00007c10: 2065 6e74 6572 5f73 6574 7570 5f6d 6f64   enter_setup_mod
-00007c20: 6520 3d20 2753 4554 5550 4531 270a 2020  e = 'SETUPE1'.  
-00007c30: 2020 2020 2020 6578 6974 5f73 6574 7570        exit_setup
-00007c40: 5f6d 6f64 6520 3d20 2753 4554 5550 4530  _mode = 'SETUPE0
-00007c50: 270a 2020 2020 2020 2020 2345 6e74 6572  '.        #Enter
-00007c60: 2073 6574 7570 206d 6f64 650a 2020 2020   setup mode.    
-00007c70: 2020 2020 7365 6c66 2e73 6572 6961 6c5f      self.serial_
-00007c80: 636f 6e6e 6563 7469 6f6e 2e77 7269 7465  connection.write
-00007c90: 2873 7472 2e65 6e63 6f64 6528 7365 6c66  (str.encode(self
-00007ca0: 2e70 7265 6669 7820 2b20 656e 7465 725f  .prefix + enter_
-00007cb0: 7365 7475 705f 6d6f 6465 202b 2073 656c  setup_mode + sel
-00007cc0: 662e 7375 6666 6978 2929 0a20 2020 2020  f.suffix)).     
-00007cd0: 2020 2023 2049 6e73 6572 7420 636f 6e66     # Insert conf
-00007ce0: 6967 7572 6174 696f 6e0a 2020 2020 2020  iguration.      
-00007cf0: 2020 636f 6e66 6967 7320 3d20 7365 6c66    configs = self
-00007d00: 2e70 7265 6669 7820 2b20 273b 272e 6a6f  .prefix + ';'.jo
-00007d10: 696e 2870 6172 616d 7329 202b 2073 656c  in(params) + sel
-00007d20: 662e 7375 6666 6978 0a20 2020 2020 2020  f.suffix.       
-00007d30: 2073 656c 662e 7365 7269 616c 5f63 6f6e   self.serial_con
-00007d40: 6e65 6374 696f 6e2e 7772 6974 6528 7374  nection.write(st
-00007d50: 722e 656e 636f 6465 2863 6f6e 6669 6773  r.encode(configs
-00007d60: 2929 0a20 2020 2020 2020 2069 6620 274e  )).        if 'N
-00007d70: 4752 454e 4131 2720 696e 2070 6172 616d  GRENA1' in param
-00007d80: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-00007d90: 656c 662e 7365 7269 616c 5f63 6f6e 6e65  elf.serial_conne
-00007da0: 6374 696f 6e2e 7772 6974 6528 7374 722e  ction.write(str.
-00007db0: 656e 636f 6465 2873 656c 662e 7072 6566  encode(self.pref
-00007dc0: 6978 202b 2027 4e47 5253 4554 272b 2062  ix + 'NGRSET'+ b
-00007dd0: 6164 5f6d 7367 202b 2073 656c 662e 7375  ad_msg + self.su
-00007de0: 6666 6978 2929 2020 2320 5365 7420 6d65  ffix))  # Set me
-00007df0: 7373 6167 6520 746f 2065 6d70 7479 0a20  ssage to empty. 
-00007e00: 2020 2020 2020 2069 6620 2753 434e 4d4f         if 'SCNMO
-00007e10: 4432 2720 696e 2070 6172 616d 733a 0a20  D2' in params:. 
-00007e20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00007e30: 7365 7269 616c 5f63 6f6e 6e65 6374 696f  serial_connectio
-00007e40: 6e2e 7772 6974 6528 7374 722e 656e 636f  n.write(str.enco
-00007e50: 6465 2873 656c 662e 7072 6566 6978 202b  de(self.prefix +
-00007e60: 2027 5345 4e4c 564c 3527 202b 2062 6164   'SENLVL5' + bad
-00007e70: 5f6d 7367 202b 2073 656c 662e 7375 6666  _msg + self.suff
-00007e80: 6978 2929 2020 2320 5365 7420 7365 6e73  ix))  # Set sens
-00007e90: 6974 6976 6974 7920 746f 2068 6967 6820  itivity to high 
-00007ea0: 312d 3230 0a20 2020 2020 2020 2023 2045  1-20.        # E
-00007eb0: 7869 7420 7365 7475 7020 6d6f 6465 0a20  xit setup mode. 
-00007ec0: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
-00007ed0: 616c 5f63 6f6e 6e65 6374 696f 6e2e 7772  al_connection.wr
-00007ee0: 6974 6528 7374 722e 656e 636f 6465 2873  ite(str.encode(s
-00007ef0: 656c 662e 7072 6566 6978 202b 2065 7869  elf.prefix + exi
-00007f00: 745f 7365 7475 705f 6d6f 6465 202b 2073  t_setup_mode + s
-00007f10: 656c 662e 7375 6666 6978 2929 0a20 2020  elf.suffix)).   
-00007f20: 2020 2020 2073 6c65 6570 2830 2e31 290a       sleep(0.1).
-00007f30: 2020 2020 2020 2020 742c 2069 7353 7563          t, isSuc
-00007f40: 6365 7373 203d 2073 656c 662e 7472 6967  cess = self.trig
-00007f50: 6765 725f 7374 6f70 5f73 6574 7469 6e67  ger_stop_setting
-00007f60: 7328 290a 2020 2020 2020 2020 7265 7475  s().        retu
-00007f70: 726e 2074 2c20 6973 5375 6363 6573 730a  rn t, isSuccess.
-00007f80: 0a20 2020 2064 6566 2073 6361 6e28 7365  .    def scan(se
-00007f90: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
-00007fa0: 0a20 2020 2020 2020 2053 6361 6e20 7468  .        Scan th
-00007fb0: 6520 5152 2063 6f64 652e 0a20 2020 2020  e QR code..     
-00007fc0: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-00007fd0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-00007fe0: 7365 6c66 2e73 6572 6961 6c5f 636f 6e6e  self.serial_conn
-00007ff0: 6563 7469 6f6e 2e77 7269 7465 2862 225c  ection.write(b"\
-00008000: 7831 625c 7833 3122 290a 2020 2020 2020  x1b\x31").      
-00008010: 2020 7374 6172 745f 7469 6d65 203d 2064    start_time = d
-00008020: 6174 6574 696d 652e 6e6f 7728 290a 2020  atetime.now().  
-00008030: 2020 2020 2020 7420 3d20 7365 6c66 2e73        t = self.s
-00008040: 6572 6961 6c5f 636f 6e6e 6563 7469 6f6e  erial_connection
-00008050: 2e72 6561 646c 696e 6528 290a 2020 2020  .readline().    
-00008060: 2020 2020 2320 7072 696e 7428 6627 676f      # print(f'go
-00008070: 7420 6d73 6720 7b74 7d27 290a 2020 2020  t msg {t}').    
-00008080: 2020 2020 656e 645f 7469 6d65 203d 2064      end_time = d
-00008090: 6174 6574 696d 652e 6e6f 7728 290a 2020  atetime.now().  
-000080a0: 2020 2020 2020 656c 6170 7365 645f 7469        elapsed_ti
-000080b0: 6d65 5f6d 7320 3d20 2865 6e64 5f74 696d  me_ms = (end_tim
-000080c0: 6520 2d20 7374 6172 745f 7469 6d65 292e  e - start_time).
-000080d0: 746f 7461 6c5f 7365 636f 6e64 7328 2920  total_seconds() 
-000080e0: 2a20 3130 3030 0a20 2020 2020 2020 2072  * 1000.        r
-000080f0: 6574 7572 6e20 742c 2065 6c61 7073 6564  eturn t, elapsed
-00008100: 5f74 696d 655f 6d73 0a0a 2020 2020 6465  _time_ms..    de
-00008110: 6620 7363 616e 5f61 6e64 5f66 6c75 7368  f scan_and_flush
-00008120: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008130: 2222 220a 2020 2020 2020 2020 5363 616e  """.        Scan
-00008140: 2074 6865 2051 5220 636f 6465 2061 6e64   the QR code and
-00008150: 2066 6c75 7368 2074 6865 2062 7566 6665   flush the buffe
-00008160: 722e 0a20 2020 2020 2020 2022 2222 0a20  r..        """. 
-00008170: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
-00008180: 6572 6961 6c5f 636f 6e6e 6563 7469 6f6e  erial_connection
-00008190: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-000081a0: 2020 2020 2020 7365 6c66 2e71 725f 6c6f        self.qr_lo
-000081b0: 6767 6572 2e65 7272 6f72 2822 4572 726f  gger.error("Erro
-000081c0: 723a 2053 6572 6961 6c20 6f62 6a65 6374  r: Serial object
-000081d0: 206e 6f74 2069 6e69 7469 616c 697a 6564   not initialized
-000081e0: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
-000081f0: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
-00008200: 2020 2074 2c20 656c 6170 7365 645f 7469     t, elapsed_ti
-00008210: 6d65 5f6d 7320 3d20 7365 6c66 2e73 6361  me_ms = self.sca
-00008220: 6e28 290a 2020 2020 2020 2020 2320 5072  n().        # Pr
-00008230: 6f63 6573 7320 7265 6365 6976 6564 2064  ocess received d
-00008240: 6174 6120 6d6f 7265 2065 6666 6963 6965  ata more efficie
-00008250: 6e74 6c79 0a20 2020 2020 2020 2069 6620  ntly.        if 
-00008260: 7420 3d3d 2062 2727 3a0a 2020 2020 2020  t == b'':.      
-00008270: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
-00008280: 7074 696f 6e28 2745 7272 6f72 2069 6e20  ption('Error in 
-00008290: 5363 616e 6e65 7220 5365 7269 616c 2063  Scanner Serial c
-000082a0: 6f6e 6e65 6374 696f 6e27 290a 2020 2020  onnection').    
-000082b0: 2020 2020 656c 6966 2074 2e73 7461 7274      elif t.start
-000082c0: 7377 6974 6828 6227 5c78 3036 2729 3a0a  swith(b'\x06'):.
-000082d0: 2020 2020 2020 2020 2020 2020 6966 2074              if t
-000082e0: 203d 3d20 6227 5c78 3036 465c 725c 6e27   == b'\x06F\r\n'
-000082f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008300: 2020 7365 6c66 2e73 6572 6961 6c5f 636f    self.serial_co
-00008310: 6e6e 6563 7469 6f6e 2e72 6573 6574 5f69  nnection.reset_i
-00008320: 6e70 7574 5f62 7566 6665 7228 290a 2020  nput_buffer().  
-00008330: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00008340: 6c66 2e73 6572 6961 6c5f 636f 6e6e 6563  lf.serial_connec
-00008350: 7469 6f6e 2e72 6573 6574 5f6f 7574 7075  tion.reset_outpu
-00008360: 745f 6275 6666 6572 2829 0a20 2020 2020  t_buffer().     
-00008370: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
-00008380: 2830 2e31 290a 2020 2020 2020 2020 2020  (0.1).          
-00008390: 2020 745f 636c 6561 6e20 3d20 745b 313a    t_clean = t[1:
-000083a0: 5d2e 6465 636f 6465 2829 2e73 7472 6970  ].decode().strip
-000083b0: 2829 2e72 6570 6c61 6365 2827 5c72 5c6e  ().replace('\r\n
-000083c0: 272c 2027 2729 0a20 2020 2020 2020 2020  ', '').         
-000083d0: 2020 2069 6620 745f 636c 6561 6e20 6973     if t_clean is
-000083e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000083f0: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00008400: 6e65 2c20 656c 6170 7365 645f 7469 6d65  ne, elapsed_time
-00008410: 5f6d 730a 2020 2020 2020 2020 2020 2020  _ms.            
-00008420: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00008430: 2020 2020 2020 7265 7475 726e 2074 5f63        return t_c
-00008440: 6c65 616e 2c20 656c 6170 7365 645f 7469  lean, elapsed_ti
-00008450: 6d65 5f6d 730a 2020 2020 2020 2020 656c  me_ms.        el
-00008460: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00008470: 7265 7475 726e 204e 6f6e 652c 2065 6c61  return None, ela
-00008480: 7073 6564 5f74 696d 655f 6d73 0a0a 2020  psed_time_ms..  
-00008490: 2020 6465 6620 7363 616e 5f65 7874 5f69    def scan_ext_i
-000084a0: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
-000084b0: 2022 2222 0a20 2020 2020 2020 2053 6361   """.        Sca
-000084c0: 6e20 7468 6520 6578 7465 726e 616c 2049  n the external I
-000084d0: 442e 0a20 2020 2020 2020 2022 2222 0a20  D..        """. 
-000084e0: 2020 2020 2020 2062 6172 636f 6465 5f72         barcode_r
-000084f0: 6561 6420 3d20 2727 0a20 2020 2020 2020  ead = ''.       
-00008500: 2073 7461 7274 5f74 696d 6520 3d20 7469   start_time = ti
-00008510: 6d65 2829 0a20 2020 2020 2020 2074 7279  me().        try
-00008520: 3a0a 2020 2020 2020 2020 2020 2020 6261  :.            ba
-00008530: 7263 6f64 655f 7265 6164 2c20 656c 6170  rcode_read, elap
-00008540: 7365 645f 7469 6d65 5f6d 7320 3d20 7365  sed_time_ms = se
-00008550: 6c66 2e73 6361 6e5f 616e 645f 666c 7573  lf.scan_and_flus
-00008560: 6828 290a 2020 2020 2020 2020 2020 2020  h().            
-00008570: 6966 2062 6172 636f 6465 5f72 6561 6420  if barcode_read 
-00008580: 6973 204e 6f6e 6520 6f72 2062 6172 636f  is None or barco
-00008590: 6465 5f72 6561 6420 3d3d 2727 3a0a 2020  de_read =='':.  
-000085a0: 2020 2020 2020 2020 2020 2020 2020 6261                ba
-000085b0: 7263 6f64 655f 7265 6164 203d 2027 270a  rcode_read = ''.
-000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085d0: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
-000085e0: 2745 7272 6f72 2069 6e20 5363 616e 6e65  'Error in Scanne
-000085f0: 7220 5365 7269 616c 2063 6f6e 6e65 6374  r Serial connect
-00008600: 696f 6e27 290a 2020 2020 2020 2020 2020  ion').          
-00008610: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00008620: 2020 2020 2020 2020 6675 6c6c 5f64 6174          full_dat
-00008630: 612c 2063 7572 5f69 642c 2072 6565 6c5f  a, cur_id, reel_
-00008640: 6964 2c20 6774 696e 203d 2073 656c 662e  id, gtin = self.
-00008650: 7265 6164 5f62 6172 636f 6465 2862 6172  read_barcode(bar
-00008660: 636f 6465 5f72 6561 6429 0a20 2020 2020  code_read).     
-00008670: 2020 2020 2020 2069 6620 7365 6c66 2e77         if self.w
-00008680: 7269 7465 5f74 6f5f 6c6f 673a 0a20 2020  rite_to_log:.   
-00008690: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-000086a0: 6820 6f70 656e 2873 656c 662e 6c6f 675f  h open(self.log_
-000086b0: 6669 6c65 6e61 6d65 2c20 2761 2729 2061  filename, 'a') a
-000086c0: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
-000086d0: 2020 2020 2020 2020 2074 696d 6573 7461           timesta
-000086e0: 6d70 203d 2064 6174 6574 696d 652e 6e6f  mp = datetime.no
-000086f0: 7728 292e 7374 7266 7469 6d65 2822 2559  w().strftime("%Y
-00008700: 2d25 6d2d 2564 2025 483a 254d 3a25 5322  -%m-%d %H:%M:%S"
-00008710: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008720: 2020 2020 2020 6c6f 675f 6d65 7373 6167        log_messag
-00008730: 6520 3d20 6622 7b74 696d 6573 7461 6d70  e = f"{timestamp
-00008740: 7d20 2d20 7b66 756c 6c5f 6461 7461 7d20  } - {full_data} 
-00008750: 2d20 456c 6170 7365 6420 5469 6d65 3a20  - Elapsed Time: 
-00008760: 7b65 6c61 7073 6564 5f74 696d 655f 6d73  {elapsed_time_ms
-00008770: 3a2e 3266 7d20 6d73 5c6e 220a 2020 2020  :.2f} ms\n".    
-00008780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008790: 662e 7772 6974 6528 6c6f 675f 6d65 7373  f.write(log_mess
-000087a0: 6167 6529 0a0a 2020 2020 2020 2020 2020  age)..          
-000087b0: 2020 7265 7475 726e 2066 756c 6c5f 6461    return full_da
-000087c0: 7461 2c20 6375 725f 6964 2c20 7265 656c  ta, cur_id, reel
-000087d0: 5f69 642c 2067 7469 6e0a 2020 2020 2020  _id, gtin.      
-000087e0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
-000087f0: 6f6e 2061 7320 653a 0a20 2020 2020 2020  on as e:.       
-00008800: 2020 2020 2073 656c 662e 7172 5f6c 6f67       self.qr_log
-00008810: 6765 722e 6572 726f 7228 6529 0a20 2020  ger.error(e).   
-00008820: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00008830: 4e6f 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65  None, None, None
-00008840: 2c20 4e6f 6e65 0a0a 2020 2020 6465 6620  , None..    def 
-00008850: 7265 6164 5f62 6172 636f 6465 2873 656c  read_barcode(sel
-00008860: 662c 2062 6172 636f 6465 5f72 6561 6429  f, barcode_read)
-00008870: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00008880: 2020 2020 2020 5265 6164 2074 6865 2062        Read the b
-00008890: 6172 636f 6465 2e0a 2020 2020 2020 2020  arcode..        
-000088a0: 2222 220a 2020 2020 2020 2020 7472 793a  """.        try:
-000088b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000088c0: 2728 3031 2927 2069 6e20 6261 7263 6f64  '(01)' in barcod
-000088d0: 655f 7265 6164 3a0a 2020 2020 2020 2020  e_read:.        
-000088e0: 2020 2020 2020 2020 6261 7263 6f64 6573          barcodes
-000088f0: 203d 2062 6172 636f 6465 5f72 6561 642e   = barcode_read.
-00008900: 7370 6c69 7428 2228 3031 2922 290a 2020  split("(01)").  
-00008910: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00008920: 7220 692c 2073 696e 676c 655f 6261 7263  r i, single_barc
-00008930: 6f64 6520 696e 2065 6e75 6d65 7261 7465  ode in enumerate
-00008940: 2862 6172 636f 6465 735b 313a 5d2c 2031  (barcodes[1:], 1
-00008950: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00008960: 2020 2020 2020 2066 756c 6c5f 6461 7461         full_data
-00008970: 203d 2066 2228 3031 297b 7369 6e67 6c65   = f"(01){single
-00008980: 5f62 6172 636f 6465 7d22 0a20 2020 2020  _barcode}".     
-00008990: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-000089a0: 7469 6e20 3d20 2729 272e 6a6f 696e 2866  tin = ')'.join(f
-000089b0: 756c 6c5f 6461 7461 2e73 706c 6974 2827  ull_data.split('
-000089c0: 2927 295b 3a32 5d29 202b 2027 2927 0a20  )')[:2]) + ')'. 
-000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089e0: 2020 2074 6167 5f64 6174 6120 3d20 6675     tag_data = fu
-000089f0: 6c6c 5f64 6174 612e 7370 6c69 7428 2729  ll_data.split(')
-00008a00: 2729 5b32 5d0a 2020 2020 2020 2020 2020  ')[2].          
-00008a10: 2020 2020 2020 2020 2020 6375 725f 6964            cur_id
-00008a20: 203d 2074 6167 5f64 6174 612e 7370 6c69   = tag_data.spli
-00008a30: 7428 2754 2729 5b31 5d2e 7374 7269 7028  t('T')[1].strip(
-00008a40: 2227 2022 292e 7370 6c69 7428 2728 2729  "' ").split('(')
-00008a50: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-00008a60: 2020 2020 2020 2020 7265 656c 5f69 6420          reel_id 
-00008a70: 3d20 7461 675f 6461 7461 2e73 706c 6974  = tag_data.split
-00008a80: 2827 5427 295b 305d 2e73 7472 6970 2822  ('T')[0].strip("
-00008a90: 2720 2229 0a0a 2020 2020 2020 2020 2020  ' ")..          
-00008aa0: 2020 2020 2020 2020 2020 6966 2066 756c            if ful
-00008ab0: 6c5f 6461 7461 2061 6e64 2063 7572 5f69  l_data and cur_i
-00008ac0: 6420 616e 6420 7265 656c 5f69 6420 616e  d and reel_id an
-00008ad0: 6420 6774 696e 3a0a 2020 2020 2020 2020  d gtin:.        
-00008ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008af0: 7365 6c66 2e71 725f 6c6f 6767 6572 2e69  self.qr_logger.i
-00008b00: 6e66 6f28 2757 696c 696f 7420 5152 2064  nfo('Wiliot QR d
-00008b10: 6574 6563 7465 6420 4754 696e 3a20 7b7d  etected GTin: {}
-00008b20: 2c20 5265 656c 3a20 7b7d 2c20 4944 3a7b  , Reel: {}, ID:{
-00008b30: 7d27 2e66 6f72 6d61 7428 6774 696e 2c20  }'.format(gtin, 
-00008b40: 6375 725f 6964 2c20 7265 656c 5f69 6429  cur_id, reel_id)
-00008b50: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008b60: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008b70: 2066 756c 6c5f 6461 7461 2c20 6375 725f   full_data, cur_
-00008b80: 6964 2c20 7265 656c 5f69 642c 2067 7469  id, reel_id, gti
-00008b90: 6e0a 2020 2020 2020 2020 2020 2020 656c  n.            el
-00008ba0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00008bb0: 2020 2020 6675 6c6c 5f64 6174 6120 3d20      full_data = 
-00008bc0: 6375 725f 6964 203d 2072 6565 6c5f 6964  cur_id = reel_id
-00008bd0: 203d 2067 7469 6e20 3d20 6261 7263 6f64   = gtin = barcod
-00008be0: 655f 7265 6164 0a20 2020 2020 2020 2020  e_read.         
-00008bf0: 2020 2020 2020 2067 7469 6e5f 7661 6c20         gtin_val 
-00008c00: 3d20 5472 7565 2069 6620 6c65 6e28 6675  = True if len(fu
-00008c10: 6c6c 5f64 6174 6129 203d 3d20 7365 6c66  ll_data) == self
-00008c20: 2e73 6774 696e 5f6c 656e 6774 6820 656c  .sgtin_length el
-00008c30: 7365 2046 616c 7365 0a20 2020 2020 2020  se False.       
-00008c40: 2020 2020 2020 2020 2069 6620 6774 696e           if gtin
-00008c50: 5f76 616c 3a0a 2020 2020 2020 2020 2020  _val:.          
-00008c60: 2020 2020 2020 2020 2020 6375 725f 6964            cur_id
-00008c70: 203d 2066 756c 6c5f 6461 7461 2e73 706c   = full_data.spl
-00008c80: 6974 2827 5427 295b 315d 2e73 7472 6970  it('T')[1].strip
-00008c90: 2822 2720 2229 2e73 706c 6974 2827 2827  ("' ").split('('
-00008ca0: 295b 305d 0a20 2020 2020 2020 2020 2020  )[0].           
-00008cb0: 2020 2020 2020 2020 2072 6565 6c5f 6964           reel_id
-00008cc0: 203d 2066 756c 6c5f 6461 7461 2e73 706c   = full_data.spl
-00008cd0: 6974 2827 5427 295b 305d 2e73 7472 6970  it('T')[0].strip
-00008ce0: 2822 2720 2229 5b2d 343a 5d0a 2020 2020  ("' ")[-4:].    
-00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d00: 6774 696e 203d 2066 756c 6c5f 6461 7461  gtin = full_data
-00008d10: 2e73 706c 6974 2827 5427 295b 305d 2e73  .split('T')[0].s
-00008d20: 7472 6970 2822 2720 2229 5b3a 2d34 5d0a  trip("' ")[:-4].
-00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d40: 2020 2020 7365 6c66 2e71 725f 6c6f 6767      self.qr_logg
-00008d50: 6572 2e69 6e66 6f28 2757 696c 696f 7420  er.info('Wiliot 
-00008d60: 5152 2064 6574 6563 7465 6420 4754 696e  QR detected GTin
-00008d70: 3a20 7b7d 2c20 5265 656c 3a20 7b7d 2c20  : {}, Reel: {}, 
-00008d80: 4944 3a7b 7d27 2e66 6f72 6d61 7428 6774  ID:{}'.format(gt
-00008d90: 696e 2c20 6375 725f 6964 2c20 7265 656c  in, cur_id, reel
-00008da0: 5f69 6429 290a 2020 2020 2020 2020 2020  _id)).          
-00008db0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00008dc0: 2066 756c 6c5f 6461 7461 2c20 6375 725f   full_data, cur_
-00008dd0: 6964 2c20 7265 656c 5f69 642c 2067 7469  id, reel_id, gti
-00008de0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00008df0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00008e00: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00008e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008e20: 2020 2020 2020 2020 2069 6620 6675 6c6c           if full
-00008e30: 5f64 6174 6120 3d3d 2027 4627 3a0a 2020  _data == 'F':.  
-00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e50: 2020 2020 2020 2020 2020 7365 6c66 2e71            self.q
-00008e60: 725f 6c6f 6767 6572 2e69 6e66 6f28 274e  r_logger.info('N
-00008e70: 6f20 6261 7263 6f64 6520 6465 7465 6374  o barcode detect
-00008e80: 6564 202d 2044 6563 6f64 696e 6720 7469  ed - Decoding ti
-00008e90: 6d65 6f75 7420 7265 6163 6865 6427 290a  meout reached').
-00008ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008eb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00008ec0: 726e 204e 6f6e 652c 204e 6f6e 652c 204e  rn None, None, N
-00008ed0: 6f6e 652c 204e 6f6e 650a 2020 2020 2020  one, None.      
-00008ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ef0: 2020 656c 6966 2066 756c 6c5f 6461 7461    elif full_data
-00008f00: 203d 3d20 2727 3a0a 2020 2020 2020 2020   == '':.        
-00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f20: 2020 2020 7261 6973 6520 4578 6365 7074      raise Except
-00008f30: 696f 6e28 2750 726f 626c 656d 2077 6974  ion('Problem wit
-00008f40: 6820 6261 7263 6f64 6520 7363 616e 6e65  h barcode scanne
-00008f50: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
-00008f60: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00008f70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008f80: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-00008f90: 725f 6964 203d 2066 756c 6c5f 6461 7461  r_id = full_data
-00008fa0: 2e73 706c 6974 2827 5427 295b 315d 0a20  .split('T')[1]. 
-00008fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fc0: 2020 2020 2020 2020 2020 2072 6565 6c5f             reel_
-00008fd0: 6964 203d 2066 756c 6c5f 6461 7461 2e73  id = full_data.s
-00008fe0: 706c 6974 2827 5427 295b 305d 0a20 2020  plit('T')[0].   
-00008ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009000: 2020 2020 2020 2020 2067 7469 6e20 3d20           gtin = 
-00009010: 2727 0a20 2020 2020 2020 2020 2020 2020  ''.             
-00009020: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00009030: 656c 662e 7172 5f6c 6f67 6765 722e 696e  elf.qr_logger.in
-00009040: 666f 2827 5769 6c69 6f74 2051 5220 6465  fo('Wiliot QR de
-00009050: 7465 6374 6564 2052 6565 6c3a 207b 7d2c  tected Reel: {},
-00009060: 2049 443a 7b7d 272e 666f 726d 6174 2863   ID:{}'.format(c
-00009070: 7572 5f69 642c 2072 6565 6c5f 6964 2929  ur_id, reel_id))
-00009080: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00009090: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
-000090a0: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
-000090b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090c0: 7365 6c66 2e71 725f 6c6f 6767 6572 2e69  self.qr_logger.i
-000090d0: 6e66 6f28 274e 6f74 2057 696c 696f 7420  nfo('Not Wiliot 
-000090e0: 6261 7263 6f64 6527 290a 0a20 2020 2020  barcode')..     
-000090f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009100: 6574 7572 6e20 6675 6c6c 5f64 6174 612c  eturn full_data,
-00009110: 2063 7572 5f69 642c 2072 6565 6c5f 6964   cur_id, reel_id
-00009120: 2c20 6774 696e 0a0a 2020 2020 2020 2020  , gtin..        
-00009130: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-00009140: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
-00009150: 2020 2073 656c 662e 7172 5f6c 6f67 6765     self.qr_logge
-00009160: 722e 6572 726f 7228 6622 4572 726f 7220  r.error(f"Error 
-00009170: 6475 7269 6e67 2072 6561 6469 6e67 2057  during reading W
-00009180: 696c 696f 7420 6261 7263 6f64 653a 207b  iliot barcode: {
-00009190: 657d 2229 0a20 2020 2020 2020 2020 2020  e}").           
-000091a0: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-000091b0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000091c0: 204e 6f6e 652c 204e 6f6e 652c 204e 6f6e   None, None, Non
-000091d0: 652c 204e 6f6e 650a 0a20 2020 2064 6566  e, None..    def
-000091e0: 2061 7574 6f5f 7363 616e 2873 656c 6629   auto_scan(self)
-000091f0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00009200: 2020 2020 2020 4175 746f 6d61 7469 6361        Automatica
-00009210: 6c6c 7920 7363 616e 2074 6865 2051 5220  lly scan the QR 
-00009220: 636f 6465 2e0a 2020 2020 2020 2020 2222  code..        ""
-00009230: 220a 2020 2020 2020 2020 7365 6c66 2e73  ".        self.s
-00009240: 6572 6961 6c5f 636f 6e6e 6563 7469 6f6e  erial_connection
-00009250: 2e77 7269 7465 2862 225c 7831 625c 7833  .write(b"\x1b\x3
-00009260: 3222 290a 2020 2020 2020 2020 7420 3d20  2").        t = 
-00009270: 7365 6c66 2e73 6572 6961 6c5f 636f 6e6e  self.serial_conn
-00009280: 6563 7469 6f6e 2e72 6561 645f 616c 6c28  ection.read_all(
-00009290: 290a 2020 2020 2020 2020 7365 6c66 2e71  ).        self.q
-000092a0: 725f 6c6f 6767 6572 2e69 6e66 6f28 6627  r_logger.info(f'
-000092b0: 6175 746f 2073 6361 6e3a 2067 6f74 206d  auto scan: got m
-000092c0: 7367 207b 747d 2729 0a20 2020 2020 2020  sg {t}').       
-000092d0: 2072 6574 7572 6e20 740a 0a20 2020 2064   return t..    d
-000092e0: 6566 2074 7269 6767 6572 5f73 746f 705f  ef trigger_stop_
-000092f0: 7365 7474 696e 6773 2873 656c 6629 3a0a  settings(self):.
-00009300: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00009310: 2020 2020 5472 6967 6765 7220 7374 6f70      Trigger stop
-00009320: 2073 6574 7469 6e67 732e 0a20 2020 2020   settings..     
-00009330: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-00009340: 6c65 6570 2830 2e30 3529 0a20 2020 2020  leep(0.05).     
-00009350: 2020 2074 203d 2073 656c 662e 7365 7269     t = self.seri
-00009360: 616c 5f63 6f6e 6e65 6374 696f 6e2e 7265  al_connection.re
-00009370: 6164 5f61 6c6c 2829 0a20 2020 2020 2020  ad_all().       
-00009380: 2073 6c65 6570 2830 2e30 3529 0a20 2020   sleep(0.05).   
-00009390: 2020 2020 2061 636b 7320 3d20 7374 7228       acks = str(
-000093a0: 7429 2e73 706c 6974 2827 3b27 295b 3a2d  t).split(';')[:-
-000093b0: 315d 0a20 2020 2020 2020 2069 7353 7563  1].        isSuc
-000093c0: 6365 7373 203d 2061 6c6c 285b 5472 7565  cess = all([True
-000093d0: 2069 6620 6163 6b2e 656e 6473 7769 7468   if ack.endswith
-000093e0: 2827 5c5c 7830 3627 2920 656c 7365 2046  ('\\x06') else F
-000093f0: 616c 7365 2066 6f72 2061 636b 2069 6e20  alse for ack in 
-00009400: 6163 6b73 5d29 0a20 2020 2020 2020 2072  acks]).        r
-00009410: 6574 7572 6e20 742c 2069 7353 7563 6365  eturn t, isSucce
-00009420: 7373 0a0a 0a63 6c61 7373 2059 6f63 746f  ss...class Yocto
-00009430: 5465 6d70 6572 6174 7572 6553 656e 736f  TemperatureSenso
-00009440: 7228 6f62 6a65 6374 293a 0a20 2020 2064  r(object):.    d
-00009450: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-00009460: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00009470: 7365 6e73 6f72 203d 204e 6f6e 650a 2020  sensor = None.  
-00009480: 2020 2020 2020 6572 726d 7367 203d 2059        errmsg = Y
-00009490: 5265 6650 6172 616d 2829 0a20 2020 2020  RefParam().     
-000094a0: 2020 2023 2053 6574 7570 2074 6865 2041     # Setup the A
-000094b0: 5049 2074 6f20 7573 6520 6c6f 6361 6c20  PI to use local 
-000094c0: 5553 4220 6465 7669 6365 730a 2020 2020  USB devices.    
-000094d0: 2020 2020 6966 2059 4150 492e 5265 6769      if YAPI.Regi
-000094e0: 7374 6572 4875 6228 2275 7362 222c 2065  sterHub("usb", e
-000094f0: 7272 6d73 6729 2021 3d20 5941 5049 2e53  rrmsg) != YAPI.S
-00009500: 5543 4345 5353 3a0a 2020 2020 2020 2020  UCCESS:.        
-00009510: 2020 2020 7261 6973 6520 4571 7569 706d      raise Equipm
-00009520: 656e 7445 7272 6f72 2827 796f 6374 6f20  entError('yocto 
-00009530: 7465 6d70 6572 6174 7572 6520 7365 6e73  temperature sens
-00009540: 6f72 2067 6f74 2069 6e69 7420 6572 726f  or got init erro
-00009550: 723a 207b 7d27 2e66 6f72 6d61 7428 6572  r: {}'.format(er
-00009560: 726d 7367 2e76 616c 7565 2929 0a0a 2020  rmsg.value))..  
-00009570: 2020 6465 6620 636f 6e6e 6563 7428 7365    def connect(se
-00009580: 6c66 2c20 7461 7267 6574 3d27 616e 7927  lf, target='any'
-00009590: 293a 0a20 2020 2020 2020 2069 6620 7461  ):.        if ta
-000095a0: 7267 6574 203d 3d20 2761 6e79 273a 0a20  rget == 'any':. 
-000095b0: 2020 2020 2020 2020 2020 2023 2072 6574             # ret
-000095c0: 7269 6576 6520 616e 7920 7465 6d70 6572  rieve any temper
-000095d0: 6174 7572 6520 7365 6e73 6f72 0a20 2020  ature sensor.   
-000095e0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
-000095f0: 6e73 6f72 203d 2059 5465 6d70 6572 6174  nsor = YTemperat
-00009600: 7572 652e 4669 7273 7454 656d 7065 7261  ure.FirstTempera
-00009610: 7475 7265 2829 0a20 2020 2020 2020 2065  ture().        e
-00009620: 6c69 6620 7461 7267 6574 203d 3d20 2727  lif target == ''
-00009630: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
-00009640: 696e 7428 2773 7065 6369 6669 6564 2069  int('specified i
-00009650: 6e76 616c 6964 2074 6172 6765 7427 290a  nvalid target').
-00009660: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00009670: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
-00009680: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00009690: 2020 2073 656c 662e 7365 6e73 6f72 203d     self.sensor =
-000096a0: 2059 5465 6d70 6572 6174 7572 652e 4669   YTemperature.Fi
-000096b0: 6e64 5465 6d70 6572 6174 7572 6528 7461  ndTemperature(ta
-000096c0: 7267 6574 202b 2027 2e74 656d 7065 7261  rget + '.tempera
-000096d0: 7475 7265 2729 0a20 2020 2020 2020 2069  ture').        i
-000096e0: 6620 7365 6c66 2e73 656e 736f 7220 6973  f self.sensor is
-000096f0: 204e 6f6e 6520 6f72 2073 656c 662e 6765   None or self.ge
-00009700: 745f 7365 6e73 6f72 5f6e 616d 6528 2920  t_sensor_name() 
-00009710: 3d3d 2027 756e 7265 736f 6c76 6564 273a  == 'unresolved':
-00009720: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00009730: 6e74 2827 4e6f 206d 6f64 756c 6520 636f  nt('No module co
-00009740: 6e6e 6563 7465 6427 290a 2020 2020 2020  nnected').      
-00009750: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00009760: 7365 0a20 2020 2020 2020 2065 6c73 653a  se.        else:
-00009770: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00009780: 7572 6e20 5472 7565 0a0a 2020 2020 6465  urn True..    de
-00009790: 6620 6765 745f 7365 6e73 6f72 5f6e 616d  f get_sensor_nam
-000097a0: 6528 7365 6c66 293a 0a20 2020 2020 2020  e(self):.       
-000097b0: 2069 6620 7365 6c66 2e73 656e 736f 7220   if self.sensor 
-000097c0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-000097d0: 2020 2020 2070 7269 6e74 2827 6e6f 2073       print('no s
-000097e0: 656e 736f 7220 6973 2063 6f6e 6e65 6374  ensor is connect
-000097f0: 6564 2e20 7472 7920 746f 2063 616c 6c20  ed. try to call 
-00009800: 636f 6e6e 6563 7428 2920 6669 7273 7427  connect() first'
-00009810: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00009820: 7475 726e 2027 270a 0a20 2020 2020 2020  turn ''..       
-00009830: 2073 656e 736f 725f 7374 7220 3d20 7365   sensor_str = se
-00009840: 6c66 2e73 656e 736f 722e 6465 7363 7269  lf.sensor.descri
-00009850: 6265 2829 0a20 2020 2020 2020 206e 616d  be().        nam
-00009860: 655f 7374 7220 3d20 7365 6e73 6f72 5f73  e_str = sensor_s
-00009870: 7472 2e73 706c 6974 2827 3d27 295b 315d  tr.split('=')[1]
-00009880: 2e73 706c 6974 2827 2e27 295b 305d 0a20  .split('.')[0]. 
-00009890: 2020 2020 2020 2072 6574 7572 6e20 6e61         return na
-000098a0: 6d65 5f73 7472 0a0a 2020 2020 6465 6620  me_str..    def 
-000098b0: 6765 745f 7465 6d70 6572 6174 7572 6528  get_temperature(
-000098c0: 7365 6c66 293a 0a20 2020 2020 2020 2069  self):.        i
-000098d0: 6620 7365 6c66 2e73 656e 736f 7220 6973  f self.sensor is
-000098e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000098f0: 2020 2070 7269 6e74 2827 7365 6e73 6f72     print('sensor
-00009900: 2069 7320 6e6f 7420 636f 6e6e 6563 7465   is not connecte
-00009910: 642e 2074 7279 2074 6f20 6361 6c6c 2063  d. try to call c
-00009920: 6f6e 6e65 6374 2829 2066 6972 7374 2729  onnect() first')
-00009930: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00009940: 7572 6e20 666c 6f61 7428 276e 616e 2729  urn float('nan')
-00009950: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00009960: 2873 656c 662e 7365 6e73 6f72 2e69 734f  (self.sensor.isO
-00009970: 6e6c 696e 6528 2929 3a0a 2020 2020 2020  nline()):.      
-00009980: 2020 2020 2020 7072 696e 7428 2773 656e        print('sen
-00009990: 736f 7220 6973 206e 6f74 2063 6f6e 6e65  sor is not conne
-000099a0: 6374 6564 206f 7220 6469 7363 6f6e 6e65  cted or disconne
-000099b0: 6374 6564 2064 7572 696e 6720 7275 6e27  cted during run'
-000099c0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-000099d0: 7475 726e 2066 6c6f 6174 2827 6e61 6e27  turn float('nan'
-000099e0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-000099f0: 6e20 7365 6c66 2e73 656e 736f 722e 6765  n self.sensor.ge
-00009a00: 745f 6375 7272 656e 7456 616c 7565 2829  t_currentValue()
-00009a10: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
-00009a20: 686f 640a 2020 2020 6465 6620 6578 6974  hod.    def exit
-00009a30: 5f61 7070 2829 3a0a 2020 2020 2020 2020  _app():.        
-00009a40: 5941 5049 2e46 7265 6541 5049 2829 0a    YAPI.FreeAPI().
+00004170: 2072 6574 7572 6e20 7365 6c66 2e73 2e69   return self.s.i
+00004180: 734f 7065 6e28 290a 2020 2020 2020 2020  sOpen().        
+00004190: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000041a0: 0a0a 2020 2020 2020 2020 6465 6620 5365  ..        def Se
+000041b0: 7461 7474 6e28 7365 6c66 2c20 6174 746e  tattn(self, attn
+000041c0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+000041d0: 6d64 203d 2022 4154 544e 207b 3a2e 3266  md = "ATTN {:.2f
+000041e0: 7d5c 725c 6e22 2e66 6f72 6d61 7428 6174  }\r\n".format(at
+000041f0: 746e 290a 2020 2020 2020 2020 2020 2020  tn).            
+00004200: 7365 6c66 2e57 7269 7465 2863 6d64 290a  self.Write(cmd).
+00004210: 2020 2020 2020 2020 2020 2020 7661 6c75              valu
+00004220: 6520 3d20 7365 6c66 2e47 6574 6174 746e  e = self.Getattn
+00004230: 2829 0a20 2020 2020 2020 2020 2020 2076  ().            v
+00004240: 616c 7565 203d 2066 6c6f 6174 2876 616c  alue = float(val
+00004250: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00004260: 6966 2076 616c 7565 2021 3d20 6174 746e  if value != attn
+00004270: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004280: 2020 7072 696e 7428 6627 4572 726f 7220    print(f'Error 
+00004290: 7365 7474 696e 6720 6174 7465 6e75 6174  setting attenuat
+000042a0: 696f 6e3a 206e 6577 203a 207b 6174 746e  ion: new : {attn
+000042b0: 7d20 6375 7272 656e 743a 207b 7661 6c75  } current: {valu
+000042c0: 657d 2729 0a20 2020 2020 2020 2020 2020  e}').           
+000042d0: 2072 6574 7572 6e20 7661 6c75 650a 0a20   return value.. 
+000042e0: 2020 2020 2020 2064 6566 2047 6574 6174         def Getat
+000042f0: 746e 2873 656c 6629 3a0a 2020 2020 2020  tn(self):.      
+00004300: 2020 2020 2020 636d 6420 3d20 2241 5454        cmd = "ATT
+00004310: 4e3f 5c72 5c6e 220a 2020 2020 2020 2020  N?\r\n".        
+00004320: 2020 2020 7661 6c75 6520 3d20 7365 6c66      value = self
+00004330: 2e51 7565 7279 2863 6d64 290a 2020 2020  .Query(cmd).    
+00004340: 2020 2020 2020 2020 7265 7475 726e 2076          return v
+00004350: 616c 7565 0a0a 0a63 6c61 7373 2054 6573  alue...class Tes
+00004360: 636f 6d3a 0a20 2020 2022 2222 0a20 2020  com:.    """.   
+00004370: 2043 6f6e 7472 6f6c 2054 4553 434f 4d20   Control TESCOM 
+00004380: 7465 7374 696e 6720 6368 616d 6265 7273  testing chambers
+00004390: 0a20 2020 2022 2222 0a20 2020 206f 7065  .    """.    ope
+000043a0: 6e5f 636d 6420 3d20 6227 4f50 454e 5c72  n_cmd = b'OPEN\r
+000043b0: 270a 2020 2020 636c 6f73 655f 636d 6420  '.    close_cmd 
+000043c0: 3d20 6227 434c 4f53 455c 7227 0a20 2020  = b'CLOSE\r'.   
+000043d0: 2063 6f6d 5f70 6f72 745f 6f62 6a20 3d20   com_port_obj = 
+000043e0: 4e6f 6e65 0a20 2020 206d 6f64 656c 735f  None.    models_
+000043f0: 6c69 7374 203d 205b 2754 432d 3530 3634  list = ['TC-5064
+00004400: 4327 2c20 2754 412d 3730 3131 4150 272c  C', 'TA-7011AP',
+00004410: 2027 5443 2d35 3036 3341 272c 2027 5443   'TC-5063A', 'TC
+00004420: 2d35 3937 3043 5027 5d0a 0a20 2020 2064  -5970CP']..    d
+00004430: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00004440: 2c20 706f 7274 3d4e 6f6e 6529 3a0a 2020  , port=None):.  
+00004450: 2020 2020 2020 7365 6c66 2e70 6f72 7420        self.port 
+00004460: 3d20 706f 7274 0a20 2020 2020 2020 2074  = port.        t
+00004470: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00004480: 6966 2070 6f72 7420 6973 206e 6f74 204e  if port is not N
+00004490: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000044a0: 2020 2020 2073 656c 662e 636f 6e6e 6563       self.connec
+000044b0: 7428 706f 7274 290a 0a20 2020 2020 2020  t(port)..       
+000044c0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+000044d0: 6e20 6173 2065 3a0a 2020 2020 2020 2020  n as e:.        
+000044e0: 2020 2020 7072 696e 7428 6529 0a20 2020      print(e).   
+000044f0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00004500: 5465 7363 6f6d 202d 2043 6f6e 6e65 6374  Tescom - Connect
+00004510: 696f 6e20 6661 696c 6564 2229 0a0a 2020  ion failed")..  
+00004520: 2020 6465 6620 636f 6e6e 6563 7428 7365    def connect(se
+00004530: 6c66 2c20 706f 7274 293a 0a20 2020 2020  lf, port):.     
+00004540: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00004550: 7061 7261 6d20 706f 7274 3a20 636f 6d20  param port: com 
+00004560: 706f 7274 2074 6f20 636f 6e6e 6563 740a  port to connect.
+00004570: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00004580: 2063 6f6d 2070 6f72 7420 6f62 6a0a 2020   com port obj.  
+00004590: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000045a0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000045b0: 2020 2063 6f6d 5f70 6f72 745f 6f62 6a20     com_port_obj 
+000045c0: 3d20 7365 6c66 2e63 6f6d 5f70 6f72 745f  = self.com_port_
+000045d0: 6f62 6a20 3d20 7365 7269 616c 2e53 6572  obj = serial.Ser
+000045e0: 6961 6c28 706f 7274 3d70 6f72 742c 2062  ial(port=port, b
+000045f0: 6175 6472 6174 653d 3936 3030 2c20 7469  audrate=9600, ti
+00004600: 6d65 6f75 743d 3129 0a20 2020 2020 2020  meout=1).       
+00004610: 2020 2020 2069 6620 636f 6d5f 706f 7274       if com_port
+00004620: 5f6f 626a 2069 7320 6e6f 7420 4e6f 6e65  _obj is not None
+00004630: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004640: 2020 7365 6c66 2e64 6f6f 725f 636d 6420    self.door_cmd 
+00004650: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00004660: 2020 2020 2020 2073 656c 662e 636f 6d5f         self.com_
+00004670: 706f 7274 5f6f 626a 2e77 7269 7465 2862  port_obj.write(b
+00004680: 274d 4f44 454c 3f5c 7227 290a 2020 2020  'MODEL?\r').    
+00004690: 2020 2020 2020 2020 2020 2020 736c 6565              slee
+000046a0: 7028 302e 3129 0a20 2020 2020 2020 2020  p(0.1).         
+000046b0: 2020 2020 2020 206d 6f64 656c 203d 2073         model = s
+000046c0: 7472 2873 656c 662e 636f 6d5f 706f 7274  tr(self.com_port
+000046d0: 5f6f 626a 2e72 6561 6428 3134 2929 0a20  _obj.read(14)). 
+000046e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000046f0: 6172 7473 203d 205b 7020 666f 7220 7020  arts = [p for p 
+00004700: 696e 206d 6f64 656c 2e73 706c 6974 2822  in model.split("
+00004710: 2722 295d 0a20 2020 2020 2020 2020 2020  '")].           
+00004720: 2020 2020 2070 6172 7473 203d 205b 7020       parts = [p 
+00004730: 666f 7220 7020 696e 2070 6172 7473 5b31  for p in parts[1
+00004740: 5d2e 7370 6c69 7428 2220 2229 5d0a 2020  ].split(" ")].  
+00004750: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00004760: 6c66 2e6d 6f64 656c 203d 2070 6172 7473  lf.model = parts
+00004770: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00004780: 2020 2020 6966 206c 656e 2873 656c 662e      if len(self.
+00004790: 6d6f 6465 6c29 203e 2030 3a0a 2020 2020  model) > 0:.    
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 7072 696e 7428 2252 4620 6368 616d 6265  print("RF chambe
+000047c0: 7220 636f 6e6e 6563 7465 6420 746f 2070  r connected to p
+000047d0: 6f72 7420 2220 2b20 7374 7228 706f 7274  ort " + str(port
+000047e0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+000047f0: 2020 2020 2020 2070 7269 6e74 2822 5465         print("Te
+00004800: 7363 6f6d 202d 2043 6861 6d62 6572 206d  scom - Chamber m
+00004810: 6f64 656c 3a22 2c20 7365 6c66 2e6d 6f64  odel:", self.mod
+00004820: 656c 290a 2020 2020 2020 2020 2020 2020  el).            
+00004830: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00004840: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00004850: 696e 7428 2254 6573 636f 6d20 2d20 4572  int("Tescom - Er
+00004860: 726f 7221 204e 6f20 6368 616d 6265 7220  ror! No chamber 
+00004870: 666f 756e 6422 290a 2020 2020 2020 2020  found").        
+00004880: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00004890: 726e 0a20 2020 2020 2020 2020 2020 2020  rn.             
+000048a0: 2020 2069 6620 7365 6c66 2e6d 6f64 656c     if self.model
+000048b0: 2069 6e20 7365 6c66 2e6d 6f64 656c 735f   in self.models_
+000048c0: 6c69 7374 3a0a 2020 2020 2020 2020 2020  list:.          
+000048d0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000048e0: 6f6f 725f 636d 6420 3d20 6227 444f 4f52  oor_cmd = b'DOOR
+000048f0: 3f5c 7227 0a20 2020 2020 2020 2020 2020  ?\r'.           
+00004900: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00004910: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004920: 656c 662e 646f 6f72 5f63 6d64 203d 2062  elf.door_cmd = b
+00004930: 274c 4944 3f5c 7227 0a20 2020 2020 2020  'LID?\r'.       
+00004940: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00004950: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00004960: 2045 7863 6570 7469 6f6e 0a20 2020 2020   Exception.     
+00004970: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00004980: 696f 6e20 6173 2065 3a0a 2020 2020 2020  ion as e:.      
+00004990: 2020 2020 2020 2320 7072 696e 7428 6529        # print(e)
+000049a0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+000049b0: 6e74 2828 2254 6573 636f 6d20 2d20 436f  nt(("Tescom - Co
+000049c0: 756c 6420 6e6f 7420 636f 6e6e 6563 7420  uld not connect 
+000049d0: 746f 2070 6f72 7420 2220 2b20 706f 7274  to port " + port
+000049e0: 2929 0a20 2020 2020 2020 2020 2020 2072  )).            r
+000049f0: 6574 7572 6e20 4e6f 6e65 0a0a 2020 2020  eturn None..    
+00004a00: 6465 6620 636c 6f73 655f 706f 7274 2873  def close_port(s
+00004a10: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00004a20: 220a 2020 2020 2020 2020 636c 6f73 6573  ".        closes
+00004a30: 2063 6f6d 2070 6f72 740a 2020 2020 2020   com port.      
+00004a40: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
+00004a50: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
+00004a60: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
+00004a70: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+00004a80: 2020 2020 2070 7269 6e74 2822 5246 2063       print("RF c
+00004a90: 6861 6d62 6572 2064 6973 636f 6e6e 6563  hamber disconnec
+00004aa0: 7465 6420 6672 6f6d 2070 6f72 743a 2022  ted from port: "
+00004ab0: 202b 2073 7472 2873 656c 662e 706f 7274   + str(self.port
+00004ac0: 2929 0a20 2020 2020 2020 2065 7863 6570  )).        excep
+00004ad0: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+00004ae0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00004af0: 696e 7428 2243 6f75 6c64 206e 6f74 2064  int("Could not d
+00004b00: 6973 636f 6e6e 6563 7422 290a 0a20 2020  isconnect")..   
+00004b10: 2064 6566 206f 7065 6e5f 6368 616d 6265   def open_chambe
+00004b20: 7228 7365 6c66 293a 0a20 2020 2020 2020  r(self):.       
+00004b30: 2022 2222 0a20 2020 2020 2020 206f 7065   """.        ope
+00004b40: 6e73 2063 6861 6d62 6572 0a20 2020 2020  ns chamber.     
+00004b50: 2020 203a 7265 7475 726e 3a20 224f 4b22     :return: "OK"
+00004b60: 2069 6620 636f 6d6d 616e 6420 7761 7320   if command was 
+00004b70: 7375 6363 6573 7366 756c 0a20 2020 2020  successful.     
+00004b80: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00004b90: 6620 7365 6c66 2e69 735f 646f 6f72 5f6f  f self.is_door_o
+00004ba0: 7065 6e28 293a 0a20 2020 2020 2020 2020  pen():.         
+00004bb0: 2020 2070 7269 6e74 2822 4368 616d 6265     print("Chambe
+00004bc0: 7220 6973 206f 7065 6e22 290a 2020 2020  r is open").    
+00004bd0: 2020 2020 2020 2020 7265 7475 726e 2027          return '
+00004be0: 4f4b 270a 2020 2020 2020 2020 7472 793a  OK'.        try:
+00004bf0: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00004c00: 6e74 2866 2243 6861 6d62 6572 207b 7365  nt(f"Chamber {se
+00004c10: 6c66 2e70 6f72 747d 2069 7320 6f70 656e  lf.port} is open
+00004c20: 696e 6722 290a 2020 2020 2020 2020 2020  ing").          
+00004c30: 2020 7365 6c66 2e63 6f6d 5f70 6f72 745f    self.com_port_
+00004c40: 6f62 6a2e 7265 7365 745f 696e 7075 745f  obj.reset_input_
+00004c50: 6275 6666 6572 2829 0a20 2020 2020 2020  buffer().       
+00004c60: 2020 2020 2073 656c 662e 636f 6d5f 706f       self.com_po
+00004c70: 7274 5f6f 626a 2e72 6573 6574 5f6f 7574  rt_obj.reset_out
+00004c80: 7075 745f 6275 6666 6572 2829 0a20 2020  put_buffer().   
+00004c90: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+00004ca0: 6d5f 706f 7274 5f6f 626a 2e77 7269 7465  m_port_obj.write
+00004cb0: 2873 656c 662e 6f70 656e 5f63 6d64 290a  (self.open_cmd).
+00004cc0: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00004cd0: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
+00004ce0: 2077 6169 745f 636f 756e 7465 7220 3d20   wait_counter = 
+00004cf0: 300a 2020 2020 2020 2020 2020 2020 7768  0.            wh
+00004d00: 696c 6520 274f 4b27 206e 6f74 2069 6e20  ile 'OK' not in 
+00004d10: 7265 733a 0a20 2020 2020 2020 2020 2020  res:.           
+00004d20: 2020 2020 2069 6620 7761 6974 5f63 6f75       if wait_cou
+00004d30: 6e74 6572 203e 3d20 3135 3a0a 2020 2020  nter >= 15:.    
+00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d50: 7261 6973 6520 4578 6365 7074 696f 6e28  raise Exception(
+00004d60: 6622 4572 726f 7220 696e 206f 7065 6e69  f"Error in openi
+00004d70: 6e67 2063 6861 6d62 6572 207b 7365 6c66  ng chamber {self
+00004d80: 2e70 6f72 747d 2229 0a20 2020 2020 2020  .port}").       
+00004d90: 2020 2020 2020 2020 2072 6573 203d 2073           res = s
+00004da0: 656c 662e 636f 6d5f 706f 7274 5f6f 626a  elf.com_port_obj
+00004db0: 2e72 6561 6428 3134 292e 6465 636f 6465  .read(14).decode
+00004dc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004dd0: 2020 2020 2020 2775 7466 2d38 2729 2e75        'utf-8').u
+00004de0: 7070 6572 2829 2e72 7374 7269 7028 275c  pper().rstrip('\
+00004df0: 7227 290a 2020 2020 2020 2020 2020 2020  r').            
+00004e00: 2020 2020 6966 206c 656e 2873 7472 2872      if len(str(r
+00004e10: 6573 2929 203e 2030 3a0a 2020 2020 2020  es)) > 0:.      
+00004e20: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00004e30: 696e 7428 6627 4368 616d 6265 7220 7b73  int(f'Chamber {s
+00004e40: 656c 662e 706f 7274 7d20 7374 6174 7573  elf.port} status
+00004e50: 3a20 2720 2b20 7374 7228 7265 7329 290a  : ' + str(res)).
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 7761 6974 5f63 6f75 6e74 6572 202b 3d20  wait_counter += 
+00004e80: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00004e90: 2020 736c 6565 7028 302e 3129 0a20 2020    sleep(0.1).   
+00004ea0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00004eb0: 7365 6c66 2e69 735f 646f 6f72 5f6f 7065  self.is_door_ope
+00004ec0: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
+00004ed0: 2020 2020 2072 6169 7365 2045 7863 6570       raise Excep
+00004ee0: 7469 6f6e 280a 2020 2020 2020 2020 2020  tion(.          
+00004ef0: 2020 2020 2020 2020 2020 6622 7b73 656c            f"{sel
+00004f00: 662e 706f 7274 7d20 446f 6f72 2073 7461  f.port} Door sta
+00004f10: 7475 7320 646f 6573 6e27 7420 6d61 7463  tus doesn't matc
+00004f20: 6820 636f 6d6d 616e 6420 7365 6e74 2122  h command sent!"
+00004f30: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00004f40: 696e 7428 6622 4368 616d 6265 7220 7b73  int(f"Chamber {s
+00004f50: 656c 662e 706f 7274 7d20 6973 206f 7065  elf.port} is ope
+00004f60: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+00004f70: 7265 7475 726e 2027 4f4b 270a 2020 2020  return 'OK'.    
+00004f80: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00004f90: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+00004fa0: 2020 2020 2020 2070 7269 6e74 2865 290a         print(e).
+00004fb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00004fc0: 726e 2022 4641 494c 220a 0a20 2020 2064  rn "FAIL"..    d
+00004fd0: 6566 2063 6c6f 7365 5f63 6861 6d62 6572  ef close_chamber
+00004fe0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00004ff0: 2222 220a 2020 2020 2020 2020 636c 6f73  """.        clos
+00005000: 6573 2063 6861 6d62 6572 0a20 2020 2020  es chamber.     
+00005010: 2020 203a 7265 7475 726e 3a20 224f 4b22     :return: "OK"
+00005020: 2069 6620 636f 6d6d 616e 6420 7761 7320   if command was 
+00005030: 7375 6363 6573 7366 756c 0a20 2020 2020  successful.     
+00005040: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00005050: 6620 7365 6c66 2e69 735f 646f 6f72 5f63  f self.is_door_c
+00005060: 6c6f 7365 6428 293a 0a20 2020 2020 2020  losed():.       
+00005070: 2020 2020 2070 7269 6e74 2822 4368 616d       print("Cham
+00005080: 6265 7220 636c 6f73 6564 2229 0a20 2020  ber closed").   
+00005090: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000050a0: 274f 4b27 0a20 2020 2020 2020 2074 7279  'OK'.        try
+000050b0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+000050c0: 696e 7428 6622 4348 414d 4245 5220 7b73  int(f"CHAMBER {s
+000050d0: 656c 662e 706f 7274 7d20 4953 2043 4c4f  elf.port} IS CLO
+000050e0: 5349 4e47 2c20 434c 4541 5220 4841 4e44  SING, CLEAR HAND
+000050f0: 5321 2121 2229 0a20 2020 2020 2020 2020  S!!!").         
+00005100: 2020 2073 6c65 6570 2832 290a 2020 2020     sleep(2).    
+00005110: 2020 2020 2020 2020 7365 6c66 2e63 6f6d          self.com
+00005120: 5f70 6f72 745f 6f62 6a2e 7772 6974 6528  _port_obj.write(
+00005130: 7365 6c66 2e63 6c6f 7365 5f63 6d64 290a  self.close_cmd).
+00005140: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00005150: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
+00005160: 2077 6169 745f 636f 756e 7465 7220 3d20   wait_counter = 
+00005170: 300a 2020 2020 2020 2020 2020 2020 7768  0.            wh
+00005180: 696c 6520 2752 4541 4459 2720 6e6f 7420  ile 'READY' not 
+00005190: 696e 2072 6573 3a0a 2020 2020 2020 2020  in res:.        
+000051a0: 2020 2020 2020 2020 6966 2077 6169 745f          if wait_
+000051b0: 636f 756e 7465 7220 3e3d 2032 303a 0a20  counter >= 20:. 
+000051c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051d0: 2020 2072 6169 7365 2045 7863 6570 7469     raise Excepti
+000051e0: 6f6e 2866 2245 7272 6f72 2069 6e20 636c  on(f"Error in cl
+000051f0: 6f73 696e 6720 6368 616d 6265 7220 7b73  osing chamber {s
+00005200: 656c 662e 706f 7274 7d22 290a 2020 2020  elf.port}").    
+00005210: 2020 2020 2020 2020 2020 2020 7265 7320              res 
+00005220: 3d20 7365 6c66 2e63 6f6d 5f70 6f72 745f  = self.com_port_
+00005230: 6f62 6a2e 7265 6164 2831 3429 2e64 6563  obj.read(14).dec
+00005240: 6f64 6528 0a20 2020 2020 2020 2020 2020  ode(.           
+00005250: 2020 2020 2020 2020 2027 7574 662d 3827           'utf-8'
+00005260: 292e 7570 7065 7228 292e 7273 7472 6970  ).upper().rstrip
+00005270: 2827 5c72 2729 0a20 2020 2020 2020 2020  ('\r').         
+00005280: 2020 2020 2020 2069 6620 2745 5252 2720         if 'ERR' 
+00005290: 696e 2072 6573 206f 7220 2752 4541 4459  in res or 'READY
+000052a0: 2720 696e 2072 6573 206f 7220 274f 4b27  ' in res or 'OK'
+000052b0: 2069 6e20 7265 733a 0a20 2020 2020 2020   in res:.       
+000052c0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000052d0: 6e74 2866 2743 6861 6d62 6572 207b 7365  nt(f'Chamber {se
+000052e0: 6c66 2e70 6f72 747d 2073 7461 7475 733a  lf.port} status:
+000052f0: 2027 202b 2073 7472 2872 6573 2929 0a20   ' + str(res)). 
+00005300: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00005310: 6620 2745 5252 2720 696e 2072 6573 3a0a  f 'ERR' in res:.
+00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005330: 2020 2020 7265 7475 726e 2022 4641 494c      return "FAIL
+00005340: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00005350: 2020 7761 6974 5f63 6f75 6e74 6572 202b    wait_counter +
+00005360: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00005370: 2020 2020 736c 6565 7028 302e 3129 0a20      sleep(0.1). 
+00005380: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00005390: 7420 7365 6c66 2e69 735f 646f 6f72 5f63  t self.is_door_c
+000053a0: 6c6f 7365 6428 293a 0a20 2020 2020 2020  losed():.       
+000053b0: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+000053c0: 7863 6570 7469 6f6e 280a 2020 2020 2020  xception(.      
+000053d0: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+000053e0: 7b73 656c 662e 706f 7274 7d20 446f 6f72  {self.port} Door
+000053f0: 2073 7461 7475 7320 646f 6573 6e27 7420   status doesn't 
+00005400: 6d61 7463 6820 636f 6d6d 616e 6420 7365  match command se
+00005410: 6e74 2122 290a 2020 2020 2020 2020 2020  nt!").          
+00005420: 2020 7072 696e 7428 6622 4368 616d 6265    print(f"Chambe
+00005430: 7220 7b73 656c 662e 706f 7274 7d20 636c  r {self.port} cl
+00005440: 6f73 6564 2229 0a20 2020 2020 2020 2020  osed").         
+00005450: 2020 2072 6574 7572 6e20 274f 4b27 0a20     return 'OK'. 
+00005460: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
+00005470: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
+00005480: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00005490: 6622 4572 726f 7220 696e 2063 6c6f 7369  f"Error in closi
+000054a0: 6e67 2063 6861 6d62 6572 207b 7365 6c66  ng chamber {self
+000054b0: 2e70 6f72 747d 2229 0a20 2020 2020 2020  .port}").       
+000054c0: 2020 2020 2070 7269 6e74 2865 290a 2020       print(e).  
+000054d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000054e0: 2022 4641 494c 220a 0a20 2020 2064 6566   "FAIL"..    def
+000054f0: 2069 735f 636f 6e6e 6563 7465 6428 7365   is_connected(se
+00005500: 6c66 293a 0a20 2020 2020 2020 2069 6620  lf):.        if 
+00005510: 7365 6c66 2e63 6f6d 5f70 6f72 745f 6f62  self.com_port_ob
+00005520: 6a20 6973 204e 6f6e 653a 0a20 2020 2020  j is None:.     
+00005530: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00005540: 6c73 650a 2020 2020 2020 2020 7265 7475  lse.        retu
+00005550: 726e 2073 656c 662e 636f 6d5f 706f 7274  rn self.com_port
+00005560: 5f6f 626a 2e69 734f 7065 6e28 290a 0a20  _obj.isOpen().. 
+00005570: 2020 2064 6566 2067 6574 5f73 7461 7465     def get_state
+00005580: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00005590: 7365 6c66 2e63 6f6d 5f70 6f72 745f 6f62  self.com_port_ob
+000055a0: 6a2e 7265 7365 745f 696e 7075 745f 6275  j.reset_input_bu
+000055b0: 6666 6572 2829 0a20 2020 2020 2020 2073  ffer().        s
+000055c0: 6c65 6570 2830 2e31 290a 2020 2020 2020  leep(0.1).      
+000055d0: 2020 7365 6c66 2e63 6f6d 5f70 6f72 745f    self.com_port_
+000055e0: 6f62 6a2e 7772 6974 6528 7365 6c66 2e64  obj.write(self.d
+000055f0: 6f6f 725f 636d 6429 0a20 2020 2020 2020  oor_cmd).       
+00005600: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
+00005610: 2020 2020 7374 6174 6520 3d20 7365 6c66      state = self
+00005620: 2e63 6f6d 5f70 6f72 745f 6f62 6a2e 7265  .com_port_obj.re
+00005630: 6164 2831 3429 2e64 6563 6f64 6528 2775  ad(14).decode('u
+00005640: 7466 2d38 2729 2e75 7070 6572 2829 2e72  tf-8').upper().r
+00005650: 7374 7269 7028 275c 7227 290a 2020 2020  strip('\r').    
+00005660: 2020 2020 7265 7475 726e 2073 7461 7465      return state
+00005670: 0a0a 2020 2020 6465 6620 6973 5f64 6f6f  ..    def is_doo
+00005680: 725f 6f70 656e 2873 656c 6629 3a0a 2020  r_open(self):.  
+00005690: 2020 2020 2020 7374 6174 6520 3d20 7365        state = se
+000056a0: 6c66 2e67 6574 5f73 7461 7465 2829 0a20  lf.get_state(). 
+000056b0: 2020 2020 2020 2069 6620 274f 5045 4e27         if 'OPEN'
+000056c0: 2069 6e20 7374 6174 653a 0a20 2020 2020   in state:.     
+000056d0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+000056e0: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+000056f0: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+00005700: 2069 735f 646f 6f72 5f63 6c6f 7365 6428   is_door_closed(
+00005710: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
+00005720: 7461 7465 203d 2073 656c 662e 6765 745f  tate = self.get_
+00005730: 7374 6174 6528 290a 2020 2020 2020 2020  state().        
+00005740: 6966 2027 434c 4f53 4527 2069 6e20 7374  if 'CLOSE' in st
+00005750: 6174 653a 0a20 2020 2020 2020 2020 2020  ate:.           
+00005760: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00005770: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00005780: 650a 0a0a 636c 6173 7320 4261 7263 6f64  e...class Barcod
+00005790: 6553 6361 6e6e 6572 286f 626a 6563 7429  eScanner(object)
+000057a0: 3a0a 2020 2020 7072 6566 6978 203d 2027  :.    prefix = '
+000057b0: 7e01 3030 3030 4027 0a20 2020 2073 7566  ~.0000@'.    suf
+000057c0: 6669 7820 3d20 273b 0327 0a20 2020 2063  fix = ';.'.    c
+000057d0: 6f6d 203d 2027 270a 2020 2020 7365 7269  om = ''.    seri
+000057e0: 616c 203d 204e 6f6e 650a 0a20 2020 2064  al = None..    d
+000057f0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00005800: 2c20 636f 6d3d 4e6f 6e65 2c20 6261 7564  , com=None, baud
+00005810: 3d31 3135 3230 302c 2063 6f6e 6669 673d  =115200, config=
+00005820: 5472 7565 2c20 6c6f 675f 7479 7065 3d27  True, log_type='
+00005830: 4e4f 5f4c 4f47 2729 3a0a 2020 2020 2020  NO_LOG'):.      
+00005840: 2020 7365 6c66 2e6c 6f67 5f74 7970 6520    self.log_type 
+00005850: 3d20 6c6f 675f 7479 7065 0a20 2020 2020  = log_type.     
+00005860: 2020 2069 6620 636f 6d20 213d 204e 6f6e     if com != Non
+00005870: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00005880: 656c 662e 6f70 656e 5f70 6f72 7428 636f  elf.open_port(co
+00005890: 6d2c 2062 6175 643d 6261 7564 2c20 636f  m, baud=baud, co
+000058a0: 6e66 6967 3d63 6f6e 6669 6729 0a20 2020  nfig=config).   
+000058b0: 2020 2020 2023 2065 6c73 653a 0a20 2020       # else:.   
+000058c0: 2020 2020 2023 2020 2020 2073 656c 662e       #     self.
+000058d0: 7365 7269 616c 203d 2073 6572 203d 2053  serial = ser = S
+000058e0: 6572 6961 6c28 290a 0a20 2020 2064 6566  erial()..    def
+000058f0: 206f 7065 6e5f 706f 7274 2873 656c 662c   open_port(self,
+00005900: 2063 6f6d 2c20 6261 7564 3d31 3135 3230   com, baud=11520
+00005910: 302c 2063 6f6e 6669 673d 5472 7565 293a  0, config=True):
+00005920: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00005930: 2e73 6572 6961 6c20 213d 204e 6f6e 6520  .serial != None 
+00005940: 616e 6420 7365 6c66 2e73 6572 6961 6c2e  and self.serial.
+00005950: 6973 5f6f 7065 6e28 293a 0a20 2020 2020  is_open():.     
+00005960: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
+00005970: 616c 2e63 6c6f 7365 506f 7274 2829 0a20  al.closePort(). 
+00005980: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
+00005990: 616c 203d 2073 6572 203d 2073 6572 6961  al = ser = seria
+000059a0: 6c2e 5365 7269 616c 2863 6f6d 2c20 6261  l.Serial(com, ba
+000059b0: 7564 2c20 7469 6d65 6f75 743d 302e 3529  ud, timeout=0.5)
+000059c0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000059d0: 7365 6c66 2e63 6865 636b 5f63 6f6d 5f70  self.check_com_p
+000059e0: 6f72 7428 293a 0a20 2020 2020 2020 2020  ort():.         
+000059f0: 2020 2070 7269 6e74 2866 277b 636f 6d7d     print(f'{com}
+00005a00: 2069 7320 6e6f 7420 6261 7263 6f64 6520   is not barcode 
+00005a10: 7363 616e 6e65 7227 290a 2020 2020 2020  scanner').      
+00005a20: 2020 6966 2073 6572 2021 3d20 4e6f 6e65    if ser != None
+00005a30: 2061 6e64 2073 656c 662e 6c6f 675f 7479   and self.log_ty
+00005a40: 7065 2021 3d20 274e 4f5f 4c4f 4727 3a0a  pe != 'NO_LOG':.
+00005a50: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00005a60: 7428 6627 4261 7263 6f64 6520 7363 616e  t(f'Barcode scan
+00005a70: 6e65 7220 287b 636f 6d7d 2920 636f 6e6e  ner ({com}) conn
+00005a80: 6563 7465 642e 2729 0a20 2020 2020 2020  ected.').       
+00005a90: 2065 6c69 6620 7365 7220 3d3d 204e 6f6e   elif ser == Non
+00005aa0: 653a 0a20 2020 2020 2020 2020 2020 2070  e:.            p
+00005ab0: 7269 6e74 2866 2742 6172 636f 6465 2073  rint(f'Barcode s
+00005ac0: 6361 6e6e 6572 202d 2050 726f 626c 656d  canner - Problem
+00005ad0: 2063 6f6e 6e65 6374 696e 6720 7b63 6f6d   connecting {com
+00005ae0: 7d27 290a 2020 2020 2020 2020 7365 6c66  }').        self
+00005af0: 2e63 6f6d 203d 2063 6f6d 0a20 2020 2020  .com = com.     
+00005b00: 2020 2073 6572 2e74 696d 6572 6f75 7420     ser.timerout 
+00005b10: 3d20 3120 2023 2072 6561 6420 7469 6d65  = 1  # read time
+00005b20: 206f 7574 0a20 2020 2020 2020 2073 6572   out.        ser
+00005b30: 2e77 7269 7465 5469 6d65 6f75 7420 3d20  .writeTimeout = 
+00005b40: 302e 3520 2023 2077 7269 7465 2074 696d  0.5  # write tim
+00005b50: 6520 6f75 742e 0a20 2020 2020 2020 2069  e out..        i
+00005b60: 6620 636f 6e66 6967 3a0a 2020 2020 2020  f config:.      
+00005b70: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
+00005b80: 6775 7265 2829 0a0a 2020 2020 6465 6620  gure()..    def 
+00005b90: 6669 6e64 5f61 6e64 5f6f 7065 6e5f 706f  find_and_open_po
+00005ba0: 7274 2873 656c 662c 2062 6175 643d 3131  rt(self, baud=11
+00005bb0: 3532 3030 2c20 636f 6e66 6967 3d54 7275  5200, config=Tru
+00005bc0: 6529 3a0a 2020 2020 2020 2020 636f 6d20  e):.        com 
+00005bd0: 3d20 7365 6c66 2e66 696e 645f 636f 6d5f  = self.find_com_
+00005be0: 706f 7274 2862 6175 6429 0a20 2020 2020  port(baud).     
+00005bf0: 2020 2069 6620 636f 6d20 6973 206e 6f74     if com is not
+00005c00: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005c10: 2020 2073 656c 662e 6f70 656e 5f70 6f72     self.open_por
+00005c20: 7428 636f 6d2c 2062 6175 642c 2063 6f6e  t(com, baud, con
+00005c30: 6669 6729 0a20 2020 2020 2020 2020 2020  fig).           
+00005c40: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00005c50: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+00005c60: 650a 0a20 2020 2064 6566 2066 696e 645f  e..    def find_
+00005c70: 636f 6d5f 706f 7274 2873 656c 662c 2062  com_port(self, b
+00005c80: 6175 643d 3131 3532 3030 293a 0a20 2020  aud=115200):.   
+00005c90: 2020 2020 2063 6f6d 506f 7274 7320 3d20       comPorts = 
+00005ca0: 7365 7269 616c 5f70 6f72 7473 2829 0a20  serial_ports(). 
+00005cb0: 2020 2020 2020 2063 6f6d 7320 3d20 5b5d         coms = []
+00005cc0: 0a20 2020 2020 2020 2066 6f72 2063 6f6d  .        for com
+00005cd0: 2069 6e20 636f 6d50 6f72 7473 3a0a 2020   in comPorts:.  
+00005ce0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00005cf0: 662e 6368 6563 6b5f 636f 6d5f 706f 7274  f.check_com_port
+00005d00: 2863 6f6d 2c20 6261 7564 293a 0a20 2020  (com, baud):.   
+00005d10: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
+00005d20: 732e 6170 7065 6e64 2863 6f6d 290a 2020  s.append(com).  
+00005d30: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00005d40: 206c 656e 2863 6f6d 7329 203e 2031 3a0a   len(coms) > 1:.
+00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d60: 2020 2020 7072 696e 7428 0a20 2020 2020      print(.     
+00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d80: 2020 2027 5761 726e 696e 6720 2d20 6d6f     'Warning - mo
+00005d90: 7265 2074 6861 6e20 6f6e 6520 6261 7263  re than one barc
+00005da0: 6f64 6520 7363 616e 6e65 7220 666f 756e  ode scanner foun
+00005db0: 642c 2075 7369 6e67 2074 6865 2066 6972  d, using the fir
+00005dc0: 7374 2062 6172 636f 6465 2073 6361 6e6e  st barcode scann
+00005dd0: 6572 2e27 290a 0a20 2020 2020 2020 2069  er.')..        i
+00005de0: 6620 6c65 6e28 636f 6d73 2920 3e20 303a  f len(coms) > 0:
+00005df0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00005e00: 7572 6e20 636f 6d73 5b30 5d0a 2020 2020  urn coms[0].    
+00005e10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00005e20: 2020 2020 2020 7072 696e 7428 2745 7272        print('Err
+00005e30: 6f72 202d 2063 6f75 6c64 206e 6f74 2066  or - could not f
+00005e40: 696e 6420 6261 7263 6f64 6520 7363 616e  ind barcode scan
+00005e50: 6e65 722e 2729 0a20 2020 2020 2020 2020  ner.').         
+00005e60: 2020 2072 6574 7572 6e20 4e6f 6e65 0a0a     return None..
+00005e70: 2020 2020 6465 6620 6368 6563 6b5f 636f      def check_co
+00005e80: 6d5f 706f 7274 2873 656c 662c 2063 6f6d  m_port(self, com
+00005e90: 3d4e 6f6e 652c 2062 6175 643d 3131 3532  =None, baud=1152
+00005ea0: 3030 293a 0a20 2020 2020 2020 2069 735f  00):.        is_
+00005eb0: 6261 725f 7363 616e 203d 2054 7275 650a  bar_scan = True.
+00005ec0: 2020 2020 2020 2020 636c 6f73 655f 706f          close_po
+00005ed0: 7274 203d 2046 616c 7365 0a20 2020 2020  rt = False.     
+00005ee0: 2020 2069 6620 6e6f 7420 7365 6c66 2e69     if not self.i
+00005ef0: 735f 6f70 656e 2829 2061 6e64 2063 6f6d  s_open() and com
+00005f00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00005f10: 2020 2020 2020 2020 2020 636c 6f73 655f            close_
+00005f20: 706f 7274 203d 2054 7275 650a 2020 2020  port = True.    
+00005f30: 2020 2020 2020 2020 7365 6c66 2e73 6572          self.ser
+00005f40: 6961 6c20 3d20 7365 7269 616c 2e53 6572  ial = serial.Ser
+00005f50: 6961 6c28 636f 6d2c 2062 6175 642c 2074  ial(com, baud, t
+00005f60: 696d 656f 7574 3d30 2e35 290a 2020 2020  imeout=0.5).    
+00005f70: 2020 2020 656c 6966 206e 6f74 2073 656c      elif not sel
+00005f80: 662e 6973 5f6f 7065 6e28 293a 0a20 2020  f.is_open():.   
+00005f90: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+00005fa0: 4261 7263 6f64 6553 6361 6e6e 6572 202d  BarcodeScanner -
+00005fb0: 2063 6865 636b 5f63 6f6d 5f70 6f72 743a   check_com_port:
+00005fc0: 204d 6973 7369 6e67 2063 6f6d 2070 6f72   Missing com por
+00005fd0: 7427 290a 2020 2020 2020 2020 2020 2020  t').            
+00005fe0: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+00005ff0: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
+00006000: 6d61 6e75 616c 5f63 6f6e 6669 6775 7265  manual_configure
+00006010: 285b 2751 5259 5044 4e27 5d29 0a20 2020  (['QRYPDN']).   
+00006020: 2020 2020 2069 6620 6e6f 7420 274e 4c53       if not 'NLS
+00006030: 2d4e 3127 2069 6e20 7374 7228 7265 7329  -N1' in str(res)
+00006040: 3a0a 2020 2020 2020 2020 2020 2020 6973  :.            is
+00006050: 5f62 6172 5f73 6361 6e20 3d20 4661 6c73  _bar_scan = Fals
+00006060: 650a 2020 2020 2020 2020 6966 2063 6c6f  e.        if clo
+00006070: 7365 5f70 6f72 743a 0a20 2020 2020 2020  se_port:.       
+00006080: 2020 2020 2073 656c 662e 7365 7269 616c       self.serial
+00006090: 2e63 6c6f 7365 2829 0a20 2020 2020 2020  .close().       
+000060a0: 2020 2020 2073 656c 662e 7365 7269 616c       self.serial
+000060b0: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+000060c0: 2072 6574 7572 6e20 6973 5f62 6172 5f73   return is_bar_s
+000060d0: 6361 6e0a 0a20 2020 2064 6566 2063 6c6f  can..    def clo
+000060e0: 7365 5f70 6f72 7428 7365 6c66 293a 0a20  se_port(self):. 
+000060f0: 2020 2020 2020 2069 6620 7365 6c66 2e73         if self.s
+00006100: 6572 6961 6c2e 6973 4f70 656e 2829 3a0a  erial.isOpen():.
+00006110: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00006120: 2e73 6572 6961 6c2e 636c 6f73 6528 290a  .serial.close().
+00006130: 0a20 2020 2064 6566 2069 735f 6f70 656e  .    def is_open
+00006140: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00006150: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00006160: 2072 6573 203d 2073 656c 662e 6d61 6e75   res = self.manu
+00006170: 616c 5f63 6f6e 6669 6775 7265 285b 2751  al_configure(['Q
+00006180: 5259 5044 4e27 5d29 0a20 2020 2020 2020  RYPDN']).       
+00006190: 2020 2020 2069 6620 274e 4c53 2d4e 3127       if 'NLS-N1'
+000061a0: 2069 6e20 7374 7228 7265 7329 3a0a 2020   in str(res):.  
+000061b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000061c0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+000061d0: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
+000061e0: 7365 0a20 2020 2020 2020 2065 7863 6570  se.        excep
+000061f0: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+00006200: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
+00006210: 2064 6566 2063 6f6e 6669 6775 7265 2873   def configure(s
+00006220: 656c 662c 2069 6c6c 5363 6e3d 2731 272c  elf, illScn='1',
+00006230: 2061 6d6c 456e 613d 2730 272c 2067 7262   amlEna='0', grb
+00006240: 456e 613d 2730 272c 2067 7262 566c 6c3d  Ena='0', grbVll=
+00006250: 2732 272c 2061 7473 456e 613d 2730 272c  '2', atsEna='0',
+00006260: 2061 7473 4475 723d 2733 3630 3030 272c   atsDur='36000',
+00006270: 2073 636e 4d6f 643d 2730 272c 0a20 2020   scnMod='0',.   
+00006280: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00006290: 7762 456e 613d 2730 2729 3a0a 2020 2020  wbEna='0'):.    
+000062a0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
+000062b0: 696c 6c53 636e 202d 2069 6c6c 756d 696e  illScn - illumin
+000062c0: 6174 696f 6e3a 2020 2020 302d 6f66 662c  ation:    0-off,
+000062d0: 2031 2d6e 6f72 6d61 6c2c 2032 2d61 6c77   1-normal, 2-alw
+000062e0: 6179 7320 6f6e 0a20 2020 2020 2020 2061  ays on.        a
+000062f0: 6d6c 456e 6120 2d20 6169 6d69 6e67 3a20  mlEna - aiming: 
+00006300: 2020 2020 2020 2020 2030 2d6f 6666 2c20           0-off, 
+00006310: 312d 6e6f 726d 616c 2c20 322d 616c 7761  1-normal, 2-alwa
+00006320: 7973 206f 6e0a 2020 2020 2020 2020 7077  ys on.        pw
+00006330: 6245 6e61 202d 2070 6f77 6572 206f 6e20  bEna - power on 
+00006340: 6265 6570 2020 2020 302d 6f66 662c 2031  beep    0-off, 1
+00006350: 2d6f 6e0a 2020 2020 2020 2020 6772 6245  -on.        grbE
+00006360: 6e61 202d 2067 6f6f 6420 7265 6164 2062  na - good read b
+00006370: 6565 7020 2020 302d 6f66 662c 2031 2d6f  eep   0-off, 1-o
+00006380: 6e0a 2020 2020 2020 2020 6174 7345 6e61  n.        atsEna
+00006390: 202d 2061 7574 6f20 736c 6565 7020 2020   - auto sleep   
+000063a0: 2020 2020 302d 6469 7361 626c 652c 2031      0-disable, 1
+000063b0: 2d65 6e61 626c 650a 2020 2020 2020 2020  -enable.        
+000063c0: 6174 7344 7572 202d 2073 6c65 6570 2064  atsDur - sleep d
+000063d0: 7572 6174 696f 6e20 2020 312d 3336 3030  uration   1-3600
+000063e0: 3020 5b73 6563 5d0a 2020 2020 2020 2020  0 [sec].        
+000063f0: 7363 6e4d 6f64 202d 2073 6361 6e20 6d6f  scnMod - scan mo
+00006400: 6465 2020 2020 2020 2020 302d 6c65 7665  de        0-leve
+00006410: 6c20 6d6f 6465 2c20 322d 7365 6e73 6520  l mode, 2-sense 
+00006420: 6d6f 6465 2c20 332d 636f 6e74 696e 756f  mode, 3-continuo
+00006430: 7573 206d 6f64 652c 2037 2d62 6174 6368  us mode, 7-batch
+00006440: 206d 6f64 650a 2020 2020 2020 2020 2727   mode.        ''
+00006450: 270a 2020 2020 2020 2020 736c 6565 7028  '.        sleep(
+00006460: 302e 3129 0a20 2020 2020 2020 2070 6172  0.1).        par
+00006470: 616d 7320 3d20 7b27 494c 4c53 434e 273a  ams = {'ILLSCN':
+00006480: 2069 6c6c 5363 6e2c 2027 414d 4c45 4e41   illScn, 'AMLENA
+00006490: 273a 2061 6d6c 456e 612c 2027 4752 4245  ': amlEna, 'GRBE
+000064a0: 4e41 273a 2067 7262 456e 612c 2027 4154  NA': grbEna, 'AT
+000064b0: 5345 4e41 273a 2061 7473 456e 612c 0a20  SENA': atsEna,. 
+000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064d0: 2027 4752 4256 4c4c 273a 2067 7262 566c   'GRBVLL': grbVl
+000064e0: 6c2c 2027 4154 5344 5552 273a 2061 7473  l, 'ATSDUR': ats
+000064f0: 4475 722c 2027 5343 4e4d 4f44 273a 2073  Dur, 'SCNMOD': s
+00006500: 636e 4d6f 642c 2027 5057 4245 4e41 273a  cnMod, 'PWBENA':
+00006510: 2070 7762 456e 617d 0a20 2020 2020 2020   pwbEna}.       
+00006520: 2070 6172 616d 7320 3d20 5b6b 6579 202b   params = [key +
+00006530: 2076 616c 7565 2066 6f72 206b 6579 2c20   value for key, 
+00006540: 7661 6c75 6520 696e 2070 6172 616d 732e  value in params.
+00006550: 6974 656d 7328 295d 0a20 2020 2020 2020  items()].       
+00006560: 2074 2c20 6973 5375 6363 6573 7320 3d20   t, isSuccess = 
+00006570: 7365 6c66 2e6d 616e 7561 6c5f 636f 6e66  self.manual_conf
+00006580: 6967 7572 6528 7061 7261 6d73 290a 2020  igure(params).  
+00006590: 2020 2020 2020 6966 2069 7353 7563 6365        if isSucce
+000065a0: 7373 2061 6e64 2073 656c 662e 6c6f 675f  ss and self.log_
+000065b0: 7479 7065 2021 3d20 274e 4f5f 4c4f 4727  type != 'NO_LOG'
+000065c0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+000065d0: 696e 7428 6627 4261 7263 6f64 6520 7363  int(f'Barcode sc
+000065e0: 616e 6e65 7220 287b 7365 6c66 2e63 6f6d  anner ({self.com
+000065f0: 7d29 2063 6f6e 6669 6775 7265 6420 7375  }) configured su
+00006600: 6363 6573 7366 756c 6c79 2e27 290a 2020  ccessfully.').  
+00006610: 2020 2020 2020 656c 6966 206e 6f74 2069        elif not i
+00006620: 7353 7563 6365 7373 3a0a 2020 2020 2020  sSuccess:.      
+00006630: 2020 2020 2020 7072 696e 7428 6627 4261        print(f'Ba
+00006640: 7263 6f64 6520 7363 616e 6e65 7220 287b  rcode scanner ({
+00006650: 7365 6c66 2e63 6f6d 7d29 2063 6f6e 6669  self.com}) confi
+00006660: 6775 7261 7469 6f6e 2066 6169 6c65 642e  guration failed.
+00006670: 2729 0a0a 2020 2020 6465 6620 7265 7374  ')..    def rest
+00006680: 6f72 655f 616c 6c5f 6661 6374 6f72 795f  ore_all_factory_
+00006690: 6465 6661 756c 7473 2873 656c 6629 3a0a  defaults(self):.
+000066a0: 2020 2020 2020 2020 736c 6565 7028 302e          sleep(0.
+000066b0: 3129 0a20 2020 2020 2020 2070 6172 616d  1).        param
+000066c0: 7320 3d20 7b27 4641 4344 4546 273a 2027  s = {'FACDEF': '
+000066d0: 277d 0a20 2020 2020 2020 2070 6172 616d  '}.        param
+000066e0: 7320 3d20 5b6b 6579 202b 2076 616c 7565  s = [key + value
+000066f0: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
+00006700: 696e 2070 6172 616d 732e 6974 656d 7328  in params.items(
+00006710: 295d 0a20 2020 2020 2020 2074 2c20 6973  )].        t, is
+00006720: 5375 6363 6573 7320 3d20 7365 6c66 2e6d  Success = self.m
+00006730: 616e 7561 6c5f 636f 6e66 6967 7572 6528  anual_configure(
+00006740: 7061 7261 6d73 290a 2020 2020 2020 2020  params).        
+00006750: 6966 2069 7353 7563 6365 7373 2061 6e64  if isSuccess and
+00006760: 2073 656c 662e 6c6f 675f 7479 7065 2021   self.log_type !
+00006770: 3d20 274e 4f5f 4c4f 4727 3a0a 2020 2020  = 'NO_LOG':.    
+00006780: 2020 2020 2020 2020 7072 696e 7428 6627          print(f'
+00006790: 4261 7263 6f64 6520 7363 616e 6e65 7220  Barcode scanner 
+000067a0: 287b 7365 6c66 2e63 6f6d 7d29 2072 6573  ({self.com}) res
+000067b0: 746f 7265 6420 6661 6374 6f72 7920 6465  tored factory de
+000067c0: 6661 756c 7420 7375 6363 6573 7366 756c  fault successful
+000067d0: 6c79 2e27 290a 2020 2020 2020 2020 656c  ly.').        el
+000067e0: 6966 206e 6f74 2069 7353 7563 6365 7373  if not isSuccess
+000067f0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00006800: 696e 7428 6627 4261 7263 6f64 6520 7363  int(f'Barcode sc
+00006810: 616e 6e65 7220 287b 7365 6c66 2e63 6f6d  anner ({self.com
+00006820: 7d29 2072 6573 746f 7265 6420 6661 6374  }) restored fact
+00006830: 6f72 7920 6465 6661 756c 7420 6661 696c  ory default fail
+00006840: 6564 2e27 290a 0a20 2020 2064 6566 206d  ed.')..    def m
+00006850: 616e 7561 6c5f 636f 6e66 6967 7572 6528  anual_configure(
+00006860: 7365 6c66 2c20 7061 7261 6d73 293a 0a20  self, params):. 
+00006870: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
+00006880: 290a 2020 2020 2020 2020 636f 6e66 6967  ).        config
+00006890: 7320 3d20 7365 6c66 2e70 7265 6669 7820  s = self.prefix 
+000068a0: 2b20 273b 272e 6a6f 696e 2870 6172 616d  + ';'.join(param
+000068b0: 7329 202b 2073 656c 662e 7375 6666 6978  s) + self.suffix
+000068c0: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+000068d0: 7269 616c 2e66 6c75 7368 496e 7075 7428  rial.flushInput(
+000068e0: 290a 2020 2020 2020 2020 7365 6c66 2e73  ).        self.s
+000068f0: 6572 6961 6c2e 666c 7573 684f 7574 7075  erial.flushOutpu
+00006900: 7428 290a 2020 2020 2020 2020 7365 6c66  t().        self
+00006910: 2e73 6572 6961 6c2e 7772 6974 6528 7374  .serial.write(st
+00006920: 722e 656e 636f 6465 2863 6f6e 6669 6773  r.encode(configs
+00006930: 2929 0a20 2020 2020 2020 2073 6c65 6570  )).        sleep
+00006940: 2830 2e31 290a 2020 2020 2020 2020 742c  (0.1).        t,
+00006950: 2069 7353 7563 6365 7373 203d 2073 656c   isSuccess = sel
+00006960: 662e 7472 6967 6765 725f 7374 6f70 5f73  f.trigger_stop_s
+00006970: 6574 7469 6e67 7328 290a 2020 2020 2020  ettings().      
+00006980: 2020 2320 7072 696e 7428 7429 0a20 2020    # print(t).   
+00006990: 2020 2020 2072 6574 7572 6e20 742c 2069       return t, i
+000069a0: 7353 7563 6365 7373 0a0a 2020 2020 6465  sSuccess..    de
+000069b0: 6620 7363 616e 2873 656c 6629 3a0a 2020  f scan(self):.  
+000069c0: 2020 2020 2020 2320 7072 696e 7428 2261        # print("a
+000069d0: 6e61 6c6f 675f 7472 6967 6765 725f 7365  nalog_trigger_se
+000069e0: 7474 696e 6722 290a 2020 2020 2020 2020  tting").        
+000069f0: 7365 6c66 2e73 6572 6961 6c2e 7772 6974  self.serial.writ
+00006a00: 6528 6222 5c78 3162 5c78 3331 2229 0a20  e(b"\x1b\x31"). 
+00006a10: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
+00006a20: 290a 2020 2020 2020 2020 2320 7420 3d20  ).        # t = 
+00006a30: 7365 722e 7265 6164 2873 6572 2e69 6e5f  ser.read(ser.in_
+00006a40: 7761 6974 696e 6729 0a20 2020 2020 2020  waiting).       
+00006a50: 2074 203d 2073 656c 662e 7365 7269 616c   t = self.serial
+00006a60: 2e72 6561 645f 616c 6c28 290a 2020 2020  .read_all().    
+00006a70: 2020 2020 2320 7072 696e 7428 7429 0a20      # print(t). 
+00006a80: 2020 2020 2020 2072 6574 7572 6e20 740a         return t.
+00006a90: 0a20 2020 2064 6566 2073 6361 6e5f 616e  .    def scan_an
+00006aa0: 645f 666c 7573 6828 7365 6c66 293a 0a20  d_flush(self):. 
+00006ab0: 2020 2020 2020 2073 656c 662e 7365 7269         self.seri
+00006ac0: 616c 2e66 6c75 7368 496e 7075 7428 290a  al.flushInput().
+00006ad0: 2020 2020 2020 2020 7365 6c66 2e73 6572          self.ser
+00006ae0: 6961 6c2e 666c 7573 684f 7574 7075 7428  ial.flushOutput(
+00006af0: 290a 2020 2020 2020 2020 7420 3d20 7365  ).        t = se
+00006b00: 6c66 2e73 6361 6e28 290a 2020 2020 2020  lf.scan().      
+00006b10: 2020 7365 6c66 2e73 6572 6961 6c2e 666c    self.serial.fl
+00006b20: 7573 6849 6e70 7574 2829 0a20 2020 2020  ushInput().     
+00006b30: 2020 2073 656c 662e 7365 7269 616c 2e66     self.serial.f
+00006b40: 6c75 7368 4f75 7470 7574 2829 0a20 2020  lushOutput().   
+00006b50: 2020 2020 2074 436c 6561 6e20 3d20 7374       tClean = st
+00006b60: 7228 7429 2e73 706c 6974 2827 5c5c 7827  r(t).split('\\x'
+00006b70: 295b 2d31 5d0a 2020 2020 2020 2020 6966  )[-1].        if
+00006b80: 2074 436c 6561 6e2e 7374 6172 7473 7769   tClean.startswi
+00006b90: 7468 2827 3036 2729 3a0a 2020 2020 2020  th('06'):.      
+00006ba0: 2020 2020 2020 7443 6c65 616e 203d 2074        tClean = t
+00006bb0: 436c 6561 6e5b 323a 5d0a 2020 2020 2020  Clean[2:].      
+00006bc0: 2020 2020 2020 7443 6c65 616e 203d 2074        tClean = t
+00006bd0: 436c 6561 6e2e 7374 7269 7028 2227 5c5c  Clean.strip("'\\
+00006be0: 6e5c 5c72 2229 0a20 2020 2020 2020 2020  n\\r").         
+00006bf0: 2020 2074 436c 6561 6e20 3d20 7443 6c65     tClean = tCle
+00006c00: 616e 2e73 706c 6974 2827 5c5c 6e27 295b  an.split('\\n')[
+00006c10: 2d31 5d0a 2020 2020 2020 2020 2020 2020  -1].            
+00006c20: 7443 6c65 616e 203d 2074 436c 6561 6e2e  tClean = tClean.
+00006c30: 7370 6c69 7428 275c 5c72 2729 5b2d 315d  split('\\r')[-1]
+00006c40: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00006c50: 7572 6e20 7443 6c65 616e 0a20 2020 2020  urn tClean.     
+00006c60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00006c70: 2020 2020 2070 7269 6e74 2827 5761 726e       print('Warn
+00006c80: 696e 6720 2d20 6e6f 7420 7265 6365 6976  ing - not receiv
+00006c90: 6564 2041 434b 2066 726f 6d20 6261 7263  ed ACK from barc
+00006ca0: 6f64 6520 7363 616e 6e65 722e 2729 0a20  ode scanner.'). 
+00006cb0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006cc0: 6e20 7374 7228 7429 2e73 706c 6974 2827  n str(t).split('
+00006cd0: 5c5c 7827 295b 2d31 5d0a 0a20 2020 2064  \\x')[-1]..    d
+00006ce0: 6566 2073 6361 6e5f 6578 745f 6964 2873  ef scan_ext_id(s
+00006cf0: 656c 662c 2073 6361 6e44 7572 3d30 2e35  elf, scanDur=0.5
+00006d00: 2c20 5661 6c69 6461 7465 436e 743d 3329  , ValidateCnt=3)
+00006d10: 3a0a 2020 2020 2020 2020 6261 7263 6f64  :.        barcod
+00006d20: 6552 6561 6420 3d20 2727 0a20 2020 2020  eRead = ''.     
+00006d30: 2020 2062 6172 636f 6465 7320 3d20 5b5d     barcodes = []
+00006d40: 0a20 2020 2020 2020 2073 7461 7274 5469  .        startTi
+00006d50: 6d65 203d 2074 696d 6528 290a 2020 2020  me = time().    
+00006d60: 2020 2020 7768 696c 6520 2828 7469 6d65      while ((time
+00006d70: 2829 202d 2073 7461 7274 5469 6d65 2920  () - startTime) 
+00006d80: 3c20 7363 616e 4475 7229 3a0a 2020 2020  < scanDur):.    
+00006d90: 2020 2020 2020 2020 6261 7263 6f64 6552          barcodeR
+00006da0: 6561 6420 3d20 7365 6c66 2e73 6361 6e5f  ead = self.scan_
+00006db0: 616e 645f 666c 7573 6828 290a 2020 2020  and_flush().    
+00006dc0: 2020 2020 2020 2020 2320 6261 7263 6f64          # barcod
+00006dd0: 6552 6561 6420 3d20 7374 7228 7429 0a20  eRead = str(t). 
+00006de0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00006df0: 6e28 6261 7263 6f64 6552 6561 6429 203c  n(barcodeRead) <
+00006e00: 2038 3a0a 2020 2020 2020 2020 2020 2020   8:.            
+00006e10: 2020 2020 6261 7263 6f64 6552 6561 6420      barcodeRead 
+00006e20: 3d20 2727 0a20 2020 2020 2020 2020 2020  = ''.           
+00006e30: 2020 2020 2063 6f6e 7469 6e75 650a 0a20       continue.. 
+00006e40: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+00006e50: 6e28 6261 7263 6f64 6573 2920 3c20 5661  n(barcodes) < Va
+00006e60: 6c69 6461 7465 436e 743a 0a20 2020 2020  lidateCnt:.     
+00006e70: 2020 2020 2020 2020 2020 2062 6172 636f             barco
+00006e80: 6465 732e 6170 7065 6e64 2862 6172 636f  des.append(barco
+00006e90: 6465 5265 6164 290a 2020 2020 2020 2020  deRead).        
+00006ea0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00006eb0: 0a0a 2020 2020 2020 2020 2020 2020 6261  ..            ba
+00006ec0: 7263 6f64 6552 6561 6420 3d20 6d6f 6465  rcodeRead = mode
+00006ed0: 2862 6172 636f 6465 7329 0a20 2020 2020  (barcodes).     
+00006ee0: 2020 2020 2020 2066 756c 6c44 6174 6120         fullData 
+00006ef0: 3d20 6375 7249 6420 3d20 7265 656c 4964  = curId = reelId
+00006f00: 203d 2067 7469 6e20 3d20 6261 7263 6f64   = gtin = barcod
+00006f10: 6552 6561 640a 2020 2020 2020 2020 2020  eRead.          
+00006f20: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00006f30: 2020 2020 2020 2069 6620 2729 2720 696e         if ')' in
+00006f40: 2066 756c 6c44 6174 613a 0a20 2020 2020   fullData:.     
+00006f50: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00006f60: 7469 6e20 3d20 2729 272e 6a6f 696e 2866  tin = ')'.join(f
+00006f70: 756c 6c44 6174 612e 7370 6c69 7428 2729  ullData.split(')
+00006f80: 2729 5b3a 325d 2920 2b20 2729 270a 2020  ')[:2]) + ')'.  
+00006f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fa0: 2020 7461 6744 6174 6120 3d20 6675 6c6c    tagData = full
+00006fb0: 4461 7461 2e73 706c 6974 2827 2927 295b  Data.split(')')[
+00006fc0: 325d 0a20 2020 2020 2020 2020 2020 2020  2].             
+00006fd0: 2020 2065 6c73 653a 2020 2320 6774 696e     else:  # gtin
+00006fe0: 2077 6974 686f 7574 2070 6172 656e 7468   without parenth
+00006ff0: 6573 6973 0a20 2020 2020 2020 2020 2020  esis.           
+00007000: 2020 2020 2020 2020 2067 7469 6e20 3d20           gtin = 
+00007010: 6675 6c6c 4461 7461 5b30 3a31 385d 0a20  fullData[0:18]. 
+00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007030: 2020 2074 6167 4461 7461 203d 2066 756c     tagData = ful
+00007040: 6c44 6174 615b 3138 3a5d 0a20 2020 2020  lData[18:].     
+00007050: 2020 2020 2020 2020 2020 2063 7572 4964             curId
+00007060: 203d 2074 6167 4461 7461 2e73 706c 6974   = tagData.split
+00007070: 2827 5427 295b 315d 2e73 7472 6970 2822  ('T')[1].strip("
+00007080: 2720 2229 2e73 706c 6974 2827 2827 295b  ' ").split('(')[
+00007090: 305d 0a20 2020 2020 2020 2020 2020 2020  0].             
+000070a0: 2020 2072 6565 6c49 6420 3d20 7461 6744     reelId = tagD
+000070b0: 6174 612e 7370 6c69 7428 2754 2729 5b30  ata.split('T')[0
+000070c0: 5d2e 7374 7269 7028 2227 2022 290a 2020  ].strip("' ").  
+000070d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000070e0: 7475 726e 2066 756c 6c44 6174 612c 2063  turn fullData, c
+000070f0: 7572 4964 2c20 7265 656c 4964 2c20 6774  urId, reelId, gt
+00007100: 696e 0a20 2020 2020 2020 2020 2020 2065  in.            e
+00007110: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+00007120: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00007130: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00007140: 6675 6c6c 4461 7461 2c20 6375 7249 642c  fullData, curId,
+00007150: 2072 6565 6c49 642c 2067 7469 6e0a 0a20   reelId, gtin.. 
+00007160: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00007170: 6e65 2c20 4e6f 6e65 2c20 4e6f 6e65 2c20  ne, None, None, 
+00007180: 4e6f 6e65 0a0a 2020 2020 6465 6620 6175  None..    def au
+00007190: 746f 5f73 6361 6e28 7365 6c66 293a 0a20  to_scan(self):. 
+000071a0: 2020 2020 2020 2023 2070 7269 6e74 2822         # print("
+000071b0: 4175 746f 6d61 7469 6320 7265 6164 696e  Automatic readin
+000071c0: 6720 7365 7474 696e 6773 2229 0a20 2020  g settings").   
+000071d0: 2020 2020 2073 656c 662e 7365 7269 616c       self.serial
+000071e0: 2e77 7269 7465 2862 225c 7831 625c 7833  .write(b"\x1b\x3
+000071f0: 3222 290a 2020 2020 2020 2020 736c 6565  2").        slee
+00007200: 7028 302e 3129 0a20 2020 2020 2020 2074  p(0.1).        t
+00007210: 203d 2073 656c 662e 7365 7269 616c 2e72   = self.serial.r
+00007220: 6561 645f 616c 6c28 290a 2020 2020 2020  ead_all().      
+00007230: 2020 2320 7072 696e 7428 7429 0a20 2020    # print(t).   
+00007240: 2020 2020 2072 6574 7572 6e20 740a 0a20       return t.. 
+00007250: 2020 2064 6566 2074 7269 6767 6572 5f73     def trigger_s
+00007260: 746f 705f 7365 7474 696e 6773 2873 656c  top_settings(sel
+00007270: 6629 3a0a 2020 2020 2020 2020 2320 7072  f):.        # pr
+00007280: 696e 7428 2254 7269 6767 6572 5f73 746f  int("Trigger_sto
+00007290: 705f 7365 7474 696e 6773 2229 0a20 2020  p_settings").   
+000072a0: 2020 2020 2023 2073 6c65 6570 2830 2e31       # sleep(0.1
+000072b0: 290a 2020 2020 2020 2020 2320 7420 3d20  ).        # t = 
+000072c0: 7365 722e 7265 6164 2873 6572 2e69 6e5f  ser.read(ser.in_
+000072d0: 7761 6974 696e 6729 0a20 2020 2020 2020  waiting).       
+000072e0: 2073 6c65 6570 2830 2e31 290a 2020 2020   sleep(0.1).    
+000072f0: 2020 2020 7420 3d20 7365 6c66 2e73 6572      t = self.ser
+00007300: 6961 6c2e 7265 6164 5f61 6c6c 2829 0a20  ial.read_all(). 
+00007310: 2020 2020 2020 2073 6c65 6570 2830 2e31         sleep(0.1
+00007320: 290a 2020 2020 2020 2020 2320 7072 696e  ).        # prin
+00007330: 7428 7429 0a20 2020 2020 2020 2061 636b  t(t).        ack
+00007340: 7320 3d20 7374 7228 7429 2e73 706c 6974  s = str(t).split
+00007350: 2827 3b27 295b 3a2d 315d 0a20 2020 2020  (';')[:-1].     
+00007360: 2020 2069 7353 7563 6365 7373 203d 2061     isSuccess = a
+00007370: 6c6c 285b 5472 7565 2069 6620 6163 6b2e  ll([True if ack.
+00007380: 656e 6473 7769 7468 2827 5c5c 7830 3627  endswith('\\x06'
+00007390: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000073a0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
+000073b0: 4661 6c73 6520 666f 7220 6163 6b20 696e  False for ack in
+000073c0: 2061 636b 735d 290a 2020 2020 2020 2020   acks]).        
+000073d0: 7265 7475 726e 2074 2c20 6973 5375 6363  return t, isSucc
+000073e0: 6573 730a 0a0a 636c 6173 7320 596f 6374  ess...class Yoct
+000073f0: 6f54 656d 7065 7261 7475 7265 5365 6e73  oTemperatureSens
+00007400: 6f72 286f 626a 6563 7429 3a0a 2020 2020  or(object):.    
+00007410: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
+00007420: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
+00007430: 2e73 656e 736f 7220 3d20 4e6f 6e65 0a20  .sensor = None. 
+00007440: 2020 2020 2020 2065 7272 6d73 6720 3d20         errmsg = 
+00007450: 5952 6566 5061 7261 6d28 290a 2020 2020  YRefParam().    
+00007460: 2020 2020 2320 5365 7475 7020 7468 6520      # Setup the 
+00007470: 4150 4920 746f 2075 7365 206c 6f63 616c  API to use local
+00007480: 2055 5342 2064 6576 6963 6573 0a20 2020   USB devices.   
+00007490: 2020 2020 2069 6620 5941 5049 2e52 6567       if YAPI.Reg
+000074a0: 6973 7465 7248 7562 2822 7573 6222 2c20  isterHub("usb", 
+000074b0: 6572 726d 7367 2920 213d 2059 4150 492e  errmsg) != YAPI.
+000074c0: 5355 4343 4553 533a 0a20 2020 2020 2020  SUCCESS:.       
+000074d0: 2020 2020 2072 6169 7365 2045 7175 6970       raise Equip
+000074e0: 6d65 6e74 4572 726f 7228 2779 6f63 746f  mentError('yocto
+000074f0: 2074 656d 7065 7261 7475 7265 2073 656e   temperature sen
+00007500: 736f 7220 676f 7420 696e 6974 2065 7272  sor got init err
+00007510: 6f72 3a20 7b7d 272e 666f 726d 6174 2865  or: {}'.format(e
+00007520: 7272 6d73 672e 7661 6c75 6529 290a 0a20  rrmsg.value)).. 
+00007530: 2020 2064 6566 2063 6f6e 6e65 6374 2873     def connect(s
+00007540: 656c 662c 2074 6172 6765 743d 2761 6e79  elf, target='any
+00007550: 2729 3a0a 2020 2020 2020 2020 6966 2074  '):.        if t
+00007560: 6172 6765 7420 3d3d 2027 616e 7927 3a0a  arget == 'any':.
+00007570: 2020 2020 2020 2020 2020 2020 2320 7265              # re
+00007580: 7472 6965 7665 2061 6e79 2074 656d 7065  trieve any tempe
+00007590: 7261 7475 7265 2073 656e 736f 720a 2020  rature sensor.  
+000075a0: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
+000075b0: 656e 736f 7220 3d20 5954 656d 7065 7261  ensor = YTempera
+000075c0: 7475 7265 2e46 6972 7374 5465 6d70 6572  ture.FirstTemper
+000075d0: 6174 7572 6528 290a 2020 2020 2020 2020  ature().        
+000075e0: 656c 6966 2074 6172 6765 7420 3d3d 2027  elif target == '
+000075f0: 273a 0a20 2020 2020 2020 2020 2020 2070  ':.            p
+00007600: 7269 6e74 2827 7370 6563 6966 6965 6420  rint('specified 
+00007610: 696e 7661 6c69 6420 7461 7267 6574 2729  invalid target')
+00007620: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00007630: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+00007640: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00007650: 2020 2020 7365 6c66 2e73 656e 736f 7220      self.sensor 
+00007660: 3d20 5954 656d 7065 7261 7475 7265 2e46  = YTemperature.F
+00007670: 696e 6454 656d 7065 7261 7475 7265 2874  indTemperature(t
+00007680: 6172 6765 7420 2b20 272e 7465 6d70 6572  arget + '.temper
+00007690: 6174 7572 6527 290a 2020 2020 2020 2020  ature').        
+000076a0: 6966 2073 656c 662e 7365 6e73 6f72 2069  if self.sensor i
+000076b0: 7320 4e6f 6e65 206f 7220 7365 6c66 2e67  s None or self.g
+000076c0: 6574 5f73 656e 736f 725f 6e61 6d65 2829  et_sensor_name()
+000076d0: 203d 3d20 2775 6e72 6573 6f6c 7665 6427   == 'unresolved'
+000076e0: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+000076f0: 696e 7428 274e 6f20 6d6f 6475 6c65 2063  int('No module c
+00007700: 6f6e 6e65 6374 6564 2729 0a20 2020 2020  onnected').     
+00007710: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00007720: 6c73 650a 2020 2020 2020 2020 656c 7365  lse.        else
+00007730: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00007740: 7475 726e 2054 7275 650a 0a20 2020 2064  turn True..    d
+00007750: 6566 2067 6574 5f73 656e 736f 725f 6e61  ef get_sensor_na
+00007760: 6d65 2873 656c 6629 3a0a 2020 2020 2020  me(self):.      
+00007770: 2020 6966 2073 656c 662e 7365 6e73 6f72    if self.sensor
+00007780: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00007790: 2020 2020 2020 7072 696e 7428 276e 6f20        print('no 
+000077a0: 7365 6e73 6f72 2069 7320 636f 6e6e 6563  sensor is connec
+000077b0: 7465 642e 2074 7279 2074 6f20 6361 6c6c  ted. try to call
+000077c0: 2063 6f6e 6e65 6374 2829 2066 6972 7374   connect() first
+000077d0: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
+000077e0: 6574 7572 6e20 2727 0a0a 2020 2020 2020  eturn ''..      
+000077f0: 2020 7365 6e73 6f72 5f73 7472 203d 2073    sensor_str = s
+00007800: 656c 662e 7365 6e73 6f72 2e64 6573 6372  elf.sensor.descr
+00007810: 6962 6528 290a 2020 2020 2020 2020 6e61  ibe().        na
+00007820: 6d65 5f73 7472 203d 2073 656e 736f 725f  me_str = sensor_
+00007830: 7374 722e 7370 6c69 7428 273d 2729 5b31  str.split('=')[1
+00007840: 5d2e 7370 6c69 7428 272e 2729 5b30 5d0a  ].split('.')[0].
+00007850: 2020 2020 2020 2020 7265 7475 726e 206e          return n
+00007860: 616d 655f 7374 720a 0a20 2020 2064 6566  ame_str..    def
+00007870: 2067 6574 5f74 656d 7065 7261 7475 7265   get_temperature
+00007880: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00007890: 6966 2073 656c 662e 7365 6e73 6f72 2069  if self.sensor i
+000078a0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+000078b0: 2020 2020 7072 696e 7428 2773 656e 736f      print('senso
+000078c0: 7220 6973 206e 6f74 2063 6f6e 6e65 6374  r is not connect
+000078d0: 6564 2e20 7472 7920 746f 2063 616c 6c20  ed. try to call 
+000078e0: 636f 6e6e 6563 7428 2920 6669 7273 7427  connect() first'
+000078f0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00007900: 7475 726e 2066 6c6f 6174 2827 6e61 6e27  turn float('nan'
+00007910: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00007920: 2028 7365 6c66 2e73 656e 736f 722e 6973   (self.sensor.is
+00007930: 4f6e 6c69 6e65 2829 293a 0a20 2020 2020  Online()):.     
+00007940: 2020 2020 2020 2070 7269 6e74 2827 7365         print('se
+00007950: 6e73 6f72 2069 7320 6e6f 7420 636f 6e6e  nsor is not conn
+00007960: 6563 7465 6420 6f72 2064 6973 636f 6e6e  ected or disconn
+00007970: 6563 7465 6420 6475 7269 6e67 2072 756e  ected during run
+00007980: 2729 0a20 2020 2020 2020 2020 2020 2072  ').            r
+00007990: 6574 7572 6e20 666c 6f61 7428 276e 616e  eturn float('nan
+000079a0: 2729 0a0a 2020 2020 2020 2020 7265 7475  ')..        retu
+000079b0: 726e 2073 656c 662e 7365 6e73 6f72 2e67  rn self.sensor.g
+000079c0: 6574 5f63 7572 7265 6e74 5661 6c75 6528  et_currentValue(
+000079d0: 290a 0a20 2020 2040 7374 6174 6963 6d65  )..    @staticme
+000079e0: 7468 6f64 0a20 2020 2064 6566 2065 7869  thod.    def exi
+000079f0: 745f 6170 7028 293a 0a20 2020 2020 2020  t_app():.       
+00007a00: 2059 4150 492e 4672 6565 4150 4928 290a   YAPI.FreeAPI().
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/tester_utils.py` & `wiliot-testers-4.0.6/wiliot_testers/tester_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -140,26 +140,15 @@
                 s.close()
         except (OSError, serial.SerialException):
             pass
         except Exception as e:
             raise (e)
     return device_ports
 
-def dict_to_csv(dict_in, path, append=False, only_titles=False):
-    if append:
-        method = 'a'
-    else:
-        method = 'w'
-    with open(path, method, newline='') as f:
-        dict_writer = DictWriter(f, fieldnames=dict_in.keys())
-        if not append:
-            dict_writer.writeheader()
-        if not only_titles:
-            dict_writer.writerow(dict_in)
-        f.close()
+
 def set_temperature():
     """
     initialize yocto temperature sensor
     :return: current temperature
     """
     # object tenp sens
     errmsg = YRefParam()
@@ -754,14 +743,205 @@
     window2.close()
 
 
 ###########################################
 #              Cloud Functions            #
 ###########################################
 
+def upload_to_cloud_api(batch_name, tester_type, run_data_csv_name=None, tags_data_csv_name=None, to_logging=False,
+                        env='', is_batch_name_inside_logs_folder=True, logger_=None, is_path=False,
+                        client=None, packets_instead_tags=False, owner_id='wiliot-ops'):
+    """
+    uploads a tester log to Wiliot cloud
+    :type batch_name: string
+    :param batch_name: folder name of the relevant log
+    :type run_data_csv_name: string
+    :param run_data_csv_name: name of desired run_data log to upload,
+                              should contain 'run_data' and end with .csv
+    :type tags_data_csv_name: string
+    :param tags_data_csv_name: name of desired tags_data log to upload,
+                               should contain 'tags_data' and end with .csv
+    :type tester_type: string
+    :param tester_type: name of the tester the run was made on (offline, tal15k, conversion, yield)
+    :type to_logging: bool
+    :param to_logging: if true, write to logging.debug the result of the upload
+    :type env: string (prod, dev, test)
+    :param env: to what cloud environment should we upload the files
+    :type is_batch_name_inside_logs_folder: bool
+    :param is_batch_name_inside_logs_folder: flag to indicate if the batch_name is the regular run folder (logs) or
+                                             this function is being used in a way we will need the full path
+    :return: True for successful upload, False otherwise
+    """
+    if logger_ is None:
+        logger = logging.getLogger()
+    else:
+        logger = logging.getLogger(logger_)
+    tester_type_name = tester_type.split('-')[0]
+    if tester_type_name not in ['offline', 'tal15k', 'conversion', 'yield', 'sample']:
+        logger.warning('Unsupported tester_type inserted to upload_to_cloud_api()\nPlease change it and retry')
+        return
+    if run_data_csv_name is not None and 'run_data' not in run_data_csv_name:
+        logger.warning('Unsupported run_data_csv_name inserted to upload_to_cloud_api()\nPlease change it and retry')
+        return
+    if tags_data_csv_name is not None and 'packets_data' not in tags_data_csv_name and \
+            'tags_data' not in tags_data_csv_name:
+        logger.warning('Unsupported tags_data_csv_name inserted to upload_to_cloud_api()\nPlease change it and retry')
+        return
+
+    file_path, api_key, is_successful = check_user_config_is_ok(env=env, owner_id=owner_id)
+    if env == 'prod':
+        env = ''
+    if not is_successful:
+        logger.warning('could not extract user credentials. please check warnings')
+        return
+    if client is None:
+        client = ManufacturingClient(api_key=api_key, env=env, logger_=logger.name)
+    else:
+        client = client
+    
+    logger.info('Upload to cloud has began\nWaiting for the server response, please wait...')
+    conn = http.client.HTTPSConnection("api.wiliot.com")
+    boundary = 'wL36Yn8afVp8Ag7AmP8qZ0SA4n1v9T'
+    headers = {
+        'Authorization': 'Bearer ' + client.auth_obj.get_token(),
+        'Content-type': 'multipart/form-data; boundary={}'.format(boundary)
+    }
+    
+    if env == 'prod' or env == '':
+        url = "/v1/manufacturing/upload/testerslogs/"
+    elif env == 'test' or env == '/test':
+        url = "/test/v1/manufacturing/upload/testerslogs/"
+    elif env == 'dev':
+        url = "/dev/v1/manufacturing/upload/testerslogs/"
+    else:
+        print('unsupported env value was inserted (env = ' + str(env) + ')')
+        return False
+    
+    url += tester_type
+    
+    if run_data_csv_name is not None:
+        # run_url = url + '-tester-runs-indicators'
+        run_url = url + '/runs-indicators'
+        logger.info("Run data csv upload to {} started".format(run_url))
+        data_list = [encode('--' + boundary)]
+        if is_batch_name_inside_logs_folder:
+            run_data_path = 'logs/' + batch_name
+        else:
+            run_data_path = batch_name
+        run_data_path = os.path.join(run_data_path, run_data_csv_name)
+        
+        if not os.path.exists(run_data_path):
+            exception_string = str(run_data_path) + ' run_data_path could not be found \n' + \
+                               'please find it and try to upload again'
+            raise Exception(exception_string)
+        if is_path:
+            run_data_path = run_data_csv_name
+        data_list.append(encode('Content-Disposition: form-data; name=file; filename={0}'.format(run_data_path)))
+        file_type = mimetypes.guess_type(run_data_path)[0] or 'application/octet-stream'
+        data_list.append(encode('Content-Type: {}'.format(file_type)))
+        data_list.append(encode(''))
+        with open(run_data_path, 'rb') as f:
+            data_list.append(f.read())
+        data_list.append(encode('--' + boundary + '--'))
+        data_list.append(encode(''))
+        body = b'\r\n'.join(data_list)
+        payload = body
+        
+        conn.request("POST", run_url, payload, headers)
+        run_data_res = conn.getresponse()
+        run_data_data = run_data_res.read()
+        logger.info("answer from cloud is:")
+        run_data_data_decoded = run_data_data.decode('utf-8')
+        run_data_data_decoded_convert = ast.literal_eval(run_data_data_decoded)
+        try:
+            logger.info(run_data_data_decoded_convert['data'])
+        
+        except Exception:
+            logger.warning('Problem with cloud upload')
+            logger.warning(run_data_data_decoded_convert['error'])
+        
+        if str(run_data_res.status) == '500':
+            logger.info(
+                'There was a problem at the Server side (status 500), please try to upload again or reach Wiliot')
+            return False
+        elif str(run_data_res.status) in ['401', '400']:
+            client.auth_obj.get_token()
+            return False
+        elif str(run_data_res.status)[0:2] == '40':
+            logger.info('There was a problem with the request (status 40*), please try to upload again or reach Wiliot')
+            logger.info('Status code is: ' + str(run_data_res.status))
+            if run_data_data_decoded_convert['error'] != 'This CSV file already uploaded':
+                return False
+        elif str(run_data_res.status) == '200':
+            logger.info('The file "' + run_data_csv_name + '" was uploaded successfully to Wiliot cloud')
+    
+    if tags_data_csv_name is not None:
+        # tags_url = url + '-tester-tags-indicators'
+        if packets_instead_tags:
+            tags_url = url + '/packets-indicators'
+            logger.info("Packet data csv upload to {} started".format(tags_url))
+        else:
+            tags_url = url + '/tags-indicators'
+            logger.info("Tags data csv upload to {} started".format(tags_url))
+        data_list = []
+        data_list.append(encode('--' + boundary))
+        if is_batch_name_inside_logs_folder:
+            tags_data_path = 'logs/' + batch_name
+        else:
+            tags_data_path = batch_name
+        tags_data_path = os.path.join(tags_data_path, tags_data_csv_name)
+        if not os.path.exists(tags_data_path):
+            exception_string = str(tags_data_path) + ' tags_data_path could not be found \n' + \
+                               'please find it and try to upload again'
+            raise Exception(exception_string)
+        
+        if is_path:
+            tags_data_path = tags_data_csv_name
+        data_list.append(encode('Content-Disposition: form-data; name=file; filename={0}'.format(tags_data_path)))
+        file_type = mimetypes.guess_type(tags_data_path)[0] or 'application/octet-stream'
+        data_list.append(encode('Content-Type: {}'.format(file_type)))
+        data_list.append(encode(''))
+        with open(tags_data_path, 'rb') as f:
+            data_list.append(f.read())
+        data_list.append(encode('--' + boundary + '--'))
+        data_list.append(encode(''))
+        body = b'\r\n'.join(data_list)
+        payload = body
+        
+        conn.request("POST", tags_url, payload, headers)
+        tags_data_res = conn.getresponse()
+        tags_data_data = tags_data_res.read()
+        logger.info("answer from cloud is:")
+        tags_data_data_decoded = tags_data_data.decode('utf-8')
+        tags_data_data_decoded_convert = ast.literal_eval(tags_data_data_decoded)
+        try:
+            logger.info(tags_data_data_decoded_convert['data'])
+        
+        except Exception:
+            logger.warning('Problem with cloud upload')
+        
+        if str(tags_data_res.status) == '500':
+            logger.info(
+                'There was a problem at the Server side (status 500), please try to upload again or reach Wiliot')
+            return False
+        elif str(tags_data_res.status) in ['401', '400']:
+            client.auth_obj.get_token()
+            return False
+        elif str(tags_data_res.status)[0:2] == '40':
+            logger.info(
+                'There was a problem at the request side (status 40*), please try to upload again or reach Wiliot')
+            logger.info('Status code is: ' + str(tags_data_res.status))
+            return False
+        elif str(tags_data_res.status) == '200':
+            logger.info('The file "' + tags_data_csv_name + '" was uploaded successfully to Wiliot cloud')
+    logger.info('-----------------------------------------------------------------------\n'
+                'upload to cloud is finished successfully\n'
+                '-----------------------------------------------------------------------')
+    return True
+
 
 def get_cloud_error_message(status_code):
     if status_code is None:
         message = 'upload failed with unknown error code, please look inside log and reach wiliot'
     elif status_code == 500:
         message = 'There was a problem at the Server side (status 500), ' \
                   'please try to upload again or reach Wiliot'
@@ -1246,15 +1426,15 @@
                     added_headers = []
                 elif tester_type.value == TesterName.SAMPLE.value:
                     added_headers = ['responded', 'responding[%]', 'passed[%]', 'testStatus',
                                      'operator', 'testTime', 'runStartTime', 'runEndTime', 'antennaType',
                                      'surface', 'numChambers', 'gwVersion', 'pyWiliotVersion',
                                      'bleAttenuation', 'loraAttenuation', 'testTimeProfilePeriod',
                                      'testTimeProfileOnTime', 'ttfpAvg', 'tbpAvg', 'tbpStd', 'rssiAvg', 'maxTtfp',
-                                     'controlLimits', 'hwVersion', 'sub1gFrequency', 'failBinStr', 'failBin']
+                                     'controlLimits', 'hwVersion', 'sub1gFrequency']
                 else:
                     added_headers = []
             elif header_type.value == HeaderType.TAG.value:
                 if tester_type.value == TesterName.OFFLINE.value:
                     added_headers = ['externalId']
                     if self.temperature_sensor_enable:
                         added_headers.append('temperatureFromSensor')
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/upload_testers_data_to_cloud.py` & `wiliot-testers-4.0.6/wiliot_testers/upload_testers_data_to_cloud.py`

 * *Files 13% similar despite different names*

```diff
@@ -57,22 +57,51 @@
 #     (B) EVEN IF ANYONE IS ADVISED OF THE POSSIBILITY OF ANY DAMAGES, LOSSES, OR COSTS; AND
 #     (C) EVEN IF ANY REMEDY FAILS OF ITS ESSENTIAL PURPOSE.
 #  """
 import logging
 import os.path
 import PySimpleGUI as Sg
 import datetime
+import numpy as np
 import csv
 import shutil
+
 from wiliot_core import WiliotDir
-from wiliot_testers.utils.upload_to_cloud_api import upload_to_cloud_api
-from wiliot_testers.wiliot_tester_tag_result import FailureCodes
-import PySimpleGUI as SimGUI
+from wiliot_testers.tester_utils import upload_to_cloud_api
+
 
-MAX_FILE_SIZE = 12 * 10**6  # 12 Mb
+MAX_FILE_SIZE = 15 * 10**6  # 15 Mb
+
+
+def get_files_path():
+    """
+    opens GUI for selecting a file and returns it
+    """
+    # Define the window's contents
+    layout = [[Sg.Text('Choose run data file that you want to upload:'), Sg.Input(key="run_data_file"),
+               Sg.FileBrowse()],
+              [Sg.Text('Choose packets data file that you want to upload:'), Sg.Input(key="tags_data_file"),
+               Sg.FileBrowse()],
+              [Sg.Text('environment:'),
+               Sg.InputCombo(('prod', 'test'), default_value="prod", key='env')],
+              [Sg.Text('Tester type:'),
+               Sg.InputCombo(('offline-tester', 'sample-test'), default_value="offline-tester", key='tester_type')],
+              [Sg.Button('Select')]]
+
+    # Create the window
+    window = Sg.Window('upload to Cloud', layout)
+
+    event, values = window.read()
+    # See if user wants to quit or window was closed
+    if event == 'Select' and (values['run_data_file'] != '' or values['tags_data_file'] != ''):
+        window.close()
+        return values
+    else:
+        window.close()
+        return None
 
 
 def create_summary_message(is_upload=True, data_folder_name=''):
     """
     summary log
     :param is_upload:
     :type is_upload: bool or None
@@ -110,205 +139,168 @@
         self.set_logging()
         file_status = self.check_files()
         if not file_status:
             return
 
         # check file size:
         self.all_run_names = [self.values['run_data_file']]
-        self.all_packets_names = [self.values['packets_data_file']]
+        self.all_packets_names = [self.values['tags_data_file']]
         self.tester_type = self.values['tester_type']
-        file_size = os.stat(self.values['packets_data_file']).st_size
+        file_size = os.stat(self.values['tags_data_file']).st_size
         if file_size > MAX_FILE_SIZE and 'offline' in self.tester_type:
-            self.split_large_file(run_data=self.values['run_data_file'], packet_data=self.values['packets_data_file'],
+            self.split_large_file(run_data=self.values['run_data_file'], packet_data=self.values['tags_data_file'],
                                   size=file_size)
 
     def get_files_path(self):
         """
-        opens GUI for selecting a file and returns it
-        """
-        layout = [
-            [Sg.Text('Choose run data file that you want to upload:', font=("Helvetica", 11)),
-             Sg.Input(key="run_data_file", font=("Helvetica", 11)),
-             Sg.FileBrowse(font=("Helvetica", 11))],
-            [Sg.Text('Choose packets data file that you want to upload:', font=("Helvetica", 11)),
-             Sg.Input(key="packets_data_file", font=("Helvetica", 11)),
-             Sg.FileBrowse(font=("Helvetica", 11))],
-            [Sg.Text('Environment:', font=("Helvetica", 11)),
-             Sg.InputCombo(('prod', 'test'), default_value="prod", key='env', font=("Helvetica", 11))],
-            [Sg.Text('Owner id:', font=("Helvetica", 11)),
-             Sg.Input('852213717688', key='owner_id', font=("Helvetica", 11))],
-            [Sg.Text('Tester type:', font=("Helvetica", 11)),
-             Sg.InputCombo(('offline-tester', 'sample-test'), default_value="offline-tester", key='tester_type',
-                           font=("Helvetica", 11))],
-            [Sg.Button('Select', font=("Helvetica", 11))]
-        ]
+            opens GUI for selecting a file and returns it
+            """
+        # Define the window's contents
+        layout = [[Sg.Text('Choose run data file that you want to upload:'), Sg.Input(key="run_data_file"),
+                   Sg.FileBrowse()],
+                  [Sg.Text('Choose packets data file that you want to upload:'), Sg.Input(key="tags_data_file"),
+                   Sg.FileBrowse()],
+                  [Sg.Text('environment:'),
+                   Sg.InputCombo(('prod', 'test'), default_value="prod", key='env')],
+                  [Sg.Text('owner id:'),
+                   Sg.Input('wiliot-ops', key='owner_id')],
+                  [Sg.Text('Tester type:'),
+                   Sg.InputCombo(('offline-tester', 'sample-test'), default_value="offline-tester", key='tester_type')],
+                  [Sg.Button('Select')]]
 
-        window = Sg.Window('upload to Cloud', layout, size=(800, 190), font=("Helvetica", 11))
+        # Create the window
+        window = Sg.Window('upload to Cloud', layout)
 
         event, values = window.read()
-        if event == 'Select' and (values['run_data_file'] != '' or values['packets_data_file'] != ''):
+        # See if user wants to quit or window was closed
+        if event == 'Select' and (values['run_data_file'] != '' or values['tags_data_file'] != ''):
             window.close()
             self.values = values
         else:
             window.close()
             self.values = None
 
     def set_logging(self):
-        """
-        Sets up logging for the object, creating a log file with the current date and time as part of the filename.
-        Returns: None
-        """
-        #  get()dirname from run_data or packets_data
-        files_dir = os.path.dirname(self.values.get('run_data_file', self.values.get('packets_data_file')))
-        if not files_dir:
-            files_dir = os.path.join(WiliotDir().get_tester_dir("upload_to_cloud"), "logs")
-            os.makedirs(files_dir, exist_ok=True)
+
+        # set log path
+        if os.path.isfile(self.values['run_data_file']):
+            files_dir = os.path.dirname(self.values['run_data_file'])
+        elif os.path.isfile(self.values['tags_data_file']):
+            files_dir = os.path.dirname(self.values['run_data_file'])
+        else:
+            env_dir = WiliotDir()
+            files_dir = os.path.join(env_dir.get_tester_dir("upload_to_cloud"), "logs")
+            if not os.path.isdir(files_dir):
+                env_dir.create_dir(files_dir)
         log_path = os.path.join(files_dir,
                                 datetime.datetime.now().strftime("%d-%m-%Y_%H-%M-%S") + 'upload_to_cloud.log')
-        logger = logging.getLogger('Manual Upload')
-        logger.setLevel(logging.DEBUG)
-        formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S')
+
+        # set logger:
         file_handler = logging.FileHandler(log_path)
-        file_handler.setFormatter(formatter)
+        file_handler.setFormatter(
+            logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S'))
+        file_handler.setLevel(logging.DEBUG)
         stream_handler = logging.StreamHandler()
-        stream_handler.setFormatter(formatter)
+        stream_handler.setFormatter(
+            logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S'))
         stream_handler.setLevel(logging.DEBUG)
+        logger = logging.getLogger('Manual Upload')
+        logger.setLevel(logging.DEBUG)
         logger.addHandler(file_handler)
         logger.addHandler(stream_handler)
         self.logger = logger
 
     def check_files(self):
-        """
-        Checks if the run_data_file and packets_data_file are valid CSV files.
-        Returns True if both files are valid, False otherwise.
-        """
         if not os.path.isfile(self.values['run_data_file']) or not self.values['run_data_file'].endswith('.csv'):
             self.logger.warning('UPLOAD: run_data file format is not csv, please insert a csv file')
             self.logger.info(create_summary_message(False))
             return False
-        if not os.path.isfile(self.values['packets_data_file']) or not self.values['packets_data_file'].endswith('.csv'):
-            self.logger.warning('UPLOAD: packets_data file format is not csv, please insert a csv file')
+        if not os.path.isfile(self.values['tags_data_file']) or not self.values['tags_data_file'].endswith('.csv'):
+            self.logger.warning('UPLOAD: tags_data file format is not csv, please insert a csv file')
             self.logger.info(create_summary_message(False))
             return False
         return True
 
     def split_large_file(self, run_data, packet_data, size):
 
-        """
-        Splits a large packet_data CSV file into smaller parts that are each under the maximum allowed size.
-        Duplicates the corresponding run_data CSV file for each part. Returns a list of file paths for each split part.
-        """
-        # Define a helper function to generate new file paths.
         def get_new_path_name(original_path, k, total, file_str):
             new_folder_name = os.path.dirname(original_path) + f'_{k}_out_of_{n_splits}'
             new_file_name = os.path.basename(original_path).replace(f'@{file_str}_data.csv',
                                                                     f'_{k}_out_of_{total}@{file_str}_data.csv')
             if not os.path.isdir(new_folder_name):
                 os.makedirs(new_folder_name)
             return os.path.join(new_folder_name, new_file_name)
 
-        # Split the file into smaller parts.
-        n_splits = -(-size // MAX_FILE_SIZE)
+        n_splits = int(np.ceil(size / MAX_FILE_SIZE))
         part = 1
         all_packets_path = []
         all_run_path = []
         # read
         f_read = open(packet_data, 'r')
         reader = csv.DictReader(f_read, delimiter=',')
         col_names = reader.fieldnames
         # write first file
         new_packet_path = get_new_path_name(packet_data, part, n_splits, 'packets')
         all_packets_path.append(new_packet_path)
         f_write = open(new_packet_path, 'w', newline='')
         writer = csv.DictWriter(f_write, fieldnames=col_names)
         writer.writeheader()
         last_loc = 0
-        tested_list = []
-        start_loc = -1
-        missing_label_count = 0
         for i, row in enumerate(reader):
-            row['common_run_name'] = os.path.basename(new_packet_path).split('@')[0]
             if os.stat(new_packet_path).st_size < MAX_FILE_SIZE or int(row['tag_run_location']) == last_loc:
                 writer.writerow(row)
                 last_loc = int(row['tag_run_location'])
-                missing_label_count += FailureCodes.MISSING_LABEL.value == int(row['fail_bin'])
             else:  # we need to split the file
-                tested_list.append(last_loc - start_loc - missing_label_count)
                 f_write.close()
                 part += 1
                 new_packet_path = get_new_path_name(packet_data, part, n_splits, 'packets')
                 all_packets_path.append(new_packet_path)
                 f_write = open(new_packet_path, 'w', newline='')
                 writer = csv.DictWriter(f_write, fieldnames=col_names)
                 writer.writeheader()
                 writer.writerow(row)
-                start_loc = last_loc
                 last_loc = int(row['tag_run_location'])
-                missing_label_count = 0
-        tested_list.append(last_loc - start_loc)
         f_write.close()
         if part > n_splits:
             self.logger.info(
                 f'Since the file cannot be split in the middle of location data, a mismatch happened and '
                 f'the number of parts is bigger than the number of split (i.e you will have a file with '
                 f'the suufix {part}_out_of{n_splits}')
-        # Duplicate the run data for each part.
+        # duplicate run data:
         for i in range(part):
-            new_run_path = get_new_path_name(run_data, i + 1, n_splits, 'run')
+            new_run_path = get_new_path_name(run_data, i+1, n_splits, 'run')
             all_run_path.append(new_run_path)
-            with open(run_data, 'r') as f_run_read:
-                run_reader = csv.DictReader(f_run_read, delimiter=',')
-                run_col_names = run_reader.fieldnames
-                run_row = run_reader.__next__()
-            run_row['common_run_name'] = os.path.basename(new_run_path).split('@')[0]
-            run_row['total_run_tested'] = str(tested_list[i])
-            with open(new_run_path, 'w', newline='') as f_run_write:
-                run_writer = csv.DictWriter(f_run_write, fieldnames=run_col_names)
-                run_writer.writeheader()
-                run_writer.writerow(run_row)
+            shutil.copyfile(run_data, new_run_path)
 
         self.all_run_names = all_run_path
         self.all_packets_names = all_packets_path
 
     def upload_to_cloud(self):
-        """
-        Uploads files to a cloud API
-        Returns True if all uploads were successful
-        """
         if self.tester_type == 'offline-tester':
             self.tester_type = 'offline-test'
 
         all_status = []
         for run_path, packet_path in zip(self.all_run_names, self.all_packets_names):
             try:
                 upload_success = upload_to_cloud_api(batch_name=os.path.dirname(run_path),
                                                      tester_type=self.tester_type,
-                                                     run_data_csv_name=os.path.basename(run_path),
-                                                     packets_data_csv_name=os.path.basename(packet_path),
-                                                     env=self.values['env'],
+                                                     run_data_csv_name=run_path,
+                                                     tags_data_csv_name=packet_path,
+                                                     to_logging=True, env=self.values['env'],
                                                      is_batch_name_inside_logs_folder=False,
-                                                     logger_=self.logger.name, owner_id=self.values['owner_id'])
+                                                     logger_=self.logger.name, packets_instead_tags=True,
+                                                     owner_id=self.values['owner_id'],
+                                                     is_path=True)
             except Exception as e:
                 self.logger.warning(f'UPLOAD: during upload_to_cloud_api an error occurred: {e}')
                 upload_success = False
 
-            if not upload_success:
-                SimGUI.theme('GreenTan')
-                SimGUI.popup_ok(
-                    "Run upload failed. Check exception error at the console and check Internet connection is available and upload logs manually",
-                    title='Upload Error',
-                    font='Calibri',
-                    keep_on_top=True,
-                    auto_close=False,
-                    no_titlebar=True)
-
-            message = create_summary_message(is_upload=upload_success, data_folder_name=os.path.dirname(run_path))
-            self.logger.info(message)
+            self.logger.info(
+                create_summary_message(is_upload=upload_success, data_folder_name=os.path.dirname(run_path)))
             all_status.append(upload_success)
-
         return all(all_status)
 
 
 if __name__ == '__main__':
     # upload to cloud
     upload_obj = UploadTestersData()
     status = upload_obj.upload_to_cloud()
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/utils/get_version.py` & `wiliot-testers-4.0.6/wiliot_testers/utils/get_version.py`

 * *Files identical despite different names*

### Comparing `wiliot-testers-4.0.14/wiliot_testers/wiliot_tester_log.py` & `wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_log.py`

 * *Files 7% similar despite different names*

```diff
@@ -129,31 +129,31 @@
                 os.mkdir(self.log_path)
             logger_name = self.run_name + '.log'
             logger_path = os.path.join(self.log_path, logger_name)
         except Exception as e:
             self.logger.critical('Params input is invalid')
             raise e
         
-        self.file_handler = logging.FileHandler(logger_path, mode='a')
-        self.file_formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S')
-        self.file_handler.setFormatter(self.file_formatter)
-        self.logger.addHandler(self.file_handler)
-        self.results_logger.addHandler(self.file_handler)
-        self.gw_logger.addHandler(self.file_handler)
-
+        file_handler = logging.FileHandler(logger_path, mode='a')
+        file_formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s', '%H:%M:%S')
+        file_handler.setFormatter(file_formatter)
+        self.logger.addHandler(file_handler)
+        self.results_logger.addHandler(file_handler)
+        self.gw_logger.addHandler(file_handler)
+        
         self.gw_logger.addHandler(stream_handler_gw)
         self.gw_logger.setLevel(logging.INFO)
-
+        
         self.results_logger.addHandler(stream_handler2)
         self.results_logger.setLevel(logging.INFO)
-
+        
         self.logger.info(
             'Log created, path : {}'.format(str(self.log_path)))
         time.sleep(0.3)
-
+    
     def create_data_dir(self, data_path=None, tester_name='tester', run_name='test'):
         """
         create the data directory
         :param data_path: the directory path of the csv data
         :type data_path: str
         :param tester_name: the tester name such as offline teser. relevant only if data path is not specified
         :type tester_name: str
@@ -163,37 +163,18 @@
                  which contains all packets received during test
         :rtype: str, str
         """
         if data_path is None:
             wiliot_dir = WiliotDir()
             wiliot_dir.create_tester_dir(tester_name)
             data_path = os.path.join(wiliot_dir.get_tester_dir(tester_name), 'logs')
-
+        
         # create folders:
         data_folder = os.path.join(data_path, run_name)
         if not os.path.exists(data_folder):
             os.makedirs(data_folder)
-        self.data_folder = data_folder
         self.run_data_name = run_name + '@run_data.csv'
         self.packets_data_name = run_name + '@packets_data.csv'
         self.run_data_path = os.path.join(data_folder, self.run_data_name)
         self.packets_data_path = os.path.join(data_folder, self.packets_data_name)
-
+        
         return self.run_data_path, self.packets_data_path
-
-
-    def  set_new_path(self, path , formatter = None):
-        self.logger.removeHandler(self.file_handler)
-        self.results_logger.removeHandler(self.file_handler)
-        self.gw_logger.removeHandler(self.file_handler)
-        self.file_handler = logging.FileHandler(path, mode='a')
-        if formatter is None:
-            self.file_formatter = logging.Formatter('%(asctime)s,%(msecs)d %(name)s %(levelname)s %(message)s',
-                                                    '%H:%M:%S')
-        else:
-            self.file_formatter = formatter
-
-        self.file_handler.setFormatter(self.file_formatter)
-        self.logger.addHandler(self.file_handler)
-        self.results_logger.addHandler(self.file_handler)
-        self.gw_logger.addHandler(self.file_handler)
-
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/wiliot_tester_tag_result.py` & `wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,24 +81,14 @@
     DUPLICATION_OFFLINE = 14  # Duplicate offline - tag was found as duplicate during offline tester run (ADVA duplicate)
     DUPLICATION_POST_PROCESS = 15  # Duplicate post process - tag was found as duplicate in post process (UID duplicate)
     GW_ERROR = 16  # GW error
     STOP_BY_USER = 17  # test stopped by the user
     SEVERAL_TAGS_UNDER_TEST = 18  # Cannot decided which tag is under test
     FAILED_QUALITY_TEST = 19  # Failed Quality Test according to the specified statistics limits.
     NOT_PRINTED = 20  # tag was not printed due to printing offset
-    CORRUPTED_PACKET_POST_PROCESS = 21  # post process - corrupted packet detection
-    DIFF_TAG_ID_WITH_SAME_ADVA_POST_PROCESS = 22  # post process - same adva but different tag id
-    ALTERING_ADVA_POST_PROCESS = 23  # post process - tag id with "good" packets sends diff adva
-    BAD_PRINTING = 24  # as a result of printing validation, tag was decided to have a bad printing label
-    INVALID_EXTERNAL_ID_POST_PROCESS = 25  # post process - specified if external id is empty or invalid
-    SHIPMENT_INTERNAL_ID_DUPLICATION = 90  # shipment API error - decided over the cloud
-    SHIPMENT_EXTERNAL_ID_DUPLICATION = 91  # shipment API error - decided over the cloud
-    SHIPMENT_TAG_NOT_EXIST = 92  # shipment API error - decided over the cloud
-    SHIPMENT_OWNER_NOT_WILIOT_OPS = 93  # shipment API error - decided over the cloud
-    SHIPMENT_SERIALIZATION_ISSUE = 94  # shipment API error - decided over the cloud
 
 
 class ConversionTypes(Enum):
     NOT_CONVERTED = 'Unconverted'
     STANDARD = 'Regular Conversion'
     DURABLE = 'Durable Conversion'
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/wiliot_tester_tag_test.py` & `wiliot-testers-4.0.6/wiliot_testers/wiliot_tester_tag_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
         return True
 
     def gw_init(self):
         """
         initialize gw and the data listener thread
         """
         if self.GwObj is None:
-            self.GwObj = WiliotGateway(auto_connect=True, logger_name=self.logger_gw.name, is_multi_processes=True,
+            self.GwObj = WiliotGateway(auto_connect=True, logger_name=self.logger_gw.name,
                                        lock_print=threading.Lock())
         try:
             if self.GwObj.connected:
                 self.GwObj.reset_buffer()
                 self.GwObj.start_continuous_listener()
                 if self.check_gw_version():
                     self._printing_func('GW obj initialized')
@@ -317,15 +317,14 @@
 
     def gw_reset_and_config(self):
         """
         reset gw and config it to tester mode
         """
         self.GwObj.reset_gw(reset_port=False)
         self.GwObj.reset_listener()
-        time.sleep(0.5)
         if not self.GwObj.is_gw_alive():
             self._printing_func('gw_reset_and_config: wait more time since gw did not respond')
             time.sleep(5)
         self.GwObj.write('!set_tester_mode 1', with_ack=True)
         self.GwObj.write('!pl_gw_config 1', with_ack=True)
         self.GwObj.write('!listen_to_tag_only 1', with_ack=True)
         self.GwObj.write('!sub1g_sync 1', with_ack=True)
@@ -354,17 +353,15 @@
         :type wait_for_gw_trigger: int or float
         :return: if trigger was detected return True
         :rtype: bool
         """
         gw_answer = ''
         gw_trigger_init = datetime.datetime.now()
         dt = datetime.datetime.now() - gw_trigger_init
-        while gw_answer == '' and dt.total_seconds() < wait_for_gw_trigger:
-            if self.is_stopped_by_user():
-                break
+        while gw_answer == '' and not self.stop_event_trig.isSet() and dt.total_seconds() < wait_for_gw_trigger:
             gw_answer = self.GwObj.read_specific_message(msg="Start Production Line GW", read_timeout=1)
             dt = datetime.datetime.now() - gw_trigger_init
         is_trigger_received = "Start Production Line GW" in gw_answer
         if not is_trigger_received:
             self._printing_func('no trigger was detected. reset and config gw again', log_level=logging.INFO)
             self.gw_reset_and_config()
             self.init_gw_test(sub_test=self.selected_test['tests'][0], is_start_gw_app=False)
@@ -670,18 +667,18 @@
         """
         self.test_end = False
         self.time_expired = False
         self.tag_results.test_start = datetime.datetime.now()
 
         self.logger_results.info(
             'Input parameters for GW:\nStage name : {}\nPattern '
-            ': {}\nTime Profile : {}\nGW Power : {}dBm\nsub1G Power : {}dBm\nRX Channel : {}\n-----------------------'
+            ': {}\nTime Profile : {}\nGW Power : {}dBm\nsub1G Power : {}dBm\n-----------------------'
             '--------------------------------------------------'.format(
                 sub_test['name'], sub_test['energizingPattern'], sub_test['timeProfile'],
-                sub_test['gw_power_dict']['abs_power'], sub_test['sub1g_power'], sub_test['rxChannel']))
+                sub_test['gw_power_dict']['abs_power'], sub_test['sub1g_power']))
 
         # Config GW according to Test Suite
         if test_num > 0:  # first sub-test is already config before the trigger
             self.init_gw_test(sub_test=sub_test, is_start_gw_app=is_start_gw_app)
 
         # doc config param
         self.tag_results.add_run_data(test_param=sub_test)
@@ -713,17 +710,14 @@
         :rtype:
         """
         if self.first_packet_timer:
             self.first_packet_timer.cancel()
         if not only_first_packet_timer and self.test_timer:
             self.test_timer.cancel()
 
-    def is_stopped_by_user(self):
-        return self.stop_event_trig is not None and self.stop_event_trig.isSet()
-
     def _printing_func(self, msg, logger_name=LoggerName.MAIN, log_level=logging.INFO):
         """
         internal function to print the logs
         :param msg: the message to print
         :type msg: str
         :param logger_name: the logger name
         :type logger_name: LoggerName
@@ -791,15 +785,15 @@
             if need_to_manual_trigger:
                 self.GwObj.config_gw(start_gw_app=True, with_ack=True)
         else:
             self._printing_func('Wait for GW trigger for {} second'.format(wait_for_gw_trigger))
             self.start_test = self.wait_for_trigger(wait_for_gw_trigger)
 
         # check if test can be started:
-        if self.is_stopped_by_user():
+        if self.stop_event_trig.isSet():
             self._printing_func('Run was stopped by the stop event before it started', log_level=logging.INFO)
             return self.test_results
 
         if not self.start_test:
             return self.test_results
 
         self.GwObj.reset_start_time()
@@ -821,17 +815,16 @@
             self.init_test(sub_test=sub_test, test_num=test_num)
 
             # Begin test timers
             self.init_test_timers(self.max_ttfp, sub_test)
 
             # Start test check
             tags_reached_criteria = []
-            while not self.test_end and not self.time_expired:
-                if self.is_stopped_by_user():
-                    break
+            while not self.test_end and not self.stop_event_trig.isSet() and not self.time_expired:
+
                 # check if trigger was received during run:
                 if self.check_if_trigger_was_received():
                     self._printing_func('Gateway got trigger during run. Please check the Machine')
                     raise Exception('Gateway got trigger during run. Please check the Machine')
 
                 # collect filtered packets
                 is_received_packet = self.get_packets(filter_value=self.selected_test['rssiThresholdSW'])
@@ -855,15 +848,15 @@
                         self.init_gw_test(sub_test=sub_test, is_start_gw_app=True)
                         self.tag_results.test_status = FailureCodes.GW_ERROR
 
             # stop gw from transmitting
             self.GwObj.stop_gw_app()
 
             # check why the test is over
-            if self.is_stopped_by_user():  # Stop event was triggered
+            if self.stop_event_trig.isSet():  # Stop event was triggered
                 self._printing_func('Stop was triggered')
                 self._printing_func('Tag marked as Fail', logger_name=LoggerName.RESULTS)
                 self.reset_timers()
                 self.tag_results.test_status = FailureCodes.STOP_BY_USER
                 self.test_results.append(self.tag_results)
 
             elif self.time_expired:  # time expired before reaching stop criteria
@@ -888,17 +881,15 @@
                                         logger_name=LoggerName.RESULTS)
                     self.tag_results.test_status = FailureCodes.PASS
                     self.tag_results.is_test_passed = True
                     self.test_results.append(self.tag_results)
 
             elif self.test_end:
                 selected_tag = self.select_tag_under_test(optional_tags=tags_reached_criteria)  # Get the best tag
-                all_selected_tags = self.test_results.get_test_unique_adva()
-                is_diff_tag_btwn_sub_tests = selected_tag not in all_selected_tags if len(all_selected_tags) > 0 else False
-                if selected_tag is not None and not is_diff_tag_btwn_sub_tests:
+                if selected_tag is not None:
                     self._printing_func('Tag {} was selected'.format(selected_tag[0].packet_data['adv_address']))
                     # selected tag performance:
                     self.tag_results.is_test_passed = self.statistics_analyzer(test_param=sub_test, test_num=test_num)
                     if self.tag_results.is_test_passed:
                         self.tag_results.test_status = FailureCodes.PASS
                         self._printing_func('Stage {} out of {} Passed'.format(test_num + 1, num_of_tests),
                                             logger_name=LoggerName.RESULTS)
@@ -933,20 +924,17 @@
 
         # prepare gw for the next run:
         if num_of_tests > 1:
             self.init_gw_test(sub_test=self.selected_test['tests'][0], is_start_gw_app=False)
         self.reset_timers()
         return self.test_results
 
-    def exit_tag_test(self, need_to_close_port=True):
+    def exit_tag_test(self):
         self.reset_timers()
-        if need_to_close_port:
-            self.GwObj.close_port(is_reset=True)
-        else:
-            self.GwObj.reset_gw()
+        self.GwObj.close_port(is_reset=True)
         self.GwObj.stop_continuous_listener()
 
 
 if __name__ == '__main__':
     from csv import DictWriter
     import os
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/yield/arduino_counter/arduino_counter.ino` & `wiliot-testers-4.0.6/wiliot_testers/yield/arduino_counter/arduino_counter.ino`

 * *Files 4% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 
 const int input = 2; // This is where the input is fed.
 int pulse = 0; // Variable for saving pulses count.
 int var = 0;
 
 void setup(){
   pinMode(input, INPUT);
-
+ 
   Serial.begin(9600);
   Serial.println(F("No pulses yet...")); // Message to send initially (no pulses detected yet).
 }
 
-void loop(){
+void loop(){ 
   if(digitalRead(input) > var)
   {
     var = 1;
     pulse++;
-
+   
     Serial.print(pulse);
     Serial.print(F(" pulse"));
 
     // Put an "s" if the amount of pulses is greater than 1.
     if(pulse > 1) {Serial.print(F("s"));}
-
+   
     Serial.println(F(" detected."));
   }
-
+ 
   if(digitalRead(input) == 0) {var = 0;}
-
+ 
   delay(1); // Delay for stability.
 }
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers/yield/configs/inlay_data.py` & `wiliot-testers-4.0.6/wiliot_testers/yield/configs/inlay_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 csv_dictionary = {
     'TEO_086': {'inlay': 'TEO_086', 'number': '086', 'number_of_rows': 1, 'received_channel': '37',
-                'energy_pattern_val': 18, 'time_profile_val': [5, 40]},
+                'energy_pattern_val': 18, 'time_profile_val': [5, 15]},
     'TIKI_096': {'inlay': 'TIKI_096', 'number': '096', 'number_of_rows': 2, 'received_channel': '37',
-                 'energy_pattern_val': 51, 'time_profile_val': [5, 40]},
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
     'TIKI_099': {'inlay': 'TIKI_099', 'number': '099', 'number_of_rows': 3, 'received_channel': '37',
-                 'energy_pattern_val': 51, 'time_profile_val': [5, 40]},
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
     'BATTERY_107': {'inlay': 'BATTERY_107', 'number': '107', 'number_of_rows': 4, 'received_channel': '37',
-                    'energy_pattern_val': 17, 'time_profile_val': [5, 40]},
+                    'energy_pattern_val': 17, 'time_profile_val': [5, 15]},
     'TIKI_117': {'inlay': 'TIKI_117', 'number': '117', 'number_of_rows': 5, 'received_channel': '37',
-                 'energy_pattern_val': 51, 'time_profile_val': [5, 40]},
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
     'TIKI_121': {'inlay': 'TIKI_121', 'number': '121', 'number_of_rows': 6, 'received_channel': '37',
-                 'energy_pattern_val': 51, 'time_profile_val': [5, 40]},
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
     'TIKI_122': {'inlay': 'TIKI_122', 'number': '122', 'number_of_rows': 7, 'received_channel': '37',
-                 'energy_pattern_val': 51, 'time_profile_val': [5, 40]},
+                 'energy_pattern_val': 51, 'time_profile_val': [5, 15]},
     '': {'inlay': '', 'number': '', 'number_of_rows': 0, 'received_channel': '', 'energy_pattern_val': 0,
          'time_profile_val': [0, 0]}}
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers.egg-info/PKG-INFO` & `wiliot-testers-4.0.6/wiliot_testers.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiliot-testers
-Version: 4.0.14
+Version: 4.0.6
 Summary: A library for interacting with Wiliot's Testers app
 Home-page: UNKNOWN
 Author: Wiliot
 Author-email: support@wiliot.com
 License: MIT
 Project-URL: Bug Tracker, https://WILIOT-ZENDESK-URL
 Platform: UNKNOWN
@@ -56,62 +56,15 @@
 * [Sample Test](wiliot_testers/sample/sample_test.py)
 * [Yield Tester](wiliot_testers/yield/yield_tester.py)
 
 For more documentation and instructions, please contact us: support@wiliot.com
 
 
 ## Release Notes:
-Version 4.0.14:
------------------
-* sample tester:
-    * add fail bin for the whole test
-    * add the option to construct specific tests including number of tested tags and the parameters for the test to pass/fail
-* upload data to cloud:
-    * supports also dev env
-    * reduce the max size of a big file
-* test equipment:
-    * improve scanner configuration
-    * add logging
-* tester sdk:
-    * add more fail bins    
-    
-
-Version 4.0.12:
------------------
-* offline tester:
-    * add responded yield to gui
-    * add the option to change the max number of bad QR
-    * fix bug in test format
-    * fix bug when working with two gw
-    * add pop up when upload failed
-    * change default line selection to True
-    * improve code for printing GUI - production and test
-* improve harvester test
-* improve function to upload tester data to cloud including big files (>15Mb)
-* tester sdk:
-    * add more function to the tester log
-    * fix bug when stop event is not specified
-* yield:
-    * add more logging including progress data
 
-Version 4.0.11:
------------------
-* offline tester:
-    * fix bug when several tags under test and test status is still pass
-    * support 8 characters barcode label
-    * Support label scanner for both barcode and QR
-    * check printer communication during the run
-    
-* upload data:
-    * fix .bat file for upload data to the cloud
-    
-* sample test:
-    * fix script error when installing on a clean environment
-    
-    
 Version 4.0.6:
 -----------------
 * offline tester:
     *  update test suite.
     *  enable line selection using text communication with the printing (currently available only if printing offset > 0 and no QR check.
     *  add tag reel location to packet data csv (i.e. the location on the reel even if multiple runs were done on the same reel)
     *  check gw trigger (optic sensor signal) and apply printing validation, right after a trigger was received (or missing label was decided)
```

### Comparing `wiliot-testers-4.0.14/wiliot_testers.egg-info/SOURCES.txt` & `wiliot-testers-4.0.6/wiliot_testers.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,19 @@
 wiliot_testers/docs/__init__.py
 wiliot_testers/docs/tester_api_flow.pdf
 wiliot_testers/docs/wiliot_logo.png
 wiliot_testers/examples/__init__.py
 wiliot_testers/examples/wiliot_tester_example.py
 wiliot_testers/offline/README.md
 wiliot_testers/offline/__init__.py
-wiliot_testers/offline/barcode_test.py
 wiliot_testers/offline/env_install.bat
 wiliot_testers/offline/env_install.py
 wiliot_testers/offline/offline_tester.py
 wiliot_testers/offline/offline_utils.py
 wiliot_testers/offline/requirements.txt
-wiliot_testers/offline/run_barcode_testing.bat
 wiliot_testers/offline/run_offline_tester.bat
 wiliot_testers/offline/tadbik_r2r_controller.py
 wiliot_testers/offline/configs/__init__.py
 wiliot_testers/offline/configs/test_configs.json
 wiliot_testers/offline/configs/tests_suites.json
 wiliot_testers/offline/docs/__init__.py
 wiliot_testers/offline/docs/example_of_timing_diagram.jpg
@@ -76,15 +74,14 @@
 wiliot_testers/sample/utils/save.png
 wiliot_testers/sample/utils/wiliot3.gif
 wiliot_testers/system_test/__init__.py
 wiliot_testers/system_test/harvester_test.py
 wiliot_testers/system_test/system_test_example.py
 wiliot_testers/utils/__init__.py
 wiliot_testers/utils/get_version.py
-wiliot_testers/utils/upload_to_cloud_api.py
 wiliot_testers/yield/__init__.py
 wiliot_testers/yield/run_yield_tester.bat
 wiliot_testers/yield/yield_tester.py
 wiliot_testers/yield/arduino_counter/__init__.py
 wiliot_testers/yield/arduino_counter/arduino_counter.ino
 wiliot_testers/yield/configs/.default_configs.json
 wiliot_testers/yield/configs/__init__.py
```

