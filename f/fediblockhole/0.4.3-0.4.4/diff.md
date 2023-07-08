# Comparing `tmp/fediblockhole-0.4.3.tar.gz` & `tmp/fediblockhole-0.4.4.tar.gz`

## Comparing `fediblockhole-0.4.3.tar` & `fediblockhole-0.4.4.tar`

### file list

```diff
@@ -1,40 +1,1056 @@
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/CHANGELOG.md
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/requirements.txt
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/setup.cfg
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/.pytest_cache/README.md
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/etc/sample.fediblockhole.conf.toml
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/samples/demo-allowlist-01.csv
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/samples/demo-allowlist-02.csv
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/samples/demo-blocklist-01.csv
--rwxr-xr-x   0        0        0    31053 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/src/fediblockhole/__init__.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/src/fediblockhole/blocklists.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/src/fediblockhole/const.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/conftest.py
--rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/data-mastodon.json
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/data-noop-01.csv
--rw-r--r--   0        0        0    43809 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/data-rapidblock.json
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/data-silences-01.csv
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/data-suspends-01.csv
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_allowlist.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_blockseverity.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_cmdline.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_configfile.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_domainblock.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_merge_comments.py
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_merge_thresholds.py
--rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_mergeplan.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_parser_csv.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_parser_json.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_parser_rapidblockcsv.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/test_parser_rapidblockjson.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/helpers/__init__.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/tests/helpers/util.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/LICENSE
--rw-r--r--   0        0        0    16485 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/README.md
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    57390 2020-02-02 00:00:00.000000 fediblockhole-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/CHANGELOG.md
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/requirements.txt
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/setup.cfg
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/pyvenv.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/.dev/Vagrantfile
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/.dev/ubuntu-20.04-packer.json
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/.dev/ubuntu-20.04-v2-packer.hcl
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/activate
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/activate.csh
+-rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/activate.fish
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/activate.ps1
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/activate_this.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/fediblock-sync
+-rwxr-xr-x   0        0        0      277 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/normalizer
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/pip
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/pip-3.10
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/pip3
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/pip3.10
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/py.test
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/pytest
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/python -> /usr/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/python3.10 -> python
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/wheel
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/wheel-3.10
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/wheel3
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/bin/wheel3.10
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip-22.0.2.virtualenv
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/py.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools-59.6.0.virtualenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel-0.37.1.virtualenv
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/__init__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_argcomplete.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_version.py
+-rw-r--r--   0        0        0    21392 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/cacheprovider.py
+-rw-r--r--   0        0        0    34737 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/capture.py
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/compat.py
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/debugging.py
+-rw-r--r--   0        0        0     5487 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/deprecated.py
+-rw-r--r--   0        0        0    25961 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/doctest.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/faulthandler.py
+-rw-r--r--   0        0        0    67085 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/fixtures.py
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/freeze_support.py
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/helpconfig.py
+-rw-r--r--   0        0        0    32558 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/hookspec.py
+-rw-r--r--   0        0        0    25716 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/junitxml.py
+-rw-r--r--   0        0        0    16929 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/legacypath.py
+-rw-r--r--   0        0        0    34031 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/logging.py
+-rw-r--r--   0        0        0    32491 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/main.py
+-rw-r--r--   0        0        0    14857 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/monkeypatch.py
+-rw-r--r--   0        0        0    26559 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/nodes.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/nose.py
+-rw-r--r--   0        0        0    10256 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/outcomes.py
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/pastebin.py
+-rw-r--r--   0        0        0    25824 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/pathlib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/py.typed
+-rw-r--r--   0        0        0    61971 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/pytester.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/pytester_assertions.py
+-rw-r--r--   0        0        0    71155 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/python.py
+-rw-r--r--   0        0        0    38400 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/python_api.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/python_path.py
+-rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/recwarn.py
+-rw-r--r--   0        0        0    20840 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/reports.py
+-rw-r--r--   0        0        0    18447 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/runner.py
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/scope.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/setuponly.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/setupplan.py
+-rw-r--r--   0        0        0    10200 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/skipping.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/stash.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/stepwise.py
+-rw-r--r--   0        0        0    53509 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/terminal.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/threadexception.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/timing.py
+-rw-r--r--   0        0        0    11708 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/tmpdir.py
+-rw-r--r--   0        0        0    14809 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/unittest.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/unraisableexception.py
+-rw-r--r--   0        0        0     4474 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/warning_types.py
+-rw-r--r--   0        0        0     5070 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/warnings.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_code/__init__.py
+-rw-r--r--   0        0        0    46740 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_code/code.py
+-rw-r--r--   0        0        0     7436 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_code/source.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_io/__init__.py
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_io/saferepr.py
+-rw-r--r--   0        0        0     8152 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_io/terminalwriter.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_io/wcwidth.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_py/__init__.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_py/error.py
+-rw-r--r--   0        0        0    49149 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/_py/path.py
+-rw-r--r--   0        0        0     6458 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/assertion/__init__.py
+-rw-r--r--   0        0        0    46610 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/assertion/rewrite.py
+-rw-r--r--   0        0        0     4382 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/assertion/truncate.py
+-rw-r--r--   0        0        0    18009 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/assertion/util.py
+-rw-r--r--   0        0        0    64018 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/config/__init__.py
+-rw-r--r--   0        0        0    21225 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/config/argparsing.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/config/compat.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/config/exceptions.py
+-rw-r--r--   0        0        0     7884 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/config/findpaths.py
+-rw-r--r--   0        0        0     8468 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/mark/__init__.py
+-rw-r--r--   0        0        0     6507 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/mark/expression.py
+-rw-r--r--   0        0        0    21179 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/_pytest/mark/structures.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/certifi/__init__.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/certifi/__main__.py
+-rw-r--r--   0        0        0   278952 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/certifi/cacert.pem
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/certifi/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/certifi/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/LICENSE
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/METADATA
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/WHEEL
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/certifi-2023.5.7.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/__init__.py
+-rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/api.py
+-rw-r--r--   0        0        0    12554 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/cd.py
+-rw-r--r--   0        0        0    19101 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/constant.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/legacy.py
+-rwxr-xr-x   0        0        0    17496 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/md.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0    18258 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/md.py
+-rwxr-xr-x   0        0        0   424312 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/md__mypyc.cpython-310-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0    11492 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/py.typed
+-rw-r--r--   0        0        0    11544 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/utils.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/version.py
+-rw-r--r--   0        0        0    20069 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/assets/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/cli/__init__.py
+-rw-r--r--   0        0        0     9744 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer/cli/normalizer.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/LICENSE
+-rw-r--r--   0        0        0    30983 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/RECORD
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/charset_normalizer-3.1.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/exceptiongroup/__init__.py
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/exceptiongroup/_catch.py
+-rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/exceptiongroup/_exceptions.py
+-rw-r--r--   0        0        0    19475 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/exceptiongroup/_formatting.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/exceptiongroup/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/exceptiongroup/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/exceptiongroup-1.1.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/exceptiongroup-1.1.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/exceptiongroup-1.1.2.dist-info/METADATA
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/exceptiongroup-1.1.2.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/exceptiongroup-1.1.2.dist-info/WHEEL
+-rwxr-xr-x   0        0        0    31053 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole/__init__.py
+-rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole/blocklists.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole/const.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole-0.4.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0    58198 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole-0.4.3.dist-info/METADATA
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole-0.4.3.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole-0.4.3.dist-info/REQUESTED
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole-0.4.3.dist-info/WHEEL
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole-0.4.3.dist-info/direct_url.json
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole-0.4.3.dist-info/entry_points.txt
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole-0.4.3.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna/package_data.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna/py.typed
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna/uts46data.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna-3.4.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna-3.4.dist-info/LICENSE.md
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna-3.4.dist-info/METADATA
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna-3.4.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/idna-3.4.dist-info/WHEEL
+-rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/iniconfig/__init__.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/iniconfig/_parse.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/iniconfig/_version.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/iniconfig/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/iniconfig/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/iniconfig-2.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/iniconfig-2.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/iniconfig-2.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/iniconfig-2.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/iniconfig-2.0.0.dist-info/licenses/LICENSE
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/_elffile.py
+-rw-r--r--   0        0        0     8926 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10194 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/markers.py
+-rw-r--r--   0        0        0    16397 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/metadata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/py.typed
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/specifiers.py
+-rw-r--r--   0        0        0    18106 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/utils.py
+-rw-r--r--   0        0        0    16326 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging/version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging-23.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging-23.1.dist-info/LICENSE
+-rw-r--r--   0        0        0    10174 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging-23.1.dist-info/LICENSE.APACHE
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging-23.1.dist-info/LICENSE.BSD
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging-23.1.dist-info/METADATA
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging-23.1.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/packaging-23.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0     9441 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    13171 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    20912 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    12307 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    28525 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     2614 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10788 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0    10339 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18669 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     8944 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12318 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    21392 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    36783 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    17362 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0    19429 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0     9456 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     9817 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3500 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    12190 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    16729 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9770 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    24145 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0        0        0    27412 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    16094 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17421 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    32524 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/req/req_tracker.py
+-rw-r--r--   0        0        0    23814 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    18288 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    28298 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9915 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11335 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    11522 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    19359 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     7662 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8906 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4708 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    48414 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distro.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    15625 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     6783 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   265969 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31254 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0     9411 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5110 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/compat.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    10510 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13546 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    31621 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20715 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    13838 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25777 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    19643 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   105697 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    99571 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98776 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   102498 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   131180 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   103312 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95946 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     3413 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    25481 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    19474 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51456 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20739 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51963 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39109 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    17720 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/scripts.py
+-rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/version.py
+-rw-r--r--   0        0        0    42943 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/__init__.py
+-rw-r--r--   0        0        0    16728 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/_ihatexml.py
+-rw-r--r--   0        0        0    32353 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/_inputstream.py
+-rw-r--r--   0        0        0    77040 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/_tokenizer.py
+-rw-r--r--   0        0        0     4931 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/_utils.py
+-rw-r--r--   0        0        0    83464 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/constants.py
+-rw-r--r--   0        0        0   117186 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/html5parser.py
+-rw-r--r--   0        0        0    15759 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/serializer.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/_base.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/_trie/py.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/__init__.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/alphabeticalattributes.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/base.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/inject_meta_charset.py
+-rw-r--r--   0        0        0     3643 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/lint.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/optionaltags.py
+-rw-r--r--   0        0        0    26897 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/sanitizer.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/filters/whitespace.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/__init__.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/genshi.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treeadapters/sax.py
+-rw-r--r--   0        0        0     3592 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/__init__.py
+-rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/base.py
+-rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/dom.py
+-rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree.py
+-rw-r--r--   0        0        0    14766 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treebuilders/etree_lxml.py
+-rw-r--r--   0        0        0     5719 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/__init__.py
+-rw-r--r--   0        0        0     7476 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/base.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/dom.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree.py
+-rw-r--r--   0        0        0     6357 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/etree_lxml.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/html5lib/treewalkers/genshi.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12795 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44025 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   204400 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/_version.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34475 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pep517/__init__.py
+-rw-r--r--   0        0        0     3457 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pep517/build.py
+-rw-r--r--   0        0        0     6084 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pep517/check.py
+-rw-r--r--   0        0        0     4098 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pep517/colorlog.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pep517/compat.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pep517/dirtools.py
+-rw-r--r--   0        0        0     6100 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pep517/envbuild.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pep517/meta.py
+-rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pep517/wrappers.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/__init__.py
+-rw-r--r--   0        0        0    11201 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pep517/in_process/_in_process.py
+-rw-r--r--   0        0        0   108287 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pkg_resources/py31compat.py
+-rw-r--r--   0        0        0    12676 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/progress/__init__.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/progress/bar.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/progress/colors.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/progress/counter.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/progress/spinner.py
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23408 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    31937 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6143 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63188 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0     9123 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40292 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5005 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35330 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21819 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    18930 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    70032 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    52776 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   212248 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9030 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    38299 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25339 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10381 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    22165 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0     5130 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    21861 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6402 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18430 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35116 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    29835 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33301 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    17592 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8810 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_lru_cache.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    26521 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10425 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9069 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4285 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    17285 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    81236 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     7614 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14048 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    13711 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    10868 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8058 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5258 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0     8637 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    32572 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    35926 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     7762 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    23916 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    26469 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    26994 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    36757 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/tabulate.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    44424 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    25935 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9122 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    18257 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0     6645 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22415 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0     2763 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20076 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39013 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19763 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    28203 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    16900 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34449 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34666 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22001 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14047 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip-22.0.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip-22.0.2.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip-22.0.2.dist-info/METADATA
+-rw-r--r--   0        0        0    74713 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip-22.0.2.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip-22.0.2.dist-info/WHEEL
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip-22.0.2.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pip-22.0.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0   108573 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/appdirs.py
+-rw-r--r--   0        0        0   232055 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/pyparsing.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30964 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy/__init__.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy/_callers.py
+-rw-r--r--   0        0        0    20483 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy/_hooks.py
+-rw-r--r--   0        0        0    17944 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy/_manager.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy/_result.py
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy/_tracing.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy/_version.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy-1.2.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy-1.2.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy-1.2.0.dist-info/METADATA
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy-1.2.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy-1.2.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pluggy-1.2.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     5237 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pytest/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pytest/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pytest/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pytest-7.4.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pytest-7.4.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     7960 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pytest-7.4.0.dist-info/METADATA
+-rw-r--r--   0        0        0    10146 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pytest-7.4.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pytest-7.4.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pytest-7.4.0.dist-info/WHEEL
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pytest-7.4.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/pytest-7.4.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/__init__.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/__version__.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/_internal_utils.py
+-rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/adapters.py
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/auth.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/certs.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/cookies.py
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/exceptions.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/hooks.py
+-rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/models.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/packages.py
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/structures.py
+-rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests/utils.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests-2.31.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests-2.31.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests-2.31.0.dist-info/METADATA
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests-2.31.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests-2.31.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/requests-2.31.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0     7448 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_deprecation_warning.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    10536 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/build_meta.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/cli-32.exe
+-rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/cli-64.exe
+-rw-r--r--   0        0        0   137216 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/cli-arm64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0    23153 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/config.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    43162 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/glob.py
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/gui-32.exe
+-rw-r--r--   0        0        0    75264 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/gui-64.exe
+-rw-r--r--   0        0        0   137728 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/gui-arm64.exe
+-rw-r--r--   0        0        0    65536 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     5217 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    50561 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    40103 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/py34compat.py
+-rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     8288 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0    20813 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    14894 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    47644 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    18079 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     9282 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    17330 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     7778 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    50421 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10515 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    17784 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    30453 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    23540 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/py35compat.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    22151 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12483 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    14538 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    20655 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    13015 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5277 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     5562 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    35579 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_msi.py
+-rw-r--r--   0        0        0    21537 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0    16030 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/bdist_wininst.py
+-rw-r--r--   0        0        0     5773 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    31612 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    16495 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     5637 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13117 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    28970 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8397 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19005 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0   232055 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/pyparsing.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   117968 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30964 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    16604 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    13212 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    87973 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    26134 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     5036 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0     8088 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/test.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7218 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools-59.6.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools-59.6.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools-59.6.0.dist-info/METADATA
+-rw-r--r--   0        0        0    21843 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools-59.6.0.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools-59.6.0.dist-info/WHEEL
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools-59.6.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/setuptools-59.6.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/toml/__init__.py
+-rw-r--r--   0        0        0    38942 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/toml/decoder.py
+-rw-r--r--   0        0        0     9940 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/toml/encoder.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/toml/ordered.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/toml/tz.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/toml-0.10.2.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/toml-0.10.2.dist-info/LICENSE
+-rw-r--r--   0        0        0     7142 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/toml-0.10.2.dist-info/METADATA
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/toml-0.10.2.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/toml-0.10.2.dist-info/WHEEL
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/toml-0.10.2.dist-info/top_level.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/tomli/_types.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/tomli/py.typed
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/tomli-2.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/tomli-2.0.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/tomli-2.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/tomli-2.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/tomli-2.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     5283 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/__init__.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/_base_connection.py
+-rw-r--r--   0        0        0    15561 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/_collections.py
+-rw-r--r--   0        0        0     7756 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/_request_methods.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/_version.py
+-rw-r--r--   0        0        0    33622 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/connection.py
+-rw-r--r--   0        0        0    42961 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/exceptions.py
+-rw-r--r--   0        0        0    11026 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/fields.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/filepost.py
+-rw-r--r--   0        0        0    22648 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/poolmanager.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/py.typed
+-rw-r--r--   0        0        0    40092 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0    19437 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34121 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7715 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    14452 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    16220 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/proxy.py
+-rw-r--r--   0        0        0     8111 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/request.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/response.py
+-rw-r--r--   0        0        0    18374 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/retry.py
+-rw-r--r--   0        0        0    18860 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     9045 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    15213 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/url.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/util.py
+-rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3/util/wait.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/INSTALLER
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/METADATA
+-rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/RECORD
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/WHEEL
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/urllib3-2.0.3.dist-info/licenses/LICENSE.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/__init__.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/__main__.py
+-rw-r--r--   0        0        0    19075 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/bdist_wheel.py
+-rw-r--r--   0        0        0    15930 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/macosx_libfile.py
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/metadata.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/pkginfo.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/util.py
+-rw-r--r--   0        0        0     7589 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/wheelfile.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/cli/__init__.py
+-rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/cli/convert.py
+-rw-r--r--   0        0        0     3364 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/cli/pack.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/cli/unpack.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/vendored/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/vendored/packaging/__init__.py
+-rw-r--r--   0        0        0     1812 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/vendored/packaging/_typing.py
+-rw-r--r--   0        0        0    29560 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel/vendored/packaging/tags.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel-0.37.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel-0.37.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel-0.37.1.dist-info/METADATA
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel-0.37.1.dist-info/RECORD
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel-0.37.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel-0.37.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/wheel-0.37.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/chart/.helmignore
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/chart/Chart.yaml
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/chart/fediblockhole.conf.toml
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/chart/values.yaml
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/chart/templates/_helpers.tpl
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/chart/templates/configmap-conf-toml.yaml
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/chart/templates/cronjob-fediblock-sync.yaml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/container/.dockerignore
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/container/Dockerfile
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/etc/sample.fediblockhole.conf.toml
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/samples/demo-allowlist-01.csv
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/samples/demo-allowlist-02.csv
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/samples/demo-blocklist-01.csv
+-rwxr-xr-x   0        0        0    31087 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/src/fediblockhole/__init__.py
+-rw-r--r--   0        0        0     8925 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/src/fediblockhole/blocklists.py
+-rw-r--r--   0        0        0     6241 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/src/fediblockhole/const.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/conftest.py
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/data-mastodon.json
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/data-noop-01.csv
+-rw-r--r--   0        0        0    43809 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/data-rapidblock.json
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/data-silences-01.csv
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/data-suspends-01.csv
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_allowlist.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_blockseverity.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_cmdline.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_configfile.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_domainblock.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_merge_comments.py
+-rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_merge_thresholds.py
+-rw-r--r--   0        0        0     6653 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_mergeplan.py
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_parser_csv.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_parser_csv_mastodon.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_parser_json.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_parser_rapidblockcsv.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/test_parser_rapidblockjson.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/tests/helpers/util.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/LICENSE
+-rw-r--r--   0        0        0    17293 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/README.md
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    58198 2020-02-02 00:00:00.000000 fediblockhole-0.4.4/PKG-INFO
```

### Comparing `fediblockhole-0.4.3/CHANGELOG.md` & `fediblockhole-0.4.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,27 @@
 
 Notable changes to the project will be documented in this changelog.
 
 This project uses [Semantic Versioning] and generally follows the conventions of [Keep A Changelog].
 
 ## [Unreleased]
 
+## [v0.4.4] - 2023-07-09
+
+### Added
+
+- Added citation for creators of #Fediblock (a64875b)
+- Added parser for Mastodon 4.1 blocklist CSV format (9f95f14)
+- Added container support (76d5b61)
+
+### Fixed
+
+- Use __future__.annotations so type hints work with Python < 2.9 (8265639)
+- test util no longer tries to load default config file if conf tomldata is empty. (2da57b2)
+
 ## [v0.4.3] - 2023-02-13
 
 ### Added
 
 - Added Mastodon public API parser type because #33 (9fe9342)
 - Added ability to set scheme when talking to instances (9fe9342)
 - Added tests of comment merging. (fb3a7ec)
```

### Comparing `fediblockhole-0.4.3/etc/sample.fediblockhole.conf.toml` & `fediblockhole-0.4.4/etc/sample.fediblockhole.conf.toml`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/src/fediblockhole/__init__.py` & `fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole/__init__.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/src/fediblockhole/blocklists.py` & `fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole/blocklists.py`

 * *Files 6% similar despite different names*

```diff
@@ -156,14 +156,32 @@
         # Convert dict to DomainBlock with the double-star operator
         # See: https://docs.python.org/3/tutorial/controlflow.html#tut-unpacking-arguments
         block = DomainBlock(**blockitem)
         if block.severity > self.max_severity:
             block.severity = self.max_severity
         return block
 
+class BlocklistParserMastodonCSV(BlocklistParserCSV):
+    """ Parse Mastodon CSV formatted blocklists
+
+    The Mastodon v4.1.x domain block CSV export prefixes its
+    field names with a '#' character because… reasons?
+    """
+    do_preparse = True
+
+    def parse_item(self, blockitem: dict) -> DomainBlock:
+        """Build a new blockitem dict with new un-#ed keys
+        """
+        newdict = {}
+        for key in blockitem:
+            newkey = key.lstrip('#')
+            newdict[newkey] = blockitem[key]
+
+        return super().parse_item(newdict)
+
 class RapidBlockParserCSV(BlocklistParserCSV):
     """ Parse RapidBlock CSV blocklists
 
     RapidBlock CSV blocklists are just a newline separated list of domains.
     """
     def preparse(self, blockdata) -> Iterable:
         """Prepend a 'domain' field header to the data
@@ -219,14 +237,15 @@
     elif boolstring in ['', 'false', 'f', '0', 'n', 'no']:
         return False
     else:
         raise ValueError(f"Cannot parse value '{boolstring}' as boolean")
 
 FORMAT_PARSERS = {
     'csv': BlocklistParserCSV,
+    'mastodon_csv': BlocklistParserMastodonCSV,
     'json': BlocklistParserJSON,
     'mastodon_api_public': BlocklistParserMastodonAPIPublic,
     'rapidblock.csv': RapidBlockParserCSV,
     'rapidblock.json': RapidBlockParserJSON,
 }
 
 # helper function to select the appropriate Parser
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fediblockhole-0.4.3/src/fediblockhole/const.py` & `fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole/const.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/data-mastodon.json` & `fediblockhole-0.4.4/tests/data-mastodon.json`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/data-noop-01.csv` & `fediblockhole-0.4.4/tests/data-noop-01.csv`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/data-rapidblock.json` & `fediblockhole-0.4.4/tests/data-rapidblock.json`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/data-silences-01.csv` & `fediblockhole-0.4.4/tests/data-silences-01.csv`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/data-suspends-01.csv` & `fediblockhole-0.4.4/tests/data-suspends-01.csv`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_allowlist.py` & `fediblockhole-0.4.4/tests/test_allowlist.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_blockseverity.py` & `fediblockhole-0.4.4/tests/test_blockseverity.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_cmdline.py` & `fediblockhole-0.4.4/tests/test_cmdline.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_configfile.py` & `fediblockhole-0.4.4/tests/test_configfile.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_domainblock.py` & `fediblockhole-0.4.4/tests/test_domainblock.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_merge_comments.py` & `fediblockhole-0.4.4/tests/test_merge_comments.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_merge_thresholds.py` & `fediblockhole-0.4.4/tests/test_merge_thresholds.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_mergeplan.py` & `fediblockhole-0.4.4/tests/test_mergeplan.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_parser_csv.py` & `fediblockhole-0.4.4/tests/test_parser_csv.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_parser_json.py` & `fediblockhole-0.4.4/tests/test_parser_json.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_parser_rapidblockcsv.py` & `fediblockhole-0.4.4/tests/test_parser_rapidblockcsv.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/tests/test_parser_rapidblockjson.py` & `fediblockhole-0.4.4/tests/test_parser_rapidblockjson.py`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/LICENSE` & `fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole-0.4.3.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

### Comparing `fediblockhole-0.4.3/README.md` & `fediblockhole-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 
 A tool for keeping a Mastodon instance blocklist synchronised with remote lists.
 
 The broad design goal for FediBlockHole is to support pulling in a list of
 blocklists from a set of trusted sources, merge them into a combined blocklist,
 and then push that merged list to a set of managed instances.
 
-Inspired by the way PiHole works for maintaining a set of blocklists of adtech
-domains.
-
 Mastodon admins can choose who they think maintain quality lists and subscribe
 to them, helping to distribute the load for maintaining blocklists among a
 community of people. Control ultimately rests with the admins themselves so they
 can outsource as much, or as little, of the effort to others as they deem
 appropriate.
 
+Inspired by the way PiHole works for maintaining a set of blocklists of adtech
+domains. Builds on the work of
+[@CaribenxMarciaX@scholar.social](https://scholar.social/@CaribenxMarciaX) and
+[@gingerrroot@kitty.town](https://kitty.town/@gingerrroot) who started the
+#Fediblock hashtag and did a lot of advocacy around it, often at great personal
+cost.
+
 ## Features
 
 ### Blocklist Sources
 
  - Read domain block lists from other instances via the Mastodon API.
  - Supports both public lists (no auth required) and 'admin' lists requiring
    authentication to an instance.
@@ -193,14 +197,15 @@
 
 The URL sources is a list of URLs to fetch blocklists from.
 
 Supported formats are currently:
 
  - Comma-Separated Values (CSV)
  - JSON
+ - Mastodon v4.1 flavoured CSV
  - RapidBlock CSV
  - RapidBlock JSON
 
 Blocklists must provide a `domain` field, and should provide a `severity` field.
 
 `domain` is the domain name of the instance to be blocked/limited.
 
@@ -210,14 +215,25 @@
 
 #### CSV format
 
 A CSV format blocklist must contain a header row with at least a `domain` and `severity` field.
 
 Optional fields, as listed about, may also be included.
 
+#### Mastodon v4.1 CSV format
+
+As of v4.1.0, Mastodon can export domain blocks as a CSV file. However, in their
+infinite wisdom, the Mastodon devs decided that field names should begin with a
+`#` character in the header, unlike the field names in the JSON output via the
+API… or in pretty much any other CSV file anywhere else.
+
+Setting the format to `mastodon_csv` will strip off the `#` character when
+parsing and FediBlockHole can then use Mastodon v4.1 CSV blocklists like any
+other CSV formatted blocklist.
+
 #### JSON format
 
 JSON is also supported. It uses the same format as the JSON returned from the Mastodon API.
 
 This is a list of dictionaries, with at minimum a `domain` field, and preferably
 a `severity` field. The other optional fields are, well, optional.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fediblockhole-0.4.3/pyproject.toml` & `fediblockhole-0.4.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fediblockhole"
-version = "0.4.3"
+version = "0.4.4"
 description = "Federated blocklist management for Mastodon"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.6"
 keywords = ["mastodon", "fediblock"]
 authors = [ 
     {name = "Justin Warren"}, {email = "justin@eigenmagic.com"}
```

### Comparing `fediblockhole-0.4.3/PKG-INFO` & `fediblockhole-0.4.4/.venv/lib/python3.10/site-packages/fediblockhole-0.4.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -690,23 +690,27 @@
 
 A tool for keeping a Mastodon instance blocklist synchronised with remote lists.
 
 The broad design goal for FediBlockHole is to support pulling in a list of
 blocklists from a set of trusted sources, merge them into a combined blocklist,
 and then push that merged list to a set of managed instances.
 
-Inspired by the way PiHole works for maintaining a set of blocklists of adtech
-domains.
-
 Mastodon admins can choose who they think maintain quality lists and subscribe
 to them, helping to distribute the load for maintaining blocklists among a
 community of people. Control ultimately rests with the admins themselves so they
 can outsource as much, or as little, of the effort to others as they deem
 appropriate.
 
+Inspired by the way PiHole works for maintaining a set of blocklists of adtech
+domains. Builds on the work of
+[@CaribenxMarciaX@scholar.social](https://scholar.social/@CaribenxMarciaX) and
+[@gingerrroot@kitty.town](https://kitty.town/@gingerrroot) who started the
+#Fediblock hashtag and did a lot of advocacy around it, often at great personal
+cost.
+
 ## Features
 
 ### Blocklist Sources
 
  - Read domain block lists from other instances via the Mastodon API.
  - Supports both public lists (no auth required) and 'admin' lists requiring
    authentication to an instance.
@@ -881,14 +885,15 @@
 
 The URL sources is a list of URLs to fetch blocklists from.
 
 Supported formats are currently:
 
  - Comma-Separated Values (CSV)
  - JSON
+ - Mastodon v4.1 flavoured CSV
  - RapidBlock CSV
  - RapidBlock JSON
 
 Blocklists must provide a `domain` field, and should provide a `severity` field.
 
 `domain` is the domain name of the instance to be blocked/limited.
 
@@ -898,14 +903,25 @@
 
 #### CSV format
 
 A CSV format blocklist must contain a header row with at least a `domain` and `severity` field.
 
 Optional fields, as listed about, may also be included.
 
+#### Mastodon v4.1 CSV format
+
+As of v4.1.0, Mastodon can export domain blocks as a CSV file. However, in their
+infinite wisdom, the Mastodon devs decided that field names should begin with a
+`#` character in the header, unlike the field names in the JSON output via the
+API… or in pretty much any other CSV file anywhere else.
+
+Setting the format to `mastodon_csv` will strip off the `#` character when
+parsing and FediBlockHole can then use Mastodon v4.1 CSV blocklists like any
+other CSV formatted blocklist.
+
 #### JSON format
 
 JSON is also supported. It uses the same format as the JSON returned from the Mastodon API.
 
 This is a list of dictionaries, with at minimum a `domain` field, and preferably
 a `severity` field. The other optional fields are, well, optional.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

