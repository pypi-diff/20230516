# Comparing `tmp/torchaction-0.0.2.dev1.tar.gz` & `tmp/torchaction-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchaction-0.0.2.dev1.tar", last modified: Mon Feb 27 13:52:28 2023, max compression
+gzip compressed data, was "torchaction-0.0.3.tar", last modified: Tue May 16 11:54:11 2023, max compression
```

## Comparing `torchaction-0.0.2.dev1.tar` & `torchaction-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,7 @@
-drwxrwxrwx   0        0        0        0 2023-02-27 13:52:28.164631 torchaction-0.0.2.dev1/
--rw-rw-rw-   0        0        0     1088 2023-02-24 05:37:01.000000 torchaction-0.0.2.dev1/LICENSE
--rw-rw-rw-   0        0        0     3617 2023-02-27 13:52:28.163631 torchaction-0.0.2.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     3311 2023-02-27 13:51:52.000000 torchaction-0.0.2.dev1/README.md
--rw-rw-rw-   0        0        0     1093 2023-02-27 13:31:19.000000 torchaction-0.0.2.dev1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-27 13:52:28.164631 torchaction-0.0.2.dev1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-27 13:52:28.122907 torchaction-0.0.2.dev1/src/
-drwxrwxrwx   0        0        0        0 2023-02-27 13:52:28.157642 torchaction-0.0.2.dev1/src/torchaction/
--rw-rw-rw-   0        0        0        0 2023-02-27 01:36:21.000000 torchaction-0.0.2.dev1/src/torchaction/__init__.py
--rw-rw-rw-   0        0        0     7099 2023-02-27 13:51:08.000000 torchaction-0.0.2.dev1/src/torchaction/actions.py
--rw-rw-rw-   0        0        0      513 2023-02-27 00:51:11.000000 torchaction-0.0.2.dev1/src/torchaction/meanloss.py
--rw-rw-rw-   0        0        0     1490 2023-02-27 05:11:53.000000 torchaction-0.0.2.dev1/src/torchaction/parse_args.py
-drwxrwxrwx   0        0        0        0 2023-02-27 13:52:28.163631 torchaction-0.0.2.dev1/src/torchaction.egg-info/
--rw-rw-rw-   0        0        0     3617 2023-02-27 13:52:28.000000 torchaction-0.0.2.dev1/src/torchaction.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-02-27 13:52:28.000000 torchaction-0.0.2.dev1/src/torchaction.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-27 13:52:28.000000 torchaction-0.0.2.dev1/src/torchaction.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-02-27 13:52:28.000000 torchaction-0.0.2.dev1/src/torchaction.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      193 2023-02-27 13:52:28.000000 torchaction-0.0.2.dev1/src/torchaction.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-02-27 13:52:28.000000 torchaction-0.0.2.dev1/src/torchaction.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1088 2023-05-15 11:52:23.370771 torchaction-0.0.3/LICENSE
+-rw-r--r--   0        0        0      967 2023-05-16 08:30:17.948485 torchaction-0.0.3/README.md
+-rw-r--r--   0        0        0      511 2023-05-16 11:54:11.588622 torchaction-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      130 2023-05-16 09:16:46.835290 torchaction-0.0.3/torchaction/__init__.py
+-rw-r--r--   0        0        0     6537 2023-05-16 09:20:37.676813 torchaction-0.0.3/torchaction/actions.py
+-rw-r--r--   0        0        0     3756 2023-05-16 09:00:37.685140 torchaction-0.0.3/torchaction/utils.py
+-rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 torchaction-0.0.3/PKG-INFO
```

### Comparing `torchaction-0.0.2.dev1/LICENSE` & `torchaction-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torchaction-0.0.2.dev1/src/torchaction/actions.py` & `torchaction-0.0.3/torchaction/actions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,151 +1,114 @@
 from typing import *
+import argparse
 from pathlib import Path
 from tqdm import tqdm
 import torch
-from torch.utils.data import random_split, Dataset, DataLoader
+from torch.utils.data import Dataset, DataLoader
 from tensorboardX import SummaryWriter
-from .parse_args import parse_args
-from .meanloss import MeanLoss
+import torchmetrics
+from .utils import check_device, split_dataset, load_model, MeanLoss
 
 
-def compare_metrics(p1, p2, names):
-    for name in names:
-        if p1[name] > p2[name]:
-            return True
-    return False
-
-
-class BasicAction:
-    def __init__(self) -> None:
-        self.parse(parse_args())
-        self.init_paras()
-
-    def check_device(self, gpus):
-        gpus=[int(x) for x in gpus.split(',')] if gpus else []
-        gpu_nums=len(gpus)
-        use_device='cpu'
-        if gpu_nums:
-            assert torch.cuda.is_available(),\
-                "Please update torch's version with cuda, you can download torch-cuda versions in https://pytorch.org/. "
-            if gpu_nums>1:
-                self.GPUS=gpus
-            use_device="cuda:{}".format(gpus[0])
-        print("Using Device {},model load into device {}".format(gpus,use_device))
-        return torch.device(use_device)
-
-    def parse(self, args):
-        # dataset
-        self.ROOT:str = args.root
-        self.NUM_CLASSES:int = args.num_classes
-        self.SPLIT_RATE:float = args.split_rate
-        # train
-        self.CKPT:str = args.ckpt
-        self.GPUS:list = []
-        self.DEVICE = self.check_device(args.gpus)
-        self.EPOCHS:int = args.epochs
-        self.BATCH_SIZE:int = args.batch_size
-        self.LR:float = args.lr
-        # save
-        self.SAVE_NAME:str = args.save_name
-        self.SAVE_SUFFIX:str = args.save_suffix
-
-    def init_paras(self):
-        # parameters
-        self.START_EPOCH:int = 0
-        # variables
-        self.dataset: Dataset = None
-        self.model: torch.nn.Module = None
-        self.loss_fun: Any = None
-        self.optimizer_fun: Any = None
-        self.output_formater = lambda x: x
-        self.train_metrics: Dict[str, Any] = None
-        self.valid_metrics: Dict[str, Any] = None
-        self.best_ckpt_selectors: List = None
-
-    def prepare_data(self):
-        dataset_length = len(self.dataset)
-        train_dataset_length = round(self.SPLIT_RATE * dataset_length)
-        valid_dataset_length = dataset_length - train_dataset_length
-        self.train_dataset, self.val_dataset = random_split(
-            self.dataset, [train_dataset_length, valid_dataset_length]
+class TrainAction:
+    def __init__(
+        self,
+        args: argparse.Namespace,
+        dataset: Dataset,
+        model: torch.nn.Module,
+        optimizer: torch.optim.Optimizer,
+        loss_func,
+        split_randomly: bool = False,
+        show_progress_bar: bool = True,
+    ) -> None:
+        # print progress bar or not
+        self.show_progress_bar = show_progress_bar
+        # parse args
+        self.args = args
+        # check device
+        self.device, self.gpus = check_device(self.args.gpus)
+        # prepare dataset
+        self.train_dataset, self.val_dataset = split_dataset(
+            dataset, self.args.split, split_randomly
         )
-        
+        # prepare dataloader
         self.train_dataloader = DataLoader(
-            dataset=self.train_dataset, batch_size=self.BATCH_SIZE, shuffle=True
+            dataset=self.train_dataset, batch_size=self.args.batch_size, shuffle=True
         )
         self.val_dataloader = DataLoader(
-            dataset=self.val_dataset, batch_size=self.BATCH_SIZE, shuffle=False
+            dataset=self.val_dataset, batch_size=self.args.batch_size, shuffle=False
         )
-
-    def prepare_model(self):
-        # put model into device
-        if self.GPUS:
-            self.model=torch.nn.DataParallel(self.model,device_ids=self.GPUS)
-        if self.CKPT:
-            checkpoint = torch.load(self.CKPT,map_location="cpu")
-            self.model.load_state_dict(checkpoint["model_state_dict"])
-            self.START_EPOCH = checkpoint["epoch"]
-        self.model.to(self.DEVICE)
-        # init optimizer
-        self.optimizer = self.optimizer_fun(self.model.parameters(),self.LR)
-        if self.CKPT:
+        # load model
+        checkpoint = None
+        if self.args.ckpt and Path(self.args.ckpt).exists():
+            print("Loading checkpoint...")
+            checkpoint = torch.load(self.args.ckpt, map_location="cpu")
+        self.model, self.epoch_start = load_model(
+            model, checkpoint, self.device, self.gpus
+        )
+        # load optimizer
+        self.optimizer = optimizer
+        if checkpoint:
             self.optimizer.load_state_dict(checkpoint["optimizer_state_dict"])
-
-    def prepare_metrics(self):
-        self.train_loss = MeanLoss(self.loss_fun)
-        self.valid_loss = MeanLoss(self.loss_fun)
-        self.best_metrics = {}
-        self.last_metrics = {}
-        for name in self.train_metrics.keys():
-            self.best_metrics.setdefault(name, 0)
-            self.last_metrics.setdefault(name, 0)
-        self.train_writer = SummaryWriter("logs/{}/train".format(self.SAVE_NAME))
-        self.valid_writer = SummaryWriter("logs/{}/valid".format(self.SAVE_NAME))
+        # prepare loss
+        self.train_loss = MeanLoss(loss_func)
+        self.valid_loss = MeanLoss(loss_func)
+        # prepare metrics
+        self.train_metrics = {
+            "acc": torchmetrics.Accuracy(task="multiclass", num_classes=self.args.nc),
+        }
+        self.valid_metrics = {
+            "acc": torchmetrics.Accuracy(task="multiclass", num_classes=self.args.nc),
+        }
+        self.best_ckpt_selectors = ["acc"]
+        self.last_metrics = dict(
+            zip(self.best_ckpt_selectors, [0] * len(self.best_ckpt_selectors))
+        )
+        self.best_metrics = dict(
+            zip(self.best_ckpt_selectors, [0] * len(self.best_ckpt_selectors))
+        )
+        # record
+        self.train_writer = SummaryWriter("logs/{}/train".format(self.args.save_name))
+        self.valid_writer = SummaryWriter("logs/{}/valid".format(self.args.save_name))
 
     def train(self):
-        assert self.dataset, "Dataset not found"
-        assert self.model, "Model not set"
-        assert self.loss_fun, "loss function should be defined"
-        assert self.optimizer_fun, "optimizer should be defined"
-        self.prepare_data()
-        self.prepare_model()
-        self.prepare_metrics()
-        for epoch in range(self.EPOCHS):
-            if epoch < self.START_EPOCH:
+        for epoch in range(self.args.epochs):
+            if epoch < self.epoch_start:
                 continue
-            self.run_single_epoch(epoch, train=True)
-            self.run_single_epoch(epoch, train=False)
+            self.run_epoch(epoch, train=True)
+            self.run_epoch(epoch, train=False)
             self.record_epoch(epoch)
 
-    def run_single_epoch(self, epoch, train=True):
+    def run_epoch(self, epoch, train=True):
         self.model.train() if train else self.model.eval()
-        bar = tqdm(self.train_dataloader if train else self.val_dataloader)
+        if self.show_progress_bar:
+            bar = tqdm(self.train_dataloader if train else self.val_dataloader)
         for batch, (x, y) in enumerate(bar):
             self.optimizer.zero_grad()
-            x = x.to(self.DEVICE)
-            y = y.to(self.DEVICE)
+            x, y = self.before_batch(x, y, batch)
+            x = x.to(self.device)
+            y = y.to(self.device)
             output = self.model(x)
             loss_mode = self.train_loss if train else self.valid_loss
             loss_val = loss_mode(output, y)
             self.optimizer.step()
             # batch metric
-            self.train_loss
-            y_predict = self.output_formater(output)
-            bar.desc = "mode:{},epoch:{}/{},batch:{}/{},loss:{:.3f}".format(
-                "train" if train else "valid",
-                epoch + 1,
-                self.EPOCHS,
-                batch + 1,
-                len(bar),
-                loss_val,
-            )
+            y_predict = self.after_batch(x, y, output, batch)
             metrics = self.train_metrics if train else self.valid_metrics
             for metric in metrics.values():
-                metric.update(y_predict.to('cpu'), y.to('cpu'))
+                metric.update(y_predict.to("cpu"), y.to("cpu"))
+            if self.show_progress_bar:
+                bar.desc = "mode:{},epoch:{}/{},batch:{}/{},loss:{:.3f}".format(
+                    "train" if train else "valid",
+                    epoch + 1,
+                    self.args.epochs,
+                    batch + 1,
+                    len(bar),
+                    loss_val,
+                )
 
     def record_epoch(self, epoch):
         self.train_writer.add_scalar("loss", self.train_loss.compute(), epoch)
         self.valid_writer.add_scalar("loss", self.valid_loss.compute(), epoch)
         self.train_loss.reset()
         self.valid_loss.reset()
         for name, metric in self.train_metrics.items():
@@ -153,31 +116,62 @@
             metric.reset()
             self.last_metrics[name] = val
             self.train_writer.add_scalar(name, val, epoch)
 
         for name, metric in self.valid_metrics.items():
             self.valid_writer.add_scalar(name, metric.compute(), epoch)
             metric.reset()
+
+        self.after_metrics(self.train_metrics, self.valid_metrics)
         self.save_best_ckpt(epoch)
         self.save_ckpt(epoch, "last")
 
     def save_ckpt(self, epoch, mode):
         Path("weights").mkdir(parents=True, exist_ok=True)
-        if self.GPUS:
-            out_model=self.model.module
+        if self.gpus:
+            out_model = self.model.module
         else:
-            out_model=self.model
+            out_model = self.model
         torch.save(
             {
                 "model_state_dict": out_model.state_dict(),
                 "optimizer_state_dict": self.optimizer.state_dict(),
                 "epoch": epoch,
             },
-            "weights/{}_ckpt_{}.{}".format(mode, self.SAVE_NAME, self.SAVE_SUFFIX),
+            "weights/{}_ckpt_{}.pth".format(mode, self.args.save_name),
         )
 
     def save_best_ckpt(self, epoch):
-        if compare_metrics(
-            self.last_metrics, self.best_metrics, self.best_ckpt_selectors
-        ):
+        if self.last_metrics["acc"] > self.best_metrics["acc"]:
             self.best_metrics = self.last_metrics.copy()
             self.save_ckpt(epoch, "best")
+
+    def before_batch(self, x, y, batch):
+        return x, y
+
+    def after_batch(self, x, y, output, batch):
+        return output
+
+    def after_metrics(self, train_metrics, valid_metrics):
+        pass
+    
+    def test(self,x):
+        self.model.eval()
+        return self.model(x)
+
+
+class TestAction:
+    def __init__(
+        self,
+        args: argparse.Namespace,
+        model: torch.nn.Module
+    ) -> None:
+        # parse args
+        self.args = args
+        # check device
+        self.device, self.gpus = check_device(args.gpus)
+        # prepare model
+        checkpoint = torch.load(args.ckpt, map_location="cpu")
+        self.model, _ = load_model(model, checkpoint, self.device, self.gpus)
+        
+    def test(self,x):
+        return self.model(x)
```

