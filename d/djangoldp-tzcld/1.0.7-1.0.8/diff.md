# Comparing `tmp/djangoldp_tzcld-1.0.7.tar.gz` & `tmp/djangoldp_tzcld-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_tzcld-1.0.7.tar", last modified: Mon May 15 09:48:48 2023, max compression
+gzip compressed data, was "dist/djangoldp_tzcld-1.0.8.tar", last modified: Tue May 16 10:54:50 2023, max compression
```

## Comparing `djangoldp_tzcld-1.0.7.tar` & `djangoldp_tzcld-1.0.8.tar`

### file list

```diff
@@ -1,42 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1682 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/
--rw-rw-rw-   0 root         (0) root         (0)    18337 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2347 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-15 09:48:46.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5896 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
--rw-rw-rw-   0 root         (0) root         (0)     9812 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 09:48:31.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
--rw-rw-rw-   0 root         (0) root         (0)     1774 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
--rw-rw-rw-   0 root         (0) root         (0)    18022 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
--rw-rw-rw-   0 root         (0) root         (0)     4403 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0022_tzcldcommunity_membership_organisation_name.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
--rw-rw-rw-   0 root         (0) root         (0)     1816 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1801 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      309 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/
+-rw-rw-rw-   0 root         (0) root         (0)    18337 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)     3189 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/templates/django_registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2347 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-16 10:54:48.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 10:54:50.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5896 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
+-rw-rw-rw-   0 root         (0) root         (0)     9812 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)    18022 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0022_tzcldcommunity_membership_organisation_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-05-16 10:54:32.000000 djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
```

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/SOURCES.txt` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+MANIFEST.in
 README.md
 setup.cfg
 setup.py
 djangoldp_tzcld/__init__.py
 djangoldp_tzcld/admin.py
 djangoldp_tzcld/apps.py
+djangoldp_tzcld/djangoldp_settings.py
 djangoldp_tzcld/models.py
 djangoldp_tzcld/permissions.py
 djangoldp_tzcld/settings.py
 djangoldp_tzcld.egg-info/PKG-INFO
 djangoldp_tzcld.egg-info/SOURCES.txt
 djangoldp_tzcld.egg-info/dependency_links.txt
 djangoldp_tzcld.egg-info/requires.txt
@@ -30,8 +32,9 @@
 djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
 djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
 djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
 djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
 djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
 djangoldp_tzcld/migrations/0021_auto_20230510_1232.py
 djangoldp_tzcld/migrations/0022_tzcldcommunity_membership_organisation_name.py
-djangoldp_tzcld/migrations/__init__.py
+djangoldp_tzcld/migrations/__init__.py
+djangoldp_tzcld/templates/django_registration/registration_form.html
```

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/models.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/permissions.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/admin.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0001_initial.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py` & `djangoldp_tzcld-1.0.8/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py`

 * *Files identical despite different names*

