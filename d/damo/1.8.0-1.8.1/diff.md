# Comparing `tmp/damo-1.8.0.tar.gz` & `tmp/damo-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "damo-1.8.0.tar", last modified: Tue May  9 17:20:48 2023, max compression
+gzip compressed data, was "damo-1.8.1.tar", last modified: Mon May 15 21:58:18 2023, max compression
```

## Comparing `damo-1.8.0.tar` & `damo-1.8.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-09 17:20:48.231830 damo-1.8.0/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7226 2023-05-09 17:20:48.231830 damo-1.8.0/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6705 2023-05-09 17:20:43.000000 damo-1.8.0/README.md
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-05-09 17:20:43.000000 damo-1.8.0/pyproject.toml
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-05-09 17:20:48.231830 damo-1.8.0/setup.cfg
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      959 2023-05-09 17:20:43.000000 damo-1.8.0/setup.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-09 17:20:48.219831 damo-1.8.0/src/
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-09 17:20:48.231830 damo-1.8.0/src/damo/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-05-09 17:20:44.000000 damo-1.8.0/src/damo/__init__.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_dist.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_fmt_str.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_fs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_paddr_layout.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      923 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_python2_support.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damo_subcmds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34053 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9985 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon_args.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8485 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon_args_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17961 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon_dbgfs.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17960 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon_result.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19344 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/_damon_sysfs.py
--rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3644 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_adjust.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_features.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      768 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_fmt_json.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13296 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_heats.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_lru_sort.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3613 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_monitor.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_nr_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_reclaim.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5144 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_record.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1196 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_report.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2970 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_report_raw.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1611 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_start.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_stat.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1545 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_stat_kdamonds.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3079 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_stat_regions.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2809 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_stat_schemes.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      677 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_stop.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_translate_damos.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      650 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_tune.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3966 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_validate.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        6 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_version.py
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5576 2023-05-09 17:20:43.000000 damo-1.8.0/src/damo/damo_wss.py
-drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-09 17:20:48.231830 damo-1.8.0/src/damo.egg-info/
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7226 2023-05-09 17:20:48.000000 damo-1.8.0/src/damo.egg-info/PKG-INFO
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1135 2023-05-09 17:20:48.000000 damo-1.8.0/src/damo.egg-info/SOURCES.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-05-09 17:20:48.000000 damo-1.8.0/src/damo.egg-info/dependency_links.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-05-09 17:20:48.000000 damo-1.8.0/src/damo.egg-info/entry_points.txt
--rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-05-09 17:20:48.000000 damo-1.8.0/src/damo.egg-info/top_level.txt
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-15 21:58:18.537882 damo-1.8.1/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7182 2023-05-15 21:58:18.537882 damo-1.8.1/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     6661 2023-05-15 21:58:14.000000 damo-1.8.1/README.md
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      104 2023-05-15 21:58:14.000000 damo-1.8.1/pyproject.toml
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       38 2023-05-15 21:58:18.537882 damo-1.8.1/setup.cfg
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1104 2023-05-15 21:58:14.000000 damo-1.8.1/setup.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-15 21:58:18.525883 damo-1.8.1/src/
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-15 21:58:18.537882 damo-1.8.1/src/damo/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        0 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/__init__.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      643 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_dist.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     9696 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_fmt_str.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3018 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_fs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5368 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_paddr_layout.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      923 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_python2_support.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      762 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damo_subcmds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    34688 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    10476 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon_args.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     8485 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon_args_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    17961 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon_dbgfs.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    18504 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon_result.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    19344 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/_damon_sysfs.py
+-rwxrwxr-x   0 sjpark    (1000) sjpark    (1000)     3546 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1849 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_adjust.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1170 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_features.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      768 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_fmt_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)    13312 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_heats.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4691 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_lru_sort.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3052 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_monitor.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2772 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_nr_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     4481 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_reclaim.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5144 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_record.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1335 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_report.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1094 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_report_json.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2970 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_report_raw.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1611 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      565 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_start.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2406 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_stat.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1545 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_stat_kdamonds.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3079 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_stat_regions.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     2809 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_stat_schemes.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      677 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_stop.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      727 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_translate_damos.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)      650 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_tune.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     3966 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_validate.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       22 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_version.py
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     5576 2023-05-15 21:58:14.000000 damo-1.8.1/src/damo/damo_wss.py
+drwxrwxr-x   0 sjpark    (1000) sjpark    (1000)        0 2023-05-15 21:58:18.537882 damo-1.8.1/src/damo.egg-info/
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     7182 2023-05-15 21:58:18.000000 damo-1.8.1/src/damo.egg-info/PKG-INFO
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)     1164 2023-05-15 21:58:18.000000 damo-1.8.1/src/damo.egg-info/SOURCES.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        1 2023-05-15 21:58:18.000000 damo-1.8.1/src/damo.egg-info/dependency_links.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)       40 2023-05-15 21:58:18.000000 damo-1.8.1/src/damo.egg-info/entry_points.txt
+-rw-rw-r--   0 sjpark    (1000) sjpark    (1000)        5 2023-05-15 21:58:18.000000 damo-1.8.1/src/damo.egg-info/top_level.txt
```

### Comparing `damo-1.8.0/PKG-INFO` & `damo-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.0
+Version: 1.8.1
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.0/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.1/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -174,15 +174,14 @@
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
 Note: Previously, one-line scheme specification format like below was used.  It
-is now DEPRECATED, and the support will be removed by 2023 Q2.  Please report
-your usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if
-you depend on those.
+is now DEPRECATED.  Please report your usecase to sj@kernel.org,
+damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
 
     $ # !!! BELOW IS NO MORE SUPPORTED
     $ echo "#min-size max-size min-acc max-acc min-age max-age action" > my_scheme
     $ echo "4K        max      0       0       60s     max     pageout" >> my_scheme
     $ sudo damo schemes -c my_scheme <pid of your workload>
```

### Comparing `damo-1.8.0/README.md` & `damo-1.8.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -44,15 +44,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.0/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.1/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -159,15 +159,14 @@
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
 Note: Previously, one-line scheme specification format like below was used.  It
-is now DEPRECATED, and the support will be removed by 2023 Q2.  Please report
-your usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if
-you depend on those.
+is now DEPRECATED.  Please report your usecase to sj@kernel.org,
+damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
 
     $ # !!! BELOW IS NO MORE SUPPORTED
     $ echo "#min-size max-size min-acc max-acc min-age max-age action" > my_scheme
     $ echo "4K        max      0       0       60s     max     pageout" >> my_scheme
     $ sudo damo schemes -c my_scheme <pid of your workload>
```

### Comparing `damo-1.8.0/setup.py` & `damo-1.8.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 # SPDX-License-Identifier: GPL-2.0
 
+import os
 import setuptools
+os.sys.path.insert(0, os.path.join(os.path.dirname(os.path.abspath(__file__)), "src"))
+
+from damo import damo_version
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="damo",
-    version="1.8.0",
+    version=damo_version.__version__,
     author="SeongJae Park",
     author_email="sj@kernel.org",
     description="DAMON user-space tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/awslabs/damo",
     project_urls={
```

### Comparing `damo-1.8.0/src/damo/_damo_dist.py` & `damo-1.8.1/src/damo/_damo_dist.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/_damo_fmt_str.py` & `damo-1.8.1/src/damo/_damo_fmt_str.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/_damo_fs.py` & `damo-1.8.1/src/damo/_damo_fs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/_damo_paddr_layout.py` & `damo-1.8.1/src/damo/_damo_paddr_layout.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/_damo_python2_support.py` & `damo-1.8.1/src/damo/_damo_python2_support.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/_damo_subcmds.py` & `damo-1.8.1/src/damo/_damo_subcmds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/_damon.py` & `damo-1.8.1/src/damo/_damon.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,18 @@
         if unit == unit_percent:
             return '%s %%' % (_damo_fmt_str.format_nr(self.percent, raw))
         elif unit == unit_samples:
             return '%s %s' % (_damo_fmt_str.format_nr(self.samples, raw),
                     unit_samples)
         raise Exception('unsupported unit for NrAccesses (%s)' % unit)
 
+    def to_kvpairs(self, raw=False):
+        return collections.OrderedDict(
+                [('samples', self.samples), ('percent', self.percent)])
+
 class DamonAge:
     usec = None
     aggr_intervals = None
 
     def __init__(self, val, unit):
         if unit == unit_usec:
             self.usec = val
@@ -143,14 +147,18 @@
 
     def to_str(self, unit, raw):
         if unit == unit_usec:
             return _damo_fmt_str.format_time_us_exact(self.usec, raw)
         return '%s %s' % (_damo_fmt_str.format_nr(self.aggr_intervals, raw),
                 unit_aggr_intervals)
 
+    def to_kvpairs(self, raw=False):
+        return collections.OrderedDict(
+                [('usec', self.usec), ('aggr_intervals', self.aggr_intervals)])
+
 class DamonRegion:
     # [start, end)
     start = None
     end = None
     # nr_accesses and age could be None
     nr_accesses = None
     age = None
@@ -197,17 +205,23 @@
         return hash(identification)
 
     @classmethod
     def from_kvpairs(cls, kvpairs):
         return DamonRegion(kvpairs['start'], kvpairs['end'])
 
     def to_kvpairs(self, raw=False):
+        if self.nr_accesses == None:
+            return collections.OrderedDict([
+                ('start', _damo_fmt_str.format_nr(self.start, raw)),
+                ('end', _damo_fmt_str.format_nr(self.end, raw))])
         return collections.OrderedDict([
             ('start', _damo_fmt_str.format_nr(self.start, raw)),
-            ('end', _damo_fmt_str.format_nr(self.end, raw))])
+            ('end', _damo_fmt_str.format_nr(self.end, raw)),
+            ('nr_accesses', self.nr_accesses.to_kvpairs(raw)),
+            ('age', self.age.to_kvpairs(raw))])
 
 class DamonTarget:
     pid = None
     regions = None
 
     def __init__(self, pid, regions):
         self.pid = pid
```

### Comparing `damo-1.8.0/src/damo/_damon_args.py` & `damo-1.8.1/src/damo/_damon_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,35 +112,50 @@
         else:
             kdamonds_str = arg
         kdamonds_kvpairs = json.loads(kdamonds_str)['kdamonds']
         return [kdamond.from_kvpairs(kvp) for kvp in kdamonds_kvpairs], None
     except Exception as e:
         return None, e
 
+target_type_explict = 'explict'
+target_type_cmd = 'cmd'
+target_type_pid = 'pid'
+target_type_unknown = None
+
+def deduced_target_type(target):
+    if target in ['vaddr', 'paddr', 'fvaddr']:
+        return target_type_explict
+    try:
+        subprocess.check_output(['which', target.split()[0]])
+        return target_type_cmd
+    except:
+        pass
+    try:
+        pid = int(target)
+        return target_type_pid
+    except:
+        pass
+    return target_type_unknown
+
 def deduce_target_update_args(args):
     args.self_started_target = False
-    if args.deducible_target == 'paddr':
+    target_type = deduced_target_type(args.deducible_target)
+    if target_type == target_type_unknown:
+        return 'target \'%s\' is not supported' % args.deducible_target
+    if target_type == target_type_explict and args.deducible_target == 'paddr':
         args.ops = 'paddr'
         args.target_pid = None
         return None
-    try:
-        subprocess.check_output(['which', args.deducible_target.split()[0]])
-        is_cmd = True
-    except:
-        is_cmd = False
-    if is_cmd:
+    if target_type == target_type_cmd:
         p = subprocess.Popen(args.deducible_target, shell=True,
                 executable='/bin/bash')
         pid = p.pid
         args.self_started_target = True
-    else:
-        try:
-            pid = int(args.deducible_target)
-        except:
-            return 'target \'%s\' is not supported' % args.deducible_target
+    elif target_type == target_type_pid:
+        pid = int(args.deducible_target)
     args.target_pid = pid
     args.ops = 'vaddr'
     if args.regions:
         args.ops = 'fvaddr'
 
 def kdamonds_for(args):
     if args.kdamonds:
```

### Comparing `damo-1.8.0/src/damo/_damon_args_schemes.py` & `damo-1.8.1/src/damo/_damon_args_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/_damon_dbgfs.py` & `damo-1.8.1/src/damo/_damon_dbgfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/_damon_result.py` & `damo-1.8.1/src/damo/_damon_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
+import collections
 import os
 import signal
 import struct
 import subprocess
 import time
 
 import _damon
@@ -18,22 +19,32 @@
     regions = None
 
     def __init__(self, start_time, end_time):
         self.start_time = start_time
         self.end_time = end_time
         self.regions = []
 
+    def to_kvpairs(self):
+        return collections.OrderedDict([
+            ('start_time', self.start_time), ('end_time', self.end_time),
+            ('regions', [r.to_kvpairs() for r in self.regions])])
+
 class DAMONRecord:
     target_id = None
     snapshots = None
 
     def __init__(self, target_id):
         self.target_id = target_id
         self.snapshots = []
 
+    def to_kvpairs(self):
+        return collections.OrderedDict([
+            ('target_id', self.target_id),
+            ('snapshots', [s.to_kvpairs() for s in self.snapshots])])
+
 class DAMONResult:
     records = None
 
     def __init__(self):
         self.records = []
 
     def record_of(self, target_id):
@@ -117,16 +128,19 @@
                 record = result.record_of(target_id)
                 if len(record.snapshots) == 0:
                     start_time = None
                 else:
                     start_time = record.snapshots[-1].end_time
                     if end_time < start_time:
                         return None, 'snapshot is not sorted by time'
-                snapshot = read_snapshot_from_record_file(f,
-                        start_time, end_time)
+                try:
+                    snapshot = read_snapshot_from_record_file(f,
+                            start_time, end_time)
+                except Exception as e:
+                    return None, 'snapshot reading failead: %s' % e
                 record.snapshots.append(snapshot)
 
     set_first_snapshot_start_time(result)
     return result, None
 
 def parse_perf_script_line(line):
         '''
```

### Comparing `damo-1.8.0/src/damo/_damon_sysfs.py` & `damo-1.8.1/src/damo/_damon_sysfs.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo.py` & `damo-1.8.1/src/damo/damo.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,22 +19,21 @@
 import damo_report
 import damo_schemes
 import damo_start
 import damo_stat
 import damo_stop
 import damo_tune
 import damo_validate
+import damo_version
 import damo_translate_damos
 
 import _damo_subcmds
 
 def pr_damo_version(args_not_use):
-    bindir = os.path.dirname(os.path.abspath(__file__))
-    with open(os.path.join(bindir, 'damo_version.py'), 'r') as f:
-        print(f.read().strip())
+    print(damo_version.__version__)
 
 subcmds = [
         _damo_subcmds.DamoSubCmd(name='record', module=damo_record,
             msg='record data accesses'),
         _damo_subcmds.DamoSubCmd(name='schemes', module=damo_schemes,
             msg='apply operation schemes'),
         _damo_subcmds.DamoSubCmd(name='report', module=damo_report,
```

### Comparing `damo-1.8.0/src/damo/damo_adjust.py` & `damo-1.8.1/src/damo/damo_adjust.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_features.py` & `damo-1.8.1/src/damo/damo_features.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_fmt_json.py` & `damo-1.8.1/src/damo/damo_fmt_json.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_heats.py` & `damo-1.8.1/src/damo/damo_heats.py`

 * *Files 1% similar despite different names*

```diff
@@ -361,14 +361,15 @@
         set_argparser(parser)
         args = parser.parse_args()
 
     damon_result, err = _damon_result.parse_damon_result(args.input)
     if err != None:
         print('monitoring result file (%s) parsing failed (%s)' %
                 (args.input, err))
+        exit(1)
 
     # Use 80x40 resolution as default for ascii plot
     if args.heatmap == 'stdout' and args.resol == [500, 500]:
         args.resol = [40, 80]
 
     if args.guide:
         pr_guide(damon_result)
```

### Comparing `damo-1.8.0/src/damo/damo_lru_sort.py` & `damo-1.8.1/src/damo/damo_lru_sort.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_monitor.py` & `damo-1.8.1/src/damo/damo_monitor.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,39 +4,20 @@
 "Record and report data access pattern in realtime"
 
 import argparse
 import os
 import signal
 import subprocess
 import sys
-import time
 
 import _damon
-
-# For supporting python 2.6
-try:
-    subprocess.DEVNULL = subprocess.DEVNULL
-except AttributeError:
-    subprocess.DEVNULL = open(os.devnull, 'wb')
-
-try:
-    subprocess.check_output = subprocess.check_output
-except AttributeError:
-    def check_output(*popenargs, **kwargs):
-        process = subprocess.Popen(stdout=subprocess.PIPE, *popenargs, **kwargs)
-        output, err = process.communicate()
-        rc = process.poll()
-        if rc:
-            raise subprocess.CalledProcessError(rc, popenargs[0])
-        return output
-
-    subprocess.check_output = check_output
+import _damon_args
 
 def cleanup():
-    if target_is_cmd and cmd_pipe.poll() == None:
+    if target_type == _damon_args.target_type_cmd and cmd_pipe.poll() == None:
         cmd_pipe.kill()
 
 def sighandler(signum, frame):
     print('\nsignal %s received' % signum)
     cleanup()
 
 def set_argparser(parser):
@@ -53,67 +34,65 @@
     if not args:
         parser = argparse.ArgumentParser()
         set_argparser(parser)
         args = parser.parse_args()
 
     _damon.ensure_root_permission()
 
-    global target_is_cmd
+    global target_type
     global cmd_pipe
 
     signal.signal(signal.SIGINT, sighandler)
     signal.signal(signal.SIGTERM, sighandler)
 
-    target_is_cmd = False
     target = args.target
     target_fields = target.split()
-    if target == 'paddr':
+    target_type = _damon_args.deduced_target_type(target)
+    if target_type == None:
+        print('invalid target \'%s\'' % target)
+        exit(1)
+    if target_type == _damon_args.target_type_explict and target == 'paddr':
         pass
-    elif not subprocess.call('which %s &> /dev/null' % target_fields[0],
-            shell=True, executable='/bin/bash'):
-        target_is_cmd = True
+    elif target_type == _damon_args.target_type_cmd:
         cmd_pipe = subprocess.Popen(target, shell=True, executable='/bin/bash',
                 stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         target = cmd_pipe.pid
     else:
-        try:
-            pid = int(target)
-        except:
-            print('invalid target \'%s\'' % target)
-            exit(1)
+        pid = int(target)
 
     bindir = os.path.dirname(sys.argv[0])
     damo = os.path.join(bindir, 'damo')
 
     record_cmd = 'timeout %s %s record \"%s\"' % (args.delay, damo, target)
 
+    report_cmd = [damo]
     if args.report_type == 'heats':
-        report_cmd = '%s report heats --heatmap stdout --resol 10 80' % damo
+        report_cmd += 'report heats --heatmap stdout --resol 10 80'.split()
     else:
-        report_cmd = '%s report wss' % damo
+        report_cmd += ['report', 'wss']
 
     nr_reports = 0
     while not args.count or nr_reports < args.count:
-        if target_is_cmd and cmd_pipe.poll() != None:
+        if (target_type == _damon_args.target_type_cmd and
+                cmd_pipe.poll() != None):
             break
         try:
             subprocess.check_output(record_cmd, shell=True,
                     stderr=subprocess.STDOUT, executable='/bin/bash')
         except subprocess.CalledProcessError as e:
             pass
         try:
-            output = subprocess.check_output(report_cmd, shell=True,
-                    executable='/bin/bash').decode()
+            output = subprocess.check_output(report_cmd).decode()
             if args.report_type == 'heats':
                 for line in output.strip().split('\n'):
                     if not line.startswith('#'):
                         print(line)
             else:
                 print(output)
         except subprocess.CalledProcessError as e:
-            break
+            pass
         nr_reports += 1
 
     cleanup()
 
 if __name__ == '__main__':
     main()
```

### Comparing `damo-1.8.0/src/damo/damo_nr_regions.py` & `damo-1.8.1/src/damo/damo_nr_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_reclaim.py` & `damo-1.8.1/src/damo/damo_reclaim.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_record.py` & `damo-1.8.1/src/damo/damo_record.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_report.py` & `damo-1.8.1/src/damo/damo_report.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python3
 # SPDX-License-Identifier: GPL-2.0
 
 import argparse
 
 import damo_heats
 import damo_nr_regions
+import damo_report_json
 import damo_report_raw
 import damo_wss
 
 import _damo_subcmds
 
 subcmds = [
         _damo_subcmds.DamoSubCmd(name='raw', module=damo_report_raw,
             msg='human readable raw data'),
+        _damo_subcmds.DamoSubCmd(name='json', module=damo_report_json,
+            msg='raw data in json format'),
         _damo_subcmds.DamoSubCmd(name='heats', module=damo_heats,
             msg='heats of regions'),
         _damo_subcmds.DamoSubCmd(name='wss', module=damo_wss,
             msg='working set size'),
         _damo_subcmds.DamoSubCmd(name='nr_regions', module=damo_nr_regions,
             msg='number of regions')]
```

### Comparing `damo-1.8.0/src/damo/damo_report_raw.py` & `damo-1.8.1/src/damo/damo_report_raw.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_schemes.py` & `damo-1.8.1/src/damo/damo_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_start.py` & `damo-1.8.1/src/damo/damo_start.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_stat.py` & `damo-1.8.1/src/damo/damo_stat.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_stat_kdamonds.py` & `damo-1.8.1/src/damo/damo_stat_kdamonds.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_stat_regions.py` & `damo-1.8.1/src/damo/damo_stat_regions.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_stat_schemes.py` & `damo-1.8.1/src/damo/damo_stat_schemes.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_stop.py` & `damo-1.8.1/src/damo/damo_stop.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_translate_damos.py` & `damo-1.8.1/src/damo/damo_translate_damos.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_tune.py` & `damo-1.8.1/src/damo/damo_tune.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_validate.py` & `damo-1.8.1/src/damo/damo_validate.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo/damo_wss.py` & `damo-1.8.1/src/damo/damo_wss.py`

 * *Files identical despite different names*

### Comparing `damo-1.8.0/src/damo.egg-info/PKG-INFO` & `damo-1.8.1/src/damo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: damo
-Version: 1.8.0
+Version: 1.8.1
 Summary: DAMON user-space tool
 Home-page: https://github.com/awslabs/damo
 Author: SeongJae Park
 Author-email: sj@kernel.org
 Project-URL: Bug Tracker, https://github.com/awslabs/damo/issues
 Project-URL: DAMON, https://damonitor.github.io
 Classifier: Programming Language :: Python :: 3
@@ -42,16 +42,16 @@
     $ # ensure your kernel is built with CONFIG_DAMON_*=y
     $ sudo pip3 install damo
     $ sudo damo record $(pidof <your workload>)
     $ damo report heats --heatmap stdout --stdout_heatmap_color emotion
 
 The last command will show the access pattern of your workload, like below:
 
-![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_zigzag_heatmap_ascii.png)
-![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.0/images/masim_stairs_heatmap_ascii.png)
+![masim zigzag heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_zigzag_heatmap_ascii.png)
+![masim stairs heatmap in ascii](https://raw.githubusercontent.com/awslabs/damo/v1.8.1/images/masim_stairs_heatmap_ascii.png)
 
 
 FAQs
 ====
 
 How can I install a kernel that is built with `CONFIG_DAMON_*=y`?
 -----------------------------------------------------------------
@@ -59,15 +59,15 @@
 Please refer to 'Install'
 [section](https://sjp38.github.io/post/damon/#install) of the project webpage.
 
 Where can I get more detailed usage?
 ------------------------------------
 
 The below sections provide quick introductions for `damo`'s major features.
-For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.0/USAGE.md) file.
+For more detailed usage, please refer to [USAGE.md](https://github.com/awslabs/damo/blob/v1.8.1/USAGE.md) file.
 
 
 What does the version number mean?
 ----------------------------------
 
 Nothing at all but indicate which version is more fresh.  A higher version
 number means it is more recently released.
@@ -174,15 +174,14 @@
 overhead.
 
     $ sudo damo schemes --damos_access_rate 0 0 --damos_sz_region 4K max \
                         --damos_age 60s max --damos_action pageout \
                         <pid of your workload>
 
 Note: Previously, one-line scheme specification format like below was used.  It
-is now DEPRECATED, and the support will be removed by 2023 Q2.  Please report
-your usecase to sj@kernel.org, damon@lists.linux.dev and linux-mm@kvack.org if
-you depend on those.
+is now DEPRECATED.  Please report your usecase to sj@kernel.org,
+damon@lists.linux.dev and linux-mm@kvack.org if you depend on those.
 
     $ # !!! BELOW IS NO MORE SUPPORTED
     $ echo "#min-size max-size min-acc max-acc min-age max-age action" > my_scheme
     $ echo "4K        max      0       0       60s     max     pageout" >> my_scheme
     $ sudo damo schemes -c my_scheme <pid of your workload>
```

### Comparing `damo-1.8.0/src/damo.egg-info/SOURCES.txt` & `damo-1.8.1/src/damo.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 src/damo/damo_heats.py
 src/damo/damo_lru_sort.py
 src/damo/damo_monitor.py
 src/damo/damo_nr_regions.py
 src/damo/damo_reclaim.py
 src/damo/damo_record.py
 src/damo/damo_report.py
+src/damo/damo_report_json.py
 src/damo/damo_report_raw.py
 src/damo/damo_schemes.py
 src/damo/damo_start.py
 src/damo/damo_stat.py
 src/damo/damo_stat_kdamonds.py
 src/damo/damo_stat_regions.py
 src/damo/damo_stat_schemes.py
```

