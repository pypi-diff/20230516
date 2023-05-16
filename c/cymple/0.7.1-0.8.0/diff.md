# Comparing `tmp/cymple-0.7.1.tar.gz` & `tmp/cymple-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cymple-0.7.1.tar", last modified: Thu Mar 30 07:06:27 2023, max compression
+gzip compressed data, was "cymple-0.8.0.tar", last modified: Tue May 16 10:50:55 2023, max compression
```

## Comparing `cymple-0.7.1.tar` & `cymple-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:06:27.117389 cymple-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-30 07:06:15.000000 cymple-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-03-30 07:06:27.117389 cymple-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-03-30 07:06:15.000000 cymple-0.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-30 07:06:15.000000 cymple-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-30 07:06:27.121389 cymple-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-30 07:06:15.000000 cymple-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:06:27.113389 cymple-0.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:06:27.117389 cymple-0.7.1/src/cymple/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-30 07:06:15.000000 cymple-0.7.1/src/cymple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-30 07:06:15.000000 cymple-0.7.1/src/cymple/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35711 2023-03-30 07:06:15.000000 cymple-0.7.1/src/cymple/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-03-30 07:06:15.000000 cymple-0.7.1/src/cymple/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-30 07:06:15.000000 cymple-0.7.1/src/cymple/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 07:06:27.117389 cymple-0.7.1/src/cymple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-03-30 07:06:27.000000 cymple-0.7.1/src/cymple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-30 07:06:27.000000 cymple-0.7.1/src/cymple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 07:06:27.000000 cymple-0.7.1/src/cymple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-30 07:06:27.000000 cymple-0.7.1/src/cymple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:50:55.927164 cymple-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-16 10:50:45.000000 cymple-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-16 10:50:55.927164 cymple-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-16 10:50:45.000000 cymple-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-16 10:50:45.000000 cymple-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-16 10:50:55.927164 cymple-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 10:50:45.000000 cymple-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:50:55.927164 cymple-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:50:55.927164 cymple-0.8.0/src/cymple/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-16 10:50:45.000000 cymple-0.8.0/src/cymple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 10:50:45.000000 cymple-0.8.0/src/cymple/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36759 2023-05-16 10:50:45.000000 cymple-0.8.0/src/cymple/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-16 10:50:45.000000 cymple-0.8.0/src/cymple/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-16 10:50:45.000000 cymple-0.8.0/src/cymple/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:50:55.927164 cymple-0.8.0/src/cymple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-16 10:50:55.000000 cymple-0.8.0/src/cymple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-16 10:50:55.000000 cymple-0.8.0/src/cymple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:50:55.000000 cymple-0.8.0/src/cymple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 10:50:55.000000 cymple-0.8.0/src/cymple.egg-info/top_level.txt
```

### Comparing `cymple-0.7.1/LICENSE` & `cymple-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cymple-0.7.1/PKG-INFO` & `cymple-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cymple
-Version: 0.7.1
+Version: 0.8.0
 Summary: A productivity enhancer for creating Cypher queries in Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # Cymple - Cypher Modular Pythonic Language Extension
 
@@ -141,14 +141,25 @@
 2. Add a json file describing the clause and the method(s) interfaces(s) of the new clause that you would like to add to the builder. If you do it for the first time, take a look at existing json files of currently supported Cypher clauses.
 3. Identify all the existing clauses that can precede your new clause, and add your new clause's name to the 'successors' list of those clauses' JSONs.
 4. Run `python src/cymple/internal/internal_renderer.py`. This script generates a new `builder.py` file with all clauses that were declared in `src/cymple/internal/declarations/`. 
 5. By default, by adding a declaration json file, the `internal_builder.py` script takes the declared clause and generates a method that simply concatenates your new clause to the builder's current query. However, if you need anything more complex than that, you can write your own implementation by creating a new method with your clause's name at `src/cymple/internal/overloads/`. Don't forget to run `python src/cymple/internal/internal_renderer.py` again :)
 6. If you're satisfied with the new clause, add a unit test in `test_clauses.py` and make sure it generates the expected Cypher string. 
 
 ### Generating Documentation
+
+Make sure you run:
+```
+pip install -r requirements-dev.txt
+```
+or
+```
+pip install sphinx
+```
+to proceed.
+
 To generate a new HTML documentation, run:
 ```
 cd docs
 make clean html
 make html
 ```
```

### Comparing `cymple-0.7.1/README.md` & `cymple-0.8.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -133,14 +133,25 @@
 2. Add a json file describing the clause and the method(s) interfaces(s) of the new clause that you would like to add to the builder. If you do it for the first time, take a look at existing json files of currently supported Cypher clauses.
 3. Identify all the existing clauses that can precede your new clause, and add your new clause's name to the 'successors' list of those clauses' JSONs.
 4. Run `python src/cymple/internal/internal_renderer.py`. This script generates a new `builder.py` file with all clauses that were declared in `src/cymple/internal/declarations/`. 
 5. By default, by adding a declaration json file, the `internal_builder.py` script takes the declared clause and generates a method that simply concatenates your new clause to the builder's current query. However, if you need anything more complex than that, you can write your own implementation by creating a new method with your clause's name at `src/cymple/internal/overloads/`. Don't forget to run `python src/cymple/internal/internal_renderer.py` again :)
 6. If you're satisfied with the new clause, add a unit test in `test_clauses.py` and make sure it generates the expected Cypher string. 
 
 ### Generating Documentation
+
+Make sure you run:
+```
+pip install -r requirements-dev.txt
+```
+or
+```
+pip install sphinx
+```
+to proceed.
+
 To generate a new HTML documentation, run:
 ```
 cd docs
 make clean html
 make html
 ```
```

### Comparing `cymple-0.7.1/setup.cfg` & `cymple-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cymple-0.7.1/src/cymple/builder.py` & `cymple-0.8.0/src/cymple/builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         """
         return CallAvailable(self.query + ' CALL')
 
 
 class CaseWhen(Query):
     """A class for representing a "CASE WHEN" clause."""
 
-    def case_when(self, filters: dict, on_true: str, on_false: str, ref_name: str, comparison_operator: str = "=", boolean_operator: str = "AND"):
+    def case_when(self, filters: dict, on_true: str, on_false: str, ref_name: str, comparison_operator: str = "=", boolean_operator: str = "AND", **kwargs):
         """Concatenate a CASE WHEN clause to the query, created from a list of given property filters.
 
         :param filters: A dict representing the set of properties to be filtered
         :type filters: dict
         :param on_true: The query to run when the predicate is true
         :type on_true: str
         :param on_false: The query to run when the predicate is false
@@ -67,19 +67,21 @@
         :param ref_name: The name which is used to refer to the newly filtered object
         :type ref_name: str
         :param comparison_operator: A string operator, according to which the comparison between property values is
             done, e.g. for "=", we get: property.name = property.value, defaults to "="
         :type comparison_operator: str
         :param boolean_operator: The boolean operator to apply between predicates, defaults to "AND"
         :type boolean_operator: str
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: CaseWhenAvailable
         """
-        filt = ' CASE WHEN ' + Properties(filters).to_str(comparison_operator, boolean_operator)
+        filt = ' CASE WHEN ' + Properties(filters).to_str(comparison_operator, boolean_operator, **kwargs)
         filt += f' THEN {on_true} ELSE {on_false} END as {ref_name}'
         return CaseWhenAvailable(self.query + filt)
 
 
 class Create(Query):
     """A class for representing a "CREATE" clause."""
 
@@ -168,38 +170,40 @@
         """
         return MergeAvailable(self.query + ' MERGE')
 
 
 class Node(Query):
     """A class for representing a "NODE" clause."""
 
-    def node(self, labels: Union[List[str], str] = None, ref_name: str = None, properties: dict = None):
+    def node(self, labels: Union[List[str], str] = None, ref_name: str = None, properties: dict = None, **kwargs):
         """Concatenate a graph Node, which may be filtered using any label/s and/or property/properties.
 
         :param labels: The neo4j label (or list of labels) for that node, defaults to None
         :type labels: Union[List[str], str]
         :param ref_name: A reference name to be used later in the rest of the query, defaults to None
         :type ref_name: str
         :param properties: A dict representing the set of properties by which the nodes are filtered, defaults to None
         :type properties: dict
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: NodeAvailable
         """
         if not labels:
             labels_string = ''
         elif isinstance(labels, str):
             labels_string = f': {labels}'
         else:
             labels_string = f': {": ".join(labels).strip()}'
 
         if not properties:
             property_string = ''
         else:
-            property_string = f' {{{str(Properties(properties))}}}'
+            property_string = f' {{{Properties(properties).to_str(**kwargs)}}}'
 
         ref_name = ref_name or ''
 
         query = self.query
         if not (query.endswith('-') or query.endswith('>') or query.endswith('<')):
             query += ' '
 
@@ -210,38 +214,40 @@
 
         return NodeAvailable(query)
 
 
 class NodeAfterMerge(Query):
     """A class for representing a "NODE AFTER MERGE" clause."""
 
-    def node(self, labels: Union[List[str], str] = None, ref_name: str = None, properties: dict = None):
+    def node(self, labels: Union[List[str], str] = None, ref_name: str = None, properties: dict = None, **kwargs):
         """Concatenate a graph Node, which may be filtered using any label/s and/or property/properties.
 
         :param labels: The neo4j label (or list of labels) for that node, defaults to None
         :type labels: Union[List[str], str]
         :param ref_name: A reference name to be used later in the rest of the query, defaults to None
         :type ref_name: str
         :param properties: A dict representing the set of properties by which the nodes are filtered, defaults to None
         :type properties: dict
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: NodeAfterMergeAvailable
         """
         if not labels:
             labels_string = ''
         elif isinstance(labels, str):
             labels_string = f': {labels}'
         else:
             labels_string = f': {": ".join(labels).strip()}'
 
         if not properties:
             property_string = ''
         else:
-            property_string = f' {{{str(Properties(properties))}}}'
+            property_string = f' {{{Properties(properties).to_str(**kwargs)}}}'
 
         ref_name = ref_name or ''
 
         query = self.query
         if not (query.endswith('-') or query.endswith('>') or query.endswith('<')):
             query += ' '
 
@@ -348,61 +354,67 @@
         ret = f" {literal_procedure}"
         return ProcedureAvailable(self.query + ret)
 
 
 class Relation(Query):
     """A class for representing a "RELATION" clause."""
 
-    def related(self, label: str = None, ref_name: str = None, properties: dict = None):
+    def related(self, label: str = None, ref_name: str = None, properties: dict = None, **kwargs):
         """Concatenate an undirectional (i.e. --) graph Relationship, which may be filtered.
 
         :param label: The relationship label (type) in the DB, defaults to None
         :type label: str
         :param ref_name: A reference name to be used later in the rest of the query, defaults to None
         :type ref_name: str
         :param properties: A dict representing the set of properties by which the relationship is filtered, defaults to
             None
         :type properties: dict
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAvailable
         """
-        return RelationAvailable(self.query + self._directed_relation('none', label, ref_name, properties))
+        return RelationAvailable(self.query + self._directed_relation('none', label, ref_name, properties, **kwargs))
 
-    def related_to(self, label: str = None, ref_name: str = None, properties: dict = {}):
+    def related_to(self, label: str = None, ref_name: str = None, properties: dict = {}, **kwargs):
         """Concatenate a forward (i.e. -->) graph Relationship, which may be filtered.
 
         :param label: The relationship label (type) in the DB, defaults to None
         :type label: str
         :param ref_name: A reference name to be used later in the rest of the query, defaults to None
         :type ref_name: str
         :param properties: A dict representing the set of properties by which the relationship is filtered, defaults to
             {}
         :type properties: dict
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAvailable
         """
-        return RelationAvailable(self.query + self._directed_relation('forward', label, ref_name, properties))
+        return RelationAvailable(self.query + self._directed_relation('forward', label, ref_name, properties, **kwargs))
 
-    def related_from(self, label: str = None, ref_name: str = None, properties: dict = {}):
+    def related_from(self, label: str = None, ref_name: str = None, properties: dict = {}, **kwargs):
         """Concatenate a backward (i.e. <--) graph Relationship, which may be filtered.
 
         :param label: The relationship label (type) in the DB, defaults to None
         :type label: str
         :param ref_name: A reference name to be used later in the rest of the query, defaults to None
         :type ref_name: str
         :param properties: A dict representing the set of properties by which the relationship is filtered, defaults to
             {}
         :type properties: dict
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAvailable
         """
-        return RelationAvailable(self.query + self._directed_relation('backward', label, ref_name, properties))
+        return RelationAvailable(self.query + self._directed_relation('backward', label, ref_name, properties, **kwargs))
 
     def related_variable_len(self, min_hops: int = -1, max_hops: int = -1):
         """Concatenate a uni-directional graph Relationship, with a variable path length.
 
         :param min_hops: The minimal desired number of hops (set -1 for maximum boundary only), defaults to -1
         :type min_hops: int
         :param max_hops: The maximal desired number of hops (set -1 for minimal boundary only), defaults to -1
@@ -420,33 +432,35 @@
         if relation_length:
             realtion_str = f'[{relation_length}]'
         else:
             realtion_str = ''
 
         return RelationAvailable(self.query + f'-{realtion_str}-')
 
-    def _directed_relation(self, direction: str, label: str, ref_name: str = None, properties: dict = {}):
+    def _directed_relation(self, direction: str, label: str, ref_name: str = None, properties: dict = {}, **kwargs):
         """Concatenate a graph Relationship (private method).
 
         :param direction: The relationship direction, can one of 'forward', 'backward' - otherwise unidirectional
         :type direction: str
         :param label: The relationship label (type) in the DB
         :type label: str
         :param ref_name: A reference name to be used later in the rest of the query, defaults to None
         :type ref_name: str
         :param properties: A dict representing the set of properties by which the relationship is filtered, defaults to
             {}
         :type properties: dict
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAvailable
         """
         relation_type = '' if label is None else f': {label}'
         relation_ref_name = '' if ref_name is None else f'{ref_name}'
-        relation_properties = f' {{{str(Properties(properties))}}}' if properties else ''
+        relation_properties = f' {{{Properties(properties).to_str(**kwargs)}}}' if properties else ''
 
         if relation_ref_name or relation_type:
             realtion_str = f'[{relation_ref_name}{relation_type}{relation_properties}]'
         else:
             realtion_str = ''
 
         if direction == 'forward':
@@ -456,61 +470,67 @@
 
         return f'-{realtion_str}-'
 
 
 class RelationAfterMerge(Query):
     """A class for representing a "RELATION AFTER MERGE" clause."""
 
-    def related(self, label: str = None, ref_name: str = None, properties: dict = None):
+    def related(self, label: str = None, ref_name: str = None, properties: dict = None, **kwargs):
         """Concatenate an undirectional (i.e. --) graph Relationship, which may be filtered.
 
         :param label: The relationship label (type) in the DB, defaults to None
         :type label: str
         :param ref_name: A reference name to be used later in the rest of the query, defaults to None
         :type ref_name: str
         :param properties: A dict representing the set of properties by which the relationship is filtered, defaults to
             None
         :type properties: dict
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAfterMergeAvailable
         """
-        return RelationAvailable(self.query + self._directed_relation('none', label, ref_name, properties))
+        return RelationAvailable(self.query + self._directed_relation('none', label, ref_name, properties, **kwargs))
 
-    def related_to(self, label: str = None, ref_name: str = None, properties: dict = {}):
+    def related_to(self, label: str = None, ref_name: str = None, properties: dict = {}, **kwargs):
         """Concatenate a forward (i.e. -->) graph Relationship, which may be filtered.
 
         :param label: The relationship label (type) in the DB, defaults to None
         :type label: str
         :param ref_name: A reference name to be used later in the rest of the query, defaults to None
         :type ref_name: str
         :param properties: A dict representing the set of properties by which the relationship is filtered, defaults to
             {}
         :type properties: dict
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAfterMergeAvailable
         """
-        return RelationAvailable(self.query + self._directed_relation('forward', label, ref_name, properties))
+        return RelationAvailable(self.query + self._directed_relation('forward', label, ref_name, properties, **kwargs))
 
-    def related_from(self, label: str = None, ref_name: str = None, properties: dict = {}):
+    def related_from(self, label: str = None, ref_name: str = None, properties: dict = {}, **kwargs):
         """Concatenate a backward (i.e. <--) graph Relationship, which may be filtered.
 
         :param label: The relationship label (type) in the DB, defaults to None
         :type label: str
         :param ref_name: A reference name to be used later in the rest of the query, defaults to None
         :type ref_name: str
         :param properties: A dict representing the set of properties by which the relationship is filtered, defaults to
             {}
         :type properties: dict
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAfterMergeAvailable
         """
-        return RelationAvailable(self.query + self._directed_relation('backward', label, ref_name, properties))
+        return RelationAvailable(self.query + self._directed_relation('backward', label, ref_name, properties, **kwargs))
 
     def related_variable_len(self, min_hops: int = -1, max_hops: int = -1):
         """Concatenate a uni-directional graph Relationship, with a variable path length.
 
         :param min_hops: The minimal desired number of hops (set -1 for maximum boundary only), defaults to -1
         :type min_hops: int
         :param max_hops: The maximal desired number of hops (set -1 for minimal boundary only), defaults to -1
@@ -528,33 +548,35 @@
         if relation_length:
             realtion_str = f'[{relation_length}]'
         else:
             realtion_str = ''
 
         return RelationAvailable(self.query + f'-{realtion_str}-')
 
-    def _directed_relation(self, direction: str, label: str, ref_name: str = None, properties: dict = {}):
+    def _directed_relation(self, direction: str, label: str, ref_name: str = None, properties: dict = {}, **kwargs):
         """Concatenate a graph Relationship (private method).
 
         :param direction: The relationship direction, can one of 'forward', 'backward' - otherwise unidirectional
         :type direction: str
         :param label: The relationship label (type) in the DB
         :type label: str
         :param ref_name: A reference name to be used later in the rest of the query, defaults to None
         :type ref_name: str
         :param properties: A dict representing the set of properties by which the relationship is filtered, defaults to
             {}
         :type properties: dict
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: RelationAfterMergeAvailable
         """
         relation_type = '' if label is None else f': {label}'
         relation_ref_name = '' if ref_name is None else f'{ref_name}'
-        relation_properties = f' {{{str(Properties(properties))}}}' if properties else ''
+        relation_properties = f' {{{Properties(properties).to_str(**kwargs)}}}' if properties else ''
 
         if relation_ref_name or relation_type:
             realtion_str = f'[{relation_ref_name}{relation_type}{relation_properties}]'
         else:
             realtion_str = ''
 
         if direction == 'forward':
@@ -695,52 +717,58 @@
         """
         return UnwindAvailable(self.query + f' UNWIND {variables}')
 
 
 class Where(Query):
     """A class for representing a "WHERE" clause."""
 
-    def where(self, name: str, comparison_operator: str, value: str):
+    def where(self, name: str, comparison_operator: str, value: str, **kwargs):
         """Concatenate a WHERE clause to the query, created as {name} {comparison_operator} {value}. E.g. x = 'abc'.
 
         :param name: The name of the object which is to be used in the comparison
         :type name: str
         :param comparison_operator: A string operator, according to which the comparison between compared object and
             the {value} is done, e.g. for "=", we get: {name} = {value}
         :type comparison_operator: str
         :param value: The value which is compared against
         :type value: str
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: WhereAvailable
         """
-        return self.where_multiple({name: value}, comparison_operator)
+        return self.where_multiple({name: value}, comparison_operator, **kwargs)
 
-    def where_multiple(self, filters: dict, comparison_operator: str = "=", boolean_operator: str = ' AND '):
+    def where_multiple(self, filters: dict, comparison_operator: str = "=", boolean_operator: str = ' AND ', **kwargs):
         """Concatenate a WHERE clause to the query, created from a list of given property filters.
 
         :param filters: A dict representing the set of properties to be filtered
         :type filters: dict
         :param comparison_operator: A string operator, according to which the comparison between property values is
             done, e.g. for "=", we get: property.name = property.value, defaults to "="
         :type comparison_operator: str
         :param boolean_operator: The boolean operator to apply between predicates, defaults to ' AND '
         :type boolean_operator: str
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: WhereAvailable
         """
-        filt = ' WHERE ' + Properties(filters).to_str(comparison_operator, boolean_operator)
+        filt = ' WHERE ' + Properties(filters).to_str(comparison_operator, boolean_operator, **kwargs)
         return WhereAvailable(self.query + filt)
 
-    def where_literal(self, statement: str):
+    def where_literal(self, statement: str, **kwargs):
         """Concatenate a literal WHERE clause to the query.
 
         :param statement: A literal string of the required filter
         :type statement: str
+        :param **kwargs: kwargs
+        :type **kwargs
 
         :return: A Query object with a query that contains the new clause.
         :rtype: WhereAvailable
         """
         filt = ' WHERE ' + statement
         return WhereAvailable(self.query + filt)
```

### Comparing `cymple-0.7.1/src/cymple/typedefs.py` & `cymple-0.8.0/src/cymple/typedefs.py`

 * *Files identical despite different names*

### Comparing `cymple-0.7.1/src/cymple.egg-info/PKG-INFO` & `cymple-0.8.0/src/cymple.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cymple
-Version: 0.7.1
+Version: 0.8.0
 Summary: A productivity enhancer for creating Cypher queries in Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8
 License-File: LICENSE
 
 # Cymple - Cypher Modular Pythonic Language Extension
 
@@ -141,14 +141,25 @@
 2. Add a json file describing the clause and the method(s) interfaces(s) of the new clause that you would like to add to the builder. If you do it for the first time, take a look at existing json files of currently supported Cypher clauses.
 3. Identify all the existing clauses that can precede your new clause, and add your new clause's name to the 'successors' list of those clauses' JSONs.
 4. Run `python src/cymple/internal/internal_renderer.py`. This script generates a new `builder.py` file with all clauses that were declared in `src/cymple/internal/declarations/`. 
 5. By default, by adding a declaration json file, the `internal_builder.py` script takes the declared clause and generates a method that simply concatenates your new clause to the builder's current query. However, if you need anything more complex than that, you can write your own implementation by creating a new method with your clause's name at `src/cymple/internal/overloads/`. Don't forget to run `python src/cymple/internal/internal_renderer.py` again :)
 6. If you're satisfied with the new clause, add a unit test in `test_clauses.py` and make sure it generates the expected Cypher string. 
 
 ### Generating Documentation
+
+Make sure you run:
+```
+pip install -r requirements-dev.txt
+```
+or
+```
+pip install sphinx
+```
+to proceed.
+
 To generate a new HTML documentation, run:
 ```
 cd docs
 make clean html
 make html
 ```
```

