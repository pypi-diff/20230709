# Comparing `tmp/port_ocean-0.1.0.dev7.tar.gz` & `tmp/port_ocean-0.1.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "port_ocean-0.1.0.dev7.tar", max compression
+gzip compressed data, was "port_ocean-0.1.0.dev8.tar", max compression
```

## Comparing `port_ocean-0.1.0.dev7.tar` & `port_ocean-0.1.0.dev8.tar`

### file list

```diff
@@ -1,79 +1,80 @@
--rw-r--r--   0        0        0     4418 2023-07-04 14:27:00.327401 port_ocean-0.1.0.dev7/README.md
--rw-r--r--   0        0        0      537 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/__init__.py
--rw-r--r--   0        0        0      121 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/cli.py
--rw-r--r--   0        0        0     5126 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/commands.py
--rw-r--r--   0        0        0      429 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/cookiecutter.json
--rw-r--r--   0        0        0       54 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
--rw-r--r--   0        0        0     2832 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
--rw-r--r--   0        0        0      449 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
--rw-r--r--   0        0        0     1699 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
--rw-r--r--   0        0        0      406 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
--rw-r--r--   0        0        0      392 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
--rw-r--r--   0        0        0       46 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
--rw-r--r--   0        0        0     1184 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
--rw-r--r--   0        0        0     1334 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/download_git_folder.py
--rw-r--r--   0        0        0      766 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/cli/list_integrations.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/clients/port/__init__.py
--rw-r--r--   0        0        0     2593 2023-07-04 14:27:00.355401 port_ocean-0.1.0.dev7/port_ocean/clients/port/authentication.py
--rw-r--r--   0        0        0     2799 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/clients/port/client.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/clients/port/mixins/__init__.py
--rw-r--r--   0        0        0     6097 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/clients/port/mixins/entities.py
--rw-r--r--   0        0        0     3029 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/clients/port/mixins/integrations.py
--rw-r--r--   0        0        0      593 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/clients/port/types.py
--rw-r--r--   0        0        0      142 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/clients/port/utils.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/config/__init__.py
--rw-r--r--   0        0        0     2463 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/config/base.py
--rw-r--r--   0        0        0      994 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/config/integration.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/consumers/__init__.py
--rw-r--r--   0        0        0      125 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/consumers/base_consumer.py
--rw-r--r--   0        0        0     3991 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/consumers/kafka_consumer.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/context/__init__.py
--rw-r--r--   0        0        0     3119 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/context/event.py
--rw-r--r--   0        0        0     4032 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/context/ocean.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/__init__.py
--rw-r--r--   0        0        0      219 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/base.py
--rw-r--r--   0        0        0      300 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/manipulation/__init__.py
--rw-r--r--   0        0        0      946 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/manipulation/base.py
--rw-r--r--   0        0        0     2674 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/manipulation/jq_manipulation.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/port_app_config/__init__.py
--rw-r--r--   0        0        0      452 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/port_app_config/api.py
--rw-r--r--   0        0        0      651 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/port_app_config/base.py
--rw-r--r--   0        0        0     1432 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/port_app_config/models.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/transport/__init__.py
--rw-r--r--   0        0        0      852 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/transport/base.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/transport/port/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/transport/port/get_related_entities.py
--rw-r--r--   0        0        0     1043 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
--rw-r--r--   0        0        0     7619 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/transport/port/transport.py
--rw-r--r--   0        0        0     1375 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/handlers/transport/port/validate_entity_relations.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/integrations/__init__.py
--rw-r--r--   0        0        0     2085 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/integrations/base.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/integrations/mixins/__init__.py
--rw-r--r--   0        0        0      692 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/integrations/mixins/events.py
--rw-r--r--   0        0        0     2557 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/integrations/mixins/handler.py
--rw-r--r--   0        0        0     9868 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/integrations/mixins/sync.py
--rw-r--r--   0        0        0      588 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/models.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/trigger_channel/__init__.py
--rw-r--r--   0        0        0      448 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/trigger_channel/base.py
--rw-r--r--   0        0        0     2962 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/trigger_channel/factory.py
--rw-r--r--   0        0        0      898 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/trigger_channel/http.py
--rw-r--r--   0        0        0     3568 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/trigger_channel/kafka.py
--rw-r--r--   0        0        0      909 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/trigger_channel/settings.py
--rw-r--r--   0        0        0      563 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/types.py
--rw-r--r--   0        0        0     2044 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/core/utils.py
--rw-r--r--   0        0        0        0 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/exceptions/__init__.py
--rw-r--r--   0        0        0      426 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/exceptions/api.py
--rw-r--r--   0        0        0       46 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/exceptions/base.py
--rw-r--r--   0        0        0      180 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/exceptions/clients.py
--rw-r--r--   0        0        0      235 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/exceptions/context.py
--rw-r--r--   0        0        0      473 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/exceptions/core.py
--rw-r--r--   0        0        0      756 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/logger_setup.py
--rw-r--r--   0        0        0     2434 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/middlewares.py
--rw-r--r--   0        0        0     4382 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/ocean.py
--rw-r--r--   0        0        0      765 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/port_ocean/utils.py
--rw-r--r--   0        0        0     2041 2023-07-04 14:27:00.359401 port_ocean-0.1.0.dev7/pyproject.toml
--rw-r--r--   0        0        0     5503 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev7/PKG-INFO
+-rw-r--r--   0        0        0     4561 2023-07-09 15:01:27.476122 port_ocean-0.1.0.dev8/README.md
+-rw-r--r--   0        0        0      537 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/__init__.py
+-rw-r--r--   0        0        0      121 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cli.py
+-rw-r--r--   0        0        0     5122 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/commands.py
+-rw-r--r--   0        0        0      429 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/cookiecutter.json
+-rw-r--r--   0        0        0       42 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.dockerignore
+-rw-r--r--   0        0        0     2698 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore
+-rw-r--r--   0        0        0      449 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Dockerfile
+-rw-r--r--   0        0        0     1699 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile
+-rw-r--r--   0        0        0      405 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/README.md
+-rw-r--r--   0        0        0       71 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/debug.py
+-rw-r--r--   0        0        0     1669 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/main.py
+-rw-r--r--   0        0        0       46 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/poetry.toml
+-rw-r--r--   0        0        0     1167 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0     1755 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/download_git_folder.py
+-rw-r--r--   0        0        0      722 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/cli/list_integrations.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/__init__.py
+-rw-r--r--   0        0        0     2528 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/authentication.py
+-rw-r--r--   0        0        0     2700 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/client.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/mixins/__init__.py
+-rw-r--r--   0        0        0     5995 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/mixins/entities.py
+-rw-r--r--   0        0        0     3051 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/mixins/integrations.py
+-rw-r--r--   0        0        0      593 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/types.py
+-rw-r--r--   0        0        0      142 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/clients/port/utils.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/config/__init__.py
+-rw-r--r--   0        0        0     2319 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/config/base.py
+-rw-r--r--   0        0        0     1066 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/config/integration.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/consumers/__init__.py
+-rw-r--r--   0        0        0      125 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/consumers/base_consumer.py
+-rw-r--r--   0        0        0     3991 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/consumers/kafka_consumer.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/context/__init__.py
+-rw-r--r--   0        0        0     3201 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/context/event.py
+-rw-r--r--   0        0        0     4038 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/context/ocean.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/__init__.py
+-rw-r--r--   0        0        0      219 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/base.py
+-rw-r--r--   0        0        0      300 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/manipulation/__init__.py
+-rw-r--r--   0        0        0      946 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/manipulation/base.py
+-rw-r--r--   0        0        0     2674 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/manipulation/jq_manipulation.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/__init__.py
+-rw-r--r--   0        0        0      452 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/api.py
+-rw-r--r--   0        0        0      651 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/base.py
+-rw-r--r--   0        0        0     1432 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/models.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/__init__.py
+-rw-r--r--   0        0        0      852 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/base.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/get_related_entities.py
+-rw-r--r--   0        0        0      988 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/order_by_entities_dependencies.py
+-rw-r--r--   0        0        0     7761 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/transport.py
+-rw-r--r--   0        0        0     1375 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/validate_entity_relations.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/__init__.py
+-rw-r--r--   0        0        0     1976 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/__init__.py
+-rw-r--r--   0        0        0      692 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/events.py
+-rw-r--r--   0        0        0     2557 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/handler.py
+-rw-r--r--   0        0        0     9891 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/sync.py
+-rw-r--r--   0        0        0      588 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/models.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/__init__.py
+-rw-r--r--   0        0        0      389 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/base.py
+-rw-r--r--   0        0        0     2864 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/factory.py
+-rw-r--r--   0        0        0      898 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/http.py
+-rw-r--r--   0        0        0     3238 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/kafka.py
+-rw-r--r--   0        0        0      909 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/settings.py
+-rw-r--r--   0        0        0      563 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/types.py
+-rw-r--r--   0        0        0     1924 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/core/utils.py
+-rw-r--r--   0        0        0        0 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/api.py
+-rw-r--r--   0        0        0       46 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/base.py
+-rw-r--r--   0        0        0      180 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/clients.py
+-rw-r--r--   0        0        0      235 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/context.py
+-rw-r--r--   0        0        0      473 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/exceptions/core.py
+-rw-r--r--   0        0        0      670 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/logger_setup.py
+-rw-r--r--   0        0        0     2475 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/middlewares.py
+-rw-r--r--   0        0        0     4325 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/ocean.py
+-rw-r--r--   0        0        0      770 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/port_ocean/utils.py
+-rw-r--r--   0        0        0     2024 2023-07-09 15:01:27.508123 port_ocean-0.1.0.dev8/pyproject.toml
+-rw-r--r--   0        0        0     5646 1970-01-01 00:00:00.000000 port_ocean-0.1.0.dev8/PKG-INFO
```

### Comparing `port_ocean-0.1.0.dev7/README.md` & `port_ocean-0.1.0.dev8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,111 +1,47 @@
 # Ocean <img src="./assets/OceanSymbol.svg" alt="Ocean" width="100" height="100" align="right">
 
 [![Lint](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
 
-Ocean is a solution created by Port to tackle the difficulties encountered when merging different third-party systems with our developer portal product. This framework offers a uniform method for executing integrations, streamlining the process and enabling platform engineers to prioritize the essential features of the third-party system.
-
-
+Ocean is an innovative solution developed by Port to seamlessly integrate various third-party systems with our developer portal product,
+empowering engineers to effortlessly prioritize key features and streamline the integration process.
 
 ## Prerequisites
 
 - Python 3.11
 
 
 
 ## Installation
-```
+In order to install the Ocean Framework, run the following command:
+
+```sh
 pip install port-ocean[cli]
 ```
 
 Or
 
 ```sh
 poetry add port-ocean[cli]
 ```
 
-[]()
-
 ## Run Integration
 
 1. source the integration venv 
 
    ```sh
    . .venv/bin/activate
    ```
 
 2. Run
 
    ```sh
    ocean sail ./path/to/integration
    ```
 
-   
-
-## Local Development (Framework)
-1. Clone the repository
-
-2. Install dependencies:
-
-   ```sh
-   make install
-   ```
-
-   Or (For installing integrations dependencies as well)
-
-   ```sh
-   make install/all
-   ```
-
-3. source the integration venv
-
-   ```sh
-   . .venv/bin/activate
-   ```
-
-   
-
-
-## Local Development (Integration)
-1. Clone the repository
-
-2. For new integration run
-
-   ```sh
-   make new
-   ```
-
-   and follow the instructions
-
-3. Install dependencies
-
-4. ```sh
-   cd DESIRED_INTEGRATION_FOLDER && make install
-   ```
-
-5. source the integration venv
-
-   ```sh
-   . .venv/bin/activate
-   ```
-
-6. Run the integration
-
-   ```sh
-   make run
-   ```
-
-   Or
-
-   ```sh
-   ocean sail
-   ```
-
-   
-
 # Export Architecture
 
 ![image](./assets/ExportArchitecture.svg)
 
 ## Real-Time updates Architecture
 ![image](./assets/RealTimeUpdatesArchitecture.svg)
 
@@ -158,14 +94,73 @@
   type: "PagerDuty"
   config:
     my_git_token: "random"
     some_other_integration_config: "Very important information"
 ```
 
 ## Contributing
-We welcome contributions to the Integration Framework project. If you have any suggestions, bug reports, or would like to contribute new features, please follow our guidelines outlined in the `CONTRIBUTING.md` file.
+
+The reason Ocean is open source is that we aim for the Port integration library to offer numerous useful out-of-the-box integrations. We have confidence that developers and DevOps professionals who rely on Port in their everyday work will be inclined to contribute and assist in making it a comprehensive tool.
+
+In order to learn how you can contribute to Ocean, read our [contributing guide](./CONTRIBUTING.md)
+
+### Local Development (Framework)
+1. Clone the repository
+
+2. Install dependencies:
+
+   ```sh
+   make install
+   ```
+
+   Or (For installing integrations dependencies as well)
+
+   ```sh
+   make install/all
+   ```
+
+3. source the integration venv
+
+   ```sh
+   . .venv/bin/activate
+   ```
+
+### Local Development (Integration)
+1. Clone the repository
+
+2. For new integration run
+
+   ```sh
+   make new
+   ```
+
+   and follow the instructions
+
+3. Install dependencies
+
+4. ```sh
+   cd DESIRED_INTEGRATION_FOLDER && make install
+   ```
+
+5. source the integration venv
+
+   ```sh
+   . .venv/bin/activate
+   ```
+
+6. Run the integration
+
+   ```sh
+   make run
+   ```
+
+   Or
+
+   ```sh
+   ocean sail
+   ```
 
 ## License
 The Integration Framework is open-source software licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0). See the `LICENSE` file for more details.
 
 ## Contact
 For any questions or inquiries, please reach out to our team at support@getport.io
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/__init__.py` & `port_ocean-0.1.0.dev8/port_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/cli/commands.py` & `port_ocean-0.1.0.dev8/port_ocean/cli/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import os
 
 import click
 import toml
 from cookiecutter.main import cookiecutter  # type: ignore
 from rich.console import Console
 
-from port_ocean.cli.download_git_folder import download_folder
+from port_ocean.cli.download_git_folder import download_github_folder
 from port_ocean.cli.list_integrations import list_git_folders
-from port_ocean.logger_setup import LogLevelType
+from port_ocean.config.integration import LogLevelType
 
 CONTEXT_SETTINGS = dict(help_option_names=["-h", "--help"])
 console = Console()
 
 
 def print_logo() -> None:
     ascii_art = """
@@ -26,15 +26,15 @@
     #+#    #+#     #+#    #+#      #+#              #+#     #+#    #+#   #+#+#      
     ########       ########       ##########       ###     ###    ###    ####      
 =====================================================================================
 By: Port.io
 """
 
     # Display ASCII art
-    Console().print(ascii_art)
+    Console().print(ascii_art.strip())
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 def cli_start() -> None:
     # Ocean root command
     pass
 
@@ -125,15 +125,15 @@
 
 @cli_start.command(name="list")
 def list_integrations() -> None:
     """
     List all available public integrations.
     """
     console.print("🌊 Here are the integrations available to you:", style="bold")
-    options = list_git_folders("https://github.com/port-labs/pulumi", "examples")
+    options = list_git_folders("port-labs", "pulumi", "examples")
 
     for option in options:
         console.print(f"⚓️ [bold][blue]{option}[/blue][/bold]")
 
 
 @cli_start.command()
 @click.argument("name", type=str)
@@ -147,10 +147,10 @@
 )
 def pull(name: str, path: str) -> None:
     """
     Pull an integration bt the NAME from the list of available public integrations.
 
     NAME: Name of the integration to pull.
     """
-    download_folder(
-        "https://github.com/port-labs/pulumi", f"examples/{name}", path or f"./{name}"
+    download_github_folder(
+        "port-labs", "pulumi", f"examples/{name}", path or f"./{name}"
     )
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore` & `port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -146,17 +146,8 @@
 # Pyre type checker
 .pyre/
 
 # pytype static type analyzer
 .pytype/
 
 # Cython debug symbols
-cython_debug/
-
-# Pycharm
-.idea/**.iml
-.idea/modules.xml
-.idea/vcs.xml
-.idea/.gitignore
-.idea/workspace.xml
-.idea/inspectionProfiles
-.idea/misc.xml
+cython_debug/
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile` & `port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml` & `port_ocean-0.1.0.dev8/port_ocean/cli/cookiecutter/{{cookiecutter.integration_slug}}/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
 [tool.black]
 line-length = 88
-target-version = ['py39', 'py310', 'py311']
+target-version = ['py311']
 include = '\.pyi?$'
 exclude = '''
 /(
   \scripts
   \.toml
   |\.sh
   |\.git
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/cli/list_integrations.py` & `port_ocean-0.1.0.dev8/port_ocean/cli/list_integrations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-import requests
+import httpx
+from rich.console import Console
 
+console = Console()
 
-def list_git_folders(repo_url: str, path: str) -> list[str]:
-    # Parse the repository URL to extract the owner and repository name
-    parts = repo_url.split("/")
-    owner = parts[-2]
-    repo_name = parts[-1].split(".")[0]
 
+def list_git_folders(owner: str, repo_name: str, path: str) -> list[str]:
     # Construct the API URL to get the contents of the folder
     api_url = f"https://api.github.com/repos/{owner}/{repo_name}/contents/{path}"
 
     # Send a GET request to the API
-    response = requests.get(api_url)
+    response = httpx.get(api_url)
 
     # Check if the request was successful
-    if response.status_code == 200:
-        contents = response.json()
-        folders = [item["name"] for item in contents if item["type"] == "dir"]
-        return folders
-    else:
-        print(f"Failed to list folders. {response.text}")
-        return []
+    if response.is_error:
+        console.print(
+            f"[bold red]Failed to list folders.[/bold red] Status Code: {response.status_code}, Error: {response.text}"
+        )
+        exit(1)
+
+    contents = response.json()
+    folders = [item["name"] for item in contents if item["type"] == "dir"]
+    return folders
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/clients/port/authentication.py` & `port_ocean-0.1.0.dev8/port_ocean/clients/port/authentication.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,26 @@
-from datetime import datetime
 from typing import Any
 
 import httpx
 from loguru import logger
 from pydantic import BaseModel, Field, PrivateAttr
 
 from port_ocean.clients.port.types import UserAgentType
+from port_ocean.utils import get_time
 
 
 class TokenResponse(BaseModel):
     access_token: str = Field(alias="accessToken")
     expires_in: int = Field(alias="expiresIn")
     token_type: str = Field(alias="tokenType")
-    _retrieved_time: datetime = PrivateAttr(datetime.now())
+    _retrieved_time: int = PrivateAttr(get_time())
 
     @property
     def expired(self) -> bool:
-        return (
-            self._retrieved_time.timestamp() + self.expires_in
-            < datetime.now().timestamp()
-        )
+        return self._retrieved_time + self.expires_in < get_time()
 
     @property
     def full_token(self) -> str:
         return f"{self.token_type} {self.access_token}"
 
 
 class PortAuthentication:
@@ -34,16 +31,16 @@
         api_url: str,
         integration_identifier: str,
         integration_type: str,
     ):
         self.api_url = api_url
         self.client_id = client_id
         self.client_secret = client_secret
-        self.integration_identifier = integration_type
-        self.integration_type = integration_identifier
+        self.integration_identifier = integration_identifier
+        self.integration_type = integration_type
         self._last_token_object: TokenResponse | None = None
 
     async def _get_token(self, client_id: str, client_secret: str) -> TokenResponse:
         async with httpx.AsyncClient() as client:
             logger.info(f"Fetching access token for clientId: {client_id}")
 
             credentials = {"clientId": client_id, "clientSecret": client_secret}
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/clients/port/client.py` & `port_ocean-0.1.0.dev8/port_ocean/clients/port/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import httpx as httpx
 from loguru import logger
-from starlette import status
 
 from port_ocean.clients.port.authentication import PortAuthentication
 from port_ocean.clients.port.mixins.entities import EntityClientMixin
 from port_ocean.clients.port.mixins.integrations import IntegrationClientMixin
 from port_ocean.clients.port.types import (
     KafkaCreds,
 )
@@ -35,33 +34,33 @@
 
     async def get_kafka_creds(self, silent: bool = False) -> KafkaCreds:
         logger.info("Fetching organization kafka credentials")
         async with httpx.AsyncClient() as client:
             response = await client.get(
                 f"{self.api_url}/kafka-credentials", headers=await self.auth.headers()
             )
-        if not response.status_code < status.HTTP_400_BAD_REQUEST:
+        if response.is_error:
             logger.error(f"Error getting kafka credentials, error: {response.text}")
         handle_status_code(silent, response)
 
-        credentials = response.json()["credentials"]
+        credentials = response.json().get("credentials")
 
         if credentials is None:
             raise KafkaCredentialsNotFound("No kafka credentials found")
 
         return credentials
 
     async def get_org_id(self) -> str:
         logger.info("Fetching organization id")
 
         async with httpx.AsyncClient() as client:
             response = await client.get(
                 f"{self.api_url}/organization", headers=await self.auth.headers()
             )
-        if not response.status_code < status.HTTP_400_BAD_REQUEST:
+        if response.is_error:
             logger.error(f"Error getting organization id, error: {response.text}")
             response.raise_for_status()
 
         return response.json()["organization"]["id"]
 
     async def get_blueprint(self, identifier: str) -> Blueprint:
         logger.info(f"Fetching blueprint with id: {identifier}")
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/clients/port/mixins/entities.py` & `port_ocean-0.1.0.dev8/port_ocean/clients/port/mixins/entities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import httpx
 from loguru import logger
-from starlette import status
 
 from port_ocean.clients.port.authentication import PortAuthentication
 from port_ocean.clients.port.types import RequestOptions, UserAgentType
 from port_ocean.clients.port.utils import handle_status_code
 from port_ocean.core.models import Entity
 
 
@@ -36,15 +35,15 @@
                     "create_missing_related_entities": str(
                         request_options.get("create_missing_related_entities", False)
                     ).lower(),
                     "validation_only": str(validation_only).lower(),
                 },
             )
 
-        if not response.status_code < status.HTTP_400_BAD_REQUEST:
+        if response.is_error:
             logger.error(
                 f"Error {'Validating' if validation_only else 'Upserting'} "
                 f"entity: {entity.identifier} of "
                 f"blueprint: {entity.blueprint}, "
                 f"error: {response.text}"
             )
         handle_status_code(silent, response)
@@ -60,20 +59,21 @@
             f"Delete entity: {entity.identifier} of blueprint: {entity.blueprint}"
         )
         async with httpx.AsyncClient() as client:
             response = await client.delete(
                 f"{self.auth.api_url}/blueprints/{entity.blueprint}/entities/{entity.identifier}",
                 headers=await self.auth.headers(user_agent_type),
                 params={
-                    "delete_dependents": request_options["delete_dependent_entities"]
-                    or False
+                    "delete_dependents": str(
+                        request_options.get("delete_dependent_entities", False)
+                    ).lower()
                 },
             )
 
-        if not response.status_code < status.HTTP_400_BAD_REQUEST:
+        if response.is_error:
             logger.error(
                 f"Error deleting "
                 f"entity: {entity.identifier} of "
                 f"blueprint: {entity.blueprint}, "
                 f"error: {response.text}"
             )
 
@@ -83,15 +83,15 @@
         logger.info(f"Validating entity {identifier} of blueprint {blueprint} exists")
 
         async with httpx.AsyncClient() as client:
             response = await client.get(
                 f"{self.auth.api_url}/blueprints/{blueprint}/entities/{identifier}",
                 headers=await self.auth.headers(),
             )
-        if response.status_code >= status.HTTP_400_BAD_REQUEST:
+        if response.is_error:
             logger.error(
                 f"Error validating "
                 f"entity: {identifier} of "
                 f"blueprint: {blueprint}, "
                 f"error: {response.text}"
             )
         response.raise_for_status()
@@ -106,25 +106,25 @@
                     "value": self.auth.user_agent(user_agent_type),
                 },
             ],
         }
 
         logger.info(f"Searching entities with query {query}")
         async with httpx.AsyncClient() as client:
-            search_req = await client.post(
+            response = await client.post(
                 f"{self.auth.api_url}/entities/search",
                 json=query,
                 headers=await self.auth.headers(user_agent_type),
                 params={
                     "exclude_calculated_properties": "true",
                     "include": ["blueprint", "identifier"],
                 },
             )
-        search_req.raise_for_status()
-        return [Entity.parse_obj(result) for result in search_req.json()["entities"]]
+        response.raise_for_status()
+        return [Entity.parse_obj(result) for result in response.json()["entities"]]
 
     async def search_dependent_entities(self, entity: Entity) -> list[Entity]:
         body = {
             "combinator": "and",
             "rules": [
                 {
                     "operator": "relatedTo",
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/clients/port/mixins/integrations.py` & `port_ocean-0.1.0.dev8/port_ocean/clients/port/mixins/integrations.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,72 +10,72 @@
 class IntegrationClientMixin:
     def __init__(self, auth: PortAuthentication):
         self.auth = auth
 
     async def get_integration(self, identifier: str) -> dict[str, Any]:
         logger.info(f"Fetching integration with id: {identifier}")
         async with httpx.AsyncClient() as client:
-            integration = await client.get(
+            response = await client.get(
                 f"{self.auth.api_url}/integration/{identifier}",
                 headers=await self.auth.headers(),
             )
-        integration.raise_for_status()
-        return integration.json()["integration"]
+        response.raise_for_status()
+        return response.json()["integration"]
 
     async def create_integration(
         self, _id: str, _type: str, changelog_destination: dict[str, Any]
     ) -> None:
         logger.info(f"Creating integration with id: {_id}")
         headers = await self.auth.headers()
         json = {
             "installationId": _id,
             "installationAppType": _type,
             "changelogDestination": changelog_destination,
         }
         async with httpx.AsyncClient() as client:
-            installation = await client.post(
+            response = await client.post(
                 f"{self.auth.api_url}/integration", headers=headers, json=json
             )
-        installation.raise_for_status()
+        response.raise_for_status()
 
     async def patch_integration(
         self, _id: str, _type: str, changelog_destination: dict[str, Any]
     ) -> None:
         logger.info(f"Updating integration with id: {_id}")
         headers = await self.auth.headers()
         json = {
             "installationId": _id,
             "installationAppType": _type,
             "changelogDestination": changelog_destination,
         }
         async with httpx.AsyncClient() as client:
-            installation = await client.patch(
+            response = await client.patch(
                 f"{self.auth.api_url}/integration/{_id}",
                 headers=headers,
                 json=json,
             )
-        installation.raise_for_status()
+        response.raise_for_status()
 
     async def initiate_integration(
-        self, _id: str, _type: str, changelog_destination: dict[str, Any]
+        self, identifier: str, _type: str, changelog_destination: dict[str, Any]
     ) -> None:
-        logger.info(f"Initiating integration with id: {_id}")
+        logger.info(f"Initiating integration with id: {identifier}")
         try:
-            integration = await self.get_integration(_id)
+            integration = await self.get_integration(identifier)
 
             logger.info("Checking for diff in integration configuration")
             if (
                 integration["changelogDestination"] != changelog_destination
                 and integration["installationAppType"] == _type
             ):
-                await self.patch_integration(_id, _type, changelog_destination)
+                await self.patch_integration(identifier, _type, changelog_destination)
         except httpx.HTTPStatusError as e:
-            if e.response.status_code == status.HTTP_400_BAD_REQUEST:
-                await self.create_integration(_id, _type, changelog_destination)
+            if e.response.status_code == status.HTTP_404_NOT_FOUND:
+                await self.create_integration(identifier, _type, changelog_destination)
                 return
 
             logger.error(
-                f"Error initiating integration with id: {_id}, error: {e.response.text}"
+                f"Error initiating integration with id: {identifier}, error: {e.response.text}"
             )
             raise
 
-        logger.info(f"Integration with id: {_id} successfully registered")
+        logger.info(f"Integration with id: {identifier} successfully registered")
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/clients/port/types.py` & `port_ocean-0.1.0.dev8/port_ocean/clients/port/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/config/base.py` & `port_ocean-0.1.0.dev8/port_ocean/config/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,32 +9,27 @@
 PROVIDER_WRAPPER_PATTERN = r"\{\{ from (.*) \}\}"
 PROVIDER_CONFIG_PATTERN = r"^[a-zA-Z0-9]+ .*$"
 
 
 def read_yaml_config_settings_source(
     settings: "BaseOceanSettings", base_path: str
 ) -> str:
-    """Loads settings from a YAML file at `Config.yaml_file`
-
-    "<file:xxxx>" patterns are replaced with the contents of file xxxx. The root path
-    were to find the files is configured with `secrets_dir`.
-    """
     yaml_file = getattr(settings.__config__, "yaml_file", "")
 
     assert yaml_file, "Settings.yaml_file not properly configured"
 
-    path = Path(base_path) / yaml_file
+    path = Path(base_path, yaml_file)
 
     if not path.exists():
         raise FileNotFoundError(f"Could not open yaml settings file at: {path}")
 
     return path.read_text("utf-8")
 
 
-def validate_config_provider_pattern(value: str) -> tuple[str, str]:
+def parse_config_provider(value: str) -> tuple[str, str]:
     match = re.match(PROVIDER_CONFIG_PATTERN, value)
     if not match:
         raise ValueError(
             f"Invalid pattern: {value}. Pattern should match: {PROVIDER_CONFIG_PATTERN}"
         )
 
     index = value.find(" ")
@@ -50,22 +45,23 @@
             raise ValueError(f"Environment variable not found: {value}")
         return result
     else:
         raise ValueError(f"Invalid provider type: {provider_type}")
 
 
 def load_providers(settings: "BaseOceanSettings", base_path: str) -> dict[str, Any]:
-    value = read_yaml_config_settings_source(settings, base_path)
-    matches = re.finditer(PROVIDER_WRAPPER_PATTERN, value)
+    yaml_content = read_yaml_config_settings_source(settings, base_path)
+    matches = re.finditer(PROVIDER_WRAPPER_PATTERN, yaml_content)
     for match in matches:
-        provider_type, provider_value = validate_config_provider_pattern(match.group(1))
+        provider_type, provider_value = parse_config_provider(match.group(1))
         data = load_from_config_provider(provider_type, provider_value)
-        value = re.sub(re.escape(match.group()), data, value, count=1)
+        # Replace the provider wrapper with the actual value
+        yaml_content = re.sub(re.escape(match.group()), data, yaml_content, count=1)
 
-    return yaml.safe_load(value)
+    return yaml.safe_load(yaml_content)
 
 
 class BaseOceanSettings(BaseSettings):
     base_path: str
 
     class Config:
         yaml_file = "./config.yaml"
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/config/integration.py` & `port_ocean-0.1.0.dev8/port_ocean/config/integration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Any
+from typing import Any, Literal
 
-from pydantic import BaseModel, Field
-from pydantic import BaseSettings
+from pydantic import BaseModel, Field, BaseSettings
 
 from port_ocean.config.base import BaseOceanSettings
 from port_ocean.core.trigger_channel.settings import (
     HttpTriggerChannelSettings,
     KafkaTriggerChannelSettings,
 )
 
@@ -27,10 +26,13 @@
     trigger_channel: KafkaTriggerChannelSettings | HttpTriggerChannelSettings = Field(
         alias="triggerChannel"
     )
     batch_work_size: int | None = Field(alias="batchWorkSize", default=None)
     integration: IntegrationSettings
 
 
+LogLevelType = Literal["ERROR", "WARNING", "INFO", "DEBUG", "CRITICAL"]
+
+
 class LoggerConfiguration(BaseModel):
-    level: str = "DEBUG"
+    level: LogLevelType = "DEBUG"
     serialize: bool = False
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/consumers/kafka_consumer.py` & `port_ocean-0.1.0.dev8/port_ocean/consumers/kafka_consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,16 +87,16 @@
                     if msg is None:
                         continue
                     if msg.error():
                         raise KafkaException(msg.error())
                     else:
                         try:
                             logger.info(
-                                "Process message"
-                                f" from topic {msg.topic()}, partition {msg.partition()}, offset {msg.offset()}"
+                                "Process message "
+                                f"from topic {msg.topic()}, partition {msg.partition()}, offset {msg.offset()}"
                             )
                             self._handle_message(msg)
                         except Exception as process_error:
                             logger.exception(
                                 "Failed process message"
                                 f" from topic {msg.topic()}, partition {msg.partition()}, offset {msg.offset()}: {str(process_error)}"
                             )
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/context/event.py` & `port_ocean-0.1.0.dev8/port_ocean/context/event.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 
 if TYPE_CHECKING:
     from port_ocean.core.handlers.port_app_config.models import PortAppConfig
 
 TriggerType = Literal["manual", "machine", "request"]
 
 
+class EventType:
+    START = "start"
+    RESYNC = "resync"
+    HTTP_REQUEST = "http_request"
+
+
 @dataclass
 class EventContext:
     event_type: str
     trigger_type: TriggerType = "machine"
     attributes: dict[str, Any] = field(default_factory=dict)
     _port_app_config: Optional["PortAppConfig"] = None
     _parent_event: Optional["EventContext"] = None
@@ -51,33 +57,32 @@
 
 
 def _get_event_context() -> EventContext:
     """
     Get the event context from the current thread.
     """
     top_event_context = _event_context_stack.top
-    if top_event_context is not None:
-        return top_event_context
+    if top_event_context is None:
+        raise EventContextNotFoundError(
+            "You must be inside an event context in order to use it"
+        )
 
-    raise EventContextNotFoundError(
-        "You must be inside an event context in order to use it"
-    )
+    return top_event_context
 
 
 event: EventContext = LocalProxy(lambda: _get_event_context())  # type: ignore
 
 
 @asynccontextmanager
 async def event_context(
     event_type: str,
     trigger_type: TriggerType = "manual",
     attributes: dict[str, Any] | None = None,
 ) -> AsyncIterator[EventContext]:
-    if attributes is None:
-        attributes = {}
+    attributes = attributes or {}
 
     parent = _event_context_stack.top
 
     _event_context_stack.push(
         EventContext(
             event_type,
             trigger_type=trigger_type,
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/context/ocean.py` & `port_ocean-0.1.0.dev8/port_ocean/context/ocean.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,26 +107,26 @@
 
 
 _port_ocean_context_stack: LocalStack[PortOceanContext] = LocalStack()
 
 
 def initialize_port_ocean_context(ocean_app: "Ocean") -> None:
     """
-    This Function initiates the PortOcean context and pushes it into the LocalStack().
+    This Function initializes the PortOcean context and pushes it into the LocalStack().
     """
     _port_ocean_context_stack.push(PortOceanContext(app=ocean_app))
 
 
 def _get_port_ocean_context() -> PortOceanContext:
     """
     Get the PortOcean context from the current thread.
     """
     port_ocean_context = _port_ocean_context_stack.top
-    if port_ocean_context is not None:
-        return port_ocean_context
+    if port_ocean_context is None:
+        raise PortOceanContextNotFoundError(
+            "You must first initialize PortOcean in order to use it"
+        )
 
-    raise PortOceanContextNotFoundError(
-        "You must first initialize PortOcean in order to use it"
-    )
+    return port_ocean_context
 
 
 ocean: PortOceanContext = LocalProxy(lambda: _get_port_ocean_context())  # type: ignore
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/handlers/manipulation/base.py` & `port_ocean-0.1.0.dev8/port_ocean/core/handlers/manipulation/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/handlers/manipulation/jq_manipulation.py` & `port_ocean-0.1.0.dev8/port_ocean/core/handlers/manipulation/jq_manipulation.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/handlers/port_app_config/base.py` & `port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/handlers/port_app_config/models.py` & `port_ocean-0.1.0.dev8/port_ocean/core/handlers/port_app_config/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/handlers/transport/base.py` & `port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/base.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/handlers/transport/port/get_related_entities.py` & `port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/get_related_entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     blueprint_identifier_to_entity = dict(
         groupby(
             entities_with_relations,
             key=lambda x: x.blueprint,
         )
     )
     blueprints = await asyncio.gather(
-        *[
+        *(
             port_client.get_blueprint(blueprint_identifier)
             for blueprint_identifier in blueprint_identifier_to_entity.keys()
-        ]
+        )
     )
     entity_to_blueprint = [
         (
             entity,
             next(
                 blueprint
                 for blueprint in blueprints
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/handlers/transport/port/transport.py` & `port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,53 +22,53 @@
 from port_ocean.exceptions.core import RelationValidationException
 
 
 class HttpPortTransport(BaseTransport):
     async def _validate_delete_dependent_entities(self, entities: list[Entity]) -> None:
         logger.info("Validated deleted entities")
         if not event.port_app_config.delete_dependent_entities:
-            deps = await asyncio.gather(
-                *[
+            dependent_entities = await asyncio.gather(
+                *(
                     self.context.port_client.search_dependent_entities(entity)
                     for entity in entities
-                ]
+                )
             )
-            new_dependent = get_unique(
+            new_dependent_entities = get_unique(
                 [
                     entity
-                    for entity in chain.from_iterable(deps)
-                    if not any([is_same_entity(item, entity) for item in entities])
+                    for entity in chain.from_iterable(dependent_entities)
+                    if not any(is_same_entity(item, entity) for item in entities)
                 ]
             )
 
-            if new_dependent:
+            if new_dependent_entities:
                 raise RelationValidationException(
-                    f"Must enable delete_dependent_entities flag or delete also dependent entities:"
-                    f" {[(dep.blueprint, dep.identifier) for dep in new_dependent]}"
+                    f"Must enable delete_dependent_entities flag or delete all dependent entities: "
+                    f" {[(dep.blueprint, dep.identifier) for dep in new_dependent_entities]}"
                 )
 
     async def _validate_entity_diff(self, diff: EntityPortDiff) -> None:
         config = event.port_app_config
         await self._validate_delete_dependent_entities(diff.deleted)
         modified_or_created_entities = diff.modified + diff.created
 
         if modified_or_created_entities:
             logger.info("Validating modified or created entities")
 
             await asyncio.gather(
-                *[
+                *(
                     self.context.port_client.validate_entity_payload(
                         entity,
                         {
                             "merge": config.enable_merge_entity,
                             "create_missing_related_entities": config.create_missing_related_entities,
                         },
                     )
                     for entity in modified_or_created_entities
-                ]
+                )
             )
 
         if not event.port_app_config.delete_dependent_entities:
             logger.info("Validating no relation blocks the operation")
             await validate_entity_relations(diff, self.context.port_client)
 
     async def _delete_diff(
@@ -92,15 +92,16 @@
             )
             is_part_of_created = any(
                 is_same_entity(entity, entity_to_delete) for entity in created_entities
             )
             if is_part_of_related:
                 if event.port_app_config.create_missing_related_entities:
                     logger.info(
-                        "Skipping entity because it is related to created entities and create_missing_related_entities is enabled"
+                        f"Skipping entity {(entity_to_delete.identifier, entity_to_delete.blueprint)} because it is "
+                        f"related to created entities and create_missing_related_entities is enabled"
                     )
                 else:
                     allowed_entities_to_delete.append(entity_to_delete)
             elif not is_part_of_created:
                 allowed_entities_to_delete.append(entity_to_delete)
 
         await self.delete(allowed_entities_to_delete, user_agent_type)
@@ -147,23 +148,23 @@
 
     async def upsert(
         self, entities: list[Entity], user_agent_type: UserAgentType
     ) -> None:
         logger.info(f"Upserting {len(entities)} entities")
         if event.port_app_config.create_missing_related_entities:
             await asyncio.gather(
-                *[
+                *(
                     self.context.port_client.upsert_entity(
                         entity,
                         event.port_app_config.get_port_request_options(),
                         user_agent_type,
                         silent=True,
                     )
                     for entity in entities
-                ]
+                )
             )
         else:
             ordered_created_entities = reversed(
                 order_by_entities_dependencies(entities)
             )
 
             for entity in ordered_created_entities:
@@ -176,23 +177,23 @@
 
     async def delete(
         self, entities: list[Entity], user_agent_type: UserAgentType
     ) -> None:
         logger.info(f"Deleting {len(entities)} entities")
         if event.port_app_config.delete_dependent_entities:
             await asyncio.gather(
-                *[
+                *(
                     self.context.port_client.delete_entity(
                         entity,
                         event.port_app_config.get_port_request_options(),
                         user_agent_type,
                         silent=True,
                     )
                     for entity in entities
-                ]
+                )
             )
         else:
             ordered_deleted_entities = order_by_entities_dependencies(entities)
 
             for entity in ordered_deleted_entities:
                 await self.context.port_client.delete_entity(
                     entity,
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/handlers/transport/port/validate_entity_relations.py` & `port_ocean-0.1.0.dev8/port_ocean/core/handlers/transport/port/validate_entity_relations.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,12 +29,12 @@
 
         if not any(
             is_same_entity(item, entity) for item in modified_or_created_entities
         ):
             required_entities.append(entity)
 
     await asyncio.gather(
-        *[
+        *(
             port_client.validate_entity_exist(item.identifier, item.blueprint)
             for item in required_entities
-        ]
+        )
     )
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/integrations/base.py` & `port_ocean-0.1.0.dev8/port_ocean/core/integrations/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import asyncio
-from typing import (
-    Any,
-)
 
 from loguru import logger
 
 from port_ocean.context.event import (
     event_context,
+    EventType,
 )
 from port_ocean.context.ocean import PortOceanContext
 from port_ocean.core.integrations.mixins.sync import SyncRawMixin, SyncMixin
 from port_ocean.core.trigger_channel.factory import (
     TriggerChannelFactory,
 )
 from port_ocean.exceptions.core import IntegrationAlreadyStartedException
@@ -18,18 +16,18 @@
 
 class BaseIntegration(SyncRawMixin, SyncMixin):
     def __init__(self, context: PortOceanContext):
         SyncRawMixin.__init__(self)
         SyncMixin.__init__(self)
         self.started = False
         self.context = context
-        self.trigger_channel = TriggerChannelFactory(
+        self.trigger_channel_factory = TriggerChannelFactory(
             context,
             self.context.config.integration.identifier,
-            {"on_action": self.trigger_action, "on_resync": self.sync_raw_all},
+            {"on_resync": self.sync_raw_all},
         )
 
     async def start(self) -> None:
         logger.info("Starting integration")
         if self.started:
             raise IntegrationAlreadyStartedException("Integration already started")
 
@@ -46,17 +44,15 @@
             self.context.config.integration.identifier,
             self.context.config.integration.type,
             self.context.config.trigger_channel.to_request(),
         )
 
         self.started = True
 
-        async with event_context("start", trigger_type="machine"):
+        async with event_context(EventType.START, trigger_type="machine"):
             await asyncio.gather(
                 *(listener() for listener in self.event_strategy["start"])
             )
 
         logger.info("Initializing trigger channel")
-        await self.trigger_channel.create_trigger_channel()
-
-    async def trigger_action(self, data: dict[Any, Any]) -> None:
-        raise NotImplementedError("trigger_action is not implemented")
+        trigger_channel = await self.trigger_channel_factory.create_trigger_channel()
+        await trigger_channel.start()
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/integrations/mixins/events.py` & `port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/events.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/integrations/mixins/handler.py` & `port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/handler.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/integrations/mixins/sync.py` & `port_ocean-0.1.0.dev8/port_ocean/core/integrations/mixins/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 from itertools import chain
 from typing import Any, Awaitable
 
 from loguru import logger
 
 from port_ocean.clients.port.types import UserAgentType
-from port_ocean.context.event import TriggerType, event_context
+from port_ocean.context.event import TriggerType, event_context, EventType
 from port_ocean.context.ocean import ocean
 from port_ocean.core.handlers.port_app_config.models import ResourceConfig
 from port_ocean.core.integrations.mixins.events import EventsMixin
 from port_ocean.core.integrations.mixins.handler import HandlerMixin
 from port_ocean.core.models import Entity
 from port_ocean.core.types import RawEntityDiff, EntityDiff, RESYNC_EVENT_LISTENER
 from port_ocean.core.utils import validate_result, zip_and_sum
@@ -60,34 +60,34 @@
         raise NotImplementedError("on_resync must be implemented")
 
     async def _calculate_raw(
         self, raw_diff: list[tuple[ResourceConfig, RawEntityDiff]]
     ) -> list[EntityDiff]:
         logger.info("Calculating diff in entities between states")
         return await asyncio.gather(
-            *[
+            *(
                 self.manipulation.parse_items(mapping, results)
                 for mapping, results in raw_diff
-            ]
+            )
         )
 
     async def _resync_function_wrapper(
         self, fn: RESYNC_EVENT_LISTENER, kind: str
-    ) -> Any:
+    ) -> list[dict[str, Any]]:
         results = await fn(kind)
         try:
             return validate_result(results)
         except RawObjectValidationException as error:
             raise RawObjectValidationException(
                 f"Failed to validate raw data for returned data from {get_function_location(fn)}, error: {error}"
             ) from error
 
     async def _get_resource_raw_results(
         self, resource_config: ResourceConfig
-    ) -> tuple[ResourceConfig, list[dict[Any, Any]]]:
+    ) -> list[dict[str, Any]]:
         logger.info(f"Fetching {resource_config.kind} resync results")
         tasks: list[Awaitable[list[dict[Any, Any]]]] = []
         with logger.contextualize(kind=resource_config.kind):
             if self.__class__._on_resync != SyncRawMixin._on_resync:
                 tasks.append(
                     self._resync_function_wrapper(self._on_resync, resource_config.kind)
                 )
@@ -107,15 +107,15 @@
             logger.info(f"Found {len(tasks)} resync tasks for {resource_config.kind}")
 
             results: list[dict[Any, Any]] = list(
                 chain.from_iterable(await asyncio.gather(*tasks))
             )
 
             logger.info(f"Triggered {len(tasks)} tasks for {resource_config.kind}")
-            return resource_config, results
+            return results
 
     async def _register_resource_raw(
         self,
         resource: ResourceConfig,
         results: list[dict[Any, Any]],
         user_agent_type: UserAgentType,
     ) -> list[Entity]:
@@ -160,25 +160,27 @@
 
     async def _register_in_batches(
         self,
         resource_config: ResourceConfig,
         user_agent_type: UserAgentType,
         batch_work_size: int | None,
     ) -> list[Entity]:
-        resource, results = await self._get_resource_raw_results(resource_config)
+        results = await self._get_resource_raw_results(resource_config)
 
         tasks = []
 
         batch_size = batch_work_size or len(results) or 1
         batches = [
             results[i : i + batch_size] for i in range(0, len(results), batch_size)
         ]
         for batch in batches:
             logger.info(f"Creating task for registering batch of {len(batch)} entities")
-            tasks.append(self._register_resource_raw(resource, batch, user_agent_type))
+            tasks.append(
+                self._register_resource_raw(resource_config, batch, user_agent_type)
+            )
 
         registered_entities_results = await asyncio.gather(*tasks)
         entities: list[Entity] = sum(registered_entities_results, [])
         logger.info(
             f"Finished registering change for {len(results)} raw results for kind: {resource_config.kind}"
         )
         return entities
@@ -255,15 +257,15 @@
         self,
         _: dict[Any, Any] | None = None,
         trigger_type: TriggerType = "machine",
         user_agent_type: UserAgentType = UserAgentType.exporter,
     ) -> None:
         logger.info("Resync was triggered")
 
-        async with event_context("resync", trigger_type=trigger_type):
+        async with event_context(EventType.RESYNC, trigger_type=trigger_type):
             app_config = await self.port_app_config_handler.get_port_app_config()
 
             entities_at_port = await ocean.port_client.search_entities(user_agent_type)
 
             created_entities = await asyncio.gather(
                 *(
                     self._register_in_batches(
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/models.py` & `port_ocean-0.1.0.dev8/port_ocean/core/models.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/trigger_channel/http.py` & `port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/http.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/trigger_channel/kafka.py` & `port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/kafka.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,38 +48,26 @@
             brokers=self.trigger_channel_config.brokers,
             security_protocol=self.trigger_channel_config.security_protocol,
             authentication_mechanism=self.trigger_channel_config.authentication_mechanism,
             kafka_security_enabled=self.trigger_channel_config.kafka_security_enabled,
         )
 
     def should_be_processed(self, msg_value: dict[Any, Any], topic: str) -> bool:
-        if "runs" in topic:
-            return (
-                msg_value.get("payload", {})
-                .get("action", {})
-                .get("invocationMethod", {})
-                .get("type", "")
-                == "KAFKA"
-            )
-
         if "change.log" in topic:
             return msg_value.get("changelogDestination", {}).get("type", "") == "KAFKA"
 
         return False
 
     async def _handle_message(self, message: dict[Any, Any], topic: str) -> None:
         if not self.should_be_processed(message, topic):
             return
 
         if "change.log" in topic:
             await self.events["on_resync"](message)
 
-        if "runs" in topic:
-            await self.events["on_action"](message)
-
     def wrapped_start(
         self, context: PortOceanContext, func: Callable[[], None]
     ) -> Callable[[], None]:
         ocean_app = context.app
 
         def wrapper() -> None:
             initialize_port_ocean_context(ocean_app=ocean_app)
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/trigger_channel/settings.py` & `port_ocean-0.1.0.dev8/port_ocean/core/trigger_channel/settings.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/types.py` & `port_ocean-0.1.0.dev8/port_ocean/core/types.py`

 * *Files identical despite different names*

### Comparing `port_ocean-0.1.0.dev7/port_ocean/core/utils.py` & `port_ocean-0.1.0.dev8/port_ocean/core/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 from typing import Iterable, Any, TypeVar
 
+from pydantic import parse_obj_as, ValidationError
+
 from port_ocean.core.handlers.manipulation.base import EntityPortDiff
 from port_ocean.core.models import Entity
 from port_ocean.exceptions.core import RawObjectValidationException
 
+T = TypeVar("T", bound=list[Any])
+
 
-def is_valid_diff_item(item: Any) -> bool:
-    return isinstance(item, list) and all([isinstance(i, dict) for i in item] or [True])
+def zip_and_sum(collection: Iterable[tuple[T, ...]]) -> tuple[T, ...]:
+    return tuple(sum(items, []) for items in zip(*collection))  # type: ignore
 
 
-def validate_result(result: Any) -> list[dict[Any, Any]]:
-    if isinstance(result, list):
-        if is_valid_diff_item(result):
-            return result
-    raise RawObjectValidationException(f"Expected dict, got {type(result)} instead")
+def validate_result(result: Any) -> list[dict[str, Any]]:
+    try:
+        return parse_obj_as(list[dict[str, Any]], result)
+    except ValidationError as e:
+        raise RawObjectValidationException(f"Expected list[dict[str, Any]], Error: {e}")
 
 
-def is_same_entity(firs_entity: Entity, second_entity: Entity) -> bool:
+def is_same_entity(first_entity: Entity, second_entity: Entity) -> bool:
     return (
-        firs_entity.identifier == second_entity.identifier
-        and firs_entity.blueprint == second_entity.blueprint
+        first_entity.identifier == second_entity.identifier
+        and first_entity.blueprint == second_entity.blueprint
     )
 
 
 def get_unique(array: list[Entity]) -> list[Entity]:
-    seen: list[Entity] = []
-    result = []
+    result: list[Entity] = []
     for item in array:
-        if all(not is_same_entity(item, seen_item) for seen_item in seen):
-            seen.append(item)
+        if all(not is_same_entity(item, seen_item) for seen_item in result):
             result.append(item)
     return result
 
 
-T = TypeVar("T", bound=list[Any])
-
-
-def zip_and_sum(collection: Iterable[tuple[T, ...]]) -> tuple[T, ...]:
-    return tuple(sum(items, []) for items in zip(*collection))  # type: ignore
-
-
 def get_port_diff(
     before: Iterable[Entity],
     after: Iterable[Entity],
 ) -> EntityPortDiff:
     return EntityPortDiff(
         deleted=get_unique(
             [
@@ -59,11 +54,11 @@
                 if not any(is_same_entity(item, item_before) for item_before in before)
             ],
         ),
         modified=get_unique(
             [
                 item
                 for item in after
-                if any(is_same_entity(item, entity_before) for entity_before in before)
+                if any(is_same_entity(item, item_before) for item_before in before)
             ],
         ),
     )
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/logger_setup.py` & `port_ocean-0.1.0.dev8/port_ocean/logger_setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 import sys
-from typing import Literal
 
 from loguru import logger
 
-from port_ocean.config.integration import LoggerConfiguration
-
-LogLevelType = Literal["ERROR", "WARNING", "INFO", "DEBUG", "CRITICAL"]
+from port_ocean.config.integration import LoggerConfiguration, LogLevelType
 
 
 def setup_logger(level: LogLevelType) -> None:
     settings = LoggerConfiguration(level=level)
     logger_format = (
         "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | "
         "<level>{level: <8}</level> | "
         "<level>{message}</level> | {extra}"
     )
 
     logger.remove()
     logger.add(
-        sys.stderr,
+        sys.stdout,
         level=settings.level.upper(),
         format=logger_format,
         serialize=settings.serialize,
         enqueue=True,  # process logs in background
         diagnose=False,  # hide variable values in log backtrace
     )
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/middlewares.py` & `port_ocean-0.1.0.dev8/port_ocean/middlewares.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from typing import Callable, Awaitable
 
 from fastapi import Request, Response
 from loguru import logger
 
 from port_ocean.exceptions.api import BaseAPIException, InternalServerException
-from .context.event import event_context
+from .context.event import event_context, EventType
 from .context.ocean import ocean
-from .utils import get_time, get_uuid
+from .utils import get_time, generate_uuid
 
 
 async def _handle_silently(
     call_next: Callable[[Request], Awaitable[Response]], request: Request
 ) -> Response:
     response: Response
     try:
         if request.url.path.startswith("/integration"):
-            async with event_context("", trigger_type="request"):
+            async with event_context(EventType.HTTP_REQUEST, trigger_type="request"):
                 await ocean.integration.port_app_config_handler.get_port_app_config()
                 response = await call_next(request)
         else:
             response = await call_next(request)
 
     except BaseAPIException as ex:
         response = ex.response()
@@ -45,15 +45,15 @@
     """Middleware used by FastAPI to process each request, featuring:
 
     - Contextualize request logs with a unique Request ID (UUID4) for each unique request.
     - Catch exceptions during the request handling. Translate custom API exceptions into responses,
       or treat (and log) unexpected exceptions.
     """
     start_time = get_time(seconds_precision=False)
-    request_id = get_uuid()
+    request_id = generate_uuid()
 
     with logger.contextualize(request_id=request_id):
         logger.bind(url=str(request.url), method=request.method).info("Request started")
         response = await _handle_silently(call_next, request)
 
         end_time = get_time(seconds_precision=False)
         time_elapsed = round(end_time - start_time, 5)
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/ocean.py` & `port_ocean-0.1.0.dev8/port_ocean/ocean.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 import uvicorn
 from fastapi import FastAPI, APIRouter
 from loguru import logger
 from pydantic import BaseSettings
 from starlette.types import Scope, Receive, Send
 
 from port_ocean.clients.port.client import PortClient
-from port_ocean.config.integration import IntegrationConfiguration
+from port_ocean.config.integration import IntegrationConfiguration, LogLevelType
 from port_ocean.context.ocean import (
     PortOceanContext,
     ocean,
     initialize_port_ocean_context,
 )
 from port_ocean.core.integrations.base import BaseIntegration
-from port_ocean.logger_setup import setup_logger, LogLevelType
+from port_ocean.logger_setup import setup_logger
 from port_ocean.middlewares import request_handler
 
 
 def _get_base_integration_class_from_module(
     module: ModuleType,
 ) -> Type[BaseIntegration]:
     for name, obj in getmembers(module):
@@ -39,19 +39,15 @@
 
 def _load_module(file_path: str) -> ModuleType:
     spec = spec_from_file_location("module_name", file_path)
     if spec is None or spec.loader is None:
         raise Exception(f"Failed to load integration from path: {file_path}")
 
     module = module_from_spec(spec)
-
-    try:
-        spec.loader.exec_module(module)
-    except Exception as e:
-        raise e
+    spec.loader.exec_module(module)
 
     return module
 
 
 def _include_target_channel_router(app: FastAPI, _ocean: PortOceanContext) -> None:
     target_channel_router = APIRouter()
```

### Comparing `port_ocean-0.1.0.dev7/port_ocean/utils.py` & `port_ocean-0.1.0.dev8/port_ocean/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     """Return current time as Unix/Epoch timestamp, in seconds.
     :param seconds_precision: if True, return with seconds precision as integer (default).
                               If False, return with milliseconds precision as floating point number of seconds.
     """
     return time() if not seconds_precision else int(time())
 
 
-def get_uuid() -> str:
+def generate_uuid() -> str:
     """Return a UUID4 as string"""
     return str(uuid4())
 
 
 def get_function_location(func: Callable[..., Any]) -> str:
     file_path = inspect.getsourcefile(func)
     line_number = inspect.getsourcelines(func)[1]
```

### Comparing `port_ocean-0.1.0.dev7/pyproject.toml` & `port_ocean-0.1.0.dev8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "port-ocean"
-version = "0.1.0.dev7"
+version = "0.1.0.dev8"
 description = "Port Ocean is a CLI tool for managing your Port projects."
 readme = "README.md"
 authors = ["Daniel Sinai <daniel@getport.io>", "Yair Siman-Tov <yair@getport.io>"]
 packages = [
     { include = "port_ocean", from = "." }
 ]
 
@@ -82,15 +82,15 @@
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
 
 [tool.black]
 line-length = 88
-target-version = ['py39', 'py310', 'py311']
+target-version = ['py311']
 include = '\.pyi?$'
 exclude = '''
 /(
   \scripts
   \.toml
   |\.sh
   |\.git
```

### Comparing `port_ocean-0.1.0.dev7/PKG-INFO` & `port_ocean-0.1.0.dev8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: port-ocean
-Version: 0.1.0.dev7
+Version: 0.1.0.dev8
 Summary: Port Ocean is a CLI tool for managing your Port projects.
 Author: Daniel Sinai
 Author-email: daniel@getport.io
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cli
@@ -26,114 +26,50 @@
 Requires-Dist: werkzeug (>=2.3.4,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Ocean <img src="./assets/OceanSymbol.svg" alt="Ocean" width="100" height="100" align="right">
 
 [![Lint](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml/badge.svg)](https://github.com/port-labs/port-ocean/actions/workflows/lint.yml)
 
-Ocean is a solution created by Port to tackle the difficulties encountered when merging different third-party systems with our developer portal product. This framework offers a uniform method for executing integrations, streamlining the process and enabling platform engineers to prioritize the essential features of the third-party system.
-
-
+Ocean is an innovative solution developed by Port to seamlessly integrate various third-party systems with our developer portal product,
+empowering engineers to effortlessly prioritize key features and streamline the integration process.
 
 ## Prerequisites
 
 - Python 3.11
 
 
 
 ## Installation
-```
+In order to install the Ocean Framework, run the following command:
+
+```sh
 pip install port-ocean[cli]
 ```
 
 Or
 
 ```sh
 poetry add port-ocean[cli]
 ```
 
-[]()
-
 ## Run Integration
 
 1. source the integration venv 
 
    ```sh
    . .venv/bin/activate
    ```
 
 2. Run
 
    ```sh
    ocean sail ./path/to/integration
    ```
 
-   
-
-## Local Development (Framework)
-1. Clone the repository
-
-2. Install dependencies:
-
-   ```sh
-   make install
-   ```
-
-   Or (For installing integrations dependencies as well)
-
-   ```sh
-   make install/all
-   ```
-
-3. source the integration venv
-
-   ```sh
-   . .venv/bin/activate
-   ```
-
-   
-
-
-## Local Development (Integration)
-1. Clone the repository
-
-2. For new integration run
-
-   ```sh
-   make new
-   ```
-
-   and follow the instructions
-
-3. Install dependencies
-
-4. ```sh
-   cd DESIRED_INTEGRATION_FOLDER && make install
-   ```
-
-5. source the integration venv
-
-   ```sh
-   . .venv/bin/activate
-   ```
-
-6. Run the integration
-
-   ```sh
-   make run
-   ```
-
-   Or
-
-   ```sh
-   ocean sail
-   ```
-
-   
-
 # Export Architecture
 
 ![image](./assets/ExportArchitecture.svg)
 
 ## Real-Time updates Architecture
 ![image](./assets/RealTimeUpdatesArchitecture.svg)
 
@@ -186,14 +122,73 @@
   type: "PagerDuty"
   config:
     my_git_token: "random"
     some_other_integration_config: "Very important information"
 ```
 
 ## Contributing
-We welcome contributions to the Integration Framework project. If you have any suggestions, bug reports, or would like to contribute new features, please follow our guidelines outlined in the `CONTRIBUTING.md` file.
+
+The reason Ocean is open source is that we aim for the Port integration library to offer numerous useful out-of-the-box integrations. We have confidence that developers and DevOps professionals who rely on Port in their everyday work will be inclined to contribute and assist in making it a comprehensive tool.
+
+In order to learn how you can contribute to Ocean, read our [contributing guide](./CONTRIBUTING.md)
+
+### Local Development (Framework)
+1. Clone the repository
+
+2. Install dependencies:
+
+   ```sh
+   make install
+   ```
+
+   Or (For installing integrations dependencies as well)
+
+   ```sh
+   make install/all
+   ```
+
+3. source the integration venv
+
+   ```sh
+   . .venv/bin/activate
+   ```
+
+### Local Development (Integration)
+1. Clone the repository
+
+2. For new integration run
+
+   ```sh
+   make new
+   ```
+
+   and follow the instructions
+
+3. Install dependencies
+
+4. ```sh
+   cd DESIRED_INTEGRATION_FOLDER && make install
+   ```
+
+5. source the integration venv
+
+   ```sh
+   . .venv/bin/activate
+   ```
+
+6. Run the integration
+
+   ```sh
+   make run
+   ```
+
+   Or
+
+   ```sh
+   ocean sail
+   ```
 
 ## License
 The Integration Framework is open-source software licensed under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0). See the `LICENSE` file for more details.
 
 ## Contact
 For any questions or inquiries, please reach out to our team at support@getport.io
```

