# Comparing `tmp/micro_trainer_transformers-0.0.1.tar.gz` & `tmp/micro_trainer_transformers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micro_trainer_transformers-0.0.1.tar", last modified: Fri May 12 16:21:25 2023, max compression
+gzip compressed data, was "micro_trainer_transformers-0.0.2.tar", last modified: Tue May 16 12:03:58 2023, max compression
```

## Comparing `micro_trainer_transformers-0.0.1.tar` & `micro_trainer_transformers-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-05-12 16:21:25.808067 micro_trainer_transformers-0.0.1/
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      786 2023-05-12 16:21:25.808067 micro_trainer_transformers-0.0.1/PKG-INFO
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      219 2023-05-09 13:47:07.000000 micro_trainer_transformers-0.0.1/README.md
-drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-05-12 16:21:25.804067 micro_trainer_transformers-0.0.1/micro_trainer_transformers/
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      197 2023-05-01 21:14:11.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers/__init__.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)    20528 2023-05-03 14:18:14.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers/arguments.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)     7534 2023-05-04 14:18:10.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers/core_args.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)    14220 2023-05-09 13:59:23.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers/core_optim.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)    18508 2023-05-11 21:22:10.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers/core_train.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)     2926 2023-05-01 20:45:05.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers/trainer.py
--rw-rw-r--   0 joefox    (1000) joefox    (1000)     2248 2023-05-07 21:20:37.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers/utils.py
-drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-05-12 16:21:25.808067 micro_trainer_transformers-0.0.1/micro_trainer_transformers.egg-info/
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      786 2023-05-12 16:21:25.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers.egg-info/PKG-INFO
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      605 2023-05-12 16:21:25.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers.egg-info/SOURCES.txt
--rw-rw-r--   0 joefox    (1000) joefox    (1000)        1 2023-05-12 16:21:25.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers.egg-info/dependency_links.txt
--rw-rw-r--   0 joefox    (1000) joefox    (1000)       20 2023-05-12 16:21:25.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers.egg-info/entry_points.txt
--rw-rw-r--   0 joefox    (1000) joefox    (1000)       38 2023-05-12 16:21:25.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers.egg-info/requires.txt
--rw-rw-r--   0 joefox    (1000) joefox    (1000)       27 2023-05-12 16:21:25.000000 micro_trainer_transformers-0.0.1/micro_trainer_transformers.egg-info/top_level.txt
--rw-rw-r--   0 joefox    (1000) joefox    (1000)       79 2023-05-12 16:21:25.808067 micro_trainer_transformers-0.0.1/setup.cfg
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      990 2023-05-12 16:17:30.000000 micro_trainer_transformers-0.0.1/setup.py
+drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-05-16 12:03:58.670513 micro_trainer_transformers-0.0.2/
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      786 2023-05-16 12:03:58.670513 micro_trainer_transformers-0.0.2/PKG-INFO
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      219 2023-05-09 13:47:07.000000 micro_trainer_transformers-0.0.2/README.md
+drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-05-16 12:03:58.670513 micro_trainer_transformers-0.0.2/micro_trainer_transformers/
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      197 2023-05-01 21:14:11.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/__init__.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)    20528 2023-05-03 14:18:14.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/arguments.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     7975 2023-05-16 11:28:00.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_args.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)    15197 2023-05-16 11:47:17.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_optim.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)    19353 2023-05-16 11:28:53.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_train.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     2926 2023-05-01 20:45:05.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/trainer.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     2285 2023-05-14 07:21:18.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers/utils.py
+drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-05-16 12:03:58.670513 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      786 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/PKG-INFO
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      605 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/SOURCES.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)        1 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/dependency_links.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       20 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/entry_points.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       37 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/requires.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       27 2023-05-16 12:03:58.000000 micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/top_level.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       79 2023-05-16 12:03:58.674513 micro_trainer_transformers-0.0.2/setup.cfg
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      989 2023-05-12 19:02:04.000000 micro_trainer_transformers-0.0.2/setup.py
```

### Comparing `micro_trainer_transformers-0.0.1/PKG-INFO` & `micro_trainer_transformers-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micro_trainer_transformers
-Version: 0.0.1
+Version: 0.0.2
 Summary: Micro version train modules Transformers trainer....
 Home-page: https://github.com/utrobinmv/micro_trainer_transformers
 Author: Utrobin Mikhail
 Author-email: utrobinmv@yandex.ru
 License: Apache
 Description: Micro version train modules Transformers trainer....
```

### Comparing `micro_trainer_transformers-0.0.1/micro_trainer_transformers/arguments.py` & `micro_trainer_transformers-0.0.2/micro_trainer_transformers/arguments.py`

 * *Files identical despite different names*

### Comparing `micro_trainer_transformers-0.0.1/micro_trainer_transformers/core_args.py` & `micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 from .utils import current_time_in_second, time_in_second_to_textdate
 from .arguments import TrainingArguments
 
 @dataclass
 class TrainigParameters:
     """Класс для параметров тренировки по умолчанию"""
     debug: bool = False
-    max_train_steps: int = 0
+    max_train_steps: Optional[int] = None
     max_train_epochs: Optional[int] = None #При None max_train_epochs = max_train_steps / val_check_interval
+    gradient_accumulation_steps: int = 1
     evaluation_strategy: str = 'steps' #'steps' or 'epoch'. Делать валидацию либо каждую эпоху или через val_check_interval шагов
     warmup_steps: Optional[int] = None
     val_check_interval: int = 0 #Использовать всегда, если evaluation_strategy, устанавливать как len(ds) / (batch_size * evaluation_strategy)
     
     num_workers: int = 4
     seed: int = 42 #seed
     collate_fn: Optional[Any] = None
@@ -70,14 +71,17 @@
         self.accum_param()
         self.change_dir()
 
     def accum_param(self):
 
         #assert self.val_check_interval > 0 #Необходимо всегда установить val_check_interval
 
+        #TO DO
+        ########evaluation_strategy=<IntervalStrategy.STEPS: 'steps' ???
+
         if self.evaluation_strategy == 'epoch':
             if self.max_train_epochs is None:
                 self.max_train_epochs = round(self.max_train_steps / self.val_check_interval)
                 self.max_train_steps = self.val_check_interval * self.max_train_epochs #Пересчитаем до полного числа эпох
         elif self.evaluation_strategy == 'steps':
             if self.max_train_steps is None:
                 self.max_train_steps = self.val_check_interval * self.max_train_epochs #Пересчитаем до полного числа эпох
@@ -121,21 +125,28 @@
         self.max_train_steps = ta.max_steps
         self.batch_size = ta.per_device_train_batch_size
         self.gradient_accumulation_steps = ta.gradient_accumulation_steps
         self.val_check_interval = ta.eval_steps
         if ta.lr_scheduler_type:
             self.lr_scheduler_type = ta.lr_scheduler_type._value_
         self.seed = ta.seed
-        if ta.metric_for_best_model:
-            self.metric_monitor_name = ta.metric_for_best_model
+
+        #Убрал так как метрика по умолчанию 'loss', а у меня 'valid_loss'
+        # if ta.metric_for_best_model: 
+        #     self.metric_monitor_name = ta.metric_for_best_model
 
         self.tf32 = ta.tf32
         self.bf16 = ta.bf16
         self.fp16 = ta.fp16
         
+        if ta.warmup_steps > 0:
+            self.warmup_steps = ta.warmup_steps
+        elif ta.warmup_ratio > 0:
+            self.warmup_steps = int(ta.max_steps * ta.warmup_ratio)
+
         if ta.greater_is_better:
             if ta.greater_is_better == True:
                 self.metric_monitor_mode = 'max'
             else:
                 self.metric_monitor_mode = 'min'
         
         self.log_every_n_steps = ta.logging_steps
```

### Comparing `micro_trainer_transformers-0.0.1/micro_trainer_transformers/core_optim.py` & `micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_optim.py`

 * *Files 6% similar despite different names*

```diff
@@ -311,16 +311,36 @@
         elif name_sheduler == "cosine_with_restarts":
             scheduler = get_cosine_with_hard_restarts_schedule_with_warmup(optimizer, num_warmup_steps=num_warmup_steps, num_training_steps=num_training_steps)
         elif name_sheduler == "polynomial":
             scheduler = get_polynomial_decay_schedule_with_warmup(optimizer, num_warmup_steps=num_warmup_steps, num_training_steps=num_training_steps)
         elif name_sheduler == "ReduceLROnPlateau":
             #Для валидационных метрик работает только в режиме epoch. 
             #В режиме step можно запускать только для метрик трейн режима train_loss и др.
-            assert self.evaluation_strategy == 'epoch'
-            scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, self.training_params.metric_monitor_mode, **self.training_params.lr_scheduler_kwargs)
+            
+            assert self.training_params.evaluation_strategy == 'epoch'
+            
+            assert self.training_params.lr_scheduler_interval == 'epoch'
+            
+            default_kwargs = {'factor': 0.5, 'patience': 2, 'verbose': True}
+            
+            if isinstance(self.training_params.lr_scheduler_kwargs, dict):
+                kwargs = self.training_params.lr_scheduler_kwargs
+                
+                #Перенесем defaul параметры если они недоступны
+                for key in default_kwargs.keys():
+                    if key not in kwargs:
+                        kwargs[key] = default_kwargs[key]
+                        print(f'Оптимизатор ReduceLROnPlateau перенесен аргумент {key}: ', default_kwargs[key])
+            
+            else:
+                kwargs = default_kwargs
+                print('Оптимизатор ReduceLROnPlateau перенесены аргументы по умолчанию: ', kwargs)
+            
+            #default 
+            scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau(optimizer, self.training_params.metric_monitor_mode, **kwargs)
         elif name_sheduler == "OneCycleLR":
             scheduler = torch.optim.lr_scheduler.OneCycleLR(optimizer, 
                 max_lr = self.training_params.learning_rate,
                 total_steps=self.training_params.max_train_steps,
                 pct_start=0.1)
 
         return (
```

### Comparing `micro_trainer_transformers-0.0.1/micro_trainer_transformers/core_train.py` & `micro_trainer_transformers-0.0.2/micro_trainer_transformers/core_train.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,15 +76,19 @@
         #print('on fit start')
         #self.current_training_step = iter(range(self.training_params.max_train_steps))
         #self.pbar_train = iter(tqdm(range(self.training_params.max_train_steps),desc='Training model',leave=True))
         
         self.train_mode_start = True
         
         self.pbar_train.clear()
-        self.pbar_train.reset(total=self.training_params.max_train_steps)
+        if self.training_params.max_train_steps is None:
+            self.pbar_train.reset(total=self._trainer.estimated_stepping_batches)
+        else:
+            self.pbar_train.reset(total=self.training_params.max_train_steps)
+            
         if self.pbar_train_restore_n > 0: #restore from checkpoint
             self.pbar_train.n = self.pbar_train_restore_n
             self.pbar_train_restore_n = 0
         
         pass 
 
     def on_train_start(self):
@@ -374,41 +378,60 @@
                                                             mode=self.training_params.metric_monitor_mode,
                                                             monitor=self.training_params.metric_monitor_name,
                                                             verbose=True))
                 
                 
         
         if self.training_params.evaluation_strategy == 'steps':
-            val_check_interval = (self.training_params.val_check_interval-1)*self.training_params.gradient_accumulation_steps
+            val_check_interval = (self.training_params.val_check_interval)*self.training_params.gradient_accumulation_steps
             check_val_every_n_epoch=None
         elif self.training_params.evaluation_strategy == 'epoch':
             val_check_interval = None
             check_val_every_n_epoch=1
         
+        max_train_kwargs = {}
+        if self.training_params.max_train_steps is None:
+            max_train_steps = None
+            max_train_kwargs = {'max_epochs': self.training_params.max_train_epochs}
+        else:
+            max_train_steps = self.training_params.max_train_steps + (self.training_params.gradient_accumulation_steps * 2)
+            max_train_kwargs = {'max_steps': max_train_steps}
+
         precision = 32
         if self.training_params.bf16:
             precision = "bf16"
         elif self.training_params.fp16:
             precision = 16
         
+        #, max_steps=max_train_steps
         self.trainer = pl.Trainer(accelerator="auto", devices="auto", 
-                max_epochs=self.training_params.max_train_epochs, max_steps=self.training_params.max_train_steps,
+                **max_train_kwargs,
                 val_check_interval=val_check_interval,
                 accumulate_grad_batches=self.training_params.gradient_accumulation_steps,
                 check_val_every_n_epoch=check_val_every_n_epoch,
                 default_root_dir=self.training_params.path_best_model,
                 logger=loggers,
                 gradient_clip_val=self.training_params.max_grad_norm,
                 callbacks=callbacks,
                 reload_dataloaders_every_n_epochs = 1 if self.training_params.data_streaming_train else 0,
                 limit_val_batches = self.training_params.limit_val_batches,
                 log_every_n_steps = self.training_params.log_every_n_steps,
                 num_sanity_val_steps=2,
                 )
 
+    def model_vis(self):
+        #https://github.com/mert-kurttutan/torchview
+        from torchview import draw_graph
+
+        model_graph = draw_graph(
+            SimpleRNN(), input_size=(2, 3),
+            graph_name='RecursiveNet',
+            roll=True
+        )
+        model_graph.visual_graph        
 
     def lr_find(self,):
         self.create_trainer(mode = 'lr_find')
         
         self.train_mode_start = False
         
         lr_finder = self.trainer.tuner.lr_find(self, self.train_dataloader())
```

### Comparing `micro_trainer_transformers-0.0.1/micro_trainer_transformers/trainer.py` & `micro_trainer_transformers-0.0.2/micro_trainer_transformers/trainer.py`

 * *Files identical despite different names*

### Comparing `micro_trainer_transformers-0.0.1/micro_trainer_transformers/utils.py` & `micro_trainer_transformers-0.0.2/micro_trainer_transformers/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import os
 import torch
 import numpy as np
 import random
 import json
 from json import JSONEncoder
 
+def division(a,b):
+    return a / b
+
 def current_time_in_second(): 
     #Возвращает время в секундах
     return round(time.time())
 
 def time_in_second_to_textdate(time_in_second):  
     #Преобразовывает секунды в текстовую дату
     local_time = time.localtime(time_in_second)
```

### Comparing `micro_trainer_transformers-0.0.1/micro_trainer_transformers.egg-info/PKG-INFO` & `micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micro-trainer-transformers
-Version: 0.0.1
+Version: 0.0.2
 Summary: Micro version train modules Transformers trainer....
 Home-page: https://github.com/utrobinmv/micro_trainer_transformers
 Author: Utrobin Mikhail
 Author-email: utrobinmv@yandex.ru
 License: Apache
 Description: Micro version train modules Transformers trainer....
```

### Comparing `micro_trainer_transformers-0.0.1/micro_trainer_transformers.egg-info/SOURCES.txt` & `micro_trainer_transformers-0.0.2/micro_trainer_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micro_trainer_transformers-0.0.1/setup.py` & `micro_trainer_transformers-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 if os.path.exists("README.md"):
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
 
 setuptools.setup(
     name="micro_trainer_transformers",
-    version="0.0.1",
+    version="0.0.2",
     author="Utrobin Mikhail",
     author_email="utrobinmv@yandex.ru",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/utrobinmv/micro_trainer_transformers",
     packages=setuptools.find_packages(),
     license="Apache",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=['pytorch-lightning<=2.0','torch','datasets'],
+    install_requires=['pytorch-lightning<2.0','torch','datasets'],
     entry_points={
         "console_scripts": []
     }
 )
```

