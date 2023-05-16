# Comparing `tmp/b2cloud-0.1.1.tar.gz` & `tmp/b2cloud-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2cloud-0.1.1.tar", max compression
+gzip compressed data, was "b2cloud-0.1.7.tar", max compression
```

## Comparing `b2cloud-0.1.1.tar` & `b2cloud-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1080 2022-12-22 02:24:57.073325 b2cloud-0.1.1/LICENSE
--rw-r--r--   0        0        0     3844 2022-12-23 01:38:51.262852 b2cloud-0.1.1/README.md
--rw-r--r--   0        0        0    21253 2022-12-22 03:21:32.545155 b2cloud-0.1.1/b2cloud/__init__.py
--rw-r--r--   0        0        0    10713 2022-12-23 00:31:06.854382 b2cloud-0.1.1/b2cloud/utilities.py
--rw-r--r--   0        0        0      634 2022-12-23 01:45:45.206224 b2cloud-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 b2cloud-0.1.1/setup.py
--rw-r--r--   0        0        0     4675 1970-01-01 00:00:00.000000 b2cloud-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-09 04:07:52.513765 b2cloud-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3844 2023-05-09 04:07:52.513934 b2cloud-0.1.7/README.md
+-rw-r--r--   0        0        0    21253 2023-05-09 04:07:52.514271 b2cloud-0.1.7/b2cloud/__init__.py
+-rw-r--r--   0        0        0    11383 2023-05-16 05:50:31.755841 b2cloud-0.1.7/b2cloud/utilities.py
+-rw-r--r--   0        0        0      634 2023-05-16 06:42:05.062505 b2cloud-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4816 1970-01-01 00:00:00.000000 b2cloud-0.1.7/setup.py
+-rw-r--r--   0        0        0     4675 1970-01-01 00:00:00.000000 b2cloud-0.1.7/PKG-INFO
```

### Comparing `b2cloud-0.1.1/LICENSE` & `b2cloud-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `b2cloud-0.1.1/README.md` & `b2cloud-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `b2cloud-0.1.1/b2cloud/__init__.py` & `b2cloud-0.1.7/b2cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `b2cloud-0.1.1/b2cloud/utilities.py` & `b2cloud-0.1.7/b2cloud/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,32 @@
 import math
 from difflib import SequenceMatcher
 import json
 
 import requests
 import fitz
+import re
+
+def normalize_and_trim_whitespace_in_text(text: str):
+    """
+    文字列を正規化し、全角スペースを半角スペースに変換し、連続したスペースを1つにし、
+    先頭と末尾のスペースを削除する
+    Args:
+        text(str): 正規化する文字列
+    Returns:
+        正規化し、スペースを調整した文字列
+    """
+    # 文字コードと全角スペースを半角スペースに変換
+    _text = re.sub(r'\s', ' ', text)
+    # 連続したスペースを1つにする
+    _text = re.sub(r'\s+', ' ', _text)
+    # 先頭と末尾のスペースを削除
+    _text = _text.strip()
+    return _text
+
 
 
 def get_postal(session:requests.Session, code:str):
     """
     B2クラウドの郵便番号情報を取得する
 
     Args:
```

### Comparing `b2cloud-0.1.1/pyproject.toml` & `b2cloud-0.1.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "b2cloud"
-version = "0.1.1"
+version = "0.1.7"
 description = "ヤマト運輸株式会社が提供する送り状発行システムB2クラウドをpythonで利用するパッケージ"
 authors = ["hgs-interman <naofumi.higashikawauchi@interman.co.jp>"]
 homepage = "https://www.interman.jp/"
 repository = "https://github.com/interman-corp/b2cloud"
 documentation = "https://github.com/interman-corp/b2cloud"
 readme = "README.md"
 license = "MIT"
```

### Comparing `b2cloud-0.1.1/setup.py` & `b2cloud-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['PyMuPDF>=1.21.1,<2.0.0', 'lxml>=4.9.2,<5.0.0', 'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'b2cloud',
-    'version': '0.1.1',
+    'version': '0.1.7',
     'description': 'ヤマト運輸株式会社が提供する送り状発行システムB2クラウドをpythonで利用するパッケージ',
     'long_description': '# b2cloud\n\nヤマト運輸株式会社の『送り状発行システムB2クラウド』を操作して伝票を印刷するためのモジュールです。\n利用にあたっては、ヤマトビジネスメンバーズのaccount情報が必要となります。\n\n## インストール\n\n```shell\npip install b2cloud\n```\n\n## コード例\n\n### 履歴の取得\n\n```python\nimport b2cloud\nimport b2cloud.utilities\n\nsession = b2cloud.login(\'your customer_code\', \'your customer_password\')\ndm = b2cloud.search_history(session, service_type=\'3\')\n\nfor entry in dm[\'feed\'][\'entry\']:\n    print(entry[\'shipment\'][\'tracking_number\'], entry[\'shipment\'][\'consignee_name\'])\n```\n\n### 新規に伝票を作成し、データに不備がないかチェックする\n\n```python\n# 伝票情報を生成する\nshipment = b2cloud.utilities.create_dm_shipment(\n    shipment_date=\'2022/12/24\',\n    consignee_telephone_display=\'00-0000-0000\',\n    consignee_name=\'テスト\',\n    consignee_zip_code=\'8900053\',\n    consignee_address1=\'鹿児島県\',\n    consignee_address2=\'鹿児島市\',\n    consignee_address3=\'中央町10\',\n    consignee_address4=\'キャンセビル６階\',\n    consignee_department1=\'インターマン株式会社\'\n)\n\n# データに不備がないかチェックする\nres = b2cloud.check_shipment(session, shipment)\nprint(res)\n\ne.g.\n{\'success\': True, \'errors\': []}\n```\n\n### 伝票の新規保存\n\n```python\n# shipmentsをpost_new_checkonlyを通す\nchecked_feed = b2cloud.post_new_checkonly(session, [shipment])\n# 伝票情報をB2クラウドに保存する\nres = b2cloud.post_new(session, checked_feed)\n```\n\n### 保存した伝票をDM形式で印刷し各伝票毎にPDFファイルに保存する\n\n```python\n# 保存済みのDM伝票を取得\ndm_feed = b2cloud.get_new(session, params={\'service_type\':\'3\'})\n# DM伝票形式（１シート8枚）で印刷\ndm_pdf = b2cloud.print_issue(session,\'3\', dm_feed)\n# １伝票毎に分割する\npdfs = b2cloud.utilities.split_pdf_dm(dm_pdf)\nfor i in range(len(pdfs)):\n    with open(f\'dm_{i}.pdf\', \'wb\') as f:\n        f.write(pdfs[i])\n```\n\n### 住所を伝票情報に変換する\n\n住所正規化サービスAddressian([https://addressian.netlify.app/](https://addressian.netlify.app/))のAPI Keyが必要です。\n\n```python\nconsignee_address = b2cloud.utilities.get_address_info(\n                                                session=session,\n                                                addressian_api_key=\'abcdefghijklmnopqrtsuvwxyz1234567890\',\n                                                address=\'鹿児島市中央町10キャンセビル6F\'\n                                            )\nprint(consignee_address)\n\ne.g.\n{\n    "consignee_zip_code": "8900053",\n    "consignee_address1": "鹿児島県",\n    "consignee_address2": "鹿児島市",\n    "consignee_address3": "中央町10",\n    "consignee_address4": "キャンセビル6F"\n}\n```\n\n## pytest\n\nパラメータでログイン情報やaddressian_api_keyを指定します。\n\n※注意\n\nテストを実行するとテスト伝票が発行されます。\nテスト実行後は、B2クラウドWEBサイトにログインして「保存分の発行」や「発行済みデータの検索」からテストデータを削除することをお勧めします。\n\n### pytest コマンド例\n\n```shell\npytest -q tests/test_01.py  --customer_code=0123456789 --customer_password=abcdefghi --addressian_api_key=abcdefghijklmnopqrtsuvwxyz1234567890\n```\n\n### パラメーターの一覧\n\n```python\nparser.addoption("--customer_code",      action="store", default="")\nparser.addoption("--customer_password",  action="store", default="")\nparser.addoption("--customer_cls_cocde", action="store", default="")\nparser.addoption("--login_user_id",      action="store", default="")\nparser.addoption("--addressian_api_key", action="store", default="")\n```\n',
     'author': 'hgs-interman',
     'author_email': 'naofumi.higashikawauchi@interman.co.jp',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://www.interman.jp/',
```

### Comparing `b2cloud-0.1.1/PKG-INFO` & `b2cloud-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b2cloud
-Version: 0.1.1
+Version: 0.1.7
 Summary: ヤマト運輸株式会社が提供する送り状発行システムB2クラウドをpythonで利用するパッケージ
 Home-page: https://www.interman.jp/
 License: MIT
 Author: hgs-interman
 Author-email: naofumi.higashikawauchi@interman.co.jp
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

