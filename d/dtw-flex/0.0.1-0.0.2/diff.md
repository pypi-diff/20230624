# Comparing `tmp/dtw_flex-0.0.1.tar.gz` & `tmp/dtw_flex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtw_flex-0.0.1.tar", last modified: Sat Jun 24 14:38:07 2023, max compression
+gzip compressed data, was "dtw_flex-0.0.2.tar", last modified: Sat Jun 24 16:04:25 2023, max compression
```

## Comparing `dtw_flex-0.0.1.tar` & `dtw_flex-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 14:38:07.236282 dtw_flex-0.0.1/
--rw-rw-rw-   0        0        0    35821 2023-06-23 18:21:03.000000 dtw_flex-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1759 2023-06-24 14:38:07.236282 dtw_flex-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1348 2023-06-24 14:36:46.000000 dtw_flex-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 14:38:07.211488 dtw_flex-0.0.1/dtw_flex/
--rw-rw-rw-   0        0        0       38 2023-06-23 18:21:03.000000 dtw_flex-0.0.1/dtw_flex/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 14:38:07.229292 dtw_flex-0.0.1/dtw_flex/core/
--rw-rw-rw-   0        0        0       39 2023-06-23 18:21:03.000000 dtw_flex-0.0.1/dtw_flex/core/__init__.py
--rw-rw-rw-   0        0        0    56412 2023-06-23 18:21:03.000000 dtw_flex-0.0.1/dtw_flex/core/dtw.py
--rw-rw-rw-   0        0        0      423 2023-06-23 18:21:03.000000 dtw_flex-0.0.1/dtw_flex/core/utils.py
--rw-rw-rw-   0        0        0     6196 2023-06-23 18:21:03.000000 dtw_flex-0.0.1/dtw_flex/core/visual_select.py
-drwxrwxrwx   0        0        0        0 2023-06-24 14:38:07.233299 dtw_flex-0.0.1/dtw_flex/core_cython/
--rw-rw-rw-   0        0        0        0 2023-06-23 18:21:03.000000 dtw_flex-0.0.1/dtw_flex/core_cython/__init__.py
--rw-rw-rw-   0        0        0   492334 2023-06-24 14:38:06.000000 dtw_flex-0.0.1/dtw_flex/core_cython/dtw_cy.c
--rw-rw-rw-   0        0        0     1197 2023-06-23 18:21:03.000000 dtw_flex-0.0.1/dtw_flex/core_cython/test.py
-drwxrwxrwx   0        0        0        0 2023-06-24 14:38:07.219268 dtw_flex-0.0.1/dtw_flex.egg-info/
--rw-rw-rw-   0        0        0     1759 2023-06-24 14:38:07.000000 dtw_flex-0.0.1/dtw_flex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      444 2023-06-24 14:38:07.000000 dtw_flex-0.0.1/dtw_flex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 14:38:07.000000 dtw_flex-0.0.1/dtw_flex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-24 14:38:07.000000 dtw_flex-0.0.1/dtw_flex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-06-24 14:38:07.000000 dtw_flex-0.0.1/dtw_flex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      736 2023-06-24 14:36:44.000000 dtw_flex-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 14:38:07.237270 dtw_flex-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      393 2023-06-24 07:30:27.000000 dtw_flex-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:04:25.602198 dtw_flex-0.0.2/
+-rw-rw-rw-   0        0        0    35821 2023-06-23 18:21:03.000000 dtw_flex-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1888 2023-06-24 16:04:25.602198 dtw_flex-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1477 2023-06-24 15:32:45.000000 dtw_flex-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 16:04:25.578328 dtw_flex-0.0.2/dtw_flex/
+-rw-rw-rw-   0        0        0       38 2023-06-23 18:21:03.000000 dtw_flex-0.0.2/dtw_flex/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:04:25.595077 dtw_flex-0.0.2/dtw_flex/core/
+-rw-rw-rw-   0        0        0       39 2023-06-23 18:21:03.000000 dtw_flex-0.0.2/dtw_flex/core/__init__.py
+-rw-rw-rw-   0        0        0    56412 2023-06-23 18:21:03.000000 dtw_flex-0.0.2/dtw_flex/core/dtw.py
+-rw-rw-rw-   0        0        0      423 2023-06-23 18:21:03.000000 dtw_flex-0.0.2/dtw_flex/core/utils.py
+-rw-rw-rw-   0        0        0     6196 2023-06-23 18:21:03.000000 dtw_flex-0.0.2/dtw_flex/core/visual_select.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:04:25.599439 dtw_flex-0.0.2/dtw_flex/core_cython/
+-rw-rw-rw-   0        0        0        0 2023-06-23 18:21:03.000000 dtw_flex-0.0.2/dtw_flex/core_cython/__init__.py
+-rw-rw-rw-   0        0        0   492334 2023-06-24 16:04:24.000000 dtw_flex-0.0.2/dtw_flex/core_cython/dtw_cy.c
+-rw-rw-rw-   0        0        0     1197 2023-06-23 18:21:03.000000 dtw_flex-0.0.2/dtw_flex/core_cython/test.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:04:25.585210 dtw_flex-0.0.2/dtw_flex.egg-info/
+-rw-rw-rw-   0        0        0     1888 2023-06-24 16:04:25.000000 dtw_flex-0.0.2/dtw_flex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      444 2023-06-24 16:04:25.000000 dtw_flex-0.0.2/dtw_flex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 16:04:25.000000 dtw_flex-0.0.2/dtw_flex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-24 16:04:25.000000 dtw_flex-0.0.2/dtw_flex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-24 16:04:25.000000 dtw_flex-0.0.2/dtw_flex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      736 2023-06-24 16:02:45.000000 dtw_flex-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 16:04:25.602198 dtw_flex-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      393 2023-06-24 07:30:27.000000 dtw_flex-0.0.2/setup.py
```

### Comparing `dtw_flex-0.0.1/LICENSE` & `dtw_flex-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dtw_flex-0.0.1/PKG-INFO` & `dtw_flex-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtw_flex
-Version: 0.0.1
+Version: 0.0.2
 Summary: dynamic time warping with amplitude and offset correction
 Author-email: Alexander Meire <alexander.meire@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/aifm00/dtw_flex
 Keywords: dtw
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -26,17 +26,17 @@
 ```python
 pip install dtw_flex
 ```
 
 ### Usage
 
 Please check the following examples:
-* [basic example](./dtw_flex/examples/example_basic.ipynb)
-* [ECG example](./dtw_flex/examples/example_ECG.ipynb)
-* [example with running window](./dtw_flex/examples/example_roll.ipynb)
+* [basic example](https://github.com/aifm00/dtw_flex/blob/main/dtw_flex/examples/example_basic.ipynb)
+* [ECG example](https://github.com/aifm00/dtw_flex/blob/main/dtw_flex/examples/example_ECG.ipynb)
+* [example with running window](https://github.com/aifm00/dtw_flex/blob/main/dtw_flex/examples/example_roll.ipynb)
 
 ## License
 
 This project is licensed under the GPLv3 License - see the LICENSE file for details
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
```

### Comparing `dtw_flex-0.0.1/README.md` & `dtw_flex-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 ```python
 pip install dtw_flex
 ```
 
 ### Usage
 
 Please check the following examples:
-* [basic example](./dtw_flex/examples/example_basic.ipynb)
-* [ECG example](./dtw_flex/examples/example_ECG.ipynb)
-* [example with running window](./dtw_flex/examples/example_roll.ipynb)
+* [basic example](https://github.com/aifm00/dtw_flex/blob/main/dtw_flex/examples/example_basic.ipynb)
+* [ECG example](https://github.com/aifm00/dtw_flex/blob/main/dtw_flex/examples/example_ECG.ipynb)
+* [example with running window](https://github.com/aifm00/dtw_flex/blob/main/dtw_flex/examples/example_roll.ipynb)
 
 ## License
 
 This project is licensed under the GPLv3 License - see the LICENSE file for details
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
```

### Comparing `dtw_flex-0.0.1/dtw_flex/core/dtw.py` & `dtw_flex-0.0.2/dtw_flex/core/dtw.py`

 * *Files identical despite different names*

### Comparing `dtw_flex-0.0.1/dtw_flex/core/visual_select.py` & `dtw_flex-0.0.2/dtw_flex/core/visual_select.py`

 * *Files identical despite different names*

### Comparing `dtw_flex-0.0.1/dtw_flex/core_cython/dtw_cy.c` & `dtw_flex-0.0.2/dtw_flex/core_cython/dtw_cy.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 /* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-s_vcc8c_\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
-            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-s_vcc8c_\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
-            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-s_vcc8c_\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
-            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-s_vcc8c_\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
-            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-s_vcc8c_\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
+            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-wx6gkpcy\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayobject.h",
+            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-wx6gkpcy\\Lib\\site-packages\\numpy\\core\\include\\numpy\\arrayscalars.h",
+            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-wx6gkpcy\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarrayobject.h",
+            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-wx6gkpcy\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ndarraytypes.h",
+            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-wx6gkpcy\\Lib\\site-packages\\numpy\\core\\include\\numpy\\ufuncobject.h"
         ],
         "include_dirs": [
-            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-s_vcc8c_\\Lib\\site-packages\\numpy\\core\\include"
+            "C:\\Users\\Laika\\AppData\\Local\\Temp\\build-env-wx6gkpcy\\Lib\\site-packages\\numpy\\core\\include"
         ],
         "name": "dtw_flex.core_cython.dtw_cy",
         "sources": [
             "dtw_flex/core_cython/dtw_cy.pyx"
         ]
     },
     "module_name": "dtw_flex.core_cython.dtw_cy"
@@ -1045,177 +1045,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":688
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":689
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":690
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":691
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":695
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":696
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":697
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":698
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":702
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":703
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":712
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":713
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":715
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":716
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":718
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":719
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":721
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":722
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":723
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1242,42 +1242,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":725
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":726
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":727
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":729
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -5977,15 +5977,15 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_weight.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":731
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5994,29 +5994,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":732
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":731
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6027,15 +6027,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":734
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6044,29 +6044,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":735
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":734
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6077,15 +6077,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":737
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6094,29 +6094,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":738
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":737
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6127,15 +6127,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":740
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6144,29 +6144,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":741
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":740
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6177,15 +6177,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":743
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6194,29 +6194,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":744
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":743
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6227,89 +6227,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":746
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":747
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":748
+    /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":747
+    /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":750
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":746
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":925
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -6317,33 +6317,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":926
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":927
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":925
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -6351,96 +6351,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":929
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":930
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":931
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":932
+    /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":931
+    /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":933
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":929
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":937
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6456,15 +6456,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":938
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6472,53 +6472,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":939
+      /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":938
+      /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":940
+    /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":941
+      /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
@@ -6526,30 +6526,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":938
+    /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":937
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6564,15 +6564,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":943
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6588,15 +6588,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":944
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6604,53 +6604,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":945
+      /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":944
+      /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":946
+    /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":947
+      /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
@@ -6658,30 +6658,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":944
+    /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":943
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6696,15 +6696,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":949
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6720,15 +6720,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":950
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6736,53 +6736,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":951
+      /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":950
+      /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":952
+    /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":953
+      /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
@@ -6790,30 +6790,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":950
+    /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":949
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6828,176 +6828,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":963
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":975
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":963
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":978
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":990
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":978
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":993
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":1000
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":993
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":1003
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":1007
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":1003
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":1010
+/* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":1014
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -7102,26 +7102,26 @@
   __pyx_slice_ = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice_);
   __Pyx_GIVEREF(__pyx_slice_);
   __pyx_tuple__2 = PyTuple_Pack(2, __pyx_slice_, __pyx_slice_); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 172, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":941
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":947
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 947, __pyx_L1_error)
@@ -7478,15 +7478,15 @@
  * from cython.parallel import prange
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../AppData/Local/Temp/build-env-s_vcc8c_/Lib/site-packages/numpy/__init__.pxd":1010
+  /* "../../AppData/Local/Temp/build-env-wx6gkpcy/Lib/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `dtw_flex-0.0.1/dtw_flex/core_cython/test.py` & `dtw_flex-0.0.2/dtw_flex/core_cython/test.py`

 * *Files identical despite different names*

### Comparing `dtw_flex-0.0.1/dtw_flex.egg-info/PKG-INFO` & `dtw_flex-0.0.2/dtw_flex.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtw-flex
-Version: 0.0.1
+Version: 0.0.2
 Summary: dynamic time warping with amplitude and offset correction
 Author-email: Alexander Meire <alexander.meire@gmail.com>
 License: GPLv3
 Project-URL: Homepage, https://github.com/aifm00/dtw_flex
 Keywords: dtw
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -26,17 +26,17 @@
 ```python
 pip install dtw_flex
 ```
 
 ### Usage
 
 Please check the following examples:
-* [basic example](./dtw_flex/examples/example_basic.ipynb)
-* [ECG example](./dtw_flex/examples/example_ECG.ipynb)
-* [example with running window](./dtw_flex/examples/example_roll.ipynb)
+* [basic example](https://github.com/aifm00/dtw_flex/blob/main/dtw_flex/examples/example_basic.ipynb)
+* [ECG example](https://github.com/aifm00/dtw_flex/blob/main/dtw_flex/examples/example_ECG.ipynb)
+* [example with running window](https://github.com/aifm00/dtw_flex/blob/main/dtw_flex/examples/example_roll.ipynb)
 
 ## License
 
 This project is licensed under the GPLv3 License - see the LICENSE file for details
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
```

### Comparing `dtw_flex-0.0.1/pyproject.toml` & `dtw_flex-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 65.5.0", "Cython >= 0.29.35", "numpy >= 1.25.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dtw_flex"
-version="0.0.1"
+version="0.0.2"
 authors = [
     {name = "Alexander Meire", email = "alexander.meire@gmail.com"},
 ]
 description = "dynamic time warping with amplitude and offset correction"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["dtw"]
```

