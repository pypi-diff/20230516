# Comparing `tmp/malbench-0.3.5.tar.gz` & `tmp/malbench-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malbench-0.3.5.tar", max compression
+gzip compressed data, was "malbench-0.4.0.tar", max compression
```

## Comparing `malbench-0.3.5.tar` & `malbench-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      545 2023-04-13 19:49:08.177178 malbench-0.3.5/data/banner.txt
--rw-r--r--   0        0        0   526052 2023-05-02 19:55:33.359376 malbench-0.3.5/data/demo.gif
--rw-r--r--   0        0        0      567 2023-05-01 23:24:48.296033 malbench-0.3.5/data/disclaimer.txt
--rw-r--r--   0        0        0        5 2023-05-03 14:14:35.545760 malbench-0.3.5/data/version.txt
--rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.3.5/LICENSE
--rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.3.5/malbench/__init__.py
--rw-r--r--   0        0        0     3000 2023-05-02 19:13:53.949742 malbench-0.3.5/malbench/__main__.py
--rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.3.5/malbench/args.py
--rw-r--r--   0        0        0     4924 2023-05-02 13:19:11.884051 malbench-0.3.5/malbench/malware.py
--rw-r--r--   0        0        0     8362 2023-05-02 19:13:53.949742 malbench-0.3.5/malbench/message.py
--rw-r--r--   0        0        0      435 2023-04-21 13:20:47.394154 malbench-0.3.5/malbench/version.py
--rw-r--r--   0        0        0      893 2023-05-03 14:14:45.691965 malbench-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     8101 2023-05-03 14:13:03.886711 malbench-0.3.5/README.md
--rw-r--r--   0        0        0     8898 1970-01-01 00:00:00.000000 malbench-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.4.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.4.0/malbench/__init__.py
+-rw-r--r--   0        0        0     3000 2023-05-02 19:13:53.949742 malbench-0.4.0/malbench/__main__.py
+-rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.4.0/malbench/args.py
+-rw-r--r--   0        0        0     6780 2023-05-15 02:55:05.437319 malbench-0.4.0/malbench/celebrations.py
+-rw-r--r--   0        0        0      545 2023-05-03 20:58:37.976822 malbench-0.4.0/malbench/data/banner.txt
+-rw-r--r--   0        0        0      567 2023-05-03 20:58:37.977821 malbench-0.4.0/malbench/data/disclaimer.txt
+-rw-r--r--   0        0        0        5 2023-05-16 03:00:05.762021 malbench-0.4.0/malbench/data/version.txt
+-rw-r--r--   0        0        0     5085 2023-05-16 02:57:51.049649 malbench-0.4.0/malbench/malware.py
+-rw-r--r--   0        0        0    12072 2023-05-16 02:57:51.050649 malbench-0.4.0/malbench/message.py
+-rw-r--r--   0        0        0      327 2023-05-08 02:07:22.949742 malbench-0.4.0/malbench/platform.py
+-rw-r--r--   0        0        0      432 2023-05-03 20:58:37.979815 malbench-0.4.0/malbench/version.py
+-rw-r--r--   0        0        0     1183 2023-05-16 02:59:58.088322 malbench-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6232 2023-05-08 02:07:22.941260 malbench-0.4.0/README.md
+-rw-r--r--   0        0        0     6917 1970-01-01 00:00:00.000000 malbench-0.4.0/PKG-INFO
```

### Comparing `malbench-0.3.5/data/banner.txt` & `malbench-0.4.0/malbench/data/banner.txt`

 * *Files identical despite different names*

### Comparing `malbench-0.3.5/data/disclaimer.txt` & `malbench-0.4.0/malbench/data/disclaimer.txt`

 * *Files identical despite different names*

### Comparing `malbench-0.3.5/LICENSE` & `malbench-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `malbench-0.3.5/malbench/__main__.py` & `malbench-0.4.0/malbench/__main__.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.5/malbench/args.py` & `malbench-0.4.0/malbench/args.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.5/malbench/malware.py` & `malbench-0.4.0/malbench/malware.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import subprocess
 import time
 import os
+from malbench import platform
 from typing import List, Optional
 
 
 class MalwareLauncher:
     """
     Class to launch malware executables.
 
@@ -49,19 +50,20 @@
         The method launches the malware executable specified by the `filepath` attribute and waits for it to complete,
         with a timeout specified by the `timeout` attribute.
 
         Returns:
             bool: `True` if the malware was detected, `False` if it went undetected.
         """
 
-        if os.name == "nt":
-            process = subprocess.Popen(self.filepath, creationflags=subprocess.CREATE_NEW_PROCESS_GROUP |
-                                       subprocess.CREATE_BREAKAWAY_FROM_JOB)
-        else:
-            process = subprocess.Popen(self.filepath)
+        with open(os.devnull, 'w') as devnull:
+            try:
+                process = subprocess.Popen(self.filepath, creationflags=platform.CREATE_NEW_PROCESS_GROUP |
+                                           platform.CREATE_BREAKAWAY_FROM_JOB, stdout=devnull, stderr=devnull)
+            except AttributeError:
+                process = subprocess.Popen(self.filepath, stdout=devnull, stderr=devnull)
 
         timestamp = time.monotonic()
         while process.poll() is None:
             # If process is running for more than two seconds, kill the process and mark it as detected.
             if time.monotonic() - timestamp >= self.timeout:
                 process.kill()
```

### Comparing `malbench-0.3.5/README.md` & `malbench-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,97 @@
-# Malbench
-Malbench is a command-line tool for testing and evaluating the effectiveness of malware detection tools (such as antivirus solutions). It does this by running a set of malware samples, and checking if the malware is flagged by the detection tool we are evaluating. Malbench is built to be modular and configurable, so it can be customized to meet the specific needs of different users and environments.
-![Malbench Terminal Demo](https://i.imgur.com/oGQNU8i.gif)
-
-## About
-### Disclaimer 
-**⚠ WARNING**: Malbench is a tool for testing antivirus software against real-world malware samples. While it does not contain any malware on its own, it is designed to run malware samples provided by the user. Use Malbench only in secure and isolated environments that you are authorized in doing so. Do **not** use Malbench on a computer or network that contains sensitive information or data that you are not willing to lose and/or become compromised. By using Malbench, you acknowledge the risks and assume full responsibility for any damages that may result.
-
-**ℹ️ NOTE**: As stated above: *Malbench does not come with any malicious code installed*. It is the user's responsibility to provide their own samples for testing purposes. This is to ensure that Malbench is used responsibly and ethically, and that users have control over the types of malware being tested.
-
-### Why Use Malbench
-Malware detection tools are an essential component of any computer security strategy, but they are not foolproof. New techniques and methods are constantly being developed to evade detection. It is important to regularly test and evaluate the effectiveness of detection tools to ensure that we are keeping up with these evolving threats.
-
-With all the different features and algorithms of modern antivirus solutions, it can be hard to find practical and objective results on what-all they defend against. Malbench can be leveraged to bulk-test known malware samples against antivirus solutions to deliver real and practical results. This is done by automatically launching multiple malware payloads on a system and seeing what samples are detected and which ones were evaded. With Malbench, users can customize their testing to meet their specific needs, selecting the malware samples they want to run, and the duration of a test.
-
-### How Antivirus is Benchmarked
-Malbench launches each malware sample selected by the user and monitors its execution. If the sample completes without error, it is flagged as `UNDETECTED`. If the sample is terminated with an error code, it is flagged as `DETECTED`, indicating that it was killed by the antivirus solution. If the sample is still running after a designated time (defaults to 2 seconds), Malbench forcibly kills the program and flags it as `UNDETECTED`, as the antivirus solution did not detect it in time.
-
-After each sample is run, Malbench displays the detection rate. The detection rate is a percentage representing the amount of samples the antivirus successfully defended against. 
-
-$$
-\text{Detection rate} = \frac{\text{Number of samples flagged as detected}}{\text{Total number of samples}} \times 100\%
-$$
-
-## Installation
-There are two ways to install Malbench, depending on whether you are a user or a developer.
-
-### For Users
-To install Malbench for general use, follow these simple steps:
-
-1.  Ensure that the following is installed on your system: [Python 3.8.1+](https://www.python.org/downloads/), and [PIP](https://pypi.org/project/pip/) (included with most Python installations).
-2.  Install Malbench via pip by running the following command:
-    ```bash
-    pip install malbench
-    ```
-
-### For Developers
-If you are a developer who wants to contribute to Malbench or modify the source code, you will need to follow a different set of installation steps: 
-
-1.  Ensure the following is installed on your system: [Python 3.8.1+](https://www.python.org/downloads/), [PIP](https://pypi.org/project/pip/) (included with most Python installations), [Git](https://git-scm.com/downloads), [Poetry](https://python-poetry.org/docs/), and an IDE of your choice ([VSCode](https://code.visualstudio.com/download) recommended).
-2.  Clone (or fork) the Malbench repository using Git:
-    ```bash
-    git clone https://github.com/youkergav/Malbench.git
-    ```
-3.  Navigate to the project directory:
-    ```bash
-    cd malbench
-    ```
-4.  Install the required dependencies using Poetry:
-    ```bash
-    poetry install
-    ```
-    *Note: Please ensure the your PATH is configured for poetry*
-5. Launch the virtual environment using one of the following methods:
-    - For general use, the virtual environment can be opened with:
-      ```
-      poetry shell
-      ```
-    - Alternatively, the virtual environment can be opened in VSCode. First ensure the [Python extension for VSCode](https://marketplace.visualstudio.com/items?itemName=ms-python.python) is installed. Then, open the `Malbench` folder in VSCode and ensure the Python interpreter is set to use the local poetry `.venv` (you may need to reload VSCode after this).
-
-## Usage
-To use Malbench, simply run the following command inside your virtual environment:
-```bash
-python -m malbench /path/to/malware
-```
-
-Replace `/path/to/malware` with your `path` argument. The `path` argument should be the path to the malware samples you want to test. This can be either a single file or a folder containing multiple files. Only executable files will be ran by Malbench.
-
-By default, Malbench will show a banner when it starts, and will prompt you to confirm that you understand the risks involved before running the malware samples. You can disable the banner using the `--no-banner` flag, and disable the confirmation prompt using the `--no-warning` flag (as seen in the demo).
-
-Malware samples are run one by one, and Malbench will wait for each sample to be stopped by the detection software or reach the specified 2 second timeout before moving on to the next sample. This timeout can be changed with the `--timeout` flag. If a sample completes successfully, Malbench will print a red message with a `[-]` prefix, indicating it wasn't stopped by the detection software. If a sample has to be forcibly terminated by the detection software, Malbench will print a green message with a `[+]` prefix, indicating is was successfully detected and stopped.
-
-A full list of arguments to use with Malbench are below. This can be displayed with `--help`.
-```bash
-usage: malbench [-h] [-v] [-t TIMEOUT] [-nB] [-nW] [-d] path
-
-positional arguments:
-  path                  file or folder path of malware executables
-
-options:
-  -h, --help            show this help message and exit
-  -v, --version         shows malbench version number and exits
-  -t TIMEOUT, --timeout TIMEOUT
-                        malware TTL before being marked as failure (2 default)
-  -nC, --no-color       disables colored output
-  -nB, --no-banner      hides the banner logo
-  -nW, --no-warning     bypasses user confirmation before running
-  -d, --dev             enables stack tracing
-```
-
-## Contributing
-Contributions to Malbench are always welcome! If you'd like to contribute, please fork the repository and create a new branch for your changes. Once you've made your changes, create a pull request and we'll review your changes. *For major changes, please open an issue first to discuss what you would like to change.*
-
-Pull Request Checklist:
-- New code follows similar coding styles of the existing codebase.
-- New code is backed up by unit tests, with a minimum of 70% coverage.
-- New code passes all linting and strict-typing rules.
-- New code is well documented with docstrings and compiled in `/docs`.
-- Updates are made to the README when applicable.
-
-## License
-This project is licensed under the [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.en.html). See the [LICENSE.md](./LICENSE.md) file for details.
-
-## Credits
-Malbench was created by [Gavin Youker](mailto:youkergav@gmail.com).
+Metadata-Version: 2.1
+Name: malbench
+Version: 0.4.0
+Summary: A tool used to benchmark antivirus solutions against real-world malware samples.
+Home-page: https://github.com/youkergav/Malbench
+License: GPL-3.0-only
+Author: Gavin Youker
+Author-email: youkergav@gmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: colorama (>=0.4.6,<0.5.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Repository, https://github.com/youkergav/Malbench
+Description-Content-Type: text/markdown
+
+# Malbench
+Malbench is a command-line tool for testing and evaluating the effectiveness of malware detection tools (such as antivirus solutions). It does this by running a set of malware samples, and checking if the malware is flagged by the detection tool we are evaluating. Malbench is built to be modular and configurable, so it can be customized to meet the specific needs of different users and environments.
+![Malbench Terminal Demo](https://i.imgur.com/oGQNU8i.gif)
+
+## About
+### Disclaimer 
+**⚠ WARNING**: Malbench is a tool for testing antivirus software against real-world malware samples. While it does not contain any malware on its own, it is designed to run malware samples provided by the user. Use Malbench only in secure and isolated environments that you are authorized in doing so. Do **not** use Malbench on a computer or network that contains sensitive information or data that you are not willing to lose and/or become compromised. By using Malbench, you acknowledge the risks and assume full responsibility for any damages that may result.
+
+**ℹ️ NOTE**: As stated above: *Malbench does not come with any malicious code installed*. It is the user's responsibility to provide their own samples for testing purposes. This is to ensure that Malbench is used responsibly and ethically, and that users have control over the types of malware being tested.
+
+### Why Use Malbench
+Malware detection tools are an essential component of any computer security strategy, but they are not foolproof. New techniques and methods are constantly being developed to evade detection. It is important to regularly test and evaluate the effectiveness of detection tools to ensure that we are keeping up with these evolving threats.
+
+With all the different features and algorithms of modern antivirus solutions, it can be hard to find practical and objective results on what-all they defend against. Malbench can be leveraged to bulk-test known malware samples against antivirus solutions to deliver real and practical results. This is done by automatically launching multiple malware payloads on a system and seeing what samples are detected and which ones were evaded. With Malbench, users can customize their testing to meet their specific needs, selecting the malware samples they want to run, and the duration of a test.
+
+### How Antivirus is Benchmarked
+Malbench launches each malware sample selected by the user and monitors its execution. If the sample completes without error, it is flagged as `UNDETECTED`. If the sample is terminated with an error code, it is flagged as `DETECTED`, indicating that it was killed by the antivirus solution. If the sample is still running after a designated time (defaults to 2 seconds), Malbench forcibly kills the program and flags it as `UNDETECTED`, as the antivirus solution did not detect it in time.
+
+After each sample is run, Malbench displays the detection rate. The detection rate is a percentage representing the amount of samples the antivirus successfully defended against. 
+
+$$
+\text{Detection rate} = \frac{\text{Number of samples flagged as detected}}{\text{Total number of samples}} \times 100\%
+$$
+
+## Installation
+To install Malbench for general use, follow these simple steps:
+
+1.  Ensure that the following is installed on your system: [Python 3.8.1+](https://www.python.org/downloads/), and [PIP](https://pypi.org/project/pip/) (included with most Python installations).
+2.  Install Malbench via pip by running the following command:
+    ```bash
+    pip install malbench
+    ```
+3.  Confirm that Malbench has been installed:
+    ```
+    malbench --version
+    ```
+
+*If you are interested in installing Malbench for development, take a look at the [CONTRIBUTING.md](./CONTRIBUTING.md) file.*
+
+## Usage
+To use Malbench, simply run the following command inside your virtual environment:
+```bash
+python -m malbench /path/to/malware
+```
+
+Replace `/path/to/malware` with your `path` argument. The `path` argument should be the path to the malware samples you want to test. This can be either a single file or a folder containing multiple files. Only executable files will be ran by Malbench.
+
+By default, Malbench will show a banner when it starts, and will prompt you to confirm that you understand the risks involved before running the malware samples. You can disable the banner using the `--no-banner` flag, and disable the confirmation prompt using the `--no-warning` flag (as seen in the demo).
+
+Malware samples are run one by one, and Malbench will wait for each sample to be stopped by the detection software or reach the specified 2 second timeout before moving on to the next sample. This timeout can be changed with the `--timeout` flag. If a sample completes successfully, Malbench will print a red message with a `[-]` prefix, indicating it wasn't stopped by the detection software. If a sample has to be forcibly terminated by the detection software, Malbench will print a green message with a `[+]` prefix, indicating is was successfully detected and stopped.
+
+A full list of arguments to use with Malbench are below. This can be displayed with `--help`.
+```bash
+usage: malbench [-h] [-v] [-t TIMEOUT] [-nB] [-nW] [-d] path
+
+positional arguments:
+  path                  file or folder path of malware executables
+
+options:
+  -h, --help            show this help message and exit
+  -v, --version         shows malbench version number and exits
+  -t TIMEOUT, --timeout TIMEOUT
+                        malware TTL before being marked as failure (2 default)
+  -nC, --no-color       disables colored output
+  -nB, --no-banner      hides the banner logo
+  -nW, --no-warning     bypasses user confirmation before running
+  -d, --dev             enables stack tracing
+```
+
+## Contributing
+Contributions to Malbench are welcomed! If you'd like to contribute, please read our [CONTRIBUTING.md](./CONTRIBUTING.md) to get started.
+
+## License
+This project is licensed under the [GNU General Public License](https://www.gnu.org/licenses/gpl-3.0.en.html). See the [LICENSE.md](./LICENSE.md) file for details.
+
+## Credits
+Malbench was created by [Gavin Youker](mailto:youkergav@gmail.com).
+
```

