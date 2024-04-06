# Comparing `tmp/micro_trainer_transformers-0.0.4.tar.gz` & `tmp/micro_trainer_transformers-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micro_trainer_transformers-0.0.4.tar", last modified: Tue Oct 31 11:31:38 2023, max compression
+gzip compressed data, was "micro_trainer_transformers-0.0.5.tar", last modified: Sat Apr  6 18:44:09 2024, max compression
```

## Comparing `micro_trainer_transformers-0.0.4.tar` & `micro_trainer_transformers-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-10-31 11:31:38.737315 micro_trainer_transformers-0.0.4/
--rw-rw-r--   0 joefox    (1000) joefox    (1000)      786 2023-10-31 11:31:38.737315 micro_trainer_transformers-0.0.4/PKG-INFO
--rw-r--r--   0 joefox    (1000) joefox    (1000)      219 2023-05-09 13:47:07.000000 micro_trainer_transformers-0.0.4/README.md
-drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-10-31 11:31:38.737315 micro_trainer_transformers-0.0.4/micro_trainer_transformers/
--rw-r--r--   0 joefox    (1000) joefox    (1000)      197 2023-05-01 21:14:11.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers/__init__.py
--rw-r--r--   0 joefox    (1000) joefox    (1000)    20528 2023-05-03 14:18:14.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers/arguments.py
-drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-10-31 11:31:38.737315 micro_trainer_transformers-0.0.4/micro_trainer_transformers/collators/
--rw-r--r--   0 joefox    (1000) joefox    (1000)       60 2023-06-12 22:17:48.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers/collators/__init__.py
--rw-r--r--   0 joefox    (1000) joefox    (1000)     6214 2023-06-13 13:29:15.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers/collators/albert_collator.py
--rw-r--r--   0 joefox    (1000) joefox    (1000)     8495 2023-10-22 10:02:17.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers/core_args.py
--rw-r--r--   0 joefox    (1000) joefox    (1000)    15501 2023-08-03 19:35:36.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers/core_optim.py
--rw-r--r--   0 joefox    (1000) joefox    (1000)    25984 2023-10-31 11:19:37.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers/core_train.py
--rw-r--r--   0 joefox    (1000) joefox    (1000)     2926 2023-05-01 20:45:05.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers/trainer.py
--rw-r--r--   0 joefox    (1000) joefox    (1000)     2803 2023-10-31 11:03:31.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers/utils.py
-drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2023-10-31 11:31:38.737315 micro_trainer_transformers-0.0.4/micro_trainer_transformers.egg-info/
--rw-r--r--   0 joefox    (1000) joefox    (1000)      786 2023-10-31 11:31:38.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers.egg-info/PKG-INFO
--rw-r--r--   0 joefox    (1000) joefox    (1000)      710 2023-10-31 11:31:38.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 joefox    (1000) joefox    (1000)        1 2023-10-31 11:31:38.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 joefox    (1000) joefox    (1000)       20 2023-10-31 11:31:38.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers.egg-info/entry_points.txt
--rw-r--r--   0 joefox    (1000) joefox    (1000)       40 2023-10-31 11:31:38.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers.egg-info/requires.txt
--rw-r--r--   0 joefox    (1000) joefox    (1000)       27 2023-10-31 11:31:38.000000 micro_trainer_transformers-0.0.4/micro_trainer_transformers.egg-info/top_level.txt
--rw-r--r--   0 joefox    (1000) joefox    (1000)       79 2023-10-31 11:31:38.737315 micro_trainer_transformers-0.0.4/setup.cfg
--rw-r--r--   0 joefox    (1000) joefox    (1000)      992 2023-10-22 06:57:08.000000 micro_trainer_transformers-0.0.4/setup.py
+drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2024-04-06 18:44:09.159584 micro_trainer_transformers-0.0.5/
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     1072 2023-05-12 16:18:59.000000 micro_trainer_transformers-0.0.5/LICENSE
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      786 2024-04-06 18:44:09.159584 micro_trainer_transformers-0.0.5/PKG-INFO
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      219 2023-05-09 13:47:07.000000 micro_trainer_transformers-0.0.5/README.md
+drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2024-04-06 18:44:09.155584 micro_trainer_transformers-0.0.5/micro_trainer_transformers/
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      197 2023-05-01 21:14:11.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers/__init__.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)    20528 2023-05-03 14:18:14.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers/arguments.py
+drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2024-04-06 18:44:09.159584 micro_trainer_transformers-0.0.5/micro_trainer_transformers/collators/
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       60 2023-06-12 22:17:48.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers/collators/__init__.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     6214 2023-06-13 13:29:15.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers/collators/albert_collator.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     8664 2023-11-01 10:53:17.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers/core_args.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)    15760 2024-04-06 18:22:22.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers/core_optim.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)    29136 2024-03-23 08:54:12.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers/core_train.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)    12055 2024-04-06 18:27:46.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers/core_trainer.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     2926 2023-05-01 20:45:05.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers/trainer.py
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)     3592 2023-11-20 14:51:08.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers/utils.py
+drwxrwxr-x   0 joefox    (1000) joefox    (1000)        0 2024-04-06 18:44:09.159584 micro_trainer_transformers-0.0.5/micro_trainer_transformers.egg-info/
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      786 2024-04-06 18:44:09.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers.egg-info/PKG-INFO
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      761 2024-04-06 18:44:09.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers.egg-info/SOURCES.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)        1 2024-04-06 18:44:09.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers.egg-info/dependency_links.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       20 2024-04-06 18:44:09.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers.egg-info/entry_points.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       40 2024-04-06 18:44:09.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers.egg-info/requires.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       27 2024-04-06 18:44:09.000000 micro_trainer_transformers-0.0.5/micro_trainer_transformers.egg-info/top_level.txt
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)       79 2024-04-06 18:44:09.159584 micro_trainer_transformers-0.0.5/setup.cfg
+-rw-rw-r--   0 joefox    (1000) joefox    (1000)      992 2023-11-01 11:41:00.000000 micro_trainer_transformers-0.0.5/setup.py
```

### Comparing `micro_trainer_transformers-0.0.4/PKG-INFO` & `micro_trainer_transformers-0.0.5/micro_trainer_transformers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: micro_trainer_transformers
-Version: 0.0.4
+Name: micro-trainer-transformers
+Version: 0.0.5
 Summary: Micro version train modules Transformers trainer....
 Home-page: https://github.com/utrobinmv/micro_trainer_transformers
 Author: Utrobin Mikhail
 Author-email: utrobinmv@yandex.ru
 License: Apache
 Description: Micro version train modules Transformers trainer....
```

### Comparing `micro_trainer_transformers-0.0.4/micro_trainer_transformers/arguments.py` & `micro_trainer_transformers-0.0.5/micro_trainer_transformers/arguments.py`

 * *Files identical despite different names*

### Comparing `micro_trainer_transformers-0.0.4/micro_trainer_transformers/collators/albert_collator.py` & `micro_trainer_transformers-0.0.5/micro_trainer_transformers/collators/albert_collator.py`

 * *Files identical despite different names*

### Comparing `micro_trainer_transformers-0.0.4/micro_trainer_transformers/core_args.py` & `micro_trainer_transformers-0.0.5/micro_trainer_transformers/core_args.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     learning_rate: float = 0.001
     weight_decay: float = 1e-2
     eps: float = 1e-8
     max_grad_norm: float = 1.0 #Максимальная норма градиента.
 
     #data
     batch_size: int = 2
-    evaluation_strategy: int = 1
+    #evaluation_strategy: int = 1 #Странная строка, вероятно здесь должна быть другая переменная?
     data_train_shuffle: bool = False
     data_streaming_train: bool = False
     data_streaming_train_iter_replace: bool = True #Не завершать эпоху по окончанию итеративного датасета, а перезапускать заново!
     data_streaming_valid: bool = False
     limit_val_batches: int or float or None = None
 
     #loss
@@ -63,14 +63,16 @@
 
     #project    
     project_name: str = 'debug_classificate'
     model_master_name: str = 'linear_simple'
     model_comment: str = ''
     root_path_checkpoint = '/checkpoints'
 
+    #local trainer
+    local_trainer: bool = False
     
     def __init__(self):
         
         self.accum_param()
         self.change_dir()
 
     def accum_param(self):
```

### Comparing `micro_trainer_transformers-0.0.4/micro_trainer_transformers/core_optim.py` & `micro_trainer_transformers-0.0.5/micro_trainer_transformers/core_optim.py`

 * *Files 4% similar despite different names*

```diff
@@ -298,14 +298,16 @@
             optimizer = torch.optim.AdamW(self.model.parameters(), 
                     lr = self.training_params.learning_rate,
                     weight_decay = self.training_params.weight_decay, 
                     eps = self.training_params.eps)
 
         if scheduler is None:
 
+            # В будущем добавить CosineAnnealingWarmRestarts Там скорость обучения периодически взбадривает модель, потом постепенно затухает. И так много раз
+
             name_sheduler = self.training_params.lr_scheduler_type
             if name_sheduler == 'constant':
                 scheduler = get_constant_schedule(optimizer)
             elif name_sheduler == "constant_with_warmup":
                 scheduler = get_constant_schedule_with_warmup(optimizer, num_warmup_steps=num_warmup_steps)
             elif name_sheduler == "inverse_sqrt":
                 scheduler = get_inverse_sqrt_schedule(optimizer, num_warmup_steps=num_warmup_steps)
```

### Comparing `micro_trainer_transformers-0.0.4/micro_trainer_transformers/core_train.py` & `micro_trainer_transformers-0.0.5/micro_trainer_transformers/core_train.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Callable, Dict, NewType, Union, List, Optional, Tuple
 
+import gc
 from tqdm.auto import tqdm
 
 import pandas as pd
 
 import torch
 import torch.nn as nn
 from torch.utils.data import Dataset
@@ -82,69 +83,77 @@
         
         self.model = model
         self.data_collator = data_collator
         self.compute_metrics_fn = compute_metrics
         
         self.loss_fn = self.training_params.loss_fn
         
-        self.pbar_train = tqdm(desc='Total training model',leave=True,position=2) 
+        self.pbar_train = None
+        if self.training_params.local_trainer == False:
+            self.pbar_train = tqdm(desc='Total training model',leave=True,position=2) 
         
         self.train_mode_start = False
         self.save_first_valid_batch = False
         self.first_valid_batch = None
 
         #Аккумулирование шагов лоса, чтобы в конце эпохи получить среднюю метрику
-        self.epoch_train_logs = []
-        self.epoch_valid_logs = []
+        self.epoch_train_logs = {}
+        self.epoch_valid_logs = {}
         self.epoch_valid_list_dict_result = []
 
+        self.validate_labels = []
+        self.validate_predictions = []
+
     def setup(self, stage=None):
         pass
 
     def prepare_data(self):
         pass
 
     def on_fit_start(self):
         #print('on fit start')
         #self.current_training_step = iter(range(self.training_params.max_train_steps))
         #self.pbar_train = iter(tqdm(range(self.training_params.max_train_steps),desc='Training model',leave=True))
         
         self.train_mode_start = True
         
-        self.pbar_train.clear()
-        if self.training_params.max_train_steps is None:
-            self.pbar_train.reset(total=self._trainer.estimated_stepping_batches)
-        else:
-            self.pbar_train.reset(total=self.training_params.max_train_steps)
-            
-        if self.pbar_train_restore_n > 0: #restore from checkpoint
-            self.pbar_train.n = self.pbar_train_restore_n
-            self.pbar_train_restore_n = 0
+        if self.pbar_train is not None:
+            self.pbar_train.clear()
+            if self.training_params.max_train_steps is None or self.training_params.max_train_steps == -1:
+                self.pbar_train.reset(total=self._trainer.estimated_stepping_batches)
+            else:
+                print('max_train_steps:',self.training_params.max_train_steps)
+                self.pbar_train.reset(total=self.training_params.max_train_steps)
+                
+            if self.pbar_train_restore_n > 0: #restore from checkpoint
+                self.pbar_train.n = self.pbar_train_restore_n
+                self.pbar_train_restore_n = 0
         
         pass 
 
     def on_train_start(self):
-        self.validate_labels = []
-        self.validate_predictions = []
-        
+        # self.validate_labels.clear()
+        # self.validate_predictions.clear()
+       
         pass
     
     def train_dataloader(self):
         #print(' === reload train dataloader...')
         if self.training_params.data_streaming_train:
             self.dataset_start_epoch_data_iter = self.dataset_train_size_count
             
             buffer_size = self.training_params.batch_size * self.training_params.val_check_interval * self.training_params.gradient_accumulation_steps
             self.data_buffer_train = []
             for _ in tqdm(range(buffer_size), desc="Reload train dataloader...",leave=False,position=3):
                 #self.pbar_train.display()
                 if self.dataset_train_size_count % (self.training_params.batch_size * self.training_params.gradient_accumulation_steps)  == 0:
-                    #self.pbar_train.refresh()
-                    self.pbar_train.update(n=0)
-                    self.pbar_train.display()
+                    if self.pbar_train is not None:
+                        #self.pbar_train.refresh()
+                        self.pbar_train.update(n=0)
+                        self.pbar_train.display()
                     
                 if buffer_size <= 0:
                     break
                 item = next(self.dataset_train_iter, "end")
                 if item == "end": #Нашли конец датасета
                     self.dataset_train_size = self.dataset_train_size_count
                     #Перезапускаем чтение датасета сначала
@@ -235,47 +244,52 @@
                 _ = next(self.dataset_train_iter)
             self.dataset_train_size_count = self.dataset_start_epoch_data_iter
             
         pass
 
     def on_save_checkpoint(self, checkpoint):
         checkpoint['dataset_start_epoch_data_iter'] = self.dataset_start_epoch_data_iter
-        checkpoint['pbar_train_n'] = self.pbar_train.n
+        if self.pbar_train is not None:
+            checkpoint['pbar_train_n'] = self.pbar_train.n
+        else:
+            checkpoint['pbar_train_n'] = 0
         checkpoint['dataset_train_size'] = self.dataset_train_size
 
         pass
 
         
     def on_train_batch_start(self, batch, batch_idx):
         
         if batch_idx % self.training_params.gradient_accumulation_steps == 0 and self.train_mode_start:
             # if self.pbar_train.total == self.pbar_train.n:
             #     self.pbar_train.total += 1
-            self.pbar_train.update()
-            self.pbar_train.display()
-            
-            t1 = self.pbar_train.start_t
-            t2 = self.pbar_train.last_print_t
-            t = t2 - t1
-            t_prognoz = t / self.pbar_train.n * self.pbar_train.total
-            
-            time_total = time_in_second_hms(t_prognoz)
-            time_str = time_in_second_hms(t_prognoz - t)
-            
-            desc_str = f'Total train model [{time_total}/{time_str}]'
-            
-            #Подсчет эпох в зависимости от датасета
-            if self.dataset_total_batches == 0:
-                if self.dataset_train_size > 0:
-                    self.dataset_total_batches = self.dataset_train_size / (self.training_params.batch_size * self.training_params.gradient_accumulation_steps)
-            else:                        
-                data_epoch = self.global_step / self.dataset_total_batches
-                desc_str += f'. Epoch {data_epoch:.2f}'
+
+            if self.pbar_train is not None:
+                self.pbar_train.update()
+                self.pbar_train.display()
+                
+                t1 = self.pbar_train.start_t
+                t2 = self.pbar_train.last_print_t
+                t = t2 - t1
+                t_prognoz = t / self.pbar_train.n * self.pbar_train.total
                 
-            self.pbar_train.set_description(desc_str)
+                time_total = time_in_second_hms(t_prognoz)
+                time_str = time_in_second_hms(t_prognoz - t)
+                
+                desc_str = f'Total train model [{time_total}/{time_str}]'
+                
+                #Подсчет эпох в зависимости от датасета
+                if self.dataset_total_batches == 0:
+                    if self.dataset_train_size > 0:
+                        self.dataset_total_batches = self.dataset_train_size / (self.training_params.batch_size * self.training_params.gradient_accumulation_steps)
+                else:                        
+                    data_epoch = self.m_trainer.global_step / self.dataset_total_batches
+                    desc_str += f'. Epoch {data_epoch:.2f}'
+                    
+                self.pbar_train.set_description(desc_str)
 
     # def on_train_batch_end(self, outputs, batch, batch_idx):
     #     print(len(outputs),batch_idx)
         
     #     pass        
 
     def _get_lr(self, optimizer):
@@ -290,15 +304,15 @@
 
             preds = self.model(**batch)
             loss = preds.loss
             
             if valid:
                 if self.compute_metrics_fn:
                     self.validate_labels.extend(list(batch['labels'].detach().cpu()))
-                    self.validate_predictions.extend(list(preds.logits.detach().cpu()))
+                    self.validate_predictions.extend(list(preds.logits.argmax(2).detach().cpu()))
             
         else:
             x = batch['image']
             y = batch['label']
 
             pred = self.model(x)
             
@@ -313,19 +327,23 @@
         if isinstance(batch, dict):
             batch_size = len(batch[list(batch.keys())[0]])
         else:
             batch_size = len(batch["labels"])
         
         loss = self.common_step(batch, batch_idx)
         
-        self.log("training_loss", loss, on_step=True, 
+        self.log("training_loss", loss.item(), on_step=True, 
                  on_epoch=True, prog_bar=False, 
                  batch_size=batch_size)
         
-        self.epoch_train_logs.append({'training_loss': loss.detach().cpu().numpy()})
+        if 'training_loss' not in self.epoch_train_logs:
+            self.epoch_train_logs['training_loss'] = 0.0
+            self.epoch_train_logs['training_items'] = 0
+        self.epoch_train_logs['training_loss'] += loss.item()
+        self.epoch_train_logs['training_items'] += 1
 
         return loss
 
     def validation_step(
         self, batch: Tuple[torch.Tensor, List[str]], batch_idx: int,
     ) -> torch.Tensor:
         
@@ -336,53 +354,68 @@
             
         if self.save_first_valid_batch:
            self.first_valid_batch = batch
            self.save_first_valid_batch = False
             
         loss = self.common_step(batch, batch_idx, valid = True)
         
-        self.log("valid_loss", loss, on_step=False, 
+        self.log("valid_loss", loss.item(), on_step=False, 
                  on_epoch=True, prog_bar=True, 
                  batch_size=batch_size)
 
-        self.epoch_valid_logs.append({'valid_loss': loss.detach().cpu().numpy()})
+        if 'valid_loss' not in self.epoch_valid_logs:
+            self.epoch_valid_logs['valid_loss'] = 0.0
+            self.epoch_valid_logs['valid_items'] = 0
+        self.epoch_valid_logs['valid_loss'] += loss.item()
+        self.epoch_valid_logs['valid_items'] += 1
+
 
     def on_train_epoch_start(self):
         self.epoch_train_logs.clear()
 
+        #cache clear
+        gc.collect()
+        torch.cuda.empty_cache()
+
     def on_validation_epoch_start(self):
-        self.validate_labels = []
-        self.validate_predictions = []
+        self.validate_labels.clear()
+        self.validate_predictions.clear()
         self.epoch_valid_logs.clear()
         
+        #cache clear
+        # gc.collect()
+        torch.cuda.empty_cache()
+
         pass
 
     def on_validation_epoch_end(self):
 
         #Соберем логи по тренировке и валидации
         #current_step = self.trainer.num_training_batches
-        current_step: int = self.trainer.global_step
+        current_step: int = self.m_trainer.global_step
         dict_result = {}
         dict_result['step'] = current_step
 
-        if len(self.epoch_train_logs) > 0:
-            df = pd.DataFrame(self.epoch_train_logs)
-            dict_result.update(dict(df.sum() / len(df)))
-        
+        if 'training_loss' in self.epoch_train_logs:
+            self.epoch_train_logs['training_loss'] = self.epoch_train_logs['training_loss'] / self.epoch_train_logs['training_items']
+            self.epoch_train_logs.pop('training_items')
+            dict_result.update(self.epoch_train_logs)
+
         if 'training_loss' not in dict_result.keys():
             dict_result['training_loss'] = 0.0
 
-        if len(self.epoch_valid_logs) > 0:
-            df = pd.DataFrame(self.epoch_valid_logs)
-            dict_result.update(dict(df.sum() / len(df)))
+        if 'valid_loss' in self.epoch_valid_logs:
+            self.epoch_valid_logs['valid_loss'] = self.epoch_valid_logs['valid_loss'] / self.epoch_valid_logs['valid_items']
+            self.epoch_valid_logs.pop('valid_items')
+            dict_result.update(self.epoch_valid_logs)
 
         if self.compute_metrics_fn:            
             
             predictions = self.validate_predictions
-            predictions = [value.argmax(1) for value in predictions]
+            #predictions = [value.argmax(1) for value in predictions]
 
 
             result_dict = self.compute_metrics_fn(
                 (pad_sequence(predictions, batch_first=True, padding_value=-100), 
                  pad_sequence(self.validate_labels, batch_first=True, padding_value=-100))
                 )
             #result_dict = self.compute_metrics_fn((torch.vstack(self.validate_predictions), torch.vstack(self.validate_labels)))
@@ -394,85 +427,95 @@
         if len(dict_result.keys()) > 0:
             self.epoch_valid_list_dict_result.append(dict_result)    
             if in_jupyter_notebook():
                 from IPython.display import display, HTML
                 pd.set_option('display.max_rows', None)
                 df = pd.DataFrame(self.epoch_valid_list_dict_result)
                 display(df)
+                del df
             else:
                 print(self.epoch_valid_list_dict_result[-1])
-        pass
+
+        #cache clear
+        # gc.collect()
+        torch.cuda.empty_cache()
 
 
     def create_trainer(self, mode='train'):
 
         set_seed(self.training_params.seed)
         
         if self.training_params.tf32:
             torch.backends.cuda.matmul.allow_tf32 = True # allow tf32 on matmul
             torch.backends.cudnn.allow_tf32 = True # allow tf32 on cudnn
         
+        use_pl_trainer = not self.training_params.local_trainer
+
         loggers = []
         
         make_dirs(self.training_params.path_log + 'wandb/')
-        
-        loggers.append(pl.loggers.TensorBoardLogger(save_dir = self.training_params.path_log + 'tensorboard',
-                                            name = None,
-                                            version = '',
-                                            ))
-        loggers.append(pl.loggers.CSVLogger(save_dir = self.training_params.path_log + 'csv_log',
-                                            name = None,
-                                            version = '',
-                                            ))
-        
-        if self.training_params.wandb and mode == 'train':
-            
-            wandb_logger = pl.loggers.WandbLogger(name = self.training_params.model_name,
-                                                project = self.training_params.project_name,
-                                                version = self.training_params.version, 
-                                                save_dir=self.training_params.path_log,
-                                                log_model=True)
-            
-            loggers.append(wandb_logger)
-            
-            #log gradients, parameter histogram and model topology (100 steps by default)
-            wandb_logger.watch(self.model, log="all", log_freq=100)
-
-
-        self.checkpoint_callback = pl.callbacks.ModelCheckpoint(monitor=self.training_params.metric_monitor_name, 
-                                                    save_top_k=self.training_params.save_total_limit, 
-                                                    save_last=True, 
-                                                    dirpath = self.training_params.path_checkpoint,
-                                                    filename = '{epoch}_{step}-{'+f'{self.training_params.metric_monitor_name}'+':.6f}',
-                                                    mode=self.training_params.metric_monitor_mode,
-                                                    )
-
-        # plugins: list = []
-        # if self.training_params.fp16:
-        #     plugins.append(pl.plugins.precision.NativeMixedPrecisionPlugin(16,'cuda',GradScaler()))
-
-        callbacks = []
-        callbacks.append(pl.callbacks.LearningRateMonitor(logging_interval='step'))
-        callbacks.append(pl.callbacks.TQDMProgressBar())
-        callbacks.append(pl.callbacks.ModelSummary(max_depth=2))
-        # callbacks.append(pl.callbacks.OnExceptionCheckpoint(dirpath=self.training_params.path_checkpoint,
-        #                                                     filename='exception'))
-        callbacks.append(self.checkpoint_callback)
-        
-        if self.training_params.evaluation_strategy == 'epoch':
-            if self.training_params.early_stopping_patience:
-                callbacks.append(pl.callbacks.EarlyStopping(patience=self.training_params.early_stopping_patience,min_delta=0.001,
-                                                            mode=self.training_params.metric_monitor_mode,
-                                                            monitor=self.training_params.metric_monitor_name,
-                                                            verbose=True))
+            
+        if use_pl_trainer:
+
+            loggers.append(pl.loggers.TensorBoardLogger(save_dir = self.training_params.path_log + 'tensorboard',
+                                                name = None,
+                                                version = '',
+                                                ))
+            loggers.append(pl.loggers.CSVLogger(save_dir = self.training_params.path_log + 'csv_log',
+                                                name = None,
+                                                version = '',
+                                                ))
+            
+            if self.training_params.wandb and mode == 'train':
                 
+                wandb_logger = pl.loggers.WandbLogger(name = self.training_params.model_name,
+                                                    project = self.training_params.project_name,
+                                                    version = self.training_params.version, 
+                                                    save_dir=self.training_params.path_log,
+                                                    log_model=True)
+                
+                loggers.append(wandb_logger)
+                
+                #log gradients, parameter histogram and model topology (100 steps by default)
+                wandb_logger.watch(self.model, log="all", log_freq=100)
+
+
+            self.checkpoint_callback = pl.callbacks.ModelCheckpoint(monitor=self.training_params.metric_monitor_name, 
+                                                        save_top_k=self.training_params.save_total_limit, 
+                                                        save_last=True, 
+                                                        dirpath = self.training_params.path_checkpoint,
+                                                        filename = '{epoch}_{step}-{'+f'{self.training_params.metric_monitor_name}'+':.6f}',
+                                                        mode=self.training_params.metric_monitor_mode,
+                                                        )
+        if use_pl_trainer:
+
+            # plugins: list = []
+            # if self.training_params.fp16:
+            #     plugins.append(pl.plugins.precision.NativeMixedPrecisionPlugin(16,'cuda',GradScaler()))
+
+            callbacks = []
+            callbacks.append(pl.callbacks.LearningRateMonitor(logging_interval='step'))
+            callbacks.append(pl.callbacks.TQDMProgressBar())
+            callbacks.append(pl.callbacks.ModelSummary(max_depth=2))
+            # callbacks.append(pl.callbacks.OnExceptionCheckpoint(dirpath=self.training_params.path_checkpoint,
+            #                                                     filename='exception'))
+            callbacks.append(self.checkpoint_callback)
+            
+            if self.training_params.evaluation_strategy == 'epoch':
+                if self.training_params.early_stopping_patience:
+                    callbacks.append(pl.callbacks.EarlyStopping(patience=self.training_params.early_stopping_patience,min_delta=0.001,
+                                                                mode=self.training_params.metric_monitor_mode,
+                                                                monitor=self.training_params.metric_monitor_name,
+                                                                verbose=True))
                 
-        
         if self.training_params.evaluation_strategy == 'steps':
-            val_check_interval = (self.training_params.val_check_interval)*self.training_params.gradient_accumulation_steps
+            if use_pl_trainer:
+                val_check_interval = (self.training_params.val_check_interval)*self.training_params.gradient_accumulation_steps
+            else:
+                val_check_interval = self.training_params.val_check_interval
             check_val_every_n_epoch=None
         else: #if self.training_params.evaluation_strategy == 'epoch':
             val_check_interval = None
             check_val_every_n_epoch=1
         
         max_train_kwargs = {}
         if self.training_params.max_train_steps is None or self.training_params.max_train_steps == -1:
@@ -482,15 +525,19 @@
                 self.training_params.max_train_epochs = self.training_params.max_train_epochs
                 self.training_params.max_train_steps = int(one_epoch_steps * self.training_params.max_train_epochs)
                 max_train_kwargs: dict[str, float] = {'max_steps': self.training_params.max_train_steps}
             else:
                 max_train_steps = None
                 max_train_kwargs = {'max_epochs': self.training_params.max_train_epochs}
         else:
-            max_train_steps = self.training_params.max_train_steps + (self.training_params.gradient_accumulation_steps * 2)
+            if use_pl_trainer:
+                #Какой то косяк в pytorch lightning Приходится добавлять несколько заключительных шагов
+                max_train_steps = self.training_params.max_train_steps + (self.training_params.gradient_accumulation_steps * 2)
+            else:
+                max_train_steps = self.training_params.max_train_steps
             max_train_kwargs = {'max_steps': max_train_steps}
 
         precision = 32
         if self.training_params.bf16:
             precision = "bf16"
         elif self.training_params.fp16:
             precision = 16
@@ -500,32 +547,47 @@
             torch.backends.cudnn.allow_tf32 = True # allow tf32 on cudnn
 
         if self.training_params.torch_compile:
             print("compiling the model... (takes a ~minute)")
             #unoptimized_model = model
             self.model = torch.compile(self.model) # requires PyTorch 2.0            
 
-        #, max_steps=max_train_steps
-        self.m_trainer = pl.Trainer(accelerator="auto", devices="auto", 
-                **max_train_kwargs,
-                precision=precision,
-                val_check_interval=val_check_interval,
-                accumulate_grad_batches=self.training_params.gradient_accumulation_steps,
-                check_val_every_n_epoch=check_val_every_n_epoch,
-                default_root_dir=self.training_params.path_best_model,
-                logger=loggers,
-                gradient_clip_val=self.training_params.max_grad_norm,
-                callbacks=callbacks,
-                # plugins=plugins,
-                reload_dataloaders_every_n_epochs = 1 if self.training_params.data_streaming_train else 0,
-                limit_val_batches = self.training_params.limit_val_batches,
-                log_every_n_steps = self.training_params.log_every_n_steps,
-                # amp_backend="apex",
-                num_sanity_val_steps=2,
-                )
+                        
+        if use_pl_trainer:
+
+            #, max_steps=max_train_steps
+            self.m_trainer = pl.Trainer(accelerator="auto", devices="auto", 
+                    **max_train_kwargs,
+                    precision=precision,
+                    val_check_interval=val_check_interval,
+                    accumulate_grad_batches=self.training_params.gradient_accumulation_steps,
+                    check_val_every_n_epoch=check_val_every_n_epoch,
+                    default_root_dir=self.training_params.path_best_model,
+                    logger=loggers,
+                    gradient_clip_val=self.training_params.max_grad_norm,
+                    callbacks=callbacks,
+                    # plugins=plugins,
+                    reload_dataloaders_every_n_epochs = 1 if self.training_params.data_streaming_train else 0,
+                    limit_val_batches = self.training_params.limit_val_batches,
+                    log_every_n_steps = self.training_params.log_every_n_steps,
+                    # amp_backend="apex",
+                    num_sanity_val_steps=2,
+                    )
+            
+        else:
+
+            from micro_trainer_transformers.core_trainer import LocalTrainer
+            self.m_trainer = LocalTrainer(**max_train_kwargs,
+                    accumulate_grad_batches=self.training_params.gradient_accumulation_steps,
+                    device='cuda',precision=precision,
+                    gradient_clip_val=self.training_params.max_grad_norm,
+                    val_check_interval=val_check_interval,
+                    path_log=self.training_params.path_log,
+                    path_checkpoints=self.training_params.path_checkpoint)
+
 
     def model_vis_save(self):
         '''
         Сохраняет визуализацию сетки
         '''
         
         self.create_trainer()
@@ -598,18 +660,19 @@
         save_log_filename = self.training_params.path_log + 'find_lr.jpg'        
         fig.savefig(save_log_filename) 
         
         print('Save image plot result to:', save_log_filename)
         
         return lr_recomend
         
-    def fit(self,resume_from_checkpoint=None):
+    def fit(self,resume_from_checkpoint=None, resume_sheduler: bool = True):
         
         self.create_trainer()
 
         save_useful_info(self.training_params.path_log,self.model,self.training_params.__dict__, self.m_trainer.__dict__)
 
-        self.m_trainer.fit(self,ckpt_path=resume_from_checkpoint)
+        self.m_trainer.fit(self,ckpt_path=resume_from_checkpoint, resume_sheduler = resume_sheduler)
         
-        print('Best model path:', self.checkpoint_callback.best_model_path)
-        print(' --- model score:', self.checkpoint_callback.best_model_score)
+        if not self.training_params.local_trainer:
+            print('Best model path:', self.checkpoint_callback.best_model_path)
+            print(' --- model score:', self.checkpoint_callback.best_model_score)
```

### Comparing `micro_trainer_transformers-0.0.4/micro_trainer_transformers/trainer.py` & `micro_trainer_transformers-0.0.5/micro_trainer_transformers/trainer.py`

 * *Files identical despite different names*

### Comparing `micro_trainer_transformers-0.0.4/micro_trainer_transformers/utils.py` & `micro_trainer_transformers-0.0.5/micro_trainer_transformers/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,21 +30,23 @@
     torch.backends.cudnn.benchmark = False
     torch.backends.cudnn.deterministic = True
     torch.manual_seed(seed)
     torch.cuda.manual_seed(seed)
     # torch.cuda.manual_seed_all(seed)
     torch.set_printoptions(precision=precision)
 
-def make_dirs(path):
+def make_dirs(path,silent=False):
     try:
         os.makedirs(path)
     except OSError:
-        print ("Создать директорию %s не удалось" % path)
+        if not silent:
+            print ("Создать директорию %s не удалось" % path)
     else:
-        print ("Успешно создана директория %s " % path)
+        if not silent:        
+            print ("Успешно создана директория %s " % path)
 
 def save_str_to_file(filename:str, str_text: str) -> None:
     '''
     Сохраняет строку в файл
     '''
     my_file = open(filename, "w")
     my_file.write(str_text)
@@ -82,7 +84,24 @@
         json.dump(pl_params, fp, indent=4, cls=CustomEncoder)    
         
     os.system(f"pip freeze > {log_dir}/requirements.txt")
     os.system(f"python -V > {log_dir}/python.txt")
     os.system(f"echo $VIRTUAL_ENV > {log_dir}/virtualenv.txt")
     os.system(f"uname -n > {log_dir}/hostname.txt")
     
+
+def optimizer_to(optim, device):
+    '''
+    convert tesors optimizer to device
+    '''
+    for param in optim.state.values():
+        # Not sure there are any global tensors in the state dict
+        if isinstance(param, torch.Tensor):
+            param.data = param.data.to(device)
+            if param._grad is not None:
+                param._grad.data = param._grad.data.to(device)
+        elif isinstance(param, dict):
+            for subparam in param.values():
+                if isinstance(subparam, torch.Tensor):
+                    subparam.data = subparam.data.to(device)
+                    if subparam._grad is not None:
+                        subparam._grad.data = subparam._grad.data.to(device)
```

### Comparing `micro_trainer_transformers-0.0.4/micro_trainer_transformers.egg-info/PKG-INFO` & `micro_trainer_transformers-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: micro-trainer-transformers
-Version: 0.0.4
+Name: micro_trainer_transformers
+Version: 0.0.5
 Summary: Micro version train modules Transformers trainer....
 Home-page: https://github.com/utrobinmv/micro_trainer_transformers
 Author: Utrobin Mikhail
 Author-email: utrobinmv@yandex.ru
 License: Apache
 Description: Micro version train modules Transformers trainer....
```

### Comparing `micro_trainer_transformers-0.0.4/micro_trainer_transformers.egg-info/SOURCES.txt` & `micro_trainer_transformers-0.0.5/micro_trainer_transformers.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 micro_trainer_transformers/__init__.py
 micro_trainer_transformers/arguments.py
 micro_trainer_transformers/core_args.py
 micro_trainer_transformers/core_optim.py
 micro_trainer_transformers/core_train.py
+micro_trainer_transformers/core_trainer.py
 micro_trainer_transformers/trainer.py
 micro_trainer_transformers/utils.py
 micro_trainer_transformers.egg-info/PKG-INFO
 micro_trainer_transformers.egg-info/SOURCES.txt
 micro_trainer_transformers.egg-info/dependency_links.txt
 micro_trainer_transformers.egg-info/entry_points.txt
 micro_trainer_transformers.egg-info/requires.txt
```

### Comparing `micro_trainer_transformers-0.0.4/setup.py` & `micro_trainer_transformers-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 if os.path.exists("README.md"):
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
 
 setuptools.setup(
     name="micro_trainer_transformers",
-    version="0.0.4",
+    version="0.0.5",
     author="Utrobin Mikhail",
     author_email="utrobinmv@yandex.ru",
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/utrobinmv/micro_trainer_transformers",
     packages=setuptools.find_packages(),
```

