# Comparing `tmp/torchlie-0.0.1rc1.tar.gz` & `tmp/torchlie-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlie-0.0.1rc1.tar", last modified: Fri Jun 23 04:49:21 2023, max compression
+gzip compressed data, was "torchlie-0.0.1rc2.tar", last modified: Sat Jun 24 13:20:44 2023, max compression
```

## Comparing `torchlie-0.0.1rc1.tar` & `torchlie-0.0.1rc2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-23 04:49:21.223213 torchlie-0.0.1rc1/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1088 2023-06-23 04:44:04.000000 torchlie-0.0.1rc1/LICENSE
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       43 2023-06-23 04:43:58.000000 torchlie-0.0.1rc1/MANIFEST.in
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      546 2023-06-23 04:49:21.221901 torchlie-0.0.1rc1/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        0 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/README.md
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-06-23 04:49:21.224185 torchlie-0.0.1rc1/setup.cfg
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1199 2023-06-23 03:50:52.000000 torchlie-0.0.1rc1/setup.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-23 04:49:21.176507 torchlie-0.0.1rc1/torchlie/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      582 2023-06-23 04:07:46.000000 torchlie-0.0.1rc1/torchlie/__init__.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-23 04:49:21.217637 torchlie-0.0.1rc1/torchlie/functional/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      289 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/__init__.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1282 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/check_contexts.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      536 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/constants.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    10767 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/lie_group.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    32701 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/se3_impl.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    35989 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/so3_impl.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1259 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/functional/utils.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    20259 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/lie_tensor.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     2262 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/options.py
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     3094 2023-06-23 03:49:29.000000 torchlie-0.0.1rc1/torchlie/types.py
-drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-23 04:49:21.191102 torchlie-0.0.1rc1/torchlie.egg-info/
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      546 2023-06-23 04:49:21.000000 torchlie-0.0.1rc1/torchlie.egg-info/PKG-INFO
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      477 2023-06-23 04:49:21.000000 torchlie-0.0.1rc1/torchlie.egg-info/SOURCES.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-06-23 04:49:21.000000 torchlie-0.0.1rc1/torchlie.egg-info/dependency_links.txt
--rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        9 2023-06-23 04:49:21.000000 torchlie-0.0.1rc1/torchlie.egg-info/top_level.txt
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-24 13:20:44.574214 torchlie-0.0.1rc2/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1088 2023-06-24 02:43:57.000000 torchlie-0.0.1rc2/LICENSE
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       43 2023-06-24 02:43:57.000000 torchlie-0.0.1rc2/MANIFEST.in
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      546 2023-06-24 13:20:44.572811 torchlie-0.0.1rc2/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        0 2023-06-24 02:43:57.000000 torchlie-0.0.1rc2/README.md
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)       38 2023-06-24 13:20:44.575132 torchlie-0.0.1rc2/setup.cfg
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1199 2023-06-24 02:43:57.000000 torchlie-0.0.1rc2/setup.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-24 13:20:44.526805 torchlie-0.0.1rc2/torchlie/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      586 2023-06-24 13:19:58.000000 torchlie-0.0.1rc2/torchlie/__init__.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-24 13:20:44.568364 torchlie-0.0.1rc2/torchlie/functional/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      289 2023-06-24 02:43:57.000000 torchlie-0.0.1rc2/torchlie/functional/__init__.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1282 2023-06-24 02:43:57.000000 torchlie-0.0.1rc2/torchlie/functional/check_contexts.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      536 2023-06-24 13:08:40.000000 torchlie-0.0.1rc2/torchlie/functional/constants.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    10768 2023-06-24 13:08:40.000000 torchlie-0.0.1rc2/torchlie/functional/lie_group.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    32734 2023-06-24 13:11:27.000000 torchlie-0.0.1rc2/torchlie/functional/se3_impl.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    36013 2023-06-24 13:11:42.000000 torchlie-0.0.1rc2/torchlie/functional/so3_impl.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     1260 2023-06-24 13:08:41.000000 torchlie-0.0.1rc2/torchlie/functional/utils.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     2266 2023-06-24 13:10:17.000000 torchlie-0.0.1rc2/torchlie/global_params.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)    20273 2023-06-24 13:08:41.000000 torchlie-0.0.1rc2/torchlie/lie_tensor.py
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)     3118 2023-06-24 13:08:41.000000 torchlie-0.0.1rc2/torchlie/types.py
+drwxrwxr-x   0 lep      (1185300626) lep      (1185300626)        0 2023-06-24 13:20:44.541531 torchlie-0.0.1rc2/torchlie.egg-info/
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      546 2023-06-24 13:20:44.000000 torchlie-0.0.1rc2/torchlie.egg-info/PKG-INFO
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)      483 2023-06-24 13:20:44.000000 torchlie-0.0.1rc2/torchlie.egg-info/SOURCES.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        1 2023-06-24 13:20:44.000000 torchlie-0.0.1rc2/torchlie.egg-info/dependency_links.txt
+-rw-rw-r--   0 lep      (1185300626) lep      (1185300626)        9 2023-06-24 13:20:44.000000 torchlie-0.0.1rc2/torchlie.egg-info/top_level.txt
```

### Comparing `torchlie-0.0.1rc1/LICENSE` & `torchlie-0.0.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1rc1/PKG-INFO` & `torchlie-0.0.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlie
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Torch extension for differentiable Lie groups.
 Home-page: https://github.com/facebookresearch/theseus/lie
 Author: Meta Research
 Keywords: lie groups,differentiable optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

### Comparing `torchlie-0.0.1rc1/setup.py` & `torchlie-0.0.1rc2/setup.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1rc1/torchlie/__init__.py` & `torchlie-0.0.1rc2/torchlie/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-__version__ = "0.0.1.rc1"
+__version__ = "0.0.1.rc2"
 
-from .types import ltype, SE3, SO3
+from .global_params import reset_global_params, set_global_params
 from .lie_tensor import (  # usort: skip
     LieTensor,
     adj,
     as_euclidean,
     as_lietensor,
     cast,
     compose,
@@ -20,8 +20,8 @@
     jtransform_from,
     left_act,
     left_project,
     local,
     log,
     transform_from,
 )
-from .options import reset_global_options, set_global_options
+from .types import SE3, SO3, ltype
```

### Comparing `torchlie-0.0.1rc1/torchlie/functional/check_contexts.py` & `torchlie-0.0.1rc2/torchlie/functional/check_contexts.py`

 * *Files identical despite different names*

### Comparing `torchlie-0.0.1rc1/torchlie/functional/constants.py` & `torchlie-0.0.1rc2/torchlie/functional/constants.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-from typing import Optional, Union
 import math
+from typing import Optional, Union
 
 import torch
 
 TEST_EPS = 5e-7
 EPS = 1e-10
 PI = math.pi
```

### Comparing `torchlie-0.0.1rc1/torchlie/functional/lie_group.py` & `torchlie-0.0.1rc2/torchlie/functional/lie_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 import abc
-from typing import Any, Callable, List, Tuple, Optional, Protocol
+from typing import Any, Callable, List, Optional, Protocol, Tuple
 
 import torch
+
 from .constants import DeviceType
 from .utils import check_jacobians_list
 
 # There are four functions associated with each Lie group operator xxx.
 # ----------------------------------------------------------------------------------
 # _xxx_impl: analytic implementation of the operator, return xxx
 # _jxxx_impl: analytic implementation of the operator jacobian, return jxxx and xxx
```

### Comparing `torchlie-0.0.1rc1/torchlie/functional/se3_impl.py` & `torchlie-0.0.1rc2/torchlie/functional/se3_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+from typing import List, Optional, Tuple, cast
+
 import torch
-from typing import cast, List, Tuple, Optional
 
-from torchlie.options import _TORCHLIE_GLOBAL_OPTIONS as LIE_OPTS
-from . import constants, lie_group, so3_impl as SO3
+from torchlie.global_params import _TORCHLIE_GLOBAL_PARAMS as LIE_PARAMS
+
+from . import constants, lie_group
+from . import so3_impl as SO3
 from .check_contexts import checks_base
 from .utils import get_module, shape_err_msg
 
-
 NAME: str = "SE3"
 DIM: int = 6
 _DIAG_6_IDX = [0, 1, 2, 3, 4, 5]
 
 _module = get_module(__name__)
 
 
@@ -44,15 +46,15 @@
                 tangent_vector.shape,
             )
         )
 
 
 def check_hat_tensor(tensor: torch.Tensor):
     def _impl(t_: torch.Tensor):
-        if t_[..., -1].abs().max() > LIE_OPTS.get_eps("se3", "hat", t_.dtype):
+        if t_[..., -1].abs().max() > LIE_PARAMS.get_eps("se3", "hat", t_.dtype):
             raise ValueError("The last row for hat tensors of SE3 must be zero")
 
         SO3.check_hat_tensor(t_[..., :3, :3])
 
     if tensor.shape[-2:] != (4, 4):
         raise ValueError(
             shape_err_msg("Hat tensors of SE3", "(..., 4, 4)", tensor.shape)
@@ -188,15 +190,15 @@
         sine_by_theta,
         one_minus_cosine_by_theta2,
     ) = SO3._exp_impl_helper(tangent_vector[..., 3:])
 
     # Compute the translation
     tangent_vector_lin = tangent_vector[..., :3].view(*size, 3, 1)
     tangent_vector_ang = tangent_vector[..., 3:].view(*size, 3, 1)
-    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
+    near_zero = theta < LIE_PARAMS.get_eps("so3", "near_zero", tangent_vector.dtype)
     theta3_nz = theta_nz * theta2_nz
     theta_minus_sine_by_theta3_t = torch.where(
         near_zero, 1.0 / 6 - theta2 / 120, (theta - sine) / theta3_nz
     )
     ret[..., 3:] = sine_by_theta * tangent_vector_lin
     ret[..., 3:] += one_minus_cosine_by_theta2 * torch.cross(
         tangent_vector_ang, tangent_vector_lin, dim=-2
@@ -239,15 +241,15 @@
         sine_by_theta,
         one_minus_cosine_by_theta2,
         theta_minus_sine_by_theta3_rot,
     )
     jac[..., 3:, 3:] = jac[..., :3, :3]
 
     # compute translation jacobians
-    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
+    near_zero = theta < LIE_PARAMS.get_eps("so3", "near_zero", tangent_vector.dtype)
     d_one_minus_cosine_by_theta2 = torch.where(
         near_zero,
         constants._NEAR_ZERO_D_ONE_MINUS_COSINE_BY_THETA2,
         (sine_by_theta - 2 * one_minus_cosine_by_theta2) / theta2_nz,
     )
     d_theta_minus_sine_by_theta3 = torch.where(
         near_zero,
@@ -286,15 +288,15 @@
     ret, (
         theta,
         theta2_nz,
         sine_by_theta,
         one_minus_cosine_by_theta2,
         theta_minus_sine_by_theta3_t,
     ) = _exp_impl_helper(tangent_vector)
-    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
+    near_zero = theta < LIE_PARAMS.get_eps("so3", "near_zero", tangent_vector.dtype)
     theta_minus_sine_by_theta3_rot = torch.where(
         near_zero, torch.zeros_like(theta), theta_minus_sine_by_theta3_t
     )
     jac, _ = _jexp_impl_helper(
         tangent_vector,
         ret[..., :3],
         theta,
@@ -353,15 +355,15 @@
     check_group_tensor(group)
     size = get_group_size(group)
 
     # Compute the rotation
     ret_ang, (theta, sine, cosine) = SO3._log_impl_helper(group[..., :3])
 
     # Compute the translation
-    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", group.dtype)
+    near_zero = theta < LIE_PARAMS.get_eps("so3", "near_zero", group.dtype)
     theta2 = theta**2
     sine_theta = sine * theta
     two_cosine_minus_two = 2 * cosine - 2
     two_cosine_minus_two_nz = torch.where(
         near_zero, constants._NON_ZERO, two_cosine_minus_two
     )
 
@@ -410,15 +412,15 @@
     two_cosine_minus_two_nz: torch.Tensor,
     a: torch.Tensor,
     b: torch.Tensor,
 ):
     ret_lin = tangent_vector[..., :3]
     ret_ang = tangent_vector[..., 3:]
     size = get_tangent_vector_size(tangent_vector)
-    d_near_zero = theta < LIE_OPTS.get_eps("so3", "d_near_zero", tangent_vector.dtype)
+    d_near_zero = theta < LIE_PARAMS.get_eps("so3", "d_near_zero", tangent_vector.dtype)
     jac = tangent_vector.new_zeros(*size, 6, 6)
     jac[..., :3, :3], (b_ret_ang,) = SO3._jlog_impl_helper(ret_ang, theta, sine, cosine)
     jac[..., 3:, 3:] = jac[..., :3, :3]
 
     theta_nz = torch.where(d_near_zero, constants._NON_ZERO, theta)
     theta4_nz = theta2_nz**2
     c = torch.where(
```

### Comparing `torchlie-0.0.1rc1/torchlie/functional/so3_impl.py` & `torchlie-0.0.1rc2/torchlie/functional/so3_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+from typing import List, Optional, Tuple, cast
+
 import torch
-from typing import cast, List, Tuple, Optional
 
-from torchlie.options import _TORCHLIE_GLOBAL_OPTIONS as LIE_OPTS
+from torchlie.global_params import _TORCHLIE_GLOBAL_PARAMS as LIE_PARAMS
+
 from . import constants, lie_group
 from .check_contexts import checks_base
 from .utils import (
+    fill_dims,
     get_module,
-    shape_err_msg,
     permute_op_dim,
+    shape_err_msg,
     unpermute_op_dim,
-    fill_dims,
 )
 
-
 NAME: str = "SO3"
 DIM: int = 3
 
 _DIAG_3_IDX = [0, 1, 2]
 
 _module = get_module(__name__)
 
 
 def check_group_tensor(tensor: torch.Tensor):
     def _impl(t_):
-        MATRIX_EPS = LIE_OPTS.get_eps("so3", "matrix", t_.dtype)
+        MATRIX_EPS = LIE_PARAMS.get_eps("so3", "matrix", t_.dtype)
         if t_.dtype != torch.float64:
             t_ = t_.double()
 
         _check = (
             torch.matmul(t_, t_.transpose(-1, -2))
             - torch.eye(3, 3, dtype=t_.dtype, device=t_.device)
         ).abs().max().item() < MATRIX_EPS
@@ -62,15 +63,15 @@
                 tangent_vector.shape,
             )
         )
 
 
 def check_hat_tensor(tensor: torch.Tensor):
     def _impl(t_: torch.Tensor):
-        if (t_.transpose(-1, -2) + t_).abs().max().item() > LIE_OPTS.get_eps(
+        if (t_.transpose(-1, -2) + t_).abs().max().item() > LIE_PARAMS.get_eps(
             "so3", "hat", t_.dtype
         ):
             raise ValueError("Hat tensors of SO3 can only be skew-symmetric.")
 
     if tensor.shape[-2:] != (3, 3):
         raise ValueError(
             shape_err_msg("Hat tensors of SO3", "(..., 3, 3)", tensor.shape)
@@ -102,15 +103,15 @@
         raise ValueError(
             shape_err_msg("Projected tensors of SO3", "(..., 3, 3)", tensor.shape)
         )
 
 
 def check_unit_quaternion(quaternion: torch.Tensor):
     def _impl(t_: torch.Tensor):
-        QUANTERNION_EPS = LIE_OPTS.get_eps("so3", "quat", t_.dtype)
+        QUANTERNION_EPS = LIE_PARAMS.get_eps("so3", "quat", t_.dtype)
 
         if t_.dtype != torch.float64:
             t_ = t_.double()
 
         if (torch.linalg.norm(t_, dim=-1) - 1).abs().max().item() >= QUANTERNION_EPS:
             raise ValueError("Not unit quaternions.")
 
@@ -216,15 +217,15 @@
 # -----------------------------------------------------------------------------
 # Exponential Map
 # -----------------------------------------------------------------------------
 def _exp_impl_helper(tangent_vector: torch.Tensor):
     theta = torch.linalg.norm(tangent_vector, dim=-1, keepdim=True).unsqueeze(-1)
     theta2 = theta**2
     # Compute the approximations when theta ~ 0
-    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
+    near_zero = theta < LIE_PARAMS.get_eps("so3", "near_zero", tangent_vector.dtype)
     theta_nz = torch.where(near_zero, constants._NON_ZERO, theta)
     theta2_nz = torch.where(near_zero, constants._NON_ZERO, theta2)
 
     cosine = torch.where(near_zero, 8 / (4 + theta2) - 1, theta.cos())
     sine = theta.sin()
     sine_by_theta = torch.where(near_zero, 0.5 * cosine + 0.5, sine / theta_nz)
     one_minus_cosine_by_theta2 = torch.where(
@@ -300,15 +301,15 @@
         theta2_nz,
         sine,
         _,
         sine_by_theta,
         one_minus_cosine_by_theta2,
     ) = _exp_impl_helper(tangent_vector)
 
-    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", tangent_vector.dtype)
+    near_zero = theta < LIE_PARAMS.get_eps("so3", "near_zero", tangent_vector.dtype)
     theta3_nz = theta_nz * theta2_nz
     theta_minus_sine_by_theta3 = torch.where(
         near_zero, torch.zeros_like(theta), (theta - sine) / theta3_nz
     )
     jac, _ = _jexp_impl_helper(
         tangent_vector,
         sine_by_theta,
@@ -363,16 +364,16 @@
     sine_axis[..., 0] = 0.5 * (group[..., 2, 1] - group[..., 1, 2])
     sine_axis[..., 1] = 0.5 * (group[..., 0, 2] - group[..., 2, 0])
     sine_axis[..., 2] = 0.5 * (group[..., 1, 0] - group[..., 0, 1])
     cosine = 0.5 * (group.diagonal(dim1=-1, dim2=-2).sum(dim=-1) - 1)
     sine = sine_axis.norm(dim=-1)
     theta = torch.atan2(sine, cosine)
 
-    near_zero = theta < LIE_OPTS.get_eps("so3", "near_zero", group.dtype)
-    near_pi = 1 + cosine <= LIE_OPTS.get_eps("so3", "near_pi", group.dtype)
+    near_zero = theta < LIE_PARAMS.get_eps("so3", "near_zero", group.dtype)
+    near_pi = 1 + cosine <= LIE_PARAMS.get_eps("so3", "near_pi", group.dtype)
     # theta != pi
     near_zero_or_near_pi = torch.logical_or(near_zero, near_pi)
     # Compute the approximation of theta / sin(theta) when theta is near to 0
     sine_nz = torch.where(near_zero_or_near_pi, constants._NON_ZERO, sine)
     scale = torch.where(
         near_zero_or_near_pi,
         1 + sine**2 / 6,
@@ -415,15 +416,15 @@
 def _jlog_impl_helper(
     tangent_vector: torch.Tensor,
     theta: torch.Tensor,
     sine: torch.Tensor,
     cosine: torch.Tensor,
 ):
     size = get_tangent_vector_size(tangent_vector)
-    d_near_zero = theta < LIE_OPTS.get_eps("so3", "d_near_zero", tangent_vector.dtype)
+    d_near_zero = theta < LIE_PARAMS.get_eps("so3", "d_near_zero", tangent_vector.dtype)
     theta2 = theta**2
     sine_theta = sine * theta
     two_cosine_minus_two = 2 * cosine - 2
     two_cosine_minus_two_nz = torch.where(
         d_near_zero, constants._NON_ZERO, two_cosine_minus_two
     )
     theta2_nz = torch.where(d_near_zero, constants._NON_ZERO, theta2)
```

### Comparing `torchlie-0.0.1rc1/torchlie/functional/utils.py` & `torchlie-0.0.1rc2/torchlie/functional/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import List
+
 import torch
 
 
 def check_jacobians_list(jacobians: List[torch.Tensor]):
     if len(jacobians) != 0:
         raise ValueError("jacobians list to be populated must be empty.")
```

### Comparing `torchlie-0.0.1rc1/torchlie/lie_tensor.py` & `torchlie-0.0.1rc2/torchlie/lie_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 # LICENSE file in the root directory of this source tree.
 import threading
 import warnings
 from typing import Any, Callable, List, Optional, Tuple
 from typing import cast as type_cast
 
 import torch
-from torch.utils._pytree import tree_flatten, tree_map_only
 from torch.types import Number
+from torch.utils._pytree import tree_flatten, tree_map_only
 
 from .functional.constants import DeviceType
 from .functional.lie_group import UnaryOperatorOpFnType
 from .types import (
-    ltype as _ltype,
-    Device,
     SE3,
     SO3,
+    Device,
     TensorType,
     _IdentityFnType,
     _JFnReturnType,
     _RandFnType,
 )
+from .types import ltype as _ltype
 
 
 class _LieAsEuclideanContext:
     contexts = threading.local()
 
     @classmethod
     def get_context(cls):
```

### Comparing `torchlie-0.0.1rc1/torchlie/options.py` & `torchlie-0.0.1rc2/torchlie/global_params.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
-from typing import Any, Dict
 from dataclasses import dataclass
+from typing import Any, Dict
 
 import torch
 
 
 def _CHECK_DTYPE_SUPPORTED(dtype):
     if dtype not in [torch.float32, torch.float64]:
         raise ValueError(
             f"Unsupported data type {dtype}. "
             "Theseus only supports 32- and 64-bit tensors."
         )
 
 
 @dataclass
-class _TorchLieOptions:
+class _TorchLieGlobalParams:
     so3_near_pi_eps_float32: float = 0
     so3_near_zero_eps_float32: float = 0
     so3_matrix_eps_float32: float = 0
     so3_quat_eps_float32: float = 0
     so3_hat_eps_float32: float = 0
     se3_hat_eps_float32: float = 0
     so3_near_pi_eps_float64: float = 0
@@ -52,19 +52,19 @@
         self.so3_d_near_zero_eps_float64 = 1e-2
         self.so3_matrix_eps_float64 = 1e-6
         self.so3_quat_eps_float64 = 5e-7
         self.so3_hat_eps_float64 = 5e-7
         self.se3_hat_eps_float64 = 5e-7
 
 
-_TORCHLIE_GLOBAL_OPTIONS = _TorchLieOptions()
+_TORCHLIE_GLOBAL_PARAMS = _TorchLieGlobalParams()
 
 
-def set_global_options(options: Dict[str, Any]) -> None:
+def set_global_params(options: Dict[str, Any]) -> None:
     for k, v in options.items():
-        if not hasattr(_TORCHLIE_GLOBAL_OPTIONS, k):
+        if not hasattr(_TORCHLIE_GLOBAL_PARAMS, k):
             raise ValueError(f"{k} is not a valid global option for torchlie.")
-        setattr(_TORCHLIE_GLOBAL_OPTIONS, k, v)
+        setattr(_TORCHLIE_GLOBAL_PARAMS, k, v)
 
 
-def reset_global_options() -> None:
-    _TORCHLIE_GLOBAL_OPTIONS.reset()
+def reset_global_params() -> None:
+    _TORCHLIE_GLOBAL_PARAMS.reset()
```

### Comparing `torchlie-0.0.1rc1/torchlie/types.py` & `torchlie-0.0.1rc2/torchlie/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 from enum import Enum
-from typing import Any, Callable, List, Optional, Protocol, Tuple, Union, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any, Callable, List, Optional, Protocol, Tuple, Union
 
 import torch
-from .functional import SE3 as _se3_impl, SO3 as _so3_impl
+
+from .functional import SE3 as _se3_impl
+from .functional import SO3 as _so3_impl
 from .functional.constants import DeviceType
 from .functional.lie_group import LieGroupFns
 
 if TYPE_CHECKING:
     from .lie_tensor import LieTensor, _LieTensorBase
```

### Comparing `torchlie-0.0.1rc1/torchlie.egg-info/PKG-INFO` & `torchlie-0.0.1rc2/torchlie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlie
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Torch extension for differentiable Lie groups.
 Home-page: https://github.com/facebookresearch/theseus/lie
 Author: Meta Research
 Keywords: lie groups,differentiable optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
```

