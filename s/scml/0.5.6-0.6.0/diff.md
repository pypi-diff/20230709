# Comparing `tmp/scml-0.5.6.tar.gz` & `tmp/scml-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scml-0.5.6.tar", last modified: Wed Mar  8 03:49:29 2023, max compression
+gzip compressed data, was "scml-0.6.0.tar", last modified: Sun Jul  9 07:24:53 2023, max compression
```

## Comparing `scml-0.5.6.tar` & `scml-0.6.0.tar`

### file list

```diff
@@ -1,126 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.733024 scml-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-08 03:49:15.000000 scml-0.5.6/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-03-08 03:49:15.000000 scml-0.5.6/.cookiecutterrc
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-08 03:49:15.000000 scml-0.5.6/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-08 03:49:15.000000 scml-0.5.6/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-08 03:49:15.000000 scml-0.5.6/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-08 03:49:15.000000 scml-0.5.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15484 2023-03-08 03:49:15.000000 scml-0.5.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-03-08 03:49:15.000000 scml-0.5.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-08 03:49:15.000000 scml-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-08 03:49:15.000000 scml-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17651 2023-03-08 03:49:29.733024 scml-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-03-08 03:49:15.000000 scml-0.5.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-03-08 03:49:29.733024 scml-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-03-08 03:49:15.000000 scml-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.701024 scml-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.709024 scml-0.5.6/src/scml/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98103 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    68914 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/cliadv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.713024 scml-0.5.6/src/scml/oneshot/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21520 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.713024 scml-0.5.6/src/scml/oneshot/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/agents/aspiration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14554 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/agents/greedy.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/agents/nothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/agents/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    17958 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/awi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/sysagents.py
--rw-r--r--   0 runner    (1001) docker     (123)    34415 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/ufun.py
--rw-r--r--   0 runner    (1001) docker     (123)    87802 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/oneshot/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.721024 scml-0.5.6/src/scml/scml2019/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6797 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14622 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/agent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20378 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/awi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11709 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/bank.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57378 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23664 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/consumers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.721024 scml-0.5.6/src/scml/scml2019/factory_managers/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/factory_managers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38211 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/factory_managers/builtins.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7189 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/insurance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8335 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/miners.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29300 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/schedulers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46524 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/simulators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59571 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2341 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/visualizers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   106856 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2019/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.721024 scml-0.5.6/src/scml/scml2020/
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.725024 scml-0.5.6/src/scml/scml2020/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/agents/bcse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/agents/decentralizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/agents/do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/agents/indneg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/agents/moving.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/agents/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/agents/reactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    28204 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/agents/satisficer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29821 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/awi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.725024 scml-0.5.6/src/scml/scml2020/components/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32793 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/components/negotiation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20521 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/components/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/components/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/components/signing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/components/simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23305 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/components/trading.py
--rw-r--r--   0 runner    (1001) docker     (123)    21723 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.725024 scml-0.5.6/src/scml/scml2020/services/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16123 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/services/controllers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27153 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/services/simulators.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   130279 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   132429 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/scml2020/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.729024 scml-0.5.6/src/scml/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.729024 scml-0.5.6/src/scml/vendor/quick/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/vendor/quick/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/vendor/quick/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/vendor/quick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29363 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/vendor/quick/quick.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-08 03:49:15.000000 scml-0.5.6/src/scml/vendor/quick/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.709024 scml-0.5.6/src/scml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17651 2023-03-08 03:49:29.000000 scml-0.5.6/src/scml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-03-08 03:49:29.000000 scml-0.5.6/src/scml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 03:49:29.000000 scml-0.5.6/src/scml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-08 03:49:29.000000 scml-0.5.6/src/scml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 03:49:29.000000 scml-0.5.6/src/scml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-08 03:49:29.000000 scml-0.5.6/src/scml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-08 03:49:29.000000 scml-0.5.6/src/scml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:29.733024 scml-0.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 03:49:15.000000 scml-0.5.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-03-08 03:49:15.000000 scml-0.5.6/tests/switches.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_can_run_tutorial2.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17344 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_factory2019.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_oneshot_do_nothing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_oneshot_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_oneshot_ufun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20339 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_scheduler2019.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_scml2019.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12090 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_scml2019factory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_scml2019tournaments.py
--rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_scml2020.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_scml2020factory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3969 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_scml2020tournaments.py
--rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_scml2021.py
--rw-r--r--   0 runner    (1001) docker     (123)    34776 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_scml2021oneshot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8400 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_scml2021tournaments.py
--rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-03-08 03:49:15.000000 scml-0.5.6/tests/test_sync_jackson.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-08 03:49:15.000000 scml-0.5.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.853773 scml-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-09 07:24:38.000000 scml-0.6.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-09 07:24:38.000000 scml-0.6.0/.cookiecutterrc
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-09 07:24:38.000000 scml-0.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-09 07:24:38.000000 scml-0.6.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-09 07:24:38.000000 scml-0.6.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-09 07:24:38.000000 scml-0.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16087 2023-07-09 07:24:38.000000 scml-0.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-09 07:24:38.000000 scml-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-09 07:24:38.000000 scml-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-09 07:24:38.000000 scml-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-07-09 07:24:53.853773 scml-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-07-09 07:24:38.000000 scml-0.6.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-09 07:24:53.853773 scml-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-07-09 07:24:38.000000 scml-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.813773 scml-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.821773 scml-0.6.0/src/scml/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107706 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68914 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/cliadv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12675 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.825773 scml-0.6.0/src/scml/oneshot/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21864 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.829773 scml-0.6.0/src/scml/oneshot/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agents/aspiration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agents/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agents/nothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/agents/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26977 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/awi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/sysagents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34415 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/ufun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91353 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/oneshot/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.833773 scml-0.6.0/src/scml/scml2019/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6797 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14622 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20378 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/awi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11709 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/bank.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57378 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23664 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/consumers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.833773 scml-0.6.0/src/scml/scml2019/factory_managers/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/factory_managers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38211 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/factory_managers/builtins.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7189 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/insurance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8335 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/miners.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29300 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/schedulers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46524 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/simulators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59571 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2341 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/visualizers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   106856 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2019/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.833773 scml-0.6.0/src/scml/scml2020/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.837773 scml-0.6.0/src/scml/scml2020/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/bcse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/decentralizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/do_nothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/indneg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/moving.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/reactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28174 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/agents/satisficer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29821 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/awi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.841773 scml-0.6.0/src/scml/scml2020/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32793 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/negotiation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20521 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13383 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23305 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/components/trading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21723 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.841773 scml-0.6.0/src/scml/scml2020/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/services/controllers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27153 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/services/simulators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   130704 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132429 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/scml2020/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.841773 scml-0.6.0/src/scml/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.845773 scml-0.6.0/src/scml/vendor/quick/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/quick/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/quick/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/quick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29363 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/quick/quick.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-09 07:24:38.000000 scml-0.6.0/src/scml/vendor/quick/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.821773 scml-0.6.0/src/scml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-09 07:24:53.000000 scml-0.6.0/src/scml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:53.853773 scml-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 07:24:38.000000 scml-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-09 07:24:38.000000 scml-0.6.0/tests/switches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19023 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_can_run_tutorial2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17344 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_factory2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_oneshot_do_nothing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_oneshot_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_oneshot_ufun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20339 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scheduler2019.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2019.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12090 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2019factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2624 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2019tournaments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2020.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2020factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3969 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2020tournaments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19588 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2021.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34967 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2021oneshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8400 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2021tournaments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2023.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_scml2023oneshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16854 2023-07-09 07:24:38.000000 scml-0.6.0/tests/test_sync_jackson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-07-09 07:24:38.000000 scml-0.6.0/tox.ini
```

### Comparing `scml-0.5.6/.cookiecutterrc` & `scml-0.6.0/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/.travis.yml` & `scml-0.6.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/CHANGELOG.rst` & `scml-0.6.0/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+0.6.0 (2023.7.9)
+----------------
+
+* Upgrading to be compatible with NegMAS 0.10.0
+* Adding step_with() to oneshot allowing for single counter-offer set stepping of the simulation (to be used to expose the simulation as RL and MARL environments later).
+* Adding current_negotiation_details to OneShotAWI to get details of running negotiation
+* Adding managed sales, supplies, total_sales, total_supplies, needed_sales, and needed_supplies to the OneShotAWI
+* Extending OneShotState returned from awi.state and awi.default_state_encoder(mechanism_states) to expose more information about the simulation
+
 0.5.6 (2023.3.8)
 ----------------
 
 * Upgrading to be compatible with NegMAS 0.9.8
 * Updating notebooks for 2023 release
 * Adding 2023 specific classes and utility functions
 * Supporting most recent negmas version on Github
```

### Comparing `scml-0.5.6/CONTRIBUTING.rst` & `scml-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/LICENSE` & `scml-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/MANIFEST.in` & `scml-0.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/PKG-INFO` & `scml-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scml
-Version: 0.5.6
+Version: 0.6.0
 Summary: ANAC Supply Chain Management League Platform
 Home-page: https://github.com/yasserfarouk/scml
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Project-URL: Documentation, https://scml.readthedocs.io/
 Project-URL: Changelog, https://scml.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/yasserfarouk/scml/issues
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: gui
+Provides-Extra: rl
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 Overview
 ========
 
@@ -84,14 +85,23 @@
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 Changelog
 =========
 
+0.6.0 (2023.7.9)
+----------------
+
+* Upgrading to be compatible with NegMAS 0.10.0
+* Adding step_with() to oneshot allowing for single counter-offer set stepping of the simulation (to be used to expose the simulation as RL and MARL environments later).
+* Adding current_negotiation_details to OneShotAWI to get details of running negotiation
+* Adding managed sales, supplies, total_sales, total_supplies, needed_sales, and needed_supplies to the OneShotAWI
+* Extending OneShotState returned from awi.state and awi.default_state_encoder(mechanism_states) to expose more information about the simulation
+
 0.5.6 (2023.3.8)
 ----------------
 
 * Upgrading to be compatible with NegMAS 0.9.8
 * Updating notebooks for 2023 release
 * Adding 2023 specific classes and utility functions
 * Supporting most recent negmas version on Github
```

### Comparing `scml-0.5.6/README.rst` & `scml-0.6.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     :alt: Supported versions
     :target: https://pypi.org/project/scml
 
 .. |supported-implementations| image:: https://img.shields.io/pypi/implementation/scml.svg
     :alt: Supported implementations
     :target: https://pypi.org/project/scml
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/yasserfarouk/scml/v0.5.6.svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/yasserfarouk/scml/v0.6.0.svg
     :alt: Commits since latest release
-    :target: https://github.com/yasserfarouk/scml/compare/v0.5.6...master
+    :target: https://github.com/yasserfarouk/scml/compare/v0.6.0...master
 
 .. |CI| image:: https://github.com/yasserfarouk/scml/workflows/CI/badge.svg
     :target: https://www.github.com/yasserfarouk/scml
     :alt: Build Status
 
 .. |PyPiPublished| image:: https://github.com/yasserfarouk/scml/workflows/PyPI/badge.svg
     :target: https://pypi.python.org/pypi/scml
```

### Comparing `scml-0.5.6/setup.cfg` & `scml-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/setup.py` & `scml-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         join(dirname(__file__), *names), encoding=kwargs.get("encoding", "utf8")
     ) as fh:
         return fh.read()
 
 
 setup(
     name="scml",
-    version="0.5.6",
+    version="0.6.0",
     description="ANAC Supply Chain Management League Platform",
     long_description="%s\n%s"
     % (
         re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
             "", read("README.rst")
         ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
@@ -72,14 +72,15 @@
         "joblib",
         "jupyter",
         "gif",
         "mip",
     ],
     extras_require={
         "gui": ["pyqt5"],
+        "rl": ["gymnasium"],
     },
     setup_requires=["pytest-runner"],
     entry_points={
         "console_scripts": [
             "scml = scml.cli:main",
             "cliadv = scml.cliadv:cli",
         ]
```

### Comparing `scml-0.5.6/src/scml/cli.py` & `scml-0.6.0/src/scml/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 from scml.scml2020 import SCML2020Agent, is_system_agent
 from scml.scml2020.utils import (
     anac2020_collusion,
     anac2020_std,
     anac2021_collusion,
     anac2021_oneshot,
     anac2021_std,
+    anac2023_collusion,
+    anac2023_oneshot,
+    anac2023_std,
 )
 from scml.scml2020.world import SCML2020World, SCML2021World, SCML2023World
 
 try:
     from scml.vendor.quick.quick import gui_option
 except:
 
@@ -740,26 +743,28 @@
         file = open(file_name, "w")
 
     def print_and_save(x):
         print(x)
         if file:
             file.write(x)
 
-    viewmetric = ["50%" if metric == "median" else metric]
+    viewmetric = [
+        "50%"
+        if metric == "median" and "median" not in results.score_stats.columns
+        else metric
+    ]
     strs = results.score_stats["agent_type"].values.tolist()
     short_names = shortest_unique_names(strs)
     mapping = dict(zip(strs, short_names))
     results.score_stats["agent_type"] = short_names
-    print_and_save(
-        tabulate(
-            results.score_stats.sort_values(by=viewmetric, ascending=False),
-            headers="keys",
-            tablefmt="psql",
-        )
-    )
+    try:
+        xdata = results.score_stats.sort_values(by=viewmetric, ascending=False)
+    except:
+        xdata = results.score_stats
+    print_and_save(tabulate(xdata, headers="keys", tablefmt="psql"))
     if metric in ("mean", "sum"):
         results.ttest["a"] = [mapping[_] for _ in results.ttest["a"]]
         results.ttest["b"] = [mapping[_] for _ in results.ttest["b"]]
         print_and_save(tabulate(results.ttest, headers="keys", tablefmt="psql"))
     else:
         results.kstest["a"] = [mapping[_] for _ in results.kstest["a"]]
         results.kstest["b"] = [mapping[_] for _ in results.kstest["b"]]
@@ -1383,18 +1388,18 @@
 DEFAULT_2021_NONCOMPETITORS = [
     # "scml.scml2020.agents.DecentralizingAgent",
     "scml.scml2020.agents.BuyCheapSellExpensiveAgent",
 ]
 # DEFAULT_STD_2021 = (
 #     "MarketAwareDecentralizingAgent;BuyCheapSellExpensiveAgent;DecentralizingAgent"
 # )
-DEFAULT_ONESHOT = "GreedySyncAgent;SingleAgreementAspirationAgent"
+DEFAULT_ONESHOT = "GreedySyncAgent;SyncRandomOneShotAgent;SingleAgreementAspirationAgent;RandomOneShotAgent"
 DEFAULT_ONESHOT_NONCOMPETITORS = [
     "scml.oneshot.agents.RandomOneShotAgent",
-    "scml.oneshot.agents.GreedyOneShotAgent",
+    "scml.oneshot.agents.SyncRandomOneShotAgent",
     "scml.oneshot.agents.SingleAgreementAspirationAgent",
 ]
 
 
 @main.command(help="Run an SCML2021 world simulation")
 @click.option("--steps", default=10, type=int, help="Number of steps.")
 @click.option(
@@ -2920,14 +2925,311 @@
     )
     parallelism = "parallel" if parallel else "serial"
     prog_callback = print_world_progress if verbosity > 1 else None
     start = perf_counter()
     kwargs["round_robin"] = True
     results = runner(
         competitors=all_competitors,
+        competitor_params=all_competitors_params,
+        non_competitors=non_competitors,
+        non_competitor_params=non_competitor_params,
+        agent_names_reveal_type=reveal_names,
+        n_competitors_per_world=cw,
+        n_configs=configs,
+        n_runs_per_world=runs,
+        max_worlds_per_config=worlds_per_config,
+        tournament_path=log,
+        total_timeout=timeout,
+        name=name,
+        verbose=verbosity > 0,
+        compact=compact,
+        n_steps=steps,
+        parallelism=parallelism,
+        world_progress_callback=prog_callback,
+        log_ufuns=log_ufuns,
+        log_negotiations=log_negs,
+        ignore_agent_exceptions=not raise_exceptions,
+        ignore_contract_execution_exceptions=not raise_exceptions,
+        **kwargs,
+    )
+    end_time = humanize_time(perf_counter() - start)
+    display_results(results, "median", output)
+    print(f"Finished in {end_time}")
+    save_run_info(name, results.path, "tournament")
+
+
+@main.command(help="Runs an SCML2023 tournament")
+@click.option(
+    "--name",
+    "-n",
+    default="random",
+    help='The name of the tournament. The special value "random" will result in a random name',
+)
+@click.option(
+    "--steps",
+    "-s",
+    default=10,
+    type=int,
+    help="Number of steps. If passed then --steps-min and --steps-max are " "ignored",
+)
+@click.option(
+    "--ttype",
+    "--tournament-type",
+    "--tournament",
+    default="std",
+    type=click.Choice(["collusion", "std", "oneshot"]),
+    help="The config to use. It can be collusion, std, or oneshot",
+)
+@click.option(
+    "--timeout",
+    "-t",
+    default=-1,
+    type=int,
+    help="Timeout the whole tournament after the given number of seconds (0 for infinite)",
+)
+@click.option(
+    "--configs",
+    default=5,
+    type=int,
+    help="Number of unique configurations to generate.",
+)
+@click.option("--runs", default=2, help="Number of runs for each configuration")
+@click.option(
+    "--max-runs",
+    default=-1,
+    type=int,
+    help="Maximum total number of runs. Zero or negative numbers mean no limit",
+)
+@click.option(
+    "--competitors",
+    default=None,
+    help="A semicolon (;) separated list of agent types to use for the competition. You"
+    " can also pass the special value default for the default builtin"
+    " agents",
+)
+@click.option(
+    "--non-competitors",
+    default="",
+    help="A semicolon (;) separated list of agent types to exist in the worlds as non-competitors "
+    "(their scores will not be calculated).",
+)
+@click.option(
+    "--log",
+    "-l",
+    type=click.Path(dir_okay=True, file_okay=False),
+    default=default_tournament_path(),
+    help="Default location to save logs (A folder will be created under it)",
+)
+@click.option(
+    "--world-config",
+    type=click.Path(dir_okay=False, file_okay=True),
+    default=None,
+    multiple=False,
+    help="A file to load extra configuration parameters for world simulations from.",
+)
+@click.option(
+    "--verbosity",
+    default=1,
+    type=int,
+    help="verbosity level (from 0 == silent to 1 == world progress)",
+)
+@click.option(
+    "--log-ufuns/--no-ufun-logs",
+    default=False,
+    help="Log ufuns into their own CSV file. Only effective if --debug is given",
+)
+@click.option(
+    "--log-negs/--no-neg-logs",
+    default=True,
+    help="Log all negotiations. Only effective if --debug is given",
+)
+@click.option(
+    "--compact/--debug",
+    default=True,
+    help="If True, effort is exerted to reduce the memory footprint which"
+    "includes reducing logs dramatically.",
+)
+@click.option(
+    "--raise-exceptions/--ignore-exceptions",
+    default=True,
+    help="Whether to ignore agent exceptions",
+)
+@click.option(
+    "--path",
+    default="",
+    help="A path to be added to PYTHONPATH in which all competitors are stored. You can path a : separated list of "
+    "paths on linux/mac and a ; separated list in windows",
+)
+@click.option(
+    "--cw",
+    default=1,
+    type=int,
+    help="Number of competitors to run at every world simulation. It must "
+    "either be left at default or be a number > 1 and < the number "
+    "of competitors passed using --competitors",
+)
+@click.option(
+    "--parallel/--serial",
+    default=True,
+    help="Run a parallel/serial tournament on a single machine",
+)
+@click.option(
+    "--output",
+    default="",
+    type=str,
+    help="A file to save the final results to",
+)
+@click_config_file.configuration_option()
+def tournament2023(
+    name,
+    steps,
+    timeout,
+    ttype,
+    log,
+    verbosity,
+    runs,
+    configs,
+    max_runs,
+    competitors,
+    world_config,
+    non_competitors,
+    compact,
+    log_ufuns,
+    log_negs,
+    raise_exceptions,
+    path,
+    cw,
+    parallel,
+    output,
+):
+    oneshot = ttype == "oneshot"
+    if not competitors:
+        competitors = DEFAULT_ONESHOT if oneshot else DEFAULT_STD_2021
+    world_type = SCML2020OneShotWorld if oneshot else SCML2021World
+    if len(output) == 0 or output == "none":
+        output = None
+    if output:
+        output = Path(output).absolute()
+        parent = output.parent
+        parent.mkdir(exist_ok=True, parents=True)
+
+    kwargs = {}
+    if world_config is not None and len(world_config) > 0:
+        for wc in world_config:
+            kwargs.update(load(wc))
+    log = _path(log)
+    if len(path) > 0:
+        sys.path.append(path)
+    warning_n_runs = 2000
+    if timeout <= 0:
+        timeout = None
+    if name == "random":
+        name = unique_name(base="", rand_digits=0)
+    if max_runs <= 0:
+        max_runs = None
+    if compact:
+        log_ufuns = False
+
+    reveal_names = True
+    if not compact:
+        verbosity = max(1, verbosity)
+
+    worlds_per_config = (
+        None if max_runs is None else int(round(max_runs / (configs * runs)))
+    )
+
+    all_competitors = competitors.split(";")
+    for i, cp in enumerate(all_competitors):
+        if "." not in cp:
+            if oneshot:
+                all_competitors[i] = ("scml.oneshot.agents.") + cp
+            else:
+                all_competitors[i] = ("scml.scml2020.agents.") + cp
+    all_competitors_params = [dict() for _ in range(len(all_competitors))]
+
+    permutation_size = len(all_competitors)
+    if cw > len(all_competitors):
+        cw = len(all_competitors)
+    recommended = runs * configs * permutation_size
+    if worlds_per_config is not None and worlds_per_config < 1:
+        print(
+            f"You need at least {(configs * runs)} runs even with a single permutation of managers."
+            f".\n\nSet --max-runs to at least {(configs * runs)} (Recommended {recommended})"
+        )
+        return
+
+    if max_runs is not None and max_runs < recommended:
+        print(
+            f"You are running {max_runs} worlds only but it is recommended to set {max_runs} to at least "
+            f"{recommended}. Will continue"
+        )
+
+    if ttype == "std":
+        agents = 1
+
+    if worlds_per_config is None:
+        n_worlds = permutation_size * runs * configs * nCr(len(all_competitors), cw)
+        if n_worlds > warning_n_runs:
+            print(
+                f"You are running the maximum possible number of permutations for each configuration. This is roughly"
+                f" {n_worlds} simulations (each for {steps} steps). That will take a VERY long time."
+                f"\n\nYou can reduce the number of simulations by setting --configs>=1 (currently {configs}) or "
+                f"--runs>= 1 (currently {runs}) to a lower value. "
+                f"\nFinally, you can limit the maximum number of worlds to run by setting --max-runs=integer."
+            )
+            max_runs = int(
+                input(
+                    f"Input the maximum number of simulations to run. Zero to run all of the {n_worlds} "
+                    f"simulations. ^C or a negative number to exit [0 : {n_worlds}]:"
+                )
+            )
+            if max_runs == 0:
+                max_runs = None
+            if max_runs is not None and max_runs < 0:
+                exit(0)
+            worlds_per_config = (
+                None if max_runs is None else int(round(max_runs / (configs * runs)))
+            )
+
+    non_competitor_params = None
+    if len(non_competitors) < 1:
+        non_competitors = None
+    else:
+        non_competitors = non_competitors.split(";")
+        for i, cp in enumerate(non_competitors):
+            if "." not in cp:
+                if oneshot:
+                    non_competitors[i] = ("scml.oneshot.agents.") + cp
+                else:
+                    non_competitors[i] = ("scml.scml2020.agents.") + cp
+
+    if non_competitors is None:
+        non_competitors = (
+            DEFAULT_ONESHOT_NONCOMPETITORS
+            if ttype == "oneshot"
+            else DEFAULT_2021_NONCOMPETITORS
+        )
+        non_competitor_params = tuple({} for _ in range(len(non_competitors)))
+    print(f"Tournament will be run between {len(all_competitors)} agents: ")
+    pprint(all_competitors)
+    print("Non-competitors are: ")
+    pprint(non_competitors)
+    runner = (
+        anac2023_std
+        if ttype == "std"
+        else anac2023_collusion
+        if ttype == "collusion"
+        else anac2023_oneshot
+    )
+    parallelism = "parallel" if parallel else "serial"
+    prog_callback = print_world_progress if verbosity > 1 else None
+    start = perf_counter()
+    kwargs["round_robin"] = True
+    results = runner(
+        competitors=all_competitors,
         competitor_params=all_competitors_params,
         non_competitors=non_competitors,
         non_competitor_params=non_competitor_params,
         agent_names_reveal_type=reveal_names,
         n_competitors_per_world=cw,
         n_configs=configs,
         n_runs_per_world=runs,
```

### Comparing `scml-0.5.6/src/scml/cliadv.py` & `scml-0.6.0/src/scml/cliadv.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/common.py` & `scml-0.6.0/src/scml/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Common functions used in all modules"""
 from __future__ import annotations
 
 import random
-from typing import Iterable, List, Optional, Tuple, Type, Union
+from typing import Iterable
 
 import numpy as np
+from numpy.typing import NDArray
 
 __all__ = [
     "fraction_cut",
     "integer_cut",
     "intin",
     "realin",
     "strin",
@@ -50,33 +51,33 @@
         l_m: minimum per level
         l_x: maximum per level
 
     Returns:
 
     """
     if l_x is None:
-        l_x = [float("inf")] * l
+        l_x = [float("inf")] * l  # type: ignore
     if not isinstance(l_x, Iterable):
-        l_x = [l_x] * l
+        l_x = [l_x] * l  # type: ignore
     if not isinstance(l_m, Iterable):
-        l_m = [l_m] * l
+        l_m = [l_m] * l  # type: ignore
     sizes = np.asarray(l_m)
     if n < sizes.sum():
         raise ValueError(
             f"Cannot generate {l} numbers summing to {n}  with a minimum summing to {sizes.sum()}"
         )
-    if n > sum(l_x):
+    if n > sum(l_x):  # type: ignore
         raise ValueError(
-            f"Cannot generate {l} numbers summing to {n}  with a maximum summing to {sum(l_x)}"
+            f"Cannot generate {l} numbers summing to {n}  with a maximum summing to {sum(l_x)}"  # type: ignore
         )
-    valid = [i for i, s in enumerate(sizes) if l_x[i] > s]
+    valid = [i for i, s in enumerate(sizes) if l_x[i] > s]  # type: ignore
     while sizes.sum() < n:
         j = random.choice(valid)
         sizes[j] += 1
-        if sizes[j] >= l_x[j]:
+        if sizes[j] >= l_x[j]:  # type: ignore
             valid.remove(j)
     return sizes.tolist()
 
 
 def realin(rng: tuple[float, float] | float) -> float:
     """
     Selects a random number within a range if given or the input if it was a float
@@ -136,57 +137,58 @@
     dtype: type[float] | type[int] = int,
 ) -> np.ndarray:
     """Creates an array with the given choices"""
     if not isinstance(x, Iterable):
         return np.ones(n, dtype=dtype) * x
     if isinstance(x, tuple) and len(x) == 2:
         if dtype == int:
-            return np.random.randint(x[0], x[1] + 1, n, dtype=dtype)
+            return np.random.randint(x[0], x[1] + 1, n, dtype=dtype)  # type: ignore
         return x[0] + np.random.rand(n) * (x[1] - x[0])
-    x = list(x)
-    if len(x) == n:
-        return np.array(x)
-    return np.array(list(random.choices(x, k=n)))
+    xlst = list(x)
+    if len(xlst) == n:
+        return np.array(xlst)
+    return np.array(list(random.choices(xlst, k=n)))
 
 
 def distribute_quantities(
     equal: bool,
     predictability: float,
-    q: list[int],
+    q: list[int] | NDArray,
     a: int,
     n_steps: int,
     limit: list[int] | None = None,
 ):
     """Used internally by generate() methods to distribute exogenous contracts
 
     Args:
         equal: whether the quantities are to be distributed equally
         predictability: how much are quantities for the same agent at different
                         times are similar
         q: The quantity per step to be distributed
         a: The number of agents to distribute over.
-        limit: The maximum quantity per step for each agent (len(limit) == a)
+        limit: The maximum quantity per step for each agent (len(limit) == a). Only used if `equal==False`
 
     Returns:
         an n_steps * a list of lists giving the distributed quantities where
         sum[s, :] ~= q[s]. The error can be up to 2*a per step
 
     """
+    q = np.asarray(q)
     if limit is not None and not isinstance(limit, Iterable):
-        limit = [limit] * a
+        limit = [limit] * a  # type: ignore
     # if we do not distribute anything just return all zeros
     if sum(q) == 0:
         return [np.asarray([0] * a, dtype=int) for _ in range(n_steps)]
     # if all quantities are to be distributed equally, just do that directly
     # ensuring each agent gets at least one item.
     # what happens if q does not divide a? q/a is rounded.
     if equal:
-        values = np.maximum(1, np.round(q / a).astype(int)).tolist()
-        if limit is not None:
-            values = [a if a < b else b for a, b in zip(values, limit)]
+        values = np.maximum(np.round(q / a).astype(int), 1).tolist()
+        # if limit is not None:
+        #     values = [a if a < b else b for a, b in zip(values, limit)]
         return [np.asarray([values[_]] * a, dtype=int) for _ in range(n_steps)]
     if predictability < 0.01:
         values = []
         for s in range(n_steps):
             values.append(integer_cut(q[s], a, 0, limit))
             assert sum(values[-1]) == q[s]
         return values
```

### Comparing `scml-0.5.6/src/scml/experiment.py` & `scml-0.6.0/src/scml/experiment.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/oneshot/__init__.py` & `scml-0.6.0/src/scml/oneshot/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from .common import *
+from .agent import *
+from .agents import *
 from .awi import *
+from .common import *
+from .policy import *
 from .sysagents import *
 from .ufun import *
 from .world import *
-from .agent import *
-from .agents import *
 
 
 def builtin_agent_types(as_str=False):
     """
     Returns all built-in agents.
 
     Args:
@@ -24,11 +25,12 @@
 
 
 __all__ = (
     common.__all__
     + world.__all__
     + ufun.__all__
     + agent.__all__
+    + policy.__all__
     + agents.__all__
     + awi.__all__
     + ["builtin_agent_types"]
 )
```

### Comparing `scml-0.5.6/src/scml/oneshot/adapter.py` & `scml-0.6.0/src/scml/oneshot/adapter.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/oneshot/agent.py` & `scml-0.6.0/src/scml/oneshot/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,21 +96,23 @@
     def running_negotiations(self) -> list[RunningNegotiationInfo]:
         """The negotiations currently requested by the agent.
 
         Returns:
 
             A list of negotiation information objects (`RunningNegotiationInfo`)
         """
+        assert self._owner is not None
         return self._owner.running_negotiations
 
     @property
     def unsigned_contracts(self) -> list[Contract]:
         """
         All contracts that are not yet signed.
         """
+        assert self._owner is not None
         return self._owner.unsigned_contracts
 
     def init(self):
         """
         Called once after the AWI is set.
 
         Remarks:
@@ -127,19 +129,30 @@
                            evaluated for any set of contracts, offers or otherwise.
 
         Remarks:
             - You can always as assume that self.ufun returns the ufun for your.
               You will not need to directly use this method in most cases.
 
         """
+        assert self._owner is not None
         return self._owner.make_ufun(add_exogenous)
 
+    def before_step(self):
+        """
+        Called at the beginning of every step.
+
+        Remarks:
+            - Use this for any proactive code  that needs to be done every
+              simulation step.
+        """
+        pass
+
     def step(self):
         """
-        Called every step.
+        Called at the end of every step.
 
         Remarks:
             - Use this for any proactive code  that needs to be done every
               simulation step.
         """
         pass
 
@@ -164,34 +177,32 @@
             negotiator_id: ID of the negotiator (and partner)
             state: Mechanism state including current step
 
         Returns:
             an outcome to offer.
         """
 
-    def respond(
-        self, negotiator_id: str, state: MechanismState, offer: Outcome
-    ) -> ResponseType:
+    def respond(self, negotiator_id: str, state: SAOState) -> ResponseType:
         """
         Responds to an offer from one of the partners.
 
         Args:
             negotiator_id: ID of the negotiator (and partner)
             state: Mechanism state including current step
-            offer: The offer received.
 
         Returns:
             A response type which can either be reject, accept, or end negotiation.
 
         Remarks:
             default behavior is to accept only if the current offer is the same
             or has a higher utility compared with what the agent would have
             proposed in the given state and reject otherwise
 
         """
+        offer = state.current_offer
         myoffer = self.propose(negotiator_id, state)
         if myoffer == offer:
             return ResponseType.ACCEPT_OFFER
         return ResponseType.REJECT_OFFER
 
     @property
     def internal_state(self) -> dict[str, Any]:
@@ -410,15 +421,15 @@
         """
 
 
 class EndingNegotiator(SAONegotiator):
     def propose(self, state):
         return None
 
-    def respond(self, state, offer):
+    def respond(self, state):
         return ResponseType.END_NEGOTIATION
 
 
 class OneShotIndNegotiatorsAgent(OneShotAgent):
     """
     A one-shot agent that deligates all of its decisions to a set of independent
     negotiators (one per partner per day).
@@ -534,15 +545,15 @@
             if self.awi.is_system(partner_id):
                 continue
             issues = (
                 self.awi.current_input_issues
                 if partner_id in self.awi.my_suppliers
                 else self.awi.current_output_issues
             )
-            mn, mx = self._urange(u, issues)
+            mn, mx = self._urange(u, tuple(issues))
             if self._normalize:
                 u = self._unorm(u, mn, mx)
                 if u is None:
                     continue
             if not self._set_reservation:
                 continue
             if (
@@ -563,15 +574,15 @@
     def step(self):
         super().step()
         self._ufuns = self._get_ufuns()
 
     def make_negotiator(
         self,
         negotiator_type=None,
-        name: str = None,
+        name: str = None,  # type: ignore
         **kwargs,
     ):
         """
         Creates a negotiator but does not add it to the controller. Call
         `add_negotiator` to add it.
 
         Args:
```

### Comparing `scml-0.5.6/src/scml/oneshot/agents/aspiration.py` & `scml-0.6.0/src/scml/oneshot/agents/aspiration.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/oneshot/agents/greedy.py` & `scml-0.6.0/src/scml/oneshot/agents/greedy.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,16 @@
             return None
 
         # over-write the unit price in the best offer with a good-enough price
         offer = list(offer)
         offer[UNIT_PRICE] = self._find_good_price(self.get_nmi(negotiator_id), state)
         return tuple(offer)
 
-    def respond(self, negotiator_id, state, offer):
+    def respond(self, negotiator_id, state):
+        offer = state.current_offer
         # find the quantity I still need and end negotiation if I need nothing more
         my_needs = self._needed(negotiator_id)
         if my_needs <= 0:
             return ResponseType.END_NEGOTIATION
 
         # reject any offers with quantities above my needs
         response = (
```

### Comparing `scml-0.5.6/src/scml/oneshot/agents/nothing.py` & `scml-0.6.0/src/scml/oneshot/agents/nothing.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,9 +14,9 @@
         it is an input or an output agent trading in raw material or final
         product).
     """
 
     def propose(self, negotiator_id, state):
         return None
 
-    def respond(self, negotiator_id, state, offer):
+    def respond(self, negotiator_id, state):
         return ResponseType.END_NEGOTIATION
```

### Comparing `scml-0.5.6/src/scml/oneshot/awi.py` & `scml-0.6.0/src/scml/oneshot/awi.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Implements the one shot version of the Agent-World Interface.
 
 """
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional, Tuple
+from collections import defaultdict
+from typing import Any, Dict, List, Literal, Optional, Tuple
 
 import numpy as np
 from negmas import AgentWorldInterface
-from negmas.outcomes import Issue
+from negmas.outcomes import DiscreteCartesianOutcomeSpace, Issue, make_os
+from negmas.sao import SAOState
 
 from ..scml2020 import FinancialReport, is_system_agent
-from .common import OneShotProfile, OneShotState
+from .common import NegotiationDetails, OneShotProfile, OneShotState
 
 __all__ = ["OneShotAWI"]
 
 
 class OneShotAWI(AgentWorldInterface):
     """
     The agent world interface for the one-shot game.
@@ -91,20 +93,29 @@
         B. Other Agents' Information:
           - *reports_of_agent*: Gives all past financial reports of a given agent.
             See `FinancialReport` for details.
           - *reports_at_step*: Gives all reports of all agents at a given step.
             See `FinancialReport` for details.
 
         C. Current Negotiations Information:
+          - *current_input_outcome_space*: The current outcome-space for all negotiations to buy
+            the input product of the agent. If the agent is at level zero, this will have no issues.
+          - *current_output_outcome_space*: The current outcome-space for all negotiations to buy
+            the output product of the agent. If the agent
+            is at level n_products - 1, this will have no issues.
           - *current_input_issues*: The current issues for all negotiations to buy
             the input product of the agent. If the agent
             is at level zero, this will be empty.
+            This is exactly the same as current_input_outcome_space.issues
           - *current_output_issues*: The current issues for all negotiations to buy
             the output product of the agent. If the agent
             is at level n_products - 1, this will be empty.
+            This is exactly the same as current_output_outcome_space.issues
+          - *current_negotiation_details*: Details on all current negotiations separated into "buy"
+            and "sell" dictionaries.
 
         D. Agent Information:
           - *current_exogenous_input_quantity*: The total quantity the agent have
             in its input exogenous contract.
           - *current_exogenous_input_price*: The total price of the agent's
             input exogenous contract.
           - *current_exogenous_output_quantity*: The total quantity the agent have
@@ -113,22 +124,36 @@
             output exogenous contract.
           - *current_disposal_cost*: The disposal cost per unit item in the current
             step.
           - *current_shortfall_penalty*: The shortfall penalty per unit item in the current
             step.
           - *current_balance*: The current balance of the agent
 
+        E. Sales and Supplies (quantities) for today:
+          - *sales*: Today's sales per customer so far.
+          - *supplies*: Today's supplies per supplier so far.
+          - *total_sales*: Today's total sales so far.
+          - *total_supplies*: Today's total supplies so far.
+          - *needed_sales*: Today's needed sales as of now (exogenous input + total supplies - exogenous output - total sales so far).
+          - *needed_supplies*: Today's needed supplies  as of now (exogenous output + total sales - exogenous input - total supplies so far).
+
+
     Services (All inherited from `negmas.situated.AgentWorldInterface`):
       - *logdebug/loginfo/logwarning/logerror*: Logs to the world log at the given log level.
       - *logdebug_agent/loginf_agnet/...*: Logs to the agent specific log at the given log level.
       - *bb_query*: Queries the bulletin-board.
       - *bb_read*: Read a section of the bulletin-board.
 
     """
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._sales: dict[str, int] = defaultdict(int)
+        self._supplies: dict[str, int] = defaultdict(int)
+
     # ================================================================
     # Static World Information (does not change during the simulation)
     # ================================================================
 
     # Market information
     # ------------------
 
@@ -179,15 +204,15 @@
 
     @property
     def catalog_prices(self) -> np.ndarray:
         """Returns the catalog prices of all products"""
         return self._world.catalog_prices
 
     @property
-    def price_multiplier(self):
+    def price_multiplier(self) -> float:
         """
         Controls the minimum and maximum prices in the negotiation agendas
 
         Remarks:
             - The base price is either the catalog price if trading price information
               is not public or the trading price.
             - The minimum unit price in any negotiation agenda is the base price of
@@ -291,30 +316,126 @@
         """Returns a list of IDs for all the agent's consumers
         (agents that can consume at least one product it may produce).
 
         """
         return self.all_consumers[self.level + 1]
 
     @property
-    def penalties_scale(self) -> str:
+    def penalties_scale(self) -> Literal["trading", "catalog", "unit", "none"]:
         return self._world.penalties_scale
 
     # =========================================================
     # Dynamic Agent Information (changes during the simulation)
     # =========================================================
+    def default_encoded_state(
+        self, mechanism_states: dict[str, SAOState]
+    ) -> OneShotState:
+        all_agents = [_ for _ in self._world.agents.keys() if self.is_system(_)]
+
+        return OneShotState(
+            exogenous_input_quantity=self.current_exogenous_input_quantity,
+            exogenous_input_price=self.current_exogenous_input_price,
+            exogenous_output_quantity=self.current_exogenous_output_quantity,
+            exogenous_output_price=self.current_exogenous_output_price,
+            disposal_cost=self.current_disposal_cost,
+            shortfall_penalty=self.current_shortfall_penalty,
+            current_balance=self.current_balance,
+            total_sales=self.total_sales,
+            total_supplies=self.total_supplies,
+            n_products=self.n_products,
+            n_processes=self.n_processes,
+            n_competitors=self.n_competitors,
+            all_suppliers=self.all_suppliers,
+            all_consumers=self.all_consumers,
+            catalog_prices=self.catalog_prices.tolist(),
+            price_multiplier=self.price_multiplier,
+            is_exogenous_forced=self.is_exogenous_forced,
+            current_step=self.current_step,
+            n_steps=self.n_steps,
+            relative_simulation_time=self.relative_time,
+            profile=self.profile,
+            n_lines=self.n_lines,
+            is_first_level=self.is_first_level,
+            is_last_level=self.is_last_level,
+            is_middle_level=self.is_middle_level,
+            my_input_product=self.my_input_product,
+            my_output_product=self.my_output_product,
+            level=self.level,
+            my_suppliers=self.my_suppliers,
+            my_consumers=self.my_consumers,
+            penalties_scale=self.penalties_scale,
+            n_input_negotiations=self.n_input_negotiations,
+            n_output_negotiations=self.n_output_negotiations,
+            trading_prices=self.trading_prices.tolist(),
+            exogenous_contract_summary=self.exogenous_contract_summary,
+            current_input_outcome_space=self.current_input_outcome_space,
+            current_output_outcome_space=self.current_output_outcome_space,
+            current_negotiation_details=self.current_negotiation_details,
+            sales=self.sales,
+            supplies=self.supplies,
+            needed_sales=self.needed_sales,
+            needed_supplies=self.needed_supplies,
+            bankrupt_agents=[_ for _ in all_agents if self.is_bankrupt(_)],
+            reports_of_agents=dict(
+                zip(all_agents, [self.reports_of_agent(_) for _ in all_agents])
+            ),
+            running_negotiations=mechanism_states,
+        )
 
     def state(self) -> Any:
+        all_agents = [_ for _ in self._world.agents.keys() if self.is_system(_)]
+
         return OneShotState(
             exogenous_input_quantity=self.current_exogenous_input_quantity,
             exogenous_input_price=self.current_exogenous_input_price,
             exogenous_output_quantity=self.current_exogenous_output_quantity,
             exogenous_output_price=self.current_exogenous_output_price,
             disposal_cost=self.current_disposal_cost,
             shortfall_penalty=self.current_shortfall_penalty,
             current_balance=self.current_balance,
+            total_sales=self.total_sales,
+            total_supplies=self.total_supplies,
+            n_products=self.n_products,
+            n_processes=self.n_processes,
+            n_competitors=self.n_competitors,
+            all_suppliers=self.all_suppliers,
+            all_consumers=self.all_consumers,
+            catalog_prices=self.catalog_prices.tolist(),
+            price_multiplier=self.price_multiplier,
+            is_exogenous_forced=self.is_exogenous_forced,
+            current_step=self.current_step,
+            n_steps=self.n_steps,
+            relative_simulation_time=self.relative_time,
+            profile=self.profile,
+            n_lines=self.n_lines,
+            is_first_level=self.is_first_level,
+            is_last_level=self.is_last_level,
+            is_middle_level=self.is_middle_level,
+            my_input_product=self.my_input_product,
+            my_output_product=self.my_output_product,
+            level=self.level,
+            my_suppliers=self.my_suppliers,
+            my_consumers=self.my_consumers,
+            penalties_scale=self.penalties_scale,
+            n_input_negotiations=self.n_input_negotiations,
+            n_output_negotiations=self.n_output_negotiations,
+            trading_prices=self.trading_prices.tolist(),
+            exogenous_contract_summary=self.exogenous_contract_summary,
+            current_input_outcome_space=self.current_input_outcome_space,
+            current_output_outcome_space=self.current_output_outcome_space,
+            current_negotiation_details=self.current_negotiation_details,
+            sales=self.sales,
+            supplies=self.supplies,
+            needed_sales=self.needed_sales,
+            needed_supplies=self.needed_supplies,
+            bankrupt_agents=[_ for _ in all_agents if self.is_bankrupt(_)],
+            reports_of_agents=dict(
+                zip(all_agents, [self.reports_of_agent(_) for _ in all_agents])
+            ),
+            running_negotiations=dict(),
         )
 
     @property
     def current_balance(self):
         return self._world.current_balance(self.agent.id)
 
     @property
@@ -429,22 +550,96 @@
         the given time-step"""
         result = self.bb_read("reports_time", str(step))
         if result is not None:
             return result
         steps = sorted(
             int(i) for i in self.bb_query("reports_time", None, query_keys=True).keys()
         )
-        for (s, prev) in zip(steps[1:], steps[:-1]):
+        for s, prev in zip(steps[1:], steps[:-1]):
             if s > step:
                 return self.bb_read("reports_time", prev)
         return self.bb_read("reports_time", str(steps[-1]))
 
     # Negotiation set information
     # ---------------------------
 
     @property
     def current_input_issues(self) -> list[Issue]:
         return self._world._current_issues[self.my_input_product]
 
     @property
     def current_output_issues(self) -> list[Issue]:
         return self._world._current_issues[self.my_output_product]
+
+    @property
+    def current_input_outcome_space(self) -> DiscreteCartesianOutcomeSpace:
+        return make_os(self._world._current_issues[self.my_input_product])
+
+    @property
+    def current_output_outcome_space(self) -> DiscreteCartesianOutcomeSpace:
+        return make_os(self._world._current_issues[self.my_output_product])
+
+    @property
+    def current_negotiation_details(self) -> dict[str, dict[str, NegotiationDetails]]:
+        """
+        Details of current negotiations separated as two dicts for buying and selling.
+
+        Remarks:
+            - current_negotiation_details["buy"] gives details on all negotiations for buying
+            - current_negotiation_details["sell"] gives details on all negotiations for selling
+        """
+        return self._world._agent_negotiations.get(
+            self.agent.id, dict(buy=dict(), sell=dict())
+        )
+
+    # Sales and supplies
+
+    @property
+    def sales(self) -> dict[str, int]:
+        """Sales per customer so far (this day)"""
+        return self._sales
+
+    @property
+    def supplies(self) -> dict[str, int]:
+        """Supplies per supplier so far (this day)"""
+        return self._supplies
+
+    @property
+    def total_sales(self) -> int:
+        """Total sales so far (this day)"""
+        return sum(self._sales.values())
+
+    @property
+    def total_supplies(self) -> int:
+        """Total supplies so far (this day)"""
+        return sum(self._supplies.values())
+
+    @property
+    def needed_sales(self) -> int:
+        """Sales that need to be secured (exogenous input + total supplies - exogenous output - total sales so far)"""
+        return (
+            self.current_exogenous_input_quantity
+            + self.total_supplies
+            - self.total_sales
+            - self.current_exogenous_output_quantity
+        )
+
+    @property
+    def needed_supplies(self) -> int:
+        """Supplies that need to be secured (exogenous output + total sales - exogenous input - total supplies so far)"""
+        return (
+            self.current_exogenous_output_quantity
+            + sum(self._sales.values())
+            - self.current_exogenous_input_quantity
+            - self.total_supplies
+        )
+
+    # helper operations (sales and supplies) -- you do not need to call these.
+    def _register_sale(self, customer: str, value: int) -> None:
+        self._sales[customer] += value
+
+    def _register_supply(self, supplier: str, value: int) -> None:
+        self._supplies[supplier] += value
+
+    def _reset_sales_and_supplies(self) -> None:
+        self._sales = defaultdict(int)
+        self._supplies = defaultdict(int)
```

### Comparing `scml-0.5.6/src/scml/oneshot/helper.py` & `scml-0.6.0/src/scml/oneshot/helper.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/oneshot/mixins.py` & `scml-0.6.0/src/scml/oneshot/mixins.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/oneshot/sysagents.py` & `scml-0.6.0/src/scml/oneshot/sysagents.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,16 @@
     MechanismState,
     Negotiator,
     NegotiatorMechanismInterface,
     RenegotiationRequest,
 )
 from negmas.sao import ControlledSAONegotiator
 
+from scml.scml2019.common import QUANTITY
+
 from .agent import OneShotAgent
 from .awi import OneShotAWI
 from .helper import AWIHelper
 from .mixins import OneShotUFunCreatorMixin
 
 __all__ = ["DefaultOneShotAdapter", "_SystemAgent"]
 
@@ -36,15 +38,27 @@
 
     def make_ufun(self, add_exogenous: bool):
         return super().make_ufun(add_exogenous, in_adapter=False)
 
     def on_negotiation_failure(self, partners, annotation, mechanism, state):
         return self._obj.on_negotiation_failure(partners, annotation, mechanism, state)
 
-    def on_negotiation_success(self, contract, mechanism):
+    def on_negotiation_success(self, contract: Contract, mechanism):
+        if contract.annotation["buyer"] == self.id:
+            self.awi._register_supply(
+                contract.annotation["seller"], contract.agreement["quantity"]
+            )
+        elif contract.annotation["seller"] == self.id:
+            self.awi._register_sale(
+                contract.annotation["buyer"], contract.agreement["quantity"]
+            )
+        else:
+            raise ValueError(
+                f"{self.id} received a  contract for which it is not a buyer nor a seller: {contract=}"
+            )
         return self._obj.on_negotiation_success(contract, mechanism)
 
     def on_contract_executed(self, contract: Contract) -> None:
         pass
 
     def on_contract_breached(
         self, contract: Contract, breaches: List[Breach], resolution: Optional[Contract]
@@ -65,14 +79,15 @@
         super().init()
 
     def reset(self):
         if hasattr(self._obj, "reset"):
             self._obj.reset()
 
     def before_step(self):
+        self.awi._reset_sales_and_supplies()
         if hasattr(self._obj, "before_step"):
             self._obj.before_step()
 
     def to_dict(self):
         return {
             "id": self.id,
             "name": self.name,
```

### Comparing `scml-0.5.6/src/scml/oneshot/ufun.py` & `scml-0.6.0/src/scml/oneshot/ufun.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/oneshot/world.py` & `scml-0.6.0/src/scml/oneshot/world.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,30 +7,31 @@
 """
 import copy
 import itertools
 import logging
 import math
 import random
 import sys
+import warnings
 from collections import defaultdict
 from typing import Any, Callable, Collection, Iterable
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 from matplotlib.axis import Axis
 from negmas import (
     DEFAULT_EDGE_TYPES,
     Agent,
     Breach,
     BreachProcessing,
+    ContiguousIssue,
     Contract,
-    DiscreteIssue,
-    Issue,
     Operations,
+    SAOResponse,
     TimeInAgreementMixin,
     World,
     make_issue,
 )
 from negmas.helpers import get_class, get_full_type_name, instantiate, unique_name
 from negmas.sao import ControlledSAONegotiator, SAOController, SAONegotiator
 
@@ -47,15 +48,15 @@
     INFINITE_COST,
     SYSTEM_BUYER_ID,
     SYSTEM_SELLER_ID,
     is_system_agent,
 )
 from .adapter import OneShotSCML2020Adapter
 from .agent import OneShotAgent
-from .common import OneShotExogenousContract, OneShotProfile
+from .common import NegotiationDetails, OneShotExogenousContract, OneShotProfile
 from .sysagents import DefaultOneShotAdapter, _SystemAgent
 
 __all__ = [
     "SCML2020OneShotWorld",
     "SCML2021OneShotWorld",
     "SCML2022OneShotWorld",
     "SCML2023OneShotWorld",
@@ -122,14 +123,15 @@
         # mechanism params
         neg_n_steps=20,
         neg_time_limit=None,
         neg_hidden_time_limit=3 * 60,
         neg_step_time_limit=60,
         negotiation_speed=0,
         shuffle_negotiations=False,
+        one_offer_per_step=False,
         # public information
         publish_exogenous_summary=True,
         publish_trading_prices=True,
         # negotiation params,
         price_multiplier=0.0,
         wide_price_range=False,
         # trading price parameters
@@ -143,14 +145,18 @@
         agent_name_reveals_position: bool = True,
         agent_name_reveals_type: bool = True,
         # evaluation paramters (for compatibility with SCML2020World)
         inventory_valuation_catalog=0,
         inventory_valuation_trading=0,
         **kwargs,
     ):
+        # neg_n_steps is ALWAYS the number of rounds. We multiply it by 2 if mechanisms are stepped one offer at a time
+        if one_offer_per_step and neg_n_steps is not None:
+            neg_n_steps *= 2
+
         self._profits: dict[str, list[float]] = defaultdict(list)
         self._breach_levels: dict[str, list[float]] = defaultdict(list)
         self._breaches_of: dict[str, list[bool]] = defaultdict(list)
         self.trading_price_discount = trading_price_discount
         self.catalog_quantities = catalog_quantities
         self.publish_exogenous_summary = publish_exogenous_summary
         self.price_multiplier = price_multiplier
@@ -193,14 +199,15 @@
                         dynamic_entry=False,
                         max_wait=len(agent_types),
                         check_offers=True,
                         enforce_issue_types=True,
                         cast_offers=True,
                         hidden_time_limit=neg_hidden_time_limit,
                         sync_calls=sync_calls,
+                        one_offer_per_step=one_offer_per_step,
                     ),
                 )
             },
             default_signing_delay=signing_delay,
             n_steps=n_steps,
             time_limit=time_limit,
             negotiation_speed=negotiation_speed,
@@ -567,31 +574,31 @@
         self.exogenous_pout = defaultdict(int)
         self.exogenous_pin = defaultdict(int)
         self.exogenous_contracts_summary = None
 
         self.initial_balances = dict(zip(self.agents.keys(), initial_balance))
         self._max_n_lines = max(_.n_lines for _ in self.profiles)
         self.a2i = dict(zip((_.id for _ in agents), range(n_agents)))
-        self._current_issues: list[list[Issue]] = []
+        self._current_issues: list[list[ContiguousIssue]] = []
         self.__contracts: dict[str, list[Contract]] = defaultdict(list)
 
         def values(x: int | tuple[int, int]):
             if not isinstance(x, Iterable):
                 return int(x), int(x)
             return int(x[0]), int(x[1])
 
         for product in range(self.n_products):
             unit_price, time, quantity = self._make_issues(product)
-            self._current_issues.append(
-                [
-                    make_issue(values(quantity), name="quantity"),
-                    make_issue(values(time), name="time"),
-                    make_issue(values(unit_price), name="unit_price"),
-                ]
-            )
+            _issues = [
+                make_issue(values(quantity), name="quantity"),
+                make_issue(values(time), name="time"),
+                make_issue(values(unit_price), name="unit_price"),
+            ]
+            assert all(isinstance(_, ContiguousIssue) for _ in _issues)
+            self._current_issues.append(_issues)
 
         def to_lists(d):
             return {
                 k: v.tolist() if isinstance(v, np.ndarray) else list(v)
                 for k, v in d.items()
             }
 
@@ -612,14 +619,18 @@
             )
         )
         self.info.update(dict(agent_inputs=to_lists(self.agent_inputs)))
         self.info.update(dict(agent_outputs=to_lists(self.agent_outputs)))
         self.info.update(dict(agent_processes=to_lists(self.agent_processes)))
         self.info.update(dict(agent_initial_balances=self.initial_balances))
         self._update_exogenous(0)
+        self._current_negotiations: list[NegotiationDetails] = []
+        self._agent_negotiations: dict[
+            str, dict[str, dict[str, NegotiationDetails]]
+        ] = dict()
 
     @classmethod
     def generate(
         cls,
         agent_types: list[str | type[OneShotAgent]],
         agent_params: list[dict[str, Any]] | None = None,
         agent_processes: list[int] | None = None,
@@ -681,15 +692,14 @@
             agent_processes: The process for each agent. If not `None` , it will override `n_agents_per_process` and must be a list/tuple
                              of the same length as `agent_types` . Morevoer, `random_agent_types` must be False in this case
             cost_increases_with_level: If true, production cost will be higher for processes nearer to the final
                                        product.
             profit_basis: The statistic used when controlling catalog prices by profit arguments. It can be np.mean,
                           np.median, np.min, np.max or any Callable[[list[float]], float] and is used to summarize
                           production costs at every level.
-            horizon: The horizon used for revealing external supply/sales as a fraction of n_steps
             equal_exogenous_supply: If true, external supply will be distributed equally among all agents in the first
                                    layer
             equal_exogenous_sales: If true, external sales will be distributed equally among all agents in the last
                                    layer
             exogenous_supply_predictability: How predictable are exogenous supplies of each agent over time. 1.0 means
                                              that every agent will have the same quantity for all of its contracts over
                                              time. 0.0 means quantities per agent are completely random
@@ -712,15 +722,15 @@
             exogenous_price_dev: The standard deviation of exogenous contract prices relative to the mean price
             price_multiplier: A value to multiply with trading/catalog price to get the upper limit on prices for all negotiations
             random_agent_types: If True, the final agent types used by the generato wil always be sampled from the given types.
                                 If False, this random sampling will only happin if len(agent_types) != n_agents.
             penalties_scale: What are `disposal_cost` and `shortfall_penalty` relative to.
                             There are four options: `trading`, `catalog` mean trading
                             and catalog prices of the product. `unit` means the unit
-                            price in the contract and `non` means the `storage-cost`
+                            price in the contract and `none` means the `storage-cost`
                             and `shortfall_penalty` are absolute values (in money unit).
                             If not given will be read through the AWI
             method: the generation method. This is only for compatibility with SCML2020World and is not used.
             **kwargs:
 
         Returns:
 
@@ -740,15 +750,15 @@
               supported on $[i, j]$ inclusive. If it is a list of values, of the length `n_processes` , it is used as
               it is otherwise, it is used to sample values for each process.
 
         """
         if agent_processes is not None and random_agent_types:
             raise ValueError(
                 "You cannot pass `agent_processes` and use `random_agent_types`. The first is only "
-                "used when you want to fix the assignment of all agents to specific processes which is compatible with randomizing agnet types"
+                "used when you want to fix the assignment of all agents to specific processes"
             )
         if agent_processes is not None and len(agent_processes) != len(agent_types):
             raise ValueError(
                 f"Length of `agent_processes` ({len(agent_processes)}) must equal the length of `agent_types` ({len(agent_types)})"
             )
         info = dict(
             n_steps=n_steps,
@@ -1281,14 +1291,50 @@
                 if SYSTEM_SELLER_ID in contract.partners:
                     contract.signatures[SYSTEM_SELLER_ID] = SYSTEM_SELLER_ID
                 else:
                     contract.signatures[SYSTEM_BUYER_ID] = SYSTEM_BUYER_ID
         if self.exogenous_dynamic:
             raise NotImplementedError("Exogenous-dynamic is not yet implemented")
 
+    def step_with(self, actions: dict[str, dict[str, SAOResponse]], init=False) -> bool:
+        """
+        Runs a simulation step for the agents given in keys passing the corresponding values as counter offers.
+
+        Returns:
+            False if this is the last negotiation.
+
+        Remarks:
+            - You must call this with `init=True` once at the beginning of every simulation to
+              make sure that `init()` and other initialization code is called correctly.
+            - Every step advances all negotiations one step.
+            - Negotiators belonging to the given agents are never called as long as a corresponding
+              action (response) is given in the agents dict.
+            - The world MUST be created with `one_offer_per_step` passed as `True` (default is `False`).
+        """
+        from scml.oneshot.awi import OneShotAWI
+
+        actions = dict()
+        for agent, responses in actions.items():
+            awi: OneShotAWI = self.agents[agent].awi  # type: ignore
+            negotiations = awi.current_negotiation_details["buy"].copy()
+            negotiations.update(awi.current_negotiation_details["sell"])
+            for partner, neg in negotiations.items():
+                neg: NegotiationDetails
+                mynegs = [
+                    _ for _ in neg.nmi.mechanism.negotiators if _.owner.id == agent
+                ]
+                assert len(mynegs) == 0
+                assert neg.nmi.mechanism.one_offer_per_step  # type: ignore
+                response = responses.get(partner, None)
+                if response is not None:
+                    actions[neg.nmi.mechanism.id] = {mynegs[0]: response}
+                else:
+                    warnings.warn(f"{agent=} has no response for partner {partner}")
+        return self.step(n_neg_steps=int(not init), actions=actions)
+
     def simulation_step(self, stage):
         s = self.current_step
 
         if stage == 0:
             self._update_exogenous(s)
 
             # publish public information
@@ -1432,14 +1478,24 @@
             reports_agent = self.bulletin_board.data["reports_agent"]
             reports_time = self.bulletin_board.data["reports_time"]
             for aid, agent in self.agents.items():
                 if is_system_agent(agent.id):
                     continue
                 self.add_financial_report(agent, reports_agent, reports_time)
 
+        # Clean negotiation details
+        # -------------------------
+        self._current_negotiations = []
+        self._agent_negotiations = dict(
+            zip(
+                [_ for _ in self.agents.keys()],
+                [dict(buy=dict(), sell=dict()) for _ in self.agents.keys()],
+            )
+        )
+
     def _breach_record(
         self,
         perpetrator,
         level,
         type_,
     ) -> dict[str, Any]:
         return {
@@ -1880,14 +1936,36 @@
         result = self.request_negotiation_about(
             caller=agent,
             issues=issues,
             partners=[self.agents[_] for _ in partners],
             req_id=req_id,
             annotation=annotation,
         )
+        if result:
+            seller = [_ for _ in partners if _ != agent.id][0]
+            buyer = agent.id
+            assert result.mechanism is not None
+            self._current_negotiations = NegotiationDetails(
+                seller=seller,
+                buyer=buyer,
+                nmi=result.mechanism.nmi,  # type: ignore
+                product=product,
+            )
+            self._agent_negotiations[seller]["sell"][buyer] = NegotiationDetails(
+                seller=seller,
+                buyer=buyer,
+                nmi=result.mechanism.nmi,  # type: ignore
+                product=product,
+            )
+            self._agent_negotiations[buyer]["buy"][seller] = NegotiationDetails(
+                seller=seller,
+                buyer=buyer,
+                nmi=result.mechanism.nmi,  # type: ignore
+                product=product,
+            )
         # if result:
         #     self._registered_negs.add(tuple(sorted([partner, agent_id])))
         return result
 
     def _make_issues(
         self, product
     ) -> tuple[tuple[int, int], tuple[int, int], tuple[int, int]]:
@@ -1947,25 +2025,30 @@
 
         for aid, a in self.agents.items():
             if is_system_agent(aid) or isinstance(a, OneShotSCML2020Adapter):
                 continue
             controllers[aid] = a.adapted_object
             a.adapted_object.make_ufun(add_exogenous=True)
 
+        # initialize negotiation details
+        self._current_negotiations = []
+        self._agent_negotiations = dict(
+            zip(
+                [_ for _ in self.agents.keys()],
+                [dict(buy=dict(), sell=dict()) for _ in self.agents.keys()],
+            )
+        )
+
         for product in range(1, self.n_products):
             unit_price, time, quantity = self._make_issues(product)
             self._current_issues[product] = [
-                DiscreteCardinalIssue(values(quantity), name="quantity"),
-                DiscreteCardinalIssue(values(time), name="time"),
-                DiscreteCardinalIssue(values(unit_price), name="unit_price"),
+                make_issue(values(quantity), name="quantity"),
+                make_issue(values(time), name="time"),
+                make_issue(values(unit_price), name="unit_price"),
             ]
-            # for ii in self._current_issues[product]:
-            #     assert isinstance(
-            #         ii, DiscreteCardinalIssue
-            #     ), f"Issue {ii.name} has type {type(ii.name)}"
             requesting_agents = (
                 self.consumers[product] if consumer_starts else self.suppliers[product]
             )
             for aid in requesting_agents:
                 if is_system_agent(aid) or isinstance(
                     self.agents[aid], OneShotSCML2020Adapter
                 ):
```

### Comparing `scml-0.5.6/src/scml/scml2019/__init__.py` & `scml-0.6.0/src/scml/scml2019/__init__.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/agent.py` & `scml-0.6.0/src/scml/scml2019/agent.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/awi.py` & `scml-0.6.0/src/scml/scml2019/awi.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/bank.py` & `scml-0.6.0/src/scml/scml2019/bank.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/common.py` & `scml-0.6.0/src/scml/scml2019/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/consumers.py` & `scml-0.6.0/src/scml/scml2019/consumers.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/factory_managers/builtins.py` & `scml-0.6.0/src/scml/scml2019/factory_managers/builtins.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/helpers.py` & `scml-0.6.0/src/scml/scml2019/helpers.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/insurance.py` & `scml-0.6.0/src/scml/scml2019/insurance.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/miners.py` & `scml-0.6.0/src/scml/scml2019/miners.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/schedulers.py` & `scml-0.6.0/src/scml/scml2019/schedulers.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/simulators.py` & `scml-0.6.0/src/scml/scml2019/simulators.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/utils.py` & `scml-0.6.0/src/scml/scml2019/utils.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/visualizers.py` & `scml-0.6.0/src/scml/scml2019/visualizers.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2019/world.py` & `scml-0.6.0/src/scml/scml2019/world.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/__init__.py` & `scml-0.6.0/src/scml/scml2020/__init__.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/agent.py` & `scml-0.6.0/src/scml/scml2020/agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Implements the world class for the SCML2020 world """
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
 import numpy as np
 from negmas import (
     Agent,
     Breach,
     Contract,
+    DiscreteCartesianOutcomeSpace,
     Issue,
     MechanismState,
     Negotiator,
     NegotiatorMechanismInterface,
     RenegotiationRequest,
     make_issue,
+    make_os,
 )
 from negmas.helpers import get_full_type_name, instantiate
 from negmas.situated import Adapter
 
 from ..oneshot.agent import OneShotAgent
 from ..oneshot.common import OneShotProfile, OneShotState
 from ..oneshot.mixins import OneShotUFunCreatorMixin
@@ -342,25 +344,70 @@
         return self.my_input_product
 
     @property
     def profile(self) -> OneShotProfile:
         """Gets the profile (static private information) associated with the agent"""
         return self._owner.get_profile()
 
-    def state(self) -> Any:
+    def state(self) -> OneShotState:
         q, p = self._owner.get_exogenous_input()
         qo, po = self._owner.get_exogenous_output()
+        # TODO add missing components
+        all_agents = [_ for _ in self._world.agents.keys() if self.is_system(_)]
         return OneShotState(
             exogenous_input_quantity=q,
             exogenous_input_price=p,
             exogenous_output_quantity=qo,
             exogenous_output_price=po,
             disposal_cost=self._owner.get_disposal_cost(),
             shortfall_penalty=self._owner.get_shortfall_penalty(),
             current_balance=self._owner.get_current_balance(),
+            total_sales=0,
+            total_supplies=0,
+            n_products=self.n_products,
+            n_processes=self.n_processes,
+            n_competitors=self.n_competitors,
+            all_suppliers=self.all_suppliers,
+            all_consumers=self.all_consumers,
+            catalog_prices=self.catalog_prices.tolist(),
+            price_multiplier=1.0,
+            is_exogenous_forced=False,
+            current_step=self._owner.awi.current_step,
+            n_steps=self._owner.awi.n_steps,
+            relative_simulation_time=self._owner.awi.relative_time,
+            profile=self.profile,
+            n_lines=self.n_lines,
+            is_first_level=self.is_first_level,
+            is_last_level=self.is_last_level,
+            is_middle_level=self.is_middle_level,
+            my_input_product=self.my_input_product,
+            my_output_product=self.my_output_product,
+            level=self.level,
+            my_suppliers=self.my_suppliers,
+            my_consumers=self.my_consumers,
+            penalties_scale=self.penalties_scale,
+            n_input_negotiations=self.n_input_negotiations,
+            n_output_negotiations=self.n_output_negotiations,
+            trading_prices=self.trading_prices.tolist(),
+            exogenous_contract_summary=self.exogenous_contract_summary,
+            current_input_outcome_space=self.current_input_outcome_space,
+            current_output_outcome_space=self.current_output_outcome_space,
+            current_negotiation_details=dict(),
+            sales=dict(),
+            supplies=dict(),
+            needed_sales=0,
+            needed_supplies=0,
+            bankrupt_agents=[_ for _ in all_agents if self.is_bankrupt(_)],
+            reports_of_agents=dict(
+                zip(
+                    all_agents,
+                    [self.reports_of_agent(_) for _ in all_agents],
+                )
+            ),
+            running_negotiations=dict(),
         )
 
     @property
     def price_multiplier(self):
         return self._owner.price_multiplier
 
     @property
@@ -424,15 +471,25 @@
                 make_issue(values=q, name="quantity"),
                 make_issue(values=t, name="time"),
                 make_issue(values=u, name="unit_price"),
             ]
         return issues
 
     @property
-    def penalties_scale(self) -> str:
+    def current_input_outcome_space(self) -> DiscreteCartesianOutcomeSpace:
+        return make_os(self.current_input_issues) if self.current_input_issues else None
+
+    @property
+    def current_output_outcome_space(self) -> DiscreteCartesianOutcomeSpace:
+        return (
+            make_os(self.current_output_issues) if self.current_output_issues else None
+        )
+
+    @property
+    def penalties_scale(self) -> Literal["trading", "catalog", "input", "none"]:
         return "unit"
 
     # Public Information
     # ==================
     @property
     def exogenous_contract_summary(self) -> List[Tuple[int, int]]:
         """
```

### Comparing `scml-0.5.6/src/scml/scml2020/agents/bcse.py` & `scml-0.6.0/src/scml/scml2020/agents/bcse.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/agents/decentralizing.py` & `scml-0.6.0/src/scml/scml2020/agents/decentralizing.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/agents/do_nothing.py` & `scml-0.6.0/src/scml/scml2020/agents/do_nothing.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/agents/indneg.py` & `scml-0.6.0/src/scml/scml2020/agents/indneg.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/agents/moving.py` & `scml-0.6.0/src/scml/scml2020/agents/moving.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/agents/random.py` & `scml-0.6.0/src/scml/scml2020/agents/random.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/agents/reactive.py` & `scml-0.6.0/src/scml/scml2020/agents/reactive.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/agents/satisficer.py` & `scml-0.6.0/src/scml/scml2020/agents/satisficer.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,21 +47,17 @@
     # Negotiation Callbacks
     # =====================
 
     def propose(self, state: MechanismState) -> Optional[Outcome]:
         """Simply calls the corresponding method on the owner"""
         return self.owner.propose(state, self.nmi, self.is_selling, self.is_requested)
 
-    def respond(
-        self, state: MechanismState, offer: Outcome, source: str = ""
-    ) -> ResponseType:
+    def respond(self, state: MechanismState, source: str = "") -> ResponseType:
         """Simply calls the corresponding method on the owner"""
-        return self.owner.respond(
-            state, self.nmi, offer, self.is_selling, self.is_requested
-        )
+        return self.owner.respond(state, self.nmi, self.is_selling, self.is_requested)
 
 
 class SatisficerAgent(SCML2020Agent):
     """
     A simple monolithic agent that tries to *carefully* make small profit
     every step.
 
@@ -582,15 +578,15 @@
         partner = [_ for _ in ami.agent_ids if _ != self.id][0]
         tentative[t:] += q
         self.last_q[partner] = q
         self.last_t[partner] = t
 
         return tuple(offer)
 
-    def respond(self, state, ami, offer, is_selling, is_requested):
+    def respond(self, state, ami, is_selling, is_requested):
         """
         Responds to an offer from one partner.
 
         Args:
             state: mechanism state including current round
             ami: Agent-mechanism-interface for accessing the negotiation mechanism
             offer: The offer proposed by the partner
@@ -604,14 +600,15 @@
               of the negotiation.
             - During negotiation, the agent starts accepting highest/lowest prices
               for selling/buying and gradually conceeds to the minimally acceptable
               price (`good_price`) defined as being `acceptable_loss` above/below
               the trading price for buying/selling.
 
         """
+        offer = state.current_offer
         # Find the price range for this negotiation
         p0, p1 = ami.issues[UNIT_PRICE].min_value, ami.issues[UNIT_PRICE].max_value
 
         # Find current trading prices (catalog price if trading prices are not available)
         awi: AWI = self.awi
         prices = awi.trading_prices
         if prices is None:
```

### Comparing `scml-0.5.6/src/scml/scml2020/awi.py` & `scml-0.6.0/src/scml/scml2020/awi.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/common.py` & `scml-0.6.0/src/scml/scml2020/common.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/components/negotiation.py` & `scml-0.6.0/src/scml/scml2020/components/negotiation.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/components/prediction.py` & `scml-0.6.0/src/scml/scml2020/components/prediction.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/components/production.py` & `scml-0.6.0/src/scml/scml2020/components/production.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/components/signing.py` & `scml-0.6.0/src/scml/scml2020/components/signing.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/components/simulation.py` & `scml-0.6.0/src/scml/scml2020/components/simulation.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/components/trading.py` & `scml-0.6.0/src/scml/scml2020/components/trading.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/factory.py` & `scml-0.6.0/src/scml/scml2020/factory.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/services/controllers.py` & `scml-0.6.0/src/scml/scml2020/services/controllers.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,28 +141,27 @@
             self.__negotiator._nmi = None
         return self.__negotiator.propose(state)
 
     def respond(
         self,
         negotiator_id: str,
         state: MechanismState,
-        offer: "Outcome",
         source: str = "",
     ) -> ResponseType:
         if negotiator_id not in self.negotiators.keys():
             return ResponseType.END_NEGOTIATION
         if self.secured >= self.target:
             return ResponseType.END_NEGOTIATION
         # if negotiator_id not in self.negotiators:
         #     breakpoint()
         self.__negotiator._nmi = self.negotiators[negotiator_id][0].nmi
         try:
-            return self.__negotiator.respond(offer=offer, state=state, source=source)
+            return self.__negotiator.respond(state=state, source=source)
         except TypeError:
-            return self.__negotiator.respond(offer=offer, state=state)
+            return self.__negotiator.respond(state=state)
 
     def __str__(self):
         return (
             f"{'selling' if self.is_seller else 'buying'} p{self.product} [{self.step}] "
             f"secured {self.secured} of {self.target} for {self.parent_name} "
             f"({len([_ for _ in self.completed.values() if _])} completed of {len(self.completed)} negotiators)"
         )
```

### Comparing `scml-0.5.6/src/scml/scml2020/services/simulators.py` & `scml-0.6.0/src/scml/scml2020/services/simulators.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/scml2020/utils.py` & `scml-0.6.0/src/scml/scml2020/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,31 +15,25 @@
 from negmas.serialization import deserialize, serialize
 from negmas.tournaments import TournamentResults, WorldRunResults, tournament
 
 from scml.oneshot.agents import (
     GreedyOneShotAgent,
     GreedySyncAgent,
     SingleAgreementAspirationAgent,
+    SyncRandomOneShotAgent,
 )
 from scml.oneshot.sysagents import _SystemAgent as OneShotSysAgent
-from scml.oneshot.world import SCML2020OneShotWorld
-from scml.scml2019.utils import anac2019_config_generator
 from scml.scml2020.agent import _SystemAgent as StdSysAgent
 from scml.scml2020.agents import (
     BuyCheapSellExpensiveAgent,
     DecentralizingAgent,
     MarketAwareIndDecentralizingAgent,
     SatisficerAgent,
 )
-from scml.scml2020.world import (
-    SCML2020Agent,
-    SCML2020World,
-    SCML2022World,
-    is_system_agent,
-)
+from scml.scml2020.world import SCML2020Agent, SCML2020World, is_system_agent
 
 __all__ = [
     "anac_config_generator_oneshot",
     "anac_config_generator_std",
     "anac_config_generator_collusion",
     "anac_assigner_oneshot",
     "anac_assigner_std",
@@ -106,14 +100,20 @@
 
 DefaultAgentsOneShot = [
     GreedyOneShotAgent,
     SingleAgreementAspirationAgent,
     GreedySyncAgent,
 ]
 
+DefaultAgentsOneShot2023 = [
+    GreedyOneShotAgent,
+    SingleAgreementAspirationAgent,
+    SyncRandomOneShotAgent,
+]
+
 
 def integer_cut(
     n: int,
     l: int,
     l_m: int | list[int],
     l_max: int | list[int] = float("inf"),  # type: ignore
 ) -> list[int]:
@@ -408,30 +408,37 @@
         "agent_params": manager_params,
     }
     config.update(kwargs)
     return [config]
 
 
 anac_config_generator_std = anac_config_generator
-anac_config_generator_oneshot = anac_config_generator
+
+
+def anac_config_generator_oneshot(*args, **kwargs):
+    if len(args) >= 5:
+        args = tuple(list(args[:4]) + [DefaultAgentsOneShot2023] + list(args[5:]))
+    else:
+        kwargs["non_competitors"] = DefaultAgentsOneShot2023
+    kwargs["oneshot_world"] = True
+    return anac_config_generator(*args, **kwargs)
 
 
 def anac_config_generator_collusion(
     year: int,
     n_competitors: int,
     n_agents_per_competitor: int,
     agent_names_reveal_type: bool = False,
     non_competitors: tuple[str | type[SCML2020Agent], ...] | None = None,
     non_competitor_params: tuple[dict[str, Any], ...] | None = None,
     *args,
     **kwargs,
 ) -> list[dict[str, Any]]:
     assert n_agents_per_competitor > 1
     return anac_config_generator(
-        *args,
         year=year,
         n_competitors=n_competitors,
         n_agents_per_competitor=n_agents_per_competitor,
         agent_names_reveal_type=agent_names_reveal_type,
         non_competitors=non_competitors,
         non_competitor_params=non_competitor_params,
         **kwargs,
@@ -574,15 +581,16 @@
                 n_min = len(assignable_factories)
                 n_rounds = int(max_n_worlds // n_min)
                 if n_rounds < 1:
                     raise ValueError(
                         f"Cannot guarantee fair assignment: n. competitors {len(assignable_factories)}, at least"
                         f" {n_min} runs are needed for fair assignment"
                     )
-                max_n_worlds = n_rounds * n_min
+                max_n_worlds = n_rounds * n_min if n_rounds > 0 else max_n_worlds
+                n_rounds = max(n_rounds, 1)
                 k = 0
                 for _ in range(n_rounds):
                     shuffle(permutation)
                     for __ in range(n_min):
                         k += 1
                         perm = copy.deepcopy(permutation)
                         perm = perm[-1:] + perm[:-1]
@@ -773,15 +781,15 @@
         )
     else:
         assert len(kwargs["world_params"]["agent_processes"]) == len(
             kwargs["world_params"]["agent_types"]
         )
     cnfg = kwargs["world_params"].pop("__exact_params")
     cnfg = deserialize(cnfg)
-    kwargs["world_params"]["random_agent_typea"] = False
+    kwargs["world_params"]["random_agent_types"] = False
     cls = get_class(f"scml.scml2020.world.SCML{int(year)}World")
     cnfg2 = cls.generate(**kwargs["world_params"])  # type: ignore
     for k in ("agent_types", "agent_params"):
         cnfg[k] = cnfg2[k]  # type: ignore
     for _p in cnfg["profiles"]:  # type: ignore
         _p.costs = np.asarray(_p.costs)  # type: ignore
     if "info" not in cnfg.keys():  # type: ignore
@@ -807,29 +815,30 @@
             kwargs["world_params"]["agent_types"]
         )
     # cnfg = SCML2020OneShotWorld.generate(**kwargs["world_params"])
     # for k in ("n_agents_per_process","n_processes"):
     #     del kwargs["world_params"][k]
     cnfg = kwargs["world_params"].pop("__exact_params")
     cnfg = deserialize(cnfg)
-    kwargs["world_params"]["random_agent_typea"] = False
+    kwargs["world_params"]["random_agent_types"] = False
     cls = get_class(f"scml.oneshot.world.SCML{int(year)}OneShotWorld")
     cnfg2 = cls.generate(**kwargs["world_params"])
     for k in ("agent_types", "agent_params", "name"):
         cnfg[k] = cnfg2[k]
     if "info" not in cnfg.keys():
         cnfg["info"] = dict()
     cnfg["info"]["is_default"] = kwargs["is_default"]
     world = cls(**cnfg)
     return world
 
 
 anac2021_oneshot_world_generator = partial(anac_oneshot_world_generator, year=2021)
 anac2022_oneshot_world_generator = partial(anac_oneshot_world_generator, year=2022)
 anac2023_oneshot_world_generator = partial(anac_oneshot_world_generator, year=2023)
+anac2024_oneshot_world_generator = partial(anac_oneshot_world_generator, year=2024)
 
 
 def balance_calculator(
     worlds: list[SCML2020World],
     scoring_context: dict[str, Any],
     dry_run: bool,
     ignore_default=True,
@@ -955,22 +964,23 @@
 balance_calculator2020 = partial(balance_calculator, consolidated=False)
 balance_calculator2021 = partial(balance_calculator, consolidated=False)
 balance_calculator2022 = partial(balance_calculator, consolidated=True)
 balance_calculator2023 = partial(balance_calculator, consolidated=True)
 
 
 def balance_calculator_collusion(
-    year: int,
     worlds: list[SCML2020World],
     scoring_context: dict[str, Any],
     dry_run: bool,
+    year: int,
     ignore_default=True,
     inventory_catalog_price_weight=0.0,
     inventory_trading_average_weight=0.5,
     raw_collusion_score_multiplier=0.2,
+    **kwargs,
 ) -> WorldRunResults:
     """A scoring function that scores factory managers' performance by the
     final balance only ignoring whatever still in their inventory after
     consolidating all factories in the simulation that belong to the same
     agent type.
 
     Args:
```

### Comparing `scml-0.5.6/src/scml/scml2020/world.py` & `scml-0.6.0/src/scml/scml2020/world.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/vendor/quick/LICENSE` & `scml-0.6.0/src/scml/vendor/quick/LICENSE`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/vendor/quick/README.md` & `scml-0.6.0/src/scml/vendor/quick/README.md`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml/vendor/quick/quick.py` & `scml-0.6.0/src/scml/vendor/quick/quick.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/src/scml.egg-info/PKG-INFO` & `scml-0.6.0/src/scml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scml
-Version: 0.5.6
+Version: 0.6.0
 Summary: ANAC Supply Chain Management League Platform
 Home-page: https://github.com/yasserfarouk/scml
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Project-URL: Documentation, https://scml.readthedocs.io/
 Project-URL: Changelog, https://scml.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/yasserfarouk/scml/issues
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: gui
+Provides-Extra: rl
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 ========
 Overview
 ========
 
@@ -84,14 +85,23 @@
       - ::
 
             PYTEST_ADDOPTS=--cov-append tox
 
 Changelog
 =========
 
+0.6.0 (2023.7.9)
+----------------
+
+* Upgrading to be compatible with NegMAS 0.10.0
+* Adding step_with() to oneshot allowing for single counter-offer set stepping of the simulation (to be used to expose the simulation as RL and MARL environments later).
+* Adding current_negotiation_details to OneShotAWI to get details of running negotiation
+* Adding managed sales, supplies, total_sales, total_supplies, needed_sales, and needed_supplies to the OneShotAWI
+* Extending OneShotState returned from awi.state and awi.default_state_encoder(mechanism_states) to expose more information about the simulation
+
 0.5.6 (2023.3.8)
 ----------------
 
 * Upgrading to be compatible with NegMAS 0.9.8
 * Updating notebooks for 2023 release
 * Adding 2023 specific classes and utility functions
 * Supporting most recent negmas version on Github
```

### Comparing `scml-0.5.6/src/scml.egg-info/SOURCES.txt` & `scml-0.6.0/src/scml.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 src/scml/oneshot/__init__.py
 src/scml/oneshot/adapter.py
 src/scml/oneshot/agent.py
 src/scml/oneshot/awi.py
 src/scml/oneshot/common.py
 src/scml/oneshot/helper.py
 src/scml/oneshot/mixins.py
+src/scml/oneshot/policy.py
 src/scml/oneshot/sysagents.py
 src/scml/oneshot/ufun.py
 src/scml/oneshot/world.py
 src/scml/oneshot/agents/__init__.py
 src/scml/oneshot/agents/aspiration.py
 src/scml/oneshot/agents/greedy.py
 src/scml/oneshot/agents/nothing.py
@@ -103,8 +104,10 @@
 tests/test_scml2019tournaments.py
 tests/test_scml2020.py
 tests/test_scml2020factory.py
 tests/test_scml2020tournaments.py
 tests/test_scml2021.py
 tests/test_scml2021oneshot.py
 tests/test_scml2021tournaments.py
+tests/test_scml2023.py
+tests/test_scml2023oneshot.py
 tests/test_sync_jackson.py
```

### Comparing `scml-0.5.6/tests/switches.py` & `scml-0.6.0/tests/switches.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_can_run_tutorial2.py` & `scml-0.6.0/tests/test_can_run_tutorial2.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 from pprint import pprint
 from time import sleep
 
 import numpy as np
 import pandas as pd
 import pytest
 from negmas import ResponseType, SAOResponse
+from negmas.genius.bridge import genius_bridge_is_running
 
 # used to check whether or not the negmas-genius bridge
 # is running
 # import a specific agent from the Genius platform
-from negmas.genius import NiceTitForTat, genius_bridge_is_running
+from negmas.genius.gnegotiators import NiceTitForTat
 from negmas.outcomes import Outcome
 from negmas.preferences import LinearAdditiveUtilityFunction, LinearUtilityFunction
 from negmas.preferences.value_fun import AffineFun, IdentityFun
 
 from scml.oneshot import *
 from scml.oneshot import OneShotIndNegotiatorsAgent
 from scml.scml2020 import is_system_agent
@@ -78,15 +79,15 @@
 
 class MyOneShotDoNothing(OneShotAgent):
     """My Agent that does nothing"""
 
     def propose(self, negotiator_id, state):
         return None
 
-    def respond(self, negotiator_id, state, offer):
+    def respond(self, negotiator_id, state):
         return ResponseType.END_NEGOTIATION
 
 
 class SimpleAgent(OneShotAgent):
     """A greedy agent based on OneShotAgent"""
 
     def before_step(self):
@@ -94,15 +95,16 @@
 
     def on_negotiation_success(self, contract, mechanism):
         self.secured += contract.agreement["quantity"]
 
     def propose(self, negotiator_id: str, state) -> Outcome:
         return self.best_offer(negotiator_id)
 
-    def respond(self, negotiator_id, state, offer, source: str = ""):
+    def respond(self, negotiator_id, state, source: str = ""):
+        offer = state.current_offer
         my_needs = self._needed(negotiator_id)
         if my_needs <= 0:
             return ResponseType.END_NEGOTIATION
         return (
             ResponseType.ACCEPT_OFFER
             if offer[QUANTITY] <= my_needs
             else ResponseType.REJECT_OFFER
@@ -150,16 +152,17 @@
         offer = super().propose(negotiator_id, state)
         if not offer:
             return None
         offer = list(offer)
         offer[UNIT_PRICE] = self._find_good_price(self.get_nmi(negotiator_id), state)
         return tuple(offer)
 
-    def respond(self, negotiator_id, state, offer, source=""):
-        response = super().respond(negotiator_id, state, offer, source)
+    def respond(self, negotiator_id, state, source=""):
+        offer = state.current_offer
+        response = super().respond(negotiator_id, state, source)
         if response != ResponseType.ACCEPT_OFFER:
             return response
         ami = self.get_nmi(negotiator_id)
         return (
             response
             if self._is_good_price(ami, state, offer[UNIT_PRICE])
             else ResponseType.REJECT_OFFER
@@ -199,17 +202,18 @@
 class AdaptiveAgent(BetterAgent):
     """Considers best price offers received when making its decisions"""
 
     def before_step(self):
         super().before_step()
         self._best_selling, self._best_buying = 0.0, float("inf")
 
-    def respond(self, negotiator_id, state, offer, source=""):
+    def respond(self, negotiator_id, state, source=""):
         """Save the best price received"""
-        response = super().respond(negotiator_id, state, offer, source)
+        offer = state.current_offer
+        response = super().respond(negotiator_id, state, source)
         ami = self.get_nmi(negotiator_id)
         if self._is_selling(ami):
             self._best_selling = max(offer[UNIT_PRICE], self._best_selling)
         else:
             self._best_buying = min(offer[UNIT_PRICE], self._best_buying)
         return response
 
@@ -272,17 +276,18 @@
         else:
             partner = contract.annotation["seller"]
             self._best_acc_buying = min(up, self._best_acc_buying)
             self._best_opp_acc_buying[partner] = min(
                 up, self._best_opp_acc_buying[partner]
             )
 
-    def respond(self, negotiator_id, state, offer, source=""):
+    def respond(self, negotiator_id, state, source=""):
+        offer = state.current_offer
         # find the quantity I still need and end negotiation if I need nothing more
-        response = super().respond(negotiator_id, state, offer, source)
+        response = super().respond(negotiator_id, state, source)
         # update my current best price to use for limiting concession in other
         # negotiations
         ami = self.get_nmi(negotiator_id)
         up = offer[UNIT_PRICE]
         if self._is_selling(ami):
             partner = ami.annotation["buyer"]
             self._best_opp_selling[partner] = max(up, self._best_selling)
@@ -515,15 +520,15 @@
         LearningAgent,
         DeepSimpleAgent,
         MySyncOneShotDoNothing,
         SyncAgent,
         SimpleSingleAgreementAgent,
         AssumeOthersFailIndNeg,
         GreedyIndNeg,
-        GeniusIndNeg,
+        # GeniusIndNeg,
     ],
 )
 @pytest.mark.skipif(
     not SCML_RUN_TUTORIAL2,
     reason="Environment is set not to run this  test. Check switches.py for details",
 )
 def test_examples(agent_type):
```

### Comparing `scml-0.5.6/tests/test_factory2019.py` & `scml-0.6.0/tests/test_factory2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_jupyter.py` & `scml-0.6.0/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_oneshot_do_nothing.py` & `scml-0.6.0/tests/test_oneshot_do_nothing.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 class MyOneShotDoNothing(OneShotAgent):
     """My Agent that does nothing"""
 
     def propose(self, negotiator_id, state):
         # print(f"proposing to {negotiator_id} at {state.step}")
         return None
 
-    def respond(self, negotiator_id, state, offer):
+    def respond(self, negotiator_id, state):
+        offer = state.current_offer
         # print(f"proposing to {negotiator_id} for {offer} at {state.step}")
         return ResponseType.REJECT_OFFER
 
     def on_negotiation_end(self, negotiator_id: str, state) -> None:
         assert state.agreement is None
```

### Comparing `scml-0.5.6/tests/test_oneshot_sync.py` & `scml-0.6.0/tests/test_oneshot_sync.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_oneshot_ufun.py` & `scml-0.6.0/tests/test_oneshot_ufun.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_scheduler2019.py` & `scml-0.6.0/tests/test_scheduler2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_scml2019.py` & `scml-0.6.0/tests/test_scml2019.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_scml2019factory.py` & `scml-0.6.0/tests/test_scml2019factory.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_scml2019tournaments.py` & `scml-0.6.0/tests/test_scml2019tournaments.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_scml2020.py` & `scml-0.6.0/tests/test_scml2020.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_scml2020factory.py` & `scml-0.6.0/tests/test_scml2020factory.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_scml2020tournaments.py` & `scml-0.6.0/tests/test_scml2020tournaments.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_scml2021.py` & `scml-0.6.0/tests/test_scml2021.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_scml2021oneshot.py` & `scml-0.6.0/tests/test_scml2021oneshot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 from collections import defaultdict
 
 import hypothesis.strategies as st
 import numpy as np
 import pandas as pd
 import pytest
 from hypothesis import given, settings
-from negmas import ResponseType, genius_bridge_is_running, save_stats
-from negmas.genius import NiceTitForTat
+from negmas import ResponseType, save_stats
+from negmas.genius.bridge import genius_bridge_is_running
+from negmas.genius.gnegotiators import NiceTitForTat
 from negmas.helpers import unique_name
 from negmas.preferences import LinearAdditiveUtilityFunction
 from negmas.preferences.value_fun import AffineFun, ConstFun, IdentityFun, LinearFun
 from negmas.sao import SAOResponse
 from numpy.testing import assert_allclose
 from pytest import mark, raises
 
@@ -47,20 +48,23 @@
 #
 #     std_types += list(get_agents(2020, as_class=True, winners_only=True))
 # except ImportError:
 #     pass
 
 
 class MyOneShotAgent(RandomOneShotAgent):
-    def respond(self, negotiator_id, state, offer, source=""):
+    def respond(self, negotiator_id, state, source=""):
+        offer = state.current_offer
+        if offer is None:
+            return ResponseType.REJECT_OFFER
         assert (
             negotiator_id in self.awi.my_consumers
             or negotiator_id in self.awi.my_suppliers
         ), (self.id, self.name, negotiator_id)
-        return super().respond(negotiator_id, state, offer, source)
+        return super().respond(negotiator_id, state, source)
 
     def propose(self, negotiator_id, state):
         assert (
             negotiator_id in self.awi.my_consumers
             or negotiator_id in self.awi.my_suppliers
         ), (self.id, self.name, negotiator_id)
         return super().propose(negotiator_id, state)
@@ -1030,15 +1034,15 @@
     force_single_thread(False)
 
 
 class MyOneShotDoNothing(OneShotAgent):
     def propose(self, negotiator_id, state):
         return None
 
-    def respond(self, negotiator_id, state, offer):
+    def respond(self, negotiator_id, state):
         return ResponseType.END_NEGOTIATION
 
 
 def test_do_nothing_goes_bankrupt():
     world = generate_world([MyOneShotDoNothing], 2, 1000, 4, cash_availability=0.001)
     world.run()
     for aid, agent in world.agents.items():
@@ -1055,15 +1059,16 @@
 
     def top_outcome(self, negotiator_id):
         return tuple(_.max_value for _ in self.get_nmi(negotiator_id).issues)
 
     def propose(self, negotiator_id, state):
         return self.top_outcome(negotiator_id)
 
-    def respond(self, negotiator_id, state, offer):
+    def respond(self, negotiator_id, state):
+        offer = state.current_offer
         return (
             ResponseType.ACCEPT_OFFER
             if self.top_outcome(negotiator_id) == offer
             else ResponseType.REJECT_OFFER
         )
 
 
@@ -1169,15 +1174,16 @@
 #         if self.awi.is_last_level and not self.ufun.ok_to_buy_at(outcome[UNIT_PRICE]):
 #             return self.bottom_outcome(negotiator_id)
 #         return outcome
 #
 #     def accept_if(self, x):
 #         return ResponseType.ACCEPT_OFFER if x else ResponseType.REJECT_OFFER
 #
-#     def respond(self, negotiator_id, state, offer):
+#     def respond(self, negotiator_id, state):
+#         offer = state.current_offer
 #         if self.awi.is_first_level:
 #             return self.accept_if(self.ufun.ok_to_sell_at(offer[UNIT_PRICE]))
 #         if self.awi.is_last_level:
 #             return self.accept_if(self.ufun.ok_to_buy_at(offer[UNIT_PRICE]))
 #         return ResponseType.ACCEPT_OFFER
 #
 # def test_price_pumping_does_not_bankrupt_rational_random_agents():
```

### Comparing `scml-0.5.6/tests/test_scml2021tournaments.py` & `scml-0.6.0/tests/test_scml2021tournaments.py`

 * *Files identical despite different names*

### Comparing `scml-0.5.6/tests/test_sync_jackson.py` & `scml-0.6.0/tests/test_sync_jackson.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,18 @@
 
     def on_negotiation_success(self, contract, mechanism):
         self.secured += contract.agreement["quantity"]
 
     def propose(self, negotiator_id: str, state) -> Outcome | None:
         return self.best_offer(negotiator_id)
 
-    def respond(self, negotiator_id, state, offer, source):
+    def respond(self, negotiator_id, state, source=None):
+        offer = state.current_offer
+        if offer is None:
+            return ResponseType.REJECT_OFFER
         my_needs = self._needed(negotiator_id)
         if my_needs <= 0:
             return ResponseType.END_NEGOTIATION
         return (
             ResponseType.ACCEPT_OFFER
             if offer[QUANTITY] <= my_needs
             else ResponseType.REJECT_OFFER
@@ -86,16 +89,17 @@
             return None
         offer = list(offer)
         offer[UNIT_PRICE] = int(
             round(self._find_good_price(self.get_nmi(negotiator_id), state))
         )
         return tuple(offer)
 
-    def respond(self, negotiator_id, state, offer, source):
-        response = super().respond(negotiator_id, state, offer, source)
+    def respond(self, negotiator_id, state, source=None):
+        offer = state.current_offer
+        response = super().respond(negotiator_id, state, source=source)
         if response != ResponseType.ACCEPT_OFFER:
             return response
         nmi = self.get_nmi(negotiator_id)
         return (
             response
             if self._is_good_price(nmi, state, offer[UNIT_PRICE])
             else ResponseType.REJECT_OFFER
@@ -199,15 +203,16 @@
         super().__init__(*args, **kwargs)
         self.round_nums = defaultdict(int)
         self.max_round_diff = max_round_diff
 
     def step(self):
         self.round_nums = defaultdict(int)
 
-    def respond(self, negotiator_id, state, offer, source=""):
+    def respond(self, negotiator_id, state, source=""):
+        offer = state.current_offer
         assert state.running, (
             f"{self.id} called to respond in a negotiation that "
             f"is no longer running\n{state}\noffer:{offer}\npartner:{negotiator_id}"
         )
         self.round_nums[negotiator_id] += 1
         max_diff = max(self.round_nums.values()) - min(self.round_nums.values())
         if max_diff > self.max_round_diff:
@@ -238,15 +243,15 @@
                             msg += (
                                 f'\n{k.replace("_SAOSyncController__", "")}:{str(v)}\n'
                             )
                 raise AssertionError(msg)
                 # print(msg)
                 # log_str = f"{datetime.now()}: on round {self.round_nums[negotiator_id]} with opp {negotiator_id}"
                 # self.awi.logdebug_agent(log_str)
-        return super().respond(negotiator_id, state, offer, source)
+        return super().respond(negotiator_id, state, source=source)
 
     def on_negotiation_success(self, contract, mechanism):
         partners = [_ for _ in contract.partners if _ != self.id]
         assert (
             len(partners) == 1
         ), f"id={self.id}, partners={contract.partners}\n{contract}\n{mechanism.state}"
         if partners[0] in self.round_nums.keys():
```

### Comparing `scml-0.5.6/tox.ini` & `scml-0.6.0/tox.ini`

 * *Files identical despite different names*

