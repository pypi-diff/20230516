# Comparing `tmp/miditok-2.0.5.tar.gz` & `tmp/miditok-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miditok-2.0.5.tar", last modified: Thu May  4 16:33:33 2023, max compression
+gzip compressed data, was "miditok-2.0.6.tar", last modified: Tue May 16 18:41:54 2023, max compression
```

## Comparing `miditok-2.0.5.tar` & `miditok-2.0.6.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.896236 miditok-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-04 16:33:14.000000 miditok-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-04 16:33:33.896236 miditok-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-04 16:33:14.000000 miditok-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.892236 miditok-2.0.5/miditok/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15114 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.892236 miditok-2.0.5/miditok/data_augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/data_augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23080 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/data_augmentation/data_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    86192 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/midi_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.896236 miditok-2.0.5/miditok/tokenizations/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/cp_word.py
--rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/midi_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/mumidi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/octuple.py
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/octuple_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/remi.py
--rw-r--r--   0 runner    (1001) docker     (123)    28075 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/remi_plus.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/structured.py
--rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/tokenizations/tsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.896236 miditok-2.0.5/miditok/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-05-04 16:33:14.000000 miditok-2.0.5/miditok/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.892236 miditok-2.0.5/miditok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-04 16:33:33.000000 miditok-2.0.5/miditok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-04 16:33:33.000000 miditok-2.0.5/miditok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 16:33:33.000000 miditok-2.0.5/miditok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-04 16:33:33.000000 miditok-2.0.5/miditok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 16:33:33.000000 miditok-2.0.5/miditok.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 16:33:33.896236 miditok-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-04 16:33:14.000000 miditok-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 16:33:33.896236 miditok-2.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_bpe_slow.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_multitrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_one_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_saving_loading_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-04 16:33:14.000000 miditok-2.0.5/tests/tests_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.109077 miditok-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-16 18:41:43.000000 miditok-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-05-16 18:41:54.109077 miditok-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-16 18:41:43.000000 miditok-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.105077 miditok-2.0.6/miditok/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.105077 miditok-2.0.6/miditok/data_augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/data_augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23080 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/data_augmentation/data_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86231 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/midi_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.109077 miditok-2.0.6/miditok/tokenizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/cp_word.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/midi_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/mmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/mumidi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/octuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/octuple_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/remi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28157 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/remi_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/tsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.109077 miditok-2.0.6/miditok/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.105077 miditok-2.0.6/miditok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-05-16 18:41:54.000000 miditok-2.0.6/miditok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-16 18:41:54.000000 miditok-2.0.6/miditok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:41:54.000000 miditok-2.0.6/miditok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 18:41:54.000000 miditok-2.0.6/miditok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 18:41:54.000000 miditok-2.0.6/miditok.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:41:54.109077 miditok-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 18:41:43.000000 miditok-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.109077 miditok-2.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_bpe_slow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_multitrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_one_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_saving_loading_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/tests_utils.py
```

### Comparing `miditok-2.0.5/LICENSE` & `miditok-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/PKG-INFO` & `miditok-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.0.5
+Version: 2.0.6
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -17,37 +17,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MidiTok
 
 Python package to tokenize MIDI music files, presented at the ISMIR 2021 LBD.
 
+![MidiTok Logo](docs/assets/logo.png?raw=true "")
+
 [![PyPI version fury.io](https://badge.fury.io/py/miditok.svg)](https://pypi.python.org/pypi/miditok/)
 [![Python 3.7](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/)
 [![Documentation Status](https://readthedocs.org/projects/miditok/badge/?version=latest)](https://miditok.readthedocs.io/en/latest/?badge=latest)
 [![GitHub CI](https://github.com/Natooz/MidiTok/actions/workflows/pytest.yml/badge.svg)](https://github.com/Natooz/MidiTok/actions/workflows/pytest.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/Natooz/MidiTok)](https://codecov.io/gh/Natooz/MidiTok)
 [![GitHub license](https://img.shields.io/github/license/Natooz/MidiTok.svg)](https://github.com/Natooz/MidiTok/blob/main/LICENSE)
 [![Downloads](https://pepy.tech/badge/MidiTok)](https://pepy.tech/project/MidiTok)
 [![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-![MidiTok Logo](docs/assets/logo.png?raw=true "")
-
-
-Using Deep Learning with symbolic music ? Then MidiTok can take care of converting your MIDI files into tokens, ready to be fed to models such as Transformer, for any generation, transcription or MIR task.
-MidiTok features most known [MIDI tokenizations](https://miditok.readthedocs.io/en/latest/tokenizations.html) (e.g. [REMI](https://arxiv.org/abs/2002.00212), [Compound Word](https://arxiv.org/abs/2101.02402)...), and is built around the idea that they all share common parameters and methods. It supports Byte Pair Encoding (BPE) and data augmentation.
+Using Deep Learning with symbolic music ? MidiTok can take care of converting (tokenizing) your MIDI files into tokens, ready to be fed to models such as Transformer, for any generation, transcription or MIR task.
+MidiTok features most known [MIDI tokenizations](https://miditok.readthedocs.io/en/latest/tokenizations.html) (e.g. [REMI](https://arxiv.org/abs/2002.00212), [Compound Word](https://arxiv.org/abs/2101.02402)...), and is built around the idea that they all share common parameters and methods. It supports [Byte Pair Encoding (BPE)](https://arxiv.org/abs/2301.11975) and data augmentation.
 
 **Documentation:** [miditok.readthedocs.com](https://miditok.readthedocs.io/en/latest/index.html)
 
 ## Install
 
 ```shell
 pip install miditok
 ```
-MidiTok uses [MIDIToolkit](https://github.com/YatingMusic/miditoolkit), which itself uses [Mido](https://github.com/mido/mido) to read and write MIDI files, and BPE is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for super fast encoding.
+MidiTok uses [MIDIToolkit](https://github.com/YatingMusic/miditoolkit), which itself uses [Mido](https://github.com/mido/mido) to read and write MIDI files, and BPE is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for super-fast encoding.
 
 ## Usage example
 
 The most basic and useful methods are summarized here. And [here](colab-notebooks/Full_Example_HuggingFace_GPT2_Transformer.ipynb) is a simple notebook example showing how to use Hugging Face models to generate music, with MidiTok taking care of tokenizing MIDIs.
 
 ```python
 from miditok import REMI
@@ -90,27 +89,28 @@
 * [REMI+](https://openreview.net/forum?id=NyR8OZFHw6i)
 * [MIDI-Like](https://link.springer.com/article/10.1007/s00521-018-3758-9)
 * [TSD](https://arxiv.org/abs/2301.11975)
 * [Structured](https://arxiv.org/abs/2107.05944)
 * [CPWord](https://ojs.aaai.org/index.php/AAAI/article/view/16091)
 * [Octuple](https://aclanthology.org/2021.findings-acl.70)
 * [MuMIDI](https://dl.acm.org/doi/10.1145/3394171.3413721)
+* [MMM](https://arxiv.org/abs/2008.06048)
 
 You can find short presentations in the [documentation](https://miditok.readthedocs.io/en/latest/tokenizations.html).
 
 ## Limitations
 
 Tokenizations using Bar tokens (REMI, Compound Word and MuMIDI) **only considers a 4/x time signature** for now. This means that each bar is considered covering 4 beats.
 REMI+ and Octuple support it.
 
 ## Contributions
 
 Contributions are gratefully welcomed, feel free to open an issue or send a PR if you want to add a tokenization or speed up the code. You can read the [contribution guide](CONTRIBUTING.md) for details.
 
-### Todo
+### Todos
 
 * Extend Time Signature to all tokenizations
 * Control Change messages
 * Option to represent pitch values as pitch intervals, as [it seems to improve performances](https://ismir2022program.ismir.net/lbd_369.html).
 * Speeding up MIDI read / load (Rust / C++ binding)
 * Data augmentation on duration values at the MIDI level
```

### Comparing `miditok-2.0.5/README.md` & `miditok-2.0.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # MidiTok
 
 Python package to tokenize MIDI music files, presented at the ISMIR 2021 LBD.
 
+![MidiTok Logo](docs/assets/logo.png?raw=true "")
+
 [![PyPI version fury.io](https://badge.fury.io/py/miditok.svg)](https://pypi.python.org/pypi/miditok/)
 [![Python 3.7](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/)
 [![Documentation Status](https://readthedocs.org/projects/miditok/badge/?version=latest)](https://miditok.readthedocs.io/en/latest/?badge=latest)
 [![GitHub CI](https://github.com/Natooz/MidiTok/actions/workflows/pytest.yml/badge.svg)](https://github.com/Natooz/MidiTok/actions/workflows/pytest.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/Natooz/MidiTok)](https://codecov.io/gh/Natooz/MidiTok)
 [![GitHub license](https://img.shields.io/github/license/Natooz/MidiTok.svg)](https://github.com/Natooz/MidiTok/blob/main/LICENSE)
 [![Downloads](https://pepy.tech/badge/MidiTok)](https://pepy.tech/project/MidiTok)
 [![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-![MidiTok Logo](docs/assets/logo.png?raw=true "")
-
-
-Using Deep Learning with symbolic music ? Then MidiTok can take care of converting your MIDI files into tokens, ready to be fed to models such as Transformer, for any generation, transcription or MIR task.
-MidiTok features most known [MIDI tokenizations](https://miditok.readthedocs.io/en/latest/tokenizations.html) (e.g. [REMI](https://arxiv.org/abs/2002.00212), [Compound Word](https://arxiv.org/abs/2101.02402)...), and is built around the idea that they all share common parameters and methods. It supports Byte Pair Encoding (BPE) and data augmentation.
+Using Deep Learning with symbolic music ? MidiTok can take care of converting (tokenizing) your MIDI files into tokens, ready to be fed to models such as Transformer, for any generation, transcription or MIR task.
+MidiTok features most known [MIDI tokenizations](https://miditok.readthedocs.io/en/latest/tokenizations.html) (e.g. [REMI](https://arxiv.org/abs/2002.00212), [Compound Word](https://arxiv.org/abs/2101.02402)...), and is built around the idea that they all share common parameters and methods. It supports [Byte Pair Encoding (BPE)](https://arxiv.org/abs/2301.11975) and data augmentation.
 
 **Documentation:** [miditok.readthedocs.com](https://miditok.readthedocs.io/en/latest/index.html)
 
 ## Install
 
 ```shell
 pip install miditok
 ```
-MidiTok uses [MIDIToolkit](https://github.com/YatingMusic/miditoolkit), which itself uses [Mido](https://github.com/mido/mido) to read and write MIDI files, and BPE is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for super fast encoding.
+MidiTok uses [MIDIToolkit](https://github.com/YatingMusic/miditoolkit), which itself uses [Mido](https://github.com/mido/mido) to read and write MIDI files, and BPE is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for super-fast encoding.
 
 ## Usage example
 
 The most basic and useful methods are summarized here. And [here](colab-notebooks/Full_Example_HuggingFace_GPT2_Transformer.ipynb) is a simple notebook example showing how to use Hugging Face models to generate music, with MidiTok taking care of tokenizing MIDIs.
 
 ```python
 from miditok import REMI
@@ -71,27 +70,28 @@
 * [REMI+](https://openreview.net/forum?id=NyR8OZFHw6i)
 * [MIDI-Like](https://link.springer.com/article/10.1007/s00521-018-3758-9)
 * [TSD](https://arxiv.org/abs/2301.11975)
 * [Structured](https://arxiv.org/abs/2107.05944)
 * [CPWord](https://ojs.aaai.org/index.php/AAAI/article/view/16091)
 * [Octuple](https://aclanthology.org/2021.findings-acl.70)
 * [MuMIDI](https://dl.acm.org/doi/10.1145/3394171.3413721)
+* [MMM](https://arxiv.org/abs/2008.06048)
 
 You can find short presentations in the [documentation](https://miditok.readthedocs.io/en/latest/tokenizations.html).
 
 ## Limitations
 
 Tokenizations using Bar tokens (REMI, Compound Word and MuMIDI) **only considers a 4/x time signature** for now. This means that each bar is considered covering 4 beats.
 REMI+ and Octuple support it.
 
 ## Contributions
 
 Contributions are gratefully welcomed, feel free to open an issue or send a PR if you want to add a tokenization or speed up the code. You can read the [contribution guide](CONTRIBUTING.md) for details.
 
-### Todo
+### Todos
 
 * Extend Time Signature to all tokenizations
 * Control Change messages
 * Option to represent pitch values as pitch intervals, as [it seems to improve performances](https://ismir2022program.ismir.net/lbd_369.html).
 * Speeding up MIDI read / load (Rust / C++ binding)
 * Data augmentation on duration values at the MIDI level
```

### Comparing `miditok-2.0.5/miditok/classes.py` & `miditok-2.0.6/miditok/classes.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/miditok/constants.py` & `miditok-2.0.6/miditok/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Constants for data encoding
 
 """
 
-CURRENT_VERSION_PACKAGE = "2.0.5"  # used when saving the config of a tokenizer
+CURRENT_VERSION_PACKAGE = "2.0.6"  # used when saving the config of a tokenizer
 
 MIDI_FILES_EXTENSIONS = [".mid", ".midi", ".MID", ".MIDI"]
 
 # Starting id of chr() method for BPE, as the 5 (0 to 4 included) firsts are ignored by 🤗tokenize
 # We also skip the 32nd (0x20) (space) as it causes issues when loading a BPE model with spaces in merged
 # Issue for reference: https://github.com/huggingface/tokenizers/issues/566
 # List of unicode characters: https://www.fileformat.info/info/charset/UTF-8/list.htm
@@ -63,17 +63,19 @@
     # Time signature params
     "time_signature_range": (8, 2),
     # Programs
     "programs": list(range(-1, 128)),
 }  # (max_beat_res, max_bar_length_in_NOTE)
 SPECIAL_TOKENS = ["PAD", "BOS", "EOS", "MASK"]  # default special tokens
 
+# Tokenizers specific parameters
 # For MuMIDI, recommended range from the GM2 specs
 # note: we ignore the "Applause" at pitch 88 of the orchestra drum set, increase to 89 if you need it
 DRUM_PITCH_RANGE = range(27, 88)
+MMM_DENSITY_BINS_MAX = (10, 20)
 
 # Defaults values when writing new MIDI files
 TIME_DIVISION = 384  # 384 and 480 are convenient as divisible by 4, 8, 12, 16, 24, 32
 TEMPO = 120
 TIME_SIGNATURE = (4, 4)
 
 # Used with chords
```

### Comparing `miditok-2.0.5/miditok/data_augmentation/data_augmentation.py` & `miditok-2.0.6/miditok/data_augmentation/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/miditok/midi_tokenizer.py` & `miditok-2.0.6/miditok/midi_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -464,14 +464,15 @@
 
         # Preprocess the MIDI file
         self.preprocess_midi(midi)
 
         # Register MIDI metadata
         self._current_midi_metadata = {
             "time_division": midi.ticks_per_beat,
+            "max_tick": midi.max_tick,
             "tempo_changes": midi.tempo_changes,
             "time_sig_changes": midi.time_signature_changes,
             "key_sig_changes": midi.key_signature_changes,
         }
 
         tokens = self._midi_to_tokens(midi, *args, **kwargs)
```

### Comparing `miditok-2.0.5/miditok/tokenizations/cp_word.py` & `miditok-2.0.6/miditok/tokenizations/cp_word.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/miditok/tokenizations/midi_like.py` & `miditok-2.0.6/miditok/tokenizations/midi_like.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/miditok/tokenizations/mumidi.py` & `miditok-2.0.6/miditok/tokenizations/mumidi.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/miditok/tokenizations/octuple.py` & `miditok-2.0.6/miditok/tokenizations/octuple.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/miditok/tokenizations/octuple_mono.py` & `miditok-2.0.6/miditok/tokenizations/octuple_mono.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/miditok/tokenizations/remi.py` & `miditok-2.0.6/miditok/tokenizations/remi.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/miditok/tokenizations/remi_plus.py` & `miditok-2.0.6/miditok/tokenizations/remi_plus.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             str, Union[bool, int, Tuple[int, int]]
         ] = ADDITIONAL_TOKENS,
         special_tokens: List[str] = SPECIAL_TOKENS,
         params: Optional[Union[str, Path]] = None,
         max_bar_embedding: Optional[int] = 60,
     ):
         additional_tokens["Program"] = True  # required
+        # code handling rest decoding is writen, but not for detection (encoding)
         additional_tokens["Rest"] = False
         self.programs = additional_tokens.get("programs", list(range(-1, 128)))
         self.max_bar_embedding = (
             max_bar_embedding  # this attribute might increase during encoding
         )
         super().__init__(
             pitch_range,
```

### Comparing `miditok-2.0.5/miditok/tokenizations/structured.py` & `miditok-2.0.6/miditok/tokenizations/structured.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/miditok/tokenizations/tsd.py` & `miditok-2.0.6/miditok/tokenizations/tsd.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/miditok/utils/utils.py` & `miditok-2.0.6/miditok/utils/utils.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/miditok.egg-info/PKG-INFO` & `miditok-2.0.6/miditok.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.0.5
+Version: 2.0.6
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -17,37 +17,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MidiTok
 
 Python package to tokenize MIDI music files, presented at the ISMIR 2021 LBD.
 
+![MidiTok Logo](docs/assets/logo.png?raw=true "")
+
 [![PyPI version fury.io](https://badge.fury.io/py/miditok.svg)](https://pypi.python.org/pypi/miditok/)
 [![Python 3.7](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/)
 [![Documentation Status](https://readthedocs.org/projects/miditok/badge/?version=latest)](https://miditok.readthedocs.io/en/latest/?badge=latest)
 [![GitHub CI](https://github.com/Natooz/MidiTok/actions/workflows/pytest.yml/badge.svg)](https://github.com/Natooz/MidiTok/actions/workflows/pytest.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/Natooz/MidiTok)](https://codecov.io/gh/Natooz/MidiTok)
 [![GitHub license](https://img.shields.io/github/license/Natooz/MidiTok.svg)](https://github.com/Natooz/MidiTok/blob/main/LICENSE)
 [![Downloads](https://pepy.tech/badge/MidiTok)](https://pepy.tech/project/MidiTok)
 [![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-![MidiTok Logo](docs/assets/logo.png?raw=true "")
-
-
-Using Deep Learning with symbolic music ? Then MidiTok can take care of converting your MIDI files into tokens, ready to be fed to models such as Transformer, for any generation, transcription or MIR task.
-MidiTok features most known [MIDI tokenizations](https://miditok.readthedocs.io/en/latest/tokenizations.html) (e.g. [REMI](https://arxiv.org/abs/2002.00212), [Compound Word](https://arxiv.org/abs/2101.02402)...), and is built around the idea that they all share common parameters and methods. It supports Byte Pair Encoding (BPE) and data augmentation.
+Using Deep Learning with symbolic music ? MidiTok can take care of converting (tokenizing) your MIDI files into tokens, ready to be fed to models such as Transformer, for any generation, transcription or MIR task.
+MidiTok features most known [MIDI tokenizations](https://miditok.readthedocs.io/en/latest/tokenizations.html) (e.g. [REMI](https://arxiv.org/abs/2002.00212), [Compound Word](https://arxiv.org/abs/2101.02402)...), and is built around the idea that they all share common parameters and methods. It supports [Byte Pair Encoding (BPE)](https://arxiv.org/abs/2301.11975) and data augmentation.
 
 **Documentation:** [miditok.readthedocs.com](https://miditok.readthedocs.io/en/latest/index.html)
 
 ## Install
 
 ```shell
 pip install miditok
 ```
-MidiTok uses [MIDIToolkit](https://github.com/YatingMusic/miditoolkit), which itself uses [Mido](https://github.com/mido/mido) to read and write MIDI files, and BPE is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for super fast encoding.
+MidiTok uses [MIDIToolkit](https://github.com/YatingMusic/miditoolkit), which itself uses [Mido](https://github.com/mido/mido) to read and write MIDI files, and BPE is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for super-fast encoding.
 
 ## Usage example
 
 The most basic and useful methods are summarized here. And [here](colab-notebooks/Full_Example_HuggingFace_GPT2_Transformer.ipynb) is a simple notebook example showing how to use Hugging Face models to generate music, with MidiTok taking care of tokenizing MIDIs.
 
 ```python
 from miditok import REMI
@@ -90,27 +89,28 @@
 * [REMI+](https://openreview.net/forum?id=NyR8OZFHw6i)
 * [MIDI-Like](https://link.springer.com/article/10.1007/s00521-018-3758-9)
 * [TSD](https://arxiv.org/abs/2301.11975)
 * [Structured](https://arxiv.org/abs/2107.05944)
 * [CPWord](https://ojs.aaai.org/index.php/AAAI/article/view/16091)
 * [Octuple](https://aclanthology.org/2021.findings-acl.70)
 * [MuMIDI](https://dl.acm.org/doi/10.1145/3394171.3413721)
+* [MMM](https://arxiv.org/abs/2008.06048)
 
 You can find short presentations in the [documentation](https://miditok.readthedocs.io/en/latest/tokenizations.html).
 
 ## Limitations
 
 Tokenizations using Bar tokens (REMI, Compound Word and MuMIDI) **only considers a 4/x time signature** for now. This means that each bar is considered covering 4 beats.
 REMI+ and Octuple support it.
 
 ## Contributions
 
 Contributions are gratefully welcomed, feel free to open an issue or send a PR if you want to add a tokenization or speed up the code. You can read the [contribution guide](CONTRIBUTING.md) for details.
 
-### Todo
+### Todos
 
 * Extend Time Signature to all tokenizations
 * Control Change messages
 * Option to represent pitch values as pitch intervals, as [it seems to improve performances](https://ismir2022program.ismir.net/lbd_369.html).
 * Speeding up MIDI read / load (Rust / C++ binding)
 * Data augmentation on duration values at the MIDI level
```

### Comparing `miditok-2.0.5/miditok.egg-info/SOURCES.txt` & `miditok-2.0.6/miditok.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 miditok.egg-info/requires.txt
 miditok.egg-info/top_level.txt
 miditok/data_augmentation/__init__.py
 miditok/data_augmentation/data_augmentation.py
 miditok/tokenizations/__init__.py
 miditok/tokenizations/cp_word.py
 miditok/tokenizations/midi_like.py
+miditok/tokenizations/mmm.py
 miditok/tokenizations/mumidi.py
 miditok/tokenizations/octuple.py
 miditok/tokenizations/octuple_mono.py
 miditok/tokenizations/remi.py
 miditok/tokenizations/remi_plus.py
 miditok/tokenizations/structured.py
 miditok/tokenizations/tsd.py
```

### Comparing `miditok-2.0.5/setup.py` & `miditok-2.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name='miditok',
     author='Nathan Fradet',
     url='https://github.com/Natooz/MidiTok',
     packages=find_packages(exclude=("tests",)),
-    version='2.0.5',
+    version='2.0.6',
     license='MIT',
     description='A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies',
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         'artificial intelligence',
         'deep learning',
```

### Comparing `miditok-2.0.5/tests/test_bpe.py` & `miditok-2.0.6/tests/test_bpe.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     r"""Reads a few MIDI files, convert them into token sequences, convert them back to MIDI files.
     The converted back MIDI files should identical to original one, expect with note starting and ending
     times quantized, and maybe a some duplicated notes removed
 
     :param data_path: root path to the data to test
     """
     random.seed(777)
-    tokenizations = ["Structured", "REMI", "REMIPlus", "MIDILike", "TSD"]
+    tokenizations = ["Structured", "REMI", "REMIPlus", "MIDILike", "TSD", "MMM"]
     data_path = Path(data_path)
     files = list(data_path.glob("**/*.mid"))
 
     # Creates tokenizers and computes BPE (build voc)
     first_tokenizers = []
     first_samples_bpe = {tok: [] for tok in tokenizations}
     for tokenization in tokenizations:
@@ -97,15 +97,15 @@
                 params=Path(
                     "tests", "test_results", f"{tokenization}_bpe", "config.txt"
                 )
             )
         )
         assert (
             tokenizers[i] == first_tokenizers[i]
-        ), f"Saving and reloading tokenizer failed. The reloaded tokenizer is different from the first one."
+        ), "Saving and reloading tokenizer failed. The reloaded tokenizer is different from the first one."
 
     # Unbatched BPE
     at_least_one_error = False
     tok_times = []
     for i, file_path in enumerate(tqdm(files, desc="Testing BPE unbatched")):
         midi = MidiFile(file_path)
```

### Comparing `miditok-2.0.5/tests/test_bpe_slow.py` & `miditok-2.0.6/tests/test_bpe_slow.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/tests/test_methods.py` & `miditok-2.0.6/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/tests/test_multitrack.py` & `miditok-2.0.6/tests/test_multitrack.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,23 @@
     saving_erroneous_midis: bool = False,
 ):
     r"""Reads a few MIDI files, convert them into token sequences, convert them back to MIDI files.
     The converted back MIDI files should identical to original one, expect with note starting and ending
     times quantized, and maybe a some duplicated notes removed
 
     """
-    tokenizations = ["REMI", "REMIPlus", "CPWord", "Octuple", "OctupleMono", "MuMIDI"]
+    tokenizations = [
+        "REMI",
+        "REMIPlus",
+        "CPWord",
+        "Octuple",
+        "OctupleMono",
+        "MuMIDI",
+        "MMM",
+    ]
     files = list(Path(data_path).glob("**/*.mid"))
     at_least_one_error = False
 
     for i, file_path in enumerate(tqdm(files, desc="Testing multitrack")):
         # Reads the MIDI
         try:
             midi = MidiFile(Path(file_path))
```

### Comparing `miditok-2.0.5/tests/test_one_track.py` & `miditok-2.0.6/tests/test_one_track.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,26 @@
     time_signature_changes_equals,
 )
 
 # Special beat res for test, up to 64 beats so the duration and time-shift values are
 # long enough for MIDI-Like and Structured encodings, and with a single beat resolution
 BEAT_RES_TEST = {(0, 64): 8}
 ADDITIONAL_TOKENS_TEST = {
-    "Chord": False,  # set to false to speed up tests as it takes some time on maestro MIDIs
+    "Chord": False,  # set false to speed up tests as it takes some time on maestro MIDIs
     "Rest": True,
     "Tempo": True,
     "TimeSignature": True,
     "Program": False,
     "rest_range": (4, 16),
     "nb_tempos": 32,
     "tempo_range": (40, 250),
     "time_signature_range": (16, 2),
+    "chord_maps": miditok.constants.CHORD_MAPS,
+    "chord_tokens_with_root_note": True,  # Tokens will look as "Chord_C:maj"
+    "chord_unknown": False,
 }
 
 
 def test_one_track_midi_to_tokens_to_midi(
     data_path: Union[str, Path, PurePath] = "./tests/Maestro_MIDIs",
     saving_erroneous_midis: bool = True,
 ):
@@ -57,14 +60,15 @@
         "Structured",
         "REMI",
         "REMIPlus",
         "CPWord",
         "Octuple",
         "OctupleMono",
         "MuMIDI",
+        "MMM",
     ]
     files = list(Path(data_path).glob("**/*.mid"))
     at_least_one_error = False
 
     for i, file_path in enumerate(tqdm(files, desc="Testing One Track")):
         # Reads the midi
         midi = MidiFile(file_path)
```

### Comparing `miditok-2.0.5/tests/test_saving_loading_config.py` & `miditok-2.0.6/tests/test_saving_loading_config.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/tests/test_utils.py` & `miditok-2.0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `miditok-2.0.5/tests/tests_utils.py` & `miditok-2.0.6/tests/tests_utils.py`

 * *Files identical despite different names*

