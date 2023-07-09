# Comparing `tmp/anyconfig-fit-backend-0.1.1.tar.gz` & `tmp/anyconfig-fit-backend-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyconfig-fit-backend-0.1.1.tar", last modified: Fri Dec 31 16:47:21 2021, max compression
+gzip compressed data, was "anyconfig-fit-backend-0.2.0.tar", last modified: Sun Jul  9 13:57:43 2023, max compression
```

## Comparing `anyconfig-fit-backend-0.1.1.tar` & `anyconfig-fit-backend-0.2.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.365942 anyconfig-fit-backend-0.1.1/
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.318942 anyconfig-fit-backend-0.1.1/.github/
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.319942 anyconfig-fit-backend-0.1.1/.github/workflows/
--rw-r--r--   0 ssato     (1000) ssato     (1000)      866 2021-12-31 15:52:45.000000 anyconfig-fit-backend-0.1.1/.github/workflows/tests.yml
--rw-r--r--   0 ssato     (1000) ssato     (1000)     1069 2021-12-30 12:28:08.000000 anyconfig-fit-backend-0.1.1/LICENSE.MIT
--rw-r--r--   0 ssato     (1000) ssato     (1000)      225 2021-12-30 12:30:24.000000 anyconfig-fit-backend-0.1.1/MANIFEST.in
--rw-r--r--   0 ssato     (1000) ssato     (1000)      186 2021-12-31 16:36:40.000000 anyconfig-fit-backend-0.1.1/NEWS
--rw-r--r--   0 ssato     (1000) ssato     (1000)     3955 2021-12-31 16:47:21.365942 anyconfig-fit-backend-0.1.1/PKG-INFO
--rw-r--r--   0 ssato     (1000) ssato     (1000)     2529 2021-12-31 16:39:29.000000 anyconfig-fit-backend-0.1.1/README.rst
--rw-r--r--   0 ssato     (1000) ssato     (1000)       66 2021-12-30 12:29:55.000000 anyconfig-fit-backend-0.1.1/mypy.ini
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.319942 anyconfig-fit-backend-0.1.1/pkg/
--rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-fit-backend-0.1.1/pkg/copr-build.sh
--rw-rw-r--   0 ssato     (1000) ssato     (1000)     1376 2021-12-31 16:36:50.000000 anyconfig-fit-backend-0.1.1/pkg/package.spec.in
--rw-r--r--   0 ssato     (1000) ssato     (1000)       94 2021-12-30 17:32:52.000000 anyconfig-fit-backend-0.1.1/requirements.txt
--rw-r--r--   0 ssato     (1000) ssato     (1000)     1712 2021-12-31 16:47:21.365942 anyconfig-fit-backend-0.1.1/setup.cfg
--rw-r--r--   0 ssato     (1000) ssato     (1000)     1501 2021-12-30 12:29:55.000000 anyconfig-fit-backend-0.1.1/setup.py
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.318942 anyconfig-fit-backend-0.1.1/src/
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.319942 anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend/
--rw-r--r--   0 ssato     (1000) ssato     (1000)      130 2021-12-31 16:46:09.000000 anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend/__init__.py
--rw-r--r--   0 ssato     (1000) ssato     (1000)     9697 2021-12-31 15:47:15.000000 anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend/parser.py
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.320942 anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend.egg-info/
--rw-r--r--   0 ssato     (1000) ssato     (1000)     3955 2021-12-31 16:47:21.000000 anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend.egg-info/PKG-INFO
--rw-r--r--   0 ssato     (1000) ssato     (1000)     3190 2021-12-31 16:47:21.000000 anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend.egg-info/SOURCES.txt
--rw-r--r--   0 ssato     (1000) ssato     (1000)        1 2021-12-31 16:47:21.000000 anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend.egg-info/dependency_links.txt
--rw-r--r--   0 ssato     (1000) ssato     (1000)       57 2021-12-31 16:47:21.000000 anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend.egg-info/entry_points.txt
--rw-r--r--   0 ssato     (1000) ssato     (1000)       10 2021-12-31 16:47:21.000000 anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend.egg-info/requires.txt
--rw-r--r--   0 ssato     (1000) ssato     (1000)       22 2021-12-31 16:47:21.000000 anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend.egg-info/top_level.txt
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.321942 anyconfig-fit-backend-0.1.1/tests/
--rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2015-05-31 04:08:11.000000 anyconfig-fit-backend-0.1.1/tests/__init__.py
--rw-r--r--   0 ssato     (1000) ssato     (1000)      300 2021-12-31 15:23:17.000000 anyconfig-fit-backend-0.1.1/tests/constants.py
--rw-r--r--   0 ssato     (1000) ssato     (1000)      108 2021-12-31 02:41:11.000000 anyconfig-fit-backend-0.1.1/tests/requirements.txt
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.321942 anyconfig-fit-backend-0.1.1/tests/res/
--rw-r--r--   0 ssato     (1000) ssato     (1000)      121 2021-12-31 02:21:26.000000 anyconfig-fit-backend-0.1.1/tests/res/README.md
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.321942 anyconfig-fit-backend-0.1.1/tests/res/ng/
--rw-r--r--   0 ssato     (1000) ssato     (1000)      130 2021-12-31 02:24:39.000000 anyconfig-fit-backend-0.1.1/tests/res/ng/README.md
--rw-r--r--   0 ssato     (1000) ssato     (1000)     1542 2021-12-31 02:22:59.000000 anyconfig-fit-backend-0.1.1/tests/res/ng/activity-activity-filecrc.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)      771 2021-12-31 02:22:59.000000 anyconfig-fit-backend-0.1.1/tests/res/ng/activity-filecrc.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)      854 2021-12-31 02:22:59.000000 anyconfig-fit-backend-0.1.1/tests/res/ng/activity-settings-corruptheader.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)      786 2021-12-31 02:22:59.000000 anyconfig-fit-backend-0.1.1/tests/res/ng/activity-settings-nodata.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)      768 2021-12-31 02:22:59.000000 anyconfig-fit-backend-0.1.1/tests/res/ng/activity-unexpected-eof.fit
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.361942 anyconfig-fit-backend-0.1.1/tests/res/ok/
--rw-r--r--   0 ssato     (1000) ssato     (1000)      771 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/Activity.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)    42364 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/Activity.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)      178 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/DeveloperData.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)     8937 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/DeveloperData.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)     2087 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/MonitoringFile.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)   285451 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/MonitoringFile.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)      221 2021-12-31 02:25:36.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/README.md
--rw-r--r--   0 ssato     (1000) ssato     (1000)     1287 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/Settings.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)    72112 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/Settings.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)     1737 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/Settings2.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)    97457 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/Settings2.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)      170 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WeightScaleMultiUser.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)     9330 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WeightScaleMultiUser.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)      150 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WeightScaleSingleUser.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)     7814 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WeightScaleSingleUser.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)      213 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutCustomTargetValues.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)    10082 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutCustomTargetValues.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)      175 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutIndividualSteps.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)     8709 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutIndividualSteps.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)      193 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutRepeatGreaterThanStep.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)     9782 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutRepeatGreaterThanStep.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)      193 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutRepeatSteps.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)     9764 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutRepeatSteps.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)      853 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/activity-settings.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)    46801 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/activity-settings.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)   121839 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/activity-small-fenix2-run.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)  7644118 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/activity-small-fenix2-run.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)     1933 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/antfs-dump.63.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)   355705 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/antfs-dump.63.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)     5785 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/compressed-speed-distance.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)   832605 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/compressed-speed-distance.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)   147940 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/developer-types-sample.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)  8174872 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/developer-types-sample.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)    88904 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/event_timestamp.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)  6555518 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/event_timestamp.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)   356829 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-edge-500-activity.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000) 22643846 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-edge-500-activity.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)     4229 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-edge-820-bike.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)   213073 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-edge-820-bike.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)     4664 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-bike.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)   243201 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-bike.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)     5597 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-run.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)   272706 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-run.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)     5187 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-walk.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)   251269 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-walk.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)   222283 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fr935-cr.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000) 14340003 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fr935-cr.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)    67518 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/null_compressed_speed_dist.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)  4648401 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/null_compressed_speed_dist.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)    28628 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/sample-activity-indoor-trainer.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)  2491413 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/sample-activity-indoor-trainer.json
--rw-r--r--   0 ssato     (1000) ssato     (1000)   104761 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/sample-activity.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)  6630708 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/sample-activity.json
-drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2021-12-31 16:47:21.365942 anyconfig-fit-backend-0.1.1/tests/res/ok/skipped/
--rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/skipped/2013-02-06-12-11-14.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/skipped/2015-10-13-08-43-15.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/skipped/20170518-191602-1740899583.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/skipped/2019-02-17-062644-ELEMNT-297E-195-0.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/skipped/Edge810-Vector-2013-08-16-15-35-10.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.1.1/tests/res/ok/skipped/activity-large-fenxi2-multisport.fit
--rw-r--r--   0 ssato     (1000) ssato     (1000)      308 2021-12-31 02:19:50.000000 anyconfig-fit-backend-0.1.1/tests/test_constants.py
--rw-r--r--   0 ssato     (1000) ssato     (1000)     1481 2021-12-31 03:33:59.000000 anyconfig-fit-backend-0.1.1/tests/test_parser.py
--rw-r--r--   0 ssato     (1000) ssato     (1000)     1207 2021-12-31 13:28:55.000000 anyconfig-fit-backend-0.1.1/tests/test_plugin.py
--rw-r--r--   0 ssato     (1000) ssato     (1000)      846 2021-12-31 15:50:00.000000 anyconfig-fit-backend-0.1.1/tox.ini
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.756507 anyconfig-fit-backend-0.2.0/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.703506 anyconfig-fit-backend-0.2.0/.github/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.705506 anyconfig-fit-backend-0.2.0/.github/workflows/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      858 2023-07-09 13:42:34.000000 anyconfig-fit-backend-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1069 2021-12-30 12:28:08.000000 anyconfig-fit-backend-0.2.0/LICENSE.MIT
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      225 2021-12-30 12:30:24.000000 anyconfig-fit-backend-0.2.0/MANIFEST.in
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      186 2021-12-31 16:36:40.000000 anyconfig-fit-backend-0.2.0/NEWS
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     3485 2023-07-09 13:57:43.756507 anyconfig-fit-backend-0.2.0/PKG-INFO
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     2110 2023-07-09 13:48:41.000000 anyconfig-fit-backend-0.2.0/README.rst
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       66 2021-12-30 12:29:55.000000 anyconfig-fit-backend-0.2.0/mypy.ini
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.705506 anyconfig-fit-backend-0.2.0/pkg/
+-rwxrwxr-x   0 ssato     (1000) ssato     (1000)      494 2018-01-01 13:54:49.000000 anyconfig-fit-backend-0.2.0/pkg/copr-build.sh
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)     1543 2023-07-09 13:55:17.000000 anyconfig-fit-backend-0.2.0/pkg/package.spec.in
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       94 2021-12-30 17:32:52.000000 anyconfig-fit-backend-0.2.0/requirements.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1674 2023-07-09 13:57:43.757507 anyconfig-fit-backend-0.2.0/setup.cfg
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1501 2021-12-30 12:29:55.000000 anyconfig-fit-backend-0.2.0/setup.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.703506 anyconfig-fit-backend-0.2.0/src/
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.705506 anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      130 2023-07-09 13:47:28.000000 anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     9697 2021-12-31 15:47:15.000000 anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend/parser.py
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.706506 anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend.egg-info/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     3485 2023-07-09 13:57:43.000000 anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend.egg-info/PKG-INFO
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     3190 2023-07-09 13:57:43.000000 anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)        1 2023-07-09 13:57:43.000000 anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       56 2023-07-09 13:57:43.000000 anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend.egg-info/entry_points.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       10 2023-07-09 13:57:43.000000 anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend.egg-info/requires.txt
+-rw-r--r--   0 ssato     (1000) ssato     (1000)       22 2023-07-09 13:57:43.000000 anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend.egg-info/top_level.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.707507 anyconfig-fit-backend-0.2.0/tests/
+-rw-rw-r--   0 ssato     (1000) ssato     (1000)        0 2015-05-31 04:08:11.000000 anyconfig-fit-backend-0.2.0/tests/__init__.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      300 2021-12-31 15:23:17.000000 anyconfig-fit-backend-0.2.0/tests/constants.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      108 2021-12-31 02:41:11.000000 anyconfig-fit-backend-0.2.0/tests/requirements.txt
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.707507 anyconfig-fit-backend-0.2.0/tests/res/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      121 2021-12-31 02:21:26.000000 anyconfig-fit-backend-0.2.0/tests/res/README.md
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.708506 anyconfig-fit-backend-0.2.0/tests/res/ng/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      130 2021-12-31 02:24:39.000000 anyconfig-fit-backend-0.2.0/tests/res/ng/README.md
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1542 2021-12-31 02:22:59.000000 anyconfig-fit-backend-0.2.0/tests/res/ng/activity-activity-filecrc.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      771 2021-12-31 02:22:59.000000 anyconfig-fit-backend-0.2.0/tests/res/ng/activity-filecrc.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      854 2021-12-31 02:22:59.000000 anyconfig-fit-backend-0.2.0/tests/res/ng/activity-settings-corruptheader.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      786 2021-12-31 02:22:59.000000 anyconfig-fit-backend-0.2.0/tests/res/ng/activity-settings-nodata.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      768 2021-12-31 02:22:59.000000 anyconfig-fit-backend-0.2.0/tests/res/ng/activity-unexpected-eof.fit
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.752507 anyconfig-fit-backend-0.2.0/tests/res/ok/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      771 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/Activity.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)    42364 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/Activity.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      178 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/DeveloperData.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     8937 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/DeveloperData.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     2087 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/MonitoringFile.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   285451 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/MonitoringFile.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      221 2021-12-31 02:25:36.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/README.md
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1287 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/Settings.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)    72112 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/Settings.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1737 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/Settings2.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)    97457 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/Settings2.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      170 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WeightScaleMultiUser.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     9330 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WeightScaleMultiUser.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      150 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WeightScaleSingleUser.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     7814 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WeightScaleSingleUser.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      213 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutCustomTargetValues.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)    10082 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutCustomTargetValues.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      175 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutIndividualSteps.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     8709 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutIndividualSteps.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      193 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutRepeatGreaterThanStep.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     9782 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutRepeatGreaterThanStep.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      193 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutRepeatSteps.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     9764 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutRepeatSteps.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      853 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/activity-settings.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)    46801 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/activity-settings.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   121839 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/activity-small-fenix2-run.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)  7644118 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/activity-small-fenix2-run.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1933 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/antfs-dump.63.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   355705 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/antfs-dump.63.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     5785 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/compressed-speed-distance.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   832605 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/compressed-speed-distance.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   147940 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/developer-types-sample.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)  8174872 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/developer-types-sample.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)    88904 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/event_timestamp.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)  6555518 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/event_timestamp.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   356829 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-edge-500-activity.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000) 22643846 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-edge-500-activity.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     4229 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-edge-820-bike.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   213073 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-edge-820-bike.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     4664 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-bike.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   243201 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-bike.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     5597 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-run.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   272706 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-run.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     5187 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-walk.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   251269 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-walk.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   222283 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fr935-cr.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000) 14340003 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fr935-cr.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)    67518 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/null_compressed_speed_dist.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)  4648401 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/null_compressed_speed_dist.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)    28628 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/sample-activity-indoor-trainer.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)  2491413 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/sample-activity-indoor-trainer.json
+-rw-r--r--   0 ssato     (1000) ssato     (1000)   104761 2021-12-31 02:23:23.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/sample-activity.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)  6630708 2021-12-31 02:25:57.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/sample-activity.json
+drwxr-xr-x   0 ssato     (1000) ssato     (1000)        0 2023-07-09 13:57:43.756507 anyconfig-fit-backend-0.2.0/tests/res/ok/skipped/
+-rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/skipped/2013-02-06-12-11-14.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/skipped/2015-10-13-08-43-15.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/skipped/20170518-191602-1740899583.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/skipped/2019-02-17-062644-ELEMNT-297E-195-0.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/skipped/Edge810-Vector-2013-08-16-15-35-10.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)        0 2021-12-31 15:30:24.000000 anyconfig-fit-backend-0.2.0/tests/res/ok/skipped/activity-large-fenxi2-multisport.fit
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      308 2021-12-31 02:19:50.000000 anyconfig-fit-backend-0.2.0/tests/test_constants.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1481 2021-12-31 03:33:59.000000 anyconfig-fit-backend-0.2.0/tests/test_parser.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)     1207 2021-12-31 13:28:55.000000 anyconfig-fit-backend-0.2.0/tests/test_plugin.py
+-rw-r--r--   0 ssato     (1000) ssato     (1000)      829 2023-07-09 13:42:34.000000 anyconfig-fit-backend-0.2.0/tox.ini
```

### Comparing `anyconfig-fit-backend-0.1.1/.github/workflows/tests.yml` & `anyconfig-fit-backend-0.2.0/.github/workflows/tests.yml`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,18 @@
     strategy:
       max-parallel: 5
       matrix:
         platform:
           - ubuntu-latest
           # - macos-latest
         python-version:
-          - 3.6
-          - 3.7
           - 3.8
           - 3.9
-          - 3
+          - "3.10"
+          - "3.11"
 
     steps:
       - uses: actions/checkout@v1
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `anyconfig-fit-backend-0.1.1/LICENSE.MIT` & `anyconfig-fit-backend-0.2.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/PKG-INFO` & `anyconfig-fit-backend-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyconfig-fit-backend
-Version: 0.1.1
+Version: 0.2.0
 Summary: Backend module for python-anyconfig to load FIT data files
 Home-page: https://github.com/ssato/python-anyconfig-fit-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
@@ -14,19 +14,18 @@
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-fit-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-fit-backend
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE.MIT
 
 ==================================
@@ -49,22 +48,14 @@
    :target: https://github.com/ssato/python-anyconfig-fit-backend/actions?query=workflow%3ATests
    :alt: [Github Actions: Test status]
 
 .. .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-fit-backend.svg
    :target: https://coveralls.io/r/ssato/python-anyconfig-fit-backend
    :alt: Coverage Status
 
-.. image:: https://img.shields.io/lgtm/alerts/g/ssato/python-anyconfig-fit-backend.svg
-   :target: https://lgtm.com/projects/g/ssato/python-anyconfig-fit-backend/alerts/
-   :alt: [Total Alerts by LGTM]
-
-.. image:: https://img.shields.io/lgtm/grade/python/g/ssato/python-anyconfig-fit-backend.svg
-   :target: https://lgtm.com/projects/g/ssato/python-anyconfig-fit-backend/context:python
-   :alt: [Code Quality by LGTM]
-
 This is a backend module for python-anyconfig to support to load and parse
 FIT (Flexible and Interoperable Data Transfer) data files.
 
 - Author: Satoru SATOH
 - License: MIT
 
 SEE ALSO:
@@ -98,9 +89,7 @@
 Otherwise, try usual ways to build and/or install python modules such like
 'python setup.py bdist', etc.
 
 .. [#] https://pypi.org/project/anyconfig-fit-backend/
 .. [#]  https://copr.fedorainfracloud.org/coprs/ssato/python-anyconfig/packages/
 
 .. vim:sw=2:ts=2:et:
-
-
```

### Comparing `anyconfig-fit-backend-0.1.1/README.rst` & `anyconfig-fit-backend-0.2.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -18,22 +18,14 @@
    :target: https://github.com/ssato/python-anyconfig-fit-backend/actions?query=workflow%3ATests
    :alt: [Github Actions: Test status]
 
 .. .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-fit-backend.svg
    :target: https://coveralls.io/r/ssato/python-anyconfig-fit-backend
    :alt: Coverage Status
 
-.. image:: https://img.shields.io/lgtm/alerts/g/ssato/python-anyconfig-fit-backend.svg
-   :target: https://lgtm.com/projects/g/ssato/python-anyconfig-fit-backend/alerts/
-   :alt: [Total Alerts by LGTM]
-
-.. image:: https://img.shields.io/lgtm/grade/python/g/ssato/python-anyconfig-fit-backend.svg
-   :target: https://lgtm.com/projects/g/ssato/python-anyconfig-fit-backend/context:python
-   :alt: [Code Quality by LGTM]
-
 This is a backend module for python-anyconfig to support to load and parse
 FIT (Flexible and Interoperable Data Transfer) data files.
 
 - Author: Satoru SATOH
 - License: MIT
 
 SEE ALSO:
```

### Comparing `anyconfig-fit-backend-0.1.1/pkg/package.spec.in` & `anyconfig-fit-backend-0.2.0/pkg/package.spec.in`

 * *Files 9% similar despite different names*

```diff
@@ -39,12 +39,16 @@
 %py3_install
 
 %files       -n python3-%{pkgname}
 %doc README.rst
 %{python3_sitelib}/*
 
 %changelog
+* Sun Jul  9 2023 Satoru SATOH <satoru.satoh@gmail.com> - 0.2.0-1
+- fix: follow changes in anyconfig
+- change: fix: drop python {2.7,3.{6,7} and add 3.1{0,1} support
+
 * Sat Jan  1 2022 Satoru SATOH <satoru.satoh@gmail.com> - 0.1.1-1
 - fix: [rpm] add a missing runtime dependency to python3-fitdecode
 
 * Sat Jan  1 2022 Satoru SATOH <satoru.satoh@gmail.com> - 0.1.0-1
 - Initial packaging
```

### Comparing `anyconfig-fit-backend-0.1.1/setup.cfg` & `anyconfig-fit-backend-0.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -23,19 +23,18 @@
 platforms = 
 	any
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: Utilities
 	License :: OSI Approved :: MIT License
 
 [options]
 include_package_data = True
```

### Comparing `anyconfig-fit-backend-0.1.1/setup.py` & `anyconfig-fit-backend-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend/parser.py` & `anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend/parser.py`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend.egg-info/PKG-INFO` & `anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyconfig-fit-backend
-Version: 0.1.1
+Version: 0.2.0
 Summary: Backend module for python-anyconfig to load FIT data files
 Home-page: https://github.com/ssato/python-anyconfig-fit-backend
 Author: Satoru SATOH
 Author-email: satoru.satoh@gmail.com
 Maintainer: Satoru SATOH
 Maintainer-email: satoru.satoh@gmail.com
 License: MIT
@@ -14,19 +14,18 @@
 Project-URL: Bug Tracker, https://github.com/ssato/python-anyconfig-fit-backend/issues
 Project-URL: Source, https://github.com/ssato/python-anyconfig-fit-backend
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: MIT License
 License-File: LICENSE.MIT
 
 ==================================
@@ -49,22 +48,14 @@
    :target: https://github.com/ssato/python-anyconfig-fit-backend/actions?query=workflow%3ATests
    :alt: [Github Actions: Test status]
 
 .. .. image:: https://img.shields.io/coveralls/ssato/python-anyconfig-fit-backend.svg
    :target: https://coveralls.io/r/ssato/python-anyconfig-fit-backend
    :alt: Coverage Status
 
-.. image:: https://img.shields.io/lgtm/alerts/g/ssato/python-anyconfig-fit-backend.svg
-   :target: https://lgtm.com/projects/g/ssato/python-anyconfig-fit-backend/alerts/
-   :alt: [Total Alerts by LGTM]
-
-.. image:: https://img.shields.io/lgtm/grade/python/g/ssato/python-anyconfig-fit-backend.svg
-   :target: https://lgtm.com/projects/g/ssato/python-anyconfig-fit-backend/context:python
-   :alt: [Code Quality by LGTM]
-
 This is a backend module for python-anyconfig to support to load and parse
 FIT (Flexible and Interoperable Data Transfer) data files.
 
 - Author: Satoru SATOH
 - License: MIT
 
 SEE ALSO:
@@ -98,9 +89,7 @@
 Otherwise, try usual ways to build and/or install python modules such like
 'python setup.py bdist', etc.
 
 .. [#] https://pypi.org/project/anyconfig-fit-backend/
 .. [#]  https://copr.fedorainfracloud.org/coprs/ssato/python-anyconfig/packages/
 
 .. vim:sw=2:ts=2:et:
-
-
```

### Comparing `anyconfig-fit-backend-0.1.1/src/anyconfig_fit_backend.egg-info/SOURCES.txt` & `anyconfig-fit-backend-0.2.0/src/anyconfig_fit_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ng/activity-activity-filecrc.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ng/activity-activity-filecrc.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ng/activity-filecrc.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ng/activity-filecrc.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ng/activity-settings-corruptheader.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ng/activity-settings-corruptheader.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ng/activity-settings-nodata.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ng/activity-settings-nodata.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ng/activity-unexpected-eof.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ng/activity-unexpected-eof.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/Activity.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/Activity.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/Activity.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/Activity.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/DeveloperData.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/DeveloperData.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/MonitoringFile.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/MonitoringFile.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/MonitoringFile.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/MonitoringFile.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/Settings.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/Settings.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/Settings.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/Settings.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/Settings2.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/Settings2.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/Settings2.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/Settings2.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/WeightScaleMultiUser.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/WeightScaleMultiUser.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/WeightScaleSingleUser.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/WeightScaleSingleUser.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutCustomTargetValues.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutCustomTargetValues.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutIndividualSteps.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutIndividualSteps.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutRepeatGreaterThanStep.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutRepeatGreaterThanStep.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/WorkoutRepeatSteps.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/WorkoutRepeatSteps.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/activity-settings.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/activity-settings.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/activity-settings.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/activity-settings.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/activity-small-fenix2-run.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/activity-small-fenix2-run.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/activity-small-fenix2-run.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/activity-small-fenix2-run.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/antfs-dump.63.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/antfs-dump.63.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/antfs-dump.63.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/antfs-dump.63.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/compressed-speed-distance.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/compressed-speed-distance.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/compressed-speed-distance.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/compressed-speed-distance.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/developer-types-sample.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/developer-types-sample.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/developer-types-sample.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/developer-types-sample.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/event_timestamp.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/event_timestamp.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/event_timestamp.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/event_timestamp.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-edge-500-activity.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-edge-500-activity.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-edge-500-activity.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-edge-500-activity.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-edge-820-bike.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-edge-820-bike.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-edge-820-bike.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-edge-820-bike.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-bike.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-bike.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-bike.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-bike.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-run.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-run.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-run.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-run.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-walk.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-walk.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fenix-5-walk.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fenix-5-walk.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fr935-cr.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fr935-cr.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/garmin-fr935-cr.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/garmin-fr935-cr.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/null_compressed_speed_dist.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/null_compressed_speed_dist.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/null_compressed_speed_dist.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/null_compressed_speed_dist.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/sample-activity-indoor-trainer.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/sample-activity-indoor-trainer.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/sample-activity-indoor-trainer.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/sample-activity-indoor-trainer.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/sample-activity.fit` & `anyconfig-fit-backend-0.2.0/tests/res/ok/sample-activity.fit`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/res/ok/sample-activity.json` & `anyconfig-fit-backend-0.2.0/tests/res/ok/sample-activity.json`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/test_parser.py` & `anyconfig-fit-backend-0.2.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tests/test_plugin.py` & `anyconfig-fit-backend-0.2.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `anyconfig-fit-backend-0.1.1/tox.ini` & `anyconfig-fit-backend-0.2.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [tox]
-envlist = py36, py37, py38, py39, py310
+envlist = py38, py39, py310, py311
 
 [gh-actions]
 python =
-    3.6: py36
-    3.7: py37
     3.8: py38
     3.9: py39
-    3.10: py310, lint, type-check
+    3.10: py310
+    3.11: py311, lint, type-check
 
 [testenv]
 deps =
     -r{toxinidir}/requirements.txt
     -r{toxinidir}/tests/requirements.txt
 setenv =
     PYTHONPATH = {toxinidir}/src
```

