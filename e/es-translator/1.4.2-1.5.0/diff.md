# Comparing `tmp/es_translator-1.4.2.tar.gz` & `tmp/es_translator-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "es_translator-1.4.2.tar", max compression
+gzip compressed data, was "es_translator-1.5.0.tar", max compression
```

## Comparing `es_translator-1.4.2.tar` & `es_translator-1.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.4.2/LICENSE.txt
--rw-r--r--   0        0        0     3704 2023-05-10 10:53:32.886660 es_translator-1.4.2/README.md
--rw-r--r--   0        0        0      136 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/__init__.py
--rw-r--r--   0        0        0      490 2022-06-20 12:45:46.183755 es_translator-1.4.2/es_translator/alpha.py
--rw-r--r--   0        0        0     5013 2023-05-12 13:02:30.048545 es_translator-1.4.2/es_translator/cli.py
--rw-r--r--   0        0        0     1893 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/es.py
--rw-r--r--   0        0        0     5325 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/es_translator.py
--rw-r--r--   0        0        0       55 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/__init__.py
--rw-r--r--   0        0        0     1690 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/abstract.py
--rw-r--r--   0        0        0       30 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/apertium/__init__.py
--rw-r--r--   0        0        0     6069 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/apertium/apertium.py
--rw-r--r--   0        0        0      722 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/apertium/pairs.py
--rw-r--r--   0        0        0     5390 2022-12-15 10:03:37.305408 es_translator-1.4.2/es_translator/interpreters/apertium/repository.py
--rw-r--r--   0        0        0       24 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/argos/__init__.py
--rw-r--r--   0        0        0     2553 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/argos/argos.py
--rw-r--r--   0        0        0      912 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/logger.py
--rw-r--r--   0        0        0      267 2022-06-20 12:45:46.183755 es_translator-1.4.2/es_translator/symlink.py
--rw-r--r--   0        0        0      842 2023-05-12 13:31:48.466306 es_translator-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     4996 1970-01-01 00:00:00.000000 es_translator-1.4.2/setup.py
--rw-r--r--   0        0        0     4654 1970-01-01 00:00:00.000000 es_translator-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     3978 2023-05-16 11:15:56.684853 es_translator-1.5.0/README.md
+-rw-r--r--   0        0        0      136 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/__init__.py
+-rw-r--r--   0        0        0      490 2022-06-20 12:45:46.183755 es_translator-1.5.0/es_translator/alpha.py
+-rw-r--r--   0        0        0     4992 2023-05-16 11:12:42.123154 es_translator-1.5.0/es_translator/cli.py
+-rw-r--r--   0        0        0     1893 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/es.py
+-rw-r--r--   0        0        0     5882 2023-05-16 11:09:04.245390 es_translator-1.5.0/es_translator/es_translator.py
+-rw-r--r--   0        0        0       55 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/__init__.py
+-rw-r--r--   0        0        0     1690 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/abstract.py
+-rw-r--r--   0        0        0       30 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/apertium/__init__.py
+-rw-r--r--   0        0        0     6069 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/apertium/apertium.py
+-rw-r--r--   0        0        0      722 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/apertium/pairs.py
+-rw-r--r--   0        0        0     5390 2022-12-15 10:03:37.305408 es_translator-1.5.0/es_translator/interpreters/apertium/repository.py
+-rw-r--r--   0        0        0       24 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/argos/__init__.py
+-rw-r--r--   0        0        0     2553 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/interpreters/argos/argos.py
+-rw-r--r--   0        0        0      912 2022-07-26 11:37:09.729633 es_translator-1.5.0/es_translator/logger.py
+-rw-r--r--   0        0        0      267 2022-06-20 12:45:46.183755 es_translator-1.5.0/es_translator/symlink.py
+-rw-r--r--   0        0        0     2560 2023-05-16 11:06:33.928295 es_translator-1.5.0/es_translator/worker.py
+-rw-r--r--   0        0        0      842 2023-05-16 11:19:12.026637 es_translator-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5275 1970-01-01 00:00:00.000000 es_translator-1.5.0/setup.py
+-rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 es_translator-1.5.0/PKG-INFO
```

### Comparing `es_translator-1.4.2/LICENSE.txt` & `es_translator-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.2/README.md` & `es_translator-1.5.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,40 +4,45 @@
 
 A lazy yet bulletproof machine translation tool for Elastichsearch.
 
 ```
 Usage: es-translator [OPTIONS]
 
 Options:
-  --url TEXT                    Elastichsearch URL  [required]
-  --index TEXT                  Elastichsearch Index  [required]
-  --interpreter TEXT            Interpreter to use to perform the translation
-  --source-language TEXT        Source language to translate from  [required]
-  --target-language TEXT        Target language to translate to  [required]
-  --intermediary-language TEXT  An intermediary language to use when no
-                                translation is available between the source
-                                and the target. If none is provided this will
-                                be calculated automatically.
-  --source-field TEXT           Document field to translate
-  --target-field TEXT           Document field where the translations are
-                                stored
-  --query-string TEXT           Search query string to filter result
-  --data-dir PATH               Path to the directory where to language model
-                                will be downloaded
-  --scan-scroll TEXT            Scroll duration (set to higher value if you're
-                                processing a lot of documents)
-  --dry-run                     Don't save anything in Elasticsearch
-  --pool-size INTEGER           Number of parallel processes to start
-  --pool-timeout INTEGER        Timeout to add a translation
-  --syslog-address TEXT         Syslog address
-  --syslog-port INTEGER         Syslog port
-  --syslog-facility TEXT        Syslog facility
-  --stdout-loglevel TEXT        Change the default log level for stdout error
-                                handler
-  --help                        Show this message and exit.
+  -u, --url TEXT                  Elastichsearch URL
+  -i, --index TEXT                Elastichsearch Index  [required]
+  -r, --interpreter TEXT          Interpreter to use to perform the
+                                  translation
+  -s, --source-language TEXT      Source language to translate from
+                                  [required]
+  -t, --target-language TEXT      Target language to translate to  [required]
+  --intermediary-language TEXT    An intermediary language to use when no
+                                  translation is available between the source
+                                  and the target. If none is provided this
+                                  will be calculated automatically.
+  --source-field TEXT             Document field to translate
+  --target-field TEXT             Document field where the translations are
+                                  stored
+  -q, --query-string TEXT         Search query string to filter result
+  -d, --data-dir PATH             Path to the directory where to language
+                                  model will be downloaded
+  --scan-scroll TEXT              Scroll duration (set to higher value if
+                                  you're processing a lot of documents)
+  --dry-run                       Don't save anything in Elasticsearch
+  --pool-size INTEGER             Number of parallel processes to start
+  --pool-timeout INTEGER          Timeout to add a translation
+  --throttle INTEGER              Throttle between each translation (in ms)
+  --syslog-address TEXT           Syslog address
+  --syslog-port INTEGER           Syslog port
+  --syslog-facility TEXT          Syslog facility
+  --stdout-loglevel TEXT          Change the default log level for stdout
+                                  error handler
+  --progressbar / --no-progressbar
+                                  Display a progressbar
+  --help                          Show this message and exit.
 ```
 
 ## Installation (Ubuntu)
 
 Install Apertium:
 
 ```
```

### Comparing `es_translator-1.4.2/es_translator/cli.py` & `es_translator-1.5.0/es_translator/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         if value.upper() == interpreter.name.upper():
             return interpreter
     names = (interpreter.name for interpreter in interpreters)
     raise click.BadParameter('must be a valid interpreter name (%s)' % ', '.join(names))
 
 
 @click.command()
-@click.option('-u', '--url', help='Elastichsearch URL', default="http://localhost:9200", required=True)
+@click.option('-u', '--url', help='Elastichsearch URL', default="http://localhost:9200")
 @click.option('-i', '--index', help='Elastichsearch Index', required=True)
 @click.option('-r', '--interpreter', help='Interpreter to use to perform the translation', default='ARGOS', callback=validate_interpreter)
 @click.option('-s', '--source-language', help='Source language to translate from', required=True, default=None)
 @click.option('-t', '--target-language', help='Target language to translate to', required=True, default=None)
 @click.option('--intermediary-language', help='An intermediary language to use when no translation is available between the source and the target. If none is provided this will be calculated automatically.')
 @click.option('--source-field', help='Document field to translate', default="content")
 @click.option('--target-field', help='Document field where the translations are stored', default="content_translated")
@@ -50,15 +50,15 @@
 @click.option('--pool-timeout', help='Timeout to add a translation', default=60 * 30)
 @click.option('--throttle', help='Throttle between each translation (in ms)', default=0)
 @click.option('--syslog-address', help='Syslog address', default='localhost')
 @click.option('--syslog-port', help='Syslog port', default=514)
 @click.option('--syslog-facility', help='Syslog facility', default='local7')
 @click.option('--stdout-loglevel', help='Change the default log level for stdout error handler', default='ERROR',
               callback=validate_loglevel)
-@click.option('-p', '--progressbar/--no-progressbar', help='Display a progressbar', default=None,
+@click.option('--progressbar/--no-progressbar', help='Display a progressbar', default=None,
             callback=validate_progressbar)
 def translate(syslog_address, syslog_port, syslog_facility, **options):
     # Configure Syslog handler
     add_syslog_handler(syslog_address, syslog_port, syslog_facility)
     add_stdout_handler(options['stdout_loglevel'])
     # We pass all options to EsTranslator then we start the translation
     # from Elasticsearch. This will download required pairs if needed.
```

### Comparing `es_translator-1.4.2/es_translator/es.py` & `es_translator-1.5.0/es_translator/es.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.2/es_translator/es_translator.py` & `es_translator-1.5.0/es_translator/es_translator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,19 @@
 import sys
 from coloredlogs import StandardErrorHandler
 from contextlib import contextmanager
-from elasticsearch import Elasticsearch
+from elasticsearch import Elasticsearch, ElasticsearchException
 from elasticsearch_dsl import Search
-from multiprocessing import Pool, JoinableQueue
+from multiprocessing import Pool, JoinableQueue, Manager
 from queue import Full
 from os import path
 from rich.progress import Progress
-from time import sleep
 # Module from the same package
-from es_translator.es import TranslatedHit
 from es_translator.logger import logger
-
-
-def translation_worker(queue):
-    while True:
-        try:
-            es_translator, hit, index, throttle = queue.get(True)
-            logger.info('Translating doc %s (%s)' % (index, hit.meta.id))
-            translated_hit = TranslatedHit(hit, es_translator.source_field, es_translator.target_field)
-            translated_hit.add_translation(es_translator.interpreter)
-            logger.info('Translated doc %s (%s)' % (index, hit.meta.id))
-            # Skip on dry run
-            if not es_translator.dry_run:
-                # Create a new  client to
-                client = Elasticsearch(es_translator.url)
-                translated_hit.save(client)
-                logger.info('Saved translation for doc %s (%s)' % (index, hit.meta.id))
-            queue.task_done()
-            sleep(throttle / 1000)
-        except Exception as error:
-            logger.warning('Unable to translate doc %s (%s)' % (index, hit.meta.id))
-            logger.warning(error)
-            queue.task_done()
-
+from es_translator.worker import translation_worker, FatalTranslationException
 
 class EsTranslator:
     def __init__(self, options):
         self.url = options['url']
         self.index = options['index']
         self.source_language = options['source_language']
         self.target_language = options['target_language']
@@ -54,40 +30,78 @@
         self.progressbar = options['progressbar']
         # The "interpreter" option is a class
         self.Interpreter = options['interpreter']
 
     @property
     def no_progressbar(self):
         return not self.progressbar
-
+    
     def start(self):
+        # Instantiate the interpreter
+        self.instantiate_interpreter()
+        # Count the total number of documents
+        total = self.search().count()
+        desc = 'Translating %s document(s)' % total
+        # Start the translation process
+        with self.print_done(desc):
+            # Configure the search object
+            search = self.configure_search()
+            # Create a queue to translate documents in parallel
+            translation_queue = self.create_translation_queue()
+            # Create a shared variable to track fatal errors
+            with self.with_shared_fatal_error() as shared_fatal_error: 
+                # Translate the documents
+                self.translate_documents(search, translation_queue, shared_fatal_error, total)
+
+    def instantiate_interpreter(self):
         with self.print_done('Instantiating %s interpreter' % self.Interpreter.name):
             self.interpreter = self.init_interpreter()
+        return self.interpreter
 
-        total = self.search().count()
-        desc = 'Translating %s document(s)' % total
+    def configure_search(self):
+        # Configure the search object
+        search = self.search()
+        search = search.source([self.source_field, self.target_field, '_routing'])
+        search = search.params(scroll=self.scan_scroll, size=self.pool_size)
+        return search
 
-        with self.print_done(desc):
-            # Add missing field and change the scroll duration
-            search = self.search()
-            search = search.source([self.source_field, self.target_field, '_routing'])
-            search = search.params(scroll=self.scan_scroll)
-            # Create a queue that is able to translate documents in parallel
-            translation_queue = JoinableQueue(self.pool_size)
-            # We create a pool
-            with Pool(self.pool_size, translation_worker, (translation_queue,)):
-                with Progress(disable=self.no_progressbar, transient=True) as progress:   
-                    documents = search.scan()         
-                    task = progress.add_task(desc, total=total)
-                    for index, hit in enumerate(documents):
-                        translation_queue.put((self, hit, index, self.throttle), True, self.pool_timeout)
-                        progress.advance(task)
-                    translation_queue.join()
-                    
+    def create_translation_queue(self):
+        # Create a queue that is able to translate documents in parallel
+        return JoinableQueue(self.pool_size)
 
+    @contextmanager
+    def with_shared_fatal_error(self):
+        # Use Manager to create a shared variable (shared_fatal_error)
+        with Manager() as manager:
+            # Shared variable between threads, initialized as None
+            yield manager.Value('b', None)
+
+    def translate_documents(self, search, translation_queue, shared_fatal_error, total):
+        # Start a pool of worker processes
+        with Pool(self.pool_size, translation_worker, (translation_queue, shared_fatal_error)):
+            # Create a progress bar
+            with Progress(disable=self.no_progressbar, transient=True) as progress:
+                documents = search.scan()
+                task = progress.add_task('Translating %s document(s)' % total, total=total)
+                for index, hit in enumerate(documents):
+                    self.process_document(translation_queue, hit, index, progress, task, shared_fatal_error)
+                translation_queue.join()
+
+    def process_document(self, translation_queue, hit, index, progress, task, shared_fatal_error):
+        # Add the document to the translation queue
+        translation_queue.put((self, hit, index), True, self.pool_timeout)
+        
+        # Update the progress bar with the current task
+        progress.advance(task)
+        
+        # Check if a fatal error occurred
+        if shared_fatal_error.value:
+            # Raise an exception to interrupt the loop
+            raise FatalTranslationException(shared_fatal_error.value)
+    
     def search(self):
         es_client = Elasticsearch(self.url)
         search = Search(index=self.index, using=es_client)
         # Add query_string to the search
         if self.query_string:
             search = search.query("query_string", query=self.query_string)
         return search
@@ -105,26 +119,22 @@
         try:
             handler = next(h for h in logger.handlers if isinstance(h, StandardErrorHandler))
             return getattr(handler, 'level', 0)
         except StopIteration:
             return 0
 
     @contextmanager
-    def print_done(self, str, quiet = False):
+    def print_done(self, str):
         logger.info(str)
         # Avoid conflicting with a high log level
         if self.stdout_loglevel > 20:
             str = '\r%s...' % str
             self.print_flush(str)
             try:
                 yield
                 print('{0} \033[92mdone\033[0m'.format(str))
-            except Full:
-                logger.error('Timeout reached (%ss).' % self.pool_timeout)
-                print('{0} \033[91merror\033[0m'.format(str))
-            except Exception as error:
+            except (FatalTranslationException, ElasticsearchException, Full) as error:
                 logger.error(error, exc_info=True)
                 print('{0} \033[91merror\033[0m'.format(str))
-                if not quiet: raise error
                 sys.exit(1)
         else:
             yield
```

### Comparing `es_translator-1.4.2/es_translator/interpreters/abstract.py` & `es_translator-1.5.0/es_translator/interpreters/abstract.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.2/es_translator/interpreters/apertium/apertium.py` & `es_translator-1.5.0/es_translator/interpreters/apertium/apertium.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.2/es_translator/interpreters/apertium/pairs.py` & `es_translator-1.5.0/es_translator/interpreters/apertium/pairs.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.2/es_translator/interpreters/apertium/repository.py` & `es_translator-1.5.0/es_translator/interpreters/apertium/repository.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.2/es_translator/interpreters/argos/argos.py` & `es_translator-1.5.0/es_translator/interpreters/argos/argos.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.2/es_translator/logger.py` & `es_translator-1.5.0/es_translator/logger.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.2/pyproject.toml` & `es_translator-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "es-translator"
-version = "1.4.2"
+version = "1.5.0"
 description = "A lazy yet bulletproof machine translation tool for Elastichsearch."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 license = "GNU AFFERO GENERAL PUBLIC LICENSE"
 packages = [{include = "es_translator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `es_translator-1.4.2/setup.py` & `es_translator-1.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 entry_points = \
 {'console_scripts': ['es-translator = es_translator.cli:translate',
                      'es-translator-pairs = es_translator.cli:pairs']}
 
 setup_kwargs = {
     'name': 'es-translator',
-    'version': '1.4.2',
+    'version': '1.5.0',
     'description': 'A lazy yet bulletproof machine translation tool for Elastichsearch.',
-    'long_description': '# ES Translator\n\n[![CircleCI](https://circleci.com/gh/ICIJ/es-translator.svg?style=svg)](https://circleci.com/gh/ICIJ/es-translator)\n\nA lazy yet bulletproof machine translation tool for Elastichsearch.\n\n```\nUsage: es-translator [OPTIONS]\n\nOptions:\n  --url TEXT                    Elastichsearch URL  [required]\n  --index TEXT                  Elastichsearch Index  [required]\n  --interpreter TEXT            Interpreter to use to perform the translation\n  --source-language TEXT        Source language to translate from  [required]\n  --target-language TEXT        Target language to translate to  [required]\n  --intermediary-language TEXT  An intermediary language to use when no\n                                translation is available between the source\n                                and the target. If none is provided this will\n                                be calculated automatically.\n  --source-field TEXT           Document field to translate\n  --target-field TEXT           Document field where the translations are\n                                stored\n  --query-string TEXT           Search query string to filter result\n  --data-dir PATH               Path to the directory where to language model\n                                will be downloaded\n  --scan-scroll TEXT            Scroll duration (set to higher value if you\'re\n                                processing a lot of documents)\n  --dry-run                     Don\'t save anything in Elasticsearch\n  --pool-size INTEGER           Number of parallel processes to start\n  --pool-timeout INTEGER        Timeout to add a translation\n  --syslog-address TEXT         Syslog address\n  --syslog-port INTEGER         Syslog port\n  --syslog-facility TEXT        Syslog facility\n  --stdout-loglevel TEXT        Change the default log level for stdout error\n                                handler\n  --help                        Show this message and exit.\n```\n\n## Installation (Ubuntu)\n\nInstall Apertium:\n\n```\nwget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash\nsudo apt install apertium-all-dev\n```\n\nCreate a Virtualenv and install Pip packages with Poetry:\n\n```\nmake install\n```\n\nOn Ubuntu 22.04 some additional packages might be needed if you use the version from Ubuntu\'s repository:\n\n```\nsudo apt install cg3 apertium-get apertium-lex-tools\n```\n\n\n## Installation (Docker)\n\nNothing to do as long as you have Docker on your system:\n\n```\ndocker run -it icij/es-translator poetry run es-translator --help\n```\n\n## Examples\n\nTranslates documents from French to Spanish on a local Elasticsearch. The translated field is `content` (the default).\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es\n```\n\nTranslates documents from French to English on a local Elasticsearch using Apertium:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language en --interpreter apertium\n```\n\nTo translate the `title` field we could do:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es --source-field title\n```\n\nTranslates documents from English to Spanish on a local Elasticsearch using 4 threads:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language en --target-language es --pool-size 4\n```\n\nTranslates documents from Portuguese to English, using an intermediary language (Apertium doesn\'t offer this translation pair):\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language pt --intermediary-language es --target-language en\n```\n',
+    'long_description': '# ES Translator\n\n[![CircleCI](https://circleci.com/gh/ICIJ/es-translator.svg?style=svg)](https://circleci.com/gh/ICIJ/es-translator)\n\nA lazy yet bulletproof machine translation tool for Elastichsearch.\n\n```\nUsage: es-translator [OPTIONS]\n\nOptions:\n  -u, --url TEXT                  Elastichsearch URL\n  -i, --index TEXT                Elastichsearch Index  [required]\n  -r, --interpreter TEXT          Interpreter to use to perform the\n                                  translation\n  -s, --source-language TEXT      Source language to translate from\n                                  [required]\n  -t, --target-language TEXT      Target language to translate to  [required]\n  --intermediary-language TEXT    An intermediary language to use when no\n                                  translation is available between the source\n                                  and the target. If none is provided this\n                                  will be calculated automatically.\n  --source-field TEXT             Document field to translate\n  --target-field TEXT             Document field where the translations are\n                                  stored\n  -q, --query-string TEXT         Search query string to filter result\n  -d, --data-dir PATH             Path to the directory where to language\n                                  model will be downloaded\n  --scan-scroll TEXT              Scroll duration (set to higher value if\n                                  you\'re processing a lot of documents)\n  --dry-run                       Don\'t save anything in Elasticsearch\n  --pool-size INTEGER             Number of parallel processes to start\n  --pool-timeout INTEGER          Timeout to add a translation\n  --throttle INTEGER              Throttle between each translation (in ms)\n  --syslog-address TEXT           Syslog address\n  --syslog-port INTEGER           Syslog port\n  --syslog-facility TEXT          Syslog facility\n  --stdout-loglevel TEXT          Change the default log level for stdout\n                                  error handler\n  --progressbar / --no-progressbar\n                                  Display a progressbar\n  --help                          Show this message and exit.\n```\n\n## Installation (Ubuntu)\n\nInstall Apertium:\n\n```\nwget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash\nsudo apt install apertium-all-dev\n```\n\nCreate a Virtualenv and install Pip packages with Poetry:\n\n```\nmake install\n```\n\nOn Ubuntu 22.04 some additional packages might be needed if you use the version from Ubuntu\'s repository:\n\n```\nsudo apt install cg3 apertium-get apertium-lex-tools\n```\n\n\n## Installation (Docker)\n\nNothing to do as long as you have Docker on your system:\n\n```\ndocker run -it icij/es-translator poetry run es-translator --help\n```\n\n## Examples\n\nTranslates documents from French to Spanish on a local Elasticsearch. The translated field is `content` (the default).\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es\n```\n\nTranslates documents from French to English on a local Elasticsearch using Apertium:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language en --interpreter apertium\n```\n\nTo translate the `title` field we could do:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es --source-field title\n```\n\nTranslates documents from English to Spanish on a local Elasticsearch using 4 threads:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language en --target-language es --pool-size 4\n```\n\nTranslates documents from Portuguese to English, using an intermediary language (Apertium doesn\'t offer this translation pair):\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language pt --intermediary-language es --target-language en\n```\n',
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `es_translator-1.4.2/PKG-INFO` & `es_translator-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: es-translator
-Version: 1.4.2
+Version: 1.5.0
 Summary: A lazy yet bulletproof machine translation tool for Elastichsearch.
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -30,40 +30,45 @@
 
 A lazy yet bulletproof machine translation tool for Elastichsearch.
 
 ```
 Usage: es-translator [OPTIONS]
 
 Options:
-  --url TEXT                    Elastichsearch URL  [required]
-  --index TEXT                  Elastichsearch Index  [required]
-  --interpreter TEXT            Interpreter to use to perform the translation
-  --source-language TEXT        Source language to translate from  [required]
-  --target-language TEXT        Target language to translate to  [required]
-  --intermediary-language TEXT  An intermediary language to use when no
-                                translation is available between the source
-                                and the target. If none is provided this will
-                                be calculated automatically.
-  --source-field TEXT           Document field to translate
-  --target-field TEXT           Document field where the translations are
-                                stored
-  --query-string TEXT           Search query string to filter result
-  --data-dir PATH               Path to the directory where to language model
-                                will be downloaded
-  --scan-scroll TEXT            Scroll duration (set to higher value if you're
-                                processing a lot of documents)
-  --dry-run                     Don't save anything in Elasticsearch
-  --pool-size INTEGER           Number of parallel processes to start
-  --pool-timeout INTEGER        Timeout to add a translation
-  --syslog-address TEXT         Syslog address
-  --syslog-port INTEGER         Syslog port
-  --syslog-facility TEXT        Syslog facility
-  --stdout-loglevel TEXT        Change the default log level for stdout error
-                                handler
-  --help                        Show this message and exit.
+  -u, --url TEXT                  Elastichsearch URL
+  -i, --index TEXT                Elastichsearch Index  [required]
+  -r, --interpreter TEXT          Interpreter to use to perform the
+                                  translation
+  -s, --source-language TEXT      Source language to translate from
+                                  [required]
+  -t, --target-language TEXT      Target language to translate to  [required]
+  --intermediary-language TEXT    An intermediary language to use when no
+                                  translation is available between the source
+                                  and the target. If none is provided this
+                                  will be calculated automatically.
+  --source-field TEXT             Document field to translate
+  --target-field TEXT             Document field where the translations are
+                                  stored
+  -q, --query-string TEXT         Search query string to filter result
+  -d, --data-dir PATH             Path to the directory where to language
+                                  model will be downloaded
+  --scan-scroll TEXT              Scroll duration (set to higher value if
+                                  you're processing a lot of documents)
+  --dry-run                       Don't save anything in Elasticsearch
+  --pool-size INTEGER             Number of parallel processes to start
+  --pool-timeout INTEGER          Timeout to add a translation
+  --throttle INTEGER              Throttle between each translation (in ms)
+  --syslog-address TEXT           Syslog address
+  --syslog-port INTEGER           Syslog port
+  --syslog-facility TEXT          Syslog facility
+  --stdout-loglevel TEXT          Change the default log level for stdout
+                                  error handler
+  --progressbar / --no-progressbar
+                                  Display a progressbar
+  --help                          Show this message and exit.
 ```
 
 ## Installation (Ubuntu)
 
 Install Apertium:
 
 ```
```

