# Comparing `tmp/QuNet-0.0.5-py3-none-any.whl.zip` & `tmp/QuNet-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 29696 bytes, number of entries: 12
+Zip file size: 30408 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-22 07:06 qunet/__init__.py
 -rw-rw-rw-  2.0 fat     6484 b- defN 23-Apr-21 07:06 qunet/data.py
 -rw-rw-rw-  2.0 fat    21896 b- defN 23-Apr-17 09:00 qunet/models.py
 -rw-rw-rw-  2.0 fat    16977 b- defN 23-Apr-20 12:40 qunet/old.py
--rw-rw-rw-  2.0 fat    10424 b- defN 23-Apr-22 09:57 qunet/optim.py
--rw-rw-rw-  2.0 fat     6552 b- defN 23-Apr-22 07:34 qunet/plots.py
--rw-rw-rw-  2.0 fat    24156 b- defN 23-Apr-22 07:26 qunet/trainer.py
--rw-rw-rw-  2.0 fat     1068 b- defN 23-Apr-22 10:02 QuNet-0.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    11416 b- defN 23-Apr-22 10:02 QuNet-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 10:02 QuNet-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 10:02 QuNet-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      879 b- defN 23-Apr-22 10:02 QuNet-0.0.5.dist-info/RECORD
-12 files, 100073 bytes uncompressed, 28262 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat    10435 b- defN 23-Apr-22 11:36 qunet/optim.py
+-rw-rw-rw-  2.0 fat     7129 b- defN 23-Apr-22 13:28 qunet/plots.py
+-rw-rw-rw-  2.0 fat    25104 b- defN 23-Apr-22 13:18 qunet/trainer.py
+-rw-rw-rw-  2.0 fat     1068 b- defN 23-Apr-22 13:30 QuNet-0.0.6.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13028 b- defN 23-Apr-22 13:30 QuNet-0.0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 13:30 QuNet-0.0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 13:30 QuNet-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      879 b- defN 23-Apr-22 13:30 QuNet-0.0.6.dist-info/RECORD
+12 files, 103221 bytes uncompressed, 28974 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: qunet/plots.py
 Comment: 
 
 Filename: qunet/trainer.py
 Comment: 
 
-Filename: QuNet-0.0.5.dist-info/LICENSE
+Filename: QuNet-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: QuNet-0.0.5.dist-info/METADATA
+Filename: QuNet-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: QuNet-0.0.5.dist-info/WHEEL
+Filename: QuNet-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: QuNet-0.0.5.dist-info/top_level.txt
+Filename: QuNet-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: QuNet-0.0.5.dist-info/RECORD
+Filename: QuNet-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qunet/optim.py

```diff
@@ -114,15 +114,15 @@
         
         for i in range(len(schedulers)):             # restore
             schedulers[i] = copy.deepcopy(save[i])            
 
 #-------------------------------------------------------------------------------
 
 
-class ConstScheduler(Scheduler):
+class Scheduler_Const(Scheduler):
     def __init__(self, lr1:float=None, samples:int=1000, enable:bool=True) -> None:
         """ 
         The scheduler sets the learning rate to lr1 and waits for `samples` samples
 
         Args:
             * lr1 - learning rate; if None, then the current rate is taken from the optimizer                        
             * samples - number of training samples to wait with  learning rate lr1
@@ -134,15 +134,15 @@
         self.done += new_samples
         if self.done >= self.samples:               
             self.enable = False
         return self.lr1
 
 #-------------------------------------------------------------------------------
 
-class LineScheduler(Scheduler):
+class Scheduler_Line(Scheduler):
     def __init__(self, lr1:float=None, lr2:float=1e-5, samples:int=1000, enable:bool=True) -> None:
         """ 
         Linear interpolation between lr1 and lr2 per sample samples
         The logarithmic scale will be curved.            
         
         Args:
             * lr1 - initial learning rate; if None, then the current rate is taken from the optimizer            
@@ -159,15 +159,15 @@
             self.enable = False
         else:
             lr = self.lr1 + self.done * (self.lr2-self.lr1) / self.samples
         return lr
 
 #-------------------------------------------------------------------------------
 
-class ExpScheduler(Scheduler):
+class Scheduler_Exp(Scheduler):
     def __init__(self, lr1:float=None, lr2:float=1e-5, samples:int=1000, enable:bool=True) -> None:
         """ 
         Exponential interpolation between lr1 and lr2 per sample samples.
         It will be a straight line on a logarithmic scale.
 
         Args:
             * lr1 - initial learning rate; if None, then the current rate is taken from the optimizer            
@@ -185,15 +185,15 @@
         else:
             beta = self.lr2/self.lr1 if  self.lr1 > 0 and self.lr2 > 0 else 1
             lr = self.lr1 * math.exp(math.log(beta) * self.done/self.samples)
         return lr
 
 #-------------------------------------------------------------------------------
 
-class CosScheduler(Scheduler):
+class Scheduler_Cos(Scheduler):
     def __init__(self, lr1:float=None, lr_hot:float=5e-3,  lr2:float=1e-5, samples:int=1000, warmup:int=100, enable:bool=True) -> None:
         """
         Cosine curve with linear heating.
 
         Args:
             * lr1 - initial learning rate; if None, then the current rate is taken from the optimizer
             * lr_hot - learning rate after warming up after `warmup` samples, starting from start
@@ -228,17 +228,17 @@
         return lr
 
 #===============================================================================
 #                                   Main
 #===============================================================================
 
 if __name__ == '__main__':
-    #scheduler = CosScheduler(lr1=1e-4, lr_hot=1e-2, lr2=1e-3, samples=4000, warmup=1000)                
-    scheduler = ExpScheduler(lr1=1e-2,  lr2=1e-6, samples=4000)                
+    #scheduler = Scheduler_Cos(lr1=1e-4, lr_hot=1e-2, lr2=1e-3, samples=4000, warmup=1000)                
+    scheduler = Scheduler_Exp(lr1=1e-2,  lr2=1e-6, samples=4000)                
     #scheduler.plot(samples=4000, epochs=50, log=True, w=5, h=4, title="ExpScheduler")
     
     lst =[
-        CosScheduler(lr1=1e-4, lr_hot=1e-2, lr2=1e-3, samples=4000, warmup=1000),
-        ConstScheduler(lr1=1e-3, samples=2000),
-        ExpScheduler  (lr1=1e-3, lr2=1e-5, samples=4000)
+        Scheduler_Cos  (lr1=1e-4, lr_hot=1e-2, lr2=1e-3, samples=4000, warmup=1000),
+        Scheduler_Const(lr1=1e-3, samples=2000),
+        Scheduler_Exp  (lr1=1e-3, lr2=1e-5, samples=4000)
     ]
     scheduler.plot_list(lst, samples=10000, epochs=50, log=True, w=5, h=4, title="Cos, Const, Exp Schedulers")
```

## qunet/plots.py

```diff
@@ -37,78 +37,89 @@
     bs_val = f"{val['batch_size'][-1]}" if len(val['batch_size']) else '?'
     tm_trn = f"{c_unit * trn['time'][-1]/(t_unit_scale*trn['samples_epoch'][-1]):.2f}" if len(trn['time']) and trn['samples_epoch'][-1] > 0 else '?'
     tm_val = f"{c_unit * val['time'][-1]/(t_unit_scale*val['samples_epoch'][-1]):.2f}" if len(val['time']) and val['samples_epoch'][-1] > 0 else '?'
 
     plt.suptitle(fr"samples={samples}, steps:{steps}; lr={lr}; batch=(trn:{bs_trn}, val:{bs_val}); time=(trn:{tm_trn}, val:{tm_val}){t_unit}/$10^{c_unit_power:.0f}$; params={hist.get('parms',0)/1e3:.0f}k", fontsize = 10)
 
     if  not view['loss'].get('show', True):
-        subplot_history(111, val, trn, view=view.get('score',{}), x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, kind='score')
+        subplot_history(111, val, trn, view=view.get('score',{}), x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, labels=hist.get('labels',[]), kind='score')
     elif not view['score'].get('show', True):
-        subplot_history(111, val, trn, view=view.get('loss',{}),  x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, kind='loss')
+        subplot_history(111, val, trn, view=view.get('loss',{}),  x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, labels=hist.get('labels',[]), kind='loss')
     else:
-        subplot_history(121, val, trn, view=view.get('score',{}), x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, kind='score')
-        subplot_history(122, val, trn, view=view.get('loss',{}),  x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, kind='loss')            
+        subplot_history(121, val, trn, view=view.get('score',{}), x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, labels=hist.get('labels',[]), kind='score')
+        subplot_history(122, val, trn, view=view.get('loss',{}),  x_min=view.get('x_min',0), x_max=view.get('x_max',None), c_unit=c_unit, c_unit_power=c_unit_power, labels=hist.get('labels',[]), kind='loss')            
     plt.show()
 
     #---------------------------------------------------------------------------    
 
-def subplot_history(sub, val, trn, view, x_min, x_max, c_unit, c_unit_power, kind):                
+def subplot_history(sub, val, trn, view, x_min, x_max, c_unit, c_unit_power, labels, kind):                
+    
     ax1 = plt.subplot(sub); ax1.grid(ls=':')                           
     if len(val['samples']) > 0 and len(trn['samples']) > 0:        
         x_max = max(val['samples'][-1], trn['samples'][-1]) if x_max is None else x_max        
         ax1.set_xlim(x_min/c_unit, x_max/c_unit)
 
     if kind == 'loss':
         best_loss  = f"{val['best_loss'] [-1][-1]:.4f}" if len(val['best_loss'])  else "?"
         loss_val   = f"{val['loss'] [-1]:.4f}"      if len(val['loss'])  else "?"
         loss_trn   = f"{trn['loss'] [-1]:.4f}"      if len(trn['loss'])  else "?"
         plt.title(f"loss = (min: {best_loss}, val: {loss_val}, trn: {loss_trn})")
+
     if kind == 'score':
         best_score = f"{val['best_score'][-1][-1]:.4f}" if len(val['best_score']) else "?"
         score_val  = f"{val['score'][-1]:.4f}"      if len(val['score']) else "?"
         score_trn  = f"{trn['score'][-1]:.4f}"      if len(trn['score']) else "?"
         plt.title(f"score = (bst: {best_score}, val: {score_val},  trn: {score_trn})")
 
+    y_min, y_max = view.get('y_min'), view.get('y_max')
     ax1.set_xlabel(fr"$10^{c_unit_power:.0f}$ samples"); ax1.set_ylabel(kind);                     
-    if view.get('y_min') is not None  and view.get('y_max') is not None:            
-        ax1.set_ylim(view['y_min'], view['y_max'])
+    if y_min is not None  and y_max is not None:            
+        ax1.set_ylim(y_min, y_max)
         if view.get('ticks', False):
-            ax1.set_yticks(np.linspace(view['y_min'], view['y_max'], view['ticks']))  
+            ax1.set_yticks(np.linspace(y_min, y_max, view['ticks']))  
 
     if len(trn['samples']):                      # trn
         ax1.plot(np.array(trn['samples'])/c_unit, trn[kind], 'darkblue', linewidth=0.5)
 
     if len(val['samples']):                      # val
         ax1.plot(np.array(val['samples'])/c_unit, val[kind], 'g', linewidth=1.5)
 
     ax1.legend([kind+'_trn',  kind+'_val'], loc='upper left', frameon = False)
     ax1.tick_params(axis='y', colors='darkgreen')
 
-    if len(trn['best_'+kind]):        
+    if view.get('labels', False):
+        y_min,y_max = ax1.get_ylim()
+        for lb in labels:                 
+            ax1.vlines(lb[1]/c_unit, y_min,y_max, linestyles=':', color='gray')
+            ax1.text  (lb[1]/c_unit, y_min+(y_max-y_min)*0.01,    lb[0])
+
+
+    if view.get('trn_checks', False) and len(trn['best_'+kind]):        
         for c in trn['best_'+kind]:
             if True:
                 ax1.scatter(c[0]/c_unit, c[2], s=3, c='darkblue', edgecolors='black', linewidths=0.5)                                
 
-    if len(val['best_'+kind]):        
+    if view.get('val_checks', False) and  len(val['best_'+kind]):        
         for c in val['best_'+kind]:
             if True:
                 ax1.scatter(c[0]/c_unit, c[2], s=7, c='g', edgecolors='black', linewidths=0.5)                                
 
-    ax2 = ax1.twinx();                                     # lr
-    ax2.set_yscale('log')        
-    if len(trn['samples']):        
-        lr1, lr2 = np.min(trn['lr']), np.max(trn['lr'])
-        if lr1 > 0 and lr2 > 0:
-            lr1, lr2 = math.floor(np.log10(lr1)), math.ceil(np.log10(lr2))
-            if lr1 == lr2:
-                lr1 -= 1; lr2 +=1
-            lr1, lr2 = 10**lr1, 10**lr2
-            ax2.set_ylim(lr1, lr2)
-        ax2.plot(np.array(trn['samples'])/c_unit, trn['lr'], ":", color='darkred')                 
-    ax2.legend(['lr'], loc='upper right', frameon = False)
-    ax2.tick_params(axis='y', colors='darkred')
-    if sub == 121:
-        ax2.set_yticklabels([])   
-        ax2.minorticks_off() # for log scale         
+    if view.get('lr', False):
+        ax2 = ax1.twinx();                                     # lr
+        ax2.set_yscale('log')        
+        if len(trn['samples']):        
+            lr1, lr2 = np.min(trn['lr']), np.max(trn['lr'])
+            if lr1 > 0 and lr2 > 0:
+                lr1, lr2 = math.floor(np.log10(lr1)), math.ceil(np.log10(lr2))
+                if lr1 == lr2:
+                    lr1 -= 1; lr2 +=1
+                lr1, lr2 = 10**lr1, 10**lr2
+                ax2.set_ylim(lr1, lr2)
+            ax2.plot(np.array(trn['samples'])/c_unit, trn['lr'], ":", color='darkred')                 
+        ax2.legend(['lr'], loc='upper right', frameon = False)
+        ax2.tick_params(axis='y', colors='darkred')
+        if sub == 121:
+            ax2.set_yticklabels([])   
+            ax2.minorticks_off() # for log scale         
 
 #---------------------------------------------------------------------------
```

## qunet/trainer.py

```diff
@@ -1,13 +1,13 @@
 ﻿import os, math, copy, time, datetime
 from   tqdm.auto import tqdm
 import numpy as np, matplotlib.pyplot as plt
 import torch, torch.nn as nn
 
-from .optim   import Scheduler, LineScheduler, ExpScheduler, CosScheduler
+from .optim   import Scheduler
 from .plots   import plot_history
 
 class Trainer:
     """
     Generic model training class.
     Any method can, of course, be overridden by inheritance or by an instance.
     """
@@ -26,20 +26,23 @@
 
         self.device     = "cuda" if torch.cuda.is_available() else "cpu"         
         self.dtype      = torch.float32 # see training large models;
         self.optim      = None
         self.schedulers = []             # список шедулеров для управления обучением
         self.scheduler  = Scheduler()    # текущий шедулер
 
-        self.copy_best_model  = False    # копировать лучшую модель
-        self.model_best_score = None     # копия лучшей модели по score        
+        self.copy_best_score_model = False  # to copy the best model by val score
+        self.copy_best_loss_model  = False  # to copy the best model by val loss
+
+        self.best_score_model = None     # copy of the best model by val score
+        self.best_loss_model  = None     # copy of the best model by val loss
          
-        self.folder_loss   = None        # папка для сохранения лучших val loss  моделей
-        self.folder_score  = None        # папка для сохранения лучших val score моделей
-        self.folder_checks = None        # папка для сохранения чекпоинтов        
+        self.folder_loss   = None        # folder to save the best val loss models
+        self.folder_score  = None        # folder to save the best val score models
+        self.folder_checks = None        # folder to save checkpoints        
 
         # -------------------------------- настройки для построения графиков ошибок и метрик
         self.view = {                    
             'w'            : 12,         # plt-plot width
             'h'            :  5,         # plt-plot height
             'count_units'  : 1e6,        # units for number of samples
             'time_units'   : 's',        # time units: ms, s, m, h
@@ -49,25 +52,28 @@
 
             'loss': {                                
                 'show'  : True,          # show loss subplot
                 'y_min' : None,          # fixing the minimum value on the y-axis
                 'y_max' : None,          # fixing the maximum value on the y-axis
                 'ticks' : None,          # how many labels on the y-axis
                 'lr'    : True,          # show learning rate
-                'checks': True,          # show the achievement of the minimum loss (dots)
-                'labels': True,          # show labels (training events)
+                'labels': True,          # show labels (training events)                
+                'trn_checks': True,          # show the achievement of the minimum training loss (dots)
+                'val_checks': True,          # show the achievement of the minimum validation loss (dots)
+
             },
             'score': {                    
                 'show'  : True,          # show score subplot    
                 'y_min' : None,          # fixing the minimum value on the y-axis
                 'y_max' : None,          # fixing the maximum value on the y-axis
                 'ticks' : None,          # how many labels on the y-axis
-                'lr'    : True,          # show learning rate
-                'checks': True,          # show the achievement of the optimum score (dots)
+                'lr'    : True,          # show learning rate                
                 'labels': True,          # show labels (training events)
+                'trn_checks': True,      # show the achievement of the optimum training score (dots)                
+                'val_checks': True,      # show the achievement of the optimum validation score (dots)                
             }
         }
 
         # -------------------------------- история и текущие метрики процесса обучения модели
         self.hist = {                    # история обучения и валидации:
             'samples': 0,                # число примеров в режиме обучения
             'steps'  : 0,                # число шагов градиентного спуска
@@ -94,15 +100,15 @@
         self.hist['params'] = sum(p.numel() for p in model.parameters() if p.requires_grad)        
 
     #---------------------------------------------------------------------------
 
     def add_label(self, text):
         """ Добавить пометку для графиков обучения """
         h = self.hist
-        self.hist( [ text, h['samples'], h['steps'], h['time_trn'], h['time_val'] ] )
+        self.hist['labels'].append( [ text, h['samples'], h['steps'], h['time_trn'], h['time_val'] ] )
 
     #---------------------------------------------------------------------------
 
     def set_optimizer(self, optim):
         """ Установить текущий оптимизатор """
         self.optim = optim
         self.set_optim_schedulers()
@@ -116,15 +122,15 @@
 
     def set_scheduler(self, scheduler):
         self.schedulers = []
         self.add_scheduler(scheduler)
 
     def add_scheduler(self, scheduler):
         scheduler.optim = self.optim
-        self.schedulers.append(scheduler.optim)        
+        self.schedulers.append(scheduler)        
 
     def del_scheduler(self, i):
         self.schedulers.pop(i)
 
     def clear_schedulers(self):
         self.scheduler = Scheduler(self.optim)        
         self.schedulers = []
@@ -134,14 +140,21 @@
             sch.enable = True
             sch.done   = 0
 
     def stop_schedulers(self):
         for sch in self.schedulers:
             sch.enable = False            
 
+    def step_schedulers(self, samples_trn):
+        for sch in self.schedulers:
+            if sch.enable:
+                sch.step(samples_trn)
+                self.scheduler = sch
+                break
+
     #---------------------------------------------------------------------------
 
     def to_device(self, X):
         if type(X) is list or type(X) is tuple:
             for i in range(len(X)):
                 X[i] = X[i].to(self.device)
         else:
@@ -293,30 +306,33 @@
         if scores is not None:
             scores_all = scores_all.cpu()
         return output_all.cpu(),  losses_all.cpu(), scores_all
 
     #---------------------------------------------------------------------------
 
     def run(self,  epochs =None,  samples=None,            
-            pre_val=False, period_val=1, period_plot=100,         
-            period_checks=1, period_val_beg = 4, samples_beg = None ): 
+            pre_val:bool=False, period_val:int=1, period_plot:int=100,         
+            period_checks:int=1, period_val_beg:int = 4, samples_beg:int = None,
+            period_call:int = 0, callback = None): 
         """
         Args:
             * epochs               - number of epochs for training (passes of one data_trn pack). If not defined (None) works "infinitely".
             * samples              - if defined, then will stop after this number of samples, even if epochs has not ended
             * pre_val              - validate before starting training
             * period_val           - period after which validation run (in epochs)
             * period_plot          - period after which the training plot is displayed (in epochs)
+            * period_call          - callback custom function call period
+            * callback             - custom function called with period_info
             * period_checks        - period after which checkpoints are made and the current model is saved (in epochs)
             * period_val_beg = 4   - validation period on the first samples_beg examples
             * samples_beg = None   - the number of samples from the start, after which the validation period will be equal to period_val.
         """
         assert self.optim is not None, "Define the optimizer first"
         self.set_optim_schedulers()        
-
+        self.model.to(self.device)
         if pre_val:
             losses, scores, counts, (samples_val, steps_val, tm_val) = self.fit(0, self.model, self.data_val, train=False)
             loss_val, score_val = self.mean(losses, scores, counts)
             self.add_hist(self.hist['val'], self.data_val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, self.scheduler.get_lr())
             print()
 
         epochs = epochs or 1_000_000
@@ -334,51 +350,57 @@
 
             if self.best_score(self.hist['best']['score_trn'], score_trn):            
                 self.hist['best']['score_trn'] = score_trn[0]
                 self.hist['best']['samples_score_trn'] = self.hist['samples']
                 self.hist['trn']['best_score'].append((self.hist['samples'], self.hist['steps'], score_trn[0].item()))
 
             period = period_val_beg if samples_beg and  self.hist['samples'] < samples_beg else period_val
-            if  epoch % period == 0 or epoch == epochs:
+            if  (period and epoch % period == 0) or epoch == epochs:
                 losses, scores, counts, (samples_val,steps_val,tm_val) = self.fit(epoch, self.model, self.data_val, train=False)
                 loss_val, score_val = self.mean(losses, scores, counts)
                 self.add_hist(self.hist['val'], self.data_val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, lr)
 
                 # save best validation loss:
                 if self.hist['best']['loss_val'] is None or self.hist['best']['loss_val'] > loss_val:
                     self.hist['best']['loss_val'] = loss_val
                     self.hist['best']['samples_loss_val'] = self.hist['samples']
                     self.hist['val']['best_loss'].append((self.hist['samples'], self.hist['steps'], loss_val))
                     if self.folder_loss:
                         self.save(self.model, folder=self.folder_loss, prefix=f"loss_{loss_val:.4f}_{self.now()}")
-
-                # save best validation score[0]
+                    if self.copy_best_loss_model:
+                        self.best_loss_model  = copy.deepcopy(self.model)
+                
                 if self.best_score(self.hist['best']['score_val'], score_val):
                     self.hist['best']['score_val'] = score_val[0]
                     self.hist['best']['samples_score_val'] = self.hist['samples']
                     self.hist['val']['best_score'].append( (self.hist['samples'], self.hist['steps'], score_val[0].item()) )
                     if self.folder_score:
                         self.save(self.model, folder=self.folder_score, prefix=f"score_{score_val[0]:.4f}_{self.now()}")
+                    if self.copy_best_score_model:
+                        self.best_score_model  = copy.deepcopy(self.model)
 
-                    if self.copy_best_model:         # копия лучшей модели по score
-                        self.model_best_score = copy.deepcopy(self.model)
-
-            if epoch % period_plot == 0 or epoch == epochs:
+            if (period_plot and epoch % period_plot == 0) or epoch == epochs:
                 self.run_progress()        
                 plot_history(self.hist, self.view) 
+            
+            if callback and period_call and epoch % period_call == 0:                
+                callback()
 
             if self.folder_checks and (epoch % period_checks == 0 or epoch == epochs):
                 self.save(self.model, folder=self.folder_checks, prefix="check_"+self.now())
 
-            self.scheduler.step(samples_trn)
+            self.step_schedulers(samples_trn)
 
             if samples is not None:
                 samples -= samples_trn
                 if samples <= 0:
-                    self.plot()
+                    self.run_progress()        
+                    plot_history(self.hist, self.view) 
+                    if callback:
+                        callback()
                     break
 
     #---------------------------------------------------------------------------
 
     def run_progress(self):
         print(f"\ntime = (trn:{self.hist['time_trn']/60:.2f}, val:{self.hist['time_val']/60:.2f}, tot:{(self.hist['time_trn']+self.hist['time_val'])/60:.2f})m  lr:{self.scheduler.get_lr():.1e}")
     #---------------------------------------------------------------------------
@@ -406,19 +428,14 @@
             hist['lr']        .append(lr)
             hist['loss']      .append(loss)
             if score is not None and len(score):
                 hist['score'] .append(score[0].item())
 
     #---------------------------------------------------------------------------
 
-    def set_scheduler(self, enable=True, kind='exp', lr0=1e-3 ):
-        pass
-
-    #---------------------------------------------------------------------------
-
     def save(self, fname, model = None, optim=None, info=""):
         model = model or self.model
         cfg = model.cfg
         state = {
             'info':            info,
             'date':            datetime.datetime.now(),   # дата и время
             'config':          cfg,                       # конфигурация модели
```

## Comparing `QuNet-0.0.5.dist-info/LICENSE` & `QuNet-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `QuNet-0.0.5.dist-info/METADATA` & `QuNet-0.0.6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuNet
-Version: 0.0.5
+Version: 0.0.6
 Summary: Working with deep learning models
 Home-page: https://github.com/step137/qunet
 Author: synset
 Author-email: steps137ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -154,24 +154,27 @@
 * `data_val`  - data for validation (instance of Data or DataLoader); may be missing;
 * `score_max` - consider that the metric (the first column of the second tensor returned by the function `metrics` of the model ); should strive to become the maximum (for example, so for accuracy).
 
 Other properties of `Trainer` allow you to customize the appearance of graphs, save models, manage training, and so on.
 They will be discussed in the relevant sections.
 
 ```python
-trainer.run(epochs=None, samples=None,
-            pre_val=False,  period_val=1, period_plot=100, period_checks=1,          
-            period_val_beg = 4, samples_beg = None)
+trainer.run(epochs =None,  samples=None,            
+            pre_val=False, period_val=1, period_plot=100,         
+            period_checks=1, period_val_beg = 4, samples_beg = None,
+            period_call:int = 0, callback = None):     
 ```
 
 * `epochs`         - number of epochs for training (passes of one data_trn pack). If not defined (None) works "infinitely".
 * `samples`        - if defined, then training will stop after this number of samples, even if epochs has not ended
 * `pre_val`        - validate before starting training
 * `period_val`     - period after which validation run (in epochs)
 * `period_plot`    - period after which the training plot is displayed (in epochs)
+* `period_call`    - callback custom function call period
+* `callback`       - custom function called with period_info
 * `period_checks`  - period after which checkpoints are made and the current model is saved (in epochs)
 * `period_val_beg` - validation period on the first `samples_beg` samples. Used when validation needs to be done less frequently at the start of training.
 * `samples_beg`   -  the number of samples from the start, after which the validation period will be equal to `period_val`
 
 <hr>
 
 ## Visualization of the training process
@@ -191,47 +194,49 @@
     'x_max'        : None,       # maximum value in samples on the x-axis (if None - last)
 
     'loss': {                                
         'show'  : True,          # show loss subplot
         'y_min' : None,          # fixing the minimum value on the y-axis
         'y_max' : None,          # fixing the maximum value on the y-axis
         'ticks' : None,          # how many labels on the y-axis
-        'lr'    : True,          # show learning rate
-        'checks': True,          # show the achievement of the minimum loss (dots)
+        'lr'    : True,          # show learning rate        
         'labels': True,          # show labels (training events)
+        'trn_checks': True,      # show the achievement of the minimum training loss (dots)
+        'val_checks': True,      # show the achievement of the minimum validation loss (dots)
     },
 
     'score': {                    
         'show'  : True,          # show score subplot    
         'y_min' : None,          # fixing the minimum value on the y-axis
         'y_max' : None,          # fixing the maximum value on the y-axis
         'ticks' : None,          # how many labels on the y-axis
         'lr'    : True,          # show learning rate
-        'checks': True,          # show the achievement of the optimum score (dots)
         'labels': True,          # show labels (training events)
+        'trn_checks': True,      # show the achievement of the optimum training score (dots)                
+        'val_checks': True,      # show the achievement of the optimum validation score (dots)                
     }
 }
 ```
 
 
 <hr>
 
 ## Using Schedules
 
 Schedulers allow you to control the learning process by changing the learning rate according to the required algorithm.
 There can be one or more schedulers. In the latter case, they are processed sequentially one after another.
 РЎСѓС‰РµСЃС‚РІСѓСЋС‚ СЃР»РµРґСѓСЋС‰РёРµ С€РµРґСѓР»РµСЂС‹:
-* `LineScheduler(lr1, lr2, samples)` - changes the learning rate from `lr1` to `lr2` over `samples` training samples. If `lr1` is not specified, the optimizer's current lr is used for it.
-* `ExpScheduler(lr1, lr2, samples)` - similar, but changing `lr` from `lr1` to `lr2` is exponential.
-* `CosScheduler(lr1, lr_hot,  lr2, samples, warmup)` - changing `lr` by cosine with preliminary linear heating during `warmup` samples from `lr1` to `lr_hot`.
-* `WaitScheduler(lr1, samples)` - wait for `samples` samples with unchanged `lr` (as usual, the last value is taken if `lr1` is not set). This scheduler is useful when using lists of schedulers.
+* `Scheduler_Line(lr1, lr2, samples)` - changes the learning rate from `lr1` to `lr2` over `samples` training samples. If `lr1` is not specified, the optimizer's current lr is used for it.
+* `Scheduler_Exp(lr1, lr2, samples)` - similar, but changing `lr` from `lr1` to `lr2` is exponential.
+* `Scheduler_Cos(lr1, lr_hot,  lr2, samples, warmup)` - changing `lr` by cosine with preliminary linear heating during `warmup` samples from `lr1` to `lr_hot`.
+* `Scheduler_Const(lr1, samples)` - wait for `samples` samples with unchanged `lr` (as usual, the last value is taken if `lr1` is not set). This scheduler is useful when using lists of schedulers.
 
 Each scheduler has a `plot` method that can be used to display the training plot:
 ```python
-sch = CosScheduler(lr1=1e-5, lr_hot=1e-2, lr2=1e-4,  samples=100e3, warmup=1e3)
+sch = Scheduler_Cos(lr1=1e-5, lr_hot=1e-2, lr2=1e-4,  samples=100e3, warmup=1e3)
 sch.plot(log=True)
 ```
 You can also call the `trainer.plot_schedulers()` method of the `Trainer` class.
 It will draw the schedule of the list of schedulers added to the trainer.
 
 Compiling a list of schedulers is done by the following methods of the `Trainer` class:
 * `set_scheduler`( sch ) - set a list of schedulers from one scheduler sch (after clearing the list);
@@ -244,28 +249,46 @@
 * `clear_schedulers`() - clear list of schedulers
 Example:
 
 
 <img src="img/schedulers.png">
 <hr>
 
-## Checkpoints and best model
+## Best Model and Checkpoints
+
+If you set these flags to `True`, then `Trainer` will save the last best model by validation score and loss:
+```python
+trainer.copy_best_score_model = True  # to copy the best model by val score
+trainer.copy_best_loss_model  = True  # to copy the best model by val loss
+```
+These models can be used to roll back if something went wrong (similarly for `trainer.best_loss_model`):
+```python
+train.model = copy.deepcopy(trainer.best_score_model)   
+```
 
+If the following folder is defined (by default `None`), then the best model by validation loss, score will be saved on disk and intermediate versions of the model will be saved with the period `period_checks` (argument of `run` function).
+```python
+trainer.folder_loss   = "models/best_loss"   # folder to save the best val loss models
+trainer.folder_score  = "models/best_score"  # folder to save the best val score models
+trainer.folder_checks = "models/checkpoints" # folder to save checkpoints        
+```
+The best score is the metric of the first column of the second return tensor in the metrics function of the model.
+If `trainer.score_max=True`, then the higher the score, the better (for example, accuracy).
 <hr>
 
-## Batch argumentation
+## Batch Argumentation
 
 <hr>
 
 
-## Working with large models
+## Working with the Large Models
 
 <hr>
 
-## Model state visualization
+## Model State Visualization
 
 <hr>
 
 ## Examples
 
 * Regression_1D - visualization of changes in model parameters
 * Interpolation_F(x)
```

## Comparing `QuNet-0.0.5.dist-info/RECORD` & `QuNet-0.0.6.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 qunet/__init__.py,sha256=IVocm0vQvQK-MkJmbU_qmmZi6dyccdcqjlLG1FUx7TU,123
 qunet/data.py,sha256=mMVzzTlLC7iwhlyyeAdAxCh0qsmjtkD9BMqNK5ptF98,6484
 qunet/models.py,sha256=iWn9WbaR6ZB5T36jtmOinmNO_Y8eGIg16g64tDC5j5w,21896
 qunet/old.py,sha256=wfsu9d4vcptlBT1lgPKHCfqDm8lirDvTTvEEzKGjTig,16977
-qunet/optim.py,sha256=Zuustf3x6hxYj2WCVY6mkJ6DUpeBk1GMjmX6nPU17Y4,10424
-qunet/plots.py,sha256=F1NbkiX_bN0KMkcRg0SsNfTf93dcTWGIdhpky2dCorw,6552
-qunet/trainer.py,sha256=T21bBf-mgGFAgzrAAAnRwUDsD_G_UcvNEOksDyD9MNA,24156
-QuNet-0.0.5.dist-info/LICENSE,sha256=TSOuIu1obl3tk6okEX3AbHzQjUhXvTKU3gY_yDhpZM0,1068
-QuNet-0.0.5.dist-info/METADATA,sha256=PD8QlZnq9AhaJhYCY9RyCGCBnbJ0FW31nGw_rPq133c,11416
-QuNet-0.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-QuNet-0.0.5.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
-QuNet-0.0.5.dist-info/RECORD,,
+qunet/optim.py,sha256=jhoIhpjX9YzEneGc8uUelIdsLidBQgaAmO43Vqz59Xo,10435
+qunet/plots.py,sha256=-z96Yhj5_kYWq296EXTwclNjBT9EgTZJeK4ZDecNCBo,7129
+qunet/trainer.py,sha256=GIVfJh3QmOKufAiPovtjfS8uaWL1OnkIEm6lH6RNGNk,25104
+QuNet-0.0.6.dist-info/LICENSE,sha256=TSOuIu1obl3tk6okEX3AbHzQjUhXvTKU3gY_yDhpZM0,1068
+QuNet-0.0.6.dist-info/METADATA,sha256=lPv9mcxzxrGvctvkM2Gn0hn686WQYf0IEOe_C9bV4_Y,13028
+QuNet-0.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+QuNet-0.0.6.dist-info/top_level.txt,sha256=fZTlCNIA7T6KO6-qMX35d8uK01uhYTGRKO117oubma8,6
+QuNet-0.0.6.dist-info/RECORD,,
```

