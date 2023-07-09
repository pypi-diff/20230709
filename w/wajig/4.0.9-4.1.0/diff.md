# Comparing `tmp/wajig-4.0.9.tar.gz` & `tmp/wajig-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wajig-4.0.9.tar", last modified: Thu Feb  2 00:59:38 2023, max compression
+gzip compressed data, was "wajig-4.1.0.tar", last modified: Sun Jul  9 05:59:13 2023, max compression
```

## Comparing `wajig-4.0.9.tar` & `wajig-4.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-02 00:59:38.972858 wajig-4.0.9/
--rw-r-----   0 gjw       (1000) gjw       (1000)    35149 2020-07-07 02:15:20.000000 wajig-4.0.9/LICENSE
--rw-r-----   0 gjw       (1000) gjw       (1000)       82 2020-07-25 22:22:49.000000 wajig-4.0.9/MANIFEST.in
--rw-r-----   0 gjw       (1000) gjw       (1000)    32951 2023-02-02 00:59:38.972858 wajig-4.0.9/PKG-INFO
--rw-r-----   0 gjw       (1000) gjw       (1000)    32069 2021-10-29 05:34:34.000000 wajig-4.0.9/README.rst
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-02 00:59:38.968858 wajig-4.0.9/docs/
--rw-r-----   0 gjw       (1000) gjw       (1000)    32372 2020-08-02 08:52:34.000000 wajig-4.0.9/docs/README.md
--rw-r-----   0 gjw       (1000) gjw       (1000)       50 2023-02-02 00:59:38.972858 wajig-4.0.9/setup.cfg
--rw-r-----   0 gjw       (1000) gjw       (1000)     2491 2023-02-02 00:59:38.000000 wajig-4.0.9/setup.py
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-02 00:59:38.968858 wajig-4.0.9/wajig/
--rwxr-x---   0 gjw       (1000) gjw       (1000)    38335 2022-08-16 19:43:34.000000 wajig-4.0.9/wajig/__init__.py
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-02 00:59:38.972858 wajig-4.0.9/wajig/bash_completion.d/
--rw-r-----   0 gjw       (1000) gjw       (1000)     4972 2022-09-09 01:07:27.000000 wajig-4.0.9/wajig/bash_completion.d/wajig.bash
--rw-r-----   0 gjw       (1000) gjw       (1000)    51078 2023-02-02 00:58:04.000000 wajig-4.0.9/wajig/commands.py
--rw-r-----   0 gjw       (1000) gjw       (1000)      289 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig/constants.py
--rw-r-----   0 gjw       (1000) gjw       (1000)     1586 2020-06-11 00:25:18.000000 wajig-4.0.9/wajig/debfile-deps.py
--rw-r-----   0 gjw       (1000) gjw       (1000)     1224 2020-07-26 06:53:41.000000 wajig-4.0.9/wajig/debfile.py
--rw-r-----   0 gjw       (1000) gjw       (1000)     4429 2021-10-24 21:34:57.000000 wajig-4.0.9/wajig/perform.py
--rwxr-x---   0 gjw       (1000) gjw       (1000)     2990 2022-11-06 19:20:40.000000 wajig-4.0.9/wajig/shell.py
--rw-r-----   0 gjw       (1000) gjw       (1000)    22441 2022-11-06 19:20:40.000000 wajig-4.0.9/wajig/util.py
-drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-02-02 00:59:38.972858 wajig-4.0.9/wajig.egg-info/
--rw-r-----   0 gjw       (1000) gjw       (1000)    32951 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/PKG-INFO
--rw-r-----   0 gjw       (1000) gjw       (1000)      415 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/SOURCES.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)        1 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/dependency_links.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)       38 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/entry_points.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)       36 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/requires.txt
--rw-r-----   0 gjw       (1000) gjw       (1000)        6 2023-02-02 00:59:38.000000 wajig-4.0.9/wajig.egg-info/top_level.txt
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 05:59:13.019310 wajig-4.1.0/
+-rw-r-----   0 gjw       (1000) gjw       (1000)    35149 2020-07-07 02:15:20.000000 wajig-4.1.0/LICENSE
+-rw-r-----   0 gjw       (1000) gjw       (1000)       82 2020-07-25 22:22:49.000000 wajig-4.1.0/MANIFEST.in
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32921 2023-07-09 05:59:13.019310 wajig-4.1.0/PKG-INFO
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32815 2023-07-09 03:06:21.000000 wajig-4.1.0/README.rst
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 05:59:13.015310 wajig-4.1.0/docs/
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32372 2020-08-02 08:52:34.000000 wajig-4.1.0/docs/README.md
+-rw-r-----   0 gjw       (1000) gjw       (1000)       50 2023-07-09 05:59:13.019310 wajig-4.1.0/setup.cfg
+-rw-r-----   0 gjw       (1000) gjw       (1000)     2498 2023-07-09 05:59:12.000000 wajig-4.1.0/setup.py
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 05:59:13.015310 wajig-4.1.0/wajig/
+-rwxr-x---   0 gjw       (1000) gjw       (1000)    40230 2023-07-09 02:54:05.000000 wajig-4.1.0/wajig/__init__.py
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 05:59:13.015310 wajig-4.1.0/wajig/bash_completion.d/
+-rw-r-----   0 gjw       (1000) gjw       (1000)     4972 2022-09-09 01:07:27.000000 wajig-4.1.0/wajig/bash_completion.d/wajig.bash
+-rw-r-----   0 gjw       (1000) gjw       (1000)    53078 2023-07-09 02:55:03.000000 wajig-4.1.0/wajig/commands.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)      289 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig/constants.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)     1586 2020-06-11 00:25:18.000000 wajig-4.1.0/wajig/debfile-deps.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)     1224 2020-07-26 06:53:41.000000 wajig-4.1.0/wajig/debfile.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)     4429 2021-10-24 21:34:57.000000 wajig-4.1.0/wajig/perform.py
+-rwxr-x---   0 gjw       (1000) gjw       (1000)     2990 2022-11-06 19:20:40.000000 wajig-4.1.0/wajig/shell.py
+-rw-r-----   0 gjw       (1000) gjw       (1000)    22441 2022-11-06 19:20:40.000000 wajig-4.1.0/wajig/util.py
+drwxr-x---   0 gjw       (1000) gjw       (1000)        0 2023-07-09 05:59:13.015310 wajig-4.1.0/wajig.egg-info/
+-rw-r-----   0 gjw       (1000) gjw       (1000)    32921 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/PKG-INFO
+-rw-r-----   0 gjw       (1000) gjw       (1000)      415 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/SOURCES.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)        1 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/dependency_links.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)       37 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/entry_points.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)       36 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/requires.txt
+-rw-r-----   0 gjw       (1000) gjw       (1000)        6 2023-07-09 05:59:12.000000 wajig-4.1.0/wajig.egg-info/top_level.txt
```

### Comparing `wajig-4.0.9/LICENSE` & `wajig-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wajig-4.0.9/PKG-INFO` & `wajig-4.1.0/docs/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: wajig
-Version: 4.0.9
-Summary: Ubunut admin managemetn tool
-Home-page: https://wajig.togaware.com
-Author: Graham Williams
-Author-email: wajig@togaware.com
-License: UNKNOWN
-Keywords: debian ubuntu admin
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Wajig: Ubuntu System Administration
 
 Wajig is a simplified, all-in-one-place, system support tool for
 Debian and Ubuntu.  It aims to cover every common (and some not so
 common) tasks you may need to perform in managing your computer. A few
 simple examples:
 
@@ -1013,9 +995,7 @@
 de-installed). You can access this list, save it to a file, and use it
 to mark those same packages for installation (or deinstallation) on
 anther machine:
 
 # dpkg --get-selections > dpkg-selections
 # dpkg --set-selections < dpkg-selections
 # apt-get dselect-upgrade
-
-
```

### Comparing `wajig-4.0.9/README.rst` & `wajig-4.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 wajig, with a special thanks to Reuben Thomas for his many suggestions
 and contributions. Graham has resumed maintenance and development.
 
 Installing
 ----------
 
 Wajig is available in the Debian and Ubuntu repositories. On Ubuntu,
-where sudo is set up by default
+with a user set up with sudo:
 
 .. code:: consoles
 
    $ sudo apt install wajig
 
 It is also available on `PyPI <https://pypi.org/project/wajig/>`__ from
 where it can be installed with:
@@ -38,15 +38,15 @@
 
    $ pip3 install wajig
 
 If sudo is not set up (see instructions below) then as root:
 
 .. code:: console
 
-   # apt-get install wajig
+   # apt install wajig
 
 Resources
 ---------
 
 -  `Home <https://wajig.togaware.com>`__ of wajig.
 -  `Support Wajig <https://togaware.com/gnulinux/>`__ with a donation.
 -  `GitHub <https://github.com/gjwgit/wajig>`__ for the source code.
@@ -243,19 +243,46 @@
 -  Ensure that user-visible changes are mentioned in
    ``debian/changelog``; use ``/usr/bin/debchange`` from within the
    project root directory and do your changes there.
 
 HowTo Release
 -------------
 
--  Ensure that the version string in ``src/wajig.py`` as updated from
-   the Makefil matches that of latest changelog.
+-  Bump version in Makefile and add debian/changelog entry.
+
+-  Check https://bugs.launchpad.net/ubuntu/+source/wajig
+
+-  Check https://bugs.debian.org/cgi-bin/pkgreport.cgi?src=wajig
+
+-  Check https://tracker.debian.org/pkg/wajig
+   
+-  Ensure that the version string in ``src/wajig.py`` is updated from
+   the Makefile matches that of latest changelog entry.
 
 -  Ensure that debuild does not emit any lintian errors/warnings.
 
+- Check on a fresh server (e.g., on Linode or VM or Docker)
+
+  $ git clone git@github.com:gjwgit/wajig.git
+  $ cd wajig
+  $ sudo apt install build-essential dh-python python3-setuptools python3-thefuzz python3-all debhelper-compat
+  $ make deb
+  $ sudo apt install python3-distro python3-levenshtein aptitude
+  $ sudo dpkg --install wajig_4.0.12_all.deb
+  $ wajig version
+  $ wajig install most
+
+- Tag the version:
+
+  $ git tag v4.0.12
+  $ git push --tags
+
+- Create a release on github: "Release v4.0.12"
+
+   
 Available Packages
 ------------------
 
 The Debian packaging system relies on your local system having some idea
 of what packages are available. This is initialised when you install
 your system. You will generally need to update this list of packages
 with what is currently available from the Debian archives for
```

### Comparing `wajig-4.0.9/docs/README.md` & `wajig-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: wajig
+Version: 4.1.0
+Summary: Debian/Ubuntu admin management tool
+Home-page: https://wajig.togaware.com
+Author: Graham Williams
+Author-email: wajig@togaware.com
+Keywords: debian ubuntu admin
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Wajig: Ubuntu System Administration
 
 Wajig is a simplified, all-in-one-place, system support tool for
 Debian and Ubuntu.  It aims to cover every common (and some not so
 common) tasks you may need to perform in managing your computer. A few
 simple examples:
```

### Comparing `wajig-4.0.9/setup.py` & `wajig-4.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # Get the long description from the README file.
 
 with open(path.join(here, 'docs/README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='wajig',
-    version='4.0.9',  # DO NOT MODIFY. Managed from Makefile.
-    description='Ubunut admin managemetn tool',
+    version='4.1.0',  # DO NOT MODIFY. Managed from Makefile.
+    description='Debian/Ubuntu admin management tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Graham Williams',
     author_email='wajig@togaware.com',
     url='https://wajig.togaware.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

### Comparing `wajig-4.0.9/wajig/__init__.py` & `wajig-4.1.0/wajig/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,51 +137,65 @@
 
     def help(args):
         args.parser.print_help()
     parser_help = subparsers.add_parser("help")
     parser_help.set_defaults(func=help, parser=parser)
 
     # ADDCDROM
-    
+
     function = commands.addcdrom
     parser_addcdrom = subparsers.add_parser(
         "addcdrom",
         aliases=["add-cdrom"],
         parents=[parser_teach],
         description=function.__doc__,
     )
     parser_addcdrom.set_defaults(func=function)
 
+    # ADDGROUP
+
+    function = commands.addgroup
+    parser_addgroup = subparsers.add_parser(
+        "addgroup",
+        aliases=["add-group"],
+        parents=[parser_teach],
+        description=function.__doc__,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser_addgroup.add_argument("username")
+    parser_addgroup.add_argument("group")
+    parser_addgroup.set_defaults(func=function)
+
     # ADDKEY
-    
+
     function = commands.addkey
     parser_addkey = subparsers.add_parser(
         "addkey",
         aliases=["add-key"],
         parents=[parser_teach],
         description=function.__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser_addkey.add_argument("key")
     parser_addkey.set_defaults(func=function)
 
     # ADDREPO
-    
+
     function = commands.addrepo
     parser_addrepo = subparsers.add_parser(
         "addrepo",
         parents=[parser_yesno, parser_teach],
         description=function.__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser_addrepo.add_argument("ppa")
     parser_addrepo.set_defaults(func=function)
 
     # ADDUSER
-    
+
     function = commands.adduser
     parser_adduser = subparsers.add_parser(
         "adduser",
         parents=[parser_teach],
         description=function.__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
@@ -289,15 +303,15 @@
         aliases=["daily-upgrade"],
         parents=[parser_teach],
         description=function.__doc__,
     )
     parser_dailyupgrade.set_defaults(func=function)
 
     # DELUSER
-    
+
     function = commands.deluser
     parser_deluser = subparsers.add_parser(
         "deluser",
         aliases=["rmuser"],
         parents=[parser_teach],
         description=function.__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter,
@@ -328,14 +342,27 @@
         "describenew",
         aliases="newdescribe new-describe describe-new".split(),
         description=function.__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser_describenew.set_defaults(func=function)
 
+    # DISABLE
+
+    function = commands.disable
+    parser_disable = subparsers.add_parser(
+        "disable",
+        aliases=["disuser", "lock"],
+        parents=[parser_teach],
+        description=function.__doc__,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser_disable.add_argument("username", nargs="+")
+    parser_disable.set_defaults(func=function)
+
     function = commands.distupgrade
     parser_distupgrade = subparsers.add_parser(
         "distupgrade",
         aliases=["dist-upgrade", "full-upgrade"],
         parents=[
             parser_backup, parser_yesno, parser_auth, parser_teach,
             parser_local, parser_dist
@@ -360,14 +387,27 @@
         "editsources",
         aliases=["edit-sources"],
         parents=[parser_teach],
         description=function.__doc__,
     )
     parser_editsources.set_defaults(func=function)
 
+    # ENABLE
+
+    function = commands.enable
+    parser_enable = subparsers.add_parser(
+        "enable",
+        aliases=["enuser", "unlock"],
+        parents=[parser_teach],
+        description=function.__doc__,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser_enable.add_argument("username", nargs="+")
+    parser_enable.set_defaults(func=function)
+
     function = commands.extract
     parser_extract = subparsers.add_parser(
         "extract",
         parents=[parser_teach],
         description=function.__doc__,
     )
     parser_extract.add_argument("debfile")
@@ -519,28 +559,38 @@
         "listdaemons",
         aliases=["list-daemons"],
         parents=[parser_teach],
         description=function.__doc__,
     )
     parser_listdaemons.set_defaults(func=function)
 
+    function = commands.listgroups
+    parser_listgroups = subparsers.add_parser(
+        "listgroups",
+        aliases=["list-groups", "groups"],
+        parents=[parser_teach],
+        description=function.__doc__,
+    )
+    parser_listgroups.set_defaults(func=function)
+
     function = commands.listfiles
     parser_listfiles = subparsers.add_parser(
         "listfiles",
         aliases=["list-files"],
         parents=[parser_teach],
         description=function.__doc__,
     )
     parser_listfiles.add_argument("package")
     parser_listfiles.set_defaults(func=function)
 
     function = commands.listhold
     parser_listhold = subparsers.add_parser(
         "listhold",
         aliases=["list-hold"],
+        parents=[parser_teach],
         description=function.__doc__,
     )
     parser_listhold.set_defaults(func=function)
 
     function = commands.listinstalled
     parser_listinstalled = subparsers.add_parser(
         "listinstalled",
@@ -832,15 +882,15 @@
         aliases="bug bugreport".split(),
         description=function.__doc__,
     )
     parser_reportbug.add_argument("package")
     parser_reportbug.set_defaults(func=function)
 
     # REPOS - list ppa repositories
-    
+
     function = commands.repos
     parser_repos = subparsers.add_parser(
         "repos",
         parents=[parser_teach, parser_grep],
         description=function.__doc__,
     )
     parser_repos.set_defaults(func=function)
@@ -850,16 +900,30 @@
         "restart",
         parents=[parser_teach],
         description=function.__doc__,
     )
     parser_restart.add_argument("daemon")
     parser_restart.set_defaults(func=function)
 
+    # RMGROUP
+
+    function = commands.rmgroup
+    parser_rmgroup = subparsers.add_parser(
+        "rmgroup",
+        aliases=["remove-group", "delgroup"],
+        parents=[parser_teach],
+        description=function.__doc__,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+    )
+    parser_rmgroup.add_argument("username")
+    parser_rmgroup.add_argument("group")
+    parser_rmgroup.set_defaults(func=function)
+
     # RMREPO
-    
+
     function = commands.rmrepo
     parser_rmrepo = subparsers.add_parser(
         "rmrepo",
         parents=[parser_yesno, parser_teach],
         description=function.__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
```

### Comparing `wajig-4.0.9/wajig/bash_completion.d/wajig.bash` & `wajig-4.1.0/wajig/bash_completion.d/wajig.bash`

 * *Files identical despite different names*

### Comparing `wajig-4.0.9/wajig/commands.py` & `wajig-4.1.0/wajig/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 """Implementation of all COMMANDs"""
 
 # Do not include any function in here that does not correspond to a COMMAND
 
 import os
 import re
-import sys
 import string
 import random
 import inspect
 import tempfile
 import subprocess
 import urllib.request
 import webbrowser
@@ -29,15 +28,31 @@
 util.ensure_initialised()
 
 NO_UPGRADES = 'No packages known to be upgradable. Run "wajig update" to update local information from the repository.'
 
 
 def addcdrom(args):
     """Add a Debian CD/DVD to APT's list of available sources"""
-    perform.execute("/usr/bin/apt-cdrom add", root=True, teach=args.teach, noop=args.noop)
+    perform.execute("/usr/bin/apt-cdrom add",
+                    root=True, teach=args.teach, noop=args.noop)
+
+
+# ADDGROUP
+
+def addgroup(args):
+    """Add a user to a group.
+
+    Unix groups are used to provide group access to commands or
+    files. For example, adding users to the group `sudo` give those
+    users super user access through the `sudo` command.
+
+    $ wajig addgroup fred sudo"""
+    cmd = f'/usr/sbin/adduser {args.username} {args.group}'
+    perform.execute(cmd, root=True, teach=args.teach, noop=args.noop)
+
 
 # ADDKEY
 
 def addkey(args):
     """Add a Repository Key to the Local Archive
 
     Normally the security key from a repository is added when the repository
@@ -48,42 +63,44 @@
     $ wajig addkey F142A4D99F16EB04
     """
     util.requires_package("apt")
     cmd = "/usr/bin/apt-key adv --keyserver keyserver.ubuntu.com --recv-keys "
     cmd += args.key
     perform.execute(cmd, root=True, teach=args.teach, noop=args.noop)
 
+
 # ADDREPO
 
 def addrepo(args):
     """Add a Launchpad PPA (Personal Package Archive) repository
 
     An example that shows how to add the daily builds of
     Google's Chromium browser:
 
     $ wajig addrepo ppa:chromium-daily
     """
     util.requires_package("add-apt-repository")
-    perform.execute("/usr/bin/add-apt-repository " + args.ppa, root=True, teach=args.teach, noop=args.noop)
+    cmd = "/usr/bin/add-apt-repository " + args.ppa
+    perform.execute(cmd, root=True, teach=args.teach, noop=args.noop)
+
 
 # ADDUSER
 
 def adduser(args):
     """Add new user, multiple users, or as listed in a file.
 
-With just a username create a new password while adding user and 
-return that.
+    With just a username create a new password while adding user and
+    return that.
 
-  $ wajig adduser fred
+    $ wajig adduser fred
 
-If a number is provided then that many new users are created and
-the output will be username:password.
+    If a number is provided then that many new users are created and
+    the output will be username:password.
 
-  $ wajig adduser 5
-"""
+    $ wajig adduser 5"""
     number = args.number
     username = args.username
 
     if number and not re.match(r"^[0-9]+$", number):
         username.insert(0, number)
         number = ""
 
@@ -95,43 +112,43 @@
     elif args.file:
         if not os.path.exists(args.file):
             print(f"wajig adduser: error: file not found '{args.file}'")
         elif not os.access(args.file, os.R_OK):
             print(f"wajig adduser: error: file not accessible '{args.file}'.")
         else:
             usernames = []
-            for l in open(args.file, 'r'):
-                usernames.append(l.strip())
-    
+            for u in open(args.file, 'r'):
+                usernames.append(u.strip())
+
     elif number and re.match(r"^[0-9]+$", number):
         usernames = []
         for i in range(int(number)):
             code = ''.join(random.choice(string.ascii_lowercase) for _ in range(7))
             usernames.append(f"u{code}")
-            
+
     else:
         for u in username:
             if not re.match(r"^[a-z][-a-z0-9_]*$", u):
                 print(f"wajig adduser: error: bad user name '{u}' " +
                       f"must start with lowercase then",
                       f"alphanumerics or underscore.")
         usernames = username
 
     util.requires_package("pwgen")
     created = []
     for u in usernames:
-        command = f'adduser {u} --gecos "" --disabled-password'
-        perform.execute(command, root=True, teach=args.teach, noop=args.noop)
+        cmd = f'adduser {u} --gecos "" --disabled-password'
+        perform.execute(cmd, root=True, teach=args.teach, noop=args.noop)
         
-        command = f"pwgen -s -y 20 1"
-        password = perform.execute(command, pipe=True, teach=args.teach, noop=args.noop)
+        cmd = f"pwgen -s 20 1"
+        password = perform.execute(cmd, pipe=True, teach=args.teach, noop=args.noop)
         if password: password = password.readline().strip()
         
-        command = f'echo "{u}:{pasword}" | sudo chpasswd'
-        perform.execute(command, root=True, teach=args.teach, noop=args.noop)
+        cmd = f'echo "{u}:{password}" | sudo chpasswd'
+        perform.execute(cmd, root=True, teach=args.teach, noop=args.noop)
 
         print()
         created.append(f"{u}:{password}")
 
     print("\n".join(created))
             
 def aptlog(args):
@@ -145,17 +162,17 @@
         "/usr/bin/update-alternatives --auto " + args.alternative, root=True, teach=args.teach, noop=args.noop
     )
 
 
 def autodownload(args):
     """Do an update followed by a download of all updated packages"""
     util.do_update(args.noop)
-    command = ("/usr/bin/apt-get --download-only --show-upgraded --assume-yes "
+    cmd = ("/usr/bin/apt-get --download-only --show-upgraded --assume-yes "
                "--force-yes dist-upgrade")
-    perform.execute(command, root=True)
+    perform.execute(cmd, root=True)
     if not args.noop:
         upgradable_packages = util.upgradable()
         if upgradable_packages:
             util.do_describe(upgradable_packages, args.verbose)
         else:
             print("no upgradable packages")
         util.show_package_versions()
@@ -175,24 +192,24 @@
     """Get source packages, unpack them, and build binary packages from them.
 
     Note: This also installs the needed build-dependencies if needed
     """
     util.requires_package("sudo")
     # First make sure dependencies are met
     if not builddeps(args):
-        command = "apt-get {} source --build " + " ".join(args.packages)
-        command = command.format(args.noauth)
-        perform.execute(command)
+        cmd = "apt-get {} source --build " + " ".join(args.packages)
+        cmd = cmd.format(args.noauth)
+        perform.execute(cmd)
 
 
 def builddeps(args):
     """Install build-dependencies for given packages"""
-    command = "/usr/bin/apt-get {} {} build-dep " + " ".join(args.packages)
-    command = command.format(args.yes, args.noauth)
-    return perform.execute(command, root=True, log=True, teach=args.teach, noop=args.noop)
+    cmd = "/usr/bin/apt-get {} {} build-dep " + " ".join(args.packages)
+    cmd = cmd.format(args.yes, args.noauth)
+    return perform.execute(cmd, root=True, log=True, teach=args.teach, noop=args.noop)
 
 
 def changelog(args):
     """Display Debian changelog of a package
 
     network on:
          changelog - if there's newer entries, display them
@@ -234,18 +251,18 @@
     else:
         tmp = tempfile.mkstemp()[1]
         with open(tmp, "w") as f:
             if package.is_installed:
                 changelog += "{:=^79}\n".format(" local changelog ")
             f.write(changelog)
         if package.is_installed:
-            command = util.local_changelog(args.package, tmp)
-            if not command:
+            cmd = util.local_changelog(args.package, tmp)
+            if not cmd:
                 return
-            perform.execute(command)
+            perform.execute(cmd)
         with open(tmp) as f:
             for line in f:
                 try:
                     print(line, end="")
                 except BrokenPipeError:
                     return
 
@@ -290,16 +307,16 @@
     """Delete user accounts
 
 With a list of usernames, delete each user.
 
   $ wajig deluser fred susan
 """
     for u in args.username:
-        command = f"sudo deluser --remove-home --backup {u}"
-        perform.execute(command, root=True, teach=args.teach, noop=args.noop)
+        cmd = f"sudo deluser --remove-home --backup {u}"
+        perform.execute(cmd, root=True, teach=args.teach, noop=args.noop)
         if not u == args.username[-1]: print()
 
 
 def dependents(args):
     """Display packages which have some form of dependency on the given package
 
     Types of dependencies:
@@ -346,14 +363,30 @@
     """Display one-line descriptions of newly-available packages
 
     This produces the same output as 'wajig new'
     """
     util.newly_available()
 
 
+# DISABLE
+
+def disable(args):
+    """Disable user accounts.
+
+    The user account is retained and can be re-ENABLEd. The action is
+    to actually place a '!' in front of the encrypted password in the
+    password file.  With a list of usernames, diable each user.
+
+    $ wajig disable fred susan"""
+    for u in args.username:
+        cmd = f"sudo usermod --lock {u}"
+        perform.execute(cmd, root=True, teach=args.teach, noop=args.noop)
+        if not u == args.username[-1]: print()
+
+
 def distupgrade(args):
     """Comprehensive system upgrade
 
     This may remove some packages in order to ensure no package is
     left stale. Use the more conservative 'upgrade' command to avoid
     that.
     """
@@ -373,67 +406,84 @@
     cmd += "full-upgrade"
     perform.execute(cmd, root=True, log=True, teach=args.teach, noop=args.noop)
 
 
 def download(args):
     """Download one or more packages without installing them"""
     print("Packages being downloaded to /var/cache/apt/archives/")
-    command = "/usr/bin/apt-get --reinstall --download-only install "
+    cmd = "/usr/bin/apt-get --reinstall --download-only install "
     packages = util.consolidate_package_names(args)
-    command = command + " ".join(packages)
-    perform.execute(command, root=True, teach=args.teach, noop=args.noop)
+    cmd = cmd + " ".join(packages)
+    perform.execute(cmd, root=True, teach=args.teach, noop=args.noop)
 
 
 def editsources(args):
     """Edit list of Debian repository locations for packages"""
     perform.execute("/usr/bin/apt edit-source", root=True, teach=args.teach, noop=args.noop)
 
 
+# ENABLE
+
+def enable(args):
+    """Enable user accounts.
+
+    A user account that has been `disable`d is re-enabled. The action
+    is to actually remove a '!' in front of the encrypted password in
+    the password file.  With a list of usernames, enable each user.
+
+    $ wajig enable mary john"""
+    for u in args.username:
+        cmd = f"sudo usermod --unlock {u}"
+        perform.execute(cmd, root=True, teach=args.teach, noop=args.noop)
+        if not u == args.username[-1]:
+            print()
+
+
 def extract(args):
     """Extract the files from a package file to a directory"""
-    command = "dpkg --extract {} {}"
-    command = command.format(args.debfile, args.destination_directory)
-    perform.execute(command, teach=args.teach, noop=args.noop)
+    cmd = "dpkg --extract {} {}"
+    cmd = cmd.format(args.debfile, args.destination_directory)
+    perform.execute(cmd, teach=args.teach, noop=args.noop)
 
 
 def fixconfigure(args):
     """Fix an interrupted install"""
     perform.execute("/usr/bin/dpkg --configure --pending", root=True, teach=args.teach, noop=args.noop)
 
 
 def fixinstall(args):
     """Fix an install interrupted by broken dependencies"""
-    command = "/usr/bin/apt-get --fix-broken {} install".format(args.noauth)
-    perform.execute(command, root=True, log=True, teach=args.teach, noop=args.noop)
+    cmd = "/usr/bin/apt-get --fix-broken {} install".format(args.noauth)
+    perform.execute(cmd, root=True, log=True, teach=args.teach, noop=args.noop)
 
 
 def fixmissing(args):
     """Fix and install even though there are missing dependencies"""
-    command = "/usr/bin/apt-get --ignore-missing {} upgrade".format(args.noauth)
-    perform.execute(command, root=True, log=True, teach=args.teach, noop=args.noop)
+    cmd = "/usr/bin/apt-get --ignore-missing {} upgrade".format(args.noauth)
+    perform.execute(cmd, root=True, log=True, teach=args.teach, noop=args.noop)
 
 
 def force(args):
     """Install packages and ignore file overwrites and depends
 
     Note: This is useful when there is a conflict of the same file from
           multiple packages or when a dependency is not installed for
           whatever reason
     """
 
-    command = "/usr/bin/dpkg --install --force overwrite --force depends "
+    cmd = "/usr/bin/dpkg --install --force overwrite --force depends "
     archives = "/var/cache/apt/archives/"
 
     # For a .deb file we simply force install it.
     if args.packages[0].endswith(".deb"):
         for package in args.packages:
             if os.path.exists(package):
-                command += "'" + package + "' "
+                cmd += "'" + package + "' "
             elif os.path.exists(archives + package):
-                command += "'" + archives + package + "' "
+                cmd += "'" + archives + package + "' "
             else:
                 message = ("File {} not found. "
                            "Searched current directory and {}."
                            "Please confirm the location and try again.")
                 print(message.format(package, archives))
                 return()
     else:
@@ -453,26 +503,26 @@
                     "install '{}'"
                 ).format(package)
                 perform.execute(dlcmd, root=True)
                 matches = perform.execute(lscmd, pipe=True)
                 debpkg = matches.readline().strip()
 
             # Force install the package from the download archive.
-            command += "'" + archives + debpkg + "' "
+            cmd += "'" + archives + debpkg + "' "
 
-    perform.execute(command, root=True, log=True, teach=args.teach, noop=args.noop)
+    perform.execute(cmd, root=True, log=True, teach=args.teach, noop=args.noop)
 
 
 def hold(args):
     """Place packages on hold (so they will not be upgraded)"""
     for package in args.packages:
         # The dpkg needs sudo but not the echo.
         # Do all of it as root then!
-        command = '/bin/echo "{} hold" | /usr/bin/dpkg --set-selections'
-        perform.execute(command.format(package), root=True, teach=args.teach, noop=args.noop)
+        cmd = '/bin/echo "{} hold" | /usr/bin/dpkg --set-selections'
+        perform.execute(cmd.format(package), root=True, teach=args.teach, noop=args.noop)
     print("The following packages are on hold:")
     perform.execute("dpkg --get-selections | grep -E 'hold$' | cut -f1", teach=args.teach, noop=args.noop)
 
 
 def info(args):
     """List the information contained in a package file"""
     perform.execute("dpkg --info " + args.package, teach=args.teach, noop=args.noop)
@@ -623,25 +673,35 @@
         if shutil.which("apt-file"):
             perform.execute("apt-file list --regexp ^{}$".format(args.package), teach=args.teach, noop=args.noop)
     else:
         for line in output.decode().strip().split('\n'):
             print(line)
 
 
+def listgroups(args):
+    """List the unix groups defined for this computer.
+
+    Groups in unix are used for managing users and their permissions
+    to access commands and files."""
+    cmd = "cat /etc/group | cut -d':' -f1 | sort"
+    perform.execute(cmd, teach=args.teach, noop=args.noop)
+
+
 def listhold(args):
     """List packages that are on hold (i.e. those that won't be upgraded)"""
-    perform.execute("dpkg --get-selections | grep -E 'hold$' | cut -f1", teach=args.teach, noop=args.noop)
+    cmd = "dpkg --get-selections | grep -E 'hold$' | cut -f1"
+    perform.execute(cmd, teach=args.teach, noop=args.noop)
 
 
 def listinstalled(args):
     """List installed packages"""
-    command = "dpkg --get-selections | cut -f1"
+    cmd = "dpkg --get-selections | cut -f1"
     if args.pattern:
-        command += " | grep -E '{}' | sort -k 1b,1".format(args.pattern)
-    perform.execute(command, teach=args.teach, noop=args.noop)
+        cmd += " | grep -E '{}' | sort -k 1b,1".format(args.pattern)
+    perform.execute(cmd, teach=args.teach, noop=args.noop)
 
 
 def listlog(args):
     """Display wajig log file"""
     perform.execute("cat " + util.log_file, teach=args.teach, noop=args.noop)
 
 # LISTNAMES
@@ -650,35 +710,35 @@
     """List all known packages; optionally filter the list with a pattern"""
     util.do_listnames(args.pattern)
 
 # LISTPACKAGES
 
 def listpackages(args):
     """List the status, version, and description of installed packages"""
-    command = "dpkg --list '*' | grep -E -v 'no description avail'"
+    cmd = "dpkg --list '*' | grep -E -v 'no description avail'"
     if args.pattern:
-        command += " | grep -E '{}' | sort -k 1b,1".format(args.pattern)
-    perform.execute(command, teach=args.teach, noop=args.noop)
+        cmd += " | grep -E '{}' | sort -k 1b,1".format(args.pattern)
+    perform.execute(cmd, teach=args.teach, noop=args.noop)
 
 
 def listscripts(args):
     """List the control scripts of the package of deb file"""
     package = args.debfile
     scripts = ["preinst", "postinst", "prerm", "postrm"]
     if package.endswith(".deb"):
-        command = "ar p " + package + " control.tar.gz | tar ztvf -"
-        pkgScripts = perform.execute(command, pipe=True).readlines()
+        cmd = "ar p " + package + " control.tar.gz | tar ztvf -"
+        pkgScripts = perform.execute(cmd, pipe=True).readlines()
         for script in scripts:
             if "./" + script in "".join(pkgScripts):
                 nlen = int((72 - len(script)) / 2)
                 print(">"*nlen, script, "<"*nlen)
-                command = "ar p " + package + " control.tar.gz |" +\
+                cmd = "ar p " + package + " control.tar.gz |" +\
                           "tar zxvf - -O ./" + script +\
                           " 2>/dev/null"
-                perform.execute(command, teach=args.teach, noop=args.noop)
+                perform.execute(cmd, teach=args.teach, noop=args.noop)
     else:
         root = "/var/lib/dpkg/info/"
         for script in scripts:
             fname = root + package + "." + script
             if os.path.exists(fname):
                 nlen = int((72 - len(script))/2)
                 print(">"*nlen, script, "<"*nlen)
@@ -707,29 +767,29 @@
     sections = set(sections)
     for section in sections:
         print(section)
 
 
 def liststatus(args):
     """Same as list but only prints first two columns, not truncated"""
-    command = "COLUMNS=400 "
-    command += "dpkg --list '*' | grep -E -v 'no description avail'"
-    command += " | awk '{print $1,$2}'"
+    cmd = "COLUMNS=400 "
+    cmd += "dpkg --list '*' | grep -E -v 'no description avail'"
+    cmd += " | awk '{print $1,$2}'"
     if args.pattern:
-        command += " | grep -E '{}' | sort -k 1b,1".format(args.pattern)
-    perform.execute(command, teach=args.teach, noop=args.noop)
+        cmd += " | grep -E '{}' | sort -k 1b,1".format(args.pattern)
+    perform.execute(cmd, teach=args.teach, noop=args.noop)
 
 
 def localupgrade(args):
     """Upgrade using only packages that are already downloaded"""
-    command = (
+    cmd = (
         "/usr/bin/apt-get --no-download --ignore-missing "
         "--show-upgraded upgrade"
     )
-    perform.execute(command, root=True, log=True, teach=args.teach, noop=args.noop)
+    perform.execute(cmd, root=True, log=True, teach=args.teach, noop=args.noop)
 
 
 def madison(args):
     """Runs the madison command of apt-cache"""
     command = "apt-cache madison " + " ".join(set(args.packages))
     perform.execute(command, teach=args.teach, noop=args.noop)
 
@@ -983,14 +1043,30 @@
     perform.execute(command, teach=args.teach, noop=args.noop)
     
 def restart(args):
     """Restart system daemons (see LIST-DAEMONS for available daemons)"""
     command = "/usr/sbin/service {} restart".format(args.daemon)
     perform.execute(command, root=True, teach=args.teach, noop=args.noop)
 
+
+# RMGROUP
+
+def rmgroup(args):
+    """Remove a user from a group.
+
+    Unix groups are used to provide group access to commands or
+    files. For example, adding users to the group `sudo` give those
+    users super user access through the `sudo` command. This command
+    allows users to be removed from groups.
+
+    $ wajig rmgroup fred sudo"""
+    cmd = f'/usr/sbin/deluser {args.username} {args.group}'
+    perform.execute(cmd, root=True, teach=args.teach, noop=args.noop)
+
+
 # RMREPO
 
 def rmrepo(args):
     """Remove a Launchpad PPA (Personal Package Archive) repository
 
     An example that shows how to remove the daily builds of
     Google's Chromium browser:
```

### Comparing `wajig-4.0.9/wajig/debfile-deps.py` & `wajig-4.1.0/wajig/debfile-deps.py`

 * *Files identical despite different names*

### Comparing `wajig-4.0.9/wajig/debfile.py` & `wajig-4.1.0/wajig/debfile.py`

 * *Files identical despite different names*

### Comparing `wajig-4.0.9/wajig/perform.py` & `wajig-4.1.0/wajig/perform.py`

 * *Files identical despite different names*

### Comparing `wajig-4.0.9/wajig/shell.py` & `wajig-4.1.0/wajig/shell.py`

 * *Files identical despite different names*

### Comparing `wajig-4.0.9/wajig/util.py` & `wajig-4.1.0/wajig/util.py`

 * *Files identical despite different names*

### Comparing `wajig-4.0.9/wajig.egg-info/PKG-INFO` & `wajig-4.1.0/wajig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: wajig
-Version: 4.0.9
-Summary: Ubunut admin managemetn tool
+Version: 4.1.0
+Summary: Debian/Ubuntu admin management tool
 Home-page: https://wajig.togaware.com
 Author: Graham Williams
 Author-email: wajig@togaware.com
-License: UNKNOWN
 Keywords: debian ubuntu admin
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -1013,9 +1011,7 @@
 de-installed). You can access this list, save it to a file, and use it
 to mark those same packages for installation (or deinstallation) on
 anther machine:
 
 # dpkg --get-selections > dpkg-selections
 # dpkg --set-selections < dpkg-selections
 # apt-get dselect-upgrade
-
-
```

