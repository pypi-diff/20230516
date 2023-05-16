# Comparing `tmp/cmind-1.1.5.tar.gz` & `tmp/cmind-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-1.1.5.tar", last modified: Fri Feb 10 11:17:59 2023, max compression
+gzip compressed data, was "cmind-1.1.6.tar", last modified: Tue May 16 11:03:23 2023, max compression
```

## Comparing `cmind-1.1.5.tar` & `cmind-1.1.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-02-10 11:17:59.371890 cmind-1.1.5/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3143 2023-02-10 11:17:59.371890 cmind-1.1.5/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2437 2022-12-20 17:12:45.000000 cmind-1.1.5/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-02-10 11:17:59.361890 cmind-1.1.5/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-02-10 11:17:05.000000 cmind-1.1.5/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2022-10-08 16:04:22.000000 cmind-1.1.5/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2022-11-09 09:00:00.000000 cmind-1.1.5/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    41081 2022-12-20 17:12:45.000000 cmind-1.1.5/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4213 2023-02-10 11:16:55.000000 cmind-1.1.5/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3189 2022-10-08 16:04:22.000000 cmind-1.1.5/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    22853 2022-12-07 14:14:42.000000 cmind-1.1.5/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2022-10-08 16:04:22.000000 cmind-1.1.5/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-02-10 11:17:59.371890 cmind-1.1.5/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2022-10-08 16:04:22.000000 cmind-1.1.5/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-02-10 11:17:59.361890 cmind-1.1.5/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-02-10 11:17:59.371890 cmind-1.1.5/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1857 2022-12-20 17:12:45.000000 cmind-1.1.5/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2022-11-09 09:00:00.000000 cmind-1.1.5/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3290 2022-12-20 17:12:45.000000 cmind-1.1.5/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2022-10-08 16:04:22.000000 cmind-1.1.5/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8807 2022-12-20 17:12:45.000000 cmind-1.1.5/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2022-12-20 17:12:45.000000 cmind-1.1.5/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-02-10 11:17:59.371890 cmind-1.1.5/cmind/repo/automation/ck/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1019 2022-12-20 17:12:45.000000 cmind-1.1.5/cmind/repo/automation/ck/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2022-11-09 09:00:00.000000 cmind-1.1.5/cmind/repo/automation/ck/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2022-10-08 16:04:22.000000 cmind-1.1.5/cmind/repo/automation/ck/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-02-10 11:17:59.371890 cmind-1.1.5/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1031 2022-12-20 17:12:45.000000 cmind-1.1.5/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2022-11-09 09:00:00.000000 cmind-1.1.5/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-02-10 11:17:59.371890 cmind-1.1.5/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2022-10-08 16:04:22.000000 cmind-1.1.5/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2022-10-08 16:04:22.000000 cmind-1.1.5/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2022-12-20 17:12:45.000000 cmind-1.1.5/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2022-12-20 17:12:45.000000 cmind-1.1.5/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-02-10 11:17:59.371890 cmind-1.1.5/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8770 2022-12-20 17:12:45.000000 cmind-1.1.5/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      295 2022-11-09 09:00:00.000000 cmind-1.1.5/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    29217 2022-12-07 14:14:42.000000 cmind-1.1.5/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2022-10-08 16:04:22.000000 cmind-1.1.5/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2022-10-08 16:04:22.000000 cmind-1.1.5/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    18348 2022-11-15 14:23:42.000000 cmind-1.1.5/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    40730 2022-12-20 17:12:45.000000 cmind-1.1.5/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-02-10 11:17:59.371890 cmind-1.1.5/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3143 2023-02-10 11:17:59.000000 cmind-1.1.5/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1207 2023-02-10 11:17:59.000000 cmind-1.1.5/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-02-10 11:17:59.000000 cmind-1.1.5/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       60 2023-02-10 11:17:59.000000 cmind-1.1.5/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-02-10 11:17:59.000000 cmind-1.1.5/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-02-10 11:17:59.000000 cmind-1.1.5/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-02-10 11:17:59.000000 cmind-1.1.5/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-02-10 11:17:59.371890 cmind-1.1.5/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2668 2022-10-25 15:44:09.000000 cmind-1.1.5/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-16 11:03:23.020871 cmind-1.1.6/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     5112 2023-05-16 11:03:10.000000 cmind-1.1.6/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.010872 cmind-1.1.6/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4908 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    41095 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4213 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3189 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    22853 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.010872 cmind-1.1.6/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.010872 cmind-1.1.6/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1858 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/cmind/repo/automation/ck/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1020 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/ck/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/ck/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/ck/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1032 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.020871 cmind-1.1.6/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8771 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    29217 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    18370 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    40730 2023-05-16 11:03:10.000000 cmind-1.1.6/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-05-16 11:03:23.010872 cmind-1.1.6/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6042 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1207 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       60 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-05-16 11:03:22.000000 cmind-1.1.6/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-05-16 11:03:23.020871 cmind-1.1.6/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2668 2023-05-16 11:03:10.000000 cmind-1.1.6/setup.py
```

### Comparing `cmind-1.1.5/cmind/artifact.py` & `cmind-1.1.6/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/cmind/automation.py` & `cmind-1.1.6/cmind/automation.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         print ('')
         print ('Path to CM repositories:    {}'.format(self.cmind.repos_path))
 
         print ('')
         print ('GitHub for CM developments:        https://github.com/mlcommons/ck/tree/master/cm')
         print ('GitHub for CM automation scripts:  https://github.com/mlcommons/ck/tree/master/cm-mlops')
         print ('Reporting issues and ideas:        https://github.com/mlcommons/ck/issues')
-        print ('Joining the open MLPerf workgroup: https://bit.ly/mlperf-edu-wg')
+        print ('Joining the open MLPerf workgroup: https://cKnowledge.org/mlcommons-taskforce')
 
         return {'return':0}
 
     ############################################################
     def search(self, i):
         """
         Find CM artifacts (slow - we plan to accelerate it in the future using different indexing mechanisms)
```

### Comparing `cmind-1.1.5/cmind/cli.py` & `cmind-1.1.6/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/cmind/config.py` & `cmind-1.1.6/cmind/config.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/cmind/core.py` & `cmind-1.1.6/cmind/core.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/cmind/net.py` & `cmind-1.1.6/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/cmind/repo/automation/automation/README.md` & `cmind-1.1.6/cmind/repo/automation/automation/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on education and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
+* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
```

### Comparing `cmind-1.1.5/cmind/repo/automation/automation/module.py` & `cmind-1.1.6/cmind/repo/automation/automation/module.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,38 @@
     """
 
     ############################################################
     def __init__(self, cmind, automation_file):
         super().__init__(cmind, automation_file)
 
     ############################################################
+    def print_input(self, i):
+        """
+        Print unified CM input.
+
+        Args:
+          (CM input dict): 
+
+          (out) (str): if 'con', output to console
+
+        Returns:
+          (CM return dict):
+
+          * return (int): return code == 0 if no error and >0 if error
+          * (error) (str): error string if return>0
+
+        """
+
+        import json
+        print (json.dumps(i, indent=2))
+
+        return {'return':0}
+
+
+    ############################################################
     def add(self, i):
         """
         Add CM automation.
 
         Args:
           (CM input dict):
```

### Comparing `cmind-1.1.5/cmind/repo/automation/automation/module_dummy.py` & `cmind-1.1.6/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/cmind/repo/automation/automation/module_misc.py` & `cmind-1.1.6/cmind/repo/automation/automation/module_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             line_number+=1
 
         md.append('\n')
 
         # Add maintainers
         md_script_readme.append('### Maintainers')
         md_script_readme.append('')
-        md_script_readme.append('* [Open MLCommons taskforce on education and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)')
+        md_script_readme.append('* [Open MLCommons taskforce on automation and reproducibility](https://cKnowledge.org/mlcommons-taskforce)')
 
 
         # Check README and if it's already automatically generated
         path_readme = os.path.join(path, 'README.md')
         path_readme_extra = os.path.join(path, 'README-extra.md')
 
         if os.path.isfile(path_readme):
```

### Comparing `cmind-1.1.5/cmind/repo/automation/ck/README.md` & `cmind-1.1.6/cmind/repo/automation/ck/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,8 +20,8 @@
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on education and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
+* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
```

### Comparing `cmind-1.1.5/cmind/repo/automation/ck/module.py` & `cmind-1.1.6/cmind/repo/automation/ck/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/cmind/repo/automation/core/README.md` & `cmind-1.1.6/cmind/repo/automation/core/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -20,8 +20,8 @@
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on education and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
+* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
```

### Comparing `cmind-1.1.5/cmind/repo/automation/core/module.py` & `cmind-1.1.6/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/cmind/repo/automation/repo/README.md` & `cmind-1.1.6/cmind/repo/automation/repo/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -220,8 +220,8 @@
                 })
     if r['return']>0:
         print(r['error'])
     ```
 
 ### Maintainers
 
-* [Open MLCommons taskforce on education and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
+* [Open MLCommons taskforce on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/mlperf-education-workgroup.md)
```

### Comparing `cmind-1.1.5/cmind/repo/automation/repo/module.py` & `cmind-1.1.6/cmind/repo/automation/repo/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/cmind/repo.py` & `cmind-1.1.6/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/cmind/repos.py` & `cmind-1.1.6/cmind/repos.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,16 +329,16 @@
 
             if desc!='': meta['desc']=desc
             if prefix!='': meta['prefix']=prefix
 
             must_update_repo_desc = True
 
 
-# GF blocked the following code because if we create a fork of mlcommons@ck for example to octoml@ck
-# and then pull octoml@ck, it attempts to rewrite .cmr.yaml with the new alias which we do not want to do!
+# GF blocked the following code because if we create a fork of mlcommons@ck for example to ctuning@mlcommons-ck
+# and then pull ctuning@mlcommons-ck, it attempts to rewrite .cmr.yaml with the new alias which we do not want to do!
 # We want to keep whatever is in .cmr.yaml to avoid ambiguities ...
 #        else:
 #            # Load meta from the repository
 #            r=utils.load_yaml_and_json(file_name_without_ext=path_to_repo_desc)
 #            if r['return']>0: return r
 #
 #            meta = r['meta']
```

### Comparing `cmind-1.1.5/cmind/utils.py` & `cmind-1.1.6/cmind/utils.py`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/cmind.egg-info/SOURCES.txt` & `cmind-1.1.6/cmind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmind-1.1.5/setup.py` & `cmind-1.1.6/setup.py`

 * *Files identical despite different names*

