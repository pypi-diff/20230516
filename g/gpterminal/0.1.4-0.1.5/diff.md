# Comparing `tmp/gpterminal-0.1.4.tar.gz` & `tmp/gpterminal-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpterminal-0.1.4.tar", last modified: Tue May 16 09:05:11 2023, max compression
+gzip compressed data, was "gpterminal-0.1.5.tar", last modified: Tue May 16 09:15:08 2023, max compression
```

## Comparing `gpterminal-0.1.4.tar` & `gpterminal-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 09:05:11.540603 gpterminal-0.1.4/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 09:05:11.540154 gpterminal-0.1.4/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2148 2023-05-15 16:21:20.000000 gpterminal-0.1.4/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 09:05:11.534660 gpterminal-0.1.4/cli/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-16 08:04:08.000000 gpterminal-0.1.4/cli/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-16 03:14:58.000000 gpterminal-0.1.4/cli/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6906 2023-05-16 08:30:54.000000 gpterminal-0.1.4/cli/cli.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-15 15:21:27.000000 gpterminal-0.1.4/cli/code_execution.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-15 15:21:12.000000 gpterminal-0.1.4/cli/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 09:05:11.539492 gpterminal-0.1.4/gpterminal.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2902 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)      301 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       50 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       59 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-05-16 09:05:11.000000 gpterminal-0.1.4/gpterminal.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-16 09:05:11.540803 gpterminal-0.1.4/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1284 2023-05-16 09:00:53.000000 gpterminal-0.1.4/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 09:15:08.152998 gpterminal-0.1.5/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3243 2023-05-16 09:15:08.152078 gpterminal-0.1.5/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2489 2023-05-16 09:14:51.000000 gpterminal-0.1.5/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 09:15:08.145321 gpterminal-0.1.5/cli/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7902 2023-05-16 08:04:08.000000 gpterminal-0.1.5/cli/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-05-16 03:14:58.000000 gpterminal-0.1.5/cli/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6906 2023-05-16 08:30:54.000000 gpterminal-0.1.5/cli/cli.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8176 2023-05-15 15:21:27.000000 gpterminal-0.1.5/cli/code_execution.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-15 15:21:12.000000 gpterminal-0.1.5/cli/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-16 09:15:08.150712 gpterminal-0.1.5/gpterminal.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3243 2023-05-16 09:15:08.000000 gpterminal-0.1.5/gpterminal.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      301 2023-05-16 09:15:08.000000 gpterminal-0.1.5/gpterminal.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-16 09:15:08.000000 gpterminal-0.1.5/gpterminal.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       50 2023-05-16 09:15:08.000000 gpterminal-0.1.5/gpterminal.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       59 2023-05-16 09:15:08.000000 gpterminal-0.1.5/gpterminal.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        4 2023-05-16 09:15:08.000000 gpterminal-0.1.5/gpterminal.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-16 09:15:08.153205 gpterminal-0.1.5/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1284 2023-05-16 09:15:00.000000 gpterminal-0.1.5/setup.py
```

### Comparing `gpterminal-0.1.4/PKG-INFO` & `gpterminal-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterminal
-Version: 0.1.4
+Version: 0.1.5
 Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
 Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -28,20 +28,24 @@
 3.代码执行：执行命令并捕获错误输出及其上下文，提供智能解决方案。
 
 ## 安装
 
 确保安装 Python 3.6 或更高版本。然后运行：
 
 ```bash
-pip install GPTerminal
+pip install gpterminal
+
+或者
+
+pip install gpterminal -i https://pypi.org/simple/ 
 ```
 
 ## 使用
 
-在命令行中输入以下命令启动 GPTerminal：
+在命令行中输入以下命令启动 gpterminal
 
 ```bash
 gpterminal
 ```
 
 然后选择您想要使用的功能。
 
@@ -96,14 +100,20 @@
 
    请注意，将 `PythonXX` 替换为您的 Python 版本号，例如 `Python36` 或 `Python39`。
 
 2. 然后，关闭并重新打开命令提示符，或者注销并重新登录您的 Windows 帐户。
 
    现在，您应该能够在命令提示符中使用 `gpterminal` 命令了。
 
+
+## 问题
+1. 需要设置api_key(必填)以及base_url(可选)
+2. 需要 api_key 的也可以耐心等待，后续我会修改代码中获取 api_key 的方式，可以让大家直接使用
+3. 具体免费 api_key 的获取方式我还在开发中，后续会更新，敬请期待
+
 ## 贡献
 
 欢迎对 GPTerminal 进行贡献！请在提交 Pull Request 之前确保您的代码符合项目的质量标准。
 
 ## 许可
 
 GPTerminal 采用 MIT 许可证。有关详细信息，请参阅 [LICENSE](LICENSE) 文件。
```

### Comparing `gpterminal-0.1.4/README.md` & `gpterminal-0.1.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,20 +9,24 @@
 3.代码执行：执行命令并捕获错误输出及其上下文，提供智能解决方案。
 
 ## 安装
 
 确保安装 Python 3.6 或更高版本。然后运行：
 
 ```bash
-pip install GPTerminal
+pip install gpterminal
+
+或者
+
+pip install gpterminal -i https://pypi.org/simple/ 
 ```
 
 ## 使用
 
-在命令行中输入以下命令启动 GPTerminal：
+在命令行中输入以下命令启动 gpterminal
 
 ```bash
 gpterminal
 ```
 
 然后选择您想要使用的功能。
 
@@ -77,14 +81,20 @@
 
    请注意，将 `PythonXX` 替换为您的 Python 版本号，例如 `Python36` 或 `Python39`。
 
 2. 然后，关闭并重新打开命令提示符，或者注销并重新登录您的 Windows 帐户。
 
    现在，您应该能够在命令提示符中使用 `gpterminal` 命令了。
 
+
+## 问题
+1. 需要设置api_key(必填)以及base_url(可选)
+2. 需要 api_key 的也可以耐心等待，后续我会修改代码中获取 api_key 的方式，可以让大家直接使用
+3. 具体免费 api_key 的获取方式我还在开发中，后续会更新，敬请期待
+
 ## 贡献
 
 欢迎对 GPTerminal 进行贡献！请在提交 Pull Request 之前确保您的代码符合项目的质量标准。
 
 ## 许可
 
 GPTerminal 采用 MIT 许可证。有关详细信息，请参阅 [LICENSE](LICENSE) 文件。
```

### Comparing `gpterminal-0.1.4/cli/ChatGPT.py` & `gpterminal-0.1.5/cli/ChatGPT.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.4/cli/cli.py` & `gpterminal-0.1.5/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.4/cli/code_execution.py` & `gpterminal-0.1.5/cli/code_execution.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.4/cli/utils.py` & `gpterminal-0.1.5/cli/utils.py`

 * *Files identical despite different names*

### Comparing `gpterminal-0.1.4/gpterminal.egg-info/PKG-INFO` & `gpterminal-0.1.5/gpterminal.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpterminal
-Version: 0.1.4
+Version: 0.1.5
 Summary: A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands
 Home-page: https://github.com/yourusername/gpterminal
 Author: Your Name
 Author-email: your.email@example.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -28,20 +28,24 @@
 3.代码执行：执行命令并捕获错误输出及其上下文，提供智能解决方案。
 
 ## 安装
 
 确保安装 Python 3.6 或更高版本。然后运行：
 
 ```bash
-pip install GPTerminal
+pip install gpterminal
+
+或者
+
+pip install gpterminal -i https://pypi.org/simple/ 
 ```
 
 ## 使用
 
-在命令行中输入以下命令启动 GPTerminal：
+在命令行中输入以下命令启动 gpterminal
 
 ```bash
 gpterminal
 ```
 
 然后选择您想要使用的功能。
 
@@ -96,14 +100,20 @@
 
    请注意，将 `PythonXX` 替换为您的 Python 版本号，例如 `Python36` 或 `Python39`。
 
 2. 然后，关闭并重新打开命令提示符，或者注销并重新登录您的 Windows 帐户。
 
    现在，您应该能够在命令提示符中使用 `gpterminal` 命令了。
 
+
+## 问题
+1. 需要设置api_key(必填)以及base_url(可选)
+2. 需要 api_key 的也可以耐心等待，后续我会修改代码中获取 api_key 的方式，可以让大家直接使用
+3. 具体免费 api_key 的获取方式我还在开发中，后续会更新，敬请期待
+
 ## 贡献
 
 欢迎对 GPTerminal 进行贡献！请在提交 Pull Request 之前确保您的代码符合项目的质量标准。
 
 ## 许可
 
 GPTerminal 采用 MIT 许可证。有关详细信息，请参阅 [LICENSE](LICENSE) 文件。
```

### Comparing `gpterminal-0.1.4/setup.py` & `gpterminal-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gpterminal",
-    version="0.1.4",
+    version="0.1.5",
     author="Your Name",
     author_email="your.email@example.com",
     description="A CLI tool to interact with GPT-3/GPT-4, answer Git questions, and execute commands",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yourusername/gpterminal",
     packages=find_packages(),
```

