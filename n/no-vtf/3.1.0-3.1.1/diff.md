# Comparing `tmp/no_vtf-3.1.0.tar.gz` & `tmp/no_vtf-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "no_vtf-3.1.0.tar", last modified: Sat Jul  1 19:19:31 2023, max compression
+gzip compressed data, was "no_vtf-3.1.1.tar", last modified: Sun Jul  9 08:32:13 2023, max compression
```

## Comparing `no_vtf-3.1.0.tar` & `no_vtf-3.1.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.722456 no_vtf-3.1.0/
--rw-r--r--   0 build     (1000) build     (1000)     1754 2023-07-01 19:09:49.000000 no_vtf-3.1.0/.build.yml
--rw-r--r--   0 build     (1000) build     (1000)      336 2023-07-01 19:09:49.000000 no_vtf-3.1.0/.gitignore
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.706455 no_vtf-3.1.0/.reuse/
--rw-r--r--   0 build     (1000) build     (1000)      189 2023-07-01 19:09:49.000000 no_vtf-3.1.0/.reuse/dep5
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.706455 no_vtf-3.1.0/LICENSES/
--rw-r--r--   0 build     (1000) build     (1000)    17023 2023-07-01 19:09:49.000000 no_vtf-3.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 build     (1000) build     (1000)     7048 2023-07-01 19:09:49.000000 no_vtf-3.1.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 build     (1000) build     (1000)    34670 2023-07-01 19:09:49.000000 no_vtf-3.1.0/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 build     (1000) build     (1000)    42098 2023-07-01 19:09:49.000000 no_vtf-3.1.0/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 build     (1000) build     (1000)      138 2023-07-01 19:09:49.000000 no_vtf-3.1.0/MANIFEST.in
--rw-r--r--   0 build     (1000) build     (1000)     9371 2023-07-01 19:19:31.722456 no_vtf-3.1.0/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)     8100 2023-07-01 19:09:49.000000 no_vtf-3.1.0/README.md
--rw-r--r--   0 build     (1000) build     (1000)       95 2023-07-01 19:09:49.000000 no_vtf-3.1.0/README.md.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.706455 no_vtf-3.1.0/builds/
--rw-r--r--   0 build     (1000) build     (1000)      559 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/common
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.710456 no_vtf-3.1.0/builds/debian/
--rw-r--r--   0 build     (1000) build     (1000)      162 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/debian/common
--rwxr-xr-x   0 build     (1000) build     (1000)      409 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/debian/env.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      412 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/debian/ksc-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      518 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/debian/python3.10-build_dep.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      863 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/debian/wine-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      188 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/diff_generated.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      196 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/nox.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      206 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/nox_wine.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      649 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/publish_frozen.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      474 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/python3.10-install.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      371 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/verify_signatures.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      272 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/with_clone.sh
--rwxr-xr-x   0 build     (1000) build     (1000)      997 2023-07-01 19:09:49.000000 no_vtf-3.1.0/builds/with_wine.sh
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.710456 no_vtf-3.1.0/ksy/
--rwxr-xr-x   0 build     (1000) build     (1000)      205 2023-07-01 19:09:49.000000 no_vtf-3.1.0/ksy/compile.sh
--rw-r--r--   0 build     (1000) build     (1000)    10409 2023-07-01 19:09:49.000000 no_vtf-3.1.0/ksy/vtf.ksy
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.710456 no_vtf-3.1.0/no_vtf/
--rw-r--r--   0 build     (1000) build     (1000)      329 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      300 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/__main__.py
--rw-r--r--   0 build     (1000) build     (1000)      160 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf/_version.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.710456 no_vtf-3.1.0/no_vtf/deferred/
--rw-r--r--   0 build     (1000) build     (1000)      186 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/deferred/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1471 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/deferred/deferred.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/filesystem/
--rw-r--r--   0 build     (1000) build     (1000)      287 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/filesystem/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     2023 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/filesystem/input_paths.py
--rw-r--r--   0 build     (1000) build     (1000)      895 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/filesystem/output_directories.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/image/
--rw-r--r--   0 build     (1000) build     (1000)      441 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1667 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/channel_separator.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/image/decoder/
--rw-r--r--   0 build     (1000) build     (1000)      198 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/decoder/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      486 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/decoder/decoder.py
--rw-r--r--   0 build     (1000) build     (1000)     7697 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/decoder/generic.py
--rw-r--r--   0 build     (1000) build     (1000)     2797 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/decoder/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)     1497 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/image.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/image/modifier/
--rw-r--r--   0 build     (1000) build     (1000)      202 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/modifier/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1632 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/modifier/fp_precision_modifier.py
--rw-r--r--   0 build     (1000) build     (1000)      540 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/modifier/modifier.py
--rw-r--r--   0 build     (1000) build     (1000)      946 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/image/ndarray.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/io/
--rw-r--r--   0 build     (1000) build     (1000)      264 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/io/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      866 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/io/bytes.py
--rw-r--r--   0 build     (1000) build     (1000)     9249 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/io/image.py
--rw-r--r--   0 build     (1000) build     (1000)     1246 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/io/io.py
--rw-r--r--   0 build     (1000) build     (1000)    22474 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/main.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/parser/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/parser/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.714456 no_vtf-3.1.0/no_vtf/parser/generated/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/parser/generated/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)    25192 2023-07-01 19:19:13.000000 no_vtf-3.1.0/no_vtf/parser/generated/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)       93 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/parser/generated/vtf.py.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/pipeline/
--rw-r--r--   0 build     (1000) build     (1000)      186 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/pipeline/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     7894 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/pipeline/pipeline.py
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/py.typed
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/task_runner/
--rw-r--r--   0 build     (1000) build     (1000)      356 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/task_runner/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)     1524 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/task_runner/parallel.py
--rw-r--r--   0 build     (1000) build     (1000)      826 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/task_runner/sequential.py
--rw-r--r--   0 build     (1000) build     (1000)     1085 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/task_runner/task_runner.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/texture/
--rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/__init__.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/texture/decoder/
--rw-r--r--   0 build     (1000) build     (1000)      204 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/decoder/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      486 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/decoder/decoder.py
--rw-r--r--   0 build     (1000) build     (1000)     4485 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/decoder/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/texture/extractor/
--rw-r--r--   0 build     (1000) build     (1000)      212 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/extractor/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      453 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/extractor/extractor.py
--rw-r--r--   0 build     (1000) build     (1000)     4010 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/extractor/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/texture/filter/
--rw-r--r--   0 build     (1000) build     (1000)      252 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/filter/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      702 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/filter/filter.py
--rw-r--r--   0 build     (1000) build     (1000)     4774 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/filter/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.718456 no_vtf-3.1.0/no_vtf/texture/namer/
--rw-r--r--   0 build     (1000) build     (1000)      196 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/namer/__init__.py
--rw-r--r--   0 build     (1000) build     (1000)      374 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/namer/namer.py
--rw-r--r--   0 build     (1000) build     (1000)     1079 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/namer/vtf.py
--rw-r--r--   0 build     (1000) build     (1000)      663 2023-07-01 19:09:49.000000 no_vtf-3.1.0/no_vtf/texture/vtf.py
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.710456 no_vtf-3.1.0/no_vtf.egg-info/
--rw-r--r--   0 build     (1000) build     (1000)     9371 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/PKG-INFO
--rw-r--r--   0 build     (1000) build     (1000)     2389 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/SOURCES.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/dependency_links.txt
--rw-r--r--   0 build     (1000) build     (1000)       49 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/entry_points.txt
--rw-r--r--   0 build     (1000) build     (1000)        1 2023-07-01 19:18:33.000000 no_vtf-3.1.0/no_vtf.egg-info/not-zip-safe
--rw-r--r--   0 build     (1000) build     (1000)      183 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/requires.txt
--rw-r--r--   0 build     (1000) build     (1000)        7 2023-07-01 19:19:31.000000 no_vtf-3.1.0/no_vtf.egg-info/top_level.txt
--rw-r--r--   0 build     (1000) build     (1000)     9847 2023-07-01 19:09:49.000000 no_vtf-3.1.0/noxfile.py
--rw-r--r--   0 build     (1000) build     (1000)      682 2023-07-01 19:09:49.000000 no_vtf-3.1.0/pyproject.toml
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.702455 no_vtf-3.1.0/resources/
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.722456 no_vtf-3.1.0/resources/docs/
--rw-r--r--   0 build     (1000) build     (1000)   123671 2023-07-01 19:09:49.000000 no_vtf-3.1.0/resources/docs/screencast.gif
--rw-r--r--   0 build     (1000) build     (1000)       95 2023-07-01 19:09:49.000000 no_vtf-3.1.0/resources/docs/screencast.gif.license
-drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-01 19:19:31.722456 no_vtf-3.1.0/resources/pyinstaller/
--rw-r--r--   0 build     (1000) build     (1000)        6 2023-07-01 19:09:49.000000 no_vtf-3.1.0/resources/pyinstaller/empty.ico
--rw-r--r--   0 build     (1000) build     (1000)       93 2023-07-01 19:09:49.000000 no_vtf-3.1.0/resources/pyinstaller/empty.ico.license
--rwxr-xr-x   0 build     (1000) build     (1000)      385 2023-07-01 19:09:49.000000 no_vtf-3.1.0/resources/pyinstaller/no_vtf.desktop
--rw-r--r--   0 build     (1000) build     (1000)     2640 2023-07-01 19:19:31.722456 no_vtf-3.1.0/setup.cfg
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.656524 no_vtf-3.1.1/
+-rw-r--r--   0 build     (1000) build     (1000)     1754 2023-07-09 08:22:01.000000 no_vtf-3.1.1/.build.yml
+-rw-r--r--   0 build     (1000) build     (1000)      336 2023-07-09 08:22:01.000000 no_vtf-3.1.1/.gitignore
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.640524 no_vtf-3.1.1/.reuse/
+-rw-r--r--   0 build     (1000) build     (1000)      189 2023-07-09 08:22:01.000000 no_vtf-3.1.1/.reuse/dep5
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.640524 no_vtf-3.1.1/LICENSES/
+-rw-r--r--   0 build     (1000) build     (1000)    17023 2023-07-09 08:22:01.000000 no_vtf-3.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 build     (1000) build     (1000)     7048 2023-07-09 08:22:01.000000 no_vtf-3.1.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 build     (1000) build     (1000)    34670 2023-07-09 08:22:01.000000 no_vtf-3.1.1/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 build     (1000) build     (1000)    42098 2023-07-09 08:22:01.000000 no_vtf-3.1.1/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 build     (1000) build     (1000)      138 2023-07-09 08:22:01.000000 no_vtf-3.1.1/MANIFEST.in
+-rw-r--r--   0 build     (1000) build     (1000)     9392 2023-07-09 08:32:13.656524 no_vtf-3.1.1/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)     8121 2023-07-09 08:22:01.000000 no_vtf-3.1.1/README.md
+-rw-r--r--   0 build     (1000) build     (1000)       95 2023-07-09 08:22:01.000000 no_vtf-3.1.1/README.md.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.644524 no_vtf-3.1.1/builds/
+-rw-r--r--   0 build     (1000) build     (1000)      559 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/common
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.644524 no_vtf-3.1.1/builds/debian/
+-rw-r--r--   0 build     (1000) build     (1000)      162 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/debian/common
+-rwxr-xr-x   0 build     (1000) build     (1000)      409 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/debian/env.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      412 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/debian/ksc-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      518 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/debian/python3.10-build_dep.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      863 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/debian/wine-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      188 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/diff_generated.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      196 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/nox.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      243 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/nox_wine.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      649 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/publish_frozen.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      474 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/python3.10-install.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      371 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/verify_signatures.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      272 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/with_clone.sh
+-rwxr-xr-x   0 build     (1000) build     (1000)      997 2023-07-09 08:22:01.000000 no_vtf-3.1.1/builds/with_wine.sh
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.644524 no_vtf-3.1.1/ksy/
+-rwxr-xr-x   0 build     (1000) build     (1000)      205 2023-07-09 08:22:01.000000 no_vtf-3.1.1/ksy/compile.sh
+-rw-r--r--   0 build     (1000) build     (1000)    10409 2023-07-09 08:22:01.000000 no_vtf-3.1.1/ksy/vtf.ksy
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.644524 no_vtf-3.1.1/no_vtf/
+-rw-r--r--   0 build     (1000) build     (1000)      329 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      300 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/__main__.py
+-rw-r--r--   0 build     (1000) build     (1000)      160 2023-07-09 08:32:13.000000 no_vtf-3.1.1/no_vtf/_version.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.648524 no_vtf-3.1.1/no_vtf/deferred/
+-rw-r--r--   0 build     (1000) build     (1000)      186 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/deferred/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1471 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/deferred/deferred.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.648524 no_vtf-3.1.1/no_vtf/filesystem/
+-rw-r--r--   0 build     (1000) build     (1000)      287 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/filesystem/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     2023 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/filesystem/input_paths.py
+-rw-r--r--   0 build     (1000) build     (1000)      895 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/filesystem/output_directories.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.648524 no_vtf-3.1.1/no_vtf/image/
+-rw-r--r--   0 build     (1000) build     (1000)      441 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/image/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1667 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/image/channel_separator.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.648524 no_vtf-3.1.1/no_vtf/image/decoder/
+-rw-r--r--   0 build     (1000) build     (1000)      198 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/image/decoder/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      486 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/image/decoder/decoder.py
+-rw-r--r--   0 build     (1000) build     (1000)     7697 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/image/decoder/generic.py
+-rw-r--r--   0 build     (1000) build     (1000)     2797 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/image/decoder/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)     1497 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/image/image.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.652524 no_vtf-3.1.1/no_vtf/image/modifier/
+-rw-r--r--   0 build     (1000) build     (1000)      202 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/image/modifier/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1632 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/image/modifier/fp_precision_modifier.py
+-rw-r--r--   0 build     (1000) build     (1000)      540 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/image/modifier/modifier.py
+-rw-r--r--   0 build     (1000) build     (1000)      946 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/image/ndarray.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.652524 no_vtf-3.1.1/no_vtf/io/
+-rw-r--r--   0 build     (1000) build     (1000)      264 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/io/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      866 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/io/bytes.py
+-rw-r--r--   0 build     (1000) build     (1000)    10840 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/io/image.py
+-rw-r--r--   0 build     (1000) build     (1000)     1066 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/io/io.py
+-rw-r--r--   0 build     (1000) build     (1000)    22608 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/main.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.652524 no_vtf-3.1.1/no_vtf/parser/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/parser/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.652524 no_vtf-3.1.1/no_vtf/parser/generated/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/parser/generated/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)    25192 2023-07-09 08:31:54.000000 no_vtf-3.1.1/no_vtf/parser/generated/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)       93 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/parser/generated/vtf.py.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.652524 no_vtf-3.1.1/no_vtf/pipeline/
+-rw-r--r--   0 build     (1000) build     (1000)      186 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/pipeline/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     8497 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/pipeline/pipeline.py
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/py.typed
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.652524 no_vtf-3.1.1/no_vtf/task_runner/
+-rw-r--r--   0 build     (1000) build     (1000)      356 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/task_runner/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)     1953 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/task_runner/parallel.py
+-rw-r--r--   0 build     (1000) build     (1000)      826 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/task_runner/sequential.py
+-rw-r--r--   0 build     (1000) build     (1000)      905 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/task_runner/task_runner.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.652524 no_vtf-3.1.1/no_vtf/texture/
+-rw-r--r--   0 build     (1000) build     (1000)        0 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/__init__.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.656524 no_vtf-3.1.1/no_vtf/texture/decoder/
+-rw-r--r--   0 build     (1000) build     (1000)      204 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/decoder/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      486 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/decoder/decoder.py
+-rw-r--r--   0 build     (1000) build     (1000)     4485 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/decoder/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.656524 no_vtf-3.1.1/no_vtf/texture/extractor/
+-rw-r--r--   0 build     (1000) build     (1000)      212 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/extractor/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      453 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/extractor/extractor.py
+-rw-r--r--   0 build     (1000) build     (1000)     4010 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/extractor/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.656524 no_vtf-3.1.1/no_vtf/texture/filter/
+-rw-r--r--   0 build     (1000) build     (1000)      252 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/filter/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      702 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/filter/filter.py
+-rw-r--r--   0 build     (1000) build     (1000)     5201 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/filter/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.656524 no_vtf-3.1.1/no_vtf/texture/namer/
+-rw-r--r--   0 build     (1000) build     (1000)      196 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/namer/__init__.py
+-rw-r--r--   0 build     (1000) build     (1000)      374 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/namer/namer.py
+-rw-r--r--   0 build     (1000) build     (1000)     1079 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/namer/vtf.py
+-rw-r--r--   0 build     (1000) build     (1000)      663 2023-07-09 08:22:01.000000 no_vtf-3.1.1/no_vtf/texture/vtf.py
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.648524 no_vtf-3.1.1/no_vtf.egg-info/
+-rw-r--r--   0 build     (1000) build     (1000)     9392 2023-07-09 08:32:13.000000 no_vtf-3.1.1/no_vtf.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1000)     2389 2023-07-09 08:32:13.000000 no_vtf-3.1.1/no_vtf.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2023-07-09 08:32:13.000000 no_vtf-3.1.1/no_vtf.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1000)       49 2023-07-09 08:32:13.000000 no_vtf-3.1.1/no_vtf.egg-info/entry_points.txt
+-rw-r--r--   0 build     (1000) build     (1000)        1 2023-07-09 08:31:09.000000 no_vtf-3.1.1/no_vtf.egg-info/not-zip-safe
+-rw-r--r--   0 build     (1000) build     (1000)      191 2023-07-09 08:32:13.000000 no_vtf-3.1.1/no_vtf.egg-info/requires.txt
+-rw-r--r--   0 build     (1000) build     (1000)        7 2023-07-09 08:32:13.000000 no_vtf-3.1.1/no_vtf.egg-info/top_level.txt
+-rw-r--r--   0 build     (1000) build     (1000)     9847 2023-07-09 08:22:01.000000 no_vtf-3.1.1/noxfile.py
+-rw-r--r--   0 build     (1000) build     (1000)      682 2023-07-09 08:22:01.000000 no_vtf-3.1.1/pyproject.toml
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.636524 no_vtf-3.1.1/resources/
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.656524 no_vtf-3.1.1/resources/docs/
+-rw-r--r--   0 build     (1000) build     (1000)   123671 2023-07-09 08:22:01.000000 no_vtf-3.1.1/resources/docs/screencast.gif
+-rw-r--r--   0 build     (1000) build     (1000)       95 2023-07-09 08:22:01.000000 no_vtf-3.1.1/resources/docs/screencast.gif.license
+drwxr-xr-x   0 build     (1000) build     (1000)        0 2023-07-09 08:32:13.656524 no_vtf-3.1.1/resources/pyinstaller/
+-rw-r--r--   0 build     (1000) build     (1000)        6 2023-07-09 08:22:01.000000 no_vtf-3.1.1/resources/pyinstaller/empty.ico
+-rw-r--r--   0 build     (1000) build     (1000)       93 2023-07-09 08:22:01.000000 no_vtf-3.1.1/resources/pyinstaller/empty.ico.license
+-rwxr-xr-x   0 build     (1000) build     (1000)      385 2023-07-09 08:22:01.000000 no_vtf-3.1.1/resources/pyinstaller/no_vtf.desktop
+-rw-r--r--   0 build     (1000) build     (1000)     2650 2023-07-09 08:32:13.660524 no_vtf-3.1.1/setup.cfg
```

### Comparing `no_vtf-3.1.0/.build.yml` & `no_vtf-3.1.1/.build.yml`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/LICENSES/CC-BY-4.0.txt` & `no_vtf-3.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/LICENSES/CC0-1.0.txt` & `no_vtf-3.1.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/LICENSES/GPL-3.0-or-later.txt` & `no_vtf-3.1.1/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/LICENSES/LGPL-3.0-or-later.txt` & `no_vtf-3.1.1/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/PKG-INFO` & `no_vtf-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: no_vtf
-Version: 3.1.0
+Version: 3.1.1
 Summary: Valve Texture Format Converter
 Home-page: https://sr.ht/~b5327157/no_vtf
 Author: b5327157
 Author-email: b5327157@protonmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Download, https://sr.ht/~b5327157/no_vtf/#application-bundle
 Project-URL: Changelog, https://git.sr.ht/~b5327157/no_vtf/refs
@@ -25,15 +25,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSES/GPL-3.0-or-later.txt
 
 # no_vtf
 
-Say no to [Source Engine](https://developer.valvesoftware.com/wiki/Source)'s [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
+Say no to [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
 
 ![Badge showing supported Python versions](https://img.shields.io/pypi/pyversions/no_vtf?style=flat-square)
 [![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
 [![Badge showing number of monthly downloads from PyPI](https://img.shields.io/pypi/dm/no_vtf?style=flat-square)](https://pypistats.org/packages/no-vtf)
 [![Badge showing source code repository hosted on SourceHut](https://img.shields.io/badge/sr.ht-repository-white?labelColor=212529&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K)](https://sr.ht/~b5327157/no_vtf)
 [![Badge showing builds.sr.ht status](https://builds.sr.ht/~b5327157/no_vtf.svg?search=tags:master)](https://builds.sr.ht/~b5327157/no_vtf?search=tags:master)
 [![Badge showing REUSE compliance status](https://api.reuse.software/badge/git.sr.ht/~b5327157/no_vtf)](https://api.reuse.software/info/git.sr.ht/~b5327157/no_vtf)
@@ -126,15 +126,15 @@
 no_vtf --help
 ```
 
 ## Supported formats
 
 ### Input
 
-All textures installed with [Team Fortress 2](https://store.steampowered.com/app/440/Team_Fortress_2/), [Source Filmmaker](https://store.steampowered.com/app/1840/Source_Filmmaker/) and [Portal 2](https://store.steampowered.com/app/620/Portal_2/) can be converted with the supported format set.
+All textures installed with many [Source Engine](https://developer.valvesoftware.com/wiki/Source) games, including [Team Fortress 2](https://store.steampowered.com/app/440/Team_Fortress_2/), [Source Filmmaker](https://store.steampowered.com/app/1840/Source_Filmmaker/) and [Portal 2](https://store.steampowered.com/app/620/Portal_2/), can be converted with the supported format set.
 
 - `RGBA8888`
 - `ABGR8888`
 - `RGB888`
 - `BGR888`
 - `I8`
 - `IA88`
```

### Comparing `no_vtf-3.1.0/README.md` & `no_vtf-3.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # no_vtf
 
-Say no to [Source Engine](https://developer.valvesoftware.com/wiki/Source)'s [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
+Say no to [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
 
 ![Badge showing supported Python versions](https://img.shields.io/pypi/pyversions/no_vtf?style=flat-square)
 [![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
 [![Badge showing number of monthly downloads from PyPI](https://img.shields.io/pypi/dm/no_vtf?style=flat-square)](https://pypistats.org/packages/no-vtf)
 [![Badge showing source code repository hosted on SourceHut](https://img.shields.io/badge/sr.ht-repository-white?labelColor=212529&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K)](https://sr.ht/~b5327157/no_vtf)
 [![Badge showing builds.sr.ht status](https://builds.sr.ht/~b5327157/no_vtf.svg?search=tags:master)](https://builds.sr.ht/~b5327157/no_vtf?search=tags:master)
 [![Badge showing REUSE compliance status](https://api.reuse.software/badge/git.sr.ht/~b5327157/no_vtf)](https://api.reuse.software/info/git.sr.ht/~b5327157/no_vtf)
@@ -97,15 +97,15 @@
 no_vtf --help
 ```
 
 ## Supported formats
 
 ### Input
 
-All textures installed with [Team Fortress 2](https://store.steampowered.com/app/440/Team_Fortress_2/), [Source Filmmaker](https://store.steampowered.com/app/1840/Source_Filmmaker/) and [Portal 2](https://store.steampowered.com/app/620/Portal_2/) can be converted with the supported format set.
+All textures installed with many [Source Engine](https://developer.valvesoftware.com/wiki/Source) games, including [Team Fortress 2](https://store.steampowered.com/app/440/Team_Fortress_2/), [Source Filmmaker](https://store.steampowered.com/app/1840/Source_Filmmaker/) and [Portal 2](https://store.steampowered.com/app/620/Portal_2/), can be converted with the supported format set.
 
 - `RGBA8888`
 - `ABGR8888`
 - `RGB888`
 - `BGR888`
 - `I8`
 - `IA88`
```

### Comparing `no_vtf-3.1.0/builds/common` & `no_vtf-3.1.1/builds/common`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/builds/debian/python3.10-build_dep.sh` & `no_vtf-3.1.1/builds/debian/python3.10-build_dep.sh`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/builds/debian/wine-install.sh` & `no_vtf-3.1.1/builds/debian/wine-install.sh`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/builds/publish_frozen.sh` & `no_vtf-3.1.1/builds/publish_frozen.sh`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/builds/with_wine.sh` & `no_vtf-3.1.1/builds/with_wine.sh`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/ksy/vtf.ksy` & `no_vtf-3.1.1/ksy/vtf.ksy`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/deferred/deferred.py` & `no_vtf-3.1.1/no_vtf/deferred/deferred.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/filesystem/input_paths.py` & `no_vtf-3.1.1/no_vtf/filesystem/input_paths.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/filesystem/output_directories.py` & `no_vtf-3.1.1/no_vtf/filesystem/output_directories.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/image/channel_separator.py` & `no_vtf-3.1.1/no_vtf/image/channel_separator.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/image/decoder/generic.py` & `no_vtf-3.1.1/no_vtf/image/decoder/generic.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/image/decoder/vtf.py` & `no_vtf-3.1.1/no_vtf/image/decoder/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/image/image.py` & `no_vtf-3.1.1/no_vtf/image/image.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/image/modifier/fp_precision_modifier.py` & `no_vtf-3.1.1/no_vtf/image/modifier/fp_precision_modifier.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/image/modifier/modifier.py` & `no_vtf-3.1.1/no_vtf/image/modifier/modifier.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/image/ndarray.py` & `no_vtf-3.1.1/no_vtf/image/ndarray.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/io/bytes.py` & `no_vtf-3.1.1/no_vtf/io/bytes.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/io/image.py` & `no_vtf-3.1.1/no_vtf/io/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,66 +20,80 @@
 
 from no_vtf.image import Image, ImageData, ImageDataTypes
 from no_vtf.image.modifier.fp_precision_modifier import FPPrecisionModifier
 from no_vtf.image.modifier.modifier import ImageModifier
 from no_vtf.io.io import IO
 
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(kw_only=True)
 class ImageIO(IO[Image[ImageDataTypes]]):
     format: str
 
     compress: Optional[bool] = None
     fps: Optional[int] = None
 
     @classmethod
-    def _initialize(cls) -> None:
-        # download() seems to be untyped because of implicit reexport
-        imageio.plugins.freeimage.download()  # type: ignore[no-untyped-call]
+    def initialize(
+        cls, formats: Optional[Sequence[str]] = None, *, _recursive: bool = True
+    ) -> None:
+        super().initialize(_recursive=False)
+
+        if not formats:
+            _ImageIOBackend.initialize()
+        else:
+            for backend_format in map(str.lower, formats):
+                match backend_format:
+                    case "apng":
+                        _ImageIOApngBackend.initialize()
+                    case "exr":
+                        _ImageIOExrBackend.initialize()
+                    case "png":
+                        _ImageIOPngBackend.initialize()
+                    case "targa" | "tga":
+                        _ImageIOTgaBackend.initialize()
+                    case "tiff":
+                        _ImageIOTiffBackend.initialize()
+
+        if _recursive:
+            for subclass in cls.__subclasses__():
+                subclass.initialize(formats)
 
     _format_pattern: ClassVar[re.Pattern[str]] = re.compile(r"[a-z0-9]+", re.ASCII | re.IGNORECASE)
 
     def __post_init__(self) -> None:
-        assert self._is_initialized(), "IO.initialize() must be called early"
-
         if not self._format_pattern.fullmatch(self.format):
             raise RuntimeError(f"Invalid format: {self.format}")
 
-    def write_sequence(self, path: pathlib.Path, sequence: Sequence[Image[ImageDataTypes]]) -> None:
-        backend = self._get_backend()
-        backend.write(path, sequence)
-
-    def readback_sequence(
-        self, path: pathlib.Path, sequence: Sequence[Image[ImageDataTypes]]
-    ) -> None:
-        backend = self._get_backend()
-        backend.readback(path, sequence)
-
-    def _get_backend(self) -> _ImageIOBackend:
         compress = self.compress
         if compress is None:
             compress = True
 
-        extension = f".{self.format}"
-
-        backend: _ImageIOBackend
+        self._backend: _ImageIOBackend
         match self.format.lower():
             case "apng":
-                backend = _ImageIOApngBackend(compress=compress, fps=self.fps)
+                self._backend = _ImageIOApngBackend(compress=compress, fps=self.fps)
             case "exr":
-                backend = _ImageIOExrBackend(compress=compress)
+                self._backend = _ImageIOExrBackend(compress=compress)
             case "png":
-                backend = _ImageIOPngBackend(compress=compress)
+                self._backend = _ImageIOPngBackend(compress=compress)
             case "targa" | "tga":
-                backend = _ImageIOTgaBackend(compress=compress)
+                self._backend = _ImageIOTgaBackend(compress=compress)
             case "tiff":
-                backend = _ImageIOTiffBackend(compress=compress)
+                self._backend = _ImageIOTiffBackend(compress=compress)
             case _:
-                backend = _ImageIOBackend(extension=extension)
-        return backend
+                extension = f".{self.format}"
+                self._backend = _ImageIOBackend(extension=extension)
+
+    def write_sequence(self, path: pathlib.Path, sequence: Sequence[Image[ImageDataTypes]]) -> None:
+        self._backend.write(path, sequence)
+
+    def readback_sequence(
+        self, path: pathlib.Path, sequence: Sequence[Image[ImageDataTypes]]
+    ) -> None:
+        self._backend.readback(path, sequence)
 
 
 class _Opener(Protocol):
     def __call__(
         self,
         uri: imageio.typing.ImageResource,
         io_mode: Literal["r", "w"],
@@ -87,14 +101,20 @@
         extension: Optional[str] = None,
         format_hint: Optional[str] = None,
     ) -> imageio.core.v3_plugin_api.PluginV3:
         ...
 
 
 class _ImageIOBackend:
+    @classmethod
+    def initialize(cls, *, _recursive: bool = True) -> None:
+        if _recursive:
+            for subclass in cls.__subclasses__():
+                subclass.initialize()
+
     def __init__(self, *, extension: Optional[str] = None) -> None:
         self._extension = extension
 
     def write(self, path: pathlib.Path, sequence: Sequence[Image[ImageDataTypes]]) -> None:
         opener = self._get_opener()
         with opener(path, "w", extension=self._extension) as image_resource:
             for image in sequence:
@@ -190,19 +210,39 @@
         self._imageio_format = imageio_format
 
     def _get_opener(self) -> _Opener:
         return functools.partial(imageio.v3.imopen, legacy_mode=True, plugin=self._imageio_format)
 
 
 class _ImageIOFreeImageBackend(_ImageIOLegacyBackend):
-    IO_FLAGS: ClassVar = imageio.plugins.freeimage.IO_FLAGS
+    _freeimage_initialized: ClassVar[bool] = False
+
+    @classmethod
+    def initialize(cls, *, _recursive: bool = True) -> None:
+        super().initialize(_recursive=False)
+
+        if not _ImageIOFreeImageBackend._freeimage_initialized:
+            # download() seems to be untyped because of implicit reexport
+            imageio.plugins.freeimage.download()  # type: ignore[no-untyped-call]
+            _ImageIOFreeImageBackend._freeimage_initialized = True
+
+        if _recursive:
+            for subclass in cls.__subclasses__():
+                subclass.initialize()
+
+    IO_FLAGS: ClassVar[
+        type[imageio.plugins.freeimage.IO_FLAGS]
+    ] = imageio.plugins.freeimage.IO_FLAGS
 
     def __init__(self, *, imageio_format: str, extension: str) -> None:
         super().__init__(imageio_format=imageio_format, extension=extension)
 
+        if not _ImageIOFreeImageBackend._freeimage_initialized:
+            raise RuntimeError("ImageIO FreeImage backend was not initialized")
+
     def _get_writer_kwargs(self, image: Image[ImageDataTypes]) -> dict[str, object]:
         kwargs = super()._get_writer_kwargs(image)
         kwargs["flags"] = self._get_flags(image)
         return kwargs
 
     def _get_flags(self, image: Image[ImageDataTypes]) -> int:
         return 0
@@ -214,15 +254,15 @@
     ] = FPPrecisionModifier(min=32, max=32)
 
     def __init__(self, *, compress: bool = True) -> None:
         super().__init__(imageio_format="EXR-FI", extension=".exr")
         self.compress = compress
 
     def _get_flags(self, image: Image[ImageDataTypes]) -> int:
-        flags = 0
+        flags = super()._get_flags(image)
         flags |= self.IO_FLAGS.EXR_ZIP if self.compress else self.IO_FLAGS.EXR_NONE
         if not np.issubdtype(image.data().dtype, np.float16):
             flags |= self.IO_FLAGS.EXR_FLOAT
         return flags
 
     def _postprocess(self, image: Image[ImageDataTypes]) -> Image[ImageDataTypes]:
         return self._fp_force_32_bits(image)
@@ -230,28 +270,28 @@
 
 class _ImageIOTgaBackend(_ImageIOFreeImageBackend):
     def __init__(self, *, compress: bool = True) -> None:
         super().__init__(imageio_format="TARGA-FI", extension=".tga")
         self.compress = compress
 
     def _get_flags(self, image: Image[ImageDataTypes]) -> int:
-        flags = 0
+        flags = super()._get_flags(image)
         flags |= self.IO_FLAGS.TARGA_SAVE_RLE if self.compress else self.IO_FLAGS.TARGA_DEFAULT
         return flags
 
 
 class _ImageIOTiffBackend(_ImageIOFreeImageBackend):
     _fp_force_32_bits: ClassVar[
         ImageModifier[ImageDataTypes, ImageDataTypes]
     ] = FPPrecisionModifier(min=32, max=32)
 
     def __init__(self, *, compress: bool = True) -> None:
         super().__init__(imageio_format="TIFF-FI", extension=".tiff")
         self.compress = compress
 
     def _get_flags(self, image: Image[ImageDataTypes]) -> int:
-        flags = 0
+        flags = super()._get_flags(image)
         flags |= self.IO_FLAGS.TIFF_DEFAULT if self.compress else self.IO_FLAGS.TIFF_NONE
         return flags
 
     def _postprocess(self, image: Image[ImageDataTypes]) -> Image[ImageDataTypes]:
         return self._fp_force_32_bits(image)
```

### Comparing `no_vtf-3.1.0/no_vtf/io/io.py` & `no_vtf-3.1.1/no_vtf/io/io.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,38 +2,27 @@
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 import pathlib
 
 from abc import abstractmethod
 from collections.abc import Sequence
-from typing import ClassVar, Generic, TypeVar
+from typing import Generic, TypeVar
 
 import no_vtf.io  # noqa: F401  # define all task runners for IO.initialize()
 
 _A_contra = TypeVar("_A_contra", contravariant=True)
 
 
 class IO(Generic[_A_contra]):
-    _initialized: ClassVar[bool] = False
-
-    @classmethod
-    def initialize(cls) -> None:
-        for subclass in cls.__subclasses__():
-            subclass._initialize()
-
-        cls._initialized = True
-
-    @classmethod
-    def _is_initialized(cls) -> bool:
-        return cls._initialized
-
     @classmethod
-    def _initialize(cls) -> None:
-        pass
+    def initialize(cls, *, _recursive: bool = True) -> None:
+        if _recursive:
+            for subclass in cls.__subclasses__():
+                subclass.initialize()
 
     def write(self, path: pathlib.Path, data: _A_contra, /) -> None:
         self.write_sequence(path, [data])
 
     def readback(self, path: pathlib.Path, data: _A_contra, /) -> None:
         self.readback_sequence(path, [data])
```

### Comparing `no_vtf-3.1.0/no_vtf/main.py` & `no_vtf-3.1.1/no_vtf/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # SPDX-FileCopyrightText: b5327157 <b5327157@protonmail.com>
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 from __future__ import annotations
 
 import contextlib
+import functools
 import inspect
 import pathlib
 import re
 import sys
 
 from collections.abc import Sequence
 from dataclasses import dataclass
@@ -503,15 +504,18 @@
     )
 
     texture_extractor = VtfExtractor()
     texture_filter = TextureCombinedFilter(texture_filters)
     texture_decoder = VtfDecoder(dynamic_range=dynamic_range, overbright_factor=overbright_factor)
     texture_namer = Vtf2TgaLikeNamer(include_mipmap_level=mipmaps, include_frame=(not animate))
 
-    Pipeline.initialize()
+    formats = [ldr_format, hdr_format]
+    pipeline_initializer = functools.partial(Pipeline.initialize, formats)
+    pipeline_initializer()
+
     pipeline = Pipeline(
         input_extension_pattern=vtf_extension_pattern,
         ldr_format=ldr_format,
         hdr_format=hdr_format,
         animate=animate,
         fps=fps,
         separate_channels=separate_channels,
@@ -526,15 +530,15 @@
 
     input_paths = InputPaths(paths)
     if input_paths.has_directories():
         _resolve_directories(input_paths, not no_progress)
 
     task_runner: TaskRunner
     if num_workers is None or num_workers > 1:
-        task_runner = ParallelRunner(max_workers=num_workers, initializer=Pipeline.initialize)
+        task_runner = ParallelRunner(max_workers=num_workers, initializer=pipeline_initializer)
     else:
         task_runner = SequentialRunner()
 
     if output_file:
         tasks = _get_tasks(pipeline, input_paths, output_file=output_file)
     else:
         tasks = _get_tasks(pipeline, input_paths, output_directory=output_directory)
```

### Comparing `no_vtf-3.1.0/no_vtf/parser/generated/vtf.py` & `no_vtf-3.1.1/no_vtf/parser/generated/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/pipeline/pipeline.py` & `no_vtf-3.1.1/no_vtf/pipeline/pipeline.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import pathlib
 import re
 
 from collections import defaultdict
 from collections.abc import Sequence
 from dataclasses import dataclass
-from typing import Generic, Literal, Optional, TypeVar, overload
+from typing import Generic, Literal, Optional, TypeVar, Union, overload
 
 from no_vtf.image.channel_separator import ChannelSeparator
 from no_vtf.image.image import Image, ImageDataTypes
 from no_vtf.io.bytes import BytesIO
 from no_vtf.io.image import ImageIO
 from no_vtf.io.io import IO
 from no_vtf.texture.decoder.decoder import TextureDecoder
@@ -23,15 +23,15 @@
 from no_vtf.texture.namer.namer import TextureNamer
 
 _A_contra = TypeVar("_A_contra", contravariant=True)
 _I = TypeVar("_I", bound=ImageDataTypes)
 _T = TypeVar("_T")
 
 
-@dataclass(frozen=True, kw_only=True)
+@dataclass(kw_only=True)
 class Pipeline(Generic[_T, _I]):
     @dataclass(frozen=True, kw_only=True)
     class Receipt:
         io_done: bool
 
     input_extension_pattern: Optional[re.Pattern[str]] = None
 
@@ -51,16 +51,34 @@
 
     extractor: TextureExtractor[_T]
     filter: Optional[TextureFilter[_T]]
     decoder: TextureDecoder[_T, _I]
     namer: TextureNamer[_T]
 
     @classmethod
-    def initialize(cls) -> None:
-        IO.initialize()
+    def initialize(cls, formats: Optional[Sequence[str]] = None) -> None:
+        if formats:
+            formats = list(
+                filter(lambda format: format not in (cls.FORMAT_RAW, cls.FORMAT_SKIP), formats)
+            )
+
+        ImageIO.initialize(formats)
+
+    def __post_init__(self) -> None:
+        self._ldr_io = self._create_io(self.ldr_format)
+        self._hdr_io = self._create_io(self.hdr_format)
+
+    def _create_io(self, output_format: str) -> Union[BytesIO, ImageIO, None]:
+        if output_format == self.FORMAT_RAW:
+            return BytesIO()
+
+        if output_format != self.FORMAT_SKIP:
+            return ImageIO(format=output_format, compress=self.compress, fps=self.fps)
+
+        return None
 
     @overload
     def __call__(self, input_file: pathlib.Path, *, output_file: pathlib.Path) -> Pipeline.Receipt:
         ...
 
     @overload
     def __call__(
@@ -133,14 +151,18 @@
                 images_by_output_path[image_output_file].append(image)
         return images_by_output_path
 
     def _get_image_format(self, image: Image[_I]) -> str:
         image_format = self.hdr_format if image.dynamic_range == "hdr" else self.ldr_format
         return image_format
 
+    def _get_io(self, image: Image[_I]) -> Union[BytesIO, ImageIO, None]:
+        io = self._hdr_io if image.dynamic_range == "hdr" else self._ldr_io
+        return io
+
     def _get_output_file(
         self,
         input_file: pathlib.Path,
         output_directory: pathlib.Path,
         texture: _T,
         image: Image[_I],
         *,
@@ -161,51 +183,53 @@
     def _process_individual(
         self, images_by_output_path: dict[pathlib.Path, list[Image[_I]]]
     ) -> bool:
         io_done = False
 
         for image_output_path, images in images_by_output_path.items():
             for image in images:
-                image_format = self._get_image_format(image)
-                if _compare_formats(image_format, self.FORMAT_RAW):
+                io = self._get_io(image)
+                if not io:
+                    continue
+
+                if isinstance(io, BytesIO):
                     assert image.raw, "image must have raw data set"
-                    io_done = self._do_io(BytesIO(), image_output_path, [image.raw]) or io_done
+                    io_done = self._do_io(io, image_output_path, [image.raw]) or io_done
                 else:
-                    image_io = ImageIO(format=image_format, compress=self.compress, fps=self.fps)
-                    io_done = self._do_io(image_io, image_output_path, [image]) or io_done
+                    io_done = self._do_io(io, image_output_path, [image]) or io_done
 
         return io_done
 
     def _process_sequences(
         self, images_by_output_path: dict[pathlib.Path, list[Image[_I]]]
     ) -> bool:
         io_done = False
 
         for image_output_path, images in images_by_output_path.items():
             if not images:
                 continue
 
-            assert (
-                len(set(map(self._get_image_format, images))) == 1
-            ), "image format must be the same for all images"
-            image_format = self._get_image_format(images[0])
+            io = self._get_io(images[0])
+            for image in images:
+                assert self._get_io(image) == io, "IO must be the same for all images"
+            if not io:
+                continue
 
-            if _compare_formats(image_format, self.FORMAT_RAW):
+            if isinstance(io, BytesIO):
                 raw_sequence = []
                 for image in images:
                     assert image.raw, "image must have raw data set"
                     raw_sequence.append(image.raw)
 
-                io_done = self._do_io(BytesIO(), image_output_path, raw_sequence) or io_done
+                io_done = self._do_io(io, image_output_path, raw_sequence) or io_done
             else:
                 if any(map(lambda image: image.dynamic_range == "hdr", images)):
                     raise RuntimeError("Animating HDR textures is not supported")
 
-                image_io = ImageIO(format=image_format, compress=self.compress, fps=self.fps)
-                io_done = self._do_io(image_io, image_output_path, images) or io_done
+                io_done = self._do_io(io, image_output_path, images) or io_done
 
         return io_done
 
     def _do_io(self, io: IO[_A_contra], path: pathlib.Path, sequence: Sequence[_A_contra]) -> bool:
         io_done = False
 
         if self.write is not False:
```

### Comparing `no_vtf-3.1.0/no_vtf/task_runner/parallel.py` & `no_vtf-3.1.1/no_vtf/task_runner/parallel.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,33 +4,45 @@
 
 import functools
 import multiprocessing
 import signal
 
 from collections.abc import Callable, Iterable, Sequence
 from dataclasses import dataclass
-from typing import Optional, TypeVar, Union
+from typing import ClassVar, Optional, TypeVar, Union
 
 from no_vtf.task_runner.sequential import SequentialRunner
 from no_vtf.task_runner.task_runner import TaskRunner
 
 _A_co = TypeVar("_A_co", covariant=True)
 
 
 @dataclass(frozen=True, kw_only=True)
 class ParallelRunner(TaskRunner):
-    max_workers: Optional[int] = None
-    initializer: Optional[Callable[[], None]] = None
+    _multiprocessing_initialized: ClassVar[bool] = False
 
     @classmethod
-    def _initialize(cls) -> None:
-        multiprocessing.freeze_support()
+    def initialize(cls, *, _recursive: bool = True) -> None:
+        super().initialize(_recursive=False)
+
+        if not ParallelRunner._multiprocessing_initialized:
+            multiprocessing.freeze_support()
+            ParallelRunner._multiprocessing_initialized = True
+
+        if _recursive:
+            for subclass in cls.__subclasses__():
+                subclass.initialize()
+
+    max_workers: Optional[int] = None
+    initializer: Optional[Callable[[], None]] = None
 
     def __post_init__(self) -> None:
-        assert self._is_initialized(), "TaskRunner.initialize() must be called early"
+        assert (
+            ParallelRunner._multiprocessing_initialized
+        ), "ParallelRunner.initialize() must be called early"
 
     def __call__(
         self, tasks: Sequence[TaskRunner.Task[_A_co]]
     ) -> Iterable[tuple[TaskRunner.Task[_A_co], Union[_A_co, Exception]]]:
         initializer = functools.partial(ParallelRunner._worker_initializer, self.initializer)
         with multiprocessing.Pool(self.max_workers, initializer=initializer) as pool:
             for task, result in pool.imap_unordered(SequentialRunner.process, tasks):
```

### Comparing `no_vtf-3.1.0/no_vtf/task_runner/sequential.py` & `no_vtf-3.1.1/no_vtf/task_runner/sequential.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/task_runner/task_runner.py` & `no_vtf-3.1.1/no_vtf/task_runner/task_runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,42 +2,31 @@
 #
 # SPDX-License-Identifier: LGPL-3.0-or-later
 
 from __future__ import annotations
 
 from abc import abstractmethod
 from collections.abc import Iterable, Sequence
-from typing import ClassVar, Protocol, TypeVar, Union
+from typing import Protocol, TypeVar, Union
 
 import no_vtf.task_runner  # noqa: F401  # define all task runners for TaskRunner.initialize()
 
 _A_co = TypeVar("_A_co", covariant=True)
 
 
 class TaskRunner:
     class Task(Protocol[_A_co]):
         @abstractmethod
         def __call__(self) -> _A_co:
             ...
 
-    _initialized: ClassVar[bool] = False
-
-    @classmethod
-    def initialize(cls) -> None:
-        for subclass in cls.__subclasses__():
-            subclass._initialize()
-
-        cls._initialized = True
-
-    @classmethod
-    def _is_initialized(cls) -> bool:
-        return cls._initialized
-
     @classmethod
-    def _initialize(cls) -> None:
-        pass
+    def initialize(cls, *, _recursive: bool = True) -> None:
+        if _recursive:
+            for subclass in cls.__subclasses__():
+                subclass.initialize()
 
     @abstractmethod
     def __call__(
         self, tasks: Sequence[TaskRunner.Task[_A_co]]
     ) -> Iterable[tuple[TaskRunner.Task[_A_co], Union[_A_co, Exception]]]:
         ...
```

### Comparing `no_vtf-3.1.0/no_vtf/texture/decoder/vtf.py` & `no_vtf-3.1.1/no_vtf/texture/decoder/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/texture/extractor/vtf.py` & `no_vtf-3.1.1/no_vtf/texture/extractor/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/texture/filter/filter.py` & `no_vtf-3.1.1/no_vtf/texture/filter/filter.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/texture/filter/vtf.py` & `no_vtf-3.1.1/no_vtf/texture/filter/vtf.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,16 +25,21 @@
                 len(set(map(lambda texture: texture.num_mipmaps, textures))) == 1
             ), "num_mipmaps must be the same for all filtered textures"
             length = textures[0].num_mipmaps
         else:
             length = max(map(lambda texture: texture.mipmap_index, textures)) + 1
 
         indices = range(*self.mipmap_levels.indices(length))
-        textures = list(filter(lambda texture: texture.mipmap_index in indices, textures))
-        return textures
+
+        textures_filtered: list[VtfTexture] = []
+        for index in indices:
+            textures_filtered.extend(
+                filter(lambda texture: texture.mipmap_index == index, textures)
+            )
+        return textures_filtered
 
 
 @dataclass(frozen=True, kw_only=True)
 class VtfResolutionFilter(TextureFilter[VtfTexture]):
     min: Optional[int] = None
     max: Optional[int] = None
 
@@ -93,16 +98,18 @@
             return []
 
         assert (
             len(set(map(lambda texture: texture.num_frames, textures))) == 1
         ), "num_frames must be the same for all filtered textures"
         indices = range(*self.frames.indices(textures[0].num_frames))
 
-        textures = list(filter(lambda texture: texture.frame_index in indices, textures))
-        return textures
+        textures_filtered: list[VtfTexture] = []
+        for index in indices:
+            textures_filtered.extend(filter(lambda texture: texture.frame_index == index, textures))
+        return textures_filtered
 
 
 @dataclass(frozen=True, kw_only=True)
 class VtfFaceFilter(TextureFilter[VtfTexture]):
     faces: slice
 
     def __call__(self, textures: Sequence[VtfTexture]) -> Sequence[VtfTexture]:
@@ -110,16 +117,18 @@
             return []
 
         assert (
             len(set(map(lambda texture: texture.num_faces, textures))) == 1
         ), "num_faces must be the same for all filtered textures"
         indices = range(*self.faces.indices(textures[0].num_faces))
 
-        textures = list(filter(lambda texture: texture.face_index in indices, textures))
-        return textures
+        textures_filtered: list[VtfTexture] = []
+        for index in indices:
+            textures_filtered.extend(filter(lambda texture: texture.face_index == index, textures))
+        return textures_filtered
 
 
 @dataclass(frozen=True, kw_only=True)
 class VtfSliceFilter(TextureFilter[VtfTexture]):
     slices: slice
 
     def __call__(self, textures: Sequence[VtfTexture]) -> Sequence[VtfTexture]:
@@ -127,9 +136,11 @@
             return []
 
         assert (
             len(set(map(lambda texture: texture.num_slices, textures))) == 1
         ), "num_slices must be the same for all filtered textures"
         indices = range(*self.slices.indices(textures[0].num_slices))
 
-        textures = list(filter(lambda texture: texture.slice_index in indices, textures))
-        return textures
+        textures_filtered: list[VtfTexture] = []
+        for index in indices:
+            textures_filtered.extend(filter(lambda texture: texture.slice_index == index, textures))
+        return textures_filtered
```

### Comparing `no_vtf-3.1.0/no_vtf/texture/namer/vtf.py` & `no_vtf-3.1.1/no_vtf/texture/namer/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf/texture/vtf.py` & `no_vtf-3.1.1/no_vtf/texture/vtf.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/no_vtf.egg-info/PKG-INFO` & `no_vtf-3.1.1/no_vtf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: no-vtf
-Version: 3.1.0
+Version: 3.1.1
 Summary: Valve Texture Format Converter
 Home-page: https://sr.ht/~b5327157/no_vtf
 Author: b5327157
 Author-email: b5327157@protonmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Download, https://sr.ht/~b5327157/no_vtf/#application-bundle
 Project-URL: Changelog, https://git.sr.ht/~b5327157/no_vtf/refs
@@ -25,15 +25,15 @@
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSES/GPL-3.0-or-later.txt
 
 # no_vtf
 
-Say no to [Source Engine](https://developer.valvesoftware.com/wiki/Source)'s [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
+Say no to [.vtf](https://developer.valvesoftware.com/wiki/Valve_Texture_Format) – convert it to one of the standard image formats.
 
 ![Badge showing supported Python versions](https://img.shields.io/pypi/pyversions/no_vtf?style=flat-square)
 [![Badge showing package version on PyPI](https://img.shields.io/pypi/v/no_vtf?style=flat-square)](https://pypi.org/project/no-vtf/)
 [![Badge showing number of monthly downloads from PyPI](https://img.shields.io/pypi/dm/no_vtf?style=flat-square)](https://pypistats.org/packages/no-vtf)
 [![Badge showing source code repository hosted on SourceHut](https://img.shields.io/badge/sr.ht-repository-white?labelColor=212529&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiIHN0YW5kYWxvbmU9Im5vIj8+CjxzdmcKICAgdmlld0JveD0iMCAwIDUxMiA1MTIiCiAgIHZlcnNpb249IjEuMSIKICAgaWQ9InN2ZzUxIgogICBzb2RpcG9kaTpkb2NuYW1lPSJzb3VyY2VodXQtd2hpdGUuc3ZnIgogICBpbmtzY2FwZTp2ZXJzaW9uPSIxLjEgKGM2OGUyMmMzODcsIDIwMjEtMDUtMjMpIgogICB4bWxuczppbmtzY2FwZT0iaHR0cDovL3d3dy5pbmtzY2FwZS5vcmcvbmFtZXNwYWNlcy9pbmtzY2FwZSIKICAgeG1sbnM6c29kaXBvZGk9Imh0dHA6Ly9zb2RpcG9kaS5zb3VyY2Vmb3JnZS5uZXQvRFREL3NvZGlwb2RpLTAuZHRkIgogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciCiAgIHhtbG5zOnN2Zz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogIDxkZWZzCiAgICAgaWQ9ImRlZnM1NSIgLz4KICA8c29kaXBvZGk6bmFtZWR2aWV3CiAgICAgaWQ9Im5hbWVkdmlldzUzIgogICAgIHBhZ2Vjb2xvcj0iIzUwNTA1MCIKICAgICBib3JkZXJjb2xvcj0iI2ZmZmZmZiIKICAgICBib3JkZXJvcGFjaXR5PSIxIgogICAgIGlua3NjYXBlOnBhZ2VzaGFkb3c9IjAiCiAgICAgaW5rc2NhcGU6cGFnZW9wYWNpdHk9IjAiCiAgICAgaW5rc2NhcGU6cGFnZWNoZWNrZXJib2FyZD0iMSIKICAgICBzaG93Z3JpZD0iZmFsc2UiCiAgICAgaW5rc2NhcGU6em9vbT0iMS42NTQyOTY5IgogICAgIGlua3NjYXBlOmN4PSIyNTYiCiAgICAgaW5rc2NhcGU6Y3k9IjI1NiIKICAgICBpbmtzY2FwZTp3aW5kb3ctd2lkdGg9IjE5MjAiCiAgICAgaW5rc2NhcGU6d2luZG93LWhlaWdodD0iMTA1OSIKICAgICBpbmtzY2FwZTp3aW5kb3cteD0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3cteT0iMCIKICAgICBpbmtzY2FwZTp3aW5kb3ctbWF4aW1pemVkPSIxIgogICAgIGlua3NjYXBlOmN1cnJlbnQtbGF5ZXI9InN2ZzUxIiAvPgogIDxwYXRoCiAgICAgZD0iTTI1NiA4QzExOSA4IDggMTE5IDggMjU2czExMSAyNDggMjQ4IDI0OCAyNDgtMTExIDI0OC0yNDhTMzkzIDggMjU2IDh6bTAgNDQ4Yy0xMTAuNSAwLTIwMC04OS41LTIwMC0yMDBTMTQ1LjUgNTYgMjU2IDU2czIwMCA4OS41IDIwMCAyMDAtODkuNSAyMDAtMjAwIDIwMHoiCiAgICAgaWQ9InBhdGg0OSIKICAgICBzdHlsZT0iZmlsbDojZmZmZmZmIiAvPgo8L3N2Zz4K)](https://sr.ht/~b5327157/no_vtf)
 [![Badge showing builds.sr.ht status](https://builds.sr.ht/~b5327157/no_vtf.svg?search=tags:master)](https://builds.sr.ht/~b5327157/no_vtf?search=tags:master)
 [![Badge showing REUSE compliance status](https://api.reuse.software/badge/git.sr.ht/~b5327157/no_vtf)](https://api.reuse.software/info/git.sr.ht/~b5327157/no_vtf)
@@ -126,15 +126,15 @@
 no_vtf --help
 ```
 
 ## Supported formats
 
 ### Input
 
-All textures installed with [Team Fortress 2](https://store.steampowered.com/app/440/Team_Fortress_2/), [Source Filmmaker](https://store.steampowered.com/app/1840/Source_Filmmaker/) and [Portal 2](https://store.steampowered.com/app/620/Portal_2/) can be converted with the supported format set.
+All textures installed with many [Source Engine](https://developer.valvesoftware.com/wiki/Source) games, including [Team Fortress 2](https://store.steampowered.com/app/440/Team_Fortress_2/), [Source Filmmaker](https://store.steampowered.com/app/1840/Source_Filmmaker/) and [Portal 2](https://store.steampowered.com/app/620/Portal_2/), can be converted with the supported format set.
 
 - `RGBA8888`
 - `ABGR8888`
 - `RGB888`
 - `BGR888`
 - `I8`
 - `IA88`
```

### Comparing `no_vtf-3.1.0/no_vtf.egg-info/SOURCES.txt` & `no_vtf-3.1.1/no_vtf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/noxfile.py` & `no_vtf-3.1.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/pyproject.toml` & `no_vtf-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/resources/docs/screencast.gif` & `no_vtf-3.1.1/resources/docs/screencast.gif`

 * *Files identical despite different names*

### Comparing `no_vtf-3.1.0/setup.cfg` & `no_vtf-3.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 	Ticket tracker = https://todo.sr.ht/~b5327157/no_vtf
 	Wiki = https://developer.valvesoftware.com/wiki/no_vtf
 url = https://sr.ht/~b5327157/no_vtf
 
 [options]
 install_requires = 
 	alive-progress >= 3.1.3, < 4
-	click >= 8.1.3, < 9
+	click >= 8.1.3, != 8.1.4, < 9
 	imageio[pillow] >= 2.29.0, < 3
 	kaitaistruct >= 0.10, < 1
 	numpy >= 1.24.3, < 2
 	Pillow >= 9.5.0, < 10
 	tifffile >= 2023.4.12, < 2024
 packages = find:
 py_modules =
```

