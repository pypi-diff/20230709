# Comparing `tmp/kui-1.5.2.tar.gz` & `tmp/kui-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kui-1.5.2.tar", last modified: Tue Jul  4 18:05:27 2023, max compression
+gzip compressed data, was "kui-1.5.3.tar", last modified: Sun Jul  9 13:45:46 2023, max compression
```

## Comparing `kui-1.5.2.tar` & `kui-1.5.3.tar`

### file list

```diff
@@ -1,88 +1,90 @@
--rw-r--r--   0        0        0    11341 2023-07-04 18:05:10.249385 kui-1.5.2/LICENSE
--rw-r--r--   0        0        0      440 2023-07-04 18:05:10.249385 kui-1.5.2/README.md
--rw-r--r--   0        0        0        0 2023-07-04 18:05:10.249385 kui-1.5.2/kui/__init__.py
--rw-r--r--   0        0        0       63 2023-07-04 18:05:10.249385 kui-1.5.2/kui/__version__.py
--rw-r--r--   0        0        0     1718 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/__init__.py
--rw-r--r--   0        0        0     6977 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/applications.py
--rw-r--r--   0        0        0     2054 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/cors.py
--rw-r--r--   0        0        0     2382 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/exceptions.py
--rw-r--r--   0        0        0     2439 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/lifespan.py
--rw-r--r--   0        0        0     1470 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/openapi.py
--rw-r--r--   0        0        0     5261 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/parameters.py
--rw-r--r--   0        0        0     3756 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/requests.py
--rw-r--r--   0        0        0     2879 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/responses.py
--rw-r--r--   0        0        0      972 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/routing.py
--rw-r--r--   0        0        0     3177 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/templates.py
--rw-r--r--   0        0        0     4532 2023-07-04 18:05:10.249385 kui-1.5.2/kui/asgi/views.py
--rw-r--r--   0        0        0      304 2023-07-04 18:05:10.249385 kui-1.5.2/kui/cors.py
--rw-r--r--   0        0        0     3794 2023-07-04 18:05:10.249385 kui-1.5.2/kui/exceptions.py
--rw-r--r--   0        0        0      123 2023-07-04 18:05:10.249385 kui-1.5.2/kui/openapi/__init__.py
--rw-r--r--   0        0        0     9382 2023-07-04 18:05:10.249385 kui-1.5.2/kui/openapi/application.py
--rw-r--r--   0        0        0     1565 2023-07-04 18:05:10.249385 kui-1.5.2/kui/openapi/extra_docs.py
--rw-r--r--   0        0        0     1644 2023-07-04 18:05:10.249385 kui-1.5.2/kui/openapi/schema.py
--rw-r--r--   0        0        0     7726 2023-07-04 18:05:10.249385 kui-1.5.2/kui/openapi/specification.py
--rw-r--r--   0        0        0      224 2023-07-04 18:05:10.249385 kui-1.5.2/kui/openapi/templates/rapidoc.html
--rw-r--r--   0        0        0      743 2023-07-04 18:05:10.253385 kui-1.5.2/kui/openapi/templates/redoc.html
--rw-r--r--   0        0        0     1522 2023-07-04 18:05:10.253385 kui-1.5.2/kui/openapi/templates/swagger.html
--rw-r--r--   0        0        0     1284 2023-07-04 18:05:10.253385 kui-1.5.2/kui/openapi/types.py
--rw-r--r--   0        0        0    14614 2023-07-04 18:05:10.253385 kui-1.5.2/kui/parameters/__init__.py
--rw-r--r--   0        0        0     6803 2023-07-04 18:05:10.253385 kui-1.5.2/kui/parameters/field_functions.py
--rw-r--r--   0        0        0      960 2023-07-04 18:05:10.253385 kui-1.5.2/kui/parameters/fields.py
--rw-r--r--   0        0        0        0 2023-07-04 18:05:10.253385 kui-1.5.2/kui/py.typed
--rw-r--r--   0        0        0     7408 2023-07-04 18:05:10.253385 kui-1.5.2/kui/responses.py
--rw-r--r--   0        0        0      429 2023-07-04 18:05:10.253385 kui-1.5.2/kui/routing/__init__.py
--rw-r--r--   0        0        0       82 2023-07-04 18:05:10.253385 kui-1.5.2/kui/routing/__main__.py
--rw-r--r--   0        0        0     1402 2023-07-04 18:05:10.253385 kui-1.5.2/kui/routing/commands.py
--rw-r--r--   0        0        0      130 2023-07-04 18:05:10.253385 kui-1.5.2/kui/routing/extensions/__init__.py
--rw-r--r--   0        0        0     2551 2023-07-04 18:05:10.253385 kui-1.5.2/kui/routing/extensions/file.py
--rw-r--r--   0        0        0     3025 2023-07-04 18:05:10.253385 kui-1.5.2/kui/routing/extensions/multimethod.py
--rw-r--r--   0        0        0    17890 2023-07-04 18:05:10.253385 kui-1.5.2/kui/routing/routers.py
--rw-r--r--   0        0        0     3368 2023-07-04 18:05:10.253385 kui-1.5.2/kui/routing/routes.py
--rw-r--r--   0        0        0     6234 2023-07-04 18:05:10.253385 kui-1.5.2/kui/routing/tree.py
--rw-r--r--   0        0        0      385 2023-07-04 18:05:10.253385 kui-1.5.2/kui/routing/typing.py
--rw-r--r--   0        0        0     4073 2023-07-04 18:05:10.253385 kui-1.5.2/kui/security.py
--rw-r--r--   0        0        0     2783 2023-07-04 18:05:10.253385 kui-1.5.2/kui/status.py
--rw-r--r--   0        0        0     1250 2023-07-04 18:05:10.253385 kui-1.5.2/kui/templates.py
--rw-r--r--   0        0        0      757 2023-07-04 18:05:10.253385 kui-1.5.2/kui/utils/__init__.py
--rw-r--r--   0        0        0      856 2023-07-04 18:05:10.253385 kui-1.5.2/kui/utils/contextvars.py
--rw-r--r--   0        0        0     1576 2023-07-04 18:05:10.253385 kui-1.5.2/kui/utils/importer.py
--rw-r--r--   0        0        0     1907 2023-07-04 18:05:10.253385 kui-1.5.2/kui/utils/inspect.py
--rw-r--r--   0        0        0     1647 2023-07-04 18:05:10.253385 kui-1.5.2/kui/utils/objects.py
--rw-r--r--   0        0        0      530 2023-07-04 18:05:10.253385 kui-1.5.2/kui/utils/pipe.py
--rw-r--r--   0        0        0     1139 2023-07-04 18:05:10.253385 kui-1.5.2/kui/utils/state.py
--rw-r--r--   0        0        0     1567 2023-07-04 18:05:10.253385 kui-1.5.2/kui/wsgi/__init__.py
--rw-r--r--   0        0        0     5515 2023-07-04 18:05:10.253385 kui-1.5.2/kui/wsgi/applications.py
--rw-r--r--   0        0        0     2031 2023-07-04 18:05:10.253385 kui-1.5.2/kui/wsgi/cors.py
--rw-r--r--   0        0        0     2325 2023-07-04 18:05:10.253385 kui-1.5.2/kui/wsgi/exceptions.py
--rw-r--r--   0        0        0     1428 2023-07-04 18:05:10.253385 kui-1.5.2/kui/wsgi/openapi.py
--rw-r--r--   0        0        0     3963 2023-07-04 18:05:10.253385 kui-1.5.2/kui/wsgi/parameters.py
--rw-r--r--   0        0        0     1835 2023-07-04 18:05:10.253385 kui-1.5.2/kui/wsgi/requests.py
--rw-r--r--   0        0        0     2879 2023-07-04 18:05:10.253385 kui-1.5.2/kui/wsgi/responses.py
--rw-r--r--   0        0        0      966 2023-07-04 18:05:10.253385 kui-1.5.2/kui/wsgi/routing.py
--rw-r--r--   0        0        0     2884 2023-07-04 18:05:10.253385 kui-1.5.2/kui/wsgi/templates.py
--rw-r--r--   0        0        0     2229 2023-07-04 18:05:10.253385 kui-1.5.2/kui/wsgi/views.py
--rw-r--r--   0        0        0     1959 2023-07-04 18:05:10.253385 kui-1.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 18:05:10.253385 kui-1.5.2/tests/asgi/__init__.py
--rw-r--r--   0        0        0     2416 2023-07-04 18:05:10.253385 kui-1.5.2/tests/asgi/test_application.py
--rw-r--r--   0        0        0     1338 2023-07-04 18:05:10.253385 kui-1.5.2/tests/asgi/test_cors.py
--rw-r--r--   0        0        0      506 2023-07-04 18:05:10.253385 kui-1.5.2/tests/asgi/test_lifespan.py
--rw-r--r--   0        0        0     5841 2023-07-04 18:05:10.253385 kui-1.5.2/tests/asgi/test_parameters.py
--rw-r--r--   0        0        0      535 2023-07-04 18:05:10.253385 kui-1.5.2/tests/asgi/test_views.py
--rw-r--r--   0        0        0    35100 2023-07-04 18:05:10.253385 kui-1.5.2/tests/openapi/test_application.py
--rw-r--r--   0        0        0      429 2023-07-04 18:05:10.253385 kui-1.5.2/tests/openapi/test_extra_docs.py
--rw-r--r--   0        0        0      247 2023-07-04 18:05:10.253385 kui-1.5.2/tests/routing/extensions/test_fileroutes.py
--rw-r--r--   0        0        0     3363 2023-07-04 18:05:10.253385 kui-1.5.2/tests/routing/extensions/test_multimethod.py
--rw-r--r--   0        0        0       88 2023-07-04 18:05:10.253385 kui-1.5.2/tests/routing/test_commands.py
--rw-r--r--   0        0        0     4558 2023-07-04 18:05:10.253385 kui-1.5.2/tests/routing/test_routes.py
--rw-r--r--   0        0        0     2444 2023-07-04 18:05:10.253385 kui-1.5.2/tests/routing/test_tree.py
--rw-r--r--   0        0        0      242 2023-07-04 18:05:10.253385 kui-1.5.2/tests/test_export_all.py
--rw-r--r--   0        0        0     4505 2023-07-04 18:05:10.253385 kui-1.5.2/tests/test_responses.py
--rw-r--r--   0        0        0     3032 2023-07-04 18:05:10.253385 kui-1.5.2/tests/test_security.py
--rw-r--r--   0        0        0        0 2023-07-04 18:05:10.253385 kui-1.5.2/tests/utils/__init__.py
--rw-r--r--   0        0        0      722 2023-07-04 18:05:10.253385 kui-1.5.2/tests/utils/test_importer.py
--rw-r--r--   0        0        0      170 2023-07-04 18:05:10.253385 kui-1.5.2/tests/utils/test_objects.py
--rw-r--r--   0        0        0      426 2023-07-04 18:05:10.253385 kui-1.5.2/tests/utils/test_state.py
--rw-r--r--   0        0        0     1290 2023-07-04 18:05:10.253385 kui-1.5.2/tests/wsgi/test_cors.py
--rw-r--r--   0        0        0     5610 2023-07-04 18:05:10.253385 kui-1.5.2/tests/wsgi/test_parameters.py
--rw-r--r--   0        0        0      453 2023-07-04 18:05:10.253385 kui-1.5.2/tests/wsgi/test_views.py
--rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 kui-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-09 13:45:26.276603 kui-1.5.3/LICENSE
+-rw-r--r--   0        0        0      440 2023-07-09 13:45:26.276603 kui-1.5.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 13:45:26.280604 kui-1.5.3/kui/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-09 13:45:26.280604 kui-1.5.3/kui/__version__.py
+-rw-r--r--   0        0        0     1718 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/__init__.py
+-rw-r--r--   0        0        0     7065 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/applications.py
+-rw-r--r--   0        0        0     2054 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/cors.py
+-rw-r--r--   0        0        0     2382 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/exceptions.py
+-rw-r--r--   0        0        0     2439 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/lifespan.py
+-rw-r--r--   0        0        0     1470 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/openapi.py
+-rw-r--r--   0        0        0     5261 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/parameters.py
+-rw-r--r--   0        0        0     3756 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/requests.py
+-rw-r--r--   0        0        0     2879 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/responses.py
+-rw-r--r--   0        0        0      972 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/routing.py
+-rw-r--r--   0        0        0     3177 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/templates.py
+-rw-r--r--   0        0        0     4532 2023-07-09 13:45:26.280604 kui-1.5.3/kui/asgi/views.py
+-rw-r--r--   0        0        0      304 2023-07-09 13:45:26.280604 kui-1.5.3/kui/cors.py
+-rw-r--r--   0        0        0     3794 2023-07-09 13:45:26.280604 kui-1.5.3/kui/exceptions.py
+-rw-r--r--   0        0        0      123 2023-07-09 13:45:26.280604 kui-1.5.3/kui/openapi/__init__.py
+-rw-r--r--   0        0        0     9382 2023-07-09 13:45:26.280604 kui-1.5.3/kui/openapi/application.py
+-rw-r--r--   0        0        0     1565 2023-07-09 13:45:26.280604 kui-1.5.3/kui/openapi/extra_docs.py
+-rw-r--r--   0        0        0     1644 2023-07-09 13:45:26.280604 kui-1.5.3/kui/openapi/schema.py
+-rw-r--r--   0        0        0     7726 2023-07-09 13:45:26.280604 kui-1.5.3/kui/openapi/specification.py
+-rw-r--r--   0        0        0      224 2023-07-09 13:45:26.280604 kui-1.5.3/kui/openapi/templates/rapidoc.html
+-rw-r--r--   0        0        0      743 2023-07-09 13:45:26.280604 kui-1.5.3/kui/openapi/templates/redoc.html
+-rw-r--r--   0        0        0     1522 2023-07-09 13:45:26.280604 kui-1.5.3/kui/openapi/templates/swagger.html
+-rw-r--r--   0        0        0     1284 2023-07-09 13:45:26.280604 kui-1.5.3/kui/openapi/types.py
+-rw-r--r--   0        0        0    14614 2023-07-09 13:45:26.280604 kui-1.5.3/kui/parameters/__init__.py
+-rw-r--r--   0        0        0     6803 2023-07-09 13:45:26.280604 kui-1.5.3/kui/parameters/field_functions.py
+-rw-r--r--   0        0        0      960 2023-07-09 13:45:26.280604 kui-1.5.3/kui/parameters/fields.py
+-rw-r--r--   0        0        0        0 2023-07-09 13:45:26.280604 kui-1.5.3/kui/py.typed
+-rw-r--r--   0        0        0     7408 2023-07-09 13:45:26.280604 kui-1.5.3/kui/responses.py
+-rw-r--r--   0        0        0      429 2023-07-09 13:45:26.280604 kui-1.5.3/kui/routing/__init__.py
+-rw-r--r--   0        0        0       82 2023-07-09 13:45:26.280604 kui-1.5.3/kui/routing/__main__.py
+-rw-r--r--   0        0        0     1402 2023-07-09 13:45:26.280604 kui-1.5.3/kui/routing/commands.py
+-rw-r--r--   0        0        0      130 2023-07-09 13:45:26.280604 kui-1.5.3/kui/routing/extensions/__init__.py
+-rw-r--r--   0        0        0     2551 2023-07-09 13:45:26.280604 kui-1.5.3/kui/routing/extensions/file.py
+-rw-r--r--   0        0        0     3025 2023-07-09 13:45:26.280604 kui-1.5.3/kui/routing/extensions/multimethod.py
+-rw-r--r--   0        0        0    17890 2023-07-09 13:45:26.280604 kui-1.5.3/kui/routing/routers.py
+-rw-r--r--   0        0        0     3368 2023-07-09 13:45:26.280604 kui-1.5.3/kui/routing/routes.py
+-rw-r--r--   0        0        0     6234 2023-07-09 13:45:26.280604 kui-1.5.3/kui/routing/tree.py
+-rw-r--r--   0        0        0      385 2023-07-09 13:45:26.280604 kui-1.5.3/kui/routing/typing.py
+-rw-r--r--   0        0        0     4073 2023-07-09 13:45:26.280604 kui-1.5.3/kui/security.py
+-rw-r--r--   0        0        0     2783 2023-07-09 13:45:26.280604 kui-1.5.3/kui/status.py
+-rw-r--r--   0        0        0     1250 2023-07-09 13:45:26.280604 kui-1.5.3/kui/templates.py
+-rw-r--r--   0        0        0      757 2023-07-09 13:45:26.280604 kui-1.5.3/kui/utils/__init__.py
+-rw-r--r--   0        0        0      856 2023-07-09 13:45:26.280604 kui-1.5.3/kui/utils/contextvars.py
+-rw-r--r--   0        0        0     1576 2023-07-09 13:45:26.280604 kui-1.5.3/kui/utils/importer.py
+-rw-r--r--   0        0        0     1907 2023-07-09 13:45:26.280604 kui-1.5.3/kui/utils/inspect.py
+-rw-r--r--   0        0        0     1647 2023-07-09 13:45:26.280604 kui-1.5.3/kui/utils/objects.py
+-rw-r--r--   0        0        0      530 2023-07-09 13:45:26.280604 kui-1.5.3/kui/utils/pipe.py
+-rw-r--r--   0        0        0     1139 2023-07-09 13:45:26.280604 kui-1.5.3/kui/utils/state.py
+-rw-r--r--   0        0        0     1567 2023-07-09 13:45:26.280604 kui-1.5.3/kui/wsgi/__init__.py
+-rw-r--r--   0        0        0     5603 2023-07-09 13:45:26.280604 kui-1.5.3/kui/wsgi/applications.py
+-rw-r--r--   0        0        0     2031 2023-07-09 13:45:26.280604 kui-1.5.3/kui/wsgi/cors.py
+-rw-r--r--   0        0        0     2325 2023-07-09 13:45:26.280604 kui-1.5.3/kui/wsgi/exceptions.py
+-rw-r--r--   0        0        0     1428 2023-07-09 13:45:26.280604 kui-1.5.3/kui/wsgi/openapi.py
+-rw-r--r--   0        0        0     3963 2023-07-09 13:45:26.280604 kui-1.5.3/kui/wsgi/parameters.py
+-rw-r--r--   0        0        0     1835 2023-07-09 13:45:26.280604 kui-1.5.3/kui/wsgi/requests.py
+-rw-r--r--   0        0        0     2879 2023-07-09 13:45:26.280604 kui-1.5.3/kui/wsgi/responses.py
+-rw-r--r--   0        0        0      966 2023-07-09 13:45:26.280604 kui-1.5.3/kui/wsgi/routing.py
+-rw-r--r--   0        0        0     2884 2023-07-09 13:45:26.280604 kui-1.5.3/kui/wsgi/templates.py
+-rw-r--r--   0        0        0     2229 2023-07-09 13:45:26.280604 kui-1.5.3/kui/wsgi/views.py
+-rw-r--r--   0        0        0     1959 2023-07-09 13:45:26.280604 kui-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-09 13:45:26.280604 kui-1.5.3/tests/asgi/__init__.py
+-rw-r--r--   0        0        0     2416 2023-07-09 13:45:26.284604 kui-1.5.3/tests/asgi/test_application.py
+-rw-r--r--   0        0        0     1338 2023-07-09 13:45:26.284604 kui-1.5.3/tests/asgi/test_cors.py
+-rw-r--r--   0        0        0      506 2023-07-09 13:45:26.284604 kui-1.5.3/tests/asgi/test_lifespan.py
+-rw-r--r--   0        0        0     5841 2023-07-09 13:45:26.284604 kui-1.5.3/tests/asgi/test_parameters.py
+-rw-r--r--   0        0        0      524 2023-07-09 13:45:26.284604 kui-1.5.3/tests/asgi/test_response_convertors.py
+-rw-r--r--   0        0        0      535 2023-07-09 13:45:26.284604 kui-1.5.3/tests/asgi/test_views.py
+-rw-r--r--   0        0        0    35100 2023-07-09 13:45:26.284604 kui-1.5.3/tests/openapi/test_application.py
+-rw-r--r--   0        0        0      429 2023-07-09 13:45:26.284604 kui-1.5.3/tests/openapi/test_extra_docs.py
+-rw-r--r--   0        0        0      247 2023-07-09 13:45:26.284604 kui-1.5.3/tests/routing/extensions/test_fileroutes.py
+-rw-r--r--   0        0        0     3363 2023-07-09 13:45:26.284604 kui-1.5.3/tests/routing/extensions/test_multimethod.py
+-rw-r--r--   0        0        0       88 2023-07-09 13:45:26.284604 kui-1.5.3/tests/routing/test_commands.py
+-rw-r--r--   0        0        0     4558 2023-07-09 13:45:26.284604 kui-1.5.3/tests/routing/test_routes.py
+-rw-r--r--   0        0        0     2444 2023-07-09 13:45:26.284604 kui-1.5.3/tests/routing/test_tree.py
+-rw-r--r--   0        0        0      242 2023-07-09 13:45:26.284604 kui-1.5.3/tests/test_export_all.py
+-rw-r--r--   0        0        0     4505 2023-07-09 13:45:26.284604 kui-1.5.3/tests/test_responses.py
+-rw-r--r--   0        0        0     3032 2023-07-09 13:45:26.284604 kui-1.5.3/tests/test_security.py
+-rw-r--r--   0        0        0        0 2023-07-09 13:45:26.284604 kui-1.5.3/tests/utils/__init__.py
+-rw-r--r--   0        0        0      722 2023-07-09 13:45:26.284604 kui-1.5.3/tests/utils/test_importer.py
+-rw-r--r--   0        0        0      170 2023-07-09 13:45:26.284604 kui-1.5.3/tests/utils/test_objects.py
+-rw-r--r--   0        0        0      426 2023-07-09 13:45:26.284604 kui-1.5.3/tests/utils/test_state.py
+-rw-r--r--   0        0        0     1290 2023-07-09 13:45:26.284604 kui-1.5.3/tests/wsgi/test_cors.py
+-rw-r--r--   0        0        0     5610 2023-07-09 13:45:26.284604 kui-1.5.3/tests/wsgi/test_parameters.py
+-rw-r--r--   0        0        0      480 2023-07-09 13:45:26.284604 kui-1.5.3/tests/wsgi/test_response_convertors.py
+-rw-r--r--   0        0        0      453 2023-07-09 13:45:26.284604 kui-1.5.3/tests/wsgi/test_views.py
+-rw-r--r--   0        0        0     1032 1970-01-01 00:00:00.000000 kui-1.5.3/PKG-INFO
```

### Comparing `kui-1.5.2/LICENSE` & `kui-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/asgi/__init__.py` & `kui-1.5.3/kui/asgi/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/asgi/applications.py` & `kui-1.5.3/kui/asgi/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Optional,
     Type,
     TypeVar,
 )
 
 from baize.datastructures import URL
 from baize.typing import Receive, Scope, Send
+from pydantic import BaseModel
 from typing_extensions import Literal
 
 from ..cors import CORSConfig
 from ..routing import AsyncViewType, BaseRoute, MiddlewareType, NoMatchFound
 from ..utils import ImmutableAttribute, State
 from .cors import allow_cors
 from .exceptions import ErrorHandlerType, ExceptionMiddleware, HTTPException
@@ -188,12 +189,13 @@
     response_converter.register(
         PurePath,
         lambda filepath, download_name=None: FileResponse(
             str(filepath), download_name=download_name
         ),
     )
     response_converter.register(URL, RedirectResponse)
+    response_converter.register(BaseModel, JSONResponse)
 
     for type_, converter in converters.items():
         response_converter.register(type_, converter)
 
     return response_converter
```

### Comparing `kui-1.5.2/kui/asgi/cors.py` & `kui-1.5.3/kui/asgi/cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/asgi/exceptions.py` & `kui-1.5.3/kui/asgi/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/asgi/lifespan.py` & `kui-1.5.3/kui/asgi/lifespan.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/asgi/openapi.py` & `kui-1.5.3/kui/asgi/openapi.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/asgi/parameters.py` & `kui-1.5.3/kui/asgi/parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/asgi/requests.py` & `kui-1.5.3/kui/asgi/requests.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/asgi/responses.py` & `kui-1.5.3/kui/asgi/responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/asgi/routing.py` & `kui-1.5.3/kui/asgi/routing.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/asgi/templates.py` & `kui-1.5.3/kui/asgi/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/asgi/views.py` & `kui-1.5.3/kui/asgi/views.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/exceptions.py` & `kui-1.5.3/kui/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/openapi/application.py` & `kui-1.5.3/kui/openapi/application.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/openapi/extra_docs.py` & `kui-1.5.3/kui/openapi/extra_docs.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/openapi/schema.py` & `kui-1.5.3/kui/openapi/schema.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/openapi/specification.py` & `kui-1.5.3/kui/openapi/specification.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/openapi/templates/redoc.html` & `kui-1.5.3/kui/openapi/templates/redoc.html`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/openapi/templates/swagger.html` & `kui-1.5.3/kui/openapi/templates/swagger.html`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/openapi/types.py` & `kui-1.5.3/kui/openapi/types.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/parameters/__init__.py` & `kui-1.5.3/kui/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/parameters/field_functions.py` & `kui-1.5.3/kui/parameters/field_functions.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/parameters/fields.py` & `kui-1.5.3/kui/parameters/fields.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/responses.py` & `kui-1.5.3/kui/responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/routing/commands.py` & `kui-1.5.3/kui/routing/commands.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/routing/extensions/file.py` & `kui-1.5.3/kui/routing/extensions/file.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/routing/extensions/multimethod.py` & `kui-1.5.3/kui/routing/extensions/multimethod.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/routing/routers.py` & `kui-1.5.3/kui/routing/routers.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/routing/routes.py` & `kui-1.5.3/kui/routing/routes.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/routing/tree.py` & `kui-1.5.3/kui/routing/tree.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/security.py` & `kui-1.5.3/kui/security.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/status.py` & `kui-1.5.3/kui/status.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/templates.py` & `kui-1.5.3/kui/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/utils/__init__.py` & `kui-1.5.3/kui/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/utils/contextvars.py` & `kui-1.5.3/kui/utils/contextvars.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/utils/importer.py` & `kui-1.5.3/kui/utils/importer.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/utils/inspect.py` & `kui-1.5.3/kui/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/utils/objects.py` & `kui-1.5.3/kui/utils/objects.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/utils/pipe.py` & `kui-1.5.3/kui/utils/pipe.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/utils/state.py` & `kui-1.5.3/kui/utils/state.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/wsgi/__init__.py` & `kui-1.5.3/kui/wsgi/__init__.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/wsgi/applications.py` & `kui-1.5.3/kui/wsgi/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import functools
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Iterable, List, Mapping, NoReturn, Optional, Type
 
 from baize.datastructures import URL
 from baize.typing import Environ, StartResponse
+from pydantic import BaseModel
 
 from ..cors import CORSConfig
 from ..routing import BaseRoute, MiddlewareType, NoMatchFound, SyncViewType
 from ..utils import ImmutableAttribute, State
 from .cors import allow_cors
 from .exceptions import ErrorHandlerType, ExceptionMiddleware, HTTPException
 from .requests import HttpRequest, request_var
@@ -147,12 +148,13 @@
     response_converter.register(
         PurePath,
         lambda filepath, download_name=None: FileResponse(
             str(filepath), download_name=download_name
         ),
     )
     response_converter.register(URL, RedirectResponse)
+    response_converter.register(BaseModel, JSONResponse)
 
     for type_, converter in converters.items():
         response_converter.register(type_, converter)
 
     return response_converter
```

### Comparing `kui-1.5.2/kui/wsgi/cors.py` & `kui-1.5.3/kui/wsgi/cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/wsgi/exceptions.py` & `kui-1.5.3/kui/wsgi/exceptions.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/wsgi/openapi.py` & `kui-1.5.3/kui/wsgi/openapi.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/wsgi/parameters.py` & `kui-1.5.3/kui/wsgi/parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/wsgi/requests.py` & `kui-1.5.3/kui/wsgi/requests.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/wsgi/responses.py` & `kui-1.5.3/kui/wsgi/responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/wsgi/routing.py` & `kui-1.5.3/kui/wsgi/routing.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/wsgi/templates.py` & `kui-1.5.3/kui/wsgi/templates.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/kui/wsgi/views.py` & `kui-1.5.3/kui/wsgi/views.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/pyproject.toml` & `kui-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kui"
-version = "1.5.2"
+version = "1.5.3"
 description = "An easy-to-use web framework."
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "baize<0.21.0,>=0.20.0",
     "pydantic>=2.0",
```

### Comparing `kui-1.5.2/tests/asgi/test_application.py` & `kui-1.5.3/tests/asgi/test_application.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/asgi/test_cors.py` & `kui-1.5.3/tests/asgi/test_cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/asgi/test_parameters.py` & `kui-1.5.3/tests/asgi/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/asgi/test_views.py` & `kui-1.5.3/tests/asgi/test_views.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/openapi/test_application.py` & `kui-1.5.3/tests/openapi/test_application.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/routing/extensions/test_multimethod.py` & `kui-1.5.3/tests/routing/extensions/test_multimethod.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/routing/test_routes.py` & `kui-1.5.3/tests/routing/test_routes.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/routing/test_tree.py` & `kui-1.5.3/tests/routing/test_tree.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/test_responses.py` & `kui-1.5.3/tests/test_responses.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/test_security.py` & `kui-1.5.3/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/utils/test_importer.py` & `kui-1.5.3/tests/utils/test_importer.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/wsgi/test_cors.py` & `kui-1.5.3/tests/wsgi/test_cors.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/tests/wsgi/test_parameters.py` & `kui-1.5.3/tests/wsgi/test_parameters.py`

 * *Files identical despite different names*

### Comparing `kui-1.5.2/PKG-INFO` & `kui-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kui
-Version: 1.5.2
+Version: 1.5.3
 Summary: An easy-to-use web framework.
 License: Apache-2.0
 Author-email: abersheeran <me@abersheeran.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

