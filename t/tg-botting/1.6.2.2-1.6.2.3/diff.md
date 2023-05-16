# Comparing `tmp/tg-botting-1.6.2.2.tar.gz` & `tmp/tg-botting-1.6.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-1.6.2.2.tar", last modified: Sat May 13 19:29:43 2023, max compression
+gzip compressed data, was "tg-botting-1.6.2.3.tar", last modified: Tue May 16 16:07:16 2023, max compression
```

## Comparing `tg-botting-1.6.2.2.tar` & `tg-botting-1.6.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 19:29:43.987284 tg-botting-1.6.2.2/
--rw-rw-rw-   0        0        0      920 2023-05-13 19:29:43.987284 tg-botting-1.6.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.6.2.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-13 19:29:43.987284 tg-botting-1.6.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1447 2023-05-13 19:28:51.000000 tg-botting-1.6.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 19:29:43.981300 tg-botting-1.6.2.2/tg_botting/
--rw-rw-rw-   0        0        0    29889 2023-05-13 19:28:51.000000 tg-botting-1.6.2.2/tg_botting/bot.py
--rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.6.2.2/tg_botting/cog.py
--rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.6.2.2/tg_botting/generals.py
--rw-rw-rw-   0        0        0    15742 2023-05-13 19:27:53.000000 tg-botting-1.6.2.2/tg_botting/objects.py
--rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.6.2.2/tg_botting/user_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-13 19:29:43.985289 tg-botting-1.6.2.2/tg_botting.egg-info/
--rw-rw-rw-   0        0        0      920 2023-05-13 19:29:43.000000 tg-botting-1.6.2.2/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-13 19:29:43.000000 tg-botting-1.6.2.2/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 19:29:43.000000 tg-botting-1.6.2.2/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-13 19:29:43.000000 tg-botting-1.6.2.2/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-13 19:29:43.000000 tg-botting-1.6.2.2/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 16:07:15.999858 tg-botting-1.6.2.3/
+-rw-rw-rw-   0        0        0      920 2023-05-16 16:07:15.999858 tg-botting-1.6.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.6.2.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 16:07:15.999858 tg-botting-1.6.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1447 2023-05-16 16:06:41.000000 tg-botting-1.6.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:07:15.999858 tg-botting-1.6.2.3/tg_botting/
+-rw-rw-rw-   0        0        0    29944 2023-05-16 16:06:41.000000 tg-botting-1.6.2.3/tg_botting/bot.py
+-rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.6.2.3/tg_botting/cog.py
+-rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.6.2.3/tg_botting/generals.py
+-rw-rw-rw-   0        0        0    15742 2023-05-13 19:27:53.000000 tg-botting-1.6.2.3/tg_botting/objects.py
+-rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.6.2.3/tg_botting/user_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:07:15.999858 tg-botting-1.6.2.3/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0      920 2023-05-16 16:07:15.000000 tg-botting-1.6.2.3/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-16 16:07:15.000000 tg-botting-1.6.2.3/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 16:07:15.000000 tg-botting-1.6.2.3/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-16 16:07:15.000000 tg-botting-1.6.2.3/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 16:07:15.000000 tg-botting-1.6.2.3/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-1.6.2.2/PKG-INFO` & `tg-botting-1.6.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.6.2.2
+Version: 1.6.2.3
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-1.6.2.2/README.md` & `tg-botting-1.6.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.2/setup.py` & `tg-botting-1.6.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.6.2.2'
+VERSION = '1.6.2.3'
 DESCRIPTION = 'python library for easy creation of a telegram bot.'
 LONG_DESCRIPTION = 'A package that allows you to create bots for telegram using its entire API.'
 
 setup(
     name="tg-botting",
     version=VERSION,
     url='https://github.com/2sweetheart2/tg_botting/tree/master',
```

### Comparing `tg-botting-1.6.2.2/tg_botting/bot.py` & `tg-botting-1.6.2.3/tg_botting/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -647,20 +647,22 @@
             rs, c, from_aliases = self.search(' '.join(ms))
             if rs:
                 for i in range(c):
                     ms.pop(0)
                 args = await self.get_args(ms)
                 need_args = signature(rs.func)
                 put_args = []
-                first = False
                 minus = 1
                 na = dict(need_args.parameters)
                 if 'self' in na.keys():
                     na.pop('self')
-                na.pop('message')
+                try:
+                    na.pop(list(na.keys())[0])
+                except:
+                    pass
                 for i in range(0,len(na)):
                     val = list(na.values())[i]
                     try:
                         if val.annotation != inspect.Parameter.empty:
                             if not isinstance(args[i-minus],val.annotation):
                                 return await self.tupe_error(message,args[i-minus],val.annotation)
                     except IndexError as e:
```

### Comparing `tg-botting-1.6.2.2/tg_botting/cog.py` & `tg-botting-1.6.2.3/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.2/tg_botting/generals.py` & `tg-botting-1.6.2.3/tg_botting/generals.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.2/tg_botting/objects.py` & `tg-botting-1.6.2.3/tg_botting/objects.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.2/tg_botting.egg-info/PKG-INFO` & `tg-botting-1.6.2.3/tg_botting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.6.2.2
+Version: 1.6.2.3
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

