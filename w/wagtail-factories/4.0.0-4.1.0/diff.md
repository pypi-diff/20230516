# Comparing `tmp/wagtail_factories-4.0.0.tar.gz` & `tmp/wagtail_factories-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_factories-4.0.0.tar", last modified: Fri Dec  2 14:32:26 2022, max compression
+gzip compressed data, was "dist/wagtail_factories-4.1.0.tar", last modified: Tue May 16 12:27:01 2023, max compression
```

## Comparing `wagtail_factories-4.0.0.tar` & `wagtail_factories-4.1.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxr-x   0 jmunn     (1001) jmunn     (1001)        0 2022-12-02 14:32:26.741201 wagtail_factories-4.0.0/
--rw-rw-r--   0 jmunn     (1001) jmunn     (1001)     1037 2022-11-28 10:53:37.000000 wagtail_factories-4.0.0/CHANGES
--rw-rw-r--   0 jmunn     (1001) jmunn     (1001)     1078 2022-06-09 08:11:43.000000 wagtail_factories-4.0.0/LICENSE
--rw-rw-r--   0 jmunn     (1001) jmunn     (1001)     6917 2022-12-02 14:32:26.741201 wagtail_factories-4.0.0/PKG-INFO
--rw-rw-r--   0 jmunn     (1001) jmunn     (1001)     6258 2022-11-19 11:18:17.000000 wagtail_factories-4.0.0/README.rst
--rw-rw-r--   0 jmunn     (1001) jmunn     (1001)       38 2022-12-02 14:32:26.741201 wagtail_factories-4.0.0/setup.cfg
--rwxrwxr-x   0 jmunn     (1001) jmunn     (1001)     2057 2022-12-02 14:26:38.000000 wagtail_factories-4.0.0/setup.py
-drwxrwxr-x   0 jmunn     (1001) jmunn     (1001)        0 2022-12-02 14:32:26.741201 wagtail_factories-4.0.0/src/
-drwxrwxr-x   0 jmunn     (1001) jmunn     (1001)        0 2022-12-02 14:32:26.741201 wagtail_factories-4.0.0/src/wagtail_factories/
--rw-rw-r--   0 jmunn     (1001) jmunn     (1001)       86 2022-12-02 14:26:38.000000 wagtail_factories-4.0.0/src/wagtail_factories/__init__.py
--rw-rw-r--   0 jmunn     (1001) jmunn     (1001)     7663 2022-12-02 14:23:52.000000 wagtail_factories-4.0.0/src/wagtail_factories/blocks.py
--rw-rw-r--   0 jmunn     (1001) jmunn     (1001)     6435 2022-11-19 11:18:17.000000 wagtail_factories-4.0.0/src/wagtail_factories/builder.py
--rw-rw-r--   0 jmunn     (1001) jmunn     (1001)     4398 2022-07-08 15:52:18.000000 wagtail_factories-4.0.0/src/wagtail_factories/factories.py
--rw-rw-r--   0 jmunn     (1001) jmunn     (1001)     1911 2022-11-19 11:18:17.000000 wagtail_factories-4.0.0/src/wagtail_factories/options.py
-drwxrwxr-x   0 jmunn     (1001) jmunn     (1001)        0 2022-12-02 14:32:26.741201 wagtail_factories-4.0.0/src/wagtail_factories.egg-info/
--rw-rw-r--   0 jmunn     (1001) jmunn     (1001)      202 2022-12-02 14:32:26.000000 wagtail_factories-4.0.0/src/wagtail_factories.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2102 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/src/wagtail_factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/src/wagtail_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/src/wagtail_factories/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/src/wagtail_factories/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/src/wagtail_factories/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-16 12:26:58.000000 wagtail_factories-4.1.0/src/wagtail_factories/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/src/wagtail_factories.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-16 12:27:01.000000 wagtail_factories-4.1.0/src/wagtail_factories.egg-info/SOURCES.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `wagtail_factories-4.0.0/CHANGES` & `wagtail_factories-4.1.0/CHANGES`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 Unreleased
 ==========
+
+4.1.0
+=====
+- Add support Wagtail 5.0
+- Drop support for Wagtail < 4.1
+
+4.0.0
+=====
+- Fix ListBlock compatibility with Wagtail 4.1
 - Add support for Wagtail 4.0 
 
 3.1.0
 =====
 - Add PageChooserBlock and DocumentChooserBlock
 
 3.0.0
```

### Comparing `wagtail_factories-4.0.0/PKG-INFO` & `wagtail_factories-4.1.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,29 @@
-Metadata-Version: 2.1
-Name: wagtail_factories
-Version: 4.0.0
-Summary: Factory boy classes for wagtail
-Home-page: https://github.com/wagtail/wagtail-factories/
-Author: Michael van Tellingen
-Author-email: michaelvantellingen@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
-Classifier: Framework :: Wagtail
-Classifier: Framework :: Wagtail :: 2
-Classifier: Framework :: Wagtail :: 3
-Classifier: Framework :: Wagtail :: 4
-Provides-Extra: docs
-Provides-Extra: test
-License-File: LICENSE
-
 =================
 wagtail-factories
 =================
 
 Factory boy classes for Wagtail CMS
 
+.. start-no-pypi
+
+Status
+------
+
+.. image:: https://readthedocs.org/projects/wagtail-factories/badge/?version=latest
+    :target: https://readthedocs.org/projects/wagtail-factories/
+
+.. image:: https://github.com/wagtail/wagtail-factories/workflows/Python%20Tests/badge.svg
+    :target: https://github.com/wagtail/wagtail-factories/actions?query=workflow%3A%22Python+Tests%22
 
+.. image:: https://img.shields.io/pypi/v/wagtail-factories.svg
+    :target: https://pypi.python.org/pypi/wagtail-factories/
+
+
+.. end-no-pypi
 
 
 
 Installation
 ============
 
 .. code-block:: shell
@@ -200,9 +184,7 @@
         )
 
         class Meta:
             model = models.MyTestPage
 
 
 This requirement does *not* apply to ``ListBlockFactory``, which is a subclass of ``SubFactory``.
-
-
```

### Comparing `wagtail_factories-4.0.0/README.rst` & `wagtail_factories-4.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,190 +1,206 @@
-=================
-wagtail-factories
-=================
-
-Factory boy classes for Wagtail CMS
-
-.. start-no-pypi
-
-Status
-------
-
-.. image:: https://readthedocs.org/projects/wagtail-factories/badge/?version=latest
-    :target: https://readthedocs.org/projects/wagtail-factories/
-
-.. image:: https://github.com/wagtail/wagtail-factories/workflows/Python%20Tests/badge.svg
-    :target: https://github.com/wagtail/wagtail-factories/actions?query=workflow%3A%22Python+Tests%22
-
-.. image:: https://img.shields.io/pypi/v/wagtail-factories.svg
-    :target: https://pypi.python.org/pypi/wagtail-factories/
-
-
-.. end-no-pypi
-
-
-
-Installation
-============
-
-.. code-block:: shell
-
-   pip install wagtail-factories
-
-
-
-Usage
-=====
-
-Documentation is still in progress, but see the `tests`_ for more examples.
-
-.. _tests: https://github.com/wagtail/wagtail-factories/tree/main/tests
-
-.. code-block:: python
-
-    import wagtail_factories
-    from . import models
-
-
-    class MyCarouselItemFactory(wagtail_factories.StructBlockFactory):
-        label = 'my-label'
-        image = factory.SubFactory(
-            wagtail_factories.ImageChooserBlockFactory)
-
-        class Meta:
-            model = models.MyBlockItem
-
-
-    class MyCarouselFactory(wagtail_factories.StructBlockFactory):
-        title = "Carousel title"
-        items = wagtail_factories.ListBlockFactory(
-            MyCarouselItemFactory)
-
-        class Meta:
-            model = models.MyCarousel
-
-
-    class MyNewsPageFactory(wagtail_factories.PageFactory):
-        class Meta:
-            model = models.MyNewsPage
-
-
-    class MyNewsPageChooserBlockFactory(wagtail_factories.PageChooserBlockFactory):
-        page = factory.SubFactory(MyNewsPageFactory)
-
-
-    class MyTestPageFactory(wagtail_factories.PageFactory):
-        body = wagtail_factories.StreamFieldFactory({
-            'carousel': factory.SubFactory(MyCarouselFactory),
-            'news_page': factory.SubFactory(MyNewsPageChooserBlockFactory),
-        })
-
-        class Meta:
-            model = models.MyTestPage
-
-
-    def test_my_page():
-        root_page = wagtail_factories.PageFactory(parent=None)
-        my_page = MyTestPageFactory(
-            parent=root_page,
-            body__0__carousel__items__0__label='Slide 1',
-            body__0__carousel__items__0__image__image__title='Image Slide 1',
-            body__0__carousel__items__1__label='Slide 2',
-            body__0__carousel__items__1__image__image__title='Image Slide 2',
-            body__0__carousel__items__2__label='Slide 3',
-            body__0__carousel__items__2__image__image__title='Image Slide 3',
-            body__1__news_page__page__title="News",
-        )
-
-
-Using StreamBlockFactory
-========================
-
-``StreamBlockFactory`` can be used in conjunction with the other block factory types to create complex, nested ``StreamValues``, much like how ``StreamBlock`` can be used to declare the blocks for a complex ``StreamField``.
-
-First, define your ``StreamBlockFactory`` subclass, using ``factory.SubFactory`` to wrap child block declarations. Be sure to include your ``StreamBlock`` subclass as the model attribute on the inner ``Meta`` class.
-
-.. code-block:: python
-
-    class MyStreamBlockFactory(wagtail_factories.StreamBlockFactory):
-        my_struct_block = factory.SubFactory(MyStructBlockFactory)
-
-        class Meta:
-            model = MyStreamBlock
-
-
-Then include your ``StreamBlockFactory`` subclass on a model factory as the argument to a ``StreamFieldFactory``.
-
-.. code-block:: python
-
-    class MyPageFactory(wagtail_factories.PageFactory):
-        body = wagtail_factories.StreamFieldFactory(MyStreamBlockFactory)
-
-        class Meta:
-            model = MyPage
-
-
-You can then use a modified version of factory_boy's deep object declaration syntax to build up ``StreamValues`` on the fly.
-
-.. code-block:: python
-
-    MyPageFactory(
-        body__0__my_struct_block__some_field="some value",
-        body__0__my_struct_block__some_other_field="some other value",
-    )
-
-
-To generate the default value for a block factory, terminate your declaration at the index and provide the block name as the value.
-
-.. code-block:: python
-
-    MyPageFactory(body__0="my_struct_block")
-
-
-Alternative StreamFieldFactory declaration syntax
-=================================================
-
-Prior to version 3.0, ``StreamFieldFactory`` could only be used by providing a dict mapping block names to block factory classes as the single argument, for example:
-
-.. code-block:: python
-
-    class MyTestPageWithStreamFieldFactory(wagtail_factories.PageFactory):
-        body = wagtail_factories.StreamFieldFactory(
-            {
-                "char_array": wagtail_factories.ListBlockFactory(
-                    wagtail_factories.CharBlockFactory
-                ),
-                "int_array": wagtail_factories.ListBlockFactory(
-                    wagtail_factories.IntegerBlockFactory
-                ),
-                "struct": MyBlockFactory,
-                "image": wagtail_factories.ImageChooserBlockFactory,
-            }
-        )
-    
-        class Meta:
-            model = models.MyTestPage
-    
-
-This style of declaration is still supported, with the caveat that nested stream blocks are not supported for this approach. From version 3.0, all ``BlockFactory`` values in a ``StreamFieldFactory`` definition of this style *must* be wrapped in factory_boy ``SubFactories``. For example, the above example must be updated to the following for 3.0 compatibility.
-
-.. code-block:: python
-
-    class MyTestPageWithStreamFieldFactory(wagtail_factories.PageFactory):
-        body = wagtail_factories.StreamFieldFactory(
-            {
-                "char_array": wagtail_factories.ListBlockFactory(
-                    wagtail_factories.CharBlockFactory
-                ),
-                "int_array": wagtail_factories.ListBlockFactory(
-                    wagtail_factories.IntegerBlockFactory
-                ),
-                "struct": factory.SubFactory(MyBlockFactory),
-                "image": factory.SubFactory(wagtail_factories.ImageChooserBlockFactory),
-            }
-        )
-
-        class Meta:
-            model = models.MyTestPage
-
-
-This requirement does *not* apply to ``ListBlockFactory``, which is a subclass of ``SubFactory``.
+Metadata-Version: 2.1
+Name: wagtail_factories
+Version: 4.1.0
+Summary: Factory boy classes for wagtail
+Home-page: https://github.com/wagtail/wagtail-factories/
+Author: Michael van Tellingen
+Author-email: michaelvantellingen@gmail.com
+License: MIT
+Description: =================
+        wagtail-factories
+        =================
+        
+        Factory boy classes for Wagtail CMS
+        
+        
+        
+        
+        
+        Installation
+        ============
+        
+        .. code-block:: shell
+        
+           pip install wagtail-factories
+        
+        
+        
+        Usage
+        =====
+        
+        Documentation is still in progress, but see the `tests`_ for more examples.
+        
+        .. _tests: https://github.com/wagtail/wagtail-factories/tree/main/tests
+        
+        .. code-block:: python
+        
+            import wagtail_factories
+            from . import models
+        
+        
+            class MyCarouselItemFactory(wagtail_factories.StructBlockFactory):
+                label = 'my-label'
+                image = factory.SubFactory(
+                    wagtail_factories.ImageChooserBlockFactory)
+        
+                class Meta:
+                    model = models.MyBlockItem
+        
+        
+            class MyCarouselFactory(wagtail_factories.StructBlockFactory):
+                title = "Carousel title"
+                items = wagtail_factories.ListBlockFactory(
+                    MyCarouselItemFactory)
+        
+                class Meta:
+                    model = models.MyCarousel
+        
+        
+            class MyNewsPageFactory(wagtail_factories.PageFactory):
+                class Meta:
+                    model = models.MyNewsPage
+        
+        
+            class MyNewsPageChooserBlockFactory(wagtail_factories.PageChooserBlockFactory):
+                page = factory.SubFactory(MyNewsPageFactory)
+        
+        
+            class MyTestPageFactory(wagtail_factories.PageFactory):
+                body = wagtail_factories.StreamFieldFactory({
+                    'carousel': factory.SubFactory(MyCarouselFactory),
+                    'news_page': factory.SubFactory(MyNewsPageChooserBlockFactory),
+                })
+        
+                class Meta:
+                    model = models.MyTestPage
+        
+        
+            def test_my_page():
+                root_page = wagtail_factories.PageFactory(parent=None)
+                my_page = MyTestPageFactory(
+                    parent=root_page,
+                    body__0__carousel__items__0__label='Slide 1',
+                    body__0__carousel__items__0__image__image__title='Image Slide 1',
+                    body__0__carousel__items__1__label='Slide 2',
+                    body__0__carousel__items__1__image__image__title='Image Slide 2',
+                    body__0__carousel__items__2__label='Slide 3',
+                    body__0__carousel__items__2__image__image__title='Image Slide 3',
+                    body__1__news_page__page__title="News",
+                )
+        
+        
+        Using StreamBlockFactory
+        ========================
+        
+        ``StreamBlockFactory`` can be used in conjunction with the other block factory types to create complex, nested ``StreamValues``, much like how ``StreamBlock`` can be used to declare the blocks for a complex ``StreamField``.
+        
+        First, define your ``StreamBlockFactory`` subclass, using ``factory.SubFactory`` to wrap child block declarations. Be sure to include your ``StreamBlock`` subclass as the model attribute on the inner ``Meta`` class.
+        
+        .. code-block:: python
+        
+            class MyStreamBlockFactory(wagtail_factories.StreamBlockFactory):
+                my_struct_block = factory.SubFactory(MyStructBlockFactory)
+        
+                class Meta:
+                    model = MyStreamBlock
+        
+        
+        Then include your ``StreamBlockFactory`` subclass on a model factory as the argument to a ``StreamFieldFactory``.
+        
+        .. code-block:: python
+        
+            class MyPageFactory(wagtail_factories.PageFactory):
+                body = wagtail_factories.StreamFieldFactory(MyStreamBlockFactory)
+        
+                class Meta:
+                    model = MyPage
+        
+        
+        You can then use a modified version of factory_boy's deep object declaration syntax to build up ``StreamValues`` on the fly.
+        
+        .. code-block:: python
+        
+            MyPageFactory(
+                body__0__my_struct_block__some_field="some value",
+                body__0__my_struct_block__some_other_field="some other value",
+            )
+        
+        
+        To generate the default value for a block factory, terminate your declaration at the index and provide the block name as the value.
+        
+        .. code-block:: python
+        
+            MyPageFactory(body__0="my_struct_block")
+        
+        
+        Alternative StreamFieldFactory declaration syntax
+        =================================================
+        
+        Prior to version 3.0, ``StreamFieldFactory`` could only be used by providing a dict mapping block names to block factory classes as the single argument, for example:
+        
+        .. code-block:: python
+        
+            class MyTestPageWithStreamFieldFactory(wagtail_factories.PageFactory):
+                body = wagtail_factories.StreamFieldFactory(
+                    {
+                        "char_array": wagtail_factories.ListBlockFactory(
+                            wagtail_factories.CharBlockFactory
+                        ),
+                        "int_array": wagtail_factories.ListBlockFactory(
+                            wagtail_factories.IntegerBlockFactory
+                        ),
+                        "struct": MyBlockFactory,
+                        "image": wagtail_factories.ImageChooserBlockFactory,
+                    }
+                )
+            
+                class Meta:
+                    model = models.MyTestPage
+            
+        
+        This style of declaration is still supported, with the caveat that nested stream blocks are not supported for this approach. From version 3.0, all ``BlockFactory`` values in a ``StreamFieldFactory`` definition of this style *must* be wrapped in factory_boy ``SubFactories``. For example, the above example must be updated to the following for 3.0 compatibility.
+        
+        .. code-block:: python
+        
+            class MyTestPageWithStreamFieldFactory(wagtail_factories.PageFactory):
+                body = wagtail_factories.StreamFieldFactory(
+                    {
+                        "char_array": wagtail_factories.ListBlockFactory(
+                            wagtail_factories.CharBlockFactory
+                        ),
+                        "int_array": wagtail_factories.ListBlockFactory(
+                            wagtail_factories.IntegerBlockFactory
+                        ),
+                        "struct": factory.SubFactory(MyBlockFactory),
+                        "image": factory.SubFactory(wagtail_factories.ImageChooserBlockFactory),
+                    }
+                )
+        
+                class Meta:
+                    model = models.MyTestPage
+        
+        
+        This requirement does *not* apply to ``ListBlockFactory``, which is a subclass of ``SubFactory``.
+        
+Platform: UNKNOWN
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Wagtail
+Classifier: Framework :: Wagtail :: 4
+Classifier: Framework :: Wagtail :: 5
+Provides-Extra: docs
+Provides-Extra: test
```

### Comparing `wagtail_factories-4.0.0/setup.py` & `wagtail_factories-4.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 
 from setuptools import find_packages, setup
 
 install_requires = [
     "factory-boy>=3.2",
-    "wagtail>=2.15,<5.0",
+    "wagtail>=4.1",
 ]
 
 docs_require = [
     "sphinx>=1.4.0",
 ]
 
 tests_require = [
@@ -27,15 +27,15 @@
 with open("README.rst") as fh:
     long_description = re.sub(
         "^.. start-no-pypi.*^.. end-no-pypi", "", fh.read(), flags=re.M | re.S
     )
 
 setup(
     name="wagtail_factories",
-    version="4.0.0",
+    version="4.1.0",
     description="Factory boy classes for wagtail",
     long_description=long_description,
     author="Michael van Tellingen",
     author_email="michaelvantellingen@gmail.com",
     url="https://github.com/wagtail/wagtail-factories/",
     install_requires=install_requires,
     tests_require=tests_require,
@@ -54,19 +54,20 @@
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Framework :: Django",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4.0",
+        "Framework :: Django :: 4.1",
         "Framework :: Wagtail",
-        "Framework :: Wagtail :: 2",
-        "Framework :: Wagtail :: 3",
         "Framework :: Wagtail :: 4",
+        "Framework :: Wagtail :: 5",
     ],
     zip_safe=False,
 )
```

### Comparing `wagtail_factories-4.0.0/src/wagtail_factories/blocks.py` & `wagtail_factories-4.1.0/src/wagtail_factories/blocks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 from collections import defaultdict
 
 import factory
 from factory.declarations import ParameteredAttribute
-from wagtail import VERSION as wagtail_version
+from wagtail import blocks
 from wagtail.documents.blocks import DocumentChooserBlock
 from wagtail.images.blocks import ImageChooserBlock
 
-if wagtail_version >= (3, 0):
-    from wagtail import blocks
-else:
-    from wagtail.core import blocks
-
 from wagtail_factories.builder import (
     ListBlockStepBuilder,
     StreamBlockStepBuilder,
     StructBlockStepBuilder,
 )
 from wagtail_factories.factories import DocumentFactory, ImageFactory, PageFactory
 from wagtail_factories.options import BlockFactoryOptions, StreamBlockFactoryOptions
@@ -133,19 +128,16 @@
         subfactory = self.get_factory()
         force_sequence = step.sequence if self.FORCE_SEQUENCE else None
         values = [
             step.recurse(subfactory, params, force_sequence=force_sequence)
             for _, params in sorted(result.items())
         ]
 
-        if wagtail_version >= (2, 16):
-            list_block_def = blocks.list_block.ListBlock(subfactory._meta.model())
-            return blocks.list_block.ListValue(list_block_def, values)
-        else:
-            return values
+        list_block_def = blocks.list_block.ListBlock(subfactory._meta.model())
+        return blocks.list_block.ListValue(list_block_def, values)
 
 
 class StructBlockFactory(factory.Factory):
     _options_class = BlockFactoryOptions
     _builder_class = StructBlockStepBuilder
 
     class Meta:
```

### Comparing `wagtail_factories-4.0.0/src/wagtail_factories/builder.py` & `wagtail_factories-4.1.0/src/wagtail_factories/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from itertools import zip_longest
 
 from factory import SubFactory
 from factory.builder import StepBuilder
-
-try:
-    from wagtail import blocks
-except ImportError:
-    # Wagtail<3.0
-    from wagtail.core import blocks
+from wagtail import blocks
 
 
 class StreamFieldFactoryException(Exception):
     pass
 
 
 class InvalidDeclaration(StreamFieldFactoryException):
```

### Comparing `wagtail_factories-4.0.0/src/wagtail_factories/factories.py` & `wagtail_factories-4.1.0/src/wagtail_factories/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 import logging
 
 import factory
 from django.utils.text import slugify
 from factory import errors, utils
 from factory.declarations import ParameteredAttribute
-from wagtail.images import get_image_model
-
-try:
-    from wagtail.models import Collection, Page, Site
-except ImportError:
-    # Wagtail<3.0
-    from wagtail.core.models import Collection, Page, Site
-
 from factory.django import DjangoModelFactory
 from wagtail.documents import get_document_model
+from wagtail.images import get_image_model
+from wagtail.models import Collection, Page, Site
 
 __all__ = [
     "CollectionFactory",
     "ImageFactory",
     "PageFactory",
     "SiteFactory",
     "DocumentFactory",
```

### Comparing `wagtail_factories-4.0.0/src/wagtail_factories/options.py` & `wagtail_factories-4.1.0/src/wagtail_factories/options.py`

 * *Files identical despite different names*

