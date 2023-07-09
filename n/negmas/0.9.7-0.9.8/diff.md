# Comparing `tmp/negmas-0.9.7.tar.gz` & `tmp/negmas-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "negmas-0.9.7.tar", last modified: Tue Jan 24 11:32:15 2023, max compression
+gzip compressed data, was "negmas-0.9.8.tar", last modified: Wed Mar  8 03:11:29 2023, max compression
```

## Comparing `negmas-0.9.7.tar` & `negmas-0.9.8.tar`

### file list

```diff
@@ -1,296 +1,303 @@
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.596655 negmas-0.9.7/
--rwxr-xr-x   0 yasser     (501) staff       (20)      187 2022-04-11 08:04:50.000000 negmas-0.9.7/AUTHORS.rst
--rwxr-xr-x   0 yasser     (501) staff       (20)     3481 2022-04-11 08:04:50.000000 negmas-0.9.7/CONTRIBUTING.rst
--rwxr-xr-x   0 yasser     (501) staff       (20)    53696 2022-12-21 10:59:06.000000 negmas-0.9.7/HISTORY.rst
--rwxr-xr-x   0 yasser     (501) staff       (20)      737 2022-04-11 08:04:50.000000 negmas-0.9.7/LICENSE
--rwxr-xr-x   0 yasser     (501) staff       (20)      168 2022-04-11 08:04:50.000000 negmas-0.9.7/MANIFEST.in
--rw-r--r--   0 yasser     (501) staff       (20)    63041 2023-01-24 11:32:15.596800 negmas-0.9.7/PKG-INFO
--rwxr-xr-x   0 yasser     (501) staff       (20)     8491 2022-12-21 08:58:42.000000 negmas-0.9.7/README.rst
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.443115 negmas-0.9.7/negmas/
--rwxr-xr-x   0 yasser     (501) staff       (20)     1096 2023-01-24 11:28:57.000000 negmas-0.9.7/negmas/__init__.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    11385 2022-04-19 04:49:27.000000 negmas-0.9.7/negmas/checkpoints.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    15219 2022-12-27 01:18:45.000000 negmas-0.9.7/negmas/common.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.448863 negmas-0.9.7/negmas/concurrent/
--rw-r--r--   0 yasser     (501) staff       (20)      175 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/concurrent/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)    20245 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/concurrent/chain.py
--rw-r--r--   0 yasser     (501) staff       (20)     2122 2023-01-15 02:27:21.000000 negmas-0.9.7/negmas/config.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.453593 negmas-0.9.7/negmas/elicitation/
--rw-r--r--   0 yasser     (501) staff       (20)      677 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/elicitation/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)    22965 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/elicitation/base.py
--rw-r--r--   0 yasser     (501) staff       (20)     1703 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/elicitation/baseline.py
--rw-r--r--   0 yasser     (501) staff       (20)     1459 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/elicitation/common.py
--rw-r--r--   0 yasser     (501) staff       (20)     2902 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/elicitation/expectors.py
--rw-r--r--   0 yasser     (501) staff       (20)    32244 2023-01-09 20:01:02.000000 negmas-0.9.7/negmas/elicitation/mechanism.py
--rw-r--r--   0 yasser     (501) staff       (20)    26073 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/elicitation/pandora.py
--rw-r--r--   0 yasser     (501) staff       (20)    12869 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/elicitation/queries.py
--rw-r--r--   0 yasser     (501) staff       (20)    12244 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/elicitation/strategy.py
--rw-r--r--   0 yasser     (501) staff       (20)     5024 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/elicitation/user.py
--rw-r--r--   0 yasser     (501) staff       (20)    41830 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/elicitation/voi.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     7775 2022-04-19 04:49:48.000000 negmas-0.9.7/negmas/events.py
--rw-r--r--   0 yasser     (501) staff       (20)       74 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/exceptions.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.454017 negmas-0.9.7/negmas/external/
--rwxr-xr-x   0 yasser     (501) staff       (20)       35 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/external/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     4317 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/ga.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.455532 negmas-0.9.7/negmas/gb/
--rw-r--r--   0 yasser     (501) staff       (20)      525 2023-01-15 01:38:27.000000 negmas-0.9.7/negmas/gb/__init__.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.456471 negmas-0.9.7/negmas/gb/adapters/
--rw-r--r--   0 yasser     (501) staff       (20)       42 2022-12-26 07:53:13.000000 negmas-0.9.7/negmas/gb/adapters/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)    13085 2023-01-20 22:49:09.000000 negmas-0.9.7/negmas/gb/adapters/tau.py
--rw-r--r--   0 yasser     (501) staff       (20)     2020 2023-01-04 10:58:42.000000 negmas-0.9.7/negmas/gb/common.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.460015 negmas-0.9.7/negmas/gb/components/
--rw-r--r--   0 yasser     (501) staff       (20)      408 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/components/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)    19549 2023-01-09 06:46:59.000000 negmas-0.9.7/negmas/gb/components/acceptance.py
--rw-r--r--   0 yasser     (501) staff       (20)     7491 2023-01-04 11:14:07.000000 negmas-0.9.7/negmas/gb/components/base.py
--rw-r--r--   0 yasser     (501) staff       (20)     3154 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/components/concession.py
--rw-r--r--   0 yasser     (501) staff       (20)    10016 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/components/inverter.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.460591 negmas-0.9.7/negmas/gb/components/models/
--rw-r--r--   0 yasser     (501) staff       (20)       44 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/components/models/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     2782 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/components/models/ufun.py
--rw-r--r--   0 yasser     (501) staff       (20)    17447 2023-01-04 11:07:54.000000 negmas-0.9.7/negmas/gb/components/offering.py
--rw-r--r--   0 yasser     (501) staff       (20)    13321 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/components/selectors.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.462184 negmas-0.9.7/negmas/gb/constraints/
--rw-r--r--   0 yasser     (501) staff       (20)      149 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/constraints/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     2142 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/constraints/base.py
--rw-r--r--   0 yasser     (501) staff       (20)      875 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/constraints/rfo.py
--rw-r--r--   0 yasser     (501) staff       (20)      640 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/constraints/rlo.py
--rw-r--r--   0 yasser     (501) staff       (20)      472 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/constraints/unique.py
--rw-r--r--   0 yasser     (501) staff       (20)       13 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/controllers.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.463251 negmas-0.9.7/negmas/gb/evaluators/
--rw-r--r--   0 yasser     (501) staff       (20)      110 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/evaluators/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     3804 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/evaluators/base.py
--rw-r--r--   0 yasser     (501) staff       (20)      810 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/evaluators/gao.py
--rw-r--r--   0 yasser     (501) staff       (20)     3302 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/evaluators/tau.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.464406 negmas-0.9.7/negmas/gb/mechanisms/
--rw-r--r--   0 yasser     (501) staff       (20)       91 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/mechanisms/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)    16113 2023-01-14 06:01:45.000000 negmas-0.9.7/negmas/gb/mechanisms/base.py
--rw-r--r--   0 yasser     (501) staff       (20)     1728 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/mechanisms/mechanisms.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.470258 negmas-0.9.7/negmas/gb/negotiators/
--rw-r--r--   0 yasser     (501) staff       (20)      546 2022-12-23 07:59:54.000000 negmas-0.9.7/negmas/gb/negotiators/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     9314 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/base.py
--rw-r--r--   0 yasser     (501) staff       (20)     2078 2022-12-24 12:15:06.000000 negmas-0.9.7/negmas/gb/negotiators/cab.py
--rw-r--r--   0 yasser     (501) staff       (20)     6262 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/limited.py
--rw-r--r--   0 yasser     (501) staff       (20)      826 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/micro.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.471934 negmas-0.9.7/negmas/gb/negotiators/modular/
--rw-r--r--   0 yasser     (501) staff       (20)      123 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/modular/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     2496 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/modular/boa.py
--rw-r--r--   0 yasser     (501) staff       (20)     2967 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/modular/mapneg.py
--rw-r--r--   0 yasser     (501) staff       (20)     4049 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/modular/modular.py
--rw-r--r--   0 yasser     (501) staff       (20)      759 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/nice.py
--rw-r--r--   0 yasser     (501) staff       (20)     1158 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/randneg.py
--rw-r--r--   0 yasser     (501) staff       (20)    16137 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/timebased.py
--rw-r--r--   0 yasser     (501) staff       (20)     2954 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/titfortat.py
--rw-r--r--   0 yasser     (501) staff       (20)     2627 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/gb/negotiators/tough.py
--rw-r--r--   0 yasser     (501) staff       (20)     3871 2023-01-04 10:31:54.000000 negmas-0.9.7/negmas/gb/negotiators/utilbased.py
--rw-r--r--   0 yasser     (501) staff       (20)     2017 2022-12-24 12:14:50.000000 negmas-0.9.7/negmas/gb/negotiators/war.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     6841 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/generics.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.475240 negmas-0.9.7/negmas/genius/
--rw-r--r--   0 yasser     (501) staff       (20)      403 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/genius/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)    23038 2022-12-21 08:59:10.000000 negmas-0.9.7/negmas/genius/bridge.py
--rw-r--r--   0 yasser     (501) staff       (20)      427 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/genius/common.py
--rw-r--r--   0 yasser     (501) staff       (20)    31150 2022-12-29 05:55:52.000000 negmas-0.9.7/negmas/genius/ginfo.py
--rw-r--r--   0 yasser     (501) staff       (20)    14301 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/genius/gnegotiators.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    27577 2022-12-21 09:01:20.000000 negmas-0.9.7/negmas/genius/negotiator.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.481729 negmas-0.9.7/negmas/helpers/
--rw-r--r--   0 yasser     (501) staff       (20)      518 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/helpers/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)      124 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/helpers/generics.py
--rw-r--r--   0 yasser     (501) staff       (20)    18790 2023-01-18 00:31:05.000000 negmas-0.9.7/negmas/helpers/inout.py
--rw-r--r--   0 yasser     (501) staff       (20)     4419 2022-12-21 08:59:10.000000 negmas-0.9.7/negmas/helpers/logging.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     2703 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/helpers/misc.py
--rw-r--r--   0 yasser     (501) staff       (20)      435 2022-12-30 05:13:18.000000 negmas-0.9.7/negmas/helpers/numba_checks.py
--rw-r--r--   0 yasser     (501) staff       (20)     8399 2022-04-19 04:49:27.000000 negmas-0.9.7/negmas/helpers/numeric.py
--rw-r--r--   0 yasser     (501) staff       (20)    13736 2022-12-29 05:00:06.000000 negmas-0.9.7/negmas/helpers/prob.py
--rw-r--r--   0 yasser     (501) staff       (20)    10856 2023-01-15 01:25:24.000000 negmas-0.9.7/negmas/helpers/strings.py
--rw-r--r--   0 yasser     (501) staff       (20)     2375 2022-12-25 14:19:26.000000 negmas-0.9.7/negmas/helpers/timeout.py
--rw-r--r--   0 yasser     (501) staff       (20)     7405 2022-04-19 04:49:48.000000 negmas-0.9.7/negmas/helpers/types.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    25328 2023-01-11 07:53:55.000000 negmas-0.9.7/negmas/inout.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    46173 2023-01-11 07:53:56.000000 negmas-0.9.7/negmas/mechanisms.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.484182 negmas-0.9.7/negmas/models/
--rw-r--r--   0 yasser     (501) staff       (20)       74 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/models/__init__.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    12413 2022-04-19 04:49:48.000000 negmas-0.9.7/negmas/models/acceptance.py
--rw-r--r--   0 yasser     (501) staff       (20)     1875 2022-12-21 10:03:52.000000 negmas-0.9.7/negmas/models/future.py
--rw-r--r--   0 yasser     (501) staff       (20)       83 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/models/preferences.py
--rw-r--r--   0 yasser     (501) staff       (20)       85 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/models/strategy.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     4058 2022-12-21 08:59:10.000000 negmas-0.9.7/negmas/mt.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.487956 negmas-0.9.7/negmas/negotiators/
--rw-r--r--   0 yasser     (501) staff       (20)      487 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/negotiators/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)      238 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/negotiators/common.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.488975 negmas-0.9.7/negmas/negotiators/components/
--rw-r--r--   0 yasser     (501) staff       (20)       54 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/negotiators/components/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     2549 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/negotiators/components/component.py
--rw-r--r--   0 yasser     (501) staff       (20)     1516 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/negotiators/controlled.py
--rw-r--r--   0 yasser     (501) staff       (20)    18313 2022-05-04 03:13:19.000000 negmas-0.9.7/negmas/negotiators/controller.py
--rw-r--r--   0 yasser     (501) staff       (20)     4239 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/negotiators/helpers.py
--rw-r--r--   0 yasser     (501) staff       (20)     4867 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/negotiators/modular.py
--rw-r--r--   0 yasser     (501) staff       (20)    13825 2022-12-21 08:59:10.000000 negmas-0.9.7/negmas/negotiators/negotiator.py
--rw-r--r--   0 yasser     (501) staff       (20)    15477 2022-04-19 04:49:49.000000 negmas-0.9.7/negmas/negotiators/simple.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.495122 negmas-0.9.7/negmas/outcomes/
--rw-r--r--   0 yasser     (501) staff       (20)     1733 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)    18654 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/base_issue.py
--rw-r--r--   0 yasser     (501) staff       (20)     2212 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/callable_issue.py
--rw-r--r--   0 yasser     (501) staff       (20)      850 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/cardinal_issue.py
--rw-r--r--   0 yasser     (501) staff       (20)     1807 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/categorical_issue.py
--rw-r--r--   0 yasser     (501) staff       (20)     3931 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/common.py
--rw-r--r--   0 yasser     (501) staff       (20)     4347 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/contiguous_issue.py
--rw-r--r--   0 yasser     (501) staff       (20)     3879 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/continuous_issue.py
--rw-r--r--   0 yasser     (501) staff       (20)     2405 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/infinite.py
--rw-r--r--   0 yasser     (501) staff       (20)    29052 2023-01-09 20:07:22.000000 negmas-0.9.7/negmas/outcomes/issue_ops.py
--rw-r--r--   0 yasser     (501) staff       (20)     3970 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/ordinal_issue.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    17143 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/outcome_ops.py
--rw-r--r--   0 yasser     (501) staff       (20)    21705 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/outcomes/outcome_space.py
--rw-r--r--   0 yasser     (501) staff       (20)     5855 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/protocols.py
--rw-r--r--   0 yasser     (501) staff       (20)      695 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/outcomes/range_issue.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.495743 negmas-0.9.7/negmas/plots/
--rw-r--r--   0 yasser     (501) staff       (20)       19 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/plots/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)    27450 2023-01-20 06:46:36.000000 negmas-0.9.7/negmas/plots/util.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.502804 negmas-0.9.7/negmas/preferences/
--rw-r--r--   0 yasser     (501) staff       (20)     1772 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/__init__.py
--rwxr-xr-x   0 yasser     (501) staff       (20)      552 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/base.py
--rw-r--r--   0 yasser     (501) staff       (20)    38580 2023-01-11 07:53:55.000000 negmas-0.9.7/negmas/preferences/base_ufun.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     7395 2022-04-19 04:49:27.000000 negmas-0.9.7/negmas/preferences/complex.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.506779 negmas-0.9.7/negmas/preferences/crisp/
--rw-r--r--   0 yasser     (501) staff       (20)      302 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/crisp/__init__.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     2522 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/crisp/const.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    34726 2023-01-05 02:43:25.000000 negmas-0.9.7/negmas/preferences/crisp/linear.py
--rw-r--r--   0 yasser     (501) staff       (20)     7606 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/preferences/crisp/mapping.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    17922 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/crisp/nonlinear.py
--rw-r--r--   0 yasser     (501) staff       (20)      945 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/crisp/random_ufun.py
--rw-r--r--   0 yasser     (501) staff       (20)     3401 2022-04-19 04:49:27.000000 negmas-0.9.7/negmas/preferences/crisp/rankonly_ufun.py
--rw-r--r--   0 yasser     (501) staff       (20)    10192 2023-01-11 07:53:56.000000 negmas-0.9.7/negmas/preferences/crisp_ufun.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    11786 2022-12-28 12:57:45.000000 negmas-0.9.7/negmas/preferences/discounted.py
--rw-r--r--   0 yasser     (501) staff       (20)    15489 2023-01-04 10:43:08.000000 negmas-0.9.7/negmas/preferences/inv_ufun.py
--rw-r--r--   0 yasser     (501) staff       (20)     3441 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/mixins.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    50155 2023-01-11 07:53:56.000000 negmas-0.9.7/negmas/preferences/ops.py
--rw-r--r--   0 yasser     (501) staff       (20)     6441 2022-04-19 04:49:27.000000 negmas-0.9.7/negmas/preferences/preferences.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.508941 negmas-0.9.7/negmas/preferences/prob/
--rw-r--r--   0 yasser     (501) staff       (20)      192 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/prob/__init__.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     9740 2022-04-19 04:49:27.000000 negmas-0.9.7/negmas/preferences/prob/independent.py
--rw-r--r--   0 yasser     (501) staff       (20)     1810 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/prob/locscale.py
--rw-r--r--   0 yasser     (501) staff       (20)     3997 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/prob/mapping.py
--rw-r--r--   0 yasser     (501) staff       (20)     1577 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/prob/random_ufun.py
--rw-r--r--   0 yasser     (501) staff       (20)     8949 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/preferences/prob_ufun.py
--rw-r--r--   0 yasser     (501) staff       (20)    22929 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/preferences/protocols.py
--rw-r--r--   0 yasser     (501) staff       (20)    25973 2022-12-28 09:30:59.000000 negmas-0.9.7/negmas/preferences/value_fun.py
--rw-r--r--   0 yasser     (501) staff       (20)     2053 2023-01-05 02:43:24.000000 negmas-0.9.7/negmas/protocols.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.511445 negmas-0.9.7/negmas/sao/
--rw-r--r--   0 yasser     (501) staff       (20)      407 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/__init__.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     1808 2022-12-27 01:12:58.000000 negmas-0.9.7/negmas/sao/common.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.516801 negmas-0.9.7/negmas/sao/components/
--rw-r--r--   0 yasser     (501) staff       (20)      408 2022-04-11 08:59:36.000000 negmas-0.9.7/negmas/sao/components/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)      152 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/components/acceptance.py
--rw-r--r--   0 yasser     (501) staff       (20)      140 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/components/base.py
--rw-r--r--   0 yasser     (501) staff       (20)      152 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/components/concession.py
--rw-r--r--   0 yasser     (501) staff       (20)      148 2022-12-21 09:08:16.000000 negmas-0.9.7/negmas/sao/components/inverter.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.518074 negmas-0.9.7/negmas/sao/components/models/
--rw-r--r--   0 yasser     (501) staff       (20)       44 2022-04-11 08:59:36.000000 negmas-0.9.7/negmas/sao/components/models/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     2782 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/components/models/ufun.py
--rw-r--r--   0 yasser     (501) staff       (20)      148 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/components/offering.py
--rw-r--r--   0 yasser     (501) staff       (20)      150 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/components/selectors.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    33940 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/controllers.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    35635 2023-01-24 10:49:45.000000 negmas-0.9.7/negmas/sao/mechanism.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.532980 negmas-0.9.7/negmas/sao/negotiators/
--rw-r--r--   0 yasser     (501) staff       (20)      590 2022-12-23 12:45:48.000000 negmas-0.9.7/negmas/sao/negotiators/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     8861 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/base.py
--rw-r--r--   0 yasser     (501) staff       (20)      140 2022-12-23 12:45:48.000000 negmas-0.9.7/negmas/sao/negotiators/cab.py
--rw-r--r--   0 yasser     (501) staff       (20)     2936 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/controlled.py
--rw-r--r--   0 yasser     (501) staff       (20)      148 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/limited.py
--rw-r--r--   0 yasser     (501) staff       (20)      144 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/micro.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.547805 negmas-0.9.7/negmas/sao/negotiators/modular/
--rw-r--r--   0 yasser     (501) staff       (20)      123 2022-04-11 08:59:36.000000 negmas-0.9.7/negmas/sao/negotiators/modular/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)      156 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/modular/boa.py
--rw-r--r--   0 yasser     (501) staff       (20)      162 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/modular/mapneg.py
--rw-r--r--   0 yasser     (501) staff       (20)      164 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/modular/modular.py
--rw-r--r--   0 yasser     (501) staff       (20)      142 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/nice.py
--rw-r--r--   0 yasser     (501) staff       (20)      148 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/randneg.py
--rw-r--r--   0 yasser     (501) staff       (20)      152 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/timebased.py
--rw-r--r--   0 yasser     (501) staff       (20)      152 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/titfortat.py
--rw-r--r--   0 yasser     (501) staff       (20)      144 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/tough.py
--rw-r--r--   0 yasser     (501) staff       (20)      152 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/sao/negotiators/utilbased.py
--rw-r--r--   0 yasser     (501) staff       (20)      140 2022-12-23 12:45:09.000000 negmas-0.9.7/negmas/sao/negotiators/war.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.550243 negmas-0.9.7/negmas/scripts/
--rwxr-xr-x   0 yasser     (501) staff       (20)       86 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/scripts/__init__.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    26479 2022-12-21 10:48:17.000000 negmas-0.9.7/negmas/scripts/app.py
--rw-r--r--   0 yasser     (501) staff       (20)    12154 2023-01-24 11:00:51.000000 negmas-0.9.7/negmas/scripts/negotiate.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.550622 negmas-0.9.7/negmas/scripts/vendor/
--rw-r--r--   0 yasser     (501) staff       (20)       35 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/scripts/vendor/__init__.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.551677 negmas-0.9.7/negmas/scripts/vendor/quick/
--rw-r--r--   0 yasser     (501) staff       (20)       35 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/scripts/vendor/quick/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)    29399 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/scripts/vendor/quick/quick.py
--rw-r--r--   0 yasser     (501) staff       (20)    11774 2022-12-21 08:59:10.000000 negmas-0.9.7/negmas/serialization.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.566859 negmas-0.9.7/negmas/situated/
--rw-r--r--   0 yasser     (501) staff       (20)     5304 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/situated/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)      307 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/situated/action.py
--rw-r--r--   0 yasser     (501) staff       (20)     2751 2022-05-18 01:56:25.000000 negmas-0.9.7/negmas/situated/adapter.py
--rw-r--r--   0 yasser     (501) staff       (20)    21625 2022-04-19 05:08:57.000000 negmas-0.9.7/negmas/situated/agent.py
--rw-r--r--   0 yasser     (501) staff       (20)    18172 2022-04-19 04:49:27.000000 negmas-0.9.7/negmas/situated/awi.py
--rw-r--r--   0 yasser     (501) staff       (20)     2023 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/situated/breaches.py
--rw-r--r--   0 yasser     (501) staff       (20)     7241 2022-04-19 04:49:27.000000 negmas-0.9.7/negmas/situated/bulletinboard.py
--rw-r--r--   0 yasser     (501) staff       (20)     3021 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/situated/common.py
--rw-r--r--   0 yasser     (501) staff       (20)     2309 2022-12-21 08:59:10.000000 negmas-0.9.7/negmas/situated/contract.py
--rw-r--r--   0 yasser     (501) staff       (20)     1932 2022-05-18 01:56:25.000000 negmas-0.9.7/negmas/situated/entity.py
--rw-r--r--   0 yasser     (501) staff       (20)     1678 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/situated/helpers.py
--rw-r--r--   0 yasser     (501) staff       (20)    10243 2022-04-19 04:49:27.000000 negmas-0.9.7/negmas/situated/mechanismfactory.py
--rw-r--r--   0 yasser     (501) staff       (20)     4882 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/situated/mixins.py
--rw-r--r--   0 yasser     (501) staff       (20)      868 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/situated/monitors.py
--rw-r--r--   0 yasser     (501) staff       (20)    19543 2022-12-21 08:59:10.000000 negmas-0.9.7/negmas/situated/neg.py
--rw-r--r--   0 yasser     (501) staff       (20)     5337 2022-04-19 04:49:27.000000 negmas-0.9.7/negmas/situated/save.py
--rw-r--r--   0 yasser     (501) staff       (20)     1034 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/situated/simple.py
--rw-r--r--   0 yasser     (501) staff       (20)   129718 2022-12-21 08:59:10.000000 negmas-0.9.7/negmas/situated/world.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    12940 2023-01-09 20:01:02.000000 negmas-0.9.7/negmas/st.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.578714 negmas-0.9.7/negmas/tests/
--rwxr-xr-x   0 yasser     (501) staff       (20)       80 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/__init__.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     1382 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/fixtures.py
--rwxr-xr-x   0 yasser     (501) staff       (20)      111 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/test_basic_agent.py
--rw-r--r--   0 yasser     (501) staff       (20)      264 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/test_cli.py
--rw-r--r--   0 yasser     (501) staff       (20)      718 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/test_ga.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    24387 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/tests/test_genius.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     5475 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/test_helpers.py
--rwxr-xr-x   0 yasser     (501) staff       (20)      897 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/test_inout.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     2446 2022-04-14 11:18:42.000000 negmas-0.9.7/negmas/tests/test_integration.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     3176 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/test_issue.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    13727 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/test_negotiators.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     1709 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/test_outcomes.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    30205 2023-01-11 07:53:56.000000 negmas-0.9.7/negmas/tests/test_preferences.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    10886 2022-12-21 08:58:42.000000 negmas-0.9.7/negmas/tests/test_protocols.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    15994 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/test_situated.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     1548 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tests/test_st.py
--rw-r--r--   0 yasser     (501) staff       (20)    22751 2023-01-09 21:25:38.000000 negmas-0.9.7/negmas/tests/test_tau.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.581791 negmas-0.9.7/negmas/tournaments/
--rw-r--r--   0 yasser     (501) staff       (20)      208 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tournaments/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)    18027 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/tournaments/neg.py
--rwxr-xr-x   0 yasser     (501) staff       (20)   117154 2022-12-21 08:59:10.000000 negmas-0.9.7/negmas/tournaments/tournaments.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.584205 negmas-0.9.7/negmas/types/
--rw-r--r--   0 yasser     (501) staff       (20)      254 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/types/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)     9679 2022-12-21 08:59:10.000000 negmas-0.9.7/negmas/types/named.py
--rw-r--r--   0 yasser     (501) staff       (20)     7492 2022-12-21 08:59:10.000000 negmas-0.9.7/negmas/types/rational.py
--rw-r--r--   0 yasser     (501) staff       (20)      473 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/types/runnable.py
--rw-r--r--   0 yasser     (501) staff       (20)      141 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/utilities.py
--rw-r--r--   0 yasser     (501) staff       (20)     2399 2022-04-11 08:04:50.000000 negmas-0.9.7/negmas/warnings.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.448135 negmas-0.9.7/negmas.egg-info/
--rw-r--r--   0 yasser     (501) staff       (20)    63041 2023-01-24 11:32:14.000000 negmas-0.9.7/negmas.egg-info/PKG-INFO
--rw-r--r--   0 yasser     (501) staff       (20)     7399 2023-01-24 11:32:14.000000 negmas-0.9.7/negmas.egg-info/SOURCES.txt
--rw-r--r--   0 yasser     (501) staff       (20)        1 2023-01-24 11:32:14.000000 negmas-0.9.7/negmas.egg-info/dependency_links.txt
--rw-r--r--   0 yasser     (501) staff       (20)      118 2023-01-24 11:32:14.000000 negmas-0.9.7/negmas.egg-info/entry_points.txt
--rw-r--r--   0 yasser     (501) staff       (20)      446 2023-01-24 11:32:14.000000 negmas-0.9.7/negmas.egg-info/requires.txt
--rw-r--r--   0 yasser     (501) staff       (20)       13 2023-01-24 11:32:14.000000 negmas-0.9.7/negmas.egg-info/top_level.txt
--rw-r--r--   0 yasser     (501) staff       (20)      100 2022-04-11 08:04:50.000000 negmas-0.9.7/pyproject.toml
--rw-r--r--   0 yasser     (501) staff       (20)     2270 2023-01-24 11:32:15.597578 negmas-0.9.7/setup.cfg
--rwxr-xr-x   0 yasser     (501) staff       (20)       69 2022-04-11 08:04:50.000000 negmas-0.9.7/setup.py
-drwxr-xr-x   0 yasser     (501) staff       (20)        0 2023-01-24 11:32:15.596314 negmas-0.9.7/tests/
--rw-r--r--   0 yasser     (501) staff       (20)        0 2022-04-11 08:04:50.000000 negmas-0.9.7/tests/__init__.py
--rw-r--r--   0 yasser     (501) staff       (20)      799 2022-04-20 00:46:25.000000 negmas-0.9.7/tests/switches.py
--rw-r--r--   0 yasser     (501) staff       (20)     5311 2022-04-20 00:46:25.000000 negmas-0.9.7/tests/test_base_issue.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     8660 2022-04-20 00:46:25.000000 negmas-0.9.7/tests/test_checkpoints.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     2370 2022-04-20 00:46:25.000000 negmas-0.9.7/tests/test_common.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    14531 2022-04-20 00:46:25.000000 negmas-0.9.7/tests/test_genius.py
--rw-r--r--   0 yasser     (501) staff       (20)     1936 2022-04-20 00:46:25.000000 negmas-0.9.7/tests/test_genius_bridge.py
--rw-r--r--   0 yasser     (501) staff       (20)    17512 2023-01-04 11:40:32.000000 negmas-0.9.7/tests/test_genius_negotiators_all.py
--rwxr-xr-x   0 yasser     (501) staff       (20)     9123 2022-12-28 12:50:08.000000 negmas-0.9.7/tests/test_inout.py
--rw-r--r--   0 yasser     (501) staff       (20)     1596 2023-01-04 10:55:46.000000 negmas-0.9.7/tests/test_inverter.py
--rw-r--r--   0 yasser     (501) staff       (20)      852 2022-04-20 00:46:25.000000 negmas-0.9.7/tests/test_jupyter.py
--rw-r--r--   0 yasser     (501) staff       (20)     3352 2022-04-20 00:45:07.000000 negmas-0.9.7/tests/test_neg_tournaments.py
--rw-r--r--   0 yasser     (501) staff       (20)       35 2022-04-20 00:45:07.000000 negmas-0.9.7/tests/test_outcome_space.py
--rw-r--r--   0 yasser     (501) staff       (20)      469 2022-04-20 00:46:25.000000 negmas-0.9.7/tests/test_prob_ufun.py
--rw-r--r--   0 yasser     (501) staff       (20)     1842 2022-12-21 08:58:42.000000 negmas-0.9.7/tests/test_sao.py
--rw-r--r--   0 yasser     (501) staff       (20)     3101 2022-12-21 08:58:42.000000 negmas-0.9.7/tests/test_sao_negotiators.py
--rwxr-xr-x   0 yasser     (501) staff       (20)    53195 2022-12-21 08:58:42.000000 negmas-0.9.7/tests/test_sao_slow.py
--rw-r--r--   0 yasser     (501) staff       (20)     9677 2022-12-21 08:58:42.000000 negmas-0.9.7/tests/test_trips_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.642977 negmas-0.9.8/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      187 2023-03-08 03:11:10.000000 negmas-0.9.8/AUTHORS.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3481 2023-03-08 03:11:10.000000 negmas-0.9.8/CONTRIBUTING.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54587 2023-03-08 03:11:10.000000 negmas-0.9.8/HISTORY.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      737 2023-03-08 03:11:10.000000 negmas-0.9.8/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      168 2023-03-08 03:11:10.000000 negmas-0.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    63855 2023-03-08 03:11:29.642977 negmas-0.9.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8491 2023-03-08 03:11:10.000000 negmas-0.9.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.602977 negmas-0.9.8/negmas/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1096 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11385 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15218 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.606977 negmas-0.9.8/negmas/concurrent/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/concurrent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20224 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/concurrent/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.606977 negmas-0.9.8/negmas/elicitation/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/elicitation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22965 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/elicitation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/elicitation/baseline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/elicitation/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/elicitation/expectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32244 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/elicitation/mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26073 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/elicitation/pandora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/elicitation/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/elicitation/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/elicitation/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41830 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/elicitation/voi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7775 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.606977 negmas-0.9.8/negmas/external/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       35 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/ga.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.606977 negmas-0.9.8/negmas/gb/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.606977 negmas-0.9.8/negmas/gb/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/adapters/tau.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.610977 negmas-0.9.8/negmas/gb/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19549 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/components/acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7492 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/components/concession.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/components/inverter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.610977 negmas-0.9.8/negmas/gb/components/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/components/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/components/models/ufun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18124 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/components/offering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13321 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/components/selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.610977 negmas-0.9.8/negmas/gb/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/constraints/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/constraints/rfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/constraints/rlo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/constraints/unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/controllers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.610977 negmas-0.9.8/negmas/gb/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/evaluators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/evaluators/gao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/evaluators/tau.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.610977 negmas-0.9.8/negmas/gb/mechanisms/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/mechanisms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16110 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/mechanisms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/mechanisms/mechanisms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.614977 negmas-0.9.8/negmas/gb/negotiators/
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/cab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/limited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/micro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.614977 negmas-0.9.8/negmas/gb/negotiators/modular/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/modular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/modular/boa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/modular/mapneg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/modular/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/nice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/randneg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16282 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/timebased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/titfortat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/tough.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/utilbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/gb/negotiators/war.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6841 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/generics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.614977 negmas-0.9.8/negmas/genius/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/genius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/genius/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/genius/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33099 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/genius/ginfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14301 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/genius/gnegotiators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28734 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/genius/negotiator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.618977 negmas-0.9.8/negmas/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/helpers/generics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18790 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/helpers/inout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/helpers/logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/helpers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/helpers/numba_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/helpers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/helpers/prob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/helpers/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/helpers/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/helpers/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25329 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/inout.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    46223 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/mechanisms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.618977 negmas-0.9.8/negmas/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12413 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/models/acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/models/future.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/models/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/models/strategy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4055 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/mt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.618977 negmas-0.9.8/negmas/negotiators/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/negotiators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/negotiators/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.618977 negmas-0.9.8/negmas/negotiators/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/negotiators/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/negotiators/components/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/negotiators/controlled.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18313 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/negotiators/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/negotiators/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/negotiators/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13825 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/negotiators/negotiator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/negotiators/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.622977 negmas-0.9.8/negmas/outcomes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18654 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/base_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/callable_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/cardinal_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/categorical_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/contiguous_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/continuous_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/infinite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29114 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/issue_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/ordinal_issue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17169 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/outcome_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21706 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/outcome_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/outcomes/range_issue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.622977 negmas-0.9.8/negmas/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27450 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/plots/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.622977 negmas-0.9.8/negmas/preferences/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      552 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39010 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/base_ufun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7395 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/complex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.626977 negmas-0.9.8/negmas/preferences/crisp/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/crisp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2522 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/crisp/const.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34726 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/crisp/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/crisp/mapping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17922 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/crisp/nonlinear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/crisp/random_ufun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/crisp/rankonly_ufun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10210 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/crisp_ufun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11786 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/discounted.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15489 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/inv_ufun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/mixins.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50336 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.626977 negmas-0.9.8/negmas/preferences/prob/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/prob/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9740 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/prob/independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/prob/locscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/prob/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/prob/random_ufun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/prob_ufun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22929 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25974 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/preferences/value_fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.626977 negmas-0.9.8/negmas/sao/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1765 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.626977 negmas-0.9.8/negmas/sao/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/components/acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/components/concession.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/components/inverter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.626977 negmas-0.9.8/negmas/sao/components/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/components/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/components/models/ufun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/components/offering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/components/selectors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33996 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/controllers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28704 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/mechanism.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.630977 negmas-0.9.8/negmas/sao/negotiators/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/cab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/controlled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/limited.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/micro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.630977 negmas-0.9.8/negmas/sao/negotiators/modular/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/modular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/modular/boa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/modular/mapneg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/modular/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/nice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/randneg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/timebased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/titfortat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/tough.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/utilbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/sao/negotiators/war.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.630977 negmas-0.9.8/negmas/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26479 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/scripts/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/scripts/negotiate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.630977 negmas-0.9.8/negmas/scripts/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/scripts/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.630977 negmas-0.9.8/negmas/scripts/vendor/quick/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/scripts/vendor/quick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29399 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/scripts/vendor/quick/quick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.634977 negmas-0.9.8/negmas/situated/
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21625 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/awi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/breaches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/bulletinboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/mechanismfactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19543 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/neg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129666 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/situated/world.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12933 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/st.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.638977 negmas-0.9.8/negmas/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1382 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/fixtures.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      111 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_basic_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_ga.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24387 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_genius.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5475 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_inout.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2446 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_integration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3176 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_issue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13598 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_negotiators.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1709 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_outcomes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10859 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_protocols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15995 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_situated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1548 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tests/test_st.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.638977 negmas-0.9.8/negmas/tournaments/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tournaments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18139 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tournaments/neg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   117188 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/tournaments/tournaments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.638977 negmas-0.9.8/negmas/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/types/rational.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/types/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-03-08 03:11:10.000000 negmas-0.9.8/negmas/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.606977 negmas-0.9.8/negmas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    63855 2023-03-08 03:11:29.000000 negmas-0.9.8/negmas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-03-08 03:11:29.000000 negmas-0.9.8/negmas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 03:11:29.000000 negmas-0.9.8/negmas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-08 03:11:29.000000 negmas-0.9.8/negmas.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-08 03:11:29.000000 negmas-0.9.8/negmas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-08 03:11:29.000000 negmas-0.9.8/negmas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-08 03:11:10.000000 negmas-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-03-08 03:11:29.642977 negmas-0.9.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       69 2023-03-08 03:11:10.000000 negmas-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.638977 negmas-0.9.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.638977 negmas-0.9.8/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/test_base_issue.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2370 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/test_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5552 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/test_inout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/test_inverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/test_outcome_space.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30160 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/test_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/test_prob_ufun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/test_sao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/test_sao_negotiators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22757 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/test_tau.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/core/test_trips_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.642977 negmas-0.9.8/tests/genius/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/genius/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14426 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/genius/test_genius.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/genius/test_genius_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17479 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/genius/test_genius_negotiators_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/genius/test_inout_with_genius.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:29.642977 negmas-0.9.8/tests/optional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/optional/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8596 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/optional/test_checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/optional/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/optional/test_neg_tournaments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51315 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/optional/test_sao_slow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-08 03:11:10.000000 negmas-0.9.8/tests/switches.py
```

### Comparing `negmas-0.9.7/CONTRIBUTING.rst` & `negmas-0.9.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/HISTORY.rst` & `negmas-0.9.8/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,33 @@
 History
 =======
 
+Release 0.9.8
+-------------
+
+* Restructuring tests
+* Using Numba only with python 3.10
+* Always using with when opening files
+* Adding more info about anac results
+* [SAO] Completely removing support for avoid_ultimatum
+* [SAO] Adding fallbacks to respond() calls in SAO to support the API with and
+  without source. The later API will be dropped later.
+* [Preferences] Adding has_ufun to Rational to check if it has a `BaseUtilityFunction`
+  as its preferences.
+* [Genius] More details on errors from genius bridge
+* [Genius] bugfix when starting genius negotitauions with no n-steps (sometims)
+* [CLI] supporting genius negotiators in the negotiate.py cli
+	Pass -n geinus.<agent-name> or genius:<agent-name>
+	The agent-name can be just the full java class name, or a simplified
+	version that is all lower without the word agent and without _
+
+Release 0.9.7
+-------------
+* minor bugfixes
+
 Release 0.9.6
 -------------
 
 * [python] Supporting 3.11 and dropping support for 3.8 and 3.9
 * [test] Adding 3.11 to tests
 * [major] Adding Generalized Bargaining Protocols
 * [buffix] testing saving exceptions in SAO
```

### Comparing `negmas-0.9.7/LICENSE` & `negmas-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/PKG-INFO` & `negmas-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: negmas
-Version: 0.9.7
+Version: 0.9.8
 Summary: NEGotiations Managed by Agent Simulations
 Home-page: https://github.com/yasserfarouk/negmas
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Keywords: negotiation,mas,multi-agent,simulation,AI
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
-Provides-Extra: elicitation
 Provides-Extra: visualization
 Provides-Extra: gui
 Provides-Extra: dask
 Provides-Extra: numba
 License-File: LICENSE
 License-File: AUTHORS.rst
 
@@ -225,14 +223,37 @@
 
 NegMAS tests use scenarios used in ANAC 2010 to ANAC 2018 competitions obtained from the Genius_ Platform. These domains
 can be found in the tests/data and notebooks/data folders.
 
 History
 =======
 
+Release 0.9.8
+-------------
+
+* Restructuring tests
+* Using Numba only with python 3.10
+* Always using with when opening files
+* Adding more info about anac results
+* [SAO] Completely removing support for avoid_ultimatum
+* [SAO] Adding fallbacks to respond() calls in SAO to support the API with and
+  without source. The later API will be dropped later.
+* [Preferences] Adding has_ufun to Rational to check if it has a `BaseUtilityFunction`
+  as its preferences.
+* [Genius] More details on errors from genius bridge
+* [Genius] bugfix when starting genius negotitauions with no n-steps (sometims)
+* [CLI] supporting genius negotiators in the negotiate.py cli
+	Pass -n geinus.<agent-name> or genius:<agent-name>
+	The agent-name can be just the full java class name, or a simplified
+	version that is all lower without the word agent and without _
+
+Release 0.9.7
+-------------
+* minor bugfixes
+
 Release 0.9.6
 -------------
 
 * [python] Supporting 3.11 and dropping support for 3.8 and 3.9
 * [test] Adding 3.11 to tests
 * [major] Adding Generalized Bargaining Protocols
 * [buffix] testing saving exceptions in SAO
```

### Comparing `negmas-0.9.7/README.rst` & `negmas-0.9.8/README.rst`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/__init__.py` & `negmas-0.9.8/negmas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """A framework for conducting multi-strand multilateral asynchronous negotiations on multiple issues."""
 from __future__ import annotations
 
 __author__ = """Yasser Mohammad"""
 __email__ = "yasserfarouk@gmail.com"
-__version__ = "0.9.7"
+__version__ = "0.9.8"
 
 
 from .config import *
 from .types import *
 from .common import *
 from .inout import *
 from .mechanisms import *
```

### Comparing `negmas-0.9.7/negmas/checkpoints.py` & `negmas-0.9.8/negmas/checkpoints.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/common.py` & `negmas-0.9.8/negmas/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 from __future__ import annotations
 
 from collections import namedtuple
 from enum import Enum, auto, unique
 from typing import TYPE_CHECKING, Any, Iterable, Protocol, Union, runtime_checkable
 
-from attr import asdict, define, field
+from attrs import asdict, define, field
 
 if TYPE_CHECKING:
     from .mechanisms import Mechanism
     from .outcomes import (
         CartesianOutcomeSpace,
         DiscreteOutcomeSpace,
         Issue,
@@ -153,20 +153,20 @@
     The type of change in preferences.
 
     Remarks:
 
         - Returned from `changes` property of `Preferences` to help the owner of the preferences in deciding what to do with the change.
         - Received by the `on_preferences_changed` method of `Rational` entities to inform them about a change in preferences.
         - Note that the `Rational` entity needs to call `changes` explicitly and call its own `on_preferences_changed` to handle changes that happen without assignment to `preferences` of the `Rational` entity.
-        - If the `preferences` of the `Rational` agent are changed through assignmen, its `on_preferences_changed` will be called with the appropriate `PreferencesChange` list.
+        - If the `preferences` of the `Rational` agent are changed through assignment, its `on_preferences_changed` will be called with the appropriate `PreferencesChange` list.
     """
 
     General = auto()
-    Scaled = auto()
-    Shifted = auto()
+    Scale = auto()
+    Shift = auto()
     ReservedValue = auto()
     ReservedOutcome = auto()
     UncertaintyReduced = auto()
     UncertaintyIncreased = auto()
 
 
 @define(frozen=True)
```

### Comparing `negmas-0.9.7/negmas/concurrent/chain.py` & `negmas-0.9.8/negmas/concurrent/chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections import defaultdict, namedtuple
 from dataclasses import dataclass
 
 from ..common import NegotiatorMechanismInterface
-from ..mechanisms import Mechanism, MechanismRoundResult, MechanismState
+from ..mechanisms import Mechanism, MechanismState, MechanismStepResult
 from ..negotiators import Negotiator
 from ..outcomes import Outcome
 from ..preferences import Preferences
 from ..sao import ResponseType
 
 __all__ = [
     "ChainNegotiationsMechanism",
@@ -275,46 +275,45 @@
 
     def _update_next(self) -> None:
         if self.__last_proposal.left:
             self.__next_agent = (self.__last_proposer_index - 1) % len(self.__chain)
         else:
             self.__next_agent = (self.__last_proposer_index + 1) % len(self.__chain)
 
-    def __call__(self, state) -> MechanismRoundResult:
-
+    def __call__(self, state) -> MechanismStepResult:
         # check that the chain is complete
         if not all(self.__chain):
             if self.dynamic_entry:
                 state.has_error = True
                 state.error_details = "The chain is not complete"
-                return MechanismRoundResult(state=state)
+                return MechanismStepResult(state=state)
             raise ValueError(
                 "The chain is not complete and dynamic entry is not allowed"
             )
 
         # find the next negotiator to ask
         negotiator = self.__chain[self.__next_agent]
 
         # if this is the first proposal, get it from the left most agent and ask the next one to respond
         if self.__last_proposal is None:
             self.__last_proposal = negotiator.propose(self.state)
             self._update_next()
             assert self.__next_agent == 1
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
 
         # if all agreements are finalized end the mechanism session with success
         agreements = [
             self.__agreements[l]
             for l in range(len(self.__chain))
             if self.__agreements[l] is not None
         ]
 
         if len(agreements) == len(self.__chain) - 1:
             state.agreement = agreements
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
         response = negotiator.respond(
             self.state,
             self.__last_proposal.outcome,
             not self.__last_proposal.left,
             self.__last_proposal.temp,
         )
 
@@ -322,26 +321,26 @@
         if response not in (
             ResponseType.ACCEPT_OFFER,
             ResponseType.REJECT_OFFER,
             ResponseType.END_NEGOTIATION,
         ):
             state.has_error = True
             state.error_details = "An unacceptable response was returned"
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
 
         # If the response is to end the negotiation, end it but only if there are not partial negotiations
         if response == ResponseType.END_NEGOTIATION:
             if len(self.__agreements) > 0:
                 state.has_error = True
                 state.error_details = (
                     "Cannot end a negotiation chain with some agreements"
                 )
-                return MechanismRoundResult(state)
+                return MechanismStepResult(state)
             state.broken = True
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
 
         # if the response is an acceptance then either register an agreement or a temporary agreement depending on
         # proposal
         if response == ResponseType.ACCEPT_OFFER:
             agreement_index = (
                 self.__next_agent
                 if self.__last_proposal.left
@@ -354,21 +353,21 @@
                 assert self.__temp_agreements[agreement_index] is None
                 self.__temp_agreements[agreement_index] = self.__last_proposal.outcome
             self.__last_proposal = self.__chain[
                 self.__last_proposer_index
             ].on_acceptance(self.state, self.__last_proposal)
             self.__last_proposer_index = self.__next_agent
             self._update_next()
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
 
         # now it must be a rejection, ask the one who rejected to propose (in either direction)
         self.__last_proposal = self.__chain[self.__next_agent].propose(self.state)
         self.__last_proposer_index = self.__next_agent
         self._update_next()
-        return MechanismRoundResult()
+        return MechanismStepResult()
 
     def on_confirm(self, level: int, left: bool) -> bool:
         """
         Called by negotiators to confirm their temporary accepted agreements
 
         Args:
             level: The caller level
@@ -463,46 +462,45 @@
             )
         else:
             self.__next_agent_level = (self.__last_proposer_level + 1) % len(
                 self.__chain
             )
         self.__next_agent_number = self.__number[self.__last_proposal.partner]
 
-    def __call__(self, state) -> MechanismRoundResult:
-
+    def __call__(self, state) -> MechanismStepResult:
         # check that the chain is complete
         if not all(len(_) > 0 for _ in self.__chain):
             if self.dynamic_entry:
                 state.has_error = True
                 state.error_details = "The chain is not complete"
-                return MechanismRoundResult(state)
+                return MechanismStepResult(state)
             raise ValueError(
                 "The chain is not complete and dynamic entry is not allowed"
             )
 
         # find the next negotiator to ask
         negotiator = self.__chain[self.__next_agent_level][self.__next_agent_number]
 
         # if this is the first proposal, get it from the left most agent and ask the next one to respond
         if self.__last_proposal is None:
             self.__last_proposal = negotiator.propose(self.state)
             self._update_next()
             assert self.__next_agent_level == 1
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
 
         # if all agreements are finalized end the mechanism session with success
         agreements = [
             self.__agreements[l]
             for l in range(len(self.__chain))
             if self.__agreements[l] is not None
         ]
 
         if len(agreements) == len(self.__chain) - 1:
             state.agreement = agreements
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
         response = negotiator.respond(
             self.state,
             self.__last_proposal.outcome,
             not self.__last_proposal.left,
             self.__last_proposal.temp,
             source=self.__chain[self.__next_agent_level][self.__next_agent_number].id,
         )
@@ -511,26 +509,26 @@
         if response not in (
             ResponseType.ACCEPT_OFFER,
             ResponseType.REJECT_OFFER,
             ResponseType.END_NEGOTIATION,
         ):
             state.has_error = True
             error_details = "An unacceptable response was returned"
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
 
         # If the response is to end the negotiation, end it but only if there are not partial negotiations
         if response == ResponseType.END_NEGOTIATION:
             if len(self.__agreements) > 0:
                 state.has_error = True
                 stae.error_details = (
                     "Cannot end a negotiation chain with some agreements",
                 )
-                return MechanismRoundResult(stae)
+                return MechanismStepResult(stae)
             state.broken = True
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
 
         # if the response is an acceptance then either register an agreement or a temporary agreement depending on
         # proposal
         if response == ResponseType.ACCEPT_OFFER:
             agreement_index = (
                 self.__next_agent_level
                 if self.__last_proposal.left
@@ -544,24 +542,24 @@
                 self.__temp_agreements[agreement_index] = self.__last_proposal.outcome
             self.__last_proposal = self.__chain[self.__last_proposer_level][
                 self.__last_proposer_number
             ].on_acceptance(self.state, self.__last_proposal)
             self.__last_proposer_level = self.__next_agent_level
             self.__last_proposer_number = self.__next_agent_number
             self._update_next()
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
 
         # now it must be a rejection, ask the one who rejected to propose (in either direction)
         self.__last_proposal = self.__chain[self.__next_agent_level][
             self.__next_agent_number
         ].propose(self.state)
         self.__last_proposer_level = self.__next_agent_level
         self.__last_proposer_number = self.__next_agent_number
         self._update_next()
-        return MechanismRoundResult(state)
+        return MechanismStepResult(state)
 
     def on_confirm(self, level: int, left: bool) -> None:
         """
         Called by negotiators to confirm their temporary accepted agreements
 
         Args:
             level: The caller level
```

### Comparing `negmas-0.9.7/negmas/config.py` & `negmas-0.9.8/negmas/config.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/elicitation/__init__.py` & `negmas-0.9.8/negmas/elicitation/__init__.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/elicitation/base.py` & `negmas-0.9.8/negmas/elicitation/base.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/elicitation/baseline.py` & `negmas-0.9.8/negmas/elicitation/baseline.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/elicitation/common.py` & `negmas-0.9.8/negmas/elicitation/common.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/elicitation/expectors.py` & `negmas-0.9.8/negmas/elicitation/expectors.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/elicitation/mechanism.py` & `negmas-0.9.8/negmas/elicitation/mechanism.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/elicitation/pandora.py` & `negmas-0.9.8/negmas/elicitation/pandora.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/elicitation/queries.py` & `negmas-0.9.8/negmas/elicitation/queries.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/elicitation/strategy.py` & `negmas-0.9.8/negmas/elicitation/strategy.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/elicitation/user.py` & `negmas-0.9.8/negmas/elicitation/user.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/elicitation/voi.py` & `negmas-0.9.8/negmas/elicitation/voi.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/events.py` & `negmas-0.9.8/negmas/events.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/ga.py` & `negmas-0.9.8/negmas/ga.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 """Implements GA-based negotiation mechanisms"""
 
 import copy
 import random
 
-from attr import define, field
+from attrs import define, field
 
-from .mechanisms import Mechanism, MechanismRoundResult, MechanismState
+from .mechanisms import Mechanism, MechanismState, MechanismStepResult
 from .outcomes import Outcome
 
 
 @define
 class GAState(MechanismState):
     """Defines extra values to keep in the mechanism state. This is accessible to all negotiators"""
 
@@ -112,12 +112,12 @@
                         break
                 else:
                     break
             else:
                 self.dominant_outcomes.append(outcomes[target])
         self._current_state.dominant_outcomes = self.dominant_outcomes  # type: ignore
 
-    def __call__(self, state: GAState) -> MechanismRoundResult:
+    def __call__(self, state: GAState) -> MechanismStepResult:
         self.update_ranks()
         self.update_dominant_outcomes()
         self.next_generation(self.select(self.population))
-        return MechanismRoundResult(state=state)
+        return MechanismStepResult(state=state)
```

### Comparing `negmas-0.9.7/negmas/gb/__init__.py` & `negmas-0.9.8/negmas/gb/__init__.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/adapters/tau.py` & `negmas-0.9.8/negmas/gb/adapters/tau.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-from attr import define, field
+from attrs import define, field
 from matplotlib.axes import itertools
 
 from negmas import SAOResponse
 from negmas.common import NegotiatorMechanismInterface
 from negmas.gb.common import GBState, ResponseType
 from negmas.gb.negotiators.base import GBNegotiator
 from negmas.outcomes import Outcome
```

### Comparing `negmas-0.9.7/negmas/gb/common.py` & `negmas-0.9.8/negmas/gb/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from __future__ import annotations
 
 from enum import IntEnum
 from functools import lru_cache
 from typing import TYPE_CHECKING, Literal, Union
 
-from attr import asdict, define, field
+from attrs import asdict, define, field
 
 from negmas.common import MechanismState, NegotiatorMechanismInterface
 from negmas.outcomes import Outcome
 
 if TYPE_CHECKING:
     from negmas.gb.negotiators.base import GBNegotiator
```

### Comparing `negmas-0.9.7/negmas/gb/components/acceptance.py` & `negmas-0.9.8/negmas/gb/components/acceptance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import math
 import random
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Callable, Iterable
 
-from attr import define, field
+from attrs import define, field
 
 from negmas import warnings
 from negmas.common import PreferencesChange, PreferencesChangeType
 from negmas.gb.common import ResponseType
 
 from .base import AcceptancePolicy, FilterResult
 from .concession import ConcessionRecommender
@@ -410,15 +410,15 @@
 
     def on_preferences_changed(self, changes: list[PreferencesChange]):
         if not self.negotiator or not self.negotiator.ufun:
             return
         if any(
             _.type
             not in (
-                PreferencesChangeType.Scaled,
+                PreferencesChangeType.Scale,
                 PreferencesChangeType.ReservedOutcome,
                 PreferencesChangeType.ReservedValue,
             )
             for _ in changes
         ):
             self.negotiator.ufun.invert().init()
```

### Comparing `negmas-0.9.7/negmas/gb/components/base.py` & `negmas-0.9.8/negmas/gb/components/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from collections import namedtuple
 from typing import TYPE_CHECKING
 
-from attr import define, field
+from attrs import define, field
 
 from ...negotiators.components.component import Component
 
 if TYPE_CHECKING:
     from negmas import ResponseType
     from negmas.gb import GBNegotiator, GBState
     from negmas.outcomes import Outcome
```

### Comparing `negmas-0.9.7/negmas/gb/components/concession.py` & `negmas-0.9.8/negmas/gb/components/concession.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import TYPE_CHECKING
 
-from attr import define
+from attrs import define
 
 from negmas.common import Value
 
 from .base import GBComponent
 
 if TYPE_CHECKING:
     from negmas.gb import GBNegotiator, GBState
```

### Comparing `negmas-0.9.7/negmas/gb/components/inverter.py` & `negmas-0.9.8/negmas/gb/components/inverter.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,19 +123,19 @@
         if self.min < ufun.reserved_value:
             self.min = ufun.reserved_value
 
     def before_proposing(self, state: GBState):
         if self._negotiator is None:
             raise ValueError("Unknown negotiator in a component")
         if self.inv is None or self.max is None or self.min is None:
-            warn(
-                f"It seems that on_prefrences_changed() was not called until propose for a ufun of type {self._negotiator.ufun.__class__.__name__}"
-                f" for negotiator {self._negotiator.id} of type {self.__class__.__name__}",
-                NegmasUnexpectedValueWarning,
-            )
+            # warn(
+            #     f"It seems that on_prefrences_changed() was not called until propose for a ufun of type {self._negotiator.ufun.__class__.__name__}"
+            #     f" for negotiator {self._negotiator.id} of type {self.__class__.__name__}",
+            #     NegmasUnexpectedValueWarning,
+            # )
             self.on_preferences_changed([PreferencesChange()])
         if self.inv is None or self.max is None or self.min is None:
             raise ValueError(
                 "Failed to find an invertor, a selector, or exreme outputs"
             )
         if not self.inv.initialized:
             self.inv.init()
@@ -150,19 +150,19 @@
               is the range of the ufun.
             - Subtracts the `tolerance` from the first and adds it to the last utility value
               which slightly enlarges the range to account for small rounding errors
         """
         if self._negotiator is None:
             raise ValueError("Unknown negotiator in a component")
         if self.max is None or self.min is None or self.best is None:
-            warn(
-                f"It seems that on_prefrences_changed() was not called until propose for a ufun of type {self._negotiator.ufun.__class__.__name__}"
-                f" for negotiator {self._negotiator.id} of type {self.__class__.__name__}",
-                NegmasUnexpectedValueWarning,
-            )
+            # warn(
+            #     f"It seems that on_prefrences_changed() was not called until propose for a ufun of type {self._negotiator.ufun.__class__.__name__}"
+            #     f" for negotiator {self._negotiator.id} of type {self.__class__.__name__}",
+            #     NegmasUnexpectedValueWarning,
+            # )
             self.on_preferences_changed([PreferencesChange()])
         if self.max is None or self.min is None:
             raise ValueError("Cannot find extreme outcomes.")
         adjusted = [(self.max - self.min) * _ + self.min for _ in urange]
         if adjusted:
             adjusted[0] -= self.eps
             adjusted[-1] += self.eps
```

### Comparing `negmas-0.9.7/negmas/gb/components/models/ufun.py` & `negmas-0.9.8/negmas/gb/components/models/ufun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from attr import define, field
+from attrs import define, field
 
 from negmas.preferences import RankOnlyUtilityFunction
 from negmas.preferences.base_ufun import BaseUtilityFunction
 from negmas.preferences.mixins import StationaryMixin
 
 from ..base import GBComponent
```

### Comparing `negmas-0.9.7/negmas/gb/components/offering.py` & `negmas-0.9.8/negmas/gb/components/offering.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import math
 import random
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
-from attr import define, field
+from attrs import define, field
 
 from negmas import warnings
 from negmas.common import PreferencesChangeType, Value
 from negmas.preferences.inv_ufun import PresortingInverseUtilityFunction
 
 from .base import FilterResult, OfferingPolicy
 from .concession import ConcessionRecommender
@@ -51,15 +51,15 @@
 
     def on_preferences_changed(self, changes: list[PreferencesChange]):
         if not self.negotiator or not self.negotiator.ufun:
             return
         if any(
             _.type
             not in (
-                PreferencesChangeType.Scaled,
+                PreferencesChangeType.Scale,
                 PreferencesChangeType.ReservedOutcome,
                 PreferencesChangeType.ReservedValue,
             )
             for _ in changes
         ):
             self.sorter = PresortingInverseUtilityFunction(
                 self.negotiator.ufun, sort_rational_only=True
@@ -114,32 +114,35 @@
     ) -> None:
         self._received.add(offer)
         return super().on_partner_proposal(state, partner_id, offer)
 
 
 @define
 class CABOfferingPolicy(OfferingPolicy):
-
     next_indx: int = 0
     sorter: PresortingInverseUtilityFunction | None = field(repr=False, default=None)
     _last_offer: Outcome | None = field(init=False, default=None)
     _repeating: bool = field(init=False, default=False)
 
     def on_preferences_changed(self, changes: list[PreferencesChange]):
         if not self.negotiator or not self.negotiator.ufun:
             return
         if any(
             _.type
             not in (
-                PreferencesChangeType.Scaled,
+                PreferencesChangeType.Scale,
                 PreferencesChangeType.ReservedOutcome,
                 PreferencesChangeType.ReservedValue,
             )
             for _ in changes
         ):
+            if self.sorter is not None:
+                warnings.warn(
+                    f"Sorter is already initialized. May be on_preferences_changed is called twice!!"
+                )
             self.sorter = PresortingInverseUtilityFunction(
                 self.negotiator.ufun, sort_rational_only=True
             )
             self.sorter.init()
             self.next_indx = 0
             self._repeating = False
 
@@ -150,14 +153,17 @@
             or not self.negotiator.ufun
             or not self.negotiator.nmi
         ):
             return self._last_offer
         if self.next_indx >= self.negotiator.nmi.n_outcomes:
             return self._last_offer
         if not self.sorter:
+            warnings.warn(
+                f"Sorter is not initialized. May be on_preferences_changed is never called before propose!!"
+            )
             self.sorter = PresortingInverseUtilityFunction(
                 self.negotiator.ufun, sort_rational_only=True
             )
             self.sorter.init()
         outcome = self.sorter.outcome_at(self.next_indx)
         if (
             outcome is None
@@ -171,15 +177,14 @@
         self.next_indx += 1
         self._last_offer = outcome
         return outcome
 
 
 @define
 class WAROfferingPolicy(OfferingPolicy):
-
     next_indx: int = 0
     sorter: PresortingInverseUtilityFunction | None = field(repr=False, default=None)
     _last_offer: Outcome | None = field(init=False, default=None)
     _repeating: bool = field(init=False, default=False)
     _irrational: bool = field(init=False, default=True)
     _irrational_index: int = field(init=False, default=-1)
 
@@ -187,20 +192,24 @@
         if not self.negotiator or not self.negotiator.ufun:
             return
         self._irrational = True
         self._irrational_index = self.negotiator.nmi.n_outcomes - 1
         if any(
             _.type
             not in (
-                PreferencesChangeType.Scaled,
+                PreferencesChangeType.Scale,
                 PreferencesChangeType.ReservedOutcome,
                 PreferencesChangeType.ReservedValue,
             )
             for _ in changes
         ):
+            if self.sorter is not None:
+                warnings.warn(
+                    f"Sorter is already initialized. May be on_preferences_changed is called twice!!"
+                )
             self.sorter = PresortingInverseUtilityFunction(
                 self.negotiator.ufun, sort_rational_only=True
             )
             self.sorter.init()
             self.next_indx = 0
             self._repeating = False
 
@@ -214,14 +223,17 @@
         if not self.negotiator or not self.negotiator.ufun or not self.negotiator.nmi:
             return self._last_offer
         if self._repeating:
             return self._last_offer
         if not self._irrational and self.next_indx >= self.negotiator.nmi.n_outcomes:
             return self._last_offer
         if not self.sorter:
+            warnings.warn(
+                f"Sorter is not initialized. May be on_preferences_changed is never called before propose!!"
+            )
             self.sorter = PresortingInverseUtilityFunction(
                 self.negotiator.ufun, sort_rational_only=True
             )
             self.sorter.init()
         nxt = self._irrational_index if self._irrational else self.next_indx
         outcome = self.sorter.outcome_at(nxt)
         if self._irrational:
@@ -328,15 +340,15 @@
 
     def on_preferences_changed(self, changes: list[PreferencesChange]):
         if not self.negotiator or not self.negotiator.ufun:
             return
         if any(
             _.type
             not in (
-                PreferencesChangeType.Scaled,
+                PreferencesChangeType.Scale,
                 PreferencesChangeType.ReservedOutcome,
                 PreferencesChangeType.ReservedValue,
             )
             for _ in changes
         ):
             self.negotiator.ufun.invert().init()
```

### Comparing `negmas-0.9.7/negmas/gb/components/selectors.py` & `negmas-0.9.8/negmas/gb/components/selectors.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/constraints/base.py` & `negmas-0.9.8/negmas/gb/constraints/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Base Constraints on offering constaints
 """
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 
-from attr import define
+from attrs import define
 
 from negmas.gb.common import GBState, ThreadState
 from negmas.outcomes.common import Outcome
 
 __all__ = [
     "OfferingConstraint",
     "LocalOfferingConstraint",
```

### Comparing `negmas-0.9.7/negmas/gb/constraints/rfo.py` & `negmas-0.9.8/negmas/gb/constraints/rfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import sys
 
-from attr import define
+from attrs import define
 
 from ..common import ThreadState
 from .base import LocalOfferingConstraint
 
 __all__ = ["RepeatFinalOfferOnly"]
```

### Comparing `negmas-0.9.7/negmas/gb/constraints/rlo.py` & `negmas-0.9.8/negmas/gb/constraints/rlo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import sys
 
-from attr import define
+from attrs import define
 
 from ..common import ThreadState
 from .base import LocalOfferingConstraint
 
 __all__ = ["RepeatLastOfferOnly"]
```

### Comparing `negmas-0.9.7/negmas/gb/evaluators/base.py` & `negmas-0.9.8/negmas/gb/evaluators/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Base Evaluation Strategies
 """
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from random import choice
 
-from attr import asdict, define
+from attrs import asdict, define
 
 from negmas.common import MechanismState
 from negmas.gb.common import GBResponse, GBState, ThreadState
 from negmas.outcomes.common import Outcome
 
 __all__ = [
     "EvaluationStrategy",
```

### Comparing `negmas-0.9.7/negmas/gb/evaluators/gao.py` & `negmas-0.9.8/negmas/gb/evaluators/gao.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/evaluators/tau.py` & `negmas-0.9.8/negmas/gb/evaluators/tau.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from collections import defaultdict
 from sys import maxsize
 from typing import Literal
 
-from attr import define, field
+from attrs import define, field
 
 from negmas.outcomes import Outcome
 
 from ..common import GBState, ResponseType
 from ..evaluators.base import EvaluationStrategy
 
 INFINITE = maxsize
```

### Comparing `negmas-0.9.7/negmas/gb/mechanisms/base.py` & `negmas-0.9.8/negmas/gb/mechanisms/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from random import shuffle
 from typing import TYPE_CHECKING, Any, Callable
 
-from attr import define
+from attrs import define
 
 from negmas.common import TraceElement
 from negmas.helpers.types import get_full_type_name, instantiate
-from negmas.mechanisms import Mechanism, MechanismRoundResult
+from negmas.mechanisms import Mechanism, MechanismStepResult
 from negmas.outcomes import Outcome
 from negmas.plots.util import default_colorizer
 from negmas.preferences import BaseUtilityFunction, Preferences
 
 from ..common import GBResponse, GBState, ResponseType, ThreadState
 from ..constraints.base import LocalOfferingConstraint, OfferingConstraint
 from ..evaluators.base import EvaluationStrategy, LocalEvaluationStrategy, all_accept
@@ -248,15 +248,15 @@
         shuffle(indices)
         threads = [self._threads[_] for _ in indices]
         results = dict()
         for t in threads:
             results[t.negotiator.id] = _do_run(t.negotiator.id, t)
         return results
 
-    def __call__(self, state: GBState) -> MechanismRoundResult:
+    def __call__(self, state: GBState) -> MechanismStepResult:
         # print(f"Round {self._current_state.step}")
         results = self.run_threads()
         # if state.step > self.outcome_space.cardinality:
         #     self.plot()
         #     breakpoint()
         responses = []
         for source, (tstate, response) in results.items():
@@ -269,19 +269,19 @@
             )
         if self._global_constraint:
             responses.append(self._global_constraint(state, self._history))
 
         e = self._combiner(responses)
 
         if e == "continue":
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
         if e is None:
             state.broken = True
         state.agreement = e
-        return MechanismRoundResult(state)
+        return MechanismStepResult(state)
 
     @property
     def full_trace(self) -> list[TraceElement]:
         def response(state: GBState):
             if state.timedout:
                 return "timedout"
             if state.ended:
```

### Comparing `negmas-0.9.7/negmas/gb/mechanisms/mechanisms.py` & `negmas-0.9.8/negmas/gb/mechanisms/mechanisms.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/__init__.py` & `negmas-0.9.8/negmas/gb/negotiators/__init__.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/base.py` & `negmas-0.9.8/negmas/gb/negotiators/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             Tuple[ResponseType, Outcome]: The response to the given offer with a counter offer if the response is REJECT
 
         """
         from negmas.sao.common import SAOResponse
 
         if self.__end_negotiation:
             return SAOResponse(ResponseType.END_NEGOTIATION, None)
-        if self.ufun is not None:
+        if self.preferences is not None:
             changes = self.ufun.changes()
             if changes:
                 self.on_preferences_changed(changes)
         if offer is None:
             return SAOResponse(ResponseType.REJECT_OFFER, self.propose_(state=state))
         response = self.respond_(state=state, offer=offer)
         if response != ResponseType.REJECT_OFFER:
```

### Comparing `negmas-0.9.7/negmas/gb/negotiators/cab.py` & `negmas-0.9.8/negmas/gb/negotiators/cab.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/limited.py` & `negmas-0.9.8/negmas/gb/negotiators/limited.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/micro.py` & `negmas-0.9.8/negmas/gb/negotiators/micro.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/modular/boa.py` & `negmas-0.9.8/negmas/gb/negotiators/modular/boa.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/modular/mapneg.py` & `negmas-0.9.8/negmas/gb/negotiators/modular/mapneg.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/modular/modular.py` & `negmas-0.9.8/negmas/gb/negotiators/modular/modular.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/nice.py` & `negmas-0.9.8/negmas/gb/negotiators/nice.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/randneg.py` & `negmas-0.9.8/negmas/gb/negotiators/randneg.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/timebased.py` & `negmas-0.9.8/negmas/gb/negotiators/timebased.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     """
     Represents a time-based negotiation strategy that is independent of the offers received during the negotiation.
 
     Args:
         offering_curve (TimeCurve): A `TimeCurve` that is to be used to sample outcomes when offering
         accepting_curve (TimeCurve): A `TimeCurve` that is to be used to decide utility range to accept
         inverter (UtilityInverter): A component used to keep track of the ufun inverse
-        stochastic (bool): If `False` the worst outcome in the current utility range will be used
+        offer_selector (OfferSelector): The way to select an offer from the set of valid offers at every time-step
     """
 
     def __init__(
         self,
         *args,
         offering_curve: TimeCurve
         | Literal["boulware"]
@@ -106,15 +106,15 @@
         | Literal["conceder"]
         | Literal["linear"]
         | float
         | None = None,
         offer_selector: OfferSelector | None = None,
         **kwargs,
     ):
-        super().__init__(*args, **kwargs)
+        super().__init__(*args, offer_selector=offer_selector, **kwargs)
         offering_curve = make_curve(offering_curve, 1.0)
         if accepting_curve is None:
             accepting_curve = offering_curve
         else:
             accepting_curve = make_curve(accepting_curve, 1.0)
         self._offering_curve = offering_curve
         self._accepting_curve = accepting_curve
@@ -229,15 +229,18 @@
 
     """
 
     def __init__(
         self,
         *args,
         max_aspiration=1.0,
-        aspiration_type="boulware",
+        aspiration_type: Literal["boulware"]
+        | Literal["conceder"]
+        | Literal["linear"]
+        | float = "boulware",
         stochastic=False,
         presort: bool = False,
         tolerance: float = 0.001,
         **kwargs,
     ):
         ufun_inverter = None if not presort else PresortingInverseUtilityFunction
         super().__init__(
```

### Comparing `negmas-0.9.7/negmas/gb/negotiators/titfortat.py` & `negmas-0.9.8/negmas/gb/negotiators/titfortat.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/tough.py` & `negmas-0.9.8/negmas/gb/negotiators/tough.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/gb/negotiators/utilbased.py` & `negmas-0.9.8/negmas/gb/negotiators/utilbased.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     """
     A negotiator that bases its decisions on the utility value of outcomes only.
 
     Args:
         inverter (UtilityInverter): A component used to keep track of the ufun inverse
         stochastic (bool): If `False` the worst outcome in the current utility range will be used
         rank_only (bool): If `True` then the ranks of outcomes not their actual utilities will be used for decision making
-        max_cardinality (int): The number of outocmes at which we switch to use the slower `SamplingInverseUtilityFunction` instead of the `PresortingInverseUtilityFunction` . Will only be used if `ufun_inverter` is `None`
+        max_cardinality (int): The number of outocmes at which we switch to use the slower `SamplingInverseUtilityFunction`
+                               instead of the `PresortingInverseUtilityFunction` . Will only be used if `ufun_inverter` is `None`
         eps (float): A tolearnace around the utility range used when sampling outocmes
     """
 
     def __init__(
         self,
         *args,
         stochastic: bool = False,
```

### Comparing `negmas-0.9.7/negmas/gb/negotiators/war.py` & `negmas-0.9.8/negmas/gb/negotiators/war.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/generics.py` & `negmas-0.9.8/negmas/generics.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/genius/bridge.py` & `negmas-0.9.8/negmas/genius/bridge.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/genius/ginfo.py` & `negmas-0.9.8/negmas/genius/ginfo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""
-Keeps information about ANAC competitions and Genius Agents
-"""
+"""Keeps information about ANAC competitions and Genius Agents."""
 from __future__ import annotations
 
 import itertools
 
+from negmas.helpers.strings import shortest_unique_names
+
 __all__ = [
     "GENIUS_INFO",
     "AGENT_BASED_NEGOTIATORS",
     "PARTY_BASED_NEGOTIATORS",
     "ALL_NEGOTIATORS",
     "TEST_FAILING_NEGOTIATORS",
     "ALL_PASSING_NEGOTIATORS",
@@ -234,16 +234,22 @@
     },
     2017: {
         "winners": [
             [("PonPokoAgent", "agents.anac.y2017.ponpokoagent.PonPokoAgent")],
             [("CaduceusDC16", "agents.anac.y2017.caduceusdc16.CaduceusDC16")],
             [("Rubick", "agents.anac.y2017.rubick.Rubick")],
         ],
+        "winners_nash": [
+            [("ParsCat2", "agents.anac.y2016.parscat.ParsCat")],
+            [("AgentKN", "agents.anac.y2017.agentkn.AgentKN")],
+            [("ParsAgent3", "agents.anac.y2017.parsagent3.ShahAgent")],
+        ],
         "linear": True,
         "learning": True,
+        "learning_full_exchange": False,
         "multilateral": True,
         "bilateral": False,
         "reservation": None,
         "discounting": False,
         "uncertainty": False,
         "elicitation": False,
     },
@@ -254,29 +260,37 @@
                     "AgreeableAgent2018",
                     "agents.anac.y2018.agreeableagent2018.AgreeableAgent2018",
                 )
             ],
             [("MengWan", "agents.anac.y2018.meng_wan.Agent36")],
             [("BetaOne", "agents.anac.y2018.beta_one.Group2")],
         ],
+        "winners_welfare": [
+            [("Herb", "agents.anac.y2018.agentherb.AgentHerb")],
+            [("Agent33", "agents.anac.y2018.agent33.Agent33")],
+            [("Sontag", "agents.anac.y2018.sontag.Sontag")],
+        ],
         "linear": True,
         "learning": True,
+        "learning_full_exchange": True,
         "multilateral": True,
         "bilateral": False,
         "reservation": None,
         "discounting": True,
         "uncertainty": False,
         "elicitation": False,
     },
     # 2019: {
-    #     "winners": [["AgentGG"],[ "KakeSoba"],[ "SAGA"]],
+    #     "winners": [[("AgentGG", "")], [("KakeSoba", "")], [("SAGA", "")]],
+    #     "winners_nash": [[("WinkyAgent", "")], [("FSEGA2019", "")], [("AgentGP", "")]],
+    #     "finalists": [[("AgentGG", "")], [("KakeSoba", "")], [("SAGA", "")]],
     #     "linear": True,
-    #     "learning": True,
-    #     "multilateral": True,
-    #     "bilateral": False,
+    #     "learning": False,
+    #     "multilateral": False,
+    #     "bilateral": True,
     #     "reservation": None,
     #     "discounting": None,
     #     "uncertainty": True,
     #     "elicitation": False,
     # },
     # 2020: {
     #     "winners": [],
@@ -294,15 +308,16 @@
 
 ALL_GENIUS_INVALID_NEGOTIATORS = [
     "agents.UIAgent",
     "agents.UIAgentExtended",
     "negotiator.parties.CounterOfferHumanNegotiationParty",
     "agents.FunctionalAcceptor",
 ]
-"""Genius agents that are known not to work (most likely because they require human interaction)"""
+"""Genius agents that are known not to work (most likely because they require
+human interaction)"""
 
 ALL_GENIUS_BASIC_NEGOTIATORS = [
     "agents.ImmediateAcceptor",
     "agents.SimpleAgent",
     "negotiator.parties.RandomCounterOfferNegotiationParty",
     "negotiator.parties.RandomParty",
     "negotiator.parties.RandomParty2",
@@ -314,15 +329,16 @@
     "negotiator.parties.ConcederNegotiationParty",
     "agents.SimilarityAgent",
     "agents.FuzzyAgent",
     "agents.OptimalBidderSimple",
     "agents.BayesianAgent",
     "agents.ABMPAgent2",
 ]
-"""Basic negotiators defined in Genius that are not based on any ANAC submissions"""
+"""Basic negotiators defined in Genius that are not based on any ANAC
+submissions."""
 
 ALL_GENIUS_NEGOTIATORS = [
     "agents.ABMPAgent2",
     "agents.BayesianAgent",
     "agents.FunctionalAcceptor",
     "agents.FuzzyAgent",
     "agents.ImmediateAcceptor",
@@ -473,49 +489,49 @@
     "agents.anac.y2018.ponpokorampage.PonPokoRampage",
     "agents.anac.y2018.seto.Seto",
     "agents.anac.y2018.shiboy.Shiboy",
     "agents.anac.y2018.smac_agent.SMAC_Agent",
     "agents.anac.y2018.sontag.Sontag",
     "agents.anac.y2018.yeela.Yeela",
 ]
-"""All Negotiators Accessible through Genius UI"""
+"""All Negotiators Accessible through Genius UI."""
 
 
-ALL_NON_SOAP_GENIUS_NEGOTIATORS = [
+ALL_NON_SAOP_GENIUS_NEGOTIATORS = [
     "parties.AlternatingMultipleOffers.RandomAmopParty",
     "parties.AlternatingMultipleOffers.RandomAmopPartyMajority",
     "parties.simplemediator.RandomFlippingMediator",
     "parties.simplemediator.FixedOrderFlippingMediator",
     "parties.simplemediator.HillClimber",
     "parties.simplemediator.Annealer",
     "parties.simplemediator.FeedbackParty",
     "parties.feedbackmediator.FeedbackMediator",
     "parties.FeedbackHillClimber",
 ]
-"""All Genius negotiators for protocols other than SAOP"""
+"""All Genius negotiators for protocols other than SAOP."""
 
 ALL_GENIUS_AMOP_NEGOTIATORS = [
     "parties.AlternatingMultipleOffers.RandomAmopParty",
     "parties.AlternatingMultipleOffers.RandomAmopPartyMajority",
 ]
-"""All Genius negotiators for the Alternating Multiple Offers Protocol"""
+"""All Genius negotiators for the Alternating Multiple Offers Protocol."""
 
 ALL_GENIUS_SIMPLE_MEDIATOR_NEGOTIATORS = [
     "parties.simplemediator.RandomFlippingMediator",
     "parties.simplemediator.FixedOrderFlippingMediator",
     "parties.simplemediator.HillClimber",
     "parties.simplemediator.Annealer",
     "parties.simplemediator.FeedbackParty",
 ]
-"""All Genius negotiators for the Simple Mediator Protocol"""
+"""All Genius negotiators for the Simple Mediator Protocol."""
 
 ALL_GENIUS_FEEDBACK_MEDIATOR_NEGOTIATORS = [
     "parties.feedbackmediator.FeedbackMediator",
 ]
-"""All Genius negotiators for the Feedback Mediator Protocol"""
+"""All Genius negotiators for the Feedback Mediator Protocol."""
 
 AGENT_BASED_NEGOTIATORS = [
     "agents.ABMPAgent",
     "agents.ABMPAgent2",
     "agents.BayesianAgent",
     "agents.BayesianAgentForAuction",
     "agents.DecUtilAgent",
@@ -567,15 +583,18 @@
     "agents.anac.y2014.Flinch.Flinch",
     "agents.anac.y2014.Gangster.Gangster",
     "agents.anac.y2014.KGAgent.KGAgent",
     "agents.anac.y2014.SimpaticoAgent.Simpatico",
     "agents.anac.y2014.Sobut.Sobut",
     "agents.anac.y2017.geneking.GeneKing",
 ]
-"""Genius agents based on the Agent base-class. These are the oldest agents"""
+"""Genius agents based on the Agent base-class.
+
+These are the oldest agents
+"""
 
 PARTY_BASED_NEGOTIATORS = [
     "agents.ai2014.group1.Group1",
     "agents.ai2014.group10.Group10",
     "agents.ai2014.group11.Group11",
     "agents.ai2014.group12.Group12",
     "agents.ai2014.group2.Group2",
@@ -620,15 +639,18 @@
     "agents.anac.y2017.agentf.AgentF",
     "agents.anac.y2017.caduceusdc16.CaduceusDC16",
     "agents.anac.y2017.farma.Farma17",
     "agents.anac.y2017.ponpokoagent.PonPokoAgent",
     "agents.anac.y2017.tangxun.taxibox",
     "agents.anac.y2017.tucagent.TucAgent",
 ]
-"""Genius agents based on the Party base-class. These are the newest agents"""
+"""Genius agents based on the Party base-class.
+
+These are the newest agents
+"""
 
 TEST_FAILING_NEGOTIATORS = [
     "agents.ABMPAgent2",  # failed some but not all tests
     "agents.BayesianAgentForAuction",
     "agents.DecUtilAgent",
     "agents.FuzzyAgent",  # fails most test but not all
     "agents.OptimalBidder",
@@ -692,43 +714,72 @@
                     if v["multilateral"] and not v["learning"]
                 )
             )
         )
     )
     - set(TEST_FAILING_NEGOTIATORS)
 )
-"""Some of the most tested negotaitors"""
+"""Some of the most tested negotaitors."""
 
 ALL_NEGOTIATORS = list(
     set(PARTY_BASED_NEGOTIATORS + AGENT_BASED_NEGOTIATORS + ALL_GENIUS_NEGOTIATORS)
 )
-"""All Genius Negotiators accessible from NegMAS"""
+"""All Genius Negotiators accessible from NegMAS."""
 
 ALL_PASSING_NEGOTIATORS = list(
     set(ALL_NEGOTIATORS)
     - set(TEST_FAILING_NEGOTIATORS)
     - set(ALL_GENIUS_INVALID_NEGOTIATORS)
 )
-"""All negotiators that passed simple tests showing they work on the bridge"""
+"""All negotiators that passed simple tests showing they work on the bridge."""
 
 ALL_ANAC_AGENTS = [_ for _ in ALL_NEGOTIATORS if "anac" in _]
-"""All agents submitted to ANAC and registered in Genius"""
+"""All agents submitted to ANAC and registered in Genius."""
+
+_names = shortest_unique_names(ALL_GENIUS_NEGOTIATORS)
+_names_simpler = [_.replace("_", "") for _ in _names]
+_names_lower = [_.lower().replace("agent", "") for _ in _names_simpler]
+
+NAME_CLASS_MAP = dict(zip(_names_lower, ALL_GENIUS_NEGOTIATORS))
+"""Mapping a short name to a Java class."""
+
+NAME_CLASS_MAP.update(dict(zip(_names_simpler, ALL_GENIUS_NEGOTIATORS)))
+NAME_CLASS_MAP.update(dict(zip(_names, ALL_GENIUS_NEGOTIATORS)))
+"""Mapping a short name to a Java class."""
+
+CLASS_NAME_MAP = dict(zip(ALL_GENIUS_NEGOTIATORS, _names))
+"""Mapping a Java class to a short name matching the class name in Java."""
+
+CLASS_NAME_MAP_SIMPLE = dict(zip(ALL_GENIUS_NEGOTIATORS, _names_lower))
+"""Mapping a Java class to a short name that is short lowercase and with no 'agent' word or underscores."""
 
+ALL_GENIUS_NEGOTIATORS_SET = set(ALL_GENIUS_NEGOTIATORS)
 
-def get_name(java_class: str) -> str:
-    """Returns the name of the agent with the given class"""
-    return java_class.split(".")[-1]
 
+def get_name(
+    java_class: str, allow_dot: bool = True, simple_version: bool = False
+) -> str:
+    """Returns the name of the agent with the given class."""
+    d = CLASS_NAME_MAP_SIMPLE if simple_version else CLASS_NAME_MAP
+    name = d[java_class]
+    if not allow_dot:
+        return name.split(".")[-1]
+    return name
 
-def get_java_class(name) -> str | None:
-    """Returns the java class for the agent with this name if known otherwise it returns None"""
-    for class_name in ALL_NEGOTIATORS:
-        if name in class_name:
-            return class_name
-    return None
+
+def get_java_class(name: str) -> str | None:
+    """Returns the java class for the agent with this name if known otherwise
+    it returns None.
+
+    The name can be either the java class itself or the short agent name
+    """
+    java_class = NAME_CLASS_MAP.get(
+        name, name if name in ALL_GENIUS_NEGOTIATORS_SET else None
+    )
+    return java_class
 
 
 def get_anac_agents(
     *,
     year: int | None = None,
     linear: bool | None = None,
     learning: bool | None = None,
@@ -737,30 +788,28 @@
     reservation: bool | None = None,
     discounting: bool | None = None,
     uncertainty: bool | None = None,
     elicitation: bool | None = None,
     winners_only: bool = False,
     finalists_only: bool = False,
 ) -> list[tuple[str, str]]:
-    """
-    Get Genius agents matching some given criteria
+    """Get Genius agents matching some given criteria.
 
     Returns:
         a list of 2-item tuples giving agent name and java class name.
 
     Remarks:
         - For all criteria other than winners_only, and finalists_only, passing
           None means no constraints otherwise the game on the given year must
           match the criterion value (True or False) to get agents from this year.
         - This function uses a heuristic and may not be completely accurate. Use
           with caution.
     """
 
     def get_agents(year, d) -> set[tuple[str, str]]:
-
         if winners_only:
             lst = d.get("winners", [[]])
             lst = list(itertools.chain(*lst))
         elif finalists_only:
             lst = d.get("finalists", [])
             lst = list(itertools.chain(*lst))
         else:
```

### Comparing `negmas-0.9.7/negmas/genius/gnegotiators.py` & `negmas-0.9.8/negmas/genius/gnegotiators.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/genius/negotiator.py` & `negmas-0.9.8/negmas/genius/negotiator.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,15 +112,14 @@
         self.__my_last_offer = None
         self.__my_last_response = ResponseType.REJECT_OFFER
         self.__my_last_offer_step = -1000
         self._preferences, self.discount = None, None
         self.issue_names = self.issues = self.issue_index = None
         self.auto_load_java = auto_load_java
         if domain_file_name is not None:
-
             from ..inout import get_domain_issues
 
             # we keep original issues details so that we can create appropriate answers to Java
             self.issues = get_domain_issues(
                 domain_file_name=domain_file_name,
             )
             if not self.issues:
@@ -341,28 +340,37 @@
             output += f"{i}{INTERNAL_SEP}{v}{ENTRY_SEP}"
         output = output[: -len(ENTRY_SEP)]
         return output
 
     def destroy_java_counterpart(self, state=None) -> None:
         if self.__started and not self.__destroyed:
             if self.java is not None:
-                self.__frozen_relative_time = self.java.get_relative_time(  # type: ignore
-                    self.java_uuid
-                )
+                try:
+                    self.__frozen_relative_time = self.java.get_relative_time(  # type: ignore
+                        self.java_uuid
+                    )
+                except:
+                    if state:
+                        self.__frozen_relative_time = state.relative_time
+                    else:
+                        self.__frozen_relative_time = self.nmi.state.relative_time
                 result = self.java.on_negotiation_end(  # type: ignore
                     self.java_uuid,
                     None
                     if state is None
                     else self._outcome2str(state.agreement)
                     if state.agreement is not None
                     else None,
                 )
-                if result in (OK, TIMEOUT):
+                if any(result.startswith(_) for _ in (OK, TIMEOUT)):
                     result = self.java.destroy_agent(self.java_uuid)  # type: ignore
-                    if result in (FAILED, TIMEOUT) and self._strict:
+                    if (
+                        any(result.startswith(_) for _ in (FAILED, TIMEOUT))
+                        and self._strict
+                    ):
                         raise ValueError(
                             f"{self._me()} ended the negotiation but failed to destroy the agent. A possible memory leak"
                         )
                 elif self._strict:
                     raise ValueError(f"{self._me()} failed to end the negotiation!!")
             self.__destroyed = True
         if self._temp_preferences_file:
@@ -423,15 +431,19 @@
             self.set_preferences(
                 make_discounted_ufun(
                     self.ufun,
                     discount_per_round=self.discount,
                     power_per_round=1.0,
                 )
             )
-        n_steps = -1 if info.n_steps is None else int(info.n_steps)  # number of steps
+        n_steps = (
+            -1
+            if info.n_steps is None or math.isinf(info.n_steps)
+            else int(info.n_steps)
+        )
         n_seconds = (
             -1
             if info.time_limit is None or math.isinf(info.time_limit)
             else int(info.time_limit)
         )  # time limit
         timeout = (
             info.negotiator_time_limit
@@ -479,17 +491,27 @@
                 n_seconds > 0,
                 self.domain_file_name,  # domain file
                 self.utility_file_name,  # Negotiator file
                 timeout,
                 self._strict,
             )
             self.__started = result == OK
+            if result != OK:
+                s = (
+                    f"{self._me()}: Failed Starting: {result.split(FIELD_SEP)}\nDomain file: {self.domain_file_name}\n"
+                    f"UFun file: {self.domain_file_name}\n{'strict' if self._strict else 'non-strict'} {n_steps=} {timeout=}"
+                )
+                if self._strict:
+                    raise ValueError(s)
+                else:
+                    warnings.warn(s, warnings.NegmasCannotStartNegotiation)
         except Exception as e:
             raise ValueError(
-                f"{self._me()}: Cannot start negotiation: {str(e)}\nDomain file: {self.domain_file_name}\nUFun file: {self.domain_file_name}\n{'strict' if self._strict else 'non-strict'} {n_steps=} {timeout=}"
+                f"{self._me()}: Cannot start negotiation: {str(e)}\nDomain file: {self.domain_file_name}\n"
+                f"UFun file: {self.domain_file_name}\n{'strict' if self._strict else 'non-strict'} {n_steps=} {timeout=}"
             )
 
     def cancel(self, reason=None) -> None:
         try:
             self.java.cancel(self.java_uuid)  # type: ignore
         except:
             pass
@@ -528,22 +550,24 @@
             if self._strict:
                 raise ValueError(f"{self._me()} received no actions while parsing")
             return ResponseType.REJECT_OFFER, None
         _, typ_, bid_str = action.split(FIELD_SEP)
         nmi = self.nmi
         if not nmi:
             raise ValueError("Cannot parse without an NMI")
-        if typ_ == FAILED:
+        if typ_.startswith(FAILED):
+            e = typ_.split(FIELD_SEP)[-1]
             raise ValueError(
-                f"{self._me()} sent an action that cannot be parsed ({action})"
+                f"{self._me()} failed in receive_message ({action}) Exception {e}"
             )
-        elif typ_ == TIMEOUT:
+        elif typ_.startswith(TIMEOUT):
+            e = typ_.split(FIELD_SEP)[-1]
             if nmi.state.relative_time < 1.0 - 1e-2:
                 raise ValueError(
-                    f"{self._me()} indicated that it timedout at relative time ({nmi.state.relative_time})"
+                    f"{self._me()} indicated that it timedout at relative time ({nmi.state.relative_time}) Exception {e}"
                 )
 
         issues = nmi.cartesian_outcome_space.issues
 
         def map_value(issue: Issue, val: str):
             if not issue.value_type:
                 return val
@@ -605,17 +629,17 @@
         received = self.java.receive_message(  # type: ignore
             self.java_uuid,
             state.current_proposer,
             "Offer",
             self._outcome2str(offer),
             state.step,
         )
-        if self._strict and received == FAILED:
+        if self._strict and received.startswith(FAILED):
             raise ValueError(
-                f"{self._me()} failed to receive message in step {state.step}"
+                f"{self._me()} failed to receive message in step {state.step}. {received.split(FIELD_SEP)[-1]}"
             )
         self.propose_sao(state)
 
     def propose_sao(self, state: SAOState) -> SAOResponse:
         if state.step == self.__my_last_offer_step:
             return SAOResponse(self.__my_last_response, self.__my_last_offer)
         response, outcome = self.parse(
@@ -669,17 +693,17 @@
         received = self.java.receive_message(  # type: ignore
             self.java_uuid,
             source,
             "Offer",
             self._outcome2str(offer),
             state.step,
         )
-        if self._strict and received == FAILED:
+        if self._strict and received.startswith(FAILED):
             raise ValueError(
-                f"{self._me()} failed to receive message in step {state.step}"
+                f"{self._me()} failed to receive message in step {state.step}: {received.split(FIELD_SEP)[-1]}"
             )
         self.propose(state)
         return self.__my_last_response
 
     def propose(self, state: GBState) -> Outcome | None:
         # saves one new offer/response every step
         if state.step == self.__my_last_offer_step:
```

### Comparing `negmas-0.9.7/negmas/helpers/__init__.py` & `negmas-0.9.8/negmas/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/helpers/inout.py` & `negmas-0.9.8/negmas/helpers/inout.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/helpers/logging.py` & `negmas-0.9.8/negmas/helpers/logging.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/helpers/misc.py` & `negmas-0.9.8/negmas/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/helpers/numeric.py` & `negmas-0.9.8/negmas/helpers/numeric.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/helpers/prob.py` & `negmas-0.9.8/negmas/helpers/prob.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/helpers/strings.py` & `negmas-0.9.8/negmas/helpers/strings.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/helpers/timeout.py` & `negmas-0.9.8/negmas/helpers/timeout.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/helpers/types.py` & `negmas-0.9.8/negmas/helpers/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
     """
     Gets the ful typename of a type. You *should not* pass an instance to this function but it may just work.
 
     An exception is that if the input is of type `str` or if it is None, it will be returned as it is
     """
     if t is None or isinstance(t, str):
         return t
+    if isinstance(t, functools.partial):
+        t = t.func
     if not hasattr(t, "__module__") and not hasattr(t, "__name__"):
         t = type(t)
     return t.__module__ + "." + t.__name__  # type: ignore
 
 
 def import_by_name(full_name: str) -> Any:
     """Imports something form a module using its full name"""
```

### Comparing `negmas-0.9.7/negmas/inout.py` & `negmas-0.9.8/negmas/inout.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import xml.etree.ElementTree as ET
 from os import PathLike, listdir
 from pathlib import Path
 from random import shuffle
 from typing import Any, Callable, Iterable, Sequence
 
-from attr import define
+from attrs import define
 
 from negmas.helpers.inout import dump
 from negmas.outcomes.outcome_space import make_os
 from negmas.preferences.crisp.linear import LinearAdditiveUtilityFunction
 from negmas.preferences.ops import ScenarioStats, calc_scenario_stats
 from negmas.serialization import PYTHON_CLASS_IDENTIFIER, serialize
```

### Comparing `negmas-0.9.7/negmas/mechanisms.py` & `negmas-0.9.8/negmas/mechanisms.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,53 +41,47 @@
 
 if TYPE_CHECKING:
     from negmas.outcomes.base_issue import Issue
     from negmas.outcomes.protocols import DiscreteOutcomeSpace
     from negmas.preferences import Preferences
     from negmas.preferences.base_ufun import BaseUtilityFunction
 
-__all__ = ["Mechanism", "MechanismRoundResult"]
+__all__ = ["Mechanism", "MechanismStepResult"]
 
 
 @define(frozen=True)
-class MechanismRoundResult:
-    """Represents the results of a negotiation round (step).
+class MechanismStepResult:
+    """
+    Represents the results of a negotiation step.
 
     This is what `round()` should return.
     """
 
     state: MechanismState
     """The returned state."""
     completed: bool = True
     """Whether the current round is completed or not."""
     broken: bool = False
     """True only if END_NEGOTIATION was selected by one agent."""
     timedout: bool = False
-    """True if a timeout occurred.
-
-    Usually not used
-    """
+    """True if a timeout occurred."""
     agreement: Outcome | None = None
-    """The agreement if any.
-
-    Allows for a single outcome or a collection of outcomes
-    """
+    """The agreement if any. Allows for a single outcome or a collection of outcomes."""
     error: bool = False
     """True if an error occurred in the mechanism."""
     error_details: str = ""
     """Error message."""
     waiting: bool = False
     """Whether to consider that the round is still running and call the round
     method again without increasing the step number."""
     exceptions: dict[str, list[str]] | None = None
     """A mapping from negotiator ID to a list of exceptions raised by that
     negotiator in this round."""
     times: dict[str, float] | None = None
-    """A mapping from negotiator ID to the time it consumed during this
-    round."""
+    """A mapping from negotiator ID to the time it consumed during this round."""
 
 
 # noinspection PyAttributeOutsideInit
 class Mechanism(NamedObject, EventSource, CheckpointMixin, ABC):
     """Base class for all negotiation Mechanisms.
 
     Override the `round` function of this class to implement a round of your mechanism
@@ -281,31 +275,34 @@
             max_cardinality=max_cardinality
             if max_cardinality is not None
             else float("inf"),
         )
         self.__discrete_outcomes = list(self.__discrete_os.enumerate_or_sample())
         return self.__discrete_outcomes
 
-    def random_outcomes(self, n: int = 1) -> list[Outcome]:
+    def random_outcomes(
+        self, n: int = 1, with_replacement: bool = False
+    ) -> list[Outcome]:
         """Returns random offers.
 
         Args:
               n: Number of outcomes to generate
+              with_replacement: If true, outcomes may be repeated
 
         Returns:
               A list of outcomes of at most n outcomes.
 
         Remarks:
 
                 - If the number of outcomes `n` cannot be satisfied, a smaller number will be returned
                 - Sampling is done without replacement (i.e. returned outcomes are unique).
         """
         return list(
             self.outcome_space.sample(
-                n, with_replacement=False, fail_if_not_enough=False
+                n, with_replacement=with_replacement, fail_if_not_enough=False
             )
         )
 
     @property
     def time(self) -> float:
         """Elapsed time since mechanism started in seconds.
 
@@ -763,19 +760,20 @@
         """Called before starting the negotiation.
 
         If it returns False then negotiation will end immediately
         """
         return True
 
     @abstractmethod
-    def __call__(self, state: MechanismState) -> MechanismRoundResult:
-        """Implements a single step of the mechanism. Override this!
+    def __call__(self, state: MechanismState) -> MechanismStepResult:
+        """
+        Implements a single step of the mechanism. Override this!
 
         Returns:
-            MechanismRoundResult giving whether the negotiation was broken or timedout and the agreement if any.
+            `MechanismStepResult` showing the result of the negotiation step
         """
         ...
 
     def step(self) -> MechanismState:
         """Runs a single step of the mechanism.
 
         Returns:
```

### Comparing `negmas-0.9.7/negmas/models/acceptance.py` & `negmas-0.9.8/negmas/models/acceptance.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/models/future.py` & `negmas-0.9.8/negmas/models/future.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/mt.py` & `negmas-0.9.8/negmas/mt.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Implements single text negotiation mechanisms
 """
 from __future__ import annotations
 
 import time
 from copy import deepcopy
 
-from attr import define, field
+from attrs import define, field
 
-from .mechanisms import Mechanism, MechanismRoundResult, MechanismState
+from .mechanisms import Mechanism, MechanismState, MechanismStepResult
 from .outcomes import Outcome
 
 __all__ = [
     "VetoMTMechanism",
 ]
 
 
@@ -83,35 +83,35 @@
 
         Returns:
             a new outcome or None to end the mechanism run
 
         """
         return self.random_outcomes(1)[0]
 
-    def __call__(self, state: MTState) -> MechanismRoundResult:
+    def __call__(self, state: MTState) -> MechanismStepResult:
         """Single round of the protocol"""
         for i, current_offer in enumerate(state.current_offers):
             new_offer = self.next_outcome(current_offer)
             responses = []
 
             for neg in self.negotiators:
                 strt = time.perf_counter()
                 responses.append(
                     neg.is_better(new_offer, current_offer, epsilon=self.epsilon)
                     is not False
                 )
                 if time.perf_counter() - strt > self.nmi.step_time_limit:
                     state.timedout = True
-                    return MechanismRoundResult(state)
+                    return MechanismStepResult(state)
 
             self.last_responses = responses
 
             if all(responses):
                 self._current_state.current_offers[i] = new_offer
 
-        return MechanismRoundResult(state)
+        return MechanismStepResult(state)
 
     def on_negotiation_end(self) -> None:
         """Used to pass the final offer for agreement between all negotiators"""
         self._agreement = self._current_state.current_offers  # type: ignore
 
         super().on_negotiation_end()
```

### Comparing `negmas-0.9.7/negmas/negotiators/components/component.py` & `negmas-0.9.8/negmas/negotiators/components/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from attr import define
+from attrs import define
 
 
 def __setattr__(self, name, value):
     pass
 
 
 def __delattr__(self, name):
```

### Comparing `negmas-0.9.7/negmas/negotiators/controlled.py` & `negmas-0.9.8/negmas/negotiators/controlled.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/negotiators/controller.py` & `negmas-0.9.8/negmas/negotiators/controller.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/negotiators/helpers.py` & `negmas-0.9.8/negmas/negotiators/helpers.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/negotiators/modular.py` & `negmas-0.9.8/negmas/negotiators/modular.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/negotiators/negotiator.py` & `negmas-0.9.8/negmas/negotiators/negotiator.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/negotiators/simple.py` & `negmas-0.9.8/negmas/negotiators/simple.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/__init__.py` & `negmas-0.9.8/negmas/outcomes/__init__.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/base_issue.py` & `negmas-0.9.8/negmas/outcomes/base_issue.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/callable_issue.py` & `negmas-0.9.8/negmas/outcomes/callable_issue.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/cardinal_issue.py` & `negmas-0.9.8/negmas/outcomes/cardinal_issue.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/categorical_issue.py` & `negmas-0.9.8/negmas/outcomes/categorical_issue.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/common.py` & `negmas-0.9.8/negmas/outcomes/common.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/contiguous_issue.py` & `negmas-0.9.8/negmas/outcomes/contiguous_issue.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/continuous_issue.py` & `negmas-0.9.8/negmas/outcomes/continuous_issue.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/infinite.py` & `negmas-0.9.8/negmas/outcomes/infinite.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/issue_ops.py` & `negmas-0.9.8/negmas/outcomes/issue_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -603,21 +603,23 @@
         - list[dict] A list of agent information dicts each contains 'agent', 'class', 'utility_file_name'
 
     Examples:
 
         >>> import pkg_resources
         >>> domain_file_name = pkg_resources.resource_filename('negmas'
         ...                                      , resource_name='tests/data/Laptop/Laptop-C-domain.xml')
-        >>> issues, _ = issues_from_xml_str(open(domain_file_name, 'r').read())
+        >>> with open(domain_file_name, 'r') as ff:
+        ...     issues, _ = issues_from_xml_str(ff.read())
         >>> print([_.cardinality for _ in issues])
         [3, 3, 3]
 
         >>> domain_file_name = pkg_resources.resource_filename('negmas'
         ...                              , resource_name='tests/data/fuzzyagent/single_issue_domain.xml')
-        >>> issues, _ = issues_from_xml_str(open(domain_file_name, 'r').read())
+        >>> with open(domain_file_name, 'r') as ff:
+        ...     issues, _ = issues_from_xml_str(ff.read())
         >>> len(issues)
         1
         >>> type(issues)
         <class 'tuple'>
         >>> str(issues[0]).split(': ')[-1]
         '(10.0, 40.0)'
         >>> print([_.cardinality for _ in issues])
```

### Comparing `negmas-0.9.7/negmas/outcomes/ordinal_issue.py` & `negmas-0.9.8/negmas/outcomes/ordinal_issue.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/outcome_ops.py` & `negmas-0.9.8/negmas/outcomes/outcome_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,29 +88,31 @@
 
     # if len(outcome) != len(issues):
     #     raise ValueError(
     #         f"Cannot convert {len(outcome)} valued outcome to a dict with {len(issues)} issues"
     #     )
 
     if isinstance(outcome, np.ndarray):
-        outcome = tuple(outcome.tolist())
+        outcome = tuple(outcome.tolist())  # type: ignore
 
     if isinstance(outcome, dict):
         names = {_.name if isinstance(_, Issue) else _ for _ in issues}
         for k in outcome.keys():
             if k not in names:
                 raise ValueError(
                     f"{k} not in the issue names ({names}). An invalid dict is given!!"
                 )
         return outcome
 
     return dict(zip([_ if isinstance(_, str) else _.name for _ in issues], outcome))
 
 
-def dict2outcome(d: dict[str, Any] | None, issues: list[str | Issue]) -> Outcome | None:
+def dict2outcome(
+    d: dict[str, Any] | None, issues: Iterable[str | Issue]
+) -> Outcome | None:
     """
     Converts the outcome to a tuple no matter what was its type
 
     Args:
         d: the dictionary to be converted
         issues: A list of issues or issue names (as strings) to order the tuple
```

### Comparing `negmas-0.9.7/negmas/outcomes/outcome_space.py` & `negmas-0.9.8/negmas/outcomes/outcome_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import random
 from functools import reduce
 from itertools import filterfalse
 from operator import mul
 from typing import TYPE_CHECKING, Callable, Iterable, Sequence, Union
 
-from attr import define, field
+from attrs import define, field
 
 from negmas.helpers import unique_name
 from negmas.helpers.types import get_full_type_name
 from negmas.outcomes.outcome_ops import (
     cast_value_types,
     outcome_is_valid,
     outcome_types_are_ok,
```

### Comparing `negmas-0.9.7/negmas/outcomes/protocols.py` & `negmas-0.9.8/negmas/outcomes/protocols.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/outcomes/range_issue.py` & `negmas-0.9.8/negmas/outcomes/range_issue.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/plots/util.py` & `negmas-0.9.8/negmas/plots/util.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/__init__.py` & `negmas-0.9.8/negmas/preferences/__init__.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/base.py` & `negmas-0.9.8/negmas/preferences/base.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/base_ufun.py` & `negmas-0.9.8/negmas/preferences/base_ufun.py`

 * *Files 1% similar despite different names*

```diff
@@ -546,21 +546,22 @@
         Examples:
 
             >>> from negmas.preferences import UtilityFunction
             >>> import pkg_resources
             >>> from negmas.inout import load_genius_domain
             >>> domain = load_genius_domain(pkg_resources.resource_filename('negmas'
             ...                             , resource_name='tests/data/Laptop/Laptop-C-domain.xml'))
-            >>> u, _ = UtilityFunction.from_xml_str(open(pkg_resources.resource_filename('negmas'
+            >>> with open(pkg_resources.resource_filename('negmas'
             ...                                      , resource_name='tests/data/Laptop/Laptop-C-prof1.xml')
-            ...                                      , 'r').read(), issues=domain.issues)
-
-            >>> u, _ = UtilityFunction.from_xml_str(open(pkg_resources.resource_filename('negmas'
+            ...                                      , 'r') as ff:
+            ...     u, _ = UtilityFunction.from_xml_str(ff.read(), issues=domain.issues)
+            >>> with open(pkg_resources.resource_filename('negmas'
             ...                                      , resource_name='tests/data/Laptop/Laptop-C-prof1.xml')
-            ...                                      , 'r').read(), issues=domain.issues)
+            ...                                      , 'r') as ff:
+            ...     u, _ = UtilityFunction.from_xml_str(ff.read(), issues=domain.issues)
             >>> assert abs(u(("Dell", "60 Gb", "19'' LCD",)) - 21.987727736172488) < 0.000001
             >>> assert abs(u(("HP", "80 Gb", "20'' LCD",)) - 22.68559475583014) < 0.000001
 
 
         """
         from negmas.preferences.complex import WeightedUtilityFunction
         from negmas.preferences.crisp.linear import (
@@ -958,15 +959,15 @@
         """
         Returns a numeric difference between the utility of the two given outcomes
         """
         return float(self(first)) - float(self(second))
 
     def __call__(self, offer: Outcome | None) -> Value:
         """
-        Calculate the utility_function value for a given outcome at the given negotiation state.
+        Calculate the utility for a given outcome at the given negotiation state.
 
         Args:
             offer: The offer to be evaluated.
 
 
         Remarks:
 
@@ -982,15 +983,33 @@
             The utility of the given outcome
         """
         if offer is None:
             return self.reserved_value  # type: ignore I know that concrete subclasses will be returning the correct type
         return self.eval(offer)
 
 
-class _General:
+class _FullyStatic:
+    """
+    Used internally to indicate that the ufun can **NEVER** change due to anything.
+    """
+
+    def is_session_dependent(self) -> bool:
+        return False
+
+    def is_volatile(self) -> bool:
+        return False
+
+    def is_state_dependent(self) -> bool:
+        return False
+
+    def is_stationary(self) -> bool:
+        return True
+
+
+class _ExtremelyDynamic:
     """
     Used internally to indicate that the ufun can change due to anything.
     """
 
     def is_session_dependent(self) -> bool:
         return True
```

### Comparing `negmas-0.9.7/negmas/preferences/complex.py` & `negmas-0.9.8/negmas/preferences/complex.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/crisp/const.py` & `negmas-0.9.8/negmas/preferences/crisp/const.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/crisp/linear.py` & `negmas-0.9.8/negmas/preferences/crisp/linear.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/crisp/mapping.py` & `negmas-0.9.8/negmas/preferences/crisp/mapping.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/crisp/nonlinear.py` & `negmas-0.9.8/negmas/preferences/crisp/nonlinear.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/crisp/random_ufun.py` & `negmas-0.9.8/negmas/preferences/crisp/random_ufun.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/crisp/rankonly_ufun.py` & `negmas-0.9.8/negmas/preferences/crisp/rankonly_ufun.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/crisp_ufun.py` & `negmas-0.9.8/negmas/preferences/crisp_ufun.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 import numpy as np
 
 from negmas import warnings
 from negmas.helpers.prob import Distribution, ScipyDistribution
 from negmas.outcomes import Issue, Outcome
 from negmas.outcomes.protocols import OutcomeSpace
 
-from .base_ufun import BaseUtilityFunction, _General
+from .base_ufun import BaseUtilityFunction, _ExtremelyDynamic
 
 __all__ = [
     "UtilityFunction",
 ]
 
 T = TypeVar("T", bound="UtilityFunction")
 
 
-class UtilityFunction(_General, BaseUtilityFunction):
+class UtilityFunction(_ExtremelyDynamic, BaseUtilityFunction):
     """Base for all crisp ufuns"""
 
     @abstractmethod
     def eval(self, offer: Outcome) -> float:
         ...
 
     def to_crisp(self) -> UtilityFunction:
```

### Comparing `negmas-0.9.7/negmas/preferences/discounted.py` & `negmas-0.9.8/negmas/preferences/discounted.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/inv_ufun.py` & `negmas-0.9.8/negmas/preferences/inv_ufun.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/mixins.py` & `negmas-0.9.8/negmas/preferences/mixins.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/ops.py` & `negmas-0.9.8/negmas/preferences/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 
 import itertools
 import math
 from math import sqrt
 from typing import TYPE_CHECKING, Iterable, Sequence, TypeVar
 
 import numpy as np
-from attr import define
+from attrs import define
 
 from negmas import warnings
 from negmas.helpers.numba_checks import jit  # type: ignore
 from negmas.outcomes import Issue, Outcome, discretize_and_enumerate_issues
 from negmas.outcomes.common import os_or_none
 from negmas.outcomes.issue_ops import enumerate_issues
 from negmas.outcomes.protocols import OutcomeSpace
 from negmas.preferences.crisp.mapping import MappingUtilityFunction
 
 if TYPE_CHECKING:
-
     from negmas.preferences.prob_ufun import ProbUtilityFunction
 
     from .base_ufun import BaseUtilityFunction
     from .crisp_ufun import UtilityFunction
     from .discounted import DiscountedUtilityFunction
 
     UFunType = TypeVar("UFunType", UtilityFunction, ProbUtilityFunction)
@@ -276,42 +275,49 @@
 
 def pareto_frontier_bf(
     points: np.ndarray | Iterable[Iterable[float]],
     eps=-1e-12,
     sort_by_welfare=True,
 ) -> np.ndarray:
     points = np.asarray(points, dtype=np.float32)
+    if len(points) < 1:
+        return points
     return _pareto_frontier_bf(points, eps, sort_by_welfare)
 
 
 @jit(nopython=True)
 def _pareto_frontier_bf(
-    points: np.ndarray | Iterable[Iterable[float]],
+    points: np.ndarray,
     eps=-1e-12,
     sort_by_welfare=True,
 ) -> np.ndarray:
-    """Finds the pareto-frontier of a set of points using brute-force. This is
+    """
+    Finds the pareto-frontier of a set of points using brute-force. This is
     extremely slow but is guaranteed to be correct.
 
     Args:
-        points: list of points
+        points: list of points each is a tuple of utility values for one outcome
         eps: A (usually negative) small number to treat as zero during calculations
         sort_by_welfare: If True, the results are sorted descindingly by total welfare
 
     Returns:
-        indices of pareto optimal outcomes
+        indices of Pareto optimal outcomes
     """
 
     frontier, indices = [], []
+    if len(points) < 1:
+        return np.empty(0, dtype=np.int64)
+    m = points.shape[1]
     for i, current in enumerate(points):
         for j, test in enumerate(points):
             if j == i:
                 continue
             has_better = has_worse = False
-            for a, b in zip(current, test, strict=True):
+            for k in range(m):
+                a, b = current[k], test[k]
                 if a > b:
                     has_better = True
                     continue
                 if a < b - eps:
                     has_worse = True
 
             if not has_better and has_worse:
@@ -420,15 +426,15 @@
     outcome_space: OutcomeSpace | None = None,
     issues: Sequence[Issue] | None = None,
     outcomes: Sequence[Outcome] | None = None,
     eps: float = 1e-12,
     subtract_reserved_value: bool = True,
 ) -> tuple[tuple[tuple[float, ...], int], ...]:
     """
-    Calculates the all Kalai bargaining solutions on the pareto frontier of a negotiation which is the most Egaliterian solution
+    Calculates the all Kalai bargaining solutions on the Pareto frontier of a negotiation which is the most Egaliterian solution
     ref:  Kalai, Ehud (1977). "Proportional solutions to bargaining situations: Intertemporal utility comparisons" (PDF). Econometrica. 45 (7): 1623–1630. doi:10.2307/1913954. JSTOR 1913954.
 
     Args:
         ufuns: A list of ufuns to use
         frontier: a list of tuples each giving the utility values at some outcome on the frontier (usually found by `pareto_frontier`) to search within
         outcome_space: The outcome-space to consider
         issues: The issues on which the ufun is defined (outcomes may be passed instead)
@@ -936,15 +942,15 @@
         issues: The set of issues (only used when outcomes is None)
         n_discretization: The number of items to discretize each real-dimension into
         sort_by_welfare: If True, the results are sorted descendingly by total welfare
         rational_only: If true, only rational outcomes can be members of the Pareto frontier.
         eps: resolution
 
     Returns:
-        Two lists of the same length. First list gives the utilities at pareto frontier points and second list gives their indices
+        Two lists of the same length. First list gives the utilities at Pareto frontier points and second list gives their indices
     """
 
     ufuns = tuple(ufuns)
     if issues:
         issues = tuple(issues)
     if outcomes:
         outcomes = tuple(outcomes)
```

### Comparing `negmas-0.9.7/negmas/preferences/preferences.py` & `negmas-0.9.8/negmas/preferences/preferences.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,16 +47,15 @@
         self.outcome_space = os_or_none(outcome_space, issues, outcomes)
         self.reserved_outcome = reserved_outcome  # type: ignore
         self._changes: list[PreferencesChange] = []
 
     @abstractmethod
     def is_volatile(self):
         """
-        Does the utiltiy of an outcome depend on factors outside the negotiation?
-
+        Does the utility of an outcome depend on factors outside the negotiation?
 
         Remarks:
             - A volatile preferences is one that can change even for the same mechanism state due to outside influence
         """
 
     @abstractmethod
     def is_not_worse(self, first: Outcome | None, second: Outcome | None) -> bool:
@@ -64,21 +63,21 @@
         Is `first` at least as good as `second`
         """
         ...
 
     @abstractmethod
     def is_session_dependent(self):
         """
-        Does the utiltiy of an outcome depend on the `NegotiatorMechanismInterface`?
+        Does the utility of an outcome depend on the `NegotiatorMechanismInterface`?
         """
 
     @abstractmethod
     def is_state_dependent(self):
         """
-        Does the utiltiy of an outcome depend on the negotiation state?
+        Does the utility of an outcome depend on the negotiation state?
         """
 
     def to_dict(self) -> dict[str, Any]:
         d = {PYTHON_CLASS_IDENTIFIER: get_full_type_name(type(self))}
         return dict(
             **d,
             outcome_space=serialize(self.outcome_space),
@@ -98,17 +97,34 @@
         return (
             not self.is_state_dependent()
             and not self.is_volatile()
             and not self.is_session_dependent()
         )
 
     def changes(self) -> list[PreferencesChange]:
+        """
+        Returns a list of changes to the preferences (if any) since last call.
+
+        Remarks:
+            - If the ufun is stationary, the return list will always be empty.
+            - If the ufun is not stationary, the ufun itself is responsible for saving the
+              changes in _changes whenever they happen.
+
+        """
         if self.is_stationary():
             return []
-        return [PreferencesChange()]
+        r = [_ for _ in self._changes]
+        self.reset_changes()
+        return r
+
+    def reset_changes(self) -> None:
+        """
+        Will be called whenever we need to reset changes.
+        """
+        self._changes = []
 
     @property
     def type(self) -> str:
         """Returns the utility_function type.
 
         Each class inheriting from this ``UtilityFunction`` class will have its own type. The default type is the empty
         string.
```

### Comparing `negmas-0.9.7/negmas/preferences/prob/independent.py` & `negmas-0.9.8/negmas/preferences/prob/independent.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/prob/locscale.py` & `negmas-0.9.8/negmas/preferences/prob/locscale.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/prob/mapping.py` & `negmas-0.9.8/negmas/preferences/prob/mapping.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/prob/random_ufun.py` & `negmas-0.9.8/negmas/preferences/prob/random_ufun.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/prob_ufun.py` & `negmas-0.9.8/negmas/preferences/prob_ufun.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 import numpy as np
 
 from negmas.helpers.numeric import get_one_float
 from negmas.helpers.prob import Distribution, Real, ScipyDistribution
 from negmas.outcomes import Outcome
 
-from .base_ufun import BaseUtilityFunction, _General
+from .base_ufun import BaseUtilityFunction, _ExtremelyDynamic
 
 __all__ = [
     "ProbUtilityFunction",
 ]
 
 
-class ProbUtilityFunction(_General, BaseUtilityFunction):
+class ProbUtilityFunction(_ExtremelyDynamic, BaseUtilityFunction):
     """A probablistic utility function. One that returns a probability distribution when called"""
 
     @abstractmethod
     def eval(self, offer: Outcome) -> Distribution:
         ...
 
     def to_prob(self) -> ProbUtilityFunction:
```

### Comparing `negmas-0.9.7/negmas/preferences/protocols.py` & `negmas-0.9.8/negmas/preferences/protocols.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/preferences/value_fun.py` & `negmas-0.9.8/negmas/preferences/value_fun.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import math
 from abc import ABC, abstractmethod
 from functools import lru_cache, reduce
 from math import cos, e, log, pow, sin
 from operator import add
 from typing import Any, Callable, Iterable
 
-from attr import asdict, define
+from attrs import asdict, define
 
 from negmas.helpers.misc import (
     monotonic_minmax,
     monotonic_multi_minmax,
     nonmonotonic_minmax,
     nonmonotonic_multi_minmax,
 )
```

### Comparing `negmas-0.9.7/negmas/protocols.py` & `negmas-0.9.8/negmas/protocols.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/sao/common.py` & `negmas-0.9.8/negmas/sao/common.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
 Common data-structures for supporting the Stacked Alternating Offers Protocol
 """
 from __future__ import annotations
 
-from collections import namedtuple
-from enum import Enum
 from functools import lru_cache
 from typing import TYPE_CHECKING
 
-from attr import define, field
+from attrs import define, field
 
 from negmas.common import NegotiatorMechanismInterface
 from negmas.gb.common import GBState, ResponseType
 
 if TYPE_CHECKING:
     from negmas.outcomes import Outcome
     from negmas.sao.negotiators.base import SAONegotiator
@@ -41,15 +39,15 @@
     current_proposer_agent: str | None = None
     n_acceptances: int = 0
     new_offers: list[tuple[str, Outcome | None]] = field(default=list)
     new_offerer_agents: list[str | None] = field(default=list)
     last_negotiator: str | None = None
 
 
-@define
+@define(frozen=True)
 class SAONMI(NegotiatorMechanismInterface):
     end_on_no_response: bool = True
 
 
 @lru_cache(1)
 def all_negotiator_types() -> list[SAONegotiator]:
     """
```

### Comparing `negmas-0.9.7/negmas/sao/components/models/ufun.py` & `negmas-0.9.8/negmas/sao/components/models/ufun.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from attr import define, field
+from attrs import define, field
 
 from negmas.preferences import RankOnlyUtilityFunction
 from negmas.preferences.base_ufun import BaseUtilityFunction
 from negmas.preferences.mixins import StationaryMixin
 
 from ..base import GBComponent
```

### Comparing `negmas-0.9.7/negmas/sao/controllers.py` & `negmas-0.9.8/negmas/sao/controllers.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,14 @@
             nmi  (NegotiatorMechanismInterface): The negotiation.
             state (MechanismState): The current state of the negotiation
             ufun (UtilityFunction): The ufun function to use before any discounting.
             role (str): role of the agent.
         """
 
     def propose(self, negotiator_id: str, state: MechanismState) -> Outcome | None:
-
         negotiator, _ = self._negotiators.get(negotiator_id, (None, None))
         if negotiator is None:
             raise ValueError(f"Unknown negotiator {negotiator_id}")
         return self.call(negotiator, "propose", state=state)
 
     def respond(
         self, negotiator_id: str, state: MechanismState, offer: Outcome, source: str
@@ -157,15 +156,14 @@
     """
 
     def __init__(self, *args, p_acceptance: float = 0.1, **kwargs):
         super().__init__(*args, **kwargs)
         self._p_acceptance = p_acceptance
 
     def propose(self, negotiator_id: str, state: MechanismState) -> Outcome | None:
-
         negotiator, cntxt = self._negotiators.get(negotiator_id, (None, None))
         if negotiator is None:
             raise ValueError(f"Unknown negotiator {negotiator_id}")
         if negotiator.nmi is None:
             return None
         return negotiator.nmi.random_outcomes(1)[0]
 
@@ -496,16 +494,18 @@
               defined for the controller if used (if any)
         """
         neg = self.negotiators[negotiator][0]
         if neg is None:
             return None
         if neg.nmi is None:
             return None
-        ufun = neg.ufun
-        if ufun is None and hasattr(self, "ufun"):
+        ufun = None
+        if self.has_ufun:
+            ufun = self.ufun
+        elif not self.has_ufun and hasattr(self, "ufun"):
             ufun = self.ufun
         if ufun is None:
             return None
         _, top_outcome = ufun.extreme_outcomes(outcome_space=neg.nmi.outcome_space)
         return top_outcome
 
     @abstractmethod
```

### Comparing `negmas-0.9.7/negmas/sao/mechanism.py` & `negmas-0.9.8/negmas/sao/mechanism.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 Implements Stacked Alternating Offers (SAO) mechanism.
 """
 from __future__ import annotations
 
 import functools
-import random
 import sys
 import time
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
 from negmas import warnings
 
 from ..common import TraceElement
 from ..events import Event
 from ..helpers import TimeoutCaller, TimeoutError, exception2str
-from ..mechanisms import Mechanism, MechanismRoundResult
+from ..mechanisms import Mechanism, MechanismStepResult
 from ..outcomes.common import Outcome
 from ..outcomes.outcome_ops import cast_value_types, outcome_types_are_ok
 from .common import ResponseType, SAOResponse, SAOState
 
 if TYPE_CHECKING:
     from negmas.preferences import Preferences
 
@@ -49,17 +48,14 @@
                         can be accessed by any negotiator through their AMI.
         max_cardinality: Maximum number or outcomes to use when disctetizing the outcome-space
         annotation: A key-value mapping to keep around. Accessible through the AMI but not used by the mechanism.
         end_on_no_response: End the negotiation if any negotiator returns NO_RESPONSE from `respond`/`counter` or returns
                             REJECT_OFFER then refuses to give an offer (by returning `None` from `proposee/`counter`).
         enable_callbacks: Enable callbacks like on_round_start, etc. Note that on_negotiation_end is always received
                           by the negotiators no matter what is the setting for this parameter.
-        avoid_ultimatum: If true, a proposal is taken from every agent in the first round then all of them are discarded
-                         except one (choose randomly) and the algorithm continues using this one. This prevents negotiators
-                         from knowing their order in the round.
         check_offers: If true, offers are checked to see if they are valid for the negotiation
                       outcome-space and if not the offer is considered None which is the same as
                       refusing to offer (NO_RESPONSE).
         enforce_issue_types: If True, the type of each issue is enforced depending on the value of `cast_offers`
         cast_offers: If true, each issue value is cast using the issue's type otherwise an incorrect type will be considered an invalid offer. See `check_offers`. Only
                      used if `enforce_issue_types`
         ignore_negotiator_exceptions: just silently ignore negotiator exceptions and consider them no-responses.
@@ -95,14 +91,20 @@
         allow_offering_just_rejected_outcome=True,
         name: str | None = None,
         max_wait: int = sys.maxsize,
         sync_calls: bool = False,
         initial_state: SAOState | None = None,
         **kwargs,
     ):
+        if avoid_ultimatum:
+            warnings.warn(
+                "Support for Avoid-Ultimatum will be removed soon. We will force avoid_ultimatum to False",
+                warnings.NegmasWarning,
+            )
+            avoid_ultimatum = False
         super().__init__(
             dynamic_entry=dynamic_entry,
             extra_callbacks=extra_callbacks,
             initial_state=SAOState() if not initial_state else initial_state,
             name=name,
             **kwargs,
         )
@@ -115,15 +117,14 @@
                 "You are passing no time_limit and no n_steps to an SAOMechanism. The mechanism may never finish!!",
                 warnings.NegmasInfiniteNegotiationWarning,
             )
         self._sync_calls = sync_calls
         self.params["end_on_no_response"] = end_on_no_response
         self.params["enable_callbacks"] = extra_callbacks
         self.params["sync_calls"] = sync_calls
-        self.params["avoid_ultimatum"] = avoid_ultimatum
         self.params["check_offers"] = check_offers
         self.params["offering_is_accepting"] = offering_is_accepting
         self.params["enforce_issue_types"] = enforce_issue_types
         self.params["cast_offers"] = cast_offers
         self.params[
             "allow_offering_just_rejected_outcome"
         ] = allow_offering_just_rejected_outcome
@@ -135,16 +136,14 @@
         self.check_offers = check_offers
         self._enforce_issue_types = enforce_issue_types
         self._cast_offers = cast_offers
 
         self._last_checked_negotiator = -1
         self._current_proposer = None
         self._frozen_neg_list = None
-        self._avoid_ultimatum = n_steps is not None and avoid_ultimatum
-        self._ultimatum_avoided = False
         self._no_responses = 0
         self._offering_is_accepting = offering_is_accepting
         self._n_waits = 0
         self._waiting_time: dict[str, float] = defaultdict(float)
         self._waiting_start: dict[str, float] = defaultdict(lambda: float("inf"))
         self._selected_first = 0
 
@@ -161,17 +160,21 @@
         added = super().add(negotiator, preferences=preferences, role=role, **kwargs)
         if (
             added
             and isinstance(negotiator, GeniusNegotiator)
             and self.nmi.time_limit is not None
             and self.nmi.time_limit != float("inf")
             and self.nmi.n_steps is not None
+            and self.nmi.n_steps != float("inf")
         ):
             warnings.warn(
-                f"{negotiator.id} of type {negotiator.__class__.__name__} is joining SAOMechanism which has a time_limit of {self.nmi.time_limit} seconds and a n_steps of {self.nmi.n_steps}. This agnet will only know about the time_limit and will not know about the n_steps!!!",
+                f"{negotiator.id} of type {negotiator.__class__.__name__} is joining "
+                f"SAOMechanism which has a time_limit of {self.nmi.time_limit} seconds "
+                f"and a n_steps of {self.nmi.n_steps}. This agnet will only know about the "
+                f"time_limit and will not know about the n_steps!!!",
                 warnings.NegmasStepAndTimeLimitWarning,
             )
         return added
 
     def set_sync_call(self, v: bool):
         self._sync_call = v
 
@@ -194,15 +197,15 @@
 
     def _stop_waiting(self, negotiator_id):
         self._waiting_time[negotiator_id] = 0.0
         self._waiting_start[negotiator_id] = float("inf")
         self._n_waits = 0
         self._frozen_neg_list = None
 
-    def __call__(self, state: SAOState) -> MechanismRoundResult:
+    def __call__(self, state: SAOState) -> MechanismStepResult:
         """implements a round of the Stacked Alternating Offers Protocol."""
         state = self._current_state
         if self._frozen_neg_list is None:
             state.new_offers = []
         negotiators: list[SAONegotiator] = self.negotiators
         n_negotiators = len(negotiators)
         # times = dict(zip([_.id for _ in negotiators], itertools.repeat(0.0)))
@@ -317,160 +320,17 @@
             proposer_indices.append(i)
         n_proposers = len(proposers)
         if n_proposers < 1:
             if not self.dynamic_entry:
                 state.broken = True
                 state.has_error = True
                 state.error_details = "No proposers and no dynamic entry"
-                return MechanismRoundResult(state, times=times, exceptions=exceptions)
-            else:
-                return MechanismRoundResult(state, times=times, exceptions=exceptions)
-        # if this is the first step (or no one has offered yet) which means that there is no _current_offer
-        if (
-            state.current_offer is None
-            and n_proposers > 1
-            and self._avoid_ultimatum
-            and not self._ultimatum_avoided
-        ):
-            if not self.dynamic_entry and not self.state.step == 0:
-                if self.end_negotiation_on_refusal_to_propose:
-                    state.broken = True
-                    return MechanismRoundResult(
-                        state,
-                        times=times,
-                        exceptions=exceptions,
-                    )
-            # if we are trying to avoid an ultimatum, we take an offer from everyone and ignore them but one.
-            # this way, the agent cannot know its order. For example, if we have two agents and 3 steps, this will
-            # be the situation after each step:
-            #
-            # Case 1: Assume that it ignored the offer from agent 1
-            # Step, Agent 0 calls received  , Agent 1 calls received    , relative time during last call
-            # 0   , counter(None)->offer1*  , counter(None) -> offer0   , 0/3
-            # 1   , counter(offer2)->offer3 , counter(offer1) -> offer2 , 1/3
-            # 2   , counter(offer4)->offer5 , counter(offer3) -> offer4 , 2/3
-            # 3   ,                         , counter(offer5)->offer6   , 3/3
-            #
-            # Case 2: Assume that it ignored the offer from agent 0
-            # Step, Agent 0 calls received  , Agent 1 calls received    , relative time during last call
-            # 0   , counter(None)->offer1   , counter(None) -> offer0*  , 0/3
-            # 1   , counter(offer0)->offer2 , counter(offer2) -> offer3 , 1/3
-            # 2   , counter(offer3)->offer4 , counter(offer4) -> offer5 , 2/3
-            # 3   , counter(offer5)->offer6 ,                           , 3/3
-            #
-            # in both cases, the agent cannot know whether its last offer going to be passed to the other agent
-            # (the ultimatum scenario) or not.
-            responses = []
-            responders = []
-            for i, neg in enumerate(proposers):
-                if not neg.capabilities.get("propose", False):
-                    continue
-                strt = time.perf_counter()
-                resp, has_exceptions = _safe_counter(neg, state=self.state, offer=None)
-                if has_exceptions:
-                    state.broken = True
-                    state.has_error = True
-                    state.error_details = str(exceptions[neg.id])
-                    return MechanismRoundResult(
-                        state,
-                        times=times,
-                        exceptions=exceptions,
-                    )
-                if resp is None:
-                    state.timedout = True
-                    return MechanismRoundResult(
-                        state,
-                        times=times,
-                        exceptions=exceptions,
-                    )
-                if resp.response != ResponseType.WAIT:
-                    self._waiting_time[neg.id] = 0.0
-                    self._waiting_start[neg.id] = float("inf")
-                    self._frozen_neg_list = None
-                else:
-                    self._waiting_start[neg.id] = min(self._waiting_start[neg.id], strt)
-                    self._waiting_time[neg.id] += (
-                        time.perf_counter() - self._waiting_start[neg.id]
-                    )
-                if (
-                    resp is None
-                    or time.perf_counter() - strt > self.nmi.step_time_limit
-                ):
-                    state.timedout = True
-                    return MechanismRoundResult(
-                        state,
-                        times=times,
-                        exceptions=exceptions,
-                    )
-                if resp.response == ResponseType.END_NEGOTIATION:
-                    state.broken = True
-                    return MechanismRoundResult(
-                        state,
-                        times=times,
-                        exceptions=exceptions,
-                    )
-                if resp.response in (ResponseType.NO_RESPONSE, ResponseType.WAIT):
-                    continue
-                if (
-                    resp.response == ResponseType.REJECT_OFFER
-                    and resp.outcome is None
-                    and self.end_negotiation_on_refusal_to_propose
-                ):
-                    continue
-                responses.append(resp)
-                responders.append(i)
-            if len(responses) < 1:
-                if not self.dynamic_entry:
-                    state.broken = True
-                    state.has_error = True
-                    state.error_details = "No proposers and no dynamic entry. This may happen if no negotiators responded to their first proposal request with an offer"
-                    return MechanismRoundResult(
-                        state,
-                        times=times,
-                        exceptions=exceptions,
-                    )
-                else:
-                    return MechanismRoundResult(
-                        state,
-                        times=times,
-                        exceptions=exceptions,
-                    )
-            # choose a random negotiator and set it as the current negotiator
-            self._ultimatum_avoided = True
-            selected = random.randint(0, len(responses) - 1)
-            resp = responses[selected]
-            neg = proposers[responders[selected]]
-            _first_proposer = proposer_indices[responders[selected]]
-            self._selected_first = _first_proposer
-            self._last_checked_negotiator = _first_proposer
-            state.current_offer = resp.outcome
-            state.new_offers.append((neg.id, resp.outcome))
-            self._current_proposer = neg
-            state.current_proposer = neg.id
-            state.n_acceptances = 1 if self._offering_is_accepting else 0
-            if self._last_checked_negotiator >= 0:
-                state.last_negotiator = self.negotiators[
-                    self._last_checked_negotiator
-                ].name
+                return MechanismStepResult(state, times=times, exceptions=exceptions)
             else:
-                state.last_negotiator = ""
-            (
-                self._current_proposer_agent,
-                state.new_offerer_agents,
-            ) = self._agent_info()
-
-            # current_proposer_agent=current_proposer_agent,
-            # new_offerer_agents=new_offerer_agents,
-            return MechanismRoundResult(
-                state,
-                times=times,
-                exceptions=exceptions,
-            )
-
-        # this is not the first round. A round will get n_negotiators responses
+                return MechanismStepResult(state, times=times, exceptions=exceptions)
         if self._frozen_neg_list is not None:
             ordered_indices = self._frozen_neg_list
         else:
             ordered_indices = [
                 (_ + self._last_checked_negotiator + 1) % n_negotiators
                 for _ in range(n_negotiators)
             ]
@@ -482,22 +342,22 @@
             resp, has_exceptions = _safe_counter(
                 neg, state=self.state, offer=state.current_offer
             )
             if has_exceptions:
                 state.broken = True
                 state.has_error = True
                 state.error_details = str(exceptions[neg.id])
-                return MechanismRoundResult(
+                return MechanismStepResult(
                     state,
                     times=times,
                     exceptions=exceptions,
                 )
             if resp is None:
                 state.timedout = True
-                return MechanismRoundResult(
+                return MechanismStepResult(
                     state,
                     times=times,
                     exceptions=exceptions,
                 )
             if resp.response == ResponseType.WAIT:
                 self._waiting_start[neg.id] = min(self._waiting_start[neg.id], strt)
                 self._waiting_time[neg.id] += time.perf_counter() - strt
@@ -515,15 +375,15 @@
                 self._frozen_neg_list = did_not_offer[indx:] + did_not_offer[:indx]
                 self._n_waits += 1
             else:
                 self._stop_waiting(neg.id)
 
             if resp is None or time.perf_counter() - strt > self.nmi.step_time_limit:
                 state.timedout = True
-                return MechanismRoundResult(
+                return MechanismStepResult(
                     state,
                     times=times,
                     exceptions=exceptions,
                 )
             if self._extra_callbacks:
                 if state.current_offer is not None:
                     for other in self.negotiators:
@@ -537,37 +397,37 @@
             if resp.response == ResponseType.NO_RESPONSE:
                 continue
             if resp.response == ResponseType.WAIT:
                 if self._n_waits > self._n_max_waits:
                     self._stop_waiting(neg.id)
                     state.timedout = True
                     state.waiting = False
-                    return MechanismRoundResult(
+                    return MechanismStepResult(
                         state,
                         times=times,
                         exceptions=exceptions,
                     )
                 state.waiting = True
-                return MechanismRoundResult(
+                return MechanismStepResult(
                     state,
                     times=times,
                     exceptions=exceptions,
                 )
             if resp.response == ResponseType.END_NEGOTIATION:
                 state.broken = True
-                return MechanismRoundResult(
+                return MechanismStepResult(
                     state,
                     times=times,
                     exceptions=exceptions,
                 )
             if resp.response == ResponseType.ACCEPT_OFFER:
                 state.n_acceptances += 1
                 if state.n_acceptances == n_negotiators:
                     state.agreement = self._current_state.current_offer
-                    return MechanismRoundResult(
+                    return MechanismStepResult(
                         state,
                         timedout=False,
                         agreement=state.current_offer,
                         times=times,
                         exceptions=exceptions,
                         broken=False,
                     )
@@ -580,15 +440,15 @@
                     proposal = None
                 if proposal is None:
                     if (
                         neg.capabilities.get("propose", True)
                         and self.end_negotiation_on_refusal_to_propose
                     ):
                         state.broken = True
-                        return MechanismRoundResult(
+                        return MechanismStepResult(
                             state,
                             times=times,
                             exceptions=exceptions,
                         )
                     state.n_acceptances = 0
                 else:
                     state.n_acceptances = 1 if self._offering_is_accepting else 0
@@ -610,15 +470,15 @@
                 else:
                     state.last_negotiator = ""
                 (
                     self._current_proposer_agent,
                     state.new_offerer_agents,
                 ) = self._agent_info()
 
-        return MechanismRoundResult(
+        return MechanismStepResult(
             state,
             times=times,
             exceptions=exceptions,
         )
 
     @property
     def full_trace(self) -> list[TraceElement]:
```

### Comparing `negmas-0.9.7/negmas/sao/negotiators/__init__.py` & `negmas-0.9.8/negmas/sao/negotiators/__init__.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/sao/negotiators/base.py` & `negmas-0.9.8/negmas/sao/negotiators/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,15 +108,16 @@
         return self.propose(state=state)
 
     @abstractmethod
     def propose(self, state: SAOState) -> Outcome | None:
         ...
 
     def respond(self, state: SAOState, offer: Outcome, source: str) -> ResponseType:
-        """Called to respond to an offer. This is the method that should be overriden to provide an acceptance strategy.
+        """
+        Called to respond to an offer. This is the method that should be overriden to provide an acceptance strategy.
 
         Args:
             state: a `SAOState` giving current state of the negotiation.
             offer: offer being tested
 
         Returns:
             ResponseType: The response to the offer
@@ -124,37 +125,41 @@
         Remarks:
             - The default implementation never ends the negotiation
             - The default implementation asks the negotiator to `propose`() and accepts the `offer` if its utility was
               at least as good as the offer that it would have proposed (and above the reserved value).
 
         """
         # Always reject offers that we do not know or if we have no kknown preferences
-        if offer is None or self.ufun is None:
+        if offer is None or self.preferences is None:
             return ResponseType.REJECT_OFFER
-        # find offer utility
-        offer_util = self.ufun(offer) if self.ufun else float("-inf")
+        offer_util = None
+        if self.has_ufun:
+            offer_util = self.ufun(offer)
         # if the offer is worse than the reserved value or its utility is less than that of the reserved outcome, reject it
-        if (self.reserved_value is not None and offer_util < self.reserved_value) or (
+        if (
+            self.reserved_value is not None
+            and offer_util is not None
+            and offer_util < self.reserved_value
+        ) or (
             self.reserved_outcome is not None
-            and self.ufun is not None
-            and offer_util < self.ufun(self.reserved_outcome)
+            and self.preferences.is_worse(offer, self.reserved_outcome)
         ):
             return ResponseType.REJECT_OFFER
         # find my last proposal (if any)
         utility = None
         if self._my_last_proposal_utility is not None:
             utility = self._my_last_proposal_utility
         # if I never proposed, find what would I have proposed at this state and its utility
         if utility is None:
             myoffer = self.propose_(state=state)
             if myoffer is None:
                 return ResponseType.NO_RESPONSE
             utility = self.ufun(myoffer)
         # accept only if I know what I would have proposed at this state (or the previous one) and it was worse than what I am about to proposed
-        if utility is not None and offer_util >= utility:
+        if utility is not None and offer_util is not None and offer_util >= utility:
             return ResponseType.ACCEPT_OFFER
         return ResponseType.REJECT_OFFER
 
     def respond_(self, state: SAOState, offer: Outcome, source: str) -> ResponseType:
         """The method to be called directly by the mechanism (through `counter` ) to respond to an offer.
 
         Args:
@@ -183,15 +188,18 @@
         if not state.running:
             warn(
                 f"{self.name} asked to respond to a negotiation that is not running:\n{state}"
             )
             return ResponseType.END_NEGOTIATION
         if self.__end_negotiation:
             return ResponseType.END_NEGOTIATION
-        return self.respond(state=state, offer=offer, source=source)
+        try:
+            return self.respond(state=state, offer=offer, source=source)
+        except TypeError:
+            return self.respond(state=state, offer=offer)
 
     def __call__(self, state: SAOState, offer: Outcome | None) -> SAOResponse:
         """
         Called by the mechanism to counter the offer. It just calls `respond_` and `propose_` as needed.
 
         Args:
             state: `SAOState` giving current state of the negotiation.
@@ -199,21 +207,27 @@
 
         Returns:
             Tuple[ResponseType, Outcome]: The response to the given offer with a counter offer if the response is REJECT
 
         """
         if self.__end_negotiation:
             return SAOResponse(ResponseType.END_NEGOTIATION, None)
-        if self.ufun is not None:
+        if self.has_ufun:
             changes = self.ufun.changes()
             if changes:
                 self.on_preferences_changed(changes)
         if offer is None:
             return SAOResponse(ResponseType.REJECT_OFFER, self.propose_(state=state))
-        response = self.respond_(
-            state=state,
-            offer=offer,
-            source=state.current_proposer if state.current_proposer else "",
-        )
+        try:
+            response = self.respond_(
+                state=state,
+                offer=offer,
+                source=state.current_proposer if state.current_proposer else "",
+            )
+        except TypeError:
+            response = self.respond_(
+                state=state,
+                offer=offer,
+            )
         if response != ResponseType.REJECT_OFFER:
             return SAOResponse(response, None)
         return SAOResponse(response, self.propose_(state=state))
```

### Comparing `negmas-0.9.7/negmas/sao/negotiators/controlled.py` & `negmas-0.9.8/negmas/sao/negotiators/controlled.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,18 @@
             return self._Negotiator__parent.propose(self.id, state)  # type: ignore
 
     def respond(
         self, state: MechanismState, offer: Outcome, source: str
     ) -> ResponseType:
         """Calls parent controller"""
         if self._Negotiator__parent:  # type: ignore
-            return self._Negotiator__parent.respond(self.id, state, offer, source)  # type: ignore
+            try:
+                return self._Negotiator__parent.respond(self.id, state, offer, source)  # type: ignore
+            except TypeError:
+                return self._Negotiator__parent.respond(self.id, state, offer)  # type: ignore
         return ResponseType.REJECT_OFFER
 
     # def _on_negotiation_start(self, state: MechanismState) -> None:
     #     """Calls parent controller"""
     #     if self._Negotiator__parent:  # type: ignore
     #         return self._Negotiator__parent._on_negotiation_start(self.id, state)  # type: ignore
```

### Comparing `negmas-0.9.7/negmas/scripts/app.py` & `negmas-0.9.8/negmas/scripts/app.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/scripts/negotiate.py` & `negmas-0.9.8/negmas/scripts/negotiate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from __future__ import annotations
 
+import sys
 from pathlib import Path
 from time import perf_counter
 
 import matplotlib
 import typer
 from matplotlib import functools
 from matplotlib import pyplot as plt
 from pandas.core.window.numba_ import Callable
 from rich import print
 from stringcase import titlecase
 
+from negmas.genius.ginfo import get_java_class
+from negmas.genius.negotiator import GeniusNegotiator
 from negmas.helpers import get_class
 from negmas.helpers.strings import camel_case, humanize_time, shortest_unique_names
 from negmas.helpers.types import get_full_type_name
 from negmas.inout import Scenario
 from negmas.mechanisms import Mechanism
 from negmas.negotiators.negotiator import Negotiator
 from negmas.preferences.ops import (
-    get_ranks,
     kalai_points,
     make_rank_ufun,
-    max_relative_welfare_points,
     max_welfare_points,
     nash_points,
     pareto_frontier,
 )
 
 app = typer.Typer()
 
+GENIUSMARKER = "genius"
+
 
 def get_screen_resolution() -> tuple[int, int]:
     from tkinter import Tk
 
     # creating tkinter window
     root = Tk()
     # getting screen's height in pixels
@@ -50,19 +53,40 @@
     if name.lower() == "gao":
         return get_class("negmas.gb.mechanisms.GAOMechanism")
     if "." not in name:
         name = f"negmas.{name}"
     return get_class(name)
 
 
+def get_genius_proper_class_name(s: str) -> str:
+    assert s.startswith(GENIUSMARKER)
+    return s.split(GENIUSMARKER)[-1]
+
+
 def create_adapter(adapter_type, negotiator_type, name):
     return adapter_type(name=name, base=negotiator_type(name=name))
 
 
+def make_genius_negotiator(*args, java_class_name: str, **kwargs):
+    return GeniusNegotiator(*args, **kwargs, java_class_name=java_class_name)
+
+
 def get_negotiator(name: str) -> type[Negotiator] | Callable[[str], Negotiator]:
+    if name.startswith(GENIUSMARKER):
+        for sp in (".", ":"):
+            x = sp.join(name.split(sp)[1:])
+            if x:
+                name = x
+                break
+        java_class = get_java_class(name)
+        if java_class is None:
+            raise ValueError(
+                f"Cannot find java class name for genius negotiatoar of type {name}"
+            )
+        return functools.partial(make_genius_negotiator, java_class_name=java_class)
     if "/" in name:
         adapter_name, _, negotiator_name = name.partition("/")
         adapter_type = get_adapter(adapter_name)
         negotiator_type = get_negotiator(negotiator_name)
         return functools.partial(create_adapter, adapter_type, negotiator_type)
     if "." not in name:
         if "_" in name:
@@ -121,14 +145,15 @@
         ["aspiration", "aspiration"],
         "--agent",
         "--negotiator",
         "-n",
         "-a",
         help="Negotiator (agent) type. To use an adapter type, put the adapter name first separated from the negotiator name by a slash (e.g. TAUAdapter/AspirationNegotiator)",
     ),
+    path: list[Path] = list(),
     reserved: list[float] = typer.Option(None, "--reserved", "-r"),
     normalize: bool = True,
     steps: int = typer.Option(None, "--steps", "-s"),  # type: ignore
     timelimit: int = typer.Option(None, "--time", "--timelimit", "-t"),  # type: ignore
     plot: bool = True,
     plot_path: Path = None,  # type: ignore
     verbose: bool = typer.Option(False, "--verbose", "-v"),
@@ -148,14 +173,16 @@
     show_end_reason: bool = True,
     show_annotations: bool = False,
     show_reserved: bool = True,
     show_total_time: bool = True,
     show_relative_time: bool = True,
     show_n_steps: bool = True,
 ):
+    for p in path:
+        sys.path.append(str(p))
     if reserved:
         assert len(reserved) == len(negotiators), f"{reserved=} but {negotiators=}"
     negotiator_names = shortest_unique_names(negotiators)
     steps: int | float
     timelimit: int | float
     if steps is None:
         steps = float("inf")
```

### Comparing `negmas-0.9.7/negmas/scripts/vendor/quick/quick.py` & `negmas-0.9.8/negmas/scripts/vendor/quick/quick.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/serialization.py` & `negmas-0.9.8/negmas/serialization.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/__init__.py` & `negmas-0.9.8/negmas/situated/__init__.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/adapter.py` & `negmas-0.9.8/negmas/situated/adapter.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/agent.py` & `negmas-0.9.8/negmas/situated/agent.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/awi.py` & `negmas-0.9.8/negmas/situated/awi.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/breaches.py` & `negmas-0.9.8/negmas/situated/breaches.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import uuid
 from enum import Enum
 
-from attr import define, field
+from attrs import define, field
 
 from .contract import Contract
 
 __all__ = ["BreachProcessing", "Breach"]
 
 
 class BreachProcessing(Enum):
```

### Comparing `negmas-0.9.7/negmas/situated/bulletinboard.py` & `negmas-0.9.8/negmas/situated/bulletinboard.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/common.py` & `negmas-0.9.8/negmas/situated/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from collections import namedtuple
 from enum import Enum
 from typing import TYPE_CHECKING, Any
 
-from attr import define, field
+from attrs import define, field
 
 if TYPE_CHECKING:
     from negmas.mechanisms import Mechanism
     from negmas.outcomes import Issue
 
     from .agent import Agent
```

### Comparing `negmas-0.9.7/negmas/situated/contract.py` & `negmas-0.9.8/negmas/situated/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import uuid
 from typing import TYPE_CHECKING, Any
 
-from attr import define, field
+from attrs import define, field
 
 if TYPE_CHECKING:
     from negmas.common import MechanismState
     from negmas.outcomes import Issue
 
 __all__ = ["Contract"]
```

### Comparing `negmas-0.9.7/negmas/situated/entity.py` & `negmas-0.9.8/negmas/situated/entity.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/helpers.py` & `negmas-0.9.8/negmas/situated/helpers.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/mechanismfactory.py` & `negmas-0.9.8/negmas/situated/mechanismfactory.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/mixins.py` & `negmas-0.9.8/negmas/situated/mixins.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/monitors.py` & `negmas-0.9.8/negmas/situated/monitors.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/neg.py` & `negmas-0.9.8/negmas/situated/neg.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/save.py` & `negmas-0.9.8/negmas/situated/save.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/simple.py` & `negmas-0.9.8/negmas/situated/simple.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/situated/world.py` & `negmas-0.9.8/negmas/situated/world.py`

 * *Files 0% similar despite different names*

```diff
@@ -818,35 +818,35 @@
         old_stdout = sys.stdout  # backup current stdout
         if self.disable_agent_printing:
             sys.stdout = open(os.devnull, "w")
         _strt = time.perf_counter()
         try:
             result = method(*args, **kwargs)
             _end = time.perf_counter()
-            if self.disable_agent_printing:
-                sys.stdout = old_stdout  # reset old stdout
             self.times[agent.id] = _end - _strt
             return result
         except Exception as e:
             _end = time.perf_counter()
-            if self.disable_agent_printing:
-                sys.stdout = old_stdout  # reset old stdout
             self.times[agent.id] = _end - _strt
             self.agent_exceptions[agent.id].append(
                 (self._current_step, exception2str())
             )
             self.on_exception(agent, e)
             if not self.ignore_agent_exception:
                 raise e
             exc_type, exc_value, exc_traceback = sys.exc_info()
             self.logerror(
                 f"Entity exception @{agent.id}: "
                 f"{traceback.format_tb(exc_traceback)}",
                 Event("entity-exception", dict(exception=e)),
             )
+        finally:
+            if self.disable_agent_printing:
+                sys.stdout.close()
+                sys.stdout = old_stdout  # reset old stdout
 
     def _add_edges(
         self,
         src: Agent | str,
         dst: list[Agent | str],
         target: dict[int, dict[tuple[Agent, Agent], list[dict[str, Any]]]],
         bi=False,
```

### Comparing `negmas-0.9.7/negmas/st.py` & `negmas-0.9.8/negmas/st.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from __future__ import annotations
 
 import math
 import random
 import time
 from copy import deepcopy
 
-from attr import define
+from attrs import define
 
-from .mechanisms import Mechanism, MechanismRoundResult, MechanismState
+from .mechanisms import Mechanism, MechanismState, MechanismStepResult
 from .outcomes import Outcome
 
 __all__ = ["VetoSTMechanism", "HillClimbingSTMechanism"]
 
 
 @define
 class STState(MechanismState):
@@ -79,33 +79,33 @@
 
         Returns:
             a new outcome or None to end the mechanism run
 
         """
         return self.random_outcomes(1)[0]
 
-    def __call__(self, state: STState) -> MechanismRoundResult:
+    def __call__(self, state: STState) -> MechanismStepResult:
         """Single round of the protocol"""
 
         new_offer = self.next_outcome(state.current_offer)
         responses = []
 
         for neg in self.negotiators:
             strt = time.perf_counter()
             responses.append(neg.is_better(new_offer, state.current_offer) is not False)
             if time.perf_counter() - strt > self.nmi.step_time_limit:
                 state.timedout = True
-                return MechanismRoundResult(state)
+                return MechanismStepResult(state)
 
         self.last_responses = responses
         state.new_offer = new_offer
         if all(responses):
             state.current_offer = new_offer
 
-        return MechanismRoundResult(state)
+        return MechanismStepResult(state)
 
     def on_negotiation_end(self) -> None:
         """Used to pass the final offer for agreement between all negotiators"""
 
         state: STState = self._current_state  # type: ignore
         if state.current_offer is not None and all(
             neg.is_acceptable_as_agreement(state.current_offer)
@@ -330,33 +330,33 @@
 
         if len(self.possible_offers) == 0:
             return None
         return self.possible_offers.pop(
             random.randint(0, len(self.possible_offers)) - 1
         )
 
-    def __call__(self, state: STState) -> MechanismRoundResult:
+    def __call__(self, state: STState) -> MechanismStepResult:
         """Single round of the protocol"""
 
         new_offer = self.next_outcome(state.current_offer)
         if new_offer is None:
             state.agreement = (state.current_offer,)
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
 
         responses = []
         for neg in self.negotiators:
             strt = time.perf_counter()
             responses.append(neg.is_better(new_offer, state.current_offer) is not False)
             if time.perf_counter() - strt > self.nmi.step_time_limit:
-                return MechanismRoundResult(state)
+                return MechanismStepResult(state)
 
         self.last_responses = responses
 
         if all(responses):
             state.current_offer = new_offer
             self.possible_offers = self.neighbors(state.current_offer)
 
-        return MechanismRoundResult(state)
+        return MechanismStepResult(state)
 
     @property
     def current_offer(self):
         return self._current_state.current_offer
```

### Comparing `negmas-0.9.7/negmas/tests/fixtures.py` & `negmas-0.9.8/negmas/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/tests/test_ga.py` & `negmas-0.9.8/negmas/tests/test_ga.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/tests/test_genius.py` & `negmas-0.9.8/negmas/tests/test_genius.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/tests/test_helpers.py` & `negmas-0.9.8/negmas/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/tests/test_inout.py` & `negmas-0.9.8/negmas/tests/test_inout.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/tests/test_integration.py` & `negmas-0.9.8/negmas/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/tests/test_issue.py` & `negmas-0.9.8/negmas/tests/test_issue.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/tests/test_negotiators.py` & `negmas-0.9.8/negmas/tests/test_negotiators.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         dict(zip(outcomes, np.linspace(0.0, 1.0, len(outcomes)).tolist())),
         outcomes=outcomes,
     )
     u2 = MappingUtilityFunction(
         dict(zip(outcomes, (1 - np.linspace(0.0, 1.0, len(outcomes))).tolist())),
         outcomes=outcomes,
     )
-    neg = SAOMechanism(outcomes=outcomes, n_steps=100, avoid_ultimatum=False)
+    neg = SAOMechanism(outcomes=outcomes, n_steps=100)
     neg.add(a1, preferences=u1)
     neg.add(a2, preferences=u2)
     neg.run()
     a1offers = neg.negotiator_offers(a1.id)
     a2offers = neg.negotiator_offers(a2.id)
     # print(a1offers)
     # print(a2offers)
@@ -138,15 +138,15 @@
 
 
 def test_top_only_negotiator():
     outcomes = [(_,) for _ in range(10)]
     a1 = ToughNegotiator(name="a1")
     a2 = ToughNegotiator(name="a2")
     u1 = 22.0 - np.linspace(0.0, 22.0, len(outcomes))
-    neg = SAOMechanism(outcomes=outcomes, n_steps=10, avoid_ultimatum=False)
+    neg = SAOMechanism(outcomes=outcomes, n_steps=10)
     neg.add(
         a1,
         preferences=MappingUtilityFunction(
             dict(zip(outcomes, u1)), outcome_space=neg.outcome_space
         ),
     )
     neg.add(
@@ -166,15 +166,15 @@
 
 
 def test_tft_propose():
     outcomes = [(_,) for _ in range(10)]
     a1 = NaiveTitForTatNegotiator(name="a1", initial_concession="min")
     a2 = ToughNegotiator(name="a2")
     u1 = 22.0 - np.linspace(0.0, 22.0, len(outcomes))
-    neg = SAOMechanism(outcomes=outcomes, n_steps=10, avoid_ultimatum=False)
+    neg = SAOMechanism(outcomes=outcomes, n_steps=10)
     neg.add(
         a1,
         preferences=MappingUtilityFunction(
             dict(zip(outcomes, u1)), outcome_space=neg.outcome_space
         ),
     )
     neg.add(
@@ -190,15 +190,15 @@
     neg.step()
     proposal = neg.negotiator_offers(neg.negotiators[0].id)[1]
     assert proposal == (1,), "Proposes second second if min concession is set"
 
     a1 = NaiveTitForTatNegotiator(name="a1")
     a2 = ToughNegotiator(name="a1")
     u1 = [50.0] * 3 + (22 - np.linspace(10.0, 22.0, len(outcomes) - 3)).tolist()
-    neg = SAOMechanism(outcomes=outcomes, n_steps=10, avoid_ultimatum=False)
+    neg = SAOMechanism(outcomes=outcomes, n_steps=10)
     neg.add(
         a1,
         preferences=MappingUtilityFunction(lambda x: u1[x[0]], outcomes=outcomes),
     )
     neg.add(
         a2,
         preferences=MappingUtilityFunction(lambda x: 22 - u1[x[0]], outcomes=outcomes),
@@ -225,17 +225,15 @@
         dict(zip(outcomes, np.linspace(0.0, 1.0, len(outcomes)).tolist())),
         outcomes=outcomes,
     )
     u2 = MappingUtilityFunction(
         dict(zip(outcomes, (1 - np.linspace(0.0, 1.0, len(outcomes))).tolist())),
         outcomes=outcomes,
     )
-    neg = SAOMechanism(
-        outcomes=outcomes, n_steps=20, avoid_ultimatum=False, time_limit=None
-    )
+    neg = SAOMechanism(outcomes=outcomes, n_steps=20, time_limit=None)
     neg.add(a1, preferences=u1)
     neg.add(a2, preferences=u2)
     neg.run()
     a1offers = neg.negotiator_offers(a1.id)
     a2offers = neg.negotiator_offers(a2.id)
     assert a1offers[0] == (9,), f"{neg.plot()}{plt.show()}{neg.extended_trace}"
     # assert a2offers[0] == (0,)
```

### Comparing `negmas-0.9.7/negmas/tests/test_outcomes.py` & `negmas-0.9.8/negmas/tests/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/tests/test_preferences.py` & `negmas-0.9.8/tests/core/test_preferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -592,29 +592,29 @@
     d = u.to_dict()
     u2 = utype.from_dict(d)
     for o in enumerate_issues(issues):
         assert abs(u(o) - u2(o)) < 1e-3
 
 
 def test_inverse_genius_domain():
-    issues, _ = issues_from_xml_str(
-        open(
-            pkg_resources.resource_filename(
-                "negmas", resource_name="tests/data/Laptop/Laptop-C-domain.xml"
-            ),
-        ).read(),
-    )
-    u, _ = UtilityFunction.from_xml_str(
-        open(
-            pkg_resources.resource_filename(
-                "negmas", resource_name="tests/data/Laptop/Laptop-C-prof1.xml"
-            ),
-        ).read(),
-        issues=issues,
-    )
+    with open(
+        pkg_resources.resource_filename(
+            "negmas", resource_name="tests/data/Laptop/Laptop-C-domain.xml"
+        ),
+    ) as ff:
+        issues, _ = issues_from_xml_str(ff.read())
+    with open(
+        pkg_resources.resource_filename(
+            "negmas", resource_name="tests/data/Laptop/Laptop-C-prof1.xml"
+        ),
+    ) as ff:
+        u, _ = UtilityFunction.from_xml_str(
+            ff.read(),
+            issues=issues,
+        )
     assert u is not None
     inv = PresortingInverseUtilityFunction(u)
     inv.init()
     for i in range(100):
         v = u(inv.one_in((i / 100.0, i / 100.0), normalized=True))
         assert v - 1e-3 <= v <= v + 0.1
 
@@ -728,65 +728,58 @@
         relative2 = _relative_fraction(u2)
         assert (
             np.abs(relative1 - relative2).max() < 1e-3
         ), f"One side normalization should not change the result of dividing outcomes\n{u1}\n{u2}"
 
 
 def test_normalization():
-    os = CartesianOutcomeSpace.from_xml_str(
-        open(
-            pkg_resources.resource_filename(
-                "negmas", resource_name="tests/data/Laptop/Laptop-C-domain.xml"
-            ),
-        ).read(),
-    )
+    with open(
+        pkg_resources.resource_filename(
+            "negmas", resource_name="tests/data/Laptop/Laptop-C-domain.xml"
+        ),
+    ) as ff:
+        os = CartesianOutcomeSpace.from_xml_str(ff.read())
     issues = os.issues
     outcomes = list(os.enumerate())
-    u, _ = UtilityFunction.from_xml_str(
-        open(
-            pkg_resources.resource_filename(
-                "negmas", resource_name="tests/data/Laptop/Laptop-C-prof1.xml"
-            ),
-        ).read(),
-        issues=issues,
-    )
+    with open(
+        pkg_resources.resource_filename(
+            "negmas", resource_name="tests/data/Laptop/Laptop-C-prof1.xml"
+        ),
+    ) as ff:
+        u, _ = UtilityFunction.from_xml_str(ff.read(), issues=issues)
     assert abs(u(("Dell", "60 Gb", "19'' LCD")) - 21.987727736172488) < 0.000001
     assert abs(u(("HP", "80 Gb", "20'' LCD")) - 22.68559475583014) < 0.000001
     utils = [u(_) for _ in outcomes]
     max_util, min_util = max(utils), min(utils)
     gt_range = dict(
         zip(outcomes, [(_ - min_util) / (max_util - min_util) for _ in utils])
     )
     gt_max = dict(zip(outcomes, [_ / max_util for _ in utils]))
 
-    u, _ = UtilityFunction.from_xml_str(
-        open(
-            pkg_resources.resource_filename(
-                "negmas", resource_name="tests/data/Laptop/Laptop-C-prof1.xml"
-            ),
-        ).read(),
-        issues=issues,
-    )
+    with open(
+        pkg_resources.resource_filename(
+            "negmas", resource_name="tests/data/Laptop/Laptop-C-prof1.xml"
+        ),
+    ) as ff:
+        u, _ = UtilityFunction.from_xml_str(ff.read(), issues=issues)
     u = normalize(u, to=(0.0, 1.0))
     utils = [u(_) for _ in outcomes]
     max_util, min_util = max(utils), min(utils)
     assert abs(max_util - 1.0) < 0.001
     assert abs(min_util) < 0.001
 
     for k, v in gt_range.items():
         assert abs(v - u(k)) < 1e-3, f"Failed for {k} got {(u(k))} expected {v}"
 
-    u, _ = UtilityFunction.from_xml_str(
-        open(
-            pkg_resources.resource_filename(
-                "negmas", resource_name="tests/data/Laptop/Laptop-C-prof1.xml"
-            ),
-        ).read(),
-        issues=issues,
-    )
+    with open(
+        pkg_resources.resource_filename(
+            "negmas", resource_name="tests/data/Laptop/Laptop-C-prof1.xml"
+        ),
+    ) as ff:
+        u, _ = UtilityFunction.from_xml_str(ff.read(), issues=issues)
     u = scale_max(u, 1.0)
     utils = [u(_) for _ in outcomes]
     max_util, min_util = max(utils), min(utils)
     assert abs(max_util - 1.0) < 0.001
 
     for k, v in gt_max.items():
         assert abs(v - u(k)) < 1e-3, f"Failed for {k} got {(u(k))} expected {v}"
```

### Comparing `negmas-0.9.7/negmas/tests/test_protocols.py` & `negmas-0.9.8/negmas/tests/test_protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 import pytest
 
 from negmas import (
     LimitedOutcomesAcceptor,
     LimitedOutcomesNegotiator,
     MappingUtilityFunction,
     Mechanism,
-    MechanismRoundResult,
+    MechanismStepResult,
     RandomNegotiator,
     SAOMechanism,
 )
 
 random.seed(0)
 
 
 class MyMechanism(Mechanism):
     def __init__(self, dynamic_entry=True, **kwargs):
         super().__init__(outcomes=20, n_steps=10, dynamic_entry=dynamic_entry, **kwargs)
         self.current = 0
 
-    def __call__(self, state) -> MechanismRoundResult:
+    def __call__(self, state) -> MechanismStepResult:
         # r = random.random()
         # if r > 1.0 / self.n_steps:
         #    return None, False, None
         self.current += 1
         if self.current < 6:
-            return MechanismRoundResult(state)
+            return MechanismStepResult(state)
         state.agreement = self.random_outcomes(1)[0]
-        return MechanismRoundResult(state)
+        return MechanismStepResult(state)
 
 
 @pytest.fixture
 def mechanism():
     return MyMechanism()
 
 
@@ -288,15 +288,15 @@
     neg.run()
     assert neg.agreement is not None
 
 
 def test_same_utility_leads_to_agreement():
     n_outcomes, n_steps = 10, 10
     accepted = [(2,), (3,), (4,), (5,)]
-    neg = SAOMechanism(outcomes=n_outcomes, n_steps=n_steps, avoid_ultimatum=False)
+    neg = SAOMechanism(outcomes=n_outcomes, n_steps=n_steps)
     opponent = LimitedOutcomesNegotiator(
         acceptable_outcomes=accepted,
         acceptance_probabilities=[1.0] * len(accepted),
     )
     acceptor = LimitedOutcomesAcceptor(
         acceptable_outcomes=accepted,
         acceptance_probabilities=[1.0] * len(accepted),
```

### Comparing `negmas-0.9.7/negmas/tests/test_situated.py` & `negmas-0.9.8/negmas/tests/test_situated.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Any, Callable, Collection
 
 import hypothesis.strategies as st
 import pytest
-from attr import asdict
+from attrs import asdict
 from hypothesis import HealthCheck, given, settings
 
 from negmas import (
     AspirationNegotiator,
     Issue,
     MappingUtilityFunction,
     MechanismState,
```

### Comparing `negmas-0.9.7/negmas/tests/test_st.py` & `negmas-0.9.8/negmas/tests/test_st.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/tests/test_tau.py` & `negmas-0.9.8/tests/core/test_tau.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 import time
 from pathlib import Path
 from typing import Iterable
 
 import hypothesis.strategies as st
 import pkg_resources
 import pytest
-from hypothesis import Verbosity, example, given, settings
+from hypothesis import Verbosity, given, settings
 from matplotlib.axes import itertools
 
 from negmas.gb.evaluators.tau import INFINITE
 from negmas.gb.mechanisms.mechanisms import GAOMechanism, TAUMechanism
 from negmas.gb.negotiators.cab import CABNegotiator, CANNegotiator, CARNegotiator
 from negmas.gb.negotiators.timebased import AspirationNegotiator
-from negmas.gb.negotiators.titfortat import NaiveTitForTatNegotiator
 from negmas.gb.negotiators.war import WABNegotiator, WANNegotiator, WARNegotiator
-from negmas.genius.gnegotiators import AgentK, Atlas3, NiceTitForTat
 from negmas.inout import Scenario
 from negmas.mechanisms import Mechanism
 from negmas.outcomes.base_issue import make_issue
 from negmas.outcomes.categorical_issue import CategoricalIssue
 from negmas.outcomes.common import Outcome
 from negmas.outcomes.outcome_space import DiscreteCartesianOutcomeSpace, make_os
 from negmas.preferences.crisp.linear import LinearAdditiveUtilityFunction as LU
@@ -35,18 +33,14 @@
 SHOW_ALL_PLOTS = False
 FORCE_PLOT = False
 SHOW_HISTORY = False
 SHOW_ALL_HISTORIES = False
 FORCE_HISTORY = False
 SAONEGOTIATORS = [
     AspirationNegotiator,
-    # NiceTitForTat,
-    # Atlas3,
-    # AgentK,
-    # NaiveTitForTatNegotiator,
 ]
 NEGOTIATORS = [
     WARNegotiator,
     CANNegotiator,
     CARNegotiator,
     WANNegotiator,
     CABNegotiator,
@@ -365,15 +359,15 @@
     for i, (x, y) in enumerate(limits):
         if y is None:
             limits[i] = (x, mxs[i])
     x1, x2 = limits[0]
     y1, y2 = limits[1]
 
     outcomes = list(os.enumerate())
-    _, frontier = pareto_frontier(ufuns, outcomes)
+    _, frontier = pareto_frontier(list(ufuns), outcomes)
     frontier = set(frontier)
 
     accepted: list[Outcome] = []
     for outcome in outcomes:
         if outcome in frontier:
             accepted.append(outcome)
             continue
@@ -458,28 +452,14 @@
         normalized=True,
         seller_reserved=0.1,
         buyer_reserved=0.1,
         force_plot=FORCE_PLOT,
     )
 
 
-@pytest.mark.skipif(not NEGMAS_RUN_GENIUS, reason="Skipping genius tests")
-def test_buyer_seller_gao_easy_genius():
-    run_buyer_seller(
-        Atlas3,
-        Atlas3,
-        normalized=True,
-        seller_reserved=0.1,
-        buyer_reserved=0.1,
-        force_plot=FORCE_PLOT,
-        mechanism_type=GAOMechanism,
-        do_asserts=False,
-    )
-
-
 def test_buyer_seller_gao_easy():
     run_buyer_seller(
         AspirationNegotiator,
         AspirationNegotiator,
         normalized=True,
         seller_reserved=0.1,
         buyer_reserved=0.1,
@@ -498,28 +478,14 @@
         buyer_reserved=0.6,
         force_plot=FORCE_PLOT,
         mechanism_type=GAOMechanism,
         do_asserts=False,
     )
 
 
-@pytest.mark.skipif(not NEGMAS_RUN_GENIUS, reason="Skipping genius tests")
-def test_buyer_seller_sao_genius():
-    run_buyer_seller(
-        Atlas3,
-        Atlas3,
-        normalized=True,
-        seller_reserved=0.5,
-        buyer_reserved=0.6,
-        force_plot=FORCE_PLOT,
-        mechanism_type=SAOMechanism,
-        do_asserts=False,
-    )
-
-
 @pytest.mark.parametrize(
     ["neg1", "neg2"], list(itertools.product(NEGOTIATORS, NEGOTIATORS))
 )
 def test_buyer_seller_alphainf(neg1, neg2):
     run_buyer_seller(
         neg1,
         neg2,
@@ -613,26 +579,30 @@
         single_issue=True,
         remove_under=False,
     )
 
 
 @pytest.mark.skipif(not NEGMAS_RUN_GENIUS, reason="Skipping genius tests")
 def test_anac_scenario_example_genius2_single():
+    from negmas.genius import Atlas3
+
     run_anac_example(
         Atlas3,
         Atlas3,
         mechanism_type=GAOMechanism,
         force_plot=FORCE_PLOT,
         single_issue=True,
         remove_under=False,
     )
 
 
 @pytest.mark.skipif(not NEGMAS_RUN_GENIUS, reason="Skipping genius tests")
 def test_anac_scenario_example_genius_single():
+    from negmas.genius import Atlas3
+
     run_anac_example(
         Atlas3,
         Atlas3,
         mechanism_type=SAOMechanism,
         force_plot=FORCE_PLOT,
         single_issue=True,
         remove_under=False,
@@ -653,14 +623,16 @@
         mechanism_type=GAOMechanism,
         force_plot=FORCE_PLOT,
     )
 
 
 @pytest.mark.skipif(not NEGMAS_RUN_GENIUS, reason="Skipping genius tests")
 def test_anac_scenario_example_genius():
+    from negmas.genius import Atlas3
+
     run_anac_example(
         Atlas3,
         Atlas3,
         mechanism_type=SAOMechanism,
         force_plot=FORCE_PLOT,
     )
 
@@ -674,14 +646,16 @@
         neg2,
         force_plot=FORCE_PLOT,
     )
 
 
 @pytest.mark.skipif(not NEGMAS_RUN_GENIUS, reason="Skipping genius tests")
 def test_adversarial_case_gao_easy_genius():
+    from negmas.genius import Atlas3
+
     run_adversarial_case(
         Atlas3,
         Atlas3,
         force_plot=FORCE_PLOT,
         mechanism_type=GAOMechanism,
         do_asserts=False,
     )
@@ -765,7 +739,39 @@
     ufuns = [U1.random(os, reserved_value=0.0), U2.random(os, reserved_value=0.0)]
     negotiator = neg(name=f"{neg.__name__}{0}")
     p.add(TAUNegotiatorAdapter(base=negotiator), preferences=ufuns[0])
     for i, u in enumerate(ufuns[1:]):
         p.add(CABNegotiator(name=f"CAB{i}"), preferences=u)
     p.run()
     assert len(p.full_trace) > 0, f"{p.state}{_plot(p)}"
+
+
+@pytest.mark.skipif(not NEGMAS_RUN_GENIUS, reason="Skipping genius tests")
+def test_buyer_seller_gao_easy_genius():
+    from negmas.genius import Atlas3
+
+    run_buyer_seller(
+        Atlas3,
+        Atlas3,
+        normalized=True,
+        seller_reserved=0.1,
+        buyer_reserved=0.1,
+        force_plot=FORCE_PLOT,
+        mechanism_type=GAOMechanism,
+        do_asserts=False,
+    )
+
+
+@pytest.mark.skipif(not NEGMAS_RUN_GENIUS, reason="Skipping genius tests")
+def test_buyer_seller_sao_genius():
+    from negmas.genius import Atlas3
+
+    run_buyer_seller(
+        Atlas3,
+        Atlas3,
+        normalized=True,
+        seller_reserved=0.5,
+        buyer_reserved=0.6,
+        force_plot=FORCE_PLOT,
+        mechanism_type=SAOMechanism,
+        do_asserts=False,
+    )
```

### Comparing `negmas-0.9.7/negmas/tournaments/neg.py` & `negmas-0.9.8/negmas/tournaments/neg.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,24 +156,25 @@
         received_utility=world.received_utility,
         received_advantage=world.received_advantage,
         partner_utility=world.partner_utility,
         partner_advantage=world.partner_advantage,
     )
 
     result = WorldRunResults(
-        world_names=[world.name], log_file_names=[world.log_file_name]
+        world_names=[world.name],
+        log_file_names=[world.log_file_name] if world.log_file_name else [],
     )
     extra = defaultdict(list)
     for aid, agent in world.competitors.items():
         agent_type = agent.type_name
         result.names.append(agent.name)
         result.ids.append(agent.id)
         result.types.append(agent_type)
         if dry_run:
-            result.scores.append(None)
+            result.scores.append(float("nan"))
             continue
         result.scores.append(fun[scoring_method](aid))
         for k, f in fun.items():
             if k == scoring_method:
                 continue
             extra[k].append(dict(type=k, score=f(aid)))
     for k in fun.keys():
@@ -196,15 +197,15 @@
     kwargs["exclude_competitors_from_reassignment"] = False
     return kwargs
 
 
 def create_neg_tournament(
     competitors: Sequence[str | type[Agent]],
     domains: Generator[NegDomain, None, None],
-    competitor_params: Sequence[dict | None] | None = None,
+    competitor_params: Sequence[dict[str, Any]] | None = None,
     **kwargs,
 ) -> PathLike:
     """
     Creates a tournament
 
     Args:
         competitors: A list of class names for the competitors
@@ -389,19 +390,20 @@
                         issues=current_issues,
                         partner_types=p,
                         index=index,
                         roles=roles,
                     )
 
 
-def domains_from_list(domains: list[NegDomain]):
+def domains_from_list(domains: list[NegDomain]) -> Generator[NegDomain, None, None]:
     """
-    Creats an appropriate `NegDomain` generator from a list/tuple of domains
+    Creates an appropriate `NegDomain` generator from a list/tuple of domains
     """
-    return cycle(domains)
+    while True:
+        yield from cycle(domains)
 
 
 if __name__ == "__main__":
     from negmas.sao import AspirationNegotiator, NaiveTitForTatNegotiator
 
     domains = random_discrete_domains(
         issues=[5, 4, (3, 5)],
```

### Comparing `negmas-0.9.7/negmas/tournaments/tournaments.py` & `negmas-0.9.8/negmas/tournaments/tournaments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1218,15 +1218,15 @@
     parallelism = method.split(":")
     if len(parallelism) != 1:
         fraction = float(parallelism[-1])
     parallelism = parallelism[0]
     max_workers = fraction if fraction is None else max(1, int(fraction * cpu_count()))
     executor = futures.ProcessPoolExecutor(max_workers=max_workers)
 
-    return executor, partial(futures.as_completed)
+    return executor, futures.as_completed
 
 
 def _submit_all(
     executor,
     assigned,
     run_ids,
     world_generator,
@@ -1596,15 +1596,14 @@
 
     # save and check attempts
     attempts_path = tournament_path / "attempts"
     attempts_path.mkdir(exist_ok=True, parents=True)
     attempts = defaultdict(int)
     files_to_remove = []
     for afile in attempts_path.glob("*"):
-
         n_attempts = 0
         if afile.is_dir():
             continue
         fname = afile.name
         if fname in run_ids:
             files_to_remove.append(afile)
             continue
@@ -2797,14 +2796,15 @@
                 len(competitors) - 1,
             )
             results = _run_eval(competitors, stage_name)
             if n_winners_per_stage == 1:
                 return results
             competitors = _keep_n(competitors, results, n_winners_per_stage)
         else:
+            competitors = list(competitors)
             random.shuffle(competitors)
             competitor_sets = _divide_into_sets(competitors, n_competitors_per_world)
 
             next_stage_competitors = []
             results = None
             for c in competitor_sets:
                 match_name_ = stage_name + _hash(c)
```

### Comparing `negmas-0.9.7/negmas/types/named.py` & `negmas-0.9.8/negmas/types/named.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/negmas/types/rational.py` & `negmas-0.9.8/negmas/types/rational.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 
 A rational agent is one that has some preferences.
 """
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
-from negmas import warnings
-
 from ..common import PreferencesChange
 from .named import NamedObject
 
 if TYPE_CHECKING:
     from ..outcomes import Outcome
     from ..preferences import (
         BaseUtilityFunction,
@@ -73,14 +71,15 @@
 
         Remarks:
 
             - You MUST call the super() version of this function either before or after your code when you are overriding
               it.
             - The most general form of change is `PreferencesChange.General` which indicates that you cannot trust anything you knew about the ufun anymore
         """
+        _ = changes
 
     def set_preferences(
         self, value: Preferences | None, force=False
     ) -> Preferences | None:
         """
         Sets tha utility function/Preferences.
 
@@ -159,35 +158,40 @@
 
         if not isinstance(v, ProbUtilityFunction):
             raise ValueError(f"Cannot assign a {type(v)} to prob_ufun")
         self.set_preferences(v)
 
     @property
     def ufun(self) -> BaseUtilityFunction | None:
-        """Returns the preferences if it is a UtilityFunction else None"""
+        """Returns the preferences if it is a `BaseUtilityFunction` else None"""
         from ..preferences import BaseUtilityFunction
 
         if self._preferences is None:
             return None
         if isinstance(self._preferences, BaseUtilityFunction):
             return self._preferences
         raise ValueError(
-            f"prefrences are not for type `BaseUtilityFunction` ({self._preferences.__class__.__name__})"
+            f"Preferences are not for type `BaseUtilityFunction` ({self._preferences.__class__.__name__})"
         )
 
     @ufun.setter
     def ufun(self, v: BaseUtilityFunction):
         self.set_preferences(v)
 
     @property
     def has_preferences(self) -> bool:
         """Does the entity has an associated ufun?"""
         return self._preferences is not None
 
     @property
+    def has_ufun(self) -> bool:
+        """Does the entity has an associated ufun?"""
+        return self.ufun is not None
+
+    @property
     def has_cardinal_preferences(self) -> bool:
         """Does the entity has an associated ufun?"""
         from negmas.preferences.protocols import CardinalCrisp
 
         return self._preferences is not None and isinstance(
             self._preferences, CardinalCrisp
         )
```

### Comparing `negmas-0.9.7/negmas/warnings.py` & `negmas-0.9.8/negmas/warnings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import warnings
 
 __all__ = [
     "warn",
     "deprecated",
     "NegmasWarning",
+    "NegmasCannotStartNegotiation",
     "NegmasIgnoredValueWarning",
     "NegmasBridgePathWarning",
     "NegmasBridgeProcessWarning",
     "NegmasInfiniteNegotiationWarning",
     "NegmasStepAndTimeLimitWarning",
     "NegmasBrdigeParsingWarning",
     "NegmasSarializationWarning",
@@ -56,14 +57,18 @@
     ...
 
 
 class NegmasStepAndTimeLimitWarning(NegmasWarning):
     ...
 
 
+class NegmasCannotStartNegotiation(NegmasWarning):
+    ...
+
+
 class NegmasBrdigeParsingWarning(NegmasWarning):
     ...
 
 
 class NegmasSarializationWarning(NegmasWarning):
     ...
```

### Comparing `negmas-0.9.7/negmas.egg-info/PKG-INFO` & `negmas-0.9.8/negmas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: negmas
-Version: 0.9.7
+Version: 0.9.8
 Summary: NEGotiations Managed by Agent Simulations
 Home-page: https://github.com/yasserfarouk/negmas
 Author: Yasser Mohammad
 Author-email: yasserfarouk@gmail.com
 Keywords: negotiation,mas,multi-agent,simulation,AI
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
-Provides-Extra: elicitation
 Provides-Extra: visualization
 Provides-Extra: gui
 Provides-Extra: dask
 Provides-Extra: numba
 License-File: LICENSE
 License-File: AUTHORS.rst
 
@@ -225,14 +223,37 @@
 
 NegMAS tests use scenarios used in ANAC 2010 to ANAC 2018 competitions obtained from the Genius_ Platform. These domains
 can be found in the tests/data and notebooks/data folders.
 
 History
 =======
 
+Release 0.9.8
+-------------
+
+* Restructuring tests
+* Using Numba only with python 3.10
+* Always using with when opening files
+* Adding more info about anac results
+* [SAO] Completely removing support for avoid_ultimatum
+* [SAO] Adding fallbacks to respond() calls in SAO to support the API with and
+  without source. The later API will be dropped later.
+* [Preferences] Adding has_ufun to Rational to check if it has a `BaseUtilityFunction`
+  as its preferences.
+* [Genius] More details on errors from genius bridge
+* [Genius] bugfix when starting genius negotitauions with no n-steps (sometims)
+* [CLI] supporting genius negotiators in the negotiate.py cli
+	Pass -n geinus.<agent-name> or genius:<agent-name>
+	The agent-name can be just the full java class name, or a simplified
+	version that is all lower without the word agent and without _
+
+Release 0.9.7
+-------------
+* minor bugfixes
+
 Release 0.9.6
 -------------
 
 * [python] Supporting 3.11 and dropping support for 3.8 and 3.9
 * [test] Adding 3.11 to tests
 * [major] Adding Generalized Bargaining Protocols
 * [buffix] testing saving exceptions in SAO
```

### Comparing `negmas-0.9.7/negmas.egg-info/SOURCES.txt` & `negmas-0.9.8/negmas.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -221,37 +221,41 @@
 negmas/tests/test_genius.py
 negmas/tests/test_helpers.py
 negmas/tests/test_inout.py
 negmas/tests/test_integration.py
 negmas/tests/test_issue.py
 negmas/tests/test_negotiators.py
 negmas/tests/test_outcomes.py
-negmas/tests/test_preferences.py
 negmas/tests/test_protocols.py
 negmas/tests/test_situated.py
 negmas/tests/test_st.py
-negmas/tests/test_tau.py
 negmas/tournaments/__init__.py
 negmas/tournaments/neg.py
 negmas/tournaments/tournaments.py
 negmas/types/__init__.py
 negmas/types/named.py
 negmas/types/rational.py
 negmas/types/runnable.py
 tests/__init__.py
 tests/switches.py
-tests/test_base_issue.py
-tests/test_checkpoints.py
-tests/test_common.py
-tests/test_genius.py
-tests/test_genius_bridge.py
-tests/test_genius_negotiators_all.py
-tests/test_inout.py
-tests/test_inverter.py
-tests/test_jupyter.py
-tests/test_neg_tournaments.py
-tests/test_outcome_space.py
-tests/test_prob_ufun.py
-tests/test_sao.py
-tests/test_sao_negotiators.py
-tests/test_sao_slow.py
-tests/test_trips_world.py
+tests/core/__init__.py
+tests/core/test_base_issue.py
+tests/core/test_common.py
+tests/core/test_inout.py
+tests/core/test_inverter.py
+tests/core/test_outcome_space.py
+tests/core/test_preferences.py
+tests/core/test_prob_ufun.py
+tests/core/test_sao.py
+tests/core/test_sao_negotiators.py
+tests/core/test_tau.py
+tests/core/test_trips_world.py
+tests/genius/__init__.py
+tests/genius/test_genius.py
+tests/genius/test_genius_bridge.py
+tests/genius/test_genius_negotiators_all.py
+tests/genius/test_inout_with_genius.py
+tests/optional/__init__.py
+tests/optional/test_checkpoints.py
+tests/optional/test_jupyter.py
+tests/optional/test_neg_tournaments.py
+tests/optional/test_sao_slow.py
```

### Comparing `negmas-0.9.7/setup.cfg` & `negmas-0.9.8/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [bumpversion]
-current_version = 0.9.7
+current_version = 0.9.8
 delete_bookmark = True
 commit = False
 tag = False
 
 [metadata]
 name = negmas
-version = 0.9.7
+version = 0.9.8
 author = Yasser Mohammad
 author_email = yasserfarouk@gmail.com
 description = NEGotiations Managed by Agent Simulations
 keywords = 
 	negotiation
 	mas
 	multi-agent
@@ -18,15 +18,14 @@
 	AI
 url = https://github.com/yasserfarouk/negmas
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 classifiers = 
 	License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 
 [options]
 packages = find:
 install_requires = 
@@ -54,25 +53,24 @@
 	gif
 	py4j
 	psutil
 	rich
 	attrs
 	typer
 include_package_data = True
-python_requires = >=3.9
+python_requires = >=3.10
 dependency_links = 
 
 [options.entry_points]
 console_scripts = 
 	negmas=negmas.scripts.app:cli
 	negotiate=negmas.scripts.negotiate:app
 	negui=negmas.gui.app:cli
 
 [options.extras_require]
-elicitation = blist; python_version < '3.10'
 visualization = 
 	flask
 	dash
 	dash-daq
 	dash-bootstrap-components
 gui = pyqt5
 dask = dask[complete]
@@ -104,15 +102,15 @@
 [tool:pytest]
 collect_ignore = ['setup.py']
 
 [mypy]
 warn_unused_configs = False
 warn_incomplete_stub = True
 check_untyped_defs = True
-python_version = 3.9
+python_version = 3.10
 strict_optional = False
 ignore_missing_imports = False
 
 [mypy-setup.*]
 check_untyped_defs = False
 
 [egg_info]
```

### Comparing `negmas-0.9.7/tests/switches.py` & `negmas-0.9.8/tests/switches.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/tests/test_base_issue.py` & `negmas-0.9.8/tests/core/test_base_issue.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/tests/test_checkpoints.py` & `negmas-0.9.8/tests/optional/test_checkpoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 #
 #     n_outcomes, n_negotiators = 5, 3
 #     n_steps = 50
 #     mechanism = SAOMechanism(
 #         outcomes=n_outcomes,
 #         n_steps=n_steps,
 #         offering_is_accepting=True,
-#         avoid_ultimatum=False,
 #         checkpoint_every=checkpoint_every,
 #         checkpoint_folder=new_folder,
 #         checkpoint_filename=filename,
 #         extra_checkpoint_info=None,
 #         exist_ok=exist_ok,
 #         single_checkpoint=single_checkpoint,
 #     )
@@ -148,15 +147,14 @@
 
     n_outcomes, n_negotiators = 5, 3
     n_steps = 50
     mechanism = SAOMechanism(
         outcomes=n_outcomes,
         n_steps=n_steps,
         offering_is_accepting=True,
-        avoid_ultimatum=False,
         checkpoint_every=checkpoint_every,
         checkpoint_folder=new_folder,
         checkpoint_filename=filename,
         extra_checkpoint_info=None,
         exist_ok=exist_ok,
         single_checkpoint=False,
     )
```

### Comparing `negmas-0.9.7/tests/test_common.py` & `negmas-0.9.8/tests/core/test_common.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/tests/test_genius.py` & `negmas-0.9.8/tests/genius/test_genius.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from negmas.genius.bridge import genius_bridge_is_running
 from negmas.genius.gnegotiators import AgentK, Caduceus
 from negmas.genius.negotiator import GeniusNegotiator
 from negmas.inout import Scenario
 from negmas.sao.mechanism import SAOMechanism
 from negmas.sao.negotiators import AspirationNegotiator
 
-TIMELIMIT = 120
+TIMELIMIT = 60
 STEPLIMIT = 1000
 
 AGENTS_WITH_NO_AGREEMENT_ON_SAME_preferences = tuple()
 
 SKIP_IF_NO_BRIDGE = not os.environ.get("NEGMAS_LONG_TEST", False)
 
 
@@ -95,15 +95,14 @@
 
 
 @pytest.mark.skipif(
     condition=SKIP_IF_NO_BRIDGE and not genius_bridge_is_running(),
     reason="No Genius Bridge, skipping genius-agent tests",
 )
 def test_old_agent():
-
     from negmas.genius import GeniusNegotiator
 
     folder_name = pkg_resources.resource_filename(
         "negmas", resource_name="tests/data/cameradomain"
     )
     domain = Scenario.from_genius_folder(folder_name)
     assert domain is not None
@@ -176,15 +175,14 @@
     single_issue=st.booleans(),
 )
 def test_genius_agents_run_using_hypothesis(
     agent_name1,
     agent_name2,
     single_issue,
 ):
-
     src = pkg_resources.resource_filename("negmas", resource_name="tests/data/Laptop")
     base_folder = src
     domain = Scenario.from_genius_folder(Path(base_folder))
     assert domain is not None
     if single_issue:
         domain = domain.to_single_issue()
         assert domain is not None
@@ -289,15 +287,14 @@
     domain = Scenario.from_genius_folder(base_folder)
     assert domain is not None
     gagent = AgentK()
     neg = domain.make_session(
         [gagent, AspirationNegotiator()],
         n_steps=n_steps,
         time_limit=float("inf"),
-        avoid_ultimatum=True,
     )
     if neg is None:
         raise ValueError(f"Failed to load domain from {base_folder}")
     current_time = 0
     for _ in range(n_steps):
         assert gagent.relative_time is not None
         assert (
@@ -385,17 +382,15 @@
         pkg_resources.resource_filename(
             "negmas", resource_name="tests/data/Car-A-domain"
         )
     )
 
     domain = Scenario.from_genius_folder(base_folder)
     assert domain is not None
-    neg = domain.make_session(
-        n_steps=n_steps, time_limit=time_limit, avoid_ultimatum=True
-    )
+    neg = domain.make_session(n_steps=n_steps, time_limit=time_limit)
     if neg is None:
         raise ValueError(f"Failed to load domain from {base_folder}")
     neg.add(
         GeniusNegotiator(java_class_name=a1, strict=True, preferences=domain.ufuns[0]),
     )
     neg.add(
         GeniusNegotiator(java_class_name=a2, strict=True, preferences=domain.ufuns[1]),
@@ -413,17 +408,15 @@
         pkg_resources.resource_filename(
             "negmas", resource_name="tests/data/Car-A-domain"
         )
     )
 
     domain = Scenario.from_genius_folder(base_folder)
     assert domain is not None
-    neg = domain.make_session(
-        n_steps=n_steps, time_limit=float("inf"), avoid_ultimatum=True
-    )
+    neg = domain.make_session(n_steps=n_steps, time_limit=float("inf"))
     if neg is None:
         raise ValueError(f"Failed to load domain from {base_folder}")
     if not isinstance(neg, SAOMechanism):
         raise ValueError(f"Loading generated a domain that is not SAO {type(neg)}")
     neg.add(Caduceus(preferences=domain.ufuns[0], strict=True))
     neg.add(Caduceus(preferences=domain.ufuns[1], strict=True))
     for _ in range(n_steps):
```

### Comparing `negmas-0.9.7/tests/test_genius_bridge.py` & `negmas-0.9.8/tests/genius/test_genius_bridge.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/tests/test_genius_negotiators_all.py` & `negmas-0.9.8/tests/genius/test_genius_negotiators_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,16 +74,15 @@
     WhaleAgent,
     XianFaAgent,
     Yushu,
     YXAgent,
 )
 from negmas.inout import Scenario
 from negmas.sao.negotiators import ToughNegotiator
-
-from .switches import NEGMAS_FASTRUN, NEGMAS_RUN_GENIUS
+from tests.switches import NEGMAS_FASTRUN, NEGMAS_RUN_GENIUS
 
 TIMELIMIT = 30
 STEPLIMIT = 50
 
 AGENTS_WITH_NO_AGREEMENT_ON_SAME_preferences = (
     "agents.anac.y2015.Mercury.Mercury",
     "parties.in4010.q12015.group19.Group19",
@@ -108,17 +107,15 @@
     opponent_factory,
     n_steps,
     time_limit,
 ):
     domain = Scenario.from_genius_folder(base_folder)
     if not domain:
         raise ValueError(f"Cannot open domain {base_folder}")
-    neg = domain.make_session(
-        n_steps=n_steps, time_limit=time_limit, avoid_ultimatum=False
-    )
+    neg = domain.make_session(n_steps=n_steps, time_limit=time_limit)
     if neg is None:
         raise ValueError(f"Failed to load domain from {base_folder}")
     opponent = opponent_factory(preferences=domain.ufuns[opponent_preferences])
     theagent = agent_factory(preferences=domain.ufuns[agent_preferences])
     if agent_starts:
         neg.add(theagent)
         neg.add(opponent)
```

### Comparing `negmas-0.9.7/tests/test_inverter.py` & `negmas-0.9.8/tests/core/test_inverter.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/tests/test_jupyter.py` & `negmas-0.9.8/tests/optional/test_jupyter.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 import papermill as pm
 import pytest
 
 NEGMAS_IGNORE_TEST_NOTEBOOKS = os.environ.get("NEGMAS_IGNORE_TEST_NOTEBOOKS", False)
 
 
 def notebooks():
-    base = Path(__file__).parent.parent / "notebooks"
+    base = Path(__file__).parent.parent.parent / "notebooks"
     return list(_ for _ in base.glob("**/*.ipynb") if "checkpoints" not in str(_))
 
 
 @pytest.mark.skipif(
     condition=NEGMAS_IGNORE_TEST_NOTEBOOKS,
     reason="No Genius Bridge, skipping genius-agent tests",
 )
 @pytest.mark.parametrize("notebook", notebooks())
 def test_notebook(notebook):
-    base = Path(__file__).parent.parent / "notebooks"
+    base = Path(__file__).parent.parent.parent / "notebooks"
     dst = notebook.relative_to(base)
     dst = Path(__file__).parent / "tmp_notebooks" / str(dst)
     dst.parent.mkdir(exist_ok=True, parents=True)
     pm.execute_notebook(notebook, dst)
 
 
 if __name__ == "__main__":
```

### Comparing `negmas-0.9.7/tests/test_neg_tournaments.py` & `negmas-0.9.8/tests/optional/test_neg_tournaments.py`

 * *Files identical despite different names*

### Comparing `negmas-0.9.7/tests/test_sao.py` & `negmas-0.9.8/tests/core/test_sao.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,35 +14,33 @@
 NEGTYPES = all_negotiator_types()
 
 
 @given(
     opp=st.sampled_from(NEGTYPES),
     start=st.booleans(),
     rejector=st.sampled_from([EndImmediately, RejectAlways]),
-    avoid_ultimatum=st.booleans(),
 )
 @example(
     opp=negmas.sao.negotiators.timebased.AdditiveFirstFollowingTBNegotiator,
     start=True,
     rejector=negmas.sao.components.acceptance.EndImmediately,
-    avoid_ultimatum=True,
 )
 @settings(deadline=500000)
-def test_do_nothing_never_gets_agreements(opp, start, rejector, avoid_ultimatum):
+def test_do_nothing_never_gets_agreements(opp, start, rejector):
     agent = make_boa(acceptance=rejector(), offering=NoneOfferingPolicy())
     issues: list[Issue] = [
         make_issue(10, "price"),
         make_issue(10, "quantity"),
         make_issue(["red", "green", "blue"], "color"),
     ]
     ufuns = [
         LinearAdditiveUtilityFunction.random(issues=issues),
         LinearAdditiveUtilityFunction.random(issues=issues),
     ]
-    session = SAOMechanism(n_steps=1000, issues=issues, avoid_ultimatum=avoid_ultimatum)
+    session = SAOMechanism(n_steps=1000, issues=issues)
     negs = [opp(), agent] if not start else [agent, opp()]
     for n, u in zip(negs, ufuns):
         session.add(n, preferences=u)
 
     assert session.run().agreement is None
```

### Comparing `negmas-0.9.7/tests/test_sao_negotiators.py` & `negmas-0.9.8/tests/core/test_sao_negotiators.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import pytest
 
 from negmas import NaiveTitForTatNegotiator, SAOMechanism, make_issue
 from negmas.gb.negotiators.micro import MiCRONegotiator
 from negmas.preferences import LinearAdditiveUtilityFunction as LUFun
 from negmas.preferences.value_fun import AffineFun, IdentityFun, LinearFun, TableFun
 from negmas.sao.negotiators.timebased import BoulwareTBNegotiator
-
-from .switches import NEGMAS_RUN_TEMP_FAILING
+from tests.switches import NEGMAS_RUN_TEMP_FAILING
 
 SHOW_PLOTS = False
 
 
 def run_buyer_seller(buyer, seller, normalized=False, callbacks=False, n_steps=100):
     # create negotiation agenda (issues)
     issues = [
@@ -25,24 +24,24 @@
     # create the mechanism
     session = SAOMechanism(
         issues=issues, n_steps=n_steps, time_limit=None, extra_callbacks=callbacks
     )
 
     # define buyer and seller utilities
     seller_utility = LUFun(
-        values=[
+        values=[  # type: ignore
             IdentityFun(),
             LinearFun(0.2),
             TableFun(dict(today=1.0, tomorrow=0.2, nextweek=0.0)),
         ],
         outcome_space=session.outcome_space,
     )
 
     buyer_utility = LUFun(
-        values={
+        values={  # type: ignore
             "price": AffineFun(-1, bias=9.0),
             "quantity": LinearFun(0.2),
             "delivery_time": TableFun(dict(today=0, tomorrow=0.7, nextweek=1.0)),
         },
         outcome_space=session.outcome_space,
     )
     if normalized:
```

### Comparing `negmas-0.9.7/tests/test_sao_slow.py` & `negmas-0.9.8/tests/optional/test_sao_slow.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,17 +206,15 @@
         if n_waits:
             self.n_waits = random.randint(0, n_waits)
         self.waited = 0
 
     def __call__(self, state, offer):
         if not self.nmi:
             return None
-        if self.waited < self.n_waits and (
-            state.step > 0 or not self.nmi.params["avoid_ultimatum"]
-        ):
+        if self.waited < self.n_waits and state.step > 0:
             self.waited += 1
             return SAOResponse(ResponseType.WAIT, None)
         if self._sleep_seconds:
             if isinstance(self._sleep_seconds, Sequence):
                 s = (
                     random.random() * (self._sleep_seconds[1] - self._sleep_seconds[0])
                     + self._sleep_seconds[0]
@@ -300,15 +298,14 @@
     c2 = MySyncController(sleep_seconds=waste_center, name="c2")
     mechanisms = []
     for m in range(2):
         mechanism = SAOMechanism(
             outcomes=n_outcomes,
             n_steps=n_steps,
             ignore_negotiator_exceptions=False,
-            avoid_ultimatum=False,
             name=f"{m}",
         )
         ufuns = MappingUtilityFunction.generate_random(
             2, outcomes=mechanism.discrete_outcomes()
         )
         mechanism.add(
             c1.create_negotiator(preferences=ufuns[0], id=f"0-{m}", name=f"0-{m}")  # type: ignore It will be SAOControlled
@@ -339,15 +336,14 @@
     c = MySyncController(sleep_seconds=waste_center)
     mechanisms, edge_names = [], []
     for _ in range(n_negotiators):
         mechanism = SAOMechanism(
             outcomes=n_outcomes,
             n_steps=n_steps,
             ignore_negotiator_exceptions=True,
-            avoid_ultimatum=False,
         )
         ufuns = MappingUtilityFunction.generate_random(
             2, outcomes=mechanism.discrete_outcomes()
         )
         edge_names.append(f"f{0}")
         mechanism.add(
             TimeWaster(
@@ -437,17 +433,15 @@
     mechanism.step()
     mechanism.run()
 
 
 @mark.parametrize("n_negotiators,oia", [(2, True), (3, True), (2, False), (3, False)])
 def test_mechanism_runs_with_offering_not_accepting(n_negotiators, oia):
     n_outcomes = 5
-    mechanism = SAOMechanism(
-        outcomes=n_outcomes, n_steps=3, offering_is_accepting=oia, avoid_ultimatum=False
-    )
+    mechanism = SAOMechanism(outcomes=n_outcomes, n_steps=3, offering_is_accepting=oia)
     ufuns = MappingUtilityFunction.generate_random(1, outcomes=n_outcomes)
     for i in range(n_negotiators):
         mechanism.add(AspirationNegotiator(name=f"agent{i}"), preferences=ufuns[0])
     assert mechanism.state.step == 0
     mechanism.step()
     assert mechanism._current_proposer and mechanism._current_proposer.name == "agent0"
     assert mechanism.state.n_acceptances == n_negotiators + int(oia) - 1
@@ -465,15 +459,14 @@
     n_outcomes = 5
     mechanisms = []
     for _ in range(10):
         mechanism = SAOMechanism(
             outcomes=n_outcomes,
             n_steps=random.randint(3, 20),
             offering_is_accepting=oia,
-            avoid_ultimatum=False,
         )
         ufuns = MappingUtilityFunction.generate_random(1, outcomes=n_outcomes)
         for i in range(n_negotiators):
             mechanism.add(AspirationNegotiator(name=f"agent{i}"), preferences=ufuns[0])
         mechanisms.append(mechanism)
 
     states = SAOMechanism.runall(mechanisms)
@@ -504,15 +497,14 @@
     for i in range(n_negotiators):
         mechanisms.append(
             SAOMechanism(
                 outcomes=n_outcomes,
                 n_steps=10,
                 time_limit=None,
                 offering_is_accepting=oia,
-                avoid_ultimatum=False,
                 end_on_no_response=False,
             )
         )
         ufuns = MappingUtilityFunction.generate_random(
             n_negotiators, outcomes=n_outcomes
         )
         for i in range(n_negotiators):
@@ -531,15 +523,14 @@
 
     file = tmp_path / "mechanism.pck"
     n_outcomes, n_negotiators = 5, 3
     mechanism = SAOMechanism(
         outcomes=n_outcomes,
         n_steps=3,
         offering_is_accepting=True,
-        avoid_ultimatum=False,
     )
     ufuns = MappingUtilityFunction.generate_random(n_negotiators, outcomes=n_outcomes)
     for i in range(n_negotiators):
         mechanism.add(AspirationNegotiator(name=f"agent{i}"), preferences=ufuns[i])
 
     assert mechanism.state.step == 0
     with open(file, "wb") as f:
@@ -562,15 +553,14 @@
 def test_checkpointing_mechanism(tmp_path):
     file = tmp_path
     n_outcomes, n_negotiators = 5, 3
     mechanism = SAOMechanism(
         outcomes=n_outcomes,
         n_steps=3,
         offering_is_accepting=True,
-        avoid_ultimatum=False,
     )
     ufuns = MappingUtilityFunction.generate_random(n_negotiators, outcomes=n_outcomes)
     for i in range(n_negotiators):
         mechanism.add(AspirationNegotiator(name=f"agent{i}"), preferences=ufuns[i])
 
     assert mechanism.state.step == 0
     file_name = mechanism.checkpoint(file)
@@ -876,29 +866,25 @@
             .normalize()
             .to_single_issue()
             .make_session()
         )
 
 
 @given(
-    avoid_ultimatum=st.booleans(),
     n_steps=st.integers(10, 11),
     n_waits=st.integers(0, 4),
     n_waits2=st.integers(0, 4),
 )
 @settings(deadline=20000, max_examples=100)
-def test_single_mechanism_history_with_waiting(
-    avoid_ultimatum, n_steps, n_waits, n_waits2
-):
+def test_single_mechanism_history_with_waiting(n_steps, n_waits, n_waits2):
     n_outcomes, waste = 5, (0.0, 0.3)
     mechanism = SAOMechanism(
         outcomes=n_outcomes,
         n_steps=n_steps,
         ignore_negotiator_exceptions=False,
-        avoid_ultimatum=avoid_ultimatum,
     )
     ufuns = MappingUtilityFunction.generate_random(2, outcomes=mechanism.outcomes)
     mechanism.add(
         TimeWaster(
             name=f"agent{0}", sleep_seconds=waste, preferences=ufuns[0], n_waits=n_waits
         )
     )
@@ -909,17 +895,15 @@
             preferences=ufuns[1],
             n_waits=n_waits2,
         )
     )
     mechanism.run()
     first = mechanism._selected_first
     n_negotiators = len(mechanism.negotiators)
-    assert (not avoid_ultimatum and first == 0) or (
-        avoid_ultimatum and 0 <= first < n_negotiators
-    )
+    assert first == 0
     assert mechanism.state.agreement is None
     assert mechanism.state.started
     assert mechanism.state.timedout or (
         n_waits + n_waits2 > 0 and mechanism.state.broken
     )
     assert mechanism.state.step == n_steps or (
         n_waits + n_waits2 > 0
@@ -936,53 +920,37 @@
     # check history details is correct
     s = [defaultdict(int), defaultdict(int)]
     r = [defaultdict(int), defaultdict(int)]
     h = [defaultdict(int), defaultdict(int)]
     first_offers = []
     ignored_offers = []
     for i, n in enumerate(mechanism.negotiators):
-        # all agents asked to offer first if avoid_ultimatum
-        if avoid_ultimatum:
-            assert n.received_offers[0] is None
-        else:
-            first_offers.append(n.received_offers[0] is None)
+        first_offers.append(n.received_offers[0] is None)
 
         # sent and received match
         for j, w in n.my_offers.items():
             # cannot send mutlipe offers in the same step
             assert j not in s[i].keys()
             # cannot send None
             assert w is not None  # or (j == 0 and not avoid_ultimatum)
-            if j == 0 and i != first and avoid_ultimatum:
-                # cannot have more than n_negotiators - 1 ignored offers
-                assert len(ignored_offers) < n_negotiators - 1
-                ignored_offers.append(w[0])
-                continue
             s[i][j] = w[0]
         for j, w in n.received_offers.items():
             # cannot receive multiple ofers in the same step
             assert j not in r[i].keys()
             # canont be asked to start offering except in the first step
             assert w is not None or j == 0
             # this is the first agent to offer, ignore its first step
-            if (first == i and j == 0) or (avoid_ultimatum and j == 0):
+            if first == i and j == 0:
                 # if this is the first agent, its first thing recieved must be None
                 assert w is None
                 continue
-            assert (
-                w is not None
-            ), f"None outcome agent {i} @ {j} (avoid={avoid_ultimatum}) first is {first}"
+            assert w is not None, f"None outcome agent {i} @ {j} first is {first}"
             r[i][j] = w[0]
 
-    # a single agent is asked to offer first if not avoid_ultimatum
-    if not avoid_ultimatum:
-        assert any(first_offers) and not all(first_offers)
-    # every agent is asked to offer and all except one are ignored if avoid_ultimatum
-    if avoid_ultimatum:
-        assert len(ignored_offers) == n_negotiators - 1
+    assert any(first_offers) and not all(first_offers)
 
     # reconstruct history
     neg_map = dict(zip((_.id for _ in mechanism.negotiators), [0, 1]))
     for state in mechanism.history:
         for _, w in state.new_offers:
             a = neg_map[_]
             # cannot see the same step twice in the history of an agent
@@ -1001,15 +969,15 @@
 
     # pprint([s, r, h])
     # history matches what is stored inside agents
     for i, n in enumerate(mechanism.negotiators):
         for j, w in s[i].items():
             assert j in r[1 - i] or (j == 0)
         for j, w in r[i].items():
-            assert j in s[1 - i] or (j == 0 and not avoid_ultimatum)
+            assert j in s[1 - i]
 
     # s and r will not have matched indices but should have matched values
     s = [list(_.values()) for _ in s]
     r = [list(_.values()) for _ in r]
     h = [list(_[0] for _ in _.values()) for _ in h]
     # history matches what is stored inside agents
     for i, n in enumerate(mechanism.negotiators):
@@ -1022,20 +990,19 @@
             assert s[1 - i][j] == w
 
 
 @given(
     keep_order=st.booleans(),
     n_first=st.integers(1, 6),
     n_second=st.integers(1, 6),
-    avoid_ultimatum=st.booleans(),
     end_on_no_response=st.booleans(),
 )
 @settings(deadline=20000)
 def test_neg_sync_loop_receives_all_offers(
-    keep_order, n_first, n_second, avoid_ultimatum, end_on_no_response
+    keep_order, n_first, n_second, end_on_no_response
 ):
     # from pprint import pprint
 
     n_outcomes, n_steps = 100, 10
     waste_center = 0.01
     c1s = [
         MySyncController(sleep_seconds=waste_center, name="c1") for _ in range(n_first)
@@ -1044,15 +1011,14 @@
         MySyncController(sleep_seconds=waste_center, name="c2") for _ in range(n_second)
     ]
     mechanisms = [
         SAOMechanism(
             outcomes=n_outcomes,
             n_steps=n_steps,
             ignore_negotiator_exceptions=False,
-            avoid_ultimatum=avoid_ultimatum,
             end_on_no_response=end_on_no_response,
             name=f"{i}v{j}",
         )
         for i in range(n_first)
         for j in range(n_second)
     ]
     for mechanism in mechanisms:
@@ -1073,40 +1039,32 @@
         states = SAOMechanism.stepall(mechanisms, keep_order=keep_order)
         if all(not _.running for _ in states):
             break
 
     for mechanism in mechanisms:
         ls = [len(mechanism.negotiator_offers(n.id)) for n in mechanism.negotiators]
         check.less_equal(abs(ls[0] - ls[1]), 1, mechanism.trace)
-        if avoid_ultimatum:
-            check.greater_equal(len(mechanism.offers), 2 * (n_steps - 1))
-            check.less_equal(len(mechanism.offers), 2 * n_steps)
-            for n in mechanism.negotiators:
-                check.greater_equal(len(mechanism.negotiator_offers(n.id)), n_steps - 1)
-            pass
-        else:
-            check.equal(len(mechanism.offers), 2 * n_steps)
-            for n in mechanism.negotiators:
-                check.equal(len(mechanism.negotiator_offers(n.id)), n_steps)
+        check.equal(len(mechanism.offers), 2 * n_steps)
+        for n in mechanism.negotiators:
+            check.equal(len(mechanism.negotiator_offers(n.id)), n_steps)
 
     for c, n_partners in itertools.chain(
         zip(c1s, itertools.repeat(n_second)), zip(c2s, itertools.repeat(n_first))
     ):
         steps = set(range(1, n_steps))
         countered_steps = set(c.countered_offers.keys())
         missing_steps = steps.difference(countered_steps)
         check.equal(len(missing_steps), 0, f"Missing steps are {missing_steps}")
-        if not avoid_ultimatum:
-            for s in steps:
-                partners = c.countered_offers[s]
-                check.equal(
-                    len(partners),
-                    n_partners,
-                    f"partners {len(partners)} (of {n_partners}) step {s}.\n{partners}",
-                )
+        for s in steps:
+            partners = c.countered_offers[s]
+            check.equal(
+                len(partners),
+                n_partners,
+                f"partners {len(partners)} (of {n_partners}) step {s}.\n{partners}",
+            )
 
     for mechanism in mechanisms:
         check.is_true(mechanism.state.started)
         check.is_none(mechanism.state.agreement)
         check.is_false(mechanism.state.has_error)
         check.is_false(mechanism.state.broken)
         check.is_false(mechanism.state.waiting)
@@ -1233,15 +1191,14 @@
 
     n_outcomes, n_negotiators = 5, 3
     n_steps = 50
     mechanism = SAOMechanism(
         outcomes=n_outcomes,
         n_steps=n_steps,
         offering_is_accepting=True,
-        avoid_ultimatum=False,
         checkpoint_every=checkpoint_every,
         checkpoint_folder=new_folder,
         checkpoint_filename=filename,
         extra_checkpoint_info=None,
         exist_ok=exist_ok,
         single_checkpoint=single_checkpoint,
     )
@@ -1355,17 +1312,15 @@
     outcome_space = make_os(issues)
     u1 = LinearUtilityFunction([-0.75, 0.25], outcome_space=outcome_space)
     u2 = LinearUtilityFunction([0.5, -0.5], outcome_space=outcome_space)
     return u1, u2, outcome_space
 
 
 def _run_neg(agents, utils, outcome_space):
-    neg = SAOMechanism(
-        outcome_space=outcome_space, n_steps=200, avoid_ultimatum=False, time_limit=None
-    )
+    neg = SAOMechanism(outcome_space=outcome_space, n_steps=200, time_limit=None)
     for a, u in zip(agents, utils):
         neg.add(a, preferences=u)
     neg.run()
     assert neg.state.agreement is not None, f"No agreement!!\n{neg.trace}"
     for a, u in zip(agents, utils):
         offers = neg.negotiator_offers(a.id)
         _, best = u.extreme_outcomes()
```

### Comparing `negmas-0.9.7/tests/test_trips_world.py` & `negmas-0.9.8/tests/core/test_trips_world.py`

 * *Files identical despite different names*

