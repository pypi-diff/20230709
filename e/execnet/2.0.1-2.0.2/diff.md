# Comparing `tmp/execnet-2.0.1.tar.gz` & `tmp/execnet-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Jul  8 11:52:44 2023, max compression
+gzip compressed data, last modified: Sun Jul  9 15:04:38 2023, max compression
```

## Comparing `execnet-2.0.1.tar` & `execnet-2.0.2.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0     3197 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/Makefile
--rw-r--r--   0        0        0        2 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/__init__.py
--rw-r--r--   0        0        0     8213 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/basics.rst
--rw-r--r--   0        0        0       98 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/changelog.rst
--rw-r--r--   0        0        0     6160 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/conf.py
--rw-r--r--   0        0        0      603 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/examples.rst
--rw-r--r--   0        0        0     1240 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/implnotes.rst
--rw-r--r--   0        0        0     3374 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/index.rst
--rw-r--r--   0        0        0      798 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/install.rst
--rw-r--r--   0        0        0      726 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/support.rst
--rw-r--r--   0        0        0    24123 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/_static/basic1.png
--rw-r--r--   0        0        0    10202 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/_static/codespeak.png
--rw-r--r--   0        0        0    36750 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/_static/execnet.png
--rw-r--r--   0        0        0    17805 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/_static/pythonring.png
--rw-r--r--   0        0        0      806 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/_templates/indexsidebar.html
--rw-r--r--   0        0        0     1298 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/_templates/layout.html
--rw-r--r--   0        0        0      379 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/conftest.py
--rw-r--r--   0        0        0      342 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/funcmultiplier.py
--rw-r--r--   0        0        0     4844 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/hybridpython.rst
--rw-r--r--   0        0        0      953 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/popen_read_multiple.py
--rw-r--r--   0        0        0      392 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/py3topy2.py
--rw-r--r--   0        0        0      671 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/redirect_remote_output.py
--rw-r--r--   0        0        0      142 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/remote1.py
--rw-r--r--   0        0        0      279 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/remotecmd.py
--rw-r--r--   0        0        0      243 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/servefiles.py
--rw-r--r--   0        0        0     3886 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/svn-sync-repo.py
--rw-r--r--   0        0        0     4859 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/sysinfo.py
--rw-r--r--   0        0        0     1348 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/taskserver.py
--rw-r--r--   0        0        0     2003 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/test_debug.rst
--rw-r--r--   0        0        0       47 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/test_funcmultiplier.py
--rw-r--r--   0        0        0     3504 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/test_group.rst
--rw-r--r--   0        0        0     6301 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/test_info.rst
--rw-r--r--   0        0        0     2990 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/test_multi.rst
--rw-r--r--   0        0        0      741 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/test_proxy.rst
--rw-r--r--   0        0        0      574 2023-07-08 11:52:44.000000 execnet-2.0.1/doc/example/test_ssh_fileserver.rst
--rw-r--r--   0        0        0      958 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/__init__.py
--rw-r--r--   0        0        0      160 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/_version.py
--rw-r--r--   0        0        0     7115 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/gateway.py
--rw-r--r--   0        0        0    51114 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/gateway_base.py
--rw-r--r--   0        0        0     2990 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/gateway_bootstrap.py
--rw-r--r--   0        0        0     6836 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/gateway_io.py
--rw-r--r--   0        0        0     2501 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/gateway_socket.py
--rw-r--r--   0        0        0    10291 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/multi.py
--rw-r--r--   0        0        0     7611 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/rsync.py
--rw-r--r--   0        0        0     3828 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/rsync_remote.py
--rw-r--r--   0        0        0     1788 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/xspec.py
--rw-r--r--   0        0        0        2 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/script/__init__.py
--rw-r--r--   0        0        0      418 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/script/loop_socketserver.py
--rw-r--r--   0        0        0      306 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/script/quitserver.py
--rw-r--r--   0        0        0     2480 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/script/shell.py
--rw-r--r--   0        0        0     3696 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/script/socketserver.py
--rw-r--r--   0        0        0     3044 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/script/socketserverservice.py
--rw-r--r--   0        0        0      186 2023-07-08 11:52:44.000000 execnet-2.0.1/src/execnet/script/xx.py
--rw-r--r--   0        0        0     5476 2023-07-08 11:52:44.000000 execnet-2.0.1/testing/conftest.py
--rw-r--r--   0        0        0    11537 2023-07-08 11:52:44.000000 execnet-2.0.1/testing/test_basics.py
--rw-r--r--   0        0        0    11840 2023-07-08 11:52:44.000000 execnet-2.0.1/testing/test_channel.py
--rw-r--r--   0        0        0      839 2023-07-08 11:52:44.000000 execnet-2.0.1/testing/test_compatibility_regressions.py
--rw-r--r--   0        0        0    16362 2023-07-08 11:52:44.000000 execnet-2.0.1/testing/test_gateway.py
--rw-r--r--   0        0        0     7526 2023-07-08 11:52:44.000000 execnet-2.0.1/testing/test_multi.py
--rw-r--r--   0        0        0     9731 2023-07-08 11:52:44.000000 execnet-2.0.1/testing/test_rsync.py
--rw-r--r--   0        0        0     3621 2023-07-08 11:52:44.000000 execnet-2.0.1/testing/test_serializer.py
--rw-r--r--   0        0        0     4028 2023-07-08 11:52:44.000000 execnet-2.0.1/testing/test_termination.py
--rw-r--r--   0        0        0     4890 2023-07-08 11:52:44.000000 execnet-2.0.1/testing/test_threadpool.py
--rw-r--r--   0        0        0     8636 2023-07-08 11:52:44.000000 execnet-2.0.1/testing/test_xspec.py
--rw-r--r--   0        0        0      188 2023-07-08 11:52:44.000000 execnet-2.0.1/.gitignore
--rw-r--r--   0        0        0     1054 2023-07-08 11:52:44.000000 execnet-2.0.1/LICENSE
--rw-r--r--   0        0        0     1593 2023-07-08 11:52:44.000000 execnet-2.0.1/README.rst
--rw-r--r--   0        0        0     1545 2023-07-08 11:52:44.000000 execnet-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2923 2023-07-08 11:52:44.000000 execnet-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      603 2023-07-09 15:04:38.000000 execnet-2.0.2/tox.ini
+-rw-r--r--   0        0        0     3197 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/Makefile
+-rw-r--r--   0        0        0        2 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/__init__.py
+-rw-r--r--   0        0        0     8213 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/basics.rst
+-rw-r--r--   0        0        0       98 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/changelog.rst
+-rw-r--r--   0        0        0     6160 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/conf.py
+-rw-r--r--   0        0        0      603 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/examples.rst
+-rw-r--r--   0        0        0     1240 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/implnotes.rst
+-rw-r--r--   0        0        0     3374 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/index.rst
+-rw-r--r--   0        0        0      798 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/install.rst
+-rw-r--r--   0        0        0      726 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/support.rst
+-rw-r--r--   0        0        0    24123 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_static/basic1.png
+-rw-r--r--   0        0        0    10202 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_static/codespeak.png
+-rw-r--r--   0        0        0    36750 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_static/execnet.png
+-rw-r--r--   0        0        0    17805 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_static/pythonring.png
+-rw-r--r--   0        0        0      806 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_templates/indexsidebar.html
+-rw-r--r--   0        0        0     1298 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/_templates/layout.html
+-rw-r--r--   0        0        0      379 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/conftest.py
+-rw-r--r--   0        0        0      342 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/funcmultiplier.py
+-rw-r--r--   0        0        0     4844 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/hybridpython.rst
+-rw-r--r--   0        0        0      953 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/popen_read_multiple.py
+-rw-r--r--   0        0        0      392 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/py3topy2.py
+-rw-r--r--   0        0        0      671 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/redirect_remote_output.py
+-rw-r--r--   0        0        0      142 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/remote1.py
+-rw-r--r--   0        0        0      279 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/remotecmd.py
+-rw-r--r--   0        0        0      243 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/servefiles.py
+-rw-r--r--   0        0        0     3886 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/svn-sync-repo.py
+-rw-r--r--   0        0        0     4859 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/sysinfo.py
+-rw-r--r--   0        0        0     1348 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/taskserver.py
+-rw-r--r--   0        0        0     2003 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_debug.rst
+-rw-r--r--   0        0        0       47 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_funcmultiplier.py
+-rw-r--r--   0        0        0     3504 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_group.rst
+-rw-r--r--   0        0        0     6301 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_info.rst
+-rw-r--r--   0        0        0     2990 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_multi.rst
+-rw-r--r--   0        0        0      741 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_proxy.rst
+-rw-r--r--   0        0        0      574 2023-07-09 15:04:38.000000 execnet-2.0.2/doc/example/test_ssh_fileserver.rst
+-rw-r--r--   0        0        0      958 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/__init__.py
+-rw-r--r--   0        0        0      160 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/_version.py
+-rw-r--r--   0        0        0     7115 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/gateway.py
+-rw-r--r--   0        0        0    51114 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/gateway_base.py
+-rw-r--r--   0        0        0     2990 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/gateway_bootstrap.py
+-rw-r--r--   0        0        0     6836 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/gateway_io.py
+-rw-r--r--   0        0        0     2501 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/gateway_socket.py
+-rw-r--r--   0        0        0    10291 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/multi.py
+-rw-r--r--   0        0        0     7611 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/rsync.py
+-rw-r--r--   0        0        0     3828 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/rsync_remote.py
+-rw-r--r--   0        0        0     1788 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/xspec.py
+-rw-r--r--   0        0        0        2 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/__init__.py
+-rw-r--r--   0        0        0      418 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/loop_socketserver.py
+-rw-r--r--   0        0        0      306 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/quitserver.py
+-rw-r--r--   0        0        0     2480 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/shell.py
+-rw-r--r--   0        0        0     3696 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/socketserver.py
+-rw-r--r--   0        0        0     3044 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/socketserverservice.py
+-rw-r--r--   0        0        0      186 2023-07-09 15:04:38.000000 execnet-2.0.2/src/execnet/script/xx.py
+-rw-r--r--   0        0        0     5476 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/conftest.py
+-rw-r--r--   0        0        0    11537 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_basics.py
+-rw-r--r--   0        0        0    11840 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_channel.py
+-rw-r--r--   0        0        0      839 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_compatibility_regressions.py
+-rw-r--r--   0        0        0    16362 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_gateway.py
+-rw-r--r--   0        0        0     7526 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_multi.py
+-rw-r--r--   0        0        0     9731 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_rsync.py
+-rw-r--r--   0        0        0     3621 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_serializer.py
+-rw-r--r--   0        0        0     4028 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_termination.py
+-rw-r--r--   0        0        0     4890 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_threadpool.py
+-rw-r--r--   0        0        0     8636 2023-07-09 15:04:38.000000 execnet-2.0.2/testing/test_xspec.py
+-rw-r--r--   0        0        0      188 2023-07-09 15:04:38.000000 execnet-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1054 2023-07-09 15:04:38.000000 execnet-2.0.2/LICENSE
+-rw-r--r--   0        0        0     1593 2023-07-09 15:04:38.000000 execnet-2.0.2/README.rst
+-rw-r--r--   0        0        0     1559 2023-07-09 15:04:38.000000 execnet-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2923 2023-07-09 15:04:38.000000 execnet-2.0.2/PKG-INFO
```

### Comparing `execnet-2.0.1/doc/Makefile` & `execnet-2.0.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/basics.rst` & `execnet-2.0.2/doc/basics.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/conf.py` & `execnet-2.0.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/examples.rst` & `execnet-2.0.2/doc/examples.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/implnotes.rst` & `execnet-2.0.2/doc/implnotes.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/index.rst` & `execnet-2.0.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/install.rst` & `execnet-2.0.2/doc/install.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/support.rst` & `execnet-2.0.2/doc/support.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/_static/basic1.png` & `execnet-2.0.2/doc/_static/basic1.png`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/_static/codespeak.png` & `execnet-2.0.2/doc/_static/codespeak.png`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/_static/execnet.png` & `execnet-2.0.2/doc/_static/execnet.png`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/_static/pythonring.png` & `execnet-2.0.2/doc/_static/pythonring.png`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/_templates/indexsidebar.html` & `execnet-2.0.2/doc/_templates/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/_templates/layout.html` & `execnet-2.0.2/doc/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/hybridpython.rst` & `execnet-2.0.2/doc/example/hybridpython.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/popen_read_multiple.py` & `execnet-2.0.2/doc/example/popen_read_multiple.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/redirect_remote_output.py` & `execnet-2.0.2/doc/example/redirect_remote_output.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/svn-sync-repo.py` & `execnet-2.0.2/doc/example/svn-sync-repo.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/sysinfo.py` & `execnet-2.0.2/doc/example/sysinfo.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/taskserver.py` & `execnet-2.0.2/doc/example/taskserver.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/test_debug.rst` & `execnet-2.0.2/doc/example/test_debug.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/test_group.rst` & `execnet-2.0.2/doc/example/test_group.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/test_info.rst` & `execnet-2.0.2/doc/example/test_info.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/test_multi.rst` & `execnet-2.0.2/doc/example/test_multi.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/test_proxy.rst` & `execnet-2.0.2/doc/example/test_proxy.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/doc/example/test_ssh_fileserver.rst` & `execnet-2.0.2/doc/example/test_ssh_fileserver.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/__init__.py` & `execnet-2.0.2/src/execnet/__init__.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/gateway.py` & `execnet-2.0.2/src/execnet/gateway.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/gateway_base.py` & `execnet-2.0.2/src/execnet/gateway_base.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/gateway_bootstrap.py` & `execnet-2.0.2/src/execnet/gateway_bootstrap.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/gateway_io.py` & `execnet-2.0.2/src/execnet/gateway_io.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/gateway_socket.py` & `execnet-2.0.2/src/execnet/gateway_socket.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/multi.py` & `execnet-2.0.2/src/execnet/multi.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/rsync.py` & `execnet-2.0.2/src/execnet/rsync.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/rsync_remote.py` & `execnet-2.0.2/src/execnet/rsync_remote.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/xspec.py` & `execnet-2.0.2/src/execnet/xspec.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/script/shell.py` & `execnet-2.0.2/src/execnet/script/shell.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/script/socketserver.py` & `execnet-2.0.2/src/execnet/script/socketserver.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/src/execnet/script/socketserverservice.py` & `execnet-2.0.2/src/execnet/script/socketserverservice.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/testing/conftest.py` & `execnet-2.0.2/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/testing/test_basics.py` & `execnet-2.0.2/testing/test_basics.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/testing/test_channel.py` & `execnet-2.0.2/testing/test_channel.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/testing/test_compatibility_regressions.py` & `execnet-2.0.2/testing/test_compatibility_regressions.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/testing/test_gateway.py` & `execnet-2.0.2/testing/test_gateway.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/testing/test_multi.py` & `execnet-2.0.2/testing/test_multi.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/testing/test_rsync.py` & `execnet-2.0.2/testing/test_rsync.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/testing/test_serializer.py` & `execnet-2.0.2/testing/test_serializer.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/testing/test_termination.py` & `execnet-2.0.2/testing/test_termination.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/testing/test_threadpool.py` & `execnet-2.0.2/testing/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/testing/test_xspec.py` & `execnet-2.0.2/testing/test_xspec.py`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/LICENSE` & `execnet-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/README.rst` & `execnet-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `execnet-2.0.1/pyproject.toml` & `execnet-2.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/execnet/_version.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
-    "/src",
     "/doc",
+    "/src",
     "/testing",
+    "tox.ini",
 ]
 
-
 [tool.mypy]
 python_version = "3.7"
```

### Comparing `execnet-2.0.1/PKG-INFO` & `execnet-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: execnet
-Version: 2.0.1
+Version: 2.0.2
 Summary: execnet: rapid multi-Python deployment
 Project-URL: Homepage, https://execnet.readthedocs.io/en/latest/
 Author: holger krekel and others
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

