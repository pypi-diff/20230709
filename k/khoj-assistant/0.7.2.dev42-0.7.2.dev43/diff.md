# Comparing `tmp/khoj_assistant-0.7.2.dev42.tar.gz` & `tmp/khoj_assistant-0.7.2.dev43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Jul  8 03:36:16 2023, max compression
+gzip compressed data, last modified: Sun Jul  9 17:12:09 2023, max compression
```

## Comparing `khoj_assistant-0.7.2.dev42.tar` & `khoj_assistant-0.7.2.dev43.tar`

### file list

```diff
@@ -1,77 +1,78 @@
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/__init__.py
--rw-r--r--   0        0        0    11048 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/configure.py
--rw-r--r--   0        0        0     5247 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     3910 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    17859 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    14688 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6930 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     7322 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0    18700 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3660 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     1813 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0      549 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0   205167 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     7946 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4222 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     4829 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     3991 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     8304 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13517 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5397 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    20657 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/routers/api.py
--rw-r--r--   0        0        0      167 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     4646 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7566 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11054 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2040 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2396 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2500 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6889 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4136 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/LICENSE
--rw-r--r--   0        0        0    24572 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/README.md
--rw-r--r--   0        0        0     2792 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/pyproject.toml
--rw-r--r--   0        0        0    26937 2023-07-08 03:36:16.000000 khoj_assistant-0.7.2.dev42/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11048 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/configure.py
+-rw-r--r--   0        0        0     5247 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     3910 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    17874 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    14688 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6930 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     7322 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0    18700 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3660 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     1813 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     7946 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4222 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     4829 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     3991 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     8304 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13517 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5397 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    19428 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/routers/api.py
+-rw-r--r--   0        0        0      167 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     2895 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0     4646 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7566 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11054 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2040 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2396 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2500 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6889 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4136 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/LICENSE
+-rw-r--r--   0        0        0    24572 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/README.md
+-rw-r--r--   0        0        0     2792 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/pyproject.toml
+-rw-r--r--   0        0        0    26937 2023-07-09 17:12:09.000000 khoj_assistant-0.7.2.dev43/PKG-INFO
```

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/configure.py` & `khoj_assistant-0.7.2.dev43/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/main.py` & `khoj_assistant-0.7.2.dev43/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/404.html` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/chat.html` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/chat.html`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
                 return;
 
             // Add message by user to chat body
             renderMessage(query, "you");
             document.getElementById("chat-input").value = "";
 
             // Generate backend API URL to execute query
-            let url = `/api/chat?q=${encodeURIComponent(query)}&n=${results_count}&client=web`;
+            let url = `/api/chat?q=${encodeURIComponent(query)}&n=${results_count}&client=web&stream=true`;
 
             let chat_body = document.getElementById("chat-body");
             let new_response = document.createElement("div");
             new_response.classList.add("chat-message", "khoj");
             new_response.attributes["data-meta"] = "🏮 Khoj at " + formatDate(new Date());
             chat_body.appendChild(new_response);
 
@@ -126,15 +126,15 @@
             // Send chat message on 'Enter'
             if (event.key === 'Enter') {
                 chat();
             }
         }
 
         window.onload = function () {
-            fetch('/api/chat/init?client=web')
+            fetch('/api/chat/history?client=web')
                 .then(response => response.json())
                 .then(data => {
                     if (data.detail) {
                         // If the server returns a 500 error with detail, render it as a message.
                         renderMessage("Hi 👋🏾, to get started <br/>1. Get your <a class='inline-chat-link' href='https://platform.openai.com/account/api-keys'>OpenAI API key</a><br/>2. Save it in the Khoj <a class='inline-chat-link' href='/config/processor/conversation'>chat settings</a> <br/>3. Click Configure on the Khoj <a class='inline-chat-link' href='/config'>settings page</a>", "khoj");
 
                         // Disable chat input field and update placeholder text
```

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/config.html` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/index.html` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.7.2.dev43/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.7.2.dev43/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.7.2.dev43/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.7.2.dev43/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.7.2.dev43/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.7.2.dev43/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.7.2.dev43/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.7.2.dev43/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.7.2.dev43/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.7.2.dev43/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.7.2.dev43/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/routers/api.py` & `khoj_assistant-0.7.2.dev43/src/khoj/routers/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 # Standard Packages
 import concurrent.futures
 import math
 import time
 import yaml
 import logging
-from datetime import datetime
+import json
 from typing import List, Optional, Union
-from functools import partial
 
 # External Packages
 from fastapi import APIRouter, HTTPException, Header, Request
 from sentence_transformers import util
 
 # Internal Packages
 from khoj.configure import configure_processor, configure_search
-from khoj.processor.conversation.gpt import converse, extract_questions
-from khoj.processor.conversation.utils import message_to_log, reciprocal_conversation_to_chatml
 from khoj.search_type import image_search, text_search
 from khoj.search_filter.date_filter import DateFilter
 from khoj.search_filter.file_filter import FileFilter
 from khoj.search_filter.word_filter import WordFilter
 from khoj.utils.config import TextSearchModel
 from khoj.utils.helpers import log_telemetry, timer
 from khoj.utils.rawconfig import (
@@ -31,15 +28,19 @@
     TextContentConfig,
     ConversationProcessorConfig,
     GithubContentConfig,
 )
 from khoj.utils.state import SearchType
 from khoj.utils import state, constants
 from khoj.utils.yaml import save_config_to_file_updated_state
-from fastapi.responses import StreamingResponse
+from fastapi.responses import StreamingResponse, Response
+from khoj.routers.helpers import perform_chat_checks, generate_chat_response
+from khoj.processor.conversation.gpt import extract_questions
+from fastapi.requests import Request
+
 
 # Initialize Router
 api = APIRouter()
 logger = logging.getLogger(__name__)
 
 # If it's a demo instance, prevent updating any of the configuration.
 if not state.demo:
@@ -404,30 +405,23 @@
             telemetry_type="api", api="update", client=client, app_config=state.config.app, properties=user_state
         )
     ]
 
     return {"status": "ok", "message": "khoj reloaded"}
 
 
-@api.get("/chat/init")
-def chat_init(
+@api.get("/chat/history")
+def chat_history(
     request: Request,
     client: Optional[str] = None,
     user_agent: Optional[str] = Header(None),
     referer: Optional[str] = Header(None),
     host: Optional[str] = Header(None),
 ):
-    if (
-        state.processor_config is None
-        or state.processor_config.conversation is None
-        or state.processor_config.conversation.openai_api_key is None
-    ):
-        raise HTTPException(
-            status_code=500, detail="Set your OpenAI API key via Khoj settings and restart it to use Khoj Chat."
-        )
+    perform_chat_checks()
 
     # Load Conversation History
     meta_log = state.processor_config.conversation.meta_log
 
     user_state = {
         "client_host": request.client.host if request.client else None,
         "user_agent": user_agent or "unknown",
@@ -440,61 +434,79 @@
             telemetry_type="api", api="chat", client=client, app_config=state.config.app, properties=user_state
         )
     ]
 
     return {"status": "ok", "response": meta_log.get("chat", [])}
 
 
-@api.get("/chat", response_class=StreamingResponse)
+@api.get("/chat", response_class=Response)
 async def chat(
     request: Request,
-    q: Optional[str] = None,
+    q: str,
     n: Optional[int] = 5,
     client: Optional[str] = None,
+    stream: Optional[bool] = False,
     user_agent: Optional[str] = Header(None),
     referer: Optional[str] = Header(None),
     host: Optional[str] = Header(None),
-) -> StreamingResponse:
-    def _save_to_conversation_log(
-        q: str,
-        gpt_response: str,
-        user_message_time: str,
-        compiled_references: List[str],
-        inferred_queries: List[str],
-        meta_log,
-    ):
-        state.processor_config.conversation.chat_session += reciprocal_conversation_to_chatml([q, gpt_response])
-        state.processor_config.conversation.meta_log["chat"] = message_to_log(
-            q,
-            gpt_response,
-            user_message_metadata={"created": user_message_time},
-            khoj_message_metadata={"context": compiled_references, "intent": {"inferred-queries": inferred_queries}},
-            conversation_log=meta_log.get("chat", []),
-        )
+) -> Response:
+    perform_chat_checks()
+    compiled_references, inferred_queries = await extract_references_and_questions(request, q, (n or 5))
+
+    # Get the (streamed) chat response from GPT.
+    gpt_response = generate_chat_response(
+        q,
+        meta_log=state.processor_config.conversation.meta_log,
+        compiled_references=compiled_references,
+        inferred_queries=inferred_queries,
+    )
+    if gpt_response is None:
+        return Response(content=gpt_response, media_type="text/plain", status_code=500)
+
+    if stream:
+        return StreamingResponse(gpt_response, media_type="text/event-stream", status_code=200)
+
+    # Get the full response from the generator if the stream is not requested.
+    aggregated_gpt_response = ""
+    while True:
+        try:
+            aggregated_gpt_response += next(gpt_response)
+        except StopIteration:
+            break
 
-    if (
-        state.processor_config is None
-        or state.processor_config.conversation is None
-        or state.processor_config.conversation.openai_api_key is None
-    ):
-        raise HTTPException(
-            status_code=500, detail="Set your OpenAI API key via Khoj settings and restart it to use Khoj Chat."
+    actual_response = aggregated_gpt_response.split("### compiled references:")[0]
+
+    response_obj = {"response": actual_response, "context": compiled_references}
+
+    user_state = {
+        "client_host": request.client.host if request.client else None,
+        "user_agent": user_agent or "unknown",
+        "referer": referer or "unknown",
+        "host": host or "unknown",
+    }
+
+    state.telemetry += [
+        log_telemetry(
+            telemetry_type="api", api="chat", client=client, app_config=state.config.app, properties=user_state
         )
+    ]
+
+    return Response(content=json.dumps(response_obj), media_type="application/json", status_code=200)
 
+
+async def extract_references_and_questions(
+    request: Request,
+    q: str,
+    n: int,
+):
     # Load Conversation History
     meta_log = state.processor_config.conversation.meta_log
 
-    # If user query is empty, return nothing
-    if not q:
-        return StreamingResponse(None)
-
     # Initialize Variables
     api_key = state.processor_config.conversation.openai_api_key
-    chat_model = state.processor_config.conversation.chat_model
-    user_message_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     conversation_type = "general" if q.startswith("@general") else "notes"
     compiled_references = []
     inferred_queries = []
 
     if conversation_type == "notes":
         # Infer search queries from user message
         with timer("Extracting search queries took", logger):
@@ -505,43 +517,8 @@
             result_list = []
             for query in inferred_queries:
                 result_list.extend(
                     await search(query, request=request, n=n, r=True, score_threshold=-5.0, dedupe=False)
                 )
             compiled_references = [item.additional["compiled"] for item in result_list]
 
-    # Switch to general conversation type if no relevant notes found for the given query
-    conversation_type = "notes" if compiled_references else "general"
-    logger.debug(f"Conversation Type: {conversation_type}")
-
-    user_state = {
-        "client_host": request.client.host if request.client else None,
-        "user_agent": user_agent or "unknown",
-        "referer": referer or "unknown",
-        "host": host or "unknown",
-    }
-
-    state.telemetry += [
-        log_telemetry(
-            telemetry_type="api", api="chat", client=client, app_config=state.config.app, properties=user_state
-        )
-    ]
-
-    try:
-        with timer("Generating chat response took", logger):
-            partial_completion = partial(
-                _save_to_conversation_log,
-                q,
-                user_message_time=user_message_time,
-                compiled_references=compiled_references,
-                inferred_queries=inferred_queries,
-                meta_log=meta_log,
-            )
-
-            gpt_response = converse(
-                compiled_references, q, meta_log, model=chat_model, api_key=api_key, completion_func=partial_completion
-            )
-
-    except Exception as e:
-        gpt_response = str(e)
-
-    return StreamingResponse(gpt_response, media_type="text/event-stream", status_code=200)
+    return compiled_references, inferred_queries
```

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/routers/web_client.py` & `khoj_assistant-0.7.2.dev43/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.7.2.dev43/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.7.2.dev43/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.7.2.dev43/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.7.2.dev43/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/search_type/image_search.py` & `khoj_assistant-0.7.2.dev43/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/search_type/text_search.py` & `khoj_assistant-0.7.2.dev43/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/utils/cli.py` & `khoj_assistant-0.7.2.dev43/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/utils/config.py` & `khoj_assistant-0.7.2.dev43/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/utils/constants.py` & `khoj_assistant-0.7.2.dev43/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/utils/helpers.py` & `khoj_assistant-0.7.2.dev43/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/utils/jsonl.py` & `khoj_assistant-0.7.2.dev43/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/utils/models.py` & `khoj_assistant-0.7.2.dev43/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.7.2.dev43/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/utils/state.py` & `khoj_assistant-0.7.2.dev43/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/src/khoj/utils/yaml.py` & `khoj_assistant-0.7.2.dev43/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/.gitignore` & `khoj_assistant-0.7.2.dev43/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/LICENSE` & `khoj_assistant-0.7.2.dev43/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/README.md` & `khoj_assistant-0.7.2.dev43/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/pyproject.toml` & `khoj_assistant-0.7.2.dev43/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.7.2.dev42/PKG-INFO` & `khoj_assistant-0.7.2.dev43/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.7.2.dev42
+Version: 0.7.2.dev43
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
```

