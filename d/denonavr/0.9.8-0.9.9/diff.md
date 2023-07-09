# Comparing `tmp/denonavr-0.9.8.tar.gz` & `tmp/denonavr-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\denonavr-0.9.8.tar", last modified: Sun Dec 13 23:22:21 2020, max compression
+gzip compressed data, was "dist\denonavr-0.9.9.tar", last modified: Sun Dec 20 23:26:32 2020, max compression
```

## Comparing `denonavr-0.9.8.tar` & `denonavr-0.9.9.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxrwx   0        0        0        0 2020-12-13 23:22:21.017711 denonavr-0.9.8/
--rw-rw-rw-   0        0        0      841 2020-12-13 23:22:21.016710 denonavr-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     4919 2020-12-13 23:02:30.000000 denonavr-0.9.8/README.rst
-drwxrwxrwx   0        0        0        0 2020-12-13 23:22:19.895776 denonavr-0.9.8/denonavr/
--rw-rw-rw-   0        0        0     1305 2020-12-13 23:02:30.000000 denonavr-0.9.8/denonavr/__init__.py
--rw-rw-rw-   0        0        0     6161 2020-12-13 23:13:01.000000 denonavr-0.9.8/denonavr/audyssey.py
--rw-rw-rw-   0        0        0    91826 2020-12-13 23:08:07.000000 denonavr-0.9.8/denonavr/denonavr.py
--rw-rw-rw-   0        0        0     7968 2020-11-18 23:53:49.000000 denonavr-0.9.8/denonavr/ssdp.py
-drwxrwxrwx   0        0        0        0 2020-12-13 23:22:19.965640 denonavr-0.9.8/denonavr.egg-info/
--rw-rw-rw-   0        0        0      841 2020-12-13 23:22:19.000000 denonavr-0.9.8/denonavr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5041 2020-12-13 23:22:19.000000 denonavr-0.9.8/denonavr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-12-13 23:22:19.000000 denonavr-0.9.8/denonavr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2018-10-07 22:17:12.000000 denonavr-0.9.8/denonavr.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2020-12-13 23:22:19.000000 denonavr-0.9.8/denonavr.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2020-12-13 23:22:19.000000 denonavr-0.9.8/denonavr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-12-13 23:22:21.017711 denonavr-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1219 2020-12-13 23:02:30.000000 denonavr-0.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2020-12-13 23:22:19.968639 denonavr-0.9.8/tests/
--rw-rw-rw-   0        0        0     7095 2020-11-18 23:43:27.000000 denonavr-0.9.8/tests/test_denonavr.py
--rw-rw-rw-   0        0        0     1139 2020-05-24 21:36:25.000000 denonavr-0.9.8/tests/test_ssdp.py
-drwxrwxrwx   0        0        0        0 2020-12-13 23:22:21.013711 denonavr-0.9.8/tests/xml/
--rw-rw-rw-   0        0        0     3287 2020-03-22 23:40:01.000000 denonavr-0.9.8/tests/xml/AVC-8500H-AppCommand-8080.xml
--rw-rw-rw-   0        0        0    67723 2018-08-04 13:23:42.000000 denonavr-0.9.8/tests/xml/AVC-8500H-Deviceinfo-8080.xml
--rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-1912-AppCommand.xml
--rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-1912-Deviceinfo.xml
--rw-rw-rw-   0        0        0     2554 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-1912-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1037 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-1912-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     5692 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-1912-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-2312CI-AppCommand.xml
--rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-2312CI-Deviceinfo.xml
--rw-rw-rw-   0        0        0     2621 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-2312CI-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1084 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-2312CI-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     5686 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-2312CI-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3311CI-AppCommand.xml
--rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3311CI-Deviceinfo.xml
--rw-rw-rw-   0        0        0     1883 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3311CI-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1169 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3311CI-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     4638 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3311CI-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3312-AppCommand.xml
--rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3312-Deviceinfo.xml
--rw-rw-rw-   0        0        0     2778 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3312-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1176 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3312-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     5702 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3312-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0     4931 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3312-formTuner_HdXml.xml
--rw-rw-rw-   0        0        0     4599 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3312-formTuner_TunerXml.xml
--rw-rw-rw-   0        0        0     1035 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3312-formZone2_Zone2XmlStatus.xml
--rw-rw-rw-   0        0        0     1034 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-3312-formZone3_Zone3XmlStatus.xml
--rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-4810-AppCommand.xml
--rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-4810-Deviceinfo.xml
--rw-rw-rw-   0        0        0     1662 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-4810-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0      190 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-4810-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     4116 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-4810-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0     3871 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-4810-formTuner_HdXml.xml
--rw-rw-rw-   0        0        0     3491 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-4810-formTuner_TunerXml.xml
--rw-rw-rw-   0        0        0      184 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-4810-formZone2_Zone2XmlStatus.xml
--rw-rw-rw-   0        0        0      184 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-4810-formZone3_Zone3XmlStatus.xml
--rw-rw-rw-   0        0        0     2171 2020-11-18 23:00:30.000000 denonavr-0.9.8/tests/xml/AVR-X1100W-AppCommand.xml
--rw-rw-rw-   0        0        0    32828 2020-10-14 07:31:47.000000 denonavr-0.9.8/tests/xml/AVR-X1100W-Deviceinfo.xml
--rw-rw-rw-   0        0        0     1414 2020-10-14 07:31:48.000000 denonavr-0.9.8/tests/xml/AVR-X1100W-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1476 2020-10-14 07:31:48.000000 denonavr-0.9.8/tests/xml/AVR-X1100W-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     2030 2020-10-14 07:31:48.000000 denonavr-0.9.8/tests/xml/AVR-X1100W-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0     3925 2020-10-14 07:31:48.000000 denonavr-0.9.8/tests/xml/AVR-X1100W-formTuner_HdXml.xml
--rw-rw-rw-   0        0        0     3599 2020-10-14 07:31:48.000000 denonavr-0.9.8/tests/xml/AVR-X1100W-formTuner_TunerXml.xml
--rw-rw-rw-   0        0        0     1331 2020-10-14 07:31:48.000000 denonavr-0.9.8/tests/xml/AVR-X1100W-formZone2_Zone2XmlStatus.xml
--rw-rw-rw-   0        0        0     1308 2020-10-14 07:31:48.000000 denonavr-0.9.8/tests/xml/AVR-X1100W-formZone3_Zone3XmlStatus.xml
--rw-rw-rw-   0        0        0     6114 2020-05-24 17:28:36.000000 denonavr-0.9.8/tests/xml/AVR-X1600H_upnp.xml
--rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-2-AppCommand.xml
--rw-rw-rw-   0        0        0    38351 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-2-Deviceinfo.xml
--rw-rw-rw-   0        0        0     1546 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-2-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1478 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-2-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     1973 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-2-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0     1762 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-AppCommand.xml
--rw-rw-rw-   0        0        0    38351 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-Deviceinfo.xml
--rw-rw-rw-   0        0        0     1546 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1478 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     1973 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0     4004 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-formTuner_HdXml.xml
--rw-rw-rw-   0        0        0     3672 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-formTuner_TunerXml.xml
--rw-rw-rw-   0        0        0     1316 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-formZone2_Zone2XmlStatus.xml
--rw-rw-rw-   0        0        0     1346 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2000-formZone3_Zone3XmlStatus.xml
--rw-rw-rw-   0        0        0     2172 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2100W-2-AppCommand.xml
--rw-rw-rw-   0        0        0    58370 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2100W-2-Deviceinfo.xml
--rw-rw-rw-   0        0        0     1487 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2100W-2-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1643 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2100W-2-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     3045 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2100W-2-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2100W-AppCommand.xml
--rw-rw-rw-   0        0        0     1815 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2100W-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1646 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2100W-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     2198 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X2100W-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0     3811 2020-11-18 23:41:35.000000 denonavr-0.9.8/tests/xml/AVR-X4100W-AppCommand.xml
--rw-rw-rw-   0        0        0    79038 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X4100W-Deviceinfo.xml
--rw-rw-rw-   0        0        0     1481 2020-11-18 23:41:19.000000 denonavr-0.9.8/tests/xml/AVR-X4100W-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1726 2020-11-18 23:41:26.000000 denonavr-0.9.8/tests/xml/AVR-X4100W-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     2184 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/AVR-X4100W-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0     2666 2020-05-24 20:57:55.000000 denonavr-0.9.8/tests/xml/AVR-X4300H-AppCommand-8080.xml
--rw-rw-rw-   0        0        0    66529 2020-05-24 20:57:46.000000 denonavr-0.9.8/tests/xml/AVR-X4300H-Deviceinfo-8080.xml
--rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-CR603-AppCommand.xml
--rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-CR603-Deviceinfo.xml
--rw-rw-rw-   0        0        0     2371 2020-11-18 23:30:28.000000 denonavr-0.9.8/tests/xml/M-CR603-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0      926 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-CR603-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     2371 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-CR603-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0     5760 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-CR603-formTuner_HdXml.xml
--rw-rw-rw-   0        0        0     5444 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-CR603-formTuner_TunerXml.xml
--rw-rw-rw-   0        0        0     1548 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-CR603-formZone2_Zone2XmlStatus.xml
--rw-rw-rw-   0        0        0     1548 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-CR603-formZone3_Zone3XmlStatus.xml
--rw-rw-rw-   0        0        0     2560 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-RC610-AppCommand.xml
--rw-rw-rw-   0        0        0    19420 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-RC610-Deviceinfo.xml
--rw-rw-rw-   0        0        0      644 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-RC610-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0      370 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-RC610-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     1819 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-RC610-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0     3546 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/M-RC610-formTuner_TunerXml.xml
--rw-rw-rw-   0        0        0     2062 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/NR1604-AppCommand.xml
--rw-rw-rw-   0        0        0    34805 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/NR1604-Deviceinfo.xml
--rw-rw-rw-   0        0        0     1595 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/NR1604-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1569 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/NR1604-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     2078 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/NR1604-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0     4009 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/NR1604-formTuner_HdXml.xml
--rw-rw-rw-   0        0        0     3677 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/NR1604-formTuner_TunerXml.xml
--rw-rw-rw-   0        0        0     1401 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/NR1604-formZone2_Zone2XmlStatus.xml
--rw-rw-rw-   0        0        0     1434 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/NR1604-formZone3_Zone3XmlStatus.xml
--rw-rw-rw-   0        0        0     2449 2020-03-22 22:16:30.000000 denonavr-0.9.8/tests/xml/NR1609-AppCommand-8080.xml
--rw-rw-rw-   0        0        0    51847 2020-03-19 22:12:53.000000 denonavr-0.9.8/tests/xml/NR1609-Deviceinfo-8080.xml
--rw-rw-rw-   0        0        0       51 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/SR5008-AppCommand.xml
--rw-rw-rw-   0        0        0    34418 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/SR5008-Deviceinfo.xml
--rw-rw-rw-   0        0        0     1330 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/SR5008-formMainZone_MainZoneXml.xml
--rw-rw-rw-   0        0        0     1603 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/SR5008-formMainZone_MainZoneXmlStatus.xml
--rw-rw-rw-   0        0        0     1919 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/SR5008-formNetAudio_StatusXml.xml
--rw-rw-rw-   0        0        0     3919 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/SR5008-formTuner_HdXml.xml
--rw-rw-rw-   0        0        0     3650 2018-10-07 21:50:33.000000 denonavr-0.9.8/tests/xml/SR5008-formTuner_TunerXml.xml
+drwxrwxrwx   0        0        0        0 2020-12-20 23:26:32.881808 denonavr-0.9.9/
+-rw-rw-rw-   0        0        0      841 2020-12-20 23:26:32.879806 denonavr-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4919 2020-12-20 23:07:58.000000 denonavr-0.9.9/README.rst
+drwxrwxrwx   0        0        0        0 2020-12-20 23:26:31.833392 denonavr-0.9.9/denonavr/
+-rw-rw-rw-   0        0        0     1305 2020-12-20 23:07:58.000000 denonavr-0.9.9/denonavr/__init__.py
+-rw-rw-rw-   0        0        0     6090 2020-12-20 23:10:43.000000 denonavr-0.9.9/denonavr/audyssey.py
+-rw-rw-rw-   0        0        0    91308 2020-12-20 23:06:17.000000 denonavr-0.9.9/denonavr/denonavr.py
+-rw-rw-rw-   0        0        0     7782 2020-12-19 16:18:04.000000 denonavr-0.9.9/denonavr/ssdp.py
+drwxrwxrwx   0        0        0        0 2020-12-20 23:26:31.868715 denonavr-0.9.9/denonavr.egg-info/
+-rw-rw-rw-   0        0        0      841 2020-12-20 23:26:31.000000 denonavr-0.9.9/denonavr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5041 2020-12-20 23:26:31.000000 denonavr-0.9.9/denonavr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-12-20 23:26:31.000000 denonavr-0.9.9/denonavr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2018-10-07 22:17:12.000000 denonavr-0.9.9/denonavr.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2020-12-20 23:26:31.000000 denonavr-0.9.9/denonavr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2020-12-20 23:26:31.000000 denonavr-0.9.9/denonavr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-12-20 23:26:32.881808 denonavr-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1219 2020-12-20 23:07:58.000000 denonavr-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2020-12-20 23:26:31.871714 denonavr-0.9.9/tests/
+-rw-rw-rw-   0        0        0     7095 2020-11-18 23:43:27.000000 denonavr-0.9.9/tests/test_denonavr.py
+-rw-rw-rw-   0        0        0     1139 2020-05-24 21:36:25.000000 denonavr-0.9.9/tests/test_ssdp.py
+drwxrwxrwx   0        0        0        0 2020-12-20 23:26:32.877806 denonavr-0.9.9/tests/xml/
+-rw-rw-rw-   0        0        0     3287 2020-03-22 23:40:01.000000 denonavr-0.9.9/tests/xml/AVC-8500H-AppCommand-8080.xml
+-rw-rw-rw-   0        0        0    67723 2018-08-04 13:23:42.000000 denonavr-0.9.9/tests/xml/AVC-8500H-Deviceinfo-8080.xml
+-rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-1912-AppCommand.xml
+-rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-1912-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     2554 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-1912-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1037 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-1912-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     5692 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-1912-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-2312CI-AppCommand.xml
+-rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-2312CI-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     2621 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-2312CI-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1084 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-2312CI-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     5686 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-2312CI-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3311CI-AppCommand.xml
+-rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3311CI-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     1883 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3311CI-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1169 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3311CI-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     4638 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3311CI-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3312-AppCommand.xml
+-rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3312-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     2778 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3312-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1176 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3312-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     5702 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3312-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0     4931 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3312-formTuner_HdXml.xml
+-rw-rw-rw-   0        0        0     4599 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3312-formTuner_TunerXml.xml
+-rw-rw-rw-   0        0        0     1035 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3312-formZone2_Zone2XmlStatus.xml
+-rw-rw-rw-   0        0        0     1034 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-3312-formZone3_Zone3XmlStatus.xml
+-rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-4810-AppCommand.xml
+-rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-4810-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     1662 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-4810-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0      190 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-4810-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     4116 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-4810-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0     3871 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-4810-formTuner_HdXml.xml
+-rw-rw-rw-   0        0        0     3491 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-4810-formTuner_TunerXml.xml
+-rw-rw-rw-   0        0        0      184 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-4810-formZone2_Zone2XmlStatus.xml
+-rw-rw-rw-   0        0        0      184 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-4810-formZone3_Zone3XmlStatus.xml
+-rw-rw-rw-   0        0        0     2171 2020-11-18 23:00:30.000000 denonavr-0.9.9/tests/xml/AVR-X1100W-AppCommand.xml
+-rw-rw-rw-   0        0        0    32828 2020-10-14 07:31:47.000000 denonavr-0.9.9/tests/xml/AVR-X1100W-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     1414 2020-10-14 07:31:48.000000 denonavr-0.9.9/tests/xml/AVR-X1100W-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1476 2020-10-14 07:31:48.000000 denonavr-0.9.9/tests/xml/AVR-X1100W-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     2030 2020-10-14 07:31:48.000000 denonavr-0.9.9/tests/xml/AVR-X1100W-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0     3925 2020-10-14 07:31:48.000000 denonavr-0.9.9/tests/xml/AVR-X1100W-formTuner_HdXml.xml
+-rw-rw-rw-   0        0        0     3599 2020-10-14 07:31:48.000000 denonavr-0.9.9/tests/xml/AVR-X1100W-formTuner_TunerXml.xml
+-rw-rw-rw-   0        0        0     1331 2020-10-14 07:31:48.000000 denonavr-0.9.9/tests/xml/AVR-X1100W-formZone2_Zone2XmlStatus.xml
+-rw-rw-rw-   0        0        0     1308 2020-10-14 07:31:48.000000 denonavr-0.9.9/tests/xml/AVR-X1100W-formZone3_Zone3XmlStatus.xml
+-rw-rw-rw-   0        0        0     6114 2020-05-24 17:28:36.000000 denonavr-0.9.9/tests/xml/AVR-X1600H_upnp.xml
+-rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-2-AppCommand.xml
+-rw-rw-rw-   0        0        0    38351 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-2-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     1546 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-2-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1478 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-2-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     1973 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-2-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0     1762 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-AppCommand.xml
+-rw-rw-rw-   0        0        0    38351 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     1546 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1478 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     1973 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0     4004 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-formTuner_HdXml.xml
+-rw-rw-rw-   0        0        0     3672 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-formTuner_TunerXml.xml
+-rw-rw-rw-   0        0        0     1316 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-formZone2_Zone2XmlStatus.xml
+-rw-rw-rw-   0        0        0     1346 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2000-formZone3_Zone3XmlStatus.xml
+-rw-rw-rw-   0        0        0     2172 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2100W-2-AppCommand.xml
+-rw-rw-rw-   0        0        0    58370 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2100W-2-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     1487 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2100W-2-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1643 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2100W-2-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     3045 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2100W-2-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0      194 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2100W-AppCommand.xml
+-rw-rw-rw-   0        0        0     1815 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2100W-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1646 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2100W-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     2198 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X2100W-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0     3811 2020-11-18 23:41:35.000000 denonavr-0.9.9/tests/xml/AVR-X4100W-AppCommand.xml
+-rw-rw-rw-   0        0        0    79038 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X4100W-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     1481 2020-11-18 23:41:19.000000 denonavr-0.9.9/tests/xml/AVR-X4100W-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1726 2020-11-18 23:41:26.000000 denonavr-0.9.9/tests/xml/AVR-X4100W-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     2184 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/AVR-X4100W-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0     2666 2020-05-24 20:57:55.000000 denonavr-0.9.9/tests/xml/AVR-X4300H-AppCommand-8080.xml
+-rw-rw-rw-   0        0        0    66529 2020-05-24 20:57:46.000000 denonavr-0.9.9/tests/xml/AVR-X4300H-Deviceinfo-8080.xml
+-rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-CR603-AppCommand.xml
+-rw-rw-rw-   0        0        0      170 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-CR603-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     2371 2020-11-18 23:30:28.000000 denonavr-0.9.9/tests/xml/M-CR603-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0      926 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-CR603-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     2371 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-CR603-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0     5760 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-CR603-formTuner_HdXml.xml
+-rw-rw-rw-   0        0        0     5444 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-CR603-formTuner_TunerXml.xml
+-rw-rw-rw-   0        0        0     1548 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-CR603-formZone2_Zone2XmlStatus.xml
+-rw-rw-rw-   0        0        0     1548 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-CR603-formZone3_Zone3XmlStatus.xml
+-rw-rw-rw-   0        0        0     2560 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-RC610-AppCommand.xml
+-rw-rw-rw-   0        0        0    19420 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-RC610-Deviceinfo.xml
+-rw-rw-rw-   0        0        0      644 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-RC610-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0      370 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-RC610-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     1819 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-RC610-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0     3546 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/M-RC610-formTuner_TunerXml.xml
+-rw-rw-rw-   0        0        0     2062 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/NR1604-AppCommand.xml
+-rw-rw-rw-   0        0        0    34805 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/NR1604-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     1595 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/NR1604-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1569 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/NR1604-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     2078 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/NR1604-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0     4009 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/NR1604-formTuner_HdXml.xml
+-rw-rw-rw-   0        0        0     3677 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/NR1604-formTuner_TunerXml.xml
+-rw-rw-rw-   0        0        0     1401 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/NR1604-formZone2_Zone2XmlStatus.xml
+-rw-rw-rw-   0        0        0     1434 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/NR1604-formZone3_Zone3XmlStatus.xml
+-rw-rw-rw-   0        0        0     2449 2020-03-22 22:16:30.000000 denonavr-0.9.9/tests/xml/NR1609-AppCommand-8080.xml
+-rw-rw-rw-   0        0        0    51847 2020-03-19 22:12:53.000000 denonavr-0.9.9/tests/xml/NR1609-Deviceinfo-8080.xml
+-rw-rw-rw-   0        0        0       51 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/SR5008-AppCommand.xml
+-rw-rw-rw-   0        0        0    34418 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/SR5008-Deviceinfo.xml
+-rw-rw-rw-   0        0        0     1330 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/SR5008-formMainZone_MainZoneXml.xml
+-rw-rw-rw-   0        0        0     1603 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/SR5008-formMainZone_MainZoneXmlStatus.xml
+-rw-rw-rw-   0        0        0     1919 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/SR5008-formNetAudio_StatusXml.xml
+-rw-rw-rw-   0        0        0     3919 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/SR5008-formTuner_HdXml.xml
+-rw-rw-rw-   0        0        0     3650 2018-10-07 21:50:33.000000 denonavr-0.9.9/tests/xml/SR5008-formTuner_TunerXml.xml
```

### Comparing `denonavr-0.9.8/PKG-INFO` & `denonavr-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: denonavr
-Version: 0.9.8
+Version: 0.9.9
 Summary: Automation Library for Denon AVR receivers
 Home-page: https://github.com/scarface-4711/denonavr
 Author: Oliver Goetz
 Author-email: scarface@mywoh.de
 License: MIT
 Description: Automation Library for Denon AVR receivers
 Platform: any
```

### Comparing `denonavr-0.9.8/README.rst` & `denonavr-0.9.9/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 denonavr
 ========
 
 .. |Build Status| .. image:: https://travis-ci.com/scarface-4711/denonavr.svg?branch=master
     :target: https://travis-ci.com/scarface-4711/denonavr
 
-Automation Library for Denon AVR receivers - current version 0.9.8
+Automation Library for Denon AVR receivers - current version 0.9.9
 
 Installation
 ------------
 
 Use pip:
 
 ``$ pip install denonavr``
```

### Comparing `denonavr-0.9.8/denonavr/__init__.py` & `denonavr-0.9.9/denonavr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # Import denonavr module
 from .denonavr import DenonAVR
 from . import ssdp
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __title__ = "denonavr"
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 
 def discover():
     """
     Discover all Denon AVR devices in LAN zone.
 
     Returns a list of dictionaries which includes all discovered Denon AVR
```

### Comparing `denonavr-0.9.8/denonavr/audyssey.py` & `denonavr-0.9.9/denonavr/audyssey.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,30 +6,28 @@
 :copyright: (c) 2016 by Oliver Goetz.
 :license: MIT, see LICENSE for more details.
 """
 
 import logging
 from io import BytesIO
 import xml.etree.ElementTree as ET
-from requests.exceptions import RequestException
+from requests.exceptions import RequestException, ConnectTimeout
 
 _LOGGER = logging.getLogger("Audyssey")
 
 MULTI_EQ_MAP = {"0": "Off", "1": "Flat", "2": "L/R Bypass", "3": "Reference"}
-MULTI_EQ_MAP_LABELS = dict((value, key) for key, value in MULTI_EQ_MAP.items())
+MULTI_EQ_MAP_LABELS = {(value, key) for key, value in MULTI_EQ_MAP.items()}
 
 REF_LVL_OFFSET_MAP = {"0": "0dB", "1": "+5dB", "2": "+10dB", "3": "+15dB"}
-REF_LVL_OFFSET_MAP_LABELS = dict(
-    (value, key) for key, value in REF_LVL_OFFSET_MAP.items()
-)
+REF_LVL_OFFSET_MAP_LABELS = {
+    (value, key) for key, value in REF_LVL_OFFSET_MAP.items()}
 
 DYNAMIC_VOLUME_MAP = {"0": "Off", "1": "Light", "2": "Medium", "3": "Heavy"}
-DYNAMIC_VOLUME_MAP_LABELS = dict(
-    (value, key) for key, value in DYNAMIC_VOLUME_MAP.items()
-)
+DYNAMIC_VOLUME_MAP_LABELS = {
+    (value, key) for key, value in DYNAMIC_VOLUME_MAP.items()}
 
 COMMAND_ENDPOINT = "/goform/AppCommand0300.xml"
 
 
 class Audyssey:
     """Audyssey Settings."""
 
@@ -53,15 +51,17 @@
 
     def send_command(self, xml_tree):
         """Send commands."""
         body = BytesIO()
         xml_tree.write(body, encoding="utf-8", xml_declaration=True)
         try:
             result = self.receiver.send_post_command(
-                command=COMMAND_ENDPOINT, body=body.getvalue())
+                COMMAND_ENDPOINT, body.getvalue())
+        except ConnectTimeout:
+            return
         except RequestException:
             _LOGGER.error(
                 "No connection to %s end point on host %s",
                 COMMAND_ENDPOINT, self.receiver.host)
             return
         finally:
             # Buffered XML not needed anymore: close
@@ -77,25 +77,25 @@
         except (ET.ParseError, TypeError):
             _LOGGER.error(
                 "End point %s on host %s returned malformed XML.",
                 COMMAND_ENDPOINT, self.receiver.host)
             return
 
     def update(self):
-        """Update settings."""
+        """Get current Audyssey settings."""
         root = ET.Element("tx")
         cmd = ET.SubElement(root, "cmd", id="3")
         ET.SubElement(cmd, "name").text = "GetAudyssey"
         valid_params = ["dynamiceq", "reflevoffset", "dynamicvol", "multeq"]
         param_list = ET.SubElement(cmd, "list")
         for param in valid_params:
             ET.SubElement(param_list, "param", name=param)
         tree = ET.ElementTree(root)
 
-        response = self.send_command(xml_tree=tree)
+        response = self.send_command(tree)
         if response is None:
             return False
 
         audyssey_params = response.find("./cmd/list")
 
         if audyssey_params is None:
             return False
@@ -119,14 +119,15 @@
             if param.get("control") is not None:
                 setattr(
                     self, "{name}_control".format(name=param.get("name")),
                     bool(int(param.get("control"))))
         return True
 
     def _set_audyssey(self, parameter, value):
+        """Set Audyssey parameter."""
         root = ET.Element("tx")
         cmd = ET.SubElement(root, "cmd", id="3")
         ET.SubElement(cmd, "name").text = "SetAudyssey"
         param_list = ET.SubElement(cmd, "list")
         ET.SubElement(param_list, "param", name=parameter).text = str(value)
         tree = ET.ElementTree(root)
 
@@ -140,39 +141,35 @@
         except AttributeError:
             pass
 
         return False
 
     def dynamiceq_off(self):
         """Turn DynamicEQ off."""
-        if self._set_audyssey(parameter="dynamiceq", value=0) is True:
+        if self._set_audyssey("dynamiceq", 0) is True:
             self.dynamiceq = False
 
     def dynamiceq_on(self):
         """Turn DynamicEQ on."""
-        if self._set_audyssey(parameter="dynamiceq", value=1) is True:
+        if self._set_audyssey("dynamiceq", 1) is True:
             self.dynamiceq = True
 
     def set_multieq(self, setting):
         """Set MultiEQ mode."""
         if self._set_audyssey(
-                parameter="multeq", value=MULTI_EQ_MAP_LABELS.get(setting)
-                ) is True:
+                "multeq", MULTI_EQ_MAP_LABELS.get(setting)) is True:
             self.multeq = setting
 
     def set_reflevoffset(self, setting):
         """Set Reference Level Offset."""
         # Reference level offset can only be used with DynamicEQ
         if self.dynamiceq is True:
             if self._set_audyssey(
-                    parameter="reflevoffset",
-                    value=REF_LVL_OFFSET_MAP_LABELS.get(setting)
+                    "reflevoffset", REF_LVL_OFFSET_MAP_LABELS.get(setting)
                         ) is True:
                 self.reflevoffset = setting
 
     def set_dynamicvol(self, setting):
         """Set Dynamic Volume."""
         if self._set_audyssey(
-                parameter="dynamicvol",
-                value=DYNAMIC_VOLUME_MAP_LABELS.get(setting)
-                ) is True:
+                "dynamicvol", DYNAMIC_VOLUME_MAP_LABELS.get(setting)) is True:
             self.dynamicvol = setting
```

### Comparing `denonavr-0.9.8/denonavr/denonavr.py` & `denonavr-0.9.9/denonavr/denonavr.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from collections import (namedtuple, OrderedDict)
 from io import BytesIO
 import logging
 import time
 import re
 import html
 import xml.etree.ElementTree as ET
-from concurrent.futures import ThreadPoolExecutor
 
 import requests
 
 from .ssdp import evaluate_scpd_xml
 
 from .audyssey import (
     Audyssey,
@@ -74,14 +73,15 @@
      ('VIDEO GAME', ['VIDEO GAME']),
      ('MONO MOVIE', ['MONO MOVIE']),
      ('DIRECT', ['DIRECT']),
      ('PURE DIRECT', ['PURE_DIRECT', 'PURE DIRECT']),
      ('DOLBY DIGITAL', ['DOLBY DIGITAL', 'DOLBY D + DOLBY SURROUND',
                         'DOLBY DIGITAL +', 'STANDARD(DOLBY)', 'DOLBY SURROUND',
                         'DOLBY D + +DOLBY SURROUND', 'NEURAL', 'DOLBY HD',
+                        'DOLBY HD + DOLBY SURROUND',
                         'MULTI IN + NEURAL:X', 'MULTI IN + DOLBY SURROUND',
                         'DOLBY D + NEURAL:X', 'DOLBY DIGITAL + NEURAL:X',
                         'DOLBY DIGITAL + + NEURAL:X', 'DOLBY ATMOS',
                         'DOLBY AUDIO - DOLBY SURROUND', 'DOLBY TRUEHD',
                         'DOLBY AUDIO - DOLBY DIGITAL PLUS',
                         'DOLBY AUDIO - TRUEHD + DSUR',
                         'DOLBY AUDIO - DOLBY TRUEHD',
@@ -296,14 +296,16 @@
         # Timeout for HTTP calls to receiver
         self.timeout = timeout
         # Receiver types could be avr, avr-x, avr-x-2016 after being determined
         self._receiver_type = None
         # Port 80 for avr and avr-x, Port 8080 port avr-x-2016
         self._receiver_port = None
 
+        self._403_error_count = 0
+
         self._support_update_avr_2016 = None
 
         self._show_all_inputs = show_all_inputs
 
         self._manufacturer = None
         self._model_name = None
         self._serial_number = None
@@ -348,28 +350,38 @@
 
     def exec_appcommand_post(self, attribute_list):
         """
         Prepare and execute a HTTP POST call to AppCommand.xml end point.
 
         Returns XML ElementTree on success and None on fail.
         """
-        # Prepare POST XML body for AppCommand.xml
-        post_root = ET.Element("tx")
-
-        for attribute in attribute_list:
-            # Append tags for each attribute
-            item = ET.Element("cmd")
-            item.set("id", "1")
-            item.text = attribute
-            post_root.append(item)
-
         # Buffer XML body as binary IO
         body = BytesIO()
-        post_tree = ET.ElementTree(post_root)
-        post_tree.write(body, encoding="utf-8", xml_declaration=True)
+
+        # Denon AppCommand.xml acts weird. It returns an error when the tx
+        # element consists of more than 5 cmd elements, but it accepts
+        # multiple XML root elements
+        chunks = [attribute_list[i:i+5] for i in range(
+            0, len(attribute_list), 5)]
+
+        for i, chunk in enumerate(chunks):
+            # Prepare POST XML body for AppCommand.xml
+            post_root = ET.Element("tx")
+
+            for attribute in chunk:
+                # Append tags for each attribute
+                item = ET.Element("cmd")
+                item.set("id", "1")
+                item.text = attribute
+                post_root.append(item)
+
+            post_tree = ET.ElementTree(post_root)
+            # XML declaration only for the first chunk
+            post_tree.write(
+                body, encoding="utf-8", xml_declaration=bool(i == 0))
 
         # Query receivers AppCommand.xml
         try:
             res = self.send_post_command(
                 self._urls.appcommand, body.getvalue())
         except requests.exceptions.ConnectTimeout:
             raise
@@ -390,83 +402,105 @@
         finally:
             # Buffered XML not needed anymore: close
             body.close()
 
     def get_status_xml(self, command, suppress_errors=False):
         """Get status XML via HTTP and return it as XML ElementTree."""
         # Get XML structure via HTTP get
+        endpoint = "http://{host}:{port}{command}".format(
+            host=self._host, port=self._receiver_port, command=command)
         # Using a long read timeout because receiver could be quite slow
-        res = requests.get("http://{host}:{port}{command}".format(
-            host=self._host, port=self._receiver_port, command=command),
-                           timeout=(
-                               self.timeout, max(self.timeout, 10)))
+        res = requests.get(
+            endpoint, timeout=(self.timeout, max(self.timeout, 10)))
         # Continue with XML processing only if HTTP status code = 200
         if res.status_code == 200:
             try:
                 # Return XML ElementTree
                 return ET.fromstring(res.text)
             except ET.ParseError as err:
                 if not suppress_errors:
                     _LOGGER.error(
                         "Host %s returned malformed XML for end point %s: %s",
                         self._host, command, err)
                 raise ValueError from err
+        elif res.status_code == 403:
+            self._handle_403_error(endpoint)
+            raise ValueError
         else:
             if not suppress_errors:
-                _LOGGER.error((
+                _LOGGER.error(
                     "Host %s returned HTTP status code %s to GET request at "
-                    "end point %s"), self._host, res.status_code, command)
+                    "end point %s", self._host, res.status_code, command)
             raise ValueError
 
     def send_get_command(self, command):
         """Send command via HTTP get to receiver."""
         # Send commands via HTTP get
+        endpoint = "http://{host}:{port}{command}".format(
+            host=self._host, port=self._receiver_port, command=command)
         # Using a long read timeout because receiver could be quite slow
-        res = requests.get("http://{host}:{port}{command}".format(
-            host=self._host, port=self._receiver_port, command=command),
-                           timeout=(
-                               self.timeout, max(self.timeout, 10)))
+        res = requests.get(
+            endpoint, timeout=(self.timeout, max(self.timeout, 10)))
         if res.status_code == 200:
             return True
+        elif res.status_code == 403:
+            self._handle_403_error(endpoint)
+            return False
         else:
-            _LOGGER.error((
+            _LOGGER.error(
                 "Host %s returned HTTP status code %s to GET command at "
-                "end point %s"), self._host, res.status_code, command)
+                "end point %s", self._host, res.status_code, command)
             return False
 
     def send_post_command(self, command, body):
         """Send command via HTTP post to receiver."""
         # Send commands via HTTP post
+        endpoint = "http://{host}:{port}{command}".format(
+            host=self._host, port=self._receiver_port, command=command)
         # Using a long read timeout because receiver could be quite slow
-        res = requests.post("http://{host}:{port}{command}".format(
-            host=self._host, port=self._receiver_port, command=command),
-                            data=body, timeout=(
-                                self.timeout, max(self.timeout, 10)))
+        res = requests.post(
+            endpoint, data=body, timeout=(self.timeout, max(self.timeout, 10)))
         if res.status_code == 200:
             return res.text
+        elif res.status_code == 403:
+            self._handle_403_error(endpoint)
         else:
-            _LOGGER.error((
+            _LOGGER.error(
                 "Host %s returned HTTP status code %s to POST command at "
-                "end point %s"), self._host, res.status_code, command)
+                "end point %s", self._host, res.status_code, command)
+
+    def _handle_403_error(self, endpoint):
+        """Handle 403 errors during API calls."""
+        self._403_error_count += 1
+        if self._403_error_count == 1:
+            _LOGGER.error(
+                "Endpoint %s responded with a 403 error. Please consider "
+                "power cycling your receiver", endpoint)
+        elif self._403_error_count % 100 == 0:
+            _LOGGER.error(
+                "%s 403 errors occured on your receiver, most recently at "
+                "endpoint %s. Please consider power cycling your receiver",
+                self._403_error_count, endpoint)
+            self._403_error_count = 0
 
     def get_device_info(self):
         """Get device information."""
         url = "http://{host}:{port}{command}".format(
             host=self._host, port=DESCRIPTION_URL[self._receiver_type].port,
             command=DESCRIPTION_URL[self._receiver_type].url)
 
         try:
             device_info = evaluate_scpd_xml(url)
         except requests.exceptions.ConnectTimeout:
             _LOGGER.error("Connection timeout when getting device information")
             return
         except requests.exceptions.RequestException:
-            device_info = False
+            device_info = None
 
-        if device_info is False:
+        if device_info is None:
             self._manufacturer = "Denon"
             self._model_name = "Unknown"
             self._serial_number = None
             _LOGGER.error(
                 "Unable to get device information of host %s, can not "
                 "use the serial number as identification", self._host)
         else:
@@ -485,110 +519,113 @@
 
     def ensure_configuration(self):
         """Ensure that configuration is loaded from receiver."""
         # Determine receiver type and input functions
         if not self._input_func_list:
             self._update_input_func_list()
 
-        # Some queries can be performed in parallel
-        with ThreadPoolExecutor(max_workers=4) as executor:
-            # Determine device info
-            if self.manufacturer is None and self.model_name is None:
-                executor.submit(self.get_device_info)
+        # Determine device info
+        if self.manufacturer is None and self.model_name is None:
+            self.get_device_info()
 
-            if self._receiver_type == AVR_X_2016.type:
-                executor.submit(self._get_receiver_name_avr_2016)
-            else:
-                executor.submit(self._get_receiver_name)
+        if self._receiver_type == AVR_X_2016.type:
+            self._get_receiver_name_avr_2016()
+        else:
+            self._get_receiver_name()
 
-            # Determine if update_avr_2016 can be used for AVR_X receiver
-            support_avr_2016 = None
-            if (self._support_update_avr_2016 is None
-                    and self._receiver_type == AVR_X.type):
-                support_avr_2016 = executor.submit(
-                    self._update_avr_2016, compatibiliy_check=True)
-
-            # Determine if sound mode is supported
-            if self._support_sound_mode is None:
-                executor.submit(self._get_support_sound_mode)
-
-            # Get result of support_avr_2016 check if it was performed
-            if support_avr_2016 is not None:
-                self._support_update_avr_2016 = support_avr_2016.result()
+        # Determine if update_avr_2016 can be used for AVR_X receiver
+        if (self._support_update_avr_2016 is None
+                and self._receiver_type == AVR_X.type):
+            self._support_update_avr_2016 = self._update_avr_2016(
+                compatibiliy_check=True)
+
+        # Determine if sound mode is supported
+        if self._support_sound_mode is None:
+            self._get_support_sound_mode()
 
     def update(self):
         """
         Get the latest status information from device.
 
         Method executes the update method for the current receiver type.
         """
+        support_avr_2016_before = self._support_update_avr_2016
+
+        # Verify that receiver config is initialized
         self.ensure_configuration()
 
+        updated_by_ensure_config = False
+        if support_avr_2016_before is None:
+            if self._support_update_avr_2016 is True:
+                updated_by_ensure_config = True
+
         if self._receiver_type == AVR_X_2016.type:
             return bool(self._update_avr_2016())
         elif self._support_update_avr_2016:
-            if self._update_avr_2016() is not True:
-                _LOGGER.debug(
-                    "Update method (AppCommand.xml) failed for zone %s",
-                    self._zone)
-                return False
+            if updated_by_ensure_config is False:
+                if self._update_avr_2016() is False:
+                    _LOGGER.debug(
+                        "Update method (AppCommand.xml) failed for zone %s",
+                        self._zone)
+                    return False
         else:
             if self._update_avr() is not True:
                 return False
 
         # Media data are only supported on non AVR devices built before 2016
-        return self._set_media_state()
+        success = self._set_media_state()
+
+        return success
+
+    def update_audyssey(self):
+        """Get current Audyssey settings."""
+        self._audyssey.update()
 
     def _update_avr(self):
         """
         Get the latest status information from device.
 
         Method queries device via HTTP and updates instance attributes.
         Returns "True" on success and "False" on fail.
         This method is for pre 2016 AVR(-X) devices
         """
-        # Use ThreadPoolExecutor to call all URLs of this method in parallel
-        executor = ThreadPoolExecutor(max_workers=2)
-
-        status_status = executor.submit(self.get_status_xml, self._urls.status)
-        status_mainzone = executor.submit(
-            self.get_status_xml, self._urls.mainzone)
-
         # Set all tags to be evaluated
         relevant_tags = {"Power": None, "InputFuncSelect": None, "Mute": None,
                          "MasterVolume": None}
 
         # Sound mode information only available in main zone
         if self._zone == MAIN_ZONE and self._support_sound_mode:
             relevant_tags["selectSurround"] = None
             relevant_tags["SurrMode"] = None
 
         # Get status XML from Denon receiver via HTTP
         try:
-            root = status_status.result()
+            root = self.get_status_xml(self._urls.status)
         except requests.exceptions.ConnectTimeout:
             # On connect timeout, the device is probably off
             self._power = POWER_OFF
             self._state = STATE_OFF
+            return False
         except (ValueError, requests.exceptions.RequestException):
             pass
         else:
             # Get the tags from this XML
             relevant_tags = self._get_status_from_xml_tags(root, relevant_tags)
 
         # Second option to update variables from different source
         if relevant_tags and self._power != POWER_OFF:
             _LOGGER.debug(
                 "Update method (Status.xml) failed for zone %s", self._zone)
             try:
-                root = status_mainzone.result()
+                root = self.get_status_xml(self._urls.mainzone)
             except requests.exceptions.ConnectTimeout:
                 # On connect timeout, the device is probably off
                 self._power = POWER_OFF
                 self._state = STATE_OFF
+                return False
             except (ValueError, requests.exceptions.RequestException):
                 pass
             else:
                 # Get the tags from this XML
                 relevant_tags = self._get_status_from_xml_tags(
                     root, relevant_tags)
 
@@ -606,139 +643,127 @@
                 _LOGGER.info("List of input functions refreshed.")
                 # If input function is still not known, log error.
                 if (self._input_func not in self._input_func_list and
                         self._input_func is not None):
                     _LOGGER.error(
                         "Input function %s is not known", self._input_func)
             else:
-                _LOGGER.error((
+                _LOGGER.error(
                     "Input function list for Denon receiver at host %s "
-                    "could not be updated."), self._host)
+                    "could not be updated.", self._host)
 
         # Finished
-        executor.shutdown(wait=False)
         return True
 
     def _update_avr_2016(self, compatibiliy_check=False):
         """
         Get the latest status information from device.
 
         Method queries device via HTTP and updates instance attributes.
         Returns "True" on success and "False" on fail.
         This method is for AVR-X devices built in 2016 and later.
         """
-        # Use ThreadPoolExecutor to call all URLs of this method in parallel
-        with ThreadPoolExecutor(max_workers=3) as executor:
+        success = True
+        # Collect tags for AppCommand.xml call
+        tags = ["GetAllZonePowerStatus", "GetAllZoneSource",
+                "GetAllZoneVolume", "GetAllZoneMuteStatus",
+                "GetSurroundModeStatus", "GetToneControl"]
 
-            success = True
-            # Collect tags for AppCommand.xml call
-            tags = ["GetAllZonePowerStatus", "GetAllZoneSource",
-                    "GetAllZoneVolume", "GetAllZoneMuteStatus",
-                    "GetSurroundModeStatus"]
-            # Execute call
-            app_command = executor.submit(self.exec_appcommand_post, tags)
+        # Execute call
+        try:
+            root = self.exec_appcommand_post(tags)
+        except requests.exceptions.ConnectTimeout:
+            if compatibiliy_check is True:
+                return None
+            # Assume device is off on connect timeout
+            self._power = POWER_OFF
+            self._state = STATE_OFF
+            return False
+        # Check result
+        if root is None:
+            if compatibiliy_check is False:
+                _LOGGER.error("Update failed.")
+            return False
 
-            # Update tone control
-            executor.submit(self._update_tone_control)
+        # Extract relevant information
+        zone = self._get_own_zone()
 
-            # Update Audyssey
-            executor.submit(self._audyssey.update())
+        try:
+            self._power = root[0].find(zone).text
+        except (AttributeError, IndexError):
+            if compatibiliy_check is False:
+                _LOGGER.error("No PowerStatus found for zone %s", self.zone)
+            success = False
 
-            try:
-                root = app_command.result()
-            except requests.exceptions.ConnectTimeout:
-                if compatibiliy_check is True:
-                    return None
-                # Assume device is off on connect timeout
-                self._power = POWER_OFF
-                self._state = STATE_OFF
-                return False
-            # Check result
-            if root is None:
-                if compatibiliy_check is False:
-                    _LOGGER.error("Update failed.")
-                return False
+        try:
+            self._mute = root[3].find(zone).text
+        except (AttributeError, IndexError):
+            if compatibiliy_check is False:
+                _LOGGER.error("No MuteStatus found for zone %s", self.zone)
+            success = False
 
-            # Extract relevant information
-            zone = self._get_own_zone()
+        try:
+            self._volume = root.find(
+                "./cmd/{zone}/volume".format(zone=zone)).text
+        except AttributeError:
+            if compatibiliy_check is False:
+                _LOGGER.error("No VolumeStatus found for zone %s", self.zone)
+            success = False
 
+        try:
+            inputfunc = root.find(
+                "./cmd/{zone}/source".format(zone=zone)).text
+        except AttributeError:
+            if compatibiliy_check is False:
+                _LOGGER.error("No Source found for zone %s", self.zone)
+            success = False
+        else:
+            # AirPlay and Internet Radio are not always listed in
+            # available sources
+            if inputfunc in ["AirPlay", "Internet Radio"]:
+                if inputfunc not in self._input_func_list:
+                    self._input_func_list[inputfunc] = inputfunc
+                    self._input_func_list_rev[inputfunc] = inputfunc
             try:
-                self._power = root[0].find(zone).text
-            except (AttributeError, IndexError):
-                if compatibiliy_check is False:
+                self._input_func = self._input_func_list_rev[inputfunc]
+            except KeyError:
+                self._input_func = inputfunc
+                # Update sources list if current source is not known yet
+                _LOGGER.info("No mapping for source %s found", inputfunc)
+                if self._update_input_func_list():
+                    _LOGGER.info("List of input functions refreshed.")
+                    # If input function is still not known, log error.
+                    if (inputfunc not in self._input_func_list and
+                            inputfunc is not None):
+                        _LOGGER.error(
+                            "Input function %s is not known", self._input_func)
+                else:
                     _LOGGER.error(
-                        "No PowerStatus found for zone %s", self.zone)
-                success = False
+                        "Input function list for Denon receiver at "
+                        "host %s could not be updated.", self._host)
+        try:
+            self._sound_mode_raw = root[4][0].text.rstrip()
+        except (AttributeError, IndexError):
+            if compatibiliy_check is False:
+                _LOGGER.error(
+                    "No SoundMode found for the main zone %s", self.zone)
+            success = False
 
-            try:
-                self._mute = root[3].find(zone).text
-            except (AttributeError, IndexError):
-                if compatibiliy_check is False:
-                    _LOGGER.error("No MuteStatus found for zone %s", self.zone)
-                success = False
+        # Now playing information is not implemented for 2016+ models, as
+        # a HEOS API query needed. So only sync the power state for now.
+        if self._receiver_type == AVR_X_2016.type:
+            if self._power == POWER_ON:
+                self._state = STATE_ON
+            else:
+                self._state = STATE_OFF
 
-            try:
-                self._volume = root.find(
-                    "./cmd/{zone}/volume".format(zone=zone)).text
-            except AttributeError:
-                if compatibiliy_check is False:
-                    _LOGGER.error(
-                        "No VolumeStatus found for zone %s", self.zone)
-                success = False
+        # Update tone control
+        self._update_tone_control(root)
 
-            try:
-                inputfunc = root.find(
-                    "./cmd/{zone}/source".format(zone=zone)).text
-            except AttributeError:
-                if compatibiliy_check is False:
-                    _LOGGER.error("No Source found for zone %s", self.zone)
-                success = False
-            else:
-                # AirPlay and Internet Radio are not always listed in
-                # available sources
-                if inputfunc in ["AirPlay", "Internet Radio"]:
-                    if inputfunc not in self._input_func_list:
-                        self._input_func_list[inputfunc] = inputfunc
-                        self._input_func_list_rev[inputfunc] = inputfunc
-                try:
-                    self._input_func = self._input_func_list_rev[inputfunc]
-                except KeyError:
-                    self._input_func = inputfunc
-                    # Update sources list if current source is not known yet
-                    _LOGGER.info(
-                        "No mapping for source %s found", inputfunc)
-                    if self._update_input_func_list():
-                        _LOGGER.info("List of input functions refreshed.")
-                        # If input function is still not known, log error.
-                        if (inputfunc not in self._input_func_list and
-                                inputfunc is not None):
-                            _LOGGER.error(
-                                "Input function %s is not known",
-                                self._input_func)
-                    else:
-                        _LOGGER.error((
-                            "Input function list for Denon receiver at "
-                            "host %s could not be updated."), self._host)
-            try:
-                self._sound_mode_raw = root[4][0].text.rstrip()
-            except (AttributeError, IndexError):
-                if compatibiliy_check is False:
-                    _LOGGER.error(
-                        "No SoundMode found for the main zone %s", self.zone
-                    )
-                success = False
-
-            # Now playing information is not implemented for 2016+ models, as
-            # a HEOS API query needed. So only sync the power state for now.
-            if self._receiver_type == AVR_X_2016.type:
-                if self._power == POWER_ON:
-                    self._state = STATE_ON
-                else:
-                    self._state = STATE_OFF
-            return success
+        return success
 
     def _update_input_func_list(self):
         """
         Update sources list from receiver.
 
         Internal method which updates sources list of receiver after getting
         sources and potential renaming information from receiver.
@@ -754,15 +779,15 @@
 
         # First input_func_list determination of AVR-X receivers
         if self._receiver_type in [AVR_X.type, AVR_X_2016.type]:
             renamed_sources, deleted_sources, status_success = (
                 self._get_renamed_deleted_sourcesapp())
 
             # Backup if previous try with AppCommand was not successful
-            if not status_success:
+            if status_success is False:
                 renamed_sources, deleted_sources = (
                     self._get_renamed_deleted_sources())
 
             # Remove all deleted sources
             if self._show_all_inputs is False:
                 for deleted_source in deleted_sources.items():
                     if deleted_source[1] == "DEL":
@@ -878,20 +903,21 @@
         Method executes the method for the current receiver type.
         """
         if self._receiver_type == AVR_X_2016.type:
             return self._get_support_sound_mode_avr_2016()
         else:
             return self._get_support_sound_mode_avr()
 
-    def _update_tone_control(self):
+    def _update_tone_control(self, root=None):
         """Update tone control related things."""
-        try:
-            root = self.exec_appcommand_post(attribute_list=['GetToneControl'])
-        except requests.exceptions.ConnectTimeout:
-            root = None
+        if root is None:
+            try:
+                root = self.exec_appcommand_post(["GetToneControl"])
+            except requests.exceptions.ConnectTimeout:
+                root = None
 
         if root is None:
             _LOGGER.error("Getting tone control failed.")
             return False
 
         try:
             self._tone_control_status = bool(int(root[0].find('status').text))
@@ -923,50 +949,41 @@
         """
         Get if sound mode is supported from device.
 
         Method queries device via HTTP.
         Returns "True" if sound mode supported and "False" if not.
         This method is for pre 2016 AVR(-X) devices
         """
-        # Use ThreadPoolExecutor to call all URLs of this method in parallel
-        executor = ThreadPoolExecutor(max_workers=2)
-        status_status = executor.submit(self.get_status_xml, self._urls.status)
-        status_mainzone = executor.submit(
-            self.get_status_xml, self._urls.mainzone)
-
         # Set sound mode tags to be checked if available
         relevant_tags = {"selectSurround": None, "SurrMode": None}
 
         # Get status XML from Denon receiver via HTTP
         try:
-            root = status_status.result()
+            root = self.get_status_xml(self._urls.status)
         except requests.exceptions.ConnectTimeout:
             return None
         except (ValueError, requests.exceptions.RequestException):
             pass
         else:
             # Process the tags from this XML
             relevant_tags = self._get_status_from_xml_tags(root, relevant_tags)
 
         # Second option to update variables from different source
         if relevant_tags:
             try:
-                root = status_mainzone.result()
+                root = self.get_status_xml(self._urls.mainzone)
             except requests.exceptions.ConnectTimeout:
                 return None
             except (ValueError, requests.exceptions.RequestException):
                 pass
             else:
                 # Get the tags from this XML
                 relevant_tags = self._get_status_from_xml_tags(root,
                                                                relevant_tags)
 
-        # Shutdown ThreadPoolExecutor
-        executor.shutdown(wait=False)
-
         # if sound mode not found in the status XML, return False
         if relevant_tags:
             self._support_sound_mode = False
             return False
         # if sound mode found, the relevant_tags are empty: return True.
         self._support_sound_mode = True
         return True
@@ -1078,15 +1095,15 @@
 
         # Collect tags for AppCommand.xml call
         tags = ["GetRenameSource", "GetDeletedSource"]
         # Execute call
         try:
             root = self.exec_appcommand_post(tags)
         except requests.exceptions.ConnectTimeout:
-            root = None
+            return (renamed_sources, deleted_sources, None)
         # Check result
         if root is None:
             _LOGGER.error("Getting renamed and deleted sources failed.")
             return (renamed_sources, deleted_sources, False)
 
         # Detect "Document Error: Data follows" title if URL does not exist
         document_error = root.find("./head/title")
@@ -1127,40 +1144,40 @@
             self._receiver_port = port
 
             # This XML is needed to get the sources of the receiver
             try:
                 root = self.get_status_xml(self._urls.deviceinfo,
                                            suppress_errors=True)
             except (ValueError, requests.exceptions.RequestException):
-                self._receiver_type = None
+                continue
             else:
                 # First test by CommApiVers
                 try:
                     if bool(DEVICEINFO_COMMAPI_PATTERN.search(
                             root.find("CommApiVers").text) is not None):
                         self._receiver_type = r_type
                         # receiver found break the loop
                         break
                 except AttributeError:
                     # AttributeError occurs when ModelName tag is not found.
                     # In this case there is no AVR-X device
-                    self._receiver_type = None
+                    continue
 
                 # if first test did not find AVR-X device, check by model name
                 if self._receiver_type is None:
                     try:
                         if bool(DEVICEINFO_AVR_X_PATTERN.search(
                                 root.find("ModelName").text) is not None):
                             self._receiver_type = r_type
                             # receiver found break the loop
                             break
                     except AttributeError:
                         # AttributeError occurs when ModelName tag is not found
                         # In this case there is no AVR-X device
-                        self._receiver_type = None
+                        continue
 
         # Set ports and update method
         if self._receiver_type is None:
             self._receiver_type = AVR.type
             self._receiver_port = AVR.port
         elif self._receiver_type == AVR_X_2016.type:
             self._receiver_port = AVR_X_2016.port
@@ -1173,15 +1190,15 @@
         # Not an AVR-X device, start determination of sources
         if self._receiver_type == AVR.type:
             # Sources list is equal to list of renamed sources.
             non_x_sources, deleted_non_x_sources, status_success = (
                 self._get_renamed_deleted_sourcesapp())
 
             # Backup if previous try with AppCommand was not successful
-            if not status_success:
+            if status_success is False:
                 non_x_sources, deleted_non_x_sources = (
                     self._get_renamed_deleted_sources())
 
             # Remove all deleted sources
             if self._show_all_inputs is False:
                 for deleted_source in deleted_non_x_sources.items():
                     if deleted_source[1] == "DEL":
@@ -2050,17 +2067,15 @@
         ET.SubElement(root, parameter_type).text = str(value)
         tree = ET.ElementTree(root)
 
         body = BytesIO()
         tree.write(body, encoding="utf-8", xml_declaration=True)
 
         try:
-            self.send_post_command(
-                command=self._urls.appcommand, body=body.getvalue()
-                )
+            self.send_post_command(self._urls.appcommand, body.getvalue())
         except requests.exceptions.RequestException:
             _LOGGER.error("No connection to %s end point on host %s",
                           self._urls.appcommand, self._host)
             return False
         finally:
             # Buffered XML not needed anymore: close
             body.close()
@@ -2069,86 +2084,70 @@
     def enable_tone_control(self):
         """Enable tone control to change settings like bass or treble."""
         if self._tone_control_status is False:
             return False
 
         if self._tone_control_adjust is True:
             return True
-        elif self._set_tone_control_command(parameter_type='adjust', value=1):
+        elif self._set_tone_control_command('adjust', 1):
             self._tone_control_adjust = True
             return True
         return False
 
     def disable_tone_control(self):
         """Disable tone control to change settings like bass or treble."""
         if self._tone_control_status is False:
             return False
 
         if self._tone_control_adjust is False:
             return True
-        elif self._set_tone_control_command(parameter_type='adjust', value=0):
+        elif self._set_tone_control_command('adjust', 0):
             self._tone_control_adjust = False
             return True
         return False
 
     def _set_tone_control(self, parameter_type, value):
         """Set tone control parameter."""
         if value < 0 or value > 12:
-            raise ValueError(
-                "Invalid value for {parameter_type}".format(
-                    parameter_type=parameter_type
-                    )
-            )
+            raise ValueError("Invalid value for {}".format(parameter_type))
 
         if not self.enable_tone_control():
             return False
 
         if self._set_tone_control_command(
-                parameter_type='{parameter_type}value'.format(
-                    parameter_type=parameter_type
-                    ), value=value
-                ):
-            setattr(
-                self,
-                '_{parameter_type}'.format(parameter_type=parameter_type),
-                value
-                )
+                '{}value'.format(parameter_type), value):
+            setattr(self, '_{}'.format(parameter_type), value)
             setattr(
-                self,
-                '_{parameter_type}_level'.format(
-                    parameter_type=parameter_type
-                    ),
+                self, '_{}_level'.format(parameter_type),
                 '{value:{sign}}dB'.format(
-                    value=value-6, sign='' if value-6 == 0 else '+'
-                    )
-                )
+                    value=value-6, sign='' if value-6 == 0 else '+'))
             return True
         return False
 
     def set_bass(self, bass):
         """
         Set receiver bass.
 
         Minimum is 0, maximum at 12
 
         Note:
         Doesn't work, if Dynamic Equalizer is active.
         """
-        return self._set_tone_control(parameter_type='bass', value=bass)
+        return self._set_tone_control('bass', bass)
 
     def set_treble(self, treble):
         """
         Set receiver treble.
 
         Minimum is 0, maximum at 12
 
         Note:
         Doesn't work, if Dynamic Equalizer is active.
         """
-        return self._set_tone_control(parameter_type='treble', value=treble)
+        return self._set_tone_control('treble', treble)
 
 
 class DenonAVRZones(DenonAVR):
     """Representing an additional zone of a Denon AVR Device."""
 
     def __init__(self, parent_avr, zone, name):
         """
```

### Comparing `denonavr-0.9.8/denonavr/ssdp.py` & `denonavr-0.9.9/denonavr/ssdp.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,27 +78,22 @@
     devices with keys "host", "modelName", "friendlyName", "presentationURL".
     """
     # Sending SSDP broadcast message to get resource urls from devices
     urls = send_ssdp_broadcast()
 
     # Check which responding device is a DenonAVR device and prepare output
     receivers = []
-    futures = []
 
-    with ThreadPoolExecutor() as executor:
-        for url in urls:
-            futures.append(executor.submit(evaluate_scpd_xml, url))
-
-        for future in futures:
-            try:
-                receiver = future.result()
-            except requests.exceptions.RequestException:
-                continue
-            if receiver is not None:
-                receivers.append(receiver)
+    for url in urls:
+        try:
+            receiver = evaluate_scpd_xml(url)
+        except requests.exceptions.RequestException:
+            continue
+        if receiver is not None:
+            receivers.append(receiver)
 
     return receivers
 
 
 def send_ssdp_broadcast():
     """
     Send SSDP broadcast messages to discover UPnP devices.
```

### Comparing `denonavr-0.9.8/denonavr.egg-info/PKG-INFO` & `denonavr-0.9.9/denonavr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: denonavr
-Version: 0.9.8
+Version: 0.9.9
 Summary: Automation Library for Denon AVR receivers
 Home-page: https://github.com/scarface-4711/denonavr
 Author: Oliver Goetz
 Author-email: scarface@mywoh.de
 License: MIT
 Description: Automation Library for Denon AVR receivers
 Platform: any
```

### Comparing `denonavr-0.9.8/denonavr.egg-info/SOURCES.txt` & `denonavr-0.9.9/denonavr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/setup.py` & `denonavr-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 """Automation Library for Denon AVR receivers."""
 from setuptools import find_packages, setup
 
 setup(name='denonavr',
-      version='0.9.8',
+      version='0.9.9',
       description='Automation Library for Denon AVR receivers',
       long_description='Automation Library for Denon AVR receivers',
       url='https://github.com/scarface-4711/denonavr',
       author='Oliver Goetz',
       author_email='scarface@mywoh.de',
       license='MIT',
       packages=find_packages(),
```

### Comparing `denonavr-0.9.8/tests/test_denonavr.py` & `denonavr-0.9.9/tests/test_denonavr.py`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/test_ssdp.py` & `denonavr-0.9.9/tests/test_ssdp.py`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVC-8500H-AppCommand-8080.xml` & `denonavr-0.9.9/tests/xml/AVC-8500H-AppCommand-8080.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVC-8500H-Deviceinfo-8080.xml` & `denonavr-0.9.9/tests/xml/AVC-8500H-Deviceinfo-8080.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-1912-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/AVR-1912-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-1912-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-1912-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-1912-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/AVR-1912-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-2312CI-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/AVR-2312CI-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-2312CI-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-2312CI-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-2312CI-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/AVR-2312CI-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-3311CI-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/AVR-3311CI-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-3311CI-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-3311CI-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-3311CI-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/AVR-3311CI-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-3312-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/AVR-3312-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-3312-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-3312-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-3312-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/AVR-3312-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-3312-formTuner_HdXml.xml` & `denonavr-0.9.9/tests/xml/AVR-3312-formTuner_HdXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-3312-formTuner_TunerXml.xml` & `denonavr-0.9.9/tests/xml/AVR-3312-formTuner_TunerXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-3312-formZone2_Zone2XmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-3312-formZone2_Zone2XmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-3312-formZone3_Zone3XmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-3312-formZone3_Zone3XmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-4810-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/AVR-4810-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-4810-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/AVR-4810-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-4810-formTuner_HdXml.xml` & `denonavr-0.9.9/tests/xml/AVR-4810-formTuner_HdXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-4810-formTuner_TunerXml.xml` & `denonavr-0.9.9/tests/xml/AVR-4810-formTuner_TunerXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X1100W-AppCommand.xml` & `denonavr-0.9.9/tests/xml/AVR-X1100W-AppCommand.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X1100W-Deviceinfo.xml` & `denonavr-0.9.9/tests/xml/AVR-X1100W-Deviceinfo.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X1100W-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X1100W-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X1100W-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-X1100W-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X1100W-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X1100W-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X1100W-formTuner_HdXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X1100W-formTuner_HdXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X1100W-formTuner_TunerXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X1100W-formTuner_TunerXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X1100W-formZone2_Zone2XmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-X1100W-formZone2_Zone2XmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X1100W-formZone3_Zone3XmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-X1100W-formZone3_Zone3XmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X1600H_upnp.xml` & `denonavr-0.9.9/tests/xml/AVR-X1600H_upnp.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-2-Deviceinfo.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-2-Deviceinfo.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-2-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-2-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-2-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-2-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-2-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-2-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-AppCommand.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-AppCommand.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-Deviceinfo.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-Deviceinfo.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-formTuner_HdXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-formTuner_HdXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-formTuner_TunerXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-formTuner_TunerXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-formZone2_Zone2XmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-formZone2_Zone2XmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2000-formZone3_Zone3XmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-X2000-formZone3_Zone3XmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2100W-2-AppCommand.xml` & `denonavr-0.9.9/tests/xml/AVR-X2100W-2-AppCommand.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2100W-2-Deviceinfo.xml` & `denonavr-0.9.9/tests/xml/AVR-X2100W-2-Deviceinfo.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2100W-2-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X2100W-2-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2100W-2-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-X2100W-2-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2100W-2-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X2100W-2-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2100W-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X2100W-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2100W-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-X2100W-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X2100W-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X2100W-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X4100W-AppCommand.xml` & `denonavr-0.9.9/tests/xml/AVR-X4100W-AppCommand.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X4100W-Deviceinfo.xml` & `denonavr-0.9.9/tests/xml/AVR-X4100W-Deviceinfo.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X4100W-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X4100W-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X4100W-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/AVR-X4100W-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X4100W-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/AVR-X4100W-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X4300H-AppCommand-8080.xml` & `denonavr-0.9.9/tests/xml/AVR-X4300H-AppCommand-8080.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/AVR-X4300H-Deviceinfo-8080.xml` & `denonavr-0.9.9/tests/xml/AVR-X4300H-Deviceinfo-8080.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-CR603-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/M-CR603-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-CR603-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/M-CR603-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-CR603-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/M-CR603-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-CR603-formTuner_HdXml.xml` & `denonavr-0.9.9/tests/xml/M-CR603-formTuner_HdXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-CR603-formTuner_TunerXml.xml` & `denonavr-0.9.9/tests/xml/M-CR603-formTuner_TunerXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-CR603-formZone2_Zone2XmlStatus.xml` & `denonavr-0.9.9/tests/xml/M-CR603-formZone2_Zone2XmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-CR603-formZone3_Zone3XmlStatus.xml` & `denonavr-0.9.9/tests/xml/M-CR603-formZone3_Zone3XmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-RC610-AppCommand.xml` & `denonavr-0.9.9/tests/xml/M-RC610-AppCommand.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-RC610-Deviceinfo.xml` & `denonavr-0.9.9/tests/xml/M-RC610-Deviceinfo.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-RC610-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/M-RC610-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-RC610-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/M-RC610-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/M-RC610-formTuner_TunerXml.xml` & `denonavr-0.9.9/tests/xml/M-RC610-formTuner_TunerXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/NR1604-AppCommand.xml` & `denonavr-0.9.9/tests/xml/NR1604-AppCommand.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/NR1604-Deviceinfo.xml` & `denonavr-0.9.9/tests/xml/NR1604-Deviceinfo.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/NR1604-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/NR1604-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/NR1604-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/NR1604-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/NR1604-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/NR1604-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/NR1604-formTuner_HdXml.xml` & `denonavr-0.9.9/tests/xml/NR1604-formTuner_HdXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/NR1604-formTuner_TunerXml.xml` & `denonavr-0.9.9/tests/xml/NR1604-formTuner_TunerXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/NR1604-formZone2_Zone2XmlStatus.xml` & `denonavr-0.9.9/tests/xml/NR1604-formZone2_Zone2XmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/NR1604-formZone3_Zone3XmlStatus.xml` & `denonavr-0.9.9/tests/xml/NR1604-formZone3_Zone3XmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/NR1609-AppCommand-8080.xml` & `denonavr-0.9.9/tests/xml/NR1609-AppCommand-8080.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/NR1609-Deviceinfo-8080.xml` & `denonavr-0.9.9/tests/xml/NR1609-Deviceinfo-8080.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/SR5008-Deviceinfo.xml` & `denonavr-0.9.9/tests/xml/SR5008-Deviceinfo.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/SR5008-formMainZone_MainZoneXml.xml` & `denonavr-0.9.9/tests/xml/SR5008-formMainZone_MainZoneXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/SR5008-formMainZone_MainZoneXmlStatus.xml` & `denonavr-0.9.9/tests/xml/SR5008-formMainZone_MainZoneXmlStatus.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/SR5008-formNetAudio_StatusXml.xml` & `denonavr-0.9.9/tests/xml/SR5008-formNetAudio_StatusXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/SR5008-formTuner_HdXml.xml` & `denonavr-0.9.9/tests/xml/SR5008-formTuner_HdXml.xml`

 * *Files identical despite different names*

### Comparing `denonavr-0.9.8/tests/xml/SR5008-formTuner_TunerXml.xml` & `denonavr-0.9.9/tests/xml/SR5008-formTuner_TunerXml.xml`

 * *Files identical despite different names*

