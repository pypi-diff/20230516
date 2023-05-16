# Comparing `tmp/pyriksprot_tagger-2023.4.2.tar.gz` & `tmp/pyriksprot_tagger-2023.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyriksprot_tagger-2023.4.2.tar", max compression
+gzip compressed data, was "pyriksprot_tagger-2023.4.3.tar", max compression
```

## Comparing `pyriksprot_tagger-2023.4.2.tar` & `pyriksprot_tagger-2023.4.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1080 2022-03-14 19:05:45.701621 pyriksprot_tagger-2023.4.2/LICENSE
--rw-r--r--   0        0        0     3694 2023-03-27 14:40:27.622646 pyriksprot_tagger-2023.4.2/README.md
--rw-r--r--   0        0        0     4674 2023-04-17 15:02:40.902581 pyriksprot_tagger-2023.4.2/pyproject.toml
--rw-r--r--   0        0        0      259 2023-04-17 09:10:35.869007 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/__init__.py
--rw-r--r--   0        0        0     5625 2023-04-17 13:47:26.532461 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/config.py
--rw-r--r--   0        0        0        0 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/resources/__init__.py
--rw-r--r--   0        0        0       68 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/resources/sparv/Makefile
--rw-r--r--   0        0        0        0 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/resources/sparv/__init__.py
--rw-r--r--   0        0        0     4963 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/resources/sparv/speech_xml_config.yaml
--rw-r--r--   0        0        0        0 2022-09-26 14:49:56.520960 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/__init__.py
--rw-r--r--   0        0        0     7224 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/git-timesync
--rwxr-xr-x   0        0        0     1786 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/git_update_mtime.sh
--rw-r--r--   0        0        0      563 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/move_empty_files.sh
--rwxr-xr-x   0        0        0      251 2022-03-14 19:05:45.717621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/setup-pipeline
--rwxr-xr-x   0        0        0      196 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/snake-it.sh
--rwxr-xr-x   0        0        0     1071 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/stanza-models.sh
--rwxr-xr-x   0        0        0     4244 2023-04-13 12:39:25.781582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/tag-it.sh
--rw-r--r--   0        0        0     1038 2023-04-14 14:18:41.032914 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/tag.py
--rw-r--r--   0        0        0      846 2023-04-14 09:19:33.724658 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/tag_info.py
--rw-r--r--   0        0        0       70 2023-04-14 12:29:53.731729 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/taggers/__init__.py
--rw-r--r--   0        0        0     1991 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/taggers/spacy2.py
--rw-r--r--   0        0        0     7179 2023-04-17 09:10:36.389014 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/taggers/stanza.py
--rw-r--r--   0        0        0     5346 2023-04-17 09:10:49.005177 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/utility.py
--rw-r--r--   0        0        0     4328 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/Makefile
--rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/README.md
--rw-r--r--   0        0        0     1709 2023-04-14 14:21:13.246887 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/Snakefile
--rw-r--r--   0        0        0       15 2023-04-14 14:12:34.288157 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/__init__.py
--rw-r--r--   0        0        0        0 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/__init__.py
--rw-r--r--   0        0        0      188 2022-03-14 19:05:45.725621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/__paths__.py
--rw-r--r--   0        0        0      735 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/compute_frequency.smk
--rw-r--r--   0        0        0      892 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/extract_speeches.smk
--rw-r--r--   0        0        0      111 2022-03-14 19:05:45.729621 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/help.smk
--rw-r--r--   0        0        0     1535 2023-04-17 13:47:47.336713 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/tag_protocols.smk
--rw-r--r--   0        0        0     1758 2023-04-13 12:39:25.785582 pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/update_repository.smk
--rw-r--r--   0        0        0     4783 1970-01-01 00:00:00.000000 pyriksprot_tagger-2023.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2022-03-14 19:05:45.701621 pyriksprot_tagger-2023.4.3/LICENSE
+-rw-r--r--   0        0        0     3694 2023-03-27 14:40:27.622646 pyriksprot_tagger-2023.4.3/README.md
+-rw-r--r--   0        0        0     4682 2023-05-16 10:46:23.548065 pyriksprot_tagger-2023.4.3/pyproject.toml
+-rw-r--r--   0        0        0      232 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/__init__.py
+-rw-r--r--   0        0        0    14366 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/cwb.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/resources/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/resources/sparv/Makefile
+-rw-r--r--   0        0        0        0 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/resources/sparv/__init__.py
+-rw-r--r--   0        0        0     4963 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/resources/sparv/speech_xml_config.yaml
+-rw-r--r--   0        0        0        0 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/__init__.py
+-rw-r--r--   0        0        0     7224 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/git-timesync
+-rwxr-xr-x   0        0        0     1786 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/git_update_mtime.sh
+-rw-r--r--   0        0        0      563 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/move_empty_files.sh
+-rwxr-xr-x   0        0        0      251 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/setup-pipeline
+-rwxr-xr-x   0        0        0      196 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/snake-it.sh
+-rwxr-xr-x   0        0        0     1071 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/stanza-models.sh
+-rwxr-xr-x   0        0        0     4244 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/tag-it.sh
+-rw-r--r--   0        0        0     1526 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/tag.py
+-rw-r--r--   0        0        0      846 2023-05-16 10:45:33.267580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/tag_info.py
+-rw-r--r--   0        0        0       77 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/taggers/__init__.py
+-rw-r--r--   0        0        0     1991 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/taggers/spacy2.py
+-rw-r--r--   0        0        0    11224 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/taggers/stanza_tagger.py
+-rw-r--r--   0        0        0     5470 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/utility.py
+-rw-r--r--   0        0        0     4328 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/Makefile
+-rw-r--r--   0        0        0        0 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/README.md
+-rw-r--r--   0        0        0     1802 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/Snakefile
+-rw-r--r--   0        0        0       15 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/rules/__init__.py
+-rw-r--r--   0        0        0      188 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/rules/__paths__.py
+-rw-r--r--   0        0        0      683 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/rules/compute_frequency.smk
+-rw-r--r--   0        0        0      892 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/rules/extract_speeches.smk
+-rw-r--r--   0        0        0      111 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/rules/help.smk
+-rw-r--r--   0        0        0     1465 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/rules/tag_protocols.smk
+-rw-r--r--   0        0        0     1657 2023-05-16 10:45:33.271580 pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/rules/update_repository.smk
+-rw-r--r--   0        0        0     4909 1970-01-01 00:00:00.000000 pyriksprot_tagger-2023.4.3/PKG-INFO
```

### Comparing `pyriksprot_tagger-2023.4.2/LICENSE` & `pyriksprot_tagger-2023.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/README.md` & `pyriksprot_tagger-2023.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/pyproject.toml` & `pyriksprot_tagger-2023.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyriksprot_tagger"
-version = "2023.4.2"
+version = "2023.4.3"
 description = "Pipeline that tags pyriksprot Parla-Clarin XML files"
 authors = ["Roger Mähler <roger.mahler@hotmail.com>"]
 packages = [
     { include = "pyriksprot_tagger" },
 ]
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
@@ -27,20 +27,26 @@
 dehyphen = "*"
 pygit2 = "*"
 cookiecutter = "*"
 pandas = "*"
 snakemake = "*"
 loguru = "*"
 stanza = "*"
-# torch = "==1.11.0+cu113"
-
-# pip install torch==1.7.0 torchvision==0.8.1 -f https://download.pytorch.org/whl/cu101/torch_stable.html
-# beräkningsserver: pip install torch==1.11.0+cu113 torchvision==0.12.0+cu113 torchaudio==0.11.0+cu113 -f https://download.pytorch.org/whl/cu113/torch_stable.html
 poetry = "^1.4.2"
-pyriksprot = "^2023.4.2"
+nltk = "^3.8.1"
+pathvalidate = "^2.5.2"
+# need to pip install torch
+torch = {extras = ["cuda"], version = "^2.0.1" }
+# torch = {extras = ["cuda"], version = "^2.0.1", source="torch"}
+
+# [[tool.poetry.source]]
+# name = "torch"
+# url = "https://download.pytorch.org/whl/cu117"
+# secondary = true
+pyriksprot = "^2023.4.4"
 
 [tool.poetry.dev-dependencies]
 black = "==20.*,>=20.8.0.b1"
 coverage = "==5.*,>=5.4.0"
 flake8 = "==3.*,>=3.8.4"
 flake8-black = "==0.*,>=0.2.1"
 isort = "==5.*,>=5.7.0"
@@ -138,15 +144,15 @@
         sort = "Name"
     [tool.coverage.html]
         directory     = "tests/coverage/html"
         show_contexts = true
 
 [tool.pyright]
 # https://github.com/microsoft/pyright/blob/main/docs/configuration.md
-include = ["workflow", "tests"]
+# include = ["pyriksprot_tagger", "tests"]
 exclude = [
     ".git",
     ".snakemake",
     ".vscode",
     "**/__init__.py",
     "**/__pycache__",
     "**/purgatory",
@@ -162,15 +168,15 @@
 reportMissingImports = true
 reportMissingTypeStubs = false
 reportUntypedFunctionDecorator = false
 reportUntypedClassDecorator = true
 reportOptionalSubscript = false
 reportOptionalMemberAccess = false
 reportOptionalCall = false
-pythonVersion = "3.8"
+pythonVersion = "3.11"
 
 [tool.dephell.main]
 from = { format = "poetry", path = "pyproject.toml" }
 to = { format = "poetry", path = "pyproject.toml" }
 
 [tool.mypy]
 allow_redefinition = true
```

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/resources/sparv/speech_xml_config.yaml` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/resources/sparv/speech_xml_config.yaml`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/git-timesync` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/git-timesync`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/git_update_mtime.sh` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/git_update_mtime.sh`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/move_empty_files.sh` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/move_empty_files.sh`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/stanza-models.sh` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/stanza-models.sh`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/tag-it.sh` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/tag-it.sh`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/tag.py` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/tag.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,56 @@
 import click
 from loguru import logger
-from pyriksprot.workflows.tag import ITagger, tag_protocols
-from pyriksprot_tagger import check_cuda
-from pyriksprot_tagger.taggers import StanzaTaggerFactory
+from pyriksprot import configuration
+from pyriksprot.workflows.tag import ITagger, TaggerProvider, tag_protocols
+from pyriksprot_tagger.utility import check_cuda
 
 
 @click.command()
+@click.argument('config_filename')
 @click.argument('source_folder')
 @click.argument('target_folder')
-@click.argument('config_filename')
 @click.option('--force', is_flag=True, default=False, help='Force if exists')
 @click.option('--recursive', is_flag=True, default=True, help='Recurse subfolders')
-@click.option('--disable-gpu', is_flag=True, default=False, help='Disable GPU')
 def main(
-    source_folder: str = None,
-    target_folder: str = None,
+    config_filename: str,
+    source_folder: str,
+    target_folder: str,
     force: bool = False,
-    recursive: bool = False,
-    disable_gpu: bool = False,
+    recursive: bool = True,
 ) -> None:
+    tagit(
+        config_filename=config_filename,
+        source_folder=source_folder,
+        target_folder=target_folder,
+        force=force,
+        recursive=recursive,
+    )
 
+
+def tagit(
+    config_filename: str,
+    source_folder: str,
+    target_folder: str,
+    force: bool = False,
+    recursive: bool = True,
+):
     check_cuda()
 
-    tagger: ITagger = StanzaTaggerFactory(use_gpu=not disable_gpu).create()
+    configuration.configure_context(source=config_filename, context="default")
+
+    tagger: ITagger = TaggerProvider.tagger_factory().create()
 
     tag_protocols(
-        tagger=tagger, source_folder=source_folder, target_folder=target_folder, force=force, recursive=recursive
+        tagger=tagger,
+        source_folder=source_folder,
+        target_folder=target_folder,
+        force=force,
+        recursive=recursive,
     )
 
     logger.info("workflow ended")
 
 
 if __name__ == "__main__":
-    main()
+    main()  # pylint: disable=no-value-for-parameter
+    # tagit("sample-data/config.yml", "sample-data/v0.6.0/parlaclarin/protocols/", "sample-data/v0.6.0/tagged_frames")
```

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/scripts/tag_info.py` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/scripts/tag_info.py`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/taggers/spacy2.py` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/taggers/spacy2.py`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/utility.py` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,31 +47,28 @@
     source_years, target_basenames = glob_wildcards(jj(source_folder, year_constraint, f"{{file}}.{source_extension}"))
     return source_years, target_basenames
 
 
 def expand_target_files(
     source_folder: str, source_extension: str, target_folder: str, target_extension: str, years: int = None
 ) -> list[str]:
-
     source_years, target_basenames = expand_basenames(source_folder, source_extension, years=years)
 
     target_files = expand(
         jj(target_folder, "{year}", f"{{basename}}.{target_extension}"),
         zip,
         year=source_years,
         basename=target_basenames,
     )
 
     return target_files
 
 
 def setup_logging():
-
     with contextlib.suppress(Exception):
-
         if sys.platform == "win32":
 
             def handler(msg):
                 if isinstance(msg, str):
                     print(msg)
                 if isinstance(msg, dict):
                     if 'level' in msg and 'debug' in msg['level']:
@@ -126,15 +123,14 @@
         if not torch.cuda.is_available():
             print(
                 "Please try (windows): pip install torch==1.7.0 torchvision==0.8.1 -f https://download.pytorch.org/whl/cu101/torch_stable.html"
             )
 
 
 def sparv_datadir(root_folder: str):
-
     if SPARV_DATADIR is not None:
         return SPARV_DATADIR
 
     for folder in ["..", "."]:
         sparv_folder = jj(root_folder, folder, "sparv")
         if isdir(sparv_folder):
             return sparv_folder
@@ -161,20 +157,23 @@
 
     return _stanza_dir
 
 
 def create_text_preprocessors(
     pipeline: str = "dedent,dehyphen,strip,pretokenize", fxs_tasks: Sequence[Callable[[str], str]] = None
 ) -> "list[Callable[[str], str]]":
-
     fxs: list[Callable[[str], str]] = []
     fxs_tasks: dict = {
         'dedent': dedent,
         'strip': str.strip,
         'pretokenize': pretokenize,
     } | (fxs_tasks or {})
     for fx_id in pipeline.split(","):
         if fx_id in fxs_tasks:
             fxs.append(fxs_tasks[fx_id])
         else:
             raise ValueError(f"Unknown text transform task: {fx_id}")
     return fxs
+
+
+def remove_csv_item(csv: str, item: str, sep: str = ',') -> str:
+    return sep.join([p for p in csv.split(sep) if p != item])
```

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/Makefile` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/Makefile`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/Snakefile` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/Snakefile`

 * *Files 8% similar despite different names*

```diff
@@ -16,50 +16,57 @@
 
 PACKAGE_PATH = abspath(jj(dirname(realpath(workflow.snakefile)), ".."))
 
 if PACKAGE_PATH not in sys.path:
     sys.path.insert(0, PACKAGE_PATH)
 
 from pyriksprot import sync_delta_names
-from pyriksprot_tagger import Config, expand_target_files, setup_logging
+from pyriksprot_tagger import expand_target_files, setup_logging
 
+from pyriksprot import configuration
+
+typed_config: configuration.Config = configuration.configure_context(
+    context="default", source=(config or {}).get("config_filename")
+)
 
 setup_logging()
 
 if sys.platform not in ["win32"]:
     shell.prefix("set -o pipefail; ")
 
-typed_config: Config = Config.load(source=(config or {}).get("config_filename"))
 
 rule all:
     input:
         expand_target_files(
             typed_config.source.folder,
             typed_config.source.extension,
             typed_config.target.folder,
             typed_config.target.extension,
-            years=config.get("year_filter", None)
+            years=config.get("year_filter", None),
         )
 
 
 include: jj("rules", "help.smk")
 include: jj("rules", "update_repository.smk")
 include: jj("rules", "compute_frequency.smk")
 include: jj("rules", "tag_protocols.smk")
+
+
 # include: jj("rules", "extract_speeches.smk")
 
 
 onstart:
     loguru_logger.info("Workflow started")
     os.makedirs(typed_config.target.folder, exist_ok=True)
     os.makedirs(typed_config.data_folder, exist_ok=True)
     os.makedirs(typed_config.log_folder, exist_ok=True)
     # os.makedirs(typed_config.extract.folder, exist_ok=True)
 
 
+
 onsuccess:
     sync_delta_names(typed_config.source.folder, "xml", typed_config.target.folder, "xml", delete=True)
     loguru_logger.info("Workflow ended")
 
 
 onerror:
     loguru_logger.error("Workflow FAILED")
```

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/compute_frequency.smk` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/rules/compute_frequency.smk`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # pylint: skip-file, disable-all
 """
 Computes global word frequency
 """
 import glob
 from pyriksprot import compute_term_frequencies
 
-# TODO: Apply optional wildcard constraint (if any)
 WORD_FREQUENCY_SOURCE_FILES = glob.glob(jj(typed_config.source.folder, "*", "*.xml"))
 
 rule word_frequency:
     message:
         "step: word_frequency"
     input:
         filenames=WORD_FREQUENCY_SOURCE_FILES,
```

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/extract_speeches.smk` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/rules/extract_speeches.smk`

 * *Files identical despite different names*

### Comparing `pyriksprot_tagger-2023.4.2/pyriksprot_tagger/workflow/rules/tag_protocols.smk` & `pyriksprot_tagger-2023.4.3/pyriksprot_tagger/workflow/rules/tag_protocols.smk`

 * *Files 8% similar despite different names*

```diff
@@ -5,44 +5,41 @@
 PoS tags Parla-CLARIN XML files using Stanza.
 """
 from os import makedirs
 from os.path import join as jj
 
 from pyriksprot import tag_protocol_xml
 
-from pyriksprot import TaggerRegistry
-from pyriksprot_tagger import StanzaTaggerFactory, check_cuda, Config
+from pyriksprot.workflows.tag import TaggerProvider, TaggerRegistry
+from pyriksprot.configuration import Config
+from pyriksprot_tagger import StanzaTaggerFactory, check_cuda
 
 typed_config: Config = typed_config
 disable_gpu: bool = config.get("disable_gpu", 0) == 1
 
 check_cuda()
 
 makedirs(typed_config.target.folder, exist_ok=True)
 
 def create_factory():
     typed_config.tagger_opts['use_gpu'] = not disable_gpu
-    return typed_config.tagger_factory.create()
+    return TaggerProvider.tagger_factory().create()
 
 def tagger():
     if StanzaTaggerFactory.identifier in TaggerRegistry.instances:
         return TaggerRegistry.instances[StanzaTaggerFactory.identifier]
     return TaggerRegistry.get(create_factory())
 
 rule tag_protocols:
     message:
         "step: tag_protocols"
-    params:
-        template=typed_config.extract.template,
-    # threads: workflow.cores * 0.75
     input:
         filename=jj(typed_config.source.folder, "{year}", "{basename}.xml"),
     output:
         filename=jj(typed_config.target.folder, "{year}", "{basename}.zip"),
-    # message: "Tagging {input.filename}."
     run:
         try:
             tag_protocol_xml(
                 input.filename,
                 output.filename,
                 tagger(),
                 storage_format="json",
```

### Comparing `pyriksprot_tagger-2023.4.2/PKG-INFO` & `pyriksprot_tagger-2023.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyriksprot-tagger
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: Pipeline that tags pyriksprot Parla-Clarin XML files
 Home-page: https://westac.se
 License: Apache-2.0
 Author: Roger Mähler
 Author-email: roger.mahler@hotmail.com
 Requires-Python: >=3.11.0,<3.12.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -15,21 +15,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Requires-Dist: click
 Requires-Dist: cookiecutter
 Requires-Dist: dehyphen
 Requires-Dist: loguru
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pandas
+Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
 Requires-Dist: poetry (>=1.4.2,<2.0.0)
 Requires-Dist: pygit2
-Requires-Dist: pyriksprot (>=2023.4.2,<2024.0.0)
+Requires-Dist: pyriksprot (>=2023.4.4,<2024.0.0)
 Requires-Dist: snakefmt
 Requires-Dist: snakemake
 Requires-Dist: stanza
+Requires-Dist: torch[cuda] (>=2.0.1,<3.0.0)
 Project-URL: Repository, https://github.com/welfare-state-analytics/pyriksprot_tagger
 Description-Content-Type: text/markdown
 
 # Riksdagens Protokoll Part-Of-Speech Tagging
 
 This package implements part-of-speech tagging of `Riksdagens Protokoll` Parla-CLARIN XML files.
```

