# Comparing `tmp/sdr-0.0.0.tar.gz` & `tmp/sdr-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/sdr/sdr/dist/.tmp-v0d49gvn/sdr-0.0.0.tar", last modified: Thu Jul  6 23:04:58 2023, max compression
+gzip compressed data, was "/home/runner/work/sdr/sdr/dist/.tmp-hwqds3xa/sdr-0.0.1.tar", last modified: Sun Jul  9 21:17:08 2023, max compression
```

## Comparing `sdr-0.0.0.tar` & `sdr-0.0.1.tar`

### file list

```diff
@@ -1,24 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:58.000000 sdr-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:58.000000 sdr-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:58.000000 sdr-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-06 23:04:39.000000 sdr-0.0.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-06 23:04:39.000000 sdr-0.0.0/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-06 23:04:39.000000 sdr-0.0.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-06 23:04:39.000000 sdr-0.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:58.000000 sdr-0.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-06 23:04:39.000000 sdr-0.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-06 23:04:39.000000 sdr-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-06 23:04:58.000000 sdr-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 23:04:39.000000 sdr-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-06 23:04:39.000000 sdr-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 23:04:39.000000 sdr-0.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 23:04:58.000000 sdr-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:58.000000 sdr-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:58.000000 sdr-0.0.0/src/sdr/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-06 23:04:39.000000 sdr-0.0.0/src/sdr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-06 23:04:58.000000 sdr-0.0.0/src/sdr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 23:04:58.000000 sdr-0.0.0/src/sdr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-06 23:04:58.000000 sdr-0.0.0/src/sdr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 23:04:58.000000 sdr-0.0.0/src/sdr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 23:04:58.000000 sdr-0.0.0/src/sdr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-06 23:04:58.000000 sdr-0.0.0/src/sdr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-09 21:16:50.000000 sdr-0.0.1/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-09 21:16:50.000000 sdr-0.0.1/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-09 21:16:50.000000 sdr-0.0.1/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-09 21:16:50.000000 sdr-0.0.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-07-09 21:16:50.000000 sdr-0.0.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-09 21:16:50.000000 sdr-0.0.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-09 21:16:50.000000 sdr-0.0.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-09 21:16:50.000000 sdr-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-09 21:17:08.000000 sdr-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-09 21:16:50.000000 sdr-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/_static/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15589 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   658057 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/examples/farrow-resampler.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   865117 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/examples/iir-filter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   566094 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/examples/phase-locked-loop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/docs/release-notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/release-notes/v0.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/release-notes/versioning.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-09 21:16:50.000000 sdr-0.0.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-09 21:16:50.000000 sdr-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-09 21:16:50.000000 sdr-0.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 21:17:08.000000 sdr-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/src/sdr/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-09 21:16:50.000000 sdr-0.0.1/src/sdr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-09 21:16:50.000000 sdr-0.0.1/src/sdr/_farrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-09 21:16:50.000000 sdr-0.0.1/src/sdr/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-07-09 21:16:50.000000 sdr-0.0.1/src/sdr/_iir_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-09 21:16:50.000000 sdr-0.0.1/src/sdr/_loop_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-07-09 21:16:50.000000 sdr-0.0.1/src/sdr/_nco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8346 2023-07-09 21:16:50.000000 sdr-0.0.1/src/sdr/_pll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-09 21:17:08.000000 sdr-0.0.1/src/sdr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/src/sdr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-09 21:17:08.000000 sdr-0.0.1/src/sdr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-09 21:17:08.000000 sdr-0.0.1/src/sdr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 21:17:08.000000 sdr-0.0.1/src/sdr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-09 21:17:08.000000 sdr-0.0.1/src/sdr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 21:17:08.000000 sdr-0.0.1/src/sdr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 21:17:08.000000 sdr-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-09 21:16:50.000000 sdr-0.0.1/tests/test_dds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-07-09 21:16:50.000000 sdr-0.0.1/tests/test_farrow_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-09 21:16:50.000000 sdr-0.0.1/tests/test_iir_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-09 21:16:50.000000 sdr-0.0.1/tests/test_loop_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-09 21:16:50.000000 sdr-0.0.1/tests/test_nco.py
```

### Comparing `sdr-0.0.0/.github/workflows/build.yaml` & `sdr-0.0.1/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `sdr-0.0.0/.github/workflows/lint.yaml` & `sdr-0.0.1/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `sdr-0.0.0/.github/workflows/release.yaml` & `sdr-0.0.1/.github/workflows/release.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -6,59 +6,58 @@
       - v*
 
 jobs:
   build:
     name: Build the package
     uses: ./.github/workflows/build.yaml
 
-  # docs:
-  #   name: Build the docs
-  #   uses: ./.github/workflows/docs.yaml
-
-  # release:
-  #   name: Create GitHub release
-  #   runs-on: ubuntu-latest
-  #   steps:
-  #     - uses: actions/checkout@v3
-  #       with:
-  #         fetch-depth: 0  # Fetch all commits and tags
-  #         ref: ${{ github.ref }}
-
-  #     - name: Get current version
-  #       id: current
-  #       run: |
-  #         version=$(git tag --sort=-version:refname | head -n 1)
-  #         echo "version=${version}" >> $GITHUB_OUTPUT
-
-  #     - name: Get previous version
-  #       id: previous
-  #       run: |
-  #         version=$(git tag --sort=-version:refname | head -n 2 | tail -1)
-  #         echo "version=${version}" >> $GITHUB_OUTPUT
-
-  #     - name: Construct release notes
-  #       run: |
-  #         # cp docs/release-notes/${{ steps.current.outputs.version }}.md release_notes.md
-  #         echo -e "\n## Commits\n" > release_notes.md
-  #         git log --oneline ${{ steps.previous.outputs.version }}..${{ steps.current.outputs.version }} >> release_notes.md
-
-  #     - name: Create GitHub release
-  #       uses: actions/create-release@v1
-  #       env:
-  #         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-  #       with:
-  #         tag_name: ${{ steps.current.outputs.version }}
-  #         release_name: galois ${{ steps.current.outputs.version }}
-  #         body_path: release_notes.md
-  #         draft: true
+  docs:
+    name: Build the docs
+    uses: ./.github/workflows/docs.yaml
+
+  release:
+    name: Create GitHub release
+    runs-on: ubuntu-latest
+    steps:
+      - uses: actions/checkout@v3
+        with:
+          fetch-depth: 0  # Fetch all commits and tags
+          ref: ${{ github.ref }}
+
+      - name: Get current version
+        id: current
+        run: |
+          version=$(git tag --sort=-version:refname | head -n 1)
+          echo "version=${version}" >> $GITHUB_OUTPUT
+
+      - name: Get previous version
+        id: previous
+        run: |
+          version=$(git tag --sort=-version:refname | head -n 2 | tail -1)
+          echo "version=${version}" >> $GITHUB_OUTPUT
+
+      - name: Construct release notes
+        run: |
+          # cp docs/release-notes/${{ steps.current.outputs.version }}.md release_notes.md
+          echo -e "\n## Commits\n" > release_notes.md
+          git log --oneline ${{ steps.previous.outputs.version }}..${{ steps.current.outputs.version }} >> release_notes.md
+
+      - name: Create GitHub release
+        uses: actions/create-release@v1
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+        with:
+          tag_name: ${{ steps.current.outputs.version }}
+          release_name: sdr ${{ steps.current.outputs.version }}
+          body_path: release_notes.md
+          draft: true
 
   publish:
     name: Publish on PyPI
-    # needs: [build, release]
-    needs: build
+    needs: [build, release]
     runs-on: ubuntu-latest
     steps:
       - name: Download build artifacts
         uses: actions/download-artifact@v3
         with:
           name: dist
           path: dist/
```

### Comparing `sdr-0.0.0/LICENSE` & `sdr-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdr-0.0.0/pyproject.toml` & `sdr-0.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -34,29 +34,31 @@
     "Intended Audience :: Telecommunications Industry",
     "License :: OSI Approved :: MIT License",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    # "Programming Language :: Python :: 3.7",
-    # "Programming Language :: Python :: 3.8",
-    # "Programming Language :: Python :: 3.9",
-    # "Programming Language :: Python :: 3.10",
-    # "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Security :: Cryptography",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 requires-python = ">=3.7"
 dependencies = [
-    # "numpy >= 1.21.0, < 1.25",  # v1.21.0 is needed for dtype support of ufuncs, see https://numpy.org/devdocs/release/1.21.0-notes.html#ufunc-signature-and-dtype-generalization-and-casting
+    "numpy >= 1.21.0",
+    "scipy",
+    "matplotlib",
     # "numba >= 0.55, < 0.58",  # v0.55 is needed for support of NumPy 1.21
-    # "typing_extensions >= 4.0.0",  # v4.0.0 is needed for use of Self (Python 3.11+) and Literal (Python 3.8+)
+    "typing_extensions >= 4.0.0",  # v4.0.0 is needed for use of Self (Python 3.11+) and Literal (Python 3.8+)
 ]
 dynamic = ["version"]
 
 # [project.optional-dependencies]
 # dev = [
 #     "pylint >= 2.14",
 #     "black >= 22.8.0",
@@ -71,15 +73,15 @@
 [project.urls]
 Homepage = "https://github.com/mhostetter/sdr"
 Source = "https://github.com/mhostetter/sdr"
 Issues = "https://github.com/mhostetter/sdr/issues"
 Documentation = "https://mhostetter.github.io/sdr/latest/"
 Discuss = "https://github.com/mhostetter/sdr/discussions"
 # Changelog = "https://mhostetter.github.io/sdr/latest/release-notes/versioning/"
-# Twitter = "https://twitter.com/galois_py"
+Twitter = "https://twitter.com/sdr_py"
 
 [tool.setuptools_scm]
 write_to = "src/sdr/_version.py"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
@@ -103,14 +105,15 @@
     "protected-access",
     "too-many-ancestors",
     "too-many-arguments",
     "too-many-branches",
     "too-many-instance-attributes",
     "too-many-lines",
     "too-many-locals",
+    "too-many-public-methods",
     "unneeded-not",
 ]
 min-similarity-lines = 100
 max-line-length = 120
 
 [tool.black]
 line-length = 120
```

