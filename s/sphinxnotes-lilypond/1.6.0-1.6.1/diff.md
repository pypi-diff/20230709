# Comparing `tmp/sphinxnotes-lilypond-1.6.0.tar.gz` & `tmp/sphinxnotes-lilypond-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxnotes-lilypond-1.6.0.tar", last modified: Fri Oct  7 16:06:59 2022, max compression
+gzip compressed data, was "sphinxnotes-lilypond-1.6.1.tar", last modified: Sun Jul  9 15:45:54 2023, max compression
```

## Comparing `sphinxnotes-lilypond-1.6.0.tar` & `sphinxnotes-lilypond-1.6.1.tar`

### file list

```diff
@@ -1,21 +1,89 @@
-drwxr-xr-x   0 la        (1000) la        (1000)        0 2022-10-07 16:06:59.808105 sphinxnotes-lilypond-1.6.0/
--rw-r--r--   0 la        (1000) la        (1000)     1520 2020-11-18 10:59:13.000000 sphinxnotes-lilypond-1.6.0/LICENSE
--rw-r--r--   0 la        (1000) la        (1000)       76 2020-12-02 00:32:40.000000 sphinxnotes-lilypond-1.6.0/MANIFEST.in
--rw-r--r--   0 la        (1000) la        (1000)      990 2022-10-07 16:06:59.808105 sphinxnotes-lilypond-1.6.0/PKG-INFO
--rw-r--r--   0 la        (1000) la        (1000)      167 2021-12-18 09:27:51.000000 sphinxnotes-lilypond-1.6.0/README.rst
--rw-r--r--   0 la        (1000) la        (1000)       38 2022-10-07 16:06:59.808105 sphinxnotes-lilypond-1.6.0/setup.cfg
--rw-r--r--   0 la        (1000) la        (1000)     1316 2021-08-12 04:00:47.000000 sphinxnotes-lilypond-1.6.0/setup.py
-drwxr-xr-x   0 la        (1000) la        (1000)        0 2022-10-07 16:06:59.808105 sphinxnotes-lilypond-1.6.0/sphinxnotes/
--rw-r--r--   0 la        (1000) la        (1000)      413 2020-12-27 02:06:20.000000 sphinxnotes-lilypond-1.6.0/sphinxnotes/__init__.py
-drwxr-xr-x   0 la        (1000) la        (1000)        0 2022-10-07 16:06:59.808105 sphinxnotes-lilypond-1.6.0/sphinxnotes/lilypond/
--rw-r--r--   0 la        (1000) la        (1000)    14162 2022-10-07 16:06:48.000000 sphinxnotes-lilypond-1.6.0/sphinxnotes/lilypond/__init__.py
--rw-r--r--   0 la        (1000) la        (1000)    46517 2022-07-21 04:53:28.000000 sphinxnotes-lilypond-1.6.0/sphinxnotes/lilypond/jianpu.py
--rw-r--r--   0 la        (1000) la        (1000)    14085 2022-07-21 04:51:01.000000 sphinxnotes-lilypond-1.6.0/sphinxnotes/lilypond/lilypond.py
-drwxr-xr-x   0 la        (1000) la        (1000)        0 2022-10-07 16:06:59.808105 sphinxnotes-lilypond-1.6.0/sphinxnotes_lilypond.egg-info/
--rw-r--r--   0 la        (1000) la        (1000)      990 2022-10-07 16:06:59.000000 sphinxnotes-lilypond-1.6.0/sphinxnotes_lilypond.egg-info/PKG-INFO
--rw-r--r--   0 la        (1000) la        (1000)      475 2022-10-07 16:06:59.000000 sphinxnotes-lilypond-1.6.0/sphinxnotes_lilypond.egg-info/SOURCES.txt
--rw-r--r--   0 la        (1000) la        (1000)        1 2022-10-07 16:06:59.000000 sphinxnotes-lilypond-1.6.0/sphinxnotes_lilypond.egg-info/dependency_links.txt
--rw-r--r--   0 la        (1000) la        (1000)       12 2022-10-07 16:06:59.000000 sphinxnotes-lilypond-1.6.0/sphinxnotes_lilypond.egg-info/namespace_packages.txt
--rw-r--r--   0 la        (1000) la        (1000)        1 2022-10-07 16:06:59.000000 sphinxnotes-lilypond-1.6.0/sphinxnotes_lilypond.egg-info/not-zip-safe
--rw-r--r--   0 la        (1000) la        (1000)       27 2022-10-07 16:06:59.000000 sphinxnotes-lilypond-1.6.0/sphinxnotes_lilypond.egg-info/requires.txt
--rw-r--r--   0 la        (1000) la        (1000)       12 2022-10-07 16:06:59.000000 sphinxnotes-lilypond-1.6.0/sphinxnotes_lilypond.egg-info/top_level.txt
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.576452 sphinxnotes-lilypond-1.6.1/
+-rw-r--r--   0 la        (1000) la        (1000)      734 2023-07-09 15:42:23.000000 sphinxnotes-lilypond-1.6.1/.cruft.json
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.569785 sphinxnotes-lilypond-1.6.1/.github/
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/.github/workflows/
+-rw-r--r--   0 la        (1000) la        (1000)      916 2023-06-27 15:31:18.000000 sphinxnotes-lilypond-1.6.1/.github/workflows/pages.yml
+-rw-r--r--   0 la        (1000) la        (1000)     1844 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/.gitignore
+-rw-r--r--   0 la        (1000) la        (1000)       88 2022-07-23 04:50:54.000000 sphinxnotes-lilypond-1.6.1/.gitmodules
+-rw-r--r--   0 la        (1000) la        (1000)     1520 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/LICENSE
+-rw-r--r--   0 la        (1000) la        (1000)      321 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/MANIFEST.in
+-rw-r--r--   0 la        (1000) la        (1000)      695 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/Makefile
+-rw-r--r--   0 la        (1000) la        (1000)     2280 2023-07-09 15:45:54.576452 sphinxnotes-lilypond-1.6.1/PKG-INFO
+-rw-r--r--   0 la        (1000) la        (1000)     1187 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/README.rst
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/
+-rw-r--r--   0 la        (1000) la        (1000)      730 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/Makefile
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.569785 sphinxnotes-lilypond-1.6.1/docs/_build/
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/0f1664a0a4703885d6c2c934900afc0ed8d9fa66/
+-rw-r--r--   0 la        (1000) la        (1000)    21392 2023-05-27 06:35:53.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/0f1664a0a4703885d6c2c934900afc0ed8d9fa66/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/17829479ac37b22588bccd631c8620bf824820b8/
+-rw-r--r--   0 la        (1000) la        (1000)    58392 2023-05-27 06:36:03.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/17829479ac37b22588bccd631c8620bf824820b8/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/1cb9f6ab10e20409e021de2f1ebfe0580953b13b/
+-rw-r--r--   0 la        (1000) la        (1000)     5486 2023-05-27 06:36:04.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/1cb9f6ab10e20409e021de2f1ebfe0580953b13b/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/551c80c9c81224483473482212a8e0cc28676c46/
+-rw-r--r--   0 la        (1000) la        (1000)    10826 2023-05-27 06:35:55.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/551c80c9c81224483473482212a8e0cc28676c46/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/5a00cd884253094c331991549f1bd46424f7d974/
+-rw-r--r--   0 la        (1000) la        (1000)    47977 2023-05-27 06:36:10.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/5a00cd884253094c331991549f1bd46424f7d974/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/6417635af1b60a22af8203dfaa0aa6f3825c6c5b/
+-rw-r--r--   0 la        (1000) la        (1000)    10040 2023-05-27 09:12:03.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/6417635af1b60a22af8203dfaa0aa6f3825c6c5b/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/7ef0252b99ff78945b448bd92460207b4f6af48c/
+-rw-r--r--   0 la        (1000) la        (1000)    10826 2023-05-27 06:36:02.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/7ef0252b99ff78945b448bd92460207b4f6af48c/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/8e738aa934a92540ad8efb31a6118c628ed06ff0/
+-rw-r--r--   0 la        (1000) la        (1000)    10826 2023-05-27 06:35:54.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/8e738aa934a92540ad8efb31a6118c628ed06ff0/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/cb9df2873e988fa19bfe45733c0bc55cb3084837/
+-rw-r--r--   0 la        (1000) la        (1000)    19174 2023-05-27 06:36:07.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/cb9df2873e988fa19bfe45733c0bc55cb3084837/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/cd75395f4fccebb4a570014ba73887037127ae98/
+-rw-r--r--   0 la        (1000) la        (1000)    10997 2023-05-27 06:35:56.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/cd75395f4fccebb4a570014ba73887037127ae98/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/d8fe038db7a667225b986a7987f97bc027b8f80f/
+-rw-r--r--   0 la        (1000) la        (1000)    10826 2023-05-27 06:36:01.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/d8fe038db7a667225b986a7987f97bc027b8f80f/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/e2f7e5d18080cd088d6653d5afeaad94d106e5ce/
+-rw-r--r--   0 la        (1000) la        (1000)     5486 2023-05-27 09:26:33.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/e2f7e5d18080cd088d6653d5afeaad94d106e5ce/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/f999d8211b328f05198e4b376a655dfdef02640d/
+-rw-r--r--   0 la        (1000) la        (1000)   132749 2023-05-27 06:36:00.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/f999d8211b328f05198e4b376a655dfdef02640d/music-page1.png
+-rw-r--r--   0 la        (1000) la        (1000)   135995 2023-05-27 06:36:01.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/f999d8211b328f05198e4b376a655dfdef02640d/music-page2.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/fe054cc0f6577b37cbee4644af6855a6ff620a5c/
+-rw-r--r--   0 la        (1000) la        (1000)    21873 2023-05-27 06:36:04.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/fe054cc0f6577b37cbee4644af6855a6ff620a5c/music.png
+-rw-r--r--   0 la        (1000) la        (1000)     4462 2023-05-27 06:36:03.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/fe054cc0f6577b37cbee4644af6855a6ff620a5c/music.preview.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/ffb362a524748a92eb3e385545fa1a68d9639ca7/
+-rw-r--r--   0 la        (1000) la        (1000)    75224 2023-05-27 06:35:53.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_lilypond/ffb362a524748a92eb3e385545fa1a68d9639ca7/music.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_build/html/_static/
+-rw-r--r--   0 la        (1000) la        (1000)      286 2023-05-23 15:42:37.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 la        (1000) la        (1000)       90 2023-05-23 15:42:37.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 la        (1000) la        (1000)       90 2023-05-23 15:42:37.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 la        (1000) la        (1000)    15941 2020-12-06 23:56:53.000000 sphinxnotes-lilypond-1.6.1/docs/_build/html/_static/sphinx-notes.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_images/
+-rw-r--r--   0 la        (1000) la        (1000)    15941 2020-12-06 23:56:53.000000 sphinxnotes-lilypond-1.6.1/docs/_images/sphinx-notes.png
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/docs/_scores/
+-rw-r--r--   0 la        (1000) la        (1000)     2218 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/_scores/alice.ly
+-rw-r--r--   0 la        (1000) la        (1000)      273 2023-05-27 09:26:30.000000 sphinxnotes-lilypond-1.6.1/docs/_scores/lily-directive-c-major-scale.txt
+-rw-r--r--   0 la        (1000) la        (1000)      391 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/_scores/lily-directive.txt
+-rw-r--r--   0 la        (1000) la        (1000)       65 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/_scores/lily-role.txt
+-rw-r--r--   0 la        (1000) la        (1000)       79 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/_scores/lilyinclude-directive.txt
+-rw-r--r--   0 la        (1000) la        (1000)      275 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/_scores/minuet-in-g.ly
+-rw-r--r--   0 la        (1000) la        (1000)      617 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/_scores/witch-spring.ly
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.576452 sphinxnotes-lilypond-1.6.1/docs/_static/
+-rw-r--r--   0 la        (1000) la        (1000)        0 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/_static/.gitkeep
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.576452 sphinxnotes-lilypond-1.6.1/docs/_templates/
+-rw-r--r--   0 la        (1000) la        (1000)      161 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/_templates/version.rst
+-rw-r--r--   0 la        (1000) la        (1000)     2153 2023-07-09 15:39:43.000000 sphinxnotes-lilypond-1.6.1/docs/changelog.rst
+-rw-r--r--   0 la        (1000) la        (1000)     4020 2023-07-09 15:42:23.000000 sphinxnotes-lilypond-1.6.1/docs/conf.py
+-rw-r--r--   0 la        (1000) la        (1000)     1860 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/conf.rst
+-rw-r--r--   0 la        (1000) la        (1000)     2392 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/examples.rst
+-rw-r--r--   0 la        (1000) la        (1000)     2939 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/index.rst
+-rw-r--r--   0 la        (1000) la        (1000)      852 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/make.bat
+-rw-r--r--   0 la        (1000) la        (1000)     2486 2023-05-27 06:42:53.000000 sphinxnotes-lilypond-1.6.1/docs/usage.rst
+-rw-r--r--   0 la        (1000) la        (1000)     2267 2023-06-18 13:22:13.000000 sphinxnotes-lilypond-1.6.1/pyproject.toml
+-rw-r--r--   0 la        (1000) la        (1000)       38 2023-07-09 15:45:54.576452 sphinxnotes-lilypond-1.6.1/setup.cfg
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/src/
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.573119 sphinxnotes-lilypond-1.6.1/src/sphinxnotes/
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.576452 sphinxnotes-lilypond-1.6.1/src/sphinxnotes/lilypond/
+-rw-r--r--   0 la        (1000) la        (1000)    14219 2023-06-22 10:41:43.000000 sphinxnotes-lilypond-1.6.1/src/sphinxnotes/lilypond/__init__.py
+-rw-r--r--   0 la        (1000) la        (1000)    46517 2022-07-21 04:53:28.000000 sphinxnotes-lilypond-1.6.1/src/sphinxnotes/lilypond/jianpu.py
+-rw-r--r--   0 la        (1000) la        (1000)    14085 2023-06-24 13:01:51.000000 sphinxnotes-lilypond-1.6.1/src/sphinxnotes/lilypond/lilypond.py
+drwxr-xr-x   0 la        (1000) la        (1000)        0 2023-07-09 15:45:54.576452 sphinxnotes-lilypond-1.6.1/src/sphinxnotes_lilypond.egg-info/
+-rw-r--r--   0 la        (1000) la        (1000)     2280 2023-07-09 15:45:54.000000 sphinxnotes-lilypond-1.6.1/src/sphinxnotes_lilypond.egg-info/PKG-INFO
+-rw-r--r--   0 la        (1000) la        (1000)     2381 2023-07-09 15:45:54.000000 sphinxnotes-lilypond-1.6.1/src/sphinxnotes_lilypond.egg-info/SOURCES.txt
+-rw-r--r--   0 la        (1000) la        (1000)        1 2023-07-09 15:45:54.000000 sphinxnotes-lilypond-1.6.1/src/sphinxnotes_lilypond.egg-info/dependency_links.txt
+-rw-r--r--   0 la        (1000) la        (1000)      157 2023-07-09 15:45:54.000000 sphinxnotes-lilypond-1.6.1/src/sphinxnotes_lilypond.egg-info/requires.txt
+-rw-r--r--   0 la        (1000) la        (1000)       12 2023-07-09 15:45:54.000000 sphinxnotes-lilypond-1.6.1/src/sphinxnotes_lilypond.egg-info/top_level.txt
```

### Comparing `sphinxnotes-lilypond-1.6.0/LICENSE` & `sphinxnotes-lilypond-1.6.1/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020, Sphinx Notes
+Copyright (c) 2023, Shengyu Zhang
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
@@ -22,8 +22,8 @@
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `sphinxnotes-lilypond-1.6.0/sphinxnotes/lilypond/__init__.py` & `sphinxnotes-lilypond-1.6.1/src/sphinxnotes/lilypond/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 from abc import abstractmethod
 from typing import Tuple, List
 
 from docutils import nodes
 from docutils.utils import unescape
 from docutils.parsers.rst import directives
 
-from sphinx.util import ensuredir, relative_uri, logging
+from sphinx.util import logging
+from sphinx.util.osutil import ensuredir, relative_uri
 from sphinx.util.docutils import SphinxDirective
 from sphinx.config import Config
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.builders.latex import LaTeXBuilder
 
 from . import lilypond
 from . import jianpu
@@ -41,24 +42,17 @@
 logger = logging.getLogger(__name__)
 
 _DIVCLS = 'lilypond'
 _SCORECLS = 'lilypond-score'
 _AUDIOCLS = 'lilypond-audio'
 _LILYDIR = '_lilypond'
 
-class lily_base_node(object):
-    """
-    Parent class of :class:`lily_inline_node` and :class:`lily_outline_node`,
-    just created for type annotations.
-    """
-    pass
+class lily_inline_node(nodes.Inline, nodes.TextElement): pass
 
-class lily_inline_node(nodes.Inline, nodes.TextElement, lily_base_node): pass
-
-class lily_outline_node(nodes.Part, nodes.Element, lily_base_node): pass
+class lily_outline_node(nodes.Part, nodes.Element): pass
 
 def lily_role(role, rawtext, text, lineno, inliner, options={}, content=[]):
     env = inliner.document.settings.env # type: ignore
 
     if not isinstance(env.app.builder, (StandaloneHTMLBuilder, LaTeXBuilder)):
         # Builder is not supported, fallback to literal_block.
         node = nodes.literal(rawtext, unescape(text, restore_backslashes=True))
@@ -137,16 +131,19 @@
 class LilyIncludeDirective(BaseLilyDirective):
 
     required_arguments = 1
     final_argument_whitespace = True
 
     def read_lily_source(self) -> str:
         fn = self.arguments[0]
-        if not path.isabs(fn):
-            # Rel to abs
+        if path.isabs(fn):
+            # Doc abs to fs abs.
+            fn = self.env.srcdir + fn
+        else:
+            # Relpath to abspath.
             fn = path.join(path.dirname(self.env.doc2path(self.env.docname)), fn)
         with open(fn, 'r') as f:
             self.env.note_dependency(fn)
             return f.read()
 
 
 class BaseJianpuDirective(BaseLilyDirective):
@@ -176,31 +173,31 @@
         if not path.isabs(fn):
             # Rel to abs
             fn = path.join(path.dirname(self.env.doc2path(self.env.docname)), fn)
         with open(fn, 'r') as f:
             self.env.note_dependency(fn)
             return f.read()
 
-def get_node_sig(node:lily_base_node) -> str:
+def get_node_sig(node:lily_inline_node|lily_outline_node) -> str:
     """Return signture of given node. """
     return sha((node['lilysrc'] + node['rawtext']).encode('utf-8')).hexdigest()
 
 
-def get_builddir_and_reldir(builder, node:lily_base_node) -> Tuple[str,str]:
+def get_builddir_and_reldir(builder, node:lily_inline_node|lily_outline_node) -> Tuple[str,str]:
     """
     Return the path of Sphinx builder's outdir and its corrsponding relative
     path.
     """
     builddir = path.join(builder.outdir, _LILYDIR)
     reluri = relative_uri(builder.get_target_uri(node['docname']), '.')
     reldir = posixpath.join(reluri, _LILYDIR)
     return (builddir, reldir)
 
 
-def pick_from_builddir(builder, node:lily_base_node) -> lilypond.Output:
+def pick_from_builddir(builder, node:lily_inline_node|lily_outline_node) -> lilypond.Output|None:
     """
     Try to pick the LilyPond outputted files (:class:`lilypond.Output`)
     already cached in builder's outdir.
     """
     sig = get_node_sig(node)
     builddir, reldir = get_builddir_and_reldir(builder, node)
     outfn = path.join(builddir, sig)
@@ -215,30 +212,30 @@
         return None
     else:
         relfn = posixpath.join(reldir, sig)
         out.relocate(relfn)
         return out
 
 
-def move_to_builddir(builder, node:lily_base_node, out:lilypond.Output):
+def move_to_builddir(builder, node:lily_inline_node|lily_outline_node, out:lilypond.Output):
     """
     Move lilypond outputted files to builder's outdir, relocate the path of
     :class:`lilypond.Output` to relative path.
     """
     sig = get_node_sig(node)
     builddir, reldir = get_builddir_and_reldir(builder, node)
     outfn = path.join(builddir, sig)
     relfn = posixpath.join(reldir, sig)
     ensuredir(path.dirname(outfn))
     shutil.move(out.outdir, outfn)
     out.relocate(relfn)
     return out
 
 
-def get_lilypond_output(self, node:lily_base_node) -> lilypond.Output:
+def get_lilypond_output(self, node:lily_inline_node|lily_outline_node) -> lilypond.Output:
     out = pick_from_builddir(self.builder, node)
 
     cached = not (out is None)
     if cached:
         logger.debug('using cached result %s' % out.outdir, location=node)
     else:
         logger.debug('creating a new lilypond document', location=node)
@@ -265,25 +262,25 @@
             shutil.rmtree(builddir)
         else:
             # Get relative path
             move_to_builddir(self.builder, node, out)
     return out
 
 
-def html_visit_lily_node(self, node:lily_base_node):
+def html_visit_lily_node(self, node:lily_inline_node|lily_outline_node):
     out = get_lilypond_output(self, node)
 
     # Create div for block level element
     if isinstance(node, lily_outline_node):
-        self.body.append(self.starttag(node, 'div', CLASS='lilypond'))
+        self.body.append(self.starttag(node, 'div', CLASS=_DIVCLS))
         self.body.append('<p>')
 
     if node.get('audio') and out.audio and node.get('controls') == 'top':
         self.body.append('<audio controls class="%s" style="%s" src="%s" %s>\n' %
-                (_SCORECLS, 'width:100%;', out.audio, 'loop' if node.get('loop') else ''))
+                (_AUDIOCLS, 'width:100%;', out.audio, 'loop' if node.get('loop') else ''))
         self.body.append('</audio>')
 
     # TODO: standalone css
     if node.get('preview') and out.preview:
         self.body.append(
             '<img class="%s" src="%s" alt="%s" style="height:%s;", align="absbottom"/>' %
             (_SCORECLS,
@@ -311,15 +308,15 @@
 
     if isinstance(node, lily_outline_node):
         self.body.append('</p>')
         self.body.append('</div>')
 
     raise nodes.SkipNode
 
-def latex_visit_lily_node(self, node:lily_base_node):
+def latex_visit_lily_node(self, node:lily_inline_node|lily_outline_node):
     """
     See sphinx/sphinx/writers/latex.py::visit_image().
     """
 
     out = get_lilypond_output(self, node)
 
     CR = '\n'
```

### Comparing `sphinxnotes-lilypond-1.6.0/sphinxnotes/lilypond/jianpu.py` & `sphinxnotes-lilypond-1.6.1/src/sphinxnotes/lilypond/jianpu.py`

 * *Files identical despite different names*

### Comparing `sphinxnotes-lilypond-1.6.0/sphinxnotes/lilypond/lilypond.py` & `sphinxnotes-lilypond-1.6.1/src/sphinxnotes/lilypond/lilypond.py`

 * *Files identical despite different names*

