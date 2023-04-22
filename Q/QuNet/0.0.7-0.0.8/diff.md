# Comparing `tmp/QuNet-0.0.7-py3-none-any.whl.zip` & `tmp/QuNet-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 30563 bytes, number of entries: 12
+Zip file size: 30601 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-22 07:06 qunet/__init__.py
 -rw-rw-rw-  2.0 fat     6484 b- defN 23-Apr-21 07:06 qunet/data.py
--rw-rw-rw-  2.0 fat    21985 b- defN 23-Apr-22 15:55 qunet/models.py
+-rw-rw-rw-  2.0 fat    22012 b- defN 23-Apr-22 16:36 qunet/models.py
 -rw-rw-rw-  2.0 fat    16977 b- defN 23-Apr-20 12:40 qunet/old.py
 -rw-rw-rw-  2.0 fat    10435 b- defN 23-Apr-22 11:36 qunet/optim.py
 -rw-rw-rw-  2.0 fat     7131 b- defN 23-Apr-22 14:25 qunet/plots.py
--rw-rw-rw-  2.0 fat    25104 b- defN 23-Apr-22 15:57 qunet/trainer.py
--rw-rw-rw-  2.0 fat     1068 b- defN 23-Apr-22 15:57 QuNet-0.0.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    13314 b- defN 23-Apr-22 15:57 QuNet-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 15:57 QuNet-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 15:57 QuNet-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      879 b- defN 23-Apr-22 15:57 QuNet-0.0.7.dist-info/RECORD
-12 files, 103598 bytes uncompressed, 29129 bytes compressed:  71.9%
+-rw-rw-rw-  2.0 fat    25071 b- defN 23-Apr-22 17:10 qunet/trainer.py
+-rw-rw-rw-  2.0 fat     1068 b- defN 23-Apr-22 17:10 QuNet-0.0.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13314 b- defN 23-Apr-22 17:10 QuNet-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 17:10 QuNet-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 17:10 QuNet-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      879 b- defN 23-Apr-22 17:10 QuNet-0.0.8.dist-info/RECORD
+12 files, 103592 bytes uncompressed, 29167 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: qunet/plots.py
 Comment: 
 
 Filename: qunet/trainer.py
 Comment: 
 
-Filename: QuNet-0.0.7.dist-info/LICENSE
+Filename: QuNet-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: QuNet-0.0.7.dist-info/METADATA
+Filename: QuNet-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: QuNet-0.0.7.dist-info/WHEEL
+Filename: QuNet-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: QuNet-0.0.7.dist-info/top_level.txt
+Filename: QuNet-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: QuNet-0.0.7.dist-info/RECORD
+Filename: QuNet-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qunet/models.py

```diff
@@ -109,21 +109,21 @@
             'drop'     : 0,             # int or list: dropout после каждого слоя            
         }
         if type(cfg) is dict:           # добавляем, меняем свойства
             self.cfg.update(copy.deepcopy(cfg))
         cfg = self.cfg
 
         n = len(cfg['channel'])
-        if type(cfg['drop'])     == int: cfg['drop']     = [cfg['drop']]    * n
-        if type(cfg['kernel'])   == int: cfg['kernel']   = [cfg['kernel']]  * n
-        if type(cfg['stride'])   == int: cfg['stride']   = [cfg['stride']]  * n
-        if type(cfg['padding'])  == int: cfg['padding']  = [cfg['padding']] * n
-        if type(cfg['pool_ker']) == int: cfg['pool_ker'] = [cfg['pool_ker']]* n
-        if type(cfg['pool_str']) == int: cfg['pool_str'] = [cfg['pool_str']]* n
-        if type(cfg['drop'])     == int: cfg['drop']     = [cfg['drop']]* n
+        if type(cfg['drop'])     == int:   cfg['drop']     = [cfg['drop']]    * n
+        if type(cfg['kernel'])   == int:   cfg['kernel']   = [cfg['kernel']]  * n
+        if type(cfg['stride'])   == int:   cfg['stride']   = [cfg['stride']]  * n
+        if type(cfg['padding'])  == int:   cfg['padding']  = [cfg['padding']] * n
+        if type(cfg['pool_ker']) == int:   cfg['pool_ker'] = [cfg['pool_ker']]* n
+        if type(cfg['pool_str']) == int:   cfg['pool_str'] = [cfg['pool_str']]* n
+        if type(cfg['drop'])==float or type(cfg['drop'])==int: cfg['drop']=[cfg['drop']]*n
         
         self.create()
 
     def forward(self, x):
         x = self.model(x)
         return x
```

## qunet/trainer.py

```diff
@@ -170,15 +170,18 @@
             * accumulate - аккумулировать градиент для стольки батчей перед сдвигом оптимизатора;
                            используем, когда большой батч или граф не помещаются в GPU
         https://pytorch.org/blog/what-every-user-should-know-about-mixed-precision-training-in-pytorch/
         """
         self.model.train(train)                     # режим обучение или тестирование
         torch.set_grad_enabled(train)               # строить или нет вычислительный граф
 
-        scaler = torch.cuda.amp.GradScaler() if torch.cuda.is_available() else None
+        scaler = None
+        if torch.cuda.is_available() and self.dtype != torch.float32:
+            scaler = torch.cuda.amp.GradScaler()
+
         if train:
             self.optim.zero_grad()                  # обнуляем градиенты
 
         samples, steps, beg, lst = 0, 0, time.time(), time.time()
         counts_all, losses_all,  scores_all = torch.empty(0,1), None,  None
         for b, (x, y_true) in enumerate(data):
             num = len(x[0]) if type(x) is list or type(x) is tuple else len(x)
@@ -267,49 +270,51 @@
         c_unit_power = round(np.log10(c_unit), 0)
         return t_unit, t_unit_scale,  c_unit, c_unit_power
 
     #---------------------------------------------------------------------------
 
     def predict(self, model, data, verbose:bool = True, whole=False):
         """
-        Вычислить предлсказание, ошибку и метрику для каждого примера в data
-        todo: выдели сразу память
+        Вычислить предсказание, ошибку и метрику для каждого примера в data        
         """
         self.model.train(False)          # режим тестирование
         torch.set_grad_enabled(False)    # вычислительный граф не строим
         data.whole = whole               # обычно по всем примерам (и по дробному батчу)
 
-        samples, steps, beg, lst = 0, 0, time.time(), time.time()
-        counts_all, losses_all, scores_all, output_all = torch.empty((0,1)), None,  None, None
+        samples, beg, lst = 0, time.time(), time.time()
+        scores_all, output_all = None, None
+
+        scaler = None
+        if torch.cuda.is_available() and self.dtype != torch.float32:
+            scaler = torch.cuda.amp.GradScaler()
+        for b, (x, y_true) in enumerate(data):
+            num = len(x[0]) if type(x) is list or type(x) is tuple else len(x)
+            x, y_true = self.to_device(x), self.to_device(y_true)
 
-        scaler = torch.cuda.amp.GradScaler() if torch.cuda.is_available() else None
-        for b, (x,y_true) in enumerate(data):
             if scaler is None:
                 y_pred = model(x)
-                loss, scores = model.metrics(x, y_pred, y_true)
+                _, scores = model.metrics(x, y_pred, y_true)
             else:
                 with torch.autocast(device_type=self.device, dtype=self.dtype):
                     y_pred = model(x)
-                    loss, scores = model.metrics(x, y_pred, y_true)
+                    _, scores = model.metrics(x, y_pred, y_true)
 
-            num = len(x[0]) if type(x) is list or type(x) is tuple else len(x)
-            samples += num                      # число просмотренных примеров за эпоху
-            losses_all = loss.detach() if losses_all is None else torch.vstack([losses_all, loss.detach()])
+            samples += num                      # число просмотренных примеров за эпоху            
             if scores is not None:
-                scores = scores.detach().mean(dim=0)
-                scores_all = scores if scores_all is None else torch.vstack([scores_all, scores])
-            counts_all = torch.vstack([counts_all, torch.Tensor([num])])
+                scores = scores.detach()
+                scores_all = scores if scores_all is None else torch.vstack([scores_all, scores])            
+            output_all = y_pred.detach() if output_all is None else torch.vstack([output_all, y_pred.detach() ])            
 
             if verbose and (time.time()-lst > 1 or b+1 == len(data) ):
                 lst = time.time()
-                self.fit_progress(0, False, (b+1)/len(data), losses_all, scores_all, counts_all, samples, steps, time.time()-beg)
+                print(f"\r[{100*(b+1)/len(data):3.0f}%]", end=" ")                
 
         if scores is not None:
             scores_all = scores_all.cpu()
-        return output_all.cpu(),  losses_all.cpu(), scores_all
+        return output_all.cpu(),  scores_all
 
     #---------------------------------------------------------------------------
 
     def run(self,  epochs =None,  samples=None,            
             pre_val:bool=False, period_val:int=1, period_plot:int=100,         
             period_checks:int=1, period_val_beg:int = 4, samples_beg:int = None,
             period_call:int = 0, callback = None):
```

## Comparing `QuNet-0.0.7.dist-info/LICENSE` & `QuNet-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `QuNet-0.0.7.dist-info/METADATA` & `QuNet-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuNet
-Version: 0.0.7
+Version: 0.0.8
 Summary: Working with deep learning models
 Home-page: https://github.com/step137/qunet
 Author: synset
 Author-email: steps137ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `QuNet-0.0.7.dist-info/RECORD` & `QuNet-0.0.8.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 qunet/__init__.py,sha256=IVocm0vQvQK-MkJmbU_qmmZi6dyccdcqjlLG1FUx7TU,123
 qunet/data.py,sha256=mMVzzTlLC7iwhlyyeAdAxCh0qsmjtkD9BMqNK5ptF98,6484
-qunet/models.py,sha256=nlUwBeMk0fC4XP_vlNavlJNm1lAt6XiQuWwSFhqb1hM,21985
+qunet/models.py,sha256=bcgxYfqWQHhHRQGURTghGhm2c1fjMcgRiI9Sq_uR5D0,22012
 qunet/old.py,sha256=wfsu9d4vcptlBT1lgPKHCfqDm8lirDvTTvEEzKGjTig,16977
 qunet/optim.py,sha256=jhoIhpjX9YzEneGc8uUelIdsLidBQgaAmO43Vqz59Xo,10435
 qunet/plots.py,sha256=83OWCZkri0cR_BGvZQVcdcdTtuyGsHR_OC45Oz3DMLM,7131
-qunet/trainer.py,sha256=fBognsGoFxOiKTtW3V_PkMMrx5kWV-c-0EDNH3crKqM,25104
-QuNet-0.0.7.dist-info/LICENSE,sha256=TSOuIu1obl3tk6okEX3AbHzQjUhXvTKU3gY_yDhpZM0,1068
-QuNet-0.0.7.dist-info/METADATA,sha256=IixP18FJIgQfjy3tuzU9GPDk1EaSf_En9DFBOnuBLRU,13314
-QuNet-0.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-QuNet-0.0.7.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
-QuNet-0.0.7.dist-info/RECORD,,
+qunet/trainer.py,sha256=ytx3hFQ_SpAq0jh6IZD4W5T3VwoSATRU9lfGrfXY5vA,25071
+QuNet-0.0.8.dist-info/LICENSE,sha256=TSOuIu1obl3tk6okEX3AbHzQjUhXvTKU3gY_yDhpZM0,1068
+QuNet-0.0.8.dist-info/METADATA,sha256=VQE-7hjvQ6OrZwQlDGhLadlcS52cX3mnFucHED_0bOc,13314
+QuNet-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+QuNet-0.0.8.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
+QuNet-0.0.8.dist-info/RECORD,,
```

