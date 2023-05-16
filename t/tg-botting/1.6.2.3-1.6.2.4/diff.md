# Comparing `tmp/tg-botting-1.6.2.3.tar.gz` & `tmp/tg-botting-1.6.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-1.6.2.3.tar", last modified: Tue May 16 16:07:16 2023, max compression
+gzip compressed data, was "tg-botting-1.6.2.4.tar", last modified: Tue May 16 16:48:03 2023, max compression
```

## Comparing `tg-botting-1.6.2.3.tar` & `tg-botting-1.6.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 16:07:15.999858 tg-botting-1.6.2.3/
--rw-rw-rw-   0        0        0      920 2023-05-16 16:07:15.999858 tg-botting-1.6.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.6.2.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 16:07:15.999858 tg-botting-1.6.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1447 2023-05-16 16:06:41.000000 tg-botting-1.6.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 16:07:15.999858 tg-botting-1.6.2.3/tg_botting/
--rw-rw-rw-   0        0        0    29944 2023-05-16 16:06:41.000000 tg-botting-1.6.2.3/tg_botting/bot.py
--rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.6.2.3/tg_botting/cog.py
--rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.6.2.3/tg_botting/generals.py
--rw-rw-rw-   0        0        0    15742 2023-05-13 19:27:53.000000 tg-botting-1.6.2.3/tg_botting/objects.py
--rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.6.2.3/tg_botting/user_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 16:07:15.999858 tg-botting-1.6.2.3/tg_botting.egg-info/
--rw-rw-rw-   0        0        0      920 2023-05-16 16:07:15.000000 tg-botting-1.6.2.3/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-16 16:07:15.000000 tg-botting-1.6.2.3/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 16:07:15.000000 tg-botting-1.6.2.3/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-16 16:07:15.000000 tg-botting-1.6.2.3/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 16:07:15.000000 tg-botting-1.6.2.3/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 16:48:03.236124 tg-botting-1.6.2.4/
+-rw-rw-rw-   0        0        0      920 2023-05-16 16:48:03.236124 tg-botting-1.6.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.6.2.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-16 16:48:03.237122 tg-botting-1.6.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1447 2023-05-16 16:47:38.000000 tg-botting-1.6.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:48:03.229143 tg-botting-1.6.2.4/tg_botting/
+-rw-rw-rw-   0        0        0    30002 2023-05-16 16:47:38.000000 tg-botting-1.6.2.4/tg_botting/bot.py
+-rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.6.2.4/tg_botting/cog.py
+-rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.6.2.4/tg_botting/generals.py
+-rw-rw-rw-   0        0        0    15742 2023-05-13 19:27:53.000000 tg-botting-1.6.2.4/tg_botting/objects.py
+-rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.6.2.4/tg_botting/user_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:48:03.235127 tg-botting-1.6.2.4/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0      920 2023-05-16 16:48:03.000000 tg-botting-1.6.2.4/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-16 16:48:03.000000 tg-botting-1.6.2.4/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 16:48:03.000000 tg-botting-1.6.2.4/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-16 16:48:03.000000 tg-botting-1.6.2.4/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 16:48:03.000000 tg-botting-1.6.2.4/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-1.6.2.3/PKG-INFO` & `tg-botting-1.6.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.6.2.3
+Version: 1.6.2.4
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-1.6.2.3/README.md` & `tg-botting-1.6.2.4/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.3/setup.py` & `tg-botting-1.6.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.6.2.3'
+VERSION = '1.6.2.4'
 DESCRIPTION = 'python library for easy creation of a telegram bot.'
 LONG_DESCRIPTION = 'A package that allows you to create bots for telegram using its entire API.'
 
 setup(
     name="tg-botting",
     version=VERSION,
     url='https://github.com/2sweetheart2/tg_botting/tree/master',
```

### Comparing `tg-botting-1.6.2.3/tg_botting/bot.py` & `tg-botting-1.6.2.4/tg_botting/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,15 +654,15 @@
                 minus = 1
                 na = dict(need_args.parameters)
                 if 'self' in na.keys():
                     na.pop('self')
                 try:
                     na.pop(list(na.keys())[0])
                 except:
-                    pass
+                    print("ERROR: ",na,'\n','put_args: ',put_args,'\nargs: ',args)
                 for i in range(0,len(na)):
                     val = list(na.values())[i]
                     try:
                         if val.annotation != inspect.Parameter.empty:
                             if not isinstance(args[i-minus],val.annotation):
                                 return await self.tupe_error(message,args[i-minus],val.annotation)
                     except IndexError as e:
```

### Comparing `tg-botting-1.6.2.3/tg_botting/cog.py` & `tg-botting-1.6.2.4/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.3/tg_botting/generals.py` & `tg-botting-1.6.2.4/tg_botting/generals.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.3/tg_botting/objects.py` & `tg-botting-1.6.2.4/tg_botting/objects.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.3/tg_botting.egg-info/PKG-INFO` & `tg-botting-1.6.2.4/tg_botting.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.6.2.3
+Version: 1.6.2.4
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

