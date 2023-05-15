# Comparing `tmp/mo_sql_parsing-9.377.23123-py2.py3-none-any.whl.zip` & `tmp/mo_sql_parsing-9.386.23135-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 38258 bytes, number of entries: 13
+Zip file size: 38297 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     2597 b- defN 22-Dec-18 22:41 mo_sql_parsing/__init__.py
--rw-rw-rw-  2.0 fat    22229 b- defN 23-Mar-26 12:53 mo_sql_parsing/formatting.py
+-rw-rw-rw-  2.0 fat    22407 b- defN 23-May-15 22:26 mo_sql_parsing/formatting.py
 -rw-rw-rw-  2.0 fat    10666 b- defN 23-May-03 23:07 mo_sql_parsing/keywords.py
--rw-rw-rw-  2.0 fat    33442 b- defN 23-May-01 12:37 mo_sql_parsing/sql_parser.py
+-rw-rw-rw-  2.0 fat    33444 b- defN 23-May-15 22:26 mo_sql_parsing/sql_parser.py
 -rw-rw-rw-  2.0 fat     7321 b- defN 23-Mar-26 12:53 mo_sql_parsing/types.py
--rw-rw-rw-  2.0 fat    22945 b- defN 23-Apr-14 10:14 mo_sql_parsing/utils.py
+-rw-rw-rw-  2.0 fat    22999 b- defN 23-May-15 22:26 mo_sql_parsing/utils.py
 -rw-rw-rw-  2.0 fat     2987 b- defN 23-Mar-26 12:53 mo_sql_parsing/windows.py
--rw-rw-rw-  2.0 fat    15922 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9345 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1134 b- defN 23-May-03 23:07 mo_sql_parsing-9.377.23123.dist-info/RECORD
-13 files, 128715 bytes uncompressed, 36352 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat    15922 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9345 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/zip-safe
+?rw-rw-r--  2.0 fat     1134 b- defN 23-May-15 22:26 mo_sql_parsing-9.386.23135.dist-info/RECORD
+13 files, 128949 bytes uncompressed, 36391 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mo_sql_parsing/utils.py
 Comment: 
 
 Filename: mo_sql_parsing/windows.py
 Comment: 
 
-Filename: mo_sql_parsing-9.377.23123.dist-info/LICENSE
+Filename: mo_sql_parsing-9.386.23135.dist-info/LICENSE
 Comment: 
 
-Filename: mo_sql_parsing-9.377.23123.dist-info/METADATA
+Filename: mo_sql_parsing-9.386.23135.dist-info/METADATA
 Comment: 
 
-Filename: mo_sql_parsing-9.377.23123.dist-info/WHEEL
+Filename: mo_sql_parsing-9.386.23135.dist-info/WHEEL
 Comment: 
 
-Filename: mo_sql_parsing-9.377.23123.dist-info/top_level.txt
+Filename: mo_sql_parsing-9.386.23135.dist-info/top_level.txt
 Comment: 
 
-Filename: mo_sql_parsing-9.377.23123.dist-info/zip-safe
+Filename: mo_sql_parsing-9.386.23135.dist-info/zip-safe
 Comment: 
 
-Filename: mo_sql_parsing-9.377.23123.dist-info/RECORD
+Filename: mo_sql_parsing-9.386.23135.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mo_sql_parsing/formatting.py

```diff
@@ -556,14 +556,17 @@
     def select_distinct(self, json, prec):
         param = ", ".join(self.dispatch(s) for s in listwrap(json["select_distinct"]))
         return f"SELECT DISTINCT {param}"
 
     def from_(self, json, prec):
         is_join = False
         from_ = json["from"]
+        if isinstance(from_, dict) and "literal" in from_:
+            content = ", ".join(self._literal(row) for row in from_["literal"])
+            return f"VALUES {content}"
         if isinstance(from_, dict) and is_set_op & from_.keys():
             source = self.op(from_, precedence["from"])
             return f"FROM {source}"
 
         from_ = listwrap(from_)
         parts = []
         for v in from_:
```

## mo_sql_parsing/sql_parser.py

```diff
@@ -423,15 +423,15 @@
             | assign("select distinct", delimited_list(select_column))
             | assign("select as struct", delimited_list(select_column))
             | assign("select as value", delimited_list(select_column))
             | SELECT + tops + delimited_list(select_column)("select")
         ) + comma
 
         row = (LB + delimited_list(Group(expression)) + RB) / to_row
-        values = VALUES + delimited_list(row) / to_values
+        values = (VALUES + delimited_list(row)) / to_values
 
         window_clause = identifier("name") + AS + (identifier | over_clause)("value")
 
         unordered_sql = Group(
             (values | selection)
             + Optional((FROM + delimited_list(table_source) + ZeroOrMore(join))("from"))
             + Optional(WHERE + expression("where"))
```

## mo_sql_parsing/utils.py

```diff
@@ -610,14 +610,16 @@
 
 def to_union_call(tokens):
     unions = tokens["union"]
     if isinstance(unions, dict):
         return unions
     elif unions.type.parser_name == "unordered_sql":
         output = dict(unions)  # REMOVE THE Group()
+        if not output:
+            output = unions[0]
     else:
         unions = list(unions)
         sources = [unions[i] for i in range(0, len(unions), 2)]
         operators = ["_".join(unions[i]) for i in range(1, len(unions), 2)]
         acc = sources[0]
         last_union = None
         for op, so in list(zip(operators, sources[1:])):
```

## Comparing `mo_sql_parsing-9.377.23123.dist-info/LICENSE` & `mo_sql_parsing-9.386.23135.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mo_sql_parsing-9.377.23123.dist-info/METADATA` & `mo_sql_parsing-9.386.23135.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.377.23123
+Version: 9.386.23135
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Software Development :: Libraries
```

