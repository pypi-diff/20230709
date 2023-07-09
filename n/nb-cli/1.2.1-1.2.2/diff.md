# Comparing `tmp/nb-cli-1.2.1.tar.gz` & `tmp/nb-cli-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb-cli-1.2.1.tar", last modified: Sun Jul  9 06:25:36 2023, max compression
+gzip compressed data, was "nb-cli-1.2.2.tar", last modified: Sun Jul  9 12:46:17 2023, max compression
```

## Comparing `nb-cli-1.2.1.tar` & `nb-cli-1.2.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1065 2023-07-09 06:24:59.789085 nb-cli-1.2.1/LICENSE
--rw-r--r--   0        0        0     3347 2023-07-09 06:24:59.789085 nb-cli-1.2.1/README.md
--rw-r--r--   0        0        0      246 2023-07-09 06:24:59.789085 nb-cli-1.2.1/build.py
--rw-r--r--   0        0        0      795 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/__init__.py
--rw-r--r--   0        0        0      202 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/__main__.py
--rw-r--r--   0        0        0     3305 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/__init__.py
--rw-r--r--   0        0        0      257 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/__init__.py
--rw-r--r--   0        0        0     6866 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/adapter.py
--rw-r--r--   0        0        0     4243 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/driver.py
--rw-r--r--   0        0        0     7195 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/plugin.py
--rw-r--r--   0        0        0    10538 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/project.py
--rw-r--r--   0        0        0     3409 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/self.py
--rw-r--r--   0        0        0     5618 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/customize.py
--rw-r--r--   0        0        0     1966 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/utils.py
--rw-r--r--   0        0        0      429 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/config/__init__.py
--rw-r--r--   0        0        0      661 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/config/model.py
--rw-r--r--   0        0        0     6220 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/config/parser.py
--rw-r--r--   0        0        0      347 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/consts.py
--rw-r--r--   0        0        0      472 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/exceptions.py
--rw-r--r--   0        0        0      214 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/extensions.py
--rw-r--r--   0        0        0     3030 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/__init__.py
--rw-r--r--   0        0        0      865 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/adapter.py
--rw-r--r--   0        0        0      374 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/driver.py
--rw-r--r--   0        0        0     6766 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/meta.py
--rw-r--r--   0        0        0     3198 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/pip.py
--rw-r--r--   0        0        0     1557 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/plugin.py
--rw-r--r--   0        0        0     2990 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/process.py
--rw-r--r--   0        0        0     2665 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/project.py
--rw-r--r--   0        0        0     5718 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/reloader.py
--rw-r--r--   0        0        0     2150 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/script.py
--rw-r--r--   0        0        0     1860 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/signal.py
--rw-r--r--   0        0        0     4082 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/store.py
--rw-r--r--   0        0        0      734 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/venv.py
--rw-r--r--   0        0        0     1193 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/i18n.py
--rw-r--r--   0        0        0     8966 2023-07-09 06:25:33.789020 nb-cli-1.2.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
--rw-r--r--   0        0        0    13886 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
--rw-r--r--   0        0        0      635 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/log/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/py.typed
--rw-r--r--   0        0        0      143 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/cookiecutter.json
--rw-r--r--   0        0        0      120 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0      847 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
--rw-r--r--   0        0        0      354 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
--rw-r--r--   0        0        0      203 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0      688 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
--rw-r--r--   0        0        0      676 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
--rw-r--r--   0        0        0      164 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/plugin/cookiecutter.json
--rw-r--r--   0        0        0      315 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/plugin/hooks/post_gen_project.py
--rw-r--r--   0        0        0      365 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0      114 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0        0 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
--rw-r--r--   0        0        0      318 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/project/bootstrap/cookiecutter.json
--rw-r--r--   0        0        0      236 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/project/bootstrap/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      141 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0      232 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      620 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0      501 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/cookiecutter.json
--rw-r--r--   0        0        0      307 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/hooks/post_gen_project.py
--rw-r--r--   0        0        0      236 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      157 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
--rw-r--r--   0        0        0       16 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
--rw-r--r--   0        0        0        0 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0     2087 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
--rw-r--r--   0        0        0      328 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      666 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
--rw-r--r--   0        0        0      232 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/meta/_package_version.py.jinja
--rw-r--r--   0        0        0      110 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/meta/nonebot_version.py.jinja
--rw-r--r--   0        0        0      105 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/meta/pip_version.py.jinja
--rw-r--r--   0        0        0      142 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/meta/python_version.py.jinja
--rw-r--r--   0        0        0      181 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
--rw-r--r--   0        0        0     1091 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/project/_prepare.py.jinja
--rw-r--r--   0        0        0      151 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/project/run_project.py.jinja
--rw-r--r--   0        0        0      222 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/script/_entrypoint.py.jinja
--rw-r--r--   0        0        0      158 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/script/list_scripts.py.jinja
--rw-r--r--   0        0        0      333 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/script/run_script.py.jinja
--rw-r--r--   0        0        0     2732 2023-07-09 06:24:59.793084 nb-cli-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 nb-cli-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-09 12:45:45.048828 nb-cli-1.2.2/LICENSE
+-rw-r--r--   0        0        0     3347 2023-07-09 12:45:45.048828 nb-cli-1.2.2/README.md
+-rw-r--r--   0        0        0      246 2023-07-09 12:45:45.048828 nb-cli-1.2.2/build.py
+-rw-r--r--   0        0        0      795 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/__init__.py
+-rw-r--r--   0        0        0      202 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/__main__.py
+-rw-r--r--   0        0        0     3305 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/cli/__init__.py
+-rw-r--r--   0        0        0      257 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6866 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/cli/commands/adapter.py
+-rw-r--r--   0        0        0     4243 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/cli/commands/driver.py
+-rw-r--r--   0        0        0     7195 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/cli/commands/plugin.py
+-rw-r--r--   0        0        0    10538 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/cli/commands/project.py
+-rw-r--r--   0        0        0     3409 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/cli/commands/self.py
+-rw-r--r--   0        0        0     5618 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/cli/customize.py
+-rw-r--r--   0        0        0     1966 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/cli/utils.py
+-rw-r--r--   0        0        0      429 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/config/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/config/model.py
+-rw-r--r--   0        0        0     6220 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/config/parser.py
+-rw-r--r--   0        0        0      347 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/consts.py
+-rw-r--r--   0        0        0      472 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/exceptions.py
+-rw-r--r--   0        0        0      214 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/extensions.py
+-rw-r--r--   0        0        0     3030 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/__init__.py
+-rw-r--r--   0        0        0      865 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/adapter.py
+-rw-r--r--   0        0        0      374 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/driver.py
+-rw-r--r--   0        0        0     6739 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/meta.py
+-rw-r--r--   0        0        0     3198 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/pip.py
+-rw-r--r--   0        0        0     1557 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/plugin.py
+-rw-r--r--   0        0        0     2990 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/process.py
+-rw-r--r--   0        0        0     2715 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/project.py
+-rw-r--r--   0        0        0     5718 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/reloader.py
+-rw-r--r--   0        0        0     2173 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/script.py
+-rw-r--r--   0        0        0     1860 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/signal.py
+-rw-r--r--   0        0        0     4082 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/store.py
+-rw-r--r--   0        0        0      734 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/handlers/venv.py
+-rw-r--r--   0        0        0     1193 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/i18n.py
+-rw-r--r--   0        0        0     8966 2023-07-09 12:46:14.897107 nb-cli-1.2.2/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
+-rw-r--r--   0        0        0    13886 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
+-rw-r--r--   0        0        0      635 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/log/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/py.typed
+-rw-r--r--   0        0        0      143 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/adapter/cookiecutter.json
+-rw-r--r--   0        0        0      120 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      847 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      354 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      203 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      688 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      676 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      164 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/plugin/cookiecutter.json
+-rw-r--r--   0        0        0      315 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/plugin/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      365 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      114 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0        0 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      318 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/bootstrap/cookiecutter.json
+-rw-r--r--   0        0        0      236 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/bootstrap/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      141 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0      232 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      620 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/simple/cookiecutter.json
+-rw-r--r--   0        0        0      307 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/simple/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      236 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/simple/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      157 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
+-rw-r--r--   0        0        0       16 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
+-rw-r--r--   0        0        0        0 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0     2087 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
+-rw-r--r--   0        0        0      328 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      666 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      232 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/scripts/meta/_package_version.py.jinja
+-rw-r--r--   0        0        0      110 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/scripts/meta/nonebot_version.py.jinja
+-rw-r--r--   0        0        0      105 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/scripts/meta/pip_version.py.jinja
+-rw-r--r--   0        0        0      142 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/scripts/meta/python_version.py.jinja
+-rw-r--r--   0        0        0      181 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
+-rw-r--r--   0        0        0     1091 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/scripts/project/_prepare.py.jinja
+-rw-r--r--   0        0        0      151 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/scripts/project/run_project.py.jinja
+-rw-r--r--   0        0        0      222 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/scripts/script/_entrypoint.py.jinja
+-rw-r--r--   0        0        0      158 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/scripts/script/list_scripts.py.jinja
+-rw-r--r--   0        0        0      333 2023-07-09 12:45:45.048828 nb-cli-1.2.2/nb_cli/template/scripts/script/run_script.py.jinja
+-rw-r--r--   0        0        0     2732 2023-07-09 12:45:45.048828 nb-cli-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 nb-cli-1.2.2/PKG-INFO
```

### Comparing `nb-cli-1.2.1/LICENSE` & `nb-cli-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/README.md` & `nb-cli-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/__init__.py` & `nb-cli-1.2.2/nb_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/cli/__init__.py` & `nb-cli-1.2.2/nb_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/cli/commands/adapter.py` & `nb-cli-1.2.2/nb_cli/cli/commands/adapter.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/cli/commands/driver.py` & `nb-cli-1.2.2/nb_cli/cli/commands/driver.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/cli/commands/plugin.py` & `nb-cli-1.2.2/nb_cli/cli/commands/plugin.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/cli/commands/project.py` & `nb-cli-1.2.2/nb_cli/cli/commands/project.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/cli/commands/self.py` & `nb-cli-1.2.2/nb_cli/cli/commands/self.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/cli/customize.py` & `nb-cli-1.2.2/nb_cli/cli/customize.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/cli/utils.py` & `nb-cli-1.2.2/nb_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/config/model.py` & `nb-cli-1.2.2/nb_cli/config/model.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/config/parser.py` & `nb-cli-1.2.2/nb_cli/config/parser.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/handlers/__init__.py` & `nb-cli-1.2.2/nb_cli/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/handlers/adapter.py` & `nb-cli-1.2.2/nb_cli/handlers/adapter.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/handlers/meta.py` & `nb-cli-1.2.2/nb_cli/handlers/meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,14 @@
         return json.loads(stdout.strip())
 
 
 def requires_nonebot(
     func: Callable[P, Coroutine[Any, Any, R]]
 ) -> Callable[P, Coroutine[Any, Any, R]]:
     @wraps(func)
-    @requires_project_root
     @requires_python
     async def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
         if await get_nonebot_version(
             cast(Optional[str], kwargs.get("python_path")),
             cast(Optional[Path], kwargs.get("cwd")),
         ):
             return await func(*args, **kwargs)
```

### Comparing `nb-cli-1.2.1/nb_cli/handlers/pip.py` & `nb-cli-1.2.2/nb_cli/handlers/pip.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/handlers/plugin.py` & `nb-cli-1.2.2/nb_cli/handlers/plugin.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/handlers/process.py` & `nb-cli-1.2.2/nb_cli/handlers/process.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/handlers/project.py` & `nb-cli-1.2.2/nb_cli/handlers/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from . import templates
 from .process import create_process
 from .meta import (
     get_project_root,
     requires_nonebot,
     get_default_python,
     get_nonebot_config,
+    requires_project_root,
 )
 
 TEMPLATE_ROOT = Path(__file__).parent.parent / "template" / "project"
 
 
 def list_project_templates() -> List[str]:
     return sorted(t.name for t in (TEMPLATE_ROOT).iterdir())
@@ -49,14 +50,15 @@
     if builtin_plugins is None:
         builtin_plugins = bot_config.builtin_plugins
 
     t = templates.get_template("project/run_project.py.jinja")
     return await t.render_async(adapters=adapters, builtin_plugins=builtin_plugins)
 
 
+@requires_project_root
 @requires_nonebot
 async def run_project(
     adapters: Optional[List[SimpleInfo]] = None,
     builtin_plugins: Optional[List[str]] = None,
     exist_bot: Path = Path("bot.py"),
     *,
     python_path: Optional[str] = None,
```

### Comparing `nb-cli-1.2.1/nb_cli/handlers/reloader.py` & `nb-cli-1.2.2/nb_cli/handlers/reloader.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/handlers/script.py` & `nb-cli-1.2.2/nb_cli/handlers/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         await t.render_async(),
         stdout=asyncio.subprocess.PIPE,
     )
     stdout, _ = await proc.communicate()
     return json.loads(stdout.strip())
 
 
+@requires_project_root
 @requires_nonebot
 async def run_script(
     script_name: str,
     script_args: Optional[List[str]] = None,
     adapters: Optional[List[SimpleInfo]] = None,
     builtin_plugins: Optional[List[str]] = None,
     *,
```

### Comparing `nb-cli-1.2.1/nb_cli/handlers/signal.py` & `nb-cli-1.2.2/nb_cli/handlers/signal.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/handlers/store.py` & `nb-cli-1.2.2/nb_cli/handlers/store.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/handlers/venv.py` & `nb-cli-1.2.2/nb_cli/handlers/venv.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/i18n.py` & `nb-cli-1.2.2/nb_cli/i18n.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo` & `nb-cli-1.2.2/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: nb-cli 1.0.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-09 06:14+0000\n"
+"POT-Creation-Date: 2023-07-09 12:42+0000\n"
 "PO-Revision-Date: 2023-01-11 08:56+0000\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `nb-cli-1.2.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po` & `nb-cli-1.2.2/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the nb-cli project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: nb-cli 1.0.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-09 06:14+0000\n"
+"POT-Creation-Date: 2023-07-09 12:42+0000\n"
 "PO-Revision-Date: 2023-01-11 08:56+0000\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -417,19 +417,19 @@
 msgid "Cannot find a valid Python interpreter."
 msgstr "无法找到可用的 Python 解释器."
 
 #: nb_cli/handlers/meta.py:146
 msgid "Python {major}.{minor} is not supported."
 msgstr "Python {major}.{minor} 不受支持."
 
-#: nb_cli/handlers/meta.py:196
+#: nb_cli/handlers/meta.py:195
 msgid "NoneBot is not installed."
 msgstr "NoneBot 未安装."
 
-#: nb_cli/handlers/meta.py:242
+#: nb_cli/handlers/meta.py:241
 msgid "pip is not installed."
 msgstr "pip 未安装."
 
 #: nb_cli/handlers/reloader.py:120
 msgid "Watchfiles detected changes in {paths}. Reloading..."
 msgstr "Watchfiles 在 {paths} 中发现变化. 正在重新加载..."
```

### Comparing `nb-cli-1.2.1/nb_cli/log/__init__.py` & `nb-cli-1.2.2/nb_cli/log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}` & `nb-cli-1.2.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}` & `nb-cli-1.2.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}` & `nb-cli-1.2.2/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb-cli-1.2.2/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore` & `nb-cli-1.2.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb-cli-1.2.2/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/nb_cli/template/scripts/project/_prepare.py.jinja` & `nb-cli-1.2.2/nb_cli/template/scripts/project/_prepare.py.jinja`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.1/pyproject.toml` & `nb-cli-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nb-cli"
-version = "1.2.1"
+version = "1.2.2"
 description = "CLI for nonebot2"
 authors = [
     { name = "yanyongyu", email = "yyy@nonebot.dev" },
 ]
 readme = "README.md"
 keywords = [
     "bot",
```

### Comparing `nb-cli-1.2.1/PKG-INFO` & `nb-cli-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-cli
-Version: 1.2.1
+Version: 1.2.2
 Summary: CLI for nonebot2
 License: MIT
 Keywords: bot,qq,nonebot,bot,qq,nonebot
 Author-email: yanyongyu <yyy@nonebot.dev>
 Requires-Python: >=3.8, <4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_7qoo0buq_/tmp5o3y7gkp_TarContainer/0/76", line 148, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_7qoo0buq_/tmp5o3y7gkp_TarContainer/0/76", line 148, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nb-cli Version: 1.2.1 Summary: CLI for nonebot2
+Metadata-Version: 2.1 Name: nb-cli Version: 1.2.2 Summary: CLI for nonebot2
 License: MIT Keywords: bot,qq,nonebot,bot,qq,nonebot Author-email: yanyongyu
 nonebot.dev> Requires-Python: >=3.8, <4.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: Robot Framework Classifier:
 Framework :: Robot Framework :: Library Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Project-URL: homepage, https://
 cli.nonebot.dev/ Project-URL: repository, https://github.com/nonebot/nb-cli
```

