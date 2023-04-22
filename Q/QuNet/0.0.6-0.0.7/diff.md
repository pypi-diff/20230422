# Comparing `tmp/QuNet-0.0.6-py3-none-any.whl.zip` & `tmp/QuNet-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 30408 bytes, number of entries: 12
+Zip file size: 30563 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-22 07:06 qunet/__init__.py
 -rw-rw-rw-  2.0 fat     6484 b- defN 23-Apr-21 07:06 qunet/data.py
--rw-rw-rw-  2.0 fat    21896 b- defN 23-Apr-17 09:00 qunet/models.py
+-rw-rw-rw-  2.0 fat    21985 b- defN 23-Apr-22 15:55 qunet/models.py
 -rw-rw-rw-  2.0 fat    16977 b- defN 23-Apr-20 12:40 qunet/old.py
 -rw-rw-rw-  2.0 fat    10435 b- defN 23-Apr-22 11:36 qunet/optim.py
--rw-rw-rw-  2.0 fat     7129 b- defN 23-Apr-22 13:28 qunet/plots.py
--rw-rw-rw-  2.0 fat    25104 b- defN 23-Apr-22 13:18 qunet/trainer.py
--rw-rw-rw-  2.0 fat     1068 b- defN 23-Apr-22 13:30 QuNet-0.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    13028 b- defN 23-Apr-22 13:30 QuNet-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 13:30 QuNet-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 13:30 QuNet-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      879 b- defN 23-Apr-22 13:30 QuNet-0.0.6.dist-info/RECORD
-12 files, 103221 bytes uncompressed, 28974 bytes compressed:  71.9%
+-rw-rw-rw-  2.0 fat     7131 b- defN 23-Apr-22 14:25 qunet/plots.py
+-rw-rw-rw-  2.0 fat    25104 b- defN 23-Apr-22 15:57 qunet/trainer.py
+-rw-rw-rw-  2.0 fat     1068 b- defN 23-Apr-22 15:57 QuNet-0.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13314 b- defN 23-Apr-22 15:57 QuNet-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 15:57 QuNet-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 15:57 QuNet-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      879 b- defN 23-Apr-22 15:57 QuNet-0.0.7.dist-info/RECORD
+12 files, 103598 bytes uncompressed, 29129 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: qunet/plots.py
 Comment: 
 
 Filename: qunet/trainer.py
 Comment: 
 
-Filename: QuNet-0.0.6.dist-info/LICENSE
+Filename: QuNet-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: QuNet-0.0.6.dist-info/METADATA
+Filename: QuNet-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: QuNet-0.0.6.dist-info/WHEEL
+Filename: QuNet-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: QuNet-0.0.6.dist-info/top_level.txt
+Filename: QuNet-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: QuNet-0.0.6.dist-info/RECORD
+Filename: QuNet-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qunet/models.py

```diff
@@ -95,34 +95,35 @@
     """
     Свёрточная сеть: (B, C, H, W) ->  (B, C', H', W')
     """
     def __init__(self, cfg) -> None:
         super().__init__()
         self.cfg = {
             'input'    : (1, 64, 64),   # входной тензор: (channels, height, width)
+            'output'   : None,          # выходной тензор устанавливает create()
             'channel'  : [16,32,64],    # число каналов в каждом слое
             'kernel'   : [3,3,3],       # int or list: размеры конволюционного ядра
             'stride'   : 1,             # int or list: шаг конволюционного ядра
             'padding'  : 1,             # int or list: забивка вокруг картинки
             'pool_ker' : 2,             # int or list: ядро max-пулинга
             'pool_str' : 2,             # int or list: шаг max-пулинга
-            'drop'     : 0,             # int or list: dropout после каждого слоя
-            'output'   : None           # выходной тензор устанавливает create()
+            'drop'     : 0,             # int or list: dropout после каждого слоя            
         }
         if type(cfg) is dict:           # добавляем, меняем свойства
             self.cfg.update(copy.deepcopy(cfg))
         cfg = self.cfg
 
         n = len(cfg['channel'])
         if type(cfg['drop'])     == int: cfg['drop']     = [cfg['drop']]    * n
         if type(cfg['kernel'])   == int: cfg['kernel']   = [cfg['kernel']]  * n
         if type(cfg['stride'])   == int: cfg['stride']   = [cfg['stride']]  * n
         if type(cfg['padding'])  == int: cfg['padding']  = [cfg['padding']] * n
         if type(cfg['pool_ker']) == int: cfg['pool_ker'] = [cfg['pool_ker']]* n
         if type(cfg['pool_str']) == int: cfg['pool_str'] = [cfg['pool_str']]* n
+        if type(cfg['drop'])     == int: cfg['drop']     = [cfg['drop']]* n
         
         self.create()
 
     def forward(self, x):
         x = self.model(x)
         return x
```

## qunet/plots.py

```diff
@@ -15,14 +15,15 @@
     plt.subplot(1,2,1)
     plt.hist(x, bins=bins, log=True, color="lightblue", ec="black");  plt.grid(ls=":",alpha=1); plt.ylabel("log10(N)")
     plt.subplot(1,2,2)
     plt.hist(x_sub, bins=bins_sub, density=True, color="lightblue", ec="black");    plt.grid(ls=":",alpha=1); plt.ylabel("Density")
     plt.show()
 
 #---------------------------------------------------------------------------
+
 def plot_history(hist, view):
     """
     """    
     val, trn, labels = hist.get('val', []), hist.get('trn', []), hist.get('labels, []')
     samples, steps             = hist.get('samples', 0), hist.get('steps', 0)    
 
     t_unit = view.get('time_units','s')
```

## qunet/trainer.py

```diff
@@ -197,15 +197,15 @@
                     loss.backward()   # вычисляем градиенты
                 else:
                     scaler.scale(loss).backward()   # вычисляем градиенты
                 if (b+1) % accumulate == 0:
                     if scaler is None:
                         self.optim.step()
                     else:
-                        scaler.step(self.optimizer) # подправляем параметры
+                        scaler.step(self.optim)     # подправляем параметры
                         scaler.update()             # Updates the scale for next iteration
                     self.optim.zero_grad()          # обнуляем градиенты
                     steps      += 1                 # шагов за эпоху
                     self.hist['steps'] += 1         # шагов за всё время
                 self.hist['samples'] += num         #  примеров за всё время
 
             samples += num                          # просмотренных примеров за эпоху
```

## Comparing `QuNet-0.0.6.dist-info/LICENSE` & `QuNet-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `QuNet-0.0.6.dist-info/METADATA` & `QuNet-0.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuNet
-Version: 0.0.6
+Version: 0.0.7
 Summary: Working with deep learning models
 Home-page: https://github.com/step137/qunet
 Author: synset
 Author-email: steps137ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -287,16 +287,16 @@
 ## Model State Visualization
 
 <hr>
 
 ## Examples
 
 * Regression_1D - visualization of changes in model parameters
-* Interpolation_F(x)
-* MNIST
+* <a href="https://colab.research.google.com/drive/179sHb3WyHNrSJKGLfKrXaAzvShmS1SSf?usp=sharing">Interpolation_F(x)</a> - interpolation of a function of one variable (example of setting up a training plot; working with the list of schedulers; adding a custom graph)
+* MNIST - recognition of handwritten digits 0-9
 * Vanishing gradient
 
 <hr>
 
 ## Versions
 
 * 0.0.4 - fixed version for competition IceCube (kaggle)
```

## Comparing `QuNet-0.0.6.dist-info/RECORD` & `QuNet-0.0.7.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 qunet/__init__.py,sha256=IVocm0vQvQK-MkJmbU_qmmZi6dyccdcqjlLG1FUx7TU,123
 qunet/data.py,sha256=mMVzzTlLC7iwhlyyeAdAxCh0qsmjtkD9BMqNK5ptF98,6484
-qunet/models.py,sha256=iWn9WbaR6ZB5T36jtmOinmNO_Y8eGIg16g64tDC5j5w,21896
+qunet/models.py,sha256=nlUwBeMk0fC4XP_vlNavlJNm1lAt6XiQuWwSFhqb1hM,21985
 qunet/old.py,sha256=wfsu9d4vcptlBT1lgPKHCfqDm8lirDvTTvEEzKGjTig,16977
 qunet/optim.py,sha256=jhoIhpjX9YzEneGc8uUelIdsLidBQgaAmO43Vqz59Xo,10435
-qunet/plots.py,sha256=-z96Yhj5_kYWq296EXTwclNjBT9EgTZJeK4ZDecNCBo,7129
-qunet/trainer.py,sha256=GIVfJh3QmOKufAiPovtjfS8uaWL1OnkIEm6lH6RNGNk,25104
-QuNet-0.0.6.dist-info/LICENSE,sha256=TSOuIu1obl3tk6okEX3AbHzQjUhXvTKU3gY_yDhpZM0,1068
-QuNet-0.0.6.dist-info/METADATA,sha256=lPv9mcxzxrGvctvkM2Gn0hn686WQYf0IEOe_C9bV4_Y,13028
-QuNet-0.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-QuNet-0.0.6.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
-QuNet-0.0.6.dist-info/RECORD,,
+qunet/plots.py,sha256=83OWCZkri0cR_BGvZQVcdcdTtuyGsHR_OC45Oz3DMLM,7131
+qunet/trainer.py,sha256=fBognsGoFxOiKTtW3V_PkMMrx5kWV-c-0EDNH3crKqM,25104
+QuNet-0.0.7.dist-info/LICENSE,sha256=TSOuIu1obl3tk6okEX3AbHzQjUhXvTKU3gY_yDhpZM0,1068
+QuNet-0.0.7.dist-info/METADATA,sha256=IixP18FJIgQfjy3tuzU9GPDk1EaSf_En9DFBOnuBLRU,13314
+QuNet-0.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+QuNet-0.0.7.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
+QuNet-0.0.7.dist-info/RECORD,,
```

