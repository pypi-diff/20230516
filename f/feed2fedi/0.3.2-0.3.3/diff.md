# Comparing `tmp/feed2fedi-0.3.2.tar.gz` & `tmp/feed2fedi-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed2fedi-0.3.2.tar", last modified: Sat Mar  4 06:54:26 2023, max compression
+gzip compressed data, was "feed2fedi-0.3.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `feed2fedi-0.3.2.tar` & `feed2fedi-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4086 2023-03-04 06:38:58.171720 feed2fedi-0.3.2/README.rst
--rw-r--r--   0        0        0     3538 2023-03-04 06:38:58.171720 feed2fedi-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      295 2023-03-04 06:38:58.171720 feed2fedi-0.3.2/src/feed2fedi/__init__.py
--rw-r--r--   0        0        0     3393 2023-03-04 06:38:58.171720 feed2fedi-0.3.2/src/feed2fedi/app.py
--rw-r--r--   0        0        0     4434 2023-03-04 06:38:58.171720 feed2fedi-0.3.2/src/feed2fedi/collect.py
--rw-r--r--   0        0        0    18493 2023-03-04 06:38:58.171720 feed2fedi-0.3.2/src/feed2fedi/control.py
--rw-r--r--   0        0        0     4040 2023-03-04 06:38:58.171720 feed2fedi-0.3.2/src/feed2fedi/publish.py
--rw-r--r--   0        0        0     5519 1970-01-01 00:00:00.000000 feed2fedi-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     4081 2023-05-16 01:22:05.288705 feed2fedi-0.3.3/README.rst
+-rw-r--r--   0        0        0     3538 2023-05-16 01:22:05.292705 feed2fedi-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-05-16 01:22:05.292705 feed2fedi-0.3.3/src/feed2fedi/__init__.py
+-rw-r--r--   0        0        0     3393 2023-05-16 01:22:05.292705 feed2fedi-0.3.3/src/feed2fedi/app.py
+-rw-r--r--   0        0        0     4434 2023-05-16 01:22:05.292705 feed2fedi-0.3.3/src/feed2fedi/collect.py
+-rw-r--r--   0        0        0    18493 2023-05-16 01:22:05.292705 feed2fedi-0.3.3/src/feed2fedi/control.py
+-rw-r--r--   0        0        0     4040 2023-05-16 01:22:05.292705 feed2fedi-0.3.3/src/feed2fedi/publish.py
+-rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 feed2fedi-0.3.3/PKG-INFO
```

### Comparing `feed2fedi-0.3.2/README.rst` & `feed2fedi-0.3.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 During the first run it will prompt for some values and create a `config.ini` file with sensible starting settings.
 
 Then edit the `config.ini` file and add the RSS/ATOM feed in the feeds section and remove the sample feed.
 
 Support Feed2Fedi
 -----------------
 
-A big thank you to the good folk over at `MastIndia`_ who have allowed me to test Feed2Fedi against their
+A big thank you to the good folk over at `CharCha`_ who have allowed me to test Feed2Fedi against their
 instance that is based on `Rebased`_ and `Soapbox`_.
 
 
 There are a number of ways you can support Feed2Fedi:
 
 - Create an issue with problems or ideas you have with/for Feed2Fedi
 - You can `buy me a coffee`_.
@@ -68,15 +68,15 @@
 
 License
 -------
 
 Feed2Fedi is licensed under the `GNU Affero General Public License v3.0`_
 
 
-.. _MastIndia: https://mastindia.co
+.. _CharCha: https://charcha.cc/
 .. _Soapbox: https://soapbox.pub/
 .. _Rebased: https://gitlab.com/soapbox-pub/rebased
 .. _feed2toot: https://gitlab.com/chaica/feed2toot
 .. _Fediverse: https://fediverse.party/
 .. _Fedinesia: https://pypi.org/project/fedinesia/
 .. _Healthchecks: https://healthchecks.io/
 .. _buy me a coffee: https://www.buymeacoffee.com/marvin8
```

### Comparing `feed2fedi-0.3.2/pyproject.toml` & `feed2fedi-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `feed2fedi-0.3.2/src/feed2fedi/app.py` & `feed2fedi-0.3.3/src/feed2fedi/app.py`

 * *Files identical despite different names*

### Comparing `feed2fedi-0.3.2/src/feed2fedi/collect.py` & `feed2fedi-0.3.3/src/feed2fedi/collect.py`

 * *Files identical despite different names*

### Comparing `feed2fedi-0.3.2/src/feed2fedi/control.py` & `feed2fedi-0.3.3/src/feed2fedi/control.py`

 * *Files identical despite different names*

### Comparing `feed2fedi-0.3.2/src/feed2fedi/publish.py` & `feed2fedi-0.3.3/src/feed2fedi/publish.py`

 * *Files identical despite different names*

### Comparing `feed2fedi-0.3.2/PKG-INFO` & `feed2fedi-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feed2fedi
-Version: 0.3.2
+Version: 0.3.3
 Summary: Makes posts to Fediverse from one or more feeds
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
@@ -76,15 +76,15 @@
 During the first run it will prompt for some values and create a `config.ini` file with sensible starting settings.
 
 Then edit the `config.ini` file and add the RSS/ATOM feed in the feeds section and remove the sample feed.
 
 Support Feed2Fedi
 -----------------
 
-A big thank you to the good folk over at `MastIndia`_ who have allowed me to test Feed2Fedi against their
+A big thank you to the good folk over at `CharCha`_ who have allowed me to test Feed2Fedi against their
 instance that is based on `Rebased`_ and `Soapbox`_.
 
 
 There are a number of ways you can support Feed2Fedi:
 
 - Create an issue with problems or ideas you have with/for Feed2Fedi
 - You can `buy me a coffee`_.
@@ -100,15 +100,15 @@
 
 License
 -------
 
 Feed2Fedi is licensed under the `GNU Affero General Public License v3.0`_
 
 
-.. _MastIndia: https://mastindia.co
+.. _CharCha: https://charcha.cc/
 .. _Soapbox: https://soapbox.pub/
 .. _Rebased: https://gitlab.com/soapbox-pub/rebased
 .. _feed2toot: https://gitlab.com/chaica/feed2toot
 .. _Fediverse: https://fediverse.party/
 .. _Fedinesia: https://pypi.org/project/fedinesia/
 .. _Healthchecks: https://healthchecks.io/
 .. _buy me a coffee: https://www.buymeacoffee.com/marvin8
```

