# Comparing `tmp/openai_function_call-0.0.5.tar.gz` & `tmp/openai_function_call-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function_call-0.0.5.tar", max compression
+gzip compressed data, was "openai_function_call-0.1.1.tar", max compression
```

## Comparing `openai_function_call-0.0.5.tar` & `openai_function_call-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,13 @@
--rw-r--r--   0        0        0     1066 2023-06-23 05:16:05.515143 openai_function_call-0.0.5/LICENSE
--rw-r--r--   0        0        0     3702 2023-06-23 05:16:05.515143 openai_function_call-0.0.5/README.md
--rw-r--r--   0        0        0     4155 2023-06-23 05:16:05.515143 openai_function_call-0.0.5/openai_function_call/__init__.py
--rw-r--r--   0        0        0      505 2023-06-23 05:16:05.515143 openai_function_call-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4436 1970-01-01 00:00:00.000000 openai_function_call-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-08 18:19:43.018939 openai_function_call-0.1.1/LICENSE
+-rw-r--r--   0        0        0     8289 2023-07-09 04:09:54.978582 openai_function_call-0.1.1/README.md
+-rw-r--r--   0        0        0      187 2023-07-08 18:19:43.033586 openai_function_call-0.1.1/openai_function_call/__init__.py
+-rw-r--r--   0        0        0      151 2023-07-08 18:19:43.034089 openai_function_call-0.1.1/openai_function_call/dsl/__init__.py
+-rw-r--r--   0        0        0     5773 2023-07-08 18:19:43.034296 openai_function_call-0.1.1/openai_function_call/dsl/completion.py
+-rw-r--r--   0        0        0      505 2023-07-08 18:19:43.034803 openai_function_call-0.1.1/openai_function_call/dsl/messages/__init__.py
+-rw-r--r--   0        0        0     1669 2023-07-08 18:19:43.035000 openai_function_call-0.1.1/openai_function_call/dsl/messages/base.py
+-rw-r--r--   0        0        0     3260 2023-07-08 18:19:43.035533 openai_function_call-0.1.1/openai_function_call/dsl/messages/messages.py
+-rw-r--r--   0        0        0     1486 2023-07-08 18:19:43.035798 openai_function_call-0.1.1/openai_function_call/dsl/messages/user.py
+-rw-r--r--   0        0        0     2202 2023-07-08 18:19:43.036083 openai_function_call-0.1.1/openai_function_call/dsl/multitask.py
+-rw-r--r--   0        0        0     6151 2023-07-08 18:19:43.036753 openai_function_call-0.1.1/openai_function_call/function_calls.py
+-rw-r--r--   0        0        0      663 2023-07-09 04:59:47.039821 openai_function_call-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9023 1970-01-01 00:00:00.000000 openai_function_call-0.1.1/PKG-INFO
```

### Comparing `openai_function_call-0.0.5/LICENSE` & `openai_function_call-0.1.1/LICENSE`

 * *Files identical despite different names*

