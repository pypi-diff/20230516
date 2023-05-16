# Comparing `tmp/aleph-sdk-python-0.6.0b1.tar.gz` & `tmp/aleph-sdk-python-0.7.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleph-sdk-python-0.6.0b1.tar", last modified: Wed Jan 25 19:02:52 2023, max compression
+gzip compressed data, was "aleph-sdk-python-0.7.0b1.tar", last modified: Tue May 16 13:19:44 2023, max compression
```

## Comparing `aleph-sdk-python-0.6.0b1.tar` & `aleph-sdk-python-0.7.0b1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.335235 aleph-sdk-python-0.6.0b1/
--rw-r--r--   0 sepal     (1000) users      (100)      595 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/.coveragerc
--rw-r--r--   0 sepal     (1000) users      (100)       54 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/.dockerignore
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.329235 aleph-sdk-python-0.6.0b1/.github/
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.330235 aleph-sdk-python-0.6.0b1/.github/workflows/
--rw-r--r--   0 sepal     (1000) users      (100)     1065 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/.github/workflows/build-wheels.yml
--rw-r--r--   0 sepal     (1000) users      (100)      854 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/.github/workflows/code-quality.yml
--rw-r--r--   0 sepal     (1000) users      (100)     1582 2023-01-25 18:56:28.000000 aleph-sdk-python-0.6.0b1/.github/workflows/pytest-docker.yml
--rw-r--r--   0 sepal     (1000) users      (100)      537 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/.gitignore
--rw-r--r--   0 sepal     (1000) users      (100)      159 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/AUTHORS.rst
--rw-r--r--   0 sepal     (1000) users      (100)       82 2023-01-25 17:30:47.000000 aleph-sdk-python-0.6.0b1/CHANGELOG.rst
--rw-r--r--   0 sepal     (1000) users      (100)     1080 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/LICENSE.txt
--rw-r--r--   0 sepal     (1000) users      (100)      711 2023-01-25 19:02:52.335235 aleph-sdk-python-0.6.0b1/PKG-INFO
--rw-r--r--   0 sepal     (1000) users      (100)     1190 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/README.md
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.330235 aleph-sdk-python-0.6.0b1/docker/
--rw-r--r--   0 sepal     (1000) users      (100)     1085 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/docker/python-3.10.dockerfile
--rw-r--r--   0 sepal     (1000) users      (100)     1085 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/docker/python-3.11.dockerfile
--rw-r--r--   0 sepal     (1000) users      (100)     1084 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/docker/python-3.9.dockerfile
--rw-r--r--   0 sepal     (1000) users      (100)     1236 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/docker/ubuntu-20.04.dockerfile
--rw-r--r--   0 sepal     (1000) users      (100)     1236 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/docker/ubuntu-22.04.dockerfile
--rw-r--r--   0 sepal     (1000) users      (100)      888 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/docker/with-ipfs.dockerfile
--rwxr-xr-x   0 sepal     (1000) users      (100)      346 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docker/with-ipfs.entrypoint.sh
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.331236 aleph-sdk-python-0.6.0b1/docs/
--rw-r--r--   0 sepal     (1000) users      (100)     7622 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/docs/Makefile
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.331236 aleph-sdk-python-0.6.0b1/docs/_static/
--rw-r--r--   0 sepal     (1000) users      (100)       18 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docs/_static/.gitignore
--rw-r--r--   0 sepal     (1000) users      (100)     2774 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docs/_static/logo.svg
--rw-r--r--   0 sepal     (1000) users      (100)       41 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docs/authors.rst
--rw-r--r--   0 sepal     (1000) users      (100)       43 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docs/changelog.rst
--rw-r--r--   0 sepal     (1000) users      (100)     9745 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/docs/conf.py
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.331236 aleph-sdk-python-0.6.0b1/docs/content/
--rw-r--r--   0 sepal     (1000) users      (100)     3241 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docs/content/account.rst
--rw-r--r--   0 sepal     (1000) users      (100)     2347 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docs/content/aggregates.rst
--rw-r--r--   0 sepal     (1000) users      (100)     1543 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docs/content/async_notes.rst
--rw-r--r--   0 sepal     (1000) users      (100)     1924 2023-01-12 11:32:12.000000 aleph-sdk-python-0.6.0b1/docs/content/cli.rst
--rw-r--r--   0 sepal     (1000) users      (100)     2604 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docs/content/introduction.rst
--rw-r--r--   0 sepal     (1000) users      (100)     1402 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docs/content/posts.rst
--rw-r--r--   0 sepal     (1000) users      (100)     1159 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docs/content/programs.rst
--rw-r--r--   0 sepal     (1000) users      (100)     1482 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/docs/index.rst
--rw-r--r--   0 sepal     (1000) users      (100)       67 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/docs/license.rst
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.331236 aleph-sdk-python-0.6.0b1/examples/
--rw-r--r--   0 sepal     (1000) users      (100)     2019 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/examples/httpgateway.py
--rw-r--r--   0 sepal     (1000) users      (100)     1948 2023-01-25 17:18:01.000000 aleph-sdk-python-0.6.0b1/examples/metrics.py
--rw-r--r--   0 sepal     (1000) users      (100)     4081 2023-01-25 18:46:34.000000 aleph-sdk-python-0.6.0b1/examples/mqtt.py
--rw-r--r--   0 sepal     (1000) users      (100)     3407 2023-01-25 17:23:58.000000 aleph-sdk-python-0.6.0b1/examples/store.py
--rw-r--r--   0 sepal     (1000) users      (100)     2467 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/mypy.ini
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.331236 aleph-sdk-python-0.6.0b1/scripts/
--rw-r--r--   0 sepal     (1000) users      (100)      322 2023-01-25 18:56:38.000000 aleph-sdk-python-0.6.0b1/scripts/build-and-shell.sh
--rw-r--r--   0 sepal     (1000) users      (100)      457 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/scripts/build-and-test.sh
--rw-r--r--   0 sepal     (1000) users      (100)      408 2023-01-25 18:57:13.000000 aleph-sdk-python-0.6.0b1/scripts/build-to-publish.sh
--rw-r--r--   0 sepal     (1000) users      (100)     1896 2023-01-25 19:02:52.336235 aleph-sdk-python-0.6.0b1/setup.cfg
--rw-r--r--   0 sepal     (1000) users      (100)      576 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/setup.py
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.329235 aleph-sdk-python-0.6.0b1/src/
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.332235 aleph-sdk-python-0.6.0b1/src/aleph_client/
--rw-r--r--   0 sepal     (1000) users      (100)      469 2023-01-25 18:57:21.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/__init__.py
--rw-r--r--   0 sepal     (1000) users      (100)     1488 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/__main__.py
--rw-r--r--   0 sepal     (1000) users      (100)     2234 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/account.py
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.332235 aleph-sdk-python-0.6.0b1/src/aleph_client/chains/
--rw-r--r--   0 sepal     (1000) users      (100)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/chains/__init__.py
--rw-r--r--   0 sepal     (1000) users      (100)     2775 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/chains/common.py
--rw-r--r--   0 sepal     (1000) users      (100)     2338 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/chains/cosmos.py
--rw-r--r--   0 sepal     (1000) users      (100)     1242 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/chains/ethereum.py
--rw-r--r--   0 sepal     (1000) users      (100)     9048 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/chains/nuls1.py
--rw-r--r--   0 sepal     (1000) users      (100)     1713 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/chains/nuls2.py
--rw-r--r--   0 sepal     (1000) users      (100)     2324 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/chains/remote.py
--rw-r--r--   0 sepal     (1000) users      (100)     2588 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/chains/sol.py
--rw-r--r--   0 sepal     (1000) users      (100)     1315 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/chains/substrate.py
--rw-r--r--   0 sepal     (1000) users      (100)     1572 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/chains/tezos.py
--rw-r--r--   0 sepal     (1000) users      (100)     1927 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/conf.py
--rw-r--r--   0 sepal     (1000) users      (100)      646 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/exceptions.py
--rw-r--r--   0 sepal     (1000) users      (100)      354 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/models.py
--rw-r--r--   0 sepal     (1000) users      (100)     1086 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/types.py
--rw-r--r--   0 sepal     (1000) users      (100)    49298 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/user_session.py
--rw-r--r--   0 sepal     (1000) users      (100)     2162 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/utils.py
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.333235 aleph-sdk-python-0.6.0b1/src/aleph_client/vm/
--rw-r--r--   0 sepal     (1000) users      (100)       70 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/vm/__init__.py
--rw-r--r--   0 sepal     (1000) users      (100)     2633 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/vm/app.py
--rw-r--r--   0 sepal     (1000) users      (100)     4093 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/src/aleph_client/vm/cache.py
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.333235 aleph-sdk-python-0.6.0b1/src/aleph_sdk_python.egg-info/
--rw-r--r--   0 sepal     (1000) users      (100)      711 2023-01-25 19:02:52.000000 aleph-sdk-python-0.6.0b1/src/aleph_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 sepal     (1000) users      (100)     2710 2023-01-25 19:02:52.000000 aleph-sdk-python-0.6.0b1/src/aleph_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 sepal     (1000) users      (100)        1 2023-01-25 19:02:52.000000 aleph-sdk-python-0.6.0b1/src/aleph_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 sepal     (1000) users      (100)       52 2023-01-25 19:02:52.000000 aleph-sdk-python-0.6.0b1/src/aleph_sdk_python.egg-info/entry_points.txt
--rw-r--r--   0 sepal     (1000) users      (100)        1 2023-01-25 18:58:13.000000 aleph-sdk-python-0.6.0b1/src/aleph_sdk_python.egg-info/not-zip-safe
--rw-r--r--   0 sepal     (1000) users      (100)      537 2023-01-25 19:02:52.000000 aleph-sdk-python-0.6.0b1/src/aleph_sdk_python.egg-info/requires.txt
--rw-r--r--   0 sepal     (1000) users      (100)       13 2023-01-25 19:02:52.000000 aleph-sdk-python-0.6.0b1/src/aleph_sdk_python.egg-info/top_level.txt
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.333235 aleph-sdk-python-0.6.0b1/tests/
--rw-r--r--   0 sepal     (1000) users      (100)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/tests/__init__.py
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.334235 aleph-sdk-python-0.6.0b1/tests/integration/
--rw-r--r--   0 sepal     (1000) users      (100)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/tests/integration/__init__.py
--rw-r--r--   0 sepal     (1000) users      (100)      118 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/tests/integration/config.py
--rw-r--r--   0 sepal     (1000) users      (100)      585 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/integration/conftest.py
--rw-r--r--   0 sepal     (1000) users      (100)     2622 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/integration/itest_aggregates.py
--rw-r--r--   0 sepal     (1000) users      (100)     4411 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/integration/itest_forget.py
--rw-r--r--   0 sepal     (1000) users      (100)     1967 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/integration/itest_posts.py
--rw-r--r--   0 sepal     (1000) users      (100)       35 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/tests/integration/pytest.ini
--rw-r--r--   0 sepal     (1000) users      (100)      607 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/integration/toolkit.py
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.335235 aleph-sdk-python-0.6.0b1/tests/unit/
--rw-r--r--   0 sepal     (1000) users      (100)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/tests/unit/__init__.py
--rw-r--r--   0 sepal     (1000) users      (100)     1169 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/conftest.py
-drwxr-xr-x   0 sepal     (1000) users      (100)        0 2023-01-25 19:02:52.335235 aleph-sdk-python-0.6.0b1/tests/unit/test_app/
--rw-r--r--   0 sepal     (1000) users      (100)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_app/__init__.py
--rw-r--r--   0 sepal     (1000) users      (100)      294 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_app/main.py
--rw-r--r--   0 sepal     (1000) users      (100)     4835 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_asynchronous.py
--rw-r--r--   0 sepal     (1000) users      (100)     2594 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_asynchronous_get.py
--rw-r--r--   0 sepal     (1000) users      (100)     1459 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_chain_ethereum.py
--rw-r--r--   0 sepal     (1000) users      (100)     1392 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_chain_nuls1.py
--rw-r--r--   0 sepal     (1000) users      (100)     4586 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_chain_nuls1_compat.py
--rw-r--r--   0 sepal     (1000) users      (100)     2245 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_chain_solana.py
--rw-r--r--   0 sepal     (1000) users      (100)     1552 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_chain_tezos.py
--rw-r--r--   0 sepal     (1000) users      (100)        0 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_chains.py
--rw-r--r--   0 sepal     (1000) users      (100)       88 2023-01-12 10:52:43.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_init.py
--rw-r--r--   0 sepal     (1000) users      (100)     2170 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_remote_account.py
--rw-r--r--   0 sepal     (1000) users      (100)      534 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_synchronous_get.py
--rw-r--r--   0 sepal     (1000) users      (100)      599 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_utils.py
--rw-r--r--   0 sepal     (1000) users      (100)      765 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_vm_app.py
--rw-r--r--   0 sepal     (1000) users      (100)     1041 2023-01-25 18:46:39.000000 aleph-sdk-python-0.6.0b1/tests/unit/test_vm_cache.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.753700 aleph-sdk-python-0.7.0b1/
+-rw-r--r--   0 user      (1000) user      (1000)      592 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/.coveragerc
+-rw-r--r--   0 user      (1000) user      (1000)       54 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/.dockerignore
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.748700 aleph-sdk-python-0.7.0b1/.github/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.749700 aleph-sdk-python-0.7.0b1/.github/workflows/
+-rw-r--r--   0 user      (1000) user      (1000)     1657 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/.github/workflows/build-wheels.yml
+-rw-r--r--   0 user      (1000) user      (1000)     1035 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/.github/workflows/code-quality.yml
+-rw-r--r--   0 user      (1000) user      (1000)     1597 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/.github/workflows/pytest-docker.yml
+-rw-r--r--   0 user      (1000) user      (1000)      537 2023-03-02 13:32:56.000000 aleph-sdk-python-0.7.0b1/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)      159 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/AUTHORS.rst
+-rw-r--r--   0 user      (1000) user      (1000)       82 2023-01-25 17:30:47.000000 aleph-sdk-python-0.7.0b1/CHANGELOG.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1080 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1907 2023-05-16 13:19:44.753700 aleph-sdk-python-0.7.0b1/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1190 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.750700 aleph-sdk-python-0.7.0b1/docker/
+-rw-r--r--   0 user      (1000) user      (1000)     1152 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docker/python-3.10.dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)     1140 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/docker/python-3.11.dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)     1151 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docker/python-3.9.dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)     1236 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docker/ubuntu-20.04.dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)     1236 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docker/ubuntu-22.04.dockerfile
+-rw-r--r--   0 user      (1000) user      (1000)      888 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docker/with-ipfs.dockerfile
+-rwxr-xr-x   0 user      (1000) user      (1000)      346 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docker/with-ipfs.entrypoint.sh
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.750700 aleph-sdk-python-0.7.0b1/docs/
+-rw-r--r--   0 user      (1000) user      (1000)     7622 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docs/Makefile
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.750700 aleph-sdk-python-0.7.0b1/docs/_static/
+-rw-r--r--   0 user      (1000) user      (1000)       18 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/_static/.gitignore
+-rw-r--r--   0 user      (1000) user      (1000)     2774 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/_static/logo.svg
+-rw-r--r--   0 user      (1000) user      (1000)       41 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/authors.rst
+-rw-r--r--   0 user      (1000) user      (1000)       43 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/changelog.rst
+-rw-r--r--   0 user      (1000) user      (1000)     9768 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docs/conf.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.751700 aleph-sdk-python-0.7.0b1/docs/content/
+-rw-r--r--   0 user      (1000) user      (1000)     3241 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/account.rst
+-rw-r--r--   0 user      (1000) user      (1000)     2347 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/aggregates.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1543 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/async_notes.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1924 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/cli.rst
+-rw-r--r--   0 user      (1000) user      (1000)     2604 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/content/introduction.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1402 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/posts.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1159 2023-03-02 14:17:37.000000 aleph-sdk-python-0.7.0b1/docs/content/programs.rst
+-rw-r--r--   0 user      (1000) user      (1000)     1482 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/docs/index.rst
+-rw-r--r--   0 user      (1000) user      (1000)       67 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/docs/license.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.751700 aleph-sdk-python-0.7.0b1/examples/
+-rw-r--r--   0 user      (1000) user      (1000)     2004 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/examples/httpgateway.py
+-rw-r--r--   0 user      (1000) user      (1000)     1911 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/examples/metrics.py
+-rw-r--r--   0 user      (1000) user      (1000)     4075 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/examples/mqtt.py
+-rw-r--r--   0 user      (1000) user      (1000)     3391 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/examples/store.py
+-rw-r--r--   0 user      (1000) user      (1000)     2467 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/mypy.ini
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.751700 aleph-sdk-python-0.7.0b1/scripts/
+-rw-r--r--   0 user      (1000) user      (1000)      322 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/scripts/build-and-shell.sh
+-rw-r--r--   0 user      (1000) user      (1000)      457 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/scripts/build-and-test.sh
+-rw-r--r--   0 user      (1000) user      (1000)      419 2023-05-16 13:01:37.000000 aleph-sdk-python-0.7.0b1/scripts/build-to-publish.sh
+-rw-r--r--   0 user      (1000) user      (1000)     2130 2023-05-16 13:19:44.759700 aleph-sdk-python-0.7.0b1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      572 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.749700 aleph-sdk-python-0.7.0b1/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.751700 aleph-sdk-python-0.7.0b1/src/aleph/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.751700 aleph-sdk-python-0.7.0b1/src/aleph/sdk/
+-rw-r--r--   0 user      (1000) user      (1000)      472 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2177 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/account.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.752700 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3757 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/common.py
+-rw-r--r--   0 user      (1000) user      (1000)     2583 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/cosmos.py
+-rw-r--r--   0 user      (1000) user      (1000)     2653 2023-05-16 11:57:28.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/ethereum.py
+-rw-r--r--   0 user      (1000) user      (1000)     9356 2023-05-16 10:29:19.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/nuls1.py
+-rw-r--r--   0 user      (1000) user      (1000)     1958 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/nuls2.py
+-rw-r--r--   0 user      (1000) user      (1000)     2351 2023-05-16 11:57:28.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/remote.py
+-rw-r--r--   0 user      (1000) user      (1000)     2849 2023-05-16 11:57:28.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/sol.py
+-rw-r--r--   0 user      (1000) user      (1000)     1474 2023-05-16 11:57:28.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/substrate.py
+-rw-r--r--   0 user      (1000) user      (1000)     2345 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/tezos.py
+-rw-r--r--   0 user      (1000) user      (1000)    51023 2023-05-16 12:59:50.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/client.py
+-rw-r--r--   0 user      (1000) user      (1000)     1794 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/conf.py
+-rw-r--r--   0 user      (1000) user      (1000)      753 2023-05-16 10:28:27.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/exceptions.py
+-rw-r--r--   0 user      (1000) user      (1000)      354 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/models.py
+-rw-r--r--   0 user      (1000) user      (1000)      893 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/types.py
+-rw-r--r--   0 user      (1000) user      (1000)     2680 2023-05-16 12:59:50.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.752700 aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/
+-rw-r--r--   0 user      (1000) user      (1000)       70 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2645 2023-05-16 10:28:43.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/app.py
+-rw-r--r--   0 user      (1000) user      (1000)     4093 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/cache.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.752700 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1907 2023-05-16 13:19:44.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2587 2023-05-16 13:19:44.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-16 13:19:44.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-01-25 18:58:13.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/not-zip-safe
+-rw-r--r--   0 user      (1000) user      (1000)      699 2023-05-16 13:19:44.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        6 2023-05-16 13:19:44.000000 aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.752700 aleph-sdk-python-0.7.0b1/tests/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.752700 aleph-sdk-python-0.7.0b1/tests/integration/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/integration/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      118 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/integration/config.py
+-rw-r--r--   0 user      (1000) user      (1000)      579 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/integration/conftest.py
+-rw-r--r--   0 user      (1000) user      (1000)     2610 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/integration/itest_aggregates.py
+-rw-r--r--   0 user      (1000) user      (1000)     4399 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/integration/itest_forget.py
+-rw-r--r--   0 user      (1000) user      (1000)     1958 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/integration/itest_posts.py
+-rw-r--r--   0 user      (1000) user      (1000)       35 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/integration/pytest.ini
+-rw-r--r--   0 user      (1000) user      (1000)      607 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/integration/toolkit.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.753700 aleph-sdk-python-0.7.0b1/tests/unit/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/unit/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1157 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/conftest.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-16 13:19:44.753700 aleph-sdk-python-0.7.0b1/tests/unit/test_app/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-01-12 10:52:43.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_app/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      291 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_app/main.py
+-rw-r--r--   0 user      (1000) user      (1000)     4891 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_asynchronous.py
+-rw-r--r--   0 user      (1000) user      (1000)     2564 2023-05-16 12:21:38.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_asynchronous_get.py
+-rw-r--r--   0 user      (1000) user      (1000)     2582 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chain_ethereum.py
+-rw-r--r--   0 user      (1000) user      (1000)     1389 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chain_nuls1.py
+-rw-r--r--   0 user      (1000) user      (1000)     4580 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chain_nuls1_compat.py
+-rw-r--r--   0 user      (1000) user      (1000)     3286 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chain_solana.py
+-rw-r--r--   0 user      (1000) user      (1000)     2167 2023-05-16 10:25:16.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chain_tezos.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_chains.py
+-rw-r--r--   0 user      (1000) user      (1000)       85 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_init.py
+-rw-r--r--   0 user      (1000) user      (1000)     2164 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_remote_account.py
+-rw-r--r--   0 user      (1000) user      (1000)      522 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_synchronous_get.py
+-rw-r--r--   0 user      (1000) user      (1000)      596 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)      765 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_vm_app.py
+-rw-r--r--   0 user      (1000) user      (1000)     1034 2023-05-12 17:34:52.000000 aleph-sdk-python-0.7.0b1/tests/unit/test_vm_cache.py
```

### Comparing `aleph-sdk-python-0.6.0b1/.coveragerc` & `aleph-sdk-python-0.7.0b1/.coveragerc`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # .coveragerc to control coverage.py
 [run]
 branch = True
-source = aleph_client
+source = aleph.sdk
 # omit = bad_file.py
 
 [paths]
 source =
     src/
     */site-packages/
```

### Comparing `aleph-sdk-python-0.6.0b1/.github/workflows/code-quality.yml` & `aleph-sdk-python-0.7.0b1/.github/workflows/code-quality.yml`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 jobs:
   code-quality:
     runs-on: ubuntu-22.04
 
     steps:
       - uses: actions/checkout@v3
 
+      - name: Workaround github issue https://github.com/actions/runner-images/issues/7192
+        run: sudo echo RESET grub-efi/install_devices | sudo debconf-communicate grub-pc
+
       - name: Install required system packages only for Ubuntu Linux
         run: |
           sudo apt-get update
           sudo apt-get -y upgrade
           sudo apt-get install -y libsecp256k1-dev
 
       - name: Install required Python packages
```

### Comparing `aleph-sdk-python-0.6.0b1/.github/workflows/pytest-docker.yml` & `aleph-sdk-python-0.7.0b1/.github/workflows/pytest-docker.yml`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     branches:
       - main
 
 jobs:
   build:
     strategy:
       matrix:
-        image: [ "python-3.9", "python-3.10", "ubuntu-20.04", "ubuntu-22.04" ]
+        image: [ "python-3.9", "python-3.10", "python-3.11", "ubuntu-20.04", "ubuntu-22.04" ]
     runs-on: ubuntu-22.04
 
     steps:
       - uses: actions/checkout@v3
 
       # Use GitHub's Docker registry to cache intermediate layers
       - run: echo ${{ secrets.GITHUB_TOKEN }} | docker login docker.pkg.github.com -u $GITHUB_ACTOR --password-stdin
```

### Comparing `aleph-sdk-python-0.6.0b1/.gitignore` & `aleph-sdk-python-0.7.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/LICENSE.txt` & `aleph-sdk-python-0.7.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/README.md` & `aleph-sdk-python-0.7.0b1/README.md`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/docker/python-3.10.dockerfile` & `aleph-sdk-python-0.7.0b1/docker/python-3.9.dockerfile`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.10-bullseye
+FROM python:3.9-bullseye
 MAINTAINER The aleph.im project
 
 RUN apt-get update && apt-get -y upgrade && apt-get install -y \
      libsecp256k1-dev \
      && rm -rf /var/lib/apt/lists/*
 
 RUN useradd -s /bin/bash --create-home user
@@ -16,22 +16,23 @@
 ENV PATH="/opt/venv/bin:$PATH"
 ENV PATH="/opt/venv/bin:$PATH"
 
 RUN pip install --upgrade pip wheel twine
 
 # Preinstall dependencies for faster steps
 RUN pip install --upgrade secp256k1 coincurve aiohttp eciespy python-magic typer
-RUN pip install --upgrade 'aleph-message~=0.3.0' eth_account pynacl base58
+RUN pip install --upgrade 'aleph-message~=0.3.1' eth_account pynacl base58
 RUN pip install --upgrade pytest pytest-cov pytest-asyncio mypy types-setuptools pytest-asyncio fastapi httpx requests
 
 WORKDIR /opt/aleph-sdk-python/
 COPY . .
 USER root
 RUN chown -R user:user /opt/aleph-sdk-python
 
+RUN git config --global --add safe.directory /opt/aleph-sdk-python
 RUN pip install -e .[testing,ethereum,solana,tezos]
 
 RUN mkdir /data
 RUN chown user:user /data
 ENV ALEPH_PRIVATE_KEY_FILE=/data/secret.key
 
 WORKDIR /home/user
```

### Comparing `aleph-sdk-python-0.6.0b1/docker/python-3.11.dockerfile` & `aleph-sdk-python-0.7.0b1/docker/ubuntu-20.04.dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-FROM python:3.11-bullseye
+FROM ubuntu:20.04
 MAINTAINER The aleph.im project
 
 RUN apt-get update && apt-get -y upgrade && apt-get install -y \
      libsecp256k1-dev \
+     python3-dev \
+     python3-venv \
+     git \
+     build-essential \
+     libgmp3-dev \
      && rm -rf /var/lib/apt/lists/*
 
 RUN useradd -s /bin/bash --create-home user
 RUN mkdir /opt/venv
 RUN mkdir /opt/aleph-sdk-python/
 RUN chown user:user /opt/venv
 RUN chown user:user /opt/aleph-sdk-python
@@ -16,22 +21,23 @@
 ENV PATH="/opt/venv/bin:$PATH"
 ENV PATH="/opt/venv/bin:$PATH"
 
 RUN pip install --upgrade pip wheel twine
 
 # Preinstall dependencies for faster steps
 RUN pip install --upgrade secp256k1 coincurve aiohttp eciespy python-magic typer
-RUN pip install --upgrade 'aleph-message~=0.3.0' eth_account pynacl base58
+RUN pip install --upgrade 'aleph-message~=0.3.1' eth_account pynacl base58
 RUN pip install --upgrade pytest pytest-cov pytest-asyncio mypy types-setuptools pytest-asyncio fastapi httpx requests
 
 WORKDIR /opt/aleph-sdk-python/
 COPY . .
 USER root
 RUN chown -R user:user /opt/aleph-sdk-python
 
+RUN git config --global --add safe.directory /opt/aleph-sdk-python
 RUN pip install -e .[testing,ethereum,solana,tezos]
 
 RUN mkdir /data
 RUN chown user:user /data
 ENV ALEPH_PRIVATE_KEY_FILE=/data/secret.key
 
 WORKDIR /home/user
```

### Comparing `aleph-sdk-python-0.6.0b1/docker/python-3.9.dockerfile` & `aleph-sdk-python-0.7.0b1/docker/python-3.11.dockerfile`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.9-bullseye
+FROM python:3.11-bullseye
 MAINTAINER The aleph.im project
 
 RUN apt-get update && apt-get -y upgrade && apt-get install -y \
      libsecp256k1-dev \
      && rm -rf /var/lib/apt/lists/*
 
 RUN useradd -s /bin/bash --create-home user
@@ -16,22 +16,23 @@
 ENV PATH="/opt/venv/bin:$PATH"
 ENV PATH="/opt/venv/bin:$PATH"
 
 RUN pip install --upgrade pip wheel twine
 
 # Preinstall dependencies for faster steps
 RUN pip install --upgrade secp256k1 coincurve aiohttp eciespy python-magic typer
-RUN pip install --upgrade 'aleph-message~=0.3.0' eth_account pynacl base58
+RUN pip install --upgrade 'aleph-message~=0.3.1' pynacl base58
 RUN pip install --upgrade pytest pytest-cov pytest-asyncio mypy types-setuptools pytest-asyncio fastapi httpx requests
 
 WORKDIR /opt/aleph-sdk-python/
 COPY . .
 USER root
 RUN chown -R user:user /opt/aleph-sdk-python
 
+RUN git config --global --add safe.directory /opt/aleph-sdk-python
 RUN pip install -e .[testing,ethereum,solana,tezos]
 
 RUN mkdir /data
 RUN chown user:user /data
 ENV ALEPH_PRIVATE_KEY_FILE=/data/secret.key
 
 WORKDIR /home/user
```

### Comparing `aleph-sdk-python-0.6.0b1/docker/ubuntu-20.04.dockerfile` & `aleph-sdk-python-0.7.0b1/docker/ubuntu-22.04.dockerfile`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM ubuntu:20.04
+FROM ubuntu:22.04
 MAINTAINER The aleph.im project
 
 RUN apt-get update && apt-get -y upgrade && apt-get install -y \
      libsecp256k1-dev \
      python3-dev \
      python3-venv \
      git \
@@ -21,15 +21,15 @@
 ENV PATH="/opt/venv/bin:$PATH"
 ENV PATH="/opt/venv/bin:$PATH"
 
 RUN pip install --upgrade pip wheel twine
 
 # Preinstall dependencies for faster steps
 RUN pip install --upgrade secp256k1 coincurve aiohttp eciespy python-magic typer
-RUN pip install --upgrade 'aleph-message~=0.3.0' eth_account pynacl base58
+RUN pip install --upgrade 'aleph-message~=0.3.1' eth_account pynacl base58
 RUN pip install --upgrade pytest pytest-cov pytest-asyncio mypy types-setuptools pytest-asyncio fastapi httpx requests
 
 WORKDIR /opt/aleph-sdk-python/
 COPY . .
 USER root
 RUN chown -R user:user /opt/aleph-sdk-python
```

### Comparing `aleph-sdk-python-0.6.0b1/docker/with-ipfs.dockerfile` & `aleph-sdk-python-0.7.0b1/docker/with-ipfs.dockerfile`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/docs/Makefile` & `aleph-sdk-python-0.7.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/docs/_static/logo.svg` & `aleph-sdk-python-0.7.0b1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/docs/conf.py` & `aleph-sdk-python-0.7.0b1/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import os
-import sys
 import inspect
+import os
 import shutil
+import sys
 
-__location__ = os.path.join(os.getcwd(), os.path.dirname(
-    inspect.getfile(inspect.currentframe())))
+__location__ = os.path.join(
+    os.getcwd(), os.path.dirname(inspect.getfile(inspect.currentframe()))
+)
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-sys.path.insert(0, os.path.join(__location__, '../src'))
+sys.path.insert(0, os.path.join(__location__, "../src"))
 
 # -- Run sphinx-apidoc ------------------------------------------------------
 # This hack is necessary since RTD does not issue `sphinx-apidoc` before running
 # `sphinx-build -b html . _build/html`. See Issue:
 # https://github.com/rtfd/readthedocs.org/issues/1139
 # DON'T FORGET: Check the box "Install your project inside a virtualenv using
 # setup.py install" in the RTD Advanced Settings.
@@ -45,73 +46,82 @@
     import sphinx
     from pkg_resources import parse_version
 
     cmd_line_template = "sphinx-apidoc -f -o {outputdir} {moduledir}"
     cmd_line = cmd_line_template.format(outputdir=output_dir, moduledir=module_dir)
 
     args = cmd_line.split(" ")
-    if parse_version(sphinx.__version__) >= parse_version('1.7'):
+    if parse_version(sphinx.__version__) >= parse_version("1.7"):
         args = args[1:]
 
     apidoc.main(args)
 except Exception as e:
     print("Running `sphinx-apidoc` failed!\n{}".format(e))
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.intersphinx', 'sphinx.ext.todo',
-              'sphinx.ext.autosummary', 'sphinx.ext.viewcode', 'sphinx.ext.coverage',
-              'sphinx.ext.doctest', 'sphinx.ext.ifconfig', 'sphinx.ext.mathjax',
-              'sphinx.ext.napoleon', 'sphinxcontrib.plantuml']
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinx.ext.intersphinx",
+    "sphinx.ext.todo",
+    "sphinx.ext.autosummary",
+    "sphinx.ext.viewcode",
+    "sphinx.ext.coverage",
+    "sphinx.ext.doctest",
+    "sphinx.ext.ifconfig",
+    "sphinx.ext.mathjax",
+    "sphinx.ext.napoleon",
+    "sphinxcontrib.plantuml",
+]
 
 # plantuml = 'java -jar docs/plantuml.jar'
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = u'aleph-sdk-python'
-copyright = u'2019, Aleph.im'
+project = "aleph-sdk-python"
+copyright = "2019, Aleph.im"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = ''  # Is set by calling `setup.py docs`
+version = ""  # Is set by calling `setup.py docs`
 # The full version, including alpha/beta/rc tags.
-release = ''  # Is set by calling `setup.py docs`
+release = ""  # Is set by calling `setup.py docs`
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
 # today = ''
 # Else, today_fmt is used as the format for a strftime call.
 # today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ["_build"]
 
 # The reST default role (used for this markup: `text`) to use for all documents.
 # default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 # add_function_parentheses = True
 
@@ -120,51 +130,51 @@
 # add_module_names = True
 
 # If true, sectionauthor and moduleauthor directives will be shown in the
 # output. They are ignored by default.
 # show_authors = False
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # A list of ignored prefixes for module index sorting.
 # modindex_common_prefix = []
 
 # If true, keep warnings as "system message" paragraphs in the built documents.
 # keep_warnings = False
 
 
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 html_theme_options = {
     #'sidebar_width': '300px',
     #'page_width': '1200px'
-    'logo': 'logo.svg',
-    'description': 'Aleph Network Client',
-    'github_user': 'aleph-im',
-    'github_repo': 'aleph-sdk-python',
-    'github_button': True,
-    'github_type': 'star',
-    'github_banner': True,
-    'travis_button': True,
-    'codecov_button': True,
-    'pre_bg': '#FFF6E5',
-    'note_bg': '#E5ECD1',
-    'note_border': '#BFCF8C',
-    'body_text': '#482C0A',
-    'sidebar_text': '#49443E',
-    'sidebar_header': '#4B4032',
-    'sidebar_collapse': False,
+    "logo": "logo.svg",
+    "description": "Aleph Network Client",
+    "github_user": "aleph-im",
+    "github_repo": "aleph-sdk-python",
+    "github_button": True,
+    "github_type": "star",
+    "github_banner": True,
+    "travis_button": True,
+    "codecov_button": True,
+    "pre_bg": "#FFF6E5",
+    "note_bg": "#E5ECD1",
+    "note_border": "#BFCF8C",
+    "body_text": "#482C0A",
+    "sidebar_text": "#49443E",
+    "sidebar_header": "#4B4032",
+    "sidebar_collapse": False,
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
@@ -186,15 +196,15 @@
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 # html_favicon = None
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 # If not '', a 'Last updated on:' timestamp is inserted at every page bottom,
 # using the given strftime format.
 # html_last_updated_fmt = '%b %d, %Y'
 
 # If true, SmartyPants will be used to convert quotes and dashes to
 # typographically correct entities.
@@ -230,35 +240,32 @@
 # base URL from which the finished HTML is served.
 # html_use_opensearch = ''
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 # html_file_suffix = None
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'aleph_client-doc'
+htmlhelp_basename = "aleph_client-doc"
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
 latex_elements = {
-# The paper size ('letterpaper' or 'a4paper').
-# 'papersize': 'letterpaper',
-
-# The font size ('10pt', '11pt' or '12pt').
-# 'pointsize': '10pt',
-
-# Additional stuff for the LaTeX preamble.
-# 'preamble': '',
+    # The paper size ('letterpaper' or 'a4paper').
+    # 'papersize': 'letterpaper',
+    # The font size ('10pt', '11pt' or '12pt').
+    # 'pointsize': '10pt',
+    # Additional stuff for the LaTeX preamble.
+    # 'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'user_guide.tex', u'aleph-sdk-python Documentation',
-   u'Aleph.im', 'manual'),
+    ("index", "user_guide.tex", "aleph-sdk-python Documentation", "Aleph.im", "manual"),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = ""
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -274,17 +281,17 @@
 # Documents to append as an appendix to all manuals.
 # latex_appendices = []
 
 # If false, no module index is generated.
 # latex_domain_indices = True
 
 # -- External mapping ------------------------------------------------------------
-python_version = '.'.join(map(str, sys.version_info[0:2]))
+python_version = ".".join(map(str, sys.version_info[0:2]))
 intersphinx_mapping = {
-    'sphinx': ('http://www.sphinx-doc.org/en/stable', None),
-    'python': ('https://docs.python.org/' + python_version, None),
-    'matplotlib': ('https://matplotlib.org', None),
-    'numpy': ('https://docs.scipy.org/doc/numpy', None),
-    'sklearn': ('http://scikit-learn.org/stable', None),
-    'pandas': ('http://pandas.pydata.org/pandas-docs/stable', None),
-    'scipy': ('https://docs.scipy.org/doc/scipy/reference', None),
+    "sphinx": ("http://www.sphinx-doc.org/en/stable", None),
+    "python": ("https://docs.python.org/" + python_version, None),
+    "matplotlib": ("https://matplotlib.org", None),
+    "numpy": ("https://docs.scipy.org/doc/numpy", None),
+    "sklearn": ("http://scikit-learn.org/stable", None),
+    "pandas": ("http://pandas.pydata.org/pandas-docs/stable", None),
+    "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
 }
```

### Comparing `aleph-sdk-python-0.6.0b1/docs/content/account.rst` & `aleph-sdk-python-0.7.0b1/docs/content/account.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/docs/content/aggregates.rst` & `aleph-sdk-python-0.7.0b1/docs/content/aggregates.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/docs/content/async_notes.rst` & `aleph-sdk-python-0.7.0b1/docs/content/async_notes.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/docs/content/cli.rst` & `aleph-sdk-python-0.7.0b1/docs/content/cli.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/docs/content/introduction.rst` & `aleph-sdk-python-0.7.0b1/docs/content/introduction.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/docs/content/posts.rst` & `aleph-sdk-python-0.7.0b1/docs/content/posts.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/docs/content/programs.rst` & `aleph-sdk-python-0.7.0b1/docs/content/programs.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/docs/index.rst` & `aleph-sdk-python-0.7.0b1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/examples/httpgateway.py` & `aleph-sdk-python-0.7.0b1/examples/httpgateway.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """ Server metrics upload.
 """
 # -*- coding: utf-8 -*-
 
 import click
 from aiohttp import web
 
-from aleph_client.chains.common import get_fallback_private_key
-from aleph_client.chains.ethereum import ETHAccount
-from aleph_client.user_session import AuthenticatedUserSession
+from aleph.sdk.chains.common import get_fallback_private_key
+from aleph.sdk.chains.ethereum import ETHAccount
+from aleph.sdk.client import AuthenticatedAlephClient
 
 app = web.Application()
 routes = web.RouteTableDef()
 
 
 @routes.get("/")
 async def hello(request):
@@ -28,15 +28,15 @@
     data["source"] = request.match_info["source"]
 
     if app["secret"] is not None:
         if secret != app["secret"]:
             return web.json_response(
                 {"status": "error", "message": "unauthorized secret"}
             )
-    async with AuthenticatedUserSession(
+    async with AuthenticatedAlephClient(
         account=app["account"], api_server="https://api2.aleph.im"
     ) as session:
         message, _status = await session.create_post(
             post_content=data,
             post_type="event",
             channel=app["channel"],
         )
```

### Comparing `aleph-sdk-python-0.6.0b1/examples/metrics.py` & `aleph-sdk-python-0.7.0b1/examples/metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 import os
 import platform
 import time
 from typing import Tuple
 
 import psutil
 from aleph_message.models import AlephMessage
+from aleph_message.status import MessageStatus
 
-from aleph_client import AuthenticatedUserSession
-from aleph_client.chains.ethereum import get_fallback_account
-from aleph_client.conf import settings
-from aleph_client.types import MessageStatus
-from aleph_client.user_session import AuthenticatedUserSessionSync
+from aleph.sdk.chains.ethereum import get_fallback_account
+from aleph.sdk.client import AuthenticatedAlephClient, AuthenticatedUserSessionSync
+from aleph.sdk.conf import settings
 
 
 def get_sysinfo():
     uptime = int(time.time() - psutil.boot_time())
     sysinfo = {
         "uptime": uptime,
         "os": platform.platform(),
@@ -67,15 +66,15 @@
         "cpu": get_cpu(),
         "cpu_cores": get_cpu_cores(),
     }
 
 
 def main():
     account = get_fallback_account()
-    with AuthenticatedUserSession(
+    with AuthenticatedAlephClient(
         account=account, api_server=settings.API_HOST
     ) as session:
         while True:
             metrics = collect_metrics()
             message, status = send_metrics(session, metrics)
             print("sent", message.item_hash)
             time.sleep(10)
```

### Comparing `aleph-sdk-python-0.6.0b1/examples/mqtt.py` & `aleph-sdk-python-0.7.0b1/examples/mqtt.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 import asyncio
 from typing import Dict
 
 import aiomqtt
 import click
 
-from aleph_client import AuthenticatedUserSession
-from aleph_client.chains.common import get_fallback_private_key
-from aleph_client.chains.ethereum import ETHAccount
-from aleph_client.conf import settings
+from aleph.sdk.chains.common import get_fallback_private_key
+from aleph.sdk.chains.ethereum import ETHAccount
+from aleph.sdk.client import AuthenticatedAlephClient
+from aleph.sdk.conf import settings
 
 
 def get_input_data(value):
     if value == b"true":
         return True
     elif value == b"false":
         return False
@@ -23,15 +23,15 @@
         v = float(value)
         return v
     except ValueError:
         return value.decode("utf-8")
 
 
 def send_metrics(account, metrics):
-    with AuthenticatedUserSession(
+    with AuthenticatedAlephClient(
         account=account, api_server=settings.API_HOST
     ) as session:
         return session.create_aggregate(
             key="metrics", content=metrics, channel="SYSINFO"
         )
 
 
@@ -72,15 +72,14 @@
     port=1883,
     ca_cert=None,
     pkey=None,
     keepalive=10,
     transport="tcp",
     auth=None,
 ):
-
     if pkey is None:
         pkey = get_fallback_private_key()
 
     account = ETHAccount(private_key=pkey)
     state: Dict = dict()
     userdata = {"account": account, "state": state, "received": False}
     client = aiomqtt.Client(loop, userdata=userdata, transport=transport)
@@ -97,15 +96,15 @@
 
     await client.connect(host, port, keepalive)
     while True:
         await asyncio.sleep(10)
         if not userdata["received"]:
             await client.reconnect()
 
-        async with AuthenticatedUserSession(
+        async with AuthenticatedAlephClient(
             account=account, api_server=settings.API_HOST
         ) as session:
             for key, value in state.items():
                 message, status = await session.create_aggregate(
                     key=key, content=value, channel="IOT_TEST"
                 )
                 print("sent", message.item_hash)
```

### Comparing `aleph-sdk-python-0.6.0b1/examples/store.py` & `aleph-sdk-python-0.7.0b1/examples/store.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
 
 import click
 from aleph_message.models import StoreMessage
+from aleph_message.status import MessageStatus
 
-from aleph_client.chains.common import get_fallback_private_key
-from aleph_client.chains.ethereum import ETHAccount
-from aleph_client.conf import settings
-from aleph_client.types import MessageStatus
-from aleph_client.user_session import AuthenticatedUserSession
+from aleph.sdk.chains.common import get_fallback_private_key
+from aleph.sdk.chains.ethereum import ETHAccount
+from aleph.sdk.client import AuthenticatedAlephClient
+from aleph.sdk.conf import settings
 
 DEFAULT_SERVER = "https://api2.aleph.im"
 
 
 async def print_output_hash(message: StoreMessage, status: MessageStatus):
     print("Successfully created STORE message")
     print(f"File hash ({message.content.item_type}): {message.content.item_hash}")
@@ -19,15 +19,15 @@
     print(f"Message hash: {message.item_hash}")
     print(
         f"Explorer URL: https://explorer.aleph.im/address/{message.chain.value}/{message.sender}/message/{message.item_hash}"
     )
 
 
 async def do_upload(account, engine, channel, filename=None, file_hash=None):
-    async with AuthenticatedUserSession(
+    async with AuthenticatedAlephClient(
         account=account, api_server=settings.API_HOST
     ) as session:
         print(filename, account.get_address())
         if filename:
             try:
                 with open(filename, "rb") as f:
                     # Do something with the file
```

### Comparing `aleph-sdk-python-0.6.0b1/mypy.ini` & `aleph-sdk-python-0.7.0b1/mypy.ini`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/setup.cfg` & `aleph-sdk-python-0.7.0b1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = aleph-sdk-python
 description = Lightweight Python Client library for the Aleph.im network
 author = Aleph.im Team
 author_email = hello@aleph.im
 license = mit
-long_description = file: README.rst
-long_description_content_type = text/x-rst; charset=UTF-8
+long_description = file: README.md
+long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/aleph-im/aleph-sdk-python
 project_urls = 
 	Documentation = https://aleph.im/
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3
@@ -18,21 +18,24 @@
 zip_safe = False
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
-	coincurve
+	coincurve; python_version<"3.11"
+	coincurve>=17.0.0; python_version>="3.11"   # Technically, this should be >=18.0.0 but there is a conflict with eciespy
 	aiohttp>=3.8.3
-	eciespy
+	eciespy; python_version<"3.11"
+	eciespy>=0.3.13; python_version>="3.11"
 	typing_extensions
 	typer
-	aleph-message~=0.3.0
+	aleph-message~=0.3.2
 	eth_account>=0.4.0
+	eth_abi==4.0.0b2; python_version>="3.11"
 	python-magic
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
@@ -47,51 +50,50 @@
 	mypy
 	secp256k1
 	pynacl
 	base58
 	fastapi
 	httpx
 	requests
-	aleph-pytezos==0.1.0
+	aleph-pytezos==0.1.1
 	types-certifi
 	types-setuptools
 	black
 	isort
 	flake8
 mqtt = 
 	aiomqtt
 	certifi
 	Click
 nuls2 = 
 	nuls2-python
 ethereum = 
 	eth_account>=0.4.0
+	eth_abi==4.0.0b2; python_version>="3.11"
 polkadot = 
 	substrate-interface==1.3.4
 cosmos = 
 	cosmospy
 solana = 
 	pynacl
 	base58
 tezos = 
 	pynacl
-	aleph-pytezos==0.1.0
+	aleph-pytezos==0.1.1
 docs = 
 	sphinxcontrib-plantuml
 
 [options.entry_points]
-console_scripts = 
-	aleph = aleph_client.__main__:app
 
 [test]
 extras = True
 
 [tool:pytest]
 addopts = 
-	--cov aleph_client --cov-report term-missing
+	--cov aleph.sdk --cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
 	build
 	.tox
 testpaths = tests
 
@@ -119,13 +121,13 @@
 ignore = E501 W291 W503 E203
 
 [isort]
 profile = black
 
 [pyscaffold]
 version = 3.2.1
-package = aleph_client
+package = aleph.sdk
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `aleph-sdk-python-0.6.0b1/setup.py` & `aleph-sdk-python-0.7.0b1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 """
-    Setup file for aleph_client.
+    Setup file for aleph.sdk
     Use setup.cfg to configure your project.
 
     This file was generated with PyScaffold 3.2.1.
     PyScaffold helps you to put up the scaffold of your new Python project.
     Learn more under: https://pyscaffold.org/
 """
 import sys
 
 from pkg_resources import VersionConflict, require
 from setuptools import setup
 
 try:
-    require('setuptools>=38.3')
+    require("setuptools>=38.3")
 except VersionConflict:
     print("Error: version of setuptools is too old (<38.3)!")
     sys.exit(1)
 
 
 if __name__ == "__main__":
     setup(use_pyscaffold=True)
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/account.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/account.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import asyncio
 import logging
 from pathlib import Path
 from typing import Optional, Type, TypeVar
 
-from aleph_client.chains.common import get_fallback_private_key
-from aleph_client.chains.ethereum import ETHAccount
-from aleph_client.chains.remote import RemoteAccount
-from aleph_client.conf import settings
-from aleph_client.types import AccountFromPrivateKey
+from aleph.sdk.chains.common import get_fallback_private_key
+from aleph.sdk.chains.ethereum import ETHAccount
+from aleph.sdk.chains.remote import RemoteAccount
+from aleph.sdk.conf import settings
+from aleph.sdk.types import AccountFromPrivateKey
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T", bound=AccountFromPrivateKey)
 
 
 def account_from_hex_string(private_key_str: str, account_type: Type[T]) -> T:
     if private_key_str.startswith("0x"):
         private_key_str = private_key_str[2:]
     return account_type(bytes.fromhex(private_key_str))
 
 
 def account_from_file(private_key_path: Path, account_type: Type[T]) -> T:
-    with open(private_key_path, "rb") as pk_fd:
-        private_key: bytes = pk_fd.read()
+    private_key = private_key_path.read_bytes()
     return account_type(private_key)
 
 
 def _load_account(
     private_key_str: Optional[str] = None,
     private_key_path: Optional[Path] = None,
     account_type: Type[AccountFromPrivateKey] = ETHAccount,
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/chains/common.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,27 @@
-import os
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Dict, Optional
 
 from coincurve.keys import PrivateKey
 from ecies import decrypt, encrypt
 
-from aleph_client.conf import settings
+from aleph.sdk.conf import settings
 
 
-def get_verification_buffer(message):
-    """Returns a serialized string to verify the message integrity
-    (this is was it signed)
+def get_verification_buffer(message: Dict) -> bytes:
+    """
+    Returns the verification buffer that Aleph nodes use to verify the signature of a message.
+    Note:
+        The verification buffer is a string of the following format:
+        b"{chain}\\n{sender}\\n{type}\\n{item_hash}"
+    Args:
+        message: Message to get the verification buffer for
+    Returns:
+        bytes: Verification buffer
     """
     return "{chain}\n{sender}\n{type}\n{item_hash}".format(**message).encode("utf-8")
 
 
 def get_public_key(private_key):
     privkey = PrivateKey(private_key)
     return privkey.public_key.format()
@@ -23,45 +29,77 @@
 
 class BaseAccount(ABC):
     CHAIN: str
     CURVE: str
     private_key: bytes
 
     def _setup_sender(self, message: Dict) -> Dict:
-        """Set the sender of the message as the account's public key.
+        """
+        Set the sender of the message as the account's public key.
         If a sender is already specified, check that it matches the account's public key.
+        Args:
+            message: Message to add the sender to
+        Returns:
+            Dict: Message with the sender set
         """
         if not message.get("sender"):
             message["sender"] = self.get_address()
             return message
         elif message["sender"] == self.get_address():
             return message
         else:
             raise ValueError("Message sender does not match the account's public key.")
 
     @abstractmethod
     async def sign_message(self, message: Dict) -> Dict:
+        """
+        Returns a signed message from an Aleph message.
+        Args:
+            message: Message to sign
+        Returns:
+            Dict: Signed message
+        """
         raise NotImplementedError
 
     @abstractmethod
     def get_address(self) -> str:
+        """
+        Returns the account's displayed address.
+        """
         raise NotImplementedError
 
     @abstractmethod
     def get_public_key(self) -> str:
+        """
+        Returns the account's public key.
+        """
         raise NotImplementedError
 
-    async def encrypt(self, content) -> bytes:
+    async def encrypt(self, content: bytes) -> bytes:
+        """
+        Encrypts a message using the account's public key.
+        Args:
+            content: Content bytes to encrypt
+        Returns:
+            bytes: Encrypted content as bytes
+        """
         if self.CURVE == "secp256k1":
             value: bytes = encrypt(self.get_public_key(), content)
             return value
         else:
             raise NotImplementedError
 
-    async def decrypt(self, content) -> bytes:
+    async def decrypt(self, content: bytes) -> bytes:
+        """
+        Decrypts a message using the account's private key.
+        Args:
+            content: Content bytes to decrypt
+        Returns:
+            bytes: Decrypted content as bytes
+        """
         if self.CURVE == "secp256k1":
             value: bytes = decrypt(self.private_key, content)
             return value
         else:
             raise NotImplementedError
 
 
@@ -71,23 +109,18 @@
     return privkey.secret
 
 
 def get_fallback_private_key(path: Optional[Path] = None) -> bytes:
     path = path or settings.PRIVATE_KEY_FILE
     private_key: bytes
     if path.exists() and path.stat().st_size > 0:
-        with open(path, "rb") as prvfile:
-            private_key = prvfile.read()
+        private_key = path.read_bytes()
     else:
         private_key = generate_key()
-        os.makedirs(path.parent, exist_ok=True)
-        with open(path, "wb") as prvfile:
-            prvfile.write(private_key)
-
-        with open(path, "rb") as prvfile:
-            print(prvfile.read())
+        path.parent.mkdir(exist_ok=True, parents=True)
+        path.write_bytes(private_key)
 
         default_key_path = path.parent / "default.key"
-        if not default_key_path.is_symlink():
+        if not default_key_path.exists():
             # Create a symlink to use this key by default
-            os.symlink(path, default_key_path)
+            default_key_path.symlink_to(path)
     return private_key
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/chains/cosmos.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/cosmos.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import base64
 import hashlib
 import json
+from typing import Union
 
 import ecdsa
 from cosmospy._wallet import privkey_to_address, privkey_to_pubkey
 
 from .common import BaseAccount, get_fallback_private_key, get_verification_buffer
 
 DEFAULT_HRP = "cosmos"
@@ -76,7 +77,16 @@
 
     def get_public_key(self) -> str:
         return privkey_to_pubkey(self.private_key).decode()
 
 
 def get_fallback_account(hrp=DEFAULT_HRP):
     return CSDKAccount(private_key=get_fallback_private_key(), hrp=hrp)
+
+
+def verify_signature(
+    signature: Union[bytes, str],
+    public_key: Union[bytes, str],
+    message: Union[bytes, str],
+) -> bool:
+    """TODO: Implement this"""
+    raise NotImplementedError("Not implemented yet")
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/chains/nuls1.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/nuls1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Barebone NULS address and message signing support.
 """
 import hashlib
 import logging
 import struct
 from binascii import hexlify, unhexlify
-from typing import Optional
+from typing import Optional, Union
 
 from coincurve.keys import PrivateKey, PublicKey
 
 from .common import (
     BaseAccount,
     get_fallback_private_key,
     get_public_key,
@@ -271,14 +271,16 @@
         output += write_with_length(self.sig_ser)
         if with_length:
             return write_with_length(output)
         else:
             return output
 
     def verify(self, message):
+        if not self.pub_key:
+            raise ValueError("Missing public key ")
         pub = PublicKey(self.pub_key)
         message = VarInt(len(message)).encode() + message
         # LOGGER.debug("Comparing with %r" % (MESSAGE_TEMPLATE.format(message).encode()))
         try:
             if self.sig_ser is None:
                 raise TypeError("sig_ser is None")
             good = pub.verify(self.sig_ser, MESSAGE_TEMPLATE.format(message).encode())
@@ -320,7 +322,16 @@
 
     def get_public_key(self):
         return get_public_key(private_key=self.private_key)
 
 
 def get_fallback_account(chain_id=8964):
     return NULSAccount(private_key=get_fallback_private_key(), chain_id=chain_id)
+
+
+def verify_signature(
+    signature: Union[bytes, str],
+    public_key: Union[bytes, str],
+    message: Union[bytes, str],
+) -> bool:
+    """TODO: Implement this"""
+    raise NotImplementedError("Not implemented yet")
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/chains/nuls2.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/nuls2.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import base64
+from typing import Union
 
 from nuls2.model.data import (
     NETWORKS,
     address_from_hash,
     public_key_to_hash,
     sign_recoverable_message,
 )
@@ -56,7 +57,16 @@
     def get_public_key(self):
         return get_public_key(private_key=self.private_key)
 
 
 def get_fallback_account(chain_id=1):
     acc = NULSAccount(private_key=get_fallback_private_key(), chain_id=chain_id)
     return acc
+
+
+def verify_signature(
+    signature: Union[bytes, str],
+    public_key: Union[bytes, str],
+    message: Union[bytes, str],
+) -> bool:
+    """TODO: Implement this"""
+    raise NotImplementedError("Not implemented yet")
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/chains/remote.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             address=properties.address,
             public_key=properties.public_key,
             host=host,
             session=session,
         )
 
     def __del__(self):
-        asyncio.run(self._session.close())
+        asyncio.get_running_loop().create_task(self._session.close())
 
     @property
     def private_key(self):
         raise NotImplementedError()
 
     async def sign_message(self, message: Dict) -> Dict:
         """Sign a message inplace."""
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/chains/sol.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/sol.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
-import os
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Dict, Optional, Union
 
 import base58
+from nacl.exceptions import BadSignatureError as NaclBadSignatureError
 from nacl.public import PrivateKey, SealedBox
-from nacl.signing import SigningKey
+from nacl.signing import SigningKey, VerifyKey
 
-from ..conf import settings
-from .common import BaseAccount, get_verification_buffer
+from ..exceptions import BadSignatureError
+from .common import BaseAccount, get_fallback_private_key, get_verification_buffer
 
 
 def encode(item):
     return base58.b58encode(bytes(item)).decode("ascii")
 
 
 class SOLAccount(BaseAccount):
@@ -57,27 +57,31 @@
 
 
 def generate_key() -> bytes:
     privkey = bytes(SigningKey.generate())
     return privkey
 
 
-def get_fallback_private_key(path: Optional[Path] = None) -> bytes:
-    path = path or settings.PRIVATE_KEY_FILE
-    private_key: bytes
-    if path.exists() and path.stat().st_size > 0:
-        with open(path, "rb") as prvfile:
-            private_key = prvfile.read()
-    else:
-        private_key = generate_key()
-        os.makedirs(path.parent, exist_ok=True)
-        with open(path, "wb") as prvfile:
-            prvfile.write(private_key)
-
-        with open(path, "rb") as prvfile:
-            print(prvfile.read())
-
-        default_key_path = path.parent / "default.key"
-        if not default_key_path.is_symlink():
-            # Create a symlink to use this key by default
-            os.symlink(path, default_key_path)
-    return private_key
+def verify_signature(
+    signature: Union[bytes, str],
+    public_key: Union[bytes, str],
+    message: Union[bytes, str],
+):
+    """
+    Verifies a signature.
+    Args:
+        signature: The signature to verify. Can be a base58 encoded string or bytes.
+        public_key: The public key to use for verification. Can be a base58 encoded string or bytes.
+        message: The message to verify. Can be an utf-8 string or bytes.
+    Raises:
+        BadSignatureError: If the signature is invalid.
+    """
+    if isinstance(signature, str):
+        signature = base58.b58decode(signature)
+    if isinstance(message, str):
+        message = message.encode("utf-8")
+    if isinstance(public_key, str):
+        public_key = base58.b58decode(public_key)
+    try:
+        VerifyKey(public_key).verify(message, signature)
+    except NaclBadSignatureError as e:
+        raise BadSignatureError from e
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/chains/substrate.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/substrate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from typing import Union
 
 from substrateinterface import Keypair
 
 from ..conf import settings
 from .common import BaseAccount, get_verification_buffer
 
 
@@ -33,15 +34,22 @@
 
 def get_fallback_account():
     return DOTAccount(mnemonics=get_fallback_mnemonics())
 
 
 def get_fallback_mnemonics():
     try:
-        with open(settings.PRIVATE_KEY_FILE, "r") as prvfile:
-            mnemonic = prvfile.read()
+        mnemonic = settings.PRIVATE_KEY_FILE.read_text()
     except OSError:
         mnemonic = Keypair.generate_mnemonic()
-        with open(settings.PRIVATE_KEY_FILE, "w") as prvfile:
-            prvfile.write(mnemonic)
+        settings.PRIVATE_KEY_FILE.write_text(mnemonic)
 
     return mnemonic
+
+
+def verify_signature(
+    signature: Union[bytes, str],
+    public_key: Union[bytes, str],
+    message: Union[bytes, str],
+) -> bool:
+    """TODO: Implement this"""
+    raise NotImplementedError("Not implemented yet")
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/chains/tezos.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/chains/tezos.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Dict, Optional, Union
 
 from aleph_pytezos.crypto.key import Key
 from nacl.public import SealedBox
 from nacl.signing import SigningKey
 
 from .common import BaseAccount, get_fallback_private_key, get_verification_buffer
 
@@ -44,7 +44,28 @@
 
     async def decrypt(self, content) -> bytes:
         return SealedBox(self._private_key).decrypt(content)
 
 
 def get_fallback_account(path: Optional[Path] = None) -> TezosAccount:
     return TezosAccount(private_key=get_fallback_private_key(path=path))
+
+
+def verify_signature(
+    signature: Union[bytes, str],
+    public_key: Union[bytes, str],
+    message: Union[bytes, str],
+) -> bool:
+    """
+    Verify a signature using the public key (hash) of a tezos account.
+
+    Note: It requires the public key hash (sp, p2, ed-prefix), not the address (tz1, tz2 prefix)!
+    Args:
+        signature: The signature to verify. Can be a base58 encoded string or bytes.
+        public_key: The public key (hash) of the account. Can be a base58 encoded string or bytes.
+        message: The message that was signed. Is a sequence of bytes in raw format or hexadecimal notation.
+    """
+    key = Key.from_encoded_key(public_key)
+    try:
+        return key.verify(signature, message)
+    except ValueError:
+        return False
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/conf.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,27 +20,23 @@
     API_HOST: str = "https://api2.aleph.im"
     MAX_INLINE_SIZE: int = 50000
     API_UNIX_SOCKET: Optional[str] = None
     REMOTE_CRYPTO_HOST: Optional[str] = None
     REMOTE_CRYPTO_UNIX_SOCKET: Optional[str] = None
     ADDRESS_TO_USE: Optional[str] = None
 
-    DEFAULT_CHANNEL: str = "TEST"
     DEFAULT_RUNTIME_ID: str = (
         "bd79839bf96e595a06da5ac0b6ba51dea6f7e2591bb913deccded04d831d29f4"
     )
     DEFAULT_VM_MEMORY: int = 128
     DEFAULT_VM_VCPUS: int = 1
     DEFAULT_VM_TIMEOUT: float = 30.0
 
     CODE_USES_SQUASHFS: bool = which("mksquashfs") is not None  # True if command exists
 
-    VM_URL_PATH = "https://aleph.sh/vm/{hash}"
-    VM_URL_HOST = "https://{hash_base32}.aleph.sh"
-
     class Config:
         env_prefix = "ALEPH_"
         case_sensitive = False
         env_file = ".env"
 
 
 # Settings singleton
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/exceptions.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,7 +30,15 @@
 class InvalidMessageError(BroadcastError):
     """
     The message could not be broadcast because it does not follow the Aleph
     message specification.
     """
 
     pass
+
+
+class BadSignatureError(Exception):
+    """
+    The signature of a message is invalid.
+    """
+
+    pass
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/types.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 from abc import abstractmethod
 from enum import Enum
 from typing import Dict, Protocol, TypeVar
 
-__all__ = ("StorageEnum", "Account", "AccountFromPrivateKey")
+__all__ = ("StorageEnum", "Account", "AccountFromPrivateKey", "GenericMessage")
 
 from aleph_message.models import AlephMessage
 
 
 class StorageEnum(str, Enum):
     ipfs = "ipfs"
     storage = "storage"
 
 
-# TODO: this class is duplicated in pyaleph. Move it to aleph-message.
-class MessageStatus(str, Enum):
-    PENDING = "pending"
-    PROCESSED = "processed"
-    REJECTED = "rejected"
-    FORGOTTEN = "forgotten"
-
-
 # Use a protocol to avoid importing crypto libraries
 class Account(Protocol):
     CHAIN: str
     CURVE: str
 
     @abstractmethod
     async def sign_message(self, message: Dict) -> Dict:
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/user_session.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,27 +37,28 @@
     PostContent,
     PostMessage,
     ProgramMessage,
     StoreContent,
     StoreMessage,
 )
 from aleph_message.models.program import Encoding, ProgramContent
+from aleph_message.status import MessageStatus
 from pydantic import ValidationError
 
-from aleph_client.types import Account, GenericMessage, MessageStatus, StorageEnum
+from aleph.sdk.types import Account, GenericMessage, StorageEnum
 
 from .conf import settings
 from .exceptions import (
     BroadcastError,
     InvalidMessageError,
     MessageNotFoundError,
     MultipleMessagesError,
 )
 from .models import MessagesResponse
-from .utils import get_message_type_value
+from .utils import check_unix_socket_valid, get_message_type_value
 
 logger = logging.getLogger(__name__)
 
 try:
     import magic
 except ImportError:
     logger.info("Could not import library 'magic', MIME type detection disabled")
@@ -67,15 +68,15 @@
 
 
 def async_wrapper(f):
     """
     Copies the docstring of wrapped functions.
     """
 
-    wrapped = getattr(AuthenticatedUserSession, f.__name__)
+    wrapped = getattr(AuthenticatedAlephClient, f.__name__)
     f.__doc__ = wrapped.__doc__
 
 
 def wrap_async(func: Callable[..., Awaitable[T]]) -> Callable[..., T]:
     """Wrap an asynchronous function into a synchronous one,
     for easy use in synchronous code.
     """
@@ -89,22 +90,22 @@
     func_caller.__annotations__ = func.__annotations__
     func_caller.__defaults__ = func.__defaults__
     func_caller.__kwdefaults__ = func.__kwdefaults__
     return func_caller
 
 
 async def run_async_watcher(
-    *args, output_queue: queue.Queue, api_server: str, **kwargs
+    *args, output_queue: queue.Queue, api_server: Optional[str], **kwargs
 ):
-    async with UserSession(api_server=api_server) as session:
+    async with AlephClient(api_server=api_server) as session:
         async for message in session.watch_messages(*args, **kwargs):
             output_queue.put(message)
 
 
-def watcher_thread(output_queue: queue.Queue, api_server: str, args, kwargs):
+def watcher_thread(output_queue: queue.Queue, api_server: Optional[str], args, kwargs):
     asyncio.run(
         run_async_watcher(
             output_queue=output_queue, api_server=api_server, *args, **kwargs
         )
     )
 
 
@@ -118,15 +119,15 @@
     should look like this (using args and kwargs for brevity, but the functions should
     be fully typed):
 
     >>> def func(self, *args, **kwargs):
     >>>     return self._wrap(self.async_session.func)(*args, **kwargs)
     """
 
-    def __init__(self, async_session: "UserSession"):
+    def __init__(self, async_session: "AlephClient"):
         self.async_session = async_session
 
     def _wrap(self, method: Callable[..., Awaitable[T]], *args, **kwargs):
         return wrap_async(method)(*args, **kwargs)
 
     def get_messages(
         self,
@@ -268,17 +269,17 @@
         )
         thread.start()
         while True:
             yield output_queue.get()
 
 
 class AuthenticatedUserSessionSync(UserSessionSync):
-    async_session: "AuthenticatedUserSession"
+    async_session: "AuthenticatedAlephClient"
 
-    def __init__(self, async_session: "AuthenticatedUserSession"):
+    def __init__(self, async_session: "AuthenticatedAlephClient"):
         super().__init__(async_session=async_session)
 
     def ipfs_push(self, content: Mapping) -> str:
         return self._wrap(self.async_session.ipfs_push, content=content)
 
     def storage_push(self, content: Mapping) -> str:
         return self._wrap(self.async_session.storage_push, content=content)
@@ -373,14 +374,15 @@
         memory: Optional[int] = None,
         vcpus: Optional[int] = None,
         timeout_seconds: Optional[float] = None,
         persistent: bool = False,
         encoding: Encoding = Encoding.zip,
         volumes: Optional[List[Mapping]] = None,
         subscriptions: Optional[List[Mapping]] = None,
+        metadata: Optional[Mapping[str, Any]] = None,
     ) -> Tuple[ProgramMessage, MessageStatus]:
         return self._wrap(
             self.async_session.create_program,
             program_ref=program_ref,
             entrypoint=entrypoint,
             runtime=runtime,
             environment_variables=environment_variables,
@@ -391,14 +393,15 @@
             memory=memory,
             vcpus=vcpus,
             timeout_seconds=timeout_seconds,
             persistent=persistent,
             encoding=encoding,
             volumes=volumes,
             subscriptions=subscriptions,
+            metadata=metadata,
         )
 
     def forget(
         self,
         hashes: List[str],
         reason: Optional[str],
         storage_engine: StorageEnum = StorageEnum.storage,
@@ -432,34 +435,64 @@
             channel=channel,
             storage_engine=storage_engine,
             allow_inlining=allow_inlining,
             sync=sync,
         )
 
 
-class UserSession:
+class AlephClient:
     api_server: str
     http_session: aiohttp.ClientSession
 
-    def __init__(self, api_server: str):
-        self.api_server = api_server
-        self.http_session = aiohttp.ClientSession(base_url=api_server)
+    def __init__(
+        self,
+        api_server: Optional[str],
+        api_unix_socket: Optional[str] = None,
+        allow_unix_sockets: bool = True,
+        timeout: Optional[aiohttp.ClientTimeout] = None,
+    ):
+        """AlephClient can use HTTP(S) or HTTP over Unix sockets.
+        Unix sockets are used when running inside a virtual machine,
+        and can be shared across containers in a more secure way than TCP ports.
+        """
+        self.api_server = api_server or settings.API_HOST
+        if not self.api_server:
+            raise ValueError("Missing API host")
+
+        unix_socket_path = api_unix_socket or settings.API_UNIX_SOCKET
+        if unix_socket_path and allow_unix_sockets:
+            check_unix_socket_valid(unix_socket_path)
+            connector = aiohttp.UnixConnector(path=unix_socket_path)
+        else:
+            connector = None
+
+        # ClientSession timeout defaults to a private sentinel object and may not be None.
+        self.http_session = (
+            aiohttp.ClientSession(
+                base_url=self.api_server, connector=connector, timeout=timeout
+            )
+            if timeout
+            else aiohttp.ClientSession(
+                base_url=self.api_server,
+                connector=connector,
+            )
+        )
 
     def __enter__(self) -> UserSessionSync:
         return UserSessionSync(async_session=self)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         close_fut = self.http_session.close()
         try:
             loop = asyncio.get_running_loop()
             loop.run_until_complete(close_fut)
         except RuntimeError:
             asyncio.run(close_fut)
 
-    async def __aenter__(self) -> "UserSession":
+    async def __aenter__(self) -> "AlephClient":
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.http_session.close()
 
     async def fetch_aggregate(
         self,
@@ -803,37 +836,49 @@
                     else:
                         data = json.loads(msg.data)
                         yield Message(**data)
                 elif msg.type == aiohttp.WSMsgType.ERROR:
                     break
 
 
-class AuthenticatedUserSession(UserSession):
+class AuthenticatedAlephClient(AlephClient):
     account: Account
 
     BROADCAST_MESSAGE_FIELDS = {
         "sender",
         "chain",
         "signature",
         "type",
         "item_hash",
         "item_type",
         "item_content",
         "time",
         "channel",
     }
 
-    def __init__(self, account: Account, api_server: str):
-        super().__init__(api_server=api_server)
+    def __init__(
+        self,
+        account: Account,
+        api_server: Optional[str],
+        api_unix_socket: Optional[str] = None,
+        allow_unix_sockets: bool = True,
+        timeout: Optional[aiohttp.ClientTimeout] = None,
+    ):
+        super().__init__(
+            api_server=api_server,
+            api_unix_socket=api_unix_socket,
+            allow_unix_sockets=allow_unix_sockets,
+            timeout=timeout,
+        )
         self.account = account
 
     def __enter__(self) -> "AuthenticatedUserSessionSync":
         return AuthenticatedUserSessionSync(async_session=self)
 
-    async def __aenter__(self) -> "AuthenticatedUserSession":
+    async def __aenter__(self) -> "AuthenticatedAlephClient":
         return self
 
     async def ipfs_push(self, content: Mapping) -> str:
         """Push arbitrary content as JSON to the IPFS service."""
 
         url = "/api/v0/ipfs/add_json"
         logger.debug(f"Pushing to IPFS on {url}")
@@ -926,15 +971,14 @@
         if response.status != 200:
             await self._handle_broadcast_error(response)
         else:
             publication_status = await response.json()
             self._log_publication_status(publication_status)
 
     async def _broadcast_deprecated(self, message_dict: Mapping[str, Any]) -> None:
-
         """
         Broadcast a message on the Aleph network using the deprecated
         /ipfs/pubsub/pub/ endpoint.
         """
 
         url = "/api/v0/ipfs/pubsub/pub"
         logger.debug(f"Posting message on {url}")
@@ -1112,15 +1156,15 @@
         if file_hash is None:
             if file_content is None:
                 if file_path is None:
                     raise ValueError(
                         "Please specify at least a file_content, a file_hash or a file_path"
                     )
                 else:
-                    file_content = open(file_path, "rb").read()
+                    file_content = Path(file_path).read_bytes()
 
             if storage_engine == StorageEnum.storage:
                 file_hash = await self.storage_push_file(file_content=file_content)
             elif storage_engine == StorageEnum.ipfs:
                 file_hash = await self.ipfs_push_file(file_content=file_content)
             else:
                 raise ValueError(f"Unknown storage engine: '{storage_engine}'")
@@ -1167,14 +1211,15 @@
         memory: Optional[int] = None,
         vcpus: Optional[int] = None,
         timeout_seconds: Optional[float] = None,
         persistent: bool = False,
         encoding: Encoding = Encoding.zip,
         volumes: Optional[List[Mapping]] = None,
         subscriptions: Optional[List[Mapping]] = None,
+        metadata: Optional[Mapping[str, Any]] = None,
     ) -> Tuple[ProgramMessage, MessageStatus]:
         """
         Post a (create) PROGRAM message.
 
         :param program_ref: Reference to the program to run
         :param entrypoint: Entrypoint to run
         :param runtime: Runtime to use
@@ -1240,14 +1285,15 @@
                     "use_latest": True,
                     "comment": "Official Aleph runtime"
                     if runtime == settings.DEFAULT_RUNTIME_ID
                     else "",
                 },
                 "volumes": volumes,
                 "time": time.time(),
+                "metadata": metadata,
             }
         )
 
         # Ensure that the version of aleph-message used supports the field.
         assert content.on.persistent == persistent
 
         return await self.submit(
@@ -1308,15 +1354,14 @@
         self,
         message_type: MessageType,
         content: Dict[str, Any],
         channel: Optional[str],
         allow_inlining: bool = True,
         storage_engine: StorageEnum = StorageEnum.storage,
     ) -> AlephMessage:
-
         message_dict: Dict[str, Any] = {
             "sender": self.account.get_address(),
             "chain": self.account.CHAIN,
             "type": message_type,
             "content": content,
             "time": time.time(),
             "channel": channel,
@@ -1349,15 +1394,14 @@
         content: Dict[str, Any],
         message_type: MessageType,
         channel: Optional[str] = None,
         storage_engine: StorageEnum = StorageEnum.storage,
         allow_inlining: bool = True,
         sync: bool = False,
     ) -> Tuple[AlephMessage, MessageStatus]:
-
         message = await self._prepare_aleph_message(
             message_type=message_type,
             content=content,
             channel=channel,
             allow_inlining=allow_inlining,
             storage_engine=storage_engine,
         )
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/utils.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import errno
 import logging
 import os
 from pathlib import Path
 from shutil import make_archive
 from typing import Tuple, Type
 from zipfile import BadZipFile, ZipFile
 
 from aleph_message.models import MessageType
 from aleph_message.models.program import Encoding
 
-from aleph_client.conf import settings
-from aleph_client.types import GenericMessage
+from aleph.sdk.conf import settings
+from aleph.sdk.types import GenericMessage
 
 logger = logging.getLogger(__name__)
 
 try:
     import magic
 except ImportError:
     logger.info("Could not import library 'magic', MIME type detection disabled")
@@ -55,7 +56,23 @@
         raise FileNotFoundError("No file or directory to create the archive from")
 
 
 def get_message_type_value(message_type: Type[GenericMessage]) -> MessageType:
     """Returns the value of the 'type' field of a message type class."""
     type_literal = message_type.__annotations__["type"]
     return type_literal.__args__[0]  # Get the value from a Literal
+
+
+def check_unix_socket_valid(unix_socket_path: str) -> bool:
+    """Check that a unix socket exists at the given path, or raise a FileNotFoundError."""
+    path = Path(unix_socket_path)
+    if not path.exists():
+        raise FileNotFoundError(
+            errno.ENOENT, os.strerror(errno.ENOENT), unix_socket_path
+        )
+    if not path.is_socket():
+        raise FileNotFoundError(
+            errno.ENOTSOCK,
+            os.strerror(errno.ENOENT),
+            unix_socket_path,
+        )
+    return True
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/vm/app.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
     async def __call__(
         self,
         scope: MutableMapping[str, Any],
         receive: Optional[Callable[[], Awaitable[Any]]] = None,
         send: Optional[Callable[[Dict[Any, Any]], Awaitable[Any]]] = None,
     ):
-        if scope["type"] in ("http", "websocket"):
+        if scope["type"] in ("http", "websocket", "lifespan"):
             if self.http_app:
                 await self.http_app(scope=scope, receive=receive, send=send)
             else:
                 raise ValueError("No HTTP app registered")
         elif scope["type"] == "aleph.message":
             for event_handler in self.event_handlers:
                 if event_handler.matches(scope):
```

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_client/vm/cache.py` & `aleph-sdk-python-0.7.0b1/src/aleph/sdk/vm/cache.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/src/aleph_sdk_python.egg-info/SOURCES.txt` & `aleph-sdk-python-0.7.0b1/src/aleph_sdk_python.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -36,40 +36,39 @@
 examples/httpgateway.py
 examples/metrics.py
 examples/mqtt.py
 examples/store.py
 scripts/build-and-shell.sh
 scripts/build-and-test.sh
 scripts/build-to-publish.sh
-src/aleph_client/__init__.py
-src/aleph_client/__main__.py
-src/aleph_client/account.py
-src/aleph_client/conf.py
-src/aleph_client/exceptions.py
-src/aleph_client/models.py
-src/aleph_client/types.py
-src/aleph_client/user_session.py
-src/aleph_client/utils.py
-src/aleph_client/chains/__init__.py
-src/aleph_client/chains/common.py
-src/aleph_client/chains/cosmos.py
-src/aleph_client/chains/ethereum.py
-src/aleph_client/chains/nuls1.py
-src/aleph_client/chains/nuls2.py
-src/aleph_client/chains/remote.py
-src/aleph_client/chains/sol.py
-src/aleph_client/chains/substrate.py
-src/aleph_client/chains/tezos.py
-src/aleph_client/vm/__init__.py
-src/aleph_client/vm/app.py
-src/aleph_client/vm/cache.py
+src/aleph/__init__.py
+src/aleph/sdk/__init__.py
+src/aleph/sdk/account.py
+src/aleph/sdk/client.py
+src/aleph/sdk/conf.py
+src/aleph/sdk/exceptions.py
+src/aleph/sdk/models.py
+src/aleph/sdk/types.py
+src/aleph/sdk/utils.py
+src/aleph/sdk/chains/__init__.py
+src/aleph/sdk/chains/common.py
+src/aleph/sdk/chains/cosmos.py
+src/aleph/sdk/chains/ethereum.py
+src/aleph/sdk/chains/nuls1.py
+src/aleph/sdk/chains/nuls2.py
+src/aleph/sdk/chains/remote.py
+src/aleph/sdk/chains/sol.py
+src/aleph/sdk/chains/substrate.py
+src/aleph/sdk/chains/tezos.py
+src/aleph/sdk/vm/__init__.py
+src/aleph/sdk/vm/app.py
+src/aleph/sdk/vm/cache.py
 src/aleph_sdk_python.egg-info/PKG-INFO
 src/aleph_sdk_python.egg-info/SOURCES.txt
 src/aleph_sdk_python.egg-info/dependency_links.txt
-src/aleph_sdk_python.egg-info/entry_points.txt
 src/aleph_sdk_python.egg-info/not-zip-safe
 src/aleph_sdk_python.egg-info/requires.txt
 src/aleph_sdk_python.egg-info/top_level.txt
 tests/__init__.py
 tests/integration/__init__.py
 tests/integration/config.py
 tests/integration/conftest.py
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/integration/conftest.py` & `aleph-sdk-python-0.7.0b1/tests/integration/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 
 import pytest
 
-from aleph_client.chains.common import get_fallback_private_key
-from aleph_client.chains.ethereum import ETHAccount
+from aleph.sdk.chains.common import get_fallback_private_key
+from aleph.sdk.chains.ethereum import ETHAccount
 
 
 @pytest.fixture
 def fixture_account():
     private_key = get_fallback_private_key()
     return ETHAccount(private_key)
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/integration/itest_aggregates.py` & `aleph-sdk-python-0.7.0b1/tests/integration/itest_aggregates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import json
 from typing import Dict
 
 import pytest
 
-from aleph_client.types import Account
-from aleph_client.user_session import AuthenticatedUserSession
+from aleph.sdk.client import AuthenticatedAlephClient
+from aleph.sdk.types import Account
 from tests.integration.toolkit import try_until
 
 from .config import REFERENCE_NODE, TARGET_NODE
 
 
 async def create_aggregate_on_target(
     account: Account,
     key: str,
     content: Dict,
     emitter_node: str,
     receiver_node: str,
     channel="INTEGRATION_TESTS",
 ):
-    async with AuthenticatedUserSession(
+    async with AuthenticatedAlephClient(
         account=account, api_server=emitter_node
     ) as tx_session:
         aggregate_message, message_status = await tx_session.create_aggregate(
             key=key,
             content=content,
             channel="INTEGRATION_TESTS",
         )
@@ -34,15 +34,15 @@
     assert item_content["key"] == key
     assert item_content["content"] == content
     assert item_content["address"] == account.get_address()
     assert aggregate_message.content.key == key
     assert aggregate_message.content.address == account.get_address()
     assert aggregate_message.content.content == content
 
-    async with AuthenticatedUserSession(
+    async with AuthenticatedAlephClient(
         account=account, api_server=receiver_node
     ) as rx_session:
         aggregate_from_receiver = await try_until(
             rx_session.fetch_aggregate,
             lambda aggregate: aggregate is not None,
             timeout=5,
             address=account.get_address(),
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/integration/itest_forget.py` & `aleph-sdk-python-0.7.0b1/tests/integration/itest_forget.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import Callable, Dict
 
 import pytest
 
-from aleph_client.types import Account
-from aleph_client.user_session import AuthenticatedUserSession
+from aleph.sdk.client import AuthenticatedAlephClient
+from aleph.sdk.types import Account
 
 from .config import REFERENCE_NODE, TARGET_NODE, TEST_CHANNEL
 from .toolkit import try_until
 
 
 async def create_and_forget_post(
     account: Account, emitter_node: str, receiver_node: str, channel=TEST_CHANNEL
 ) -> str:
     async def wait_matching_posts(
         item_hash: str,
         condition: Callable[[Dict], bool],
         timeout: int = 5,
     ):
-        async with AuthenticatedUserSession(
+        async with AuthenticatedAlephClient(
             account=account, api_server=receiver_node
         ) as rx_session:
             return await try_until(
                 rx_session.get_posts,
                 condition,
                 timeout=timeout,
                 hashes=[item_hash],
             )
 
-    async with AuthenticatedUserSession(
+    async with AuthenticatedAlephClient(
         account=account, api_server=emitter_node
     ) as tx_session:
         post_message, message_status = await tx_session.create_post(
             post_content="A considerate and politically correct post.",
             post_type="POST",
             channel="INTEGRATION_TESTS",
         )
@@ -42,15 +42,15 @@
         post_message.item_hash,
         lambda response: len(response["posts"]) > 0,
     )
     print(get_post_response)
 
     post_hash = post_message.item_hash
     reason = "This well thought-out content offends me!"
-    async with AuthenticatedUserSession(
+    async with AuthenticatedAlephClient(
         account=account, api_server=emitter_node
     ) as tx_session:
         forget_message, forget_status = await tx_session.forget(
             hashes=[post_hash],
             reason=reason,
             channel=channel,
         )
@@ -99,15 +99,15 @@
 async def test_forget_a_forget_message(fixture_account):
     """
     Attempts to forget a forget message. This should fail.
     """
 
     # TODO: this test should be moved to the PyAleph API tests, once a framework is in place.
     post_hash = await create_and_forget_post(fixture_account, TARGET_NODE, TARGET_NODE)
-    async with AuthenticatedUserSession(
+    async with AuthenticatedAlephClient(
         account=fixture_account, api_server=TARGET_NODE
     ) as session:
         get_post_response = await session.get_posts(hashes=[post_hash])
         assert len(get_post_response["posts"]) == 1
         post = get_post_response["posts"][0]
 
         forget_message_hash = post["forgotten_by"][0]
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/integration/itest_posts.py` & `aleph-sdk-python-0.7.0b1/tests/integration/itest_posts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 import pytest
 from aleph_message.models import MessagesResponse
 
-from aleph_client.user_session import AuthenticatedUserSession
+from aleph.sdk.client import AuthenticatedAlephClient
 from tests.integration.toolkit import try_until
 
 from .config import REFERENCE_NODE, TARGET_NODE
 
 
 async def create_message_on_target(
     fixture_account, emitter_node: str, receiver_node: str
 ):
     """
     Create a POST message on the target node, then fetch it from the reference node.
     """
-    async with AuthenticatedUserSession(
+    async with AuthenticatedAlephClient(
         account=fixture_account, api_server=emitter_node
     ) as tx_session:
         post_message, message_status = await tx_session.create_post(
             post_content=None,
             post_type="POST",
             channel="INTEGRATION_TESTS",
         )
 
     def response_contains_messages(response: MessagesResponse) -> bool:
         return len(response.messages) > 0
 
-    async with AuthenticatedUserSession(
+    async with AuthenticatedAlephClient(
         account=fixture_account, api_server=receiver_node
     ) as rx_session:
         responses = await try_until(
             rx_session.get_messages,
             response_contains_messages,
             timeout=5,
             hashes=[post_message.item_hash],
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/integration/toolkit.py` & `aleph-sdk-python-0.7.0b1/tests/integration/toolkit.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/conftest.py` & `aleph-sdk-python-0.7.0b1/tests/unit/conftest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
 import pytest as pytest
 
-import aleph_client.chains.ethereum as ethereum
-import aleph_client.chains.sol as solana
-import aleph_client.chains.tezos as tezos
-from aleph_client.chains.common import get_fallback_private_key
+import aleph.sdk.chains.ethereum as ethereum
+import aleph.sdk.chains.sol as solana
+import aleph.sdk.chains.tezos as tezos
+from aleph.sdk.chains.common import get_fallback_private_key
 
 
 @pytest.fixture
 def fallback_private_key() -> bytes:
     with NamedTemporaryFile() as private_key_file:
         yield get_fallback_private_key(path=Path(private_key_file.name))
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/test_asynchronous.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_asynchronous.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 from aleph_message.models import (
     AggregateMessage,
     ForgetMessage,
     PostMessage,
     ProgramMessage,
     StoreMessage,
 )
+from aleph_message.status import MessageStatus
 
-from aleph_client import AuthenticatedUserSession
-from aleph_client.types import Account, MessageStatus, StorageEnum
+from aleph.sdk.client import AuthenticatedAlephClient
+from aleph.sdk.types import Account, StorageEnum
 
 
 @pytest.fixture
 def mock_session_with_post_success(
     ethereum_account: Account,
-) -> AuthenticatedUserSession:
+) -> AuthenticatedAlephClient:
     class MockResponse:
         def __init__(self, sync: bool):
             self.sync = sync
 
         async def __aenter__(self):
             return self
 
@@ -44,20 +45,20 @@
 
     http_session = AsyncMock()
     http_session.post = MagicMock()
     http_session.post.side_effect = lambda *args, **kwargs: MockResponse(
         sync=kwargs.get("sync", False)
     )
 
-    user_session = AuthenticatedUserSession(
+    client = AuthenticatedAlephClient(
         account=ethereum_account, api_server="http://localhost"
     )
-    user_session.http_session = http_session
+    client.http_session = http_session
 
-    return user_session
+    return client
 
 
 @pytest.mark.asyncio
 async def test_create_post(mock_session_with_post_success):
     async with mock_session_with_post_success as session:
         content = {"Hello": "World"}
 
@@ -126,14 +127,15 @@
 async def test_create_program(mock_session_with_post_success):
     async with mock_session_with_post_success as session:
         program_message, message_status = await session.create_program(
             program_ref="cafecafecafecafecafecafecafecafecafecafecafecafecafecafecafecafe",
             entrypoint="main:app",
             runtime="facefacefacefacefacefacefacefacefacefacefacefacefacefacefaceface",
             channel="TEST",
+            metadata={"tags": ["test"]},
         )
 
     assert mock_session_with_post_success.http_session.post.called_once
     assert isinstance(program_message, ProgramMessage)
 
 
 @pytest.mark.asyncio
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/test_asynchronous_get.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_asynchronous_get.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import unittest
 from typing import Any, Dict
 from unittest.mock import AsyncMock
 
 import pytest
 from aleph_message.models import MessagesResponse, MessageType
 
-from aleph_client.conf import settings
-from aleph_client.user_session import UserSession
+from aleph.sdk.client import AlephClient
+from aleph.sdk.conf import settings
 
 
-def make_mock_session(get_return_value: Dict[str, Any]) -> UserSession:
+def make_mock_session(get_return_value: Dict[str, Any]) -> AlephClient:
     class MockResponse:
         async def __aenter__(self):
             return self
 
         async def __aexit__(self, exc_type, exc_val, exc_tb):
             ...
 
@@ -26,18 +26,18 @@
 
     class MockHttpSession(AsyncMock):
         def get(self, *_args, **_kwargs):
             return MockResponse()
 
     http_session = MockHttpSession()
 
-    user_session = UserSession(api_server="http://localhost")
-    user_session.http_session = http_session
+    client = AlephClient(api_server="http://localhost")
+    client.http_session = http_session
 
-    return user_session
+    return client
 
 
 @pytest.mark.asyncio
 async def test_fetch_aggregate():
     mock_session = make_mock_session(
         {"data": {"corechannel": {"nodes": [], "resource_nodes": []}}}
     )
@@ -61,28 +61,28 @@
         )
         assert response.keys() == {"corechannel"}
         assert response["corechannel"].keys() == {"nodes", "resource_nodes"}
 
 
 @pytest.mark.asyncio
 async def test_get_posts():
-    async with UserSession(api_server=settings.API_HOST) as session:
+    async with AlephClient(api_server=settings.API_HOST) as session:
         response: MessagesResponse = await session.get_messages(
             message_type=MessageType.post,
         )
 
         messages = response.messages
         assert len(messages) > 1
         for message in messages:
             assert message.type == MessageType.post
 
 
 @pytest.mark.asyncio
 async def test_get_messages():
-    async with UserSession(api_server=settings.API_HOST) as session:
+    async with AlephClient(api_server=settings.API_HOST) as session:
         response: MessagesResponse = await session.get_messages(
             pagination=2,
         )
 
         messages = response.messages
         assert len(messages) > 1
         assert messages[0].type
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/test_chain_ethereum.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_chain_tezos.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,73 @@
+import json
 from dataclasses import asdict, dataclass
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
 import pytest
 
-from aleph_client.chains.ethereum import get_fallback_account
+from aleph.sdk.chains.common import get_verification_buffer
+from aleph.sdk.chains.tezos import TezosAccount, get_fallback_account, verify_signature
 
 
 @dataclass
 class Message:
     chain: str
     sender: str
     type: str
     item_hash: str
 
 
-def test_get_fallback_account():
+def test_get_fallback_account(tezos_account: TezosAccount):
     with NamedTemporaryFile() as private_key_file:
-        account = get_fallback_account(path=Path(private_key_file.name))
-        assert account.CHAIN == "ETH"
+        account: TezosAccount = get_fallback_account(path=Path(private_key_file.name))
+
+        assert account.CHAIN == "TEZOS"
         assert account.CURVE == "secp256k1"
-        assert account._account.address
+        assert account._account.public_key()
 
 
 @pytest.mark.asyncio
-async def test_ETHAccount(ethereum_account):
-    account = ethereum_account
-
-    message = Message("ETH", account.get_address(), "SomeType", "ItemHash")
-    signed = await account.sign_message(asdict(message))
+async def test_tezos_account(tezos_account: TezosAccount):
+    message = Message("TEZOS", tezos_account.get_address(), "SomeType", "ItemHash")
+    signed = await tezos_account.sign_message(asdict(message))
     assert signed["signature"]
-    assert len(signed["signature"]) == 132
+    assert len(signed["signature"]) == 188
 
-    address = account.get_address()
-    assert address
-    assert type(address) == str
-    assert len(address) == 42
-
-    pubkey = account.get_public_key()
-    assert type(pubkey) == str
-    assert len(pubkey) == 68
+    address = tezos_account.get_address()
+    assert address is not None
+    assert isinstance(address, str)
+    assert len(address) == 36
+
+    pubkey = tezos_account.get_public_key()
+    assert isinstance(pubkey, str)
+    assert len(pubkey) == 55
 
 
 @pytest.mark.asyncio
-async def test_decrypt_secp256k1(ethereum_account):
-    account = ethereum_account
+async def test_verify_signature(tezos_account: TezosAccount):
+    message = asdict(
+        Message(
+            "TEZOS",
+            tezos_account.get_address(),
+            "POST",
+            "SomeHash",
+        )
+    )
+    await tezos_account.sign_message(message)
+    assert message["signature"]
+    raw_signature = json.loads(message["signature"])["signature"]
+    public_key = tezos_account.get_public_key()
+
+    assert verify_signature(raw_signature, public_key, get_verification_buffer(message))
 
-    assert account.CURVE == "secp256k1"
+
+@pytest.mark.asyncio
+async def test_decrypt_secp256k1(tezos_account: TezosAccount):
+    assert tezos_account.CURVE == "secp256k1"
     content = b"SomeContent"
 
-    encrypted = await account.encrypt(content)
-    assert type(encrypted) == bytes
-    decrypted = await account.decrypt(encrypted)
-    assert type(decrypted) == bytes
+    encrypted = await tezos_account.encrypt(content)
+    assert isinstance(encrypted, bytes)
+    decrypted = await tezos_account.decrypt(encrypted)
+    assert isinstance(decrypted, bytes)
     assert content == decrypted
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/test_chain_nuls1.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_chain_nuls1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 from coincurve.keys import PrivateKey
 
-from aleph_client.chains.nuls1 import NulsSignature
+from aleph.sdk.chains.nuls1 import NulsSignature
 
 SECRET = (
     b"\xc4\xfe\xe65\x96\x14\xb4:\r: \x05;\x12j\x9bJ"
     b"\x14\x0eY\xe3BY\x0f\xd6\xee\xfc\x9d\xfe\x8fv\xbc"
 )
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/test_chain_nuls1_compat.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_chain_nuls1_compat.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
 import pytest
 import secp256k1
 from coincurve.keys import PrivateKey
 
-from aleph_client.chains.common import get_fallback_private_key
-from aleph_client.chains.nuls1 import LOGGER, MESSAGE_TEMPLATE, NulsSignature, VarInt
+from aleph.sdk.chains.common import get_fallback_private_key
+from aleph.sdk.chains.nuls1 import LOGGER, MESSAGE_TEMPLATE, NulsSignature, VarInt
 
 SECRET = (
     b"\xc4\xfe\xe65\x96\x14\xb4:\r: \x05;\x12j\x9bJ"
     b"\x14\x0eY\xe3BY\x0f\xd6\xee\xfc\x9d\xfe\x8fv\xbc"
 )
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/test_chain_solana.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_chain_solana.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
 import base58
 import pytest
 from nacl.signing import VerifyKey
 
-from aleph_client.chains.common import get_verification_buffer
-from aleph_client.chains.sol import SOLAccount, get_fallback_account
+from aleph.sdk.chains.common import get_verification_buffer
+from aleph.sdk.chains.sol import SOLAccount, get_fallback_account, verify_signature
+from aleph.sdk.exceptions import BadSignatureError
 
 
 @dataclass
 class Message:
     chain: str
     sender: str
     type: str
@@ -45,15 +46,14 @@
     # assert len(address) == 44  # can also be 43?
     signature = json.loads(message["signature"])
 
     pubkey = base58.b58decode(signature["publicKey"])
     assert type(pubkey) == bytes
     assert len(pubkey) == 32
 
-    # modeled according to https://github.com/aleph-im/pyaleph/blob/master/src/aleph/chains/solana.py
     verify_key = VerifyKey(pubkey)
     verification_buffer = get_verification_buffer(message)
     assert get_verification_buffer(initial_message) == verification_buffer
     verif = verify_key.verify(
         verification_buffer, signature=base58.b58decode(signature["signature"])
     )
 
@@ -67,7 +67,44 @@
     content = b"SomeContent"
 
     encrypted = await solana_account.encrypt(content)
     assert type(encrypted) == bytes
     decrypted = await solana_account.decrypt(encrypted)
     assert type(decrypted) == bytes
     assert content == decrypted
+
+
+@pytest.mark.asyncio
+async def test_verify_signature(solana_account):
+    message = asdict(
+        Message(
+            "SOL",
+            solana_account.get_address(),
+            "POST",
+            "SomeHash",
+        )
+    )
+    await solana_account.sign_message(message)
+    assert message["signature"]
+    raw_signature = json.loads(message["signature"])["signature"]
+    assert type(raw_signature) == str
+
+    verify_signature(raw_signature, message["sender"], get_verification_buffer(message))
+
+
+@pytest.mark.asyncio
+async def test_verify_signature_with_forged_signature(solana_account):
+    message = asdict(
+        Message(
+            "SOL",
+            solana_account.get_address(),
+            "POST",
+            "SomeHash",
+        )
+    )
+    await solana_account.sign_message(message)
+    assert message["signature"]
+    # create forged 64 bit signature from random bytes
+    forged = base58.b58encode(bytes(64)).decode("utf-8")
+
+    with pytest.raises(BadSignatureError):
+        verify_signature(forged, message["sender"], get_verification_buffer(message))
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/test_chain_tezos.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_chain_ethereum.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,100 @@
 from dataclasses import asdict, dataclass
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 
 import pytest
 
-from aleph_client.chains.tezos import TezosAccount, get_fallback_account
+from aleph.sdk.chains.common import get_verification_buffer
+from aleph.sdk.chains.ethereum import get_fallback_account, verify_signature
+from aleph.sdk.exceptions import BadSignatureError
 
 
 @dataclass
 class Message:
     chain: str
     sender: str
     type: str
     item_hash: str
 
 
-def test_get_fallback_account(tezos_account: TezosAccount):
+def test_get_fallback_account():
     with NamedTemporaryFile() as private_key_file:
-        account: TezosAccount = get_fallback_account(path=Path(private_key_file.name))
-
-        assert account.CHAIN == "TEZOS"
+        account = get_fallback_account(path=Path(private_key_file.name))
+        assert account.CHAIN == "ETH"
         assert account.CURVE == "secp256k1"
-        assert account._account.public_key()
+        assert account._account.address
 
 
 @pytest.mark.asyncio
-async def test_tezos_account(tezos_account: TezosAccount):
-    message = Message("TEZOS", tezos_account.get_address(), "SomeType", "ItemHash")
-    signed = await tezos_account.sign_message(asdict(message))
+async def test_ETHAccount(ethereum_account):
+    account = ethereum_account
+
+    message = Message("ETH", account.get_address(), "SomeType", "ItemHash")
+    signed = await account.sign_message(asdict(message))
     assert signed["signature"]
-    assert len(signed["signature"]) == 188
+    assert len(signed["signature"]) == 132
+
+    address = account.get_address()
+    assert address
+    assert type(address) == str
+    assert len(address) == 42
+
+    pubkey = account.get_public_key()
+    assert type(pubkey) == str
+    assert len(pubkey) == 68
+
+
+@pytest.mark.asyncio
+async def test_verify_signature(ethereum_account):
+    account = ethereum_account
 
-    address = tezos_account.get_address()
-    assert address is not None
-    assert isinstance(address, str)
-    assert len(address) == 36
-
-    pubkey = tezos_account.get_public_key()
-    assert isinstance(pubkey, str)
-    assert len(pubkey) == 55
+    message = asdict(
+        Message(
+            "ETH",
+            account.get_address(),
+            "POST",
+            "SomeHash",
+        )
+    )
+    await account.sign_message(message)
+    assert message["signature"]
+
+    verify_signature(
+        message["signature"], message["sender"], get_verification_buffer(message)
+    )
 
 
 @pytest.mark.asyncio
-async def test_decrypt_secp256k1(tezos_account: TezosAccount):
-    assert tezos_account.CURVE == "secp256k1"
+async def test_verify_signature_with_forged_signature(ethereum_account):
+    account = ethereum_account
+
+    message = asdict(
+        Message(
+            "ETH",
+            account.get_address(),
+            "POST",
+            "SomeHash",
+        )
+    )
+    await account.sign_message(message)
+    assert message["signature"]
+
+    forged_signature = "0x" + "0" * 130
+    with pytest.raises(BadSignatureError):
+        verify_signature(
+            forged_signature, message["sender"], get_verification_buffer(message)
+        )
+
+
+@pytest.mark.asyncio
+async def test_decrypt_secp256k1(ethereum_account):
+    account = ethereum_account
+
+    assert account.CURVE == "secp256k1"
     content = b"SomeContent"
 
-    encrypted = await tezos_account.encrypt(content)
-    assert isinstance(encrypted, bytes)
-    decrypted = await tezos_account.decrypt(encrypted)
-    assert isinstance(decrypted, bytes)
+    encrypted = await account.encrypt(content)
+    assert type(encrypted) == bytes
+    decrypted = await account.decrypt(encrypted)
+    assert type(decrypted) == bytes
     assert content == decrypted
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/test_remote_account.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_remote_account.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from unittest.mock import patch
 
 import pytest
 
-from aleph_client.chains.ethereum import ETHAccount
-from aleph_client.chains.remote import AccountProperties, RemoteAccount
+from aleph.sdk.chains.ethereum import ETHAccount
+from aleph.sdk.chains.remote import AccountProperties, RemoteAccount
 
 
 @pytest.mark.asyncio
 async def test_remote_storage():
     host = "http://localhost:8888"
     private_key = (
         b"xRR\xd4P\xdb9\x93(U\xa7\xd5\x81\xba\xc7\x9fiT"
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/test_utils.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     ForgetMessage,
     MessageType,
     PostMessage,
     ProgramMessage,
     StoreMessage,
 )
 
-from aleph_client.utils import get_message_type_value
+from aleph.sdk.utils import get_message_type_value
 
 
 def test_get_message_type_value():
     assert get_message_type_value(PostMessage) == MessageType.post
     assert get_message_type_value(AggregateMessage) == MessageType.aggregate
     assert get_message_type_value(StoreMessage) == MessageType.store
     assert get_message_type_value(ProgramMessage) == MessageType.program
```

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/test_vm_app.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_vm_app.py`

 * *Files identical despite different names*

### Comparing `aleph-sdk-python-0.6.0b1/tests/unit/test_vm_cache.py` & `aleph-sdk-python-0.7.0b1/tests/unit/test_vm_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import pytest
 
-from aleph_client.vm.cache import TestVmCache, sanitize_cache_key
+from aleph.sdk.vm.cache import TestVmCache, sanitize_cache_key
 
 
 @pytest.mark.asyncio
 async def test_local_vm_cache():
     cache = TestVmCache()
     assert (await cache.get("doesnotexist")) is None
-    assert len(await (cache.keys())) == 0
+    assert len(await cache.keys()) == 0
     key = "thisdoesexist"
     value = "yay, I exist!"
     await cache.set(key, value)
     cached_value = await cache.get(key)
     assert cached_value is not None
     assert cached_value.decode() == value
     assert (await cache.keys())[0] == key
     assert (await cache.keys("*exist"))[0] == key
     await cache.delete(key)
     assert (await cache.get(key)) is None
-    assert len(await (cache.keys())) == 0
+    assert len(await cache.keys()) == 0
 
 
 def test_sanitize_cache_keys():
     assert sanitize_cache_key("abc")
     assert sanitize_cache_key("abc123")
     assert sanitize_cache_key("abc_123")
     with pytest.raises(ValueError):
```

