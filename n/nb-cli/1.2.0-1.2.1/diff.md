# Comparing `tmp/nb-cli-1.2.0.tar.gz` & `tmp/nb-cli-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb-cli-1.2.0.tar", last modified: Sat Jul  8 16:00:00 2023, max compression
+gzip compressed data, was "nb-cli-1.2.1.tar", last modified: Sun Jul  9 06:25:36 2023, max compression
```

## Comparing `nb-cli-1.2.0.tar` & `nb-cli-1.2.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0     1065 2023-07-08 15:59:26.355390 nb-cli-1.2.0/LICENSE
--rw-r--r--   0        0        0     3347 2023-07-08 15:59:26.355390 nb-cli-1.2.0/README.md
--rw-r--r--   0        0        0      246 2023-07-08 15:59:26.355390 nb-cli-1.2.0/build.py
--rw-r--r--   0        0        0      795 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/__init__.py
--rw-r--r--   0        0        0      202 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/__main__.py
--rw-r--r--   0        0        0     3305 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/__init__.py
--rw-r--r--   0        0        0      257 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/__init__.py
--rw-r--r--   0        0        0     6866 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/adapter.py
--rw-r--r--   0        0        0     4243 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/driver.py
--rw-r--r--   0        0        0     7195 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/plugin.py
--rw-r--r--   0        0        0    10538 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/project.py
--rw-r--r--   0        0        0     3409 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/commands/self.py
--rw-r--r--   0        0        0     5459 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/customize.py
--rw-r--r--   0        0        0     1966 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/cli/utils.py
--rw-r--r--   0        0        0      429 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/config/__init__.py
--rw-r--r--   0        0        0      661 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/config/model.py
--rw-r--r--   0        0        0     6220 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/config/parser.py
--rw-r--r--   0        0        0      347 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/consts.py
--rw-r--r--   0        0        0      472 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/exceptions.py
--rw-r--r--   0        0        0      214 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/extensions.py
--rw-r--r--   0        0        0     3030 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/__init__.py
--rw-r--r--   0        0        0      865 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/adapter.py
--rw-r--r--   0        0        0      374 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/driver.py
--rw-r--r--   0        0        0     6766 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/meta.py
--rw-r--r--   0        0        0     3198 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/pip.py
--rw-r--r--   0        0        0     1557 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/plugin.py
--rw-r--r--   0        0        0     2990 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/process.py
--rw-r--r--   0        0        0     2665 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/project.py
--rw-r--r--   0        0        0     5718 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/reloader.py
--rw-r--r--   0        0        0     2150 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/script.py
--rw-r--r--   0        0        0     1860 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/signal.py
--rw-r--r--   0        0        0     4082 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/store.py
--rw-r--r--   0        0        0      734 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/handlers/venv.py
--rw-r--r--   0        0        0     1193 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/i18n.py
--rw-r--r--   0        0        0     8966 2023-07-08 15:59:57.571354 nb-cli-1.2.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
--rw-r--r--   0        0        0    13886 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
--rw-r--r--   0        0        0      635 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/log/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/py.typed
--rw-r--r--   0        0        0      143 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/cookiecutter.json
--rw-r--r--   0        0        0      120 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0      847 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
--rw-r--r--   0        0        0      354 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
--rw-r--r--   0        0        0      203 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0      688 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
--rw-r--r--   0        0        0      676 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
--rw-r--r--   0        0        0      164 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/plugin/cookiecutter.json
--rw-r--r--   0        0        0      315 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/plugin/hooks/post_gen_project.py
--rw-r--r--   0        0        0      365 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0      114 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0        0 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
--rw-r--r--   0        0        0      318 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/bootstrap/cookiecutter.json
--rw-r--r--   0        0        0      236 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/bootstrap/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      141 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0      232 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      620 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0      501 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/cookiecutter.json
--rw-r--r--   0        0        0      307 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/hooks/post_gen_project.py
--rw-r--r--   0        0        0      236 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      157 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
--rw-r--r--   0        0        0       16 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
--rw-r--r--   0        0        0        0 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0     2087 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
--rw-r--r--   0        0        0      328 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      666 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
--rw-r--r--   0        0        0      232 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/meta/_package_version.py.jinja
--rw-r--r--   0        0        0      110 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/meta/nonebot_version.py.jinja
--rw-r--r--   0        0        0      105 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/meta/pip_version.py.jinja
--rw-r--r--   0        0        0      142 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/meta/python_version.py.jinja
--rw-r--r--   0        0        0      181 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
--rw-r--r--   0        0        0     1091 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/project/_prepare.py.jinja
--rw-r--r--   0        0        0      151 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/project/run_project.py.jinja
--rw-r--r--   0        0        0      222 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/script/_entrypoint.py.jinja
--rw-r--r--   0        0        0      158 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/script/list_scripts.py.jinja
--rw-r--r--   0        0        0      333 2023-07-08 15:59:26.355390 nb-cli-1.2.0/nb_cli/template/scripts/script/run_script.py.jinja
--rw-r--r--   0        0        0     2732 2023-07-08 15:59:26.359390 nb-cli-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 nb-cli-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-09 06:24:59.789085 nb-cli-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3347 2023-07-09 06:24:59.789085 nb-cli-1.2.1/README.md
+-rw-r--r--   0        0        0      246 2023-07-09 06:24:59.789085 nb-cli-1.2.1/build.py
+-rw-r--r--   0        0        0      795 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/__init__.py
+-rw-r--r--   0        0        0      202 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/__main__.py
+-rw-r--r--   0        0        0     3305 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/__init__.py
+-rw-r--r--   0        0        0      257 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6866 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/adapter.py
+-rw-r--r--   0        0        0     4243 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/driver.py
+-rw-r--r--   0        0        0     7195 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/plugin.py
+-rw-r--r--   0        0        0    10538 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/project.py
+-rw-r--r--   0        0        0     3409 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/commands/self.py
+-rw-r--r--   0        0        0     5618 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/customize.py
+-rw-r--r--   0        0        0     1966 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/cli/utils.py
+-rw-r--r--   0        0        0      429 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/config/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/config/model.py
+-rw-r--r--   0        0        0     6220 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/config/parser.py
+-rw-r--r--   0        0        0      347 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/consts.py
+-rw-r--r--   0        0        0      472 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/exceptions.py
+-rw-r--r--   0        0        0      214 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/extensions.py
+-rw-r--r--   0        0        0     3030 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/__init__.py
+-rw-r--r--   0        0        0      865 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/adapter.py
+-rw-r--r--   0        0        0      374 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/driver.py
+-rw-r--r--   0        0        0     6766 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/meta.py
+-rw-r--r--   0        0        0     3198 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/pip.py
+-rw-r--r--   0        0        0     1557 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/plugin.py
+-rw-r--r--   0        0        0     2990 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/process.py
+-rw-r--r--   0        0        0     2665 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/project.py
+-rw-r--r--   0        0        0     5718 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/reloader.py
+-rw-r--r--   0        0        0     2150 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/script.py
+-rw-r--r--   0        0        0     1860 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/signal.py
+-rw-r--r--   0        0        0     4082 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/store.py
+-rw-r--r--   0        0        0      734 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/handlers/venv.py
+-rw-r--r--   0        0        0     1193 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/i18n.py
+-rw-r--r--   0        0        0     8966 2023-07-09 06:25:33.789020 nb-cli-1.2.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
+-rw-r--r--   0        0        0    13886 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
+-rw-r--r--   0        0        0      635 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/log/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/py.typed
+-rw-r--r--   0        0        0      143 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/cookiecutter.json
+-rw-r--r--   0        0        0      120 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      847 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      354 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      203 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      688 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      676 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      164 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/plugin/cookiecutter.json
+-rw-r--r--   0        0        0      315 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/plugin/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      365 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      114 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0        0 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      318 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/project/bootstrap/cookiecutter.json
+-rw-r--r--   0        0        0      236 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/project/bootstrap/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      141 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0      232 2023-07-09 06:24:59.789085 nb-cli-1.2.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      620 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      501 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/cookiecutter.json
+-rw-r--r--   0        0        0      307 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      236 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      157 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
+-rw-r--r--   0        0        0       16 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
+-rw-r--r--   0        0        0        0 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0     2087 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
+-rw-r--r--   0        0        0      328 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      666 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      232 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/meta/_package_version.py.jinja
+-rw-r--r--   0        0        0      110 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/meta/nonebot_version.py.jinja
+-rw-r--r--   0        0        0      105 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/meta/pip_version.py.jinja
+-rw-r--r--   0        0        0      142 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/meta/python_version.py.jinja
+-rw-r--r--   0        0        0      181 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
+-rw-r--r--   0        0        0     1091 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/project/_prepare.py.jinja
+-rw-r--r--   0        0        0      151 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/project/run_project.py.jinja
+-rw-r--r--   0        0        0      222 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/script/_entrypoint.py.jinja
+-rw-r--r--   0        0        0      158 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/script/list_scripts.py.jinja
+-rw-r--r--   0        0        0      333 2023-07-09 06:24:59.793084 nb-cli-1.2.1/nb_cli/template/scripts/script/run_script.py.jinja
+-rw-r--r--   0        0        0     2732 2023-07-09 06:24:59.793084 nb-cli-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 nb-cli-1.2.1/PKG-INFO
```

### Comparing `nb-cli-1.2.0/LICENSE` & `nb-cli-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/README.md` & `nb-cli-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/__init__.py` & `nb-cli-1.2.1/nb_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/cli/__init__.py` & `nb-cli-1.2.1/nb_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/cli/commands/adapter.py` & `nb-cli-1.2.1/nb_cli/cli/commands/adapter.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/cli/commands/driver.py` & `nb-cli-1.2.1/nb_cli/cli/commands/driver.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/cli/commands/plugin.py` & `nb-cli-1.2.1/nb_cli/cli/commands/plugin.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/cli/commands/project.py` & `nb-cli-1.2.1/nb_cli/cli/commands/project.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/cli/commands/self.py` & `nb-cli-1.2.1/nb_cli/cli/commands/self.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/cli/customize.py` & `nb-cli-1.2.1/nb_cli/cli/customize.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import partial
 from collections import Counter
 from typing import Dict, List, Optional
 
 import click
 
 from nb_cli import _, cache
+from nb_cli.exceptions import ProjectNotFoundError
 from nb_cli.handlers import run_script, list_scripts
 
 from .utils import run_async
 
 
 class ClickAliasedCommand(click.Command):
     def __init__(self, *args, **kwargs) -> None:
@@ -114,15 +115,20 @@
                 script_name=script_name,
             )
         )
 
     @run_async  # type: ignore
     @cache(ttl=None)
     async def _load_scripts(self, ctx: click.Context) -> List[click.Command]:
-        scripts = await list_scripts()
+        try:
+            scripts = await list_scripts()
+        except ProjectNotFoundError:
+            # not in a project
+            return []
+
         # check duplicate
         elements = Counter(scripts).most_common()
         if elements and elements[0][1] > 1:
             script_names = ", ".join(e[0] for e in elements if e[1] > 1)
             raise ValueError(
                 f"Duplicate script names {script_names} found. "
                 "Please check your configuration."
```

### Comparing `nb-cli-1.2.0/nb_cli/cli/utils.py` & `nb-cli-1.2.1/nb_cli/cli/utils.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/config/model.py` & `nb-cli-1.2.1/nb_cli/config/model.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/config/parser.py` & `nb-cli-1.2.1/nb_cli/config/parser.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/__init__.py` & `nb-cli-1.2.1/nb_cli/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/adapter.py` & `nb-cli-1.2.1/nb_cli/handlers/adapter.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/meta.py` & `nb-cli-1.2.1/nb_cli/handlers/meta.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/pip.py` & `nb-cli-1.2.1/nb_cli/handlers/pip.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/plugin.py` & `nb-cli-1.2.1/nb_cli/handlers/plugin.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/process.py` & `nb-cli-1.2.1/nb_cli/handlers/process.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/project.py` & `nb-cli-1.2.1/nb_cli/handlers/project.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/reloader.py` & `nb-cli-1.2.1/nb_cli/handlers/reloader.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/script.py` & `nb-cli-1.2.1/nb_cli/handlers/script.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/signal.py` & `nb-cli-1.2.1/nb_cli/handlers/signal.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/store.py` & `nb-cli-1.2.1/nb_cli/handlers/store.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/handlers/venv.py` & `nb-cli-1.2.1/nb_cli/handlers/venv.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/i18n.py` & `nb-cli-1.2.1/nb_cli/i18n.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo` & `nb-cli-1.2.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: nb-cli 1.0.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-08 15:40+0000\n"
+"POT-Creation-Date: 2023-07-09 06:14+0000\n"
 "PO-Revision-Date: 2023-01-11 08:56+0000\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
```

### Comparing `nb-cli-1.2.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po` & `nb-cli-1.2.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the nb-cli project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: nb-cli 1.0.0\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-07-08 15:40+0000\n"
+"POT-Creation-Date: 2023-07-09 06:14+0000\n"
 "PO-Revision-Date: 2023-01-11 08:56+0000\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: zh_Hans_CN\n"
 "Language-Team: zh_Hans_CN <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
@@ -42,15 +42,15 @@
 
 #: nb_cli/cli/__init__.py:104 nb_cli/cli/commands/adapter.py:45
 #: nb_cli/cli/commands/driver.py:42 nb_cli/cli/commands/plugin.py:45
 #: nb_cli/cli/commands/self.py:41
 msgid "What do you want to do?"
 msgstr "你想要进行什么操作?"
 
-#: nb_cli/cli/customize.py:108
+#: nb_cli/cli/customize.py:109
 msgid "Run script {script_name!r}"
 msgstr "运行脚本 {script_name!r}"
 
 #: nb_cli/cli/utils.py:53
 msgid "Package {name} not found."
 msgstr "包 {name} 未找到."
```

### Comparing `nb-cli-1.2.0/nb_cli/log/__init__.py` & `nb-cli-1.2.1/nb_cli/log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}` & `nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}` & `nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}` & `nb-cli-1.2.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb-cli-1.2.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore` & `nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb-cli-1.2.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/nb_cli/template/scripts/project/_prepare.py.jinja` & `nb-cli-1.2.1/nb_cli/template/scripts/project/_prepare.py.jinja`

 * *Files identical despite different names*

### Comparing `nb-cli-1.2.0/pyproject.toml` & `nb-cli-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nb-cli"
-version = "1.2.0"
+version = "1.2.1"
 description = "CLI for nonebot2"
 authors = [
     { name = "yanyongyu", email = "yyy@nonebot.dev" },
 ]
 readme = "README.md"
 keywords = [
     "bot",
```

### Comparing `nb-cli-1.2.0/PKG-INFO` & `nb-cli-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-cli
-Version: 1.2.0
+Version: 1.2.1
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

 * *File "/tmp/diffoscope_gfan1jey_/tmpm181kiqx_TarContainer/0/76", line 148, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_gfan1jey_/tmpm181kiqx_TarContainer/0/76", line 148, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nb-cli Version: 1.2.0 Summary: CLI for nonebot2
+Metadata-Version: 2.1 Name: nb-cli Version: 1.2.1 Summary: CLI for nonebot2
 License: MIT Keywords: bot,qq,nonebot,bot,qq,nonebot Author-email: yanyongyu
 nonebot.dev> Requires-Python: >=3.8, <4.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Framework :: Robot Framework Classifier:
 Framework :: Robot Framework :: Library Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Project-URL: homepage, https://
 cli.nonebot.dev/ Project-URL: repository, https://github.com/nonebot/nb-cli
```

