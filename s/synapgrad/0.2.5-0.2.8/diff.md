# Comparing `tmp/synapgrad-0.2.5-py3-none-any.whl.zip` & `tmp/synapgrad-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 22280 bytes, number of entries: 19
+Zip file size: 22499 bytes, number of entries: 19
 -rw-rw-rw-  2.0 fat       72 b- defN 23-Apr-08 18:28 synapgrad/__init__.py
 -rw-rw-rw-  2.0 fat    21680 b- defN 23-Apr-12 10:56 synapgrad/engine.py
--rw-rw-rw-  2.0 fat      306 b- defN 23-Apr-13 00:11 synapgrad/nn/__init__.py
+-rw-rw-rw-  2.0 fat      340 b- defN 23-Apr-13 21:18 synapgrad/nn/__init__.py
 -rw-rw-rw-  2.0 fat     4883 b- defN 23-Apr-13 00:43 synapgrad/nn/activations.py
--rw-rw-rw-  2.0 fat     1997 b- defN 23-Apr-11 18:05 synapgrad/nn/layers.py
+-rw-rw-rw-  2.0 fat     2174 b- defN 23-Apr-13 13:34 synapgrad/nn/layers.py
 -rw-rw-rw-  2.0 fat     8087 b- defN 23-Apr-13 00:32 synapgrad/nn/losses.py
 -rw-rw-rw-  2.0 fat     2477 b- defN 23-Apr-11 18:04 synapgrad/nn/modules.py
 -rw-rw-rw-  2.0 fat     2150 b- defN 23-Apr-11 00:40 synapgrad/nn/neurons.py
 -rw-rw-rw-  2.0 fat       46 b- defN 23-Apr-08 14:30 synapgrad/optim/__init__.py
--rw-rw-rw-  2.0 fat     4004 b- defN 23-Apr-11 19:24 synapgrad/optim/optimizers.py
+-rw-rw-rw-  2.0 fat     5290 b- defN 23-Apr-13 12:38 synapgrad/optim/optimizers.py
 -rw-rw-rw-  2.0 fat      154 b- defN 23-Apr-11 17:18 synapgrad/utils/__init__.py
 -rw-rw-rw-  2.0 fat     3403 b- defN 23-Apr-11 18:19 synapgrad/utils/data.py
 -rw-rw-rw-  2.0 fat     1272 b- defN 23-Apr-11 01:07 synapgrad/utils/graph.py
 -rw-rw-rw-  2.0 fat    10586 b- defN 23-Apr-12 12:20 synapgrad/utils/train.py
--rw-rw-rw-  2.0 fat     1088 b- defN 23-Apr-13 00:59 synapgrad-0.2.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4762 b- defN 23-Apr-13 00:59 synapgrad-0.2.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 00:59 synapgrad-0.2.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-13 00:59 synapgrad-0.2.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1525 b- defN 23-Apr-13 00:59 synapgrad-0.2.5.dist-info/RECORD
-19 files, 68594 bytes uncompressed, 19806 bytes compressed:  71.1%
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Apr-13 21:18 synapgrad-0.2.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4700 b- defN 23-Apr-13 21:18 synapgrad-0.2.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-13 21:18 synapgrad-0.2.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-Apr-13 21:18 synapgrad-0.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1525 b- defN 23-Apr-13 21:18 synapgrad-0.2.8.dist-info/RECORD
+19 files, 70029 bytes uncompressed, 20025 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: synapgrad/utils/graph.py
 Comment: 
 
 Filename: synapgrad/utils/train.py
 Comment: 
 
-Filename: synapgrad-0.2.5.dist-info/LICENSE
+Filename: synapgrad-0.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: synapgrad-0.2.5.dist-info/METADATA
+Filename: synapgrad-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: synapgrad-0.2.5.dist-info/WHEEL
+Filename: synapgrad-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: synapgrad-0.2.5.dist-info/top_level.txt
+Filename: synapgrad-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: synapgrad-0.2.5.dist-info/RECORD
+Filename: synapgrad-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synapgrad/nn/__init__.py

```diff
@@ -1,6 +1,6 @@
 
 from .modules import Module, Sequential
 from .neurons import Neuron
-from .layers import Linear, Flatten
+from .layers import Linear, Flatten #, Conv2D, BatchNorm2d, MaxPool2D
 from .losses import Loss, MSELoss, CrossEntropyLoss, NLLLoss, BCELoss, BCEWithLogitsLoss
 from .activations import relu_fn, ReLU, Tanh, tanh_fn, sigmoid_fn, Sigmoid, softmax_fn, Softmax, LogSoftmax
```

## synapgrad/nn/layers.py

```diff
@@ -35,28 +35,35 @@
         self.start_dim = start_dim
         self.end_dim = end_dim
     
     def forward(self, x: Tensor) -> Tensor:
         return x.flatten(self.start_dim, self.end_dim)
 
 
-
-# class Conv2D(Layer):
+class Conv2D(nn.Module):
+    
+    def __init__(self, filters, kernel_size, strides=None, padding=None) -> None:
+        self.filters = filters
+        self.kernel_size = kernel_size
+        self.strides = strides
+        self.padding = padding
+    
+    def forward(self, x: Tensor) -> Tensor:
+        return super().forward(x)
+    
+    
+class BatchNorm2d(nn.Module):
     
-#     def __init__(self, filters, kernel_size, strides=None, padding=None) -> None:
-#         self.filters = filters
-#         self.kernel_size = kernel_size
-#         self.strides = strides
-#         self.padding = padding
+    def __init__(self) -> None:
+        super().__init__()
         
-#     def __call__(self, x:np.ndarray) -> np.ndarray:
-#         super().__call__(x)
-#         ...
-    
-# class BatchNorm2d(Layer):
-#     ...
-    
-# class MaxPool2D(Layer):
-    
-#     def __call__(self, x:np.ndarray) -> np.ndarray:
-#         super().__call__(x)
-#         ...
+    def forward(self, x: Tensor) -> Tensor:
+        return super().forward(x)
+    
+    
+class MaxPool2D(nn.Module):
+    
+    def __init__(self) -> None:
+        super().__init__()
+        
+    def forward(self, x: Tensor) -> Tensor:
+        return super().forward(x)
```

## synapgrad/optim/optimizers.py

```diff
@@ -25,86 +25,112 @@
 class SGD(Optimizer):
     """Reference: 
         https://pytorch.org/docs/stable/generated/torch.optim.SGD.html
     """
     
     def __init__(self, parameters: list[Tensor], lr=0.001, momentum=0, dampening=0,
                  weight_decay=0, nesterov=False, maximize=False) -> None:
+        """
+        Implements stochastic gradient descent (optionally with momentum).
+
+        Args:
+            params (iterable): Iterable of parameters to optimize.
+            lr (float): Learning rate.
+            momentum (float, optional): Momentum factor (default: 0).
+            dampening (float, optional): Dampening for momentum (default: 0).
+            weight_decay (float, optional): Weight decay factor (default: 0).
+            nesterov (bool, optional): Enables Nesterov momentum (default: False).
+            maximize (bool, optional): Whether to maximize the objective (default: False).
+
+        """
         super().__init__(parameters, lr)
         self.momentum = momentum
-        self.acum_m = []
+        self.momentum_buffer = []
         self.nesterov = nesterov
         self.dampening = dampening
         self.maximize = maximize
         self.weight_decay = weight_decay
         
         if nesterov and (momentum <= 0 or dampening != 0):
             raise ValueError("Nesterov momentum requires a momentum and zero dampening")
     
     def step(self):
         super().step()
         with engine.no_grad():
             for i, p in enumerate(self.parameters):
                 grad = p._grad
                 
-                p.data -= self.lr*grad
+                # Weight decay
+                if self.weight_decay != 0:
+                    grad = grad + self.weight_decay*p.data
                 
-                # Pytorch version with extra attrs (Not working yet)
-                # # Weight decay
-                # if self.weight_decay != 0:
-                #     grad += self.weight_decay*p.data
-                
-                # # Momentum
-                # if self.momentum != 0:
-                #     if self.t > 1:
-                #         self.acum_m[i] = self.momentum*self.acum_m[i] + (1-self.dampening)*grad
-                #     else:
-                #         self.acum_m.append(grad)
-                
-                #     # Nesterov
-                #     if self.nesterov:
-                #         grad += self.momentum*self.acum_m[i]
-                #     else:
-                #         grad = self.acum_m[i]
-                
-                # # Update Parameter
-                # if self.maximize:
-                #     p.data += self.lr*grad
-                # else:
-                #     p.data -= self.lr*grad
+                # Momentum
+                if self.momentum != 0:
+                    if self.t > 1:
+                        self.momentum_buffer[i] = self.momentum*self.momentum_buffer[i] + (1.0 - self.dampening)*grad
+                    else:
+                        self.momentum_buffer.append(grad)
+                
+                    # Nesterov
+                    if self.nesterov:
+                        grad = grad + self.momentum*self.momentum_buffer[i]
+                    else:
+                        grad = self.momentum_buffer[i]
+                
+                # Update Parameter
+                if self.maximize:
+                    p.data += self.lr*grad
+                else:
+                    p.data -= p.data - self.lr*grad
         
     
 class Adam(Optimizer):
-    # TODO: Nos working properly
+    """Reference: 
+        https://pytorch.org/docs/stable/generated/torch.optim.Adam.html
+    """
     
-    def __init__(self, parameters: list[Tensor], lr=0.001, beta1=0.9, beta2=0.999, epsilon=1e-8) -> None:
-        """Simplified Adam optimizer -> https://pytorch.org/docs/stable/generated/torch.optim.Adam.html
-            amsgrad = False, maximize = False, weight_decay = 0
+    def __init__(self, parameters: list[Tensor], lr=0.001, betas=(0.9, 0.999), eps=1e-8,
+                    weight_decay=0, maximize=False) -> None:
+        """
+        Implements Adam algorithm.
+        
         Args:
-            beta1 (float): Exponential decay rate for the moving average of the gradient.
-            beta2 (float): Exponential decay rate for the moving average of the squared gradient.
-            epsilon (float): Small value for numerical stability.
+            params (iterable): Iterable of model parameters to optimize.
+            lr (float, optional): Learning rate. Default is 0.001.
+            betas (tuple, optional): Coefficients used for computing running averages of gradient and its square.
+                                    Default is (0.9, 0.999).
+            eps (float, optional): Term added to the denominator to improve numerical stability. Default is 1e-08.
+            weight_decay (float, optional): Weight decay (L2 penalty) factor. Default is 0.
+            maximize (bool, optional): Whether to maximize or minimize the objective function. Default is False.
+        
         """
         super().__init__(parameters, lr)
-        self.beta1 = beta1
-        self.beta2 = beta2
-        self.epsilon = epsilon
+        self.beta1 = betas[0]
+        self.beta2 = betas[1]
+        self.epsilon = eps
+        self.weight_decay = weight_decay
+        self.maximize = maximize
         
-        self.mt = [0 for _ in range(len(parameters))]
-        self.vt = [0 for _ in range(len(parameters))]
+        self.m1 = [0 for _ in range(len(parameters))]
+        self.m2 = [0 for _ in range(len(parameters))]
     
     def step(self):
         super().step()
         with engine.no_grad():
             for i, p in enumerate(self.parameters):
-                # Update the moving average of the gradient
-                m = self.beta1 * self.mt[i] + (1 - self.beta1) * p._grad
-                self.mt[i] = m
-                m_corrected = m / (1 - self.beta1)
-
-                # Update the moving average of the squared gradient
-                v = self.beta2 * self.vt[i]+ (1 - self.beta2) * p._grad**2
-                self.vt[i] = v
-                v_corrected = v / (1 - self.beta2)
+                grad = -p._grad if self.maximize else p._grad   
+                    
+                # Weight decay
+                if self.weight_decay != 0:
+                    grad = grad + self.weight_decay*p.data
+                    
+                # Update biased first moment estimate
+                self.m1[i] = self.beta1 * self.m1[i] + (1.0 - self.beta1) * grad
+                
+                # Update biased second raw moment estimate
+                self.m2[i] = self.beta2 * self.m2[i] + (1.0 - self.beta2) * grad**2.0
+                
+                m1_corrected = self.m1[i] / (1.0 - self.beta1**self.t)
+                m2_corrected = self.m2[i] / (1.0 - self.beta2**self.t)
 
                 # Update the parameters using the Adam formula
-                p.data -= self.lr * m_corrected / (np.sqrt(v_corrected) + self.epsilon)
+                p.data -= (self.lr * m1_corrected) / (np.sqrt(m2_corrected) + self.epsilon)
```

## Comparing `synapgrad-0.2.5.dist-info/LICENSE` & `synapgrad-0.2.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `synapgrad-0.2.5.dist-info/METADATA` & `synapgrad-0.2.8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapgrad
-Version: 0.2.5
+Version: 0.2.8
 Summary: An autograd Tensor-based engine with a deep learning library built on top of it made from scratch
 Home-page: https://github.com/pgmesa/synapgrad
 Author: Pablo García Mesa
 Author-email: pgmesa.sm@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
@@ -78,15 +78,15 @@
 - [x] 2. MLP for handwritten digits classification (MNIST dataset) 
 - [ ] 3. CNN for handwritten digits classification (MNIST dataset)
 
 > :warning: The 3rd example has not been implemented yet
 
 Example 1 (synapgrad MLP solution)     |  Example 2 and 3
 :-------------------------:|:-------------------------:
-![Board Image](/assets/example_moons.png) | ![Check Image](/assets/example_mnist.png) 
+![Image 1](/assets/example_moons.png) | ![Image 2](/assets/example_mnist.png) 
 
 ## Comparisons with other frameworks
 In order to see the efficiency of synapgrad, it is compared with other existing engines (in this case torch and micrograd).
 
 
 | Training Example | synapgrad | torch | micrograd |
 |     :---:        |  :---:  |  :---:  |   :---:   |  
@@ -110,20 +110,18 @@
     y2 = (x2 / x)
     z = y * y2 * x2
     z = z.sum()
     z.backward()
 utils.graph.draw(z)
 ```
 
-![Board Image](/assets/graph_example.svg)
+![Graph Image](/assets/graph_example.svg)
 
 ## Running tests
 To run the unit tests you will have to install PyTorch. In these tests, gradients calculation as well as losses, layers, etc, are assessed with pytorch to check everything is working fine. To run the tests:
 ```bash
 python -m pytest
 ```
 
 ## ToDo list
-- Add extra parameters to SGD
-- Finish Adam optimizer
 - Implement training example 3 (Conv2D, MaxPool2D, BatchNorm2D)
```

## Comparing `synapgrad-0.2.5.dist-info/RECORD` & `synapgrad-0.2.8.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 synapgrad/__init__.py,sha256=rzU1koPmJ4_LyMdxWzho4Qd-qWUqh16aKSgmF5HBOEw,72
 synapgrad/engine.py,sha256=eXyXbUrLbujcr3eGt-iQSarPGGzKzVTBuCdeXuFfVSU,21680
-synapgrad/nn/__init__.py,sha256=Kcf0btBxd4xFxNVjwDe7ukNHaeU7LTqIxzN9aTTd3Yk,306
+synapgrad/nn/__init__.py,sha256=ZWcUAUrg9znsANp3CW6N0heJkGdYqkKL2w974saqzjM,340
 synapgrad/nn/activations.py,sha256=eopMfwYDloR2jR6UmjYceoQznb2mFC280zu44WLQB8A,4883
-synapgrad/nn/layers.py,sha256=61GmWQJ8f3m0O5YuE04l9FU8-mWUlMgBHJHepzmW_lg,1997
+synapgrad/nn/layers.py,sha256=B8lJ6vq07GRAZJ33fUfzmQBBragUdims9VIHHlo02Tg,2174
 synapgrad/nn/losses.py,sha256=KQwCKoKFS6aptCbH3qllsMviNqFZO1o3qlS3VXhrfaw,8087
 synapgrad/nn/modules.py,sha256=Jqw51sbU2S35HR5XpZ1-8ty0rncD25BHbNaDNmshui8,2477
 synapgrad/nn/neurons.py,sha256=zjHsq9Xa61biK3LMkVI21Ca2xJs1E4Aaird2F7MyVg0,2150
 synapgrad/optim/__init__.py,sha256=8X56jD7Dcyw-Hdux1K7_YK9_oc3BuNPk9YwC7gSNWaE,46
-synapgrad/optim/optimizers.py,sha256=pTX9bo4PVRXhx8d4v4AUAXdPhqF0H6dxADxgjPZUgj4,4004
+synapgrad/optim/optimizers.py,sha256=cca-em5N6rxG7vqQ3zeAU0sb9g-6RrDoYaTHpvwOGY4,5290
 synapgrad/utils/__init__.py,sha256=eCwZrBr9yWO92hufOIWwAFhwrA_JuMCsmHeDL7PSAtE,154
 synapgrad/utils/data.py,sha256=cwSsVZwEbB6BU9tWrf5aIeZo9u5KNgar7rVYa6WV328,3403
 synapgrad/utils/graph.py,sha256=D2e2tdOw9tyRRdc3fR2rs0nh7kEMFGWat-hlNE4NHIs,1272
 synapgrad/utils/train.py,sha256=V3j4iqSW9sjSfIz9bski95Ni25KuYzIAkjqD4o3-Tjg,10586
-synapgrad-0.2.5.dist-info/LICENSE,sha256=tILw81bLBHb_8uhiXZAlAo5QrlyMSCJH33lb7GYpz6E,1088
-synapgrad-0.2.5.dist-info/METADATA,sha256=pmu_6ecmNsvQ2hLxLv_upONSZ5VzPS-9MVv8KoOApdU,4762
-synapgrad-0.2.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-synapgrad-0.2.5.dist-info/top_level.txt,sha256=D7_rcC0S5ytl1AFRAo5c73mZggZB-Z_zm_GNIGe0QgM,10
-synapgrad-0.2.5.dist-info/RECORD,,
+synapgrad-0.2.8.dist-info/LICENSE,sha256=tILw81bLBHb_8uhiXZAlAo5QrlyMSCJH33lb7GYpz6E,1088
+synapgrad-0.2.8.dist-info/METADATA,sha256=u6cIqsLuXJ1aqKqzfWAYWNZaO4pQyZ8I8Kr-Vb5tcaA,4700
+synapgrad-0.2.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+synapgrad-0.2.8.dist-info/top_level.txt,sha256=D7_rcC0S5ytl1AFRAo5c73mZggZB-Z_zm_GNIGe0QgM,10
+synapgrad-0.2.8.dist-info/RECORD,,
```

