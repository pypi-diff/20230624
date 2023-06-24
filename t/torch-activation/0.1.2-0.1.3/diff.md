# Comparing `tmp/torch_activation-0.1.2.tar.gz` & `tmp/torch_activation-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_activation-0.1.2.tar", max compression
+gzip compressed data, was "torch_activation-0.1.3.tar", max compression
```

## Comparing `torch_activation-0.1.2.tar` & `torch_activation-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1086 2023-06-16 00:29:16.944161 torch_activation-0.1.2/LICENSE
--rw-r--r--   0        0        0      466 2023-06-23 22:31:18.215046 torch_activation-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2041 2023-06-23 22:30:32.455234 torch_activation-0.1.2/README.md
--rw-r--r--   0        0        0      556 2023-06-23 22:31:19.225348 torch_activation-0.1.2/torch_activation/__init__.py
--rw-r--r--   0        0        0     2742 2023-06-23 22:30:32.476477 torch_activation-0.1.2/torch_activation/composite.py
--rw-r--r--   0        0        0     3331 2023-06-22 12:04:21.368192 torch_activation-0.1.2/torch_activation/glus.py
--rw-r--r--   0        0        0     2541 2023-06-22 12:04:21.370191 torch_activation-0.1.2/torch_activation/lincomb.py
--rw-r--r--   0        0        0     2282 2023-06-22 12:04:21.371197 torch_activation-0.1.2/torch_activation/non_linear.py
--rw-r--r--   0        0        0     6320 2023-06-22 12:04:21.372196 torch_activation-0.1.2/torch_activation/relus.py
--rw-r--r--   0        0        0     3546 2023-06-22 12:04:21.373204 torch_activation-0.1.2/torch_activation/trig.py
--rw-r--r--   0        0        0     4601 2023-06-23 22:30:32.478000 torch_activation-0.1.2/torch_activation/utils.py
--rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 torch_activation-0.1.2/setup.py
--rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 torch_activation-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-06-16 00:29:16.944161 torch_activation-0.1.3/LICENSE
+-rw-r--r--   0        0        0      466 2023-06-24 06:40:34.720551 torch_activation-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2041 2023-06-23 22:30:32.455234 torch_activation-0.1.3/README.md
+-rw-r--r--   0        0        0      552 2023-06-24 06:40:35.941443 torch_activation-0.1.3/torch_activation/__init__.py
+-rw-r--r--   0        0        0     2859 2023-06-24 05:41:13.351285 torch_activation-0.1.3/torch_activation/curves.py
+-rw-r--r--   0        0        0     3763 2023-06-24 06:23:42.258780 torch_activation-0.1.3/torch_activation/glus.py
+-rw-r--r--   0        0        0     2638 2023-06-24 06:20:26.237034 torch_activation-0.1.3/torch_activation/lincomb.py
+-rw-r--r--   0        0        0     3035 2023-06-24 06:27:50.261452 torch_activation-0.1.3/torch_activation/piece_wise.py
+-rw-r--r--   0        0        0     6332 2023-06-24 06:40:08.391181 torch_activation-0.1.3/torch_activation/relus.py
+-rw-r--r--   0        0        0     4356 2023-06-24 06:14:38.547478 torch_activation-0.1.3/torch_activation/trig.py
+-rw-r--r--   0        0        0     4601 2023-06-23 22:30:32.478000 torch_activation-0.1.3/torch_activation/utils.py
+-rw-r--r--   0        0        0     2728 1970-01-01 00:00:00.000000 torch_activation-0.1.3/setup.py
+-rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 torch_activation-0.1.3/PKG-INFO
```

### Comparing `torch_activation-0.1.2/LICENSE` & `torch_activation-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_activation-0.1.2/README.md` & `torch_activation-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `torch_activation-0.1.2/torch_activation/__init__.py` & `torch_activation-0.1.3/torch_activation/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from .composite import DELU, DReLUs
+from .piece_wise import DELU
 from .trig import CosLU, GCU, SinLU
 from .lincomb import LinComb, NormLinComb
-from .non_linear import CoLU, ScaledSoftSign
+from .curves import CoLU, ScaledSoftSign, Phish
 from .glus import ReGLU, GeGLU, SeGLU, SwiGLU
 from .relus import ShiLU, CReLU, ReLUN, SquaredReLU, StarReLU
 
 
 __all__ = ["ShiLU", "DELU", "CReLU", "GCU",
            "CosLU", "CoLU", "ReLUN",
            "SquaredReLU", "ScaledSoftSign",
            "ReGLU", "GeGLU", "SeGLU", "SwiGLU"
            "LinComb", "NormLinComb", "SinLU"
            "DReLUs", "StarReLU"]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

### Comparing `torch_activation-0.1.2/torch_activation/composite.py` & `torch_activation-0.1.3/torch_activation/piece_wise.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 class DELU(nn.Module):
     r"""
     Applies the DELU activation function:
 
     :math:`\text{DELU}(x) = \begin{cases} \text{SiLU}(x), x \leqslant 0 \\x(n-1), \text{otherwise} \end{cases}`
 
+    The DELU activation function is defined by combining the SiLU activation function and a modified ReLU-like function. 
+    It provides a smooth output near zero and a buffer region to the left of zero, with the "n" parameter controlling the slope of the linear part of the function.
+    
     Args:
         n (float, optional): Scaling factor for the positive part of the input. Default: 1.0.
         inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
@@ -43,17 +46,17 @@
 
     def _forward_inplace(self, x):
         x[x <= 0] = F.silu(x[x <= 0])
         x[x > 0] = (self.n + 0.5) * x[x > 0] + \
             torch.abs(torch.exp(-x[x > 0]) - 1)
         return x
     
-
+"""
 class DReLUs(nn.Module):
-    r"""
+    
     Applies the DReLUs activation function:
 
     :math:`\text{DReLUs}(x) = \begin{cases} \alpha (e ^ x - 1), x \leqslant 0 \\x, \text{otherwise} \end{cases}`
 
     Args:
         alpha (float, optional): Scaling factor for the positive part of the input. Default: 1.0.
         inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
@@ -62,15 +65,15 @@
         - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
         - Output: :math:`(*)`, same shape as the input.
 
     Examples:
         >>> m = nn.DReLUs()
         >>> x = torch.randn(2)
         >>> output = m(x)
-    """
+    
     
     def __init__(self, alpha: float = 1.0, inplace: bool = False):
         self.alpha = alpha
         self.inplace = inplace
         
     def forward(self, x) -> Tensor:
         return self._forward_inplace(x) if self.inplace else self._forward(x)
@@ -78,8 +81,8 @@
     def _forward(self, x):
         return torch.where(x > 0, x,
                            self.alpha * (torch.exp(x) - 1))
         
     def _forward_inplace(self, x):
         x[x <= 0] = (torch.exp(x[x <= 0]) - 1) * self.alpha
         return x
-        
+ """
```

### Comparing `torch_activation-0.1.2/torch_activation/glus.py` & `torch_activation-0.1.3/torch_activation/glus.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 class ReGLU(nn.Module):
     r"""
     Applies the GeGLU activation function, defined as:
 
     :math:`\text{GeGLU}(x) = \text{ReLU} (xW + b) \odot (xV + c)`
 
+    A GLU variation with the function applied to the first half of input is ReLU instead of sigmoid.
+    
     Args:
         dim (int, optional): the dimension on which to split the input. Default: -1 
 
     Shape:
         - Input: :math:`(\ast_1, N, \ast_2)` where `*` means, any number of additional
           dimensions
         - Output: :math:`(\ast_1, M, \ast_2)` where :math:`M=N/2`
@@ -38,14 +40,16 @@
 
 class GeGLU(nn.Module):
     r"""
     Applies the GeGLU activation function, defined as:
 
     :math:`\text{GeGLU}(x) = \text{GELU} (xW + b) \odot (xV + c)`
 
+    A GLU variation with the function applied to the first half of input is GELU instead of sigmoid.
+
     Args:
         dim (int, optional): the dimension on which to split the input. Default: -1 
 
     Shape:
         - Input: :math:`(\ast_1, N, \ast_2)` where `*` means, any number of additional
           dimensions
         - Output: :math:`(\ast_1, M, \ast_2)` where :math:`M=N/2`
@@ -68,14 +72,16 @@
 
 class SwiGLU(nn.Module):
     r"""
     Applies the SwiGLU activation function, defined as:
 
     :math:`\sigma(x) =  \text{Swish} (xW + b) \odot (xV + c)`
 
+    A GLU variation with the function applied to the first half of input is Swish (SiLU) instead of sigmoid.
+    
     Args:
         dim (int, optional): the dimension on which to split the input. Default: -1 
 
     Shape:
         - Input: :math:`(\ast_1, N, \ast_2)` where `*` means, any number of additional
           dimensions
         - Output: :math:`(\ast_1, M, \ast_2)` where :math:`M=N/2`
@@ -97,14 +103,16 @@
     
 class SeGLU(nn.Module):
     r"""
     Applies the SeGLU activation function, defined as:
 
     :math:`\text{SeGLU}(x) =  \text{SELU} (xW + b) \odot (xV + c)`
 
+    A GLU variation with the function applied to the first half of input is SELU instead of sigmoid.
+
     Args:
         dim (int, optional): the dimension on which to split the input. Default: -1 
 
     Shape:
         - Input: :math:`(\ast_1, N, \ast_2)` where `*` means, any number of additional
           dimensions
         - Output: :math:`(\ast_1, M, \ast_2)` where :math:`M=N/2`
```

### Comparing `torch_activation-0.1.2/torch_activation/lincomb.py` & `torch_activation-0.1.3/torch_activation/lincomb.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 class LinComb(nn.Module):
     r"""
     Applies the LinComb activation function:
     
     :math:`\text{LinComb}(x) = \sum_{i=1}^{n} w_i \cdot F_i(x)`
     
+    LinComb is an analog of linear combination of a set of activation functions.
+    Thus, is more flexible and adaptable to the data in exchange for speed.
+    
     Args:
         activations: List of activation functions.
         
     Shape:
         - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
         - Output: :math:`(*)`
 
-    Attributes:
-        weights: Trainable weights for linear combination.
-
     Examples::
 
         >>> activations = [nn.ReLU(), nn.Sigmoid()]
         >>> m = LinComb(activation_functions)
         >>> input = torch.randn(10)
         >>> output = m(input)
     """
@@ -45,24 +45,23 @@
 
 class NormLinComb(nn.Module):
     r"""
     Applies the LinComb activation function:
     
     :math:`\text{NormLinComb}(x) = \frac{\sum_{i=1}^{n} w_i \cdot F_i(x)}{\|\|W\|\|}`
     
+    A version of `LinComb` with normalized linear combination using weight's norm.
+    
     Args:
         activations (): List of activation functions.
         
     Shape:
         - Input: :math:`(*)` where :math:`*` means any number of additional dimensions.
         - Output: :math:`(*)`
 
-    Attributes:
-        weights: Trainable weights for linear combination.
-
     Examples::
 
         >>> activations = [nn.ReLU(), nn.Sigmoid()]
         >>> m = NormLinComb(activation_functions)
         >>> input = torch.randn(10)
         >>> output = m(input)
     """
```

### Comparing `torch_activation-0.1.2/torch_activation/non_linear.py` & `torch_activation-0.1.3/torch_activation/curves.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,11 +73,35 @@
 
     def forward(self, x) -> Tensor:
         abs_x = x.abs()
         alpha_x = self.alpha * x
         denom = self.beta + abs_x
         result = alpha_x / denom
         return result
+    
+
+class Phish(torch.nn.Module):
+    r"""
+    Applies the Phish activation function:
+
+    :math:`\text{Phish}(x) = x \odot \tanh (\text{GELU} (x))`
+
+    Shape:
+        - Input: :math:`(*)`, where :math:`*` means any number of dimensions.
+        - Output: :math:`(*)`, same shape as the input.
+
+    Examples:
+        >>> m = Phish()
+        >>> x = torch.randn(2, 3)
+        >>> output = m(x)
+    """
+
+    def __init__(self):
+        super(Phish, self).__init__()
+
+    def forward(self, x) -> Tensor:
+        x *= nn.Tanh(F.gelu(x))
+        return x
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `torch_activation-0.1.2/torch_activation/relus.py` & `torch_activation-0.1.3/torch_activation/relus.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 
 class ShiLU(nn.Module):
     r"""
     Applies the ShiLU activation function:
 
     :math:`\text{ShiLU}(x) = \alpha \cdot \text{ReLU}(x) + \beta`
+    
+    
 
     Args:
         alpha (float, optional): Scaling factor for the positive part of the input. Default: 1.0.
         beta (float, optional): Bias term added to the output. Default: 0.0.
         inplace (bool, optional): can optionally do the operation in-place. Default: ``False``
 
     Shape:
```

### Comparing `torch_activation-0.1.2/torch_activation/utils.py` & `torch_activation-0.1.3/torch_activation/utils.py`

 * *Files identical despite different names*

### Comparing `torch_activation-0.1.2/setup.py` & `torch_activation-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=1.0.0']
 
 setup_kwargs = {
     'name': 'torch-activation',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'A library of new activation function implement in PyTorch to save time in experiment and have fun',
     'long_description': "# PyTorch Activations\n\nPyTorch Activations is a collection of activation functions for the PyTorch library. This project aims to provide an easy-to-use solution for experimenting with different activation functions or simply adding variety to your models.\n\n\n## Installation\n\nYou can install PyTorch Activations using pip:\n\n```bash\n$ pip install torch-activation\n```\n\n## Usage\n\nTo use the activation functions, import them from torch_activation. Here's an example:\n\n```python\nimport torch_activation as tac\n\nm = tac.ShiLU(inplace=True)\nx = torch.rand(16, 3, 384, 384)\nm(x)\n```\n\nOr in `nn.Sequential`:\n\n```python\nimport torch\nimport torch.nn as nn\nimport torch_activation as tac\n\nclass Net(nn.Module):\n    def __init__(self):\n        super(Net, self).__init__()\n        self.net = nn.Sequential(\n            nn.Conv2d(64, 32, 2),\n            tac.DELU(),\n            nn.ConvTranspose2d(32, 64, 2),\n            tac.ReLU(inplace=True),\n        )\n\n    def forward(self, x):\n        return self.net(x)\n```\n\nActivation functions can be imported directly from the package, such as `torch_activation.CoLU`, or from submodules, such as `torch_activation.non_linear.CoLU`.\n\nFor a comprehensive list of available functions, please refer to the [LIST_OF_FUNCTION](LIST_OF_FUNCTION.md) file.\n\nTo learn more about usage, please refer to [Documentation](https://torch-activation.readthedocs.io)\n\nWe hope you find PyTorch Activations useful for your experimentation and model development. Enjoy exploring different activation functions!\n\n## Contact\n\nAlan Huynh - [LinkedIn](https://www.linkedin.com/in/alan-huynh-64b357194/) - [hdmquan@outlook.com](mailto:hdmquan@outlook.com)\n\nProject Link: [https://github.com/alan191006/torch_activation](https://github.com/alan191006/torch_activation)\n\nDocumentation Link: [https://torch-activation.readthedocs.io](https://torch-activation.readthedocs.io)\n\nPyPI Link: [https://pypi.org/project/torch-activation/](https://pypi.org/project/torch-activation/)\n\n",
     'author': 'Alan Huynh',
     'author_email': 'hdmquan@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `torch_activation-0.1.2/PKG-INFO` & `torch_activation-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-activation
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library of new activation function implement in PyTorch to save time in experiment and have fun
 License: MIT
 Author: Alan Huynh
 Author-email: hdmquan@outlook.com
 Requires-Python: >=3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

