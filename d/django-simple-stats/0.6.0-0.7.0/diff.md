# Comparing `tmp/django-simple-stats-0.6.0.tar.gz` & `tmp/django-simple-stats-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-simple-stats-0.6.0.tar", last modified: Mon May  8 09:29:11 2023, max compression
+gzip compressed data, was "django-simple-stats-0.7.0.tar", last modified: Tue May 16 10:15:04 2023, max compression
```

## Comparing `django-simple-stats-0.6.0.tar` & `django-simple-stats-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 09:29:11.092419 django-simple-stats-0.6.0/
--rw-rw-rw-   0        0        0     1078 2022-03-11 07:15:01.000000 django-simple-stats-0.6.0/LICENSE
--rw-rw-rw-   0        0        0    14026 2023-05-08 09:29:11.091421 django-simple-stats-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    12913 2023-05-08 08:14:06.000000 django-simple-stats-0.6.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-08 09:29:11.083421 django-simple-stats-0.6.0/django_simple_stats.egg-info/
--rw-rw-rw-   0        0        0    14026 2023-05-08 09:29:10.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-05-08 09:29:11.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-08 09:29:10.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-03-11 07:16:38.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-05-08 09:29:10.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-08 09:29:10.000000 django-simple-stats-0.6.0/django_simple_stats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-08 09:29:11.092419 django-simple-stats-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1124 2023-05-08 08:14:12.000000 django-simple-stats-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:29:11.086419 django-simple-stats-0.6.0/simple_stats/
--rw-rw-rw-   0        0        0      235 2023-05-08 08:13:47.000000 django-simple-stats-0.6.0/simple_stats/__init__.py
--rw-rw-rw-   0        0        0     6643 2023-05-08 09:15:43.000000 django-simple-stats-0.6.0/simple_stats/stats.py
-drwxrwxrwx   0        0        0        0 2023-05-08 09:29:11.089422 django-simple-stats-0.6.0/tests/
--rw-rw-rw-   0        0        0      314 2023-05-08 08:11:10.000000 django-simple-stats-0.6.0/tests/test_decl.py
--rw-rw-rw-   0        0        0     1016 2023-05-08 08:44:00.000000 django-simple-stats-0.6.0/tests/test_stats.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:15:04.286631 django-simple-stats-0.7.0/
+-rw-rw-rw-   0        0        0     1078 2022-03-11 07:15:01.000000 django-simple-stats-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0    15191 2023-05-16 10:15:04.285630 django-simple-stats-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14061 2023-05-16 09:58:25.000000 django-simple-stats-0.7.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 10:15:04.266883 django-simple-stats-0.7.0/django_simple_stats.egg-info/
+-rw-rw-rw-   0        0        0    15191 2023-05-16 10:15:04.000000 django-simple-stats-0.7.0/django_simple_stats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-05-16 10:15:04.000000 django-simple-stats-0.7.0/django_simple_stats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 10:15:04.000000 django-simple-stats-0.7.0/django_simple_stats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-03-11 07:16:38.000000 django-simple-stats-0.7.0/django_simple_stats.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-05-16 10:15:04.000000 django-simple-stats-0.7.0/django_simple_stats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-16 10:15:04.000000 django-simple-stats-0.7.0/django_simple_stats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 10:15:04.287629 django-simple-stats-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1124 2023-05-16 09:59:15.000000 django-simple-stats-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:15:04.272022 django-simple-stats-0.7.0/simple_stats/
+-rw-rw-rw-   0        0        0      304 2023-05-16 09:54:42.000000 django-simple-stats-0.7.0/simple_stats/__init__.py
+-rw-rw-rw-   0        0        0     7676 2023-05-16 10:07:08.000000 django-simple-stats-0.7.0/simple_stats/stats.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:15:04.282295 django-simple-stats-0.7.0/tests/
+-rw-rw-rw-   0        0        0      314 2023-05-08 08:11:10.000000 django-simple-stats-0.7.0/tests/test_decl.py
+-rw-rw-rw-   0        0        0     1016 2023-05-08 08:44:00.000000 django-simple-stats-0.7.0/tests/test_stats.py
```

### Comparing `django-simple-stats-0.6.0/LICENSE` & `django-simple-stats-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-simple-stats-0.6.0/PKG-INFO` & `django-simple-stats-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-stats
-Version: 0.6.0
+Version: 0.7.0
 Summary: A django package for creating simple stats from a query
 Home-page: https://github.com/spapas/django-simple-stats
 Author: Serafeim Papastefanos
 Author-email: spapas@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python
@@ -18,22 +18,34 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 .. image:: https://badge.fury.io/py/django-simple-stats.svg
     :target: https://badge.fury.io/py/django-simple-stats
     
+.. image:: https://github.com/spapas/django-simple-stats/actions/workflows/ghtox.yml/badge.svg
+    :target: https://github.com/spapas/django-simple-stats/actions/workflows/ghtox.yml
+    
 django-simple-stats
 -------------------
 
 A django package for creating stats from a query. 
 This package should be compatible with all 
 Django versions > 3.x
 
+You can use something like this:
+
+.. code-block:: python
 
+    class TravelStats(StatSet):
+        total = QueryAggregateSingleStat(label='Total')
+        amount = QueryAggregateSingleStat(label='Total amount', method='sum')
+        port__name = QueryAggregateStat(label='By port', )
+    
+to get something like this:
 
 .. image:: ./showme.png
   :alt: How does it look
 
 Installation
 ============
 
@@ -57,14 +69,18 @@
 
 * The ``choice_aggregate``  / ``ChoiceAggregateStat`` is similar to the ``query_aggregate`` but will use a ``choices`` attribute to return better looking values. This will not return Null values
 
 * The ``choice_aggregate_with_null`` / ``ChoiceAggregateNullStat`` is the same as ``choice_aggregate`` but will return Null values (so you can add a ``(None, "Empty")`` choice to your choices)
 
 * The ``query_aggregate_date`` / ``QueryAggregateDateStat`` is similar to the ``query_aggregate`` but will return the aggregates on a specific date field; use ``what`` to pass ``year``, ``month``, ``day``.
 
+* The ``query_aggregate_datetime`` / ``QueryAggregateDateTimeStat`` is similar to the ``query_aggregate_date`` but will return the aggregates on time also.
+
+* The ``query_aggregate_extract_date`` / ``QueryAggregateExtractDateStat`` is similar to ``query_aggregate_date`` but will use ``Extract`` for the date instead of ``Trunc``. This is useful if you want to group by the month/day/hour etc as a *specific* value, i.e this will group all rows of June on the same row while ``query_aggregate_date`` will differntiate between June 21 and June 22 and June 23.
+
 * Finally, the ``query_aggregate_buckets`` // ``QueryAggregateBucketsStat`` is used to create buckets of values. You'll pass the list of buckets and the query will  return the results that belong in each bucket. The stats module will run individual queries with ``field__gte`` for each value. So for example if you pass ``[100, 50, 10]`` and you have a field ``price`` it will run ``price__gte=100``, ``price__gte=50``, ``price__gte=10`` and return the results.
 
 
 Usage
 =====
 
 Both a declarative (similar to how Django models/forms work) and a functional API can be used.
@@ -306,14 +322,15 @@
         create_xls_resp(response)
         return response
             
 
 Changelog
 =========
 
+* v.0.7.0: Add ``query_aggregate_extract_date`` and ``QueryAggregateExtractDateStat``
 * v.0.6.0: Add tests!
 * v.0.5.1: Allow adding a formatter for the values
 * v.0.5.0: Add declarative API
 * v.0.4.0: Allow the aggregate function to run on a different field using ``aggr_field``
 * v.0.3.1: Fix small bug with ``choice_aggregate_with_null``
 * v.0.3.0: Add ``choice_aggregate_with_null`` and throw if stat kind is not found
 * v.0.2.1: Fix small bug with column aliases
```

### Comparing `django-simple-stats-0.6.0/README.rst` & `django-simple-stats-0.7.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 .. image:: https://badge.fury.io/py/django-simple-stats.svg
     :target: https://badge.fury.io/py/django-simple-stats
     
+.. image:: https://github.com/spapas/django-simple-stats/actions/workflows/ghtox.yml/badge.svg
+    :target: https://github.com/spapas/django-simple-stats/actions/workflows/ghtox.yml
+    
 django-simple-stats
 -------------------
 
 A django package for creating stats from a query. 
 This package should be compatible with all 
 Django versions > 3.x
 
+You can use something like this:
+
+.. code-block:: python
 
+    class TravelStats(StatSet):
+        total = QueryAggregateSingleStat(label='Total')
+        amount = QueryAggregateSingleStat(label='Total amount', method='sum')
+        port__name = QueryAggregateStat(label='By port', )
+    
+to get something like this:
 
 .. image:: ./showme.png
   :alt: How does it look
 
 Installation
 ============
 
@@ -36,14 +48,18 @@
 
 * The ``choice_aggregate``  / ``ChoiceAggregateStat`` is similar to the ``query_aggregate`` but will use a ``choices`` attribute to return better looking values. This will not return Null values
 
 * The ``choice_aggregate_with_null`` / ``ChoiceAggregateNullStat`` is the same as ``choice_aggregate`` but will return Null values (so you can add a ``(None, "Empty")`` choice to your choices)
 
 * The ``query_aggregate_date`` / ``QueryAggregateDateStat`` is similar to the ``query_aggregate`` but will return the aggregates on a specific date field; use ``what`` to pass ``year``, ``month``, ``day``.
 
+* The ``query_aggregate_datetime`` / ``QueryAggregateDateTimeStat`` is similar to the ``query_aggregate_date`` but will return the aggregates on time also.
+
+* The ``query_aggregate_extract_date`` / ``QueryAggregateExtractDateStat`` is similar to ``query_aggregate_date`` but will use ``Extract`` for the date instead of ``Trunc``. This is useful if you want to group by the month/day/hour etc as a *specific* value, i.e this will group all rows of June on the same row while ``query_aggregate_date`` will differntiate between June 21 and June 22 and June 23.
+
 * Finally, the ``query_aggregate_buckets`` // ``QueryAggregateBucketsStat`` is used to create buckets of values. You'll pass the list of buckets and the query will  return the results that belong in each bucket. The stats module will run individual queries with ``field__gte`` for each value. So for example if you pass ``[100, 50, 10]`` and you have a field ``price`` it will run ``price__gte=100``, ``price__gte=50``, ``price__gte=10`` and return the results.
 
 
 Usage
 =====
 
 Both a declarative (similar to how Django models/forms work) and a functional API can be used.
@@ -285,14 +301,15 @@
         create_xls_resp(response)
         return response
             
 
 Changelog
 =========
 
+* v.0.7.0: Add ``query_aggregate_extract_date`` and ``QueryAggregateExtractDateStat``
 * v.0.6.0: Add tests!
 * v.0.5.1: Allow adding a formatter for the values
 * v.0.5.0: Add declarative API
 * v.0.4.0: Allow the aggregate function to run on a different field using ``aggr_field``
 * v.0.3.1: Fix small bug with ``choice_aggregate_with_null``
 * v.0.3.0: Add ``choice_aggregate_with_null`` and throw if stat kind is not found
 * v.0.2.1: Fix small bug with column aliases
```

### Comparing `django-simple-stats-0.6.0/django_simple_stats.egg-info/PKG-INFO` & `django-simple-stats-0.7.0/django_simple_stats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-simple-stats
-Version: 0.6.0
+Version: 0.7.0
 Summary: A django package for creating simple stats from a query
 Home-page: https://github.com/spapas/django-simple-stats
 Author: Serafeim Papastefanos
 Author-email: spapas@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python
@@ -18,22 +18,34 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
 License-File: LICENSE
 
 .. image:: https://badge.fury.io/py/django-simple-stats.svg
     :target: https://badge.fury.io/py/django-simple-stats
     
+.. image:: https://github.com/spapas/django-simple-stats/actions/workflows/ghtox.yml/badge.svg
+    :target: https://github.com/spapas/django-simple-stats/actions/workflows/ghtox.yml
+    
 django-simple-stats
 -------------------
 
 A django package for creating stats from a query. 
 This package should be compatible with all 
 Django versions > 3.x
 
+You can use something like this:
+
+.. code-block:: python
 
+    class TravelStats(StatSet):
+        total = QueryAggregateSingleStat(label='Total')
+        amount = QueryAggregateSingleStat(label='Total amount', method='sum')
+        port__name = QueryAggregateStat(label='By port', )
+    
+to get something like this:
 
 .. image:: ./showme.png
   :alt: How does it look
 
 Installation
 ============
 
@@ -57,14 +69,18 @@
 
 * The ``choice_aggregate``  / ``ChoiceAggregateStat`` is similar to the ``query_aggregate`` but will use a ``choices`` attribute to return better looking values. This will not return Null values
 
 * The ``choice_aggregate_with_null`` / ``ChoiceAggregateNullStat`` is the same as ``choice_aggregate`` but will return Null values (so you can add a ``(None, "Empty")`` choice to your choices)
 
 * The ``query_aggregate_date`` / ``QueryAggregateDateStat`` is similar to the ``query_aggregate`` but will return the aggregates on a specific date field; use ``what`` to pass ``year``, ``month``, ``day``.
 
+* The ``query_aggregate_datetime`` / ``QueryAggregateDateTimeStat`` is similar to the ``query_aggregate_date`` but will return the aggregates on time also.
+
+* The ``query_aggregate_extract_date`` / ``QueryAggregateExtractDateStat`` is similar to ``query_aggregate_date`` but will use ``Extract`` for the date instead of ``Trunc``. This is useful if you want to group by the month/day/hour etc as a *specific* value, i.e this will group all rows of June on the same row while ``query_aggregate_date`` will differntiate between June 21 and June 22 and June 23.
+
 * Finally, the ``query_aggregate_buckets`` // ``QueryAggregateBucketsStat`` is used to create buckets of values. You'll pass the list of buckets and the query will  return the results that belong in each bucket. The stats module will run individual queries with ``field__gte`` for each value. So for example if you pass ``[100, 50, 10]`` and you have a field ``price`` it will run ``price__gte=100``, ``price__gte=50``, ``price__gte=10`` and return the results.
 
 
 Usage
 =====
 
 Both a declarative (similar to how Django models/forms work) and a functional API can be used.
@@ -306,14 +322,15 @@
         create_xls_resp(response)
         return response
             
 
 Changelog
 =========
 
+* v.0.7.0: Add ``query_aggregate_extract_date`` and ``QueryAggregateExtractDateStat``
 * v.0.6.0: Add tests!
 * v.0.5.1: Allow adding a formatter for the values
 * v.0.5.0: Add declarative API
 * v.0.4.0: Allow the aggregate function to run on a different field using ``aggr_field``
 * v.0.3.1: Fix small bug with ``choice_aggregate_with_null``
 * v.0.3.0: Add ``choice_aggregate_with_null`` and throw if stat kind is not found
 * v.0.2.1: Fix small bug with column aliases
```

### Comparing `django-simple-stats-0.6.0/setup.py` & `django-simple-stats-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.rst') as f:
         return f.read()
 
 setup(
     name='django-simple-stats',
-    version='0.6.0',
+    version='0.7.0',
     description="A django package for creating simple stats from a query",
     long_description=readme(),
     author='Serafeim Papastefanos',
     author_email='spapas@gmail.com',
     license='MIT',
     url='https://github.com/spapas/django-simple-stats',
     zip_safe=False,
```

### Comparing `django-simple-stats-0.6.0/simple_stats/stats.py` & `django-simple-stats-0.7.0/simple_stats/stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,17 +6,15 @@
     Max,
     DateField,
     DateTimeField,
     When,
     Case,
     Q,
 )
-from django.db.models.functions import (
-    Trunc,
-)
+from django.db.models.functions import Trunc, Extract
 import copy
 from collections import OrderedDict
 
 
 def get_aggregate_function(name):
     if name == "count":
         return Count
@@ -53,27 +51,50 @@
                 (z.get(field), z["aggr"])
                 for z in qs.values(field)
                 .annotate(aggr=aggr_function(aggr_field))
                 .order_by("-aggr")
                 if z.get(field) is not None
             ]
         elif c["kind"] in ("query_aggregate_date", "query_aggregate_datetime"):
+            def format_date(d, what):
+                if what == 'year':
+                    return d.strftime("%Y")
+                elif what == 'month':
+                    return d.strftime("%Y-%m")
+                elif what == 'day':
+                    return d.strftime("%Y-%m-%d")
+                elif what == 'hour':
+                    return d.strftime("%Y-%m-%d %H")
+                else:
+                    return d 
+
+
             output_field_cls = (
                 DateTimeField if c["kind"] == "query_aggregate_datetime" else DateField
             )
             values = [
-                (getattr(z["aggr"], c["what"]), z["aggr2"])
+                #(getattr(z["aggr"], c["what"]), z["aggr2"])
+                (format_date(z["aggr"], c['what']), z["aggr2"])
                 for z in qs.annotate(
                     aggr=Trunc(field, c["what"], output_field=output_field_cls())
                 )
                 .values("aggr")
                 .annotate(aggr2=aggr_function(aggr_field))
                 .order_by("aggr")
             ]
 
+        elif c["kind"] in ("query_aggregate_extract_date"):
+            values = [
+                (z["aggr"], z["aggr2"])
+                for z in qs.annotate(aggr=Extract(field, c["what"]))
+                .values("aggr")
+                .annotate(aggr2=aggr_function(aggr_field))
+                .order_by("aggr")
+            ]
+
         elif c["kind"] in ["choice_aggregate", "choice_aggregate_with_null"]:
             values = [
                 (get_choice_label(c["choices"], x[field]), x["aggr"])
                 for x in qs.values(field)
                 .annotate(aggr=aggr_function(aggr_field))
                 .distinct()
                 .order_by(("-aggr"))
@@ -155,14 +176,22 @@
     kind = "query_aggregate_single"
 
 
 class QueryAggregateDateStat(StatBase):
     kind = "query_aggregate_date"
 
 
+class QueryAggregateDateTimeStat(StatBase):
+    kind = "query_aggregate_datetime"
+
+
+class QueryAggregateExtractDateStat(StatBase):
+    kind = "query_aggregate_extract_date"
+
+
 class QueryAggregateBucketsStat(StatBase):
     kind = "query_aggregate_buckets"
 
 
 class ChoiceAggregateStat(StatBase):
     kind = "choice_aggregate"
```

### Comparing `django-simple-stats-0.6.0/tests/test_stats.py` & `django-simple-stats-0.7.0/tests/test_stats.py`

 * *Files identical despite different names*

