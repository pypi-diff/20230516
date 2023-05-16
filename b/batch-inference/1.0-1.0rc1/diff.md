# Comparing `tmp/batch_inference-1.0-py3-none-any.whl.zip` & `tmp/batch_inference-1.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,31 @@
-Zip file size: 23888 bytes, number of entries: 29
--rw-rw-rw-  2.0 fat      258 b- defN 23-May-16 09:38 batch_inference/__init__.py
--rw-rw-rw-  2.0 fat      903 b- defN 23-May-16 09:38 batch_inference/batch_context.py
--rw-rw-rw-  2.0 fat     2037 b- defN 23-May-16 09:38 batch_inference/decorators.py
--rw-rw-rw-  2.0 fat      457 b- defN 23-May-16 09:38 batch_inference/logger.py
--rw-rw-rw-  2.0 fat     5523 b- defN 23-May-16 09:38 batch_inference/model_host.py
--rw-rw-rw-  2.0 fat     2629 b- defN 23-May-16 09:38 batch_inference/remote_model_host.py
--rw-rw-rw-  2.0 fat      101 b- defN 23-May-16 09:38 batch_inference/aio/__init__.py
--rw-rw-rw-  2.0 fat      759 b- defN 23-May-16 09:38 batch_inference/aio/batch_context.py
--rw-rw-rw-  2.0 fat     6637 b- defN 23-May-16 09:38 batch_inference/aio/model_host.py
--rw-rw-rw-  2.0 fat       96 b- defN 23-May-16 09:38 batch_inference/aio/remote_model_host/__init__.py
--rw-rw-rw-  2.0 fat     1330 b- defN 23-May-16 09:38 batch_inference/aio/remote_model_host/model_host_client.py
--rw-rw-rw-  2.0 fat     1373 b- defN 23-May-16 09:38 batch_inference/aio/remote_model_host/model_host_pb2.py
--rw-rw-rw-  2.0 fat     2897 b- defN 23-May-16 09:38 batch_inference/aio/remote_model_host/model_host_pb2_grpc.py
--rw-rw-rw-  2.0 fat     3280 b- defN 23-May-16 09:38 batch_inference/aio/remote_model_host/model_host_server.py
--rw-rw-rw-  2.0 fat      726 b- defN 23-May-16 09:38 batch_inference/aio/remote_model_host/msgpack_serialization.py
--rw-rw-rw-  2.0 fat     2952 b- defN 23-May-16 09:38 batch_inference/aio/remote_model_host/remote_model_host.py
--rw-rw-rw-  2.0 fat      199 b- defN 23-May-16 09:38 batch_inference/batcher/__init__.py
--rw-rw-rw-  2.0 fat     1161 b- defN 23-May-16 09:38 batch_inference/batcher/batcher.py
--rw-rw-rw-  2.0 fat     4365 b- defN 23-May-16 09:38 batch_inference/batcher/bucket_seq_batcher.py
--rw-rw-rw-  2.0 fat     3118 b- defN 23-May-16 09:38 batch_inference/batcher/concat_batcher.py
--rw-rw-rw-  2.0 fat     1264 b- defN 23-May-16 09:38 batch_inference/batcher/multi_batcher.py
--rw-rw-rw-  2.0 fat     2745 b- defN 23-May-16 09:38 batch_inference/batcher/seq_batcher.py
--rw-rw-rw-  2.0 fat      602 b- defN 23-May-16 09:38 batch_inference/batcher/tensor_ops_np.py
--rw-rw-rw-  2.0 fat      559 b- defN 23-May-16 09:38 batch_inference/batcher/tensor_ops_pt.py
--rw-rw-rw-  2.0 fat     1162 b- defN 23-May-16 09:39 batch_inference-1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4798 b- defN 23-May-16 09:39 batch_inference-1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-16 09:39 batch_inference-1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 23-May-16 09:39 batch_inference-1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2764 b- defN 23-May-16 09:39 batch_inference-1.0.dist-info/RECORD
-29 files, 54803 bytes uncompressed, 19302 bytes compressed:  64.8%
+Zip file size: 23155 bytes, number of entries: 29
+-rw-rw-rw-  2.0 fat      258 b- defN 23-May-15 03:03 batch_inference/__init__.py
+-rw-rw-rw-  2.0 fat      903 b- defN 23-May-15 03:03 batch_inference/batch_context.py
+-rw-rw-rw-  2.0 fat     2037 b- defN 23-May-15 03:03 batch_inference/decorators.py
+-rw-rw-rw-  2.0 fat      457 b- defN 23-May-15 03:03 batch_inference/logger.py
+-rw-rw-rw-  2.0 fat     5418 b- defN 23-May-15 03:03 batch_inference/model_host.py
+-rw-rw-rw-  2.0 fat     2629 b- defN 23-May-15 03:03 batch_inference/remote_model_host.py
+-rw-rw-rw-  2.0 fat      101 b- defN 23-May-15 03:03 batch_inference/aio/__init__.py
+-rw-rw-rw-  2.0 fat      680 b- defN 23-May-15 03:03 batch_inference/aio/batch_context.py
+-rw-rw-rw-  2.0 fat     6273 b- defN 23-May-15 03:03 batch_inference/aio/model_host.py
+-rw-rw-rw-  2.0 fat       96 b- defN 23-May-15 03:03 batch_inference/aio/remote_model_host/__init__.py
+-rw-rw-rw-  2.0 fat     1330 b- defN 23-May-15 03:03 batch_inference/aio/remote_model_host/model_host_client.py
+-rw-rw-rw-  2.0 fat     1373 b- defN 23-May-15 03:03 batch_inference/aio/remote_model_host/model_host_pb2.py
+-rw-rw-rw-  2.0 fat     2897 b- defN 23-May-15 03:03 batch_inference/aio/remote_model_host/model_host_pb2_grpc.py
+-rw-rw-rw-  2.0 fat     3166 b- defN 23-May-15 03:03 batch_inference/aio/remote_model_host/model_host_server.py
+-rw-rw-rw-  2.0 fat      726 b- defN 23-May-15 03:03 batch_inference/aio/remote_model_host/msgpack_serialization.py
+-rw-rw-rw-  2.0 fat     2879 b- defN 23-May-15 03:03 batch_inference/aio/remote_model_host/remote_model_host.py
+-rw-rw-rw-  2.0 fat      199 b- defN 23-May-15 03:03 batch_inference/batcher/__init__.py
+-rw-rw-rw-  2.0 fat     1161 b- defN 23-May-15 03:03 batch_inference/batcher/batcher.py
+-rw-rw-rw-  2.0 fat     4365 b- defN 23-May-15 03:03 batch_inference/batcher/bucket_seq_batcher.py
+-rw-rw-rw-  2.0 fat     3118 b- defN 23-May-15 03:03 batch_inference/batcher/concat_batcher.py
+-rw-rw-rw-  2.0 fat     1264 b- defN 23-May-15 03:03 batch_inference/batcher/multi_batcher.py
+-rw-rw-rw-  2.0 fat     2745 b- defN 23-May-15 03:03 batch_inference/batcher/seq_batcher.py
+-rw-rw-rw-  2.0 fat      602 b- defN 23-May-15 03:03 batch_inference/batcher/tensor_ops_np.py
+-rw-rw-rw-  2.0 fat      559 b- defN 23-May-15 03:03 batch_inference/batcher/tensor_ops_pt.py
+-rw-rw-rw-  2.0 fat     1162 b- defN 23-May-15 03:04 batch_inference-1.0rc1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2982 b- defN 23-May-15 03:04 batch_inference-1.0rc1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-15 03:04 batch_inference-1.0rc1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 23-May-15 03:04 batch_inference-1.0rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     2779 b- defN 23-May-15 03:04 batch_inference-1.0rc1.dist-info/RECORD
+29 files, 52267 bytes uncompressed, 18539 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -66,23 +66,23 @@
 
 Filename: batch_inference/batcher/tensor_ops_np.py
 Comment: 
 
 Filename: batch_inference/batcher/tensor_ops_pt.py
 Comment: 
 
-Filename: batch_inference-1.0.dist-info/LICENSE
+Filename: batch_inference-1.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: batch_inference-1.0.dist-info/METADATA
+Filename: batch_inference-1.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: batch_inference-1.0.dist-info/WHEEL
+Filename: batch_inference-1.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: batch_inference-1.0.dist-info/top_level.txt
+Filename: batch_inference-1.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: batch_inference-1.0.dist-info/RECORD
+Filename: batch_inference-1.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## batch_inference/model_host.py

```diff
@@ -28,20 +28,17 @@
         if model_cls is None and model_obj is None:
             raise RuntimeError(f"Either model_cls or model_obj must be provided")
         self.model_cls = model_cls
         self.model_obj = model_obj
         self.batcher = batcher
         self.max_batch_size = max_batch_size
         self.wait_n = wait_n
-        if self.wait_n > self.max_batch_size:
-            self.wait_n = self.max_batch_size
-        
         self.num_workers = num_workers
         self.wait_ms = wait_ms
-        self.cycle_time = 1.0
+        self.cycle_time = 0.1
         self.stopped = True
         # double queue size to avoid blocking
         self.batch_queue = [queue.Queue(maxsize=2 * max_batch_size)] * num_workers
         self.threads = []
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         if self.model_obj is not None:
@@ -69,61 +66,62 @@
             thread = threading.Thread(
                 target=self._wait_batch_ready_and_process, args=(i,)
             )
             thread.start()
             self.threads.append(thread)
 
     def stop(self):
+        logger.debug(f"stop() is called")
         self.stopped = True
-        logger.debug(f"notify worker threads to stop")
+        logger.debug(f"notify worker thread to stop")
         for thread in self.threads:
             thread.join()
-        logger.debug(f"all worker threads are stopped")
+        logger.debug(f"worker thread is stopped")
 
     def _get_new_batch(self, idx) -> List[BatchContext]:
-        # blocking until get at least one request
+        # blocking util get at least request
         try:
             batch_list: List[BatchContext] = [
                 self.batch_queue[idx].get(block=True, timeout=self.cycle_time)
             ]
         except queue.Empty:
             return []
 
-        # get more already arrived requests
+        # append the left requests
         while (
             len(batch_list) < self.max_batch_size and not self.batch_queue[idx].empty()
         ):
             try:
                 batch_list.append(self.batch_queue[idx].get(block=False))
             except queue.Empty:
                 break
 
         # check if we still need to wait
-        if self.wait_ms <= 0 or len(batch_list) >= self.wait_n:
+        if self.wait_ms < 0 or len(batch_list) >= self.wait_n:
             return batch_list
 
         # wait for `wait_ms` ms to see if there's more requests to batch
-        current_time = time.perf_counter()
+        current_time = time.time()
         end_time = current_time + self.wait_ms / 1000.0
         while end_time - current_time > 0 and len(batch_list) < self.wait_n:
             try:
                 batch_list.append(
                     self.batch_queue[idx].get(timeout=end_time - current_time)
                 )
-                current_time = time.perf_counter()
+                current_time = time.time()
             except queue.Empty:
                 break
         return batch_list
 
     def _wait_batch_ready_and_process(self, idx):
         while not self.stopped:
             batch_list = self._get_new_batch(idx)
             if len(batch_list) == 0:
                 continue
-            # logger.info(f"get batch of size {len(batch_list)}")
+            logging.debug(f"Batch Size: {len(batch_list)}")
             try:
                 requests = [batch_ctx.request for batch_ctx in batch_list]
                 batched_requests, unbatch_ctx = self.batcher.batch(requests)
                 if issubclass(type(self.batcher), MultiBatcher):
                     batched_responses = []
                     for i in batched_requests:
                         batched_responses.append(self.model_obj.predict_batch(*i))
```

## batch_inference/aio/batch_context.py

```diff
@@ -2,26 +2,26 @@
 # Licensed under the MIT License.
 
 import asyncio
 from typing import Any
 
 
 class BatchContext:
-    def __init__(self, request: Any) -> None:
-        self.request = request
-        self.response = None
+    def __init__(self) -> None:
+        self.requests = []
+        self.responses = []
+        self.result_ready = asyncio.Event()
         self.error = None
-        self.response_ready = asyncio.Event()
 
-    async def get_response(self) -> Any:
-        await self.response_ready.wait()
-        if self.error is not None:
-            raise self.error
-        return self.response
-
-    def set_response(self, response: Any = None):
-        self.response = response
-        self.response_ready.set()
+    def size(self):
+        return len(self.requests)
+
+    def add_request(self, request: Any):
+        self.requests.append(request)
+        return len(self.requests) - 1
+
+    def set_result_ready(self):
+        self.result_ready.set()
 
     def set_error(self, error: Exception):
         self.error = error
-        self.response_ready.set()
+        self.result_ready.set()
```

## batch_inference/aio/model_host.py

```diff
@@ -1,17 +1,16 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import asyncio
 import sys
 import threading
-import time
 from types import TracebackType
-from typing import Any, List, Optional, Type
+from typing import Any, Optional, Type
 
 from ..batcher.batcher import Batcher
 from ..batcher.multi_batcher import MultiBatcher
 from ..logger import logger
 from .batch_context import BatchContext
 
 
@@ -20,15 +19,14 @@
         self,
         model_cls=None,
         model_obj=None,
         batcher: Batcher = None,
         max_batch_size=32,
         wait_ms: int = 5,
         wait_n: int = 16,
-        num_workers: int = 1,
         event_loop=None,
     ):
         if model_cls is None and model_obj is None:
             raise RuntimeError(f"Either model_cls or model_obj must be provided")
         self.model_cls = model_cls
         self.model_obj = model_obj
         self.batcher = batcher
@@ -40,123 +38,121 @@
         self.wait_n = wait_n
         if self.wait_n > self.max_batch_size:
             self.wait_n = self.max_batch_size
 
         self.event_loop = event_loop
         self.cv = None
         self.batch_queue = []
-        self.num_workers = num_workers
-        self.threads = []
+        self.thread = None
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         if self.model_obj is not None:
             raise RuntimeError(
                 f"model_obj has already been set, you can't call __call__() to create it again",
             )
         # pass the originl arguments and construtor the origial model instance.
         self.model_obj = self.model_cls(*args, **kwds)
         return self
 
     async def predict(self, *input_list):
         async with self.cv:
-            batch_ctx = BatchContext(input_list)
-            self.batch_queue.append(batch_ctx)
+            is_first_request = len(self.batch_queue) == 0
+            if is_first_request or self.batch_queue[-1].size() >= self.max_batch_size:
+                self.batch_queue.append(BatchContext())
+            #     logger.debug(f'I am the first query of a new batch')
+            # else:
+            #     logger.debug(f'I am added to an existing batch')
+            last_batch: BatchContext = self.batch_queue[-1]
+            idx = last_batch.add_request(input_list)
             self.cv.notify(n=1)
-        response = await batch_ctx.get_response()
-        return response
+
+        await last_batch.result_ready.wait()
+        if last_batch.error is not None:
+            raise last_batch.error
+        return last_batch.responses[idx]
 
     async def start(self):
         if self.event_loop is None:
             self.event_loop = asyncio.get_event_loop()
 
         if sys.version_info >= (3, 10):
             batch_queue_lock = asyncio.Lock()
             self.cv = asyncio.Condition(lock=batch_queue_lock)
         else:
             batch_queue_lock = asyncio.Lock(loop=self.event_loop)
             self.cv = asyncio.Condition(lock=batch_queue_lock, loop=self.event_loop)
-        for _ in range(self.num_workers):
-            thread = threading.Thread(target=self._wait_batch_ready_and_process)
-            thread.start()
-            self.threads.append(thread)
+        self.thread = threading.Thread(target=self._wait_batch_ready_and_process)
+        self.thread.start()
 
     async def stop(self):
+        logger.debug(f"stop() is called")
         async with self.cv:
             self.batch_queue.append(None)
-            self.cv.notify_all()
-        logger.debug(f"notify worker threads to stop")
-        for thread in self.threads:
-            await self.event_loop.run_in_executor(None, thread.join)
-        logger.debug(f"all worker threads are stopped")
+            self.cv.notify(n=1)
+        logger.debug(f"notify worker thread to stop")
+        await self.event_loop.run_in_executor(None, self.thread.join)
+        logger.debug(f"worker thread is stopped")
 
     async def _get_new_batch(self):
-        batch_list = []
+        # WorkerLoop will be notified when there's a new request
+        # take first BatchContext out of quueue
+        early_ret_n = self.wait_n
+        wait_timeout = -1
+        if self.wait_ms > 0:
+            wait_timeout = self.wait_ms / 1000.0  # in seconds
 
         async with self.cv:
             await self.cv.wait_for(lambda: len(self.batch_queue) > 0)
+            try:
+                await asyncio.wait_for(
+                    self.cv.wait_for(
+                        lambda: self.batch_queue[0]
+                        is None  # should exit, no more request
+                        or len(self.batch_queue[0].requests) >= early_ret_n,
+                    ),
+                    wait_timeout,
+                )
+            except asyncio.TimeoutError:
+                # logger.info(f'wait batch size to reach {early_ret_n} timeout, actual batch size={len(self.batch_queue[0].requests)}')
+                pass
+            batch_ctx: BatchContext = self.batch_queue.pop(0)
 
-            # get already arrived requests
-            while len(batch_list) < self.max_batch_size and len(self.batch_queue) > 0:
-                if self.batch_queue[0] is None:  # end of processing
-                    return batch_list
-                batch_list.append(self.batch_queue.pop(0))
-
-            # check if we still need to wait
-            if self.wait_ms <= 0 or len(batch_list) >= self.wait_n:
-                return batch_list
-
-            # wait for `wait_ms` ms to see if there's more requests to batch
-            current_time = time.perf_counter()
-            end_time = current_time + self.wait_ms / 1000.0
-            while current_time < end_time and len(batch_list) < self.wait_n:
-                try:
-                    await asyncio.wait_for(
-                        self.cv.wait_for(lambda: len(self.batch_queue) > 0),
-                        end_time - current_time,
-                    )
-                    if self.batch_queue[0] is None:  # end of processing
-                        return batch_list
-                    batch_list.append(self.batch_queue.pop(0))
-                    current_time = time.perf_counter()
-                except asyncio.TimeoutError:
-                    # logger.info(f'wait batch size to reach {self.wait_n} timeout(={self.wait_ms}ms), actual batch size={len(batch_list)}')
-                    break
-        return batch_list
+            return batch_ctx
 
     def _wait_batch_ready_and_process(self):
         while True:
-            batch_list = asyncio.run_coroutine_threadsafe(
-                self._get_new_batch(), self.event_loop
-            ).result()
-            if len(batch_list) == 0:
-                break
-            # logger.info(f"get batch of size {len(batch_list)}")
+            f = asyncio.run_coroutine_threadsafe(self._get_new_batch(), self.event_loop)
+            batch_ctx = f.result()
+
+            if batch_ctx is None:
+                return
+
+            # logger.info(f"get batch of size {len(batch_ctx.requests)}")
+
             try:
-                requests = [batch_ctx.request for batch_ctx in batch_list]
-                batched_requests, unbatch_ctx = self.batcher.batch(requests)
+                batched_requests, unbatch_ctx = self.batcher.batch(batch_ctx.requests)
                 if issubclass(type(self.batcher), MultiBatcher):
                     batched_responses = []
                     for i in batched_requests:
                         batched_responses.append(self.model_obj.predict_batch(*i))
                 else:
                     batched_responses = self.model_obj.predict_batch(*batched_requests)
-                responses = self.batcher.unbatch(
+                batch_ctx.responses = self.batcher.unbatch(
                     batched_responses,
                     unbatch_ctx,
                 )
-                for i, ctx in enumerate(batch_list):
-                    self.event_loop.call_soon_threadsafe(ctx.set_response, responses[i])
+                self.event_loop.call_soon_threadsafe(batch_ctx.set_result_ready)
             except Exception as e:
-                for ctx in batch_list:
-                    self.event_loop.call_soon_threadsafe(ctx.set_error, e)
+                self.event_loop.call_soon_threadsafe(
+                    lambda: batch_ctx.set_error(error=e),
+                )
                 logger.error(e, exc_info=True)
-        # logger.info(f'worker thread is stopped')
 
     async def __aenter__(self):
-        await self.start()
+        self.start()
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
```

## batch_inference/aio/remote_model_host/model_host_server.py

```diff
@@ -39,23 +39,21 @@
         file_lock,
         model_cls,
         grpc_port,
         batcher: Batcher,
         max_batch_size=32,
         wait_ms: int = 5,
         wait_n: int = 16,
-        num_workers: int = 1,
         event_loop=None,
     ):
         self.model_cls = model_cls
         self.batcher = batcher
         self.max_batch_size = max_batch_size
         self.wait_ms = wait_ms
         self.wait_n = wait_n
-        self.num_workers = num_workers
 
         if event_loop is None:
             self.event_loop = asyncio.get_event_loop()
         else:
             self.event_loop = event_loop
 
         self.grpc_port = grpc_port
@@ -67,15 +65,14 @@
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         self.model_host = ModelHost(
             model_cls=self.model_cls,
             batcher=self.batcher,
             max_batch_size=self.max_batch_size,
             wait_ms=self.wait_ms,
             wait_n=self.wait_n,
-            num_workers=self.num_workers,
             event_loop=self.event_loop,
         )(*args, **kwds)
         return self
 
     # read this for details of creating async grpc server:
     # https://github.com/grpc/grpc/blob/master/examples/python/helloworld/async_greeter_client.py
     async def start(self):
```

## batch_inference/aio/remote_model_host/remote_model_host.py

```diff
@@ -20,29 +20,27 @@
         self,
         model_cls,
         grpc_port,
         batcher: Batcher,
         max_batch_size=32,
         wait_ms: int = 5,
         wait_n: int = 16,
-        num_workers: int = 1,
         event_loop=None,
     ):
         file_lock = self._get_server_file_lock(grpc_port)
         self.is_server = file_lock is not None
         if self.is_server:
             self.processor = ModelHostServer(
                 file_lock,
                 model_cls,
                 grpc_port,
                 batcher,
                 max_batch_size=max_batch_size,
                 wait_ms=wait_ms,
                 wait_n=wait_n,
-                num_workers=num_workers,
                 event_loop=event_loop,
             )
         else:
             self.processor = ModelHostClient(grpc_port)
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         if self.is_server:
```

## Comparing `batch_inference-1.0.dist-info/LICENSE` & `batch_inference-1.0rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `batch_inference-1.0.dist-info/RECORD` & `batch_inference-1.0rc1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 batch_inference/__init__.py,sha256=o8mDEPAoYIQJDuXaKSzGG5Mv7xa6TmNAb2aj2EMArUc,258
 batch_inference/batch_context.py,sha256=DK6WS7lhBrVTiPmzFo5SmhYAfe4oOGlyA8TTXuiQ48c,903
 batch_inference/decorators.py,sha256=rQYygFKIh6jYrmuIGLx8yCZ5MF--7AoueUjVsgYVtuM,2037
 batch_inference/logger.py,sha256=aHL6b07Opr7zFqhMvf_h_fBTLRm21ZX4g3YeBsd-hEY,457
-batch_inference/model_host.py,sha256=nvfjWzdt3YIP9OkYhbzGHBaBXY_5yCXPuNRDY5ZihGU,5523
+batch_inference/model_host.py,sha256=NxDHVCvnkaZj-h4x4iM8odtNhWgozGisAbHyzkRlwHc,5418
 batch_inference/remote_model_host.py,sha256=EMEn9OAiH2FC8kKQgDpvHMut1wwFZiA2BLYNbLKsklw,2629
 batch_inference/aio/__init__.py,sha256=oripAu20ljFwauwj_EEB9sUWbdGxEgwa5c_hvBvhVOI,101
-batch_inference/aio/batch_context.py,sha256=_dB6jlf-s9a9ExpSxKZOClnwNGr2IQfG-ytJEcBkRfQ,759
-batch_inference/aio/model_host.py,sha256=jaOJin5Y-2lxeStLjRynjylkA4cdrqMcdpZj4tddDxs,6637
+batch_inference/aio/batch_context.py,sha256=5hB3GnnMrq1wBJbxBaHwf8hy4slofiaMstKzndbyQBc,680
+batch_inference/aio/model_host.py,sha256=ETsuSTvPA5e7S1xOHX0F2MW8qA6tAOYygoKegh4Gv0E,6273
 batch_inference/aio/remote_model_host/__init__.py,sha256=5K7xjH5l065Dv7kNZIQDG5mwE1Ua6i_WoRBc0NdSGfE,96
 batch_inference/aio/remote_model_host/model_host_client.py,sha256=HmmRPxlRUL5t6omJO-aQ8X_r6U7j3sbWQj55yEyqO6c,1330
 batch_inference/aio/remote_model_host/model_host_pb2.py,sha256=HA49qtc4XOrrn5Xsg4q2U7zhC14YCLa7N4jmpg5NYk8,1373
 batch_inference/aio/remote_model_host/model_host_pb2_grpc.py,sha256=pS3zlv8ehFxtGOQfVe6lZWRRDjf-UrNMpxIFrhGmGDE,2897
-batch_inference/aio/remote_model_host/model_host_server.py,sha256=1al3NwxX1QBICYHkBMIC9U8n2i044e-gtxNhe4rLEIE,3280
+batch_inference/aio/remote_model_host/model_host_server.py,sha256=ee9hrVVgOtB4604b1uq4KrGhdjEIDErPEK9-tF_ZF1Y,3166
 batch_inference/aio/remote_model_host/msgpack_serialization.py,sha256=TFYf8gIUSjS0ePrtkkGwZeE5ig6WjuMBihuIdhAxPNg,726
-batch_inference/aio/remote_model_host/remote_model_host.py,sha256=52_bK0sdyekjd8PGfnOW4tjagcZgn3_O_4n5e6pQCnc,2952
+batch_inference/aio/remote_model_host/remote_model_host.py,sha256=6LKNch64D8SwH7RO5Ccn-p9H0oGE9rsqXePUuRfsj2I,2879
 batch_inference/batcher/__init__.py,sha256=aJZ7B-H7hGw2lGlmwjDLMF62-wpiTrGGNnW0xm_ikqE,199
 batch_inference/batcher/batcher.py,sha256=MifBvPZAI1Ra_9HyMmUClNftErIsqBE0bUVHh5ER8eg,1161
 batch_inference/batcher/bucket_seq_batcher.py,sha256=RfwLGQFPB6XmBXFVnKfeQc_0xj9OJMoVIIifB4O7KuQ,4365
 batch_inference/batcher/concat_batcher.py,sha256=uRFT9yHjSHcSmXIBWDBm-zlmAQCR2LN7tvQzyzE50AE,3118
 batch_inference/batcher/multi_batcher.py,sha256=gQIxu9C3_03iWKoedvPYjXES_QkQyTWlbDnX52IPUA0,1264
 batch_inference/batcher/seq_batcher.py,sha256=7es00sOTePz4YbeY8xpvmrtP1FrwBDXaVORoRgu9uIo,2745
 batch_inference/batcher/tensor_ops_np.py,sha256=zdHnFMp0Oz3PUm6fsnhLD7VAjhme8Z5lKNJmoHetd7I,602
 batch_inference/batcher/tensor_ops_pt.py,sha256=rBehSZ14gvubRkmLvwaL_iP1qADRwYbE76Z1II4fStA,559
-batch_inference-1.0.dist-info/LICENSE,sha256=mQaUD2Gx8LUz-n2ZuvVReLKAj74RPqUd-_rYVyzNXys,1162
-batch_inference-1.0.dist-info/METADATA,sha256=d0PnzJ0LlqJJfOhUyMC4nKamqcmCfSsAooa0jAB3bOI,4798
-batch_inference-1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-batch_inference-1.0.dist-info/top_level.txt,sha256=AHAC3MTRbSjVNbH2dk8zWVcoFHjFoUqkm5v8bo39gIo,16
-batch_inference-1.0.dist-info/RECORD,,
+batch_inference-1.0rc1.dist-info/LICENSE,sha256=mQaUD2Gx8LUz-n2ZuvVReLKAj74RPqUd-_rYVyzNXys,1162
+batch_inference-1.0rc1.dist-info/METADATA,sha256=5Uk7URvYPn0Lesop4UHdF3oB6SxvOVrlG9BLf_gdlqQ,2982
+batch_inference-1.0rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+batch_inference-1.0rc1.dist-info/top_level.txt,sha256=AHAC3MTRbSjVNbH2dk8zWVcoFHjFoUqkm5v8bo39gIo,16
+batch_inference-1.0rc1.dist-info/RECORD,,
```

