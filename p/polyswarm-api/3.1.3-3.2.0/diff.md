# Comparing `tmp/polyswarm-api-3.1.3.tar.gz` & `tmp/polyswarm-api-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyswarm-api-3.1.3.tar", last modified: Mon Mar 13 17:35:40 2023, max compression
+gzip compressed data, was "polyswarm-api-3.2.0.tar", last modified: Tue Mar 21 20:11:10 2023, max compression
```

## Comparing `polyswarm-api-3.1.3.tar` & `polyswarm-api-3.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 17:35:40.892897 polyswarm-api-3.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-03-13 17:35:15.000000 polyswarm-api-3.1.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-13 17:35:15.000000 polyswarm-api-3.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1756 2023-03-13 17:35:40.892897 polyswarm-api-3.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-03-13 17:35:15.000000 polyswarm-api-3.1.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-03-13 17:35:15.000000 polyswarm-api-3.1.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-13 17:35:40.892897 polyswarm-api-3.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-03-13 17:35:15.000000 polyswarm-api-3.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 17:35:40.888897 polyswarm-api-3.1.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 17:35:40.888897 polyswarm-api-3.1.3/src/polyswarm_api/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-13 17:35:15.000000 polyswarm-api-3.1.3/src/polyswarm_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    31165 2023-03-13 17:35:15.000000 polyswarm-api-3.1.3/src/polyswarm_api/api.py
--rw-rw-rw-   0 root         (0) root         (0)    20044 2023-03-13 17:35:15.000000 polyswarm-api-3.1.3/src/polyswarm_api/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-03-13 17:35:15.000000 polyswarm-api-3.1.3/src/polyswarm_api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    36203 2023-03-13 17:35:15.000000 polyswarm-api-3.1.3/src/polyswarm_api/resources.py
--rw-rw-rw-   0 root         (0) root         (0)      967 2023-03-13 17:35:15.000000 polyswarm-api-3.1.3/src/polyswarm_api/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-13 17:35:40.892897 polyswarm-api-3.1.3/src/polyswarm_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1756 2023-03-13 17:35:40.000000 polyswarm-api-3.1.3/src/polyswarm_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-03-13 17:35:40.000000 polyswarm-api-3.1.3/src/polyswarm_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-13 17:35:40.000000 polyswarm-api-3.1.3/src/polyswarm_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-03-13 17:35:40.000000 polyswarm-api-3.1.3/src/polyswarm_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-13 17:35:40.000000 polyswarm-api-3.1.3/src/polyswarm_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      951 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/src/polyswarm_api/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    31285 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    20072 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1431 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    36029 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)      967 2023-03-21 20:10:43.000000 polyswarm-api-3.2.0/src/polyswarm_api/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 20:11:10.382619 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1756 2023-03-21 20:11:10.000000 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-03-21 20:11:10.000000 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 20:11:10.000000 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-03-21 20:11:10.000000 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-03-21 20:11:10.000000 polyswarm-api-3.2.0/src/polyswarm_api.egg-info/top_level.txt
```

### Comparing `polyswarm-api-3.1.3/LICENSE` & `polyswarm-api-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.1.3/PKG-INFO` & `polyswarm-api-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm-api
-Version: 3.1.3
+Version: 3.2.0
 Summary: Client library to simplify interacting with the PolySwarm consumer API
 Home-page: https://github.com/polyswarm/polyswarm-api
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `polyswarm-api-3.1.3/README.md` & `polyswarm-api-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.1.3/setup.py` & `polyswarm-api-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # The README.md will be used as the content for the PyPi package details page on the Python Package Index.
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 
 setup(
     name='polyswarm-api',
-    version='3.1.3',
+    version='3.2.0',
     description='Client library to simplify interacting with the PolySwarm consumer API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='PolySwarm Developers',
     author_email='info@polyswarm.io',
     url='https://github.com/polyswarm/polyswarm-api',
     license='MIT',
```

### Comparing `polyswarm-api-3.1.3/src/polyswarm_api/api.py` & `polyswarm-api-3.2.0/src/polyswarm_api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -651,22 +651,24 @@
         logger.info('Downloading %s into %s', hash_, out_dir)
         hash_ = resources.Hash.from_hashable(hash_, hash_type=hash_type)
         artifact = resources.LocalArtifact.download(self, hash_.hash, hash_.hash_type, folder=out_dir).result()
         artifact.handle.close()
 
         return artifact
 
-    def sandbox(self, sha256_hash):
+    def sandbox(self, instance_id):
+        logger.info('Sandboxing %s', instance_id)
+        return resources.SandboxResult.create(self, artifact_id=instance_id).result()
+
+    def sandbox_list(self):
         """
-        Send a scanned artifact by hash to the sandboxing system.
-        :param sha256_hash:
-        :param force: 
+        List sandboxes available in polyswarm.
         """
-        logger.info('Sandboxing %s', sha256_hash)
-        return resources.SandboxResult.sandbox(self, sha256_hash)
+        logger.info('Listing sandbox names')
+        return resources.SandboxName.list(self)
 
     def download_archive(self, out_dir, s3_path):
         """
         Grab the data in the s3 path provided in the stream() method, and write the contents
         in the provided directory.
         :param out_dir: Destination directory to download the file.
         :param s3_path: Target S3 object to download.
@@ -700,19 +702,20 @@
         logger.info('Streaming since %s', since)
         return resources.ArtifactArchive.get(self, since=since).result()
 
     def rerun_metadata(self, hashes, analyses=None, skip_es=None):
         logger.info('Rerunning metadata for hashes %s', hashes)
         return resources.ArtifactInstance.metadata_rerun(self, hashes, analyses=analyses, skip_es=skip_es).result()
 
-    def tool_metadata_create(self, sha256, tool, tool_metadata):
-        logger.info('Create tool metadata %s %s %s', sha256, tool, tool_metadata)
-        return resources.ToolMetadata.create(self, sha256=sha256, tool=tool, tool_metadata=tool_metadata).result()
+    def tool_metadata_create(self, instance_id, tool, tool_metadata):
+        logger.info('Create tool metadata %s %s %s', instance_id, tool, tool_metadata)
+        return resources.ToolMetadata.create(
+            self, instance_id=instance_id, tool=tool, tool_metadata=tool_metadata).result()
 
-    def tool_metadata_list(self, sha256):
+    def tool_metadata_list(self, instance_id):
         logger.info('List tool metadata')
-        return resources.ToolMetadata.list(self, sha256=sha256).result()
+        return resources.ToolMetadata.list(self, instance_id=instance_id).result()
 
     def __repr__(self):
         clsname = '{0.__module__}.{0.__name__}'.format(self.__class__)
         attrs = 'uri={0.uri!r}, community={0.community!r}, timeout={0.timeout!r}'.format(self)
         return '<{}({}) at 0x{:x}>'.format(clsname, attrs, id(self))
```

### Comparing `polyswarm-api-3.1.3/src/polyswarm_api/core.py` & `polyswarm-api-3.2.0/src/polyswarm_api/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
     def parse_result(cls, api, content, **kwargs):
         logger.debug('Parsing resource %s', cls.__name__)
         return cls(content, api=api, **kwargs)
 
 
 class BaseJsonResource(BaseResource):
     RESOURCE_ENDPOINT = None
-    RESOURCE_ID_KEY = 'id'
+    RESOURCE_ID_KEYS = ['id']
 
     def __init__(self, content, *args, **kwargs):
         super(BaseJsonResource, self).__init__(content, *args, **kwargs)
         self.json = content
 
     def __int__(self):
         id_ = getattr(self, 'id', None)
@@ -328,15 +328,15 @@
     @classmethod
     def _params(cls, method, *param_keys, **kwargs):
         params = {}
         json_params = {}
         for k, v in kwargs.items():
             if v is not None:
                 # try to parse "*_id" stuff as integer
-                if k.endswith('_id'):
+                if k == 'id' or k.endswith('_id'):
                     try:
                         parsed_value = str(int(v))
                     except Exception:
                         # fallback to string
                         parsed_value = str(v)
                 elif isinstance(v, bool):
                     parsed_value = int(v)
@@ -351,35 +351,35 @@
 
         params = params if params else None
         json_params = json_params if json_params else None
         return params, json_params
 
     @classmethod
     def _list_params(cls, **kwargs):
-        return cls._params('GET', cls.RESOURCE_ID_KEY, **kwargs)
+        return cls._params('GET', *cls.RESOURCE_ID_KEYS, **kwargs)
 
     @classmethod
     def _create_params(cls, **kwargs):
-        return cls._params('POST', cls.RESOURCE_ID_KEY, **kwargs)
+        return cls._params('POST', *cls.RESOURCE_ID_KEYS, **kwargs)
 
     @classmethod
     def _get_params(cls, **kwargs):
-        return cls._params('GET', cls.RESOURCE_ID_KEY, **kwargs)
+        return cls._params('GET', *cls.RESOURCE_ID_KEYS, **kwargs)
 
     @classmethod
     def _head_params(cls, **kwargs):
-        return cls._params('HEAD', cls.RESOURCE_ID_KEY, **kwargs)
+        return cls._params('HEAD', *cls.RESOURCE_ID_KEYS, **kwargs)
 
     @classmethod
     def _update_params(cls, **kwargs):
-        return cls._params('PUT', cls.RESOURCE_ID_KEY, **kwargs)
+        return cls._params('PUT', *cls.RESOURCE_ID_KEYS, **kwargs)
 
     @classmethod
     def _delete_params(cls, **kwargs):
-        return cls._params('DELETE', cls.RESOURCE_ID_KEY, **kwargs)
+        return cls._params('DELETE', *cls.RESOURCE_ID_KEYS, **kwargs)
 
     @classmethod
     def _list_headers(cls, api):
         return None
 
     @classmethod
     def _create_headers(cls, api):
```

### Comparing `polyswarm-api-3.1.3/src/polyswarm_api/exceptions.py` & `polyswarm-api-3.2.0/src/polyswarm_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.1.3/src/polyswarm_api/resources.py` & `polyswarm-api-3.2.0/src/polyswarm_api/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,16 @@
                 'url': '{}/ioc/known'.format(api.uri),
                 'params': {
                     'id': id
                 }
             },
             result_parser=cls,
         ).execute()
-        
+
+
 class ArtifactInstance(core.BaseJsonResource, core.Hashable):
     RESOURCE_ENDPOINT = '/instance'
 
     def __init__(self, content, api=None):
         super(ArtifactInstance, self).__init__(content=content, api=api,
                                                hash_value=content['sha256'], hash_type='sha256')
         # Artifact fields
@@ -819,15 +820,15 @@
 
 class HistoricalHuntResultList(HistoricalHuntResult):
     RESOURCE_ENDPOINT = '/hunt/historical/results/list'
 
 
 class TagLink(core.BaseJsonResource):
     RESOURCE_ENDPOINT = '/tags/link'
-    RESOURCE_ID_KEY = 'hash'
+    RESOURCE_ID_KEYS = ['hash']
 
     def __init__(self, content, api=None):
         super(TagLink, self).__init__(content, api=api)
         self.id = content.get('id')
         self.sha256 = content.get('sha256')
         self.created = core.parse_isoformat(content.get('created'))
         self.updated = core.parse_isoformat(content.get('updated'))
@@ -846,28 +847,28 @@
         params.extend(('or_family', p) for p in kwargs.get('or_families', empty))
         params.append(('emerging', kwargs.get('emerging', empty)))
         return params, None
 
 
 class MalwareFamily(core.BaseJsonResource):
     RESOURCE_ENDPOINT = '/tags/family'
-    RESOURCE_ID_KEY = 'name'
+    RESOURCE_ID_KEYS = ['name']
 
     def __init__(self, content, api=None):
         super(MalwareFamily, self).__init__(content, api=api)
         self.id = content.get('id')
         self.created = core.parse_isoformat(content.get('created'))
         self.updated = core.parse_isoformat(content.get('updated'))
         self.name = content.get('name')
         self.emerging = core.parse_isoformat(content.get('emerging'))
 
 
 class Tag(core.BaseJsonResource):
     RESOURCE_ENDPOINT = '/tags/tag'
-    RESOURCE_ID_KEY = 'name'
+    RESOURCE_ID_KEYS = ['name']
 
     def __init__(self, content, api=None):
         super(Tag, self).__init__(content, api=api)
         self.id = content.get('id')
         self.created = core.parse_isoformat(content.get('created'))
         self.updated = core.parse_isoformat(content.get('updated'))
         self.name = content.get('name')
@@ -970,24 +971,18 @@
     def __str__(self):
         return self.hash
 
     def __repr__(self):
         return "{}={}".format(self.hash_type, self.hash)
 
 
-class SandboxResult(core.BaseJsonResource):
+class SandboxResult(ArtifactInstance):
+    RESOURCE_ENDPOINT = "/sandbox"
+    RESOURCE_ID_KEYS = ['artifact_id']
 
-    def __init__(self, content, api=None):
-        super(SandboxResult, self).__init__(content, api=api)
 
-    @classmethod
-    def sandbox(cls, api, sha256):
-        return core.PolyswarmRequest(
-            api,
-            {
-                'method':
-                'POST',
-                'url':
-                '{}/consumer/submission/{}/sandbox/{}'.format(api.uri, api.community, sha256)
-            },
-            result_parser=cls,
-        ).execute()
+class SandboxName(core.BaseJsonResource):
+    RESOURCE_ENDPOINT = "/sandbox/name"
+
+    def __init__(self, content, api=None):
+        super(SandboxName, self).__init__(content, api=api)
+        self.name = content
```

### Comparing `polyswarm-api-3.1.3/src/polyswarm_api/settings.py` & `polyswarm-api-3.2.0/src/polyswarm_api/settings.py`

 * *Files identical despite different names*

### Comparing `polyswarm-api-3.1.3/src/polyswarm_api.egg-info/PKG-INFO` & `polyswarm-api-3.2.0/src/polyswarm_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyswarm-api
-Version: 3.1.3
+Version: 3.2.0
 Summary: Client library to simplify interacting with the PolySwarm consumer API
 Home-page: https://github.com/polyswarm/polyswarm-api
 Author: PolySwarm Developers
 Author-email: info@polyswarm.io
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

