# Comparing `tmp/torch_activation-0.1.1.tar.gz` & `tmp/torch_activation-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_activation-0.1.1.tar", max compression
+gzip compressed data, was "torch_activation-0.1.2.tar", max compression
```

## Comparing `torch_activation-0.1.1.tar` & `torch_activation-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      466 2023-06-15 08:18:26.113267 torch_activation-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3450 2023-06-15 13:03:48.769903 torch_activation-0.1.1/README.md
--rw-r--r--   0        0        0      568 2023-06-13 07:56:12.907632 torch_activation-0.1.1/torch_activation/__init__.py
--rw-r--r--   0        0        0     2773 2023-05-26 05:12:46.037659 torch_activation-0.1.1/torch_activation/composite.py
--rw-r--r--   0        0        0     3485 2023-06-15 07:47:52.228991 torch_activation-0.1.1/torch_activation/glu_family.py
--rw-r--r--   0        0        0     2617 2023-06-15 08:19:53.268211 torch_activation-0.1.1/torch_activation/lincomb.py
--rw-r--r--   0        0        0     2417 2023-06-15 08:18:56.286253 torch_activation-0.1.1/torch_activation/non_linear.py
--rw-r--r--   0        0        0     6141 2023-06-15 08:32:42.119866 torch_activation-0.1.1/torch_activation/relu_family.py
--rw-r--r--   0        0        0     3525 2023-06-15 08:35:39.534749 torch_activation-0.1.1/torch_activation/trig.py
--rw-r--r--   0        0        0     2877 2023-05-26 04:49:13.643443 torch_activation-0.1.1/torch_activation/utils.py
--rw-r--r--   0        0        0     4197 1970-01-01 00:00:00.000000 torch_activation-0.1.1/setup.py
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 torch_activation-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-06-16 00:29:16.944161 torch_activation-0.1.2/LICENSE
+-rw-r--r--   0        0        0      466 2023-06-23 22:31:18.215046 torch_activation-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2041 2023-06-23 22:30:32.455234 torch_activation-0.1.2/README.md
+-rw-r--r--   0        0        0      556 2023-06-23 22:31:19.225348 torch_activation-0.1.2/torch_activation/__init__.py
+-rw-r--r--   0        0        0     2742 2023-06-23 22:30:32.476477 torch_activation-0.1.2/torch_activation/composite.py
+-rw-r--r--   0        0        0     3331 2023-06-22 12:04:21.368192 torch_activation-0.1.2/torch_activation/glus.py
+-rw-r--r--   0        0        0     2541 2023-06-22 12:04:21.370191 torch_activation-0.1.2/torch_activation/lincomb.py
+-rw-r--r--   0        0        0     2282 2023-06-22 12:04:21.371197 torch_activation-0.1.2/torch_activation/non_linear.py
+-rw-r--r--   0        0        0     6320 2023-06-22 12:04:21.372196 torch_activation-0.1.2/torch_activation/relus.py
+-rw-r--r--   0        0        0     3546 2023-06-22 12:04:21.373204 torch_activation-0.1.2/torch_activation/trig.py
+-rw-r--r--   0        0        0     4601 2023-06-23 22:30:32.478000 torch_activation-0.1.2/torch_activation/utils.py
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 torch_activation-0.1.2/setup.py
+-rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 torch_activation-0.1.2/PKG-INFO
```

### Comparing `torch_activation-0.1.1/torch_activation/__init__.py` & `torch_activation-0.1.2/torch_activation/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .composite import DELU, DReLUs
 from .trig import CosLU, GCU, SinLU
 from .lincomb import LinComb, NormLinComb
 from .non_linear import CoLU, ScaledSoftSign
-from .glu_family import ReGLU, GeGLU, SeGLU, SwiGLU
-from .relu_family import ShiLU, CReLU, ReLUN, SquaredReLU, StarReLU
+from .glus import ReGLU, GeGLU, SeGLU, SwiGLU
+from .relus import ShiLU, CReLU, ReLUN, SquaredReLU, StarReLU
 
 
 __all__ = ["ShiLU", "DELU", "CReLU", "GCU",
            "CosLU", "CoLU", "ReLUN",
            "SquaredReLU", "ScaledSoftSign",
            "ReGLU", "GeGLU", "SeGLU", "SwiGLU"
            "LinComb", "NormLinComb", "SinLU"
            "DReLUs", "StarReLU"]
 
-__version__ = "0.1.0"
+__version__ = "0.1.2"
```

### Comparing `torch_activation-0.1.1/torch_activation/composite.py` & `torch_activation-0.1.2/torch_activation/composite.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,35 +7,32 @@
 class DELU(nn.Module):
     r"""
     Applies the DELU activation function:
 
     :math:`\text{DELU}(x) = \begin{cases} \text{SiLU}(x), x \leqslant 0 \\x(n-1), \text{otherwise} \end{cases}`
 
     Args:
-        n: Scaling factor for the positive part of the input. Default: 1.0.
-        inplace: can optionally do the operation in-place. Default: ``False``
+        n (float, optional): Scaling factor for the positive part of the input. Default: 1.0.
+        inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
-    Attributes:
-        n: Scaling factor for the positive part of the input. Default: 1.0.
-
     Examples:
         >>> m = nn.DELU()
         >>> x = torch.randn(2)
         >>> output = m(x)
 
         >>> m = nn.DELU(inplace=True)
         >>> x = torch.randn(2)
         >>> m(x)
     """
 
-    def __init__(self, n=1.0, inplace=False):
+    def __init__(self, n: float = 1.0, inplace: bool = False):
         super(DELU, self).__init__()
         self.n = torch.nn.Parameter(torch.tensor(n))
         self.inplace = inplace
 
     def forward(self, x) -> Tensor:
         return self._forward_inplace(x) if self.inplace else self._forward(x)
 
@@ -51,35 +48,33 @@
         return x
     
 
 class DReLUs(nn.Module):
     r"""
     Applies the DReLUs activation function:
 
-    :math:`\text{DELU}(x) = \begin{cases} \alpha (e ^ x - 1), x \leqslant 0 \\x, \text{otherwise} \end{cases}`
+    :math:`\text{DReLUs}(x) = \begin{cases} \alpha (e ^ x - 1), x \leqslant 0 \\x, \text{otherwise} \end{cases}`
 
     Args:
-        n: Scaling factor for the positive part of the input. Default: 1.0.
-        inplace: can optionally do the operation in-place. Default: ``False``
+        alpha (float, optional): Scaling factor for the positive part of the input. Default: 1.0.
+        inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
-    Attributes:
-        n: Scaling factor for the positive part of the input. Default: 1.0.
-
     Examples:
         >>> m = nn.DReLUs()
         >>> x = torch.randn(2)
         >>> output = m(x)
     """
     
-    def __init__(self, alpha):
+    def __init__(self, alpha: float = 1.0, inplace: bool = False):
         self.alpha = alpha
+        self.inplace = inplace
         
     def forward(self, x) -> Tensor:
         return self._forward_inplace(x) if self.inplace else self._forward(x)
         
     def _forward(self, x):
         return torch.where(x > 0, x,
                            self.alpha * (torch.exp(x) - 1))
```

### Comparing `torch_activation-0.1.1/torch_activation/glu_family.py` & `torch_activation-0.1.2/torch_activation/glus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,129 +1,129 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch import Tensor
 
 
-class ReGLU(torch.nn.Module):
+class ReGLU(nn.Module):
     r"""
     Applies the GeGLU activation function, defined as:
 
     :math:`\text{GeGLU}(x) = \text{ReLU} (xW + b) \odot (xV + c)`
 
     Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-        size: The size of the last dimension of the input tensor.
+        dim (int, optional): the dimension on which to split the input. Default: -1 
 
     Shape:
-        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
-        - Output: :math:`(*)`
+        - Input: :math:`(\ast_1, N, \ast_2)` where `*` means, any number of additional
+          dimensions
+        - Output: :math:`(\ast_1, M, \ast_2)` where :math:`M=N/2`
 
     Examples::
 
         >>> m = ReGLU(20)
         >>> input = torch.randn(3, 20, 20)
         >>> output = m(input)
 
     """
 
-    def __init__(self, size:int):
+    def __init__(self, dim: int = -1):
         super(ReGLU, self).__init__()
-        self.linear = nn.Linear(size, size*2)
+        self.dim = dim
 
     def forward(self, x) -> Tensor:
-        a, b = self.linear(x).chunk(2, dim=-1)
+        a, b = x.chunk(2, dim=self.dim)
         return a * F.relu(b)
 
 
-class GeGLU(torch.nn.Module):
+class GeGLU(nn.Module):
     r"""
     Applies the GeGLU activation function, defined as:
 
     :math:`\text{GeGLU}(x) = \text{GELU} (xW + b) \odot (xV + c)`
 
     Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-        size: The size of the last dimension of the input tensor.
+        dim (int, optional): the dimension on which to split the input. Default: -1 
 
     Shape:
-        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
-        - Output: :math:`(*)`
+        - Input: :math:`(\ast_1, N, \ast_2)` where `*` means, any number of additional
+          dimensions
+        - Output: :math:`(\ast_1, M, \ast_2)` where :math:`M=N/2`
 
     Examples::
 
         >>> m = GeGLU(20)
         >>> input = torch.randn(3, 20, 20)
         >>> output = m(input)
     """
 
-    def __init__(self, size:int):
+    def __init__(self, dim: int = -1):
         super(GeGLU, self).__init__()
-        self.linear = nn.Linear(size, size*2)
+        self.dim = dim
 
     def forward(self, x) -> Tensor:
-        a, b = self.linear(x).chunk(2, dim=-1)
+        a, b = x.chunk(2, dim=-1)
         return a * F.gelu(b)
 
 
-class SwiGLU(torch.nn.Module):
+class SwiGLU(nn.Module):
     r"""
     Applies the SwiGLU activation function, defined as:
 
     :math:`\sigma(x) =  \text{Swish} (xW + b) \odot (xV + c)`
 
     Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-        size: The size of the last dimension of the input tensor.
+        dim (int, optional): the dimension on which to split the input. Default: -1 
 
     Shape:
-        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
-        - Output: :math:`(*)`
+        - Input: :math:`(\ast_1, N, \ast_2)` where `*` means, any number of additional
+          dimensions
+        - Output: :math:`(\ast_1, M, \ast_2)` where :math:`M=N/2`
 
     Examples::
 
         >>> m = SwiGLU(20)
         >>> input = torch.randn(3, 20, 20)
         >>> output = m(input)
     """
 
-    def __init__(self, size:int):
+    def __init__(self, dim: int = -1):
         super(SwiGLU, self).__init__()
-        self.linear = nn.Linear(size, size*2)
+        self.dim = dim
 
     def forward(self, x) -> Tensor:
-        a, b = self.linear(x).chunk(2, dim=-1)
+        a, b = x.chunk(2, dim=-1)
         return a * F.silu(b)
     
-class SeGLU(torch.nn.Module):
+class SeGLU(nn.Module):
     r"""
     Applies the SeGLU activation function, defined as:
 
     :math:`\text{SeGLU}(x) =  \text{SELU} (xW + b) \odot (xV + c)`
 
     Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-        size: The size of the last dimension of the input tensor.
+        dim (int, optional): the dimension on which to split the input. Default: -1 
 
     Shape:
-        - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
-        - Output: :math:`(*)`
+        - Input: :math:`(\ast_1, N, \ast_2)` where `*` means, any number of additional
+          dimensions
+        - Output: :math:`(\ast_1, M, \ast_2)` where :math:`M=N/2`
 
     Examples::
 
         >>> m = SeGLU(20)
         >>> input = torch.randn(3, 20, 20)
         >>> output = m(input)
     """
 
-    def __init__(self, size:int):
+    def __init__(self, dim: int = -1):
         super(SeGLU, self).__init__()
-        self.linear = nn.Linear(size, size*2)
+        self.dim = dim
 
     def forward(self, x) -> Tensor:
-        a, b = self.linear(x).chunk(2, dim=-1)
+        a, b = x.chunk(2, dim=-1)
         return a * F.selu(b)
 
 if __name__ == "__main__":
     pass
```

### Comparing `torch_activation-0.1.1/torch_activation/lincomb.py` & `torch_activation-0.1.2/torch_activation/lincomb.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from torch import Tensor
+from typing import Iterable
 
 
 class LinComb(nn.Module):
     r"""
     Applies the LinComb activation function:
     
     :math:`\text{LinComb}(x) = \sum_{i=1}^{n} w_i \cdot F_i(x)`
     
     Args:
-        activation: List of activation functions.
+        activations: List of activation functions.
         
     Shape:
         - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
         - Output: :math:`(*)`
 
     Attributes:
-        activations: List containing the activation functions.
         weights: Trainable weights for linear combination.
 
     Examples::
 
         >>> activations = [nn.ReLU(), nn.Sigmoid()]
         >>> m = LinComb(activation_functions)
         >>> input = torch.randn(10)
         >>> output = m(input)
     """
     
-    def __init__(self, activations: list):
+    def __init__(self, activations: Iterable[str]):
         super(LinComb, self).__init__()
         self.activation_functions = nn.ModuleList(activations)
         self.weights = nn.Parameter(torch.Tensor(len(activations)))
 
         self.weights.data.uniform_(-1, 1)
 
     def forward(self, input) -> Tensor:
@@ -46,33 +46,32 @@
 class NormLinComb(nn.Module):
     r"""
     Applies the LinComb activation function:
     
     :math:`\text{NormLinComb}(x) = \frac{\sum_{i=1}^{n} w_i \cdot F_i(x)}{\|\|W\|\|}`
     
     Args:
-        activation: List of activation functions.
+        activations (): List of activation functions.
         
     Shape:
         - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
         - Output: :math:`(*)`
 
     Attributes:
-        activations: List containing the activation functions.
         weights: Trainable weights for linear combination.
 
     Examples::
 
         >>> activations = [nn.ReLU(), nn.Sigmoid()]
         >>> m = NormLinComb(activation_functions)
         >>> input = torch.randn(10)
         >>> output = m(input)
     """
     
-    def __init__(self, activations: list):
+    def __init__(self, activations: Iterable[str]):
         super(LinComb, self).__init__()
         self.activation_functions = nn.ModuleList(activations)
         self.weights = nn.Parameter(torch.Tensor(len(activations)))
 
         self.weights.data.uniform_(-1, 1)
 
     def forward(self, input) -> Tensor:
```

### Comparing `torch_activation-0.1.1/torch_activation/non_linear.py` & `torch_activation-0.1.2/torch_activation/non_linear.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 class CoLU(nn.Module):
     r"""
     Applies the Collapsing Linear Unit activation function:
 
     :math:`\text{CoLU}(x) = \frac{x}{1-x \cdot e^{-(x + e^x)}}`
 
     Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
+        inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
     Examples::
 
@@ -43,37 +43,33 @@
 class ScaledSoftSign(torch.nn.Module):
     r"""
     Applies the ScaledSoftSign activation function:
 
     :math:`\text{ScaledSoftSign}(x) = \frac{\alpha \cdot x}{\beta + \|x\|}`
 
     Args:
-        alpha: The initial value of the alpha parameter.
-        beta: The initial value of the beta parameter.
-        inplace: can optionally do the operation in-place. Default: ``False``
+        alpha (float, optional): The initial value of the alpha parameter.
+        beta (float, optional): The initial value of the beta parameter.
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
-    Attributes:
-        alpha (nn.Parameter): The alpha scaling parameter.
-        beta (nn.Parameter): The beta scaling parameter.
-
     Examples:
         >>> m = ScaledSoftSign(alpha=0.5, beta=1.0)
         >>> x = torch.randn(2, 3)
         >>> output = m(x)
 
         >>> m = ScaledSoftSign(inplace=True)
         >>> x = torch.randn(2, 3)
         >>> m(x)
     """
 
-    def __init__(self, alpha=1.0, beta=1.0):
+    def __init__(self, alpha: float = 1.0, beta: float = 1.0):
+        
         super(ScaledSoftSign, self).__init__()
 
         self.alpha = torch.nn.Parameter(torch.tensor(alpha))
         self.beta = torch.nn.Parameter(torch.tensor(beta))
 
     def forward(self, x) -> Tensor:
         abs_x = x.abs()
```

### Comparing `torch_activation-0.1.1/torch_activation/relu_family.py` & `torch_activation-0.1.2/torch_activation/relus.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,209 +8,203 @@
 class ShiLU(nn.Module):
     r"""
     Applies the ShiLU activation function:
 
     :math:`\text{ShiLU}(x) = \alpha \cdot \text{ReLU}(x) + \beta`
 
     Args:
-        alpha : Scaling factor for the positive part of the input. Default: 1.0.
-        beta : Bias term added to the output. Default: 0.0.
-        inplace: can optionally do the operation in-place. Default: ``False``
+        alpha (float, optional): Scaling factor for the positive part of the input. Default: 1.0.
+        beta (float, optional): Bias term added to the output. Default: 0.0.
+        inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
-        
-    Attributes:
-        alpha : Scaling factor for the positive part of the input. Default: 1.0.
-        beta : Bias term added to the output. Default: 0.0.
 
     .. image:: ../images/activation_images/ShiLU.png
 
     Examples::
-    
-        >>> m = ShiLU(alpha=2.0, beta=1.0)
+
+        >>> m = torch_activation.ShiLU(alpha=2.0, beta=1.0)
         >>> x = torch.randn(2)
         >>> output = m(x)
 
-        >>> m = ShiLU(inplace=True)
+        >>> m = torch_activation.ShiLU(inplace=True)
         >>> x = torch.randn(2, 3, 4)
         >>> m(x)
     """
 
-    def __init__(self, alpha=1.0, beta=0.0, inplace=False):
+    def __init__(self, alpha: float = 1.0, beta: float = 0.0, 
+                 inplace: bool = False):
         super().__init__()
         self.alpha = nn.Parameter(torch.tensor(alpha))
-        self.beta  = nn.Parameter(torch.tensor(beta))
+        self.beta = nn.Parameter(torch.tensor(beta))
         self.inplace = inplace
 
     def forward(self, x) -> Tensor:
         if self.inplace:
             F.relu_(x)
             x.mul_(self.alpha)
             x.add_(self.beta)
             return x
-        else:    
+        else:
             return self.alpha * F.relu(x) + self.beta
-        
+
 
 class CReLU(nn.Module):
     r"""
     Applies the Concatenated Rectified Linear Unit activation function.
 
     :math:`\text{CReLU}(x) = \text{ReLU}(x) \oplus \text{ReLU}(-x)`
 
     Args:
-        dim: Dimension along which to concatenate in the output tensor. Default: 1
-        inplace: can optionally do the operation in-place. Default: ``False``
+        dim (int, optional): Dimension along which to concatenate in the output tensor. Default: 1
+        inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*, C, *)` where :math:`*` means any number of additional dimensions
         - Output: :math:`(*, 2C, *)`
 
     Examples::
 
-        >>> m = nn.CReLU()
+        >>> m = torch_activation.CReLU()
         >>> x = torch.randn(2, 3)
         >>> output = m(x)
-        
-        >>> m = CReLU(inplace=True)
+
+        >>> m = torch_activation.CReLU(inplace=True)
         >>> x = torch.randn(2, 3, 4)
         >>> m(x)
     """
-    
-    
-    def __init__(self, dim=0):
+
+    def __init__(self, dim: int = 0):
         super(CReLU, self).__init__()
         self.dim = dim
 
     def forward(self, x) -> Tensor:
         return F.relu(torch.cat((x, -x), dim=self.dim))
-        
-        
+
+
 class ReLUN(nn.Module):
     r"""Applies the element-wise function:
 
     :math:`\text{ReLUN}(x) = \min(\text{ReLU}(x), n)`
 
     Args:
-        n: Upper bound for the function's output. Default is 1.0.
-        inplace: can optionally do the operation in-place. Default: ``False``
+        n (float, optional): Upper bound for the function's output. Default is 1.0.
+        inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
-        
-    Attributes:
-        n: Upper bound for the function's output. Default is 1.0.
-        
+
     Examples::
 
-        >>> m = nn.ReLUN(n=6.0) # ReLU6
+        >>> m = torch_activation.ReLUN(n=6.0) # ReLU6
         >>> x = torch.randn(2)
         >>> output = m(x)
-        
-        >>> m = nn.ReLUN(inplace=True)
+
+        >>> m = torch_activation.ReLUN(inplace=True)
         >>> x = torch.randn(2)
         >>> m(x)
 
     """
-    def __init__(self, n=1.0, inplace=False):
+
+    def __init__(self, n: float = 1.0, inplace: bool = False):
         super(ReLUN, self).__init__()
         self.n = nn.Parameter(torch.tensor(n))
         self.inplace = inplace
 
     def forward(self, x) -> Tensor:
         if self.inplace:
             x.clamp_max_(self.n.data)
             x.relu_()
             return x
         else:
             return torch.clamp(x, 0, self.n.data)
-        
-        
+
+
 class SquaredReLU(nn.Module):
     r"""
     Applies the element-wise function:
 
     :math:`\text{SquaredReLU}(x) = \text{ReLU}(x)^2`
 
     Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
+        inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
     Examples::
 
-        >>> m = nn.SquaredReLU()
+        >>> m = torch_activation.SquaredReLU()
         >>> x = torch.randn(2)
         >>> output = m(x)
 
-        >>> m = nn.SquaredReLU(inplace=True)
+        >>> m = torch_activation.SquaredReLU(inplace=True)
         >>> x = torch.randn(2)
         >>> m(x)
     """
-    
-    
-    def __init__(self, inplace=False):
+
+    def __init__(self, inplace: bool = False):
         super().__init__()
         self.inplace = inplace
 
     def forward(self, x) -> Tensor:
         if self.inplace:
             return F.relu_(x).pow_(2)
         else:
             return F.relu(x).pow(2)
-        
+
+
 class StarReLU(nn.Module):
     r"""
     Applies the element-wise function:
 
     :math:`\text{StarReLU}(x) = s \cdot \text{ReLU}(x)^2 + b`
 
     Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
-        s: Scaled factor for StarReLU, shared across channel. Default: 0.8944
-        b: Bias term for StarReLU, shared across channel. Default: -0.4472
+        s (float, optional): Scaled factor for StarReLU, shared across channel. Default: 0.8944
+        b (float, optional): Bias term for StarReLU, shared across channel. Default: -0.4472
+        learnable (bool, optional): optionally make ``s`` and ``b`` trainable. Default: ``True``
+        inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
         
     .. image:: ../images/activation_images/SquaredReLU.png
 
     Examples::
 
-        >>> m = nn.StarReLU(s=1.0, b=0.0)
+        >>> m = torch_activation.StarReLU(s=1.0, b=0.0)
         >>> x = torch.randn(3, 384, 384)
         >>> output = m(x)
 
-        >>> m = nn.StarReLU(learnable=True, inplace=True)
+        >>> m = torch_activation.StarReLU(learnable=True, inplace=True)
         >>> x = torch.randn(3, 384, 384)
         >>> m(x)
     """
-    
-    
-    def __init__(self, s=0.8944, b=-0.4472, learnable=True, inplace=False):
+
+    def __init__(self, s: float = 0.8944, b: float = -0.4472, 
+                 learnable: bool = True, inplace: bool = False):
         super().__init__()
         self.inplace = inplace
         if learnable:
             self.s = nn.Parameter(torch.tensor(s))
             self.b = nn.Parameter(torch.tensor(b))
         else:
             self.s = torch.tensor(s)
             self.b = torch.tensor(b)
-        
 
     def forward(self, x) -> Tensor:
         if self.inplace:
             return F.relu_(x).pow_(2) \
                              .mul_(self.s) \
                              .add_(self.b)
         else:
             return self.s * F.relu(x).pow(2) + self.b
-    
-    
+
+
 if __name__ == '__main__':
-    pass
+    pass
```

### Comparing `torch_activation-0.1.1/torch_activation/trig.py` & `torch_activation-0.1.2/torch_activation/trig.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class GCU(nn.Module):
     r"""
     Applies the Growing Cosine Unit activation function:
 
     :math:`\text{GCU}(x) = x \cos (x)`
 
     Args:
-        inplace: can optionally do the operation in-place. Default: ``False``
+        inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
         
     Examples::
 
@@ -27,15 +27,15 @@
         >>> output = m(x)
 
         >>> m = nn.GCU(inplace=True)
         >>> x = torch.randn(2)
         >>> m(x)
     """
 
-    def __init__(self, inplace=False):
+    def __init__(self, inplace: bool = False):
         super(GCU, self).__init__()
         self.inplace = inplace
 
     def forward(self, x) -> Tensor:
         if self.inplace:
             return x.mul_(torch.cos(x))
         else:
@@ -45,38 +45,35 @@
 class CosLU(nn.Module):
     r"""
     Applies the Cosine Linear Unit function:
 
     :math:`\text{CosLU}(x) = (x + \alpha \cdot \cos(\beta x)) \cdot \sigma(x)`
 
     Args:
-        alpha: Scaling factor for the cosine term. Default is 1.0.
-        beta: Frequency factor for the cosine term. Default is 1.0.
-        inplace: can optionally do the operation in-place. Default: ``False``
+        alpha (float, optional): Scaling factor for the cosine term. Default is 1.0.
+        beta (float, optional): Frequency factor for the cosine term. Default is 1.0.
+        inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
-    Attributes:
-        alpha: Scaling factor for the cosine term. Default is 1.0.
-        beta: Frequency factor for the cosine term. Default is 1.0.
-
     Examples::
 
         >>> m = CosLU(alpha=2.0, beta=1.0)
         >>> x = torch.randn(2)
         >>> output = m(x)
 
         >>> m = CosLU(inplace=True)
         >>> x = torch.randn(2, 3, 4)
         >>> m(x) 
     """
 
-    def __init__(self, alpha=1.0, beta=1.0, inplace=False):
+    def __init__(self, alpha: float = 1.0, beta: float = 1.0, 
+                 inplace: bool = False):
         super(CosLU, self).__init__()
         self.alpha = nn.Parameter(torch.tensor(alpha))
         self.beta = nn.Parameter(torch.tensor(beta))
         self.inplace = inplace
 
     def forward(self, x) -> Tensor:
         return self._forward_inplace(x) if self.inplace else self._forward(x)
@@ -97,27 +94,27 @@
 class SinLU(nn.Module):
     r"""
     Applies the Sinu-sigmoidal Linear Unit activation function:
 
     :math:`\text{SinLU}(x) = (x + \alpha \sin (\beta x)) \sigma (x)`
 
     Args:
-        a: Initial value for sine function magnitude. Default: 1.0.
-        b: Initial value for sine function period. Default: 1.0.
+        a (float, optional): Initial value for sine function magnitude. Default: 1.0.
+        b (float, optional): Initial value for sine function period. Default: 1.0.
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
     Examples::
 
         >>> m = nn.SinLU(a=5.0, b=6.0)
         >>> x = torch.randn(2)
         >>> output = m(x)
     """
-    def __init__(self, a=1.0, b=1.0):
+    def __init__(self, a: float = 1.0, b: float = 1.0):
         super(SinLU, self).__init__()
         self.a = nn.Parameter(torch.Tensor([a]))
         self.b = nn.Parameter(torch.Tensor([b]))
 
     def forward(self, x) -> Tensor:
         return (x + self.a * torch.sin(self.b * x)) * torch.sigmoid(x)
```

