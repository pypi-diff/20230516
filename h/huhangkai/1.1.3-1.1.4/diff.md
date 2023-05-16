# Comparing `tmp/huhangkai-1.1.3.tar.gz` & `tmp/huhangkai-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhangkai-1.1.3.tar", last modified: Tue May 16 10:49:15 2023, max compression
+gzip compressed data, was "huhangkai-1.1.4.tar", last modified: Tue May 16 11:15:23 2023, max compression
```

## Comparing `huhangkai-1.1.3.tar` & `huhangkai-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 10:49:15.894184 huhangkai-1.1.3/
--rw-rw-rw-   0        0        0      228 2023-05-16 10:49:15.894184 huhangkai-1.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 10:49:15.880222 huhangkai-1.1.3/commen/
--rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.3/commen/__init__.py
--rw-rw-rw-   0        0        0    32340 2023-05-08 06:03:41.000000 huhangkai-1.1.3/commen/init_project.py
--rw-rw-rw-   0        0        0     4508 2023-05-08 06:03:41.000000 huhangkai-1.1.3/commen/unit_dict.py
--rw-rw-rw-   0        0        0    20401 2023-05-08 07:11:26.000000 huhangkai-1.1.3/commen/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-05-08 06:03:41.000000 huhangkai-1.1.3/commen/unit_logger.py
--rw-rw-rw-   0        0        0     6122 2023-05-08 06:03:41.000000 huhangkai-1.1.3/commen/unit_request.py
--rw-rw-rw-   0        0        0     2443 2023-05-16 10:44:11.000000 huhangkai-1.1.3/commen/unit_tasks.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:49:15.892189 huhangkai-1.1.3/huhangkai.egg-info/
--rw-rw-rw-   0        0        0      228 2023-05-16 10:49:15.000000 huhangkai-1.1.3/huhangkai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-05-16 10:49:15.000000 huhangkai-1.1.3/huhangkai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 10:49:15.000000 huhangkai-1.1.3/huhangkai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-16 10:49:15.000000 huhangkai-1.1.3/huhangkai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-16 10:49:15.000000 huhangkai-1.1.3/huhangkai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 10:49:15.895181 huhangkai-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      495 2023-05-16 10:49:08.000000 huhangkai-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:15:23.026404 huhangkai-1.1.4/
+-rw-rw-rw-   0        0        0      228 2023-05-16 11:15:23.025407 huhangkai-1.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 11:15:23.013438 huhangkai-1.1.4/commen/
+-rw-rw-rw-   0        0        0      929 2023-01-30 02:59:52.000000 huhangkai-1.1.4/commen/__init__.py
+-rw-rw-rw-   0        0        0    32340 2023-05-08 06:03:41.000000 huhangkai-1.1.4/commen/init_project.py
+-rw-rw-rw-   0        0        0     4508 2023-05-08 06:03:41.000000 huhangkai-1.1.4/commen/unit_dict.py
+-rw-rw-rw-   0        0        0    20401 2023-05-08 07:11:26.000000 huhangkai-1.1.4/commen/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-05-08 06:03:41.000000 huhangkai-1.1.4/commen/unit_logger.py
+-rw-rw-rw-   0        0        0     6122 2023-05-08 06:03:41.000000 huhangkai-1.1.4/commen/unit_request.py
+-rw-rw-rw-   0        0        0     2461 2023-05-16 11:14:52.000000 huhangkai-1.1.4/commen/unit_tasks.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:15:23.024409 huhangkai-1.1.4/huhangkai.egg-info/
+-rw-rw-rw-   0        0        0      228 2023-05-16 11:15:22.000000 huhangkai-1.1.4/huhangkai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-05-16 11:15:22.000000 huhangkai-1.1.4/huhangkai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 11:15:22.000000 huhangkai-1.1.4/huhangkai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-16 11:15:22.000000 huhangkai-1.1.4/huhangkai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 11:15:22.000000 huhangkai-1.1.4/huhangkai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 11:15:23.026404 huhangkai-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-05-16 11:15:17.000000 huhangkai-1.1.4/setup.py
```

### Comparing `huhangkai-1.1.3/commen/__init__.py` & `huhangkai-1.1.4/commen/__init__.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.3/commen/init_project.py` & `huhangkai-1.1.4/commen/init_project.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.3/commen/unit_dict.py` & `huhangkai-1.1.4/commen/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.3/commen/unit_fun.py` & `huhangkai-1.1.4/commen/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.3/commen/unit_logger.py` & `huhangkai-1.1.4/commen/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.3/commen/unit_request.py` & `huhangkai-1.1.4/commen/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhangkai-1.1.3/commen/unit_tasks.py` & `huhangkai-1.1.4/commen/unit_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                                             hour=hour, minute=minute, second=second, args=(schedules,))
             else:
                 Scheduler.scheduler.add_job(fun, 'cron', year=year, day_of_week=day_of_week, month=month, day=day,
                                             hour=hour, minute=minute, second=second)
             return True
         elif schedules:
             for schedule in schedules:
-                if schedule.cron.strip():
+                if schedule.cron and schedule.cron.strip():
                     try:
                         second, minute, hour, day, month, day_of_week, year = self.get_cron(schedule.cron.strip())
                         Scheduler.scheduler.add_job(fun, 'cron', year=year, day_of_week=day_of_week, month=month,
                                                     day=day, hour=hour, minute=minute, second=second, args=(schedule,))
                     except Exception as e:
                         print("Error:" + str(e))
         return True
```

