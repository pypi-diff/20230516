# Comparing `tmp/viewm2m-0.0.7.tar.gz` & `tmp/viewm2m-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viewm2m-0.0.7.tar", last modified: Tue May 16 14:43:50 2023, max compression
+gzip compressed data, was "viewm2m-0.0.8.tar", last modified: Tue May 16 14:49:34 2023, max compression
```

## Comparing `viewm2m-0.0.7.tar` & `viewm2m-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 14:43:50.674153 viewm2m-0.0.7/
--rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 14:43:50.674041 viewm2m-0.0.7/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-05-16 12:08:58.000000 viewm2m-0.0.7/README.md
--rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-05-16 14:43:50.674189 viewm2m-0.0.7/setup.cfg
--rw-r--r--   0 liufangjing   (501) staff       (20)     1924 2023-05-16 14:43:34.000000 viewm2m-0.0.7/setup.py
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 14:43:50.673057 viewm2m-0.0.7/viewm2m/
--rw-r--r--   0 liufangjing   (501) staff       (20)      459 2023-05-16 14:43:22.000000 viewm2m-0.0.7/viewm2m/__init__.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     6540 2023-05-16 14:11:57.000000 viewm2m-0.0.7/viewm2m/captor.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     6819 2023-05-16 13:43:11.000000 viewm2m-0.0.7/viewm2m/viewm2m.py
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 14:43:50.673904 viewm2m-0.0.7/viewm2m.egg-info/
--rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 14:43:50.000000 viewm2m-0.0.7/viewm2m.egg-info/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)      263 2023-05-16 14:43:50.000000 viewm2m-0.0.7/viewm2m.egg-info/SOURCES.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-05-16 14:43:50.000000 viewm2m-0.0.7/viewm2m.egg-info/dependency_links.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       50 2023-05-16 14:43:50.000000 viewm2m-0.0.7/viewm2m.egg-info/entry_points.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       29 2023-05-16 14:43:50.000000 viewm2m-0.0.7/viewm2m.egg-info/requires.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)        8 2023-05-16 14:43:50.000000 viewm2m-0.0.7/viewm2m.egg-info/top_level.txt
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 14:49:34.166954 viewm2m-0.0.8/
+-rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 14:49:34.166844 viewm2m-0.0.8/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-05-16 12:08:58.000000 viewm2m-0.0.8/README.md
+-rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-05-16 14:49:34.167035 viewm2m-0.0.8/setup.cfg
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1598 2023-05-16 14:49:24.000000 viewm2m-0.0.8/setup.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 14:49:34.165984 viewm2m-0.0.8/viewm2m/
+-rw-r--r--   0 liufangjing   (501) staff       (20)      491 2023-05-16 14:47:17.000000 viewm2m-0.0.8/viewm2m/__init__.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     6540 2023-05-16 14:11:57.000000 viewm2m-0.0.8/viewm2m/captor.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     7092 2023-05-16 14:48:48.000000 viewm2m-0.0.8/viewm2m/viewm2m.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 14:49:34.166712 viewm2m-0.0.8/viewm2m.egg-info/
+-rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 14:49:34.000000 viewm2m-0.0.8/viewm2m.egg-info/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)      263 2023-05-16 14:49:34.000000 viewm2m-0.0.8/viewm2m.egg-info/SOURCES.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-05-16 14:49:34.000000 viewm2m-0.0.8/viewm2m.egg-info/dependency_links.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       49 2023-05-16 14:49:34.000000 viewm2m-0.0.8/viewm2m.egg-info/entry_points.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       29 2023-05-16 14:49:34.000000 viewm2m-0.0.8/viewm2m.egg-info/requires.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)        8 2023-05-16 14:49:34.000000 viewm2m-0.0.8/viewm2m.egg-info/top_level.txt
```

### Comparing `viewm2m-0.0.7/setup.py` & `viewm2m-0.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="viewm2m",                                     # 包的分发名称，使用字母、数字、_、-
-    version="0.0.7",                                        # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    author="byte",                                       # 作者名字
-    author_email="liufangjing_byte@163.com",                      # 作者邮箱
-    description="用于捕获接口并转换为可导入metersphere平台的json格式",                            # 包的简介描述
-    long_description=long_description,                      # 包的详细介绍(一般通过加载README.md)
-    long_description_content_type="text/markdown",          # 和上条命令配合使用，声明加载的是markdown文件
-    url="https://github.com/zerobyte1o1/mitmproxy2metersphere",                              # 项目开源地址，我这里写的是同性交友官网，大家可以写自己真实的开源网址
-    packages=setuptools.find_packages(),                    # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
-    classifiers=[                                           # 关于包的其他元数据(metadata)
-        "Programming Language :: Python :: 3",              # 该软件包仅与Python3兼容
-        "License :: OSI Approved :: MIT License",           # 根据MIT许可证开源
-        "Operating System :: OS Independent",               # 与操作系统无关
+    name="viewm2m",  # 包的分发名称，使用字母、数字、_、-
+    version="0.0.8",  # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
+    author="byte",  # 作者名字
+    author_email="liufangjing_byte@163.com",  # 作者邮箱
+    description="用于捕获接口并转换为可导入metersphere平台的json格式",  # 包的简介描述
+    long_description=long_description,  # 包的详细介绍(一般通过加载README.md)
+    long_description_content_type="text/markdown",  # 和上条命令配合使用，声明加载的是markdown文件
+    url="https://github.com/zerobyte1o1/mitmproxy2metersphere",  # 项目开源地址，我这里写的是同性交友官网，大家可以写自己真实的开源网址
+    packages=setuptools.find_packages(),
+    # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
+    classifiers=[  # 关于包的其他元数据(metadata)
+        "Programming Language :: Python :: 3",  # 该软件包仅与Python3兼容
+        "License :: OSI Approved :: MIT License",  # 根据MIT许可证开源
+        "Operating System :: OS Independent",  # 与操作系统无关
     ],
-    install_requires=['mitmproxy==9.0.1','Kivy==2.1.0'],  # 依赖的包
+    install_requires=['mitmproxy==9.0.1', 'Kivy==2.1.0'],  # 依赖的包
     entry_points={
-              'console_scripts': [
-                  'viewm2m = viewm2m.__init__:main'
-              ]
-          },
+        'console_scripts': [
+            'viewm2m = viewm2m.viewm2m:main'
+        ]
+    },
     python_requires='>=3'
 )
```

### Comparing `viewm2m-0.0.7/viewm2m/captor.py` & `viewm2m-0.0.8/viewm2m/captor.py`

 * *Files identical despite different names*

### Comparing `viewm2m-0.0.7/viewm2m/viewm2m.py` & `viewm2m-0.0.8/viewm2m/viewm2m.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import platform
 import threading
+
+import click
 from kivy.clock import Clock
 from kivy.app import App
 from kivy.uix.boxlayout import BoxLayout
 from kivy.uix.textinput import TextInput
 from kivy.uix.button import Button
 from kivy.uix.togglebutton import ToggleButton
 import json
@@ -105,15 +107,14 @@
     )
     master.addons.add(Mitmproxy2Metersphere())
 
     await master.run()
     return master
 
 
-
 def run_asyncio_loop(loop):
     asyncio.set_event_loop(loop)
     loop.run_until_complete(start_proxy('127.0.0.1', 8083))
     loop.stop()
 
 
 class Middle:
@@ -185,9 +186,13 @@
     def toggle_record(self, instance):
         Middle.record = not Middle.record
 
     def update_label(self, instance):
         self.real_time_label.text = Middle.info_desk
 
 
-
-MyApp().run()
+@click.command(context_settings={"strict": True})
+@click.option('-r', '--repeat', default=False, type=click.BOOL, help='是否允许重复')
+@click.option('-p', '--port', default='8083', help='设置端口号')
+def main(repeat,port):
+    print(repeat,port)
+    MyApp().run()
```

