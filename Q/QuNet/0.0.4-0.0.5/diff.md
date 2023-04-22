# Comparing `tmp/QuNet-0.0.4-py3-none-any.whl.zip` & `tmp/QuNet-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 23928 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat        3 b- defN 23-Apr-17 09:46 qunet/__init__.py
--rw-rw-rw-  2.0 fat     4089 b- defN 23-Apr-19 07:30 qunet/data.py
+Zip file size: 29696 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-22 07:06 qunet/__init__.py
+-rw-rw-rw-  2.0 fat     6484 b- defN 23-Apr-21 07:06 qunet/data.py
 -rw-rw-rw-  2.0 fat    21896 b- defN 23-Apr-17 09:00 qunet/models.py
 -rw-rw-rw-  2.0 fat    16977 b- defN 23-Apr-20 12:40 qunet/old.py
--rw-rw-rw-  2.0 fat     5344 b- defN 23-Apr-17 11:35 qunet/optim.py
--rw-rw-rw-  2.0 fat     7781 b- defN 23-Apr-19 13:39 qunet/plotter.py
--rw-rw-rw-  2.0 fat    21632 b- defN 23-Apr-19 13:40 qunet/trainer.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Apr-20 12:50 QuNet-0.0.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      453 b- defN 23-Apr-20 12:50 QuNet-0.0.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 12:50 QuNet-0.0.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-20 12:50 QuNet-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      876 b- defN 23-Apr-20 12:50 QuNet-0.0.4.dist-info/RECORD
-12 files, 80215 bytes uncompressed, 22490 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat    10424 b- defN 23-Apr-22 09:57 qunet/optim.py
+-rw-rw-rw-  2.0 fat     6552 b- defN 23-Apr-22 07:34 qunet/plots.py
+-rw-rw-rw-  2.0 fat    24156 b- defN 23-Apr-22 07:26 qunet/trainer.py
+-rw-rw-rw-  2.0 fat     1068 b- defN 23-Apr-22 10:02 QuNet-0.0.5.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    11416 b- defN 23-Apr-22 10:02 QuNet-0.0.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-22 10:02 QuNet-0.0.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-22 10:02 QuNet-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      879 b- defN 23-Apr-22 10:02 QuNet-0.0.5.dist-info/RECORD
+12 files, 100073 bytes uncompressed, 28262 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -9,29 +9,29 @@
 
 Filename: qunet/old.py
 Comment: 
 
 Filename: qunet/optim.py
 Comment: 
 
-Filename: qunet/plotter.py
+Filename: qunet/plots.py
 Comment: 
 
 Filename: qunet/trainer.py
 Comment: 
 
-Filename: QuNet-0.0.4.dist-info/LICENSE
+Filename: QuNet-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: QuNet-0.0.4.dist-info/METADATA
+Filename: QuNet-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: QuNet-0.0.4.dist-info/WHEEL
+Filename: QuNet-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: QuNet-0.0.4.dist-info/top_level.txt
+Filename: QuNet-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: QuNet-0.0.4.dist-info/RECORD
+Filename: QuNet-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qunet/__init__.py

```diff
@@ -1 +1,5 @@
-﻿
+﻿from .models  import *
+from .data    import *
+from .trainer import *
+from .optim   import *
+from .plots   import *
```

## qunet/data.py

```diff
@@ -1,49 +1,88 @@
 ﻿import os, gc, math, copy, time, datetime
 import numpy as np, matplotlib.pyplot as plt
 import torch, torch.nn as nn
 from   tqdm.auto import tqdm
 
 class Data:
     """
-    Класс даных. Обычно в задаче переопределяется.
-    Для работы тренера Trainer в итераторе __next__ должен возвращать кортеж
+    Класс даных. Может в задаче переопределяется.
+    Для работы тренера Trainer в итераторе __next__ экземпляр Data должен возвращать кортеж X,Y где 
+        X - тензор или кортеж тензоров для входа модели,
+        Y - тензор или кортеж тензоров для целевых значений модели.
+    Модель - это класс (наследник nn.Module) с методом forward и metrics.
+    Первый даёт тензор или список (кортеж) тензоров на выходе модели
+    Второй вычсляет ошибку (скаляр) и метрики качества (тензор для каждого примера)
+
+    Кортеж батча данных используется в тренере следуюшим образом:
+        for X,Y in data:  # при обучении
+            y = model(X)
+            loss, score = model.metrics(y, Y)
+
+        y = model(X) # в продакшене
+
     необходимых для модели данных (батча), отправленных на нужное устройство device.
-    Ниже пример для задачи Y=f(X). 
-    
-    В простых случаях, можно использовать стандартный DataLoader:
-    from torchvision            import datasets
-    from torchvision.transforms import ToTensor 
-    from torch.utils.data       import DataLoader
-
-    mnist = datasets.MNIST(root='data', train=True,  transform=ToTensor(), download=True)
-    print(mnist.data.shape, mnist.targets.shape, mnist.classes)
-    plt.imshow(255-mnist.data[0], cmap='gray');
 
-    data_trn  = DataLoader(dataset=mnist, batch_size=1024, shuffle=True)
+    Таким образом, dataset это список или кортеж из двух элементов (ввод и цель).
+    Каждый элемент может быть тензором или списком (кортежем) тензоров.    
+        Data(dataset = (X,Y) )               # 2 тензора (ввод и цель)
+        Data(dataset = ( (X1,X2), Y) )       # ввод список тензоров, цель -тензор
+        Data(dataset = ( (X1,X2), (Y1,Y2)) ) # ввод список тензоров, цель -список тензоров
+    Предполагается, что все тензоры в dataset имеют одинаковую длину (по первому индексу).
+
+    С Trainer можно также  использовать стандартный DataLoader:
+        from torchvision            import datasets
+        from torchvision.transforms import ToTensor 
+        from torch.utils.data       import DataLoader
+
+        mnist = datasets.MNIST(root='data', train=True,  transform=ToTensor(), download=True)
+        print(mnist.data.shape, mnist.targets.shape, mnist.classes)
+        plt.imshow(255-mnist.data[0], cmap='gray');
+
+        data_trn  = DataLoader(dataset=mnist, batch_size=1024, shuffle=True)
     """
-    def __init__(self, dataset, shuffle=True, batch_size=64, device='cpu', whole_batch=False, n_packs=1) -> None:
+    def __init__(self, dataset, shuffle=True, batch_size=64,  whole_batch=False, n_packs=1) -> None:
         assert type(dataset) is list or type(dataset) is tuple, f"data = [X, Y, ...] <- list or tuple; got: {type(dataset)}"
-        assert len(dataset),           "empty data"
-        self.data = [d for d in dataset] # мешать будем поочереди (tuple не годится!?)
-        self.shuffle    = shuffle      # перемешивать или нет данные
-        self.device     = device       # на какое устройство отправлять
-        self.batch_size = batch_size   # размер батча
-        self.N     = len(dataset[0])   # число примеров todo: проверь, что одинаковое для всех
+        assert len(dataset) == 2,      "dataset must be (X,Y)"
+        self.X = dataset[0]             
+        self.Y = dataset[1]
+
+        self.shuffle    = shuffle      # перемешивать или нет данные        
+        self.batch_size = batch_size   # размер батча        
         self.start = 0                 # индекс начала текущего батча
         self.n_packs = n_packs         # разбить весть датасет на packs паков
         self.pack_id = 0               # номер текущего пака
         self.whole_batch = whole_batch # брать только батчи размера batch_size
-        print(f"data:{[d.shape for d in self.data]}")
+
+        # число примеров todo: проверь, что одинаковое для всех в списках
+        self.X_list = type(self.X) is list or type(self.X) is tuple
+        self.Y_list = type(self.Y) is list or type(self.Y) is tuple
+
+        self.N = len(self.X[0]) if self.Y_list else len(self.X)
+        assert self.N == len(self.Y[0]) if self.Y_list else len(self.Y), "X, Y must have the same number of examples"        
+
+    #---------------------------------------------------------------------------
 
     def mix(self):
         """ Перемешать данные. С list по памяти эффективнее, чем с tuple."""
         idx = torch.randperm( self.N )
-        for i in range(len(self.data)):
-            self.data[i] = self.data[i][idx]        
+
+        if self.X_list:
+            for i in range(len(self.X)):
+                self.X[i] = self.X[i][idx]        
+        else:
+            self.X = self.X[idx]        
+
+        if self.Y_list:
+            for i in range(len(self.Y)):
+                self.Y[i] = self.Y[i][idx]        
+        else:
+            self.Y = self.Y[idx]        
+
+    #---------------------------------------------------------------------------
 
     def __next__(self):        
         if (self.start >= self.N ) \
            or                      \
            (self.whole_batch and self.start + self.batch_size > self.N ):
                 self.start = self.pack_id = 0                
                 if self.shuffle:
@@ -53,15 +92,27 @@
         n = self.N // self.n_packs
         if self.start > self.pack_id * n + n:
             self.pack_id += 1
             raise StopIteration
 
         s, B = self.start, self.batch_size
         self.start += self.batch_size
-        return tuple([ d[s: s+B].to(self.device) for d in self.data] )                
+
+        if self.X_list:
+            X = [d[s: s+B] for d in self.X]
+        else:
+            X = self.X[s: s+B]
+
+        if self.Y_list:
+            Y = [d[s: s+B] for d in self.Y]
+        else:
+            Y = self.Y[s: s+B]
+
+
+        return (X, Y)                
 
     def __iter__(self):
         return self
 
     def __len__(self):
         nb = self.N  // self.batch_size
         if not self.whole_batch and self.N  % self.batch_size:
```

## qunet/optim.py

```diff
@@ -5,99 +5,208 @@
 
         
 #===============================================================================
 #                                   Shedulers
 #===============================================================================
 
 class Scheduler:
-    def __init__(self, optim=None) -> None:
-        self.optim = optim
-        self.enable = False
-        self.lr = 0
-
-    def set(self, lr1=1e-3, lr2=1e-5, samples=1e3, enable=True):        
-        self.lr1 = lr1 or self.get_lr()
-        self.lr2 = lr2 or self.get_lr()
-        assert self.lr1 > 0 and self.lr2 > 0, "wrong lr limits in Scheduler"
-        assert samples > 1,                   "wrong samples limits in Scheduler"
+    def __init__(self) -> None:
+        self.optim  = None
+        self.enable = False        
+        self.done   = 0
+        self.lr     = 0
+
+    def set(self, lr1=None, lr2=None, samples=1e3, enable=True):        
+        self.lr1 = lr1
+        self.lr2 = lr2    
+        assert samples > 1,  "wrong samples limits in Scheduler"
         self.samples = samples        
         self.enable  = enable
         self.done    = 0
         if enable:
             self.set_lr(self.lr1)
 
     def set_lr(self, lr):
         if self.optim is not None:
             for g in self.optim.param_groups:
                 g['lr'] = lr
         
     def get_lr(self):        
         if self.optim is None:
-            return 0
+            return self.lr
         else:
             return self.optim.param_groups[0]['lr']    # а если не одна группа?
 
     def step(self, samples):
         if self.enable:
+            if self.lr1 is None:
+                self.lr1 = self.get_lr()
+            if self.lr2 is None:
+                self.lr2 = self.get_lr()
+            assert self.lr1 >= 0 and self.lr2 >= 0, "wrong lr limits in Scheduler"                
+
             self.lr = self.new_lr(samples)
             self.set_lr(self.lr)
+        return self.lr
 
-    def plot(self, samples=1000, epochs = 100, w=8, h=5, log=True):    
-        """ Нарисовать кривую обучения для пройденных "samples" за "epochs" эпох """
+    def plot(self, samples=1000, epochs = 100,  log=True, w=8, h=5, title=""):    
+        """ 
+        Draw a learning curve for `samples` passed over `epochs` epochs 
+        Args:
+            * samples - number of examples the optimizer must pass
+            * epochs - number of `epochs` (optimizer steps)
+            * log - logarithmic y-axis scale
+            * w  - chart width
+            * h  - chart height
+            * title - chart title
+        """
         done = self.done
         self.done = 0
         s = int(samples/epochs)
-        lr =   np.array([(self.lr1, 0)] + [ (self.new_lr(s), self.done) for i in range(epochs)] )
+        lr =   np.array([(self.lr1, 0)] + [ (self.step(s), self.done) for i in range(epochs)] )
         plt.figure(figsize=(w,h), facecolor ='w')        
+        plt.title(title)
         plt.plot(lr[:,1], lr[:,0], "-o", markersize=3); 
         if log: plt.yscale('log')        
         plt.xlabel("epoch"); plt.ylabel("lr"); plt.grid(ls=":");         
         plt.show()
         self.done = done
 
 #-------------------------------------------------------------------------------
 
+    def plot_list(self, schedulers, samples=1000, epochs = 100,  log=True, w=8, h=5, title=""):
+        """ 
+        Draw a learning curve for `samples` passed over `epochs` epochs 
+        Args:
+            * schedulers - list of schedulers
+            * samples - number of examples the optimizer must pass
+            * epochs - number of `epochs` (optimizer steps)
+            * log - logarithmic y-axis scale
+            * w  - chart width
+            * h  - chart height
+            * title - chart title
+        """
+        assert len(schedulers) > 0
+        save = [ copy.deepcopy(sch) for sch in schedulers ]
+        for sch in schedulers:
+            sch.done = 0
+            sch.enable = True
+        s = int(samples/epochs)
+
+        sch = schedulers[0]
+        hist, sch_id, tot =  [ (sch.lr1, 0) ], 0, 0
+        for epoch in range(epochs):            
+            lr = sch.step(s)            
+            tot += s
+            hist += [ (lr, tot) ]
+            if not sch.enable:
+                sch_id += 1
+                if sch_id >= len(schedulers):
+                    break
+                sch = schedulers[sch_id]
+
+        hist = np.array(hist)
+        plt.figure(figsize=(w,h), facecolor ='w')        
+        plt.title(title)
+        plt.plot(hist[:,1], hist[:,0], "-o", markersize=3); 
+        if log: plt.yscale('log')        
+        plt.xlabel("epoch"); plt.ylabel("lr"); plt.grid(ls=":");         
+        plt.show()
+        
+        for i in range(len(schedulers)):             # restore
+            schedulers[i] = copy.deepcopy(save[i])            
+
+#-------------------------------------------------------------------------------
+
+
+class ConstScheduler(Scheduler):
+    def __init__(self, lr1:float=None, samples:int=1000, enable:bool=True) -> None:
+        """ 
+        The scheduler sets the learning rate to lr1 and waits for `samples` samples
+
+        Args:
+            * lr1 - learning rate; if None, then the current rate is taken from the optimizer                        
+            * samples - number of training samples to wait with  learning rate lr1
+        """
+        super().__init__()
+        self.set(lr1=lr1,  samples=samples, enable=enable)
+
+    def new_lr(self, new_samples):            
+        self.done += new_samples
+        if self.done >= self.samples:               
+            self.enable = False
+        return self.lr1
+
+#-------------------------------------------------------------------------------
+
 class LineScheduler(Scheduler):
-    """ 
-    Линейная интерполяция между lr1 и lr2 за samples примеров
-    В логарифической шкале будет изогнута.
-    """
+    def __init__(self, lr1:float=None, lr2:float=1e-5, samples:int=1000, enable:bool=True) -> None:
+        """ 
+        Linear interpolation between lr1 and lr2 per sample samples
+        The logarithmic scale will be curved.            
+        
+        Args:
+            * lr1 - initial learning rate; if None, then the current rate is taken from the optimizer            
+            * lr2 - final learning rate after `samples` samples, starting from start
+            * samples - number of training samples to change the learning rate from lr1 to lr2            
+        """
+        super().__init__()
+        self.set(lr1=lr1, lr2=lr2, samples=samples, enable=enable)
+
     def new_lr(self, new_samples):            
         self.done += new_samples
         if self.done >= self.samples:   
             lr = self.lr2
             self.enable = False
         else:
             lr = self.lr1 + self.done * (self.lr2-self.lr1) / self.samples
         return lr
 
 #-------------------------------------------------------------------------------
 
 class ExpScheduler(Scheduler):
-    """ 
-    Экспоненциальная интерполяция между lr1 и lr2 за samples примеров.
-    В логарифической шкале будет прямая.
-    """
+    def __init__(self, lr1:float=None, lr2:float=1e-5, samples:int=1000, enable:bool=True) -> None:
+        """ 
+        Exponential interpolation between lr1 and lr2 per sample samples.
+        It will be a straight line on a logarithmic scale.
+
+        Args:
+            * lr1 - initial learning rate; if None, then the current rate is taken from the optimizer            
+            * lr2 - final learning rate after `samples` samples, starting from start
+            * samples - number of training samples to change the learning rate from lr1 to lr2            
+        """
+        super().__init__()
+        self.set(lr1=lr1, lr2=lr2, samples=samples, enable=enable)
+
     def new_lr(self, new_samples):            
         self.done += new_samples
         if self.done >= self.samples:   
             lr = self.lr2
             self.enable = False
         else:
             beta = self.lr2/self.lr1 if  self.lr1 > 0 and self.lr2 > 0 else 1
             lr = self.lr1 * math.exp(math.log(beta) * self.done/self.samples)
         return lr
 
 #-------------------------------------------------------------------------------
 
 class CosScheduler(Scheduler):
-    """
-    Косинусная кривая с разогревом.
-    src: https://d2l.ai/chapter_optimization/lr-scheduler.html 
-    """
+    def __init__(self, lr1:float=None, lr_hot:float=5e-3,  lr2:float=1e-5, samples:int=1000, warmup:int=100, enable:bool=True) -> None:
+        """
+        Cosine curve with linear heating.
+
+        Args:
+            * lr1 - initial learning rate; if None, then the current rate is taken from the optimizer
+            * lr_hot - learning rate after warming up after `warmup` samples, starting from start
+            * lr2 - final learning rate after `samples` samples, starting from start
+            * samples - number of training samples to change the learning rate from lr1 to lr2
+            * warmup - number of training samples to warm up from lr1 to lr_hot
+        """
+        super().__init__()
+        self.set(lr1=lr1, lr2=lr2, samples=samples, lr_hot=lr_hot, warmup=warmup, enable=enable)
 
     def set(self, lr1=1e-5, lr2=1e-5, samples=1e3, lr_hot=5e-3, warmup=1e1, enable=True):        
         super().set(lr1=lr1, lr2=lr2, samples=samples, enable=enable)
         self.lr_hot = lr_hot or self.get_lr()        
         assert self.lr_hot > 0,  "wrong lr limits in Scheduler"
         assert warmup >= 0,      "wrong samples limits in Scheduler"
         assert samples > warmup, "should be fewer warm-up samples (warm) than the total number of samples"
@@ -119,12 +228,17 @@
         return lr
 
 #===============================================================================
 #                                   Main
 #===============================================================================
 
 if __name__ == '__main__':
-
-    scheduler = CosScheduler()        
-    scheduler.set(lr1=1e-6, lr2=1e-5, samples=40000, lr_hot=1e-3, warmup=1000)
-    scheduler.plot(samples=40000, log=False)
-   
+    #scheduler = CosScheduler(lr1=1e-4, lr_hot=1e-2, lr2=1e-3, samples=4000, warmup=1000)                
+    scheduler = ExpScheduler(lr1=1e-2,  lr2=1e-6, samples=4000)                
+    #scheduler.plot(samples=4000, epochs=50, log=True, w=5, h=4, title="ExpScheduler")
+    
+    lst =[
+        CosScheduler(lr1=1e-4, lr_hot=1e-2, lr2=1e-3, samples=4000, warmup=1000),
+        ConstScheduler(lr1=1e-3, samples=2000),
+        ExpScheduler  (lr1=1e-3, lr2=1e-5, samples=4000)
+    ]
+    scheduler.plot_list(lst, samples=10000, epochs=50, log=True, w=5, h=4, title="Cos, Const, Exp Schedulers")
```

## qunet/trainer.py

```diff
@@ -1,325 +1,408 @@
-﻿"""
-Предполагается следующая абстракция:
-Модель получает ненулевой кортеж  небходимых данных data=(X,Y,...):
-В forward она возвращает кортеж  (float, тензор, тензор):
-    Model.forward(data):    
-        return output, loss, score
-где
-    loss   : float = ошибка по батчу с графом для обратного распространения (скаляр!)
-    output : (B,*) результат работы модели (без графа), B - число примеров в батче
-    score  : None or (B,1) or (B,n) - метрики качества работы (без графа)
-Если метрик score нет, то  модель для них должна вернуть None. Если метрика одна - тензор (B,1).
-Если нужны ошибки по каждому примеру, помещаем их в score, но loss всё равно оставляем скалярным.
-
-Внимание: 
-    Если выход модели один, после слоя Linear тензор имеет форму (B,1) 
-    Поэтому таргетные данные также должны иметь форму (B,1), иначе получим неверный loss.
-    X, = torch.arange(5).view(-1,1).to(torch.float32),  torch.arange(5).to(torch.float32)
-    loss = (X-Y).pow(2).mean()  # 4 так как (B,1) - (B,) = (B,1) - (1,B) = (B,B)
-"""
-import os, math, copy, time, datetime
+﻿import os, math, copy, time, datetime
 from   tqdm.auto import tqdm
 import numpy as np, matplotlib.pyplot as plt
 import torch, torch.nn as nn
 
-from .optim   import LineScheduler, ExpScheduler, CosScheduler
-from .plotter import Plotter
+from .optim   import Scheduler, LineScheduler, ExpScheduler, CosScheduler
+from .plots   import plot_history
 
 class Trainer:
     """
-    Универсальный класс обучения модели.
-    Любой метод можно, естественно, переопределить наследованием или у экземпляра.
+    Generic model training class.
+    Any method can, of course, be overridden by inheritance or by an instance.
     """
     def __init__(self, model, data_trn, data_val, score_max=False) -> None:
-        self.model = model
-        
-        self.optim = None
-        self.scheduler = ExpScheduler()
-        self.data_trn = data_trn
-        self.data_val = data_val
-
-        self.score_max = score_max      # метрика должна быть максимальной (например accuracy)
-
-        self.best_loss_val  = None      # лучшее значение валидационной ошибки
-        self.best_loss_trn  = None      # лучшее значение тренировочная ошибки
-        self.best_score_val = None      # лучшее значение валидационной метрики (первой)
-        self.best_score_trn = None      # лучшее значение тенировочной метрики (первой)
-        self.samples_best_loss_val = 0  # когда была лучшая валидационная ошибка
-        self.samples_best_loss_trn = 0  # когда была лучшая тренировочная ошибка
-        self.samples_best_score_val= 0  # когда была лучшая валиадционная метрика        
-        self.samples_best_score_trn= 0  # когда была лучшая тренировочная метрика
-
-        self.samples  = 0               # число примеров в режиме обучения
-        self.steps    = 0               # число шагов градиентного спуска
-
-        # история обучения и валидации
-        self.hist_trn = {'samples':[], 'steps':[], 'batch_size':[], 'lr':[], 'samples_epoch':[], 'steps_epoch':[], 'time':[], 'loss':[], 'score':[], 'best_loss':[], 'best_score':[] }
-        self.hist_val = {'samples':[], 'steps':[], 'batch_size':[], 'lr':[], 'samples_epoch':[], 'steps_epoch':[], 'time':[], 'loss':[], 'score':[], 'best_loss':[], 'best_score':[] }
-        self.labels   = []
-
-        self.time_trn = 0               # общее время тренировки
-        self.time_val = 0               # общее время валидациии
-
-        self.model_best_score = None    # копия лучшей модели по score
-        self.copy_best_model  = False   # копировать лучшую модель
-        
-        self.plotter = Plotter()        # класс рисования графиков
-
-        self.cfg = {
-            'folder_loss'  : None,      # папка для сохранения лучших val loss  моделей
-            'folder_score' : None,      # папка для сохранения лучших val score моделей
-            'folder_checks': None,      # папка для сохранения чекпоинтов
-            'samples_unit_power':  6,   # единицы измерения числа примеров 10^samples_unit_power
-            'x_min':         0,         # дипазон графика в samples по x (если < 0 последние x_min sampes)
-            'x_max':         None,
-            'plot_loss': {
-                'show':  True,
-                'y_min': None, 'y_max': None, 
-                'ticks': None,
+        """
+        Args:
+            * model     - model for traininig;
+            * data_trn  - training data (Data or DataLoader instance);
+            * data_val  - data for validation (instance of Data or DataLoader); may be missing;
+            * score_max - consider that the metric (the first column of the second tensor returned by the function `metrics` of the model ); should strive to become the maximum (for example, so for accuracy).            
+        """
+        self.model      = model
+        self.data_trn   = data_trn
+        self.data_val   = data_val
+        self.score_max = score_max       # метрика должна быть максимальной (например accuracy)
+
+        self.device     = "cuda" if torch.cuda.is_available() else "cpu"         
+        self.dtype      = torch.float32 # see training large models;
+        self.optim      = None
+        self.schedulers = []             # список шедулеров для управления обучением
+        self.scheduler  = Scheduler()    # текущий шедулер
+
+        self.copy_best_model  = False    # копировать лучшую модель
+        self.model_best_score = None     # копия лучшей модели по score        
+         
+        self.folder_loss   = None        # папка для сохранения лучших val loss  моделей
+        self.folder_score  = None        # папка для сохранения лучших val score моделей
+        self.folder_checks = None        # папка для сохранения чекпоинтов        
+
+        # -------------------------------- настройки для построения графиков ошибок и метрик
+        self.view = {                    
+            'w'            : 12,         # plt-plot width
+            'h'            :  5,         # plt-plot height
+            'count_units'  : 1e6,        # units for number of samples
+            'time_units'   : 's',        # time units: ms, s, m, h
+
+            'x_min'        : 0,          # minimum value in samples on the x-axis (if < 0 last x_min samples)
+            'x_max'        : None,       # maximum value in samples on the x-axis (if None - last)
+
+            'loss': {                                
+                'show'  : True,          # show loss subplot
+                'y_min' : None,          # fixing the minimum value on the y-axis
+                'y_max' : None,          # fixing the maximum value on the y-axis
+                'ticks' : None,          # how many labels on the y-axis
+                'lr'    : True,          # show learning rate
+                'checks': True,          # show the achievement of the minimum loss (dots)
+                'labels': True,          # show labels (training events)
             },
-            'plot_score': {
-                'show':  True,
-                'y_min': None, 'y_max': None, 
-                'ticks': None,
+            'score': {                    
+                'show'  : True,          # show score subplot    
+                'y_min' : None,          # fixing the minimum value on the y-axis
+                'y_max' : None,          # fixing the maximum value on the y-axis
+                'ticks' : None,          # how many labels on the y-axis
+                'lr'    : True,          # show learning rate
+                'checks': True,          # show the achievement of the optimum score (dots)
+                'labels': True,          # show labels (training events)
             }
         }
-        
+
+        # -------------------------------- история и текущие метрики процесса обучения модели
+        self.hist = {                    # история обучения и валидации:
+            'samples': 0,                # число примеров в режиме обучения
+            'steps'  : 0,                # число шагов градиентного спуска
+
+            'time_trn': 0,               # общее время тренировки
+            'time_val': 0,               # общее время валидациии
+
+            'best':  {
+                'loss_val': None,        # лучшее значение валидационной ошибки
+                'loss_trn': None,        # лучшее значение тренировочная ошибки
+                'score_val': None,       # лучшее значение валидационной метрики (первой)
+                'score_trn': None,       # лучшее значение тенировочной метрики (первой)
+
+                'samples_loss_val': 0,   # когда была лучшая валидационная ошибка
+                'samples_loss_trn': 0,   # когда была лучшая тренировочная ошибка
+                'samples_score_val': 0,  # когда была лучшая валиадционная метрика
+                'samples_score_trn': 0,  # когда была лучшая тренировочная метрика
+            },
+
+            'trn'    : {'samples':[], 'steps':[], 'batch_size':[], 'lr':[], 'samples_epoch':[], 'steps_epoch':[], 'time':[], 'loss':[], 'score':[], 'best_loss':[], 'best_score':[] },
+            'val'    : {'samples':[], 'steps':[], 'batch_size':[], 'lr':[], 'samples_epoch':[], 'steps_epoch':[], 'time':[], 'loss':[], 'score':[], 'best_loss':[], 'best_score':[] },
+            'labels' : []
+        }    
+        self.hist['params'] = sum(p.numel() for p in model.parameters() if p.requires_grad)        
+
+    #---------------------------------------------------------------------------
+
+    def add_label(self, text):
+        """ Добавить пометку для графиков обучения """
+        h = self.hist
+        self.hist( [ text, h['samples'], h['steps'], h['time_trn'], h['time_val'] ] )
+
     #---------------------------------------------------------------------------
 
     def set_optimizer(self, optim):
         """ Установить текущий оптимизатор """
         self.optim = optim
-        self.scheduler.optim = optim
+        self.set_optim_schedulers()
+
+    def set_optim_schedulers(self):
+        self.scheduler.optim = self.optim
+        for sch in self.schedulers:
+            sch.optim = self.optim
 
     #---------------------------------------------------------------------------
 
+    def set_scheduler(self, scheduler):
+        self.schedulers = []
+        self.add_scheduler(scheduler)
+
     def add_scheduler(self, scheduler):
-        """ 
-        Установить текущий оптимизатор. todo: список шедулеров
-        """
-        assert self.optim is not None, "Define the optimizer first"
-        self.scheduler = scheduler
-        self.scheduler.optim = self.optim
+        scheduler.optim = self.optim
+        self.schedulers.append(scheduler.optim)        
+
+    def del_scheduler(self, i):
+        self.schedulers.pop(i)
+
+    def clear_schedulers(self):
+        self.scheduler = Scheduler(self.optim)        
+        self.schedulers = []
+
+    def reset_schedulers(self):
+        for sch in self.schedulers:
+            sch.enable = True
+            sch.done   = 0
+
+    def stop_schedulers(self):
+        for sch in self.schedulers:
+            sch.enable = False            
+
+    #---------------------------------------------------------------------------
+
+    def to_device(self, X):
+        if type(X) is list or type(X) is tuple:
+            for i in range(len(X)):
+                X[i] = X[i].to(self.device)
+        else:
+            X = X.to(self.device)
+        return X
 
     #---------------------------------------------------------------------------
 
     def fit(self, epoch, model, data,  train=True, accumulate=1, verbose=1):
         """
         Args:
             * train      - True: режим тренировки, иначе валидации
             * accumulate - аккумулировать градиент для стольки батчей перед сдвигом оптимизатора;
-                           используем, когда большой батч или граф не помещаются в GPU        
+                           используем, когда большой батч или граф не помещаются в GPU
+        https://pytorch.org/blog/what-every-user-should-know-about-mixed-precision-training-in-pytorch/
         """
-        self.model.train(train)              # режим обучение или тестирование
-        torch.set_grad_enabled(train)        # строить или нет вычислительный граф
+        self.model.train(train)                     # режим обучение или тестирование
+        torch.set_grad_enabled(train)               # строить или нет вычислительный граф
 
+        scaler = torch.cuda.amp.GradScaler() if torch.cuda.is_available() else None
         if train:
-            self.optim.zero_grad()            # обнуляем градиенты
+            self.optim.zero_grad()                  # обнуляем градиенты
 
         samples, steps, beg, lst = 0, 0, time.time(), time.time()
-        counts_all, losses_all,  scores_all = torch.empty((0,1)), None,  None
-        for b, batch in enumerate(data):
-            loss, _, scores = model(batch)
-                        
+        counts_all, losses_all,  scores_all = torch.empty(0,1), None,  None
+        for b, (x, y_true) in enumerate(data):
+            num = len(x[0]) if type(x) is list or type(x) is tuple else len(x)
+            x, y_true = self.to_device(x), self.to_device(y_true)
+
+            if scaler is None:
+                y_pred = model(x)
+                loss, scores = model.metrics(x, y_pred, y_true)
+            else:
+                with torch.autocast(device_type=self.device, dtype=self.dtype):
+                    y_pred = model(x)
+                    loss, scores = model.metrics(x, y_pred, y_true)
+
             if train:
-                loss.backward()               # вычисляем градиенты
+                if scaler is None:
+                    loss.backward()   # вычисляем градиенты
+                else:
+                    scaler.scale(loss).backward()   # вычисляем градиенты
                 if (b+1) % accumulate == 0:
-                    self.optim.step()         # подправляем параметры
-                    self.optim.zero_grad()    # обнуляем градиенты
-                    steps      += 1           # число сделанных шагов
-                    self.steps += 1           # число сделанных шагов за всё время
-                self.samples += len(batch[0]) # число просмотренных примеров за всё время
+                    if scaler is None:
+                        self.optim.step()
+                    else:
+                        scaler.step(self.optimizer) # подправляем параметры
+                        scaler.update()             # Updates the scale for next iteration
+                    self.optim.zero_grad()          # обнуляем градиенты
+                    steps      += 1                 # шагов за эпоху
+                    self.hist['steps'] += 1         # шагов за всё время
+                self.hist['samples'] += num         #  примеров за всё время
 
-            samples += len(batch[0])          # число просмотренных примеров за эпоху
+            samples += num                          # просмотренных примеров за эпоху
             losses_all = loss.detach() if losses_all is None else torch.vstack([losses_all, loss.detach()])
             if scores is not None:
                 scores = scores.detach().mean(dim=0)
                 scores_all = scores if scores_all is None else torch.vstack([scores_all, scores])
-            counts_all = torch.vstack([counts_all, torch.Tensor([len(batch[0])])])
+            counts_all = torch.vstack([counts_all, torch.Tensor([num])])
 
             if verbose and (time.time()-lst > 1 or b+1 == len(data) ):
                 lst = time.time()
                 self.fit_progress(epoch, train, (b+1)/len(data),
                                   losses_all, scores_all, counts_all, samples, steps, time.time()-beg)
 
-        if train: self.time_trn += (time.time()-beg)
-        else:     self.time_val += (time.time()-beg)
+        if train: self.hist['time_trn'] += (time.time()-beg)
+        else:     self.hist['time_val'] += (time.time()-beg)
 
         if scores_all is not None:
             scores_all = scores_all.cpu()
-        return losses_all.cpu(), scores_all, counts_all, (samples,steps,time.time()-beg)
-    
+        return losses_all.cpu(), scores_all, counts_all, (samples, steps, time.time()-beg)
+
     #---------------------------------------------------------------------------
 
     def mean(self, losses, scores, counts):
-        """ Вычислить среднее по всей эпохе """      
-        loss  = ((losses.detach().cpu() * counts).sum(dim=0) / counts.sum()).item()        
+        """ Вычислить среднее по всей эпохе """
+        loss  = ((losses.detach().cpu() * counts).sum(dim=0) / counts.sum()).item()
         if scores is not None:
             scores = ((scores.detach().cpu() * counts).sum(dim=0) / counts.sum())
         return (loss, scores)
-            
+
     #---------------------------------------------------------------------------
 
     def fit_progress(self, epoch, train, done, losses, scores, counts, samples, steps, tm):
-        """ 
-        Вывод информации о прогрессе обучения (эпоха, время, ошибка и т.п.) 
+        """
+        Вывод информации о прогрессе обучения (эпоха, время, ошибка и т.п.)
         В конкретном проекте можно перопределить.
         """
         loss, score = self.mean(losses, scores, counts)
-        steps, samples = max(steps, 1), max(samples, 1)             # just in case
+        steps, samples = max(steps, 0), max(samples, 1)             # just in case
         st = ""
         if score is not None and len(score):
             st += f"score={score[0]:.4f} "                          # главная метрика
             if len(score) > 1: st += "("                            # вспомогательные
             for i in range(1, len(score)):
                 st += f"{score[i]:.4f}" + (", " if i+1 < len(score) else ") ")
-        st += f"loss={loss:.4f} "                
-        print(f"\r{epoch:3d}{'t' if train else 'v'}[{100*done:3.0f}%]  {st}  samples={samples} steps={steps}  time={1e3*tm/steps:.3}ms/step  {1e6*tm/samples:.2f}s/1e6", end="  ")
+        st += f"loss={loss:.4f} "
+
+        t_unit, t_unit_scale,  c_unit, c_unit_power = self.unit_scales()
+        print(f"\r{epoch:3d}{'t' if train else 'v'}[{100*done:3.0f}%]  {st}  samples={samples} steps={steps}  time={(0.0 if steps==0 else 1e3*tm/(t_unit_scale*steps)):.3}{t_unit}/step  {c_unit*tm/(t_unit_scale*samples):.2f}{t_unit}/10^{c_unit_power:.0f}", end="                ")
+
+    #---------------------------------------------------------------------------
+
+    def unit_scales(self):
+        """ Единичы измерения числа примеров и времени """
+        view = self.view
+        t_unit = view['time_units'] if 'time_units' in view and view['time_units'] in ['ms','s','m','h']  else 's'
+        t_unit_scale = dict(ms=1e-3, s=1, m=60, h=3600)[t_unit]
+        c_unit = view['count_units'] if view.get('count_units',0) > 0  else 1
+        c_unit_power = round(np.log10(c_unit), 0)
+        return t_unit, t_unit_scale,  c_unit, c_unit_power
 
     #---------------------------------------------------------------------------
 
     def predict(self, model, data, verbose:bool = True, whole=False):
         """
         Вычислить предлсказание, ошибку и метрику для каждого примера в data
         todo: выдели сразу память
         """
         self.model.train(False)          # режим тестирование
         torch.set_grad_enabled(False)    # вычислительный граф не строим
         data.whole = whole               # обычно по всем примерам (и по дробному батчу)
 
         samples, steps, beg, lst = 0, 0, time.time(), time.time()
-        counts_all, losses_all, scores_all, output_all = torch.empty((0,1)), None,  None, None        
+        counts_all, losses_all, scores_all, output_all = torch.empty((0,1)), None,  None, None
 
-        for b, batch in enumerate(data):
-            samples += len(batch[0])                  # число просмотренных примеров
-            loss, output, scores = model(batch)
-            
+        scaler = torch.cuda.amp.GradScaler() if torch.cuda.is_available() else None
+        for b, (x,y_true) in enumerate(data):
+            if scaler is None:
+                y_pred = model(x)
+                loss, scores = model.metrics(x, y_pred, y_true)
+            else:
+                with torch.autocast(device_type=self.device, dtype=self.dtype):
+                    y_pred = model(x)
+                    loss, scores = model.metrics(x, y_pred, y_true)
+
+            num = len(x[0]) if type(x) is list or type(x) is tuple else len(x)
+            samples += num                      # число просмотренных примеров за эпоху
             losses_all = loss.detach() if losses_all is None else torch.vstack([losses_all, loss.detach()])
             if scores is not None:
-                scores = scores.detach().mean(0)
+                scores = scores.detach().mean(dim=0)
                 scores_all = scores if scores_all is None else torch.vstack([scores_all, scores])
-            counts_all = torch.vstack([counts_all, torch.Tensor([len(batch[0])])])
-            output_all = output if output_all is None else torch.vstack([output_all, output.detach()])
+            counts_all = torch.vstack([counts_all, torch.Tensor([num])])
 
             if verbose and (time.time()-lst > 1 or b+1 == len(data) ):
-                lst = time.time()                                
+                lst = time.time()
                 self.fit_progress(0, False, (b+1)/len(data), losses_all, scores_all, counts_all, samples, steps, time.time()-beg)
 
         if scores is not None:
             scores_all = scores_all.cpu()
         return output_all.cpu(),  losses_all.cpu(), scores_all
 
     #---------------------------------------------------------------------------
 
-    def run(self, 
-            epochs = 100,             # число эпох для обучения (проходов одного пака data_trn)
-            pre_val=False,            # перед началом обучения сделать валидацию            
-            period_plot=100,          # через сколько эпох выводить график обучения 
-            period_checks=1,          # через сколько эпох делать чекпоинты (сохранять модель)
-            period_val=1,             # через сколько эпох делать валидацию
-            period_val_beg = 4,       # период валидации на первых samples_beg примерах
-            samples_beg = None,       # потом включается period_val
-            stop_after_samples=None): # остановится после этого числа примеров
+    def run(self,  epochs =None,  samples=None,            
+            pre_val=False, period_val=1, period_plot=100,         
+            period_checks=1, period_val_beg = 4, samples_beg = None ): 
         """
         Args:
-            * epochs               - число эпох для обучения (полных проходов data_trn)
-            * pre_val              - перед началом обучения сделать валидацию
-            * period_val           - через сколько эпох делать валидацию
-            * period_plot          - через сколько эпох выводить график обучения
-            * period_checks        - через сколько эпох делать чекпоинты (сохранять модель)
-            * period_val_beg = 4,  - период валидации на первых samples_beg примерах
-            * samples_beg = None,  - потом включается period_val                        
-            * stop_after_samples   - остановится после этого числа примеров
+            * epochs               - number of epochs for training (passes of one data_trn pack). If not defined (None) works "infinitely".
+            * samples              - if defined, then will stop after this number of samples, even if epochs has not ended
+            * pre_val              - validate before starting training
+            * period_val           - period after which validation run (in epochs)
+            * period_plot          - period after which the training plot is displayed (in epochs)
+            * period_checks        - period after which checkpoints are made and the current model is saved (in epochs)
+            * period_val_beg = 4   - validation period on the first samples_beg examples
+            * samples_beg = None   - the number of samples from the start, after which the validation period will be equal to period_val.
         """
         assert self.optim is not None, "Define the optimizer first"
-        self.scheduler.optim = self.optim
+        self.set_optim_schedulers()        
 
         if pre_val:
             losses, scores, counts, (samples_val, steps_val, tm_val) = self.fit(0, self.model, self.data_val, train=False)
             loss_val, score_val = self.mean(losses, scores, counts)
-            self.add_hist(self.hist_val, self.data_val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, self.scheduler.get_lr())
+            self.add_hist(self.hist['val'], self.data_val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, self.scheduler.get_lr())
             print()
-        
+
+        epochs = epochs or 1_000_000
         #for epoch in tqdm(range(1, epochs+1)):
         for epoch in range(1, epochs+1):
             losses, scores, counts, (samples_trn,steps_trn,tm_trn) = self.fit(epoch, self.model, self.data_trn, train=True)
             loss_trn, score_trn = self.mean(losses, scores, counts)
             lr = self.scheduler.get_lr()
-            self.add_hist(self.hist_trn, self.data_trn.batch_size, samples_trn, steps_trn, tm_trn, loss_trn, score_trn, lr)
+            self.add_hist(self.hist['trn'], self.data_trn.batch_size, samples_trn, steps_trn, tm_trn, loss_trn, score_trn, lr)
 
-            if self.best_loss_trn is None or self.best_loss_trn > loss_trn:
-                self.best_loss_trn = loss_trn
-                self.samples_best_loss_trn = self.samples
-                self.hist_trn['best_loss'].append( (self.samples, self.steps, loss_trn) )
-            if self.best_score_trn is None or self.best_score_trn > score_trn[0]:
-                self.best_score_trn = score_trn[0]
-                self.samples_best_score_trn = self.samples
-                self.hist_trn['best_score'].append((self.samples, self.steps, score_trn[0].item()))
+            if self.hist['best']['loss_trn'] is None or self.hist['best']['loss_trn'] > loss_trn:
+                self.hist['best']['loss_trn'] = loss_trn
+                self.hist['best']['samples_loss_trn'] = self.hist['samples']
+                self.hist['trn']['best_loss'].append( (self.hist['samples'], self.hist['steps'], loss_trn) )
+
+            if self.best_score(self.hist['best']['score_trn'], score_trn):            
+                self.hist['best']['score_trn'] = score_trn[0]
+                self.hist['best']['samples_score_trn'] = self.hist['samples']
+                self.hist['trn']['best_score'].append((self.hist['samples'], self.hist['steps'], score_trn[0].item()))
 
-            period = period_val_beg if samples_beg and  self.samples < samples_beg else period_val
-            if  epoch % period == 0 or epoch == epochs:                
+            period = period_val_beg if samples_beg and  self.hist['samples'] < samples_beg else period_val
+            if  epoch % period == 0 or epoch == epochs:
                 losses, scores, counts, (samples_val,steps_val,tm_val) = self.fit(epoch, self.model, self.data_val, train=False)
                 loss_val, score_val = self.mean(losses, scores, counts)
-                self.add_hist(self.hist_val, self.data_val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, lr)
+                self.add_hist(self.hist['val'], self.data_val.batch_size, samples_val, steps_val, tm_val, loss_val, score_val, lr)
 
                 # save best validation loss:
-                if self.best_loss_val is None or self.best_loss_val > loss_val:       
-                    self.best_loss_val = loss_val
-                    self.samples_best_loss_val = self.samples
-                    self.hist_val['best_loss'].append((self.samples, self.steps, loss_val))
-                    if self.cfg.get('folder_loss', False):
-                        self.save(self.model, folder=self.cfg['folder_loss'], prefix=f"loss_{loss_val:.4f}_{self.now()}")
+                if self.hist['best']['loss_val'] is None or self.hist['best']['loss_val'] > loss_val:
+                    self.hist['best']['loss_val'] = loss_val
+                    self.hist['best']['samples_loss_val'] = self.hist['samples']
+                    self.hist['val']['best_loss'].append((self.hist['samples'], self.hist['steps'], loss_val))
+                    if self.folder_loss:
+                        self.save(self.model, folder=self.folder_loss, prefix=f"loss_{loss_val:.4f}_{self.now()}")
 
                 # save best validation score[0]
-                if score_val is not None  and len(score_val) \
-                and (self.best_score_val is None \
-                     or (self.best_score_val < score_val[0] and self.score_max) \
-                     or (self.best_score_val > score_val[0] and not self.score_max)                     
-                ):  
-                    self.best_score_val = score_val[0]
-                    self.samples_best_score_val = self.samples
-                    self.hist_val['best_score'].append( (self.samples, self.steps, score_val[0].item()) )
-                    if self.cfg.get('folder_score', False):
-                        self.save(self.model, folder=self.cfg['folder_score'], prefix=f"score_{score_val[0]:.4f}_{self.now()}")
+                if self.best_score(self.hist['best']['score_val'], score_val):
+                    self.hist['best']['score_val'] = score_val[0]
+                    self.hist['best']['samples_score_val'] = self.hist['samples']
+                    self.hist['val']['best_score'].append( (self.hist['samples'], self.hist['steps'], score_val[0].item()) )
+                    if self.folder_score:
+                        self.save(self.model, folder=self.folder_score, prefix=f"score_{score_val[0]:.4f}_{self.now()}")
 
                     if self.copy_best_model:         # копия лучшей модели по score
-                        self.model_best_score = copy.deepcopy(self.model) 
+                        self.model_best_score = copy.deepcopy(self.model)
 
             if epoch % period_plot == 0 or epoch == epochs:
-                print(f"\ntime = (trn:{self.time_trn/60:.2f}, val:{self.time_val/60:.2f}, tot:{(self.time_trn+self.time_val)/60:.2f})m  lr:{self.scheduler.get_lr():.1e}")
-                self.plot()
+                self.run_progress()        
+                plot_history(self.hist, self.view) 
+
+            if self.folder_checks and (epoch % period_checks == 0 or epoch == epochs):
+                self.save(self.model, folder=self.folder_checks, prefix="check_"+self.now())
 
-            if self.cfg.get('folder_checks', False) and (epoch % period_checks == 0 or epoch == epochs):
-                self.save(self.model, folder="", prefix="check_"+self.now())
+            self.scheduler.step(samples_trn)
 
-            if stop_after_samples is not None:
-                stop_after_samples -= samples_trn
-                if stop_after_samples <= 0:
+            if samples is not None:
+                samples -= samples_trn
+                if samples <= 0:
                     self.plot()
                     break
 
-            self.scheduler.step(samples_trn)
+    #---------------------------------------------------------------------------
 
-    def plot(self):
-        self.plotter.plot(self.cfg, self.model, data=dict(
-                            hist_val=self.hist_val, hist_trn=self.hist_trn, labels=self.labels,
-                            samples = self.samples, steps = self.steps)
-                        )
+    def run_progress(self):
+        print(f"\ntime = (trn:{self.hist['time_trn']/60:.2f}, val:{self.hist['time_val']/60:.2f}, tot:{(self.hist['time_trn']+self.hist['time_val'])/60:.2f})m  lr:{self.scheduler.get_lr():.1e}")
+    #---------------------------------------------------------------------------
+            
+    def best_score(self, best, score):
+        return score is not None  and len(score) \
+                and (best is None \
+                or (best < score[0] and     self.score_max) \
+                or (best > score[0] and not self.score_max) )
 
     #---------------------------------------------------------------------------
 
     def now(self):
         return datetime.datetime.now().strftime("%m-%d %H:%M:%S")
 
     #---------------------------------------------------------------------------
 
     def add_hist(self, hist, batch_size, samples, steps, tm, loss, score, lr):
-            hist['samples']   .append(self.samples)
-            hist['steps']     .append(self.steps)            
+            hist['samples']   .append(self.hist['samples'])
+            hist['steps']     .append(self.hist['steps'])
             hist['samples_epoch']   .append(samples)
             hist['steps_epoch']     .append(steps)
             hist['batch_size'].append(batch_size)
             hist['time']      .append(tm)
             hist['lr']        .append(lr)
             hist['loss']      .append(loss)
             if score is not None and len(score):
@@ -332,27 +415,16 @@
 
     #---------------------------------------------------------------------------
 
     def save(self, fname, model = None, optim=None, info=""):
         model = model or self.model
         cfg = model.cfg
         state = {
-            'info':            info, 
+            'info':            info,
             'date':            datetime.datetime.now(),   # дата и время
             'config':          cfg,                       # конфигурация модели
-            'model' :          model.state_dict(),        # параметры модели         
+            'model' :          model.state_dict(),        # параметры модели
             'optimizer':       optim.state_dict() if optim is not None else None,
-
-            'data': {                                     # история обучения
-                'steps':           self.steps,            
-                'samples':         self.samples,
-                'hist_trn':        self.hist_trn,
-                'hist_val':        self.hist_val,
-                'labels':          self.labels,             
-                'best_loss_val':   self.best_loss_val,
-                'best_loss_trn':   self.best_loss_trn,                          
-                'best_score_val':  self.best_score_val,
-                'best_score_trn':  self.best_score_trn,
-            }
-        }    
+            'hist':            self.hist,
+        }
         torch.save(state, fname)
-        
+
```

## Comparing `QuNet-0.0.4.dist-info/LICENSE` & `QuNet-0.0.5.dist-info/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
+
```

