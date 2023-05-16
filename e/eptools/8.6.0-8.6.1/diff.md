# Comparing `tmp/eptools-8.6.0.tar.gz` & `tmp/eptools-8.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\EasypostLibrary\eptools\dist\tmpjcg97s_5\eptools-8.6.0.tar", last modified: Tue May 16 07:39:47 2023, max compression
+gzip compressed data, was "c:\EasypostLibrary\eptools\dist\tmp9ou_8br9\eptools-8.6.1.tar", last modified: Tue May 16 09:57:57 2023, max compression
```

## Comparing `eptools-8.6.0.tar` & `eptools-8.6.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:47.000000 eptools-8.6.0/
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:46.000000 eptools-8.6.0/eptools/
--rw-rw-rw-   0        0        0      792 2023-04-27 15:46:33.000000 eptools-8.6.0/eptools/configuration.py
--rw-rw-rw-   0        0        0     6386 2023-05-16 07:36:24.000000 eptools-8.6.0/eptools/InvoiceDate.py
--rw-rw-rw-   0        0        0     9497 2023-05-11 09:45:44.000000 eptools-8.6.0/eptools/logger.py
--rw-rw-rw-   0        0        0     2401 2023-03-20 16:11:43.000000 eptools-8.6.0/eptools/mail_factory.py
--rw-rw-rw-   0        0        0    16253 2023-05-15 14:48:46.000000 eptools-8.6.0/eptools/SalesForceApiIntegration.py
--rw-rw-rw-   0        0        0     2305 2023-04-20 09:00:19.000000 eptools-8.6.0/eptools/sf_factory.py
--rw-rw-rw-   0        0        0    12808 2023-02-23 18:24:58.000000 eptools-8.6.0/eptools/slacker.py
--rw-rw-rw-   0        0        0    10443 2023-04-20 15:28:40.000000 eptools-8.6.0/eptools/slack_factory.py
--rw-rw-rw-   0        0        0    12115 2023-05-11 09:30:54.000000 eptools-8.6.0/eptools/SQLFactory.py
--rw-rw-rw-   0        0        0    31294 2023-03-24 15:03:41.000000 eptools-8.6.0/eptools/WindowsServiceBase.py
--rw-rw-rw-   0        0        0        0 2021-06-30 13:43:34.000000 eptools-8.6.0/eptools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:39:47.000000 eptools-8.6.0/eptools.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-16 07:39:46.000000 eptools-8.6.0/eptools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      944 2023-05-16 07:39:46.000000 eptools-8.6.0/eptools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       92 2023-05-16 07:39:46.000000 eptools-8.6.0/eptools.egg-info/requires.txt
--rw-rw-rw-   0        0        0      469 2023-05-16 07:39:46.000000 eptools-8.6.0/eptools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 07:39:46.000000 eptools-8.6.0/eptools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1069 2021-03-05 11:50:38.000000 eptools-8.6.0/LICENSE
--rw-rw-rw-   0        0        0      944 2023-05-16 07:39:47.000000 eptools-8.6.0/PKG-INFO
--rw-rw-rw-   0        0        0      108 2021-03-05 11:44:12.000000 eptools-8.6.0/pyproject.toml
--rw-rw-rw-   0        0        0      500 2022-03-29 12:52:14.000000 eptools-8.6.0/README.md
--rw-rw-rw-   0        0        0      588 2023-05-16 07:39:47.000000 eptools-8.6.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2021-03-05 11:49:21.000000 eptools-8.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:57:56.000000 eptools-8.6.1/
+drwxrwxrwx   0        0        0        0 2023-05-16 09:57:56.000000 eptools-8.6.1/eptools/
+-rw-rw-rw-   0        0        0      792 2023-04-27 15:46:33.000000 eptools-8.6.1/eptools/configuration.py
+-rw-rw-rw-   0        0        0     6386 2023-05-16 07:36:24.000000 eptools-8.6.1/eptools/InvoiceDate.py
+-rw-rw-rw-   0        0        0     9497 2023-05-11 09:45:44.000000 eptools-8.6.1/eptools/logger.py
+-rw-rw-rw-   0        0        0     2401 2023-03-20 16:11:43.000000 eptools-8.6.1/eptools/mail_factory.py
+-rw-rw-rw-   0        0        0    16610 2023-05-16 09:56:30.000000 eptools-8.6.1/eptools/SalesForceApiIntegration.py
+-rw-rw-rw-   0        0        0     2305 2023-04-20 09:00:19.000000 eptools-8.6.1/eptools/sf_factory.py
+-rw-rw-rw-   0        0        0    12808 2023-02-23 18:24:58.000000 eptools-8.6.1/eptools/slacker.py
+-rw-rw-rw-   0        0        0    10443 2023-04-20 15:28:40.000000 eptools-8.6.1/eptools/slack_factory.py
+-rw-rw-rw-   0        0        0    12115 2023-05-11 09:30:54.000000 eptools-8.6.1/eptools/SQLFactory.py
+-rw-rw-rw-   0        0        0    31294 2023-03-24 15:03:41.000000 eptools-8.6.1/eptools/WindowsServiceBase.py
+-rw-rw-rw-   0        0        0        0 2021-06-30 13:43:34.000000 eptools-8.6.1/eptools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:57:56.000000 eptools-8.6.1/eptools.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-16 09:57:56.000000 eptools-8.6.1/eptools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      944 2023-05-16 09:57:56.000000 eptools-8.6.1/eptools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       92 2023-05-16 09:57:56.000000 eptools-8.6.1/eptools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      469 2023-05-16 09:57:56.000000 eptools-8.6.1/eptools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 09:57:56.000000 eptools-8.6.1/eptools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1069 2021-03-05 11:50:38.000000 eptools-8.6.1/LICENSE
+-rw-rw-rw-   0        0        0      944 2023-05-16 09:57:56.000000 eptools-8.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2021-03-05 11:44:12.000000 eptools-8.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0      500 2022-03-29 12:52:14.000000 eptools-8.6.1/README.md
+-rw-rw-rw-   0        0        0      588 2023-05-16 09:57:57.000000 eptools-8.6.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2021-03-05 11:49:21.000000 eptools-8.6.1/setup.py
```

### Comparing `eptools-8.6.0/eptools/configuration.py` & `eptools-8.6.1/eptools/configuration.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.0/eptools/InvoiceDate.py` & `eptools-8.6.1/eptools/InvoiceDate.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.0/eptools/logger.py` & `eptools-8.6.1/eptools/logger.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.0/eptools/mail_factory.py` & `eptools-8.6.1/eptools/mail_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.0/eptools/SalesForceApiIntegration.py` & `eptools-8.6.1/eptools/SalesForceApiIntegration.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from eptools.configuration import *
 import pyodbc
 
 
 apiVersion = 'v46.0'
 token = None
 sf = None
+logs = None
 
 # CONFIGURATION #
 # To use the configuration methods in a function set decorator! #
 def reloadconfig(func):  
     def wrap(*args, **kwargs):
         setglobals(globals())
         getglobals_new_globals = getglobals()
@@ -273,45 +274,54 @@
 
 
 ##
 #
 # PART WORKING BY DATABASE
 #
 
-def getEmailFromDB(client_nr):
+def getEmailFromDB(client_nr, logger = None):
+    global logs
+    if logger:
+        logs = logger
     try: 
         sql = """
                 SELECT EmailMailRoom 
                 FROM [EasyPost].[dbo].[SFAccounts]
                 WHERE CustomerIdPost = {}""".format(client_nr)
         results = []
-        with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json') as sql_factory:
+        with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json', logger = logs) as sql_factory:
             sql_factory.execute(sql)
             result = sql_factory.fetchone()
         return ';'.join(result)
     except Exception as ex:
         print(ex)
  
-def AddressFromDB(client_nr):
+def AddressFromDB(client_nr, logger = None):
+    global logs
+    if logger:
+        logs = logger
     try: 
         sql = """
                 SELECT BillingPostalCode, BillingCity, BillingAddress as BillingStreet, Name
                 FROM [EasyPost].[dbo].[SFAccounts]
                 WHERE CustomerIdPost = {}""".format(client_nr)
         results = []
-        with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json') as sql_factory:
+        with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json', logger = logs) as sql_factory:
             sql_factory.execute(sql)
             columns = [column[0] for column in sql_factory.cursor.description]
             for row in sql_factory.fetchall():
                 results.append(dict(zip(columns, row)))
         return results
     except Exception as ex:
         print(ex)
 
-def getHubAndRound(client_nr):
+def getHubAndRound(client_nr, logger = None):
+    global logs
+    if logger:
+        logs = logger
     try: 
         sql = """
                 DECLARE @CustomerIdPost INT -- replace INT with the data type of your CustomerIdPost column
                 SET @CustomerIdPost = {}
 				SELECT top(1) * FROM (
 					-- PART 1 -- CHECK PickupLocations
 					SELECT CustomerIdPost, Hub,RouteName, P.Name, 'SFPickupLocations' as Location, 1 as Priority
@@ -342,31 +352,34 @@
 					SELECT ch.CustomerId, ch.HubName as Hub, ch.RoundName as RouteName, c.Name, 'CustomerHub' as Location, 99 as Priority
 					FROM EasyPostLogistiek.dbo.CustomerHub ch
 					LEFT JOIN EasyPost.dbo.Companies c on ch.CustomerId=c.Id
 					WHERE ch.CustomerId = @CustomerIdPost
 				) innr
 				order by Priority""".format(client_nr)
         results = []
-        with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json') as sql_factory:
+        with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json', logger = logs) as sql_factory:
             sql_factory.execute(sql)
             columns = [column[0] for column in sql_factory.cursor.description]
             for row in sql_factory.fetchall():
                 results.append(dict(zip(columns, row)))
         return results
     except Exception as ex:
         print(ex)
 
-def getIdByName(client_name):
+def getIdByName(client_name, logger = None):
+    global logs
+    if logger:
+        logs = logger
     try: 
         sql = """
                 SELECT CustomerIdPost
                 FROM [EasyPost].[dbo].[SFAccounts]
                 WHERE Name = '{}'""".format(client_name)
         results = []
-        with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json') as sql_factory:
+        with SQLFactory(SQLConnection.PRINTDB, config_path='c:\Software\Configs\eptools.json', logger = logs) as sql_factory:
             sql_factory.execute(sql)
             columns = [column[0] for column in sql_factory.cursor.description]
             for row in sql_factory.fetchall():
                 results.append(dict(zip(columns, row)))
         return results
     except Exception as ex:
         print(ex)
```

### Comparing `eptools-8.6.0/eptools/sf_factory.py` & `eptools-8.6.1/eptools/sf_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.0/eptools/slacker.py` & `eptools-8.6.1/eptools/slacker.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.0/eptools/slack_factory.py` & `eptools-8.6.1/eptools/slack_factory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.0/eptools/SQLFactory.py` & `eptools-8.6.1/eptools/SQLFactory.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.0/eptools/WindowsServiceBase.py` & `eptools-8.6.1/eptools/WindowsServiceBase.py`

 * *Files identical despite different names*

### Comparing `eptools-8.6.0/eptools.egg-info/PKG-INFO` & `eptools-8.6.1/eptools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptools
-Version: 8.6.0
+Version: 8.6.1
 Summary: EasyPost Tools
 Home-page: UNKNOWN
 Author: Arno De Decker
 Author-email: arno.dedecker@easypost.eu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eptools-8.6.0/LICENSE` & `eptools-8.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eptools-8.6.0/PKG-INFO` & `eptools-8.6.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eptools
-Version: 8.6.0
+Version: 8.6.1
 Summary: EasyPost Tools
 Home-page: UNKNOWN
 Author: Arno De Decker
 Author-email: arno.dedecker@easypost.eu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eptools-8.6.0/setup.cfg` & `eptools-8.6.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 7074 6f6f 6c73 0d0a 7665 7273   = eptools..vers
-00000020: 696f 6e20 3d20 382e 362e 300d 0a61 7574  ion = 8.6.0..aut
+00000020: 696f 6e20 3d20 382e 362e 310d 0a61 7574  ion = 8.6.1..aut
 00000030: 686f 7220 3d20 4172 6e6f 2044 6520 4465  hor = Arno De De
 00000040: 636b 6572 0d0a 6175 7468 6f72 5f65 6d61  cker..author_ema
 00000050: 696c 203d 2061 726e 6f2e 6465 6465 636b  il = arno.dedeck
 00000060: 6572 4065 6173 7970 6f73 742e 6575 0d0a  er@easypost.eu..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 4561  description = Ea
 00000080: 7379 506f 7374 2054 6f6f 6c73 0d0a 6c6f  syPost Tools..lo
 00000090: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
```

