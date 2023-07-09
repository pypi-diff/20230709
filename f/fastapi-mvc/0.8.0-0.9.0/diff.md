# Comparing `tmp/fastapi-mvc-0.8.0.tar.gz` & `tmp/fastapi-mvc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-mvc-0.8.0.tar", max compression
+gzip compressed data, was "fastapi-mvc-0.9.0.tar", max compression
```

## Comparing `fastapi-mvc-0.8.0.tar` & `fastapi-mvc-0.9.0.tar`

### file list

```diff
@@ -1,108 +1,117 @@
--rw-r--r--   0        0        0     1074 2022-02-08 21:32:54.638904 fastapi-mvc-0.8.0/LICENSE
--rw-r--r--   0        0        0    10791 2022-02-08 21:32:54.638904 fastapi-mvc-0.8.0/README.md
--rw-r--r--   0        0        0      177 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/__init__.py
--rw-r--r--   0        0        0       94 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/__main__.py
--rw-r--r--   0        0        0       19 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/cli/__init__.py
--rw-r--r--   0        0        0      866 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/cli/cli.py
--rw-r--r--   0        0        0       19 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/cli/commands/__init__.py
--rw-r--r--   0        0        0     3008 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/cli/commands/new.py
--rw-r--r--   0        0        0     1472 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/cli/commands/run.py
--rw-r--r--   0        0        0      107 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/generators/__init__.py
--rw-r--r--   0        0        0     1547 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/generators/project.py
--rw-r--r--   0        0        0      131 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/parsers/__init__.py
--rw-r--r--   0        0        0     1969 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/parsers/ini.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/template/__init__.py
--rw-r--r--   0        0        0     1141 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/template/cookiecutter.json
--rw-r--r--   0        0        0     1951 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/template/hooks/post_gen_project.py
--rw-r--r--   0        0        0      221 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.dockerignore
--rw-r--r--   0        0        0     1238 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.github/workflows/integration.yml
--rw-r--r--   0        0        0     5928 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.github/workflows/main.yml
--rw-r--r--   0        0        0      387 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.gitignore
--rw-r--r--   0        0        0      225 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/CHANGELOG.md
--rw-r--r--   0        0        0     2674 2022-02-08 21:32:54.642904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Dockerfile
--rw-r--r--   0        0        0    77126 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/LICENSE
--rw-r--r--   0        0        0     1413 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Makefile
--rw-r--r--   0        0        0    16148 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/README.md
--rw-r--r--   0        0        0       24 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/TAG
--rw-r--r--   0        0        0     2045 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Vagrantfile
--rwxr-xr-x   0        0        0      533 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/clean-image.sh
--rwxr-xr-x   0        0        0     3970 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/dev-env.sh
--rwxr-xr-x   0        0        0      525 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/image.sh
--rwxr-xr-x   0        0        0     1889 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/install.sh
--rwxr-xr-x   0        0        0      285 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/integration-test.sh
--rwxr-xr-x   0        0        0     1326 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/metrics.sh
--rwxr-xr-x   0        0        0      264 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/unit-test.sh
--rw-r--r--   0        0        0      349 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/.helmignore
--rw-r--r--   0        0        0     1183 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/Chart.yaml
--rw-r--r--   0        0        0     2127 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/README.md
--rw-r--r--   0        0        0     1932 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/NOTES.txt
--rw-r--r--   0        0        0     2213 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/_helpers.tpl
--rw-r--r--   0        0        0      547 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/configmap.yml
--rw-r--r--   0        0        0     3242 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/deployment.yaml
--rw-r--r--   0        0        0     1060 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/hpa.yaml
--rw-r--r--   0        0        0      774 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/ingress.yaml
--rw-r--r--   0        0        0      516 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/service.yaml
--rw-r--r--   0        0        0      423 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      523 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0     1901 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/values.yaml
--rw-r--r--   0        0        0      407 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/fastapi-mvc.ini
--rw-r--r--   0        0        0     1885 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/manifests/all-redis-operator-resources.yaml
--rw-r--r--   0        0        0      568 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/manifests/persistent-storage-no-pvc-deletion.yaml
--rw-r--r--   0        0        0     1464 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/pyproject.toml
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/integration/__init__.py
--rw-r--r--   0        0        0     1010 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/integration/test_ready_endpoint.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/__init__.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/__init__.py
--rw-r--r--   0        0        0      442 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/conftest.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/controllers/__init__.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/controllers/api/__init__.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/controllers/api/v1/__init__.py
--rw-r--r--   0        0        0      725 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/controllers/api/v1/test_ready.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/exceptions/__init__.py
--rw-r--r--   0        0        0     1489 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/exceptions/test_http.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/models/__init__.py
--rw-r--r--   0        0        0      783 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/models/test_ready.py
--rw-r--r--   0        0        0     2670 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/models/test_response.py
--rw-r--r--   0        0        0      966 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/test_asgi.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/utils/__init__.py
--rw-r--r--   0        0        0     8227 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/utils/test_aiohttp_client.py
--rw-r--r--   0        0        0     3559 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/utils/test_redis.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/__init__.py
--rw-r--r--   0        0        0        0 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/commands/__init__.py
--rw-r--r--   0        0        0     3582 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/commands/test_serve.py
--rw-r--r--   0        0        0      108 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/conftest.py
--rw-r--r--   0        0        0      628 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/test_cli.py
--rw-r--r--   0        0        0     1702 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/test_wsgi.py
--rw-r--r--   0        0        0      224 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/__init__.py
--rw-r--r--   0        0        0       67 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/__init__.py
--rw-r--r--   0        0        0     2772 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/asgi.py
--rw-r--r--   0        0        0       67 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/controllers/__init__.py
--rw-r--r--   0        0        0       67 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/controllers/api/__init__.py
--rw-r--r--   0        0        0       67 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/controllers/api/v1/__init__.py
--rw-r--r--   0        0        0     2038 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/controllers/api/v1/ready.py
--rw-r--r--   0        0        0      175 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/exceptions/__init__.py
--rw-r--r--   0        0        0     2586 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/exceptions/http.py
--rw-r--r--   0        0        0      189 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/models/__init__.py
--rw-r--r--   0        0        0     1539 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/models/ready.py
--rw-r--r--   0        0        0     3700 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/models/response.py
--rw-r--r--   0        0        0      415 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/utils/__init__.py
--rw-r--r--   0        0        0     6441 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/utils/aiohttp_client.py
--rw-r--r--   0        0        0     8385 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/utils/redis.py
--rw-r--r--   0        0        0       67 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/__init__.py
--rw-r--r--   0        0        0      658 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/cli.py
--rw-r--r--   0        0        0       67 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/commands/__init__.py
--rw-r--r--   0        0        0     2572 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/commands/serve.py
--rw-r--r--   0        0        0      316 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/__init__.py
--rw-r--r--   0        0        0     1546 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/application.py
--rw-r--r--   0        0        0     7480 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/gunicorn.conf.py
--rw-r--r--   0        0        0     1295 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/redis.py
--rw-r--r--   0        0        0      289 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/router.py
--rw-r--r--   0        0        0      114 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/version.py
--rw-r--r--   0        0        0     1601 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/wsgi.py
--rw-r--r--   0        0        0       88 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/utils/__init__.py
--rw-r--r--   0        0        0     2454 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/utils/shell.py
--rw-r--r--   0        0        0       73 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/fastapi_mvc/version.py
--rw-r--r--   0        0        0     1671 2022-02-08 21:32:54.646904 fastapi-mvc-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    14673 2022-02-08 21:33:00.194974 fastapi-mvc-0.8.0/setup.py
--rw-r--r--   0        0        0    12238 2022-02-08 21:33:00.195792 fastapi-mvc-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-02-14 21:30:59.764882 fastapi-mvc-0.9.0/LICENSE
+-rw-r--r--   0        0        0    10572 2022-02-14 21:30:59.764882 fastapi-mvc-0.9.0/README.md
+-rw-r--r--   0        0        0      177 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/__init__.py
+-rw-r--r--   0        0        0       94 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/__main__.py
+-rw-r--r--   0        0        0       19 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/cli/__init__.py
+-rw-r--r--   0        0        0      848 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/cli/cli.py
+-rw-r--r--   0        0        0     2112 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/cli/new.py
+-rw-r--r--   0        0        0     1063 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/cli/run.py
+-rw-r--r--   0        0        0      481 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/commands/__init__.py
+-rw-r--r--   0        0        0      639 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/commands/base.py
+-rw-r--r--   0        0        0      899 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/commands/install_project.py
+-rw-r--r--   0        0        0     1822 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/commands/invoker.py
+-rw-r--r--   0        0        0     2533 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/commands/new_project.py
+-rw-r--r--   0        0        0     1252 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/commands/run_uvicorn.py
+-rw-r--r--   0        0        0     1391 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/commands/verify_install.py
+-rw-r--r--   0        0        0      191 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/exceptions/__init__.py
+-rw-r--r--   0        0        0      168 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/exceptions/command.py
+-rw-r--r--   0        0        0      166 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/exceptions/ini.py
+-rw-r--r--   0        0        0      107 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/generators/__init__.py
+-rw-r--r--   0        0        0     1549 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/generators/project.py
+-rw-r--r--   0        0        0      131 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/parsers/__init__.py
+-rw-r--r--   0        0        0     3730 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/parsers/ini.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/template/__init__.py
+-rw-r--r--   0        0        0     1141 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/template/cookiecutter.json
+-rw-r--r--   0        0        0     1951 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/template/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      221 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.dockerignore
+-rw-r--r--   0        0        0     1238 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.github/workflows/integration.yml
+-rw-r--r--   0        0        0     5928 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.github/workflows/main.yml
+-rw-r--r--   0        0        0      387 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.gitignore
+-rw-r--r--   0        0        0      225 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/CHANGELOG.md
+-rw-r--r--   0        0        0     2674 2022-02-14 21:30:59.768882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Dockerfile
+-rw-r--r--   0        0        0    77126 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/LICENSE
+-rw-r--r--   0        0        0     1413 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Makefile
+-rw-r--r--   0        0        0    16148 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/README.md
+-rw-r--r--   0        0        0       24 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/TAG
+-rw-r--r--   0        0        0     2045 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Vagrantfile
+-rwxr-xr-x   0        0        0      533 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/clean-image.sh
+-rwxr-xr-x   0        0        0     3970 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/dev-env.sh
+-rwxr-xr-x   0        0        0      525 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/image.sh
+-rwxr-xr-x   0        0        0     1889 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/install.sh
+-rwxr-xr-x   0        0        0      285 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/integration-test.sh
+-rwxr-xr-x   0        0        0     1326 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/metrics.sh
+-rwxr-xr-x   0        0        0      264 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/unit-test.sh
+-rw-r--r--   0        0        0      349 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/.helmignore
+-rw-r--r--   0        0        0     1183 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/Chart.yaml
+-rw-r--r--   0        0        0     2127 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/README.md
+-rw-r--r--   0        0        0     1932 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/NOTES.txt
+-rw-r--r--   0        0        0     2213 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/_helpers.tpl
+-rw-r--r--   0        0        0      547 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/configmap.yml
+-rw-r--r--   0        0        0     3242 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/deployment.yaml
+-rw-r--r--   0        0        0     1060 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/hpa.yaml
+-rw-r--r--   0        0        0      774 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/ingress.yaml
+-rw-r--r--   0        0        0      516 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/service.yaml
+-rw-r--r--   0        0        0      423 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      523 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0     1901 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/values.yaml
+-rw-r--r--   0        0        0      407 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/fastapi-mvc.ini
+-rw-r--r--   0        0        0     1885 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/manifests/all-redis-operator-resources.yaml
+-rw-r--r--   0        0        0      568 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/manifests/persistent-storage-no-pvc-deletion.yaml
+-rw-r--r--   0        0        0     1464 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1010 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/integration/test_ready_endpoint.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/__init__.py
+-rw-r--r--   0        0        0      442 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/conftest.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/controllers/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/controllers/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/controllers/api/v1/__init__.py
+-rw-r--r--   0        0        0      725 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/controllers/api/v1/test_ready.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/exceptions/__init__.py
+-rw-r--r--   0        0        0     1489 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/exceptions/test_http.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/models/__init__.py
+-rw-r--r--   0        0        0      783 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/models/test_ready.py
+-rw-r--r--   0        0        0     2670 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/models/test_response.py
+-rw-r--r--   0        0        0      966 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/test_asgi.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/utils/__init__.py
+-rw-r--r--   0        0        0     8227 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/utils/test_aiohttp_client.py
+-rw-r--r--   0        0        0     3559 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/utils/test_redis.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3582 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/commands/test_serve.py
+-rw-r--r--   0        0        0      108 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/conftest.py
+-rw-r--r--   0        0        0      628 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/test_cli.py
+-rw-r--r--   0        0        0     1702 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/test_wsgi.py
+-rw-r--r--   0        0        0      224 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/__init__.py
+-rw-r--r--   0        0        0       67 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/__init__.py
+-rw-r--r--   0        0        0     2772 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/asgi.py
+-rw-r--r--   0        0        0       67 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/controllers/__init__.py
+-rw-r--r--   0        0        0       67 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/controllers/api/__init__.py
+-rw-r--r--   0        0        0       67 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/controllers/api/v1/__init__.py
+-rw-r--r--   0        0        0     2038 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/controllers/api/v1/ready.py
+-rw-r--r--   0        0        0      175 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/exceptions/__init__.py
+-rw-r--r--   0        0        0     2586 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/exceptions/http.py
+-rw-r--r--   0        0        0      189 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/models/__init__.py
+-rw-r--r--   0        0        0     1539 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/models/ready.py
+-rw-r--r--   0        0        0     3700 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/models/response.py
+-rw-r--r--   0        0        0      415 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/utils/__init__.py
+-rw-r--r--   0        0        0     6441 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/utils/aiohttp_client.py
+-rw-r--r--   0        0        0     8385 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/utils/redis.py
+-rw-r--r--   0        0        0       67 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/__init__.py
+-rw-r--r--   0        0        0      658 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/cli.py
+-rw-r--r--   0        0        0       67 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2572 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/commands/serve.py
+-rw-r--r--   0        0        0      316 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/__init__.py
+-rw-r--r--   0        0        0     1546 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/application.py
+-rw-r--r--   0        0        0     7480 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/gunicorn.conf.py
+-rw-r--r--   0        0        0     1295 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/redis.py
+-rw-r--r--   0        0        0      289 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/router.py
+-rw-r--r--   0        0        0      114 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/version.py
+-rw-r--r--   0        0        0     1601 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/wsgi.py
+-rw-r--r--   0        0        0       88 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/utils/__init__.py
+-rw-r--r--   0        0        0     3249 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/utils/shell.py
+-rw-r--r--   0        0        0       73 2022-02-14 21:30:59.772882 fastapi-mvc-0.9.0/fastapi_mvc/version.py
+-rw-r--r--   0        0        0     1616 2022-02-14 21:30:59.776883 fastapi-mvc-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    14434 2022-02-14 21:31:07.028244 fastapi-mvc-0.9.0/setup.py
+-rw-r--r--   0        0        0    11967 2022-02-14 21:31:07.029023 fastapi-mvc-0.9.0/PKG-INFO
```

### Comparing `fastapi-mvc-0.8.0/LICENSE` & `fastapi-mvc-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/README.md` & `fastapi-mvc-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -252,21 +252,17 @@
 
   Run development uvicorn server.
 
   The 'fastapi-mvc run' commands runs development uvicorn server for a
   fastapi-mvc project at the current working directory.
 
 Options:
-  --host TEXT                  Host to bind.  [default: 127.0.0.1]
-  -p, --port INTEGER           Port to bind.  [default: 8000]
-  -w, --workers INTEGER RANGE  The number of worker processes for handling
-                               requests.  [default: 1]
-
-  --no-reload                  Disable auto-reload.
-  --help                       Show this message and exit.
+  --host TEXT      Host to bind.  [default: 127.0.0.1]
+  -p, --port TEXT  Port to bind.  [default: 8000]
+  --help           Show this message and exit.
 ```
 
 ## Contributing
 
 [CONTRIBUTING](https://github.com/rszamszur/fastapi-mvc/blob/master/CONTRIBUTING.md)
 
 ## License
```

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/cli/cli.py` & `fastapi-mvc-0.9.0/fastapi_mvc/cli/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """FastAPI MVC CLI root implementation."""
 import logging
 
 import click
-from fastapi_mvc.cli.commands.new import new
-from fastapi_mvc.cli.commands.run import run
+from fastapi_mvc.cli.new import new
+from fastapi_mvc.cli.run import run
 
 
 @click.group()
 @click.option(
     "-v",
     "--verbose",
     help="Enable verbose logging.",
```

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/cli/commands/new.py` & `fastapi-mvc-0.9.0/fastapi_mvc/cli/new.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 """FastAPI MVC CLI new command implementation."""
-import os
-from datetime import datetime
-
 import click
-from fastapi_mvc.generators import ProjectGenerator
-from fastapi_mvc.utils import ShellUtils
-from fastapi_mvc.version import __version__
+from fastapi_mvc.commands import Invoker, GenerateNewProject, InstallProject
 
 
 @click.command()
 @click.argument(
     "APP_PATH",
     nargs=1,
     type=click.Path(exists=False),
@@ -93,36 +88,14 @@
     \f
 
     Args:
         app_path(str): CLI command argument - new application path.
         options(dict): CLI command options.
 
     """
-    app_name = os.path.basename(app_path)
-    output_dir = os.path.dirname(app_path)
-
-    if not output_dir:
-        output_dir = "."
-
-    author, email = ShellUtils.get_git_user_info()
-
-    context = {
-        "project_name": app_name,
-        "redis": "no" if options["skip_redis"] else "yes",
-        "aiohttp": "no" if options["skip_aiohttp"] else "yes",
-        "github_actions": "no" if options["skip_actions"] else "yes",
-        "vagrantfile": "no" if options["skip_vagrantfile"] else "yes",
-        "helm": "no" if options["skip_helm"] else "yes",
-        "codecov": "no" if options["skip_codecov"] else "yes",
-        "author": author,
-        "email": email,
-        "license": options["license"],
-        "repo_url": options["repo_url"],
-        "year": datetime.today().year,
-        "fastapi_mvc_version": __version__,
-    }
-
-    generator = ProjectGenerator()
-    generator.new(context=context, output_dir=output_dir)
+    invoker = Invoker()
+    invoker.on_start = GenerateNewProject(app_path=app_path, options=options)
 
     if not options["skip_install"]:
-        ShellUtils.run_project_install(app_path)
+        invoker.on_finish = InstallProject(app_path=app_path)
+
+    invoker.execute()
```

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/generators/project.py` & `fastapi-mvc-0.9.0/fastapi_mvc/generators/project.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class ProjectGenerator(object):
     """Project generator class definition."""
 
     def __init__(self):
         """Initialize ProjectGenerator class object instance."""
         self._log = logging.getLogger(self.__class__.__name__)
-        self._log.info("Initialize fastapi-mvc project generator.")
+        self._log.debug("Initialize fastapi-mvc project generator.")
         self._template_dir = os.path.abspath(
             os.path.join(
                 os.path.abspath(__file__),
                 "../../template",
             )
         )
 
@@ -28,15 +28,15 @@
             output_dir(str): Directory in which the project is to be created.
 
         Raises:
             OutputDirExistsException: If provided output directory already
                 exists.
 
         """
-        self._log.info(
+        self._log.debug(
             "Begin generating a new project at path: {0:s}".format(output_dir)
         )
         self._log.debug("Cookiecutter context: {0}".format(context))
 
         try:
             cookiecutter(
                 self._template_dir,
```

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/cookiecutter.json` & `fastapi-mvc-0.9.0/fastapi_mvc/template/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/hooks/post_gen_project.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.github/workflows/integration.yml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.github/workflows/integration.yml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.github/workflows/main.yml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Dockerfile` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Dockerfile`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/LICENSE` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Makefile` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Makefile`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/README.md` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Vagrantfile` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/Vagrantfile`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/clean-image.sh` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/clean-image.sh`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/dev-env.sh` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/dev-env.sh`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/image.sh` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/image.sh`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/install.sh` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/install.sh`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/metrics.sh` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/build/metrics.sh`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/Chart.yaml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/Chart.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/README.md` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/README.md`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/NOTES.txt` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/_helpers.tpl` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/configmap.yml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/configmap.yml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/deployment.yaml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/hpa.yaml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/ingress.yaml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/ingress.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/service.yaml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/service.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/tests/test-connection.yaml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/tests/test-connection.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/values.yaml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/values.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/manifests/all-redis-operator-resources.yaml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/manifests/all-redis-operator-resources.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/manifests/persistent-storage-no-pvc-deletion.yaml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/manifests/persistent-storage-no-pvc-deletion.yaml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/pyproject.toml` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/integration/test_ready_endpoint.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/integration/test_ready_endpoint.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/controllers/api/v1/test_ready.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/controllers/api/v1/test_ready.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/exceptions/test_http.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/exceptions/test_http.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/models/test_ready.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/models/test_ready.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/models/test_response.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/models/test_response.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/test_asgi.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/test_asgi.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/utils/test_aiohttp_client.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/utils/test_aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/utils/test_redis.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/app/utils/test_redis.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/commands/test_serve.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/commands/test_serve.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/test_cli.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/test_wsgi.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/tests/unit/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/asgi.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/asgi.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/controllers/api/v1/ready.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/controllers/api/v1/ready.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/exceptions/http.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/exceptions/http.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/models/ready.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/models/ready.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/models/response.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/models/response.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/utils/aiohttp_client.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/utils/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/utils/redis.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/app/utils/redis.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/cli.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/commands/serve.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/cli/commands/serve.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/application.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/application.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/gunicorn.conf.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/redis.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/config/redis.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/wsgi.py` & `fastapi-mvc-0.9.0/fastapi_mvc/template/{{cookiecutter.folder_name}}/{{cookiecutter.package_name}}/wsgi.py`

 * *Files identical despite different names*

### Comparing `fastapi-mvc-0.8.0/pyproject.toml` & `fastapi-mvc-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-mvc"
-version = "0.8.0"
+version = "0.9.0"
 description = "Create and develop production grade FastAPI projects."
 authors = ["Radosław Szamszur <radoslawszamszur@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/rszamszur/fastapi-mvc"
 documentation = "https://fastapi-mvc.netlify.app"
 classifiers = [
@@ -25,15 +25,14 @@
     "Framework :: FastAPI",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 cookiecutter = "~1.7.3"
 click = "~7.1.2"
-uvicorn = {extras = ["standard"], version = "~0.17.4"}
 
 [tool.poetry.dev-dependencies]
 pytest = "~6.2.5"
 pytest-cov = "~2.12.0"
 pytest-cookies = "~0.6.1"
 flake8 = "~3.9.2"
 flake8-docstrings = "~1.6.0"
```

### Comparing `fastapi-mvc-0.8.0/setup.py` & `fastapi-mvc-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['fastapi_mvc',
  'fastapi_mvc.cli',
- 'fastapi_mvc.cli.commands',
+ 'fastapi_mvc.commands',
+ 'fastapi_mvc.exceptions',
  'fastapi_mvc.generators',
  'fastapi_mvc.parsers',
  'fastapi_mvc.template',
  'fastapi_mvc.template.hooks',
  'fastapi_mvc.template.{{cookiecutter.folder_name}}.tests',
  'fastapi_mvc.template.{{cookiecutter.folder_name}}.tests.integration',
  'fastapi_mvc.template.{{cookiecutter.folder_name}}.tests.unit',
@@ -41,26 +42,24 @@
                           '{{cookiecutter.folder_name}}/build/*',
                           '{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/*',
                           '{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/*',
                           '{{cookiecutter.folder_name}}/charts/{{cookiecutter.chart_name}}/templates/tests/*',
                           '{{cookiecutter.folder_name}}/manifests/*']}
 
 install_requires = \
-['click>=7.1.2,<7.2.0',
- 'cookiecutter>=1.7.3,<1.8.0',
- 'uvicorn[standard]>=0.17.4,<0.18.0']
+['click>=7.1.2,<7.2.0', 'cookiecutter>=1.7.3,<1.8.0']
 
 entry_points = \
 {'console_scripts': ['fastapi-mvc = fastapi_mvc.cli.cli:cli']}
 
 setup_kwargs = {
     'name': 'fastapi-mvc',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'Create and develop production grade FastAPI projects.',
-    'long_description': '<div align="center">\n<h1>fastapi-mvc</h1>\n\n![fastapi-mvc](https://github.com/rszamszur/fastapi-mvc-template/blob/master/assets/readme.gif?raw=true)\n[![CI](https://github.com/rszamszur/fastapi-mvc/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/rszamszur/fastapi-mvc/actions/workflows/main.yml)\n[![codecov](https://codecov.io/gh/rszamszur/fastapi-mvc/branch/master/graph/badge.svg?token=7ESV30TYZS)](https://codecov.io/gh/rszamszur/fastapi-mvc)\n[![K8s integration](https://github.com/rszamszur/fastapi-mvc/actions/workflows/integration.yml/badge.svg)](https://github.com/rszamszur/fastapi-mvc/actions/workflows/integration.yml)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![PyPI](https://img.shields.io/pypi/v/fastapi-mvc)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/fastapi-mvc)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastapi-mvc)\n![GitHub](https://img.shields.io/github/license/rszamszur/fastapi-mvc?color=blue)\n\n</div>\n\n---\n\n**Documentation**: [https://fastapi-mvc.netlify.app](https://fastapi-mvc.netlify.app)\n\n**Source Code**: [https://github.com/rszamszur/fastapi-mvc](https://github.com/rszamszur/fastapi-mvc)\n\n**Example generated project**: https://github.com/rszamszur/fastapi-mvc-example\n\n---\n\n## Features\n<details>\n  <summary>Generated project core implemented using MVC architectural pattern</summary>\n  \n  Generated project is structured in MVC architectural pattern to help developers who don\'t know FastAPI yet but are familiar with MVC to get up to speed quickly.\n</details>\n\n<details>\n  <summary>WSGI + ASGI for high performance and better configuration</summary>\n\n#### TLDR;\n\nRunning WSGI as a master worker with ASGI workers gives better results than running pure ASGI (for FastAPI for now):\n* better performance (requests per second)\n* better support for different protocols\n* broader configuration\n* better support with using reverse proxy\n---\nFirst of all, whether it\'s ASGI, WSGI, or combined, think of this as something that serves the application. For instance, Ruby on Rails uses Puma. The result of any of those servers is a TCP/IP or UNIX socket which is later on utilized by reverse proxy ex: Nginx (a TCP/IP socket you can access directly over the network, but still in production, usually it\'ll be behind a reverse proxy).\n\nNow to WSGI + ASGI part. FastAPI is implemented with asyncio (https://docs.python.org/3/library/asyncio.html), so having a pure WSGI server doesn\'t make sense since you\'d lose all the benefits of asynchronous concurrency. That\'s where ASGI comes in. However, Python journey with asyncio is still pretty young. Most projects have yet to reach maturity level (you should expect early bugs and a limited feature set). FastAPI, as ASGI server uses uvicorn, which is still prior 1.x.x release (17 in total so far, current 0.16.0) and lacks support for some protocols (ex: no HTTP/2).\nMoreover, some reverse proxy might not know how to work with asynchronous servers, and some problems or early bugs on this layer might happen as well.\n\nI\'m not saying uvicorn is bad. Quite contrary, if you\'d run 4 pure uvicorn workes, you\'d still get great results. But if you\'d run the same amount of workers with gunicorn (WSGI) as a master worker, it turns out you can even pump those numbers up.\n\nGunicorn with 4 Uvicorn Workers (source: https://stackoverflow.com/a/62977786/10566747):\n```\nRequests per second: 7891.28 [#/sec] (mean)\nTime per request: 126.722 [ms] (mean)\nTime per request: 0.127 [ms] (mean, across all concurrent requests)\n```\n\nPure Uvicorn with 4 workers:\n```\nRequests per second: 4359.68 [#/sec] (mean)\nTime per request: 229.375 [ms] (mean)\nTime per request: 0.229 [ms] (mean, across all concurrent requests)\n```\n\n~80% better\n\nI guess gunicorn does a better job in worker management. However, it\'s a more mature project, so it\'s probably a matter of time when uvicorn (or other ASGI for that matter) will catch up to this benchmark.\n\nLast but not least, gunicorn gives a ton of settings to configure (https://docs.gunicorn.org/en/stable/settings.html), which can come in handy.\n</details>\n\n<details>\n  <summary>Generated project comes with tests at 99% coverage</summary>\n  \n  Unit test coverage is at 99% regardless of chosen configuration. There is also a placeholder for integration tests with an example dummy test.\n</details>\n\n<details>\n  <summary>Proper Dockerfile created with best practices for the cloud and Kubernetes</summary>\n  \nContainer image features:\n* Based on distroless image\n* Run as PID 1 (with child processes)\n* Utilizes multi-stage build for smallest size possible, also this results in having only necessary libraries/dependencies/tools in outcome container image.\n* DigestSHA - immutable identifier instead of tags, for better reproducibility and security.\n* Signal handling, for Kubernetes to be able to gracefully shut down pods.\n* Created with common layers.\n* By default runs as non-root user\n\nBased on Google [Best practices for building containers](https://cloud.google.com/architecture/best-practices-for-building-containers), [Top 20 Dockerfile best practices](https://sysdig.com/blog/dockerfile-best-practices), and own experience.\n</details>\n\n<details>\n  <summary>Extensive GitHub actions for CI</summary>\n  \n![ci_example](https://github.com/rszamszur/fastapi-mvc-template/blob/master/assets/ci.png?raw=true)\n</details>\n\n<details>\n  <summary>Helm chart for Kubernetes</summary>\n  \nFor easily deploying application in Kubernetes cluster.\n</details>\n\n<details>\n  <summary>Reproducible virtualized development environment</summary>\n\nEasily boot virtual machine with Vagrant. Code and test straight away. \n\n*Note: Project directory is rsync\'ed between Host and Guest.*\n\n*Note2: provided Vagrant vm doesn\'t have port forwarding configured which means, that application won\'t be accessible on Host OS.*\n</details>\n\n<details>\n  <summary>Redis and aiohttp utilities</summary>\n  \nFor your discretion, I\'ve provided some basic utilities:\n* RedisClient `.app.utils.redis`\n* AiohttpClient `.app.utils.aiohttp_client`\n\nThey\'re initialized in `asgi.py` on FastAPI startup event handler, and are available for whole application scope without passing object instances between controllers.\n</details>\n\n<details>\n  <summary>Kubernetes deployment with HA Redis cluster</summary>\n  \nApplication stack in Kubernetes:\n![k8s_arch](https://github.com/rszamszur/fastapi-mvc-template/blob/master/assets/k8s_arch.png?raw=true)\n</details>\n\n<details>\n  <summary>Readable and documented code</summary>\n  \nThe metrics stage in CI workflow ensures important PEP rules are enforced. For additional readability and formatting checks - black is used. Every piece of generated code is documented with docstrings. Last but not least there is also extended README with how to.\n</details>\n\n<details>\n  <summary>Configurable from env</summary>\n  \nGenerated application provides flexibility of configuration. All significant settings are defined by the environment variables, each with the default value.\n</details>\n\n<details>\n  <summary>Generated project uses <a href="https://github.com/python-poetry/poetry" target="_blank">Poetry</a> dependency management</summary>\n\nPoetry comes with all the tools you might need to manage your project in a deterministic way. Moreover, it\'s based on new unified Python project settings file - <a href="https://www.python.org/dev/peps/pep-0518/" target="_blank">PEP 518</a> that replaces `setup.py`.\n</details>\n\n## Quick start\n\n```shell\npip install fastapi-mvc\nfastapi-mvc new /tmp/demo-project\ncd /tmp/demo-project\nfastapi-mvc run\n```\n\n## Prerequisites\n\n* Python 3.7 or later installed [How to install python](https://docs.python-guide.org/starting/installation/)\n* Poetry [How to install poetry](https://python-poetry.org/docs/#installation) or pip [How to install pip](https://pip.pypa.io/en/stable/installation/) installed\n* make (optional)\n\n## Installation\n\n```shell\npip install fastapi-mvc\n```\n\nOr directly from source:\n```shell\ngit clone git@github.com:rszamszur/fastapi-mvc.git\ncd fastapi-mvc\nmake install\n```\n\n## Getting started\n\nCreating a new FastAPI project is as easy as:\n```shell\nfastapi-mvc new my-project\n```\n\nTo run development uvicorn server:\n```shell\ncd my-project\nfastapi-mvc run\n```\n\nTo run production WSGI + ASGI server:\n```shell\ncd my-project\npoetry run my-project serve\n# or if project virtualenv PATH is set\nmy-project serve\n```\n\nTo confirm it\'s working:\n```shell\ncurl localhost:8000/api/ready\n{"status":"ok"}\n```\n\n## CLI\n\nThis package exposes simple CLI for easier interaction:\n\n```shell\n$ fastapi-mvc --help\nUsage: fastapi-mvc [OPTIONS] COMMAND [ARGS]...\n\n  Create and develop production grade FastAPI projects.\n\n  Documentation: https://fastapi-mvc.netlify.app\n\n  Source Code: https://github.com/rszamszur/fastapi-mvc\n\nOptions:\n  -v, --verbose  Enable verbose logging.\n  --help         Show this message and exit.\n\nCommands:\n  new  Create a new FastAPI application.\n  run  Run development uvicorn server.\n```\n```shell\n$ fastapi-mvc new --help\nUsage: fastapi-mvc new [OPTIONS] APP_PATH\n\n  Create a new FastAPI application.\n\n  The \'fastapi-mvc new\' command creates a new FastAPI application with a\n  default directory structure and configuration at the path you specify.\n\nOptions:\n  -R, --skip-redis                Skip Redis utility files.\n  -A, --skip-aiohttp              Skip aiohttp utility files.\n  -V, --skip-vagrantfile          Skip Vagrantfile.\n  -H, --skip-helm                 Skip Helm chart files.\n  -G, --skip-actions              Skip GitHub actions files.\n  -C, --skip-codecov              Skip codecov in GitHub actions.\n  -I, --skip-install              Dont run make install\n  --license [MIT|BSD2|BSD3|ISC|Apache2.0|LGPLv3+|LGPLv3|LGPLv2+|LGPLv2|no]\n                                  Choose license.  [default: MIT]\n  --repo-url TEXT                 Repository url.\n  --help                          Show this message and exit.\n```\n```shell\n$ fastapi-mvc run --help\nUsage: fastapi-mvc run [OPTIONS]\n\n  Run development uvicorn server.\n\n  The \'fastapi-mvc run\' commands runs development uvicorn server for a\n  fastapi-mvc project at the current working directory.\n\nOptions:\n  --host TEXT                  Host to bind.  [default: 127.0.0.1]\n  -p, --port INTEGER           Port to bind.  [default: 8000]\n  -w, --workers INTEGER RANGE  The number of worker processes for handling\n                               requests.  [default: 1]\n\n  --no-reload                  Disable auto-reload.\n  --help                       Show this message and exit.\n```\n\n## Contributing\n\n[CONTRIBUTING](https://github.com/rszamszur/fastapi-mvc/blob/master/CONTRIBUTING.md)\n\n## License\n\n[MIT](https://github.com/rszamszur/fastapi-mvc/blob/master/LICENSE)\n',
+    'long_description': '<div align="center">\n<h1>fastapi-mvc</h1>\n\n![fastapi-mvc](https://github.com/rszamszur/fastapi-mvc-template/blob/master/assets/readme.gif?raw=true)\n[![CI](https://github.com/rszamszur/fastapi-mvc/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/rszamszur/fastapi-mvc/actions/workflows/main.yml)\n[![codecov](https://codecov.io/gh/rszamszur/fastapi-mvc/branch/master/graph/badge.svg?token=7ESV30TYZS)](https://codecov.io/gh/rszamszur/fastapi-mvc)\n[![K8s integration](https://github.com/rszamszur/fastapi-mvc/actions/workflows/integration.yml/badge.svg)](https://github.com/rszamszur/fastapi-mvc/actions/workflows/integration.yml)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n![PyPI](https://img.shields.io/pypi/v/fastapi-mvc)\n![PyPI - Downloads](https://img.shields.io/pypi/dm/fastapi-mvc)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fastapi-mvc)\n![GitHub](https://img.shields.io/github/license/rszamszur/fastapi-mvc?color=blue)\n\n</div>\n\n---\n\n**Documentation**: [https://fastapi-mvc.netlify.app](https://fastapi-mvc.netlify.app)\n\n**Source Code**: [https://github.com/rszamszur/fastapi-mvc](https://github.com/rszamszur/fastapi-mvc)\n\n**Example generated project**: https://github.com/rszamszur/fastapi-mvc-example\n\n---\n\n## Features\n<details>\n  <summary>Generated project core implemented using MVC architectural pattern</summary>\n  \n  Generated project is structured in MVC architectural pattern to help developers who don\'t know FastAPI yet but are familiar with MVC to get up to speed quickly.\n</details>\n\n<details>\n  <summary>WSGI + ASGI for high performance and better configuration</summary>\n\n#### TLDR;\n\nRunning WSGI as a master worker with ASGI workers gives better results than running pure ASGI (for FastAPI for now):\n* better performance (requests per second)\n* better support for different protocols\n* broader configuration\n* better support with using reverse proxy\n---\nFirst of all, whether it\'s ASGI, WSGI, or combined, think of this as something that serves the application. For instance, Ruby on Rails uses Puma. The result of any of those servers is a TCP/IP or UNIX socket which is later on utilized by reverse proxy ex: Nginx (a TCP/IP socket you can access directly over the network, but still in production, usually it\'ll be behind a reverse proxy).\n\nNow to WSGI + ASGI part. FastAPI is implemented with asyncio (https://docs.python.org/3/library/asyncio.html), so having a pure WSGI server doesn\'t make sense since you\'d lose all the benefits of asynchronous concurrency. That\'s where ASGI comes in. However, Python journey with asyncio is still pretty young. Most projects have yet to reach maturity level (you should expect early bugs and a limited feature set). FastAPI, as ASGI server uses uvicorn, which is still prior 1.x.x release (17 in total so far, current 0.16.0) and lacks support for some protocols (ex: no HTTP/2).\nMoreover, some reverse proxy might not know how to work with asynchronous servers, and some problems or early bugs on this layer might happen as well.\n\nI\'m not saying uvicorn is bad. Quite contrary, if you\'d run 4 pure uvicorn workes, you\'d still get great results. But if you\'d run the same amount of workers with gunicorn (WSGI) as a master worker, it turns out you can even pump those numbers up.\n\nGunicorn with 4 Uvicorn Workers (source: https://stackoverflow.com/a/62977786/10566747):\n```\nRequests per second: 7891.28 [#/sec] (mean)\nTime per request: 126.722 [ms] (mean)\nTime per request: 0.127 [ms] (mean, across all concurrent requests)\n```\n\nPure Uvicorn with 4 workers:\n```\nRequests per second: 4359.68 [#/sec] (mean)\nTime per request: 229.375 [ms] (mean)\nTime per request: 0.229 [ms] (mean, across all concurrent requests)\n```\n\n~80% better\n\nI guess gunicorn does a better job in worker management. However, it\'s a more mature project, so it\'s probably a matter of time when uvicorn (or other ASGI for that matter) will catch up to this benchmark.\n\nLast but not least, gunicorn gives a ton of settings to configure (https://docs.gunicorn.org/en/stable/settings.html), which can come in handy.\n</details>\n\n<details>\n  <summary>Generated project comes with tests at 99% coverage</summary>\n  \n  Unit test coverage is at 99% regardless of chosen configuration. There is also a placeholder for integration tests with an example dummy test.\n</details>\n\n<details>\n  <summary>Proper Dockerfile created with best practices for the cloud and Kubernetes</summary>\n  \nContainer image features:\n* Based on distroless image\n* Run as PID 1 (with child processes)\n* Utilizes multi-stage build for smallest size possible, also this results in having only necessary libraries/dependencies/tools in outcome container image.\n* DigestSHA - immutable identifier instead of tags, for better reproducibility and security.\n* Signal handling, for Kubernetes to be able to gracefully shut down pods.\n* Created with common layers.\n* By default runs as non-root user\n\nBased on Google [Best practices for building containers](https://cloud.google.com/architecture/best-practices-for-building-containers), [Top 20 Dockerfile best practices](https://sysdig.com/blog/dockerfile-best-practices), and own experience.\n</details>\n\n<details>\n  <summary>Extensive GitHub actions for CI</summary>\n  \n![ci_example](https://github.com/rszamszur/fastapi-mvc-template/blob/master/assets/ci.png?raw=true)\n</details>\n\n<details>\n  <summary>Helm chart for Kubernetes</summary>\n  \nFor easily deploying application in Kubernetes cluster.\n</details>\n\n<details>\n  <summary>Reproducible virtualized development environment</summary>\n\nEasily boot virtual machine with Vagrant. Code and test straight away. \n\n*Note: Project directory is rsync\'ed between Host and Guest.*\n\n*Note2: provided Vagrant vm doesn\'t have port forwarding configured which means, that application won\'t be accessible on Host OS.*\n</details>\n\n<details>\n  <summary>Redis and aiohttp utilities</summary>\n  \nFor your discretion, I\'ve provided some basic utilities:\n* RedisClient `.app.utils.redis`\n* AiohttpClient `.app.utils.aiohttp_client`\n\nThey\'re initialized in `asgi.py` on FastAPI startup event handler, and are available for whole application scope without passing object instances between controllers.\n</details>\n\n<details>\n  <summary>Kubernetes deployment with HA Redis cluster</summary>\n  \nApplication stack in Kubernetes:\n![k8s_arch](https://github.com/rszamszur/fastapi-mvc-template/blob/master/assets/k8s_arch.png?raw=true)\n</details>\n\n<details>\n  <summary>Readable and documented code</summary>\n  \nThe metrics stage in CI workflow ensures important PEP rules are enforced. For additional readability and formatting checks - black is used. Every piece of generated code is documented with docstrings. Last but not least there is also extended README with how to.\n</details>\n\n<details>\n  <summary>Configurable from env</summary>\n  \nGenerated application provides flexibility of configuration. All significant settings are defined by the environment variables, each with the default value.\n</details>\n\n<details>\n  <summary>Generated project uses <a href="https://github.com/python-poetry/poetry" target="_blank">Poetry</a> dependency management</summary>\n\nPoetry comes with all the tools you might need to manage your project in a deterministic way. Moreover, it\'s based on new unified Python project settings file - <a href="https://www.python.org/dev/peps/pep-0518/" target="_blank">PEP 518</a> that replaces `setup.py`.\n</details>\n\n## Quick start\n\n```shell\npip install fastapi-mvc\nfastapi-mvc new /tmp/demo-project\ncd /tmp/demo-project\nfastapi-mvc run\n```\n\n## Prerequisites\n\n* Python 3.7 or later installed [How to install python](https://docs.python-guide.org/starting/installation/)\n* Poetry [How to install poetry](https://python-poetry.org/docs/#installation) or pip [How to install pip](https://pip.pypa.io/en/stable/installation/) installed\n* make (optional)\n\n## Installation\n\n```shell\npip install fastapi-mvc\n```\n\nOr directly from source:\n```shell\ngit clone git@github.com:rszamszur/fastapi-mvc.git\ncd fastapi-mvc\nmake install\n```\n\n## Getting started\n\nCreating a new FastAPI project is as easy as:\n```shell\nfastapi-mvc new my-project\n```\n\nTo run development uvicorn server:\n```shell\ncd my-project\nfastapi-mvc run\n```\n\nTo run production WSGI + ASGI server:\n```shell\ncd my-project\npoetry run my-project serve\n# or if project virtualenv PATH is set\nmy-project serve\n```\n\nTo confirm it\'s working:\n```shell\ncurl localhost:8000/api/ready\n{"status":"ok"}\n```\n\n## CLI\n\nThis package exposes simple CLI for easier interaction:\n\n```shell\n$ fastapi-mvc --help\nUsage: fastapi-mvc [OPTIONS] COMMAND [ARGS]...\n\n  Create and develop production grade FastAPI projects.\n\n  Documentation: https://fastapi-mvc.netlify.app\n\n  Source Code: https://github.com/rszamszur/fastapi-mvc\n\nOptions:\n  -v, --verbose  Enable verbose logging.\n  --help         Show this message and exit.\n\nCommands:\n  new  Create a new FastAPI application.\n  run  Run development uvicorn server.\n```\n```shell\n$ fastapi-mvc new --help\nUsage: fastapi-mvc new [OPTIONS] APP_PATH\n\n  Create a new FastAPI application.\n\n  The \'fastapi-mvc new\' command creates a new FastAPI application with a\n  default directory structure and configuration at the path you specify.\n\nOptions:\n  -R, --skip-redis                Skip Redis utility files.\n  -A, --skip-aiohttp              Skip aiohttp utility files.\n  -V, --skip-vagrantfile          Skip Vagrantfile.\n  -H, --skip-helm                 Skip Helm chart files.\n  -G, --skip-actions              Skip GitHub actions files.\n  -C, --skip-codecov              Skip codecov in GitHub actions.\n  -I, --skip-install              Dont run make install\n  --license [MIT|BSD2|BSD3|ISC|Apache2.0|LGPLv3+|LGPLv3|LGPLv2+|LGPLv2|no]\n                                  Choose license.  [default: MIT]\n  --repo-url TEXT                 Repository url.\n  --help                          Show this message and exit.\n```\n```shell\n$ fastapi-mvc run --help\nUsage: fastapi-mvc run [OPTIONS]\n\n  Run development uvicorn server.\n\n  The \'fastapi-mvc run\' commands runs development uvicorn server for a\n  fastapi-mvc project at the current working directory.\n\nOptions:\n  --host TEXT      Host to bind.  [default: 127.0.0.1]\n  -p, --port TEXT  Port to bind.  [default: 8000]\n  --help           Show this message and exit.\n```\n\n## Contributing\n\n[CONTRIBUTING](https://github.com/rszamszur/fastapi-mvc/blob/master/CONTRIBUTING.md)\n\n## License\n\n[MIT](https://github.com/rszamszur/fastapi-mvc/blob/master/LICENSE)\n',
     'author': 'Radosław Szamszur',
     'author_email': 'radoslawszamszur@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/rszamszur/fastapi-mvc',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `fastapi-mvc-0.8.0/PKG-INFO` & `fastapi-mvc-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mvc
-Version: 0.8.0
+Version: 0.9.0
 Summary: Create and develop production grade FastAPI projects.
 Home-page: https://github.com/rszamszur/fastapi-mvc
 License: MIT
 Author: Radosław Szamszur
 Author-email: radoslawszamszur@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -21,15 +21,14 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click (>=7.1.2,<7.2.0)
 Requires-Dist: cookiecutter (>=1.7.3,<1.8.0)
-Requires-Dist: uvicorn[standard] (>=0.17.4,<0.18.0)
 Project-URL: Documentation, https://fastapi-mvc.netlify.app
 Project-URL: Issues, https://github.com/rszamszur/fastapi-mvc/issues
 Project-URL: Repository, https://github.com/rszamszur/fastapi-mvc
 Description-Content-Type: text/markdown
 
 <div align="center">
 <h1>fastapi-mvc</h1>
@@ -285,21 +284,17 @@
 
   Run development uvicorn server.
 
   The 'fastapi-mvc run' commands runs development uvicorn server for a
   fastapi-mvc project at the current working directory.
 
 Options:
-  --host TEXT                  Host to bind.  [default: 127.0.0.1]
-  -p, --port INTEGER           Port to bind.  [default: 8000]
-  -w, --workers INTEGER RANGE  The number of worker processes for handling
-                               requests.  [default: 1]
-
-  --no-reload                  Disable auto-reload.
-  --help                       Show this message and exit.
+  --host TEXT      Host to bind.  [default: 127.0.0.1]
+  -p, --port TEXT  Port to bind.  [default: 8000]
+  --help           Show this message and exit.
 ```
 
 ## Contributing
 
 [CONTRIBUTING](https://github.com/rszamszur/fastapi-mvc/blob/master/CONTRIBUTING.md)
 
 ## License
```

