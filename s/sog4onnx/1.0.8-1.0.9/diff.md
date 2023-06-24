# Comparing `tmp/sog4onnx-1.0.8.tar.gz` & `tmp/sog4onnx-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sog4onnx-1.0.8.tar", last modified: Fri Apr 15 11:50:22 2022, max compression
+gzip compressed data, was "sog4onnx-1.0.9.tar", last modified: Tue Apr 26 11:22:31 2022, max compression
```

## Comparing `sog4onnx-1.0.8.tar` & `sog4onnx-1.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 11:50:22.288818 sog4onnx-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-04-15 11:50:15.000000 sog4onnx-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10268 2022-04-15 11:50:22.288818 sog4onnx-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9891 2022-04-15 11:50:15.000000 sog4onnx-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-15 11:50:22.288818 sog4onnx-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-04-15 11:50:15.000000 sog4onnx-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 11:50:22.288818 sog4onnx-1.0.8/sog4onnx/
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-04-15 11:50:15.000000 sog4onnx-1.0.8/sog4onnx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-04-15 11:50:15.000000 sog4onnx-1.0.8/sog4onnx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12603 2022-04-15 11:50:15.000000 sog4onnx-1.0.8/sog4onnx/onnx_operation_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-15 11:50:22.288818 sog4onnx-1.0.8/sog4onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10268 2022-04-15 11:50:22.000000 sog4onnx-1.0.8/sog4onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-04-15 11:50:22.000000 sog4onnx-1.0.8/sog4onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-15 11:50:22.000000 sog4onnx-1.0.8/sog4onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-04-15 11:50:22.000000 sog4onnx-1.0.8/sog4onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-15 11:50:22.000000 sog4onnx-1.0.8/sog4onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 11:22:31.108214 sog4onnx-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-04-26 11:22:24.000000 sog4onnx-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    10610 2022-04-26 11:22:31.108214 sog4onnx-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10233 2022-04-26 11:22:24.000000 sog4onnx-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-26 11:22:31.108214 sog4onnx-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2022-04-26 11:22:24.000000 sog4onnx-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 11:22:31.108214 sog4onnx-1.0.9/sog4onnx/
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-04-26 11:22:24.000000 sog4onnx-1.0.9/sog4onnx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-04-26 11:22:24.000000 sog4onnx-1.0.9/sog4onnx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12888 2022-04-26 11:22:24.000000 sog4onnx-1.0.9/sog4onnx/onnx_operation_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 11:22:31.108214 sog4onnx-1.0.9/sog4onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10610 2022-04-26 11:22:31.000000 sog4onnx-1.0.9/sog4onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-04-26 11:22:31.000000 sog4onnx-1.0.9/sog4onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-26 11:22:31.000000 sog4onnx-1.0.9/sog4onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-04-26 11:22:31.000000 sog4onnx-1.0.9/sog4onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-04-26 11:22:31.000000 sog4onnx-1.0.9/sog4onnx.egg-info/top_level.txt
```

### Comparing `sog4onnx-1.0.8/LICENSE` & `sog4onnx-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sog4onnx-1.0.8/PKG-INFO` & `sog4onnx-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sog4onnx
-Version: 1.0.8
+Version: 1.0.9
 Summary: Simple ONNX operation generator. Simple Operation Generator for ONNX.
 Home-page: https://github.com/PINTO0309/sog4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -55,14 +55,15 @@
 ## 2. CLI Usage
 ```bash
 $ sog4onnx -h
 
 usage: sog4onnx [-h]
   --op_type OP_TYPE
   --opset OPSET
+  --op_name OP_NAME
   [--input_variables NAME TYPE VALUE]
   [--output_variables NAME TYPE VALUE]
   [--attributes NAME DTYPE VALUE]
   [--output_onnx_file_path OUTPUT_ONNX_FILE_PATH]
   [--non_verbose]
 
 optional arguments:
@@ -72,14 +73,17 @@
   --op_type OP_TYPE
         ONNX OP type.
         https://github.com/onnx/onnx/blob/main/docs/Operators.md
 
   --opset OPSET
         ONNX opset number.
 
+  --op_name OP_NAME
+        OP name.
+
   --input_variables NAME DTYPE VALUE
         input_variables can be specified multiple times.
         --input_variables variable_name numpy.dtype shape
         https://github.com/onnx/onnx/blob/main/docs/Operators.md
 
         e.g.
         --input_variables i1 float32 [1,3,5,5] \
@@ -124,14 +128,15 @@
 >>> from sog4onnx import generate
 >>> help(generate)
 Help on function generate in module sog4onnx.onnx_operation_generator:
 
 generate(
   op_type: str,
   opset: int,
+  op_name: str,
   input_variables: dict,
   output_variables: dict,
   attributes: Union[dict, NoneType] = None,
   output_onnx_file_path: Union[str, NoneType] = '',
   non_verbose: Union[bool, NoneType] = False
 ) -> onnx.onnx_ml_pb2.ModelProto
 
@@ -145,14 +150,17 @@
         e.g. "Add", "Div", "Gemm", ...
 
     opset: int
         ONNX opset number.
 
         e.g. 11
 
+    op_name: str
+        OP name.
+
     input_variables: Optional[dict]
         Specify input variables for the OP to be generated.
         See below for the variables that can be specified.
         https://github.com/onnx/onnx/blob/main/docs/Operators.md
         {"input_var_name1": [numpy.dtype, shape], "input_var_name2": [dtype, shape], ...}
 
         e.g.
@@ -207,14 +215,15 @@
 ```
 
 ## 4. CLI Execution
 ```bash
 $ sog4onnx \
 --op_type Gemm \
 --opset 1 \
+--op_name gemm_custom1 \
 --input_variables i1 float32 [1,2,3] \
 --input_variables i2 float32 [1,1] \
 --input_variables i3 int32 [0] \
 --output_variables o1 float32 [1,2,3] \
 --attributes alpha float32 1.0 \
 --attributes beta float32 1.0 \
 --attributes transA int32 0 \
@@ -225,14 +234,15 @@
 ```python
 import numpy as np
 from sog4onnx import generate
 
 single_op_graph = generate(
     op_type = 'Gemm',
     opset = 1,
+    op_name = "gemm_custom1",
     input_variables = {
       "i1": [np.float32, [1,2,3]],
       "i2": [np.float32, [1,1]],
       "i3": [np.int32, [0]],
     },
     output_variables = {
       "o1": [np.float32, [1,2,3]],
@@ -250,14 +260,15 @@
 
 ## 6. Sample
 ### 6-1. opset=1, Gemm
 ```bash
 $ sog4onnx \
 --op_type Gemm \
 --opset 1 \
+--op_name gemm_custom1 \
 --input_variables i1 float32 [1,2,3] \
 --input_variables i2 float32 [1,1] \
 --input_variables i3 int32 [0] \
 --output_variables o1 float32 [1,2,3] \
 --attributes alpha float32 1.0 \
 --attributes beta float32 1.0 \
 --attributes transA int32 0 \
@@ -268,27 +279,29 @@
 ![image](https://user-images.githubusercontent.com/33194443/163018647-a6880370-8772-4af1-9ffe-59820a621c30.png)
 
 ### 6-2. opset=11, Add
 ```bash
 $ sog4onnx \
 --op_type Add \
 --opset 11 \
+--op_name add_custom1 \
 --input_variables i1 float32 [1,2,3] \
 --input_variables i2 float32 [1,2,3] \
 --output_variables o1 float32 [1,2,3] \
 --non_verbose
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163042479-9998ba73-ee26-44ea-bd6b-dcd04539190b.png)
 ![image](https://user-images.githubusercontent.com/33194443/163042529-5dbd1b5f-e8d1-47d0-8a9e-aacd91539c2b.png)
 
 ### 6-3. opset=11, NonMaxSuppression
 ```bash
 $ sog4onnx \
 --op_type NonMaxSuppression \
 --opset 11 \
+--op_name nms_custom1 \
 --input_variables boxes float32 [1,6,4] \
 --input_variables scores float32 [1,1,6] \
 --input_variables max_output_boxes_per_class int64 [1] \
 --input_variables iou_threshold float32 [1] \
 --input_variables score_threshold float32 [1] \
 --output_variables selected_indices int64 [3,3] \
 --attributes center_point_box int64 1
@@ -297,14 +310,15 @@
 ![image](https://user-images.githubusercontent.com/33194443/163291789-59e4e5c8-26f4-4971-ab22-1486093f1be0.png)
 
 ### 6-4. opset=11, Constant
 ```bash
 $ sog4onnx \
 --op_type Constant \
 --opset 11 \
+--op_name const_custom1 \
 --output_variables boxes float32 [1,6,4] \
 --attributes value float32 \
 [[\
 [0.5,0.5,1.0,1.0],\
 [0.5,0.6,1.0,1.0],\
 [0.5,0.4,1.0,1.0],\
 [0.5,10.5,1.0,1.0],\
@@ -320,8 +334,11 @@
 3. https://github.com/NVIDIA/TensorRT/tree/main/tools/onnx-graphsurgeon
 4. https://github.com/PINTO0309/sne4onnx
 5. https://github.com/PINTO0309/snd4onnx
 6. https://github.com/PINTO0309/snc4onnx
 7. https://github.com/PINTO0309/scs4onnx
 8. https://github.com/PINTO0309/PINTO_model_zoo
 
+## 8. Issues
+https://github.com/PINTO0309/simple-onnx-processing-tools/issues
+
```

### Comparing `sog4onnx-1.0.8/README.md` & `sog4onnx-1.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 ## 2. CLI Usage
 ```bash
 $ sog4onnx -h
 
 usage: sog4onnx [-h]
   --op_type OP_TYPE
   --opset OPSET
+  --op_name OP_NAME
   [--input_variables NAME TYPE VALUE]
   [--output_variables NAME TYPE VALUE]
   [--attributes NAME DTYPE VALUE]
   [--output_onnx_file_path OUTPUT_ONNX_FILE_PATH]
   [--non_verbose]
 
 optional arguments:
@@ -58,14 +59,17 @@
   --op_type OP_TYPE
         ONNX OP type.
         https://github.com/onnx/onnx/blob/main/docs/Operators.md
 
   --opset OPSET
         ONNX opset number.
 
+  --op_name OP_NAME
+        OP name.
+
   --input_variables NAME DTYPE VALUE
         input_variables can be specified multiple times.
         --input_variables variable_name numpy.dtype shape
         https://github.com/onnx/onnx/blob/main/docs/Operators.md
 
         e.g.
         --input_variables i1 float32 [1,3,5,5] \
@@ -110,14 +114,15 @@
 >>> from sog4onnx import generate
 >>> help(generate)
 Help on function generate in module sog4onnx.onnx_operation_generator:
 
 generate(
   op_type: str,
   opset: int,
+  op_name: str,
   input_variables: dict,
   output_variables: dict,
   attributes: Union[dict, NoneType] = None,
   output_onnx_file_path: Union[str, NoneType] = '',
   non_verbose: Union[bool, NoneType] = False
 ) -> onnx.onnx_ml_pb2.ModelProto
 
@@ -131,14 +136,17 @@
         e.g. "Add", "Div", "Gemm", ...
 
     opset: int
         ONNX opset number.
 
         e.g. 11
 
+    op_name: str
+        OP name.
+
     input_variables: Optional[dict]
         Specify input variables for the OP to be generated.
         See below for the variables that can be specified.
         https://github.com/onnx/onnx/blob/main/docs/Operators.md
         {"input_var_name1": [numpy.dtype, shape], "input_var_name2": [dtype, shape], ...}
 
         e.g.
@@ -193,14 +201,15 @@
 ```
 
 ## 4. CLI Execution
 ```bash
 $ sog4onnx \
 --op_type Gemm \
 --opset 1 \
+--op_name gemm_custom1 \
 --input_variables i1 float32 [1,2,3] \
 --input_variables i2 float32 [1,1] \
 --input_variables i3 int32 [0] \
 --output_variables o1 float32 [1,2,3] \
 --attributes alpha float32 1.0 \
 --attributes beta float32 1.0 \
 --attributes transA int32 0 \
@@ -211,14 +220,15 @@
 ```python
 import numpy as np
 from sog4onnx import generate
 
 single_op_graph = generate(
     op_type = 'Gemm',
     opset = 1,
+    op_name = "gemm_custom1",
     input_variables = {
       "i1": [np.float32, [1,2,3]],
       "i2": [np.float32, [1,1]],
       "i3": [np.int32, [0]],
     },
     output_variables = {
       "o1": [np.float32, [1,2,3]],
@@ -236,14 +246,15 @@
 
 ## 6. Sample
 ### 6-1. opset=1, Gemm
 ```bash
 $ sog4onnx \
 --op_type Gemm \
 --opset 1 \
+--op_name gemm_custom1 \
 --input_variables i1 float32 [1,2,3] \
 --input_variables i2 float32 [1,1] \
 --input_variables i3 int32 [0] \
 --output_variables o1 float32 [1,2,3] \
 --attributes alpha float32 1.0 \
 --attributes beta float32 1.0 \
 --attributes transA int32 0 \
@@ -254,27 +265,29 @@
 ![image](https://user-images.githubusercontent.com/33194443/163018647-a6880370-8772-4af1-9ffe-59820a621c30.png)
 
 ### 6-2. opset=11, Add
 ```bash
 $ sog4onnx \
 --op_type Add \
 --opset 11 \
+--op_name add_custom1 \
 --input_variables i1 float32 [1,2,3] \
 --input_variables i2 float32 [1,2,3] \
 --output_variables o1 float32 [1,2,3] \
 --non_verbose
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163042479-9998ba73-ee26-44ea-bd6b-dcd04539190b.png)
 ![image](https://user-images.githubusercontent.com/33194443/163042529-5dbd1b5f-e8d1-47d0-8a9e-aacd91539c2b.png)
 
 ### 6-3. opset=11, NonMaxSuppression
 ```bash
 $ sog4onnx \
 --op_type NonMaxSuppression \
 --opset 11 \
+--op_name nms_custom1 \
 --input_variables boxes float32 [1,6,4] \
 --input_variables scores float32 [1,1,6] \
 --input_variables max_output_boxes_per_class int64 [1] \
 --input_variables iou_threshold float32 [1] \
 --input_variables score_threshold float32 [1] \
 --output_variables selected_indices int64 [3,3] \
 --attributes center_point_box int64 1
@@ -283,14 +296,15 @@
 ![image](https://user-images.githubusercontent.com/33194443/163291789-59e4e5c8-26f4-4971-ab22-1486093f1be0.png)
 
 ### 6-4. opset=11, Constant
 ```bash
 $ sog4onnx \
 --op_type Constant \
 --opset 11 \
+--op_name const_custom1 \
 --output_variables boxes float32 [1,6,4] \
 --attributes value float32 \
 [[\
 [0.5,0.5,1.0,1.0],\
 [0.5,0.6,1.0,1.0],\
 [0.5,0.4,1.0,1.0],\
 [0.5,10.5,1.0,1.0],\
@@ -305,7 +319,10 @@
 2. https://docs.nvidia.com/deeplearning/tensorrt/onnx-graphsurgeon/docs/index.html
 3. https://github.com/NVIDIA/TensorRT/tree/main/tools/onnx-graphsurgeon
 4. https://github.com/PINTO0309/sne4onnx
 5. https://github.com/PINTO0309/snd4onnx
 6. https://github.com/PINTO0309/snc4onnx
 7. https://github.com/PINTO0309/scs4onnx
 8. https://github.com/PINTO0309/PINTO_model_zoo
+
+## 8. Issues
+https://github.com/PINTO0309/simple-onnx-processing-tools/issues
```

### Comparing `sog4onnx-1.0.8/setup.py` & `sog4onnx-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sog4onnx-1.0.8/sog4onnx/onnx_operation_generator.py` & `sog4onnx-1.0.9/sog4onnx/onnx_operation_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     np.dtype('int32'): onnx.TensorProto.INT32,
     np.dtype('int64'): onnx.TensorProto.INT64,
 }
 
 def generate(
     op_type: str,
     opset: int,
+    op_name: str,
     input_variables: Optional[dict] = None,
     output_variables: Optional[dict] = None,
     attributes: Optional[dict] = None,
     output_onnx_file_path: Optional[str] = '',
     non_verbose: Optional[bool] = False,
 ) -> onnx.ModelProto:
     """
@@ -79,14 +80,17 @@
         e.g. "Add", "Div", "Gemm", ...\n\
         https://github.com/onnx/onnx/blob/main/docs/Operators.md
 
     opset: int
         ONNX opset number.\n\
         e.g. 11
 
+    op_name: str
+        OP name.
+
     input_variables: Optional[dict]
         Specify input variables for the OP to be generated.\n\
         See below for the variables that can be specified.\n\n\
         {"input_var_name1": [numpy.dtype, shape], "input_var_name2": [dtype, shape], ...}\n\n\
         e.g. input_variables = {"name1": [np.float32, [1,224,224,3]], "name2": [np.bool_, [0]], ...}\n\
         https://github.com/onnx/onnx/blob/main/docs/Operators.md
 
@@ -148,14 +152,15 @@
     # 2. Node Generation
     node = None
     value_info = None
     if op_type not in ['Constant', 'ConstantOfShape']:
         # non constant
         node = gs.Node(
             op=op_type,
+            name=op_name,
             attrs=attributes,
             inputs=input_gs_variables,
             outputs=output_gs_variables
         )
     else:
         # constant
         for attr_name, attr_values in attributes.items():
@@ -172,14 +177,15 @@
                 dtype,
                 attr_values.shape
             )
             node = onnx.helper.make_node(
                 op_type,
                 inputs=[],
                 outputs=[constant_name],
+                name=op_name,
                 value=onnx.helper.make_tensor(
                     name='value',
                     data_type=dtype,
                     dims=attr_values.shape,
                     vals=attr_values,
                 ),
             )
@@ -239,18 +245,25 @@
     )
     parser.add_argument(
         '--opset',
         type=int,
         required=True,
         help='ONNX opset number.'
     )
+    parser.add_argument(
+        '--op_name',
+        type=str,
+        required=True,
+        help='OP name.'
+    )
     """
     python3 onnx_operation_generator.py \
     --op_type Gemm \
     --opset 11 \
+    --op_name gemm_custom1 \
     --input_variables i1 np.float32 [1,2,3] \
     --input_variables i2 np.float32 [1,1] \
     --input_variables i3 np.float32 0 \
     --attributes "{\"alpha\": 1.0, \"beta\": 1.0, \"transA\": 0, \"transB\": 0}"
     """
     parser.add_argument(
         '--input_variables',
@@ -373,14 +386,15 @@
     else:
         output_onnx_file_path = f'{args.op_type}.onnx'
 
     # Generate
     single_op_graph = generate(
         op_type=args.op_type,
         opset=args.opset,
+        op_name=args.op_name,
         input_variables=input_variables_tmp,
         output_variables=output_variables_tmp,
         attributes=attributes_tmp,
         output_onnx_file_path=output_onnx_file_path,
         non_verbose=args.non_verbose,
     )
```

### Comparing `sog4onnx-1.0.8/sog4onnx.egg-info/PKG-INFO` & `sog4onnx-1.0.9/sog4onnx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sog4onnx
-Version: 1.0.8
+Version: 1.0.9
 Summary: Simple ONNX operation generator. Simple Operation Generator for ONNX.
 Home-page: https://github.com/PINTO0309/sog4onnx
 Author: Katsuya Hyodo
 Author-email: rmsdh122@yahoo.co.jp
 License: MIT License
 Platform: linux
 Platform: unix
@@ -55,14 +55,15 @@
 ## 2. CLI Usage
 ```bash
 $ sog4onnx -h
 
 usage: sog4onnx [-h]
   --op_type OP_TYPE
   --opset OPSET
+  --op_name OP_NAME
   [--input_variables NAME TYPE VALUE]
   [--output_variables NAME TYPE VALUE]
   [--attributes NAME DTYPE VALUE]
   [--output_onnx_file_path OUTPUT_ONNX_FILE_PATH]
   [--non_verbose]
 
 optional arguments:
@@ -72,14 +73,17 @@
   --op_type OP_TYPE
         ONNX OP type.
         https://github.com/onnx/onnx/blob/main/docs/Operators.md
 
   --opset OPSET
         ONNX opset number.
 
+  --op_name OP_NAME
+        OP name.
+
   --input_variables NAME DTYPE VALUE
         input_variables can be specified multiple times.
         --input_variables variable_name numpy.dtype shape
         https://github.com/onnx/onnx/blob/main/docs/Operators.md
 
         e.g.
         --input_variables i1 float32 [1,3,5,5] \
@@ -124,14 +128,15 @@
 >>> from sog4onnx import generate
 >>> help(generate)
 Help on function generate in module sog4onnx.onnx_operation_generator:
 
 generate(
   op_type: str,
   opset: int,
+  op_name: str,
   input_variables: dict,
   output_variables: dict,
   attributes: Union[dict, NoneType] = None,
   output_onnx_file_path: Union[str, NoneType] = '',
   non_verbose: Union[bool, NoneType] = False
 ) -> onnx.onnx_ml_pb2.ModelProto
 
@@ -145,14 +150,17 @@
         e.g. "Add", "Div", "Gemm", ...
 
     opset: int
         ONNX opset number.
 
         e.g. 11
 
+    op_name: str
+        OP name.
+
     input_variables: Optional[dict]
         Specify input variables for the OP to be generated.
         See below for the variables that can be specified.
         https://github.com/onnx/onnx/blob/main/docs/Operators.md
         {"input_var_name1": [numpy.dtype, shape], "input_var_name2": [dtype, shape], ...}
 
         e.g.
@@ -207,14 +215,15 @@
 ```
 
 ## 4. CLI Execution
 ```bash
 $ sog4onnx \
 --op_type Gemm \
 --opset 1 \
+--op_name gemm_custom1 \
 --input_variables i1 float32 [1,2,3] \
 --input_variables i2 float32 [1,1] \
 --input_variables i3 int32 [0] \
 --output_variables o1 float32 [1,2,3] \
 --attributes alpha float32 1.0 \
 --attributes beta float32 1.0 \
 --attributes transA int32 0 \
@@ -225,14 +234,15 @@
 ```python
 import numpy as np
 from sog4onnx import generate
 
 single_op_graph = generate(
     op_type = 'Gemm',
     opset = 1,
+    op_name = "gemm_custom1",
     input_variables = {
       "i1": [np.float32, [1,2,3]],
       "i2": [np.float32, [1,1]],
       "i3": [np.int32, [0]],
     },
     output_variables = {
       "o1": [np.float32, [1,2,3]],
@@ -250,14 +260,15 @@
 
 ## 6. Sample
 ### 6-1. opset=1, Gemm
 ```bash
 $ sog4onnx \
 --op_type Gemm \
 --opset 1 \
+--op_name gemm_custom1 \
 --input_variables i1 float32 [1,2,3] \
 --input_variables i2 float32 [1,1] \
 --input_variables i3 int32 [0] \
 --output_variables o1 float32 [1,2,3] \
 --attributes alpha float32 1.0 \
 --attributes beta float32 1.0 \
 --attributes transA int32 0 \
@@ -268,27 +279,29 @@
 ![image](https://user-images.githubusercontent.com/33194443/163018647-a6880370-8772-4af1-9ffe-59820a621c30.png)
 
 ### 6-2. opset=11, Add
 ```bash
 $ sog4onnx \
 --op_type Add \
 --opset 11 \
+--op_name add_custom1 \
 --input_variables i1 float32 [1,2,3] \
 --input_variables i2 float32 [1,2,3] \
 --output_variables o1 float32 [1,2,3] \
 --non_verbose
 ```
 ![image](https://user-images.githubusercontent.com/33194443/163042479-9998ba73-ee26-44ea-bd6b-dcd04539190b.png)
 ![image](https://user-images.githubusercontent.com/33194443/163042529-5dbd1b5f-e8d1-47d0-8a9e-aacd91539c2b.png)
 
 ### 6-3. opset=11, NonMaxSuppression
 ```bash
 $ sog4onnx \
 --op_type NonMaxSuppression \
 --opset 11 \
+--op_name nms_custom1 \
 --input_variables boxes float32 [1,6,4] \
 --input_variables scores float32 [1,1,6] \
 --input_variables max_output_boxes_per_class int64 [1] \
 --input_variables iou_threshold float32 [1] \
 --input_variables score_threshold float32 [1] \
 --output_variables selected_indices int64 [3,3] \
 --attributes center_point_box int64 1
@@ -297,14 +310,15 @@
 ![image](https://user-images.githubusercontent.com/33194443/163291789-59e4e5c8-26f4-4971-ab22-1486093f1be0.png)
 
 ### 6-4. opset=11, Constant
 ```bash
 $ sog4onnx \
 --op_type Constant \
 --opset 11 \
+--op_name const_custom1 \
 --output_variables boxes float32 [1,6,4] \
 --attributes value float32 \
 [[\
 [0.5,0.5,1.0,1.0],\
 [0.5,0.6,1.0,1.0],\
 [0.5,0.4,1.0,1.0],\
 [0.5,10.5,1.0,1.0],\
@@ -320,8 +334,11 @@
 3. https://github.com/NVIDIA/TensorRT/tree/main/tools/onnx-graphsurgeon
 4. https://github.com/PINTO0309/sne4onnx
 5. https://github.com/PINTO0309/snd4onnx
 6. https://github.com/PINTO0309/snc4onnx
 7. https://github.com/PINTO0309/scs4onnx
 8. https://github.com/PINTO0309/PINTO_model_zoo
 
+## 8. Issues
+https://github.com/PINTO0309/simple-onnx-processing-tools/issues
+
```

