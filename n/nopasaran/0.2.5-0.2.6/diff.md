# Comparing `tmp/nopasaran-0.2.5.tar.gz` & `tmp/nopasaran-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopasaran-0.2.5.tar", last modified: Sat Jul  8 10:11:09 2023, max compression
+gzip compressed data, was "nopasaran-0.2.6.tar", last modified: Sun Jul  9 12:11:15 2023, max compression
```

## Comparing `nopasaran-0.2.5.tar` & `nopasaran-0.2.6.tar`

### file list

```diff
@@ -1,72 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-08 10:10:57.000000 nopasaran-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-08 10:11:09.851551 nopasaran-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-08 10:10:57.000000 nopasaran-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.839551 nopasaran-0.2.5/nopasaran/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.843551 nopasaran-0.2.5/nopasaran/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/controllers/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/controllers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/controllers/protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2633 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.843551 nopasaran-0.2.5/nopasaran/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/definitions/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/definitions/control_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/definitions/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/definitions/transitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.847551 nopasaran-0.2.5/nopasaran/interpreters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/interpreters/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/interpreters/action_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/interpreters/condition_interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2130 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/interpreters/interpreter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/interpreters/transition_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.847551 nopasaran-0.2.5/nopasaran/ipsec_tunnels/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/ipsec_tunnels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/ipsec_tunnels/ipsec_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.847551 nopasaran-0.2.5/nopasaran/machines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/machines/action_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     9036 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/machines/state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.847551 nopasaran-0.2.5/nopasaran/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/parsers/interpreter_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/parsers/state_machine_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.847551 nopasaran-0.2.5/nopasaran/primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/nopasaran/primitives/action_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      925 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/action_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/control_channel_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/data_manipulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/ip_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/nested_machine_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/tcp_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     9859 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/tmp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/action_primitives/udp_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/nopasaran/primitives/condition_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/condition_primitives/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/condition_primitives/condition_primitives.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/condition_primitives/variable_comparisons.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/nopasaran/primitives/transition_primitives/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/transition_primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/transition_primitives/assignment_transitions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/primitives/transition_primitives/transition_primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/nopasaran/sniffers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/sniffers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/sniffers/sniffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-08 10:10:57.000000 nopasaran-0.2.5/nopasaran/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.843551 nopasaran-0.2.5/nopasaran.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-08 10:11:09.000000 nopasaran-0.2.5/nopasaran.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 10:11:09.851551 nopasaran-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-08 10:11:08.000000 nopasaran-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 10:11:09.851551 nopasaran-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 10:10:57.000000 nopasaran-0.2.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-09 12:11:07.000000 nopasaran-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-09 12:11:15.164183 nopasaran-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-09 12:11:07.000000 nopasaran-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/controllers/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/controllers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/controllers/protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/definitions/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/definitions/control_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/definitions/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/definitions/transitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/errors/parsing_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/interpreters/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/interpreters/action_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      862 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/interpreters/condition_interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2130 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/interpreters/interpreter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/interpreters/transition_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/ipsec_tunnels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/ipsec_tunnels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/ipsec_tunnels/ipsec_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran/machines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/machines/action_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/machines/state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/parsers/interpreter_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/parsers/state_machine_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/primitives/action_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1244 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/action_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/control_channel_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/data_channel_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/data_manipulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/event_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/io_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/ip_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/nested_machine_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11862 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/tcp_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/action_primitives/udp_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/primitives/condition_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/condition_primitives/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      307 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/condition_primitives/condition_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/condition_primitives/variable_comparisons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/primitives/transition_primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/transition_primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/transition_primitives/assignment_transitions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      332 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/primitives/transition_primitives/transition_primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/nopasaran/sniffers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/sniffers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/sniffers/sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-09 12:11:07.000000 nopasaran-0.2.6/nopasaran/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.160183 nopasaran-0.2.6/nopasaran.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-09 12:11:15.000000 nopasaran-0.2.6/nopasaran.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 12:11:15.164183 nopasaran-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-09 12:11:14.000000 nopasaran-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:15.164183 nopasaran-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 12:11:07.000000 nopasaran-0.2.6/tests/__init__.py
```

### Comparing `nopasaran-0.2.5/LICENSE` & `nopasaran-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/PKG-INFO` & `nopasaran-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.5
+Version: 0.2.6
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.5/README.md` & `nopasaran-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/__main__.py` & `nopasaran-0.2.6/nopasaran/__main__.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/controllers/controller.py` & `nopasaran-0.2.6/nopasaran/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/controllers/factory.py` & `nopasaran-0.2.6/nopasaran/controllers/factory.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/controllers/protocol.py` & `nopasaran-0.2.6/nopasaran/controllers/protocol.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/decorators.py` & `nopasaran-0.2.6/nopasaran/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
-
 from functools import wraps
 
 from nopasaran.parsers.interpreter_parser import Parser
-
+from nopasaran.errors.parsing_error import ParsingError
 
 def parsing_decorator(input_args, output_args, optional_inputs=False, optional_outputs=False):
     """
     Decorator for parsing inputs and outputs of a function.
     
     This decorator parses the inputs and outputs of a function based on the specified constraints.
     
@@ -17,16 +16,21 @@
         optional_inputs (bool, optional): Whether optional inputs are allowed. Defaults to False.
         optional_outputs (bool, optional): Whether optional outputs are allowed. Defaults to False.
     
     Returns:
         function: The decorated function.
     
     Raises:
-        RuntimeError: If an error occurs while parsing or executing the function.
+        ParsingError: If an error occurs while parsing or executing the function.
     """
+    def handle_parsing_error(func, message):
+        error_msg = f"Error while {message} '{func.__name__}':"
+        logging.error("[Parsing] " + error_msg)
+        raise ParsingError(error_msg)
+
     def decorator(func):
         @wraps(func)
         def wrapper(line, variable_dict):
             """
             Wrapper function for the decorator.
             
             This function parses the inputs and outputs, logs the details, and calls the decorated function.
@@ -35,29 +39,31 @@
                 line (str): The command line to parse.
                 variable_dict (dict): The dictionary of variables.
             
             Returns:
                 The result of the decorated function.
             
             Raises:
-                RuntimeError: If an error occurs while parsing or executing the function.
+                ParsingError: If an error occurs while parsing or executing the function.
             """
-            logging.debug("[Parsing] Primitive name: {}. Expecting {} input(s) and {} output(s). Optional inputs: {}. Optional outputs: {}"
+            logging.debug("[Parsing] [Primitive - {}] Expecting {} input(s) and {} output(s). Optional inputs: {}. Optional outputs: {}"
                          .format(func.__name__, input_args, output_args, optional_inputs, optional_outputs))
             
             try:
                 inputs, outputs = Parser.parse(line, input_args, output_args, optional_inputs, optional_outputs)
-                logging.debug("[Parsing] Received inputs: {}. Received outputs: {}".format(inputs, outputs))
+                logging.debug("[Parsing] [Primitive - {}] Received inputs: {}. Received outputs: {}".format(func.__name__, inputs, outputs))
+            except ParsingError as e:
+                handle_parsing_error(func, "parsing the command line")
             except Exception as e:
-                error_msg = "Error while parsing primitive '{}': {}".format(func.__name__, e)
-                logging.error("[Parsing] " + error_msg)
-                raise RuntimeError(error_msg)
+                handle_parsing_error(func, f"parsing the command line '{e}'")
+            
             try:
                 return func(inputs, outputs, variable_dict)
+            except ParsingError as e:
+                handle_parsing_error(func, "executing the function")
             except Exception as e:
-                error_msg = "Error while executing primitive {}".format(func.__name__)
-                logging.error("[Parsing] " + error_msg)
-                raise RuntimeError(error_msg)
-            
+                logging.error("[Execution] " + str(e))
+                handle_parsing_error(func, "executing the function")
+
         return wrapper
-    
+
     return decorator
```

### Comparing `nopasaran-0.2.5/nopasaran/definitions/control_channel.py` & `nopasaran-0.2.6/nopasaran/definitions/control_channel.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/interpreters/action_interpreter.py` & `nopasaran-0.2.6/nopasaran/interpreters/action_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/interpreters/condition_interpreter.py` & `nopasaran-0.2.6/nopasaran/interpreters/condition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/interpreters/interpreter.py` & `nopasaran-0.2.6/nopasaran/interpreters/interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/interpreters/transition_interpreter.py` & `nopasaran-0.2.6/nopasaran/interpreters/transition_interpreter.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/ipsec_tunnels/ipsec_conf.py` & `nopasaran-0.2.6/nopasaran/ipsec_tunnels/ipsec_conf.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/machines/action_queue.py` & `nopasaran-0.2.6/nopasaran/machines/action_queue.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/machines/state_machine.py` & `nopasaran-0.2.6/nopasaran/machines/state_machine.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,70 +26,69 @@
         self.sniffer = Sniffer(self, filter='')
         self.variables = {}
         self.redirections = {}
         self.parameters = parameters
         self.root_state_machine = self if root_state_machine is None else root_state_machine
         self.returned_value = None
         self.actions = ActionQueue()
-        logging.info('Parameters received: {}'.format(parameters))
-        logging.debug('Machine ID: {}. Initialized.'.format(self.machine_id))
+        logging.info('[State Machine - {}] Parameters received: {}'.format(self.machine_id, parameters))
+        logging.debug('[State Machine - {}] Initialized.'.format(self.machine_id))
 
     def start(self):
         """
         Start the state machine and execute actions.
         """
-        logging.debug('Machine ID: {}. Starting machine.'.format(self.machine_id))
+        logging.debug('[State Machine - {}] Starting machine.'.format(self.machine_id))
         self.trigger_event(EventNames.STARTED.name)
         while True:
             next_action = self.actions.dequeue_next_action()
             if next_action is None:
-                logging.warning('Machine ID: {}. Dequeue returned None. Stopping.'.format(self.machine_id))
+                logging.warning('[State Machine - {}] Dequeue returned None. Stopping.'.format(self.machine_id))
                 break
-            logging.debug('Executing action: {}'.format(next_action))
             self.execute_action(next_action)
 
     def execute_action(self, action):
         """
         Execute an action.
 
         Args:
             action (dict): The action to execute.
         """
-        logging.debug('Machine ID: {}: Executing action: {}'.format(self.machine_id, action))
+        logging.debug('[State Machine - {}] Executing action: {}'.format(self.machine_id, action))
         if Command.EXECUTE_ACTION.name in action:
             ActionInterpreter.evaluate(action[Command.EXECUTE_ACTION.name], self)
         elif Command.ASSIGN_VARIABLES.name in action:
             self.assign_variables(action[Command.ASSIGN_VARIABLES.name])
-            logging.info('Machine ID: {}: Variables assigned: {}'.format(self.machine_id, self.variables))
+            logging.info('[State Machine - {}] Variables assigned: {}'.format(self.machine_id, self.variables))
         elif Command.SET_STATE.name in action:
             self.update_state(action[Command.SET_STATE.name])
 
     def get_nested_machine(self, nested_state_json, parameters):
         """
         Get a nested state machine.
 
         Args:
             nested_state_json (dict): The JSON representation of the nested state machine.
             parameters (list): The parameters for the nested state machine.
 
         Returns:
             StateMachine: The nested state machine.
         """
-        logging.debug('Machine ID: {}: Getting nested finite state machine.'.format(self.machine_id))
+        logging.debug('[State Machine - {}] Getting nested finite state machine.'.format(self.machine_id))
         nested_machine = StateMachine(state_json=nested_state_json, parameters=parameters, root_state_machine=self.root_state_machine)
         return nested_machine
 
     def update_state(self, state):
         """
         Update the current state of the state machine.
 
         Args:
             state (str): The new state.
         """
-        logging.debug('Machine ID: {}: Setting state to: {}'.format(self.machine_id, state))
+        logging.debug('[State Machine - {}] Setting state to: {}'.format(self.machine_id, state))
         self.current_state = state
 
     def start_sniffer(self):
         """
         Start the sniffer for the state machine.
         """
         logging.debug('Starting sniffer for machine with ID: {}'.format(self.machine_id))
@@ -105,51 +104,51 @@
     def assign_variables(self, variables):
         """
         Assign variables to the state machine.
 
         Args:
             variables (dict): The variables to assign.
         """
-        logging.debug('Machine ID: {}: Setting variables: {}'.format(self.machine_id, variables))
+        logging.debug('[State Machine - {}] Setting variables: {}'.format(self.machine_id, variables))
         self.variables = variables
 
     def set_variable_value(self, name, new_value):
         """
         Set the value of a variable.
 
         Args:
             name (str): The name of the variable.
             new_value: The new value for the variable.
         """
-        logging.info('Machine ID: {}: Setting variable {} to: {}'.format(self.machine_id, name, new_value))
+        logging.info('[State Machine - {}] Setting variable {} to: {}'.format(self.machine_id, name, new_value))
         self.variables[name] = new_value
 
     def get_variable_value(self, variable_name):
         """
         Get the value of a variable.
 
         Args:
             variable_name (str): The name of the variable.
 
         Returns:
             The value of the variable.
         """
         if variable_name not in self.variables:
-            logging.error('Machine ID: {}: Variable {} does not exist.'.format(self.machine_id, variable_name))
+            logging.error('[State Machine - {}] Variable {} does not exist.'.format(self.machine_id, variable_name))
         return self.variables[variable_name]
 
     def update_variable_value(self, variable_name, new_value):
         """
         Update the value of a variable.
 
         Args:
             variable_name (str): The name of the variable.
             new_value: The new value for the variable.
         """
-        logging.info('Machine ID: {}: Updating variable {} to: {}'.format(self.machine_id, variable_name, new_value))
+        logging.info('[State Machine - {}] Updating variable {} to: {}'.format(self.machine_id, variable_name, new_value))
         self.variables[variable_name] = new_value
 
     def update_sniffer_filter(self, filter):
         """
         Update the filter for the sniffer.
 
         Args:
@@ -170,32 +169,32 @@
         """
         Add a redirection from an event to a state.
 
         Args:
             event (str): The event to redirect.
             state (str): The state to redirect to.
         """
-        logging.debug('Machine ID: {}: Adding redirection from event {} to state {}.'.format(self.machine_id, event, state))
+        logging.debug('[State Machine - {}] Adding redirection from event {} to state {}.'.format(self.machine_id, event, state))
         self.redirections[event] = state
 
     def trigger_event(self, event):
         """
         Trigger an event.
 
         Args:
             event (str): The event to trigger.
         """
-        logging.debug('Machine ID: {}: Event {} triggered'.format(self.machine_id, event))
+        logging.debug('[State Machine - {}] Event {} triggered'.format(self.machine_id, event))
         next_states = self.state_machine_parser.get_next_states_on_event(self.current_state, event)
         if next_states is not None:
             self.make_transition(next_states)
         elif event in self.redirections:
             self.add_transition_actions(self.redirections[event])
         else:
-            logging.warning('Machine ID: {}: No matching event for {}. Skipping.'.format(self.machine_id, event))
+            logging.warning('[State Machine - {}] No matching event for {}. Skipping.'.format(self.machine_id, event))
 
     def add_transition_actions(self, next_state_name, assignable=False, state=None):
         """
         Add transition actions for the next state.
 
         Args:
             next_state_name (str): The name of the next state.
```

### Comparing `nopasaran-0.2.5/nopasaran/parsers/interpreter_parser.py` & `nopasaran-0.2.6/nopasaran/parsers/interpreter_parser.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/parsers/state_machine_parser.py` & `nopasaran-0.2.6/nopasaran/parsers/state_machine_parser.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import uuid
 
+def patch_xstate(array_to_to_parse, field):
+            actions = ArrayParser.get_safe_array(array_to_to_parse[field])
+            types = [action['type'] for action in actions]
+            return types
+
 
 class ArrayParser:
     """
     Parser class for handling arrays.
     
     This class provides methods to handle arrays in a safe manner.
     """
@@ -79,29 +84,33 @@
         Args:
             state (str): The state for which to get the entry actions.
         
         Returns:
             list or None: The list of entry actions, or None if no entry actions are defined.
         """
         if 'entry' in self.states[state]:
-            return ArrayParser.get_safe_array(self.states[state]['entry'])
+            # Patching the changement of xstate discovered on th 9th of July 2023
+            #return ArrayParser.get_safe_array(self.states[state]['entry'])
+            return patch_xstate(self.states[state], 'entry')
         return None
 
     def get_exit_actions(self, state):
         """
         Get the exit actions for a state.
         
         Args:
             state (str): The state for which to get the exit actions.
         
         Returns:
             list or None: The list of exit actions, or None if no exit actions are defined.
         """
         if 'exit' in self.states[state]:
-            return ArrayParser.get_safe_array(self.states[state]['exit'])
+            # Patching the changement of xstate discovered on th 9th of July 2023
+            #return ArrayParser.get_safe_array(self.states[state]['exit'])
+            return patch_xstate(self.states[state], 'exit')
         return None
 
     def get_next_states_on_event(self, state, event):
         """
         Get the next states on an event for a state.
         
         Args:
@@ -150,9 +159,11 @@
         Args:
             next_state (dict): The next state.
         
         Returns:
             list or None: The list of transition actions, or None if no transition actions are defined.
         """
         if 'actions' in next_state:
-            return ArrayParser.get_safe_array(next_state['actions'])
+            # Patching the changement of xstate discovered on th 9th of July 2023
+            #return ArrayParser.get_safe_array(next_state['actions'])
+            return patch_xstate(next_state, 'actions')
         return None
```

### Comparing `nopasaran-0.2.5/nopasaran/primitives/action_primitives/action_primitives.py` & `nopasaran-0.2.6/nopasaran/primitives/action_primitives/action_primitives.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 from nopasaran.primitives.primitives import Primitives
-from nopasaran.primitives.action_primitives.tmp import TmpPrimitives
 from nopasaran.primitives.action_primitives.data_manipulation import DataManipulationPrimitives
 from nopasaran.primitives.action_primitives.nested_machine_utils import NestedMachinePrimitives
+from nopasaran.primitives.action_primitives.data_channel_primitives import DataChannelPrimitives
 from nopasaran.primitives.action_primitives.control_channel_primitives import ControlChannelPrimitives
+from nopasaran.primitives.action_primitives.event_primitives import EventPrimitives
+from nopasaran.primitives.action_primitives.io_primitives import IOPrimitives
 from nopasaran.primitives.action_primitives.ip_primitives import IPPrimitives
 from nopasaran.primitives.action_primitives.tcp_primitives import TCPPrimitives
 from nopasaran.primitives.action_primitives.udp_primitives import UDPPrimitives
 
 class ActionPrimitives(Primitives):
     """
     Class containing action primitives for the state machine.
     """
-    classes = [TmpPrimitives, DataManipulationPrimitives, NestedMachinePrimitives, ControlChannelPrimitives, IPPrimitives, TCPPrimitives, UDPPrimitives]
+    classes = [
+        DataManipulationPrimitives, 
+        NestedMachinePrimitives, 
+        DataChannelPrimitives, 
+        ControlChannelPrimitives, 
+        EventPrimitives, 
+        IOPrimitives, 
+        IPPrimitives, 
+        TCPPrimitives, 
+        UDPPrimitives
+        ]
```

### Comparing `nopasaran-0.2.5/nopasaran/primitives/action_primitives/control_channel_primitives.py` & `nopasaran-0.2.6/nopasaran/primitives/action_primitives/control_channel_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/primitives/action_primitives/data_manipulation.py` & `nopasaran-0.2.6/nopasaran/primitives/action_primitives/data_manipulation.py`

 * *Files 17% similar despite different names*

```diff
@@ -78,8 +78,34 @@
             outputs (List[str]): The list of output variable names. It contains one mandatory output argument, which is the name of the variable to store the generated random float.
             
             state_machine: The state machine object.
 
         Returns:
             None
         """
-        state_machine.set_variable_value(outputs[0], utils.set_random_float(inputs[0], inputs[1]))
+        state_machine.set_variable_value(outputs[0], utils.set_random_float(inputs[0], inputs[1]))
+
+    @staticmethod
+    @parsing_decorator(input_args=1, output_args=0)
+    def pop(inputs, outputs, state_machine):
+        """
+        Remove the first element from a list stored in the machine's state.
+
+        Number of input arguments: 1
+
+        Number of output arguments: 0
+
+        Optional input arguments: No
+
+        Optional output arguments: No
+
+        Args:
+            inputs (List[str]): The list of input variable names. It contains one mandatory input argument, which is the name of a variable representing the list.
+            
+            outputs (List[str]): The list of output variable names.
+            
+            state_machine: The state machine object.
+
+        Returns:
+            None
+        """
+        state_machine.get_variable_value(inputs[0]).pop(0)
```

### Comparing `nopasaran-0.2.5/nopasaran/primitives/action_primitives/ip_primitives.py` & `nopasaran-0.2.6/nopasaran/primitives/action_primitives/ip_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/primitives/action_primitives/nested_machine_utils.py` & `nopasaran-0.2.6/nopasaran/primitives/action_primitives/nested_machine_utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/primitives/action_primitives/tcp_primitives.py` & `nopasaran-0.2.6/nopasaran/primitives/action_primitives/tcp_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/primitives/action_primitives/udp_primitives.py` & `nopasaran-0.2.6/nopasaran/primitives/action_primitives/udp_primitives.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/primitives/condition_primitives/variable_comparisons.py` & `nopasaran-0.2.6/nopasaran/primitives/condition_primitives/variable_comparisons.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     Class containing methods for comparing variables in a state machine.
     """
 
     @staticmethod
     @parsing_decorator(input_args=2, output_args=0)
     def equal(inputs, outputs, state_variables):
         """
-        Check if two values in the state variables are equal.
+        Check if the two variables stored in the state are equal before the transition occurs.
 
         Number of input arguments: 2
         
         Number of output arguments: 0
         
         Optional input arguments: No
         
@@ -31,15 +31,15 @@
         """
         return state_variables[inputs[0]] == state_variables[inputs[1]]
 
     @staticmethod
     @parsing_decorator(input_args=2, output_args=0)
     def gt(inputs, outputs, state_variables):
         """
-        Check if the first value in the state variables is greater than the second value.
+        Check if the first value stored in the state variables is greater than the second value before the transition occurs.
 
         Number of input arguments: 2
         
         Number of output arguments: 0
         
         Optional input arguments: No
         
@@ -57,15 +57,15 @@
         """
         return state_variables[inputs[0]] > state_variables[inputs[1]]
 
     @staticmethod
     @parsing_decorator(input_args=2, output_args=0)
     def gte(inputs, outputs, state_variables):
         """
-        Check if the first value in the state variables is greater than or equal to the second value.
+        Check if the first value stored in the state variables is greater than or equal to the second value before the transition occurs.
 
         Number of input arguments: 2
         
         Number of output arguments: 0
         
         Optional input arguments: No
         
@@ -83,15 +83,15 @@
         """
         return state_variables[inputs[0]] >= state_variables[inputs[1]]
 
     @staticmethod
     @parsing_decorator(input_args=2, output_args=0)
     def lt(inputs, outputs, state_variables):
         """
-        Check if the first value in the state variables is less than the second value.
+        Check if the first value stored in the state variables is less than the second value before the transition occurs.
 
         Number of input arguments: 2
         
         Number of output arguments: 0
         
         Optional input arguments: No
         
@@ -109,15 +109,15 @@
         """
         return state_variables[inputs[0]] < state_variables[inputs[1]]
 
     @staticmethod
     @parsing_decorator(input_args=2, output_args=0)
     def lte(inputs, outputs, state_variables):
         """
-        Check if the first value in the state variables is less than or equal to the second value.
+        Check if the first value stored in the state variables is less than or equal to the second value before the transition occurs.
 
         Number of input arguments: 2
         
         Number of output arguments: 0
         
         Optional input arguments: No
```

### Comparing `nopasaran-0.2.5/nopasaran/primitives/transition_primitives/assignment_transitions.py` & `nopasaran-0.2.6/nopasaran/primitives/transition_primitives/assignment_transitions.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/sniffers/sniffer.py` & `nopasaran-0.2.6/nopasaran/sniffers/sniffer.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran/utils.py` & `nopasaran-0.2.6/nopasaran/utils.py`

 * *Files identical despite different names*

### Comparing `nopasaran-0.2.5/nopasaran.egg-info/PKG-INFO` & `nopasaran-0.2.6/nopasaran.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopasaran
-Version: 0.2.5
+Version: 0.2.6
 Summary: NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.
 Home-page: https://github.com/BenIlies/NoPASARAN
 Author: Ilies Benhabbour
 Author-email: ilies.benhabbour@kaust.edu.sa
 License: UNKNOWN
 Description: # NoPASARAN
```

### Comparing `nopasaran-0.2.5/nopasaran.egg-info/SOURCES.txt` & `nopasaran-0.2.6/nopasaran.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 nopasaran/controllers/factory.py
 nopasaran/controllers/protocol.py
 nopasaran/definitions/__init__.py
 nopasaran/definitions/commands.py
 nopasaran/definitions/control_channel.py
 nopasaran/definitions/events.py
 nopasaran/definitions/transitions.py
+nopasaran/errors/__init__.py
+nopasaran/errors/parsing_error.py
 nopasaran/interpreters/__init__.py
 nopasaran/interpreters/action_interpreter.py
 nopasaran/interpreters/condition_interpreter.py
 nopasaran/interpreters/interpreter.py
 nopasaran/interpreters/transition_interpreter.py
 nopasaran/ipsec_tunnels/__init__.py
 nopasaran/ipsec_tunnels/ipsec_conf.py
@@ -34,19 +36,21 @@
 nopasaran/parsers/interpreter_parser.py
 nopasaran/parsers/state_machine_parser.py
 nopasaran/primitives/__init__.py
 nopasaran/primitives/primitives.py
 nopasaran/primitives/action_primitives/__init__.py
 nopasaran/primitives/action_primitives/action_primitives.py
 nopasaran/primitives/action_primitives/control_channel_primitives.py
+nopasaran/primitives/action_primitives/data_channel_primitives.py
 nopasaran/primitives/action_primitives/data_manipulation.py
+nopasaran/primitives/action_primitives/event_primitives.py
+nopasaran/primitives/action_primitives/io_primitives.py
 nopasaran/primitives/action_primitives/ip_primitives.py
 nopasaran/primitives/action_primitives/nested_machine_utils.py
 nopasaran/primitives/action_primitives/tcp_primitives.py
-nopasaran/primitives/action_primitives/tmp.py
 nopasaran/primitives/action_primitives/udp_primitives.py
 nopasaran/primitives/condition_primitives/__init__.py
 nopasaran/primitives/condition_primitives/condition_primitives.py
 nopasaran/primitives/condition_primitives/variable_comparisons.py
 nopasaran/primitives/transition_primitives/__init__.py
 nopasaran/primitives/transition_primitives/assignment_transitions.py
 nopasaran/primitives/transition_primitives/transition_primitives.py
```

### Comparing `nopasaran-0.2.5/setup.py` & `nopasaran-0.2.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 requirements_file = os.path.join(os.path.dirname(__file__), "requirements.txt")
 with open(requirements_file, "r") as f:
     requirements = [str(req) for req in parse_requirements(f)]
 
 # Version will automatically be updated when pushed on the main branch
 setup(
     name="nopasaran",
-    version='0.2.5',
+    version='0.2.6',
     author="Ilies Benhabbour",
     author_email="ilies.benhabbour@kaust.edu.sa",
     description="NoPASARAN is an advanced network tool designed to detect, fingerprint, and locate network middleboxes in a unified framework.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/BenIlies/NoPASARAN",
     packages=find_packages(),
```

