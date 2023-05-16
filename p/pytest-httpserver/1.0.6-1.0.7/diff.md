# Comparing `tmp/pytest_httpserver-1.0.6.tar.gz` & `tmp/pytest_httpserver-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_httpserver-1.0.6.tar", max compression
+gzip compressed data, was "pytest_httpserver-1.0.7.tar", max compression
```

## Comparing `pytest_httpserver-1.0.6.tar` & `pytest_httpserver-1.0.7.tar`

### file list

```diff
@@ -1,55 +1,73 @@
--rw-r--r--   0        0        0     9989 2022-09-12 07:25:14.312314 pytest_httpserver-1.0.6/CHANGES.rst
--rw-r--r--   0        0        0     2464 2022-09-03 08:53:55.022256 pytest_httpserver-1.0.6/CONTRIBUTION.md
--rw-r--r--   0        0        0     1069 2021-08-07 09:45:33.704177 pytest_httpserver-1.0.6/LICENSE
--rw-r--r--   0        0        0     4780 2022-09-07 19:46:29.729832 pytest_httpserver-1.0.6/README.md
--rw-r--r--   0        0        0      615 2022-07-13 16:49:54.026996 pytest_httpserver-1.0.6/doc/Makefile
--rw-r--r--   0        0        0        0 2020-01-13 18:30:17.841633 pytest_httpserver-1.0.6/doc/_static/.placeholder
--rw-r--r--   0        0        0     1689 2022-09-07 19:46:29.729832 pytest_httpserver-1.0.6/doc/api.rst
--rw-r--r--   0        0        0     9120 2022-07-13 16:49:54.026996 pytest_httpserver-1.0.6/doc/background.rst
--rw-r--r--   0        0        0       42 2022-04-26 06:28:54.759199 pytest_httpserver-1.0.6/doc/changes.rst
--rw-r--r--   0        0        0     5856 2022-09-12 07:25:14.313314 pytest_httpserver-1.0.6/doc/conf.py
--rw-r--r--   0        0        0     2420 2021-08-07 09:45:33.704177 pytest_httpserver-1.0.6/doc/fixtures.rst
--rw-r--r--   0        0        0      107 2021-08-07 09:45:33.704177 pytest_httpserver-1.0.6/doc/guide.rst
--rw-r--r--   0        0        0    23321 2022-09-12 06:46:31.629976 pytest_httpserver-1.0.6/doc/howto.rst
--rw-r--r--   0        0        0     1312 2022-07-13 16:49:54.027996 pytest_httpserver-1.0.6/doc/index.rst
--rw-r--r--   0        0        0    17789 2022-07-13 16:49:54.027996 pytest_httpserver-1.0.6/doc/tutorial.rst
--rw-r--r--   0        0        0     2229 2022-07-13 16:49:54.027996 pytest_httpserver-1.0.6/doc/upgrade.rst
--rwxr-xr-x   0        0        0      391 2022-07-13 16:49:54.027996 pytest_httpserver-1.0.6/example.py
--rw-r--r--   0        0        0     1331 2022-07-13 16:49:54.027996 pytest_httpserver-1.0.6/example_pytest.py
--rw-r--r--   0        0        0     2076 2022-09-12 07:25:14.313314 pytest_httpserver-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      835 2022-09-07 19:46:29.730832 pytest_httpserver-1.0.6/pytest_httpserver/__init__.py
--rw-r--r--   0        0        0     7214 2022-09-07 19:46:29.730832 pytest_httpserver-1.0.6/pytest_httpserver/blocking_httpserver.py
--rw-r--r--   0        0        0    46859 2022-09-07 19:46:29.731832 pytest_httpserver-1.0.6/pytest_httpserver/httpserver.py
--rw-r--r--   0        0        0        0 2021-11-09 09:15:44.243511 pytest_httpserver-1.0.6/pytest_httpserver/py.typed
--rw-r--r--   0        0        0     1525 2022-07-13 16:49:54.028996 pytest_httpserver-1.0.6/pytest_httpserver/pytest_plugin.py
--rw-r--r--   0        0        0      603 2022-07-13 16:49:54.028996 pytest_httpserver-1.0.6/tests/assets/Makefile
--rw-r--r--   0        0        0      179 2020-01-13 18:30:17.843633 pytest_httpserver-1.0.6/tests/assets/README
--rw-r--r--   0        0        0      194 2020-01-13 18:30:17.843633 pytest_httpserver-1.0.6/tests/assets/rootCA.cnf
--rw-r--r--   0        0        0     1350 2020-01-13 18:30:17.843633 pytest_httpserver-1.0.6/tests/assets/rootCA.crt
--rw-r--r--   0        0        0     1679 2020-01-13 18:30:17.843633 pytest_httpserver-1.0.6/tests/assets/rootCA.key
--rw-r--r--   0        0        0       17 2020-01-13 18:30:17.843633 pytest_httpserver-1.0.6/tests/assets/rootCA.srl
--rw-r--r--   0        0        0      198 2020-01-13 18:30:17.843633 pytest_httpserver-1.0.6/tests/assets/server.cnf
--rw-r--r--   0        0        0     1688 2020-01-13 18:30:17.843633 pytest_httpserver-1.0.6/tests/assets/server.crt
--rw-r--r--   0        0        0     1078 2020-01-13 18:30:17.843633 pytest_httpserver-1.0.6/tests/assets/server.csr
--rw-r--r--   0        0        0     1704 2020-01-13 18:30:17.843633 pytest_httpserver-1.0.6/tests/assets/server.key
--rw-r--r--   0        0        0      200 2020-01-13 18:30:17.843633 pytest_httpserver-1.0.6/tests/assets/v3.ext
--rw-r--r--   0        0        0      593 2022-09-03 11:18:13.478145 pytest_httpserver-1.0.6/tests/conftest.py
--rw-r--r--   0        0        0     3343 2022-09-09 07:40:14.155206 pytest_httpserver-1.0.6/tests/test_blocking_httpserver.py
--rw-r--r--   0        0        0     1849 2022-09-12 06:46:31.629976 pytest_httpserver-1.0.6/tests/test_blocking_httpserver_howto.py
--rw-r--r--   0        0        0     2557 2021-11-09 09:15:44.243511 pytest_httpserver-1.0.6/tests/test_handler_errors.py
--rw-r--r--   0        0        0     4377 2022-07-13 16:49:54.028996 pytest_httpserver-1.0.6/tests/test_headers.py
--rw-r--r--   0        0        0     1864 2022-07-13 16:49:54.029996 pytest_httpserver-1.0.6/tests/test_json_matcher.py
--rw-r--r--   0        0        0     3183 2022-07-13 16:49:54.029996 pytest_httpserver-1.0.6/tests/test_mixed.py
--rw-r--r--   0        0        0     1817 2022-07-13 16:49:54.029996 pytest_httpserver-1.0.6/tests/test_oneshot.py
--rw-r--r--   0        0        0     1675 2022-07-13 16:49:54.029996 pytest_httpserver-1.0.6/tests/test_ordered.py
--rw-r--r--   0        0        0     3588 2022-07-13 16:49:54.029996 pytest_httpserver-1.0.6/tests/test_permanent.py
--rw-r--r--   0        0        0     1194 2022-07-13 16:49:54.029996 pytest_httpserver-1.0.6/tests/test_port_changing.py
--rw-r--r--   0        0        0     1488 2022-07-13 16:49:54.029996 pytest_httpserver-1.0.6/tests/test_querymatcher.py
--rw-r--r--   0        0        0     1355 2022-07-13 16:49:54.029996 pytest_httpserver-1.0.6/tests/test_querystring.py
--rw-r--r--   0        0        0     6365 2022-09-12 06:46:48.840120 pytest_httpserver-1.0.6/tests/test_release.py
--rw-r--r--   0        0        0     1202 2022-07-13 16:49:54.029996 pytest_httpserver-1.0.6/tests/test_ssl.py
--rw-r--r--   0        0        0     1875 2022-07-13 16:49:54.029996 pytest_httpserver-1.0.6/tests/test_urimatch.py
--rw-r--r--   0        0        0     3122 2022-07-13 16:49:54.029996 pytest_httpserver-1.0.6/tests/test_wait.py
--rw-r--r--   0        0        0      122 2020-01-13 18:30:17.844633 pytest_httpserver-1.0.6/tests/test_with_statement.py
--rw-r--r--   0        0        0     5722 1970-01-01 00:00:00.000000 pytest_httpserver-1.0.6/setup.py
--rw-r--r--   0        0        0     5897 1970-01-01 00:00:00.000000 pytest_httpserver-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11390 2023-05-16 19:40:52.284019 pytest_httpserver-1.0.7/CHANGES.rst
+-rw-r--r--   0        0        0     3225 2023-05-16 18:58:37.762110 pytest_httpserver-1.0.7/CONTRIBUTION.md
+-rw-r--r--   0        0        0     1069 2021-08-07 09:45:33.000000 pytest_httpserver-1.0.7/LICENSE
+-rw-r--r--   0        0        0     4780 2023-01-18 22:01:30.858852 pytest_httpserver-1.0.7/README.md
+-rw-r--r--   0        0        0      615 2023-01-18 22:01:30.858852 pytest_httpserver-1.0.7/doc/Makefile
+-rw-r--r--   0        0        0        0 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/doc/_static/.placeholder
+-rw-r--r--   0        0        0     1689 2023-01-18 22:01:30.858852 pytest_httpserver-1.0.7/doc/api.rst
+-rw-r--r--   0        0        0     8752 2023-05-16 19:40:52.284019 pytest_httpserver-1.0.7/doc/background.rst
+-rw-r--r--   0        0        0       42 2023-01-18 22:01:30.859852 pytest_httpserver-1.0.7/doc/changes.rst
+-rw-r--r--   0        0        0     5856 2023-05-16 19:40:52.284019 pytest_httpserver-1.0.7/doc/conf.py
+-rw-r--r--   0        0        0     2420 2021-08-07 09:45:33.000000 pytest_httpserver-1.0.7/doc/fixtures.rst
+-rw-r--r--   0        0        0      107 2021-08-07 09:45:33.000000 pytest_httpserver-1.0.7/doc/guide.rst
+-rw-r--r--   0        0        0    18202 2023-05-16 18:58:37.763110 pytest_httpserver-1.0.7/doc/howto.rst
+-rw-r--r--   0        0        0     1312 2023-01-18 22:01:30.859852 pytest_httpserver-1.0.7/doc/index.rst
+-rw-r--r--   0        0        0    17789 2023-05-16 18:58:37.763110 pytest_httpserver-1.0.7/doc/tutorial.rst
+-rw-r--r--   0        0        0     2229 2023-01-18 22:01:30.860852 pytest_httpserver-1.0.7/doc/upgrade.rst
+-rwxr-xr-x   0        0        0      391 2023-02-03 07:55:52.748134 pytest_httpserver-1.0.7/example.py
+-rw-r--r--   0        0        0     1331 2023-01-18 22:01:30.860852 pytest_httpserver-1.0.7/example_pytest.py
+-rw-r--r--   0        0        0     2127 2023-05-16 19:40:52.284019 pytest_httpserver-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      835 2023-01-18 22:01:30.861852 pytest_httpserver-1.0.7/pytest_httpserver/__init__.py
+-rw-r--r--   0        0        0     7214 2023-02-03 07:55:52.829130 pytest_httpserver-1.0.7/pytest_httpserver/blocking_httpserver.py
+-rw-r--r--   0        0        0    49366 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/pytest_httpserver/httpserver.py
+-rw-r--r--   0        0        0        0 2021-11-09 09:15:44.000000 pytest_httpserver-1.0.7/pytest_httpserver/py.typed
+-rw-r--r--   0        0        0     2333 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/pytest_httpserver/pytest_plugin.py
+-rw-r--r--   0        0        0      603 2023-01-18 22:01:30.863852 pytest_httpserver-1.0.7/tests/assets/Makefile
+-rw-r--r--   0        0        0      179 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/README
+-rw-r--r--   0        0        0      194 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/rootCA.cnf
+-rw-r--r--   0        0        0     1350 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/rootCA.crt
+-rw-r--r--   0        0        0     1679 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/rootCA.key
+-rw-r--r--   0        0        0       17 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/rootCA.srl
+-rw-r--r--   0        0        0      198 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/server.cnf
+-rw-r--r--   0        0        0     1688 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/server.crt
+-rw-r--r--   0        0        0     1078 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/server.csr
+-rw-r--r--   0        0        0     1704 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/server.key
+-rw-r--r--   0        0        0      200 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/assets/v3.ext
+-rw-r--r--   0        0        0      593 2023-02-03 07:55:52.757134 pytest_httpserver-1.0.7/tests/conftest.py
+-rw-r--r--   0        0        0     1849 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_example_blocking_httpserver.py
+-rw-r--r--   0        0        0      129 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_example_query_params1.py
+-rw-r--r--   0        0        0      165 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_example_query_params2.py
+-rw-r--r--   0        0        0     1495 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_authorization_headers.py
+-rw-r--r--   0        0        0      750 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_case_insensitive_matcher.py
+-rw-r--r--   0        0        0      369 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_check.py
+-rw-r--r--   0        0        0     1160 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_check_handler_errors.py
+-rw-r--r--   0        0        0      360 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_custom_handler.py
+-rw-r--r--   0        0        0      780 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_header_value_matcher.py
+-rw-r--r--   0        0        0      347 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_json_matcher.py
+-rw-r--r--   0        0        0      357 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_query_params_dict.py
+-rw-r--r--   0        0        0       99 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_query_params_never_do_this.py
+-rw-r--r--   0        0        0       98 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_query_params_proper_use.py
+-rw-r--r--   0        0        0      187 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_regexp.py
+-rw-r--r--   0        0        0      235 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_timeout_requests.py
+-rw-r--r--   0        0        0      390 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_url_matcher.py
+-rw-r--r--   0        0        0      788 2023-05-16 18:58:37.764109 pytest_httpserver-1.0.7/tests/examples/test_howto_wait_success.py
+-rw-r--r--   0        0        0     3481 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_blocking_httpserver.py
+-rw-r--r--   0        0        0     2557 2021-11-09 09:15:44.000000 pytest_httpserver-1.0.7/tests/test_handler_errors.py
+-rw-r--r--   0        0        0     4280 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_headers.py
+-rw-r--r--   0        0        0      567 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_ip_protocols.py
+-rw-r--r--   0        0        0     1864 2023-02-03 07:56:47.174314 pytest_httpserver-1.0.7/tests/test_json_matcher.py
+-rw-r--r--   0        0        0     3309 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_mixed.py
+-rw-r--r--   0        0        0     1817 2023-01-18 22:01:30.865852 pytest_httpserver-1.0.7/tests/test_oneshot.py
+-rw-r--r--   0        0        0     1675 2023-01-18 22:01:30.865852 pytest_httpserver-1.0.7/tests/test_ordered.py
+-rw-r--r--   0        0        0     1077 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_parse_qs.py
+-rw-r--r--   0        0        0     4122 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_permanent.py
+-rw-r--r--   0        0        0     1194 2023-02-03 07:56:47.174314 pytest_httpserver-1.0.7/tests/test_port_changing.py
+-rw-r--r--   0        0        0     1488 2023-01-18 22:01:30.866852 pytest_httpserver-1.0.7/tests/test_querymatcher.py
+-rw-r--r--   0        0        0     1355 2023-02-03 07:55:52.798132 pytest_httpserver-1.0.7/tests/test_querystring.py
+-rw-r--r--   0        0        0     6401 2023-05-16 18:58:37.765109 pytest_httpserver-1.0.7/tests/test_release.py
+-rw-r--r--   0        0        0     1202 2023-02-03 07:55:52.799132 pytest_httpserver-1.0.7/tests/test_ssl.py
+-rw-r--r--   0        0        0     1875 2023-02-03 07:55:52.818131 pytest_httpserver-1.0.7/tests/test_urimatch.py
+-rw-r--r--   0        0        0     3122 2023-02-03 07:55:52.851129 pytest_httpserver-1.0.7/tests/test_wait.py
+-rw-r--r--   0        0        0      122 2020-01-13 18:30:17.000000 pytest_httpserver-1.0.7/tests/test_with_statement.py
+-rw-r--r--   0        0        0     5722 1970-01-01 00:00:00.000000 pytest_httpserver-1.0.7/setup.py
+-rw-r--r--   0        0        0     5898 1970-01-01 00:00:00.000000 pytest_httpserver-1.0.7/PKG-INFO
```

### Comparing `pytest_httpserver-1.0.6/CHANGES.rst` & `pytest_httpserver-1.0.7/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,55 @@
 =============
 Release Notes
 =============
 
+.. _Release Notes_1.0.7:
+
+1.0.7
+=====
+
+.. _Release Notes_1.0.7_Upgrade Notes:
+
+Upgrade Notes
+-------------
+
+- With werkzeug 2.3.x the headers type has been updated to not allow integers as header values. This restriction followed up in pytest-httpserver.
+
+
+.. _Release Notes_1.0.7_Deprecation Notes:
+
+Deprecation Notes
+-----------------
+
+- Python versions earlier than 3.8 have been deprecated in order to support
+  the latest werkzeug. Users using 3.7 or earlier python may use
+  pytest-httpserver with earlier werkzeug versions but tests are no longer run
+  for these python versions.
+
+
+.. _Release Notes_1.0.7_Bug Fixes:
+
+Bug Fixes
+---------
+
+- Type hinting for header_value_matcher has been fixed. From now, specifying a
+  callable as ``Callable[[str, Optional[str], str], bool]`` will be accepted
+  also. Providing a ``HeaderValueMatcher`` object will be also accepted as
+  before, as it provides the same callable signature.
+
+- Fix Werkzeug deprecation warning about ``parse_authorization_header`` call.
+  Replace ``parse_authorization_header`` with ``Authorization.from_header`` as
+  suggested. This fix should not introduce any functional change for the
+  users.
+
+- Fix Werkzeug deprecation warning about ``werkzeug.urls.url_decode`` call. This
+  call has been changed to ``urllib.parse.parse_qsl`` in the implementation.
+  This fix should not introduce any functional change for the users.
+
+
 .. _Release Notes_1.0.6:
 
 1.0.6
 =====
 
 .. _Release Notes_1.0.6_New Features:
```

### Comparing `pytest_httpserver-1.0.6/CONTRIBUTION.md` & `pytest_httpserver-1.0.7/CONTRIBUTION.md`

 * *Files 26% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 https://pytest-httpserver.readthedocs.io/en/latest/background.html
 
 
 ## Rules
 
 There are a few rules you are kindly asked to accept:
 
-* Coding style is checked by `pre-commit`. You can run `make precommit` before proceeding
-  with the PR.
+* Coding style is checked by `pre-commit`. You can run `make precommit` before
+  proceeding with the PR. To install the pre-commit hooks to your git (so it
+  will be run for each commit), run `pre-commit install`.
 
 * Tests should be written for the new code. If there's a complex logic
   implemented, it should be tested on different valid and invalid inputs and
   scenarios.
 
 * The software is released under the MIT license, which is simple and liberal.
   Due to the size of the project, there are no contribution agreements, but you
@@ -37,22 +38,35 @@
 
 * The development is arranged around a virtualenv which needs to be created by
   the `make dev` command. It will create it in the `.venv` directory.
 
 * You can let your IDE of your choice to use the `.venv/bin/python` interpreter,
   so it will know all the dependencies.
 
-* running tests on the localhost can be done by issuing `make quick-test`. It is
-  "quick" because it tests the software with only one interpreter. Note that the
+* running tests on the localhost can be done by issuing `make test`. Note that the
   library can be used by many supported interpreters and unless it is absolutely
   required, we don't want to drop support.
 
+* running tests on multiple versions of interpreter locally can be done by
+  `tox`. Keep in mind that the CI job uses github actions with caching for
+  effective use, and `tox` is provided for the developers only.
+
+
 ## More technical details
 
 * Release notes must be written for significant changes. This is done by
   the `reno` tool. If you don't write any notes, no problem, it will be written
   by someone who merges your PR.
 
 * Documentation also needs to be written and updated. It means mostly
   docstrings, but if the PR changes the code and the way of working
   conceptually, the main documentation (located in the doc directory) needs to
   be updated and extended.
+
+* nix files are provided on a best-effort basis. `tox.nix` can be used to run
+  `tox`, `shell.nix` can be used instead of poetry for development. No tests
+  have been written for these (yet!), so they may be out of sync occasionally.
+
+* to release a new version, you can use the `scripts/release.py` script to make
+  the wheels and sdist, generate the changelog, and tag the commit. This tool
+  won't upload the artifacts as they need to be checked manually (by installing
+  the wheel to a new venv, for example).
```

### Comparing `pytest_httpserver-1.0.6/LICENSE` & `pytest_httpserver-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/README.md` & `pytest_httpserver-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/doc/Makefile` & `pytest_httpserver-1.0.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/doc/api.rst` & `pytest_httpserver-1.0.7/doc/api.rst`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/doc/background.rst` & `pytest_httpserver-1.0.7/doc/background.rst`

 * *Files 4% similar despite different names*

```diff
@@ -36,32 +36,23 @@
 
 This API allows to define an expected request and the response which will be
 sent back to the client in a single line. This is one of the key features so
 using the library is not complicated.
 
 Example:
 
-.. code-block:: python
-
-    def test_query_params(httpserver):
-        httpserver.expect_request("/foo", query_string={"user": "user1"}).respond_with_data(
-            "OK"
-        )
+.. literalinclude :: ../tests/examples/test_example_query_params1.py
+   :language: python
 
 It is simple in the most simple cases, but once the expectation is more
 specific, the line can grow significantly, so here the user is expected to put
 the literals into variables:
 
-.. code-block:: python
-
-    def test_query_params(httpserver):
-        httpserver.expect_request("/foo", query_string=expected_query).respond_with_data(
-            "OK"
-        )
-
+.. literalinclude :: ../tests/examples/test_example_query_params2.py
+   :language: python
 
 If the user wants something more complex, classes are available for this which
 can be instantiated and then specified for the parameters normally accepting
 only built-in types.
 
 The easy case should be made easy, with the possibility of making advanced
 things in a bit more complex way.
@@ -172,20 +163,19 @@
 Supporting the latest python versions (such as 3.7 and 3.8 at the time of
 writing this), is a must. Supporting the older versions is preferred, following
 the state of the officially supported python versions by PSF.
 
 The library should be tested periodically on the supported versions.
 
 Dropping support for old python versions is possible if supporting would cause
-an issue or require extensive workaround. Currently, 3.4 is still supported by
-the library, however it is deprecated by PSF. As it causes no problems for
-*pytest-httpserver* (there's an additional requirement for this in the setup.py,
-but that's all), the support for this version will be maintained as long as
-possible. Once a new change is added to the library which require great effort
-to maintain compatibility with 3.4, the support for it will be dropped.
+an issue or require extensive workaround.
+
+Python support for a given version is also dropped if it is near to the end of
+support or when a dependency deprecates it - this is needed to move forward with
+the community in order to support the latest versions of the dependencies.
 
 
 Testing and coverage
 --------------------
 
 It is not required to have 100% test coverage but all possible use-cases should
 be covered. Github actions is used to test the library on all the supported
```

### Comparing `pytest_httpserver-1.0.6/doc/conf.py` & `pytest_httpserver-1.0.7/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 author = "Zsolt Cserna"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "1.0.6"
+version = "1.0.7"
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
```

### Comparing `pytest_httpserver-1.0.6/doc/fixtures.rst` & `pytest_httpserver-1.0.7/doc/fixtures.rst`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/doc/howto.rst` & `pytest_httpserver-1.0.7/doc/howto.rst`

 * *Files 22% similar despite different names*

```diff
@@ -11,25 +11,21 @@
 
 Matching query parameters
 -------------------------
 
 To match query parameters, you must not included them to the URI, as this will
 not work:
 
-.. code-block:: python
-
-    def test_query_params(httpserver):
-        httpserver.expect_request("/foo?user=bar")  # never do this
+.. literalinclude :: ../tests/examples/test_howto_query_params_never_do_this.py
+   :language: python
 
 There's an explicit place where the query string should go:
 
-.. code-block:: python
-
-    def test_query_params(httpserver):
-        httpserver.expect_request("/foo", query_string="user=bar")
+.. literalinclude :: ../tests/examples/test_howto_query_params_proper_use.py
+   :language: python
 
 The ``query_string`` is the parameter which does not contain the leading
 question mark ``?``.
 
 .. note::
 
     The reason behind this is the underlying http server library *werkzeug*,
@@ -39,23 +35,17 @@
 
 
 As the order of the parameters in the query string usually does not matter, you
 can specify a dict for the ``query_string`` parameter (the naming may look a bit
 strange but we wanted to keep API compatibility and this dict matching feature
 was added later).
 
-.. code-block:: python
-
-    def test_query_params(httpserver):
-        httpserver.expect_request(
-            "/foo", query_string={"user": "user1", "group": "group1"}
-        ).respond_with_data("OK")
 
-        assert requests.get("/foo?user=user1&group=group1").status_code == 200
-        assert requests.get("/foo?group=group1&user=user1").status_code == 200
+.. literalinclude :: ../tests/examples/test_howto_query_params_dict.py
+   :language: python
 
 In the example above, both requests pass the test as we specified the expected
 query string as a dictionary.
 
 Behind the scenes an additional step is done by the library: it parses up the
 query_string into the dict and then compares it with the dict provided.
 
@@ -66,38 +56,28 @@
 The simplest form of URI matching is providing as a string. This is a equality
 match, if the URI of the request is not equal with the specified one, the
 request will not be handled.
 
 If this is not desired, you can specify a regexp object (returned by the
 ``re.compile()`` call).
 
-.. code:: python
-
-    httpserver.expect_request(re.compile("^/foo"), method="GET")
+.. literalinclude :: ../tests/examples/test_howto_regexp.py
+   :language: python
 
 The above will match every URI starting with "/foo".
 
 There's an additional way to extend this functionality. You can specify your own
 method which will receive the URI. All you need is to subclass from the
 ``URIPattern`` class and define the ``match()`` method which will get the uri as
 string and should return a boolean value.
 
 
-.. code:: python
-
-    class PrefixMatch(URIPattern):
-        def __init__(self, prefix: str):
-            self.prefix = prefix
-
-        def match(self, uri):
-            return uri.startswith(self.prefix)
-
+.. literalinclude :: ../tests/examples/test_howto_url_matcher.py
+   :language: python
 
-    def test_uripattern_object(httpserver: HTTPServer):
-        httpserver.expect_request(PrefixMatch("/foo")).respond_with_json({"foo": "bar"})
 
 Authentication
 --------------
 
 When doing http digest authentication, the client may send a request like this:
 
 .. code::
@@ -117,58 +97,16 @@
 
 Implementing a matcher is difficult for this request as the order of the
 parameters in the ``Authorization`` header value is arbitrary.
 
 By default, pytest-httpserver includes an Authorization header parser so the
 order of the parameters in the ``Authorization`` header does not matter.
 
-.. code:: python
-
-    def test_authorization_headers(httpserver: HTTPServer):
-        headers_with_values_in_direct_order = {
-            "Authorization": (
-                'Digest username="Mufasa",'
-                'realm="testrealm@host.com",'
-                'nonce="dcd98b7102dd2f0e8b11d0f600bfb0c093",'
-                'uri="/dir/index.html",'
-                "qop=auth,"
-                "nc=00000001,"
-                'cnonce="0a4f113b",'
-                'response="6629fae49393a05397450978507c4ef1",'
-                'opaque="5ccc069c403ebaf9f0171e9517f40e41"'
-            )
-        }
-        httpserver.expect_request(
-            uri="/", headers=headers_with_values_in_direct_order
-        ).respond_with_data("OK")
-        response = requests.get(
-            httpserver.url_for("/"), headers=headers_with_values_in_direct_order
-        )
-        assert response.status_code == 200
-        assert response.text == "OK"
-
-        headers_with_values_in_modified_order = {
-            "Authorization": (
-                "Digest qop=auth,"
-                'username="Mufasa",'
-                'nonce="dcd98b7102dd2f0e8b11d0f600bfb0c093",'
-                'uri="/dir/index.html",'
-                "nc=00000001,"
-                'realm="testrealm@host.com",'
-                'response="6629fae49393a05397450978507c4ef1",'
-                'cnonce="0a4f113b",'
-                'opaque="5ccc069c403ebaf9f0171e9517f40e41"'
-            )
-        }
-        response = requests.get(
-            httpserver.url_for("/"), headers=headers_with_values_in_modified_order
-        )
-        assert response.status_code == 200
-        assert response.text == "OK"
-
+.. literalinclude :: ../tests/examples/test_howto_authorization_headers.py
+   :language: python
 
 JSON matching
 -------------
 
 Matching the request data can be done in two different ways. One way is to
 provide a python string (or bytes object) whose value will be compared to the
 request body.
@@ -181,24 +119,16 @@
 could be dict, list or anything which can be the result of `json.loads()` call).
 The request's body will be loaded as json and the result will be compared to the
 provided object. If the request's body cannot be loaded as json, the matcher
 will fail and *pytest-httpserver* will proceed with the next registered matcher.
 
 Example:
 
-.. code:: python
-
-    def test_json_matcher(httpserver: HTTPServer):
-        httpserver.expect_request("/foo", json={"foo": "bar"}).respond_with_data(
-            "Hello world!"
-        )
-        resp = requests.get(httpserver.url_for("/foo"), json={"foo": "bar"})
-        assert resp.status_code == 200
-        assert resp.text == "Hello world!"
-
+.. literalinclude :: ../tests/examples/test_howto_json_matcher.py
+   :language: python
 
 .. note::
     JSON requests usually come with ``Content-Type: application/json`` header.
     *pytest-httpserver* provides the *headers* parameter to match the headers of
     the request, however matching json body does not imply matching the
     *Content-Type* header. If matching the header is intended, specify the expected
     *Content-Type* header and its value to the headers parameter.
@@ -218,37 +148,16 @@
 
 For each http header, you can specify a callable object (eg. a python function)
 which will be called with the header name, header actual value and the expected
 value, and will be able to determine the matching.
 
 You need to implement such a function and then use it:
 
-.. code:: python
-
-    def case_insensitive_matcher(header_name: str, actual: str, expected: str) -> bool:
-        if header_name == "X-Foo":
-            return actual.lower() == expected.lower()
-        else:
-            return actual == expected
-
-
-    def test_case_insensitive_matching(httpserver: HTTPServer):
-        httpserver.expect_request(
-            "/", header_value_matcher=case_insensitive_matcher, headers={"X-Foo": "bar"}
-        ).respond_with_data("OK")
-
-        assert (
-            requests.get(httpserver.url_for("/"), headers={"X-Foo": "bar"}).status_code
-            == 200
-        )
-        assert (
-            requests.get(httpserver.url_for("/"), headers={"X-Foo": "BAR"}).status_code
-            == 200
-        )
-
+.. literalinclude :: ../tests/examples/test_howto_case_insensitive_matcher.py
+   :language: python
 
 .. note::
     Header value matcher is the basis of the ``Authorization`` header parsing.
 
 
 If you want to change the matching of only one header, you may want to use the
 ``HeaderValueMatcher`` class.
@@ -281,57 +190,26 @@
             == 200
         )
 
 
 In case you don't want to change the defaults, you can provide the
 ``HeaderValueMatcher`` object itself.
 
-.. code:: python
-
-    from pytest_httpserver import HeaderValueMatcher
-
-
-    def case_insensitive_compare(actual: str, expected: str) -> bool:
-        return actual.lower() == expected.lower()
-
-
-    def test_own_matcher_object(httpserver: HTTPServer):
-        matcher = HeaderValueMatcher({"X-Bar": case_insensitive_compare})
-
-        httpserver.expect_request(
-            "/", headers={"X-Bar": "bar"}, header_value_matcher=matcher
-        ).respond_with_data("OK")
-
-        assert (
-            requests.get(httpserver.url_for("/"), headers={"X-Bar": "bar"}).status_code
-            == 200
-        )
-        assert (
-            requests.get(httpserver.url_for("/"), headers={"X-Bar": "BAR"}).status_code
-            == 200
-        )
+.. literalinclude :: ../tests/examples/test_howto_header_value_matcher.py
+   :language: python
 
 Using custom request handler
 ----------------------------
 In the case the response is not static, for example it depends on the request,
 you can pass a function to the ``respond_with_handler`` function. This function
 will be called with a request object and it should return a Response object.
 
-.. code:: python
-
-    from werkzeug.wrappers import Request, Response
-    from random import randint
-
-
-    def test_expected_request_handler(httpserver: HTTPServer):
-        def handler(request: Request):
-            return Response(str(randint(1, 10)))
-
-        httpserver.expect_request("/foobar").respond_with_handler(handler)
 
+.. literalinclude :: ../tests/examples/test_howto_custom_handler.py
+   :language: python
 
 The above code implements a handler which returns a random number between 1 and
 10. Not particularly useful but shows that the handler can return any computed
 or derived value.
 
 In the response handler you can also use the ``assert`` statement, similar to
 the tests, but there's a big difference. As the server is running in its own
@@ -340,65 +218,23 @@
 of the httpserver.
 
 In case you want to ensure that there was no other exception raised which was
 unhandled, you can call the ``check_handler_errors()`` method of the httpserver.
 
 Two notable examples for this:
 
-.. code:: python
-
-    def test_check_assertions_raises_handler_assertions(httpserver: HTTPServer):
-        def handler(_):
-            assert 1 == 2
-
-        httpserver.expect_request("/foobar").respond_with_handler(handler)
-
-        requests.get(httpserver.url_for("/foobar"))
-
-        # if you leave this "with" statement out, check_assertions() will break
-        # the test by re-raising the assertion error caused by the handler
-        # pytest will pick this exception as it was happened in the main thread
-        with pytest.raises(AssertionError):
-            httpserver.check_assertions()
-
-        httpserver.check_handler_errors()
-
-
-    def test_check_handler_errors_raises_handler_error(httpserver: HTTPServer):
-        def handler(_):
-            raise ValueError("should be propagated")
-
-        httpserver.expect_request("/foobar").respond_with_handler(handler)
-
-        requests.get(httpserver.url_for("/foobar"))
-
-        httpserver.check_assertions()
-
-        # if you leave this "with" statement out, check_handler_errors() will
-        # break the test with the original exception
-        with pytest.raises(ValueError):
-            httpserver.check_handler_errors()
-
+.. literalinclude :: ../tests/examples/test_howto_check_handler_errors.py
+   :language: python
 
 If you want to call both methods (``check_handler_errors()`` and
 ``check_assertions()``) you can call the ``check()`` method, which will call
 these.
 
-
-.. code:: python
-
-    def test_check_assertions(httpserver: HTTPServer):
-        def handler(_):
-            assert 1 == 2
-
-        httpserver.expect_request("/foobar").respond_with_handler(handler)
-
-        requests.get(httpserver.url_for("/foobar"))
-
-        httpserver.check()
+.. literalinclude :: ../tests/examples/test_howto_check.py
+   :language: python
 
 .. note::
     The scope of the errors checked by the ``check()`` method may
     change in the future - it is added to check all possible errors happened in
     the server.
 
 
@@ -474,66 +310,42 @@
 
 * timeout: time (in seconds) until time is out
 
 Behind the scenes it synchronizes the state of the server with the main thread.
 
 Last, you need to assert on the ``result`` attribute of the context object.
 
-.. code-block:: python
-
-    def test_wait_success(httpserver: HTTPServer):
-        waiting_timeout = 0.1
-
-        with httpserver.wait(stop_on_nohandler=False, timeout=waiting_timeout) as waiting:
-            requests.get(httpserver.url_for("/foobar"))
-            httpserver.expect_oneshot_request("/foobar").respond_with_data("OK foobar")
-            requests.get(httpserver.url_for("/foobar"))
-        assert waiting.result
-
-        httpserver.expect_oneshot_request("/foobar").respond_with_data("OK foobar")
-        httpserver.expect_oneshot_request("/foobaz").respond_with_data("OK foobaz")
-        with httpserver.wait(timeout=waiting_timeout) as waiting:
-            requests.get(httpserver.url_for("/foobar"))
-            requests.get(httpserver.url_for("/foobaz"))
-        assert waiting.result
-
+.. literalinclude :: ../tests/examples/test_howto_wait_success.py
+   :language: python
 
 In the above code, all the request.get() calls could be in a different thread,
 eg. running in parallel, but the exit condition of the context object is to wait
 for the specified conditions.
 
 
 Emulating connection refused error
 ----------------------------------
 
 If by any chance, you want to emulate network errors such as *Connection reset
 by peer* or *Connection refused*, you can simply do it by connecting to a random
 port number where no service is listening:
 
-.. code-block:: python
-
-    import pytest
-    import requests
-
-
-    def test_connection_refused():
-        # assumes that there's no server listening at localhost:1234
-        with pytest.raises(requests.exceptions.ConnectionError):
-            requests.get("http://localhost:1234")
-
+.. literalinclude :: ../tests/examples/test_howto_timeout_requests.py
+   :language: python
 
-However connecting to the port where the httpserver had been started will still
+However, connecting to the port where the httpserver had been started will still
 succeed as the server is running continuously. This is working by design as
 starting/stopping the server is costly.
 
 .. code-block:: python
 
     import pytest
     import requests
 
+
     # setting a fixed port for httpserver
     @pytest.fixture(scope="session")
     def httpserver_listen_address():
         return ("127.0.0.1", 8000)
 
 
     # this test will pass
@@ -603,28 +415,54 @@
 
     @pytest.fixture(scope="session")
     def ca():
         return trustme.CA()
 
 
     @pytest.fixture(scope="session")
-    def localhost_cert(ca):
-        return ca.issue_cert("localhost")
+    def httpserver_ssl_context(ca):
+        context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+        localhost_cert = ca.issue_cert("localhost")
+        localhost_cert.configure_cert(context)
+        return context
 
 
     @pytest.fixture(scope="session")
-    def httpserver_ssl_context(localhost_cert):
-        context = ssl.SSLContext(ssl.PROTOCOL_TLS_SERVER)
+    def httpclient_ssl_context(ca):
+        with ca.cert_pem.tempfile() as ca_temp_path:
+            return ssl.create_default_context(cafile=ca_temp_path)
 
-        crt = localhost_cert.cert_chain_pems[0]
-        key = localhost_cert.private_key_pem
-        with crt.tempfile() as crt_file, key.tempfile() as key_file:
-            context.load_cert_chain(crt_file, key_file)
 
-        return context
+    @pytest.mark.asyncio
+    async def test_aiohttp(httpserver, httpclient_ssl_context):
+        import aiohttp
+
+        httpserver.expect_request("/").respond_with_data("hello world!")
+        connector = aiohttp.TCPConnector(ssl=httpclient_ssl_context)
+        async with aiohttp.ClientSession(connector=connector) as session:
+            async with session.get(httpserver.url_for("/")) as result:
+                assert (await result.text()) == "hello world!"
+
+
+    def test_requests(httpserver, ca):
+        import requests
+
+        httpserver.expect_request("/").respond_with_data("hello world!")
+        with ca.cert_pem.tempfile() as ca_temp_path:
+            result = requests.get(httpserver.url_for("/"), verify=ca_temp_path)
+        assert result.text == "hello world!"
+
+
+    def test_httpx(httpserver, httpclient_ssl_context):
+        import httpx
+
+        httpserver.expect_request("/").respond_with_data("hello world!")
+        result = httpx.get(httpserver.url_for("/"), verify=httpclient_ssl_context)
+        assert result.text == "hello world!"
+
 
 Using httpserver on a dual-stack (IPv4 and IPv6) system
 -------------------------------------------------------
 
 *pytest-httpserver* can only listen on one address and it also means that
 address family is determined by that. As it relies on *Werkzeug*, it passes the
 provided host parameter to it and then it is up to *Werkzeug* how the port
@@ -668,9 +506,9 @@
 
 This is an experimental feature so *pytest-httpserver* has no fixture for it
 yet. If you find this feature useful any you have ideas or suggestions related
 to this, feel free to open an issue.
 
 Example:
 
-.. literalinclude :: ../tests/test_blocking_httpserver_howto.py
+.. literalinclude :: ../tests/examples/test_example_blocking_httpserver.py
    :language: python
```

### Comparing `pytest_httpserver-1.0.6/doc/index.rst` & `pytest_httpserver-1.0.7/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/doc/tutorial.rst` & `pytest_httpserver-1.0.7/doc/tutorial.rst`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 which is higher than 1024. In the examples on this page when we are referring to
 the url *http://localhost/...* it is assumed that the url contains the http port
 also.
 
 It is advised to use the ``url_for()`` method to construct an URL as it will
 always contain the correct port number in the URL.
 
-If you need the http port as an integer, you can get is by the ``port``
+If you need the http port as an integer, you can get it by the ``port``
 attribute of the ``httpserver`` object.
 
 
 How to test your http client
 ----------------------------
 
 .. note::
```

### Comparing `pytest_httpserver-1.0.6/doc/upgrade.rst` & `pytest_httpserver-1.0.7/doc/upgrade.rst`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/example_pytest.py` & `pytest_httpserver-1.0.7/example_pytest.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/pyproject.toml` & `pytest_httpserver-1.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest_httpserver"
-version = "1.0.6"
+version = "1.0.7"
 description = "pytest-httpserver is a httpserver for pytest"
 authors = ["Zsolt Cserna <cserna.zsolt@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://pytest-httpserver.readthedocs.io/en/latest/"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -20,15 +20,15 @@
     { path = "CHANGES.rst", format = "sdist" },
     { path = "CONTRIBUTION.md", format = "sdist" },
     { path = "example*.py", format = "sdist" },
     { path = "doc", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
+python = ">=3.8,<4.0"
 Werkzeug = ">= 2.0.0"
 
 
 [tool.poetry.plugins.pytest11]
 pytest_httpserver = "pytest_httpserver.pytest_plugin"
 
 [tool.poetry.urls]
@@ -42,18 +42,19 @@
 requests = "^2.28.1"
 Sphinx = "^5.1.1"
 sphinx-rtd-theme = "^1.0.0"
 reno = "^3.5.0"
 mypy = "^0.971"
 types-requests = "^2.28.9"
 pytest = "^7.1.3"
-pytest-cov = "^3.0.0"
-coverage = "^6.4.4"
-ipdb = "^0.13.9"
+pytest-cov = ">=3,<5"
+coverage = ">=6.4.4,<8.0.0"
 types-toml = "^0.10.8"
+toml = "^0.10.2"
+black = "^23.1.0"
 
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
 Sphinx = "^5.1.1"
@@ -61,21 +62,22 @@
 
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.1.3"
-pytest-cov = "^3.0.0"
-coverage = "^6.4.4"
+pytest-cov = ">=3,<5"
+coverage = ">=6.4.4,<8.0.0"
 requests = "^2.28.1"
 mypy = "^0.971"
 types-requests = "^2.28.9"
 pre-commit = "^2.20.0"
 types-toml = "^0.10.8"
+toml = "^0.10.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 markers = [
```

### Comparing `pytest_httpserver-1.0.6/pytest_httpserver/__init__.py` & `pytest_httpserver-1.0.7/pytest_httpserver/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/pytest_httpserver/blocking_httpserver.py` & `pytest_httpserver-1.0.7/pytest_httpserver/blocking_httpserver.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/pytest_httpserver/httpserver.py` & `pytest_httpserver-1.0.7/pytest_httpserver/httpserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import abc
+import ipaddress
 import json
 import queue
 import re
 import threading
 import time
+import urllib.parse
 from collections import defaultdict
 from contextlib import contextmanager
 from contextlib import suppress
 from copy import copy
 from enum import Enum
 from ssl import SSLContext
 from typing import Any
@@ -17,29 +19,31 @@
 from typing import Mapping
 from typing import MutableMapping
 from typing import Optional
 from typing import Pattern
 from typing import Tuple
 from typing import Union
 
-import werkzeug.urls
+import werkzeug.http
+from werkzeug.datastructures import Authorization
 from werkzeug.datastructures import MultiDict
-from werkzeug.http import parse_authorization_header
 from werkzeug.serving import make_server
 from werkzeug.wrappers import Request
 from werkzeug.wrappers import Response
 
 URI_DEFAULT = ""
 METHOD_ALL = "__ALL"
 
 HEADERS_T = Union[
-    Mapping[str, Union[str, int, Iterable[Union[str, int]]]],
-    Iterable[Tuple[str, Union[str, int]]],
+    Mapping[str, Union[str, Iterable[str]]],
+    Iterable[Tuple[str, str]],
 ]
 
+HVMATCHER_T = Callable[[str, Optional[str], str], bool]
+
 
 class Undefined:
     def __repr__(self):
         return "<UNDEFINED>"
 
 
 UNDEFINED = Undefined()
@@ -126,15 +130,18 @@
     DEFAULT_MATCHERS: MutableMapping[str, Callable[[Optional[str], str], bool]] = {}
 
     def __init__(self, matchers: Optional[Mapping[str, Callable[[Optional[str], str], bool]]] = None):
         self.matchers = self.DEFAULT_MATCHERS if matchers is None else matchers
 
     @staticmethod
     def authorization_header_value_matcher(actual: Optional[str], expected: str) -> bool:
-        return parse_authorization_header(actual) == parse_authorization_header(expected)
+        callable = getattr(Authorization, "from_header", None)
+        if callable is None:  # Werkzeug < 2.3.0
+            callable = werkzeug.http.parse_authorization_header
+        return callable(actual) == callable(expected)
 
     @staticmethod
     def default_header_value_matcher(actual: Optional[str], expected: str) -> bool:
         return actual == expected
 
     def __call__(self, header_name: str, actual: Optional[str], expected: str) -> bool:
         try:
@@ -209,15 +216,15 @@
             values specified for the same key in the request, the first element will be used.
             If you want to match multiple values, use a MultiDict object from werkzeug, which
             represents multiple values for one key.
         """
         self.query_dict = query_dict
 
     def get_comparing_values(self, request_query_string: bytes) -> tuple:
-        query = werkzeug.urls.url_decode(request_query_string)
+        query = MultiDict(urllib.parse.parse_qsl(request_query_string.decode("utf-8")))
         if isinstance(self.query_dict, MultiDict):
             return (query, self.query_dict)
         else:
             return (query.to_dict(), dict(self.query_dict))
 
 
 class BooleanQueryMatcher(QueryMatcher):
@@ -284,28 +291,34 @@
     :param headers: dictionary of the headers of the request to be matched
     :param query_string: the http query string, after ``?``, such as ``username=user``.
         If string is specified it will be encoded to bytes with the encode method of
         the string. If dict is specified, it will be matched to the ``key=value`` pairs
         specified in the request. If multiple values specified for a given key, the first
         value will be used. If multiple values needed to be handled, use ``MultiDict``
         object from werkzeug.
+    :param header_value_matcher: :py:class:`HeaderValueMatcher` that matches
+        values of headers, or a ``Callable[[str, Optional[str], str], bool]``
+        receiving the header key (from `headers`), header value (or `None`) and the expected
+        value (from `headers`) and should return ``True`` if the header matches, ``False`` otherwise.
+    :param json: a python object (eg. a dict) whose value will be compared to the request body after it
+        is loaded as json. If load fails, this matcher will be failed also. *Content-Type* is not checked.
+        If that's desired, add it to the headers parameter.
     """
 
     def __init__(
         self,
         uri: Union[str, URIPattern, Pattern[str]],
         method: str = METHOD_ALL,
         data: Union[str, bytes, None] = None,
         data_encoding: str = "utf-8",
         headers: Optional[Mapping[str, str]] = None,
         query_string: Union[None, QueryMatcher, str, bytes, Mapping] = None,
-        header_value_matcher: Optional[HeaderValueMatcher] = None,
+        header_value_matcher: Optional[HVMATCHER_T] = None,
         json: Any = UNDEFINED,
     ):
-
         if json is not UNDEFINED and data is not None:
             raise ValueError("data and json parameters are mutually exclusive")
 
         self.uri = uri
         self.method = method
         self.query_string = query_string
         self.query_matcher = _create_query_matcher(self.query_string)
@@ -317,15 +330,18 @@
 
         if isinstance(data, str):
             data = data.encode(data_encoding)
 
         self.data = data
         self.data_encoding = data_encoding
 
-        self.header_value_matcher = HeaderValueMatcher() if header_value_matcher is None else header_value_matcher
+        self.header_value_matcher: HVMATCHER_T = HeaderValueMatcher()
+
+        if header_value_matcher is not None:
+            self.header_value_matcher = header_value_matcher
 
     def __repr__(self):
         """
         Returns the string representation of the object, with the known parameters.
         """
 
         class_name = self.__class__.__name__
@@ -606,14 +622,17 @@
         self.server_thread = None
         self.assertions: List[str] = []
         self.handler_errors: List[Exception] = []
         self.log: List[Tuple[Request, Response]] = []
         self.ssl_context = ssl_context
         self.no_handler_status_code = 500
 
+    def __repr__(self):
+        return f"<{self.__class__.__name__} host={self.host} port={self.port}>"
+
     def clear(self):
         """
         Clears and resets the state attributes of the object.
 
         This method is useful when the object needs to be re-used but stopping the server is not feasible.
 
         """
@@ -646,28 +665,35 @@
     def url_for(self, suffix: str):
         """
         Return an url for a given suffix.
 
         This basically means that it prepends the string ``http://$HOST:$PORT/`` to the `suffix` parameter
         (where $HOST and $PORT are the parameters given to the constructor).
 
+        When host is an IPv6 address, the required square brackets will be added
+        to it, forming a valid URL.
+
+        When SSL or TLS is in use, the protocol of the returned URL will be ``https``.
+
         :param suffix: the suffix which will be added to the base url. It can start with ``/`` (slash) or
             not, the url will be the same.
         :return: the full url which refers to the server
         """
 
         if not suffix.startswith("/"):
             suffix = "/" + suffix
 
         if self.ssl_context is None:
             protocol = "http"
         else:
             protocol = "https"
 
-        return "{}://{}:{}{}".format(protocol, self.host, self.port, suffix)
+        host = self.format_host(self.host)
+
+        return "{}://{}:{}{}".format(protocol, host, self.port, suffix)
 
     def create_matcher(self, *args, **kwargs) -> RequestMatcher:
         """
         Creates a :py:class:`.RequestMatcher` instance with the specified parameters.
 
         This method can be overridden if you want to use your own matcher.
         """
@@ -833,14 +859,32 @@
 
         It stops the server if the server is running.
         Please note that depending on the internal things of werkzeug, it may take 0.5 seconds.
         """
         if self.is_running():
             self.stop()
 
+    @staticmethod
+    def format_host(host):
+        """
+        Formats a hostname so it can be used in a URL.
+        Notably, this adds brackets around IPV6 addresses when
+        they are missing.
+        """
+        try:
+            ipaddress.IPv6Address(host)
+            is_ipv6 = True
+        except ValueError:
+            is_ipv6 = False
+
+        if is_ipv6 and not host.startswith("[") and not host.endswith("]"):
+            return f"[{host}]"
+
+        return host
+
 
 class HTTPServer(HTTPServerBase):  # pylint: disable=too-many-instance-attributes
     """
     Server instance which manages handlers to serve pre-defined requests.
 
     :param host: the host or IP where the server will listen
     :param port: the TCP port where the server will listen
@@ -906,15 +950,15 @@
         self,
         uri: Union[str, URIPattern, Pattern[str]],
         method: str = METHOD_ALL,
         data: Union[str, bytes, None] = None,
         data_encoding: str = "utf-8",
         headers: Optional[Mapping[str, str]] = None,
         query_string: Union[None, QueryMatcher, str, bytes, Mapping] = None,
-        header_value_matcher: Optional[HeaderValueMatcher] = None,
+        header_value_matcher: Optional[HVMATCHER_T] = None,
         handler_type: HandlerType = HandlerType.PERMANENT,
         json: Any = UNDEFINED,
     ) -> RequestHandler:
         """
         Create and register a request handler.
 
         If `handler_type` is `HandlerType.PERMANENT` a permanent request handler is created. This handler can be used as
@@ -940,15 +984,18 @@
         :param headers: dictionary of the headers of the request to be matched
         :param query_string: the http query string, after ``?``, such as ``username=user``.
             If string is specified it will be encoded to bytes with the encode method of
             the string. If dict is specified, it will be matched to the ``key=value`` pairs
             specified in the request. If multiple values specified for a given key, the first
             value will be used. If multiple values needed to be handled, use ``MultiDict``
             object from werkzeug.
-        :param header_value_matcher: :py:class:`HeaderValueMatcher` that matches values of headers.
+        :param header_value_matcher: :py:class:`HeaderValueMatcher` that matches
+            values of headers, or a ``Callable[[str, Optional[str], str], bool]``
+            receiving the header key (from `headers`), header value (or `None`) and the expected
+            value (from `headers`) and should return ``True`` if the header matches, ``False`` otherwise.
         :param handler_type: type of handler
         :param json: a python object (eg. a dict) whose value will be compared to the request body after it
             is loaded as json. If load fails, this matcher will be failed also. *Content-Type* is not checked.
             If that's desired, add it to the headers parameter.
 
         :return: Created and register :py:class:`RequestHandler`.
 
@@ -978,15 +1025,15 @@
         self,
         uri: Union[str, URIPattern, Pattern[str]],
         method: str = METHOD_ALL,
         data: Union[str, bytes, None] = None,
         data_encoding: str = "utf-8",
         headers: Optional[Mapping[str, str]] = None,
         query_string: Union[None, QueryMatcher, str, bytes, Mapping] = None,
-        header_value_matcher: Optional[HeaderValueMatcher] = None,
+        header_value_matcher: Optional[HVMATCHER_T] = None,
         json: Any = UNDEFINED,
     ) -> RequestHandler:
         """
         Create and register a oneshot request handler.
 
         This is a method for convenience. See :py:meth:`expect_request` for documentation.
 
@@ -1000,15 +1047,18 @@
         :param headers: dictionary of the headers of the request to be matched
         :param query_string: the http query string, after ``?``, such as ``username=user``.
             If string is specified it will be encoded to bytes with the encode method of
             the string. If dict is specified, it will be matched to the ``key=value`` pairs
             specified in the request. If multiple values specified for a given key, the first
             value will be used. If multiple values needed to be handled, use ``MultiDict``
             object from werkzeug.
-        :param header_value_matcher: :py:class:`HeaderValueMatcher` that matches values of headers.
+        :param header_value_matcher: :py:class:`HeaderValueMatcher` that matches
+            values of headers, or a ``Callable[[str, Optional[str], str], bool]``
+            receiving the header key (from `headers`), header value (or `None`) and the expected
+            value (from `headers`) and should return ``True`` if the header matches, ``False`` otherwise.
         :param json: a python object (eg. a dict) whose value will be compared to the request body after it
             is loaded as json. If load fails, this matcher will be failed also. *Content-Type* is not checked.
             If that's desired, add it to the headers parameter.
 
         :return: Created and register :py:class:`RequestHandler`.
 
         Parameters `json` and `data` are mutually exclusive.
@@ -1030,15 +1080,15 @@
         self,
         uri: Union[str, URIPattern, Pattern[str]],
         method: str = METHOD_ALL,
         data: Union[str, bytes, None] = None,
         data_encoding: str = "utf-8",
         headers: Optional[Mapping[str, str]] = None,
         query_string: Union[None, QueryMatcher, str, bytes, Mapping] = None,
-        header_value_matcher: Optional[HeaderValueMatcher] = None,
+        header_value_matcher: Optional[HVMATCHER_T] = None,
         json: Any = UNDEFINED,
     ) -> RequestHandler:
         """
         Create and register a ordered request handler.
 
         This is a method for convenience. See :py:meth:`expect_request` for documentation.
 
@@ -1052,15 +1102,18 @@
         :param headers: dictionary of the headers of the request to be matched
         :param query_string: the http query string, after ``?``, such as ``username=user``.
             If string is specified it will be encoded to bytes with the encode method of
             the string. If dict is specified, it will be matched to the ``key=value`` pairs
             specified in the request. If multiple values specified for a given key, the first
             value will be used. If multiple values needed to be handled, use ``MultiDict``
             object from werkzeug.
-        :param header_value_matcher: :py:class:`HeaderValueMatcher` that matches values of headers.
+        :param header_value_matcher: :py:class:`HeaderValueMatcher` that matches
+            values of headers, or a ``Callable[[str, Optional[str], str], bool]``
+            receiving the header key (from `headers`), header value (or `None`) and the expected
+            value (from `headers`) and should return ``True`` if the header matches, ``False`` otherwise.
         :param json: a python object (eg. a dict) whose value will be compared to the request body after it
             is loaded as json. If load fails, this matcher will be failed also. *Content-Type* is not checked.
             If that's desired, add it to the headers parameter.
 
         :return: Created and register :py:class:`RequestHandler`.
 
         Parameters `json` and `data` are mutually exclusive.
```

### Comparing `pytest_httpserver-1.0.6/tests/assets/Makefile` & `pytest_httpserver-1.0.7/tests/assets/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/assets/rootCA.crt` & `pytest_httpserver-1.0.7/tests/assets/rootCA.crt`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/assets/rootCA.key` & `pytest_httpserver-1.0.7/tests/assets/rootCA.key`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/assets/server.crt` & `pytest_httpserver-1.0.7/tests/assets/server.crt`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/assets/server.csr` & `pytest_httpserver-1.0.7/tests/assets/server.csr`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/assets/server.key` & `pytest_httpserver-1.0.7/tests/assets/server.key`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/conftest.py` & `pytest_httpserver-1.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/test_blocking_httpserver.py` & `pytest_httpserver-1.0.7/tests/test_blocking_httpserver.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 def test_behave_workflow(httpserver: BlockingHTTPServer):
     request = dict(
         method="GET",
         url=httpserver.url_for("/my/path"),
     )
 
     with when_a_request_is_being_sent_to_the_server(request) as server_connection:
-
         client_connection = then_the_server_gets_the_request(httpserver, request)
 
         response = {"foo": "bar"}
 
         when_the_server_responds_to(client_connection, response)
 
         then_the_response_is_got_from(server_connection, response)
@@ -72,15 +71,14 @@
 def test_raises_assertion_error_when_request_does_not_match(httpserver: BlockingHTTPServer):
     request = dict(
         method="GET",
         url=httpserver.url_for("/my/path"),
     )
 
     with when_a_request_is_being_sent_to_the_server(request):
-
         with pytest.raises(AssertionError) as exc:
             httpserver.assert_request(uri="/not/my/path/")
 
         assert "/not/my/path/" in str(exc)
         assert "does not match" in str(exc)
 
 
@@ -95,28 +93,30 @@
 def test_ignores_when_request_is_not_asserted(httpserver: BlockingHTTPServer):
     request = dict(
         method="GET",
         url=httpserver.url_for("/my/path"),
     )
 
     with when_a_request_is_being_sent_to_the_server(request) as server_connection:
-
         assert server_connection.get(timeout=9).text == "No handler found for this request"
 
 
 def test_raises_assertion_error_when_request_was_not_responded(httpserver: BlockingHTTPServer):
     request = dict(
         method="GET",
         url=httpserver.url_for("/my/path"),
     )
 
     with when_a_request_is_being_sent_to_the_server(request):
-
         then_the_server_gets_the_request(httpserver, request)
 
         httpserver.stop()  # waiting for timeout of waiting for the response
 
         with pytest.raises(AssertionError) as exc:
             httpserver.check_assertions()
 
         assert "/my/path" in str(exc)
         assert "no response" in str(exc).lower()
+
+
+def test_repr(httpserver: BlockingHTTPServer):
+    assert repr(httpserver) == f"<BlockingHTTPServer host=localhost port={httpserver.port}>"
```

### Comparing `pytest_httpserver-1.0.6/tests/test_blocking_httpserver_howto.py` & `pytest_httpserver-1.0.7/tests/examples/test_example_blocking_httpserver.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/test_handler_errors.py` & `pytest_httpserver-1.0.7/tests/test_handler_errors.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/test_headers.py` & `pytest_httpserver-1.0.7/tests/test_headers.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,23 +78,22 @@
     assert response.status_code == 200
     assert response.text == "OK"
 
 
 def test_header_one_key_multiple_values(httpserver: HTTPServer):
     httpserver.expect_request(uri="/t1").respond_with_data(headers=[("X-Foo", "123"), ("X-Foo", "456")])
     httpserver.expect_request(uri="/t2").respond_with_data(headers={"X-Foo": ["123", "456"]})
-    httpserver.expect_request(uri="/t3").respond_with_data(headers={"X-Foo": [123, 456]})
 
     headers = Headers()
     headers.add("X-Foo", "123")
     headers.add("X-Foo", "456")
 
-    httpserver.expect_request(uri="/t4").respond_with_data(headers=headers)
+    httpserver.expect_request(uri="/t3").respond_with_data(headers=headers)
 
-    for uri in ("/t1", "/t2", "/t3", "/t4"):
+    for uri in ("/t1", "/t2", "/t3"):
         conn = http.client.HTTPConnection("localhost:{}".format(httpserver.port))
         conn.request("GET", uri)
         response = conn.getresponse()
         conn.close()
 
         assert response.status == 200
         assert response.headers.get_all("X-Foo") == ["123", "456"]
```

### Comparing `pytest_httpserver-1.0.6/tests/test_json_matcher.py` & `pytest_httpserver-1.0.7/tests/test_json_matcher.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/test_mixed.py` & `pytest_httpserver-1.0.7/tests/test_mixed.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,7 +78,11 @@
         httpserver.check_assertions()
 
     # handlers must be still intact but as the ordered are failed
     # everything will fail
     assert len(httpserver.ordered_handlers) == 2
     assert len(httpserver.oneshot_handlers) == 2
     assert len(httpserver.handlers) == 1
+
+
+def test_repr(httpserver: HTTPServer):
+    assert repr(httpserver) == f"<HTTPServer host=localhost port={httpserver.port}>"
```

### Comparing `pytest_httpserver-1.0.6/tests/test_oneshot.py` & `pytest_httpserver-1.0.7/tests/test_oneshot.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/test_ordered.py` & `pytest_httpserver-1.0.7/tests/test_ordered.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/test_permanent.py` & `pytest_httpserver-1.0.7/tests/test_permanent.py`

 * *Files 8% similar despite different names*

```diff
@@ -89,7 +89,20 @@
 
 def test_server_cleared_for_each_test(httpserver: HTTPServer):
     assert httpserver.log == []
     assert httpserver.assertions == []
     assert httpserver.ordered_handlers == []
     assert httpserver.oneshot_handlers == []
     assert httpserver.handlers == []
+
+
+def test_response_handler_replaced(httpserver: HTTPServer):
+    # https://github.com/csernazs/pytest-httpserver/issues/229
+    handler = httpserver.expect_request("/foobar")
+    handler.respond_with_data("FOO")
+    response = requests.get(httpserver.url_for("/foobar"))
+    assert response.text == "FOO"
+    assert response.status_code == 200
+    handler.respond_with_json({"foo": "bar"})
+    response = requests.get(httpserver.url_for("/foobar"))
+    assert response.json() == {"foo": "bar"}
+    assert response.status_code == 200
```

### Comparing `pytest_httpserver-1.0.6/tests/test_port_changing.py` & `pytest_httpserver-1.0.7/tests/test_port_changing.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/test_querymatcher.py` & `pytest_httpserver-1.0.7/tests/test_querymatcher.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/test_querystring.py` & `pytest_httpserver-1.0.7/tests/test_querystring.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/test_release.py` & `pytest_httpserver-1.0.7/tests/test_release.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
     def extract(self):
         self.wheel.extract()
         self.sdist.extract()
 
 
 @pytest.fixture(scope="session")
-def build(request) -> Iterable[Build]:
+def build() -> Iterable[Build]:
     dist_path = Path("dist").resolve()
     if dist_path.is_dir():
         shutil.rmtree(dist_path)
 
     try:
         subprocess.run(["poetry", "build"], check=True)
         assert dist_path.is_dir()
@@ -191,23 +191,25 @@
             "httpserver.py",
             "py.typed",
             "pytest_plugin.py",
         },
         "tests": {
             "assets",
             "conftest.py",
+            "examples",
             "test_blocking_httpserver.py",
-            "test_blocking_httpserver_howto.py",
             "test_handler_errors.py",
             "test_headers.py",
+            "test_ip_protocols.py",
             "test_json_matcher.py",
             "test_mixed.py",
             "test_oneshot.py",
             "test_ordered.py",
             "test_permanent.py",
+            "test_parse_qs.py",
             "test_port_changing.py",
             "test_querymatcher.py",
             "test_querystring.py",
             "test_release.py",
             "test_ssl.py",
             "test_urimatch.py",
             "test_wait.py",
```

### Comparing `pytest_httpserver-1.0.6/tests/test_ssl.py` & `pytest_httpserver-1.0.7/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/test_urimatch.py` & `pytest_httpserver-1.0.7/tests/test_urimatch.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/tests/test_wait.py` & `pytest_httpserver-1.0.7/tests/test_wait.py`

 * *Files identical despite different names*

### Comparing `pytest_httpserver-1.0.6/setup.py` & `pytest_httpserver-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 ['Werkzeug>=2.0.0']
 
 entry_points = \
 {'pytest11': ['pytest_httpserver = pytest_httpserver.pytest_plugin']}
 
 setup_kwargs = {
     'name': 'pytest-httpserver',
-    'version': '1.0.6',
+    'version': '1.0.7',
     'description': 'pytest-httpserver is a httpserver for pytest',
     'long_description': '[![Build Status](https://github.com/csernazs/pytest-httpserver/workflows/build/badge.svg?branch=master)](https://github.com/csernazs/pytest-httpserver/actions?query=workflow%3Abuild+branch%3Amaster)\n[![Documentation Status](https://readthedocs.org/projects/pytest-httpserver/badge/?version=latest)](https://pytest-httpserver.readthedocs.io/en/latest/?badge=latest)\n [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)\n[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=K6PU3AGBZW4QC&item_name=pytest-httpserver&currency_code=EUR&source=url)\n[![codecov](https://codecov.io/gh/csernazs/pytest-httpserver/branch/master/graph/badge.svg?token=MX2JXbHqRH)](https://codecov.io/gh/csernazs/pytest-httpserver)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n## pytest_httpserver\n\nHTTP server for pytest\n\n\n### Nutshell\n\nThis library is designed to help to test http clients without contacting the real http server.\nIn other words, it is a fake http server which is accessible via localhost can be started with\nthe pre-defined expected http requests and their responses.\n\n### Example\n\n#### Handling a simple GET request\n```python\ndef test_my_client(\n    httpserver,\n):  # httpserver is a pytest fixture which starts the server\n    # set up the server to serve /foobar with the json\n    httpserver.expect_request("/foobar").respond_with_json({"foo": "bar"})\n    # check that the request is served\n    assert requests.get(httpserver.url_for("/foobar")).json() == {"foo": "bar"}\n```\n\n#### Handing a POST request with an expected json body\n```python\ndef test_json_request(\n    httpserver,\n):  # httpserver is a pytest fixture which starts the server\n    # set up the server to serve /foobar with the json\n    httpserver.expect_request(\n        "/foobar", method="POST", json={"id": 12, "name": "foo"}\n    ).respond_with_json({"foo": "bar"})\n    # check that the request is served\n    assert requests.post(\n        httpserver.url_for("/foobar"), json={"id": 12, "name": "foo"}\n    ).json() == {"foo": "bar"}\n```\n\n\nYou can also use the library without pytest. There\'s a with statement to ensure that the server is stopped.\n\n\n```python\nwith HTTPServer() as httpserver:\n    # set up the server to serve /foobar with the json\n    httpserver.expect_request("/foobar").respond_with_json({"foo": "bar"})\n    # check that the request is served\n    print(requests.get(httpserver.url_for("/foobar")).json())\n```\n\n### Documentation\n\nPlease find the API documentation at https://pytest-httpserver.readthedocs.io/en/latest/.\n\n### Features\n\nYou can set up a dozen of expectations for the requests, and also what response should be sent by the server to the client.\n\n\n#### Requests\n\nThere are three different types:\n\n- **permanent**: this will be always served when there\'s match for this request, you can make as many HTTP requests as you want\n- **oneshot**: this will be served only once when there\'s a match for this request, you can only make 1 HTTP request\n- **ordered**: same as oneshot but the order must be strictly matched to the order of setting up\n\nYou can also fine-tune the expected request. The following can be specified:\n\n- URI (this is a must)\n- HTTP method\n- headers\n- query string\n- data (HTTP body of the request)\n- JSON (HTTP body loaded as JSON)\n\n\n#### Responses\n\nOnce you have the expectations for the request set up, you should also define the response you want to send back.\nThe following is supported currently:\n\n- respond arbitrary data (string or bytearray)\n- respond a json (a python dict converted in-place to json)\n- respond a Response object of werkzeug\n- use your own function\n\nSimilar to requests, you can fine-tune what response you want to send:\n\n- HTTP status\n- headers\n- data\n\n\n#### Behave support\n\nUsing the `BlockingHTTPServer` class, the assertion for a request and the\nresponse can be performed in real order. For more info, see the\n[test](tests/test_blocking_httpserver.py), the\n[howto](https://pytest-httpserver.readthedocs.io/en/latest/howto.html#running-httpserver-in-blocking-mode)\nand the [API\ndocumentation](https://pytest-httpserver.readthedocs.io/en/latest/api.html#blockinghttpserver).\n\n\n### Missing features\n* HTTP/2\n* Keepalive\n* ~~TLS~~\n\n### Donation\n\nIf you want to donate to this project, you can find the donate button at the top\nof the README.\n\nCurrently, this project is based heavily on werkzeug. Werkzeug does all the heavy lifting\nbehind the scenes, parsing HTTP request and defining Request and Response objects, which\nare currently transparent in the API.\n\nIf you wish to donate, please consider donating to them: https://palletsprojects.com/donate\n',
     'author': 'Zsolt Cserna',
     'author_email': 'cserna.zsolt@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/csernazs/pytest-httpserver',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+    'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `pytest_httpserver-1.0.6/PKG-INFO` & `pytest_httpserver-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pytest-httpserver
-Version: 1.0.6
+Version: 1.0.7
 Summary: pytest-httpserver is a httpserver for pytest
 Home-page: https://github.com/csernazs/pytest-httpserver
 License: MIT
 Author: Zsolt Cserna
 Author-email: cserna.zsolt@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Werkzeug (>=2.0.0)
 Project-URL: Bug Tracker, https://github.com/csernazs/pytest-httpserver/issues
 Project-URL: Documentation, https://pytest-httpserver.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/csernazs/pytest-httpserver
 Description-Content-Type: text/markdown
```

