# Comparing `tmp/lightning-graphcore-0.0.0.dev0.tar.gz` & `tmp/lightning-graphcore-0.1.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-graphcore-0.0.0.dev0.tar", last modified: Tue Mar 14 09:28:50 2023, max compression
+gzip compressed data, was "lightning-graphcore-0.1.0.dev0.tar", last modified: Fri Apr 21 22:21:15 2023, max compression
```

## Comparing `lightning-graphcore-0.0.0.dev0.tar` & `lightning-graphcore-0.1.0.dev0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 jirka     (1000) jirka     (1000)        0 2023-03-14 09:28:50.854220 lightning-graphcore-0.0.0.dev0/
--rw-rw-r--   0 jirka     (1000) jirka     (1000)      346 2023-03-13 20:37:28.000000 lightning-graphcore-0.0.0.dev0/CHANGELOG.md
--rw-rw-r--   0 jirka     (1000) jirka     (1000)    11352 2023-03-14 08:26:06.000000 lightning-graphcore-0.0.0.dev0/LICENSE
--rw-rw-r--   0 jirka     (1000) jirka     (1000)      709 2023-03-13 20:37:28.000000 lightning-graphcore-0.0.0.dev0/MANIFEST.in
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     3266 2023-03-14 09:28:50.854220 lightning-graphcore-0.0.0.dev0/PKG-INFO
--rw-------   0 jirka     (1000) jirka     (1000)     1904 2023-03-14 09:28:35.000000 lightning-graphcore-0.0.0.dev0/README.md
--rw-rw-r--   0 jirka     (1000) jirka     (1000)       28 2023-03-14 08:52:23.000000 lightning-graphcore-0.0.0.dev0/requirements.txt
--rw-rw-r--   0 jirka     (1000) jirka     (1000)       38 2023-03-14 09:28:50.854220 lightning-graphcore-0.0.0.dev0/setup.cfg
--rwxrwxr-x   0 jirka     (1000) jirka     (1000)     4162 2023-03-14 08:23:12.000000 lightning-graphcore-0.0.0.dev0/setup.py
-drwxrwxr-x   0 jirka     (1000) jirka     (1000)        0 2023-03-14 09:28:50.850221 lightning-graphcore-0.0.0.dev0/src/
-drwxrwxr-x   0 jirka     (1000) jirka     (1000)        0 2023-03-14 09:28:50.850221 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore/
--rw-rw-r--   0 jirka     (1000) jirka     (1000)      452 2023-03-14 08:26:06.000000 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore/__about__.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)      360 2023-03-14 09:28:34.000000 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore/__init__.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     2313 2023-03-14 08:56:57.000000 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore/accelerator.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     3848 2023-03-14 08:56:59.000000 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore/precision.py
--rw-rw-r--   0 jirka     (1000) jirka     (1000)    17007 2023-03-14 08:56:59.000000 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore/strategy.py
-drwxrwxr-x   0 jirka     (1000) jirka     (1000)        0 2023-03-14 09:28:50.854220 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore.egg-info/
--rw-rw-r--   0 jirka     (1000) jirka     (1000)     3266 2023-03-14 09:28:50.000000 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore.egg-info/PKG-INFO
--rw-rw-r--   0 jirka     (1000) jirka     (1000)      533 2023-03-14 09:28:50.000000 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore.egg-info/SOURCES.txt
--rw-rw-r--   0 jirka     (1000) jirka     (1000)        1 2023-03-14 09:28:50.000000 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore.egg-info/dependency_links.txt
--rw-rw-r--   0 jirka     (1000) jirka     (1000)        1 2023-03-14 09:28:50.000000 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore.egg-info/not-zip-safe
--rw-rw-r--   0 jirka     (1000) jirka     (1000)      153 2023-03-14 09:28:50.000000 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore.egg-info/requires.txt
--rw-rw-r--   0 jirka     (1000) jirka     (1000)       20 2023-03-14 09:28:50.000000 lightning-graphcore-0.0.0.dev0/src/lightning_graphcore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:21:15.832266 lightning-graphcore-0.1.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11352 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-21 22:21:15.832266 lightning-graphcore-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 22:21:15.832266 lightning-graphcore-0.1.0.dev0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4162 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:21:15.828266 lightning-graphcore-0.1.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:21:15.832266 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-04-21 22:21:05.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:21:15.832266 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 22:21:15.000000 lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/top_level.txt
```

### Comparing `lightning-graphcore-0.0.0.dev0/LICENSE` & `lightning-graphcore-0.1.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.0.0.dev0/MANIFEST.in` & `lightning-graphcore-0.1.0.dev0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.0.0.dev0/setup.py` & `lightning-graphcore-0.1.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-graphcore-0.0.0.dev0/src/lightning_graphcore/accelerator.py` & `lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/accelerator.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,30 +10,37 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Dict, List
 
 import torch
-from lightning_fabric.utilities.types import _DEVICE
 from lightning_utilities.core.imports import package_available
-from pytorch_lightning.accelerators.accelerator import Accelerator
+
+if package_available("lightning"):
+    from lightning.fabric.utilities.types import _DEVICE
+    from lightning.pytorch.accelerators.accelerator import Accelerator
+elif package_available("pytorch_lightning"):
+    from lightning_fabric.utilities.types import _DEVICE
+    from pytorch_lightning.accelerators.accelerator import Accelerator
+else:
+    raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
 
 _POPTORCH_AVAILABLE = package_available("poptorch")
 
 if _POPTORCH_AVAILABLE:
     import poptorch
 
     _IPU_AVAILABLE = poptorch.ipuHardwareIsAvailable()
 else:
     poptorch = None
     _IPU_AVAILABLE = False
 
 
-class AcceleratorIPU(Accelerator):
+class IPUAccelerator(Accelerator):
     """Accelerator for IPUs.
 
     .. warning::  Use of this accelerator beyond import and instantiation is experimental.
     """
 
     def setup_device(self, device: torch.device) -> None:
         pass
@@ -48,15 +55,15 @@
     @staticmethod
     def parse_devices(devices: int) -> int:
         """Accelerator device parsing logic."""
         return devices
 
     @staticmethod
     def get_parallel_devices(devices: int) -> List[int]:
-        """Gets parallel devices for the Accelerator."""
+        """Get parallel devices for the Accelerator."""
         return list(range(devices))
 
     @staticmethod
     def auto_device_count() -> int:
         """Get the devices when set to auto."""
         # TODO (@kaushikb11): 4 is the minimal unit they are shipped in.
         # Update this when api is exposed by the Graphcore team.
```

### Comparing `lightning-graphcore-0.0.0.dev0/src/lightning_graphcore/precision.py` & `lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/precision.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,30 +9,44 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Any, Callable, Literal, Union, cast
 
-from lightning_fabric.utilities.types import Optimizable
-from pytorch_lightning.plugins.precision.precision_plugin import PrecisionPlugin
-from pytorch_lightning.utilities import GradClipAlgorithmType
-from pytorch_lightning.utilities.exceptions import MisconfigurationException
-from pytorch_lightning.utilities.model_helpers import is_overridden
-from pytorch_lightning.utilities.rank_zero import WarningCache
+from lightning_utilities.core.imports import package_available
 from torch import Tensor
 from torch.optim import LBFGS, Optimizer
 from typing_extensions import get_args
 
+if package_available("lightning"):
+    from lightning.fabric.utilities.types import Optimizable
+    from lightning.pytorch import LightningModule
+    from lightning.pytorch.plugins.precision.precision_plugin import PrecisionPlugin
+    from lightning.pytorch.utilities import GradClipAlgorithmType
+    from lightning.pytorch.utilities.exceptions import MisconfigurationException
+    from lightning.pytorch.utilities.model_helpers import is_overridden
+    from lightning.pytorch.utilities.rank_zero import WarningCache
+elif package_available("pytorch_lightning"):
+    from lightning_fabric.utilities.types import Optimizable
+    from pytorch_lightning import LightningModule
+    from pytorch_lightning.plugins.precision.precision_plugin import PrecisionPlugin
+    from pytorch_lightning.utilities import GradClipAlgorithmType
+    from pytorch_lightning.utilities.exceptions import MisconfigurationException
+    from pytorch_lightning.utilities.model_helpers import is_overridden
+    from pytorch_lightning.utilities.rank_zero import WarningCache
+else:
+    raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
+
 warning_cache = WarningCache()
 
 _PRECISION_INPUT = Literal["32-true", "16-mixed"]
 
 
-class PrecisionIPU(PrecisionPlugin):
+class IPUPrecision(PrecisionPlugin):
     """Precision plugin for IPU integration.
 
     .. warning::  This is an :ref:`experimental <versioning:Experimental API>` feature.
 
     Raises:
         ValueError:
             If the precision is neither 16-mixed nor 32-true.
@@ -43,28 +57,28 @@
         if precision not in supported_precision:
             raise ValueError(
                 f"`Trainer(accelerator='ipu', precision={precision!r})` is not supported."
                 f" `precision` must be one of: {supported_precision}."
             )
         self.precision = cast(_PRECISION_INPUT, str(precision))
 
-    def backward(  # type: ignore[override]
+    def backward(
         self,
         tensor: Tensor,
         model: LightningModule,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         if is_overridden("backward", model):
             warning_cache.warn(
                 "You have overridden the `LightningModule.backward` hook but it will be ignored since IPUs handle"
                 " the backward logic internally."
             )
 
-    def optimizer_step(  # type: ignore[override]
+    def optimizer_step(
         self,
         optimizer: Optimizable,
         model: LightningModule,
         closure: Callable[[], Any],
         **kwargs: Any,
     ) -> Any:
         """IPUs handle the optimizer step internally."""
```

### Comparing `lightning-graphcore-0.0.0.dev0/src/lightning_graphcore/strategy.py` & `lightning-graphcore-0.1.0.dev0/src/lightning_graphcore/strategy.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,44 +13,76 @@
 # limitations under the License.
 import json
 import os
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import pytorch_lightning as pl
 import torch
-from lightning_fabric.plugins import CheckpointIO, ClusterEnvironment
-from lightning_fabric.utilities.cloud_io import get_filesystem
 from lightning_utilities.core.apply_func import apply_to_collection
-from pytorch_lightning import Trainer
-from pytorch_lightning.accelerators import Accelerator
-from pytorch_lightning.overrides.base import _LightningModuleWrapperBase
-from pytorch_lightning.plugins.precision import PrecisionPlugin
-from pytorch_lightning.strategies.parallel import ParallelStrategy
-from pytorch_lightning.strategies.strategy import TBroadcast
-from pytorch_lightning.strategies.utils import _fp_to_half
-from pytorch_lightning.trainer.states import RunningStage, TrainerFn
-from pytorch_lightning.utilities import rank_zero_warn
-from pytorch_lightning.utilities.data import _get_dataloader_init_args_and_kwargs, _reinstantiate_wrapped_cls
-from pytorch_lightning.utilities.exceptions import MisconfigurationException
-from pytorch_lightning.utilities.model_helpers import is_overridden
-from pytorch_lightning.utilities.types import STEP_OUTPUT
+from lightning_utilities.core.imports import package_available
 from torch import Tensor
 from torch.utils.data import DataLoader, Sampler
 
+if package_available("lightning"):
+    from lightning.fabric.plugins import CheckpointIO, ClusterEnvironment
+    from lightning.fabric.utilities.cloud_io import get_filesystem
+    from lightning.pytorch import Trainer
+    from lightning.pytorch.accelerators import Accelerator
+    from lightning.pytorch.overrides.base import _LightningModuleWrapperBase
+    from lightning.pytorch.plugins.precision import PrecisionPlugin
+    from lightning.pytorch.strategies.parallel import ParallelStrategy
+    from lightning.pytorch.strategies.strategy import TBroadcast
+    from lightning.pytorch.strategies.utils import _fp_to_half
+    from lightning.pytorch.trainer.states import RunningStage, TrainerFn
+    from lightning.pytorch.utilities import rank_zero_warn
+    from lightning.pytorch.utilities.data import _get_dataloader_init_args_and_kwargs, _reinstantiate_wrapped_cls
+    from lightning.pytorch.utilities.exceptions import MisconfigurationException
+    from lightning.pytorch.utilities.model_helpers import is_overridden
+    from lightning.pytorch.utilities.types import STEP_OUTPUT
+elif package_available("pytorch_lightning"):
+    from lightning_fabric.plugins import CheckpointIO, ClusterEnvironment
+    from lightning_fabric.utilities.cloud_io import get_filesystem
+    from pytorch_lightning import Trainer
+    from pytorch_lightning.accelerators import Accelerator
+    from pytorch_lightning.overrides.base import _LightningModuleWrapperBase
+    from pytorch_lightning.plugins.precision import PrecisionPlugin
+    from pytorch_lightning.strategies.parallel import ParallelStrategy
+    from pytorch_lightning.strategies.strategy import TBroadcast
+    from pytorch_lightning.strategies.utils import _fp_to_half
+    from pytorch_lightning.trainer.states import RunningStage, TrainerFn
+    from pytorch_lightning.utilities import rank_zero_warn
+    from pytorch_lightning.utilities.data import _get_dataloader_init_args_and_kwargs, _reinstantiate_wrapped_cls
+    from pytorch_lightning.utilities.exceptions import MisconfigurationException
+    from pytorch_lightning.utilities.model_helpers import is_overridden
+    from pytorch_lightning.utilities.types import STEP_OUTPUT
+else:
+    raise ModuleNotFoundError("You are missing `lightning` or `pytorch-lightning` package, please install it.")
+
 from lightning_graphcore.accelerator import _IPU_AVAILABLE, _POPTORCH_AVAILABLE
 
 if _POPTORCH_AVAILABLE:
     import poptorch
 else:
     poptorch = None
 
 
-class StrategyIPU(ParallelStrategy):
+class IPUStrategy(ParallelStrategy):
     """Plugin for training on IPU devices.
 
+    Args:
+        device_iterations: Number of iterations to run on device at once before returning to host.
+            This can be used as an optimization to speed up training.
+            https://docs.graphcore.ai/projects/poptorch-user-guide/en/latest/batching.html
+        autoreport: Enable auto-reporting for IPUs using PopVision
+            https://docs.graphcore.ai/projects/graphcore-popvision-user-guide/en/latest/graph/graph.html
+        autoreport_dir: Optional directory to store autoReport output.
+        training_opts: Optional ``poptorch.Options`` to override the default created options for training.
+        inference_opts: Optional ``poptorch.Options`` to override the default
+            created options for validation/testing and predicting.
+
     .. warning::  This is an :ref:`experimental <versioning:Experimental API>` feature.
     """
 
     strategy_name = "ipu_strategy"
 
     def __init__(
         self,
@@ -61,25 +93,14 @@
         parallel_devices: Optional[List[torch.device]] = None,
         cluster_environment: Optional[ClusterEnvironment] = None,
         checkpoint_io: Optional[CheckpointIO] = None,
         precision_plugin: Optional[PrecisionPlugin] = None,
         training_opts: Optional["poptorch.Options"] = None,
         inference_opts: Optional["poptorch.Options"] = None,
     ) -> None:
-        """Arguments:
-        device_iterations: Number of iterations to run on device at once before returning to host.
-        This can be used as an optimization to speed up training.
-        https://docs.graphcore.ai/projects/poptorch-user-guide/en/latest/batching.html
-        autoreport: Enable auto-reporting for IPUs using PopVision
-        https://docs.graphcore.ai/projects/graphcore-popvision-user-guide/en/latest/graph/graph.html
-        autoreport_dir: Optional directory to store autoReport output.
-        training_opts: Optional ``poptorch.Options`` to override the default created options for training.
-        inference_opts: Optional ``poptorch.Options`` to override the default
-        created options for validation/testing and predicting.
-        """
         super().__init__(
             accelerator=accelerator,
             parallel_devices=parallel_devices,
             cluster_environment=cluster_environment,
             checkpoint_io=checkpoint_io,
             precision_plugin=precision_plugin,
         )
@@ -230,36 +251,34 @@
         def to_tuple(x: Any) -> Tuple:
             return tuple(x)
 
         def to_tensor(x: Any) -> Tensor:
             return torch.tensor(x).unsqueeze(0).repeat(self._n_replicate)
 
         args = apply_to_collection(args, dtype=list, function=to_tuple)
-        args = apply_to_collection(args, dtype=(int, float), function=to_tensor)
-        return args
+        return apply_to_collection(args, dtype=(int, float), function=to_tensor)
 
     def batch_to_device(self, batch: Any, device: Optional[torch.device] = None, dataloader_idx: int = 0) -> Any:
         # This override is necessary because the cast must occur before the data
         # is moved to the device to prevent wasteful host->device copies.
-        batch = apply_to_collection(batch, Tensor, function=_fp_to_half, precision=self.precision_plugin.precision)
         # We don't call `super().batch_to_device` because `data.to(device)` is not
         # currently necessary for IPUs. The movement of data from host<->IPU is
         # currently handled by PopTorch.
-        return batch
+        return apply_to_collection(batch, Tensor, function=_fp_to_half, precision=self.precision_plugin.precision)
 
     def _disable_zero_grad(self) -> None:
         lightning_module = self.lightning_module
         assert lightning_module is not None
         if is_overridden("optimizer_zero_grad", lightning_module):
             assert lightning_module is not None  # `is_overridden` returns False otherwise
             rank_zero_warn(
                 "You have overridden the `LightningModule.optimizer_zero_grad` hook but it will be ignored since"
                 " IPUs handle the zeroing of gradients internally."
             )
-        lightning_module.optimizer_zero_grad = None  # type: ignore[assignment]
+        lightning_module.optimizer_zero_grad = None
 
     def _step(self, stage: RunningStage, *args: Any, **kwargs: Any) -> STEP_OUTPUT:
         args = self._prepare_input(args)
         poptorch_model = self.poptorch_models[stage]
         with pl.core.module._jit_is_scripting():
             return poptorch_model(*args, **kwargs)
 
@@ -283,17 +302,15 @@
         if self._update_dataloader_original is not None:
             # undo dataloader patching
             pl.trainer.connectors.data_connector._update_dataloader = self._update_dataloader_original
 
         assert self.lightning_module is not None
         if self._optimizer_zero_grad_original is not None:
             # re-enable `optimizer_zero_grad`
-            self.lightning_module.optimizer_zero_grad = (  # type: ignore[method-assign]
-                self._optimizer_zero_grad_original
-            )
+            self.lightning_module.optimizer_zero_grad = self._optimizer_zero_grad_original
 
         for model in self.poptorch_models.values():
             model.destroy()
 
         super().teardown()
 
     def _compiled(self, model: Any) -> bool:
@@ -303,15 +320,15 @@
     def _detach_models(self) -> None:
         """Detaches all stage specific models from IPU devices."""
         for k, model in self.poptorch_models.items():
             if self._compiled(model) and model.isAttachedToDevice():
                 model.detachFromDevice()
 
     def _load_model(self, stage: RunningStage) -> None:
-        """Loads the stage specific accelerator model onto device if compiled and not attached to IPU devices.
+        """Load the stage specific accelerator model onto device if compiled and not attached to IPU devices.
 
         Args:
             stage: The stage to load
         """
         self._detach_models()
         model = self.poptorch_models[stage]
         if self._compiled(model) and not model.isAttachedToDevice():
```

### Comparing `lightning-graphcore-0.0.0.dev0/src/lightning_graphcore.egg-info/SOURCES.txt` & `lightning-graphcore-0.1.0.dev0/src/lightning_graphcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

