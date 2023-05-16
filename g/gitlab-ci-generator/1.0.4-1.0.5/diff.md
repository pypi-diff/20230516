# Comparing `tmp/gitlab-ci-generator-1.0.4.tar.gz` & `tmp/gitlab-ci-generator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlab-ci-generator-1.0.4.tar", last modified: Mon May 15 17:33:34 2023, max compression
+gzip compressed data, was "gitlab-ci-generator-1.0.5.tar", last modified: Tue May 16 20:16:36 2023, max compression
```

## Comparing `gitlab-ci-generator-1.0.4.tar` & `gitlab-ci-generator-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/
--rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.4/MANIFEST.in
--rw-r--r--   0 developer  (9999) developer  (9999)     8723 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/PKG-INFO
--rw-rw-rw-   0 developer  (9999) developer  (9999)     8374 2022-09-07 16:43:31.000000 gitlab-ci-generator-1.0.4/README.md
--rw-r--r--   0 developer  (9999) developer  (9999)        6 2023-05-15 17:33:33.000000 gitlab-ci-generator-1.0.4/VERSION.txt
--rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/setup.cfg
--rw-rw-rw-   0 developer  (9999) developer  (9999)     1113 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.4/setup.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/src/
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/
--rw-r--r--   0 developer  (9999) developer  (9999)     8723 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/PKG-INFO
--rw-r--r--   0 developer  (9999) developer  (9999)      499 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/SOURCES.txt
--rw-r--r--   0 developer  (9999) developer  (9999)        1 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/dependency_links.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       93 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/entry_points.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       29 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/requires.txt
--rw-r--r--   0 developer  (9999) developer  (9999)       28 2023-05-15 17:33:34.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/top_level.txt
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/
--rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/__init__.py
--rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/gitlab_ci_generator.py
-drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-15 17:33:34.066469 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/templates/
--rw-rw-rw-   0 developer  (9999) developer  (9999)     1896 2022-09-06 14:08:49.000000 gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       83 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.5/MANIFEST.in
+-rw-r--r--   0 developer  (9999) developer  (9999)     8787 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/PKG-INFO
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     8438 2023-05-16 20:16:20.000000 gitlab-ci-generator-1.0.5/README.md
+-rw-r--r--   0 developer  (9999) developer  (9999)        6 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/VERSION.txt
+-rw-rw-rw-   0 developer  (9999) developer  (9999)       78 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/setup.cfg
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     1113 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.5/setup.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/src/
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/
+-rw-r--r--   0 developer  (9999) developer  (9999)     8787 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/PKG-INFO
+-rw-r--r--   0 developer  (9999) developer  (9999)      499 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)        1 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       93 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/entry_points.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       29 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/requires.txt
+-rw-r--r--   0 developer  (9999) developer  (9999)       28 2023-05-16 20:16:36.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/top_level.txt
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)        0 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/__init__.py
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     5706 2022-09-02 17:24:19.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/gitlab_ci_generator.py
+drwxr-xr-x   0 developer  (9999) developer  (9999)        0 2023-05-16 20:16:36.244666 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/templates/
+-rw-rw-rw-   0 developer  (9999) developer  (9999)     1933 2023-05-16 20:06:50.000000 gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/templates/gitlab-template.jinja
```

### Comparing `gitlab-ci-generator-1.0.4/PKG-INFO` & `gitlab-ci-generator-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-ci-generator
-Version: 1.0.4
+Version: 1.0.5
 Summary: Generates a mono-repo ci file.
 Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
 Author: Gary Schaetz
 Author-email: gary@schaetzkc.com
 License: MIT
 Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
 Description-Content-Type: text/markdown
@@ -127,14 +127,15 @@
   - build
   - post-deploy
 
 example-1:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-1
+    PROJECT_JOB_NAME: example-1
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
       changes:
@@ -144,14 +145,15 @@
     include: example/example-folder-1/.gitlab-example.yml    
     strategy: depend
  
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
+    PROJECT_JOB_NAME: example-2
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-2/**/*
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
```

### Comparing `gitlab-ci-generator-1.0.4/README.md` & `gitlab-ci-generator-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
   - build
   - post-deploy
 
 example-1:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-1
+    PROJECT_JOB_NAME: example-1
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
       changes:
@@ -133,14 +134,15 @@
     include: example/example-folder-1/.gitlab-example.yml    
     strategy: depend
  
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
+    PROJECT_JOB_NAME: example-2
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-2/**/*
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
```

### Comparing `gitlab-ci-generator-1.0.4/setup.py` & `gitlab-ci-generator-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.4/src/gitlab_ci_generator.egg-info/PKG-INFO` & `gitlab-ci-generator-1.0.5/src/gitlab_ci_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlab-ci-generator
-Version: 1.0.4
+Version: 1.0.5
 Summary: Generates a mono-repo ci file.
 Home-page: https://gitlab.com/gary.schaetz/public/gitlab-ci-generator
 Author: Gary Schaetz
 Author-email: gary@schaetzkc.com
 License: MIT
 Keywords: gitlab,template,generator,gitlab-ci.yml,dynamic,pipeline
 Description-Content-Type: text/markdown
@@ -127,14 +127,15 @@
   - build
   - post-deploy
 
 example-1:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-1
+    PROJECT_JOB_NAME: example-1
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
       changes:
@@ -144,14 +145,15 @@
     include: example/example-folder-1/.gitlab-example.yml    
     strategy: depend
  
 example-2:
   stage: build
   variables:
     PROJECT_SUBDIR: example/example-folder-2
+    PROJECT_JOB_NAME: example-2
   rules:
     - if: !reference [.job_changes_rules,standard-rule-if]
       changes:
         - example/example-folder-2/**/*
         - example/example-folder-1/**/*
     - if: !reference [.job_changes_rules,manual-rule-if]
       when: manual
```

### Comparing `gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/gitlab_ci_generator.py` & `gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/gitlab_ci_generator.py`

 * *Files identical despite different names*

### Comparing `gitlab-ci-generator-1.0.4/src/gitlab_ci_generator_package/templates/gitlab-template.jinja` & `gitlab-ci-generator-1.0.5/src/gitlab_ci_generator_package/templates/gitlab-template.jinja`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 {% endif %}
 
 {% for job in jobs %}
 {{ job.name }}:
   stage: build
   variables:
     PROJECT_SUBDIR: {{ job.folder }}
+    PROJECT_JOB_NAME: {{ job.name }}
   rules:
 {% for rule in pipeline_info.shared_reference_rules %}
     - if: !reference [{{ rule.rule_source }},{{ rule.rule_name }}]
 {% if rule.when %}
       when: {{ rule.when }}
 {% endif -%}
 {% if rule.only_changes == true %}
```

