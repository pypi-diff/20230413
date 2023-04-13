# Comparing `tmp/padiff-0.1.0-py3-none-any.whl.zip` & `tmp/padiff-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,28 @@
-Zip file size: 20308 bytes, number of entries: 15
--rw-r--r--  2.0 unx      715 b- defN 23-Jan-18 04:39 padiff/__init__.py
--rw-r--r--  2.0 unx     2820 b- defN 23-Jan-18 04:38 padiff/actions.py
--rw-r--r--  2.0 unx     7335 b- defN 23-Jan-18 04:38 padiff/auto_diff.py
--rw-r--r--  2.0 unx     7681 b- defN 23-Jan-18 04:38 padiff/cmd.py
--rw-r--r--  2.0 unx     9121 b- defN 23-Jan-18 04:38 padiff/report.py
--rw-r--r--  2.0 unx     1992 b- defN 23-Jan-18 04:38 padiff/stack_info.py
--rw-r--r--  2.0 unx    11882 b- defN 23-Jan-18 04:38 padiff/utils.py
--rw-r--r--  2.0 unx    11166 b- defN 23-Jan-18 04:38 padiff/weights.py
--rw-r--r--  2.0 unx     2319 b- defN 23-Jan-18 04:38 padiff/yaml_loader.py
--rw-r--r--  2.0 unx      610 b- defN 23-Jan-18 04:38 padiff/configs/__init__.py
--rw-r--r--  2.0 unx      195 b- defN 23-Jan-18 04:38 padiff/configs/assign_weight.yaml
--rw-r--r--  2.0 unx      706 b- defN 23-Jan-18 04:39 padiff-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-18 04:39 padiff-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-18 04:39 padiff-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1133 b- defN 23-Jan-18 04:39 padiff-0.1.0.dist-info/RECORD
-15 files, 57774 bytes uncompressed, 18468 bytes compressed:  68.0%
+Zip file size: 48881 bytes, number of entries: 26
+-rw-r--r--  2.0 unx     8515 b- defN 23-Apr-13 08:16 padiff/__init__.py
+-rw-r--r--  2.0 unx     3244 b- defN 23-Apr-13 08:16 padiff/auto_diff.py
+-rw-r--r--  2.0 unx     6302 b- defN 23-Apr-13 08:16 padiff/file_loader.py
+-rw-r--r--  2.0 unx    20366 b- defN 23-Apr-13 08:16 padiff/utils.py
+-rw-r--r--  2.0 unx     6658 b- defN 23-Apr-13 08:16 padiff/weights.py
+-rw-r--r--  2.0 unx   149617 b- defN 23-Apr-13 08:16 padiff/configs/api_mapping.json
+-rw-r--r--  2.0 unx       99 b- defN 23-Apr-13 08:16 padiff/configs/assign_weight.yaml
+-rw-r--r--  2.0 unx     1085 b- defN 23-Apr-13 08:16 padiff/special_init/__init__.py
+-rw-r--r--  2.0 unx     1110 b- defN 23-Apr-13 08:16 padiff/special_init/init_BatchNorm2D.py
+-rw-r--r--  2.0 unx     1320 b- defN 23-Apr-13 08:16 padiff/special_init/init_LSTM.py
+-rw-r--r--  2.0 unx     2124 b- defN 23-Apr-13 08:16 padiff/special_init/init_MultiHeadAttention.py
+-rw-r--r--  2.0 unx     1612 b- defN 23-Apr-13 08:16 padiff/special_init/special_init_pool.py
+-rw-r--r--  2.0 unx    11186 b- defN 23-Apr-13 08:16 padiff/trainer/Checker.py
+-rw-r--r--  2.0 unx     1267 b- defN 23-Apr-13 08:16 padiff/trainer/OptimizerHelper.py
+-rw-r--r--  2.0 unx     4730 b- defN 23-Apr-13 08:16 padiff/trainer/Runner.py
+-rw-r--r--  2.0 unx     4691 b- defN 23-Apr-13 08:16 padiff/trainer/Trainer.py
+-rw-r--r--  2.0 unx      691 b- defN 23-Apr-13 08:16 padiff/trainer/__init__.py
+-rw-r--r--  2.0 unx     1277 b- defN 23-Apr-13 08:16 padiff/trainer/trainer_utils/__init__.py
+-rw-r--r--  2.0 unx     2755 b- defN 23-Apr-13 08:16 padiff/trainer/trainer_utils/actions.py
+-rw-r--r--  2.0 unx    11003 b- defN 23-Apr-13 08:16 padiff/trainer/trainer_utils/hooks.py
+-rw-r--r--  2.0 unx    10269 b- defN 23-Apr-13 08:16 padiff/trainer/trainer_utils/module_struct.py
+-rw-r--r--  2.0 unx     6280 b- defN 23-Apr-13 08:16 padiff/trainer/trainer_utils/report.py
+-rw-r--r--  2.0 unx      678 b- defN 23-Apr-13 08:19 padiff-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 08:19 padiff-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-13 08:19 padiff-0.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2223 b- defN 23-Apr-13 08:19 padiff-0.2.0.dist-info/RECORD
+26 files, 259201 bytes uncompressed, 45287 bytes compressed:  82.5%
```

## zipnote {}

```diff
@@ -1,46 +1,79 @@
 Filename: padiff/__init__.py
 Comment: 
 
-Filename: padiff/actions.py
+Filename: padiff/auto_diff.py
 Comment: 
 
-Filename: padiff/auto_diff.py
+Filename: padiff/file_loader.py
 Comment: 
 
-Filename: padiff/cmd.py
+Filename: padiff/utils.py
 Comment: 
 
-Filename: padiff/report.py
+Filename: padiff/weights.py
 Comment: 
 
-Filename: padiff/stack_info.py
+Filename: padiff/configs/api_mapping.json
 Comment: 
 
-Filename: padiff/utils.py
+Filename: padiff/configs/assign_weight.yaml
 Comment: 
 
-Filename: padiff/weights.py
+Filename: padiff/special_init/__init__.py
 Comment: 
 
-Filename: padiff/yaml_loader.py
+Filename: padiff/special_init/init_BatchNorm2D.py
 Comment: 
 
-Filename: padiff/configs/__init__.py
+Filename: padiff/special_init/init_LSTM.py
 Comment: 
 
-Filename: padiff/configs/assign_weight.yaml
+Filename: padiff/special_init/init_MultiHeadAttention.py
+Comment: 
+
+Filename: padiff/special_init/special_init_pool.py
+Comment: 
+
+Filename: padiff/trainer/Checker.py
+Comment: 
+
+Filename: padiff/trainer/OptimizerHelper.py
+Comment: 
+
+Filename: padiff/trainer/Runner.py
+Comment: 
+
+Filename: padiff/trainer/Trainer.py
+Comment: 
+
+Filename: padiff/trainer/__init__.py
+Comment: 
+
+Filename: padiff/trainer/trainer_utils/__init__.py
+Comment: 
+
+Filename: padiff/trainer/trainer_utils/actions.py
+Comment: 
+
+Filename: padiff/trainer/trainer_utils/hooks.py
+Comment: 
+
+Filename: padiff/trainer/trainer_utils/module_struct.py
+Comment: 
+
+Filename: padiff/trainer/trainer_utils/report.py
 Comment: 
 
-Filename: padiff-0.1.0.dist-info/METADATA
+Filename: padiff-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: padiff-0.1.0.dist-info/WHEEL
+Filename: padiff-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: padiff-0.1.0.dist-info/top_level.txt
+Filename: padiff-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: padiff-0.1.0.dist-info/RECORD
+Filename: padiff-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## padiff/__init__.py

```diff
@@ -8,14 +8,248 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .auto_diff import auto_diff
 
-__all__ = ["auto_diff"]
+__version__ = "0.2.0"
+
+
+# for api -> Layer
+
+import sys, os
+import inspect
+from functools import partial
+
+from importlib.abc import MetaPathFinder, Loader
+from importlib.machinery import SourceFileLoader, ExtensionFileLoader, PathFinder
+
+from .file_loader import global_json_loader as jsons
+
+
+def module_filter(name):
+    if name in jsons.paddle_apis.keys() or name in jsons.torch_apis.keys():
+        return True, name.partition(".")[0]
+    return False, None
+
+
+class PaDiffFinder(MetaPathFinder):
+    def find_spec(self, fullname, path, target=None):
+        if fullname in sys.modules.keys():
+            return None
+        found, module_type = module_filter(fullname)
+        if found:
+            spec = self.sys_find_spec(fullname, path, target)
+            # ExtensionFileLoader loader .so and other lib file
+            # if loader is None, python may use a _NamespaceLoader or other way to init
+            if spec is not None and not isinstance(spec.loader, (ExtensionFileLoader)) and spec.loader is not None:
+                spec._module_type = module_type
+                spec.loader = PaDiffLoader(spec.loader)
+            return spec
+        return None
+
+    # find module by using sys defined finders
+    def sys_find_spec(self, fullname, path, target=None):
+        for finder in sys.meta_path:
+            if isinstance(finder, PaDiffFinder):
+                continue
+            try:
+                find_spec = finder.find_spec
+            except AttributeError:
+                continue
+            spec = find_spec(fullname, path, target)
+            if spec is not None:
+                spec._finder = finder
+                spec._fullname = fullname
+                return spec
+
+        return None
+
+
+def wrap_func(fullname, func):
+    def wrapped(*args, **kwargs):
+
+        if fullname.startswith("paddle"):
+            from .trainer.trainer_utils import paddle_api_hook
+
+            class PaddleApi(paddle.nn.Layer):
+                def __init__(self, func):
+                    super(PaddleApi, self).__init__()
+                    self._func = func
+                    self.__name__ = fullname
+                    self.__api__ = True
+
+                def forward(self, *args, **kwargs):
+                    return self._func(*args, **kwargs)
+
+                def __str__(self):
+                    return self.__name__
+
+            layer = PaddleApi(func)
+            # need idx to support single step, set idx -1 here to skip api in single step mode
+            handle = layer.register_forward_post_hook(partial(paddle_api_hook, net_id=-1))
+
+        elif fullname.startswith("torch"):
+            from .trainer.trainer_utils import torch_api_hook
+
+            class TorchApi(torch.nn.Module):
+                def __init__(self, func):
+                    super(TorchApi, self).__init__()
+                    self.func = func
+                    self.__name__ = fullname
+                    self.__api__ = True
+
+                def forward(self, *args, **kwargs):
+                    return self.func(*args, **kwargs)
+
+                def __str__(self):
+                    return self.__name__
+
+            layer = TorchApi(func)
+            handle = layer.register_forward_hook(partial(torch_api_hook, net_id=-1))
+
+        else:
+            raise RuntimeError("Import Err: module_type not in (paddle, torch)")
+
+        out = layer(*args, **kwargs)
+
+        handle.remove()
+
+        return out
+
+    return wrapped
+
+
+def wrap_method(method_fullname, method):
+    def wrapped(tensor_obj, *args, **kwargs):
+        if method_fullname.startswith("paddle"):
+            from .trainer.trainer_utils import paddle_api_hook
 
-__version__ = "0.1.0"
+            class PaddleMethod(paddle.nn.Layer):
+                def __init__(self, method):
+                    super(PaddleMethod, self).__init__()
+                    self._method = method
+                    self.__name__ = method_fullname
+                    self.__api__ = True
+
+                def forward(self, *args, **kwargs):
+                    return self._method(tensor_obj, *args, **kwargs)
+
+                def __str__(self):
+                    return self.__name__
+
+            layer = PaddleMethod(method)
+            handle = layer.register_forward_post_hook(partial(paddle_api_hook, net_id=-1))
+
+        elif method_fullname.startswith("torch"):
+            from .trainer.trainer_utils import torch_api_hook
+
+            class TorchMethod(torch.nn.Module):
+                def __init__(self, method):
+                    super(TorchMethod, self).__init__()
+                    self._method = method
+                    self.__name__ = method_fullname
+                    self.__api__ = True
+
+                def forward(self, *args, **kwargs):
+                    return self._method(tensor_obj, *args, **kwargs)
+
+                def __str__(self):
+                    return self.__name__
+
+            layer = TorchMethod(method)
+            handle = layer.register_forward_hook(partial(torch_api_hook, net_id=-1))
+
+        else:
+            raise RuntimeError("Import Err: module_type not in (paddle, torch)")
+
+        out = layer(*args, **kwargs)
+
+        handle.remove()
+
+        return out
+
+    return wrapped
+
+
+def wrap_api_method(module):
+    if module.__name__.startswith("paddle"):
+        apis = jsons.paddle_apis[module.__name__]
+    elif module.__name__.startswith("torch"):
+        apis = jsons.torch_apis[module.__name__]
+    else:
+        apis = []
+
+    for api in apis:
+        if api in module.__dict__.keys():
+            obj = module.__dict__[api]
+            if (inspect.isfunction(obj) or inspect.isbuiltin(obj)) and not hasattr(obj, "padiff_wrapped"):
+                module.__dict__[api] = wrap_func(module.__name__ + "." + api, obj)
+                setattr(module.__dict__[api], "padiff_wrapped", True)
+
+    def replace_method(local_tensor, method_fullname):
+        method_name = method_fullname.rpartition(".")[2]
+        if hasattr(local_tensor, method_name):
+            origin_method = getattr(local_tensor, method_name)
+            # callable member of torch.Tensor is methoddescriptor
+            # but callable member of paddle.Tensor is function
+            if not hasattr(origin_method, "padiff_wrapped") and (
+                inspect.ismethoddescriptor(origin_method) or inspect.isfunction(origin_method)
+            ):
+                method_impl = wrap_method(method_fullname, origin_method)
+                setattr(method_impl, "padiff_wrapped", True)
+                setattr(local_tensor, method_name, method_impl)
+
+    if os.getenv("PADIFF_TENSOR_METHOD") != "OFF":
+        if module.__name__ == "paddle":
+            local_tensor = module.Tensor
+            for method_fullname in jsons.paddle_tensor_methods:
+                replace_method(local_tensor, method_fullname)
+
+        if module.__name__ == "torch":
+            local_tensor = module.Tensor
+            for method_fullname in jsons.torch_tensor_methods:
+                replace_method(local_tensor, method_fullname)
+
+
+class PaDiffLoader(Loader):
+    def __init__(self, _loader):
+        self._loader = _loader
+
+    def exec_module(self, module):
+        self._loader.exec_module(module)
+        wrap_api_method(module)
+
+    def create_module(self, spec):
+        return None
+
+
+if os.getenv("PADIFF_API_CHECK") != "OFF":
+    for name in jsons.TORCH_PATH:
+        if name in sys.modules.keys():
+            module = sys.modules[name]
+            wrap_api_method(module)
+
+    for name in jsons.PADDLE_PATH:
+        if name in sys.modules.keys():
+            module = sys.modules[name]
+            wrap_api_method(module)
+
+    sys.meta_path = [PaDiffFinder()] + sys.meta_path
+
+
+import paddle
+import torch
+
+from .utils import LayerMap
+from .weights import assign_weight
+from .auto_diff import auto_diff
+from .special_init import add_special_init
 
-from . import configs
+__all__ = [
+    "auto_diff",
+    "LayerMap",
+    "assign_weight",
+    "add_special_init",
+]
```

## padiff/auto_diff.py

```diff
@@ -8,186 +8,85 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import contextlib
-from functools import partial
 
 import paddle
 import torch
-
-from .report import Report, check_forward_and_backward, current_torch_report, current_paddle_report, report_guard
-from .stack_info import *
 from .utils import (
-    for_each_grad_tensor,
     log,
-    max_diff,
-    reset_log_dir,
-    tensors_mean,
-    traversal_layers,
-    map_structure_and_replace_key,
     init_options,
-    modify_layer_mapping,
+    init_LayerMap,
+    init_padiff_path,
 )
-from .weights import assign_weight, check_weight_grad, remove_inplace
-from .yaml_loader import global_yaml_loader as yamls
-from .cmd import PaDiff_Cmd
+from .weights import assign_weight
+from .trainer import Trainer
+
 
 paddle.set_printoptions(precision=10)
 torch.set_printoptions(precision=10)
 
 
-def auto_diff(layer, module, example_inp, auto_weights=True, options={}, layer_mapping={}):
+def auto_diff(
+    layer, module, example_inp, auto_weights=True, options={}, layer_map=None, loss_fn=None, optimizer=None, steps=1
+):
     """
     Given example inputs, automatically find the first layer with precision diff.
 
     Args:
         layer (paddle.nn.Layer): paddle layer that needs compare
         module (torch.nn.Module): torch module that needs compare
         example_inp (paddle_input, torch_input): input data for paddle layer and torch module.
             paddle_input and torch_input should be dict and send into net like `module(**input)`.
         auto_weights (boolean, optional): uniformly init the parameters of models
         options (dict, optional):
             atol, compare_mode
-        layer_mapping (dict, optional): manually map paddle layer and torch module.
+        layer_map (class LayerMap, optional): manually map paddle layer and torch module.
     Returns:
         True for success, False for failed.
     """
+
+    # checkout inputs
     assert isinstance(layer, paddle.nn.Layer), "Invalid Argument."
     assert isinstance(module, torch.nn.Module), "Invalid Argument."
     assert isinstance(example_inp, (tuple, list)), "Invalid Argument."
-    log("Start auto_diff, may need a while to generate reports...")
 
     paddle_input, torch_input = example_inp
     assert isinstance(paddle_input, dict), "Invalid Argument."
     assert isinstance(torch_input, dict), "Invalid Argument."
-    paddle.set_device("cpu")
-    module = module.to("cpu")
 
-    reset_log_dir()
-    _preprocess(layer, module, auto_weights, options, layer_mapping)
+    if loss_fn is not None:
+        paddle_loss, torch_loss = loss_fn
+        assert callable(paddle_loss), "Invalid loss function"
+        assert callable(torch_loss), "Invalid loss function"
+        options["use_loss"] = True
+
+    if optimizer is not None:
+        paddle_opt, torch_opt = optimizer
+        options["use_opt"] = True
+        if isinstance(paddle_opt, paddle.optimizer.Optimizer) and isinstance(torch_opt, torch.optim.Optimizer):
+            options["opt_type"] = "Opt"
+        else:
+            options["opt_type"] = "Lambda"
+
+    # prepare models and options
+    options["steps"] = steps
+    init_options(options)
+    layer_map = init_LayerMap(layer, module, layer_map)
+    init_padiff_path(layer, module)
+    trainer = Trainer(layer, module, loss_fn, optimizer, layer_map, options)
+    if auto_weights and not assign_weight(layer, module, layer_map):
+        return False
 
-    torch_report = Report("torch")
-    paddle_report = Report("paddle")
-    with report_guard(torch_report, paddle_report):
-        with _register_torch_hooker(module, options, layer_mapping):
-            try:
-                torch_output = module(**torch_input)
-                loss = tensors_mean(torch_output, "torch")
-                if options["diff_phase"] == "both":
-                    loss.backward()
-            except Exception as e:
-                raise RuntimeError(
-                    "Exception is thrown while running forward of torch_module, please check the legality of module.\n{}".format(
-                        str(e)
-                    )
-                )
-
-        with _register_paddle_hooker(layer, options, layer_mapping):
-            try:
-                paddle_output = layer(**paddle_input)
-                loss = tensors_mean(paddle_output, "paddle")
-                if options["diff_phase"] == "both":
-                    loss.backward()
-            except Exception as e:
-                raise RuntimeError(
-                    "Exception is thrown while running forward of paddle_layer, please check the legality of layer.\n{}".format(
-                        str(e)
-                    )
-                )
-
-    log("Max elementwise output diff is {}\n".format(max_diff(paddle_output, torch_output)))
-
-    weight_check, grad_check = check_weight_grad(layer, module, layer_mapping=layer_mapping, options=options)
-    ret = check_forward_and_backward(torch_report, paddle_report, options)
-    ret = ret and weight_check and grad_check
+    ret = trainer.train(example_inp)
 
-    if options["cmd"]:
-        PaDiff_Cmd(paddle_report, torch_report, options).cmdloop()
+    if ret:
+        log("SUCCESS !!!\n")
+    else:
+        log("FAILED !!!\n")
 
     # TODO(linjieccc): pytest failed if log clean is enabled
     # clean_log_dir()
     return ret
-
-
-def tensor_hook(x_grad, bwd_item, nth_tensor):
-    # print (nth_tensor, bwd_item.input_grads, bwd_item.input)
-    bwd_item.set_input_grads(nth_tensor, x_grad)
-    return x_grad
-
-
-def torch_layer_hook(module, input, output, idx, options):
-    rep = current_torch_report()
-    frame_info, frames = extract_frame_summary()
-    fwd_item = rep.put_item("forward", input, output, module, idx, frame_info, frames)
-    bwd_item = rep.put_item("backward", input, output, module, idx, frame_info, frames)
-    bwd_item.set_forward(fwd_item)
-    for i, (t,) in enumerate(for_each_grad_tensor(input)):
-        t.register_hook(partial(tensor_hook, bwd_item=bwd_item, nth_tensor=i))
-    return None
-
-
-def paddle_layer_hook(module, input, output, idx, options):
-    p_rep = current_paddle_report()
-    frame_info, frames = extract_frame_summary()
-    fwd_item = p_rep.put_item("forward", input, output, module, idx, frame_info, frames)
-    bwd_item = p_rep.put_item("backward", input, output, module, idx, frame_info, frames)
-    bwd_item.set_forward(fwd_item)
-    for i, (t,) in enumerate(for_each_grad_tensor(input)):
-        t.register_hook(partial(tensor_hook, bwd_item=bwd_item, nth_tensor=i))
-
-    if options["single_step"]:
-        t_rep = current_torch_report()
-        t_fwd_item = t_rep.find_item(p_rep, idx)
-
-        def tt2pt(tt):
-            if isinstance(tt, torch.Tensor):
-                return paddle.to_tensor(tt.detach().numpy())
-            else:
-                return tt
-
-        return map_structure_and_replace_key(tt2pt, [t_fwd_item.output], output)
-    else:
-        return None
-
-
-@contextlib.contextmanager
-def _register_paddle_hooker(layer, options, layer_mapping={}):
-    remove_handles = []
-    # TODO(xiongkun): duplicate layer is not support, implement custom generator to support (different net_id is ok).
-    idx = 0
-    layers = [layer]
-    layers.extend(traversal_layers(layer, layer_mapping))
-    for mod in layers:
-        handle = mod.register_forward_post_hook(partial(paddle_layer_hook, idx=idx, options=options))
-        remove_handles.append(handle)
-        idx += 1
-    yield
-    for h in remove_handles:
-        h.remove()
-
-
-@contextlib.contextmanager
-def _register_torch_hooker(module, options, layer_mapping={}):
-    remove_handles = []
-    idx = 0
-    modules = [module]
-    modules.extend(traversal_layers(module, layer_mapping))
-    for mod in modules:
-        handle = mod.register_forward_hook(partial(torch_layer_hook, idx=idx, options=options))
-        remove_handles.append(handle)
-        idx += 1
-    yield
-    for h in remove_handles:
-        h.remove()
-
-
-def _preprocess(layer, module, auto_weights, options, layer_mapping):
-    init_options(options)
-    modify_layer_mapping(layer_mapping)
-    remove_inplace(layer, module)
-    yamls.options = options
-    if auto_weights:
-        assign_weight(layer, module, options=options, layer_mapping=layer_mapping)
```

## padiff/utils.py

```diff
@@ -11,22 +11,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import sys
 import shutil
-import warnings
-from collections import namedtuple
 from itertools import zip_longest
 
 import numpy as np
 import paddle
 import torch
-from paddle.fluid.layers.utils import flatten, pack_sequence_as, map_structure
+
+try:
+    from paddle.fluid.layers.utils import flatten, pack_sequence_as, map_structure
+except:
+    from paddle.utils import flatten, pack_sequence_as, map_structure
+from .file_loader import global_yaml_loader as yamls
+
+from .special_init import global_special_init_pool as init_pool
+from .special_init import build_name
+from itertools import zip_longest
+
+
+"""
+    clone tensor
+"""
 
 
 def is_tensor(x):
     return isinstance(x, (paddle.Tensor, torch.Tensor))
 
 
 def is_tensors(*x):
@@ -47,14 +59,56 @@
 def set_require_grad(x):
     if hasattr(x, "requires_grad"):
         x.requires_grad = True
     if hasattr(x, "stop_gradient"):
         x.stop_gradient = False
 
 
+def _clone_tensor(inp):
+    """
+    clone into cpu to save GPU memory.
+    """
+    if isinstance(inp, (torch.Tensor, paddle.Tensor)):
+        if inp.numel() == 0:
+            if isinstance(inp, torch.Tensor):
+                return torch.tensor([], dtype=inp.dtype)
+            else:
+                return paddle.to_tensor([], dtype=inp.dtype)
+        new_t = inp.detach().cpu().clone()
+        if is_require_grad(inp):
+            set_require_grad(new_t)
+        return new_t
+    else:
+        return inp
+
+
+def clone_tensors(inputs):
+    """
+    Clone the tensors in inputs. for example:
+    Inputs = [2, Tensor1, "sdf", Tensor2]
+    Return = [Tensor1_cloned, Tensor2_cloned]
+    """
+    cloned_inputs = []
+    for (t,) in for_each_tensor(inputs):
+        cloned_inputs.append(_clone_tensor(t))
+    return cloned_inputs
+
+
+def clone_structure(inputs):
+    """
+    Clone a nested structure.
+    """
+    return map_structure(_clone_tensor, inputs)
+
+
+"""
+    traversal tools
+"""
+
+
 def for_each_tensor(*structure):
     flat_structure = [flatten(s) for s in structure]
     entries = zip(*flat_structure)
     entries = filter(lambda x: is_tensors(*x), entries)
     for tensors in entries:
         yield tensors
 
@@ -94,304 +148,470 @@
     Apply `func` to each entry in `structure` and return a new structure.
     """
     flat_structure = [flatten(s) for s in structure1]
     entries = zip(*flat_structure)
     return pack_sequence_as(structure2, [func(*x) for x in entries])
 
 
-def _clone_tensor(inp):
-    """
-    clone into cpu to save GPU memory.
-    """
-    if isinstance(inp, (torch.Tensor, paddle.Tensor)):
-        new_t = inp.detach().cpu().clone()
-        if is_require_grad(inp):
-            set_require_grad(new_t)
-        return new_t
-    else:
-        return inp
+"""
+    log utils
+"""
 
+diff_log_path = os.path.join(sys.path[0], "diff_log")
+__reset_log_dir__ = False
 
-def clone_tensors(inputs):
-    """
-    Clone the tensors in inputs. for example:
-    Inputs = [2, Tensor1, "sdf", Tensor2]
-    Return = [Tensor1_cloned, Tensor2_cloned]
-    """
-    cloned_inputs = []
-    for (t,) in for_each_tensor(inputs):
-        cloned_inputs.append(_clone_tensor(t))
-    return cloned_inputs
 
+def reset_log_dir():
+    if os.path.exists(diff_log_path):
+        shutil.rmtree(diff_log_path)
+    os.makedirs(diff_log_path)
 
-def clone_structure(inputs):
-    """
-    Clone a nested structure.
-    """
-    return map_structure(_clone_tensor, inputs)
 
+def clean_log_dir():
+    if not os.listdir(diff_log_path):
+        os.rmdir(diff_log_path)
 
-def is_sublayer(father_net, child_net):
-    """
-    return True if child_net is the DIRECTL children of father_net.
-    """
 
-    def _is_sublayer(father_net, child_net, layer_type):
+def log_file(filename, mode, info):
+    global __reset_log_dir__
+    if not __reset_log_dir__:
+        reset_log_dir()
+        __reset_log_dir__ = True
+
+    filepath = os.path.join(sys.path[0], "diff_log", filename)
+    with open(filepath, mode) as f:
+        f.write(info)
 
-        for child in father_net.children():
-            check_list = child if isinstance(child, layer_type["layer_list"]) else [child]
-            for l in check_list:
-                if isinstance(l, layer_type["sequential"]):
-                    if _is_sublayer(l, child_net, layer_type):
-                        return True
-                else:
-                    if id(l) == id(child_net):
-                        return True
-        return False
-
-    if isinstance(father_net, torch.nn.Module) and isinstance(child_net, torch.nn.Module):
-        layer_type = {
-            "sequential": torch.nn.Sequential,
-            "layer_list": torch.nn.ModuleList,
-        }
-        if _is_sublayer(father_net, child_net, layer_type):
-            return True
-        return False
-    elif isinstance(father_net, paddle.nn.Layer) and isinstance(child_net, paddle.nn.Layer):
-        layer_type = {
-            "sequential": paddle.nn.Sequential,
-            "layer_list": paddle.nn.LayerList,
-        }
-        if _is_sublayer(father_net, child_net, layer_type):
-            return True
-        return False
-    else:
-        raise RuntimeError("father net is not Module / Layer")
+    return filepath
 
 
-def traversal_layers(net, layer_mapping):
-    for child in net.children():
-        if not (isinstance(child, torch.nn.Sequential) or isinstance(child, paddle.nn.Sequential)):
-            yield child
-        ignore_sublayer = False
-        for key, val in layer_mapping.items():
-            if id(child) == id(key) or id(child) == id(val):
-                ignore_sublayer = True
-        if not ignore_sublayer:
-            for sublayer in traversal_layers(child, layer_mapping):
-                yield sublayer
-
-
-class TableView:
-    """
-    A search speedup wrapper class.
-    """
-
-    def __init__(self, data, key=None):
-        self.data = data
-        self.view = {}
-        assert callable(key), "Key must be callable with a paramter: x -> key."
-        for item in self.data:
-            if key(item) not in self.view:
-                self.view[key(item)] = [item]
-            else:
-                warnings.warn("Warning: duplicate key is found, use list + pop strategy.")
-                self.view[key(item)].append(item)
+def log(*args):
+    print("[AutoDiff]", *args)
 
-    def __getitem__(self, key):
-        assert key in self.view, "{} is not found in index.".format(key)
-        ret = self.view[key].pop(0)  # pop for sorting.
-        return ret
-
-    def __len__(self):
-        return len(self.data)
-
-    def __contains__(self, key):
-        return key in self.view
-
-
-class TreeView:
-    """
-    This class is used to organize ReportItems in order of backward process
-
-    wrap items as a tree structure:
-    [1, 2, 3, 4, 5, 6]
-    the last item is the root of the layers.
-    if the child is 2 and 5, then we can construct a tree:
-      6
-      |---------|
-      2         5
-      |         |
-    [1,2]    [3,4,5]   <--- recursive construct.
-    """
-
-    def __init__(self, data):
-        """data is the forward items. the last one is the root layer."""
-        Node = namedtuple("Node", ["value", "children"])
-
-        def _construct_tree(begin_idx, end_idx):
-            if end_idx < begin_idx:
-                raise RuntimeError("[{}, {}] is invalid.".format(begin_idx, end_idx))
-            root = Node(value=data[end_idx], children=[])
-            last = begin_idx
-            for i in range(begin_idx, end_idx):
-                if is_sublayer(root.value.net, data[i].net):
-                    root.children.append(_construct_tree(last, i))
-                    last = i + 1
-            return root
 
-        self.root = _construct_tree(0, len(data) - 1)
-        self.data = data
+def model_repr_info(model):
+    extra_lines = []
+    extra_repr = model.extra_repr()
+    if extra_repr:
+        extra_lines = extra_repr.split("\n")
+    if len(extra_lines) == 1:
+        repr_info = extra_lines[0]
+    else:
+        repr_info = ""
 
-    def __len__(self):
-        return len(self.data)
+    retstr = model.__class__.__name__ + "(" + repr_info + ")"
+    return retstr
 
-    def traversal_forward(self):
-        """
-        with the order of:
-        child1, child2, child3 ... childn, root
-        """
 
-        def _traversal_forward(root):
-            for child in root.children:
-                for item in _traversal_forward(child):
-                    yield item
-            yield root.value
+def weight_struct_info(layer, module, paddle_sublayer, torch_submodule):
+    t_title = "Torch Model\n" + "=" * 25 + "\n"
+    t_retval = print_weight_struct(module, mark=torch_submodule, prefix=[" " * 4])
+    t_info = t_title + "\n".join(t_retval)
 
-        for item in _traversal_forward(self.root):
-            yield item
+    p_title = "Paddle Model\n" + "=" * 25 + "\n"
+    p_retval = print_weight_struct(layer, mark=paddle_sublayer, prefix=[" " * 4])
+    p_info = p_title + "\n".join(p_retval)
 
-    def traversal_backward(self):
-        """
-        with the order of:
-        childn, childn-1, child... child1, root
-        """
+    retstr = ""
 
-        def _traversal_backward(root):
-            for child in root.children[::-1]:
-                for item in _traversal_backward(child):
-                    yield item
-            yield root.value
+    if len(p_retval) + len(t_retval) > 100:
+        log_file("paddle_weight_check.log", "w", p_info)
+        log_file("torch_weight_check.log", "w", t_info)
+        retstr += f"Model Struct saved to `{diff_log_path + '/torch_weight_check.log'}` and `{diff_log_path + '/paddle_weight_check.log'}`.\n"
+        retstr += "Please view the reports and checkout the layers which is marked with `<---  *** HERE ***` !\n"
+    else:
+        retstr += t_info
+        retstr += "\n"
+        retstr += p_info
+        retstr += "\n"
+
+    retstr += "\nNOTICE: layer/module will be marked with `(skip)` for: \n"
+    retstr += "    1. This layer/module is contained by layer_map.\n"
+    retstr += "    2. This layer/module has no parameter, so padiff think it is a wrap layer.\n"
+
+    retstr += "\nHint:\n"
+    retstr += "    1. Check the definition order of params in layer/module is the same.\n"
+    retstr += "    2. Check the corresponding layer/module have the same style:\n"
+    retstr += "       param <=> param, buffer <=> buffer, embedding <=> embedding ...\n"
+    retstr += "       cases like param <=> buffer, param <=> embedding are not allowed,\n"
+    retstr += "       because padiff can not know how to init the parameters.\n"
+    retstr += "    3. If you can not change model codes, try to use a `LayerMap`\n"
+    retstr += "       which can solve almost any problem.\n"
+    retstr += "    0. Visit `https://github.com/PaddlePaddle/PaDiff` to find more infomation !!!\n"
+
+    return retstr
+
+
+def print_weight_struct(net, mark=None, prefix=[]):
+    cur_str = ""
+    for i, s in enumerate(prefix):
+        if i == len(prefix) - 1:
+            cur_str += s
+        else:
+            if s == " |--- ":
+                cur_str += " |    "
+            elif s == " +--- ":
+                cur_str += "      "
+            else:
+                cur_str += s
 
-        for item in _traversal_backward(self.root):
-            yield item
+    cur_str += str(net.__class__.__name__)
 
+    if not hasattr(net, "no_skip"):
+        cur_str += "  (skip)"
 
-diff_log_path = os.path.join(sys.path[0], "diff_log")
+    if os.getenv("PADIFF_PATH_LOG") == "ON" and hasattr(net, "padiff_path"):
+        cur_str += "  (" + net.padiff_path + ")"
 
+    if mark is net:
+        cur_str += "    <---  *** HERE ***"
 
-def reset_log_dir():
-    if os.path.exists(diff_log_path):
-        shutil.rmtree(diff_log_path)
-    os.makedirs(diff_log_path)
+    ret_strs = [cur_str]
 
+    children = list(net.children())
+    for i, child in enumerate(children):
+        pre = " |--- "
+        if i == len(children) - 1:
+            pre = " +--- "
+        prefix.append(pre)
+        retval = print_weight_struct(child, mark, prefix)
+        ret_strs.extend(retval)
+        prefix.pop()
 
-def clean_log_dir():
-    if not os.listdir(diff_log_path):
-        os.rmdir(diff_log_path)
+    return ret_strs
 
 
-def tensors_mean(inp, mode):
-    """
-    TODO(wuzhanfei): This function is used to calcu loss in same way for paddle layer and torch module
-    need to support real opt later
-    """
-    if isinstance(inp, torch.Tensor) or isinstance(inp, paddle.Tensor):
-        return inp.mean()
+def debug_print(net, mark=None, prefix=[]):
+    retval = print_weight_struct(net, mark=None, prefix=[])
+    print("\n".join(retval))
 
-    if mode == "torch":
-        means = []
-        for t in for_each_tensor(inp):
-            means.append(t[0].mean())
-        loss = torch.stack(means).mean()
-        return loss
-    elif mode == "paddle":
-        means = []
-        for t in for_each_tensor(inp):
-            means.append(t[0].mean())
-        loss = paddle.stack(means).mean()
-        return loss
-    else:
-        raise RuntimeError("unrecognized mode `{}`, expected: `torch` or `paddle`".format(mode))
 
+"""
+    tensor compare or compute
+"""
 
-def max_diff(paddle_output, torch_output):
-    p_values = []
-    t_values = []
-    for t in for_each_tensor(paddle_output):
-        p_values.append(t[0])
-    for t in for_each_tensor(torch_output):
-        t_values.append(t[0])
 
+def max_diff(paddle_output, torch_output):
     _max_diff = 0
-    for (pt, tt) in zip(p_values, t_values):
-        temp = np.abs(tt.detach().numpy() - pt.detach().numpy()).max()
+    for (pt,), (tt,) in zip(for_each_tensor(paddle_output), for_each_tensor(torch_output)):
+        if tt.numel() == 0 or pt.numel() == 0:
+            continue
+        temp = np.abs(tt.detach().cpu().numpy() - pt.detach().numpy()).max()
         if temp > _max_diff:
             _max_diff = temp
 
     return _max_diff
 
 
-def log(*args):
-    print("[AutoDiff]", *args)
-
-
-def compare_tensor(tensor1, tensor2, atol=0, rtol=1e-7, compare_mode="mean"):
+def compare_tensor_ret_bool(tensor1, tensor2, atol=0, rtol=1e-7, compare_mode="mean"):
     """
     compare tensor and return bool
     """
     if tensor1 is None and tensor2 is None:
         return True
     if compare_mode == "strict":
         return np.allclose(tensor1, tensor2, atol=atol, rtol=rtol)
     elif compare_mode == "mean":
         return np.allclose(tensor1.mean(), tensor2.mean(), atol=atol, rtol=rtol)
     else:
         raise RuntimeError("compare_mode `{}` is not supported, use `strict` or `mean` instead".format(compare_mode))
 
 
-def assert_tensor_equal(tensor1, tensor2, atol=0, rtol=1e-7, compare_mode="mean"):
+def assert_tensor_equal(tensor1, tensor2, options):
     """if equal: return None
     else: raise Error and Error Message.
     """
+    atol = options["atol"]
+    rtol = options["rtol"]
+    compare_mode = options["compare_mode"]
     if tensor1 is None and tensor2 is None:
         return True
     if compare_mode == "mean":
         np.testing.assert_allclose(tensor1.mean(), tensor2.mean(), atol=atol, rtol=rtol)
     elif compare_mode == "strict":
         np.testing.assert_allclose(tensor1, tensor2, atol=atol, rtol=rtol)
 
 
+def tensors_mean(inp, mode):
+    """
+    TODO(wuzhanfei): This function is used to calcu loss in same way for paddle layer and torch module
+    need to support real opt later
+    """
+    if isinstance(inp, torch.Tensor) or isinstance(inp, paddle.Tensor):
+        return inp.mean()
+
+    if mode == "torch":
+        means = []
+        for t in for_each_tensor(inp):
+            means.append(t[0].to(torch.float32).mean())
+        loss = torch.stack(means).mean()
+        return loss
+    elif mode == "paddle":
+        means = []
+        for t in for_each_tensor(inp):
+            means.append(t[0].astype("float32").mean())
+        loss = paddle.stack(means).mean()
+        return loss
+    else:
+        raise RuntimeError("unrecognized mode `{}`, expected: `torch` or `paddle`".format(mode))
+
+
+"""
+    init tools
+"""
+
+
 def init_options(options):
     default_options = {
         "atol": 0,
         "rtol": 1e-7,
         "diff_phase": "both",
         "compare_mode": "mean",
         "single_step": False,
         "debug": False,
         "cmd": False,
+        "use_loss": False,
+        "use_opt": False,
+        "steps": 1,
     }
 
-    for key in default_options.keys():
-        if key not in options.keys():
-            options[key] = default_options[key]
+    default_options.update(options)
+    options.update(default_options)
 
     if options["single_step"]:
-        options["diff_phase"] = "forward"
-        log("In single_step mode, diff_phase is set to `forward`.")
+        options["steps"] = 1
+        log("  In single_step mode, steps will be set to `1`.")
+        options["use_opt"] = False
+        log("  In single_step mode, optimizer will not be used.")
+    elif options["diff_phase"] == "backward":
+        options["diff_phase"] = "both"
+        log("  Not in single_step mode, diff_phase `backward` is not supported, set to `both` instead.")
+
+    if options["diff_phase"] == "forward":
+        if options["use_opt"]:
+            options["use_opt"] = False
+            log("  Diff_phase is `forward`, optimizer will not be used.")
+        if options["steps"] > 1:
+            options["steps"] = 1
+            log("  Diff_phase is `forward`, steps is set to `1`.")
+
+    if options["steps"] > 1 and options["use_opt"] == False:
+        options["steps"] = 1
+        log("  Steps is set to `1`, because optimizers are not given.")
 
     log("Your options:")
     print("{")
     for key in options.keys():
-        print("  {}: `{}`".format(key, options[key]))
+        if key in ["atol", "rtol", "compare_mode", "single_step", "steps", "use_loss", "use_opt"]:
+            print("  {}: `{}`".format(key, options[key]))
     print("}")
 
+    yamls.options = options
+
+
+def init_LayerMap(layer, module, layer_map):
+    if layer_map is None:
+        layer_map = LayerMap()
+    elif isinstance(layer_map, dict):
+        new_map = LayerMap()
+        new_map.map = layer_map
+        layer_map = new_map
+    else:
+        assert isinstance(layer_map, LayerMap), "Invalid Argument."
+
+    layer_map.ignore_class(layer)
+    layer_map.ignore_class(module)
+
+    return layer_map
+
+
+def init_padiff_path(layer, module):
+    def _set_padiff_path(net, path):
+        for name, child in net.named_children():
+            path.append(name)
+            if not hasattr(child, "padiff_path"):
+                setattr(child, "padiff_path", ".".join(path))
+            _set_padiff_path(child, path)
+            path.pop()
+
+    setattr(layer, "padiff_path", layer.__class__.__name__)
+    setattr(module, "padiff_path", module.__class__.__name__)
+
+    _set_padiff_path(layer, [layer.__class__.__name__])
+    _set_padiff_path(module, [module.__class__.__name__])
+
+
+"""
+    LayerMap
+"""
+
+
+def is_wrap_layer(layer):
+    if isinstance(layer, paddle.nn.Layer):
+        no_param = len(list(layer.parameters(include_sublayers=False))) == 0
+    elif isinstance(layer, torch.nn.Module):
+        no_param = len(list(layer.parameters(recurse=False))) == 0
+    return no_param
+
+
+class LayerMap(object):
+    def __init__(self):
+        self._layer_one2one = {}  # key: torch.nn.Module, value: paddle.nn.Layer
+        self._layer_ignore = set()  # ignore layer in this set
+        self._layer_ignore_sublayer = set()  # ignore sublayer of layers in this set (do not include themselves)
+
+        self._ignore_cls = (  # these classes will be ignored
+            paddle.nn.Sequential,
+            torch.nn.Sequential,
+        )
+
+    @staticmethod
+    def modify_layer_map(layer_map):
+        swap_keys = []
+        for key in layer_map.keys():
+            if not isinstance(key, torch.nn.Module):
+                swap_keys.append(key)
+        for key in swap_keys:
+            layer_map[layer_map[key]] = key
+            layer_map.pop(key)
+
+    @property
+    def map(self):
+        return self._layer_one2one
+
+    @map.setter
+    def map(self, inp):
+        assert isinstance(inp, dict), "LayerMap.map wants `dict` obj as input"
+        LayerMap.modify_layer_map(inp)
+        self._layer_one2one.update(inp)
+        self._layer_ignore_sublayer.update(set(inp.keys()))
+        self._layer_ignore_sublayer.update(set(inp.values()))
+
+    def ignore(self, inp):
+        if isinstance(inp, (list, tuple)):
+            self._layer_ignore.update(set(inp))
+        elif isinstance(inp, (paddle.nn.Layer, torch.nn.Module)):
+            self._layer_ignore.add(inp)
+        else:
+            raise RuntimeError("Unexpect input type for LayerMap.ignore: {}".format(type(inp)))
+
+    def ignore_recursively(self, layers):
+        if isinstance(layers, (paddle.nn.Layer, torch.nn.Module)):
+            layers = [layers]
+        self._layer_ignore_sublayer.update(set(layers))
+        self._layer_ignore.update(set(layers))
+
+    def ignore_class(self, layer, ign_cls=None):
+        ignored = set()
+        if ign_cls == None:
+            ign_cls = self._ignore_cls
+        for sublayer in self.layers_skip_ignore(layer):
+            if isinstance(sublayer, ign_cls):
+                ignored.add(sublayer)
+        self._layer_ignore.update(ignored)
+
+    def _traversal_layers_with_ignore(self, net):
+        for child in net.children():
+            if (child not in self._layer_ignore and not is_wrap_layer(child)) or (
+                child in self.map.keys() or child in self.map.values()
+            ):
+                if not hasattr(child, "no_skip"):
+                    setattr(child, "no_skip", True)
+                yield child
+            if child not in self._layer_ignore_sublayer:
+                for sublayer in self._traversal_layers_with_ignore(child):
+                    yield sublayer
+
+    def _traversal_layers_for_model_struct(self, net):
+        # any in self._layer_ignore_sublayer should be returned
+        # to check whether an api should be record
+        for child in net.children():
+            if (child not in self._layer_ignore and not is_wrap_layer(child)) or (
+                child in self._layer_ignore_sublayer
+            ):
+                if not hasattr(child, "no_skip"):
+                    setattr(child, "no_skip", True)
+                yield child
+            if child not in self._layer_ignore_sublayer:
+                for sublayer in self._traversal_layers_with_ignore(child):
+                    yield sublayer
+
+    def special_init_layers(self):
+        return self.map.items()
+
+    def weight_init_layers(self, layer):
+        # layers in layer_map should be inited in `special_init`, so they will be skipped here
+        layers = [layer]
+        if isinstance(layer, paddle.nn.Layer):
+            layers.extend(filter(lambda x: x not in self.map.values(), self._traversal_layers_with_ignore(layer)))
+        elif isinstance(layer, torch.nn.Module):
+            layers.extend(filter(lambda x: x not in self.map.keys(), self._traversal_layers_with_ignore(layer)))
+        else:
+            raise RuntimeError("Invalid model type: {}".format(type(layer)))
+        return layers
+
+    def layers_skip_ignore(self, layer):
+        layers = [layer]
+        layers.extend(self._traversal_layers_with_ignore(layer))
+        return layers
+
+    def struct_hook_layers(self, layer):
+        layers = [layer]
+        layers.extend(self._traversal_layers_for_model_struct(layer))
+        return layers
+
+    def auto(self, layer, module):
+        """
+        This function will try to find components which support special init, and add them to layer_map automatically.
+
+        NOTICE: LayerMap.auto suppose that all sublayers/submodules are defined in same order, if not, this method may not work correctly.
+        """
+
+        def _traversal_layers(net, path, registered):
+            for name, child in net.named_children():
+                path.append(name)
+                if child.__class__.__name__ in registered and child not in self._layer_ignore:
+                    yield (child, ".".join(path))
+                if child.__class__.__name__ not in registered and child not in self._layer_ignore_sublayer:
+                    for sublayer, ret_path in _traversal_layers(child, path, registered):
+                        yield (sublayer, ret_path)
+                path.pop()
+
+        paddle_layers = list(_traversal_layers(layer, [layer.__class__.__name__], init_pool.registered_paddle_layers))
+        torch_modules = list(
+            _traversal_layers(module, [module.__class__.__name__], init_pool.registered_torch_modules)
+        )
+
+        _map = {}
+
+        log("auto update LayerMap start searching...\n")
+
+        for paddle_info, torch_info in zip_longest(paddle_layers, torch_modules, fillvalue=None):
+            if paddle_info is None or torch_info is None:
+                print(
+                    "\nError: The number of registered paddle sublayer and torch submodule is not the same! Check your model struct first!"
+                )
+                log("auto update LayerMap FAILED!!!\n")
+                return
+
+            paddle_layer, paddle_path = paddle_info
+            torch_module, torch_path = torch_info
+            paddle_name = paddle_layer.__class__.__name__
+            torch_name = torch_module.__class__.__name__
+            name = build_name(paddle_name, torch_name)
+            if name in init_pool.funcs.keys():
+                _map.update({torch_module: paddle_layer})
+                print(
+                    f"++++    paddle `{paddle_name}` at `{paddle_path}` <==> torch `{torch_name}` at `{torch_path}`."
+                )
+            else:
+                print(
+                    "\nError: When generating LayerMap in order, find that paddle sublayer can not matchs torch submodule."
+                )
+                print(f"    paddle: `{paddle_name}` at `{paddle_path}`")
+                print(f"    torch:  `{torch_name}` at `{torch_path}`")
+                log("auto update LayerMap FAILED!!!\n")
+                return
+        print()
+        log("auto update LayerMap SUCCESS!!!\n")
 
-def modify_layer_mapping(layer_mapping):
-    remove_keys = []
-    for key in layer_mapping.keys():
-        if not isinstance(key, paddle.nn.Layer):
-            remove_keys.append(key)
-    for key in remove_keys:
-        layer_mapping[layer_mapping[key]] = key
-        layer_mapping.pop(key)
+        self.map = _map
```

## padiff/weights.py

```diff
@@ -8,247 +8,183 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import os
-import sys
 from itertools import zip_longest
 
 import numpy
 import paddle
 import torch
 
+from .utils import (
+    log,
+    map_for_each_sublayer,
+    LayerMap,
+    weight_struct_info,
+    model_repr_info,
+)
+from .file_loader import global_yaml_loader as yamls
 
-from .utils import log, map_for_each_sublayer, compare_tensor, traversal_layers
-from .yaml_loader import global_yaml_loader as yamls
+from .special_init import global_special_init_pool as init_pool
+from .special_init import build_name
 
 
-def process_each_weight(process, layer, module, options, layer_mapping={}):
+def process_each_weight(process, layer, module, layer_map=LayerMap()):
     """
     Apply process for each pair of parameters in layer(paddle) and module(torch)
 
     Args:
         process (function): process applied to parameters
         layer (paddle.nn.Layer): input paddle layer
         module (torch.nn.Module): input torch module
-        layer_mapping (dict, optional): manually map paddle layer and torch module.
-        options (dict, optional):
-            atol, rtol, compare_mode, single_step
+        layer_map (dict, optional): manually map paddle layer and torch module.
     """
 
     def _process_runner(
         process,
         paddle_sublayer,
         torch_submodule,
-        param_name,
+        paddle_pname,
+        torch_pname,
         paddle_param,
         torch_param,
     ):
-        try:
-            settings = yamls.get_weight_settings(paddle_sublayer, torch_submodule, param_name)
-        except Exception as e:
-            p_model_log = os.path.join(sys.path[0], "diff_log", "paddle_model_struct.log")
-            t_model_log = os.path.join(sys.path[0], "diff_log", "torch_model_struct.log")
-            with open(p_model_log, "w") as log:
-                log.write(str(layer))
-            with open(t_model_log, "w") as log:
-                log.write(str(module))
-            raise e
+
+        settings = yamls.get_weight_settings(paddle_sublayer, torch_submodule, paddle_pname)
 
         process(
             paddle_sublayer,
             torch_submodule,
-            param_name,
+            paddle_pname,
+            torch_pname,
             paddle_param,
             torch_param,
             settings,
         )
 
-    layers = [layer]
-    modules = [module]
-    layers.extend(filter(lambda x: x not in layer_mapping.keys(), traversal_layers(layer, layer_mapping)))
-    modules.extend(filter(lambda x: x not in layer_mapping.values(), traversal_layers(module, layer_mapping)))
+    layers = layer_map.weight_init_layers(layer)
+    modules = layer_map.weight_init_layers(module)
 
     for paddle_sublayer, torch_submodule in zip_longest(layers, modules, fillvalue=None):
         if paddle_sublayer is None or torch_submodule is None:
             raise RuntimeError("Torch and Paddle return difference number of sublayers. Check your model.")
-        for (name, paddle_param), torch_param in zip(
+        for (paddle_pname, paddle_param), (torch_pname, torch_param) in zip(
             paddle_sublayer.named_parameters(prefix="", include_sublayers=False),
-            torch_submodule.parameters(recurse=False),
+            torch_submodule.named_parameters(prefix="", recurse=False),
         ):
-            _process_runner(
-                process,
-                paddle_sublayer,
-                torch_submodule,
-                name,
-                paddle_param,
-                torch_param,
-            )
+            try:
+                _process_runner(
+                    process,
+                    paddle_sublayer,
+                    torch_submodule,
+                    paddle_pname,
+                    torch_pname,
+                    paddle_param,
+                    torch_param,
+                )
+            except Exception as e:
+                err_str = f"Error occured between:\n"
+                err_str += f"    paddle: {model_repr_info(paddle_sublayer)}\n"
+                err_str += f"            {paddle_sublayer.padiff_path + '.' + paddle_pname}\n"
+                err_str += f"    torch: {model_repr_info(torch_submodule)}\n"
+                err_str += f"           {torch_submodule.padiff_path + '.' + torch_pname}\n\n"
+                err_str += f"{type(e).__name__ + ':  ' + str(e)}\n"
+                err_str += weight_struct_info(layer, module, paddle_sublayer, torch_submodule)
+                raise RuntimeError(err_str)
 
 
-def _shape_check(
+def shape_check(
     paddle_sublayer,
     torch_submodule,
-    param_name,
+    paddle_pname,
+    torch_pname,
     paddle_param,
     torch_param,
     settings,
 ):
     p_shape = list(paddle_param.shape)
     t_shape = list(torch_param.shape)
     if settings["transpose"]:
         t_shape.reverse()
-    assert p_shape == t_shape, (
-        "Shape of param `{}` is not the same. {} vs {}\n"
-        "Hint: \n"
-        "      1. check whether your paddle model definition and torch model definition are corresponding.\n"
-        "      2. check the weight shape of paddle:`{}` and torch:`{}` is the same.\n"
-    ).format(param_name, p_shape, t_shape, paddle_sublayer, torch_submodule)
+    assert p_shape == t_shape, ("Shape of paddle param `{}` and torch param `{}` is not the same. {} vs {}\n").format(
+        paddle_pname, torch_pname, p_shape, t_shape
+    )
 
 
 def _assign_weight(
     paddle_sublayer,
     torch_submodule,
-    param_name,
+    paddle_pname,
+    torch_pname,
     paddle_param,
     torch_param,
     settings,
 ):
-    _shape_check(
+    shape_check(
         paddle_sublayer,
         torch_submodule,
-        param_name,
+        paddle_pname,
+        torch_pname,
         paddle_param,
         torch_param,
         settings,
     )
-    np_value = paddle.randn(paddle_param.shape).numpy()
-    paddle.assign(paddle.to_tensor(np_value), paddle_param)
+    np_value = torch_param.data.detach().cpu().numpy()
     if settings["transpose"]:
-        torch_param.data = torch.as_tensor(numpy.transpose(np_value)).type(torch_param.dtype)
-    else:
-        torch_param.data = torch.as_tensor(np_value).type(torch_param.dtype)
+        np_value = numpy.transpose(np_value)
 
+    paddle.assign(paddle.to_tensor(np_value), paddle_param)
 
-def assign_weight(layer, module, options, layer_mapping={}):
+
+def assign_weight(layer, module, layer_map=LayerMap()):
     """
     Init weights of layer(paddle) and module(torch) with same value
 
     Args:
         layer (paddle.nn.Layer): input paddle layer
         module (torch.nn.Module): input torch module
-        layer_mapping (dict, optional): manually map paddle layer and torch module.
     """
 
-    for paddle_sublayer, torch_submodule in layer_mapping.items():
-        assign_config = yamls.assign_yaml.get(paddle_sublayer.__class__.__name__, None)
-        if assign_config is None or assign_config.get("init", False) == False:
+    assert isinstance(layer, paddle.nn.Layer), "The first param of assign_weight should be a paddle.nn.Layer"
+    assert isinstance(module, torch.nn.Module), "The second param of assign_weight should be a torch.nn.Module"
+
+    for torch_submodule, paddle_sublayer in layer_map.special_init_layers():
+        paddle_layer_name = paddle_sublayer.__class__.__name__
+        torch_module_name = torch_submodule.__class__.__name__
+        key_name = build_name(paddle_layer_name, torch_module_name)
+        if key_name not in init_pool.funcs.keys():
             log(
-                "*** Auto weight paddle layer `{}` and torch module `{}` is not supported ***".format(
-                    paddle_sublayer.__class__.__name__, torch_submodule.__class__.__name__
+                "*** Special init paddle layer `{}` and torch module `{}` is not supported ***".format(
+                    paddle_layer_name, torch_module_name
                 )
             )
-            log("*** Checkout the parameters are inited by yourself!!! ***")
+            log("    Checkout the parameters are inited by yourself")
+            log("    ,or you can register your init method!")
         else:
-            special_init(paddle_sublayer, torch_submodule)
-
-    process_each_weight(_assign_weight, layer, module, options, layer_mapping)
-
-
-def check_weight_grad(layer, module, options, layer_mapping={}):
-    """
-    Compare weights and grads between layer(paddle) and module(torch)
-
-    Args:
-        layer (paddle.nn.Layer): input paddle layer
-        module (torch.nn.Module): input torch module
-        layer_mapping (dict, optional): manually map paddle layer and torch module.
-        options (dict, optional):
-            atol, compare_mode
-    """
-    if options["diff_phase"] == "forward":
-        log("Diff_phase is `forward`. Weight and grad check skipped.")
-        return True, True
-
-    _weight_check = True
-    _grad_check = True
-
-    def _check_weight_grad(
-        paddle_sublayer,
-        torch_submodule,
-        param_name,
-        paddle_param,
-        torch_param,
-        settings,
-    ):
-        nonlocal _weight_check, _grad_check
-        _shape_check(
-            paddle_sublayer,
-            torch_submodule,
-            param_name,
-            paddle_param,
-            torch_param,
-            settings,
-        )
-        p_param = paddle_param.numpy()
-        t_param = torch_param.detach().numpy()
-        p_grad = paddle_param.grad.numpy() if paddle_param.grad is not None else None
-        t_grad = torch_param.grad.detach().numpy() if torch_param.grad is not None else None
-        if settings["transpose"]:
-            t_param = numpy.transpose(t_param)
-            if t_grad is not None:
-                t_grad = numpy.transpose(t_grad)
-
-        weight_log_path = os.path.join(sys.path[0], "diff_log", "weight_diff.log")
-        grad_log_path = os.path.join(sys.path[0], "diff_log", "grad_diff.log")
-
-        _weight_check = compare_tensor(
-            p_param,
-            t_param,
-            atol=settings["atol"],
-            rtol=settings["rtol"],
-            compare_mode=settings["compare_mode"],
-        )
-        _grad_check = compare_tensor(
-            p_grad, t_grad, atol=settings["atol"], rtol=settings["rtol"], compare_mode=settings["compare_mode"]
-        )
-
-        if _weight_check is False:
-            with open(weight_log_path, "a") as f:
-                f.write(
-                    "After training, weight value is different for param `{}`.\n"
-                    "paddle: `{}` with value:\n{}\n"
-                    "torch: `{}` with value:\n{}\n\n".format(
-                        param_name, paddle_sublayer, p_param, torch_submodule, t_param
-                    )
-                )
-
-        if _grad_check is False:
-            with open(grad_log_path, "a") as f:
-                f.write(
-                    "After training, grad value is different for param `{}`.\n"
-                    "paddle: `{}` with value\n{}\n"
-                    "torch: `{}` with value\n{}\n\n".format(
-                        param_name, paddle_sublayer, p_grad, torch_submodule, t_grad
-                    )
+            try:
+                init_pool.funcs[key_name](paddle_sublayer, torch_submodule)
+            except Exception as e:
+                print(
+                    f"Special init paddle layer `{paddle_layer_name}` and torch module `{torch_module_name}` failed."
                 )
-
-    process_each_weight(_check_weight_grad, layer, module, options, layer_mapping)
-
-    if _weight_check and _grad_check:
-        log("weight and weight.grad is compared.")
-    else:
-        diff_log_path = os.path.join(sys.path[0], "diff_log")
-        log("Differences in weight or grad !!!")
-        log("Check reports at `{}`\n".format(diff_log_path))
-
-    return _weight_check, _grad_check
+                print(type(e).__name__ + ":  " + str(e))
+                log("Assign weight Failed !!!")
+                return False
+
+    try:
+        process_each_weight(_assign_weight, layer, module, layer_map)
+        log("Assign weight success !!!")
+        return True
+    except Exception as e:
+        log("Assign weight Failed !!!\n")
+        print(type(e).__name__ + ":  " + str(e))
+        return False
 
 
 def remove_inplace(layer, module):
     """
     Set `inplace` tag to `False` for torch module
 
     Args:
@@ -257,55 +193,7 @@
     """
 
     def _remove_inplace(layer, module):
         if hasattr(module, "inplace"):
             module.inplace = False
 
     map_for_each_sublayer(_remove_inplace, layer, module)
-
-
-def special_init(paddle_layer, torch_module):
-    def init_LSTM(layer, module):
-        for (name, paddle_param), torch_param in zip(
-            layer.named_parameters(prefix="", include_sublayers=False),
-            module.parameters(recurse=False),
-        ):
-            settings = yamls.get_weight_settings(layer, module, name)
-            _assign_weight(layer, module, name, paddle_param, torch_param, settings)
-
-    def init_MultiHeadAttention(layer, module):
-        name_param_dict = {}
-        for i, param in enumerate(layer.named_parameters()):
-            pname = param[0]
-            if "cross_attn" in pname:
-                pname = pname.replace("cross_attn", "multihead_attn")
-            elif "q" not in pname and "k" not in pname and "v" not in pname:
-                continue
-            param_np = param[1].numpy()
-            pname = pname.replace("q_proj.", "in_proj_")
-            pname = pname.replace("k_proj.", "in_proj_")
-            pname = pname.replace("v_proj.", "in_proj_")
-            if pname not in name_param_dict:
-                name_param_dict[pname] = param_np
-            elif "_weight" in pname:
-                name_param_dict[pname] = numpy.concatenate((name_param_dict[pname], param_np), axis=1)
-            else:
-                name_param_dict[pname] = numpy.concatenate((name_param_dict[pname], param_np), axis=0)
-
-        device = torch.device("cuda:0")
-        for i, param in enumerate(module.named_parameters()):
-            pname, pa = param[0], param[1]
-            if "in_proj" in pname or "multihead_attn" in pname:
-                param_np = name_param_dict[pname]
-            else:
-                param_np = layer.state_dict()[pname].numpy()
-            if pname.endswith("weight"):
-                param_np = numpy.transpose(param_np)
-
-            param[1].data = torch.from_numpy(param_np)
-
-    special_init_tools = {
-        "LSTM": init_LSTM,
-        "MultiHeadAttention": init_MultiHeadAttention,
-    }
-    name = paddle_layer.__class__.__name__
-    special_init_tools[name](paddle_layer, torch_module)
```

## padiff/configs/assign_weight.yaml

```diff
@@ -1,14 +1,6 @@
-LSTM:
-  torch: LSTM
-  init: True
-
 Linear:
   torch:
     - Linear
     - NonDynamicallyQuantizableLinear
   param:
     weight: transpose
-
-MultiHeadAttention:
-  torch: MultiHeadAttention
-  init: True
```

## Comparing `padiff/actions.py` & `padiff/trainer/trainer_utils/actions.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .utils import assert_tensor_equal
+from .. import utils
 import torch
 import paddle
 
+import warnings
+
 
 class ActionPool:
     def __init__(self):
         self.pool = []
 
     def register(self, cls):
         name = cls.__name__
@@ -67,28 +69,23 @@
     def priority(self):
         return 0
 
     def __call__(self, torch_item, paddle_item, cfg):
         """
         NOTE:
         """
-        atol = cfg["atol"]
-        rtol = cfg["rtol"]
         is_debug = cfg["debug"]
-        compare_mode = cfg["compare_mode"]
         torch_tensors = torch_item.compare_tensors()
         paddle_tensors = paddle_item.compare_tensors()
         for (tt,), (pt,) in zip(torch_tensors, paddle_tensors):
+            if tt.numel() == 0 or pt.numel() == 0:
+                warnings.warn("Found Tensor shape is [0], compare skipped!")
+                continue
             try:
-                assert_tensor_equal(
-                    tt.detach().numpy(),
-                    pt.numpy(),
-                    atol=atol,
-                    compare_mode=compare_mode,
-                )
+                utils.assert_tensor_equal(tt.detach().cpu().numpy(), pt.numpy(), cfg)
             except Exception as e:
                 if is_debug:
                     print("Mean of inputs:")
                     print(torch_item.input[0].numpy().mean())
                     print(paddle_item.input[0].numpy().mean())
                     import pdb
```

## Comparing `padiff/configs/__init__.py` & `padiff/trainer/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,7 +7,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+from .. import utils
+from .Trainer import Trainer
+
+__all__ = [
+    "Trainer",
+]
```

## Comparing `padiff-0.1.0.dist-info/METADATA` & `padiff-0.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: padiff
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tools to automatically diff precision between Paddle and Pytorch Model.
 Home-page: https://github.com/PaddlePaddle/PaDiff
 Author: PaddlePaddle Author
 Author-email: 
 License: Apache 2.0
 Keywords: padiff automatically diff precision between paddle and pytorch model
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Requires-Dist: numpy
 
-UNKNOWN
-
-
```

