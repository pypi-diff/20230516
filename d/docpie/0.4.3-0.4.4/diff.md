# Comparing `tmp/docpie-0.4.3.tar.gz` & `tmp/docpie-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/docpie-0.4.3.tar", last modified: Sun Jul 21 13:44:41 2019, max compression
+gzip compressed data, was "docpie-0.4.4.tar", last modified: Tue May 16 05:55:28 2023, max compression
```

## Comparing `docpie-0.4.3.tar` & `docpie-0.4.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2019-07-21 13:44:41.000000 docpie-0.4.3/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    10890 2019-07-21 13:41:37.000000 docpie-0.4.3/CHANGELOG.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1078 2019-07-21 12:59:33.000000 docpie-0.4.3/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       56 2019-07-21 12:59:33.000000 docpie-0.4.3/MANIFEST.in
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6068 2019-07-21 13:44:41.000000 docpie-0.4.3/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3904 2019-07-21 13:41:10.000000 docpie-0.4.3/README.rst
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2019-07-21 13:44:41.000000 docpie-0.4.3/docpie/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     5620 2019-07-21 13:40:03.000000 docpie-0.4.3/docpie/__init__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     5834 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/bashlog.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     9858 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/complete.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    52530 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/element.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1561 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/error.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2019-07-21 13:44:41.000000 docpie-0.4.3/docpie/example/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      451 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/calculator_example.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      631 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/change_section_title_example.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      436 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/counted_example.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      699 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/cp.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3412 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/customize_output_and_exit_code.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2019-07-21 13:44:41.000000 docpie-0.4.3/docpie/example/git/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        0 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/git/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2304 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/git/git.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      886 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/git/git_add.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1433 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/git/git_branch.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      975 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/git/git_checkout.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1284 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/git/git_clone.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     2118 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/git/git_commit.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      938 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/git/git_push.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      932 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/git/git_remote.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      712 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/hide_options_in_help_extra.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      740 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/hide_options_in_help_inherit.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      546 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/interactive_example.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      569 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/naval_fate.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      213 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/odd_even_example.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      352 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/option_format_example.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1445 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/option_format_indent_example.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      543 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/options_shortcut_example.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      285 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/quick_example.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3298 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/example/serialization.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    34499 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/parser.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    29999 2019-07-21 13:40:03.000000 docpie-0.4.3/docpie/pie.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    88520 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/test.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     9278 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/tokens.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2135 2019-07-21 12:59:33.000000 docpie-0.4.3/docpie/tracemore.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2019-07-21 13:44:41.000000 docpie-0.4.3/docpie.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6068 2019-07-21 13:44:40.000000 docpie-0.4.3/docpie.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1215 2019-07-21 13:44:40.000000 docpie-0.4.3/docpie.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2019-07-21 13:44:40.000000 docpie-0.4.3/docpie.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2019-07-21 13:44:40.000000 docpie-0.4.3/docpie.egg-info/top_level.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       90 2019-07-21 13:44:41.000000 docpie-0.4.3/setup.cfg
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     1564 2019-07-21 12:59:33.000000 docpie-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:55:28.732000 docpie-0.4.4/
+-rw-rw-rw-   0        0        0    11118 2023-05-16 05:52:27.000000 docpie-0.4.4/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1078 2023-05-12 06:11:35.000000 docpie-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-05-12 06:11:35.000000 docpie-0.4.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     5128 2023-05-16 05:55:28.732000 docpie-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3909 2023-05-16 05:52:27.000000 docpie-0.4.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-16 05:55:28.697993 docpie-0.4.4/docpie/
+-rw-rw-rw-   0        0        0     5621 2023-05-16 05:52:27.000000 docpie-0.4.4/docpie/__init__.py
+-rw-rw-rw-   0        0        0     6237 2023-05-16 05:52:27.000000 docpie-0.4.4/docpie/bashlog.py
+-rw-rw-rw-   0        0        0     9858 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/complete.py
+-rw-rw-rw-   0        0        0    52856 2023-05-16 05:52:27.000000 docpie-0.4.4/docpie/element.py
+-rw-rw-rw-   0        0        0     1561 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/error.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:55:28.719998 docpie-0.4.4/docpie/example/
+-rw-rw-rw-   0        0        0      451 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/calculator_example.py
+-rw-rw-rw-   0        0        0      631 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/change_section_title_example.py
+-rw-rw-rw-   0        0        0      436 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/counted_example.py
+-rw-rw-rw-   0        0        0      699 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/cp.py
+-rw-rw-rw-   0        0        0     3412 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/customize_output_and_exit_code.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:55:28.731000 docpie-0.4.4/docpie/example/git/
+-rw-rw-rw-   0        0        0        0 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/git/__init__.py
+-rw-rw-rw-   0        0        0     2304 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/git/git.py
+-rw-rw-rw-   0        0        0      886 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/git/git_add.py
+-rw-rw-rw-   0        0        0     1433 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/git/git_branch.py
+-rw-rw-rw-   0        0        0      975 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/git/git_checkout.py
+-rw-rw-rw-   0        0        0     1284 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/git/git_clone.py
+-rw-rw-rw-   0        0        0     2118 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/git/git_commit.py
+-rw-rw-rw-   0        0        0      938 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/git/git_push.py
+-rw-rw-rw-   0        0        0      932 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/git/git_remote.py
+-rw-rw-rw-   0        0        0      712 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/hide_options_in_help_extra.py
+-rw-rw-rw-   0        0        0      740 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/hide_options_in_help_inherit.py
+-rw-rw-rw-   0        0        0      546 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/interactive_example.py
+-rw-rw-rw-   0        0        0      569 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/naval_fate.py
+-rw-rw-rw-   0        0        0      213 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/odd_even_example.py
+-rw-rw-rw-   0        0        0      352 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/option_format_example.py
+-rw-rw-rw-   0        0        0     1445 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/option_format_indent_example.py
+-rw-rw-rw-   0        0        0      543 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/options_shortcut_example.py
+-rw-rw-rw-   0        0        0      285 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/quick_example.py
+-rw-rw-rw-   0        0        0     3298 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/example/serialization.py
+-rw-rw-rw-   0        0        0    34499 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/parser.py
+-rw-rw-rw-   0        0        0    30000 2023-05-16 05:52:27.000000 docpie-0.4.4/docpie/pie.py
+-rw-rw-rw-   0        0        0    90155 2023-05-16 05:52:27.000000 docpie-0.4.4/docpie/test.py
+-rw-rw-rw-   0        0        0     9278 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/tokens.py
+-rw-rw-rw-   0        0        0     2135 2023-05-12 06:11:35.000000 docpie-0.4.4/docpie/tracemore.py
+drwxrwxrwx   0        0        0        0 2023-05-16 05:55:28.702994 docpie-0.4.4/docpie.egg-info/
+-rw-rw-rw-   0        0        0     5128 2023-05-16 05:55:28.000000 docpie-0.4.4/docpie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1215 2023-05-16 05:55:28.000000 docpie-0.4.4/docpie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 05:55:28.000000 docpie-0.4.4/docpie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 05:55:28.000000 docpie-0.4.4/docpie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      100 2023-05-16 05:55:28.733000 docpie-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1564 2023-05-12 06:11:35.000000 docpie-0.4.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `docpie-0.4.3/CHANGELOG.md` & `docpie-0.4.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 ## TODO
 
 *   Refactory
 *   Add a bash auto-complete tool [#2](https://github.com/TylerTemp/docpie/issues/2)
 *   Document needs a better organization
 
+## 0.4.4
+
+*   [fix] change auto balance function, fix the issue that won't work for this case:
+    
+        """
+        Usage: 
+            cp [options] <source>... <target>
+        
+        Options:
+            -R
+        """
+
 ## 0.4.3
 
 *   [change] no more `locals` under `docpie` function as it may lead to unexpected behavior
 
 ## 0.4.2
 
 *   [fix] when no `options` section presented, fix the bug that `python` style
```

### Comparing `docpie-0.4.3/LICENSE` & `docpie-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/PKG-INFO` & `docpie-0.4.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,166 +1,174 @@
-Metadata-Version: 1.1
-Name: docpie
-Version: 0.4.3
-Summary: An easy and Pythonic way to create your POSIX command line interface
-Home-page: http://docpie.comes.today/
-Author: TylerTemp
-Author-email: tylertempdev@gmail.com
-License: MIT
-Download-URL: https://github.com/TylerTemp/docpie/tarball/0.4.3/
-Description: .. docpie
-        .. README.rst
-        
-        docpie
-        ======
-        
-        `An easy and Pythonic way to create your POSIX command line`
-        
-        View on: `GitHub <https://github.com/TylerTemp/docpie/>`__ /
-        `PyPi <https://pypi.org/project/docpie/>`__
-        
-        .. image:: https://travis-ci.org/TylerTemp/docpie.svg?branch=master
-            :target: https://travis-ci.org/TylerTemp/docpie
-        
-        .. contents::
-        
-        ChangeLog
-        ---------
-        
-        version 0.4.3:
-        
-        -   [change] no more ``locals`` under ``docpie`` function as it may lead to unexpected behavior
-        
-        `full changelog & TODOs <https://github.com/TylerTemp/docpie/blob/master/CHANGELOG.md>`__
-        
-        
-        Summary
-        -------
-        
-        How do you define your command line interface?
-        Write a parse by yourself or spend hours learning ``optparse`` / ``argparse`` ,
-        and modify both code side and document every time you update the interface?
-        
-        
-        Life is short, man! You can simply do it this way:
-        
-        .. code:: python
-        
-           """
-           My copy script
-        
-           Usage:
-             cp.py [options] <source_file> <target_file>
-             cp.py [options] <source_file>... <target_directory>
-        
-           Options:
-             -h -? --help    print this screen
-             --version       print the version of this script
-             -v --verbose    print more information while  running
-           """
-        
-           from docpie import docpie
-           args = docpie(__doc__)
-           print(args)
-        
-        Now run it
-        
-        .. code:: bash
-        
-           $ python cp.py a.txt b.txt c.txt /tmp
-           {'--': False,
-            '--help': False,
-            '--verbose': False,
-            '--version': False,
-            '-?': False,
-            '-h': False,
-            '-v': False,
-            '<source_file>': ['a.txt', 'b.txt', 'c.txt'],
-            '<target_directory>': '/tmp',
-            '<target_file>': None}
-        
-        Write a ``__doc__``, pass it to a function, DONE! Isn't it simple?
-        
-        `try it \>\> <http://docpie.comes.today/try?argvnofilestr=a.txt%20b.txt%20c.txt%20%2Ftmp&attachopt=on&attachvalue=on&auto2dashes=on&doc=My%20copy%20script%5Cn%5CnUsage%3A%5Cn%20%20cp.py%20%5Boptions%5D%20%3Csource_file%3E%20%3Ctarget_file%3E%5Cn%20%20cp.py%20%5Boptions%5D%20%3Csource_file%3E...%20%3Ctarget_directory%3E%5Cn%5CnOptions%3A%5Cn%20%20-h%20-%3F%20--help%20%20%20%20print%20this%20screen%5Cn%20%20--version%20%20%20%20%20%20%20print%20the%20version%20of%20this%20script%5Cn%20%20-v%20--verbose%20%20%20%20print%20more%20information%20while%20%20running&help=on&replace=on&stdopt=on>`__
-        
-        Installation
-        ------------
-        
-        Install release version:
-        
-        .. code:: python
-        
-            pip install docpie
-        
-        Install nightly/dev version:
-        
-        .. code:: bash
-        
-            pip install git+https://github.com/TylerTemp/docpie.git@dev
-        
-        ``docpie`` has been tested with Python:
-        
-        -   2.6, 2.7, pypy-2.0, pypy-2.6
-        -   3.2, 3.3, 3.4, 3.5, pypy3-2.4
-        
-        You can run test suit by ``python setup.py test``
-        
-        Get Start!
-        ----------
-        
-        Interested? Visit `Wiki <https://github.com/TylerTemp/docpie/wiki>`__
-        and get start!
-        
-        Or you can `try it in your browser <http://docpie.comes.today/try/>`__
-        
-        Why docpie?
-        -----------
-        
-        ``docpie`` can greatly reduce the work you need to be done for
-        command-line interface. What you see is what you get.
-        Every time you only need to update your document, and keep the
-        code unchanged.
-        
-        See `here <https://github.com/TylerTemp/docpie/wiki/Why-docpie>`__ for more reasons.
-        
-        Reference
-        ---------
-        
-        the code in ``bashlog.py`` is taken from
-        `tornado <https://github.com/tornadoweb/tornado>`__, and
-        ``tracemore.py`` is from `python
-        Cookbook <http://www.amazon.com/Python-Cookbook-Third-David-Beazley/dp/1449340377/ref=sr_1_1?ie=UTF8&qid=1440593849&sr=8-1&keywords=python+cookbook>`__
-        
-        Many examples & tests are from ``docopt``.
-        
-        License
-        -------
-        
-        ``docpie`` is released under
-        `MIT-License <https://github.com/TylerTemp/docpie/blob/master/LICENSE>`__
-        
-        Donate
-        ------
-        
-        If you like this project, you can buy me a beer so I can make it better!
-        
-        .. image:: https://dn-tyler.qbox.me/alipay.ico
-            :target: https://dn-tyler.qbox.me/myalipay.png
-        
-        .. image:: https://button.flattr.com/flattr-badge-large.png
-            :target: https://flattr.com/submit/auto?user_id=TylerTemp&url=http%3A%2F%2Fdocpie.comes.today
-        
-Keywords: option arguments parsing optparse argparse getopt docopt
-Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Utilities
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Metadata-Version: 2.1
+Name: docpie
+Version: 0.4.4
+Summary: An easy and Pythonic way to create your POSIX command line interface
+Home-page: http://docpie.comes.today/
+Download-URL: https://github.com/TylerTemp/docpie/tarball/0.4.4/
+Author: TylerTemp
+Author-email: tylertempdev@gmail.com
+License: MIT
+Keywords: option arguments parsing optparse argparse getopt docopt
+Platform: any
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Utilities
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
+
+.. docpie
+.. README.rst
+
+docpie
+======
+
+`An easy and Pythonic way to create your POSIX command line`
+
+View on: `GitHub <https://github.com/TylerTemp/docpie/>`__ /
+`PyPi <https://pypi.org/project/docpie/>`__
+
+.. image:: https://travis-ci.org/TylerTemp/docpie.svg?branch=master
+    :target: https://travis-ci.org/TylerTemp/docpie
+
+.. contents::
+
+ChangeLog
+---------
+
+version 0.4.4:
+
+change auto balance function, fix the issue that won't work for this case
+
+.. code-block:: python
+
+    """
+    Usage:
+        cp [options] <source>... <target>
+
+    Options:
+        -R
+    """
+
+Summary
+-------
+
+How do you define your command line interface?
+Write a parse by yourself or spend hours learning ``optparse`` / ``argparse`` ,
+and modify both code side and document every time you update the interface?
+
+
+Life is short, man! You can simply do it this way:
+
+.. code:: python
+
+   """
+   My copy script
+
+   Usage:
+     cp.py [options] <source_file> <target_file>
+     cp.py [options] <source_file>... <target_directory>
+
+   Options:
+     -h -? --help    print this screen
+     --version       print the version of this script
+     -v --verbose    print more information while  running
+   """
+
+   from docpie import docpie
+   args = docpie(__doc__)
+   print(args)
+
+Now run it
+
+.. code:: bash
+
+   $ python cp.py a.txt b.txt c.txt /tmp
+   {'--': False,
+    '--help': False,
+    '--verbose': False,
+    '--version': False,
+    '-?': False,
+    '-h': False,
+    '-v': False,
+    '<source_file>': ['a.txt', 'b.txt', 'c.txt'],
+    '<target_directory>': '/tmp',
+    '<target_file>': None}
+
+Write a ``__doc__``, pass it to a function, DONE! Isn't it simple?
+
+`try it \>\> <http://docpie.comes.today/try?argvnofilestr=a.txt%20b.txt%20c.txt%20%2Ftmp&attachopt=on&attachvalue=on&auto2dashes=on&doc=My%20copy%20script%5Cn%5CnUsage%3A%5Cn%20%20cp.py%20%5Boptions%5D%20%3Csource_file%3E%20%3Ctarget_file%3E%5Cn%20%20cp.py%20%5Boptions%5D%20%3Csource_file%3E...%20%3Ctarget_directory%3E%5Cn%5CnOptions%3A%5Cn%20%20-h%20-%3F%20--help%20%20%20%20print%20this%20screen%5Cn%20%20--version%20%20%20%20%20%20%20print%20the%20version%20of%20this%20script%5Cn%20%20-v%20--verbose%20%20%20%20print%20more%20information%20while%20%20running&help=on&replace=on&stdopt=on>`__
+
+Installation
+------------
+
+Install release version:
+
+.. code:: python
+
+    pip install docpie
+
+Install nightly/dev version:
+
+.. code:: bash
+
+    pip install git+https://github.com/TylerTemp/docpie.git@dev
+
+``docpie`` has been tested with Python:
+
+-   2.6, 2.7, pypy-2.0, pypy-2.6
+-   3.2, 3.3, 3.4, 3.5, pypy3-2.4
+
+You can run test suit by ``python setup.py test``
+
+Get Start!
+----------
+
+Interested? Visit `Wiki <https://github.com/TylerTemp/docpie/wiki>`__
+and get start!
+
+Or you can `try it in your browser <http://docpie.comes.today/try/>`__
+
+Why docpie?
+-----------
+
+``docpie`` can greatly reduce the work you need to be done for
+command-line interface. What you see is what you get.
+Every time you only need to update your document, and keep the
+code unchanged.
+
+See `here <https://github.com/TylerTemp/docpie/wiki/Why-docpie>`__ for more reasons.
+
+Reference
+---------
+
+the code in ``bashlog.py`` is taken from
+`tornado <https://github.com/tornadoweb/tornado>`__, and
+``tracemore.py`` is from `python
+Cookbook <http://www.amazon.com/Python-Cookbook-Third-David-Beazley/dp/1449340377/ref=sr_1_1?ie=UTF8&qid=1440593849&sr=8-1&keywords=python+cookbook>`__
+
+Many examples & tests are from ``docopt``.
+
+License
+-------
+
+``docpie`` is released under
+`MIT-License <https://github.com/TylerTemp/docpie/blob/master/LICENSE>`__
+
+Donate
+------
+
+If you like this project, you can buy me a beer so I can make it better!
+
+.. image:: https://dn-tyler.qbox.me/alipay.ico
+    :target: https://dn-tyler.qbox.me/myalipay.png
+
+.. image:: https://button.flattr.com/flattr-badge-large.png
+    :target: https://flattr.com/submit/auto?user_id=TylerTemp&url=http%3A%2F%2Fdocpie.comes.today
```

### Comparing `docpie-0.4.3/README.rst` & `docpie-0.4.4/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,27 @@
     :target: https://travis-ci.org/TylerTemp/docpie
 
 .. contents::
 
 ChangeLog
 ---------
 
-version 0.4.3:
+version 0.4.4:
 
--   [change] no more ``locals`` under ``docpie`` function as it may lead to unexpected behavior
+change auto balance function, fix the issue that won't work for this case
 
-`full changelog & TODOs <https://github.com/TylerTemp/docpie/blob/master/CHANGELOG.md>`__
+.. code-block:: python
 
+    """
+    Usage:
+        cp [options] <source>... <target>
+
+    Options:
+        -R
+    """
 
 Summary
 -------
 
 How do you define your command line interface?
 Write a parse by yourself or spend hours learning ``optparse`` / ``argparse`` ,
 and modify both code side and document every time you update the interface?
```

### Comparing `docpie-0.4.3/docpie/__init__.py` & `docpie-0.4.4/docpie/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
            'ExpectArgumentExit', 'ExpectArgumentHitDoubleDashesExit',
            'AmbiguousPrefixExit',
            'logger']
 
 # it's not a good idea but it can avoid loop importing
 __version__ = Docpie._version
 
-__timestamp__ = 1563716272.669418  # last sumbit
+__timestamp__ = 1684215839.7577085  # last sumbit
 
 logger = getLogger('docpie')
 
 
 def docpie(doc, argv=None, help=True, version=None,
            stdopt=True, attachopt=True, attachvalue=True,
            helpstyle='python',
```

### Comparing `docpie-0.4.3/docpie/bashlog.py` & `docpie-0.4.4/docpie/bashlog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 '''A simple wrapper of logging that support color prompt on Linux'''
 import sys
+import subprocess
 import logging
 from logging import DEBUG, INFO, WARNING, ERROR, CRITICAL
 
 __all__ = ['getlogger', 'stdoutlogger', 'filelogger', 'streamlogger',
            'ColorFormatter',
            'DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL']
 # Note: Only terminal which support color can use this
@@ -23,15 +24,24 @@
     basestring_type = basestring
 
 _TO_UNICODE_TYPES = (unicode_type, type(None))
 
 
 def _stderr_supports_color():
     if sys.platform.startswith('win32'):
-        return False
+        # return 'CYGWIN' in platform.system().lower()
+        try:
+            p = subprocess.Popen(['uname', '-a'], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        except FileNotFoundError:
+            return False
+        p_out, p_err = p.communicate()
+        if p.returncode != 0:
+            return False
+        p_content = p_out.decode('utf-8')
+        return 'cygwin' in p_content.lower()
     if hasattr(sys.stderr, 'isatty') and sys.stderr.isatty():
         return True
     return False
 
 
 def to_unicode(value):
     """Converts a string argument to a unicode string.
```

### Comparing `docpie-0.4.3/docpie/complete.py` & `docpie-0.4.4/docpie/complete.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/element.py` & `docpie-0.4.4/docpie/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -907,26 +907,31 @@
     # TODO: better solution
     def balance_value_for_ellipsis_args(self):
         # This method can deal more complex situation now:
         # (<arg1> <arg2>)... <arg3>
         # <arg>... <arg2> cmd
         # <arg>... (cmd <arg2>) <arg3>
         # see: https://github.com/TylerTemp/docpie/blob/master/CHANGELOG.md#026
+        logger.debug("try balance %s", self)
 
         ele_num = len(self)
         for index_1, element in enumerate(self, 1):
             if index_1 == ele_num:    # the last one
+                logger.debug("already last one: %s", self)
                 return False
 
             if isinstance(element, OptionsShortcut):
+                logger.debug("skip OptionsShortcut: %s", self)
                 continue
 
             if not element.matched():
                 logger.debug('%r not matched at all', element)
-                return False
+                if isinstance(element, Required):
+                    return False
+                continue
 
             # 1, 0, list
             ellipsis_args = self.can_lend_value(element)
             if ellipsis_args == 1:
                 continue
             elif ellipsis_args == 0:
                 return False
@@ -1281,16 +1286,18 @@
         matched_status = self._match_oneline(argv)
 
         if all(matched_status):
             logger.debug('%s matched', self)
             return True
         logger.debug('%s matching failed %s / %s', self, matched_status, argv)
         if self.balance_value_for_ellipsis_args():
-            logger.debug('%s balace value succeed', self)
+            logger.debug('%s balance value succeed', self)
             return True
+        else:
+            logger.debug('%s balance value failed', self)
 
         self.load_value(self_value)
         argv.load_value(argv_value)
         # saver.rollback(self, argv)
         return False
 
     def __eq__(self, other):
```

### Comparing `docpie-0.4.3/docpie/error.py` & `docpie-0.4.4/docpie/error.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/change_section_title_example.py` & `docpie-0.4.4/docpie/example/change_section_title_example.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/cp.py` & `docpie-0.4.4/docpie/example/cp.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/customize_output_and_exit_code.py` & `docpie-0.4.4/docpie/example/customize_output_and_exit_code.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/git/git.py` & `docpie-0.4.4/docpie/example/git/git.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/git/git_add.py` & `docpie-0.4.4/docpie/example/git/git_add.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/git/git_branch.py` & `docpie-0.4.4/docpie/example/git/git_branch.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/git/git_checkout.py` & `docpie-0.4.4/docpie/example/git/git_checkout.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/git/git_clone.py` & `docpie-0.4.4/docpie/example/git/git_clone.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/git/git_commit.py` & `docpie-0.4.4/docpie/example/git/git_commit.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/git/git_push.py` & `docpie-0.4.4/docpie/example/git/git_push.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/git/git_remote.py` & `docpie-0.4.4/docpie/example/git/git_remote.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/hide_options_in_help_extra.py` & `docpie-0.4.4/docpie/example/hide_options_in_help_extra.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/hide_options_in_help_inherit.py` & `docpie-0.4.4/docpie/example/hide_options_in_help_inherit.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/interactive_example.py` & `docpie-0.4.4/docpie/example/interactive_example.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/naval_fate.py` & `docpie-0.4.4/docpie/example/naval_fate.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/option_format_indent_example.py` & `docpie-0.4.4/docpie/example/option_format_indent_example.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/options_shortcut_example.py` & `docpie-0.4.4/docpie/example/options_shortcut_example.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/example/serialization.py` & `docpie-0.4.4/docpie/example/serialization.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/parser.py` & `docpie-0.4.4/docpie/parser.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/pie.py` & `docpie-0.4.4/docpie/pie.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 logger = logging.getLogger('docpie')
 
 
 class Docpie(dict):
 
     # Docpie version
-    # it's not a good idea but it can avoid loop importing
-    _version = '0.4.3'
+    # it's not a good idea, but it can avoid loop importing
+    _version = '0.4.4'
 
     option_name = 'Options:'
     usage_name = 'Usage:'
     doc = None
 
     case_sensitive = False
     auto2dashes = True
```

### Comparing `docpie-0.4.3/docpie/test.py` & `docpie-0.4.4/docpie/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -2256,14 +2256,51 @@
 
         sys.argv = ['prog', 'source', 'target']
         self.eq(doc, {'--': False, '-f': False, '-v': False,
                       '--verbose': False, '-X': False, '-R': False,
                       '<source_file>': ['source'],
                       '<target_directory>': 'target'})
 
+    def test_cp_option_not_work(self):
+        doc = """Example for docpie, linux cp-like command
+
+
+    NAME
+         cp -- copy files
+
+    USAGE:
+         cp [options] <source_file> ... <target_directory>
+
+    OPTIONS:
+         -f    If the destination file cannot be opened, remove it and create a
+               new file, without prompting for confirmation regardless of its per-
+               missions.
+         -v, --verbose
+               Cause cp to be verbose, showing files as they are copied.
+         -X    Do not copy Extended Attributes (EAs) or resource forks.
+         -R    If source_file designates a directory, cp copies the directory and
+               the entire subtree connected at that point."""
+
+        sys.argv = ['prog', 'source', 'target', '-R']
+        self.eq(doc, {'--': False, '-f': False, '-v': False,
+                      '--verbose': False, '-X': False, '-R': True,
+                      '<source_file>': ['source'],
+                      '<target_directory>': 'target'})
+        sys.argv = ['prog', 'source1', 'source2', 'target', '-R']
+        self.eq(doc, {'--': False, '-f': False, '-v': False,
+                      '--verbose': False, '-X': False, '-R': True,
+                      '<source_file>': ['source1', 'source2'],
+                      '<target_directory>': 'target'})
+
+        sys.argv = ['prog', 'source1', '-R', 'source2', 'target']
+        self.eq(doc, {'--': False, '-f': False, '-v': False,
+                      '--verbose': False, '-X': False, '-R': True,
+                      '<source_file>': ['source1', 'source2'],
+                      '<target_directory>': 'target'})
+
     def test_option_section_title(self):
         doc = """
         Usage: prog [options]
 
         OpTiOnS:
             -a
         Another OpTiOnS:
```

### Comparing `docpie-0.4.3/docpie/tokens.py` & `docpie-0.4.4/docpie/tokens.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie/tracemore.py` & `docpie-0.4.4/docpie/tracemore.py`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/docpie.egg-info/PKG-INFO` & `docpie-0.4.4/docpie.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,166 +1,174 @@
-Metadata-Version: 1.1
-Name: docpie
-Version: 0.4.3
-Summary: An easy and Pythonic way to create your POSIX command line interface
-Home-page: http://docpie.comes.today/
-Author: TylerTemp
-Author-email: tylertempdev@gmail.com
-License: MIT
-Download-URL: https://github.com/TylerTemp/docpie/tarball/0.4.3/
-Description: .. docpie
-        .. README.rst
-        
-        docpie
-        ======
-        
-        `An easy and Pythonic way to create your POSIX command line`
-        
-        View on: `GitHub <https://github.com/TylerTemp/docpie/>`__ /
-        `PyPi <https://pypi.org/project/docpie/>`__
-        
-        .. image:: https://travis-ci.org/TylerTemp/docpie.svg?branch=master
-            :target: https://travis-ci.org/TylerTemp/docpie
-        
-        .. contents::
-        
-        ChangeLog
-        ---------
-        
-        version 0.4.3:
-        
-        -   [change] no more ``locals`` under ``docpie`` function as it may lead to unexpected behavior
-        
-        `full changelog & TODOs <https://github.com/TylerTemp/docpie/blob/master/CHANGELOG.md>`__
-        
-        
-        Summary
-        -------
-        
-        How do you define your command line interface?
-        Write a parse by yourself or spend hours learning ``optparse`` / ``argparse`` ,
-        and modify both code side and document every time you update the interface?
-        
-        
-        Life is short, man! You can simply do it this way:
-        
-        .. code:: python
-        
-           """
-           My copy script
-        
-           Usage:
-             cp.py [options] <source_file> <target_file>
-             cp.py [options] <source_file>... <target_directory>
-        
-           Options:
-             -h -? --help    print this screen
-             --version       print the version of this script
-             -v --verbose    print more information while  running
-           """
-        
-           from docpie import docpie
-           args = docpie(__doc__)
-           print(args)
-        
-        Now run it
-        
-        .. code:: bash
-        
-           $ python cp.py a.txt b.txt c.txt /tmp
-           {'--': False,
-            '--help': False,
-            '--verbose': False,
-            '--version': False,
-            '-?': False,
-            '-h': False,
-            '-v': False,
-            '<source_file>': ['a.txt', 'b.txt', 'c.txt'],
-            '<target_directory>': '/tmp',
-            '<target_file>': None}
-        
-        Write a ``__doc__``, pass it to a function, DONE! Isn't it simple?
-        
-        `try it \>\> <http://docpie.comes.today/try?argvnofilestr=a.txt%20b.txt%20c.txt%20%2Ftmp&attachopt=on&attachvalue=on&auto2dashes=on&doc=My%20copy%20script%5Cn%5CnUsage%3A%5Cn%20%20cp.py%20%5Boptions%5D%20%3Csource_file%3E%20%3Ctarget_file%3E%5Cn%20%20cp.py%20%5Boptions%5D%20%3Csource_file%3E...%20%3Ctarget_directory%3E%5Cn%5CnOptions%3A%5Cn%20%20-h%20-%3F%20--help%20%20%20%20print%20this%20screen%5Cn%20%20--version%20%20%20%20%20%20%20print%20the%20version%20of%20this%20script%5Cn%20%20-v%20--verbose%20%20%20%20print%20more%20information%20while%20%20running&help=on&replace=on&stdopt=on>`__
-        
-        Installation
-        ------------
-        
-        Install release version:
-        
-        .. code:: python
-        
-            pip install docpie
-        
-        Install nightly/dev version:
-        
-        .. code:: bash
-        
-            pip install git+https://github.com/TylerTemp/docpie.git@dev
-        
-        ``docpie`` has been tested with Python:
-        
-        -   2.6, 2.7, pypy-2.0, pypy-2.6
-        -   3.2, 3.3, 3.4, 3.5, pypy3-2.4
-        
-        You can run test suit by ``python setup.py test``
-        
-        Get Start!
-        ----------
-        
-        Interested? Visit `Wiki <https://github.com/TylerTemp/docpie/wiki>`__
-        and get start!
-        
-        Or you can `try it in your browser <http://docpie.comes.today/try/>`__
-        
-        Why docpie?
-        -----------
-        
-        ``docpie`` can greatly reduce the work you need to be done for
-        command-line interface. What you see is what you get.
-        Every time you only need to update your document, and keep the
-        code unchanged.
-        
-        See `here <https://github.com/TylerTemp/docpie/wiki/Why-docpie>`__ for more reasons.
-        
-        Reference
-        ---------
-        
-        the code in ``bashlog.py`` is taken from
-        `tornado <https://github.com/tornadoweb/tornado>`__, and
-        ``tracemore.py`` is from `python
-        Cookbook <http://www.amazon.com/Python-Cookbook-Third-David-Beazley/dp/1449340377/ref=sr_1_1?ie=UTF8&qid=1440593849&sr=8-1&keywords=python+cookbook>`__
-        
-        Many examples & tests are from ``docopt``.
-        
-        License
-        -------
-        
-        ``docpie`` is released under
-        `MIT-License <https://github.com/TylerTemp/docpie/blob/master/LICENSE>`__
-        
-        Donate
-        ------
-        
-        If you like this project, you can buy me a beer so I can make it better!
-        
-        .. image:: https://dn-tyler.qbox.me/alipay.ico
-            :target: https://dn-tyler.qbox.me/myalipay.png
-        
-        .. image:: https://button.flattr.com/flattr-badge-large.png
-            :target: https://flattr.com/submit/auto?user_id=TylerTemp&url=http%3A%2F%2Fdocpie.comes.today
-        
-Keywords: option arguments parsing optparse argparse getopt docopt
-Platform: any
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Utilities
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: Implementation :: PyPy
+Metadata-Version: 2.1
+Name: docpie
+Version: 0.4.4
+Summary: An easy and Pythonic way to create your POSIX command line interface
+Home-page: http://docpie.comes.today/
+Download-URL: https://github.com/TylerTemp/docpie/tarball/0.4.4/
+Author: TylerTemp
+Author-email: tylertempdev@gmail.com
+License: MIT
+Keywords: option arguments parsing optparse argparse getopt docopt
+Platform: any
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Topic :: Utilities
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.2
+Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+License-File: LICENSE
+
+.. docpie
+.. README.rst
+
+docpie
+======
+
+`An easy and Pythonic way to create your POSIX command line`
+
+View on: `GitHub <https://github.com/TylerTemp/docpie/>`__ /
+`PyPi <https://pypi.org/project/docpie/>`__
+
+.. image:: https://travis-ci.org/TylerTemp/docpie.svg?branch=master
+    :target: https://travis-ci.org/TylerTemp/docpie
+
+.. contents::
+
+ChangeLog
+---------
+
+version 0.4.4:
+
+change auto balance function, fix the issue that won't work for this case
+
+.. code-block:: python
+
+    """
+    Usage:
+        cp [options] <source>... <target>
+
+    Options:
+        -R
+    """
+
+Summary
+-------
+
+How do you define your command line interface?
+Write a parse by yourself or spend hours learning ``optparse`` / ``argparse`` ,
+and modify both code side and document every time you update the interface?
+
+
+Life is short, man! You can simply do it this way:
+
+.. code:: python
+
+   """
+   My copy script
+
+   Usage:
+     cp.py [options] <source_file> <target_file>
+     cp.py [options] <source_file>... <target_directory>
+
+   Options:
+     -h -? --help    print this screen
+     --version       print the version of this script
+     -v --verbose    print more information while  running
+   """
+
+   from docpie import docpie
+   args = docpie(__doc__)
+   print(args)
+
+Now run it
+
+.. code:: bash
+
+   $ python cp.py a.txt b.txt c.txt /tmp
+   {'--': False,
+    '--help': False,
+    '--verbose': False,
+    '--version': False,
+    '-?': False,
+    '-h': False,
+    '-v': False,
+    '<source_file>': ['a.txt', 'b.txt', 'c.txt'],
+    '<target_directory>': '/tmp',
+    '<target_file>': None}
+
+Write a ``__doc__``, pass it to a function, DONE! Isn't it simple?
+
+`try it \>\> <http://docpie.comes.today/try?argvnofilestr=a.txt%20b.txt%20c.txt%20%2Ftmp&attachopt=on&attachvalue=on&auto2dashes=on&doc=My%20copy%20script%5Cn%5CnUsage%3A%5Cn%20%20cp.py%20%5Boptions%5D%20%3Csource_file%3E%20%3Ctarget_file%3E%5Cn%20%20cp.py%20%5Boptions%5D%20%3Csource_file%3E...%20%3Ctarget_directory%3E%5Cn%5CnOptions%3A%5Cn%20%20-h%20-%3F%20--help%20%20%20%20print%20this%20screen%5Cn%20%20--version%20%20%20%20%20%20%20print%20the%20version%20of%20this%20script%5Cn%20%20-v%20--verbose%20%20%20%20print%20more%20information%20while%20%20running&help=on&replace=on&stdopt=on>`__
+
+Installation
+------------
+
+Install release version:
+
+.. code:: python
+
+    pip install docpie
+
+Install nightly/dev version:
+
+.. code:: bash
+
+    pip install git+https://github.com/TylerTemp/docpie.git@dev
+
+``docpie`` has been tested with Python:
+
+-   2.6, 2.7, pypy-2.0, pypy-2.6
+-   3.2, 3.3, 3.4, 3.5, pypy3-2.4
+
+You can run test suit by ``python setup.py test``
+
+Get Start!
+----------
+
+Interested? Visit `Wiki <https://github.com/TylerTemp/docpie/wiki>`__
+and get start!
+
+Or you can `try it in your browser <http://docpie.comes.today/try/>`__
+
+Why docpie?
+-----------
+
+``docpie`` can greatly reduce the work you need to be done for
+command-line interface. What you see is what you get.
+Every time you only need to update your document, and keep the
+code unchanged.
+
+See `here <https://github.com/TylerTemp/docpie/wiki/Why-docpie>`__ for more reasons.
+
+Reference
+---------
+
+the code in ``bashlog.py`` is taken from
+`tornado <https://github.com/tornadoweb/tornado>`__, and
+``tracemore.py`` is from `python
+Cookbook <http://www.amazon.com/Python-Cookbook-Third-David-Beazley/dp/1449340377/ref=sr_1_1?ie=UTF8&qid=1440593849&sr=8-1&keywords=python+cookbook>`__
+
+Many examples & tests are from ``docopt``.
+
+License
+-------
+
+``docpie`` is released under
+`MIT-License <https://github.com/TylerTemp/docpie/blob/master/LICENSE>`__
+
+Donate
+------
+
+If you like this project, you can buy me a beer so I can make it better!
+
+.. image:: https://dn-tyler.qbox.me/alipay.ico
+    :target: https://dn-tyler.qbox.me/myalipay.png
+
+.. image:: https://button.flattr.com/flattr-badge-large.png
+    :target: https://flattr.com/submit/auto?user_id=TylerTemp&url=http%3A%2F%2Fdocpie.comes.today
```

### Comparing `docpie-0.4.3/docpie.egg-info/SOURCES.txt` & `docpie-0.4.4/docpie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docpie-0.4.3/setup.py` & `docpie-0.4.4/setup.py`

 * *Files identical despite different names*

