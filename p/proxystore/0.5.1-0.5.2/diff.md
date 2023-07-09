# Comparing `tmp/proxystore-0.5.1.tar.gz` & `tmp/proxystore-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxystore-0.5.1.tar", last modified: Thu Jun  8 01:01:09 2023, max compression
+gzip compressed data, was "proxystore-0.5.2.tar", last modified: Sun Jul  9 00:17:59 2023, max compression
```

## Comparing `proxystore-0.5.1.tar` & `proxystore-0.5.2.tar`

### file list

```diff
@@ -1,235 +1,235 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.569710 proxystore-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/ISSUE_TEMPLATE/01_bug.yml
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/ISSUE_TEMPLATE/02_feature.yml
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/ISSUE_TEMPLATE/03_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/release.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/cache.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/check-docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-08 01:01:00.000000 proxystore-0.5.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-08 01:01:00.000000 proxystore-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-08 01:01:00.000000 proxystore-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-08 01:01:00.000000 proxystore-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-08 01:01:09.569710 proxystore-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-08 01:01:00.000000 proxystore-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/docs/_overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/_overrides/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.545709 proxystore-0.5.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.545709 proxystore-0.5.1/docs/_templates/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/docs/_templates/python/material/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/docs/_templates/python/material/docstring/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/_templates/python/material/docstring/admonition.html
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/_templates/python/material/function.html
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/_templates/python/material/module.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.549709 proxystore-0.5.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/api/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/api/legacy-docs.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/concepts/connector.md
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/concepts/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/concepts/proxy.md
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/concepts/store.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/contributing/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/contributing/issues-pull-requests.md
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/contributing/releases.md
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/contributing/style-guide.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/css/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/css/mkdocstrings.css
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/generate_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/get-started.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/guides/endpoints-debugging.md
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/guides/endpoints.md
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/guides/globus-compute.md
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/guides/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/guides/performance.md
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/known-issues.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/publications/
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/publications/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)   134472 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/endpoint-overview.svg
--rw-r--r--   0 runner    (1001) docker     (123)   149176 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/endpoint-peering.svg
--rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)    45464 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    31401 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    31236 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/logo-light.png
--rw-r--r--   0 runner    (1001) docker     (123)   106893 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/proxystore-overview.svg
--rw-r--r--   0 runner    (1001) docker     (123)   106939 2023-06-08 01:01:00.000000 proxystore-0.5.1/docs/static/proxystore-schematic.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.553709 proxystore-0.5.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/examples/globus-compute/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/globus-compute/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/globus-compute/mapreduce_globus_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/globus-compute/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/examples/parsl/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/parsl/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/parsl/mapreduce_parsl.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/parsl/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-08 01:01:00.000000 proxystore-0.5.1/examples/store_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-08 01:01:00.000000 proxystore-0.5.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/proxystore/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/proxystore/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/proxystore/connectors/dim/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/margo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/ucx.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/dim/zmq.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    23197 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/connectors/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.561710 proxystore-0.5.1/proxystore/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12712 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/endpoint/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/globus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.561710 proxystore-0.5.1/proxystore/p2p/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/counter.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/relay_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/p2p/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.561710 proxystore-0.5.1/proxystore/store/
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/store/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-08 01:01:00.000000 proxystore-0.5.1/proxystore/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.557709 proxystore-0.5.1/proxystore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 01:01:09.000000 proxystore-0.5.1/proxystore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-08 01:01:00.000000 proxystore-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 01:01:09.569710 proxystore-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/testing/mocked/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocked/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocked/globus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocked/pymargo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocked/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocked/ucx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/mocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/relay_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/testing/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/scripts/peer_connection_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/scripts/peer_endpoint_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/scripts/peer_manager_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 01:01:00.000000 proxystore-0.5.1/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/tests/connectors/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/connector_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.565709 proxystore-0.5.1/tests/connectors/dim/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/dim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/dim/margo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/dim/ucx_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/dim/zmq_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/endpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/file_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/globus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/local_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/multi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/connectors/redis_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.569710 proxystore-0.5.1/tests/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/commands_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/endpoint_peering_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/endpoint_solo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/serve_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/endpoint/storage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/factory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/globus_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.569710 proxystore-0.5.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/integration/endpoints_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.569710 proxystore-0.5.1/tests/p2p/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/chunks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/counter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/messages_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/relay_cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/relay_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/relay_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/p2p/task_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/serialization_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:01:09.569710 proxystore-0.5.1/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/cache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/init_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/shims_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/store_basics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/store_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/store_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/store/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/timer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-08 01:01:00.000000 proxystore-0.5.1/tests/utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-08 01:01:00.000000 proxystore-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.934738 proxystore-0.5.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.914738 proxystore-0.5.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.914738 proxystore-0.5.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/ISSUE_TEMPLATE/01_bug.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/ISSUE_TEMPLATE/02_feature.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/ISSUE_TEMPLATE/03_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/release.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.914738 proxystore-0.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/workflows/cache.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/workflows/check-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/workflows/integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-09 00:17:50.000000 proxystore-0.5.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-09 00:17:50.000000 proxystore-0.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-09 00:17:50.000000 proxystore-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-09 00:17:50.000000 proxystore-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-09 00:17:59.934738 proxystore-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-09 00:17:50.000000 proxystore-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.918738 proxystore-0.5.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.918738 proxystore-0.5.2/docs/_overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/_overrides/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.910738 proxystore-0.5.2/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.910738 proxystore-0.5.2/docs/_templates/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.918738 proxystore-0.5.2/docs/_templates/python/material/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.918738 proxystore-0.5.2/docs/_templates/python/material/docstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/_templates/python/material/docstring/admonition.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/_templates/python/material/function.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/_templates/python/material/module.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.918738 proxystore-0.5.2/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/api/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/api/legacy-docs.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.918738 proxystore-0.5.2/docs/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/concepts/connector.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/concepts/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/concepts/proxy.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/concepts/store.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.918738 proxystore-0.5.2/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/contributing/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/contributing/issues-pull-requests.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/contributing/releases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/contributing/style-guide.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.918738 proxystore-0.5.2/docs/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/css/mkdocstrings.css
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/generate_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/get-started.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.918738 proxystore-0.5.2/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/guides/endpoints-debugging.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/guides/endpoints.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/guides/globus-compute.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/guides/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/guides/performance.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/known-issues.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.918738 proxystore-0.5.2/docs/publications/
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/publications/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.922738 proxystore-0.5.2/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   134472 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/static/endpoint-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   149176 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/static/endpoint-peering.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    46990 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45464 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/static/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31401 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31236 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/static/logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (123)   106893 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/static/proxystore-overview.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   106939 2023-07-09 00:17:50.000000 proxystore-0.5.2/docs/static/proxystore-schematic.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.922738 proxystore-0.5.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-09 00:17:50.000000 proxystore-0.5.2/examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-09 00:17:50.000000 proxystore-0.5.2/examples/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.922738 proxystore-0.5.2/examples/globus-compute/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-09 00:17:50.000000 proxystore-0.5.2/examples/globus-compute/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-09 00:17:50.000000 proxystore-0.5.2/examples/globus-compute/mapreduce_globus_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-09 00:17:50.000000 proxystore-0.5.2/examples/globus-compute/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.922738 proxystore-0.5.2/examples/parsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-09 00:17:50.000000 proxystore-0.5.2/examples/parsl/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-09 00:17:50.000000 proxystore-0.5.2/examples/parsl/mapreduce_parsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-09 00:17:50.000000 proxystore-0.5.2/examples/parsl/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-09 00:17:50.000000 proxystore-0.5.2/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-09 00:17:50.000000 proxystore-0.5.2/examples/store_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-09 00:17:50.000000 proxystore-0.5.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.922738 proxystore-0.5.2/proxystore/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.922738 proxystore-0.5.2/proxystore/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.926738 proxystore-0.5.2/proxystore/connectors/dim/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/dim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/dim/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19432 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/dim/margo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/dim/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18547 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/dim/ucx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/dim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/dim/zmq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23675 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/connectors/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.926738 proxystore-0.5.2/proxystore/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/endpoint/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/endpoint/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/endpoint/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/endpoint/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/endpoint/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17312 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/endpoint/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/endpoint/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/endpoint/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/endpoint/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/endpoint/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/globus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.926738 proxystore-0.5.2/proxystore/p2p/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/p2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/p2p/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15123 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/p2p/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/p2p/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/p2p/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14235 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/p2p/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/p2p/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/p2p/relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/p2p/relay_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/p2p/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6366 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.930738 proxystore-0.5.2/proxystore/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/store/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-09 00:17:50.000000 proxystore-0.5.2/proxystore/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.922738 proxystore-0.5.2/proxystore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-09 00:17:59.000000 proxystore-0.5.2/proxystore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-07-09 00:17:59.000000 proxystore-0.5.2/proxystore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 00:17:59.000000 proxystore-0.5.2/proxystore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-09 00:17:59.000000 proxystore-0.5.2/proxystore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-09 00:17:59.000000 proxystore-0.5.2/proxystore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-09 00:17:59.000000 proxystore-0.5.2/proxystore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-09 00:17:50.000000 proxystore-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 00:17:59.934738 proxystore-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.930738 proxystore-0.5.2/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.930738 proxystore-0.5.2/testing/mocked/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/mocked/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/mocked/globus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/mocked/pymargo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/mocked/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/mocked/ucx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/mocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/relay_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.930738 proxystore-0.5.2/testing/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/scripts/peer_connection_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/scripts/peer_endpoint_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/scripts/peer_manager_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-09 00:17:50.000000 proxystore-0.5.2/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.930738 proxystore-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.930738 proxystore-0.5.2/tests/connectors/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/connector_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.930738 proxystore-0.5.2/tests/connectors/dim/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/dim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/dim/margo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/dim/ucx_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/dim/zmq_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/endpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/globus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/local_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/multi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/connectors/redis_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.934738 proxystore-0.5.2/tests/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/endpoint/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/endpoint/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14342 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/endpoint/commands_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/endpoint/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/endpoint/endpoint_peering_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/endpoint/endpoint_solo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/endpoint/serve_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/endpoint/storage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/factory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/globus_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.934738 proxystore-0.5.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/integration/endpoints_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.934738 proxystore-0.5.2/tests/p2p/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/p2p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/p2p/chunks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7568 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/p2p/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/p2p/counter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9470 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/p2p/manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/p2p/messages_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/p2p/relay_cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/p2p/relay_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/p2p/relay_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/p2p/task_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/serialization_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:17:59.934738 proxystore-0.5.2/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/store/cache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/store/init_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/store/metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/store/shims_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/store/store_basics_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/store/store_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/store/store_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/store/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/timer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-07-09 00:17:50.000000 proxystore-0.5.2/tests/utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-09 00:17:50.000000 proxystore-0.5.2/tox.ini
```

### Comparing `proxystore-0.5.1/.github/ISSUE_TEMPLATE/01_bug.yml` & `proxystore-0.5.2/.github/ISSUE_TEMPLATE/01_bug.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/.github/ISSUE_TEMPLATE/02_feature.yml` & `proxystore-0.5.2/.github/ISSUE_TEMPLATE/02_feature.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/.github/release.yml` & `proxystore-0.5.2/.github/release.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/.github/workflows/cache.yml` & `proxystore-0.5.2/.github/workflows/cache.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/.github/workflows/check-docs.yml` & `proxystore-0.5.2/.github/workflows/check-docs.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/.github/workflows/docs.yml` & `proxystore-0.5.2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/.github/workflows/integration.yml` & `proxystore-0.5.2/.github/workflows/integration.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/.github/workflows/publish.yml` & `proxystore-0.5.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/.github/workflows/tests.yml` & `proxystore-0.5.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/.gitignore` & `proxystore-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/.pre-commit-config.yaml` & `proxystore-0.5.2/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -13,29 +13,30 @@
       - id: check-merge-conflict
       - id: name-tests-test
   - repo: 'https://github.com/psf/black'
     rev: 23.3.0
     hooks:
       - id: black
   - repo: 'https://github.com/codespell-project/codespell'
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
   - repo: 'https://github.com/charliermarsh/ruff-pre-commit'
-    rev: v0.0.270
+    rev: v0.0.276
     hooks:
       - id: ruff
         args:
           - '--fix'
           - '--exit-non-zero-on-fix'
   - repo: 'https://github.com/pre-commit/mirrors-mypy'
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         additional_dependencies:
+          - click >= 8.1.0, != 8.1.4
           - globus-sdk
           - parsl
           - quart
           - types-redis
           - types-requests
           - uvicorn
           - websockets
```

### Comparing `proxystore-0.5.1/LICENSE` & `proxystore-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/PKG-INFO` & `proxystore-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxystore
-Version: 0.5.1
+Version: 0.5.2
 Summary: Lazy object proxy interface for distributed stores.
 Author: Globus Labs
 Author-email: Greg Pauloski <jgpauloski@uchicago.edu>
 Maintainer-email: Greg Pauloski <jgpauloski@uchicago.edu>, Valerie Hayot-Sasson <vhayot@uchicago.edu>
 License: FILE
 Project-URL: homepage, https://proxystore.dev
 Project-URL: documentation, https://docs.proxystore.dev
@@ -21,14 +21,15 @@
 Provides-Extra: zmq
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # ProxyStore
 
+[![DOI](https://zenodo.org/badge/357984234.svg)](https://zenodo.org/badge/latestdoi/357984234)
 [![docs](https://github.com/proxystore/proxystore/actions/workflows/docs.yml/badge.svg)](https://github.com/proxystore/proxystore/actions/workflows/docs.yml)
 [![tests](https://github.com/proxystore/proxystore/actions/workflows/tests.yml/badge.svg?label=tests)](https://github.com/proxystore/proxystore/actions)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/proxystore/proxystore/main.svg)](https://results.pre-commit.ci/latest/github/proxystore/proxystore/main)
 
 ProxyStore provides pass-by-reference semantics for distributed Python
 applications through transparent object proxies. Moving data via proxies
 (1) decouples control flow from data flow, (2) enables producers to
```

### Comparing `proxystore-0.5.1/README.md` & `proxystore-0.5.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # ProxyStore
 
+[![DOI](https://zenodo.org/badge/357984234.svg)](https://zenodo.org/badge/latestdoi/357984234)
 [![docs](https://github.com/proxystore/proxystore/actions/workflows/docs.yml/badge.svg)](https://github.com/proxystore/proxystore/actions/workflows/docs.yml)
 [![tests](https://github.com/proxystore/proxystore/actions/workflows/tests.yml/badge.svg?label=tests)](https://github.com/proxystore/proxystore/actions)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/proxystore/proxystore/main.svg)](https://results.pre-commit.ci/latest/github/proxystore/proxystore/main)
 
 ProxyStore provides pass-by-reference semantics for distributed Python
 applications through transparent object proxies. Moving data via proxies
 (1) decouples control flow from data flow, (2) enables producers to
```

### Comparing `proxystore-0.5.1/docs/_templates/python/material/function.html` & `proxystore-0.5.2/docs/_templates/python/material/function.html`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/_templates/python/material/module.html` & `proxystore-0.5.2/docs/_templates/python/material/module.html`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/api/cli.md` & `proxystore-0.5.2/docs/api/cli.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/concepts/connector.md` & `proxystore-0.5.2/docs/concepts/connector.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/concepts/index.md` & `proxystore-0.5.2/docs/concepts/index.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/concepts/proxy.md` & `proxystore-0.5.2/docs/concepts/proxy.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/concepts/store.md` & `proxystore-0.5.2/docs/concepts/store.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/contributing/index.md` & `proxystore-0.5.2/docs/contributing/index.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/contributing/issues-pull-requests.md` & `proxystore-0.5.2/docs/contributing/issues-pull-requests.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/contributing/releases.md` & `proxystore-0.5.2/docs/contributing/releases.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/contributing/style-guide.md` & `proxystore-0.5.2/docs/contributing/style-guide.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/css/extra.css` & `proxystore-0.5.2/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/css/mkdocstrings.css` & `proxystore-0.5.2/docs/css/mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/examples.md` & `proxystore-0.5.2/docs/examples.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/generate_api.py` & `proxystore-0.5.2/docs/generate_api.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/get-started.md` & `proxystore-0.5.2/docs/get-started.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/guides/endpoints-debugging.md` & `proxystore-0.5.2/docs/guides/endpoints-debugging.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/guides/endpoints.md` & `proxystore-0.5.2/docs/guides/endpoints.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/guides/globus-compute.md` & `proxystore-0.5.2/docs/guides/globus-compute.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/guides/performance.md` & `proxystore-0.5.2/docs/guides/performance.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/installation.md` & `proxystore-0.5.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/known-issues.md` & `proxystore-0.5.2/docs/known-issues.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     * Affected versions: `>=0.4.0,<0.6.0`
     * Python 3.7 support will be removed in `0.6.0`. See [Issue #236](https://github.com/proxystore/proxystore/issues/236){target=_blank}.
 
 ## MyPy
 
 ### Implicit re-exports
 
+*Affected versions:* `<=0.5.1`
+
 Examples throughout the documentation generally suggest importing
 [`Store`][proxystore.store.base.Store] like the following.
 ```python title="example.py"
 from proxystore.store import Store
 ```
 
 MyPy will raise an attribute defined error if run with `--no-implicit-reexport`.
```

### Comparing `proxystore-0.5.1/docs/publications/index.md` & `proxystore-0.5.2/docs/publications/index.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/static/endpoint-overview.svg` & `proxystore-0.5.2/docs/static/endpoint-overview.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/static/endpoint-peering.svg` & `proxystore-0.5.2/docs/static/endpoint-peering.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/static/favicon.png` & `proxystore-0.5.2/docs/static/favicon.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/static/icon.png` & `proxystore-0.5.2/docs/static/icon.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/static/logo-dark.png` & `proxystore-0.5.2/docs/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/static/logo-light.png` & `proxystore-0.5.2/docs/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/static/proxystore-overview.svg` & `proxystore-0.5.2/docs/static/proxystore-overview.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/docs/static/proxystore-schematic.svg` & `proxystore-0.5.2/docs/static/proxystore-schematic.svg`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/examples/README.md` & `proxystore-0.5.2/examples/README.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/examples/globus-compute/README.md` & `proxystore-0.5.2/examples/globus-compute/README.md`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/examples/globus-compute/mapreduce_globus_compute.py` & `proxystore-0.5.2/examples/globus-compute/mapreduce_globus_compute.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/examples/globus-compute/run.sh` & `proxystore-0.5.2/examples/globus-compute/run.sh`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/examples/parsl/mapreduce_parsl.py` & `proxystore-0.5.2/examples/parsl/mapreduce_parsl.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/examples/parsl/run.sh` & `proxystore-0.5.2/examples/parsl/run.sh`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/examples/store_metrics.py` & `proxystore-0.5.2/examples/store_metrics.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/mkdocs.yml` & `proxystore-0.5.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/__init__.py` & `proxystore-0.5.2/proxystore/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/__init__.py` & `proxystore-0.5.2/proxystore/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/connector.py` & `proxystore-0.5.2/proxystore/connectors/connector.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/dim/margo.py` & `proxystore-0.5.2/proxystore/connectors/dim/margo.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/dim/models.py` & `proxystore-0.5.2/proxystore/connectors/dim/models.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/dim/ucx.py` & `proxystore-0.5.2/proxystore/connectors/dim/ucx.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/dim/utils.py` & `proxystore-0.5.2/proxystore/connectors/dim/utils.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/dim/zmq.py` & `proxystore-0.5.2/proxystore/connectors/dim/zmq.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/endpoint.py` & `proxystore-0.5.2/proxystore/connectors/endpoint.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/file.py` & `proxystore-0.5.2/proxystore/connectors/file.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/globus.py` & `proxystore-0.5.2/proxystore/connectors/globus.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,19 +239,21 @@
 
 
 class GlobusKey(NamedTuple):
     """Key to object transferred with Globus.
 
     Attributes:
         filename: Unique object filename.
-        task_id: Globus transfer task ID for the file.
+        task_id: Globus transfer task IDs for the file.
     """
 
     filename: str
-    task_id: str
+    # We support single strings for backwards compatibility with
+    # proxies created in v0.5.1 or older.
+    task_id: str | tuple[str, ...]
 
     def __eq__(self, other: Any) -> bool:
         """Match keys by filename only.
 
         This is a hack around the fact that the task_id is not created until
         after the filename is so there can be a state where the task_id
         is empty.
@@ -285,27 +287,29 @@
         performed on the command line with `#!bash proxystore-globus-auth`.
         Authentication only needs to be performed once per system.
 
     Args:
         endpoints: Globus endpoints to keep in sync. If passed as a `dict`,
             the dictionary must match the format expected by
             [`GlobusEndpoints.from_dict()`][proxystore.store.globus.GlobusEndpoints.from_dict].
+            Note that given `n` endpoints there will be `n-1` Globus transfers
+            per operation, so we suggest not using too many endpoints at the
+            same time.
         polling_interval: Interval in seconds to check if Globus
             tasks have finished.
         sync_level: Globus transfer sync level.
         timeout: Timeout in seconds for waiting on Globus tasks.
         clear: Clear all objects on
             [`close()`][proxystore.connectors.globus.GlobusConnector.close] by
             deleting the `local_path` of each endpoint.
 
     Raises:
         GlobusAuthFileError: If the Globus authentication file cannot be found.
         ValueError: If `endpoints` is of an incorrect type.
-        ValueError: If the `#!python len(endpoints) != 2` because this
-            implementation can currently only keep two endpoints in sync.
+        ValueError: If fewer than two endpoints are provided.
     """
 
     def __init__(
         self,
         endpoints: GlobusEndpoints
         | list[GlobusEndpoint]
         | dict[str, dict[str, str]],
@@ -322,18 +326,16 @@
         elif isinstance(endpoints, dict):
             self.endpoints = GlobusEndpoints.from_dict(endpoints)
         else:
             raise ValueError(
                 'endpoints must be of type GlobusEndpoints or a list of '
                 f'GlobusEndpoint. Got {type(endpoints)}.',
             )
-        if len(endpoints) != 2:
-            raise ValueError(
-                'ProxyStore only supports two endpoints at a time',
-            )
+        if len(endpoints) < 2:
+            raise ValueError('At least two Globus endpoints are required.')
         self.polling_interval = polling_interval
         self.sync_level = sync_level
         self.timeout = timeout
         self.clear = clear
 
         try:
             authorizer = get_proxystore_authorizer()
@@ -382,100 +384,103 @@
         local_path = os.path.expanduser(endpoint.local_path)
         return os.path.join(local_path, filename)
 
     def _get_local_endpoint(self) -> GlobusEndpoint:
         """Get endpoint local to current host."""
         return self.endpoints.get_by_host(hostname())
 
-    def _validate_task_id(self, task_id: str) -> bool:
+    def _validate_task_id(self, task_ids: str | tuple[str, ...]) -> bool:
         """Validate key contains a real Globus task id."""
-        try:
-            self._transfer_client.get_task(task_id)
-        except globus_sdk.TransferAPIError as e:
-            if e.http_status == 400:
-                return False
-            raise e
+        task_ids = task_ids if isinstance(task_ids, tuple) else (task_ids,)
+        for tid in task_ids:
+            try:
+                self._transfer_client.get_task(tid)
+            except globus_sdk.TransferAPIError as e:
+                if e.http_status == 400:
+                    return False
+                raise e
         return True
 
-    def _wait_on_tasks(self, *tasks: str) -> None:
+    def _wait_on_tasks(self, task_ids: str | tuple[str, ...]) -> None:
         """Wait on list of Globus tasks."""
-        for task in tasks:
+        task_ids = task_ids if isinstance(task_ids, tuple) else (task_ids,)
+        for tid in task_ids:
             done = self._transfer_client.task_wait(
-                task,
+                tid,
                 timeout=self.timeout,
                 polling_interval=self.polling_interval,
             )
             if not done:
                 raise RuntimeError(
-                    f'Task {task} did not complete within the timeout',
+                    f'Task {tid} did not complete within the timeout',
                 )
 
     def _transfer_files(
         self,
         filenames: str | list[str],
         delete: bool = False,
-    ) -> str:
-        """Launch Globus Transfer to sync endpoints.
+    ) -> tuple[str, ...]:
+        """Launch Globus Transfers to sync endpoints.
 
         Args:
             filenames: Filename or list of filenames to transfer.
                 Note must be filenames, not filepaths.
             delete: If `True`, delete the filenames rather than syncing them.
 
         Returns:
-            Globus Task UUID that can be used to check the status of the \
-            transfer.
+            Tuple of Globus Task UUID that can be used to check the status of
+            the transfers.
         """
         src_endpoint = self._get_local_endpoint()
         dst_endpoints = [ep for ep in self.endpoints if ep != src_endpoint]
-        assert len(dst_endpoints) == 1
-        dst_endpoint = dst_endpoints[0]
-
-        transfer_task: globus_sdk.DeleteData | globus_sdk.TransferData
-        if delete:
-            transfer_task = globus_sdk.DeleteData(
-                self._transfer_client,
-                endpoint=dst_endpoint.uuid,
-            )
-        else:
-            transfer_task = globus_sdk.TransferData(
-                self._transfer_client,
-                source_endpoint=src_endpoint.uuid,
-                destination_endpoint=dst_endpoint.uuid,
-                sync_level=self.sync_level,
-            )
+        tids: list[str] = []
 
-        transfer_task['notify_on_succeeded'] = False
-        transfer_task['notify_on_failed'] = False
-        transfer_task['notify_on_inactive'] = False
-
-        if isinstance(filenames, str):
-            filenames = [filenames]
-
-        for filename in filenames:
-            if isinstance(transfer_task, globus_sdk.DeleteData):
-                transfer_task.add_item(
-                    path=os.path.join(dst_endpoint.endpoint_path, filename),
-                )
-            elif isinstance(transfer_task, globus_sdk.TransferData):
-                transfer_task.add_item(
-                    source_path=os.path.join(
-                        src_endpoint.endpoint_path,
-                        filename,
-                    ),
-                    destination_path=os.path.join(
-                        dst_endpoint.endpoint_path,
-                        filename,
-                    ),
+        for dst_endpoint in dst_endpoints:
+            transfer_task: globus_sdk.DeleteData | globus_sdk.TransferData
+            if delete:
+                transfer_task = globus_sdk.DeleteData(
+                    self._transfer_client,
+                    endpoint=dst_endpoint.uuid,
                 )
             else:
-                raise AssertionError('Unreachable.')
+                transfer_task = globus_sdk.TransferData(
+                    self._transfer_client,
+                    source_endpoint=src_endpoint.uuid,
+                    destination_endpoint=dst_endpoint.uuid,
+                    sync_level=self.sync_level,
+                )
+
+            transfer_task['notify_on_succeeded'] = False
+            transfer_task['notify_on_failed'] = False
+            transfer_task['notify_on_inactive'] = False
+
+            if isinstance(filenames, str):
+                filenames = [filenames]
+
+            for filename in filenames:
+                src_path = os.path.join(src_endpoint.endpoint_path, filename)
+                dst_path = os.path.join(dst_endpoint.endpoint_path, filename)
+
+                if isinstance(transfer_task, globus_sdk.DeleteData):
+                    transfer_task.add_item(path=dst_path)
+                elif isinstance(transfer_task, globus_sdk.TransferData):
+                    transfer_task.add_item(
+                        source_path=src_path,
+                        destination_path=dst_path,
+                    )
+                else:
+                    raise AssertionError('Unreachable.')
+
+            tdata = _submit_transfer_action(
+                self._transfer_client,
+                transfer_task,
+            )
+            tids.append(tdata['task_id'])
 
-        tdata = _submit_transfer_action(self._transfer_client, transfer_task)
-        return tdata['task_id']
+        return tuple(tids)
 
     def close(self, clear: bool | None = None) -> None:
         """Close the connector and clean up.
 
         Warning:
             This will delete the directory at `local_path` on each endpoint
             by default.
@@ -604,17 +609,17 @@
 
         path = self._get_filepath(filename)
         os.makedirs(os.path.dirname(path), exist_ok=True)
 
         with open(path, 'wb', buffering=0) as f:
             f.write(obj)
 
-        task_id = self._transfer_files(filename)
+        tids = self._transfer_files(filename)
 
-        return GlobusKey(filename=filename, task_id=task_id)
+        return GlobusKey(filename=filename, task_id=tids)
 
     def put_batch(self, objs: Sequence[bytes]) -> list[GlobusKey]:
         """Put a batch of serialized objects in the store.
 
         Args:
             objs: Sequence of serialized objects to put in the store.
 
@@ -627,18 +632,18 @@
         for filename, obj in zip(filenames, objs):
             path = self._get_filepath(filename)
             os.makedirs(os.path.dirname(path), exist_ok=True)
 
             with open(path, 'wb', buffering=0) as f:
                 f.write(obj)
 
-        task_id = self._transfer_files(filenames)
+        tids = self._transfer_files(filenames)
 
         return [
-            GlobusKey(filename=filename, task_id=task_id)
+            GlobusKey(filename=filename, task_id=tids)
             for filename in filenames
         ]
 
 
 def _submit_transfer_action(
     client: globus_sdk.TransferClient,
     task: globus_sdk.DeleteData | globus_sdk.TransferData,
```

### Comparing `proxystore-0.5.1/proxystore/connectors/local.py` & `proxystore-0.5.2/proxystore/connectors/local.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/multi.py` & `proxystore-0.5.2/proxystore/connectors/multi.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/connectors/redis.py` & `proxystore-0.5.2/proxystore/connectors/redis.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/endpoint/__init__.py` & `proxystore-0.5.2/proxystore/endpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/endpoint/cli.py` & `proxystore-0.5.2/proxystore/endpoint/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 from __future__ import annotations
 
 import logging
 import os
 import sys
 import uuid
+from typing import ClassVar
 
 import click
 import requests
 
 import proxystore
 from proxystore.endpoint import client
 from proxystore.endpoint.commands import configure_endpoint
@@ -38,15 +39,15 @@
     red = '\x1b[0;31m'
     green = '\x1b[0;32m'
     yellow = '\x1b[0;33m'
     cyan = '\x1b[0;36m'
     bold_red = '\x1b[1;31m'
     reset = '\x1b[0m'
 
-    FORMATS = {
+    FORMATS: ClassVar[dict[int, str]] = {
         logging.DEBUG: f'{cyan}DEBUG:{reset} %(message)s',
         logging.INFO: f'{green}INFO:{reset} %(message)s',
         logging.WARNING: f'{yellow}WARNING:{reset} %(message)s',
         logging.ERROR: f'{red}ERROR:{reset} %(message)s',
         logging.CRITICAL: f'{bold_red}CRITICAL:{reset} %(message)s',
     }
```

### Comparing `proxystore-0.5.1/proxystore/endpoint/client.py` & `proxystore-0.5.2/proxystore/endpoint/client.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/endpoint/commands.py` & `proxystore-0.5.2/proxystore/endpoint/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,27 +173,43 @@
         are logged to the default logger.
     """
     if proxystore_dir is None:
         proxystore_dir = home_dir()
 
     endpoints = get_configs(proxystore_dir)
 
+    max_status_chars = max(
+        len('STATUS'),
+        *(len(e.name) for e in EndpointStatus),
+    )
+    # Note: endpoints can be empty so we need to pass an iterable rather
+    # than unpacking the arguments
+    max_endpoint_chars = max([18] + [len(e.name) for e in endpoints])
+
     if len(endpoints) == 0:
         logger.info(f'No valid endpoint configurations in {proxystore_dir}.')
-    else:
-        eps = [(e.name, str(e.uuid)) for e in endpoints]
-        eps = sorted(eps, key=lambda x: x[0])
-        logger.info(f'{"NAME":<18} {"STATUS":<8} UUID', extra={'simple': True})
-        logger.info('=' * (19 + 9 + len(eps[0][1])), extra={'simple': True})
-        for name, uuid_ in eps:
-            status = get_status(name, proxystore_dir)
-            logger.info(
-                f'{name:18.18} {status.name:<8.8} {uuid_}',
-                extra={'simple': True},
-            )
+        return 0
+
+    eps = [(e.name, str(e.uuid)) for e in endpoints]
+    eps = sorted(eps, key=lambda x: x[0])
+    logger.info(
+        f'{"NAME":<{max_endpoint_chars}} {"STATUS":<{max_status_chars}} UUID',
+        extra={'simple': True},
+    )
+
+    toprule_len = 2 + max_endpoint_chars + max_status_chars + len(eps[0][1])
+    logger.info('=' * toprule_len, extra={'simple': True})
+
+    for name, uuid_ in eps:
+        status = get_status(name, proxystore_dir)
+        logger.info(
+            f'{name:{max_endpoint_chars}.{max_endpoint_chars}} '
+            f'{status.name:<{max_status_chars}.{max_status_chars}} {uuid_}',
+            extra={'simple': True},
+        )
 
     return 0
 
 
 def remove_endpoint(
     name: str,
     *,
```

### Comparing `proxystore-0.5.1/proxystore/endpoint/config.py` & `proxystore-0.5.2/proxystore/endpoint/config.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/endpoint/endpoint.py` & `proxystore-0.5.2/proxystore/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/endpoint/exceptions.py` & `proxystore-0.5.2/proxystore/endpoint/exceptions.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/endpoint/messages.py` & `proxystore-0.5.2/proxystore/endpoint/messages.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/endpoint/serve.py` & `proxystore-0.5.2/proxystore/endpoint/serve.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/endpoint/storage.py` & `proxystore-0.5.2/proxystore/endpoint/storage.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/factory.py` & `proxystore-0.5.2/proxystore/factory.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/globus.py` & `proxystore-0.5.2/proxystore/globus.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/p2p/__init__.py` & `proxystore-0.5.2/proxystore/p2p/__init__.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/p2p/chunks.py` & `proxystore-0.5.2/proxystore/p2p/chunks.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/p2p/connection.py` & `proxystore-0.5.2/proxystore/p2p/connection.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/p2p/counter.py` & `proxystore-0.5.2/proxystore/p2p/counter.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/p2p/manager.py` & `proxystore-0.5.2/proxystore/p2p/manager.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/p2p/messages.py` & `proxystore-0.5.2/proxystore/p2p/messages.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/p2p/relay.py` & `proxystore-0.5.2/proxystore/p2p/relay.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/p2p/relay_client.py` & `proxystore-0.5.2/proxystore/p2p/relay_client.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/p2p/task.py` & `proxystore-0.5.2/proxystore/p2p/task.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/proxy.py` & `proxystore-0.5.2/proxystore/proxy.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/serialize.py` & `proxystore-0.5.2/proxystore/serialize.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/store/__init__.py` & `proxystore-0.5.2/proxystore/store/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,23 @@
 from proxystore.proxy import Proxy
 from proxystore.store.base import ConnectorT
 from proxystore.store.base import Store
 from proxystore.store.base import StoreFactory
 from proxystore.store.exceptions import ProxyStoreFactoryError
 from proxystore.store.exceptions import StoreExistsError
 
+__all__ = [
+    'Store',
+    'StoreFactory',
+    'get_store',
+    'register_store',
+    'store_registration',
+    'unregister_store',
+]
+
 T = TypeVar('T')
 
 _stores: dict[str, Store[Any]] = {}
 logger = logging.getLogger(__name__)
 
 
 def get_store(val: str | Proxy[T]) -> Store[Any] | None:
```

### Comparing `proxystore-0.5.1/proxystore/store/base.py` & `proxystore-0.5.2/proxystore/store/base.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/store/cache.py` & `proxystore-0.5.2/proxystore/store/cache.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/store/endpoint.py` & `proxystore-0.5.2/proxystore/store/endpoint.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/store/exceptions.py` & `proxystore-0.5.2/proxystore/store/exceptions.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/store/file.py` & `proxystore-0.5.2/proxystore/store/file.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/store/globus.py` & `proxystore-0.5.2/proxystore/store/globus.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/store/local.py` & `proxystore-0.5.2/proxystore/store/local.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/store/metrics.py` & `proxystore-0.5.2/proxystore/store/metrics.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/store/multi.py` & `proxystore-0.5.2/proxystore/store/multi.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/store/redis.py` & `proxystore-0.5.2/proxystore/store/redis.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/store/utils.py` & `proxystore-0.5.2/proxystore/store/utils.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/timer.py` & `proxystore-0.5.2/proxystore/timer.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore/utils.py` & `proxystore-0.5.2/proxystore/utils.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore.egg-info/PKG-INFO` & `proxystore-0.5.2/proxystore.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxystore
-Version: 0.5.1
+Version: 0.5.2
 Summary: Lazy object proxy interface for distributed stores.
 Author: Globus Labs
 Author-email: Greg Pauloski <jgpauloski@uchicago.edu>
 Maintainer-email: Greg Pauloski <jgpauloski@uchicago.edu>, Valerie Hayot-Sasson <vhayot@uchicago.edu>
 License: FILE
 Project-URL: homepage, https://proxystore.dev
 Project-URL: documentation, https://docs.proxystore.dev
@@ -21,14 +21,15 @@
 Provides-Extra: zmq
 Provides-Extra: dev
 Provides-Extra: docs
 License-File: LICENSE
 
 # ProxyStore
 
+[![DOI](https://zenodo.org/badge/357984234.svg)](https://zenodo.org/badge/latestdoi/357984234)
 [![docs](https://github.com/proxystore/proxystore/actions/workflows/docs.yml/badge.svg)](https://github.com/proxystore/proxystore/actions/workflows/docs.yml)
 [![tests](https://github.com/proxystore/proxystore/actions/workflows/tests.yml/badge.svg?label=tests)](https://github.com/proxystore/proxystore/actions)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/proxystore/proxystore/main.svg)](https://results.pre-commit.ci/latest/github/proxystore/proxystore/main)
 
 ProxyStore provides pass-by-reference semantics for distributed Python
 applications through transparent object proxies. Moving data via proxies
 (1) decouples control flow from data flow, (2) enables producers to
```

### Comparing `proxystore-0.5.1/proxystore.egg-info/SOURCES.txt` & `proxystore-0.5.2/proxystore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/proxystore.egg-info/requires.txt` & `proxystore-0.5.2/proxystore.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-click
+click!=8.1.4
 cloudpickle>=1.6.0
 cryptography>=39.0.1
 globus-sdk>=3.3.0
 lazy-object-proxy>=1.6.0
 typing-extensions>=4.3.0
 
 [:python_version < "3.8"]
```

### Comparing `proxystore-0.5.1/pyproject.toml` & `proxystore-0.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proxystore"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
     {name = "Globus Labs"},
     {name = "Greg Pauloski", email = "jgpauloski@uchicago.edu"},
 ]
 maintainers = [
     {name = "Greg Pauloski", email = "jgpauloski@uchicago.edu"},
     {name = "Valerie Hayot-Sasson", email = "vhayot@uchicago.edu"},
@@ -20,15 +20,16 @@
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
-    "click",
+    # Click 8.1.4 fails mypy: https://github.com/pallets/click/issues/2558
+    "click!=8.1.4",
     "cloudpickle>=1.6.0",
     "cryptography>=39.0.1",
     "globus-sdk>=3.3.0",
     "lazy-object-proxy>=1.6.0",
     "typing-extensions>=4.3.0",
     "importlib-metadata; python_version<'3.8'",
 ]
```

### Comparing `proxystore-0.5.1/testing/compat.py` & `proxystore-0.5.2/testing/compat.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/connectors.py` & `proxystore-0.5.2/testing/connectors.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/endpoint.py` & `proxystore-0.5.2/testing/endpoint.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/mocked/globus.py` & `proxystore-0.5.2/testing/mocked/globus.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/mocked/pymargo.py` & `proxystore-0.5.2/testing/mocked/pymargo.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/mocked/redis.py` & `proxystore-0.5.2/testing/mocked/redis.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/mocked/ucx.py` & `proxystore-0.5.2/testing/mocked/ucx.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/mocking.py` & `proxystore-0.5.2/testing/mocking.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/relay_server.py` & `proxystore-0.5.2/testing/relay_server.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/scripts/peer_connection_bandwidth.py` & `proxystore-0.5.2/testing/scripts/peer_connection_bandwidth.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/scripts/peer_endpoint_bandwidth.py` & `proxystore-0.5.2/testing/scripts/peer_endpoint_bandwidth.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/scripts/peer_manager_bandwidth.py` & `proxystore-0.5.2/testing/scripts/peer_manager_bandwidth.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/stores.py` & `proxystore-0.5.2/testing/stores.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/testing/utils.py` & `proxystore-0.5.2/testing/utils.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/conftest.py` & `proxystore-0.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/connectors/connector_test.py` & `proxystore-0.5.2/tests/connectors/connector_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/connectors/dim/margo_test.py` & `proxystore-0.5.2/tests/connectors/dim/margo_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/connectors/dim/ucx_test.py` & `proxystore-0.5.2/tests/connectors/dim/ucx_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/connectors/dim/zmq_test.py` & `proxystore-0.5.2/tests/connectors/dim/zmq_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/connectors/endpoint_test.py` & `proxystore-0.5.2/tests/connectors/endpoint_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/connectors/file_test.py` & `proxystore-0.5.2/tests/connectors/file_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/connectors/globus_test.py` & `proxystore-0.5.2/tests/connectors/globus_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,20 +177,18 @@
     s3 = GlobusConnector(endpoints=eps.dict())
     assert s1.config() == s2.config() == s3.config()
 
     with pytest.raises(ValueError):
         # Invalid endpoint type
         GlobusConnector(endpoints=None)  # type: ignore[arg-type]
 
-    with pytest.raises(ValueError):
-        # Too many endpoints
-        GlobusConnector(endpoints=[EP1, EP2, EP3])
-
-    with pytest.raises(ValueError):
-        # Not enough endpoints
+    with pytest.raises(
+        ValueError,
+        match='At least two Globus endpoints are required.',
+    ):
         GlobusConnector(endpoints=[EP1])
 
 
 def test_globus_connector_internals(globus_connector) -> None:
     """Test GlobusConnector internal mechanisms."""
     connector = GlobusConnector.from_config(globus_connector.config())
```

### Comparing `proxystore-0.5.1/tests/connectors/local_test.py` & `proxystore-0.5.2/tests/connectors/local_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/connectors/multi_test.py` & `proxystore-0.5.2/tests/connectors/multi_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/connectors/redis_test.py` & `proxystore-0.5.2/tests/connectors/redis_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/endpoint/cli_test.py` & `proxystore-0.5.2/tests/endpoint/cli_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/endpoint/client_test.py` & `proxystore-0.5.2/tests/endpoint/client_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/endpoint/commands_test.py` & `proxystore-0.5.2/tests/endpoint/commands_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/endpoint/config_test.py` & `proxystore-0.5.2/tests/endpoint/config_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/endpoint/endpoint_peering_test.py` & `proxystore-0.5.2/tests/endpoint/endpoint_peering_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/endpoint/endpoint_solo_test.py` & `proxystore-0.5.2/tests/endpoint/endpoint_solo_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/endpoint/serve_test.py` & `proxystore-0.5.2/tests/endpoint/serve_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/endpoint/storage_test.py` & `proxystore-0.5.2/tests/endpoint/storage_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/factory_test.py` & `proxystore-0.5.2/tests/factory_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/globus_test.py` & `proxystore-0.5.2/tests/globus_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/integration/endpoints_test.py` & `proxystore-0.5.2/tests/integration/endpoints_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/p2p/chunks_test.py` & `proxystore-0.5.2/tests/p2p/chunks_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/p2p/connection_test.py` & `proxystore-0.5.2/tests/p2p/connection_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/p2p/counter_test.py` & `proxystore-0.5.2/tests/p2p/counter_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/p2p/manager_test.py` & `proxystore-0.5.2/tests/p2p/manager_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/p2p/messages_test.py` & `proxystore-0.5.2/tests/p2p/messages_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/p2p/relay_cli_test.py` & `proxystore-0.5.2/tests/p2p/relay_cli_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/p2p/relay_client_test.py` & `proxystore-0.5.2/tests/p2p/relay_client_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/p2p/relay_test.py` & `proxystore-0.5.2/tests/p2p/relay_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/p2p/task_test.py` & `proxystore-0.5.2/tests/p2p/task_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/proxy_test.py` & `proxystore-0.5.2/tests/proxy_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/serialization_test.py` & `proxystore-0.5.2/tests/serialization_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/store/cache_test.py` & `proxystore-0.5.2/tests/store/cache_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/store/init_test.py` & `proxystore-0.5.2/tests/store/init_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/store/metrics_test.py` & `proxystore-0.5.2/tests/store/metrics_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/store/shims_test.py` & `proxystore-0.5.2/tests/store/shims_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/store/store_basics_test.py` & `proxystore-0.5.2/tests/store/store_basics_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/store/store_metrics_test.py` & `proxystore-0.5.2/tests/store/store_metrics_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/store/store_proxy_test.py` & `proxystore-0.5.2/tests/store/store_proxy_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/store/utils_test.py` & `proxystore-0.5.2/tests/store/utils_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/timer_test.py` & `proxystore-0.5.2/tests/timer_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tests/utils_test.py` & `proxystore-0.5.2/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `proxystore-0.5.1/tox.ini` & `proxystore-0.5.2/tox.ini`

 * *Files identical despite different names*

