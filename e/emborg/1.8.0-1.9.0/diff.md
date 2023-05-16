# Comparing `tmp/emborg-1.8.0.tar.gz` & `tmp/emborg-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/emborg-1.8.0.tar", last modified: Sat Oct 12 17:13:11 2019, max compression
+gzip compressed data, was "dist/emborg-1.9.0.tar", last modified: Fri Nov  8 22:24:33 2019, max compression
```

## Comparing `emborg-1.8.0.tar` & `emborg-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2019-10-12 17:13:11.000000 emborg-1.8.0/
--rw-r--r--   0 ken       (1000) officers   (501)     3110 2019-10-12 17:13:11.000000 emborg-1.8.0/PKG-INFO
--rw-r--r--   0 ken       (1000) officers   (501)     1956 2019-10-12 17:07:39.000000 emborg-1.8.0/README.rst
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2019-10-12 17:13:11.000000 emborg-1.8.0/emborg/
--rw-r--r--   0 ken       (1000) officers   (501)       92 2019-10-12 17:07:39.000000 emborg-1.8.0/emborg/__init__.py
--rw-r--r--   0 ken       (1000) officers   (501)     2226 2018-12-06 22:18:56.000000 emborg-1.8.0/emborg/collection.py
--rw-r--r--   0 ken       (1000) officers   (501)    38533 2019-10-11 14:35:02.000000 emborg-1.8.0/emborg/command.py
--rw-r--r--   0 ken       (1000) officers   (501)     6687 2019-04-15 02:36:36.000000 emborg-1.8.0/emborg/help.py
--rw-r--r--   0 ken       (1000) officers   (501)     3715 2019-09-30 05:32:19.000000 emborg-1.8.0/emborg/main.py
--rw-r--r--   0 ken       (1000) officers   (501)     5929 2019-04-16 17:53:02.000000 emborg-1.8.0/emborg/overdue.py
--rw-r--r--   0 ken       (1000) officers   (501)     9374 2019-10-07 06:48:39.000000 emborg-1.8.0/emborg/preferences.py
--rw-r--r--   0 ken       (1000) officers   (501)     3947 2019-04-15 02:36:56.000000 emborg-1.8.0/emborg/python.py
--rw-r--r--   0 ken       (1000) officers   (501)    19488 2019-10-06 06:43:12.000000 emborg-1.8.0/emborg/settings.py
--rw-r--r--   0 ken       (1000) officers   (501)     2690 2019-09-23 00:23:33.000000 emborg-1.8.0/emborg/utilities.py
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2019-10-12 17:13:11.000000 emborg-1.8.0/emborg.egg-info/
--rw-r--r--   0 ken       (1000) officers   (501)     3110 2019-10-12 17:13:11.000000 emborg-1.8.0/emborg.egg-info/PKG-INFO
--rw-r--r--   0 ken       (1000) officers   (501)      385 2019-10-12 17:13:11.000000 emborg-1.8.0/emborg.egg-info/SOURCES.txt
--rw-r--r--   0 ken       (1000) officers   (501)        1 2019-10-12 17:13:11.000000 emborg-1.8.0/emborg.egg-info/dependency_links.txt
--rw-r--r--   0 ken       (1000) officers   (501)       82 2019-10-12 17:13:11.000000 emborg-1.8.0/emborg.egg-info/entry_points.txt
--rw-r--r--   0 ken       (1000) officers   (501)       45 2019-10-12 17:13:11.000000 emborg-1.8.0/emborg.egg-info/requires.txt
--rw-r--r--   0 ken       (1000) officers   (501)        7 2019-10-12 17:13:11.000000 emborg-1.8.0/emborg.egg-info/top_level.txt
--rw-r--r--   0 ken       (1000) officers   (501)       38 2019-10-12 17:13:11.000000 emborg-1.8.0/setup.cfg
--rw-r--r--   0 ken       (1000) officers   (501)     1194 2019-10-12 17:07:39.000000 emborg-1.8.0/setup.py
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2019-11-08 22:24:33.000000 emborg-1.9.0/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     3110 2019-11-08 22:24:33.000000 emborg-1.9.0/PKG-INFO
+-rw-rw-r--   0 ken       (1000) ken       (1000)     1956 2019-11-08 19:24:03.000000 emborg-1.9.0/README.rst
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2019-11-08 22:24:33.000000 emborg-1.9.0/emborg/
+-rw-rw-r--   0 ken       (1000) ken       (1000)       92 2019-11-08 19:24:03.000000 emborg-1.9.0/emborg/__init__.py
+-rw-rw-r--   0 ken       (1000) ken       (1000)     2226 2019-11-03 00:51:41.000000 emborg-1.9.0/emborg/collection.py
+-rw-rw-r--   0 ken       (1000) ken       (1000)    39804 2019-11-07 04:59:41.000000 emborg-1.9.0/emborg/command.py
+-rw-rw-r--   0 ken       (1000) ken       (1000)     6692 2019-11-03 00:52:22.000000 emborg-1.9.0/emborg/help.py
+-rw-rw-r--   0 ken       (1000) ken       (1000)     3715 2019-11-03 00:51:41.000000 emborg-1.9.0/emborg/main.py
+-rw-rw-r--   0 ken       (1000) ken       (1000)     5929 2019-11-03 00:51:41.000000 emborg-1.9.0/emborg/overdue.py
+-rw-rw-r--   0 ken       (1000) ken       (1000)     9356 2019-11-03 00:52:24.000000 emborg-1.9.0/emborg/preferences.py
+-rw-rw-r--   0 ken       (1000) ken       (1000)     3952 2019-11-03 00:52:28.000000 emborg-1.9.0/emborg/python.py
+-rw-rw-r--   0 ken       (1000) ken       (1000)    19624 2019-11-03 00:52:33.000000 emborg-1.9.0/emborg/settings.py
+-rw-rw-r--   0 ken       (1000) ken       (1000)     2690 2019-11-03 00:51:41.000000 emborg-1.9.0/emborg/utilities.py
+drwxrwxr-x   0 ken       (1000) ken       (1000)        0 2019-11-08 22:24:33.000000 emborg-1.9.0/emborg.egg-info/
+-rw-rw-r--   0 ken       (1000) ken       (1000)     3110 2019-11-08 22:24:33.000000 emborg-1.9.0/emborg.egg-info/PKG-INFO
+-rw-rw-r--   0 ken       (1000) ken       (1000)      385 2019-11-08 22:24:33.000000 emborg-1.9.0/emborg.egg-info/SOURCES.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)        1 2019-11-08 22:24:33.000000 emborg-1.9.0/emborg.egg-info/dependency_links.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)       82 2019-11-08 22:24:33.000000 emborg-1.9.0/emborg.egg-info/entry_points.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)       45 2019-11-08 22:24:33.000000 emborg-1.9.0/emborg.egg-info/requires.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)        7 2019-11-08 22:24:33.000000 emborg-1.9.0/emborg.egg-info/top_level.txt
+-rw-rw-r--   0 ken       (1000) ken       (1000)       38 2019-11-08 22:24:33.000000 emborg-1.9.0/setup.cfg
+-rw-rw-r--   0 ken       (1000) ken       (1000)     1194 2019-11-08 19:24:03.000000 emborg-1.9.0/setup.py
```

### Comparing `emborg-1.8.0/PKG-INFO` & `emborg-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: emborg
-Version: 1.8.0
+Version: 1.9.0
 Summary: Borg front end.
 Home-page: https://emborg.readthedocs.io
 Author: Ken Kundert
 Author-email: emborg@nurdletech.com
 License: GPLv3+
 Download-URL: https://github.com/kenkundert/emborg/tarball/master
 Description: Emborg — Front-End to Borg Backup
@@ -13,16 +13,16 @@
         .. image:: https://img.shields.io/pypi/v/emborg.svg
             :target: https://pypi.python.org/pypi/emborg
         
         .. image:: https://img.shields.io/pypi/pyversions/emborg.svg
             :target: https://pypi.python.org/pypi/emborg/
         
         :Author: Ken Kundert
-        :Version: 1.8.0
-        :Released: 2019-10-12
+        :Version: 1.9.0
+        :Released: 2019-11-08
         
         *Emborg* is a simple command line utility to orchestrate backups. It is built as 
         a front-end to Borg, a powerful and fast deduplicating backup program.  With 
         *Emborg*, you specify all the details about your backups once in advance, and 
         then use a very simple command line interface for your day-to-day activities.  
         The details are contained in ~/.config/emborg.  That directory contains a file 
         (settings) that contains shared settings, and then another file for each backup
```

### Comparing `emborg-1.8.0/README.rst` & `emborg-1.9.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 .. image:: https://img.shields.io/pypi/v/emborg.svg
     :target: https://pypi.python.org/pypi/emborg
 
 .. image:: https://img.shields.io/pypi/pyversions/emborg.svg
     :target: https://pypi.python.org/pypi/emborg/
 
 :Author: Ken Kundert
-:Version: 1.8.0
-:Released: 2019-10-12
+:Version: 1.9.0
+:Released: 2019-11-08
 
 *Emborg* is a simple command line utility to orchestrate backups. It is built as 
 a front-end to Borg, a powerful and fast deduplicating backup program.  With 
 *Emborg*, you specify all the details about your backups once in advance, and 
 then use a very simple command line interface for your day-to-day activities.  
 The details are contained in ~/.config/emborg.  That directory contains a file 
 (settings) that contains shared settings, and then another file for each backup
```

### Comparing `emborg-1.8.0/emborg/collection.py` & `emborg-1.9.0/emborg/collection.py`

 * *Files identical despite different names*

### Comparing `emborg-1.8.0/emborg/command.py` & `emborg-1.9.0/emborg/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,84 @@
         )
         out = borg.stdout
         if out:
             output(out.rstrip())
         rm(settings.lockfile)
 
 
+# CheckCommand command {{{1
+class CheckCommand(Command):
+    NAMES = 'check'.split()
+    DESCRIPTION = 'checks the repository and its archives'
+    USAGE = dedent("""
+        Usage:
+            emborg check [options] [<archive>]
+
+        Options:
+            -A, --all                           mount all available archives
+            -e, --include-external              check all archives in repository, not just
+                                                those associated with this configuration
+            -v, --verify-data                   perform a full integrity verification (slow)
+
+        The most recently created archive is checked if one is not specified
+        unless --all is given, in which case all archives are checked.
+    """).strip()
+    REQUIRES_EXCLUSIVITY = True
+    COMPOSITE_CONFIGS = True
+
+    @classmethod
+    def run(cls, command, args, settings, options):
+        # read command line
+        cmdline = docopt(cls.USAGE, argv=[command] + args)
+        archive = cmdline['<archive>']
+        check_all = cmdline['--all']
+        verify = ['--verify-data'] if cmdline['--verify-data'] else []
+        include_external_archives = cmdline['--include-external']
+
+        # identify archive or archives to check
+        if check_all:
+            archive = None
+        elif not archive:
+            archive = get_name_of_latest_archive(settings)
+
+        # run borg
+        borg = settings.run_borg(
+            cmd = 'check',
+            args = verify + [settings.destination(archive)],
+            emborg_opts = options,
+            strip_prefix = include_external_archives,
+        )
+        out = borg.stdout
+        if out:
+            output(out.rstrip())
+
+
+# ConfigsCommand command {{{1
+class ConfigsCommand(Command):
+    NAMES = 'configs'.split()
+    DESCRIPTION = 'list available backup configurations'
+    USAGE = dedent("""
+        Usage:
+            emborg configs
+    """).strip()
+    REQUIRES_EXCLUSIVITY = False
+    COMPOSITE_CONFIGS = None
+
+    @classmethod
+    def run(cls, command, args, settings, options):
+        # read command line
+        docopt(cls.USAGE, argv=[command] + args)
+
+        configurations = Collection(settings.configurations)
+        if configurations:
+            output('Available Configurations:', *configurations, sep='\n    ')
+        else:
+            output('No configurations available.')
+
+
 # CreateCommand command {{{1
 class CreateCommand(Command):
     NAMES = 'create backup'.split()
     DESCRIPTION = 'create an archive of the current files'
     USAGE = dedent("""
         Usage:
             emborg create [options]
@@ -240,15 +310,18 @@
 
         # check for required settings
         src_dirs = render_paths(settings.src_dirs)
         if not src_dirs:
             raise Error('src_dirs: setting has no value.')
 
         # check the dependencies are available
-        for each in settings.values('must_exist'):
+        must_exist = settings.value('must_exist')
+        if is_str(must_exist):
+            must_exist = [must_exist]
+        for each in must_exist:
             path = to_path(each)
             if not path.exists():
                 raise Error(
                     'does not exist, perform setup and restart.',
                     culprit=each
                 )
 
@@ -299,87 +372,43 @@
 
         # prune the archives if requested
         try:
             # check the archives if requested
             activity = 'checking'
             if settings.check_after_create:
                 narrate('checking archive')
+                if settings.check_after_create == 'latest':
+                    args = []
+                elif settings.check_after_create in [True, 'all']:
+                    args = ['--all']
+                elif settings.check_after_create == 'all in repository':
+                    args = ['--all', '--include-external']
+                else:
+                    warn(
+                        'unknown value: {}, checking latest.'.format(
+                            settings.check_after_create
+                        ),
+                        cuplrit='check_after_create'
+                    )
+                    args = []
                 check = CheckCommand()
-                check.run('check', [], settings, options)
+                check.run('check', args, settings, options)
 
             activity = 'pruning'
             if settings.prune_after_create:
                 narrate('pruning archives')
                 prune = PruneCommand()
                 prune.run('prune', [], settings, options)
         except Error as e:
             e.reraise(codicil=(
                 f'This error occurred while {activity} the archives.',
                 'No error was reported while creating the archive.'
             ))
 
 
-# CheckCommand command {{{1
-class CheckCommand(Command):
-    NAMES = 'check'.split()
-    DESCRIPTION = 'checks the repository and its archives'
-    USAGE = dedent("""
-        Usage:
-            emborg check [options]
-
-        Options:
-            -e, --include-external   check all archives in repository, not just
-                                     those associated with this configuration
-            -v, --verify-data        perform a full integrity verification (slow)
-    """).strip()
-    REQUIRES_EXCLUSIVITY = True
-    COMPOSITE_CONFIGS = True
-
-    @classmethod
-    def run(cls, command, args, settings, options):
-        # read command line
-        cmdline = docopt(cls.USAGE, argv=[command] + args)
-        verify = ['--verify-data'] if cmdline['--verify-data'] else []
-        include_external_archives = cmdline['--include-external']
-
-        # run borg
-        borg = settings.run_borg(
-            cmd = 'check',
-            args = verify + [settings.destination()],
-            emborg_opts = options,
-            strip_prefix = include_external_archives,
-        )
-        out = borg.stdout
-        if out:
-            output(out.rstrip())
-
-
-# ConfigsCommand command {{{1
-class ConfigsCommand(Command):
-    NAMES = 'configs'.split()
-    DESCRIPTION = 'list available backup configurations'
-    USAGE = dedent("""
-        Usage:
-            emborg configs
-    """).strip()
-    REQUIRES_EXCLUSIVITY = False
-    COMPOSITE_CONFIGS = None
-
-    @classmethod
-    def run(cls, command, args, settings, options):
-        # read command line
-        docopt(cls.USAGE, argv=[command] + args)
-
-        configurations = Collection(settings.configurations)
-        if configurations:
-            output('Available Configurations:', *configurations, sep='\n    ')
-        else:
-            output('No configurations available.')
-
-
 # DeleteCommand command {{{1
 class DeleteCommand(Command):
     NAMES = 'delete'.split()
     DESCRIPTION = 'delete an archive currently contained in the repository'
     USAGE = dedent("""
         Usage:
             emborg [options] delete [<archive>]
```

### Comparing `emborg-1.8.0/emborg/help.py` & `emborg-1.9.0/emborg/help.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Help
 # Output a help topic.
 
 # License {{{1
-# Copyright (C) 2018 Kenneth S. Kundert
+# Copyright (C) 2018-2019 Kenneth S. Kundert
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `emborg-1.8.0/emborg/main.py` & `emborg-1.9.0/emborg/main.py`

 * *Files identical despite different names*

### Comparing `emborg-1.8.0/emborg/overdue.py` & `emborg-1.9.0/emborg/overdue.py`

 * *Files identical despite different names*

### Comparing `emborg-1.8.0/emborg/preferences.py` & `emborg-1.9.0/emborg/preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Avendesora Password Generator Settings
+# Emborg Settings
 #
-# Copyright (C) 2018 Kenneth S. Kundert
+# Copyright (C) 2018-2019 Kenneth S. Kundert
 
 # License {{{1
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
```

### Comparing `emborg-1.8.0/emborg/python.py` & `emborg-1.9.0/emborg/python.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # Read and Write Python files
 #
 # Package for reading and writing Python files.
 
 # License {{{1
-# Copyright (C) 2018 Kenneth S. Kundert
+# Copyright (C) 2018-2019 Kenneth S. Kundert
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
 #
 # This program is distributed in the hope that it will be useful, but WITHOUT
```

### Comparing `emborg-1.8.0/emborg/settings.py` & `emborg-1.9.0/emborg/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Settings
 
 # License {{{1
-# Copyright (C) 2018 Kenneth S. Kundert
+# Copyright (C) 2018-2019 Kenneth S. Kundert
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # This program is distributed in the hope that it will be useful,
@@ -37,16 +37,16 @@
     PROGRAM_NAME,
     SETTINGS_FILE,
 )
 from .python import PythonFile
 from .utilities import gethostname, getusername, render_paths
 from shlib import getmod, mv, rm, Run, to_path, render_command, to_path
 from inform import (
-    Error, codicil, conjoin, display, done, full_stop, get_informer, indent,
-    is_str, narrate, output, render, warn,
+    Color, Error, codicil, conjoin, display, done, full_stop, get_informer, 
+    indent, is_str, narrate, output, render, warn,
 )
 from textwrap import dedent
 import arrow
 import os
 
 
 # Utilities {{{1
@@ -260,30 +260,30 @@
             return to_path(parent_dir, self.resolve(value))
         return to_path(self.resolve(value))
 
     # handle errors {{{2
     def fail(self, *msg, comment=''):
         msg = full_stop(' '.join(str(m) for m in msg))
         try:
-            if self.notify:
+            if self.notify and not Color.isTTY():
                 Run(
                     ['mail', '-s', f'{PROGRAM_NAME} on {hostname}: {msg}'] + self.notify.split(),
                     stdin=dedent(f'''
                         {msg}
                         {comment}
                         config = {self.config_name}
                         source = {username}@{hostname}:{', '.join(str(d) for d in self.src_dirs)}
                         destination = {self.repository}
                     ''').lstrip(),
                     modes='soeW'
                 )
         except Error:
             pass
         try:
-            if self.notifier:
+            if self.notifier and not Color.isTTY():
                 Run(
                     self.notifier.format(
                         msg=msg, hostname=hostname,
                         user_name=username, prog_name=PROGRAM_NAME,
                     ),
                     modes='soeW'
                 )
@@ -320,18 +320,21 @@
                 args.append('--list')
                 if 'trial-run' not in options:
                     args.append('--stats')
             for path in render_paths(self.values('excludes')):
                 args.extend(['--exclude', path])
             exclude_from = self.value('exclude_from')
             if exclude_from:
-                path = to_path(self.config_dir, exclude_from)
-                if not path.exists():
-                    raise Error('--exclude-from file does not exist.', culprit=path)
-                args.extend(['--exclude-from', str(path)])
+                if is_str(exclude_from):
+                    exclude_from = [exclude_from]
+                for each in exclude_from:
+                    path = to_path(self.config_dir, each)
+                    if not path.exists():
+                        raise Error('--exclude-from file does not exist.', culprit=path)
+                    args.extend(['--exclude-from', str(path)])
 
         if cmd == 'extract':
             if 'verbose' in options:
                 args.append('--list')
 
         if cmd == 'init':
             if self.passphrase or self.avendesora_account:
@@ -487,17 +490,16 @@
     # enter {{{2
     def __enter__(self):
         # resolve src directories
         self.src_dirs = [self.resolve_path(d) for d in self.src_dirs]
         if not self.src_dirs:
             raise Error('no source directories given.')
 
-        # resolve repository and archive
+        # resolve repository
         self.repository = self.resolve_path(self.repository)
-        self.archive = self.resolve(self.archive)
 
         # resolve other files and directories
         data_dir = self.resolve_path(DATA_DIR)
         self.data_dir = data_dir
 
         if not data_dir.exists():
             # data dir does not exist, create it
```

### Comparing `emborg-1.8.0/emborg/utilities.py` & `emborg-1.9.0/emborg/utilities.py`

 * *Files identical despite different names*

### Comparing `emborg-1.8.0/emborg.egg-info/PKG-INFO` & `emborg-1.9.0/emborg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: emborg
-Version: 1.8.0
+Version: 1.9.0
 Summary: Borg front end.
 Home-page: https://emborg.readthedocs.io
 Author: Ken Kundert
 Author-email: emborg@nurdletech.com
 License: GPLv3+
 Download-URL: https://github.com/kenkundert/emborg/tarball/master
 Description: Emborg — Front-End to Borg Backup
@@ -13,16 +13,16 @@
         .. image:: https://img.shields.io/pypi/v/emborg.svg
             :target: https://pypi.python.org/pypi/emborg
         
         .. image:: https://img.shields.io/pypi/pyversions/emborg.svg
             :target: https://pypi.python.org/pypi/emborg/
         
         :Author: Ken Kundert
-        :Version: 1.8.0
-        :Released: 2019-10-12
+        :Version: 1.9.0
+        :Released: 2019-11-08
         
         *Emborg* is a simple command line utility to orchestrate backups. It is built as 
         a front-end to Borg, a powerful and fast deduplicating backup program.  With 
         *Emborg*, you specify all the details about your backups once in advance, and 
         then use a very simple command line interface for your day-to-day activities.  
         The details are contained in ~/.config/emborg.  That directory contains a file 
         (settings) that contains shared settings, and then another file for each backup
```

### Comparing `emborg-1.8.0/setup.py` & `emborg-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup
 
 with open('README.rst') as file:
     readme = file.read()
 
 setup(
     name = 'emborg',
-    version = '1.8.0',
+    version = '1.9.0',
     author = 'Ken Kundert',
     author_email = 'emborg@nurdletech.com',
     description = 'Borg front end.',
     long_description = readme,
     url = 'https://emborg.readthedocs.io',
     download_url = 'https://github.com/kenkundert/emborg/tarball/master',
     license = 'GPLv3+',
```

