# Comparing `tmp/viewm2m-0.0.2.tar.gz` & `tmp/viewm2m-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viewm2m-0.0.2.tar", last modified: Tue May 16 13:21:29 2023, max compression
+gzip compressed data, was "viewm2m-0.0.3.tar", last modified: Tue May 16 13:58:28 2023, max compression
```

## Comparing `viewm2m-0.0.2.tar` & `viewm2m-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 13:21:29.731667 viewm2m-0.0.2/
--rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 13:21:29.731548 viewm2m-0.0.2/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-05-16 12:08:58.000000 viewm2m-0.0.2/README.md
--rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-05-16 13:21:29.731697 viewm2m-0.0.2/setup.cfg
--rw-r--r--   0 liufangjing   (501) staff       (20)     1923 2023-05-16 13:21:26.000000 viewm2m-0.0.2/setup.py
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 13:21:29.730551 viewm2m-0.0.2/viewm2m/
--rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-05-16 12:06:47.000000 viewm2m-0.0.2/viewm2m/__init__.py
--rw-r--r--   0 liufangjing   (501) staff       (20)     6835 2023-05-16 13:09:15.000000 viewm2m-0.0.2/viewm2m/viewm2m.py
-drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 13:21:29.731405 viewm2m-0.0.2/viewm2m.egg-info/
--rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 13:21:29.000000 viewm2m-0.0.2/viewm2m.egg-info/PKG-INFO
--rw-r--r--   0 liufangjing   (501) staff       (20)      245 2023-05-16 13:21:29.000000 viewm2m-0.0.2/viewm2m.egg-info/SOURCES.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-05-16 13:21:29.000000 viewm2m-0.0.2/viewm2m.egg-info/dependency_links.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       49 2023-05-16 13:21:29.000000 viewm2m-0.0.2/viewm2m.egg-info/entry_points.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)       29 2023-05-16 13:21:29.000000 viewm2m-0.0.2/viewm2m.egg-info/requires.txt
--rw-r--r--   0 liufangjing   (501) staff       (20)        8 2023-05-16 13:21:29.000000 viewm2m-0.0.2/viewm2m.egg-info/top_level.txt
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 13:58:28.740007 viewm2m-0.0.3/
+-rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 13:58:28.739884 viewm2m-0.0.3/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)        0 2023-05-16 12:08:58.000000 viewm2m-0.0.3/README.md
+-rw-r--r--   0 liufangjing   (501) staff       (20)       38 2023-05-16 13:58:28.740039 viewm2m-0.0.3/setup.cfg
+-rw-r--r--   0 liufangjing   (501) staff       (20)     1924 2023-05-16 13:45:20.000000 viewm2m-0.0.3/setup.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 13:58:28.738886 viewm2m-0.0.3/viewm2m/
+-rw-r--r--   0 liufangjing   (501) staff       (20)      367 2023-05-16 13:57:49.000000 viewm2m-0.0.3/viewm2m/__init__.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     6540 2023-05-16 13:46:54.000000 viewm2m-0.0.3/viewm2m/captor.py
+-rw-r--r--   0 liufangjing   (501) staff       (20)     6819 2023-05-16 13:43:11.000000 viewm2m-0.0.3/viewm2m/viewm2m.py
+drwxr-xr-x   0 liufangjing   (501) staff       (20)        0 2023-05-16 13:58:28.739731 viewm2m-0.0.3/viewm2m.egg-info/
+-rw-r--r--   0 liufangjing   (501) staff       (20)      453 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/PKG-INFO
+-rw-r--r--   0 liufangjing   (501) staff       (20)      263 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/SOURCES.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)        1 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/dependency_links.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       50 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/entry_points.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)       29 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/requires.txt
+-rw-r--r--   0 liufangjing   (501) staff       (20)        8 2023-05-16 13:58:28.000000 viewm2m-0.0.3/viewm2m.egg-info/top_level.txt
```

### Comparing `viewm2m-0.0.2/setup.py` & `viewm2m-0.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="viewm2m",                                     # 包的分发名称，使用字母、数字、_、-
-    version="0.0.2",                                        # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
+    version="0.0.3",                                        # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
     author="byte",                                       # 作者名字
     author_email="liufangjing_byte@163.com",                      # 作者邮箱
     description="用于捕获接口并转换为可导入metersphere平台的json格式",                            # 包的简介描述
     long_description=long_description,                      # 包的详细介绍(一般通过加载README.md)
     long_description_content_type="text/markdown",          # 和上条命令配合使用，声明加载的是markdown文件
     url="https://github.com/zerobyte1o1/mitmproxy2metersphere",                              # 项目开源地址，我这里写的是同性交友官网，大家可以写自己真实的开源网址
     packages=setuptools.find_packages(),                    # 如果项目由多个文件组成，我们可以使用find_packages()自动发现所有包和子包，而不是手动列出每个包，在这种情况下，包列表将是example_pkg
@@ -17,12 +17,12 @@
         "Programming Language :: Python :: 3",              # 该软件包仅与Python3兼容
         "License :: OSI Approved :: MIT License",           # 根据MIT许可证开源
         "Operating System :: OS Independent",               # 与操作系统无关
     ],
     install_requires=['mitmproxy==9.0.1','Kivy==2.1.0'],  # 依赖的包
     entry_points={
               'console_scripts': [
-                  'viewm2m = viewm2m.viewm2m:main'
+                  'viewm2m = viewm2m.__init__:main'
               ]
           },
     python_requires='>=3'
 )
```

### Comparing `viewm2m-0.0.2/viewm2m/viewm2m.py` & `viewm2m-0.0.3/viewm2m/viewm2m.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     )
     master.addons.add(Mitmproxy2Metersphere())
 
     await master.run()
     return master
 
 
-#
+
 def run_asyncio_loop(loop):
     asyncio.set_event_loop(loop)
     loop.run_until_complete(start_proxy('127.0.0.1', 8083))
     loop.stop()
 
 
 class Middle:
@@ -185,9 +185,9 @@
     def toggle_record(self, instance):
         Middle.record = not Middle.record
 
     def update_label(self, instance):
         self.real_time_label.text = Middle.info_desk
 
 
-def main():
-    MyApp().run()
+
+MyApp().run()
```

