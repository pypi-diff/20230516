# Comparing `tmp/fluent.migrate-0.8.1.tar.gz` & `tmp/fluent.migrate-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fluent.migrate-0.8.1.tar", last modified: Wed Feb 26 18:57:15 2020, max compression
+gzip compressed data, was "dist/fluent.migrate-0.9.tar", last modified: Wed May 13 13:27:32 2020, max compression
```

## Comparing `fluent.migrate-0.8.1.tar` & `fluent.migrate-0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 axelhecht   (501) staff       (20)        0 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/
--rw-r--r--   0 axelhecht   (501) staff       (20)     2789 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/PKG-INFO
-drwxr-xr-x   0 axelhecht   (501) staff       (20)        0 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/fluent/
--rw-r--r--   0 axelhecht   (501) staff       (20)       65 2019-04-13 16:15:48.000000 fluent.migrate-0.8.1/fluent/__init__.py
-drwxr-xr-x   0 axelhecht   (501) staff       (20)        0 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/fluent/migrate/
--rw-r--r--   0 axelhecht   (501) staff       (20)    11324 2019-11-27 14:34:26.000000 fluent.migrate-0.8.1/fluent/migrate/validator.py
--rw-r--r--   0 axelhecht   (501) staff       (20)    19346 2020-02-21 11:34:30.000000 fluent.migrate-0.8.1/fluent/migrate/transforms.py
--rw-r--r--   0 axelhecht   (501) staff       (20)     1865 2020-02-13 09:05:38.000000 fluent.migrate-0.8.1/fluent/migrate/merge.py
--rw-r--r--   0 axelhecht   (501) staff       (20)     2969 2019-11-06 16:31:13.000000 fluent.migrate-0.8.1/fluent/migrate/util.py
--rw-r--r--   0 axelhecht   (501) staff       (20)      151 2019-07-19 10:25:43.000000 fluent.migrate-0.8.1/fluent/migrate/__init__.py
--rw-r--r--   0 axelhecht   (501) staff       (20)    12206 2020-02-26 18:05:45.000000 fluent.migrate-0.8.1/fluent/migrate/_context.py
--rw-r--r--   0 axelhecht   (501) staff       (20)     6209 2020-02-26 18:03:49.000000 fluent.migrate-0.8.1/fluent/migrate/context.py
--rw-r--r--   0 axelhecht   (501) staff       (20)     2736 2019-09-26 15:45:15.000000 fluent.migrate-0.8.1/fluent/migrate/blame.py
--rw-r--r--   0 axelhecht   (501) staff       (20)      267 2019-04-13 16:15:48.000000 fluent.migrate-0.8.1/fluent/migrate/errors.py
--rw-r--r--   0 axelhecht   (501) staff       (20)     5123 2019-11-13 11:09:55.000000 fluent.migrate-0.8.1/fluent/migrate/helpers.py
--rwxr-xr-x   0 axelhecht   (501) staff       (20)     5664 2019-11-27 11:36:20.000000 fluent.migrate-0.8.1/fluent/migrate/tool.py
--rw-r--r--   0 axelhecht   (501) staff       (20)     1577 2019-11-13 11:30:14.000000 fluent.migrate-0.8.1/fluent/migrate/changesets.py
-drwxr-xr-x   0 axelhecht   (501) staff       (20)        0 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/fluent.migrate.egg-info/
--rw-r--r--   0 axelhecht   (501) staff       (20)     2789 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/fluent.migrate.egg-info/PKG-INFO
--rw-r--r--   0 axelhecht   (501) staff       (20)      588 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/fluent.migrate.egg-info/SOURCES.txt
--rw-r--r--   0 axelhecht   (501) staff       (20)      110 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/fluent.migrate.egg-info/entry_points.txt
--rw-r--r--   0 axelhecht   (501) staff       (20)       77 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/fluent.migrate.egg-info/requires.txt
--rw-r--r--   0 axelhecht   (501) staff       (20)        7 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/fluent.migrate.egg-info/top_level.txt
--rw-r--r--   0 axelhecht   (501) staff       (20)        1 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/fluent.migrate.egg-info/dependency_links.txt
--rw-r--r--   0 axelhecht   (501) staff       (20)     1815 2019-11-13 12:47:27.000000 fluent.migrate-0.8.1/README.md
--rw-r--r--   0 axelhecht   (501) staff       (20)      948 2020-02-26 18:56:21.000000 fluent.migrate-0.8.1/setup.py
--rw-r--r--   0 axelhecht   (501) staff       (20)      292 2020-02-26 18:57:15.000000 fluent.migrate-0.8.1/setup.cfg
+drwxr-xr-x   0 axelhecht   (501) staff       (20)        0 2020-05-13 13:27:32.000000 fluent.migrate-0.9/
+-rw-r--r--   0 axelhecht   (501) staff       (20)     2787 2020-05-13 13:27:32.000000 fluent.migrate-0.9/PKG-INFO
+drwxr-xr-x   0 axelhecht   (501) staff       (20)        0 2020-05-13 13:27:32.000000 fluent.migrate-0.9/fluent/
+-rw-r--r--   0 axelhecht   (501) staff       (20)       65 2019-04-13 16:15:48.000000 fluent.migrate-0.9/fluent/__init__.py
+drwxr-xr-x   0 axelhecht   (501) staff       (20)        0 2020-05-13 13:27:32.000000 fluent.migrate-0.9/fluent/migrate/
+-rw-r--r--   0 axelhecht   (501) staff       (20)    11324 2019-11-27 14:34:26.000000 fluent.migrate-0.9/fluent/migrate/validator.py
+-rw-r--r--   0 axelhecht   (501) staff       (20)    21002 2020-05-13 12:56:42.000000 fluent.migrate-0.9/fluent/migrate/transforms.py
+-rw-r--r--   0 axelhecht   (501) staff       (20)     1982 2020-04-14 11:31:03.000000 fluent.migrate-0.9/fluent/migrate/merge.py
+-rw-r--r--   0 axelhecht   (501) staff       (20)     2969 2019-11-06 16:31:13.000000 fluent.migrate-0.9/fluent/migrate/util.py
+-rw-r--r--   0 axelhecht   (501) staff       (20)      151 2019-07-19 10:25:43.000000 fluent.migrate-0.9/fluent/migrate/__init__.py
+-rw-r--r--   0 axelhecht   (501) staff       (20)    12206 2020-02-26 18:05:45.000000 fluent.migrate-0.9/fluent/migrate/_context.py
+-rw-r--r--   0 axelhecht   (501) staff       (20)     6209 2020-02-26 18:03:49.000000 fluent.migrate-0.9/fluent/migrate/context.py
+-rw-r--r--   0 axelhecht   (501) staff       (20)     2736 2019-09-26 15:45:15.000000 fluent.migrate-0.9/fluent/migrate/blame.py
+-rw-r--r--   0 axelhecht   (501) staff       (20)      313 2020-04-14 11:29:43.000000 fluent.migrate-0.9/fluent/migrate/errors.py
+-rw-r--r--   0 axelhecht   (501) staff       (20)     5123 2019-11-13 11:09:55.000000 fluent.migrate-0.9/fluent/migrate/helpers.py
+-rwxr-xr-x   0 axelhecht   (501) staff       (20)     5664 2019-11-27 11:36:20.000000 fluent.migrate-0.9/fluent/migrate/tool.py
+-rw-r--r--   0 axelhecht   (501) staff       (20)     1577 2019-11-13 11:30:14.000000 fluent.migrate-0.9/fluent/migrate/changesets.py
+drwxr-xr-x   0 axelhecht   (501) staff       (20)        0 2020-05-13 13:27:32.000000 fluent.migrate-0.9/fluent.migrate.egg-info/
+-rw-r--r--   0 axelhecht   (501) staff       (20)     2787 2020-05-13 13:27:32.000000 fluent.migrate-0.9/fluent.migrate.egg-info/PKG-INFO
+-rw-r--r--   0 axelhecht   (501) staff       (20)      588 2020-05-13 13:27:32.000000 fluent.migrate-0.9/fluent.migrate.egg-info/SOURCES.txt
+-rw-r--r--   0 axelhecht   (501) staff       (20)      110 2020-05-13 13:27:32.000000 fluent.migrate-0.9/fluent.migrate.egg-info/entry_points.txt
+-rw-r--r--   0 axelhecht   (501) staff       (20)       77 2020-05-13 13:27:32.000000 fluent.migrate-0.9/fluent.migrate.egg-info/requires.txt
+-rw-r--r--   0 axelhecht   (501) staff       (20)        7 2020-05-13 13:27:32.000000 fluent.migrate-0.9/fluent.migrate.egg-info/top_level.txt
+-rw-r--r--   0 axelhecht   (501) staff       (20)        1 2020-05-13 13:27:32.000000 fluent.migrate-0.9/fluent.migrate.egg-info/dependency_links.txt
+-rw-r--r--   0 axelhecht   (501) staff       (20)     1815 2019-11-13 12:47:27.000000 fluent.migrate-0.9/README.md
+-rw-r--r--   0 axelhecht   (501) staff       (20)      946 2020-05-13 13:05:10.000000 fluent.migrate-0.9/setup.py
+-rw-r--r--   0 axelhecht   (501) staff       (20)      292 2020-05-13 13:27:32.000000 fluent.migrate-0.9/setup.cfg
```

### Comparing `fluent.migrate-0.8.1/PKG-INFO` & `fluent.migrate-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluent.migrate
-Version: 0.8.1
+Version: 0.9
 Summary: Toolchain to migrate legacy translation to Fluent.
 Home-page: https://hg.mozilla.org/l10n/fluent-migration/
 Author: Mozilla
 Author-email: l10n-drivers@mozilla.org
 License: APL 2
 Description: Fluent Migration Tools
         ======================
```

### Comparing `fluent.migrate-0.8.1/fluent/migrate/validator.py` & `fluent.migrate-0.9/fluent/migrate/validator.py`

 * *Files identical despite different names*

### Comparing `fluent.migrate-0.8.1/fluent/migrate/transforms.py` & `fluent.migrate-0.9/fluent/migrate/transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -278,41 +278,44 @@
       - in DTD files: known named, decimal, and hexadecimal HTML entities.
 
     Consult the following files for the list of known named HTML entities:
 
     https://github.com/python/cpython/blob/2.7/Lib/htmlentitydefs.py
     https://github.com/python/cpython/blob/3.6/Lib/html/entities.py
 
+    By default, leading and trailing whitespace on each line as well as
+    leading and trailing empty lines will be stripped from the source
+    translation's content. Set `trim=False` to disable this behavior.
     """
 
-    def __init__(self, path, key, trim=False):
+    def __init__(self, path, key, trim=None):
         if path.endswith('.ftl'):
             raise NotSupportedError(
                 'Please use COPY_PATTERN to migrate from Fluent files '
                 '({})'.format(path))
 
         super(LegacySource, self).__init__(path, key)
         self.trim = trim
 
     def get_text(self, ctx):
         return ctx.get_legacy_source(self.path, self.key)
 
     @staticmethod
     def trim_text(text):
-        # strip leading white-space
+        # strip leading white-space from each line
         text = re.sub('^[ \t]+', '', text, flags=re.M)
-        # strip trailing white-space
+        # strip trailing white-space from each line
         text = re.sub('[ \t]+$', '', text, flags=re.M)
         # strip leading and trailing empty lines
         text = text.strip('\r\n')
         return text
 
     def __call__(self, ctx):
         text = self.get_text(ctx)
-        if self.trim:
+        if self.trim is not False:
             text = self.trim_text(text)
         return FTL.TextElement(text)
 
 
 class COPY(LegacySource):
     """Create a Pattern with the translation value from the given source."""
 
@@ -521,18 +524,58 @@
             ]
         )
 
         return Transform.pattern_of(select)
 
 
 class CONCAT(Transform):
-    """Create a new Pattern from Patterns, PatternElements and Expressions."""
+    """Create a new Pattern from Patterns, PatternElements and Expressions.
+
+    When called with at least two elements, `CONCAT` disables the trimming
+    behavior of the elements which are subclasses of `LegacySource` by
+    setting `trim=False`, unless `trim` has already been set explicitly. The
+    following two `CONCAT` calls are equivalent:
+
+       CONCAT(
+           FTL.TextElement("Hello"),
+           COPY("file.properties", "hello")
+       )
+
+       CONCAT(
+           FTL.TextElement("Hello"),
+           COPY("file.properties", "hello", trim=False)
+       )
+
+    Set `trim=True` explicitly to force trimming:
+
+       CONCAT(
+           FTL.TextElement("Hello "),
+           COPY("file.properties", "hello", trim=True)
+       )
+
+    When called with a single element and when the element is a subclass of
+    `LegacySource`, the trimming behavior is not changed. The following two
+    transforms are equivalent:
+
+       CONCAT(COPY("file.properties", "hello"))
+
+       COPY("file.properties", "hello")
+    """
 
     def __init__(self, *elements, **kwargs):
         # We want to support both passing elements as *elements in the
         # migration specs and as elements=[]. The latter is used by
         # FTL.BaseNode.traverse when it recreates the traversed node using its
         # attributes as kwargs.
         self.elements = list(kwargs.get('elements', elements))
 
+        # We want to make CONCAT(COPY()) equivalent to COPY() so that it's
+        # always safe (no-op) to wrap transforms in a CONCAT. This is used by
+        # the implementation of transforms_from.
+        if len(self.elements) > 1:
+            for elem in self.elements:
+                # Only change trim if it hasn't been set explicitly.
+                if isinstance(elem, LegacySource) and elem.trim is None:
+                    elem.trim = False
+
     def __call__(self, ctx):
         return Transform.pattern_of(*self.elements)
```

### Comparing `fluent.migrate-0.8.1/fluent/migrate/merge.py` & `fluent.migrate-0.9/fluent/migrate/merge.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # coding=utf8
 from __future__ import unicode_literals
 from __future__ import absolute_import
 
 import fluent.syntax.ast as FTL
 
+from .errors import SkipTransform
 from .transforms import evaluate
 from .util import get_message, get_transform
 
 
 def merge_resource(ctx, reference, current, transforms, in_changeset):
     """Transform legacy translations into FTL.
 
@@ -46,11 +47,14 @@
         transform = get_transform(transforms, ident)
 
         # Make sure this message is supposed to be migrated as part of the
         # current changeset.
         if transform is not None and in_changeset(ident):
             if transform.comment is None:
                 transform.comment = entry.comment
-            return evaluate(ctx, transform)
+            try:
+                return evaluate(ctx, transform)
+            except SkipTransform:
+                return None
 
     body = merge_body(reference.body)
     return FTL.Resource(body)
```

### Comparing `fluent.migrate-0.8.1/fluent/migrate/util.py` & `fluent.migrate-0.9/fluent/migrate/util.py`

 * *Files identical despite different names*

### Comparing `fluent.migrate-0.8.1/fluent/migrate/_context.py` & `fluent.migrate-0.9/fluent/migrate/_context.py`

 * *Files identical despite different names*

### Comparing `fluent.migrate-0.8.1/fluent/migrate/context.py` & `fluent.migrate-0.9/fluent/migrate/context.py`

 * *Files identical despite different names*

### Comparing `fluent.migrate-0.8.1/fluent/migrate/blame.py` & `fluent.migrate-0.9/fluent/migrate/blame.py`

 * *Files identical despite different names*

### Comparing `fluent.migrate-0.8.1/fluent/migrate/helpers.py` & `fluent.migrate-0.9/fluent/migrate/helpers.py`

 * *Files identical despite different names*

### Comparing `fluent.migrate-0.8.1/fluent/migrate/tool.py` & `fluent.migrate-0.9/fluent/migrate/tool.py`

 * *Files identical despite different names*

### Comparing `fluent.migrate-0.8.1/fluent/migrate/changesets.py` & `fluent.migrate-0.9/fluent/migrate/changesets.py`

 * *Files identical despite different names*

### Comparing `fluent.migrate-0.8.1/fluent.migrate.egg-info/PKG-INFO` & `fluent.migrate-0.9/fluent.migrate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluent.migrate
-Version: 0.8.1
+Version: 0.9
 Summary: Toolchain to migrate legacy translation to Fluent.
 Home-page: https://hg.mozilla.org/l10n/fluent-migration/
 Author: Mozilla
 Author-email: l10n-drivers@mozilla.org
 License: APL 2
 Description: Fluent Migration Tools
         ======================
```

### Comparing `fluent.migrate-0.8.1/fluent.migrate.egg-info/SOURCES.txt` & `fluent.migrate-0.9/fluent.migrate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluent.migrate-0.8.1/README.md` & `fluent.migrate-0.9/README.md`

 * *Files identical despite different names*

### Comparing `fluent.migrate-0.8.1/setup.py` & `fluent.migrate-0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(
     name='fluent.migrate',
-    version='0.8.1',
+    version='0.9',
     description='Toolchain to migrate legacy translation to Fluent.',
     author='Mozilla',
     author_email='l10n-drivers@mozilla.org',
     license='APL 2',
     url='https://hg.mozilla.org/l10n/fluent-migration/',
     keywords=['fluent', 'localization', 'l10n'],
     classifiers=[
@@ -16,15 +16,15 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.7',
     ],
     packages=['fluent', 'fluent.migrate'],
     install_requires=[
-        'compare-locales >=7.6, <7.7',
+        'compare-locales >=7.6, <8.1',
         'fluent.syntax >=0.17.0, <0.18',
         'six',
     ],
     extras_require={
         'hg': ['python-hglib',],
     },
     tests_require=[
```

