# Comparing `tmp/tiny_ai_helper-0.1.3.tar.gz` & `tmp/tiny_ai_helper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_ai_helper-0.1.3.tar", last modified: Tue Mar 14 12:41:55 2023, max compression
+gzip compressed data, was "tiny_ai_helper-0.1.4.tar", last modified: Fri Apr  7 18:30:49 2023, max compression
```

## Comparing `tiny_ai_helper-0.1.3.tar` & `tiny_ai_helper-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-03-14 12:41:55.069274 tiny_ai_helper-0.1.3/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.3/LICENSE
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-03-14 12:41:55.069274 tiny_ai_helper-0.1.3/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.3/README.md
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-03-14 12:41:55.069274 tiny_ai_helper-0.1.3/setup.cfg
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     1029 2023-03-14 12:40:28.000000 tiny_ai_helper-0.1.3/setup.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-03-14 12:41:55.069274 tiny_ai_helper-0.1.3/tiny_ai_helper/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)    15585 2023-03-14 12:32:06.000000 tiny_ai_helper-0.1.3/tiny_ai_helper/Model.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     9625 2023-03-13 13:49:06.000000 tiny_ai_helper-0.1.3/tiny_ai_helper/Trainer.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      252 2023-03-14 12:40:04.000000 tiny_ai_helper-0.1.3/tiny_ai_helper/__init__.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     4723 2023-03-13 14:23:06.000000 tiny_ai_helper-0.1.3/tiny_ai_helper/layers.py
--rw-rw-r--   0 www-data  (1000) www-data  (1000)     8928 2023-03-14 10:03:30.000000 tiny_ai_helper-0.1.3/tiny_ai_helper/utils.py
-drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-03-14 12:41:55.069274 tiny_ai_helper-0.1.3/tiny_ai_helper.egg-info/
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-03-14 12:41:54.000000 tiny_ai_helper-0.1.3/tiny_ai_helper.egg-info/PKG-INFO
--rw-rw-r--   0 www-data  (1000) www-data  (1000)      304 2023-03-14 12:41:54.000000 tiny_ai_helper-0.1.3/tiny_ai_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-03-14 12:41:54.000000 tiny_ai_helper-0.1.3/tiny_ai_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-03-14 12:41:54.000000 tiny_ai_helper-0.1.3/tiny_ai_helper.egg-info/top_level.txt
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-07 18:30:49.516121 tiny_ai_helper-0.1.4/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1103 2023-03-09 17:46:27.000000 tiny_ai_helper-0.1.4/LICENSE
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-04-07 18:30:49.516121 tiny_ai_helper-0.1.4/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       74 2022-09-27 15:48:25.000000 tiny_ai_helper-0.1.4/README.md
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       38 2023-04-07 18:30:49.516121 tiny_ai_helper-0.1.4/setup.cfg
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     1029 2023-04-07 18:28:26.000000 tiny_ai_helper-0.1.4/setup.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-07 18:30:49.516121 tiny_ai_helper-0.1.4/tiny_ai_helper/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    14082 2023-04-07 11:12:37.000000 tiny_ai_helper-0.1.4/tiny_ai_helper/Model.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    10249 2023-04-07 17:50:21.000000 tiny_ai_helper-0.1.4/tiny_ai_helper/Trainer.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      367 2023-04-07 18:28:32.000000 tiny_ai_helper-0.1.4/tiny_ai_helper/__init__.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     6232 2023-03-23 11:28:02.000000 tiny_ai_helper-0.1.4/tiny_ai_helper/layers.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)     9071 2023-03-15 18:42:46.000000 tiny_ai_helper-0.1.4/tiny_ai_helper/mp.py
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)    14131 2023-04-07 17:46:52.000000 tiny_ai_helper-0.1.4/tiny_ai_helper/utils.py
+drwxrwxr-x   0 www-data  (1000) www-data  (1000)        0 2023-04-07 18:30:49.516121 tiny_ai_helper-0.1.4/tiny_ai_helper.egg-info/
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      784 2023-04-07 18:30:49.000000 tiny_ai_helper-0.1.4/tiny_ai_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)      325 2023-04-07 18:30:49.000000 tiny_ai_helper-0.1.4/tiny_ai_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)        1 2023-04-07 18:30:49.000000 tiny_ai_helper-0.1.4/tiny_ai_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 www-data  (1000) www-data  (1000)       15 2023-04-07 18:30:49.000000 tiny_ai_helper-0.1.4/tiny_ai_helper.egg-info/top_level.txt
```

### Comparing `tiny_ai_helper-0.1.3/LICENSE` & `tiny_ai_helper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_ai_helper-0.1.3/PKG-INFO` & `tiny_ai_helper-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny_ai_helper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

### Comparing `tiny_ai_helper-0.1.3/setup.py` & `tiny_ai_helper-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from setuptools import setup, find_packages
 from os.path import abspath, dirname, join
 
 setup(
 	name="tiny_ai_helper",
-	version="0.1.3",
+	version="0.1.4",
 	description="Tiny AI Helper for PyTorch",
 	long_description=open(join(abspath(dirname(__file__)), 'README.md'), encoding='utf-8').read(),
 	long_description_content_type='text/markdown',
 	author="Ildar Bikmamatov",
 	author_email="support@bayrell.org",
 	license="MIT License",
 	url = "https://github.com/bayrell/ai_helper",
```

### Comparing `tiny_ai_helper-0.1.3/tiny_ai_helper/Model.py` & `tiny_ai_helper-0.1.4/tiny_ai_helper/Model.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 ##
 # Tiny ai helper
 # Copyright (с) Ildar Bikmamatov 2022 - 2023 <support@bayrell.org>
 # License: MIT
 ##
 
-import torch, json, os
+import torch, time, json, math, gc, os
 from torch.utils.data import DataLoader, TensorDataset
 from .utils import TransformDataset, list_files, \
-    get_default_device, batch_to, tensor_size, load_json
+    get_default_device, batch_to, tensor_size, load_json, summary
 
 
 class Model:
     
     def __init__(self, name=None):
         self.device = None
         self.transform_x = None
@@ -95,21 +95,24 @@
         
         if optimizer is not None:
             self.optimizer = optimizer
         
         if scheduler is not None:
             self.scheduler = scheduler
         
-        if self.loss == None:
-            self.loss = nn.MSELoss()
+        if self.loss is None:
+            self.loss = torch.nn.MSELoss()
         
-        if self.optimizer == None:
-            self.optimizer = torch.optim.Adam(self.module.parameters(), lr=lr)
+        if self.optimizer is None:
+            try:
+                self.optimizer = torch.optim.Adam(self.module.parameters(), lr=lr)
+            except:
+                pass
         
-        if self.scheduler == None:
+        if self.scheduler is None and self.optimizer is not None:
             self.scheduler = torch.optim.lr_scheduler.ReduceLROnPlateau( self.optimizer )
         
     
     def to(self, device):
         self.module = self.module.to(device)
         self.device = device
     
@@ -118,14 +121,22 @@
         self.to( get_default_device() )
     
     
     def to_cpu(self):
         self.to( torch.device("cpu") )
     
     
+    def train(self):
+        self.module.train()
+    
+    
+    def eval(self):
+        self.module.eval()
+    
+    
     def load_file(self, file_path):
         
         """
         Load model from file
         """
         
         save_metrics = torch.load(file_path)
@@ -260,56 +271,73 @@
     
     
     def predict(self, x, batch_size=64):
         
         """
         Predict
         """
+         
+        if self.transform_x is not None:
+            x = self.transform_x(x)
+        
+        if self.device:
+            x = x.to( self.device )
+        
+        y = self.module(x)
         
-        y = None
+        return y
+    
+    
+    def predict_dataset(self, dataset, predict, batch_size=64, predict_obj=None):
         
-        if isinstance(x, torch.utils.data.Dataset):
+        """
+        Predict dataset
+        """
+        
+        loader = DataLoader(
+            dataset,
+            batch_size=batch_size,
+            drop_last=False,
+            shuffle=False
+        )
+        
+        self.module.eval()
+        
+        pos = 0
+        next_pos = 0
+        dataset_count = len(dataset)
+        time_start = time.time()
+        
+        for batch_x, batch_y in loader:
             
-            y = torch.tensor([])
+            if self.transform_x:
+                batch_x = self.transform_x(batch_x)
             
-            if self.transform_x is not None:
-                x = TransformDataset(
-                    x,
-                    transform_x=self.transform_x
-                )
+            if self.device:
+                batch_x = batch_to(batch_x, self.device)
             
-            loader = DataLoader(
-                x,
-                batch_size=batch_size,
-                drop_last=False,
-                shuffle=False
-            )
+            batch_predict = self.module(batch_x)
+            predict(batch_x, batch_y, batch_predict, predict_obj)
             
-            self.module.eval()
+            # Show progress
+            pos = pos + len(batch_x)
+            if pos > next_pos:
+                next_pos = pos + 16
+                t = str(round(time.time() - time_start))
+                print ("\r" + str(math.floor(pos / dataset_count * 100)) + "% " + t + "s", end='')
             
-            for batch_x, _ in loader:
-                
-                if self.device:
-                    batch_x = batch_to(batch_x, self.device)
-                
-                batch_predict = self.module(batch_x)
-                y = torch.cat( (y, batch_predict) )
-        
-        else:
-        
-            if self.device:
-                x = x.to( self.device )
+            del batch_x, batch_y, batch_predict
             
-            if self.transform_x is not None:
-                x = self.transform_x(x)
+            # Clear cache
+            if torch.cuda.is_available():
+                torch.cuda.empty_cache()
             
-            self.module.eval()
-            y = self.module(x)
+            gc.collect()
         
-        return y
+        print ("\nOk")
     
     
     def get_metrics(self, metric_name):
         
         """
         Returns metrics by name
         """
@@ -412,130 +440,25 @@
                     epoch_index > 0 and \
                     not (epoch_index in epoch_indexes):
                     
                     file_path = os.path.join( self.model_path, file_name )
                     os.unlink(file_path)
     
     
-    def summary(self, dataset: TensorDataset):
+    def summary(self, x):
         
         """
         Show model summary
         """
         
-        hooks = []
-        layers = []
-        res = {
-            "layer_name_max": 10,
-            "params_count": 0,
-            "params_train_count": 0,
-            "total_size": 0,
-        }
-        
-        def forward_hook(module, input, output):
-            
-            class_name = module.__class__.__module__ + "." + module.__class__.__name__
-            layer = {
-                "name": module.__class__.__name__,
-                "class_name": module.__class__.__module__ + "." + module.__class__.__name__,
-                "shape": output.shape,
-                "params": 0
-            }
-            
-            if res["layer_name_max"] < len(module.__class__.__name__):
-                res["layer_name_max"] = len(module.__class__.__name__)
-            
-            # Get weight
-            if hasattr(module, "weight"):
-                params, size = tensor_size(module.weight)
-                res["params_count"] += params
-                res["total_size"] += size
-                layer["params"] += params
-                
-                if module.weight.requires_grad:
-                    res["params_train_count"] += params
-            
-            # Get bias
-            if hasattr(module, "bias"):
-                params, size = tensor_size(module.bias)
-                res["params_count"] += params
-                res["total_size"] += size
-                layer["params"] += params
-                
-                if module.bias.requires_grad:
-                    res["params_train_count"] += params
-            
-            # Add output size
-            params, size = tensor_size(output)
-            res["total_size"] += size
-            
-            # Add layer
-            layers.append(layer)
-                
-        def add_hooks(module):
-            hooks.append(module.register_forward_hook(forward_hook))
-        
-        # Get input tensor
-        if self.transform_x is not None:
-            dataset = TransformDataset(
-                dataset,
-                transform_x=self.transform_x
-            )
-        
-        loader = DataLoader(
-            dataset,
-            batch_size=2,
-            drop_last=False,
-            shuffle=False
+        summary(self.module, x,
+            device=self.device,
+            model_name=self.name,
+            transform_x=self.transform_x,
         )
-        it = loader._get_iterator()
-        
-        x, _ = next(it)
-        x = batch_to(x, self.device)
-        
-        # Add input size
-        params, size = tensor_size(x)
-        res["total_size"] += size
-        
-        # Module predict
-        module: torch.nn.Module = self.module
-        module.apply(add_hooks)
-        y = module(x)
-        
-        # Clear cache
-        if torch.cuda.is_available():
-            torch.cuda.empty_cache()
-        
-        # Remove hooks
-        for item in hooks:
-            item.remove()
-        
-        # Print info
-        def format_row(res, args):
-            layer_name_max = res["layer_name_max"] + 5
-            s = "{:<5} {:>"+str(layer_name_max)+"} {:>20} {:>15}"
-            return s.format(*args)
-        
-        res['total_size'] = round(res['total_size'] / 1024 / 1024 * 100) / 100
-        
-        width = 63
-        print( "=" * width )
-        print( format_row(res, ["", "Layer", "Output", "Params"]) )
-        print( "-" * width )
-        
-        for i, layer in enumerate(layers):
-            shape = "(" + ", ".join(map(str,layer["shape"])) + ")"
-            print( format_row(res, [i + 1, layer["name"], shape, layer["params"]]) )
-        
-        print( "-" * width )
-        print( f"Model name: {self.name}" )
-        print( f"Total params: {res['params_count']}" )
-        print( f"Trainable params: {res['params_train_count']}" )
-        print( f"Total size: {res['total_size']} MiB" )
-        print( "=" * width )
     
     
     def draw_history(self, ax, metrics=[], label=None, legend=True, convert=None):
         
         """
         Draw history to axes
         """
@@ -549,14 +472,15 @@
         
         if label:
             ax.set_xlabel( label )
         
         if legend:
             ax.legend()
     
+    
     def show_history(self, metrics=[]):
         
         """
         Show history
         """
         
         import matplotlib.pyplot as plt
@@ -568,8 +492,40 @@
             convert=lambda x: x * 100
         )
         self.draw_history(ax[1],
             ["loss_train", "loss_val"],
             label="Loss"
         )
         plt.show()
-    
+    
+    
+    def show_history_log(self):
+        
+        h = list(self.history.keys())
+        h.sort()
+        
+        for epoch in h:
+            
+            res = self.history[epoch]
+            
+            acc_train = res["acc_train"] if "acc_train" in res else 0
+            acc_val = res["acc_val"] if "acc_val" in res else 0
+            acc_rel = res["acc_rel"] if "acc_rel" in res else 0
+            loss_train = res["loss_train"] if "loss_train" in res else 0
+            loss_val = res["loss_val"] if "loss_val" in res else 0
+            res_lr = res["res_lr"] if "res_lr" in res else 0
+            time = res["time"] if "time" in res else 0
+            
+            acc_train = str(round(acc_train * 10000) / 100)
+            acc_val = str(round(acc_val * 10000) / 100)
+            acc_train = acc_train.ljust(5, "0")
+            acc_val = acc_val.ljust(5, "0")
+            acc_rel_str = str(round(acc_rel * 100) / 100).ljust(4, "0")
+            loss_train = '%.3e' % loss_train
+            loss_val = '%.3e' % loss_val
+            res_lr_str = str(res_lr)
+            
+            print (f"Epoch {epoch}, " +
+                f"acc: {acc_train}%, acc_val: {acc_val}%, rel: {acc_rel_str}, " +
+                f"loss: {loss_train}, loss_val: {loss_val}, lr: {res_lr_str}, " +
+                f"t: {time}s"
+            )
```

### Comparing `tiny_ai_helper-0.1.3/tiny_ai_helper/Trainer.py` & `tiny_ai_helper-0.1.4/tiny_ai_helper/Trainer.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,53 +3,59 @@
 ##
 # Tiny ai helper
 # Copyright (с) Ildar Bikmamatov 2022 - 2023 <support@bayrell.org>
 # License: MIT
 ##
 
 import torch, time
-from .utils import TransformDataset, get_default_device, batch_to
+from .utils import get_default_device, batch_to
 from torch.utils.data import DataLoader, TensorDataset
 
 
 class Trainer:
     
     def __init__(self):
         
         self.device = None
         self.model = None
         self.epoch = 0
-        self.loss_train = 0
-        self.loss_val = 0
+        self.loss_train = 1
+        self.loss_val = 1
         self.acc_train = 0
         self.acc_val = 0
         self.count_train = 0
         self.count_val = 0
         self.batch_iter = 0
         self.time_start = 0
         self.time_end = 0
         self.train_loader = None
         self.val_loader = None
         self.max_best_models = 5
         self.min_epoch = 5
         self.max_epoch = 10
-        self.min_loss_val = 1e-5
+        self.min_loss_val = -1
+        self.min_lr = 1e-5
         self.do_training = False
         
     
     def check_is_trained(self):
         
         """
         Returns True if model is trained
         """
         
         if self.epoch >= self.max_epoch:
             return True
         
-        if self.loss_val < self.min_loss_val and self.epoch >= self.min_epoch:
+        if self.count_val > 0 and \
+            (self.loss_val / self.count_val) < self.min_loss_val and \
+            self.epoch >= self.min_epoch:
+            return True
+        
+        if self.model.optimizer.param_groups[0]["lr"] < self.min_lr:
             return True
         
         return False
     
     
     def on_start_train(self):
         pass
@@ -85,15 +91,15 @@
     
     def on_end_epoch(self):
         
         # Получить текущий lr
         res_lr = []
         for param_group in self.model.optimizer.param_groups:
             res_lr.append(param_group['lr'])
-        res_lr = str(res_lr)
+        res_lr_str = str(res_lr)
         
         # Результат обучения
         loss_train = '%.3e' % (self.loss_train / self.count_train)
         loss_val = '%.3e' % (self.loss_val / self.count_val)
         
         acc_train = self.acc_train / self.count_train
         acc_val = self.acc_val / self.count_val
@@ -104,29 +110,30 @@
         acc_val = acc_val.ljust(5, "0")
         acc_rel_str = str(round(acc_rel * 100) / 100).ljust(4, "0")
         time = str(round(self.time_end - self.time_start))
         
         print ("\r", end='')
         print (f"Epoch {self.epoch}, " +
             f"acc: {acc_train}%, acc_val: {acc_val}%, rel: {acc_rel_str}, " +
-            f"loss: {loss_train}, loss_val: {loss_val}, lr: {res_lr}, " +
+            f"loss: {loss_train}, loss_val: {loss_val}, lr: {res_lr_str}, " +
             f"t: {time}s"
         )
         
         # Update model history
         self.model.epoch = self.epoch
         self.model.history[self.epoch] = {
             "loss_train": self.loss_train / self.count_train,
             "loss_val": self.loss_val / self.count_val,
             "acc_train": self.acc_train / self.count_train,
             "acc_val": self.acc_val / self.count_val,
             "acc_rel": acc_rel,
             "count_train": self.count_train,
             "count_val": self.count_val,
             "batch_iter": self.batch_iter,
+            "res_lr": res_lr,
             "time": time,
         }
         
         # Save model
         self.model.save_epoch()
         self.model.save_the_best_models(epoch_count=self.max_best_models)
     
@@ -135,41 +142,50 @@
         pass
     
     
     def stop_training(self):
         self.do_training = False
     
     
+    def calc_metrics(self, kind, batch_x, batch_y, batch_predict, loss_value):
+        
+        """
+        Calc metrics
+        """
+        
+        get_acc_fn = self.model.acc_fn
+        acc = get_acc_fn(batch_predict, batch_y)
+        loss_value_item = loss_value.item()
+        batch_count = len(batch_x[0]) if isinstance(batch_x, list) else len(batch_x)
+        
+        if kind == "train":
+            self.acc_train = self.acc_train + acc
+            self.loss_train = self.loss_train + loss_value_item
+            self.count_train = self.count_train + batch_count
+            self.batch_iter = self.batch_iter + batch_count
+        
+        elif kind == "valid":
+            self.acc_val = self.acc_val + acc
+            self.loss_val = self.loss_val + loss_value_item
+            self.count_val = self.count_val + batch_count
+            self.batch_iter = self.batch_iter + batch_count
+    
+    
     def fit(self, model, train_dataset, val_dataset, batch_size=64, epochs=10):
         
         """
         Fit model
         """
         
         self.device = model.device
         self.model = model
         self.len_train = len(train_dataset)
         self.len_val = len(val_dataset)
         self.max_epoch = epochs
         
-        # Create new transform dataset
-        if self.model.transform_x is not None or self.model.transform_y is not None:
-            
-            train_dataset = TransformDataset(
-                train_dataset,
-                transform_x=self.model.transform_x,
-                transform_y=self.model.transform_y
-            )
-            
-            val_dataset = TransformDataset(
-                val_dataset,
-                transform_x=self.model.transform_x,
-                transform_y=self.model.transform_y
-            )
-        
         self.train_loader = DataLoader(
             train_dataset,
             batch_size=batch_size,
             drop_last=False,
             shuffle=True
         )
         
@@ -181,24 +197,23 @@
         )
         
         if self.device is None:
             self.device = get_default_device()
             self.model.to(self.device)
         
         module = self.model.module
-        get_acc_fn = self.model.acc_fn
         
         try:
             self.epoch = self.model.epoch
-            self.do_trainin = True
+            self.do_training = True
             
             # Start train
             self.on_start_train()
             
-            while self.do_trainin and not self.check_is_trained():
+            while self.do_training and not self.check_is_trained():
                 
                 self.loss_train = 0
                 self.loss_val = 0
                 self.acc_train = 0
                 self.acc_val = 0
                 self.count_train = 0
                 self.count_val = 0
@@ -208,82 +223,89 @@
                 
                 self.on_start_epoch()
                 module.train()
                 
                 # Обучение
                 for batch_x, batch_y in self.train_loader:
                     
-                    batch_count = len(batch_x[0]) if isinstance(batch_x, list) else len(batch_x)
+                    if self.model.transform_x:
+                        batch_x = self.model.transform_x(batch_x)
+                    
+                    if self.model.transform_y:
+                        batch_y = self.model.transform_y(batch_y)
+                    
                     batch_x = batch_to(batch_x, self.device)
                     batch_y = batch_to(batch_y, self.device)
                     
+                    # Start batch
                     self.on_start_batch_train(batch_x, batch_y)
                     
                     # Predict
-                    model_predict = module(batch_x)
-                    loss_value = self.model.loss(model_predict, batch_y)
-                    loss_value_item = loss_value.item()
-                    acc = get_acc_fn(model_predict, batch_y)
+                    batch_predict = module(batch_x)
+                    loss_value = self.model.loss(batch_predict, batch_y)
                     
-                    del batch_x, batch_y
+                    # Calc metrics
+                    self.calc_metrics("train", batch_x, batch_y, batch_predict, loss_value)
+                    del batch_x, batch_y, batch_predict
                     
                     # Вычислим градиент
                     self.model.optimizer.zero_grad()
                     loss_value.backward()
                     del loss_value
                     
                     # Оптимизируем
                     self.model.optimizer.step()
                     
-                    self.acc_train = self.acc_train + acc
-                    self.loss_train = self.loss_train + loss_value_item
-                    self.count_train = self.count_train + batch_count
-                    self.batch_iter = self.batch_iter + batch_count
-                    
+                    # End batch
                     self.on_end_batch_train()
                   
-                # Clear cache
-                if torch.cuda.is_available():
-                    torch.cuda.empty_cache()
+                    # Clear cache
+                    if torch.cuda.is_available():
+                        torch.cuda.empty_cache()
                 
                 module.eval()
                 
                 # Вычислим ошибку на проверочном датасете
                 for batch_x, batch_y in self.val_loader:
                     
+                    if self.model.transform_x:
+                        batch_x = self.model.transform_x(batch_x)
+                    
+                    if self.model.transform_y:
+                        batch_y = self.model.transform_y(batch_y)
+                    
                     batch_x = batch_to(batch_x, self.device)
                     batch_y = batch_to(batch_y, self.device)
                     
+                    # Start batch
                     self.on_start_batch_val(batch_x, batch_y)
                     
                     # Predict
-                    model_predict = module(batch_x)
-                    loss_value = self.model.loss(model_predict, batch_y)
-                    acc = get_acc_fn(model_predict, batch_y)
-                    
-                    batch_count = len(batch_x[0]) if isinstance(batch_x, list) else len(batch_x)
-                    self.acc_val = self.acc_val + acc
-                    self.loss_val = self.loss_val + loss_value.item()
-                    self.count_val = self.count_val + batch_count
-                    self.batch_iter = self.batch_iter + batch_count
+                    batch_predict = module(batch_x)
+                    loss_value = self.model.loss(batch_predict, batch_y)
+                    
+                    # Calc metrics
+                    self.calc_metrics("valid", batch_x, batch_y, batch_predict, loss_value)
+                    del batch_x, batch_y, batch_predict, loss_value
                     
+                    # End batch
                     self.on_end_batch_val()
                     
                     # Clear cache
-                    del batch_x, batch_y, loss_value
                     if torch.cuda.is_available():
                         torch.cuda.empty_cache()
                     
                 # Двигаем шедулер
                 self.model.scheduler.step(self.loss_val)
                 self.time_end = time.time()
                 
                 self.on_end_epoch()
             
             self.on_end_train()
+            self.do_training = False
             
         except KeyboardInterrupt:
             
             print ("")
             print ("Stopped manually")
             print ("")
```

### Comparing `tiny_ai_helper-0.1.3/tiny_ai_helper/layers.py` & `tiny_ai_helper-0.1.4/tiny_ai_helper/layers.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,25 @@
     """
     
     def __call__(self, t):
         t = t[:,None,:]
         return t
 
 
+class InsertLastAxis(torch.nn.Module):
+    
+    """
+    Insert last Axis for convolution layer
+    """
+    
+    def __call__(self, t):
+        t = t[:,None]
+        return t
+
+
 class MoveRGBToEnd(torch.nn.Module):
         
     def __call__(self, t):
         l = len(t.shape)
         t = torch.moveaxis(t, l-3, l-1)
         return t
 
@@ -56,52 +67,76 @@
         
         t = t.to(torch.float)
         t = t / 255.0
         
         return t
 
 
+class ToFloat(torch.nn.Module):
+    
+    def __call__(self, t):
+        
+        t = t.to(torch.float)
+        
+        return t
+
+
 class ReadImage(torch.nn.Module):
     
     def __init__(self, mode=None):
         
         self.mode=mode
     
-    def __call__(self, t):
+    def __call__(self, batch):
         
-        t = Image.open(t)
+        res = []
+        for t in batch:
         
-        if self.mode is not None and self.mode != t.mode:
-            t = t.convert(self.mode)
+            t = Image.open(t)
+            
+            if self.mode is not None and self.mode != t.mode:
+                t = t.convert(self.mode)
+            
+            res.append(t)
         
-        t = torch.from_numpy( np.array(t) )
+        return res
+
+
+class ImageToTensor(torch.nn.Module):
+    
+    def __call__(self, batch):
         
-        return t
+        res = torch.tensor([])
+        for t in batch:
+            
+            t = torch.from_numpy( np.array(t) )
+            t = t[None, :]
+            res = torch.cat( (res, t) )
+        
+        return res
 
 
 class ResizeImage(torch.nn.Module):
     
     def __init__(self, size, contain=True, color=None):
         
         torch.nn.Module.__init__(self)
         
         self.size = size
         self.contain = contain
         self.color = color
     
-    def __call__(self, t):
+    def __call__(self, batch):
         
-        t = resize_image(t, self.size, contain=self.contain, color=self.color)
+        res = []
+        for t in batch:
+            t = resize_image(t, self.size, contain=self.contain, color=self.color)
+            res.append(t)
         
-        return t
-    
-    def extra_repr(self) -> str:
-        return 'size={}, contain={}, color={}'.format(
-            self.size, self.contain, self.color
-        )
+        return res
 
 
 class NormalizeImage(torch.nn.Module):
     
     def __init__(self, mean, std, inplace=False):
         
         import torchvision
@@ -123,15 +158,15 @@
         return 'mean={}, std={}, inplace={}'.format(
             self.mean, self.std, self.inplace
         )
 
 
 class PreparedModule(torch.nn.Module):
     
-    def __init__(self, module, weight_path, forward=None, *args, **kwargs):
+    def __init__(self, module, weight_path=None, forward=None, *args, **kwargs):
         
         torch.nn.Module.__init__(self)
         
         self.module = module
         self.weight_path = weight_path
         self._forward = forward
         
@@ -149,40 +184,47 @@
             
         return x
     
     def load_weight(self):
         """
         Load weight
         """
-        state_dict = torch.load( self.weight_path )
-        self.module.load_state_dict( state_dict )
+        if self.weight_path:
+            state_dict = torch.load( self.weight_path )
+            self.module.load_state_dict( state_dict )
     
     def state_dict(self, *args, destination=None, prefix='', keep_vars=False):
         pass
     
     
 class Stacking(torch.nn.Module):
     
-    def __init__(self, *args):
+    def __init__(self, *args, is_tensor_list=True):
         torch.nn.Module.__init__(self)
         for i, module in enumerate(args):
             self.add_module(str(i), module)
+        
+        self.is_tensor_list = is_tensor_list
     
     def forward(self, tensor_list):
         
         device = tensor_list[0].device
         res = torch.tensor([]).to(device)
         
         keys = list(self._modules.keys())
         for index, m in enumerate(keys):
+            
+            if self.is_tensor_list:
+                x = tensor_list[index]
+            else:
+                x = tensor_list
+            
             if self._modules[m] is not None:
                 module = self._modules[m]
-                x = module(tensor_list[index])
-            else:
-                x = tensor_list[index]
+                x = module(x)
             
             res = torch.cat( (res, x), dim = 1 )
             
         return res
     
     def state_dict(self, destination=None, prefix='', keep_vars=False):
         keys = self._modules.keys()
@@ -199,8 +241,31 @@
 class Pipe():
     def __init__(self, *args):
         self.pipe = args
     
     def __call__(self, value):
         for fn in self.pipe:
             value = fn(value)
-        return value
+        return value
+
+
+class ModuleRemoveLastClassifier(PreparedModule):
+    
+    def __init__(self, module, weight_path=None, *args, **kwargs):
+        
+        PreparedModule.__init__(self, module, weight_path, *args, **kwargs)
+        
+        # Remove last layer
+        classifier = list(self.module.classifier.children())
+        classifier = classifier[:-1]
+        self.module.classifier = torch.nn.Sequential(*classifier)
+
+
+class ModuleRemoveAllClassifier(PreparedModule):
+    
+    def __init__(self, module, weight_path=None, *args, **kwargs):
+        PreparedModule.__init__(self, module, weight_path, *args, **kwargs)
+    
+    def forward(self, x):
+        x = self.module.features(x)
+        x = self.module.avgpool(x)
+        return x
```

### Comparing `tiny_ai_helper-0.1.3/tiny_ai_helper.egg-info/PKG-INFO` & `tiny_ai_helper-0.1.4/tiny_ai_helper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-ai-helper
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tiny AI Helper for PyTorch
 Home-page: https://github.com/bayrell/ai_helper
 Author: Ildar Bikmamatov
 Author-email: support@bayrell.org
 License: MIT License
 Keywords: ai helper,pytorch
 Platform: UNKNOWN
```

