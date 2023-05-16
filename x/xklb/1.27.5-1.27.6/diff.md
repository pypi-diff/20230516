# Comparing `tmp/xklb-1.27.5.tar.gz` & `tmp/xklb-1.27.6.tar.gz`

## Comparing `xklb-1.27.5.tar` & `xklb-1.27.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.27.5/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.27.5/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.27.5/Windows.md
--rw-r--r--   0        0        0   416092 2020-02-02 00:00:00.000000 xklb-1.27.5/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.27.5/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.27.5/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.27.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.27.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.27.5/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.27.5/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/__init__.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/books.py
--rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/consts.py
--rw-r--r--   0        0        0     8450 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/dl_config.py
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/dl_extract.py
--rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/fs_extract.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/hn_extract.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/lb.py
--rw-r--r--   0        0        0    35208 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/playback.py
--rw-r--r--   0        0        0    28867 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/praw_extract.py
--rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/stats.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/tube_extract.py
--rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/utils.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.27.5/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.27.5/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.27.5/LICENSE
--rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.27.5/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.27.5/pyproject.toml
--rw-r--r--   0        0        0    44035 2020-02-02 00:00:00.000000 xklb-1.27.5/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.27.6/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.27.6/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.27.6/Windows.md
+-rw-r--r--   0        0        0   416100 2020-02-02 00:00:00.000000 xklb-1.27.6/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.27.6/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.27.6/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.27.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.27.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.27.6/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.27.6/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/__init__.py
+-rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/books.py
+-rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/consts.py
+-rw-r--r--   0        0        0     8450 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/dl_config.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14414 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/lb.py
+-rw-r--r--   0        0        0    35208 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/playback.py
+-rw-r--r--   0        0        0    28867 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/stats.py
+-rw-r--r--   0        0        0     4060 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/utils.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.27.6/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.27.6/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.27.6/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.27.6/LICENSE
+-rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.27.6/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.27.6/pyproject.toml
+-rw-r--r--   0        0        0    44035 2020-02-02 00:00:00.000000 xklb-1.27.6/PKG-INFO
```

### Comparing `xklb-1.27.5/Windows.md` & `xklb-1.27.6/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/pdm.lock` & `xklb-1.27.6/pdm.lock`

 * *Files 1% similar despite different names*

```diff
@@ -899,15 +899,15 @@
     "asttokens>=2.1.0",
     "executing>=1.2.0",
     "pure-eval",
 ]
 
 [[package]]
 name = "stevedore"
-version = "5.0.0"
+version = "5.1.0"
 requires_python = ">=3.8"
 summary = "Manage dynamic plugins for Python applications"
 dependencies = [
     "pbr!=2.1.0,>=2.0.0",
 ]
 
 [[package]]
@@ -982,15 +982,15 @@
 name = "tzdata"
 version = "2023.3"
 requires_python = ">=2"
 summary = "Provider of IANA time zone data"
 
 [[package]]
 name = "tzlocal"
-version = "5.0"
+version = "5.0.1"
 requires_python = ">=3.7"
 summary = "tzinfo object for the local timezone"
 dependencies = [
     "backports-zoneinfo; python_version < \"3.9\"",
     "tzdata; platform_system == \"Windows\"",
 ]
 
@@ -2611,17 +2611,17 @@
 "ssort 0.11.6" = [
     {url = "https://files.pythonhosted.org/packages/27/c6/4fdb102b282380d5b4791d90302ba8778689f24bef118707fd50f037752e/ssort-0.11.6.tar.gz", hash = "sha256:21fec493487f32dff50d30efa5b6aad18286e9817600b64bfe686ae062bae7ae"},
 ]
 "stack-data 0.6.2" = [
     {url = "https://files.pythonhosted.org/packages/6a/81/aa96c25c27f78cdc444fec27d80f4c05194c591465e491a1358d8a035bc1/stack_data-0.6.2-py3-none-any.whl", hash = "sha256:cbb2a53eb64e5785878201a97ed7c7b94883f48b87bfb0bbe8b623c74679e4a8"},
     {url = "https://files.pythonhosted.org/packages/db/18/aa7f2b111aeba2cd83503254d9133a912d7f61f459a0c8561858f0d72a56/stack_data-0.6.2.tar.gz", hash = "sha256:32d2dd0376772d01b6cb9fc996f3c8b57a357089dec328ed4b6553d037eaf815"},
 ]
-"stevedore 5.0.0" = [
-    {url = "https://files.pythonhosted.org/packages/41/1b/bad9124b400334d48aed1e04799032909fd8f1ca4a8e0eb30841284dd489/stevedore-5.0.0-py3-none-any.whl", hash = "sha256:bd5a71ff5e5e5f5ea983880e4a1dd1bb47f8feebbb3d95b592398e2f02194771"},
-    {url = "https://files.pythonhosted.org/packages/f1/25/993d09dc7be3e7927228853c75324104d734bb784bd766b025ebf9f47b16/stevedore-5.0.0.tar.gz", hash = "sha256:2c428d2338976279e8eb2196f7a94910960d9f7ba2f41f3988511e95ca447021"},
+"stevedore 5.1.0" = [
+    {url = "https://files.pythonhosted.org/packages/4b/68/e739fd061b0aba464bef8e8be48428b2aabbfb3f2f8f2f8ca257363ee6b2/stevedore-5.1.0-py3-none-any.whl", hash = "sha256:8cc040628f3cea5d7128f2e76cf486b2251a4e543c7b938f58d9a377f6694a2d"},
+    {url = "https://files.pythonhosted.org/packages/ac/d6/77387d3fc81f07bc8877e6f29507bd7943569093583b0a07b28cfa286780/stevedore-5.1.0.tar.gz", hash = "sha256:a54534acf9b89bc7ed264807013b505bf07f74dbe4bcfa37d32bd063870b087c"},
 ]
 "subliminal 2.1.0" = [
     {url = "https://files.pythonhosted.org/packages/7e/9e/f43da338d9f21ec693a153d5c8effae866f2b8448ae39a257337bf1b318d/subliminal-2.1.0-py2-none-any.whl", hash = "sha256:4b659bd523baefa7e260be4010311b2056bc3a4cc484e76c7fc3d213c9daebc0"},
     {url = "https://files.pythonhosted.org/packages/d6/f6/d523ddbb9304fa3597101903c0004bdba50c495a1e0d355cdd763df6f2d8/subliminal-2.1.0-py3-none-any.whl", hash = "sha256:c7751e7af83e8e80c924c2c596318d9e2535f249784a41840eaee5f4a4f49d79"},
     {url = "https://files.pythonhosted.org/packages/dd/3a/ac02011988ad013f24a11cb6123a7ff9e17a75369964c7edd9f64bfea80f/subliminal-2.1.0.tar.gz", hash = "sha256:c6439cc733a4f37f01f8c14c096d44fd28d75d1f6f6e2d1d1003b1b82c65628b"},
 ]
 "tabulate 0.9.0" = [
@@ -2647,17 +2647,17 @@
     {url = "https://files.pythonhosted.org/packages/31/25/5abcd82372d3d4a3932e1fa8c3dbf9efac10cc7c0d16e78467460571b404/typing_extensions-4.5.0-py3-none-any.whl", hash = "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"},
     {url = "https://files.pythonhosted.org/packages/d3/20/06270dac7316220643c32ae61694e451c98f8caf4c8eab3aa80a2bedf0df/typing_extensions-4.5.0.tar.gz", hash = "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb"},
 ]
 "tzdata 2023.3" = [
     {url = "https://files.pythonhosted.org/packages/70/e5/81f99b9fced59624562ab62a33df639a11b26c582be78864b339dafa420d/tzdata-2023.3.tar.gz", hash = "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a"},
     {url = "https://files.pythonhosted.org/packages/d5/fb/a79efcab32b8a1f1ddca7f35109a50e4a80d42ac1c9187ab46522b2407d7/tzdata-2023.3-py2.py3-none-any.whl", hash = "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"},
 ]
-"tzlocal 5.0" = [
-    {url = "https://files.pythonhosted.org/packages/0a/93/55e34fba4b61fd4ba30e9341edb313f474d0e18006e8400b05e36b71a7bd/tzlocal-5.0-py3-none-any.whl", hash = "sha256:c640e3fdccbb6fee1172ce211cefd3c3c04eaf2b0fbf676f0ac7958c41f373e4"},
-    {url = "https://files.pythonhosted.org/packages/23/0a/b3d3e8a9dd99e4a7789309de8ed12a625ed80efbe4f1cd4282efda88734e/tzlocal-5.0.tar.gz", hash = "sha256:f96e29a599ef562233cec21ef0d6f7065c3050d0221293e839d1ede093ab1755"},
+"tzlocal 5.0.1" = [
+    {url = "https://files.pythonhosted.org/packages/84/d2/730a87f0dbf184760394a85088d0d2366a5a8a32bc32ffd869a83f1de854/tzlocal-5.0.1-py3-none-any.whl", hash = "sha256:f3596e180296aaf2dbd97d124fe76ae3a0e3d32b258447de7b939b3fd4be992f"},
+    {url = "https://files.pythonhosted.org/packages/ee/f5/3e644f08771b242f7460438cdc0aaad4d1484c1f060f1e52f4738d342983/tzlocal-5.0.1.tar.gz", hash = "sha256:46eb99ad4bdb71f3f72b7d24f4267753e240944ecfc16f25d2719ba89827a803"},
 ]
 "update-checker 0.18.0" = [
     {url = "https://files.pythonhosted.org/packages/0c/ba/8dd7fa5f0b1c6a8ac62f8f57f7e794160c1f86f31c6d0fb00f582372a3e4/update_checker-0.18.0-py3-none-any.whl", hash = "sha256:cbba64760a36fe2640d80d85306e8fe82b6816659190993b7bdabadee4d4bbfd"},
     {url = "https://files.pythonhosted.org/packages/5c/0b/1bec4a6cc60d33ce93d11a7bcf1aeffc7ad0aa114986073411be31395c6f/update_checker-0.18.0.tar.gz", hash = "sha256:6a2d45bb4ac585884a6b03f9eade9161cedd9e8111545141e9aa9058932acb13"},
 ]
 "urllib3 1.25.11" = [
     {url = "https://files.pythonhosted.org/packages/56/aa/4ef5aa67a9a62505db124a5cb5262332d1d4153462eb8fd89c9fa41e5d92/urllib3-1.25.11-py2.py3-none-any.whl", hash = "sha256:f5321fbe4bf3fefa0efd0bfe7fb14e90909eb62a48ccda331726b4319897dd5e"},
```

### Comparing `xklb-1.27.5/readme.py` & `xklb-1.27.6/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.27.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.27.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/.github/workflows/push.yaml` & `xklb-1.27.6/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/sql/transfer.sql` & `xklb-1.27.6/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/av.py` & `xklb-1.27.6/xklb/av.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from datetime import datetime, timezone
 from typing import Dict, Optional
 
+import ffmpeg
+
 from xklb import subtitle, utils
 from xklb.consts import DBType
 from xklb.utils import combine, log, safe_unpack
 
 
 def get_subtitle_tags(args, f, streams, codec_types) -> dict:
     attachment_count = sum(1 for s in codec_types if s == "attachment")
@@ -94,30 +96,30 @@
         mutagen_tags = {}
 
     stream_tags = parse_tags(mutagen_tags, tiny_tags)
     return stream_tags
 
 
 def munge_av_tags(args, media, f) -> Optional[dict]:
-    import ffmpeg
-
     try:
         probe = ffmpeg.probe(f, show_chapters=None)
     except (KeyboardInterrupt, SystemExit) as sys_exit:
         raise SystemExit(130) from sys_exit
     except Exception as e:
         log.error(f"[{f}] Failed reading header. Metadata corruption")
         log.debug(e)
         if args.delete_unplayable:
             utils.trash(f)
         return None
 
-    if args.check_corrupt:
-        error_log = ffmpeg.input(f, loglevel="error", output=None)  # TODO: test that this actually works...
-        if error_log.returncode != 0:
+    if args.check_corrupt or args.delete_corrupt:
+        output = ffmpeg.output(ffmpeg.input(f), "/dev/null", f="null")
+        try:
+            error_log = ffmpeg.run(output, capture_stderr=True)
+        except ffmpeg.Error:
             log.warning(f"[{f}] Data corruption")
             if args.delete_corrupt:
                 utils.trash(f)
 
     if "format" not in probe:
         log.error(f"[{f}] Failed reading format")
         log.warning(probe)
```

### Comparing `xklb-1.27.5/xklb/books.py` & `xklb-1.27.6/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/consts.py` & `xklb-1.27.6/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/db.py` & `xklb-1.27.6/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/dl_config.py` & `xklb-1.27.6/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/dl_extract.py` & `xklb-1.27.6/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/fs_extract.py` & `xklb-1.27.6/xklb/fs_extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,17 @@
     parser.add_argument("--io-multiplier", default="1")
     parser.add_argument("--ocr", "--OCR", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--speech-recognition", "--speech", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--scan-subtitles", "--scan-subtitle", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--extra-media-data", default={})
     parser.add_argument("--extra-playlist-data", default={})
 
-    parser.add_argument("--delete-unplayable", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--check-corrupt", action="store_true", help=argparse.SUPPRESS)
-    parser.add_argument("--delete-corrupt", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--delete-unplayable", action="store_true")
+    parser.add_argument("--check-corrupt", action="store_true")
+    parser.add_argument("--delete-corrupt", action="store_true")
     parser.add_argument("--force", "-f", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
     parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
     if action == SC.fsadd:
         parser.add_argument("paths", nargs="+")
```

### Comparing `xklb-1.27.5/xklb/gui.py` & `xklb-1.27.6/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/hn_extract.py` & `xklb-1.27.6/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/lb.py` & `xklb-1.27.6/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/play_actions.py` & `xklb-1.27.6/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/playback.py` & `xklb-1.27.6/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/player.py` & `xklb-1.27.6/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/praw_extract.py` & `xklb-1.27.6/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/stats.py` & `xklb-1.27.6/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/subtitle.py` & `xklb-1.27.6/xklb/subtitle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 import tempfile
 from pathlib import Path
 from typing import List, Optional
 
 import ffmpeg
-from ffmpeg import Error
 
 from xklb import db, utils
 from xklb.consts import SUB_TEMP_DIR
 from xklb.utils import flatten, log, remove_consecutive_whitespace, remove_text_inside_brackets
 
 SUBTITLE_FORMATS = "vtt|srt|ssa|ass|jss|aqt|mpl2|mpsub|pjs|rt|sami|smi|stl|xml|txt|psb|ssf|usf"
 IMAGE_SUBTITLE_CODECS = ["dvbsub", "dvdsub", "pgssub", "xsub", "dvb_subtitle", "dvd_subtitle", "hdmv_pgs_subtitle"]
 
 
 def extract(video_file, stream_index) -> Optional[str]:
-    import ffmpeg
-
     Path(SUB_TEMP_DIR).mkdir(parents=True, exist_ok=True)
     temp_srt = tempfile.mktemp(".srt", dir=SUB_TEMP_DIR)
 
     stream_id = "0:" + str(stream_index)
 
     try:
         ffmpeg.input(video_file).output(temp_srt, map=stream_id).global_args("-nostdin").run(quiet=True)
-    except Error as e:
+    except ffmpeg.Error as e:
         log.info(
             f"Could not extract subtitle {stream_id} from video file. Likely incorrect subtitle character encoding set. %s",
             video_file,
         )
         log.debug(e.stderr.decode())
         return None
 
     return temp_srt
 
 
 def convert_to_srt(path) -> str:
-    import ffmpeg
-
     Path(SUB_TEMP_DIR).mkdir(parents=True, exist_ok=True)
     temp_srt = tempfile.mktemp(".srt", dir=SUB_TEMP_DIR)
     try:
         ffmpeg.input(path).output(temp_srt).global_args("-nostdin").run(quiet=True)
-    except Error as e:
+    except ffmpeg.Error as e:
         log.info("Could not convert subtitle")
         log.info(e.stderr.decode())
         raise UnicodeDecodeError("utf-8", b"Dr. John A. Zoidberg", 1, 2, "Bleh!") from e
 
     return temp_srt
```

### Comparing `xklb-1.27.5/xklb/tabs_actions.py` & `xklb-1.27.6/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/tabs_extract.py` & `xklb-1.27.6/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/tube_backend.py` & `xklb-1.27.6/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/tube_extract.py` & `xklb-1.27.6/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/utils.py` & `xklb-1.27.6/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/__init__.py` & `xklb-1.27.6/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/bigdirs.py` & `xklb-1.27.6/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/christen.py` & `xklb-1.27.6/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/copy_play_counts.py` & `xklb-1.27.6/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/dedupe.py` & `xklb-1.27.6/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/merge_dbs.py` & `xklb-1.27.6/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/merge_online_local.py` & `xklb-1.27.6/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/move_list.py` & `xklb-1.27.6/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/optimize_db.py` & `xklb-1.27.6/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/redownload.py` & `xklb-1.27.6/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/relmv.py` & `xklb-1.27.6/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/scatter.py` & `xklb-1.27.6/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/streaming_tab_loader.py` & `xklb-1.27.6/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/mining/data.py` & `xklb-1.27.6/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/mining/extract_links.py` & `xklb-1.27.6/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/mining/nouns.py` & `xklb-1.27.6/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/mining/pushshift.py` & `xklb-1.27.6/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.27.6/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/assets/kotobago.png` & `xklb-1.27.6/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/.gitignore` & `xklb-1.27.6/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/LICENSE` & `xklb-1.27.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/README.md` & `xklb-1.27.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.27.005)
+    xk media library subcommands (v1.27.006)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.27.5/pyproject.toml` & `xklb-1.27.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.27.5/PKG-INFO` & `xklb-1.27.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.27.5
+Version: 1.27.6
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -99,15 +99,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.27.005)
+    xk media library subcommands (v1.27.006)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

