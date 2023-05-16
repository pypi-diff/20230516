# Comparing `tmp/opn_sonarqube_api-2.0.0.320423.tar.gz` & `tmp/opn_sonarqube_api-2.1.0.486996.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/opn_sonarqube_api-2.0.0.320423.tar", last modified: Fri Feb 21 17:36:57 2020, max compression
+gzip compressed data, was "dist/opn_sonarqube_api-2.1.0.486996.tar", last modified: Thu Sep 10 14:37:52 2020, max compression
```

## Comparing `opn_sonarqube_api-2.0.0.320423.tar` & `opn_sonarqube_api-2.1.0.486996.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/
--rw-rw-rw-   0 root         (0) root         (0)       96 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      174 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    17374 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/
--rw-rw-rw-   0 root         (0) root         (0)       36 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/users.py
--rw-rw-rw-   0 root         (0) root         (0)     1786 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/user_token.py
--rw-rw-rw-   0 root         (0) root         (0)     1123 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     3257 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/rules.py
--rw-rw-rw-   0 root         (0) root         (0)     9274 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/components.py
--rw-rw-rw-   0 root         (0) root         (0)     4868 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     1309 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6598 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/qualitygates.py
--rw-rw-rw-   0 root         (0) root         (0)     2425 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/groups.py
--rw-rw-rw-   0 root         (0) root         (0)     6330 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/qualityprofiles.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/cmd/
--rw-rw-rw-   0 root         (0) root         (0)       33 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/cmd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5675 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/cmd/export_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     5331 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/cmd/migrate_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     3248 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/cmd/activate_rules.py
--rw-rw-rw-   0 root         (0) root         (0)     2764 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/sonarqube_api/api.py
--rw-r--r--   0 root         (0) root         (0)     5966 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      238 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     4135 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       67 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/DESCRIPTION.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/tests/
--rw-rw-rw-   0 root         (0) root         (0)       24 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15957 2020-02-21 17:36:20.000000 opn_sonarqube_api-2.0.0.320423/tests/test_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2415 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/opn_sonarqube_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)       20 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/opn_sonarqube_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/opn_sonarqube_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     5966 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/opn_sonarqube_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      208 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/opn_sonarqube_api.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/opn_sonarqube_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1058 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/opn_sonarqube_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-02-21 17:36:57.000000 opn_sonarqube_api-2.0.0.320423/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/
+-rw-rw-rw-   0 root         (0) root         (0)       96 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      174 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      204 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17756 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/users.py
+-rw-rw-rw-   0 root         (0) root         (0)     1891 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/user_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     3294 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     9729 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/components.py
+-rw-rw-rw-   0 root         (0) root         (0)     4868 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     1309 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     7523 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/qualitygates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2566 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/groups.py
+-rw-rw-rw-   0 root         (0) root         (0)     6505 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/qualityprofiles.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5675 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/export_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     5331 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/migrate_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     3248 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/activate_rules.py
+-rw-rw-rw-   0 root         (0) root         (0)     3015 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/sonarqube_api/api.py
+-rw-r--r--   0 root         (0) root         (0)     5923 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      238 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       67 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/DESCRIPTION.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15993 2020-09-10 14:36:31.000000 opn_sonarqube_api-2.1.0.486996/tests/test_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2353 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       20 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     5923 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      208 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1058 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2020-09-10 14:37:52.000000 opn_sonarqube_api-2.1.0.486996/setup.cfg
```

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonar.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonar.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,18 @@
     """
     # Default host is local
     DEFAULT_HOST = 'http://localhost'
     DEFAULT_PORT = 9000
     DEFAULT_BASE_PATH = ''
 
     def __init__(self, host=None, port=None, user=None, password=None,
-                 base_path=None, token=None):
+                 base_path=None, token=None, headers=None):
 
         self.api = SonarAPIHandler(host=host or self.DEFAULT_HOST, port=port or self.DEFAULT_PORT, user=user, password=password,
-                                   base_path=base_path or self.DEFAULT_BASE_PATH, token=token)
+                                   base_path=base_path or self.DEFAULT_BASE_PATH, token=token, headers=headers)
         self._group = SonarAPIGroup(api=self.api)
         self._permissions = SonarAPIPermissionTemplates(api=self.api)
         self._user_token = SonarAPIUserToken(api=self.api)
         self._user = SonarAPIUser(api=self.api)
         self._metrics = SonarAPIMetrics(api=self.api)
         self._qualityprofile = SonarAPIQualityProfile(api=self.api)
         self._resources = SonarAPIResources(api=self.api)
@@ -404,14 +404,24 @@
         :param query: query to send
         :param ps: pageSize
         :param selected: all/selected/deselected
         :return: request response
         """
         return self._qgates.search_project(gateId, query, ps, selected)
 
+    def qg_get_for_project(self, project, organization='default-organization'):
+        """
+        get qg summary for a project
+
+        :param project: project to use
+        :param organization: organization or 'default-organization'
+        :return: request response
+        """
+        return self._qgates.get_for_project(project, organization)
+
     def create_condition_qualitygates(self, gateid, metric, op, error):
         """
         create a condition for a quality gate
 
         :param gateid: id of the quality gate
         :param metric: metric of the condition
         :param op: operator of the condition
```

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/authentication.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/authentication.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/user_token.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/user_token.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         data = {
             'name': token_name,
             'login': user_login
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.USER_TOKEN_GENERATE_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def revoke_token(self, token_name, user_login):
         """
         Revoke user token.
 
         :param token_name: name of the token to revoke
         :param user_login: user to generate token for
@@ -40,20 +40,20 @@
         data = {
             'name': token_name,
             'login': user_login
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.USER_TOKEN_REVOKE_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def search_token(self, user_login):
         """
         List existing token for user.
         """
         data = {
             'login': user_login
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.USER_TOKEN_SEARCH_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
```

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/settings.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         # Build main data to post
         data = {
             'keys': key
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.GET_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def set(self, key, value):
         """
         Retrieve setting.
 
         :param key: name of the setting to update
         :param value: value to set
@@ -37,9 +37,9 @@
         data = {
             'key': key,
             'value': value
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.SET_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
```

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/rules.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             'severity': severity.upper(),
             'status': status.upper(),
             'template_key': template_key
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.RULES_CREATE_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def get_rules(self, active_only=False, profile=None, languages=None,
                   custom_only=False):
         """
         Yield rules in status ready, that are not template rules.
 
         :param active_only: filter only active rules
@@ -85,8 +85,8 @@
             n_rules = res['total']
 
             # Update page number (next) in queryset
             qs['p'] = page_num + 1
 
             # Yield rules
             for rule in res['rules']:
-                yield rule
+                yield rule
```

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/permissions.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/permissions.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             'name': template_name,
             'description': template_description,
             'projectKeyPattern': project_key_pattern
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_TEMPLATE_CREATE_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def search_template(self, template_name):
         """
         Search template with specified name.
 
         :param template_name: name of the group
         :return: request response
@@ -54,15 +54,15 @@
         # Build main data to post
         data = {
             'q': template_name
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_TEMPLATE_LIST_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def delete_template(self, template_id):
         """
         Delete template id.
 
         :param template_id: id of the template to delete
         :return: request response
@@ -70,15 +70,15 @@
         # Build main data to post
         data = {
             'templateId': template_id
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_TEMPLATE_DELETE_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def update_template(self, template_id, template_name, template_description, project_key_pattern):
         """
         update permission template.
 
         :param template_id: id of the template to update
         :param template_name: new name
@@ -92,15 +92,15 @@
             'name': template_name,
             'description': template_description,
             'projectKeyPattern': project_key_pattern
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_TEMPLATE_UPDATE_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def list_groups_of_template(self, template_id):
         """
         get permission template's groups.
 
         :param template_id: id of the template to update
         :return: request response
@@ -108,15 +108,15 @@
         # Build main data to post
         data = {
             'templateId': template_id,
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_TEMPLATE_GROUPS, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def add_group_to_template(self, template_id, group_name, permission):
         """
         update permission template.
 
         :param template_id: id of the template to update
         :param group_name: name of the group to associate
@@ -128,15 +128,15 @@
             'templateId': template_id,
             'groupName': group_name,
             'permission': permission
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_TEMPLATE_ADD_GROUP, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def remove_group_from_template(self, template_id, group_name, permission):
         """
         update permission template.
 
         :param template_id: id of the template to update
         :param group_name: name of the group to associate
@@ -148,15 +148,15 @@
             'templateId': template_id,
             'groupName': group_name,
             'permission': permission
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_TEMPLATE_REMOVE_GROUP, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def add_permission_to_user(self, user_name, permission):
         """
         update user's permission.
 
         :param user_name: name of the group to associate
         :param permission: permission to set in ['admin', 'gateadmin', 'profileadmin', 'scan', 'provisioning']
@@ -166,15 +166,15 @@
         data = {
             'login': user_name,
             'permission': permission
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_ADD_USER, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def remove_permission_to_user(self, user_name, permission):
         """
         update user's permission.
 
         :param user_name: name of the group to associate
         :param permission: permission to remove in ['admin', 'gateadmin', 'profileadmin', 'scan', 'provisioning']
@@ -184,15 +184,15 @@
         data = {
             'login': user_name,
             'permission': permission
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_REMOVE_USER, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def search_permission_for_user(self, user_name):
         """
         list user permission.
 
         :param user_name: name of the user to search
         :return: request response
@@ -201,15 +201,15 @@
         data = {
             'q': user_name,
             'ps': 100
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_SEARCH_USER, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def add_permission_to_group(self, group_name, permission):
         """
         update group's permission.
 
         :param group_name: name of the group to associate
         :param permission: permission to set in ['admin', 'gateadmin', 'profileadmin', 'scan', 'provisioning']
@@ -219,15 +219,15 @@
         data = {
             'groupName': group_name,
             'permission': permission
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_ADD_GROUP, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def remove_permission_to_group(self, group_name, permission):
         """
         update group's permission.
 
         :param group_name: name of the group to associate
         :param permission: permission to remove in ['admin', 'gateadmin', 'profileadmin', 'scan', 'provisioning']
@@ -237,15 +237,15 @@
         data = {
             'groupName': group_name,
             'permission': permission
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_REMOVE_GROUP, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def search_permission_for_group(self, group_name):
         """
         list groups permission.
 
         :param group_name: name of the group to associate
         :return: request response
@@ -254,8 +254,8 @@
         data = {
             'q': group_name,
             'ps': 100
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PERMISSIONS_SEARCH_GROUP, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
```

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/components.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/components.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,10 +20,10 @@
             'ps': ps,
             'facets': facets,
             'f': f
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.SEARCH_PROJECT_ENDPOINT, params=query)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
```

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/resources.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/resources.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/metrics.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/metrics.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/qualitygates.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/qualitygates.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # Endpoint for resources and rules
     LIST_ENDPOINT = '/api/qualitygates/list'
     DETAIL_ENDPOINT = '/api/qualitygates/show'
     CREATE_ENDPOINT = '/api/qualitygates/create'
     DESTROY_ENDPOINT = '/api/qualitygates/destroy'
     SELECT_ENDPOINT = '/api/qualitygates/select'
     SEARCH_ENDPOINT = '/api/qualitygates/search'
-
+    PROJECT_ENDPOINT = '/api/qualitygates/get_by_project'
     CREATE_COND_ENDPOINT = '/api/qualitygates/create_condition'
     DELETE_COND_ENDPOINT = '/api/qualitygates/delete_condition'
     UPDATE_COND_ENDPOINT = '/api/qualitygates/update_condition'
 
     def __init__(self, api=None):
         self._api = api
 
@@ -52,15 +52,15 @@
         """
         list quality gates.
 
         :return: request response
         """
         # Make call (might raise exception) and return
         res = self._api._make_call('get', self.LIST_ENDPOINT)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def show(self, id=None, name=None):
         """
         get quality gate details, using id or name (id is prior is both are set)
 
         :param id: id of the quality gate
         :param name: name of the quality gate
@@ -69,15 +69,15 @@
         # Build main data to post
         params = {
             'id' if id is not None else 'name': id if id is not None else name
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('get', self.DETAIL_ENDPOINT, params=params)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def create(self, name):
         """
         create a new empty quality agte
 
         :param name: name of the quality gate
         :return: request response
@@ -86,15 +86,15 @@
         data = {
             'name': name
         }
 
         # Make call (might raise exception) and return
         try:
             res = self._api._make_call('post', self.CREATE_ENDPOINT, data=data)
-            return json.loads(res.content)
+            return res if res.status_code == 204 else json.loads(res.content)
         except ValidationError:
             print ('Error trying to create quality gate: ', sys.exc_info()[1])
 
     def destroy(self, id):
         """
         delete a quality agte
 
@@ -142,15 +142,33 @@
             'ps': ps,
             'selected': selected,
             'gateId': gateId
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.SEARCH_ENDPOINT, params=query)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
+
+    def get_for_project(self, project, organization='default-organization'):
+        """
+        get qg summary for a project
+
+        :param project: project to use
+        :param organization: organization or 'default-organization'
+        :return: request response
+        """
+        # Build main data to post
+        data = {
+            'project': project,
+            'organization': organization
+        }
+
+        # Make call (might raise exception) and return
+        res = self._api._make_call('post', self.PROJECT_ENDPOINT, data=data)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def create_condition(self, gateid, metric, op, error):
         """
         create a condition for a quality gate
 
         :param gateid: id of the quality gate
         :param metric: metric of the condition
@@ -165,15 +183,15 @@
             'op': op,
             'error': error
         }
 
         # Make call (might raise exception) and return
         try:
             res = self._api._make_call('post', self.CREATE_COND_ENDPOINT, data=data)
-            return json.loads(res.content)
+            return res if res.status_code == 204 else json.loads(res.content)
         except ClientError:
             print ('Error trying to create condition for quality gate %s with metric %s, op %s, and error %s.' % (gateid, metric, op, error))
 
     def delete_condition(self, id):
         """
         delete a condition in quality gate
 
@@ -186,15 +204,15 @@
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.DELETE_COND_ENDPOINT, data=data)
         # Return none in case of 404 not found
         if res is None:
             return res
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def update_condition(self, id, metric, op, error):
         """
         update a condition for a quality gate
 
         :param id: id of the condition
         :param metric: metric of the condition
@@ -208,8 +226,8 @@
             'metric': metric,
             'op': op,
             'error': error
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.UPDATE_COND_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
```

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/groups.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/groups.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         data = {
             'name': group_name,
             'description': group_description
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.GROUP_CREATE_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def search_group(self, group_name):
         """
         Search group with specified name.
 
         :param group_name: name of the group
         :return: request response
@@ -39,15 +39,15 @@
         # Build main data to post
         data = {
             'q': group_name
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.GROUP_LIST_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def delete_group(self, group_id):
         """
         Delete group id.
 
         :param group_id: id of the group
         :return: request response
@@ -55,15 +55,15 @@
         # Build main data to post
         data = {
             'id': group_id
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.GROUP_DELETE_ENDPOINT_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def update_group(self, group_id, group_name, group_description):
         """
         Delete group id.
 
         :param group_id: id of the group to update
         :param group_name: new name
@@ -75,8 +75,8 @@
             'id': group_id,
             'name': group_name,
             'description': group_description
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.GROUP_UPDATE_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
```

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/sonarapi/qualityprofiles.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/sonarapi/qualityprofiles.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             'ps': ps,
             'selected': selected,
             'key': key
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.PROJECTS_ENDPOINT, params=query)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def restore_quality_profile_from_xml(self, backup, project_name):
         """
         Create a quality profile with rules from a xml file
 
         :param project_name: name of the project, used to name the profile
         :param backup: contents of xml file to config quality profile
@@ -59,30 +59,30 @@
         if existing_qp is not None and existing_qp["profiles"] is not None:
             for profile in existing_qp["profiles"]:
                 if profile['name'] == project_name and profile['language'] == language:
                     self.delete_quality_profile(project_name, language)
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.RESTORE_QUALITY_PROFILE_FROM_XML_ENDPOINT, files=dict(backup=backup))
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def search_quality_profile(self, profile_name):
         """
 
         :param profile_name:
         :return:
         """
 
         data = {
             'profileName': profile_name
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('get', self.SEARCH_QUALITY_PROFILE_ENDPOINT, data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def delete_quality_profile(self, profile_name, language):
         """
 
         :param profileName:
         :return:
         """
@@ -118,15 +118,15 @@
             'isInherited': isinherited,
             'isDefault': isdefault,
             'organization': organization
         }
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.CREATE_QUALITY_PROFILE_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
 
     def add_project_to_quality_profile(self, profile_key, project_key):
         """
         Adds the project to the quality profile
 
         :param profile_key: key of the profile
         :param project_key: key of the project
@@ -169,8 +169,8 @@
             # Note: sort by key to allow checking easily
             params = ';'.join('{}={}'.format(k, v) for k, v in sorted(params.items()) if v)
             if params:
                 data['params'] = params
 
         # Make call (might raise exception) and return
         res = self._api._make_call('post', self.RULES_ACTIVATION_ENDPOINT, data=data)
-        return json.loads(res.content)
+        return res if res.status_code == 204 else json.loads(res.content)
```

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/cmd/export_rules.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/export_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/cmd/migrate_rules.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/migrate_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/cmd/activate_rules.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/cmd/activate_rules.py`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.0.0.320423/sonarqube_api/api.py` & `opn_sonarqube_api-2.1.0.486996/sonarqube_api/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 import requests
 from .exceptions import ClientError, AuthError, ValidationError, ServerError
 
 
 class SonarAPIHandler(object):
 
     def __init__(self, host=None, port=None, user=None, password=None,
-                 base_path=None, token=None):
+                 base_path=None, token=None, headers=None):
         """
         Set connection info and session, including auth (if user+password
         and/or auth token were provided).
         """
         self._host = host
         self._port = port
         self._base_path = base_path
         self._session = requests.Session()
+        self._headers = headers
 
         # Prefer revocable authentication token over username/password if
         # both are provided
         if token:
             self._session.auth = token, ''
         elif user and password:
             self._session.auth = user, password
@@ -31,15 +32,15 @@
         Return the complete url including host and port for a given endpoint.
 
         :param endpoint: service endpoint as str
         :return: complete url (including host and port) as str
         """
         return '{}:{}{}{}'.format(self._host, self._port, self._base_path, endpoint)
 
-    def _make_call(self, method, endpoint, data={}, params={}, files=None):
+    def _make_call(self, method, endpoint, data={}, params={}, files=None, headers=None):
         """
         Make the call to the service with the given method, queryset and data,
         using the initial session.
 
         Note: data is not passed as a single dictionary for better testability
         (see https://github.com/kako-nawao/python-sonarqube-api/issues/15).
 
@@ -47,15 +48,21 @@
         :param endpoint: relative url to make the call
         :param data: queryset or body
         :return: response
         """
         # Get method and make the call
         call = getattr(self._session, method.lower())
         url = self.get_url(endpoint)
-        res = call(url, data=data, params=params, files=files)
+
+        _headers = {}
+        if headers is not None:
+            _headers.update(headers)
+        if self._headers is not None:
+            _headers.update(self._headers)
+        res = call(url, data=data, params=params, files=files, headers=_headers)
 
         # Analyse response status and return or raise exception
         # Note: redirects are followed automatically by requests
         if res.status_code < 300:
             # OK, return http response
             return res
```

### Comparing `opn_sonarqube_api-2.0.0.320423/PKG-INFO` & `opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
-Name: opn_sonarqube_api
-Version: 2.0.0.320423
+Name: opn-sonarqube-api
+Version: 2.1.0.486996
 Summary: Open SonarQube API Handler
-Home-page: https://github.com/kako-nawao/python-sonarqube-api
+Home-page: UNKNOWN
 Author: open sas
 Author-email: sebastien.bettinger@open-groupe.com
 License: MIT
 Description: ====================
         Python SonarQube API
         ====================
```

### Comparing `opn_sonarqube_api-2.0.0.320423/README.rst` & `opn_sonarqube_api-2.1.0.486996/README.rst`

 * *Files identical despite different names*

### Comparing `opn_sonarqube_api-2.0.0.320423/tests/test_api.py` & `opn_sonarqube_api-2.1.0.486996/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,27 +92,27 @@
         mock_post.return_value = resp
         with self.assertRaises(ValidationError):
             self.h.activate_rule(None, 'py-234454', reset=True, severity='MAJOR', format='^setUp|tearDown$', files=None)
 
         # Check call, params and severity were ignored
         url = self.h.get_url(self.h._qualityprofile.RULES_ACTIVATION_ENDPOINT)
         mock_post.assert_called_with(url, data={'rule_key': None, 'profile_key': 'py-234454', 'reset': 'true'},
-                                     params={}, files=None)
+                                     params={}, files=None, headers={})
         mock_post.reset_mock()
 
         # Now post proper data, with
         resp.status_code = 200
         resp.json.return_value = {'result': 'ok'}
         resp.content = json.dumps(resp.json.return_value)
         self.h.activate_rule('py:S1291', 'py-234454', format='^setUp|tearDown$')
 
         # Check call, params and severity added
         mock_post.assert_called_with(url, data={'rule_key': 'py:S1291', 'profile_key': 'py-234454',
                                                 'reset': 'false', 'params': 'format=^setUp|tearDown$'},
-                                     files=None, params={})
+                                     files=None, params={}, headers={})
 
     @mock.patch('sonarqube_api.api.requests.Session.post')
     def test_create_rule(self, mock_post):
         # Rule exists, error
         resp = mock.MagicMock(status_code=400)
         resp.json.return_value = {'errors': [{'msg': 'rule already exists'}]}
         resp.content = json.dumps(resp.json.return_value)
@@ -132,15 +132,15 @@
         posted_data = {
             'custom_key': 'x1', 'name': 'Do not frobnicate',
             'markdown_description': 'Frobnicating is wrong and should be avoided',
             'params': 'message=Reemove forbnication;xpathQuery=DEFFN/SJS',
             'severity': 'MAJOR', 'status': 'ACTIVE', 'template_key': 'XPath'
         }
         url = self.h.get_url(self.h._rules.RULES_CREATE_ENDPOINT)
-        mock_post.assert_called_with(url, data=posted_data, params={}, files=None)
+        mock_post.assert_called_with(url, data=posted_data, params={}, files=None, headers={})
 
     @mock.patch('sonarqube_api.api.SonarAPIHandler._make_call')
     def test_get_metrics(self, mock_call):
         # Two pages, once each
         resp = mock.MagicMock(status_code=200)
         resp.json.side_effect = [
             {'p': 1, 'ps': 2, 'total': 3, 'metrics': [{'project': 'lala', 'coverage': 70, 'violations': 56},
```

### Comparing `opn_sonarqube_api-2.0.0.320423/setup.py` & `opn_sonarqube_api-2.1.0.486996/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,18 @@
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='opn_sonarqube_api',
 
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='2.0.0.320423',
+    version='2.1.0.486996',
 
     description='Open SonarQube API Handler',
     long_description=long_description,
-    url='https://github.com/kako-nawao/python-sonarqube-api',
     author='open sas',
     author_email='sebastien.bettinger@open-groupe.com',
     license='MIT',
 
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         'Development Status :: 5 - Production/Stable',
```

### Comparing `opn_sonarqube_api-2.0.0.320423/opn_sonarqube_api.egg-info/PKG-INFO` & `opn_sonarqube_api-2.1.0.486996/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
-Name: opn-sonarqube-api
-Version: 2.0.0.320423
+Name: opn_sonarqube_api
+Version: 2.1.0.486996
 Summary: Open SonarQube API Handler
-Home-page: https://github.com/kako-nawao/python-sonarqube-api
+Home-page: UNKNOWN
 Author: open sas
 Author-email: sebastien.bettinger@open-groupe.com
 License: MIT
 Description: ====================
         Python SonarQube API
         ====================
```

### Comparing `opn_sonarqube_api-2.0.0.320423/opn_sonarqube_api.egg-info/SOURCES.txt` & `opn_sonarqube_api-2.1.0.486996/opn_sonarqube_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

