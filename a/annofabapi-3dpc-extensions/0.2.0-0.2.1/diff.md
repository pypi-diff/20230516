# Comparing `tmp/annofabapi-3dpc-extensions-0.2.0.tar.gz` & `tmp/annofabapi_3dpc_extensions-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annofabapi-3dpc-extensions-0.2.0.tar", max compression
+gzip compressed data, was "annofabapi_3dpc_extensions-0.2.1.tar", max compression
```

## Comparing `annofabapi-3dpc-extensions-0.2.0.tar` & `annofabapi_3dpc_extensions-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1081 2021-08-26 01:48:52.092351 annofabapi-3dpc-extensions-0.2.0/LICENSE
--rw-r--r--   0        0        0     2845 2021-09-01 02:21:29.189132 annofabapi-3dpc-extensions-0.2.0/README.md
--rw-r--r--   0        0        0       71 2021-08-31 12:26:44.037132 annofabapi-3dpc-extensions-0.2.0/annofab_3dpc/__init__.py
--rw-r--r--   0        0        0       22 2022-04-26 04:14:32.587448 annofabapi-3dpc-extensions-0.2.0/annofab_3dpc/__version__.py
--rw-r--r--   0        0        0    10506 2022-04-26 04:06:50.036288 annofabapi-3dpc-extensions-0.2.0/annofab_3dpc/annotation.py
--rw-r--r--   0        0        0        0 2021-09-01 03:06:03.469132 annofabapi-3dpc-extensions-0.2.0/annofab_3dpc/py.typed
--rw-r--r--   0        0        0     1898 2022-04-26 04:14:41.479892 annofabapi-3dpc-extensions-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3627 2022-05-06 00:27:45.216731 annofabapi-3dpc-extensions-0.2.0/setup.py
--rw-r--r--   0        0        0     3850 2022-05-06 00:27:45.217264 annofabapi-3dpc-extensions-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-16 07:20:49.314808 annofabapi_3dpc_extensions-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2905 2023-05-16 07:20:49.314808 annofabapi_3dpc_extensions-0.2.1/README.md
+-rw-r--r--   0        0        0       71 2023-05-16 07:20:49.314808 annofabapi_3dpc_extensions-0.2.1/annofab_3dpc/__init__.py
+-rw-r--r--   0        0        0      131 2023-05-16 07:21:02.919369 annofabapi_3dpc_extensions-0.2.1/annofab_3dpc/__version__.py
+-rw-r--r--   0        0        0    10506 2023-05-16 07:20:49.314808 annofabapi_3dpc_extensions-0.2.1/annofab_3dpc/annotation.py
+-rw-r--r--   0        0        0        0 2023-05-16 07:20:49.314808 annofabapi_3dpc_extensions-0.2.1/annofab_3dpc/py.typed
+-rw-r--r--   0        0        0     1612 2023-05-16 07:21:02.919369 annofabapi_3dpc_extensions-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3729 1970-01-01 00:00:00.000000 annofabapi_3dpc_extensions-0.2.1/PKG-INFO
```

### Comparing `annofabapi-3dpc-extensions-0.2.0/LICENSE` & `annofabapi_3dpc_extensions-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `annofabapi-3dpc-extensions-0.2.0/README.md` & `annofabapi_3dpc_extensions-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 [![Build Status](https://travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions.svg?branch=master)](https://travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions)
 [![PyPI version](https://badge.fury.io/py/annofabapi-3dpc-extensions.svg)](https://badge.fury.io/py/annofabapi-3dpc-extensions)
 [![Python Versions](https://img.shields.io/pypi/pyversions/annofabapi-3dpc-extensions.svg)](https://pypi.org/project/annofabapi-3dpc-extensions/)
 [![Documentation Status](https://readthedocs.org/projects/annofabapi-3dpc-extensions/badge/?version=latest)](https://annofabapi-3dpc-extensions.readthedocs.io/en/latest/?badge=latest)
 
 
 
-[annofabapi](https://github.com/kurusugawa-computer/annofab-api-python-client)の3DPC（3D Point Cloud） Editor用の拡張機能です。
+[annofabapi](https://github.com/kurusugawa-computer/annofab-api-python-client)の3次元アノテーション用の拡張機能です。
 
 # Install
 
-* Python 3.7+
+* Python 3.8+
 
 # Install
 
 ```
 $ pip install annofabapi-3dpc-extensions
 ```
 
@@ -63,9 +63,11 @@
 
 # セグメント情報が格納されたファイルを読み込む
 with parser.open_outer_file(Path(segment_annotation_data.data_uri).name) as f:
     dict_segmenta_data = json.load(f)
     segment_data = SegmentData.from_dict(dict_segmenta_data)
     assert type(segment_data) == SegmentData
     assert len(segment_data.points) > 0
+    print(segment_data.points)
+    # => [130439, 130442, ... ]
 
 ```
```

### Comparing `annofabapi-3dpc-extensions-0.2.0/annofab_3dpc/annotation.py` & `annofabapi_3dpc_extensions-0.2.1/annofab_3dpc/annotation.py`

 * *Files identical despite different names*

### Comparing `annofabapi-3dpc-extensions-0.2.0/pyproject.toml` & `annofabapi_3dpc_extensions-0.2.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,73 +1,68 @@
 [tool.poetry]
 name = "annofabapi-3dpc-extensions"
-version = "0.2.0"
+version = "0.2.1"  # `poetry-dynamic-versioning`を使ってGitHubのバージョンタグを取得している。変更不要
 description = "annofabapiの3DPC Editor用の拡張機能です。"
-authors = ["yuji38kwmt"]
+authors = ["Kurusugawa Computer Inc."]
 packages = [
     { include = "annofab_3dpc" }
 ]
 readme="README.md"
 repository="https://github.com/kurusugawa-computer/annofabapi-3dpc-extensions"
 classifiers = [
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
         "Topic :: Utilities",
         "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8.1"
 dataclasses-json="*"
 numpy = "*"
 
 [tool.poetry.dev-dependencies]
 # テストコードで利用するため
 annofabapi = ">=0.47.0"
 
 # test library
 pytest = "*"
 pytest-xdist = "*"
 pytest-cov = "*"
 
 # format library
-isort = "*" # import文をsortするために利用する
-autoflake = "*" # 未使用のimport文を削除するために利用する
-black = "*"
+isort = "^5"
+autoflake = "*"
+black = "^23"
 
 # lint library
-flake8 = "*"
-mypy = "*"
-pylint = "*"
+flake8 = "^6"
+mypy = "^1"
+pylint = "^2"
+
+
 
 # document library
-sphinx = "*"
-docutils = "*"
+sphinx = "^7"
 # pandasのdocumentationページに近いレイアウトにするためのパッケージ
-pydata-sphinx-theme = "*"
+pydata-sphinx-theme = ">=0.13.3"
 
 
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
-profile = "black"
 line_length = 120
-# `__init__.py`の順番が変わるとエラーになる可能性があるので、スキップする
-skip="annofab_3dpc/__init__.py"
-
 [tool.mypy]
 # スタブが無いパッケージのエラーは無視させる.サードパーティのライブラリに型情報がないケースもあるため
 ignore_missing_imports = true
+check_untyped_defs = true
 
-[build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+[tool.poetry-dynamic-versioning]
+enable = false
+format = "{base}"
 
+[build-system]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
+build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `annofabapi-3dpc-extensions-0.2.0/setup.py` & `annofabapi_3dpc_extensions-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,94 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: annofabapi-3dpc-extensions
+Version: 0.2.1
+Summary: annofabapiの3DPC Editor用の拡張機能です。
+Home-page: https://github.com/kurusugawa-computer/annofabapi-3dpc-extensions
+Author: Kurusugawa Computer Inc.
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Dist: dataclasses-json
+Requires-Dist: numpy
+Project-URL: Repository, https://github.com/kurusugawa-computer/annofabapi-3dpc-extensions
+Description-Content-Type: text/markdown
 
-packages = \
-['annofab_3dpc']
+# annofabapi-3dpc-extensions
+[![Build Status](https://travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions.svg?branch=master)](https://travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions)
+[![PyPI version](https://badge.fury.io/py/annofabapi-3dpc-extensions.svg)](https://badge.fury.io/py/annofabapi-3dpc-extensions)
+[![Python Versions](https://img.shields.io/pypi/pyversions/annofabapi-3dpc-extensions.svg)](https://pypi.org/project/annofabapi-3dpc-extensions/)
+[![Documentation Status](https://readthedocs.org/projects/annofabapi-3dpc-extensions/badge/?version=latest)](https://annofabapi-3dpc-extensions.readthedocs.io/en/latest/?badge=latest)
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['dataclasses-json', 'numpy']
-
-setup_kwargs = {
-    'name': 'annofabapi-3dpc-extensions',
-    'version': '0.2.0',
-    'description': 'annofabapiの3DPC Editor用の拡張機能です。',
-    'long_description': '# annofabapi-3dpc-extensions\n[![Build Status](https://travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions.svg?branch=master)](https://travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions)\n[![PyPI version](https://badge.fury.io/py/annofabapi-3dpc-extensions.svg)](https://badge.fury.io/py/annofabapi-3dpc-extensions)\n[![Python Versions](https://img.shields.io/pypi/pyversions/annofabapi-3dpc-extensions.svg)](https://pypi.org/project/annofabapi-3dpc-extensions/)\n[![Documentation Status](https://readthedocs.org/projects/annofabapi-3dpc-extensions/badge/?version=latest)](https://annofabapi-3dpc-extensions.readthedocs.io/en/latest/?badge=latest)\n\n\n\n[annofabapi](https://github.com/kurusugawa-computer/annofab-api-python-client)の3DPC（3D Point Cloud） Editor用の拡張機能です。\n\n# Install\n\n* Python 3.7+\n\n# Install\n\n```\n$ pip install annofabapi-3dpc-extensions\n```\n\n\n# Usage\n\ncuboidアノテーションやセグメントアノテーションに対応したデータクラスを利用できます。\n\n```python\nfrom annofabapi.parser import SimpleAnnotationDirParser\n\nfrom annofab_3dpc.annotation import (\n    CuboidAnnotationDetailDataV2,\n    EulerAnglesZXY,\n    SegmentAnnotationDetailData,\n    SegmentData,\n    convert_annotation_detail_data,\n)\n\nparser = SimpleAnnotationDirParser("tests/data/task1/input1.json")\nresult = parser.parse(convert_annotation_detail_data)\n\nsegment_annotation_data = result.details[0].data\ncuboid_annotation_data = result.details[1].data\nassert type(segment_annotation_data) == SegmentAnnotationDetailData\nassert type(cuboid_annotation_data) == CuboidAnnotationDetailDataV2\n\n\n### cuboid annotation\n\nprint(cuboid_annotation_data)\n# => CuboidAnnotationDetailDataV2(shape=CuboidShapeV2(dimensions=Size(width=6.853874863204751, height=0.2929844409227371, depth=4.092537841193188), location=Location(x=-11.896872014598989, y=-3.0571381239812996, z=0.3601047024130821), rotation=EulerAnglesZXY(x=0, y=0, z=0), direction=CuboidDirection(front=Vector3(x=1, y=0, z=0), up=Vector3(x=0, y=0, z=1))), kind=\'CUBOID\', version=\'2\')\n\n# オイラー角をクォータニオンに変換\nprint(cuboid_annotation_data.shape.rotation.to_quaternion())\n# => [1.0, 0.0, 0.0, 0.0]\n\n# クォータニオンからオイラー角に変換\nprint(EulerAnglesZXY.from([1.0, 0.0, 0.0, 0.0]))\n# => EulerAnglesZXY(x=-0.0, y=0.0, z=0.0)\n\n\n### segment annotation\nprint(segment_annotation_data)\n# => SegmentAnnotationDetailData(data_uri=\'./input1/7ba51c15-f07a-4e29-8584-a4eaf3a6812a\')\n\n# セグメント情報が格納されたファイルを読み込む\nwith parser.open_outer_file(Path(segment_annotation_data.data_uri).name) as f:\n    dict_segmenta_data = json.load(f)\n    segment_data = SegmentData.from_dict(dict_segmenta_data)\n    assert type(segment_data) == SegmentData\n    assert len(segment_data.points) > 0\n\n```\n',
-    'author': 'yuji38kwmt',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/kurusugawa-computer/annofabapi-3dpc-extensions',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
 
+[annofabapi](https://github.com/kurusugawa-computer/annofab-api-python-client)の3次元アノテーション用の拡張機能です。
+
+# Install
+
+* Python 3.8+
+
+# Install
+
+```
+$ pip install annofabapi-3dpc-extensions
+```
+
+
+# Usage
+
+cuboidアノテーションやセグメントアノテーションに対応したデータクラスを利用できます。
+
+```python
+from annofabapi.parser import SimpleAnnotationDirParser
+
+from annofab_3dpc.annotation import (
+    CuboidAnnotationDetailDataV2,
+    EulerAnglesZXY,
+    SegmentAnnotationDetailData,
+    SegmentData,
+    convert_annotation_detail_data,
+)
+
+parser = SimpleAnnotationDirParser("tests/data/task1/input1.json")
+result = parser.parse(convert_annotation_detail_data)
+
+segment_annotation_data = result.details[0].data
+cuboid_annotation_data = result.details[1].data
+assert type(segment_annotation_data) == SegmentAnnotationDetailData
+assert type(cuboid_annotation_data) == CuboidAnnotationDetailDataV2
+
+
+### cuboid annotation
+
+print(cuboid_annotation_data)
+# => CuboidAnnotationDetailDataV2(shape=CuboidShapeV2(dimensions=Size(width=6.853874863204751, height=0.2929844409227371, depth=4.092537841193188), location=Location(x=-11.896872014598989, y=-3.0571381239812996, z=0.3601047024130821), rotation=EulerAnglesZXY(x=0, y=0, z=0), direction=CuboidDirection(front=Vector3(x=1, y=0, z=0), up=Vector3(x=0, y=0, z=1))), kind='CUBOID', version='2')
+
+# オイラー角をクォータニオンに変換
+print(cuboid_annotation_data.shape.rotation.to_quaternion())
+# => [1.0, 0.0, 0.0, 0.0]
+
+# クォータニオンからオイラー角に変換
+print(EulerAnglesZXY.from([1.0, 0.0, 0.0, 0.0]))
+# => EulerAnglesZXY(x=-0.0, y=0.0, z=0.0)
+
+
+### segment annotation
+print(segment_annotation_data)
+# => SegmentAnnotationDetailData(data_uri='./input1/7ba51c15-f07a-4e29-8584-a4eaf3a6812a')
+
+# セグメント情報が格納されたファイルを読み込む
+with parser.open_outer_file(Path(segment_annotation_data.data_uri).name) as f:
+    dict_segmenta_data = json.load(f)
+    segment_data = SegmentData.from_dict(dict_segmenta_data)
+    assert type(segment_data) == SegmentData
+    assert len(segment_data.points) > 0
+    print(segment_data.points)
+    # => [130439, 130442, ... ]
+
+```
 
-setup(**setup_kwargs)
```

