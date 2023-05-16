# Comparing `tmp/billarchive-0.3.tar.gz` & `tmp/billarchive-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "billarchive-0.3.tar", last modified: Sun Sep 25 08:55:52 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `billarchive-0.3.tar` & `billarchive-0.4.tar`

### file list

```diff
@@ -1,17 +1,9 @@
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2022-09-25 08:55:52.259502 billarchive-0.3/
--rw-r--r--   0 ntome     (1000) ntome     (1000)      498 2022-09-25 08:55:50.000000 billarchive-0.3/COPYING.wtfpl
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1801 2022-09-25 08:55:52.259502 billarchive-0.3/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)      837 2022-09-25 08:55:50.000000 billarchive-0.3/README.md
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2022-09-25 08:55:52.259502 billarchive-0.3/billarchive/
--rw-r--r--   0 ntome     (1000) ntome     (1000)       20 2022-09-25 08:55:50.000000 billarchive-0.3/billarchive/__init__.py
--rw-r--r--   0 ntome     (1000) ntome     (1000)       53 2022-09-25 08:55:50.000000 billarchive-0.3/billarchive/__main__.py
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)     8005 2022-09-25 08:55:50.000000 billarchive-0.3/billarchive/billarchive.py
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2022-09-25 08:55:52.259502 billarchive-0.3/billarchive.egg-info/
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1801 2022-09-25 08:55:52.000000 billarchive-0.3/billarchive.egg-info/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)      329 2022-09-25 08:55:52.000000 billarchive-0.3/billarchive.egg-info/SOURCES.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        1 2022-09-25 08:55:52.000000 billarchive-0.3/billarchive.egg-info/dependency_links.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)       70 2022-09-25 08:55:52.000000 billarchive-0.3/billarchive.egg-info/entry_points.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)       34 2022-09-25 08:55:52.000000 billarchive-0.3/billarchive.egg-info/requires.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)       12 2022-09-25 08:55:52.000000 billarchive-0.3/billarchive.egg-info/top_level.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1074 2022-09-25 08:55:52.259502 billarchive-0.3/setup.cfg
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)      139 2022-09-25 08:55:50.000000 billarchive-0.3/setup.py
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 billarchive-0.4/config_example
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 billarchive-0.4/billarchive/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 billarchive-0.4/billarchive/__main__.py
+-rwxr-xr-x   0        0        0     9214 2020-02-02 00:00:00.000000 billarchive-0.4/billarchive/billarchive.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 billarchive-0.4/.gitignore
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 billarchive-0.4/COPYING.wtfpl
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 billarchive-0.4/README.md
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 billarchive-0.4/pyproject.toml
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 billarchive-0.4/PKG-INFO
```

### Comparing `billarchive-0.3/billarchive/billarchive.py` & `billarchive-0.4/billarchive/billarchive.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from dateutil.parser import parse as parse_date
 from dateutil.relativedelta import relativedelta
 import magic
 from woob.capabilities.base import empty, BaseObject
 from woob.capabilities.bill import CapDocument
 from woob.tools.application.repl import ReplApplication
+from woob.capabilities.base import NotLoaded, NotAvailable
 
 from . import __version__
 
 
 def to_datetime(obj):
     if isinstance(obj, datetime.date):
         obj = datetime.datetime.combine(obj, datetime.time())
@@ -59,31 +60,40 @@
 
 def parse_date_since(s):
     match = duration_re.fullmatch(s)
     if match:
         unit = match['unit']
         if not unit.endswith('s'):
             unit += 's'
-        return datetime.date.today() - relativedelta(**{unit: int(match['quantity'])})
+        return to_datetime(datetime.date.today() - relativedelta(**{unit: int(match['quantity'])}))
 
     try:
         return parse_date(s)
     except ValueError:
         pass
 
 
 class FilenameFormatter(Formatter):
+    def __init__(self, *args, slash_character_replacement=None, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.slash_character_replacement = slash_character_replacement or "_slash_"
+
     def convert_field(self, value, conv):
         protect = conv is None and isinstance(value, str)
 
         if conv == "u":
             conv = None
 
+        if (conv == "d"):
+            conv = None
+            if (value in [NotLoaded, NotAvailable]):
+                return datetime.datetime.min
+
         if protect:
-            value = value.replace("/", "_slash_")
+            value = value.replace("/", self.slash_character_replacement)
             if value.startswith("."):
                 value = f"dot_{value[1:]}"
             return value
         else:
             return super().convert_field(value, conv)
 
 
@@ -93,14 +103,26 @@
     def __init__(self, backend, app):
         self.backend = backend
         self.config = app.config
         self.storage = app.storage
         self.logger = getLogger(f'downloader.{backend.name}')
         self.app = app
 
+    def str2bool(self, str):
+        if str is True:
+            return True
+        if str is False:
+            return False
+        if str.upper() == "True".upper():
+            return True
+        if str.upper() == "False".upper():
+            return False
+        self.logger.error("Cannot convert '%s' to boolean." % str)
+        raise ValueError
+
     def get_date_until(self, subscription, is_initial=False):
         option = 'sync_until'
         if is_initial:
             option = 'initial_sync_until'
 
         v = None
         s = self.get_backend_config(option, default=None)
@@ -140,31 +162,29 @@
         accepted_types = self.get_backend_config('accepted_types', default='').strip().lower()
         if not accepted_types:
             return True
 
         return (document.type or '').lower() in accepted_types.split()
 
     def download_document(self, subscription, document):
-        formatter = FilenameFormatter()
-
         store_prefix = ('db', self.backend.name, subscription.id, 'documents', document.id)
         self._set_meta_info(store_prefix)
         self.storage.set(*store_prefix, 'object', to_dict(document))
 
         if not self.is_accepted_type(document):
             self.logger.info('%s document has no accepted type, no download', document)
             return
 
         template = self.get_backend_config('filename', default=self.default_filename)
-        filename = formatter.format(
+        filename = self.formatter.format(
             template,
             subscription=subscription, document=document, extension=document.format,
         )
         path = self.root_path() / filename
-        path.parent.mkdir(exist_ok=True)
+        path.parent.mkdir(exist_ok=True, parents=True)
 
         if not document.has_file:
             self.logger.info('%s document has no file, no download', document)
             return
 
         if path.exists():
             self.logger.info('%s already exists for document %s, no download', path, document)
@@ -192,34 +212,42 @@
         self.storage.set(*store_prefix, 'info', 'downloaded_at', datetime.datetime.now())
 
     def download_subscription(self, subscription):
         self.logger.debug('downloading subscription %s', subscription)
 
         store_prefix = ('db', self.backend.name, subscription.id, 'subscription')
 
-        is_initial = bool(self.storage.get(*store_prefix, 'info', 'first_seen', default=None))
+        is_initial = not bool(self.storage.get(*store_prefix, 'info', 'first_seen', default=None))
         self._set_meta_info(store_prefix)
         self.storage.set(*store_prefix, 'object', to_dict(subscription))
 
+        download_when_listing = self.str2bool(self.get_backend_config('download_when_listing', default=False))
+
         # collect documents first, some backends do not support well mixing download and listing
         documents = []
         for document in self.backend.iter_documents(subscription):
             # TODO timezones?
             if document.date and to_datetime(document.date) < self.get_date_until(subscription, is_initial):
                 self.logger.info('reached date threshold for %r', subscription)
                 break
 
-            documents.append(document)
+            if download_when_listing:
+                self.download_document(subscription, document)
+            else:
+                documents.append(document)
 
         for document in documents:
             self.download_document(subscription, document)
 
     def download(self):
+        slash_character_replacement = self.get_backend_config('slash_character_replacement', default=None)
+        self.formatter = FilenameFormatter(slash_character_replacement=slash_character_replacement)
+
         self.app.print('Processing backend %r' % self.backend.name)
-        self.root_path().mkdir(exist_ok=True)
+        self.root_path().mkdir(exist_ok=True, parents=True)
         for subscription in self.backend.iter_subscription():
             self.download_subscription(subscription)
 
 
 class BillDlApp(ReplApplication):
     APPNAME = 'billarchive'
     VERSION = __version__
@@ -234,15 +262,14 @@
             return BackendDownloader(backend, self).download()
 
         for _ in self._do_and_retry(download):
             pass
 
     def main(self, argv):
         self.load_config()
-        self.create_storage()
         try:
             return super().main(argv)
         finally:
             self.storage.save()
 
 
 if __name__ == '__main__':
```

