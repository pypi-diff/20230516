# Comparing `tmp/finetune_eval_harness-0.6.0.dev0.tar.gz` & `tmp/finetune_eval_harness-0.6.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finetune_eval_harness-0.6.0.dev0.tar", last modified: Mon May  8 21:37:54 2023, max compression
+gzip compressed data, was "finetune_eval_harness-0.6.1.dev1.tar", last modified: Tue May 16 21:53:24 2023, max compression
```

## Comparing `finetune_eval_harness-0.6.0.dev0.tar` & `finetune_eval_harness-0.6.1.dev1.tar`

### file list

```diff
@@ -1,47 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.648788 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-08 21:37:54.000000 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-08 21:37:54.000000 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 21:37:54.000000 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-08 21:37:54.000000 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 21:37:54.000000 finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/hf_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/data_trainining_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11455 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/initial_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/model_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    48785 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/trainer_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)    53665 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/utility_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23681 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/hf_scripts/utils_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/process_args.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/german_europarl.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/german_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/german_quad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/germeval2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/germeval2018.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/gnad10.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tasks/qa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/templates/new_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/templates/new_task_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:54.652788 finetune_eval_harness-0.6.0.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tests/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tests/test_stability.py
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-05-08 21:37:53.000000 finetune_eval_harness-0.6.0.dev0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:24.890076 finetune_eval_harness-0.6.1.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-16 21:53:24.890076 finetune_eval_harness-0.6.1.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:53:24.890076 finetune_eval_harness-0.6.1.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:24.882076 finetune_eval_harness-0.6.1.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:24.882076 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:24.886076 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9603 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/initial_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/model_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48785 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54543 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23681 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/process_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:24.886076 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/bulgarian_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/croatian_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/czech_subjectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/danish_misogyny.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/dutch_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/ehealth_kd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/eur_lux.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/finish_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/flue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/german_europarl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/german_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/german_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/germeval2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/germeval2018.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/gnad10.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/greek_legal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/klej_dyk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/maltese_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/mapa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/polish_dyk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/rucola.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/slovak_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/spanish_conll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/spanish_ehealth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/spanish_quad.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/swedish_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/szeged_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/task_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-16 21:53:23.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/wiki_cat_es.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:53:24.886076 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-16 21:53:24.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-05-16 21:53:24.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-16 21:53:24.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 21:53:24.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 21:53:24.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 21:53:24.000000 finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness.egg-info/top_level.txt
```

### Comparing `finetune_eval_harness-0.6.0.dev0/LICENSE` & `finetune_eval_harness-0.6.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.0.dev0/PKG-INFO` & `finetune_eval_harness-0.6.1.dev1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: finetune_eval_harness
-Version: 0.6.0.dev0
+Version: 0.6.1.dev1
 Summary: Finetune_Eval_Harness
 Home-page: UNKNOWN
 Author: DFKI Berlin
 Author-email: akga01@dfki.de
-License: UNKNOWN
+License: MIT
 Keywords: deep learning
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Finetune-Evaluation-Harness
 
 ![Build Status](https://github.com/malteos/finetune-evaluation-harness/actions/workflows/coverage_eval.yml/badge.svg)
 ![Build Status](https://github.com/malteos/finetune-evaluation-harness/actions/workflows/pull_request.yml/badge.svg)
@@ -91,9 +91,13 @@
 To implement a new task in eval harness, see [this guide](./docs/task_guide.md).
 
 
 ## Evaluating the Coverage of the Current Code
 Please go to Github Actions sections of this repository and start the build named "Evaluate", this would check if the coverage on existing code is more than 80%. The build
 status is also visible on the main repo page.
 
+## Guidelines On Running Tasks
+- In some instances for specific tasks, please make sure to specify the exact dataset config depending on your needs
+- If text sequence processing fails for some classification, please try with setting --use_fast_tokenizer as False
+
```

### Comparing `finetune_eval_harness-0.6.0.dev0/README.md` & `finetune_eval_harness-0.6.1.dev1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -68,7 +68,11 @@
 To implement a new task in eval harness, see [this guide](./docs/task_guide.md).
 
 
 ## Evaluating the Coverage of the Current Code
 Please go to Github Actions sections of this repository and start the build named "Evaluate", this would check if the coverage on existing code is more than 80%. The build
 status is also visible on the main repo page.
 
+## Guidelines On Running Tasks
+- In some instances for specific tasks, please make sure to specify the exact dataset config depending on your needs
+- If text sequence processing fails for some classification, please try with setting --use_fast_tokenizer as False
+
```

### Comparing `finetune_eval_harness-0.6.0.dev0/finetune_eval_harness.egg-info/PKG-INFO` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: finetune-eval-harness
-Version: 0.6.0.dev0
+Version: 0.6.1.dev1
 Summary: Finetune_Eval_Harness
 Home-page: UNKNOWN
 Author: DFKI Berlin
 Author-email: akga01@dfki.de
-License: UNKNOWN
+License: MIT
 Keywords: deep learning
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Finetune-Evaluation-Harness
 
 ![Build Status](https://github.com/malteos/finetune-evaluation-harness/actions/workflows/coverage_eval.yml/badge.svg)
 ![Build Status](https://github.com/malteos/finetune-evaluation-harness/actions/workflows/pull_request.yml/badge.svg)
@@ -91,9 +91,13 @@
 To implement a new task in eval harness, see [this guide](./docs/task_guide.md).
 
 
 ## Evaluating the Coverage of the Current Code
 Please go to Github Actions sections of this repository and start the build named "Evaluate", this would check if the coverage on existing code is more than 80%. The build
 status is also visible on the main repo page.
 
+## Guidelines On Running Tasks
+- In some instances for specific tasks, please make sure to specify the exact dataset config depending on your needs
+- If text sequence processing fails for some classification, please try with setting --use_fast_tokenizer as False
+
```

### Comparing `finetune_eval_harness-0.6.0.dev0/hf_scripts/data_trainining_args.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/data_trainining_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,18 @@
     )
     train_batch_size: int = field(
         default=2, metadata={"help": "Size of train batch size"}
     )
     label_value: Optional[str] = field(
         default=None, metadata={"help": "label from the original dataset"}
     )
+    special_task_type: Optional[str] = field(
+        default=None, 
+        metadata={"help": "Is this some special task (eg multi-label classification). Use: multi_label_classification"}   
+    )
     remove_labels: Optional[List[str]] = field(
         default=None,
         metadata={
             "help": "Labels which have to removed (please verify these from the original dataset)"
         },
     )
     peft_choice: Optional[str] = field(
```

### Comparing `finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_class.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import sys
 from transformers import (
     PretrainedConfig,
     set_seed,
 )
 from transformers.utils import send_example_telemetry
 from transformers.utils.versions import require_version
-from hf_scripts import utility_functions
+from . import utility_functions
+import itertools
 
 require_version(
     "datasets>=1.8.0",
     "To fix: pip install -r examples/pytorch/text-classification/requirements.txt",
 )
 
 
@@ -53,15 +54,21 @@
             "float32",
             "float64",
         ]
         if is_regression:
             num_labels = 1
         else:
             # label_list = raw_datasets["train"].unique("label")
-            label_list = raw_datasets["train"].unique(label_value)
+            
+            if(isinstance(raw_datasets["train"][label_value][0], list)):
+                concat_list = list(itertools.chain.from_iterable(raw_datasets["train"][label_value]))
+                label_list = list(set(concat_list))
+            else:
+                label_list = raw_datasets["train"].unique(label_value)
+
             label_list.sort()  # Let's sort it for determinism
             num_labels = len(label_list)
 
     all_columns = raw_datasets.column_names
     # column_others = all_columns['train'].remove(data_args.label_value)
     column_others = all_columns["train"].remove(label_value)
 
@@ -215,15 +222,15 @@
     )
 
     logger.info(
         f"remaining trainable paramaters{utility_functions.print_trainable_parameters(model)}"
     )
 
     metrics_eval = utility_functions.train_eval_prediction(
-        "classification",
+        data_args.special_task_type if data_args.special_task_type is not None else "classification",
         model,
         training_args,
         data_args,
         model_args,
         train_dataset,
         eval_dataset,
         None,
```

### Comparing `finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_ner.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_ner.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,31 @@
     DataCollatorForTokenClassification,
     PretrainedConfig,
     set_seed,
 )
 from transformers.utils import send_example_telemetry
 from transformers.utils.versions import require_version
 from datasets import ClassLabel
-from hf_scripts.utility_functions import *
-import hf_scripts
+from . import utility_functions
+import numpy as np 
+
 
 def run_task_evaluation(model_args, data_args, training_args, init_args):
 
     #model_args, data_args, training_args = hf_scripts.utility_functions.parse_hf_arguments(args)
-    (training_args, data_args) = hf_scripts.utility_functions.prepend_data_args(training_args, data_args, init_args)
+    (training_args, data_args) = utility_functions.prepend_data_args(training_args, data_args, init_args)
     send_example_telemetry("run_ner", model_args, data_args)
 
-    logger = hf_scripts.utility_functions.prepare_logger(training_args)
-    last_checkpoint = hf_scripts.utility_functions.detect_last_checkpoint(logger, training_args)
+    logger = utility_functions.prepare_logger(training_args)
+    last_checkpoint = utility_functions.detect_last_checkpoint(logger, training_args)
 
     # Set seed before initializing model.
     set_seed(training_args.seed)
 
-    raw_datasets = hf_scripts.utility_functions.load_raw_dataset_ner(data_args, model_args)
+    raw_datasets = utility_functions.load_raw_dataset_ner(data_args, model_args)
 
     # raw_datasets = raw_datasets.map(lambda x: {"ner_tags": [int(i) for i in x["ner_tags"].split(",")]})
     # raw_datasets = raw_datasets.map(lambda x: {"pos_tags": [int(i) for i in x["pos_tags"].split(",")]})
 
     if training_args.do_train:
         column_names = raw_datasets["train"].column_names
         features = raw_datasets["train"].features
@@ -51,63 +52,63 @@
     else:
         label_column_name = column_names[1]
 
     # label_list = get_label_list(labels)
     # If the labels are of type ClassLabel, they are already integers and we have the map stored somewhere.
     # Otherwise, we have to get the list of labels manually.
 
-    label_list, label_to_id, feature_file_exists, labels_are_int = hf_scripts.utility_functions.generate_label_list(
+    label_list, label_to_id, feature_file_exists, labels_are_int = utility_functions.generate_label_list(
         raw_datasets, features, ClassLabel, label_column_name
     )
 
     num_labels = len(label_list)
     logger.info(f"Number of distinct labels {num_labels}")
 
-    config = hf_scripts.utility_functions.load_config(
+    config = utility_functions.load_config(
         model_args.model_name_or_path,
         num_labels,
         "ner",
         model_args.cache_dir,
         model_args.model_revision,
         model_args.use_auth_token,
         "ner",
     )
-    tokenizer = hf_scripts.utility_functions.load_tokenizer(
+    tokenizer = utility_functions.load_tokenizer(
         model_args.tokenizer_name if model_args.tokenizer_name else model_args.model_name_or_path,
         model_args.cache_dir,
         model_args.use_fast_tokenizer,
         model_args.model_revision,
         model_args.use_auth_token,
         None,
         True if config.model_type in {"bloom", "gpt2", "roberta"} else False,
     )
 
-    model = hf_scripts.utility_functions.load_model(
+    model = utility_functions.load_model(
         model_args.model_name_or_path,
         bool(".ckpt" in model_args.model_name_or_path),
         config,
         model_args.cache_dir,
         model_args.model_revision,
         model_args.use_auth_token,
         "ner",
     )
 
-    hf_scripts.utility_functions.print_trainable_parameters(model)
+    utility_functions.print_trainable_parameters(model)
 
-    if data_args.peft_choice in hf_scripts.utility_functions.peft_choice_list:
-        model = hf_scripts.utility_functions.load_model_peft(model, data_args, "TOKEN_CLS")
+    if data_args.peft_choice in utility_functions.peft_choice_list:
+        model = utility_functions.load_model_peft(model, data_args, "TOKEN_CLS")
 
-    model = hf_scripts.utility_functions.freeze_layers(model_args, model)
+    model = utility_functions.freeze_layers(model_args, model)
 
     if tokenizer.pad_token is None:
         tokenizer.pad_token = tokenizer.eos_token
 
     model.resize_token_embeddings(len(tokenizer))
 
-    hf_scripts.utility_functions.check_tokenizer_instance(tokenizer)
+    utility_functions.check_tokenizer_instance(tokenizer)
 
     '''
     # Model has labels -> use them.
     if model.config.label2id != PretrainedConfig(num_labels=num_labels).label2id:
         if list(sorted(model.config.label2id.keys())) == list(sorted(label_list)):
             # Reorganize `label_list` to match the ordering of the model.
             if labels_are_int:
@@ -126,15 +127,15 @@
             )
     '''
 
     # Set the correspondences label/ID inside the model config
     model.config.label2id = {l: i for i, l in enumerate(label_list)}
     model.config.id2label = {i: l for i, l in enumerate(label_list)}
 
-    b_to_i_label = hf_scripts.utility_functions.generate_b_to_i_label(feature_file_exists, label_list)
+    b_to_i_label = utility_functions.generate_b_to_i_label(feature_file_exists, label_list)
 
     # Preprocessing the dataset
     # Padding strategy
     padding = "max_length" if data_args.pad_to_max_length else False
 
     fn_kwargs = {
         "tokenizer": tokenizer,
@@ -142,32 +143,32 @@
         "padding": padding,
         "data_args": data_args,
         "label_column_name": label_column_name,
         "label_to_id": label_to_id,
         "b_to_i_label": b_to_i_label,
     }
 
-    train_dataset, eval_dataset, predict_dataset = hf_scripts.utility_functions.map_train_validation_predict_ds_ner(
+    train_dataset, eval_dataset, predict_dataset = utility_functions.map_train_validation_predict_ds_ner(
         training_args, data_args, raw_datasets, fn_kwargs
     )
 
     # Data collator
     data_collator = DataCollatorForTokenClassification(
         tokenizer, pad_to_multiple_of=8 if training_args.fp16 else None
     )
 
     # Metrics
     metric = evaluate.load("seqeval")
 
     def compute_metrics(p):
         predictions, labels = p
         predictions = np.argmax(predictions, axis=2)
-        return hf_scripts.utility_functions.get_true_predictions_labels(label_list, predictions, labels, metric, data_args)
+        return utility_functions.get_true_predictions_labels(label_list, predictions, labels, metric, data_args)
 
-    metrics_eval = hf_scripts.utility_functions.train_eval_prediction(
+    metrics_eval = utility_functions.train_eval_prediction(
         "token-classification",
         model,
         training_args,
         data_args,
         model_args,
         train_dataset,
         eval_dataset,
```

### Comparing `finetune_eval_harness-0.6.0.dev0/hf_scripts/hgf_fine_tune_qa.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/hgf_fine_tune_qa.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,16 @@
 from datasets import load_dataset, ClassLabel, Value
 import evaluate
 from . import trainer_qa
 from transformers import EvalPrediction, set_seed, HfArgumentParser, TrainingArguments
 from transformers.utils import check_min_version, send_example_telemetry
 from transformers.utils.versions import require_version
 
-# from utils_qa import postprocess_qa_predictions
 from . import utils_qa
-from hf_scripts.model_args import ModelArguments
-from hf_scripts.data_trainining_args import DataTrainingArguments
-from hf_scripts.utility_functions import *
-from hf_scripts import utility_functions
+from . import utility_functions
 
 require_version(
     "datasets>=1.8.0",
     "To fix: pip install -r examples/pytorch/question-answering/requirements.txt",
 )
 
 
@@ -75,15 +71,18 @@
     # Preprocessing is slighlty different for training and evaluation.
 
     # this is imp step because the evaluation logic expects id of string
     print(raw_datasets["train"].features)
     new_features = raw_datasets["train"].features.copy()
     new_features["id"] = Value("string")
     raw_datasets["train"] = raw_datasets["train"].cast(new_features)
-    raw_datasets["test"] = raw_datasets["test"].cast(new_features)
+    if "test" not in raw_datasets:
+        raw_datasets["test"] = raw_datasets["validation"].cast(new_features)
+    else:
+        raw_datasets["test"] = raw_datasets["test"].cast(new_features)
 
     if training_args.do_train:
         column_names = raw_datasets["train"].column_names
     
     # no need of elif and else logic as train split will always have column names
     '''
     elif training_args.do_eval:
@@ -139,16 +138,21 @@
             )
         if data_args.max_train_samples is not None:
             # Number of samples might increase during Feature Creation, We select only specified max samples
             max_train_samples = min(len(train_dataset), data_args.max_train_samples)
             train_dataset = train_dataset.select(range(max_train_samples))
 
     if training_args.do_eval:
+        
+        if("test" in raw_datasets):
+            eval_examples = raw_datasets["test"]
+        else:
+            eval_examples = raw_datasets["validation"]
 
-        eval_examples = raw_datasets["test"]
+        #eval_examples = raw_datasets["test"]
         # eval_examples = raw_datasets["validation"]
         if data_args.max_eval_samples is not None:
             # We will select sample from whole data
             max_eval_samples = min(len(eval_examples), data_args.max_eval_samples)
             eval_examples = eval_examples.select(range(max_eval_samples))
         # Validation Feature Creation
         fn_kwargs_validation = {
@@ -176,17 +180,24 @@
             # During Feature creation dataset samples might increase, we will select required samples again
             max_eval_samples = min(len(eval_dataset), data_args.max_eval_samples)
             eval_dataset = eval_dataset.select(range(max_eval_samples))
 
     predict_dataset = None
     predict_examples = None
     if training_args.do_predict:
+        #if "test" not in raw_datasets:
+        #    raise ValueError("--do_predict requires a test dataset")
+
         if "test" not in raw_datasets:
-            raise ValueError("--do_predict requires a test dataset")
-        predict_examples = raw_datasets["test"]
+            predict_examples = raw_datasets["validation"]
+        else:
+            predict_examples = raw_datasets["test"]
+
+        #predict_examples = raw_datasets["test"]
+
         if data_args.max_predict_samples is not None:
             # We will select sample from whole data
             predict_examples = predict_examples.select(
                 range(data_args.max_predict_samples)
             )
         # Predict Feature Creation
         with training_args.main_process_first(
```

### Comparing `finetune_eval_harness-0.6.0.dev0/hf_scripts/model_args.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/model_args.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.0.dev0/hf_scripts/trainer.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/trainer.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.0.dev0/hf_scripts/trainer_qa.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/trainer_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.0.dev0/hf_scripts/utility_functions.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/utility_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 import os
 import sys
-from dataclasses import dataclass, field
-from hf_scripts.model_args import ModelArguments
-from hf_scripts.data_trainining_args import DataTrainingArguments
-from hf_scripts.initial_arguments import InitialArguments
+sys.path.append('../')
 import numpy as np
+from dataclasses import dataclass, field
 from . import trainer_qa
-from hf_scripts import hgf_fine_tune_class, hgf_fine_tune_ner, hgf_fine_tune_qa
+from . import hgf_fine_tune_class, hgf_fine_tune_ner, hgf_fine_tune_qa
+from .model_args import ModelArguments
+from .data_trainining_args import DataTrainingArguments
+from .initial_arguments import InitialArguments
 import evaluate
 import transformers
 from transformers import (
     AutoConfig,
     AutoModelForSequenceClassification,
     AutoModelForTokenClassification,
     AutoModelForQuestionAnswering,
@@ -28,19 +29,19 @@
 from peft import (
     get_peft_model,
     LoraConfig,
 )
 from peft import PrefixTuningConfig, PromptEncoderConfig, PromptTuningConfig, TaskType
 from peft.utils.other import fsdp_auto_wrap_policy
 from os import path
-from tasks import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY
+from tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY 
 import json
 from typing import Any, Dict
 from . import utils_qa
-from datasets import load_dataset
+from datasets import load_dataset, DatasetDict
 
 """
 File containing utlility functions used over all the hf_scripts folder for all the tasks
 """
 
 
 # dict used in sequence classification task
@@ -72,14 +73,15 @@
     dataset_name = TASK_REGISTRY[each_task]().get_dataset_id()
     if TASK_REGISTRY[each_task]().get_task_type() == "classification":
         label_value = TASK_REGISTRY[each_task]().get_label_name()
         data_args.label_value = label_value
 
     if TASK_REGISTRY[each_task]().get_task_type() == "ner":
         data_args.is_task_ner = True
+        data_args.label_column_name = TASK_REGISTRY[each_task]().get_label_name()
     data_args.dataset_name = dataset_name
 
     return data_args
 
 
 def prepend_data_args(
     training_args: TrainingArguments,
@@ -471,15 +473,19 @@
                 json.dump(metrics_list, fp)
             fp.close()
 
         else:
             # file exists read the prev entry, add new one and then write
             with open(log_file_path, "r") as new_file_path:
                 curr_list = json.load(new_file_path)
-                curr_list = curr_list + [metrics]
+                print("curr_list", curr_list)
+                print("metrics", metrics)
+                curr_list = {**curr_list, **metrics}
+                
+                #curr_list = curr_list + [metrics]
 
             with open(log_file_path, "w") as new_file_path:
                 json.dump(curr_list, new_file_path)
 
             new_file_path.close()
 
         #trainer.log_metrics("eval", metrics)
@@ -802,22 +808,37 @@
         logger: object of Logger class
 
     """
     #raw_datasets = {}
     #raw_datasets["train"]=[]
     #raw_datasets["test"]=[]
 
+    raw_datasets = load_dataset(
+        data_args.dataset_name,
+        data_args.dataset_config_name,
+        cache_dir=model_args.cache_dir,
+        use_auth_token=True if model_args.use_auth_token else None,
+    )
+
     if data_args.task_name is not None:
         # Downloading and loading a dataset from the hub.
         raw_datasets = load_dataset(
             "glue",
             data_args.task_name,
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
+    if "train" not in raw_datasets:
+        train_testvalid = raw_datasets.train_test_split(test=0.1)
+        test_valid = train_testvalid['test']
+        raw_datasets = DatasetDict({
+            'train': train_testvalid['train'],
+            'test': train_testvalid['test']
+        })
+
     if data_args.is_subset == True:
         raw_datasets = load_dataset(
             data_args.dataset_name,
             data_args.dataset_config_name,
             cache_dir=model_args.cache_dir,
             use_auth_token=True if model_args.use_auth_token else None,
         )
@@ -1155,16 +1176,20 @@
                 fn_kwargs=fn_kwargs,
                 load_from_cache_file=not data_args.overwrite_cache,
                 desc="Running tokenizer on train dataset",
             )
 
     if training_args.do_eval:
         if "validation" not in raw_datasets:
-            raise ValueError("--do_eval requires a validation dataset")
-        eval_dataset = raw_datasets["validation"]
+            #raise ValueError("--do_eval requires a validation dataset")
+            eval_dataset = raw_datasets["test"]
+        else:
+            eval_dataset = raw_datasets["validation"]
+        #eval_dataset = raw_datasets["validation"]
+
         if data_args.max_eval_samples is not None:
             max_eval_samples = min(len(eval_dataset), data_args.max_eval_samples)
             eval_dataset = eval_dataset.select(range(max_eval_samples))
         with training_args.main_process_first(
             desc="validation dataset map pre-processing"
         ):
             eval_dataset = eval_dataset.map(
```

### Comparing `finetune_eval_harness-0.6.0.dev0/hf_scripts/utils_qa.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/hf_scripts/utils_qa.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.0.dev0/process_args.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/process_args.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,34 @@
+import sys
+sys.path.append('./')
 from transformers import HfArgumentParser, TrainingArguments
-from tasks import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY
+#from tasks import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY
+from tasks.task_registry import get_all_tasks, TASK_REGISTRY, TASK_TYPE_REGISTRY
+import logging
+sys.path.append('../')
+'''
 from hf_scripts.utility_functions import (
     map_source_file,
     peft_choice_list,
     add_labels_data_args,
 )
 from hf_scripts.model_args import ModelArguments
 from hf_scripts.data_trainining_args import DataTrainingArguments
 from hf_scripts.initial_arguments import InitialArguments
-import logging
+'''
+
+from hf_scripts.utility_functions import (
+    map_source_file,
+    peft_choice_list,
+    add_labels_data_args,
+)
+
+from hf_scripts.model_args import ModelArguments
+from hf_scripts.data_trainining_args import DataTrainingArguments
+from hf_scripts.initial_arguments import InitialArguments
 
 
 def process_arguments(args):
     """
     main method accepts argaprse arguments and process it to utilize the training scripts
     """
```

### Comparing `finetune_eval_harness-0.6.0.dev0/setup.py` & `finetune_eval_harness-0.6.1.dev1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from setuptools import find_packages, setup
 
 setup(
     name = "finetune_eval_harness",
-    version="0.6.0.dev0",
+    version="0.6.1.dev1",
     description="Finetune_Eval_Harness",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
+    license="MIT",
     author="DFKI Berlin",
     author_email="akga01@dfki.de",
     #url="https://github.com/malteos/finetune-evaluation-harness",
     #package_dir={"":""},
-    packages=[
-            'hf_scripts', 
-            'tasks',
-            'templates',
-            'tests',
-    ],
-    scripts = [
-        'process_args.py',
-        'main.py'
-    ],
-    python_requires=">=3.7.0",
+    # packages=[
+    #         'hf_scripts', 
+    #         'tasks',
+    #         'templates',
+    #         'tests',
+    # ],
+    # scripts = [
+    #     'process_args.py',
+    #     'main.py'
+    # ],
+    package_dir={"": "src"},
+    packages=find_packages("src"),
+    entry_points={"console_scripts": ["finetune-eval-harness=finetune_eval_harness.main:main"]},
+    python_requires=">=3.8.0",
     install_requires=[
         'pyarrow==6.0.1',
         'wandb',
         'jupyter',
         'ipywidgets>=8.0.2',
         'seqeval',
         'pandas==1.5.3',
```

### Comparing `finetune_eval_harness-0.6.0.dev0/tasks/classification.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `finetune_eval_harness-0.6.0.dev0/tasks/german_europarl.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/swedish_ner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,25 @@
-from tasks.ner import NamedEntityRecognition
+#from tasks.ner import NamedEntityRecognition
+from .ner import NamedEntityRecognition
 
-
-class GermanEuroParl(NamedEntityRecognition):
+class SwedishNer(NamedEntityRecognition):
 
     """
-    Class for German Europarl Task
+    Class for Swedish NER
     """
-
-    DATASET_ID = "akash418/german_europarl"
-    TASK_NAME = "german_europarl"
-    HOMEPAGE_URL = "https://huggingface.co/datasets/akash418/german_europarl"
+    
+    DATASET_ID = "swedish_ner_corpus"  # HF datasets ID
+    TASK_NAME = "swedish_ner"
+    HOMEPAGE_URL = "https://huggingface.co/datasets/swedish_ner_corpus"
+    LABEL_NAME = "ner_tags"
 
     def get_dataset_id(self):
-        """
-        return HF dataset id
-        """
         return self.DATASET_ID
 
     def get_task_name(self):
-        """
-        return task name
-        """
         return self.TASK_NAME
 
     def get_url(self):
-        """
-        return url
-        """
         return self.HOMEPAGE_URL
+    
+    def get_label_name(self):
+        return self.LABEL_NAME
```

### Comparing `finetune_eval_harness-0.6.0.dev0/tasks/germeval2017.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/germeval2017.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from tasks.classification import Classification
+#from tasks.classification import Classification
+from .classification import Classification
+
 
 _CITATION = """
 @inproceedings{germevaltask2017,
 title = {{GermEval 2017: Shared Task on Aspect-based Sentiment in Social Media Customer Feedback}},
 author = {Michael Wojatzki and Eugen Ruppert and Sarah Holschneider and Torsten Zesch and Chris Biemann},
 year = {2017},
 booktitle = {Proceedings of the GermEval 2017 - Shared Task on Aspect-based Sentiment in Social Media Customer Feedback},
```

### Comparing `finetune_eval_harness-0.6.0.dev0/tasks/germeval2018.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/germeval2018.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from tasks.classification import Classification
+#from tasks.classification import Classification
+from .classification import Classification
+
 
 _CITATION = """
 @inproceedings{vamvas2020germeval,
     author    = "Wiegand, Michael, and Siegel, Melanie and Ruppenhofer, Josef",
     title     = "Overview of the GermEval 2018 Shared Task on the Identification of Offensive Language",
     booktitle = "Proceedings of the GermEval 2018 Workshop  14th Conference on Natural Language Processing (KONSENS)",
     address   = "Vienna, SAustria",
```

### Comparing `finetune_eval_harness-0.6.0.dev0/tasks/gnad10.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/klej_dyk.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-from tasks.classification import Classification
+#from tasks.classification import Classification
+from .classification import Classification
 
 
-class Gnad10(Classification):
+class KlejDyk(Classification):
 
     """
-    Class for GNAD10 Classification Task
+    Class for Klej Dyk Classification Task
     """
-    
-    DATASET_ID = "gnad10"  # HF datasets ID
-    TASKNAME = "gnad10"
-    LABEL_NAME = "label"
-    HOMEPAGE_URL = "https://huggingface.co/datasets/gnad10"
+
+
+    DATASET_ID = "allegro/klej-dyk"  # HF datasets ID
+    TASK_NAME = "klej_dyk"
+    LABEL_NAME = "target"  # column name from HF dataset
+    HOMEPAGE_URL = "https://huggingface.co/datasets/allegro/klej-dyk"
 
     def get_dataset_id(self):
         return self.DATASET_ID
 
+    def get_task_name(self):
+        return self.TASK_NAME
+
     def get_label_name(self):
         return self.LABEL_NAME
 
-    def get_task_name(self):
-        return self.TASKNAME
-
     def get_url(self):
-        return self.HOMEPAGE_URL
+        return self.HOMEPAGE_URL
+
```

### Comparing `finetune_eval_harness-0.6.0.dev0/tasks/ner.py` & `finetune_eval_harness-0.6.1.dev1/src/finetune_eval_harness/tasks/ner.py`

 * *Files identical despite different names*

