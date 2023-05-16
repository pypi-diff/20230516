# Comparing `tmp/raspisump-1.5.tar.gz` & `tmp/raspisump-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raspisump-1.5.tar", last modified: Wed May 10 18:32:53 2023, max compression
+gzip compressed data, was "raspisump-1.6.tar", last modified: Tue May 16 16:42:20 2023, max compression
```

## Comparing `raspisump-1.5.tar` & `raspisump-1.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.408204 raspisump-1.5/
--rw-r--r--   0 al        (1000) users      (984)     1073 2023-02-19 16:52:26.000000 raspisump-1.5/LICENSE
--rw-r--r--   0 al        (1000) users      (984)      278 2023-05-10 18:31:52.000000 raspisump-1.5/MANIFEST.in
--rw-r--r--   0 al        (1000) users      (984)     3953 2023-05-10 18:32:53.408204 raspisump-1.5/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)     3182 2023-05-10 18:31:52.000000 raspisump-1.5/README.md
--rw-r--r--   0 al        (1000) users      (984)       22 2023-05-10 18:31:52.000000 raspisump-1.5/VERSION
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.401537 raspisump-1.5/bin/
--rw-r--r--   0 al        (1000) users      (984)      359 2022-04-12 11:43:48.000000 raspisump-1.5/bin/emailtest
--rwxr-xr-x   0 al        (1000) users      (984)      696 2022-04-12 11:43:48.000000 raspisump-1.5/bin/rsump.py
--rwxr-xr-x   0 al        (1000) users      (984)      617 2022-04-12 11:43:48.000000 raspisump-1.5/bin/rsumpchart.py
--rwxr-xr-x   0 al        (1000) users      (984)      535 2023-05-10 18:31:52.000000 raspisump-1.5/bin/rsumpmonitor.py
--rwxr-xr-x   0 al        (1000) users      (984)      660 2022-04-12 11:43:48.000000 raspisump-1.5/bin/rsumpwebchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.401537 raspisump-1.5/conf/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.401537 raspisump-1.5/conf/charts/
--rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.5/conf/charts/README.md
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.401537 raspisump-1.5/conf/csv/
--rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.5/conf/csv/README.md
--rw-r--r--   0 al        (1000) users      (984)     1112 2023-05-10 18:31:52.000000 raspisump-1.5/conf/lighttpd.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.401537 raspisump-1.5/conf/logs/
--rw-r--r--   0 al        (1000) users      (984)      217 2022-04-12 11:43:48.000000 raspisump-1.5/conf/logs/README.md
--rw-r--r--   0 al        (1000) users      (984)     5687 2022-04-12 11:43:48.000000 raspisump-1.5/conf/raspisump.conf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.404870 raspisump-1.5/conf/web/
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.404870 raspisump-1.5/conf/web/css/
--rw-r--r--   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.5/conf/web/css/index.html
--rw-r--r--   0 al        (1000) users      (984)      614 2022-04-12 11:43:48.000000 raspisump-1.5/conf/web/css/raspi.css
--rw-r--r--   0 al        (1000) users      (984)      690 2022-04-12 11:43:48.000000 raspisump-1.5/conf/web/css/raspi.css~
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.404870 raspisump-1.5/conf/web/images/
--rw-r--r--   0 al        (1000) users      (984)    51981 2022-04-12 11:43:48.000000 raspisump-1.5/conf/web/images/logo.png
--rwxr-xr-x   0 al        (1000) users      (984)      906 2022-04-12 11:43:48.000000 raspisump-1.5/conf/web/index.html
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.404870 raspisump-1.5/cron/
--rw-r--r--   0 al        (1000) users      (984)      140 2022-04-12 11:43:48.000000 raspisump-1.5/cron/README.md
--rw-r--r--   0 al        (1000) users      (984)      258 2022-04-12 11:43:48.000000 raspisump-1.5/cron/picrontab
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.404870 raspisump-1.5/docs/
--rw-r--r--   0 al        (1000) users      (984)      275 2022-04-12 11:43:48.000000 raspisump-1.5/docs/README.md
--rw-r--r--   0 al        (1000) users      (984)    10942 2023-05-10 18:31:52.000000 raspisump-1.5/docs/install.md
--rw-r--r--   0 al        (1000) users      (984)   133692 2023-05-10 18:31:52.000000 raspisump-1.5/docs/install.pdf
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.408204 raspisump-1.5/raspisump/
--rwxr-xr-x   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/__init__.py
--rw-r--r--   0 al        (1000) users      (984)     4886 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/alerts.py
--rw-r--r--   0 al        (1000) users      (984)     1963 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/checkpid.py
--rw-r--r--   0 al        (1000) users      (984)     2053 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/emailtest.py
--rw-r--r--   0 al        (1000) users      (984)     3670 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/heartbeat.py
--rw-r--r--   0 al        (1000) users      (984)     1791 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/log.py
--rw-r--r--   0 al        (1000) users      (984)     2618 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/reading.py
--rw-r--r--   0 al        (1000) users      (984)     2541 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/todaychart.py
--rw-r--r--   0 al        (1000) users      (984)     1488 2022-04-12 11:43:48.000000 raspisump-1.5/raspisump/webchart.py
-drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-10 18:32:53.408204 raspisump-1.5/raspisump.egg-info/
--rw-r--r--   0 al        (1000) users      (984)     3953 2023-05-10 18:32:53.000000 raspisump-1.5/raspisump.egg-info/PKG-INFO
--rw-r--r--   0 al        (1000) users      (984)      784 2023-05-10 18:32:53.000000 raspisump-1.5/raspisump.egg-info/SOURCES.txt
--rw-r--r--   0 al        (1000) users      (984)        1 2023-05-10 18:32:53.000000 raspisump-1.5/raspisump.egg-info/dependency_links.txt
--rw-r--r--   0 al        (1000) users      (984)       13 2023-05-10 18:32:53.000000 raspisump-1.5/raspisump.egg-info/requires.txt
--rw-r--r--   0 al        (1000) users      (984)       10 2023-05-10 18:32:53.000000 raspisump-1.5/raspisump.egg-info/top_level.txt
--rw-r--r--   0 al        (1000) users      (984)       38 2023-05-10 18:32:53.408204 raspisump-1.5/setup.cfg
--rwxr-xr-x   0 al        (1000) users      (984)     2229 2023-05-10 18:31:52.000000 raspisump-1.5/setup.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.720138 raspisump-1.6/
+-rw-r--r--   0 al        (1000) users      (984)     1073 2023-02-19 16:52:26.000000 raspisump-1.6/LICENSE
+-rw-r--r--   0 al        (1000) users      (984)      278 2023-05-10 18:31:52.000000 raspisump-1.6/MANIFEST.in
+-rw-r--r--   0 al        (1000) users      (984)     3940 2023-05-16 16:42:20.716805 raspisump-1.6/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)     3168 2023-05-11 10:55:58.000000 raspisump-1.6/README.md
+-rw-r--r--   0 al        (1000) users      (984)       23 2023-05-16 16:38:14.000000 raspisump-1.6/VERSION
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.710138 raspisump-1.6/bin/
+-rw-r--r--   0 al        (1000) users      (984)      362 2023-05-16 16:38:14.000000 raspisump-1.6/bin/emailtest
+-rwxr-xr-x   0 al        (1000) users      (984)      866 2023-05-16 16:38:14.000000 raspisump-1.6/bin/rsump.py
+-rwxr-xr-x   0 al        (1000) users      (984)      619 2023-05-16 16:38:14.000000 raspisump-1.6/bin/rsumpchart.py
+-rwxr-xr-x   0 al        (1000) users      (984)      537 2023-05-16 16:38:14.000000 raspisump-1.6/bin/rsumpmonitor.py
+-rwxr-xr-x   0 al        (1000) users      (984)      662 2023-05-16 16:38:14.000000 raspisump-1.6/bin/rsumpwebchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.710138 raspisump-1.6/conf/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/charts/
+-rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.6/conf/charts/README.md
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/csv/
+-rw-r--r--   0 al        (1000) users      (984)       80 2022-04-12 11:43:48.000000 raspisump-1.6/conf/csv/README.md
+-rw-r--r--   0 al        (1000) users      (984)     1112 2023-05-10 18:31:52.000000 raspisump-1.6/conf/lighttpd.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/logs/
+-rw-r--r--   0 al        (1000) users      (984)      217 2022-04-12 11:43:48.000000 raspisump-1.6/conf/logs/README.md
+-rw-r--r--   0 al        (1000) users      (984)     5687 2022-04-12 11:43:48.000000 raspisump-1.6/conf/raspisump.conf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/web/
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/web/css/
+-rw-r--r--   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.6/conf/web/css/index.html
+-rw-r--r--   0 al        (1000) users      (984)      614 2022-04-12 11:43:48.000000 raspisump-1.6/conf/web/css/raspi.css
+-rw-r--r--   0 al        (1000) users      (984)      690 2022-04-12 11:43:48.000000 raspisump-1.6/conf/web/css/raspi.css~
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/conf/web/images/
+-rw-r--r--   0 al        (1000) users      (984)    51981 2022-04-12 11:43:48.000000 raspisump-1.6/conf/web/images/logo.png
+-rwxr-xr-x   0 al        (1000) users      (984)      906 2022-04-12 11:43:48.000000 raspisump-1.6/conf/web/index.html
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/cron/
+-rw-r--r--   0 al        (1000) users      (984)      140 2022-04-12 11:43:48.000000 raspisump-1.6/cron/README.md
+-rw-r--r--   0 al        (1000) users      (984)      258 2022-04-12 11:43:48.000000 raspisump-1.6/cron/picrontab
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.713472 raspisump-1.6/docs/
+-rw-r--r--   0 al        (1000) users      (984)      275 2022-04-12 11:43:48.000000 raspisump-1.6/docs/README.md
+-rw-r--r--   0 al        (1000) users      (984)    11066 2023-05-16 16:38:14.000000 raspisump-1.6/docs/install.md
+-rw-r--r--   0 al        (1000) users      (984)   133692 2023-05-10 18:31:52.000000 raspisump-1.6/docs/install.pdf
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.716805 raspisump-1.6/raspisump/
+-rwxr-xr-x   0 al        (1000) users      (984)        0 2022-04-12 11:43:48.000000 raspisump-1.6/raspisump/__init__.py
+-rw-r--r--   0 al        (1000) users      (984)     4910 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/alerts.py
+-rw-r--r--   0 al        (1000) users      (984)     1980 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/checkpid.py
+-rw-r--r--   0 al        (1000) users      (984)     1962 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/emailtest.py
+-rw-r--r--   0 al        (1000) users      (984)     4594 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/heartbeat.py
+-rw-r--r--   0 al        (1000) users      (984)      821 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/log.py
+-rw-r--r--   0 al        (1000) users      (984)     2704 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/reading.py
+-rw-r--r--   0 al        (1000) users      (984)     2565 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/todaychart.py
+-rw-r--r--   0 al        (1000) users      (984)     1490 2023-05-16 16:38:14.000000 raspisump-1.6/raspisump/webchart.py
+drwxr-xr-x   0 al        (1000) users      (984)        0 2023-05-16 16:42:20.716805 raspisump-1.6/raspisump.egg-info/
+-rw-r--r--   0 al        (1000) users      (984)     3940 2023-05-16 16:42:20.000000 raspisump-1.6/raspisump.egg-info/PKG-INFO
+-rw-r--r--   0 al        (1000) users      (984)      784 2023-05-16 16:42:20.000000 raspisump-1.6/raspisump.egg-info/SOURCES.txt
+-rw-r--r--   0 al        (1000) users      (984)        1 2023-05-16 16:42:20.000000 raspisump-1.6/raspisump.egg-info/dependency_links.txt
+-rw-r--r--   0 al        (1000) users      (984)       13 2023-05-16 16:42:20.000000 raspisump-1.6/raspisump.egg-info/requires.txt
+-rw-r--r--   0 al        (1000) users      (984)       10 2023-05-16 16:42:20.000000 raspisump-1.6/raspisump.egg-info/top_level.txt
+-rw-r--r--   0 al        (1000) users      (984)       38 2023-05-16 16:42:20.720138 raspisump-1.6/setup.cfg
+-rwxr-xr-x   0 al        (1000) users      (984)     2316 2023-05-16 16:38:14.000000 raspisump-1.6/setup.py
```

### Comparing `raspisump-1.5/LICENSE` & `raspisump-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `raspisump-1.5/PKG-INFO` & `raspisump-1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.5
+Version: 1.6
 Summary: A sump pit monitoring system for Raspberry Pi
-Home-page: http://www.linuxnorth.org/raspi-sump/
+Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -29,15 +29,15 @@
 
 # What's New
 
 See the [changelog](https://github.com/alaudet/raspi-sump/blob/master/changelog) for the latest information on Raspi-Sump features.
 
 # Supported Versions of Raspbian / Raspberry Pi OS
 
-Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster and Stretch).
+Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster)
 
 # Discord Group
 
 Discuss and get support from other users. Email (alaudet@linuxnorth.org) for an invite link.
 
 
 # Install Dependencies
@@ -66,23 +66,23 @@
     /home/pi/raspi-sump/docs
 
 They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
 
 
 # Python2 (End of Life was January 1, 2020)
 
-Python2 installs of Raspi-Sump are no longer be supported.
+Python2 installs of Raspi-Sump are no longer supported.
 
 
 # More Info
 
-Further details provided at http://www.linuxnorth.org/raspi-sump/
+Further details provided at https://www.linuxnorth.org/raspi-sump/
 
 An example hourly updating graph is available for view.
-http://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
+https://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
 
 # Disclaimer
 
 You are welcome to use Raspi-Sump but there is no guarantee it will work. Your house may still flood if your sump pump fails. This software comes with no warranty. See License details.
 
 This is not a replacement for a properly maintained water pumping system. It is one tool you can use to give yourself extra piece-of-mind.
```

### Comparing `raspisump-1.5/README.md` & `raspisump-1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # What's New
 
 See the [changelog](https://github.com/alaudet/raspi-sump/blob/master/changelog) for the latest information on Raspi-Sump features.
 
 # Supported Versions of Raspbian / Raspberry Pi OS
 
-Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster and Stretch).
+Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster)
 
 # Discord Group
 
 Discuss and get support from other users. Email (alaudet@linuxnorth.org) for an invite link.
 
 
 # Install Dependencies
@@ -45,23 +45,23 @@
     /home/pi/raspi-sump/docs
 
 They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
 
 
 # Python2 (End of Life was January 1, 2020)
 
-Python2 installs of Raspi-Sump are no longer be supported.
+Python2 installs of Raspi-Sump are no longer supported.
 
 
 # More Info
 
-Further details provided at http://www.linuxnorth.org/raspi-sump/
+Further details provided at https://www.linuxnorth.org/raspi-sump/
 
 An example hourly updating graph is available for view.
-http://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
+https://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
 
 # Disclaimer
 
 You are welcome to use Raspi-Sump but there is no guarantee it will work. Your house may still flood if your sump pump fails. This software comes with no warranty. See License details.
 
 This is not a replacement for a properly maintained water pumping system. It is one tool you can use to give yourself extra piece-of-mind.
```

### Comparing `raspisump-1.5/bin/rsump.py` & `raspisump-1.6/bin/rsump.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
-# http://www.linuxnorth.org/raspi-sump/
+# https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
-# MIT License -- http://www.linuxnorth.org/raspi-sump/license.html
+# MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import time
 
-try:
-    import ConfigParser as configparser # Python2
-except ImportError:
-    import configparser # Python3
-from raspisump import reading
+import configparser
+from raspisump import reading, log
 
 config = configparser.RawConfigParser()
 
 config.read('/home/pi/raspi-sump/raspisump.conf')
 reading_interval = config.getint('pit', 'reading_interval')
 
 if reading_interval == 0:
-    reading.water_depth()
+    try:
+        reading.water_depth()
+    except RuntimeError:
+        print("ERROR -- Cannot Access gpio pins.  Make sure user is part of the gpio group.")
+        log.log_event("error_log", "GPIO ERROR -- Cannot Access gpio pins.  Make sure user is part of the gpio group.")
 else:
     while True:
         reading.water_depth()
         time.sleep(reading_interval)
```

### Comparing `raspisump-1.5/bin/rsumpmonitor.py` & `raspisump-1.6/bin/rsumpmonitor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
-# http://www.linuxnorth.org/raspi-sump/
+# https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
-# MIT License -- http://www.linuxnorth.org/raspi-sump/license.html
+# MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 from raspisump import checkpid
 
 
 def main():
     '''run checkpid.py module to restart Raspi-Sump if the rsump.py process is
     stopped or has spawned multiple processes.'''
```

### Comparing `raspisump-1.5/bin/rsumpwebchart.py` & `raspisump-1.6/bin/rsumpwebchart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
-# http://www.linuxnorth.org/raspi-sump/
+# https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
-# MIT License -- http://www.linuxnorth.org/raspi-sump/license.html
+# MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import time
 from raspisump import webchart
 
 
 def main():
     '''Pass variables to webchart.py'''
```

### Comparing `raspisump-1.5/conf/lighttpd.conf` & `raspisump-1.6/conf/lighttpd.conf`

 * *Files identical despite different names*

### Comparing `raspisump-1.5/conf/raspisump.conf` & `raspisump-1.6/conf/raspisump.conf`

 * *Files identical despite different names*

### Comparing `raspisump-1.5/conf/web/css/raspi.css` & `raspisump-1.6/conf/web/css/raspi.css`

 * *Files identical despite different names*

### Comparing `raspisump-1.5/conf/web/css/raspi.css~` & `raspisump-1.6/conf/web/css/raspi.css~`

 * *Files identical despite different names*

### Comparing `raspisump-1.5/conf/web/images/logo.png` & `raspisump-1.6/conf/web/images/logo.png`

 * *Files identical despite different names*

### Comparing `raspisump-1.5/conf/web/index.html` & `raspisump-1.6/conf/web/index.html`

 * *Files identical despite different names*

### Comparing `raspisump-1.5/docs/install.md` & `raspisump-1.6/docs/install.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Install
 =======
 Disclaimer: You could damage your raspberry pi if you do not insert a voltage divider between the echo pin on the sensor and the GPIO pin on the Raspberry Pi.
 If you choose to do this you do it at your own risk.
 
-Installation instructions assume Python3 on Raspberry Pi OS 11 or Raspbian version 10 or 9.
+Installation instructions assume Python3 on Raspberry Pi OS 11 (Bullseye) or Raspbian version 10 (Buster).
 
 Supported OS Versions
 =====================
 Raspberry Pi OS 11 (Bullseye)
 
 Raspbian OS 10 (Buster)
 
-Raspbian OS 9 (Stretch) - Support ended on June 30, 2022.  Upgrade to Bullseye
+Raspbian OS 9 (Stretch) - Support ended on June 30, 2022.  Upgrade to Bullseye.
 
 
 Default 'pi' User Account
 =========================
 
-Raspberry Pi OS have changed the automatic creation of the 'pi' user account on Raspberry Pi OS 11 (Bullseye).  Raspi-Sump depends on that account existing.  When installing Raspberry Pi OS for the first time, you must create a user named pi for Raspi-Sump to work.
+Raspberry Pi OS have changed the automatic creation of the 'pi' user account on Raspberry Pi OS 11 (Bullseye).  Raspi-Sump depends on that account existing.  When installing Raspberry Pi OS for the first time, you must create a user named pi for Raspi-Sump to work. Future versions of Raspi-Sump will not have this requirement, but for the time being it is still required.
 
 For more information see the [Raspberry PI OS Announcement](https://www.raspberrypi.com/news/raspberry-pi-bullseye-update-april-2022/) on the default pi user account.
 
 
 Creating a pi user
 ==================
 
@@ -326,8 +326,8 @@
 you will create a chart of sump pit activity for the day which will be viewable
 on this page.  It will also copy historical information that you can access
 from the link in the web page.
 
 You are only limited by your own imagination on how to view your charts.  I
 have setup a bash script that automatically creates the graph on my Pi and
 moves it to an offsite webserver where I can view today's readouts and
-historical data.
+historical data.
```

### Comparing `raspisump-1.5/docs/install.pdf` & `raspisump-1.6/docs/install.pdf`

 * *Files identical despite different names*

### Comparing `raspisump-1.5/raspisump/alerts.py` & `raspisump-1.6/raspisump/alerts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 '''Send SMTP email alerts in case of sump pump failure.'''
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
-# http://www.linuxnorth.org/raspi-sump/
+# https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
-# MIT License -- http://www.linuxnorth.org/raspi-sump/license.html
+# MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import os
 import time
 import smtplib
 from datetime import datetime
 import platform
-try:
-    import ConfigParser as configparser  # Python2
-except ImportError:
-    import configparser  # Python3
+import configparser
 from collections import deque
 import csv
 from raspisump import log
 
 
 config = configparser.RawConfigParser()
 
@@ -29,16 +26,15 @@
            'email_from': config.get('email', 'email_from'),
            'smtp_authentication': config.getint(
                'email', 'smtp_authentication'),
            'smtp_tls': config.getint('email', 'smtp_tls'),
            'smtp_server': config.get('email', 'smtp_server'),
            'username': config.get('email', 'username'),
            'password': config.get('email', 'password'),
-           'unit': config.get('pit', 'unit')
-          }
+           'unit': config.get('pit', 'unit')}
 # If item in raspisump.conf add to configs dict above.  If not then provide
 # a default value
 try:
     configs['alert_interval'] = config.getint('email', 'alert_interval')
 except configparser.NoOptionError:
     configs['alert_interval'] = 5
 
@@ -48,18 +44,20 @@
     configs['alert_when'] = 'high'
 
 
 def current_time():
     '''Return the current time as reported by the OS.'''
     return time.strftime('%I:%M%P %Z')
 
+
 def host_name():
     '''Return the Raspberry Pi's Hostname'''
     return platform.node()
 
+
 def unit_types():
     '''Determine  if inches or centimeters'''
 
     unit = configs['unit']
 
     if unit == 'imperial':
         return 'inches'
@@ -87,21 +85,23 @@
         message = email_contents['message_low']
 
     return "\r\n".join((
         "From: {}".format(configs['email_from']),
         "To: {}".format(configs['email_to']),
         "{}".format(subject),
         "",
-        "{} - {} - {} {} {}.".format(hostname, time_of_day, message, str(water_depth), unit_type),
+        "{} - {} - {} {} {}.".format(hostname,
+                                     time_of_day,
+                                     message,
+                                     str(water_depth), unit_type),
         "Next alert in {} minutes".format(configs['alert_interval']),
         )
         )
 
 
-
 def smtp_alerts(water_depth):
     '''Send email alert if water level greater than critical distance.'''
     recipients = configs['email_to'].split(', ')
     email_body = email_content(water_depth)
     server = smtplib.SMTP(configs['smtp_server'])
 
     # Check if smtp server uses TLS
@@ -128,27 +128,27 @@
 
     alert_interval = configs['alert_interval']
 
     alert_log = '/home/pi/raspi-sump/logs/alert_log'
 
     if not os.path.isfile(alert_log):
         smtp_alerts(water_depth)
-        log.log_alerts('Email SMS Alert Sent')
+        log.log_event('alert_log', 'Email SMS Alert Sent')
 
     else:
         with open(alert_log, 'rt') as f:
             last_row = deque(csv.reader(f), 1)[0]
             last_alert_sent = last_row[0]
             current_time = time.strftime('%Y-%m-%d %H:%M:%S')
             last_alert_time = datetime.strptime(
                 last_alert_sent, '%Y-%m-%d %H:%M:%S'
             )
             time_now = datetime.strptime(current_time, '%Y-%m-%d %H:%M:%S')
             delta = (time_now - last_alert_time)
             minutes_passed = delta.seconds / 60
-            
+
         if minutes_passed >= alert_interval:
             smtp_alerts(water_depth)
-            log.log_alerts('Email SMS Alert Sent')
+            log.log_event('alert_log', 'Email SMS Alert Sent')
 
         else:
             pass
```

### Comparing `raspisump-1.5/raspisump/checkpid.py` & `raspisump-1.6/raspisump/checkpid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 '''Monitor the health of a process and restart it if it has stopped
 or if it has spawned multiple processes.'''
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
-# http://www.linuxnorth.org/raspi-sump/
+# https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
-# MIT License -- http://www.linuxnorth.org/raspi-sump/license.html
+# MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import subprocess
 from raspisump import log
 
+
 def check_pid(process):
     '''Check status of process.'''
     cmdp1 = 'ps aux'
     cmdp2 = 'grep -v grep'
     cmdp3 = 'grep -v sudo'
     cmdp4 = 'grep -c ' + process
     cmdp1list = cmdp1.split(' ')
@@ -32,20 +33,20 @@
     part2.stdout.close()
     part4 = subprocess.Popen(cmdp4list, stdin=part3.stdout,
                              stdout=subprocess.PIPE
                              )
     part3.stdout.close()
     number_of_processes = int(part4.communicate()[0])
     if number_of_processes == 0:
-        log.log_restarts('Process stopped, restarting')
+        log.log_errors('rsump.py process stopped, restarting')
         restart(process)
     elif number_of_processes == 1:
         exit(0)
     else:
-        log.log_restarts('Multiple processes...killing and restarting')
+        log.log_errors('Multiple rsump.py processes...killing and restarting')
         kill_start(process)
 
 
 def restart(process):
     '''Restart process'''
     restart_cmd = process + ' &'
     restart_now = restart_cmd.split(' ')
```

### Comparing `raspisump-1.5/raspisump/emailtest.py` & `raspisump-1.6/raspisump/emailtest.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 """Send an email on command to test."""
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
-# http://www.linuxnorth.org/raspi-sump/
+# https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import smtplib
-
-try:
-    import ConfigParser as configparser  # Python2
-except ImportError:
-    import configparser  # Python3
+import configparser
 from raspisump import alerts
 
 
 config = configparser.RawConfigParser()
 
 config.read("/home/pi/raspi-sump/raspisump.conf")
```

### Comparing `raspisump-1.5/raspisump/heartbeat.py` & `raspisump-1.6/raspisump/heartbeat.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 '''Send Heartbeat alert to test that email notifications are working.'''
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
-# http://www.linuxnorth.org/raspi-sump/
+# https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
 # MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import os
 import time
 import smtplib
-from datetime import datetime
-try:
-    import ConfigParser as configparser  # Python2
-except ImportError:
-    import configparser  # Python3
+from datetime import datetime, timedelta
+import configparser
 from collections import deque
 import csv
 from raspisump import log, alerts
 
 
 config = configparser.RawConfigParser()
 
@@ -31,41 +28,65 @@
            'smtp_tls': config.getint('email', 'smtp_tls'),
            'smtp_server': config.get('email', 'smtp_server'),
            'username': config.get('email', 'username'),
            'password': config.get('email', 'password')
            }
 
 try:
-    configs['heartbeat_interval'] = config.getint('email', 'heartbeat_interval')
+    configs['heartbeat_interval'] = config.getint('email',
+                                                  'heartbeat_interval')
 except configparser.NoOptionError:
     configs['heartbeat_interval'] = 10080
 
-def heartbeat_email_content():
 
+def get_last_alert_time():
+    '''Retrieve the last alert time string from logfile'''
+    heartbeat_log = '/home/pi/raspi-sump/logs/heartbeat_log'
+    with open(heartbeat_log, 'rt') as f:
+        last_row = deque(csv.reader(f), 1)[0]
+        return last_row[0]
+
+
+def heartbeat_email_content():
     '''Build the contents of email body which will be sent as an alert'''
+    heartbeat_interval_time = configs['heartbeat_interval']
+    current_time = time.strftime('%Y-%m-%d %H:%M:%S')
+    last_alert = datetime.strptime(current_time, '%Y-%m-%d %H:%M:%S')
+    future_date = last_alert + timedelta(minutes=heartbeat_interval_time + 1)
+
+    weekday = future_date.strftime('%A')[0:3]
+    month = future_date.strftime('%B')
+    hour = future_date.strftime('%I')
+    minute = future_date.strftime('%M')
+    am_pm = future_date.strftime('%p').lower()
 
     time_of_day = alerts.current_time()
     hostname = alerts.host_name()
-    
-    subject = 'Subject: Raspi-Sump Heartbeat Notification' 
+    subject = 'Subject: Raspi-Sump Heartbeat Notification'
     message = 'Raspi-Sump Email Notifications Working'
 
     return "\r\n".join((
         "From: {}".format(configs['email_from']),
         "To: {}".format(configs['email_to']),
         "{}".format(subject),
         "",
         "{} - {} - {}.".format(hostname, time_of_day, message),
-        "Next email test in {} minutes".format(configs['heartbeat_interval']),
+        "Next heartbeat: {} {} {} at {}:{} {}".format(weekday,
+                                                      month,
+                                                      future_date.day,
+                                                      hour,
+                                                      minute,
+                                                      am_pm),
         )
         )
 
 
 def heartbeat_alerts():
-    '''Send heartbeat email alert if water level greater than critical distance.'''
+    '''Send heartbeat email alert if water level greater
+    than critical distance.'''
     recipients = configs['email_to'].split(', ')
     email_body = heartbeat_email_content()
     server = smtplib.SMTP(configs['smtp_server'])
 
     # Check if smtp server uses TLS
     if configs['smtp_tls'] == 1:
         server.starttls()
@@ -83,30 +104,27 @@
     server.quit()
 
 
 def determine_if_heartbeat():
     '''Determine if a heartbeat notification is required and if so, send
     the notification.'''
 
-    heartbeat_interval_time = configs['heartbeat_interval']
     heartbeat_log = '/home/pi/raspi-sump/logs/heartbeat_log'
     if not os.path.isfile(heartbeat_log):
         heartbeat_alerts()
-        log.log_heartbeat("Heartbeat Email Sent")
+        log.log_event("heartbeat_log", "Heartbeat Email Sent")
 
     else:
-        with open(heartbeat_log, 'rt') as f:
-            last_row = deque(csv.reader(f), 1)[0]
-            last_email_sent = last_row[0]
-            current_time = time.strftime('%Y-%m-%d %H:%M:%S')
-            last_heartbeat_time = datetime.strptime(
-                last_email_sent, '%Y-%m-%d %H:%M:%S'
-            )
-            time_now = datetime.strptime(current_time, '%Y-%m-%d %H:%M:%S')
-            delta = (time_now - last_heartbeat_time)
-            minutes_passed = int((delta).total_seconds() / 60)
-
-            if minutes_passed >= heartbeat_interval_time:
-                heartbeat_alerts()
-                log.log_heartbeat("Heartbeat Email Sent")
-            else:
-                pass
+        heartbeat_interval_time = configs['heartbeat_interval']
+        last_email_sent = get_last_alert_time()
+        current_time = time.strftime('%Y-%m-%d %H:%M:%S')
+        last_heartbeat_time = datetime.strptime(last_email_sent,
+                                                '%Y-%m-%d %H:%M:%S')
+        time_now = datetime.strptime(current_time, '%Y-%m-%d %H:%M:%S')
+        delta = (time_now - last_heartbeat_time)
+        minutes_passed = int((delta).total_seconds() / 60)
+
+        if minutes_passed >= heartbeat_interval_time:
+            heartbeat_alerts()
+            log.log_event("heartbeat_log", "Heartbeat Email Sent")
+        else:
+            pass
```

### Comparing `raspisump-1.5/raspisump/reading.py` & `raspisump-1.6/raspisump/reading.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """ Module to take a water_level reading."""
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
-# http://www.linuxnorth.org/raspi-sump/
+# https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
-# MIT License -- http://www.linuxnorth.org/raspi-sump/license.html
+# MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
-try:
-    import ConfigParser as configparser  # Python2
-except ImportError:
-    import configparser  # Python3
+import configparser
 from hcsr04sensor import sensor
 from raspisump import log, alerts, heartbeat
 
 config = configparser.RawConfigParser()
 config.read("/home/pi/raspi-sump/raspisump.conf")
 
 configs = {
@@ -55,32 +52,33 @@
     unit = configs["unit"]
 
     value = sensor.Measurement(trig_pin, echo_pin, temperature, unit)
 
     try:
         raw_distance = value.raw_distance(sample_wait=0.3)
     except SystemError:
-        log.log_errors(
-            "**ERROR - Signal not received. Possible cable or sensor problem."
-        )
+        log.log_event("error_log",
+                      "ERROR - Signal not received. Possible cable or sensor problem.")
         exit(0)
 
     return round(value.depth(raw_distance, pit_depth), 1)
 
 
 def water_depth():
     """Determine the depth of the water, log result and generate alert
     if needed.
     """
 
     critical_water_level = configs["critical_water_level"]
     water_depth = water_reading()
-
     if water_depth < 0.0:
         water_depth = 0.0
+        log.log_reading(water_depth)
+        log.log_event("error_log",
+                      "ERROR - Negative reading adjusted to 0.0. Possible degrading sensor.")
     log.log_reading(water_depth)
 
     if water_depth > critical_water_level and configs["alert_when"] == "high":
         alerts.determine_if_alert(water_depth)
     elif water_depth < critical_water_level and configs["alert_when"] == "low":
         alerts.determine_if_alert(water_depth)
     else:
```

### Comparing `raspisump-1.5/raspisump/todaychart.py` & `raspisump-1.6/raspisump/todaychart.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Graph sump pit activity."""
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
-# http://www.linuxnorth.org/raspi-sump/
+# https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
-# MIT License -- http://www.linuxnorth.org/raspi-sump/license.html
+# MIT License -- https://www.linuxnorth.org/raspi-sump/license.html
 
 import time
 import numpy as np
 import matplotlib as mpl
 
 mpl.use("Agg")
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 from matplotlib import rcParams
 
 rcParams.update({"figure.autolayout": True})
-try:
-    import ConfigParser as configparser  # Python2
-except ImportError:
-    import configparser  # Python3
+import configparser
 
 config = configparser.RawConfigParser()
 config.read("/home/pi/raspi-sump/raspisump.conf")
 configs = {"unit": config.get("pit", "unit")}
 
 try:
     configs["line_color"] = config.get("charts", "line_color")
@@ -51,14 +48,15 @@
         unpack=True,
         converters={0: lambda x: mdates.datestr2num(x.decode("utf8"))},
     )
 
     fig = plt.figure(figsize=(10, 3.5))
 
     # axisbg is deprecated in matplotlib 2.x. Maintain 1.x compatibility
+    # This if/else can now be removed
     if MPL_VERSION > 1:
         fig.add_subplot(111, facecolor="white", frameon=False)
     else:
         fig.add_subplot(111, axisbg="white", frameon=False)
 
     rcParams.update({"font.size": 9})
     plt.plot_date(
@@ -78,14 +76,15 @@
         plt.ylabel("inches")
     if unit == "metric":
         plt.ylabel("centimeters")
 
     plt.xlabel("Time of Day")
     plt.xticks(rotation=30)
     plt.grid(True, color="#ECE5DE", linestyle="solid")
+    # This if/else statement can be removed as buster and bullseye use > 2
     if MPL_VERSION < 3:
         plt.tick_params(axis="x", bottom="off", top="off")
         plt.tick_params(axis="y", left="off", right="off")
     else:
         plt.tick_params(axis="x", bottom=False, top=False)
         plt.tick_params(axis="y", left=False, right=False)
     plt.savefig(filename, dpi=72)
```

### Comparing `raspisump-1.5/raspisump/webchart.py` & `raspisump-1.6/raspisump/webchart.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Create charts for viewing on Raspberry Pi Web Server."""
 
 # Raspi-sump, a sump pump monitoring system.
 # Al Audet
-# http://www.linuxnorth.org/raspi-sump/
+# https://www.linuxnorth.org/raspi-sump/
 #
 # All configuration changes should be done in raspisump.conf
-# MIT License -- http://www.linuxnorth.org/raspi-sump/license.htmlimport os
+# MIT License -- https://www.linuxnorth.org/raspi-sump/license.htmlimport os
 
 import os
 import subprocess
 import time
 from raspisump import todaychart
```

### Comparing `raspisump-1.5/raspisump.egg-info/PKG-INFO` & `raspisump-1.6/raspisump.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: raspisump
-Version: 1.5
+Version: 1.6
 Summary: A sump pit monitoring system for Raspberry Pi
-Home-page: http://www.linuxnorth.org/raspi-sump/
+Home-page: https://www.linuxnorth.org/raspi-sump/
 Download-URL: https://github.com/alaudet/raspi-sump/releases
 Author: Al Audet
 Author-email: alaudet@linuxnorth.org
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
@@ -29,15 +29,15 @@
 
 # What's New
 
 See the [changelog](https://github.com/alaudet/raspi-sump/blob/master/changelog) for the latest information on Raspi-Sump features.
 
 # Supported Versions of Raspbian / Raspberry Pi OS
 
-Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster and Stretch).
+Raspi-Sump is currently supported on Raspberry Pi OS (Bullseye) and Raspian (Buster)
 
 # Discord Group
 
 Discuss and get support from other users. Email (alaudet@linuxnorth.org) for an invite link.
 
 
 # Install Dependencies
@@ -66,23 +66,23 @@
     /home/pi/raspi-sump/docs
 
 They are also available on github https://github.com/alaudet/raspi-sump/blob/master/docs/install.md
 
 
 # Python2 (End of Life was January 1, 2020)
 
-Python2 installs of Raspi-Sump are no longer be supported.
+Python2 installs of Raspi-Sump are no longer supported.
 
 
 # More Info
 
-Further details provided at http://www.linuxnorth.org/raspi-sump/
+Further details provided at https://www.linuxnorth.org/raspi-sump/
 
 An example hourly updating graph is available for view.
-http://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
+https://www.linuxnorth.org/raspi-sump/raspi-sump-today.html
 
 # Disclaimer
 
 You are welcome to use Raspi-Sump but there is no guarantee it will work. Your house may still flood if your sump pump fails. This software comes with no warranty. See License details.
 
 This is not a replacement for a properly maintained water pumping system. It is one tool you can use to give yourself extra piece-of-mind.
```

### Comparing `raspisump-1.5/raspisump.egg-info/SOURCES.txt` & `raspisump-1.6/raspisump.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raspisump-1.5/setup.py` & `raspisump-1.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-version = "1.5"
+version = "1.6"
 
 homedir = "/home/pi/raspi-sump/"
 
 if os.path.isfile(homedir + "raspisump.conf"):
     cmd = "cp -u " + homedir + "raspisump.conf " + homedir + "raspisump.conf.save"
     os.system(cmd)
 
@@ -49,21 +49,23 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "Topic :: Home Automation",
         "License :: OSI Approved :: MIT License",
     ],
     author="Al Audet",
     author_email="alaudet@linuxnorth.org",
-    url="http://www.linuxnorth.org/raspi-sump/",
+    url="https://www.linuxnorth.org/raspi-sump/",
     download_url="https://github.com/alaudet/raspi-sump/releases",
     license="MIT License",
     packages=["raspisump"],
     scripts=raspi_sump_files,
     data_files=add_files,
     install_requires=["hcsr04sensor"],
 )
 
 if os.path.isdir(homedir):
     cmd = "chown -R pi " + homedir
     os.system(cmd)
     cmd = "chmod 600 " + homedir + "raspisump.conf"
-    os.system(cmd)
+    os.system(cmd)
+    cmd = "chmod 600 " + homedir + "sample_config/raspisump.conf"
+    os.system(cmd)
```

