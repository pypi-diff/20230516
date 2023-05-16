# Comparing `tmp/tldextract-3.4.1.tar.gz` & `tmp/tldextract-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tldextract-3.4.1.tar", last modified: Wed Apr 26 23:31:34 2023, max compression
+gzip compressed data, was "tldextract-3.4.2.tar", last modified: Tue May 16 19:30:06 2023, max compression
```

## Comparing `tldextract-3.4.1.tar` & `tldextract-3.4.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.373156 tldextract-3.4.1/
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.360626 tldextract-3.4.1/.github/
--rw-r--r--   0 john       (501) staff       (20)       25 2022-06-01 21:35:53.000000 tldextract-3.4.1/.github/FUNDING.yml
--rw-r--r--   0 john       (501) staff       (20)      129 2020-10-23 23:38:03.000000 tldextract-3.4.1/.gitignore
--rw-r--r--   0 john       (501) staff       (20)      469 2023-04-26 23:28:14.000000 tldextract-3.4.1/.travis.yml
--rw-r--r--   0 john       (501) staff       (20)    12995 2023-04-26 23:26:27.000000 tldextract-3.4.1/CHANGELOG.md
--rw-r--r--   0 john       (501) staff       (20)     1522 2020-10-11 21:23:20.000000 tldextract-3.4.1/LICENSE
--rw-r--r--   0 john       (501) staff       (20)      116 2022-04-01 00:16:04.000000 tldextract-3.4.1/MANIFEST.in
--rw-r--r--   0 john       (501) staff       (20)     2177 2023-04-26 23:31:34.373349 tldextract-3.4.1/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)     9874 2023-04-26 23:08:06.000000 tldextract-3.4.1/README.md
--rw-r--r--   0 john       (501) staff       (20)       68 2022-04-01 00:16:04.000000 tldextract-3.4.1/conftest.py
--rw-r--r--   0 john       (501) staff       (20)       37 2022-04-01 00:16:04.000000 tldextract-3.4.1/pytest.ini
--rw-r--r--   0 john       (501) staff       (20)      327 2023-04-26 23:31:34.373990 tldextract-3.4.1/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)     2769 2023-04-26 23:28:16.000000 tldextract-3.4.1/setup.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.364137 tldextract-3.4.1/tests/
--rw-r--r--   0 john       (501) staff       (20)        0 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/__init__.py
--rw-r--r--   0 john       (501) staff       (20)      783 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/cli_test.py
--rw-r--r--   0 john       (501) staff       (20)      428 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/conftest.py
--rw-r--r--   0 john       (501) staff       (20)     1935 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/custom_suffix_test.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.364951 tldextract-3.4.1/tests/fixtures/
--rw-r--r--   0 john       (501) staff       (20)       31 2020-10-11 21:23:20.000000 tldextract-3.4.1/tests/fixtures/fake_suffix_list_fixture.dat
--rw-r--r--   0 john       (501) staff       (20)      248 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/integration_test.py
--rw-r--r--   0 john       (501) staff       (20)    10790 2023-04-10 01:08:44.000000 tldextract-3.4.1/tests/main_test.py
--rw-r--r--   0 john       (501) staff       (20)     3419 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/test_cache.py
--rw-r--r--   0 john       (501) staff       (20)     1539 2023-01-12 01:07:59.000000 tldextract-3.4.1/tests/test_parallel.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.370515 tldextract-3.4.1/tldextract/
--rw-r--r--   0 john       (501) staff       (20)   238022 2023-04-26 18:51:17.000000 tldextract-3.4.1/tldextract/.tld_set_snapshot
--rw-r--r--   0 john       (501) staff       (20)      216 2023-04-10 01:08:44.000000 tldextract-3.4.1/tldextract/__init__.py
--rw-r--r--   0 john       (501) staff       (20)       90 2023-01-12 01:07:59.000000 tldextract-3.4.1/tldextract/__main__.py
--rw-r--r--   0 john       (501) staff       (20)      160 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract/_version.py
--rw-r--r--   0 john       (501) staff       (20)     8717 2023-04-10 01:08:44.000000 tldextract-3.4.1/tldextract/cache.py
--rw-r--r--   0 john       (501) staff       (20)     2415 2023-04-10 01:15:19.000000 tldextract-3.4.1/tldextract/cli.py
--rw-r--r--   0 john       (501) staff       (20)        0 2022-04-01 00:16:04.000000 tldextract-3.4.1/tldextract/py.typed
--rw-r--r--   0 john       (501) staff       (20)     1182 2023-01-12 01:07:59.000000 tldextract-3.4.1/tldextract/remote.py
--rw-r--r--   0 john       (501) staff       (20)     3399 2023-01-12 01:48:06.000000 tldextract-3.4.1/tldextract/suffix_list.py
--rw-r--r--   0 john       (501) staff       (20)    14443 2023-01-12 01:48:06.000000 tldextract-3.4.1/tldextract/tldextract.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2023-04-26 23:31:34.372819 tldextract-3.4.1/tldextract.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     2177 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      783 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)       51 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/entry_points.txt
--rw-r--r--   0 john       (501) staff       (20)       56 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)       11 2023-04-26 23:31:34.000000 tldextract-3.4.1/tldextract.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)      676 2023-04-26 23:28:17.000000 tldextract-3.4.1/tox.ini
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-16 19:30:06.156952 tldextract-3.4.2/
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-16 19:30:06.144838 tldextract-3.4.2/.github/
+-rw-r--r--   0 john       (501) staff       (20)       25 2022-06-05 23:30:19.000000 tldextract-3.4.2/.github/FUNDING.yml
+-rw-r--r--   0 john       (501) staff       (20)      129 2022-05-03 19:53:33.000000 tldextract-3.4.2/.gitignore
+-rw-r--r--   0 john       (501) staff       (20)      469 2023-01-14 03:27:06.000000 tldextract-3.4.2/.travis.yml
+-rw-r--r--   0 john       (501) staff       (20)    13327 2023-05-16 19:28:08.000000 tldextract-3.4.2/CHANGELOG.md
+-rw-r--r--   0 john       (501) staff       (20)     1522 2022-05-03 19:53:33.000000 tldextract-3.4.2/LICENSE
+-rw-r--r--   0 john       (501) staff       (20)      116 2022-05-03 19:53:33.000000 tldextract-3.4.2/MANIFEST.in
+-rw-r--r--   0 john       (501) staff       (20)     2177 2023-05-16 19:30:06.157137 tldextract-3.4.2/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)     9874 2023-05-13 22:04:35.000000 tldextract-3.4.2/README.md
+-rw-r--r--   0 john       (501) staff       (20)       68 2022-05-03 19:53:33.000000 tldextract-3.4.2/conftest.py
+-rw-r--r--   0 john       (501) staff       (20)       37 2022-05-03 19:53:33.000000 tldextract-3.4.2/pytest.ini
+-rw-r--r--   0 john       (501) staff       (20)      327 2023-05-16 19:30:06.157813 tldextract-3.4.2/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)     2769 2023-05-13 22:04:35.000000 tldextract-3.4.2/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-16 19:30:06.148655 tldextract-3.4.2/tests/
+-rw-r--r--   0 john       (501) staff       (20)        0 2021-01-11 20:42:27.000000 tldextract-3.4.2/tests/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)      783 2022-06-05 23:30:19.000000 tldextract-3.4.2/tests/cli_test.py
+-rw-r--r--   0 john       (501) staff       (20)      428 2022-05-03 19:53:33.000000 tldextract-3.4.2/tests/conftest.py
+-rw-r--r--   0 john       (501) staff       (20)     1935 2022-09-20 19:51:12.000000 tldextract-3.4.2/tests/custom_suffix_test.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-16 19:30:06.149040 tldextract-3.4.2/tests/fixtures/
+-rw-r--r--   0 john       (501) staff       (20)       31 2021-01-11 20:42:27.000000 tldextract-3.4.2/tests/fixtures/fake_suffix_list_fixture.dat
+-rw-r--r--   0 john       (501) staff       (20)      248 2022-06-05 23:30:19.000000 tldextract-3.4.2/tests/integration_test.py
+-rw-r--r--   0 john       (501) staff       (20)    13567 2023-05-16 19:20:59.000000 tldextract-3.4.2/tests/main_test.py
+-rw-r--r--   0 john       (501) staff       (20)     3419 2022-06-05 23:30:19.000000 tldextract-3.4.2/tests/test_cache.py
+-rw-r--r--   0 john       (501) staff       (20)     1539 2022-09-17 08:16:28.000000 tldextract-3.4.2/tests/test_parallel.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-16 19:30:06.153927 tldextract-3.4.2/tldextract/
+-rw-r--r--   0 john       (501) staff       (20)   238022 2023-05-13 22:04:35.000000 tldextract-3.4.2/tldextract/.tld_set_snapshot
+-rw-r--r--   0 john       (501) staff       (20)      216 2023-01-27 07:03:29.000000 tldextract-3.4.2/tldextract/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)       90 2022-06-05 23:36:58.000000 tldextract-3.4.2/tldextract/__main__.py
+-rw-r--r--   0 john       (501) staff       (20)      160 2023-05-16 19:30:06.000000 tldextract-3.4.2/tldextract/_version.py
+-rw-r--r--   0 john       (501) staff       (20)     8717 2023-01-27 07:03:29.000000 tldextract-3.4.2/tldextract/cache.py
+-rw-r--r--   0 john       (501) staff       (20)     2415 2023-05-13 22:04:35.000000 tldextract-3.4.2/tldextract/cli.py
+-rw-r--r--   0 john       (501) staff       (20)        0 2022-05-03 19:53:33.000000 tldextract-3.4.2/tldextract/py.typed
+-rw-r--r--   0 john       (501) staff       (20)     1499 2023-05-16 19:20:59.000000 tldextract-3.4.2/tldextract/remote.py
+-rw-r--r--   0 john       (501) staff       (20)     3399 2022-10-03 18:40:04.000000 tldextract-3.4.2/tldextract/suffix_list.py
+-rw-r--r--   0 john       (501) staff       (20)    16315 2023-05-16 19:11:37.000000 tldextract-3.4.2/tldextract/tldextract.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2023-05-16 19:30:06.156663 tldextract-3.4.2/tldextract.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     2177 2023-05-16 19:30:06.000000 tldextract-3.4.2/tldextract.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      783 2023-05-16 19:30:06.000000 tldextract-3.4.2/tldextract.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2023-05-16 19:30:06.000000 tldextract-3.4.2/tldextract.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)       51 2023-05-16 19:30:06.000000 tldextract-3.4.2/tldextract.egg-info/entry_points.txt
+-rw-r--r--   0 john       (501) staff       (20)       56 2023-05-16 19:30:06.000000 tldextract-3.4.2/tldextract.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)       11 2023-05-16 19:30:06.000000 tldextract-3.4.2/tldextract.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)      676 2023-01-14 03:27:06.000000 tldextract-3.4.2/tox.ini
```

### Comparing `tldextract-3.4.1/CHANGELOG.md` & `tldextract-3.4.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 # tldextract Changelog
 
 After upgrading, update your cache file by deleting it or via `tldextract
 --update`.
 
+## 3.4.2 (2023-05-16)
+
+* Bugfixes
+  * Speed up 10-40% on "average" inputs, and even more on pathological inputs, like long subdomains
+    * Optimize `suffix_index()` ([#283](https://github.com/john-kurkowski/tldextract/issues/283))
+    * Optimize netloc extraction ([#284](https://github.com/john-kurkowski/tldextract/issues/284))
+
 ## 3.4.1 (2023-04-26)
 
 * Bugfixes
   * Fix Pyright not finding tldextract public interface ([#279](https://github.com/john-kurkowski/tldextract/issues/279))
   * Fix various Pyright checks
   * Use SPDX license identifier ([#280](https://github.com/john-kurkowski/tldextract/issues/280))
   * Support Python 3.11
```

### Comparing `tldextract-3.4.1/LICENSE` & `tldextract-3.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/PKG-INFO` & `tldextract-3.4.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldextract
-Version: 3.4.1
+Version: 3.4.2
 Summary: Accurately separates a URL's subdomain, domain, and public suffix, using the Public Suffix List (PSL). By default, this includes the public ICANN TLDs and their exceptions. You can optionally support the Public Suffix List's private domains as well.
 Home-page: https://github.com/john-kurkowski/tldextract
 Author: John Kurkowski
 Author-email: john.kurkowski@gmail.com
 License: BSD-3-Clause
 Keywords: tld domain subdomain url parse extract urlparse urlsplit public suffix list publicsuffix publicsuffixlist
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tldextract-3.4.1/README.md` & `tldextract-3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/setup.py` & `tldextract-3.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/tests/cli_test.py` & `tldextract-3.4.2/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/tests/custom_suffix_test.py` & `tldextract-3.4.2/tests/custom_suffix_test.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/tests/test_cache.py` & `tldextract-3.4.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/tests/test_parallel.py` & `tldextract-3.4.2/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/tldextract/.tld_set_snapshot` & `tldextract-3.4.2/tldextract/.tld_set_snapshot`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/tldextract/cache.py` & `tldextract-3.4.2/tldextract/cache.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/tldextract/cli.py` & `tldextract-3.4.2/tldextract/cli.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/tldextract/remote.py` & `tldextract-3.4.2/tldextract/remote.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,50 @@
 "tldextract helpers for testing and fetching remote resources."
 
 import re
 import socket
 from urllib.parse import scheme_chars
 
 IP_RE = re.compile(
-    # pylint: disable-next=line-too-long
-    r"^(([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])\.){3}([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])$"
+    r"^(([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])\.)"
+    r"{3}([0-9]|[1-9][0-9]|1[0-9]{2}|2[0-4][0-9]|25[0-5])$"
 )
 
-SCHEME_RE = re.compile(r"^([" + scheme_chars + "]+:)?//")
+scheme_chars_set = set(scheme_chars)
 
 
 def lenient_netloc(url: str) -> str:
     """Extract the netloc of a URL-like string, similar to the netloc attribute
     returned by urllib.parse.{urlparse,urlsplit}, but extract more leniently,
     without raising errors."""
-
     return (
-        SCHEME_RE.sub("", url)
+        _schemeless_url(url)
         .partition("/")[0]
         .partition("?")[0]
         .partition("#")[0]
-        .split("@")[-1]
+        .rpartition("@")[-1]
         .partition(":")[0]
         .strip()
         .rstrip(".")
     )
 
 
+def _schemeless_url(url: str) -> str:
+    double_slashes_start = url.find("//")
+    if double_slashes_start == 0:
+        return url[2:]
+    if (
+        double_slashes_start < 2
+        or not url[double_slashes_start - 1] == ":"
+        or set(url[: double_slashes_start - 1]) - scheme_chars_set
+    ):
+        return url
+    return url[double_slashes_start + 2 :]
+
+
 def looks_like_ip(maybe_ip: str) -> bool:
     """Does the given str look like an IP address?"""
     if not maybe_ip[0].isdigit():
         return False
 
     try:
         socket.inet_aton(maybe_ip)
```

### Comparing `tldextract-3.4.1/tldextract/suffix_list.py` & `tldextract-3.4.2/tldextract/suffix_list.py`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/tldextract/tldextract.py` & `tldextract-3.4.2/tldextract/tldextract.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,18 +46,17 @@
     >>> # join part only if truthy
     >>> '.'.join(part for part in ext if part)
     '127.0.0.1'
 """
 
 import logging
 import os
-import re
+import urllib.parse
 from functools import wraps
 from typing import FrozenSet, List, NamedTuple, Optional, Sequence, Union
-import urllib.parse
 
 import idna
 
 from .cache import DiskCache, get_cache_dir
 from .remote import IP_RE, lenient_netloc, looks_like_ip
 from .suffix_list import get_suffix_lists
 
@@ -67,16 +66,14 @@
 CACHE_TIMEOUT = os.environ.get("TLDEXTRACT_CACHE_TIMEOUT")
 
 PUBLIC_SUFFIX_LIST_URLS = (
     "https://publicsuffix.org/list/public_suffix_list.dat",
     "https://raw.githubusercontent.com/publicsuffix/list/master/public_suffix_list.dat",
 )
 
-_UNICODE_DOTS_RE = re.compile("[\u002e\u3002\uff0e\uff61]")
-
 
 class ExtractResult(NamedTuple):
     """namedtuple of a URL's subdomain, domain, and suffix."""
 
     subdomain: str
     domain: str
     suffix: str
@@ -247,19 +244,23 @@
         ExtractResult(subdomain='forums', domain='bbc', suffix='co.uk')
         """
         return self._extract_netloc(url.netloc, include_psl_private_domains)
 
     def _extract_netloc(
         self, netloc: str, include_psl_private_domains: Optional[bool]
     ) -> ExtractResult:
-        labels = _UNICODE_DOTS_RE.split(netloc)
+        labels = (
+            netloc.replace("\u3002", "\u002e")
+            .replace("\uff0e", "\u002e")
+            .replace("\uff61", "\u002e")
+            .split(".")
+        )
 
-        translations = [_decode_punycode(label) for label in labels]
         suffix_index = self._get_tld_extractor().suffix_index(
-            translations, include_psl_private_domains=include_psl_private_domains
+            labels, include_psl_private_domains=include_psl_private_domains
         )
 
         suffix = ".".join(labels[suffix_index:])
         if not suffix and netloc and looks_like_ip(netloc):
             return ExtractResult("", netloc, "")
 
         subdomain = ".".join(labels[: suffix_index - 1]) if suffix_index else ""
@@ -345,49 +346,97 @@
         # set the default value
         self.include_psl_private_domains = include_psl_private_domains
         self.public_tlds = public_tlds
         self.private_tlds = private_tlds
         self.tlds_incl_private = frozenset(public_tlds + private_tlds + extra_tlds)
         self.tlds_excl_private = frozenset(public_tlds + extra_tlds)
 
+        public_false_tlds = self.get_false_intermediate_suffixes(public_tlds)
+        private_false_tlds = self.get_false_intermediate_suffixes(private_tlds)
+        extra_false_tlds = self.get_false_intermediate_suffixes(extra_tlds)
+        self.false_tlds_incl_private = frozenset(
+            public_false_tlds + private_false_tlds + extra_false_tlds
+        )
+        self.false_tlds_excl_private = frozenset(public_false_tlds + extra_false_tlds)
+
+    def get_false_intermediate_suffixes(self, tlds: List[str]) -> List[str]:
+        """From list of suffixes, identify false intermediate suffixes.
+
+        Example: If valid TLDs include only ["a.b.c.d", "d"], then
+        ["b.c.d", "c.d"] are false intermediate suffixes.
+        """
+        valid_tlds = set(tlds)
+        false_tlds = set()
+        for tld in valid_tlds:
+            labels = tld.split(".")
+            variants = {".".join(labels[-i:]) for i in range(1, len(labels))}
+            false_tlds.update(variants)
+        return list(false_tlds.difference(valid_tlds))
+
     def tlds(
         self, include_psl_private_domains: Optional[bool] = None
     ) -> FrozenSet[str]:
         """Get the currently filtered list of suffixes."""
         if include_psl_private_domains is None:
             include_psl_private_domains = self.include_psl_private_domains
 
         return (
             self.tlds_incl_private
             if include_psl_private_domains
             else self.tlds_excl_private
         )
 
+    def false_tlds(
+        self, include_psl_private_domains: Optional[bool] = None
+    ) -> FrozenSet[str]:
+        """Get the currently filtered list of false intermediate suffixes."""
+        if include_psl_private_domains is None:
+            include_psl_private_domains = self.include_psl_private_domains
+
+        return (
+            self.false_tlds_incl_private
+            if include_psl_private_domains
+            else self.false_tlds_excl_private
+        )
+
     def suffix_index(
-        self, lower_spl: List[str], include_psl_private_domains: Optional[bool] = None
+        self, spl: List[str], include_psl_private_domains: Optional[bool] = None
     ) -> int:
         """Returns the index of the first suffix label.
         Returns len(spl) if no suffix is found
         """
         tlds = self.tlds(include_psl_private_domains)
-        length = len(lower_spl)
-        for i in range(length):
-            maybe_tld = ".".join(lower_spl[i:])
-            exception_tld = "!" + maybe_tld
-            if exception_tld in tlds:
-                return i + 1
-
-            if maybe_tld in tlds:
-                return i
+        false_tlds = self.false_tlds(include_psl_private_domains)
+        i = len(spl)
+        j = i
+        maybe_tld = ""
+        prev_maybe_tld = ""
+        for label in reversed(spl):
+            maybe_tld = (
+                f"{_decode_punycode(label)}.{maybe_tld}"
+                if maybe_tld
+                else _decode_punycode(label)
+            )
 
-            wildcard_tld = "*." + ".".join(lower_spl[i + 1 :])
-            if wildcard_tld in tlds:
-                return i
+            if "!" + maybe_tld in tlds:
+                return j
+            if "*." + prev_maybe_tld in tlds:
+                return j - 1
 
-        return length
+            if maybe_tld in tlds:
+                j -= 1
+                i = j
+                prev_maybe_tld = maybe_tld
+                continue
+            if maybe_tld in false_tlds:
+                j -= 1
+                prev_maybe_tld = maybe_tld
+                continue
+            break
+        return i
 
 
 def _decode_punycode(label: str) -> str:
     lowered = label.lower()
     looks_like_puny = lowered.startswith("xn--")
     if looks_like_puny:
         try:
```

### Comparing `tldextract-3.4.1/tldextract.egg-info/PKG-INFO` & `tldextract-3.4.2/tldextract.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tldextract
-Version: 3.4.1
+Version: 3.4.2
 Summary: Accurately separates a URL's subdomain, domain, and public suffix, using the Public Suffix List (PSL). By default, this includes the public ICANN TLDs and their exceptions. You can optionally support the Public Suffix List's private domains as well.
 Home-page: https://github.com/john-kurkowski/tldextract
 Author: John Kurkowski
 Author-email: john.kurkowski@gmail.com
 License: BSD-3-Clause
 Keywords: tld domain subdomain url parse extract urlparse urlsplit public suffix list publicsuffix publicsuffixlist
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tldextract-3.4.1/tldextract.egg-info/SOURCES.txt` & `tldextract-3.4.2/tldextract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tldextract-3.4.1/tox.ini` & `tldextract-3.4.2/tox.ini`

 * *Files identical despite different names*

