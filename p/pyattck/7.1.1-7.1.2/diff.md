# Comparing `tmp/pyattck-7.1.1.tar.gz` & `tmp/pyattck-7.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyattck-7.1.1.tar", max compression
+gzip compressed data, was "pyattck-7.1.2.tar", max compression
```

## Comparing `pyattck-7.1.1.tar` & `pyattck-7.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1065 2023-03-06 21:52:11.057911 pyattck-7.1.1/LICENSE.md
--rw-r--r--   0        0        0    15855 2023-03-06 21:52:11.057911 pyattck-7.1.1/README.md
--rw-r--r--   0        0        0      114 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/__init__.py
--rw-r--r--   0        0        0    14496 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/attck.py
--rw-r--r--   0        0        0     1110 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/base.py
--rw-r--r--   0        0        0      123 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/cli.py
--rw-r--r--   0        0        0     6641 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/configuration.py
--rw-r--r--   0        0        0     1213 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/data/logging.yml
--rw-r--r--   0        0        0     5309 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/enterprise.py
--rw-r--r--   0        0        0     4183 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/ics.py
--rw-r--r--   0        0        0     3070 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/mobile.py
--rw-r--r--   0        0        0     1998 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/preattck.py
--rw-r--r--   0        0        0        0 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/utils/__init__.py
--rw-r--r--   0        0        0      816 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/utils/exceptions.py
--rw-r--r--   0        0        0     1260 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/utils/interactive.py
--rw-r--r--   0        0        0     7149 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/utils/layout.py
--rw-r--r--   0        0        0     1549 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/utils/logger.py
--rw-r--r--   0        0        0     3644 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/utils/menu.py
--rw-r--r--   0        0        0      655 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/utils/utils.py
--rw-r--r--   0        0        0       80 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyattck/utils/version.py
--rw-r--r--   0        0        0      877 2023-03-06 21:52:11.145917 pyattck-7.1.1/pyproject.toml
--rw-r--r--   0        0        0    17126 1970-01-01 00:00:00.000000 pyattck-7.1.1/setup.py
--rw-r--r--   0        0        0    16771 1970-01-01 00:00:00.000000 pyattck-7.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-16 02:53:46.053746 pyattck-7.1.2/LICENSE.md
+-rw-r--r--   0        0        0    15855 2023-05-16 02:53:46.057746 pyattck-7.1.2/README.md
+-rw-r--r--   0        0        0      114 2023-05-16 02:53:46.141747 pyattck-7.1.2/pyattck/__init__.py
+-rw-r--r--   0        0        0    14496 2023-05-16 02:53:46.141747 pyattck-7.1.2/pyattck/attck.py
+-rw-r--r--   0        0        0     1110 2023-05-16 02:53:46.141747 pyattck-7.1.2/pyattck/base.py
+-rw-r--r--   0        0        0      123 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/cli.py
+-rw-r--r--   0        0        0     6641 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/configuration.py
+-rw-r--r--   0        0        0     1213 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/data/logging.yml
+-rw-r--r--   0        0        0     5309 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/enterprise.py
+-rw-r--r--   0        0        0     4183 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/ics.py
+-rw-r--r--   0        0        0     3070 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/mobile.py
+-rw-r--r--   0        0        0     1998 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/preattck.py
+-rw-r--r--   0        0        0        0 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/utils/__init__.py
+-rw-r--r--   0        0        0      816 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/utils/exceptions.py
+-rw-r--r--   0        0        0     1260 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/utils/interactive.py
+-rw-r--r--   0        0        0     7149 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/utils/layout.py
+-rw-r--r--   0        0        0     1549 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/utils/logger.py
+-rw-r--r--   0        0        0     3644 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/utils/menu.py
+-rw-r--r--   0        0        0      655 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/utils/utils.py
+-rw-r--r--   0        0        0       80 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyattck/utils/version.py
+-rw-r--r--   0        0        0      877 2023-05-16 02:53:46.145748 pyattck-7.1.2/pyproject.toml
+-rw-r--r--   0        0        0    17126 1970-01-01 00:00:00.000000 pyattck-7.1.2/setup.py
+-rw-r--r--   0        0        0    16771 1970-01-01 00:00:00.000000 pyattck-7.1.2/PKG-INFO
```

### Comparing `pyattck-7.1.1/LICENSE.md` & `pyattck-7.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/README.md` & `pyattck-7.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/attck.py` & `pyattck-7.1.2/pyattck/attck.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/base.py` & `pyattck-7.1.2/pyattck/base.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/configuration.py` & `pyattck-7.1.2/pyattck/configuration.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/data/logging.yml` & `pyattck-7.1.2/pyattck/data/logging.yml`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/enterprise.py` & `pyattck-7.1.2/pyattck/enterprise.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/ics.py` & `pyattck-7.1.2/pyattck/ics.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/mobile.py` & `pyattck-7.1.2/pyattck/mobile.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/preattck.py` & `pyattck-7.1.2/pyattck/preattck.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/utils/exceptions.py` & `pyattck-7.1.2/pyattck/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/utils/interactive.py` & `pyattck-7.1.2/pyattck/utils/interactive.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/utils/layout.py` & `pyattck-7.1.2/pyattck/utils/layout.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/utils/logger.py` & `pyattck-7.1.2/pyattck/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/utils/menu.py` & `pyattck-7.1.2/pyattck/utils/menu.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyattck/utils/utils.py` & `pyattck-7.1.2/pyattck/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pyattck-7.1.1/pyproject.toml` & `pyattck-7.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyattck"
-version = "7.1.1"
+version = "7.1.2"
 description = "A Python package to interact with the Mitre ATT&CK Frameworks"
 authors = ["Swimlane <info@swimlane.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/swimlane/pyattck"
 repository = "https://github.com/swimlane/pyattck"
 
@@ -12,15 +12,15 @@
 pyattck = "pyattck.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 requests = "^2.27.1"
 fire = "^0.4.0"
 attrs = "^21.4.0"
-pyattck-data = "^2.5.0"
+pyattck-data = "^2.6.3"
 rich = "^12.5.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pylama = "^8.3.8"
 coverage = "^6.4.1"
 recommonmark = "^0.7.1"
```

### Comparing `pyattck-7.1.1/setup.py` & `pyattck-7.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 
 package_data = \
 {'': ['*'], 'pyattck': ['data/*']}
 
 install_requires = \
 ['attrs>=21.4.0,<22.0.0',
  'fire>=0.4.0,<0.5.0',
- 'pyattck-data>=2.5.0,<3.0.0',
+ 'pyattck-data>=2.6.3,<3.0.0',
  'requests>=2.27.1,<3.0.0',
  'rich>=12.5.1,<13.0.0']
 
 entry_points = \
 {'console_scripts': ['pyattck = pyattck.cli:main']}
 
 setup_kwargs = {
     'name': 'pyattck',
-    'version': '7.1.1',
+    'version': '7.1.2',
     'description': 'A Python package to interact with the Mitre ATT&CK Frameworks',
     'long_description': '![pyattck](https://github.com/swimlane/pyattck/workflows/Testing%20pyattck/badge.svg)\n![](./images/ubuntu_support.svg)\n![](./images/macos_support.svg)\n![](./images/windows_support.svg)\n![](./images/code_coverage.svg)\n\n# Welcome to pyattck\'s Documentation\n\n```\n    .______   ____    ____  ___   .___________.___________.  ______  __  ___\n    |   _  \\  \\   \\  /   / /   \\  |           |           | /      ||  |/  /\n    |  |_)  |  \\   \\/   / /  ^  \\ `---|  |----`---|  |----`|  ,----\'|  \'  /\n    |   ___/    \\_    _/ /  /_\\  \\    |  |        |  |     |  |     |    <\n    |  |          |  |  /  _____  \\   |  |        |  |     |  `----.|  .  \\\n    | _|          |__| /__/     \\__\\  |__|        |__|      \\______||__|\\__\\\n\n```\n\tA Python package to interact with MITRE ATT&CK Frameworks\n\n> Current Version is 7.1.1\n\n**pyattck** is a light-weight framework for MITRE ATT&CK Frameworks. This package extracts details from the MITRE Enterprise, PRE-ATT&CK, Mobile, and ICS Frameworks.\n\n## Why?\n\n`pyattck` assist organizations and individuals with accessing MITRE ATT&CK Framework(s) in a programmatic way. Meaning, you can access all defined actors, malwares, mitigations, tactics, techniques, and tools defined by the Enterprise, Mobile, Pre-Attck, and ICS frameworks via a command-line utility or embedding into your own code base.\n\nThere are many reasons why you would want to access this data in an automated (scripted/coded) way but a few examples are:\n\n* Generate reports with additional details about a technique (or any object defined in the framework) \n* A build pipeline of detection rules with additional MITRE ATT&CK details for categorization\n* Quickly searching for specific details about a technique without navigating a web page\n\nThere are other benefits that `pyattck` provide as well which includes the ability to provide additional contextual data. You can find more information about this data [here](https://github.com/swimlane/pyattck-data) but the basics are that `pyattck` utilizes multiple open-source repositories to gather additional contextual data like commands used to execute a technique, country and other details about a malicious actor, other variants of malware similar to a defined tool/malware, etc. \n\nThis additional context is what makes `pyattck` truly powerful and enables people to build more robust testing and validation of their detection rules, validates testing assumptions, etc. Truly there are countless ways that `pyattck` could be utilized to help blue, red, and purple teams defend organizations (and themselves).\n\n## Features\n\nThe **pyattck** package retrieves all Tactics, Techniques, Actors, Malware, Tools, and Mitigations from the MITRE ATT&CK Frameworks as well as any defined relationships within the MITRE ATT&CK dataset (including sub-techniques).\n\nIn addition, Techniques, Actors, and Tools (if applicable) now have collected data from third-party resources that are accessible via different properties. For more detailed information about these features, see [External Datasets](https://github.com/swimlane/pyattck-data).\n\nThe **pyattck** package allows you to:\n\n  * Specify a URL or local file path for the MITRE ATT&CK Enterprise Framework json, generated dataset, and/or a config.yml file.\n  * Access data from the MITRE PRE-ATT&CK Framework\n  * Access data from the MITRE Mobile ATT&CK Framework\n  * Access data from the MITRE ICS ATT&CK Framework\n  * Access sub-techniques as nested objects or you can turn it off and access as normal technique\n  * Access compliance controls (currently NIST 800-53 v5) related to a MITRE ATT&CK Technique\n  * pyattck now utilizes structured data models. More information can be found at [pyattck-data](https://github.com/swimlane/pyattck-data)\n  * Run an interactive console menu system to access pyattck data\n\n# Table of Contents\n\n1. [Installation](#installation)\n2. [Usage Example](#usage-example)\n3. [Configuration](#configuration)\n4. [Notes](#note)\n\n## Installation\n\nYou can install **pyattck** on OS X, Linux, or Windows. You can also install it directly from the source. To install, see the commands under the relevant operating system heading, below.\n\n### macOS, Linux and Windows:\n\n```bash\npip install pyattck\n```\n\n### Installing from source\n\n```bash\ngit clone https://github.com/swimlane/pyattck.git\ncd pyattck\npython setup.py install\n```\n\n## Usage example\n\nTo use **pyattck** you must instantiate an **Attck** object. Although you can interact directly with each class, the intended use is through a **Attck** object:\n\n```python\nfrom pyattck import Attck\n\nattack = Attck()\n```\n\nBy default, `sub-techniques` are accessible under each technique object. You can turn this behavior off by passing `nested_techniques=False` when creating your `Attck` object.\n\nAs an example, the default behavior looks like the following example:\n\n```python\nfrom pyattck import Attck\n\nattack = Attck()\n\nfor technique in attack.enterprise.techniques:\n    print(technique.id)\n    print(technique.name)\n    for subtechnique in technique.techniques:\n        print(subtechnique.id)\n        print(subtechnique.name)\n```\n\nYou can access the following `main` properties on your **Attck** object:\n\n* enterprise\n* preattack\n* mobile\n* ics\n\nOnce you specify the MITRE ATT&CK Framework, you can access additional properties.\n\nHere are the accessible objects under the [Enterprise](docs/enterprise.md) property:\n\n* [actors](docs/actor.md)\n* [controls](docs/control.md)\n* [malwares](docs/malware.md)\n* [mitigations](docs/mitigation.md)\n* [tactics](docs/tactic.md)\n* [techniques](docs/technique.md)\n* [tools](docs/tools.md)\n\nFor more information on object types under the `enterprise` property, see [Enterprise](docs/enterprise.md).\n\nHere are the accessible objects under the [PreAttck](docs/preattck.md) property:\n\n* [actors](docs/actor.md)\n* [tactics](docs/tactic.md)\n* [techniques](docs/technique.md)\n\nFor more information on object types under the `preattck` property, see [PreAttck](docs/preattck.md).\n\nHere are the accessible objects under the [Mobile](docs/mobile.md) property:\n\n* [actors](docs/actor.md)\n* [malwares](docs/malware.md)\n* [mitigations](docs/mitigation.md)\n* [tactics](docs/tactic.md)\n* [techniques](docs/technique.md)\n* [tools](docs/tools.md)\n\nFor more information on object types under the `mobile` property, see [Mobile](docs/mobile.md).\n\nHere are the accessible objects under the [ICS](docs/ics.md) property:\n\n* [controls](docs/control.md)\n* [malwares](docs/malware.md)\n* [mitigations](docs/mitigation.md)\n* [tactics](docs/tactic.md)\n* [techniques](docs/technique.md)\n\nFor more information on object types under the `ics` property, see [ICS](docs/ics.md).\n\n## Interactive Menu Usage\n\nTo utilize the new interactive menu system within pyattck, you must set `interactive` to `True`. By doing so, it will launch the interactive console menu system.\n\nUsing a script your can launch this by running:\n\n```python\nfrom pyattck import Attck\n\nAttck(interactive=True)\n```\n\nOr you can also run interactive mode on the command line:\n\n```bash\npyattck --interactive\n```\n\nCheckout a gif example below:\n\n![](images/pyattck_interactive_menu.gif)\n\n## Configuration\n\n`pyattck` allows you to configure if you store external data and where it is stored. \n\n```python\nfrom pyattck import Attck\n\nattck = Attck(\n    nested_techniques=True,\n    use_config=False,\n    save_config=False,\n    config_file_path=\'~/pyattck/config.yml\',\n    data_path=\'~/pyattck/data\',\n    enterprise_attck_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_enterprise_attck_v1.json",\n    pre_attck_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_pre_attck_v1.json",\n    mobile_attck_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_mobile_attck_v1.json,\n    ics_attck_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_ics_attck_v1.json",\n    nist_controls_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_nist_controls_v1.json",\n    generated_nist_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/attck_to_nist_controls.json",\n    **kwargs\n)\n```\n\nBy default, `pyattck` will (now) pull the latest external data from their respective locations using HTTP GET requests. `pyattck` currently pulls from the following locations:\n\n* enterprise_attck_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_enterprise_attck_v1.json"\n* pre_attck_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_pre_attck_v1.json"\n* mobile_attck_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_mobile_attck_v1.json"\n* ics_attck_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_ics_attck_v1.json"\n* nist_controls_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/merged_nist_controls_v1.json"\n* generated_nist_json="https://swimlane-pyattck.s3.us-west-2.amazonaws.com/attck_to_nist_controls.json"\n\nYou have several options when instantiating the `Attck` object. As of `4.0.0` you can now specify any of the following options:\n\n* use_config - When you specify this argument as `True` pyattck will attempt to retrieve the configuration specified in the `config_file_path` location. If this file is corrupted or cannot be found, we will default to retrieving data from the specified `*_attck_json` locations.\n* save_config - When you specify this argument as `True` pyattck will save the configuration file to the specified location set by `config_file_path`. Additionally, we will save all downloaded files to the `data_path` location specified. If you have specified a local path location instead of a download URL for any of the `*_attck_json` parameters we will save this location in our configuration and reference this location going forward. \n* config_file_path - The path to store a configuration file. Default is `~/pyattck/config.yml`\n* data_path - The path to store any data files downloaded to the local system. Default is `~/pyattck/data`\n\n### JSON Locations\n\nAdditionally, you can specify the location for each individual `*_attck_json` files by passing in either a URI or a local file path. If you have passed in a local file path, we will simply read from this file. \n\nIf you have used the default values or specified an alternative URI location to retrieve these JSON files from, you can additionally pass in `**kwargs` that will be passed along to the `Requests` python package when performing any HTTP requests.\n\n## Note\n\nWe understand that there are many different open-source projects being released, even on a daily basis, but we wanted to provide a straightforward Python package that allowed the user to identify known relationships between all verticals of the MITRE ATT&CK Framework.\n\nIf you are unfamiliar with the MITRE ATT&CK Framework, there are a few key components to ensure you have a firm grasp around. The first is Tactics & Techniques. When looking at the [MITRE ATT&CK Framework](https://attack.mitre.org/), the Tactics are the columns and represent the different phases of an attack.\n\n   > The MITRE ATT&CK Framework is NOT an all encompassing/defacto security coverage map - it is rather a FRAMEWORK and additional avenues should also be considered when assessing your security posture.\n\nTechniques are the rows of the framework and are categorized underneath specific Tactics (columns). They are data points within the framework that provides guidance when assessing your security gaps. Additionally, (most) Techniques contain mitigation guidance in addition to information about their relationship to tools, malware, and even actors/groups that have used this technique during recorded attacks.\n\nThis means, if your organization is focused on TTPs (Tactics Techniques and Procedures) used by certain actors/groups then MITRE ATT&CK Framework is perfect for you. If you are not at this security maturing within your organization, no worries! The ATT&CK Framework still provides really good guidance in a simple and straightforward layout, but programmatically it is not straightforward--especially if you wanted to measure (or map) your security controls using the framework.\n\n### Developing and Testing\n\nYou can add features or bugs or run the code in a development environment.\n\n1. To get a development and testing environment up and running, use this [Dockerfile](https://github.com/swimlane/pyattck/blob/master/Dockerfile).\n\n2. To use the `Dockerfile` run, cd to this repository directory and run:\n\n  ```\n  docker build --force-rm -t pyattck .\n  ```\n\n3. Next, run the docker container:\n\n  ```\n  docker run pyattck\n  ```\n\n  Running this calls the test python file in [bin/test.py](https://github.com/swimlane/pyattck/blob/master/bin/test.py).\n\n4. Modify the test python file for additional testing and development.\n\n## Running the tests\n\nTests within this project should cover all available properties and methods. As this project grows the tests will become more robust but for now we are testing that they exist and return outputs.\n\n## Contributing\n\nPlease read [CONTRIBUTING.md](https://github.com/swimlane/pyattck/blob/master/CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.\n\n## Versioning\n\nWe use [SemVer](http://semver.org/) for versioning.\n\n## Change Log\n\nFor details on features for a specific version of `pyattck`, see the [CHANGELOG.md](https://github.com/swimlane/pyattck/blob/master/CHANGELOG.md).\n\n## Authors\n\n* Josh Rickard - *Initial work* - [MSAdministrator](https://github.com/msadministrator)\n\nSee also the list of [contributors](https://github.com/swimlane/pyattck/contributors).\n\n## License\n\nThis project is licensed under the [MIT License](https://github.com/swimlane/pyattck/blob/master/LICENSE.md).\n\n## Acknowledgments\n\nFirst of all, I would like to thank everyone who contributes to open-source projects, especially the maintainers and creators of these projects. Without them, this capability would not be possible.\n\nThis data set is generated from many different sources. As we continue to add more sources, we will continue to add them here. Again thank you to all of these projects. In no particular order, `pyattck` utilizes data from the following projects:\n\n* [Mitre ATT&CK APT3 Adversary Emulation Field Manual](https://attack.mitre.org/docs/APT3_Adversary_Emulation_Field_Manual.xlsx)\n* [Atomic Red Team (by Red Canary)](https://github.com/redcanaryco/atomic-red-team)\n* [Atomic Threat Coverage](https://github.com/atc-project/atomic-threat-coverage)\n* [attck_empire (by dstepanic)](https://github.com/dstepanic/attck_empire)\n* [sentinel-attack (by BlueTeamLabs)](https://github.com/BlueTeamLabs/sentinel-attack)\n* [Litmus_test (by Kirtar22)](https://github.com/Kirtar22/Litmus_Test)\n* [nsm-attack (by oxtf)](https://github.com/0xtf/nsm-attack)\n* [osquery-attck (by teoseller)](https://github.com/teoseller/osquery-attck)\n* [Mitre Stockpile](https://github.com/mitre/stockpile)\n* [SysmonHunter (by baronpan)](https://github.com/baronpan/SysmonHunter)\n* [ThreatHunting-Book (by 12306Bro)](https://github.com/12306Bro/Threathunting-book)\n* [threat_hunting_tables (by dwestgard)](https://github.com/dwestgard/threat_hunting_tables)\n* [APT Groups & Operations](https://docs.google.com/spreadsheets/d/1H9_xaxQHpWaa4O_Son4Gx0YOIzlcBWMsdvePFX68EKU/edit#gid=1864660085)\n* [C2Matrix (by @jorgeorchilles, @brysonbort, @adam_mashinchi)](https://www.thec2matrix.com/)\n* [Elemental](https://github.com/Elemental-attack/Elemental)\n* [MalwareArchaeology - ATTACK](https://github.com/MalwareArchaeology/ATTACK)\n* [Attack-Technique-Dataset](https://github.com/NewBee119/Attack-Technique-Dataset)\n\n\n```eval_rst\n.. toctree::\n   :titlesonly:\n\n   configuration\n   pyattck/attck\n   Dataset <https://github.com/swimlane/pyattck-data>\n   Data Models <https://github.com/swimlane/pyattck-data>\n   enterprise/enterprise\n   preattck/preattck\n   mobile/mobileattck\n   ics/icsattck\n```\n',
     'author': 'Swimlane',
     'author_email': 'info@swimlane.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/swimlane/pyattck',
```

### Comparing `pyattck-7.1.1/PKG-INFO` & `pyattck-7.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyattck
-Version: 7.1.1
+Version: 7.1.2
 Summary: A Python package to interact with the Mitre ATT&CK Frameworks
 Home-page: https://github.com/swimlane/pyattck
 License: MIT
 Author: Swimlane
 Author-email: info@swimlane.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=21.4.0,<22.0.0)
 Requires-Dist: fire (>=0.4.0,<0.5.0)
-Requires-Dist: pyattck-data (>=2.5.0,<3.0.0)
+Requires-Dist: pyattck-data (>=2.6.3,<3.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rich (>=12.5.1,<13.0.0)
 Project-URL: Repository, https://github.com/swimlane/pyattck
 Description-Content-Type: text/markdown
 
 ![pyattck](https://github.com/swimlane/pyattck/workflows/Testing%20pyattck/badge.svg)
 ![](./images/ubuntu_support.svg)
```

