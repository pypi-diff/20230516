# Comparing `tmp/python-mecab-kor-1.2.6.tar.gz` & `tmp/python-mecab-kor-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-mecab-kor-1.2.6.tar", last modified: Wed Jan  4 07:25:11 2023, max compression
+gzip compressed data, was "python-mecab-kor-1.2.7.tar", last modified: Tue May 16 18:29:57 2023, max compression
```

## Comparing `python-mecab-kor-1.2.6.tar` & `python-mecab-kor-1.2.7.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6469 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     4798 2022-12-23 04:26:48.000000 python-mecab-kor-1.2.6/README.md
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/mecab/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       78 2023-01-04 07:24:54.000000 python-mecab-kor-1.2.6/mecab/__init__.py
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     3253 2022-12-23 04:24:51.000000 python-mecab-kor-1.2.6/mecab/mecab.py
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/mecab/pybind/
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/mecab/pybind/_mecab/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      414 2022-12-23 04:10:56.000000 python-mecab-kor-1.2.6/mecab/pybind/_mecab/_mecab.cpp
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      874 2022-12-23 04:10:56.000000 python-mecab-kor-1.2.6/mecab/pybind/_mecab/dictionaryinfo.cpp
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5490 2022-12-23 04:10:56.000000 python-mecab-kor-1.2.6/mecab/pybind/_mecab/lattice.cpp
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1579 2022-12-23 04:10:56.000000 python-mecab-kor-1.2.6/mecab/pybind/_mecab/node.cpp
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      447 2022-12-23 04:10:56.000000 python-mecab-kor-1.2.6/mecab/pybind/_mecab/path.cpp
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1217 2022-12-23 04:10:56.000000 python-mecab-kor-1.2.6/mecab/pybind/_mecab/tagger.cpp
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/python_mecab_kor.egg-info/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6469 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/python_mecab_kor.egg-info/PKG-INFO
--rw-r--r--   0 hyunwoongko   (501) staff       (20)      505 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/python_mecab_kor.egg-info/SOURCES.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/python_mecab_kor.egg-info/dependency_links.txt
--rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2022-12-23 04:27:02.000000 python-mecab-kor-1.2.6/python_mecab_kor.egg-info/not-zip-safe
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       13 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/python_mecab_kor.egg-info/top_level.txt
-drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/scripts/
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     5443 2022-12-23 04:28:26.000000 python-mecab-kor-1.2.6/scripts/install_mecab_ko_dic.sh
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     1230 2023-01-04 07:24:32.000000 python-mecab-kor-1.2.6/scripts/install_requirements.sh
--rw-r--r--   0 hyunwoongko   (501) staff       (20)       38 2023-01-04 07:25:11.000000 python-mecab-kor-1.2.6/setup.cfg
--rw-r--r--   0 hyunwoongko   (501) staff       (20)     6886 2022-12-23 04:25:35.000000 python-mecab-kor-1.2.6/setup.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-16 18:29:57.133187 python-mecab-kor-1.2.7/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1490 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/LICENSE
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5564 2023-05-16 18:29:57.133056 python-mecab-kor-1.2.7/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     4798 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/README.md
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-16 18:29:57.131045 python-mecab-kor-1.2.7/mecab/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       78 2023-05-16 18:29:39.000000 python-mecab-kor-1.2.7/mecab/__init__.py
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     3253 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/mecab/mecab.py
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-16 18:29:57.130286 python-mecab-kor-1.2.7/mecab/pybind/
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-16 18:29:57.132013 python-mecab-kor-1.2.7/mecab/pybind/_mecab/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      414 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/mecab/pybind/_mecab/_mecab.cpp
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      874 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/mecab/pybind/_mecab/dictionaryinfo.cpp
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5490 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/mecab/pybind/_mecab/lattice.cpp
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1579 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/mecab/pybind/_mecab/node.cpp
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      447 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/mecab/pybind/_mecab/path.cpp
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1217 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/mecab/pybind/_mecab/tagger.cpp
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-16 18:29:57.132650 python-mecab-kor-1.2.7/python_mecab_kor.egg-info/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5564 2023-05-16 18:29:57.000000 python-mecab-kor-1.2.7/python_mecab_kor.egg-info/PKG-INFO
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)      513 2023-05-16 18:29:57.000000 python-mecab-kor-1.2.7/python_mecab_kor.egg-info/SOURCES.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2023-05-16 18:29:57.000000 python-mecab-kor-1.2.7/python_mecab_kor.egg-info/dependency_links.txt
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)        1 2023-05-16 18:28:53.000000 python-mecab-kor-1.2.7/python_mecab_kor.egg-info/not-zip-safe
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       13 2023-05-16 18:29:57.000000 python-mecab-kor-1.2.7/python_mecab_kor.egg-info/top_level.txt
+drwxr-xr-x   0 hyunwoongko   (501) staff       (20)        0 2023-05-16 18:29:57.132887 python-mecab-kor-1.2.7/scripts/
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     5443 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/scripts/install_mecab_ko_dic.sh
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     1218 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/scripts/install_requirements.sh
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)       38 2023-05-16 18:29:57.133224 python-mecab-kor-1.2.7/setup.cfg
+-rw-r--r--   0 hyunwoongko   (501) staff       (20)     6886 2023-05-16 18:28:44.000000 python-mecab-kor-1.2.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-mecab-kor-1.2.6/PKG-INFO` & `python-mecab-kor-1.2.7/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,133 +1,112 @@
-Metadata-Version: 2.1
-Name: python-mecab-kor
-Version: 1.2.6
-Summary: Yet another python binding for mecab-ko
-Home-page: https://github.com/hyunwoongko/python-mecab-kor
-Author: Hyunwoong Ko
-Author-email: gusdnd852@gmail.com
-License: BSD
-Description: # python-mecab-kor
-        <a href="https://github.com/hyunwoongko/python-mecab-kor/releases"><img alt="GitHub release" src="https://img.shields.io/github/release/hyunwoongko/python-mecab-kor.svg" /></a>
-        <a href="https://github.com/hyunwoongko/python-mecab-kor/issues"><img alt="Issues" src="https://img.shields.io/github/issues/hyunwoongko/python-mecab-kor"/></a>
-        
-        ## 1. Why another package? 
-        [python-mecab-ko](https://github.com/jonghwanhyeon/python-mecab-ko) is great package but sadly it is not being maintained well now.
-        So I decided to maintain it myself and I've fixed a lot of problems about installation.
-        Be careful that the package name is changed `ko` to `kor` because I can't keep the package name same with the original.
-        
-        ## 2. What OS have you tested successfully so far?
-        It has been successfully installed on the following OS list.
-        If the installation succeeds or fails on your OS, please report it through the [issue page](https://github.com/hyunwoongko/python-mecab-kor/issues). 
-        I will do my best to fix your errors. 
-        
-        - Linux Ubuntu
-        - Linux CentOS
-        - Amazon Linux
-        - Mac OS
-        
-        **Please note that I don't have any plan with Windows OS.**
-        
-        ## 3. Installation
-        ```
-        pip install python-mecab-kor
-        ```
-        
-        ## 4. Usage
-        
-        ```python
-        from mecab import MeCab
-        
-        mecab = MeCab()
-        
-        mecab.morphs('영등포구청역에 있는 맛집 좀 알려주세요.')
-        # ['영등포구청역', '에', '있', '는', '맛집', '좀', '알려', '주', '세요', '.']
-        
-        # drop_space=False
-        mecab.morphs('영등포구청역에 있는 맛집 좀 알려주세요.', drop_space=False)
-        # ['영등포구청역', '에', ' ', '있', '는', ' ', '맛집', ' ', '좀', ' ', '알려', '주', '세요', '.']
-        
-        mecab.nouns('우리나라에는 무릎 치료를 잘하는 정형외과가 없는가!')
-        # ['우리', '나라', '무릎', '치료', '정형외과']
-        
-        mecab.pos('자연주의 쇼핑몰은 어떤 곳인가?')
-        # [('자연주의', 'NNG'), ('쇼핑몰', 'NNG'), ('은', 'JX'), ('어떤', 'MM'), ('곳', 'NNG'), ('인가', 'VCP+EF'), ('?', 'SF')]
-        
-        # drop_space=False
-        mecab.pos('자연주의 쇼핑몰은 어떤 곳인가?', drop_space=False)
-        # [('자연주의', 'NNG'), (' ', 'SP'), ('쇼핑몰', 'NNG'), ('은', 'JX'), (' ', 'SP'), ('어떤', 'MM'), (' ', 'SP'), ('곳', 'NNG'), ('인가', 'VCP+EF'), ('?', 'SF')]
-        
-        mecab.parse('즐거운 하루\n보내세요!')
-        # [
-        #     ('즐거운', Feature(
-        #         pos='VA+ETM', semantic=None, has_jongseong=True, reading='즐거운',
-        #         type='Inflect', start_pos='VA', end_pos='ETM',
-        #         expression='즐겁/VA/*+ᆫ/ETM/*')),
-        #     ('하루', Feature(
-        #         pos='NNG', semantic=None, has_jongseong=False, reading='하루',
-        #         type=None, start_pos=None, end_pos=None,
-        #         expression=None)),
-        #     ('보내', Feature(
-        #         pos='VV', semantic=None, has_jongseong=False, reading='보내',
-        #         type=None, start_pos=None, end_pos=None,
-        #         expression=None)),
-        #     ('세요', Feature(
-        #         pos='EP+EF', semantic=None, has_jongseong=False, reading='세요',
-        #         type='Inflect', start_pos='EP', end_pos='EF',
-        #         expression='시/EP/*+어요/EF/*')),
-        #     ('!', Feature(
-        #         pos='SF', semantic=None, has_jongseong=None, reading=None,
-        #         type=None, start_pos=None, end_pos=None,
-        #         expression=None))
-        # ]
-        
-        # drop_space=False
-        mecab.parse('즐거운 하루\n보내세요!', drop_space=False)
-        # [
-        #     ('즐거운', Feature(
-        #         pos='VA+ETM', semantic=None, has_jongseong=True, reading='즐거운',
-        #         type='Inflect', start_pos='VA', end_pos='ETM',
-        #         expression='즐겁/VA/*+ᆫ/ETM/*')),
-        #     (' ', Feature(
-        #         pos='SP', semantic=None, has_jongseong=None, reading=None,
-        #         type=None, start_pos=None, end_pos=None,
-        #         expression=None)),
-        #     ('하루', Feature(
-        #         pos='NNG', semantic=None, has_jongseong=False, reading='하루',
-        #         type=None, start_pos=None, end_pos=None,
-        #         expression=None)),
-        #     ('\n', Feature(
-        #         pos='SP', semantic=None, has_jongseong=None, reading=None,
-        #         type=None, start_pos=None, end_pos=None,
-        #         expression=None)),
-        #     ('보내', Feature(
-        #         pos='VV', semantic=None, has_jongseong=False, reading='보내',
-        #         type=None, start_pos=None, end_pos=None,
-        #         expression=None)),
-        #     ('세요', Feature(
-        #         pos='EP+EF', semantic=None, has_jongseong=False, reading='세요',
-        #         type='Inflect', start_pos='EP', end_pos='EF',
-        #         expression='시/EP/*+어요/EF/*')),
-        #     ('!', Feature(
-        #         pos='SF', semantic=None, has_jongseong=None, reading=None,
-        #         type=None, start_pos=None, end_pos=None,
-        #         expression=None))
-        # ]
-        
-        ```
-        
-        ## 5. References
-        - [konlpy](https://github.com/konlpy/konlpy/)
-        - [python-mecab-ko](https://github.com/jonghwanhyeon/python-mecab-ko)
-        
-Keywords: mecab mecab-ko python-mecab python-mecab-ko python-mecab-kor
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Natural Language :: Korean
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Text Processing
-Classifier: Topic :: Text Processing :: Linguistic
-Requires-Python: >=3
-Description-Content-Type: text/markdown
+# python-mecab-kor
+<a href="https://github.com/hyunwoongko/python-mecab-kor/releases"><img alt="GitHub release" src="https://img.shields.io/github/release/hyunwoongko/python-mecab-kor.svg" /></a>
+<a href="https://github.com/hyunwoongko/python-mecab-kor/issues"><img alt="Issues" src="https://img.shields.io/github/issues/hyunwoongko/python-mecab-kor"/></a>
+
+## 1. Why another package? 
+[python-mecab-ko](https://github.com/jonghwanhyeon/python-mecab-ko) is great package but sadly it is not being maintained well now.
+So I decided to maintain it myself and I've fixed a lot of problems about installation.
+Be careful that the package name is changed `ko` to `kor` because I can't keep the package name same with the original.
+
+## 2. What OS have you tested successfully so far?
+It has been successfully installed on the following OS list.
+If the installation succeeds or fails on your OS, please report it through the [issue page](https://github.com/hyunwoongko/python-mecab-kor/issues). 
+I will do my best to fix your errors. 
+
+- Linux Ubuntu
+- Linux CentOS
+- Amazon Linux
+- Mac OS
+
+**Please note that I don't have any plan with Windows OS.**
+
+## 3. Installation
+```
+pip install python-mecab-kor
+```
+
+## 4. Usage
+
+```python
+from mecab import MeCab
+
+mecab = MeCab()
+
+mecab.morphs('영등포구청역에 있는 맛집 좀 알려주세요.')
+# ['영등포구청역', '에', '있', '는', '맛집', '좀', '알려', '주', '세요', '.']
+
+# drop_space=False
+mecab.morphs('영등포구청역에 있는 맛집 좀 알려주세요.', drop_space=False)
+# ['영등포구청역', '에', ' ', '있', '는', ' ', '맛집', ' ', '좀', ' ', '알려', '주', '세요', '.']
+
+mecab.nouns('우리나라에는 무릎 치료를 잘하는 정형외과가 없는가!')
+# ['우리', '나라', '무릎', '치료', '정형외과']
+
+mecab.pos('자연주의 쇼핑몰은 어떤 곳인가?')
+# [('자연주의', 'NNG'), ('쇼핑몰', 'NNG'), ('은', 'JX'), ('어떤', 'MM'), ('곳', 'NNG'), ('인가', 'VCP+EF'), ('?', 'SF')]
+
+# drop_space=False
+mecab.pos('자연주의 쇼핑몰은 어떤 곳인가?', drop_space=False)
+# [('자연주의', 'NNG'), (' ', 'SP'), ('쇼핑몰', 'NNG'), ('은', 'JX'), (' ', 'SP'), ('어떤', 'MM'), (' ', 'SP'), ('곳', 'NNG'), ('인가', 'VCP+EF'), ('?', 'SF')]
+
+mecab.parse('즐거운 하루\n보내세요!')
+# [
+#     ('즐거운', Feature(
+#         pos='VA+ETM', semantic=None, has_jongseong=True, reading='즐거운',
+#         type='Inflect', start_pos='VA', end_pos='ETM',
+#         expression='즐겁/VA/*+ᆫ/ETM/*')),
+#     ('하루', Feature(
+#         pos='NNG', semantic=None, has_jongseong=False, reading='하루',
+#         type=None, start_pos=None, end_pos=None,
+#         expression=None)),
+#     ('보내', Feature(
+#         pos='VV', semantic=None, has_jongseong=False, reading='보내',
+#         type=None, start_pos=None, end_pos=None,
+#         expression=None)),
+#     ('세요', Feature(
+#         pos='EP+EF', semantic=None, has_jongseong=False, reading='세요',
+#         type='Inflect', start_pos='EP', end_pos='EF',
+#         expression='시/EP/*+어요/EF/*')),
+#     ('!', Feature(
+#         pos='SF', semantic=None, has_jongseong=None, reading=None,
+#         type=None, start_pos=None, end_pos=None,
+#         expression=None))
+# ]
+
+# drop_space=False
+mecab.parse('즐거운 하루\n보내세요!', drop_space=False)
+# [
+#     ('즐거운', Feature(
+#         pos='VA+ETM', semantic=None, has_jongseong=True, reading='즐거운',
+#         type='Inflect', start_pos='VA', end_pos='ETM',
+#         expression='즐겁/VA/*+ᆫ/ETM/*')),
+#     (' ', Feature(
+#         pos='SP', semantic=None, has_jongseong=None, reading=None,
+#         type=None, start_pos=None, end_pos=None,
+#         expression=None)),
+#     ('하루', Feature(
+#         pos='NNG', semantic=None, has_jongseong=False, reading='하루',
+#         type=None, start_pos=None, end_pos=None,
+#         expression=None)),
+#     ('\n', Feature(
+#         pos='SP', semantic=None, has_jongseong=None, reading=None,
+#         type=None, start_pos=None, end_pos=None,
+#         expression=None)),
+#     ('보내', Feature(
+#         pos='VV', semantic=None, has_jongseong=False, reading='보내',
+#         type=None, start_pos=None, end_pos=None,
+#         expression=None)),
+#     ('세요', Feature(
+#         pos='EP+EF', semantic=None, has_jongseong=False, reading='세요',
+#         type='Inflect', start_pos='EP', end_pos='EF',
+#         expression='시/EP/*+어요/EF/*')),
+#     ('!', Feature(
+#         pos='SF', semantic=None, has_jongseong=None, reading=None,
+#         type=None, start_pos=None, end_pos=None,
+#         expression=None))
+# ]
+
+```
+
+## 5. References
+- [konlpy](https://github.com/konlpy/konlpy/)
+- [python-mecab-ko](https://github.com/jonghwanhyeon/python-mecab-ko)
```

#### html2text {}

```diff
@@ -1,49 +1,46 @@
-Metadata-Version: 2.1 Name: python-mecab-kor Version: 1.2.6 Summary: Yet
-another python binding for mecab-ko Home-page: https://github.com/hyunwoongko/
-python-mecab-kor Author: Hyunwoong Ko Author-email: gusdnd852@gmail.com
-License: BSD Description: # python-mecab-kor [GitHub_release] [Issues] ## 1.
-Why another package? [python-mecab-ko](https://github.com/jonghwanhyeon/python-
-mecab-ko) is great package but sadly it is not being maintained well now. So I
-decided to maintain it myself and I've fixed a lot of problems about
-installation. Be careful that the package name is changed `ko` to `kor` because
-I can't keep the package name same with the original. ## 2. What OS have you
-tested successfully so far? It has been successfully installed on the following
-OS list. If the installation succeeds or fails on your OS, please report it
-through the [issue page](https://github.com/hyunwoongko/python-mecab-kor/
-issues). I will do my best to fix your errors. - Linux Ubuntu - Linux CentOS -
-Amazon Linux - Mac OS **Please note that I don't have any plan with Windows
-OS.** ## 3. Installation ``` pip install python-mecab-kor ``` ## 4. Usage
-```python from mecab import MeCab mecab = MeCab() mecab.morphs
-('ìë±í¬êµ¬ì²­ì­ì ìë ë§ì§ ì¢ ìë ¤ì£¼ì¸ì.') #
-['ìë±í¬êµ¬ì²­ì­', 'ì', 'ì', 'ë', 'ë§ì§', 'ì¢', 'ìë ¤', 'ì£¼',
-'ì¸ì', '.'] # drop_space=False mecab.morphs('ìë±í¬êµ¬ì²­ì­ì ìë
-ë§ì§ ì¢ ìë ¤ì£¼ì¸ì.', drop_space=False) # ['ìë±í¬êµ¬ì²­ì­', 'ì',
-' ', 'ì', 'ë', ' ', 'ë§ì§', ' ', 'ì¢', ' ', 'ìë ¤', 'ì£¼', 'ì¸ì',
-'.'] mecab.nouns('ì°ë¦¬ëë¼ìë ë¬´ë¦ ì¹ë£ë¥¼ ìíë ì íì¸ê³¼ê°
-ìëê°!') # ['ì°ë¦¬', 'ëë¼', 'ë¬´ë¦', 'ì¹ë£', 'ì íì¸ê³¼']
-mecab.pos('ìì°ì£¼ì ì¼íëª°ì ì´ë¤ ê³³ì¸ê°?') # [('ìì°ì£¼ì',
-'NNG'), ('ì¼íëª°', 'NNG'), ('ì', 'JX'), ('ì´ë¤', 'MM'), ('ê³³', 'NNG'),
-('ì¸ê°', 'VCP+EF'), ('?', 'SF')] # drop_space=False mecab.pos('ìì°ì£¼ì
-ì¼íëª°ì ì´ë¤ ê³³ì¸ê°?', drop_space=False) # [('ìì°ì£¼ì', 'NNG'),
-(' ', 'SP'), ('ì¼íëª°', 'NNG'), ('ì', 'JX'), (' ', 'SP'), ('ì´ë¤',
-'MM'), (' ', 'SP'), ('ê³³', 'NNG'), ('ì¸ê°', 'VCP+EF'), ('?', 'SF')]
-mecab.parse('ì¦ê±°ì´ íë£¨\në³´ë´ì¸ì!') # [ # ('ì¦ê±°ì´', Feature( #
-pos='VA+ETM', semantic=None, has_jongseong=True, reading='ì¦ê±°ì´', #
-type='Inflect', start_pos='VA', end_pos='ETM', # expression='ì¦ê²/VA/*+á«/
-ETM/*')), # ('íë£¨', Feature( # pos='NNG', semantic=None,
-has_jongseong=False, reading='íë£¨', # type=None, start_pos=None,
-end_pos=None, # expression=None)), # ('ë³´ë´', Feature( # pos='VV',
-semantic=None, has_jongseong=False, reading='ë³´ë´', # type=None,
-start_pos=None, end_pos=None, # expression=None)), # ('ì¸ì', Feature( #
-pos='EP+EF', semantic=None, has_jongseong=False, reading='ì¸ì', #
-type='Inflect', start_pos='EP', end_pos='EF', # expression='ì/EP/*+ì´ì/EF/
-*')), # ('!', Feature( # pos='SF', semantic=None, has_jongseong=None,
-reading=None, # type=None, start_pos=None, end_pos=None, # expression=None)) #
-] # drop_space=False mecab.parse('ì¦ê±°ì´ íë£¨\në³´ë´ì¸ì!',
+# python-mecab-kor [GitHub_release] [Issues] ## 1. Why another package?
+[python-mecab-ko](https://github.com/jonghwanhyeon/python-mecab-ko) is great
+package but sadly it is not being maintained well now. So I decided to maintain
+it myself and I've fixed a lot of problems about installation. Be careful that
+the package name is changed `ko` to `kor` because I can't keep the package name
+same with the original. ## 2. What OS have you tested successfully so far? It
+has been successfully installed on the following OS list. If the installation
+succeeds or fails on your OS, please report it through the [issue page](https:/
+/github.com/hyunwoongko/python-mecab-kor/issues). I will do my best to fix your
+errors. - Linux Ubuntu - Linux CentOS - Amazon Linux - Mac OS **Please note
+that I don't have any plan with Windows OS.** ## 3. Installation ``` pip
+install python-mecab-kor ``` ## 4. Usage ```python from mecab import MeCab
+mecab = MeCab() mecab.morphs('ìë±í¬êµ¬ì²­ì­ì ìë ë§ì§ ì¢
+ìë ¤ì£¼ì¸ì.') # ['ìë±í¬êµ¬ì²­ì­', 'ì', 'ì', 'ë', 'ë§ì§',
+'ì¢', 'ìë ¤', 'ì£¼', 'ì¸ì', '.'] # drop_space=False mecab.morphs
+('ìë±í¬êµ¬ì²­ì­ì ìë ë§ì§ ì¢ ìë ¤ì£¼ì¸ì.', drop_space=False)
+# ['ìë±í¬êµ¬ì²­ì­', 'ì', ' ', 'ì', 'ë', ' ', 'ë§ì§', ' ', 'ì¢', '
+', 'ìë ¤', 'ì£¼', 'ì¸ì', '.'] mecab.nouns('ì°ë¦¬ëë¼ìë ë¬´ë¦
+ì¹ë£ë¥¼ ìíë ì íì¸ê³¼ê° ìëê°!') # ['ì°ë¦¬', 'ëë¼',
+'ë¬´ë¦', 'ì¹ë£', 'ì íì¸ê³¼'] mecab.pos('ìì°ì£¼ì ì¼íëª°ì ì´ë¤
+ê³³ì¸ê°?') # [('ìì°ì£¼ì', 'NNG'), ('ì¼íëª°', 'NNG'), ('ì', 'JX'),
+('ì´ë¤', 'MM'), ('ê³³', 'NNG'), ('ì¸ê°', 'VCP+EF'), ('?', 'SF')] #
+drop_space=False mecab.pos('ìì°ì£¼ì ì¼íëª°ì ì´ë¤ ê³³ì¸ê°?',
+drop_space=False) # [('ìì°ì£¼ì', 'NNG'), (' ', 'SP'), ('ì¼íëª°',
+'NNG'), ('ì', 'JX'), (' ', 'SP'), ('ì´ë¤', 'MM'), (' ', 'SP'), ('ê³³',
+'NNG'), ('ì¸ê°', 'VCP+EF'), ('?', 'SF')] mecab.parse('ì¦ê±°ì´
+íë£¨\në³´ë´ì¸ì!') # [ # ('ì¦ê±°ì´', Feature( # pos='VA+ETM',
+semantic=None, has_jongseong=True, reading='ì¦ê±°ì´', # type='Inflect',
+start_pos='VA', end_pos='ETM', # expression='ì¦ê²/VA/*+á«/ETM/*')), #
+('íë£¨', Feature( # pos='NNG', semantic=None, has_jongseong=False,
+reading='íë£¨', # type=None, start_pos=None, end_pos=None, #
+expression=None)), # ('ë³´ë´', Feature( # pos='VV', semantic=None,
+has_jongseong=False, reading='ë³´ë´', # type=None, start_pos=None,
+end_pos=None, # expression=None)), # ('ì¸ì', Feature( # pos='EP+EF',
+semantic=None, has_jongseong=False, reading='ì¸ì', # type='Inflect',
+start_pos='EP', end_pos='EF', # expression='ì/EP/*+ì´ì/EF/*')), # ('!',
+Feature( # pos='SF', semantic=None, has_jongseong=None, reading=None, #
+type=None, start_pos=None, end_pos=None, # expression=None)) # ] #
+drop_space=False mecab.parse('ì¦ê±°ì´ íë£¨\në³´ë´ì¸ì!',
 drop_space=False) # [ # ('ì¦ê±°ì´', Feature( # pos='VA+ETM', semantic=None,
 has_jongseong=True, reading='ì¦ê±°ì´', # type='Inflect', start_pos='VA',
 end_pos='ETM', # expression='ì¦ê²/VA/*+á«/ETM/*')), # (' ', Feature( #
 pos='SP', semantic=None, has_jongseong=None, reading=None, # type=None,
 start_pos=None, end_pos=None, # expression=None)), # ('íë£¨', Feature( #
 pos='NNG', semantic=None, has_jongseong=False, reading='íë£¨', # type=None,
 start_pos=None, end_pos=None, # expression=None)), # ('\n', Feature( #
@@ -52,15 +49,8 @@
 pos='VV', semantic=None, has_jongseong=False, reading='ë³´ë´', # type=None,
 start_pos=None, end_pos=None, # expression=None)), # ('ì¸ì', Feature( #
 pos='EP+EF', semantic=None, has_jongseong=False, reading='ì¸ì', #
 type='Inflect', start_pos='EP', end_pos='EF', # expression='ì/EP/*+ì´ì/EF/
 *')), # ('!', Feature( # pos='SF', semantic=None, has_jongseong=None,
 reading=None, # type=None, start_pos=None, end_pos=None, # expression=None)) #
 ] ``` ## 5. References - [konlpy](https://github.com/konlpy/konlpy/) - [python-
-mecab-ko](https://github.com/jonghwanhyeon/python-mecab-ko) Keywords: mecab
-mecab-ko python-mecab python-mecab-ko python-mecab-kor Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
-Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
-Natural Language :: Korean Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
-Text Processing Classifier: Topic :: Text Processing :: Linguistic Requires-
-Python: >=3 Description-Content-Type: text/markdown
+mecab-ko](https://github.com/jonghwanhyeon/python-mecab-ko)
```

### Comparing `python-mecab-kor-1.2.6/README.md` & `python-mecab-kor-1.2.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: python-mecab-kor
+Version: 1.2.7
+Summary: Yet another python binding for mecab-ko
+Home-page: https://github.com/hyunwoongko/python-mecab-kor
+Author: Hyunwoong Ko
+Author-email: gusdnd852@gmail.com
+License: BSD
+Keywords: mecab mecab-ko python-mecab python-mecab-ko python-mecab-kor
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: Korean
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: Linguistic
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # python-mecab-kor
 <a href="https://github.com/hyunwoongko/python-mecab-kor/releases"><img alt="GitHub release" src="https://img.shields.io/github/release/hyunwoongko/python-mecab-kor.svg" /></a>
 <a href="https://github.com/hyunwoongko/python-mecab-kor/issues"><img alt="Issues" src="https://img.shields.io/github/issues/hyunwoongko/python-mecab-kor"/></a>
 
 ## 1. Why another package? 
 [python-mecab-ko](https://github.com/jonghwanhyeon/python-mecab-ko) is great package but sadly it is not being maintained well now.
 So I decided to maintain it myself and I've fixed a lot of problems about installation.
```

#### html2text {}

```diff
@@ -1,8 +1,18 @@
-# python-mecab-kor [GitHub_release] [Issues] ## 1. Why another package?
+Metadata-Version: 2.1 Name: python-mecab-kor Version: 1.2.7 Summary: Yet
+another python binding for mecab-ko Home-page: https://github.com/hyunwoongko/
+python-mecab-kor Author: Hyunwoong Ko Author-email: gusdnd852@gmail.com
+License: BSD Keywords: mecab mecab-ko python-mecab python-mecab-ko python-
+mecab-kor Classifier: Development Status :: 4 - Beta Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: Korean Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
+Topic :: Text Processing Classifier: Topic :: Text Processing :: Linguistic
+Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
+LICENSE # python-mecab-kor [GitHub_release] [Issues] ## 1. Why another package?
 [python-mecab-ko](https://github.com/jonghwanhyeon/python-mecab-ko) is great
 package but sadly it is not being maintained well now. So I decided to maintain
 it myself and I've fixed a lot of problems about installation. Be careful that
 the package name is changed `ko` to `kor` because I can't keep the package name
 same with the original. ## 2. What OS have you tested successfully so far? It
 has been successfully installed on the following OS list. If the installation
 succeeds or fails on your OS, please report it through the [issue page](https:/
```

### Comparing `python-mecab-kor-1.2.6/mecab/mecab.py` & `python-mecab-kor-1.2.7/mecab/mecab.py`

 * *Files identical despite different names*

### Comparing `python-mecab-kor-1.2.6/mecab/pybind/_mecab/dictionaryinfo.cpp` & `python-mecab-kor-1.2.7/mecab/pybind/_mecab/dictionaryinfo.cpp`

 * *Files identical despite different names*

### Comparing `python-mecab-kor-1.2.6/mecab/pybind/_mecab/lattice.cpp` & `python-mecab-kor-1.2.7/mecab/pybind/_mecab/lattice.cpp`

 * *Files identical despite different names*

### Comparing `python-mecab-kor-1.2.6/mecab/pybind/_mecab/node.cpp` & `python-mecab-kor-1.2.7/mecab/pybind/_mecab/node.cpp`

 * *Files identical despite different names*

### Comparing `python-mecab-kor-1.2.6/mecab/pybind/_mecab/tagger.cpp` & `python-mecab-kor-1.2.7/mecab/pybind/_mecab/tagger.cpp`

 * *Files identical despite different names*

### Comparing `python-mecab-kor-1.2.6/scripts/install_mecab_ko_dic.sh` & `python-mecab-kor-1.2.7/scripts/install_mecab_ko_dic.sh`

 * *Files identical despite different names*

### Comparing `python-mecab-kor-1.2.6/scripts/install_requirements.sh` & `python-mecab-kor-1.2.7/scripts/install_requirements.sh`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     elif [ "$os" == "Darwin" ]; then
         if [[ $(command -v brew) == "" ]]; then
             echo "This script require Homebrew!"
             echo "Try https://brew.sh/"
             exit 0
         fi
         if [[ $(uname -m) == 'arm64' ]]; then
-          $sudo arch -arm64 brew install curl git
+          arch -arm64 brew install curl git
         else
-          $sudo brew install curl git
+          brew install curl git
         fi
     fi
 }
 
 install_requirements
```

### Comparing `python-mecab-kor-1.2.6/setup.py` & `python-mecab-kor-1.2.7/setup.py`

 * *Files identical despite different names*

