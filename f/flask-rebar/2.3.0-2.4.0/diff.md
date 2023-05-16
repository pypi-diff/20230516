# Comparing `tmp/flask-rebar-2.3.0.tar.gz` & `tmp/flask-rebar-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-rebar-2.3.0.tar", last modified: Tue Nov 29 14:12:51 2022, max compression
+gzip compressed data, was "flask-rebar-2.4.0.tar", last modified: Tue May 16 17:29:34 2023, max compression
```

## Comparing `flask-rebar-2.3.0.tar` & `flask-rebar-2.4.0.tar`

### file list

```diff
@@ -1,78 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.972022 flask-rebar-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (116)      200 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (116)     1073 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      138 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5225 2022-11-29 14:12:51.972022 flask-rebar-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4037 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.940022 flask-rebar-2.3.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.944022 flask-rebar-2.3.0/examples/todo/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/examples/todo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3013 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/examples/todo/generate_output.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.944022 flask-rebar-2.3.0/examples/todo/todo/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/examples/todo/todo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1366 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/examples/todo/todo/app.py
--rw-r--r--   0 runner    (1001) docker     (116)       91 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/examples/todo/todo/database.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.944022 flask-rebar-2.3.0/examples/todo/todo/handlers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/examples/todo/todo/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2565 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/examples/todo/todo/handlers/todo_handlers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1859 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/examples/todo/todo/schemas.py
--rw-r--r--   0 runner    (1001) docker     (116)       57 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/examples/todo/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.948022 flask-rebar-2.3.0/flask_rebar/
--rw-r--r--   0 runner    (1001) docker     (116)      541 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.948022 flask-rebar-2.3.0/flask_rebar/authenticators/
--rw-r--r--   0 runner    (1001) docker     (116)      189 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/authenticators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      769 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/authenticators/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     2268 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/authenticators/header_api_key.py
--rw-r--r--   0 runner    (1001) docker     (116)     2151 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/compat.py
--rw-r--r--   0 runner    (1001) docker     (116)     3875 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)     2550 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/messages.py
--rw-r--r--   0 runner    (1001) docker     (116)    30966 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/rebar.py
--rw-r--r--   0 runner    (1001) docker     (116)      407 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/request_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.948022 flask-rebar-2.3.0/flask_rebar/swagger_generation/
--rw-r--r--   0 runner    (1001) docker     (116)      612 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6997 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_generation/authenticator_to_swagger.py
--rw-r--r--   0 runner    (1001) docker     (116)     8290 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_generation/generator_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    20364 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_generation/marshmallow_to_swagger.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.948022 flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_generator/
--rw-r--r--   0 runner    (1001) docker     (116)      388 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6295 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_generator_base.py
--rw-r--r--   0 runner    (1001) docker     (116)    13591 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_generator_v2.py
--rw-r--r--   0 runner    (1001) docker     (116)    13138 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_generator_v3.py
--rw-r--r--   0 runner    (1001) docker     (116)     3183 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_objects.py
--rw-r--r--   0 runner    (1001) docker     (116)     2117 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_words.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.948022 flask-rebar-2.3.0/flask_rebar/swagger_ui/
--rw-r--r--   0 runner    (1001) docker     (116)       73 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1432 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/blueprint.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.968022 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/
--rw-r--r--   0 runner    (1001) docker     (116)      445 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (116)     1141 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (116)     2388 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/oauth2-redirect.html
--rw-r--r--   0 runner    (1001) docker     (116)  1534401 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (116) 11349827 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map
--rw-r--r--   0 runner    (1001) docker     (116)   330779 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (116)  2226997 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map
--rw-r--r--   0 runner    (1001) docker     (116)    33055 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui.css
--rw-r--r--   0 runner    (1001) docker     (116)       91 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui.css.map
--rw-r--r--   0 runner    (1001) docker     (116)   349441 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui.js
--rw-r--r--   0 runner    (1001) docker     (116)  2222505 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui.js.map
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.972022 flask-rebar-2.3.0/flask_rebar/swagger_ui/templates/
--rw-r--r--   0 runner    (1001) docker     (116)     3818 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/swagger_ui/templates/index.html.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.972022 flask-rebar-2.3.0/flask_rebar/testing/
--rw-r--r--   0 runner    (1001) docker     (116)      444 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    85712 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/testing/swagger_jsonschema.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.972022 flask-rebar-2.3.0/flask_rebar/utils/
--rw-r--r--   0 runner    (1001) docker     (116)       36 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       36 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (116)     5723 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (116)     1096 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/utils/marshmallow_objects_helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     7397 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/utils/request_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     5174 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/flask_rebar/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:12:51.948022 flask-rebar-2.3.0/flask_rebar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5225 2022-11-29 14:12:51.000000 flask-rebar-2.3.0/flask_rebar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2292 2022-11-29 14:12:51.000000 flask-rebar-2.3.0/flask_rebar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-29 14:12:51.000000 flask-rebar-2.3.0/flask_rebar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      314 2022-11-29 14:12:51.000000 flask-rebar-2.3.0/flask_rebar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       21 2022-11-29 14:12:51.000000 flask-rebar-2.3.0/flask_rebar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      176 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-11-29 14:12:51.972022 flask-rebar-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2066 2022-11-29 14:12:47.000000 flask-rebar-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.750270 flask-rebar-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-16 17:29:34.750270 flask-rebar-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.718270 flask-rebar-2.4.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.722270 flask-rebar-2.4.0/examples/todo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/generate_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.722270 flask-rebar-2.4.0/examples/todo/todo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.722270 flask-rebar-2.4.0/examples/todo/todo/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/handlers/todo_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/todo/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/examples/todo/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar/authenticators/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/authenticators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/authenticators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/authenticators/header_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31006 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/rebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/request_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar/swagger_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6996 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/authenticator_to_swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/marshmallow_to_swagger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6295 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13591 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13266 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_words.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar/swagger_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/blueprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.746270 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/oauth2-redirect.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1534401 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123) 11349827 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   330779 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2226997 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    33055 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 17:29:30.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)   349441 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2222505 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.746270 flask-rebar-2.4.0/flask_rebar/swagger_ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/swagger_ui/templates/index.html.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.746270 flask-rebar-2.4.0/flask_rebar/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85712 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/testing/swagger_jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.746270 flask-rebar-2.4.0/flask_rebar/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/utils/marshmallow_objects_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/utils/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/flask_rebar/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.726270 flask-rebar-2.4.0/flask_rebar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-16 17:29:34.000000 flask-rebar-2.4.0/flask_rebar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-16 17:29:34.000000 flask-rebar-2.4.0/flask_rebar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:29:34.000000 flask-rebar-2.4.0/flask_rebar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-16 17:29:34.000000 flask-rebar-2.4.0/flask_rebar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 17:29:34.000000 flask-rebar-2.4.0/flask_rebar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 17:29:34.750270 flask-rebar-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:29:34.750270 flask-rebar-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/tests/test_deprecation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29629 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/tests/test_rebar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/tests/test_request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-05-16 17:29:31.000000 flask-rebar-2.4.0/tests/test_validation.py
```

### Comparing `flask-rebar-2.3.0/LICENSE` & `flask-rebar-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/PKG-INFO` & `flask-rebar-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: flask-rebar
-Version: 2.3.0
+Version: 2.4.0
 Summary: Flask-Rebar combines flask, marshmallow, and swagger for robust REST services.
 Home-page: https://github.com/plangrid/flask-rebar
 Author: Barak Alon
 Author-email: barak.s.alon@gmail.com
 License: MIT
 Keywords: flask,rest,marshmallow,openapi,swagger
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 Provides-Extra: enum
 License-File: LICENSE
```

### Comparing `flask-rebar-2.3.0/README.rst` & `flask-rebar-2.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/examples/todo/generate_output.py` & `flask-rebar-2.4.0/examples/todo/generate_output.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/examples/todo/todo/app.py` & `flask-rebar-2.4.0/examples/todo/todo/app.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/examples/todo/todo/handlers/todo_handlers.py` & `flask-rebar-2.4.0/examples/todo/todo/handlers/todo_handlers.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/examples/todo/todo/schemas.py` & `flask-rebar-2.4.0/examples/todo/todo/schemas.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/__init__.py` & `flask-rebar-2.4.0/flask_rebar/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/authenticators/base.py` & `flask-rebar-2.4.0/flask_rebar/authenticators/base.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/authenticators/header_api_key.py` & `flask-rebar-2.4.0/flask_rebar/authenticators/header_api_key.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/compat.py` & `flask-rebar-2.4.0/flask_rebar/compat.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     Our wrapper for Schema.dump that includes optional validation.
     Note that as of Flask-Rebar 2.x (hence Marshmallow 3.x), Marshmallow's default behavior is to NOT validate on dump
     Accordingly, we are making validation "opt-in" here, which can be controlled at schema level with
     RequireOnDumpMixin or globally via validate_on_dump attribute of Rebar instance
     """
     try:
         force_validation = current_app.extensions["rebar"]["instance"].validate_on_dump
-    except RuntimeError:  # running outside app context (some unit test cases, potentially ad hoc scripts)
+    except (
+        RuntimeError
+    ):  # running outside app context (some unit test cases, potentially ad hoc scripts)
         force_validation = False
 
     if isinstance(schema, RequireOnDumpMixin) or force_validation:
         try:
             # We do an initial schema.dump here in order to support arbitrary data objects (e.g., ORM objects, etc.)
             # and give us something we can pass to .load below
             # Since marshmallow 3 doesn't validate on dump, this has the effect of stripping unknown fields.
```

### Comparing `flask-rebar-2.3.0/flask_rebar/errors.py` & `flask-rebar-2.4.0/flask_rebar/errors.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/messages.py` & `flask-rebar-2.4.0/flask_rebar/messages.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/rebar.py` & `flask-rebar-2.4.0/flask_rebar/rebar.py`

 * *Files 0% similar despite different names*

```diff
@@ -843,15 +843,17 @@
                 )
 
         @app.teardown_request
         def teardown(exception):
             if isinstance(exception, SystemExit):
                 try:
                     run_unhandled_exception_handlers(exception)
-                except Exception:  # make sure the exception handlers dont prevent teardown
+                except (
+                    Exception
+                ):  # make sure the exception handlers dont prevent teardown
                     pass
 
     def _create_json_error_response(
         self, message, http_status_code, additional_data=None, headers=None
     ):
         """
         Compiles a response object for an error.
```

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_generation/__init__.py` & `flask-rebar-2.4.0/flask_rebar/swagger_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_generation/authenticator_to_swagger.py` & `flask-rebar-2.4.0/flask_rebar/swagger_generation/authenticator_to_swagger.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,14 @@
         "get_security_schemes": lambda self, obj, context: dict([func(obj)]),
         "get_security_requirements": lambda self, obj, context: [{func(obj)[0]: []}],
     }
     return type(name, (AuthenticatorConverter,), meta)
 
 
 class HeaderApiKeyConverter(AuthenticatorConverter):
-
     AUTHENTICATOR_TYPE = HeaderApiKeyAuthenticator
 
     def get_security_requirements(self, obj, context):
         """
         :param HeaderApiKeyAuthenticator obj:
         :param _Context context:
         :return: list
```

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_generation/generator_utils.py` & `flask-rebar-2.4.0/flask_rebar/swagger_generation/generator_utils.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_generation/marshmallow_to_swagger.py` & `flask-rebar-2.4.0/flask_rebar/swagger_generation/marshmallow_to_swagger.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,19 +23,22 @@
 from marshmallow.validate import Validator
 
 from flask_rebar import compat
 from flask_rebar.validation import QueryParamList
 from flask_rebar.validation import CommaSeparatedList
 from flask_rebar.swagger_generation import swagger_words as sw
 
+LoadDumpOptions = None
 try:
-    from marshmallow_enum import EnumField, LoadDumpOptions
-except ImportError:
-    EnumField = None
-    LoadDumpOptions = None
+    EnumField = m.fields.Enum
+except AttributeError:
+    try:
+        from marshmallow_enum import EnumField, LoadDumpOptions
+    except ImportError:
+        EnumField = None
 
 
 # Special value to signify that a JSONSchema field should be left unset
 class UNSET(object):
     pass
 
 
@@ -468,15 +471,19 @@
 
     @sets_swagger_attr(sw.collection_format)
     def get_collection_format(self, obj, context):
         return sw.csv if context.openapi_version == 2 else UNSET
 
     @sets_swagger_attr(sw.style)
     def get_style(self, obj, context):
-        return sw.simple if context.openapi_version == 3 else UNSET
+        return sw.form if context.openapi_version == 3 else UNSET
+
+    @sets_swagger_attr(sw.explode)
+    def get_explode(self, obj, context):
+        return False if context.openapi_version == 3 else UNSET
 
 
 class MultiArrayConverter(ListConverter):
     MARSHMALLOW_TYPE = QueryParamList
 
     @sets_swagger_attr(sw.collection_format)
     def get_collection_format(self, obj, context):
@@ -635,29 +642,35 @@
 
 class EnumConverter(FieldConverter):
     MARSHMALLOW_TYPE = EnumField
 
     @sets_swagger_attr(sw.type_)
     def get_type(self, obj, context):
         # Note: we don't (yet?) support mix-and-match between load_by and dump_by. Pick one.
-        if obj.by_value or (obj.load_by == obj.dump_by == LoadDumpOptions.value):
+        if obj.by_value or (
+            LoadDumpOptions is not None
+            and obj.load_by == obj.dump_by == LoadDumpOptions.value
+        ):
             # I'm going out on a limb and assuming your enum uses same type for all vals, else caveat emptor:
             value_type = type(next(iter(obj.enum)).value)
             if value_type is int:
                 return sw.integer
             elif value_type is float:
                 return sw.number
             else:
                 return sw.string
         else:
             return sw.string
 
     @sets_swagger_attr(sw.enum)
     def get_enum(self, obj, context):
-        if obj.by_value or (obj.load_by == obj.dump_by == LoadDumpOptions.value):
+        if obj.by_value or (
+            LoadDumpOptions is not None
+            and obj.load_by == obj.dump_by == LoadDumpOptions.value
+        ):
             return [entry.value for entry in obj.enum]
         else:
             return [entry.name for entry in obj.enum]
 
 
 ALL_CONVERTERS = tuple(
     [
```

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_generator_base.py` & `flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_base.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_generator_v2.py` & `flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_v2.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_generator_v3.py` & `flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_generator_v3.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         response_converter_registry=None,
         tags=None,
         servers=None,
         default_response_schema=Error(),
         authenticator_converter_registry=None,
         include_hidden=False,
     ):
-
         super(SwaggerV3Generator, self).__init__(
             openapi_major_version=3,
             version=version,
             title=title,
             description=description,
             default_response_schema=default_response_schema,
             query_string_converter_registry=query_string_converter_registry,
@@ -329,23 +328,26 @@
         for prop, field in get_schema_fields(schema):
             jsonschema = converter(field)
 
             # Pardon the ugliness.
             # We need the "explode" key to be at the parameters level, not at the schema level.
             explode = jsonschema.pop(sw.explode, None)
             description = jsonschema.pop(sw.description, None)
+            style = jsonschema.pop(sw.style, None)
 
             parameter = {
                 sw.name: prop,
                 sw.in_: in_,
                 sw.schema: jsonschema,
                 sw.required: bool(field.required),
             }
 
             if explode is not None:
                 parameter[sw.explode] = explode
             if description is not None:
                 parameter[sw.description] = description
+            if style is not None:
+                parameter[sw.style] = style
 
             parameters.append(parameter)
 
         return parameters
```

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_objects.py` & `flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_objects.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_generation/swagger_words.py` & `flask-rebar-2.4.0/flask_rebar/swagger_generation/swagger_words.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_ui/blueprint.py` & `flask-rebar-2.4.0/flask_rebar/swagger_ui/blueprint.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_ui/static/favicon-32x32.png` & `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_ui/static/oauth2-redirect.html` & `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/oauth2-redirect.html`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js` & `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map` & `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-bundle.js.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js` & `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map` & `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui-standalone-preset.js.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui.css` & `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui.js` & `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.js`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_ui/static/swagger-ui.js.map` & `flask-rebar-2.4.0/flask_rebar/swagger_ui/static/swagger-ui.js.map`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/swagger_ui/templates/index.html.jinja2` & `flask-rebar-2.4.0/flask_rebar/swagger_ui/templates/index.html.jinja2`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/testing/swagger_jsonschema.py` & `flask-rebar-2.4.0/flask_rebar/testing/swagger_jsonschema.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/utils/deprecation.py` & `flask-rebar-2.4.0/flask_rebar/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/utils/marshmallow_objects_helpers.py` & `flask-rebar-2.4.0/flask_rebar/utils/marshmallow_objects_helpers.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/utils/request_utils.py` & `flask-rebar-2.4.0/flask_rebar/utils/request_utils.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar/validation.py` & `flask-rebar-2.4.0/flask_rebar/validation.py`

 * *Files identical despite different names*

### Comparing `flask-rebar-2.3.0/flask_rebar.egg-info/PKG-INFO` & `flask-rebar-2.4.0/flask_rebar.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: flask-rebar
-Version: 2.3.0
+Version: 2.4.0
 Summary: Flask-Rebar combines flask, marshmallow, and swagger for robust REST services.
 Home-page: https://github.com/plangrid/flask-rebar
 Author: Barak Alon
 Author-email: barak.s.alon@gmail.com
 License: MIT
 Keywords: flask,rest,marshmallow,openapi,swagger
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 Provides-Extra: enum
 License-File: LICENSE
```

### Comparing `flask-rebar-2.3.0/flask_rebar.egg-info/SOURCES.txt` & `flask-rebar-2.4.0/flask_rebar.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -55,8 +55,13 @@
 flask_rebar/swagger_ui/templates/index.html.jinja2
 flask_rebar/testing/__init__.py
 flask_rebar/testing/swagger_jsonschema.py
 flask_rebar/utils/__init__.py
 flask_rebar/utils/defaults.py
 flask_rebar/utils/deprecation.py
 flask_rebar/utils/marshmallow_objects_helpers.py
-flask_rebar/utils/request_utils.py
+flask_rebar/utils/request_utils.py
+tests/test_deprecation_utils.py
+tests/test_errors.py
+tests/test_rebar.py
+tests/test_request_utils.py
+tests/test_validation.py
```

### Comparing `flask-rebar-2.3.0/setup.py` & `flask-rebar-2.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Sphinx==1.7.0",
     "sphinx_rtd_theme==0.2.4",
 ]
 
 if __name__ == "__main__":
     setup(
         name="flask-rebar",
-        version="2.3.0",
+        version="2.4.0",
         author="Barak Alon",
         author_email="barak.s.alon@gmail.com",
         description="Flask-Rebar combines flask, marshmallow, and swagger for robust REST services.",
         long_description=open("README.rst").read(),
         keywords=["flask", "rest", "marshmallow", "openapi", "swagger"],
         license="MIT",
         packages=find_packages(exclude=("test*", "examples")),
@@ -37,18 +37,17 @@
         classifiers=[
             "Environment :: Web Environment",
             "Framework :: Flask",
             "Intended Audience :: Developers",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
             "Programming Language :: Python",
-            "Programming Language :: Python :: 3.6",
-            "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
             "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
             "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
             "Topic :: Software Development :: Libraries :: Application Frameworks",
             "Topic :: Software Development :: Libraries :: Python Modules",
         ],
     )
```

