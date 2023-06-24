# Comparing `tmp/entityshape-0.0.1.tar.gz` & `tmp/entityshape-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entityshape-0.0.1.tar", max compression
+gzip compressed data, was "entityshape-0.0.2.tar", max compression
```

## Comparing `entityshape-0.0.1.tar` & `entityshape-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2023-06-23 08:56:36.556587 entityshape-0.0.1/LICENSE
--rw-r--r--   0        0        0     2558 2023-06-23 15:50:04.508322 entityshape-0.0.1/README.md
--rw-r--r--   0        0        0     2134 2023-06-23 15:26:04.636468 entityshape-0.0.1/entityshape/__init__.py
--rw-r--r--   0        0        0      514 2023-06-23 15:26:04.636468 entityshape-0.0.1/entityshape/enums.py
--rw-r--r--   0        0        0      167 2023-06-23 15:26:04.636468 entityshape-0.0.1/entityshape/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-23 15:26:04.636468 entityshape-0.0.1/entityshape/models/__init__.py
--rw-r--r--   0        0        0      185 2023-06-22 19:34:42.343203 entityshape-0.0.1/entityshape/models/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    14398 2023-06-23 14:20:32.369313 entityshape-0.0.1/entityshape/models/__pycache__/compareshape.cpython-311.pyc
--rw-r--r--   0        0        0     1724 2023-06-23 12:36:47.097067 entityshape-0.0.1/entityshape/models/__pycache__/conditions.cpython-311.pyc
--rw-r--r--   0        0        0      812 2023-06-23 14:18:07.589525 entityshape-0.0.1/entityshape/models/__pycache__/property_value.cpython-311.pyc
--rw-r--r--   0        0        0     2504 2023-06-23 12:36:00.409117 entityshape-0.0.1/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc
--rw-r--r--   0        0        0     9488 2023-06-23 14:18:07.586192 entityshape-0.0.1/entityshape/models/__pycache__/result.cpython-311.pyc
--rw-r--r--   0        0        0    17190 2023-06-23 14:18:07.596192 entityshape-0.0.1/entityshape/models/__pycache__/shape.cpython-311.pyc
--rw-r--r--   0        0        0     6532 2023-06-23 12:36:00.409117 entityshape-0.0.1/entityshape/models/__pycache__/shape_claim.cpython-311.pyc
--rw-r--r--   0        0        0      823 2023-06-22 19:38:04.854916 entityshape-0.0.1/entityshape/models/__pycache__/statement_value.cpython-311.pyc
--rw-r--r--   0        0        0    12458 2023-06-23 15:26:04.636468 entityshape-0.0.1/entityshape/models/compareshape.py
--rw-r--r--   0        0        0      245 2023-06-23 15:26:04.636468 entityshape-0.0.1/entityshape/models/property_value.py
--rw-r--r--   0        0        0     5616 2023-06-23 15:26:04.636468 entityshape-0.0.1/entityshape/models/result.py
--rw-r--r--   0        0        0    14070 2023-06-23 15:26:04.636468 entityshape-0.0.1/entityshape/models/shape.py
--rw-r--r--   0        0        0      252 2023-06-23 15:26:04.636468 entityshape-0.0.1/entityshape/models/statement_value.py
--rw-r--r--   0        0        0     3154 2023-06-23 15:26:04.639801 entityshape-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3408 1970-01-01 00:00:00.000000 entityshape-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-23 08:56:36.556587 entityshape-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2865 2023-06-24 09:13:25.089278 entityshape-0.0.2/README.md
+-rw-r--r--   0        0        0     2208 2023-06-24 12:40:28.882874 entityshape-0.0.2/entityshape/__init__.py
+-rw-r--r--   0        0        0      538 2023-06-24 12:30:09.051783 entityshape-0.0.2/entityshape/enums.py
+-rw-r--r--   0        0        0      167 2023-06-23 15:26:04.636468 entityshape-0.0.2/entityshape/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-23 15:26:04.636468 entityshape-0.0.2/entityshape/models/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-24 12:27:51.347797 entityshape-0.0.2/entityshape/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    14398 2023-06-24 12:27:51.351131 entityshape-0.0.2/entityshape/models/__pycache__/compareshape.cpython-311.pyc
+-rw-r--r--   0        0        0     1724 2023-06-23 12:36:47.097067 entityshape-0.0.2/entityshape/models/__pycache__/conditions.cpython-311.pyc
+-rw-r--r--   0        0        0      812 2023-06-24 12:27:51.451131 entityshape-0.0.2/entityshape/models/__pycache__/property_value.cpython-311.pyc
+-rw-r--r--   0        0        0     2504 2023-06-23 12:36:00.409117 entityshape-0.0.2/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc
+-rw-r--r--   0        0        0     9989 2023-06-24 12:46:17.549232 entityshape-0.0.2/entityshape/models/__pycache__/result.cpython-311.pyc
+-rw-r--r--   0        0        0    17190 2023-06-24 12:27:51.461131 entityshape-0.0.2/entityshape/models/__pycache__/shape.cpython-311.pyc
+-rw-r--r--   0        0        0     6532 2023-06-23 12:36:00.409117 entityshape-0.0.2/entityshape/models/__pycache__/shape_claim.cpython-311.pyc
+-rw-r--r--   0        0        0      967 2023-06-24 12:43:06.050877 entityshape-0.0.2/entityshape/models/__pycache__/statement_value.cpython-311.pyc
+-rw-r--r--   0        0        0    12458 2023-06-23 15:26:04.636468 entityshape-0.0.2/entityshape/models/compareshape.py
+-rw-r--r--   0        0        0      245 2023-06-23 15:26:04.636468 entityshape-0.0.2/entityshape/models/property_value.py
+-rw-r--r--   0        0        0     5981 2023-06-24 12:46:17.125895 entityshape-0.0.2/entityshape/models/result.py
+-rw-r--r--   0        0        0    14070 2023-06-23 15:26:04.636468 entityshape-0.0.2/entityshape/models/shape.py
+-rw-r--r--   0        0        0      377 2023-06-24 12:41:01.799816 entityshape-0.0.2/entityshape/models/statement_value.py
+-rw-r--r--   0        0        0     3138 2023-06-24 12:54:46.053903 entityshape-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 entityshape-0.0.2/PKG-INFO
```

### Comparing `entityshape-0.0.1/LICENSE` & `entityshape-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.1/README.md` & `entityshape-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 Based on https://github.com/Teester/entityshape by Mark Tully 
 and https://github.com/dpriskorn/PyEntityshape by Dennis Priskorn
 
 # Features
 * compare a given wikidata item with an entityschema and dig into missing properties, too many statement, etc.
 * determine whether an item is valid according to a certain schema or not
 
+# Limitations
+The shape and compareshape classes currently only support:
+* cardinality (too many or not enough values)
+* whether the property is allowed or not
+* whether the value of a statement on a given property is correct/incorrect
+
+It is still a bit unclear if and how the qualifier validation works.
+
 # Installation
 Get it from pypi
 
 `$ pip install pyentityshape`
 
 # Usage
 Example:
```

### Comparing `entityshape-0.0.1/entityshape/__init__.py` & `entityshape-0.0.2/entityshape/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     qid = ""  # item
     eid = ""  # entityshape
     lang = ""  # language
     result: Result = Result()
     eid_regex = re.compile(r"E\d+")
     qid_regex = re.compile(r"Q\d+")
+    compare_shape_result: dict = {}
 
     def __check__(self):
         if not self.lang:
             raise LangError("We only support 2 and 3 letter language codes")
         if not self.eid:
             raise EidError("We need an entityshape EID")
         if not re.match(self.eid_regex, self.eid):
@@ -37,20 +38,20 @@
         """This method checks if we got the 3 parameters we need and
         gets the results and return them"""
         self.__check__()
         shape: Shape = Shape(self.eid, self.lang)
         comparison: CompareShape = CompareShape(
             shape.get_schema_shape(), self.qid, self.lang
         )
-        result: dict = {
+        self.compare_shape_result: dict = {
             "general": comparison.get_general(),
             "properties": comparison.get_properties(),
             "statements": comparison.get_statements(),
         }
-        self.result = Result(**result)
+        self.result = Result(**self.compare_shape_result)
         self.result.analyze()
         # print(self.result)
         return self.result
 
     # def check_lang(self):
     #     if not self.lang or 4 > len(self.lang) > 1:
     #         raise LangError("We only support 2 and 3 letter language codes")
```

### Comparing `entityshape-0.0.1/entityshape/enums.py` & `entityshape-0.0.2/entityshape/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,7 +17,8 @@
 
 
 class StatementResponse(Enum):
     NOT_IN_SCHEMA = "not in schema"
     ALLOWED = "allowed"
     INCORRECT = "incorrect"
     CORRECT = "correct"
+    MISSING = "missing"
```

### Comparing `entityshape-0.0.1/entityshape/models/__pycache__/compareshape.cpython-311.pyc` & `entityshape-0.0.2/entityshape/models/__pycache__/compareshape.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x30aa9564 (Fri Jun 23 14:20:32 2023 UTC)
+moddate:  0x8cb99564 (Fri Jun 23 15:26:04 2023 UTC)
 files sz: 12458
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `entityshape-0.0.1/entityshape/models/__pycache__/conditions.cpython-311.pyc` & `entityshape-0.0.2/entityshape/models/__pycache__/conditions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.1/entityshape/models/__pycache__/property_value.cpython-311.pyc` & `entityshape-0.0.2/entityshape/models/__pycache__/property_value.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8fa99564 (Fri Jun 23 14:17:51 2023 UTC)
+moddate:  0x8cb99564 (Fri Jun 23 15:26:04 2023 UTC)
 files sz: 245
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `entityshape-0.0.1/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc` & `entityshape-0.0.2/entityshape/models/__pycache__/propertyanalyzer.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.1/entityshape/models/__pycache__/result.cpython-311.pyc` & `entityshape-0.0.2/entityshape/models/__pycache__/result.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,82 +1,98 @@
 magic:    0xa70d0d0a
-moddate:  0x8fa99564 (Fri Jun 23 14:17:51 2023 UTC)
-files sz: 5616
+moddate:  0x99e59664 (Sat Jun 24 12:46:17 2023 UTC)
+files sz: 5981
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
-      0x9700640064016c006d015a016d025a026d035a030100640064026c046d
-      055a056d065a060100640064036c076d085a086d095a096d0a5a0a010064
-      0064046c0b6d0c5a0c0100640064056c0d6d0e5a0e010002004700640684
-      0064076505a6030000ab0300000000000000005a0f64085300
+      0x9700640064016c005a00640064026c016d025a026d035a036d045a0401
+      00640064036c056d065a066d075a070100640064046c086d095a096d0a5a
+      0a6d0b5a0b0100640064056c0c6d0d5a0d0100640064066c0e6d0f5a0f01
+      00020065006a1000000000000000006511a6010000ab0100000000000000
+      005a12020047006407840064086506a6030000ab0300000000000000005a
+      1364015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('Any', 'Dict', 'Set'))
-                 6 IMPORT_NAME              0 (typing)
-                 8 IMPORT_FROM              1 (Any)
-                10 STORE_NAME               1 (Any)
-                12 IMPORT_FROM              2 (Dict)
-                14 STORE_NAME               2 (Dict)
-                16 IMPORT_FROM              3 (Set)
-                18 STORE_NAME               3 (Set)
-                20 POP_TOP
+                 4 LOAD_CONST               1 (None)
+                 6 IMPORT_NAME              0 (logging)
+                 8 STORE_NAME               0 (logging)
    
-     3          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               2 (('BaseModel', 'Field'))
-                26 IMPORT_NAME              4 (pydantic)
-                28 IMPORT_FROM              5 (BaseModel)
-                30 STORE_NAME               5 (BaseModel)
-                32 IMPORT_FROM              6 (Field)
-                34 STORE_NAME               6 (Field)
-                36 POP_TOP
+     2          10 LOAD_CONST               0 (0)
+                12 LOAD_CONST               2 (('Any', 'Dict', 'Set'))
+                14 IMPORT_NAME              1 (typing)
+                16 IMPORT_FROM              2 (Any)
+                18 STORE_NAME               2 (Any)
+                20 IMPORT_FROM              3 (Dict)
+                22 STORE_NAME               3 (Dict)
+                24 IMPORT_FROM              4 (Set)
+                26 STORE_NAME               4 (Set)
+                28 POP_TOP
    
-     5          38 LOAD_CONST               0 (0)
-                40 LOAD_CONST               3 (('Necessity', 'PropertyResponse', 'StatementResponse'))
-                42 IMPORT_NAME              7 (entityshape.enums)
-                44 IMPORT_FROM              8 (Necessity)
-                46 STORE_NAME               8 (Necessity)
-                48 IMPORT_FROM              9 (PropertyResponse)
-                50 STORE_NAME               9 (PropertyResponse)
-                52 IMPORT_FROM             10 (StatementResponse)
-                54 STORE_NAME              10 (StatementResponse)
-                56 POP_TOP
+     4          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('BaseModel', 'ValidationError'))
+                34 IMPORT_NAME              5 (pydantic)
+                36 IMPORT_FROM              6 (BaseModel)
+                38 STORE_NAME               6 (BaseModel)
+                40 IMPORT_FROM              7 (ValidationError)
+                42 STORE_NAME               7 (ValidationError)
+                44 POP_TOP
    
-     6          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               4 (('PropertyValue',))
-                62 IMPORT_NAME             11 (entityshape.models.property_value)
-                64 IMPORT_FROM             12 (PropertyValue)
-                66 STORE_NAME              12 (PropertyValue)
-                68 POP_TOP
+     6          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('Necessity', 'PropertyResponse', 'StatementResponse'))
+                50 IMPORT_NAME              8 (entityshape.enums)
+                52 IMPORT_FROM              9 (Necessity)
+                54 STORE_NAME               9 (Necessity)
+                56 IMPORT_FROM             10 (PropertyResponse)
+                58 STORE_NAME              10 (PropertyResponse)
+                60 IMPORT_FROM             11 (StatementResponse)
+                62 STORE_NAME              11 (StatementResponse)
+                64 POP_TOP
    
-     7          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               5 (('StatementValue',))
-                74 IMPORT_NAME             13 (entityshape.models.statement_value)
-                76 IMPORT_FROM             14 (StatementValue)
-                78 STORE_NAME              14 (StatementValue)
-                80 POP_TOP
+     7          66 LOAD_CONST               0 (0)
+                68 LOAD_CONST               5 (('PropertyValue',))
+                70 IMPORT_NAME             12 (entityshape.models.property_value)
+                72 IMPORT_FROM             13 (PropertyValue)
+                74 STORE_NAME              13 (PropertyValue)
+                76 POP_TOP
    
-    10          82 PUSH_NULL
-                84 LOAD_BUILD_CLASS
-                86 LOAD_CONST               6 (<code object Result, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 10>)
-                88 MAKE_FUNCTION            0
-                90 LOAD_CONST               7 ('Result')
-                92 LOAD_NAME                5 (BaseModel)
-                94 PRECALL                  3
-                98 CALL                     3
-               108 STORE_NAME              15 (Result)
-               110 LOAD_CONST               8 (None)
-               112 RETURN_VALUE
+     8          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               6 (('StatementValue',))
+                82 IMPORT_NAME             14 (entityshape.models.statement_value)
+                84 IMPORT_FROM             15 (StatementValue)
+                86 STORE_NAME              15 (StatementValue)
+                88 POP_TOP
+   
+    10          90 PUSH_NULL
+                92 LOAD_NAME                0 (logging)
+                94 LOAD_ATTR               16 (getLogger)
+               104 LOAD_NAME               17 (__name__)
+               106 PRECALL                  1
+               110 CALL                     1
+               120 STORE_NAME              18 (logger)
+   
+    13         122 PUSH_NULL
+               124 LOAD_BUILD_CLASS
+               126 LOAD_CONST               7 (<code object Result, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 13>)
+               128 MAKE_FUNCTION            0
+               130 LOAD_CONST               8 ('Result')
+               132 LOAD_NAME                6 (BaseModel)
+               134 PRECALL                  3
+               138 CALL                     3
+               148 STORE_NAME              19 (Result)
+               150 LOAD_CONST               1 (None)
+               152 RETURN_VALUE
    consts
       0
+      None
       ('Any', 'Dict', 'Set')
-      ('BaseModel', 'Field')
+      ('BaseModel', 'ValidationError')
       ('Necessity', 'PropertyResponse', 'StatementResponse')
       ('PropertyValue',)
       ('StatementValue',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
@@ -87,316 +103,330 @@
             0965046508650a660219000000000000000000650664043c00000069005a
             0b65046505650c660219000000000000000000650664053c000000020065
             0da6000000ab0000000000000000005a0e650f6508190000000000000000
             00650664063c0000000200650da6000000ab0000000000000000005a1065
             0f650819000000000000000000650664073c0000000200650da6000000ab
             0000000000000000005a11650f650819000000000000000000650664083c
             0000000200650da6000000ab0000000000000000005a12650f6508190000
-            00000000000000650664093c000000640a5a1365146506640b3c00000002
-            00650da6000000ab0000000000000000005a15650f650819000000000000
-            0000006506640c3c0000000200650da6000000ab0000000000000000005a
+            00000000000000650664093c0000000200650da6000000ab000000000000
+            0000005a13650f6508190000000000000000006506640a3c000000640b5a
+            1465156506640c3c0000000200650da6000000ab0000000000000000005a
             16650f6508190000000000000000006506640d3c0000000200650da60000
             00ab0000000000000000005a17650f650819000000000000000000650664
             0e3c0000000200650da6000000ab0000000000000000005a18650f650819
             0000000000000000006506640f3c0000000200650da6000000ab00000000
-            00000000005a19650f650819000000000000000000650664103c00000065
-            1a64118400a6000000ab0000000000000000005a1b651a64128400a60000
-            00ab0000000000000000005a1c651a64138400a6000000ab000000000000
-            0000005a1d651a64148400a6000000ab0000000000000000005a1e651a64
-            158400a6000000ab0000000000000000005a1f651a641665146602641784
-            04a6000000ab0000000000000000005a20651a64188400a6000000ab0000
-            000000000000005a21641984005a22641a84005a23641b84005a24641c84
-            005a25641d84005a26641e84005a27641f84005a28642084005a29642184
-            005a2a642284005a2b64235300
-          10           0 RESUME                   0
+            00000000005a19650f650819000000000000000000650664103c00000002
+            00650da6000000ab0000000000000000005a1a650f650819000000000000
+            000000650664113c000000651b64128400a6000000ab0000000000000000
+            005a1c651b64138400a6000000ab0000000000000000005a1d651b641484
+            00a6000000ab0000000000000000005a1e651b64158400a6000000ab0000
+            000000000000005a1f651b64168400a6000000ab0000000000000000005a
+            20651b64176515660264188404a6000000ab0000000000000000005a2165
+            1b64198400a6000000ab0000000000000000005a22641a84005a23641b84
+            005a24641c84005a25641d84005a26641e84005a27641f84005a28642084
+            005a29642184005a2a642284005a2b642384005a2c64245300
+          13           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Result')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          11          12 BUILD_MAP                0
+          14          12 BUILD_MAP                0
                       14 STORE_NAME               3 (general)
                       16 LOAD_NAME                4 (Dict)
                       18 LOAD_NAME                5 (Any)
                       20 LOAD_NAME                5 (Any)
                       22 BUILD_TUPLE              2
                       24 BINARY_SUBSCR
                       34 LOAD_NAME                6 (__annotations__)
                       36 LOAD_CONST               1 ('general')
                       38 STORE_SUBSCR
          
-          12          42 LOAD_CONST               2 ('')
+          15          42 LOAD_CONST               2 ('')
                       44 STORE_NAME               7 (name)
                       46 LOAD_NAME                8 (str)
                       48 LOAD_NAME                6 (__annotations__)
                       50 LOAD_CONST               3 ('name')
                       52 STORE_SUBSCR
          
-          13          56 BUILD_MAP                0
+          16          56 BUILD_MAP                0
                       58 STORE_NAME               9 (properties)
                       60 LOAD_NAME                4 (Dict)
                       62 LOAD_NAME                8 (str)
                       64 LOAD_NAME               10 (PropertyValue)
                       66 BUILD_TUPLE              2
                       68 BINARY_SUBSCR
                       78 LOAD_NAME                6 (__annotations__)
                       80 LOAD_CONST               4 ('properties')
                       82 STORE_SUBSCR
          
-          14          86 BUILD_MAP                0
+          17          86 BUILD_MAP                0
                       88 STORE_NAME              11 (statements)
                       90 LOAD_NAME                4 (Dict)
                       92 LOAD_NAME                5 (Any)
                       94 LOAD_NAME               12 (StatementValue)
                       96 BUILD_TUPLE              2
                       98 BINARY_SUBSCR
                      108 LOAD_NAME                6 (__annotations__)
                      110 LOAD_CONST               5 ('statements')
                      112 STORE_SUBSCR
          
-          15         116 PUSH_NULL
+          18         116 PUSH_NULL
                      118 LOAD_NAME               13 (set)
                      120 PRECALL                  0
                      124 CALL                     0
                      134 STORE_NAME              14 (missing_properties)
                      136 LOAD_NAME               15 (Set)
                      138 LOAD_NAME                8 (str)
                      140 BINARY_SUBSCR
                      150 LOAD_NAME                6 (__annotations__)
                      152 LOAD_CONST               6 ('missing_properties')
                      154 STORE_SUBSCR
          
-          16         158 PUSH_NULL
+          19         158 PUSH_NULL
                      160 LOAD_NAME               13 (set)
                      162 PRECALL                  0
                      166 CALL                     0
                      176 STORE_NAME              16 (required_properties)
                      178 LOAD_NAME               15 (Set)
                      180 LOAD_NAME                8 (str)
                      182 BINARY_SUBSCR
                      192 LOAD_NAME                6 (__annotations__)
                      194 LOAD_CONST               7 ('required_properties')
                      196 STORE_SUBSCR
          
-          17         200 PUSH_NULL
+          20         200 PUSH_NULL
                      202 LOAD_NAME               13 (set)
                      204 PRECALL                  0
                      208 CALL                     0
                      218 STORE_NAME              17 (incorrect_statements)
                      220 LOAD_NAME               15 (Set)
                      222 LOAD_NAME                8 (str)
                      224 BINARY_SUBSCR
                      234 LOAD_NAME                6 (__annotations__)
                      236 LOAD_CONST               8 ('incorrect_statements')
                      238 STORE_SUBSCR
          
-          18         242 PUSH_NULL
+          21         242 PUSH_NULL
                      244 LOAD_NAME               13 (set)
                      246 PRECALL                  0
                      250 CALL                     0
-                     260 STORE_NAME              18 (properties_with_too_many_statements)
+                     260 STORE_NAME              18 (missing_statements)
                      262 LOAD_NAME               15 (Set)
                      264 LOAD_NAME                8 (str)
                      266 BINARY_SUBSCR
                      276 LOAD_NAME                6 (__annotations__)
-                     278 LOAD_CONST               9 ('properties_with_too_many_statements')
+                     278 LOAD_CONST               9 ('missing_statements')
                      280 STORE_SUBSCR
          
-          19         284 LOAD_CONST              10 (False)
-                     286 STORE_NAME              19 (analyzed)
-                     288 LOAD_NAME               20 (bool)
-                     290 LOAD_NAME                6 (__annotations__)
-                     292 LOAD_CONST              11 ('analyzed')
-                     294 STORE_SUBSCR
-         
-          20         298 PUSH_NULL
-                     300 LOAD_NAME               13 (set)
-                     302 PRECALL                  0
-                     306 CALL                     0
-                     316 STORE_NAME              21 (required_properties_that_are_missing)
-                     318 LOAD_NAME               15 (Set)
-                     320 LOAD_NAME                8 (str)
-                     322 BINARY_SUBSCR
+          22         284 PUSH_NULL
+                     286 LOAD_NAME               13 (set)
+                     288 PRECALL                  0
+                     292 CALL                     0
+                     302 STORE_NAME              19 (properties_with_too_many_statements)
+                     304 LOAD_NAME               15 (Set)
+                     306 LOAD_NAME                8 (str)
+                     308 BINARY_SUBSCR
+                     318 LOAD_NAME                6 (__annotations__)
+                     320 LOAD_CONST              10 ('properties_with_too_many_statements')
+                     322 STORE_SUBSCR
+         
+          23         326 LOAD_CONST              11 (False)
+                     328 STORE_NAME              20 (analyzed)
+                     330 LOAD_NAME               21 (bool)
                      332 LOAD_NAME                6 (__annotations__)
-                     334 LOAD_CONST              12 ('required_properties_that_are_missing')
+                     334 LOAD_CONST              12 ('analyzed')
                      336 STORE_SUBSCR
          
-          21         340 PUSH_NULL
+          24         340 PUSH_NULL
                      342 LOAD_NAME               13 (set)
                      344 PRECALL                  0
                      348 CALL                     0
-                     358 STORE_NAME              22 (optional_properties_that_are_missing)
+                     358 STORE_NAME              22 (required_properties_that_are_missing)
                      360 LOAD_NAME               15 (Set)
                      362 LOAD_NAME                8 (str)
                      364 BINARY_SUBSCR
                      374 LOAD_NAME                6 (__annotations__)
-                     376 LOAD_CONST              13 ('optional_properties_that_are_missing')
+                     376 LOAD_CONST              13 ('required_properties_that_are_missing')
                      378 STORE_SUBSCR
          
-          22         382 PUSH_NULL
+          25         382 PUSH_NULL
                      384 LOAD_NAME               13 (set)
                      386 PRECALL                  0
                      390 CALL                     0
-                     400 STORE_NAME              23 (properties_without_enough_correct_statements)
+                     400 STORE_NAME              23 (optional_properties_that_are_missing)
                      402 LOAD_NAME               15 (Set)
                      404 LOAD_NAME                8 (str)
                      406 BINARY_SUBSCR
                      416 LOAD_NAME                6 (__annotations__)
-                     418 LOAD_CONST              14 ('properties_without_enough_correct_statements')
+                     418 LOAD_CONST              14 ('optional_properties_that_are_missing')
                      420 STORE_SUBSCR
          
-          23         424 PUSH_NULL
+          26         424 PUSH_NULL
                      426 LOAD_NAME               13 (set)
                      428 PRECALL                  0
                      432 CALL                     0
-                     442 STORE_NAME              24 (properties_that_are_not_allowed)
+                     442 STORE_NAME              24 (properties_without_enough_correct_statements)
                      444 LOAD_NAME               15 (Set)
                      446 LOAD_NAME                8 (str)
                      448 BINARY_SUBSCR
                      458 LOAD_NAME                6 (__annotations__)
-                     460 LOAD_CONST              15 ('properties_that_are_not_allowed')
+                     460 LOAD_CONST              15 ('properties_without_enough_correct_statements')
                      462 STORE_SUBSCR
          
-          24         466 PUSH_NULL
+          27         466 PUSH_NULL
                      468 LOAD_NAME               13 (set)
                      470 PRECALL                  0
                      474 CALL                     0
-                     484 STORE_NAME              25 (statements_with_property_that_is_not_allowed)
+                     484 STORE_NAME              25 (properties_that_are_not_allowed)
                      486 LOAD_NAME               15 (Set)
                      488 LOAD_NAME                8 (str)
                      490 BINARY_SUBSCR
                      500 LOAD_NAME                6 (__annotations__)
-                     502 LOAD_CONST              16 ('statements_with_property_that_is_not_allowed')
+                     502 LOAD_CONST              16 ('properties_that_are_not_allowed')
                      504 STORE_SUBSCR
          
-          26         508 LOAD_NAME               26 (property)
-         
-          27         510 LOAD_CONST              17 (<code object some_required_properties_are_missing, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 26>)
-                     512 MAKE_FUNCTION            0
-         
-          26         514 PRECALL                  0
-                     518 CALL                     0
-         
-          27         528 STORE_NAME              27 (some_required_properties_are_missing)
-         
-          30         530 LOAD_NAME               26 (property)
-         
-          31         532 LOAD_CONST              18 (<code object properties_with_too_many_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 30>)
-                     534 MAKE_FUNCTION            0
+          28         508 PUSH_NULL
+                     510 LOAD_NAME               13 (set)
+                     512 PRECALL                  0
+                     516 CALL                     0
+                     526 STORE_NAME              26 (statements_with_property_that_is_not_allowed)
+                     528 LOAD_NAME               15 (Set)
+                     530 LOAD_NAME                8 (str)
+                     532 BINARY_SUBSCR
+                     542 LOAD_NAME                6 (__annotations__)
+                     544 LOAD_CONST              17 ('statements_with_property_that_is_not_allowed')
+                     546 STORE_SUBSCR
          
-          30         536 PRECALL                  0
-                     540 CALL                     0
+          30         550 LOAD_NAME               27 (property)
          
-          31         550 STORE_NAME              28 (properties_with_too_many_statements_found)
+          31         552 LOAD_CONST              18 (<code object some_required_properties_are_missing, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 30>)
+                     554 MAKE_FUNCTION            0
          
-          34         552 LOAD_NAME               26 (property)
+          30         556 PRECALL                  0
+                     560 CALL                     0
          
-          35         554 LOAD_CONST              19 (<code object incorrect_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 34>)
-                     556 MAKE_FUNCTION            0
+          31         570 STORE_NAME              28 (some_required_properties_are_missing)
          
-          34         558 PRECALL                  0
-                     562 CALL                     0
+          34         572 LOAD_NAME               27 (property)
          
-          35         572 STORE_NAME              29 (incorrect_statements_found)
+          35         574 LOAD_CONST              19 (<code object properties_with_too_many_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 34>)
+                     576 MAKE_FUNCTION            0
          
-          38         574 LOAD_NAME               26 (property)
+          34         578 PRECALL                  0
+                     582 CALL                     0
          
-          39         576 LOAD_CONST              20 (<code object properties_without_enough_correct_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 38>)
-                     578 MAKE_FUNCTION            0
+          35         592 STORE_NAME              29 (properties_with_too_many_statements_found)
          
-          38         580 PRECALL                  0
-                     584 CALL                     0
+          38         594 LOAD_NAME               27 (property)
          
-          39         594 STORE_NAME              30 (properties_without_enough_correct_statements_found)
+          39         596 LOAD_CONST              20 (<code object incorrect_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 38>)
+                     598 MAKE_FUNCTION            0
          
-          42         596 LOAD_NAME               26 (property)
+          38         600 PRECALL                  0
+                     604 CALL                     0
          
-          43         598 LOAD_CONST              21 (<code object statements_with_properties_that_are_not_allowed_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 42>)
-                     600 MAKE_FUNCTION            0
+          39         614 STORE_NAME              30 (incorrect_statements_found)
          
-          42         602 PRECALL                  0
-                     606 CALL                     0
+          42         616 LOAD_NAME               27 (property)
          
-          43         616 STORE_NAME              31 (statements_with_properties_that_are_not_allowed_found)
+          43         618 LOAD_CONST              21 (<code object properties_without_enough_correct_statements_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 42>)
+                     620 MAKE_FUNCTION            0
          
-          46         618 LOAD_NAME               26 (property)
+          42         622 PRECALL                  0
+                     626 CALL                     0
          
-          47         620 LOAD_CONST              22 ('return')
-                     622 LOAD_NAME               20 (bool)
-                     624 BUILD_TUPLE              2
-                     626 LOAD_CONST              23 (<code object is_valid, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 46>)
-                     628 MAKE_FUNCTION            4 (annotations)
+          43         636 STORE_NAME              31 (properties_without_enough_correct_statements_found)
          
-          46         630 PRECALL                  0
-                     634 CALL                     0
+          46         638 LOAD_NAME               27 (property)
          
-          47         644 STORE_NAME              32 (is_valid)
+          47         640 LOAD_CONST              22 (<code object statements_with_properties_that_are_not_allowed_found, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 46>)
+                     642 MAKE_FUNCTION            0
          
-          61         646 LOAD_NAME               26 (property)
+          46         644 PRECALL                  0
+                     648 CALL                     0
          
-          62         648 LOAD_CONST              24 (<code object is_empty, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 61>)
-                     650 MAKE_FUNCTION            0
+          47         658 STORE_NAME              32 (statements_with_properties_that_are_not_allowed_found)
          
-          61         652 PRECALL                  0
-                     656 CALL                     0
+          50         660 LOAD_NAME               27 (property)
          
-          62         666 STORE_NAME              33 (is_empty)
+          51         662 LOAD_CONST              23 ('return')
+                     664 LOAD_NAME               21 (bool)
+                     666 BUILD_TUPLE              2
+                     668 LOAD_CONST              24 (<code object is_valid, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 50>)
+                     670 MAKE_FUNCTION            4 (annotations)
          
-          65         668 LOAD_CONST              25 (<code object analyze, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 65>)
-                     670 MAKE_FUNCTION            0
-                     672 STORE_NAME              34 (analyze)
+          50         672 PRECALL                  0
+                     676 CALL                     0
          
-          78         674 LOAD_CONST              26 (<code object __find_properties_with_too_many_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 78>)
-                     676 MAKE_FUNCTION            0
-                     678 STORE_NAME              35 (__find_properties_with_too_many_statements__)
+          51         686 STORE_NAME              33 (is_valid)
          
-          84         680 LOAD_CONST              27 (<code object __find_incorrect_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 84>)
-                     682 MAKE_FUNCTION            0
-                     684 STORE_NAME              36 (__find_incorrect_statements__)
+          65         688 LOAD_NAME               27 (property)
          
-          90         686 LOAD_CONST              28 (<code object __find_required_properties__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 90>)
-                     688 MAKE_FUNCTION            0
-                     690 STORE_NAME              37 (__find_required_properties__)
+          66         690 LOAD_CONST              25 (<code object is_empty, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 65>)
+                     692 MAKE_FUNCTION            0
          
-          96         692 LOAD_CONST              29 (<code object __find_missing_properties__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 96>)
-                     694 MAKE_FUNCTION            0
-                     696 STORE_NAME              38 (__find_missing_properties__)
+          65         694 PRECALL                  0
+                     698 CALL                     0
          
-         102         698 LOAD_CONST              30 (<code object __find_required_properties_that_are_missing__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 102>)
-                     700 MAKE_FUNCTION            0
-                     702 STORE_NAME              39 (__find_required_properties_that_are_missing__)
+          66         708 STORE_NAME              34 (is_empty)
          
-         109         704 LOAD_CONST              31 (<code object __find_optional_properties_that_are_missing__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 109>)
-                     706 MAKE_FUNCTION            0
-                     708 STORE_NAME              40 (__find_optional_properties_that_are_missing__)
-         
-         115         710 LOAD_CONST              32 (<code object __find_properties_with_not_enough_correct_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 115>)
+          69         710 LOAD_CONST              26 (<code object analyze, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 69>)
                      712 MAKE_FUNCTION            0
-                     714 STORE_NAME              41 (__find_properties_with_not_enough_correct_statements__)
+                     714 STORE_NAME              35 (analyze)
          
-         121         716 LOAD_CONST              33 (<code object __find_properties_that_are_not_allowed__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 121>)
+          82         716 LOAD_CONST              27 (<code object __find_properties_with_too_many_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 82>)
                      718 MAKE_FUNCTION            0
-                     720 STORE_NAME              42 (__find_properties_that_are_not_allowed__)
+                     720 STORE_NAME              36 (__find_properties_with_too_many_statements__)
          
-         127         722 LOAD_CONST              34 (<code object __find_statements_with_property_that_is_not_allowed__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 127>)
+          88         722 LOAD_CONST              28 (<code object __find_incorrect_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 88>)
                      724 MAKE_FUNCTION            0
-                     726 STORE_NAME              43 (__find_statements_with_property_that_is_not_allowed__)
-                     728 LOAD_CONST              35 (None)
-                     730 RETURN_VALUE
+                     726 STORE_NAME              37 (__find_incorrect_statements__)
+         
+         100         728 LOAD_CONST              29 (<code object __find_required_properties__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 100>)
+                     730 MAKE_FUNCTION            0
+                     732 STORE_NAME              38 (__find_required_properties__)
+         
+         106         734 LOAD_CONST              30 (<code object __find_missing_properties__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 106>)
+                     736 MAKE_FUNCTION            0
+                     738 STORE_NAME              39 (__find_missing_properties__)
+         
+         112         740 LOAD_CONST              31 (<code object __find_required_properties_that_are_missing__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 112>)
+                     742 MAKE_FUNCTION            0
+                     744 STORE_NAME              40 (__find_required_properties_that_are_missing__)
+         
+         119         746 LOAD_CONST              32 (<code object __find_optional_properties_that_are_missing__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 119>)
+                     748 MAKE_FUNCTION            0
+                     750 STORE_NAME              41 (__find_optional_properties_that_are_missing__)
+         
+         125         752 LOAD_CONST              33 (<code object __find_properties_with_not_enough_correct_statements__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 125>)
+                     754 MAKE_FUNCTION            0
+                     756 STORE_NAME              42 (__find_properties_with_not_enough_correct_statements__)
+         
+         131         758 LOAD_CONST              34 (<code object __find_properties_that_are_not_allowed__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 131>)
+                     760 MAKE_FUNCTION            0
+                     762 STORE_NAME              43 (__find_properties_that_are_not_allowed__)
+         
+         137         764 LOAD_CONST              35 (<code object __find_statements_with_property_that_is_not_allowed__, file "/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py", line 137>)
+                     766 MAKE_FUNCTION            0
+                     768 STORE_NAME              44 (__find_statements_with_property_that_is_not_allowed__)
+                     770 LOAD_CONST              36 (None)
+                     772 RETURN_VALUE
          consts
             'Result'
             'general'
             ''
             'name'
             'properties'
             'statements'
             'missing_properties'
             'required_properties'
             'incorrect_statements'
+            'missing_statements'
             'properties_with_too_many_statements'
             False
             'analyzed'
             'required_properties_that_are_missing'
             'optional_properties_that_are_missing'
             'properties_without_enough_correct_statements'
             'properties_that_are_not_allowed'
@@ -405,212 +435,212 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                26           0 RESUME                   0
+                30           0 RESUME                   0
                
-                28           2 LOAD_GLOBAL              1 (NULL + bool)
+                32           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (required_properties_that_are_missing)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'required_properties_that_are_missing')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'some_required_properties_are_missing'
-               firstlineno 26
+               firstlineno 30
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                30           0 RESUME                   0
+                34           0 RESUME                   0
                
-                32           2 LOAD_GLOBAL              1 (NULL + bool)
+                36           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (properties_with_too_many_statements)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'properties_with_too_many_statements')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'properties_with_too_many_statements_found'
-               firstlineno 30
+               firstlineno 34
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                34           0 RESUME                   0
+                38           0 RESUME                   0
                
-                36           2 LOAD_GLOBAL              1 (NULL + bool)
+                40           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (incorrect_statements)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'incorrect_statements')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'incorrect_statements_found'
-               firstlineno 34
+               firstlineno 38
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                38           0 RESUME                   0
+                42           0 RESUME                   0
                
-                40           2 LOAD_GLOBAL              1 (NULL + bool)
+                44           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (properties_without_enough_correct_statements)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'properties_without_enough_correct_statements')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'properties_without_enough_correct_statements_found'
-               firstlineno 38
+               firstlineno 42
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000005300
-                42           0 RESUME                   0
+                46           0 RESUME                   0
                
-                44           2 LOAD_GLOBAL              1 (NULL + bool)
+                48           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (statements_with_property_that_is_not_allowed)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 RETURN_VALUE
                consts
                   None
                names      ('bool', 'statements_with_property_that_is_not_allowed')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'statements_with_properties_that_are_not_allowed_found'
-               firstlineno 42
+               firstlineno 46
                lnotab 0x0202
             'return'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab00000000000000000001007403000000000000000000007c006a0200
                   000000000000000c006f1f7c006a0300000000000000000c006f177c006a
                   0400000000000000000c006f0f7c006a0500000000000000000c006f077c
                   006a0600000000000000000c00a6010000ab0100000000000000005300
-                46           0 RESUME                   0
+                50           0 RESUME                   0
                
-                52           2 LOAD_FAST                0 (self)
+                56           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (analyze)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                
-                53          42 LOAD_GLOBAL              3 (NULL + bool)
+                57          42 LOAD_GLOBAL              3 (NULL + bool)
                
-                54          54 LOAD_FAST                0 (self)
+                58          54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (properties_with_too_many_statements_found)
                             66 UNARY_NOT
                             68 JUMP_IF_FALSE_OR_POP    31 (to 132)
                
-                55          70 LOAD_FAST                0 (self)
+                59          70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                3 (incorrect_statements_found)
                             82 UNARY_NOT
                
-                54          84 JUMP_IF_FALSE_OR_POP    23 (to 132)
+                58          84 JUMP_IF_FALSE_OR_POP    23 (to 132)
                
-                56          86 LOAD_FAST                0 (self)
+                60          86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                4 (some_required_properties_are_missing)
                             98 UNARY_NOT
                
-                54         100 JUMP_IF_FALSE_OR_POP    15 (to 132)
+                58         100 JUMP_IF_FALSE_OR_POP    15 (to 132)
                
-                57         102 LOAD_FAST                0 (self)
+                61         102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                5 (properties_without_enough_correct_statements_found)
                            114 UNARY_NOT
                
-                54         116 JUMP_IF_FALSE_OR_POP     7 (to 132)
+                58         116 JUMP_IF_FALSE_OR_POP     7 (to 132)
                
-                58         118 LOAD_FAST                0 (self)
+                62         118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                6 (statements_with_properties_that_are_not_allowed_found)
                            130 UNARY_NOT
                
-                53     >>  132 PRECALL                  1
+                57     >>  132 PRECALL                  1
                            136 CALL                     1
                            146 RETURN_VALUE
                consts
                   'check if the properties are all allowed,\n        all required properties are present,\n        not too many statements,\n        and none of the statements are incorrect'
                names      ('analyze', 'bool', 'properties_with_too_many_statements_found', 'incorrect_statements_found', 'some_required_properties_are_missing', 'properties_without_enough_correct_statements_found', 'statements_with_properties_that_are_not_allowed_found')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'is_valid'
-               firstlineno 46
+               firstlineno 50
                lnotab 0x020628010c0110010eff02020efe02030efd02040efb
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007401000000000000000000007403000000000000000000007c006a
                   020000000000000000a6010000ab01000000000000000064016b02000000
                   006f177403000000000000000000007c006a030000000000000000a60100
                   00ab01000000000000000064016b0200000000a6010000ab010000000000
                   0000005300
-                61           0 RESUME                   0
+                65           0 RESUME                   0
                
-                63           2 LOAD_GLOBAL              1 (NULL + bool)
+                67           2 LOAD_GLOBAL              1 (NULL + bool)
                             14 LOAD_GLOBAL              3 (NULL + len)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (properties)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_CONST               1 (0)
                             54 COMPARE_OP               2 (==)
@@ -630,15 +660,15 @@
                   0
                names      ('bool', 'len', 'properties', 'statements')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'is_empty'
-               firstlineno 61
+               firstlineno 65
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
@@ -652,333 +682,377 @@
                   000000000001007c00a00600000000000000000000000000000000000000
                   00a6000000ab00000000000000000001007c00a007000000000000000000
                   0000000000000000000000a6000000ab00000000000000000001007c00a0
                   080000000000000000000000000000000000000000a6000000ab00000000
                   000000000001007c00a00900000000000000000000000000000000000000
                   00a6000000ab000000000000000000010064017c005f0000000000000000
                   006400530064005300
-                65           0 RESUME                   0
+                69           0 RESUME                   0
                
-                66           2 LOAD_FAST                0 (self)
+                70           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (analyzed)
                             14 POP_JUMP_FORWARD_IF_TRUE   189 (to 394)
                
-                67          16 LOAD_FAST                0 (self)
+                71          16 LOAD_FAST                0 (self)
                             18 LOAD_METHOD              1 (__find_missing_properties__)
                             40 PRECALL                  0
                             44 CALL                     0
                             54 POP_TOP
                
-                68          56 LOAD_FAST                0 (self)
+                72          56 LOAD_FAST                0 (self)
                             58 LOAD_METHOD              2 (__find_required_properties__)
                             80 PRECALL                  0
                             84 CALL                     0
                             94 POP_TOP
                
-                69          96 LOAD_FAST                0 (self)
+                73          96 LOAD_FAST                0 (self)
                             98 LOAD_METHOD              3 (__find_incorrect_statements__)
                            120 PRECALL                  0
                            124 CALL                     0
                            134 POP_TOP
                
-                70         136 LOAD_FAST                0 (self)
+                74         136 LOAD_FAST                0 (self)
                            138 LOAD_METHOD              4 (__find_properties_with_too_many_statements__)
                            160 PRECALL                  0
                            164 CALL                     0
                            174 POP_TOP
                
-                71         176 LOAD_FAST                0 (self)
+                75         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD              5 (__find_properties_with_not_enough_correct_statements__)
                            200 PRECALL                  0
                            204 CALL                     0
                            214 POP_TOP
                
-                72         216 LOAD_FAST                0 (self)
+                76         216 LOAD_FAST                0 (self)
                            218 LOAD_METHOD              6 (__find_required_properties_that_are_missing__)
                            240 PRECALL                  0
                            244 CALL                     0
                            254 POP_TOP
                
-                73         256 LOAD_FAST                0 (self)
+                77         256 LOAD_FAST                0 (self)
                            258 LOAD_METHOD              7 (__find_optional_properties_that_are_missing__)
                            280 PRECALL                  0
                            284 CALL                     0
                            294 POP_TOP
                
-                74         296 LOAD_FAST                0 (self)
+                78         296 LOAD_FAST                0 (self)
                            298 LOAD_METHOD              8 (__find_properties_that_are_not_allowed__)
                            320 PRECALL                  0
                            324 CALL                     0
                            334 POP_TOP
                
-                75         336 LOAD_FAST                0 (self)
+                79         336 LOAD_FAST                0 (self)
                            338 LOAD_METHOD              9 (__find_statements_with_property_that_is_not_allowed__)
                            360 PRECALL                  0
                            364 CALL                     0
                            374 POP_TOP
                
-                76         376 LOAD_CONST               1 (True)
+                80         376 LOAD_CONST               1 (True)
                            378 LOAD_FAST                0 (self)
                            380 STORE_ATTR               0 (analyzed)
                            390 LOAD_CONST               0 (None)
                            392 RETURN_VALUE
                
-                66     >>  394 LOAD_CONST               0 (None)
+                70     >>  394 LOAD_CONST               0 (None)
                            396 RETURN_VALUE
                consts
                   None
                   True
                names      ('analyzed', '__find_missing_properties__', '__find_required_properties__', '__find_incorrect_statements__', '__find_properties_with_too_many_statements__', '__find_properties_with_not_enough_correct_statements__', '__find_required_properties_that_are_missing__', '__find_optional_properties_that_are_missing__', '__find_properties_that_are_not_allowed__', '__find_statements_with_property_that_is_not_allowed__')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       'analyze'
-               firstlineno 65
+               firstlineno 69
                lnotab 0x02010e0128012801280128012801280128012801280112f6
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d3e7d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721a7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001008c3f64005300
-                78           0 RESUME                   0
+                82           0 RESUME                   0
                
-                79           2 LOAD_FAST                0 (self)
+                83           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (properties)
                             14 GET_ITER
                        >>   16 FOR_ITER                62 (to 142)
                             18 STORE_FAST               1 (property_)
                
-                80          20 LOAD_FAST                0 (self)
+                84          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (properties)
                             32 LOAD_FAST                1 (property_)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-                81          46 LOAD_FAST                2 (value)
+                85          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (response)
                             58 LOAD_GLOBAL              4 (PropertyResponse)
                             70 LOAD_ATTR                3 (TOO_MANY_STATEMENTS)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    26 (to 140)
                
-                82          88 LOAD_FAST                0 (self)
+                86          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (properties_with_too_many_statements)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                1 (property_)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                        >>  140 JUMP_BACKWARD           63 (to 16)
                
-                79     >>  142 LOAD_CONST               0 (None)
+                83     >>  142 LOAD_CONST               0 (None)
                            144 RETURN_VALUE
                consts
                   None
                names      ('properties', 'response', 'PropertyResponse', 'TOO_MANY_STATEMENTS', 'properties_with_too_many_statements', 'add')
                varnames   ('self', 'property_', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_properties_with_too_many_statements__'
-               firstlineno 78
+               firstlineno 82
                lnotab 0x020112011a012a0136fd
             code
                argcount  : 1
                nlocals   : 3
-               stacksize : 4
+               stacksize : 6
                flags     : 3
                code
-                  0x97007c006a00000000000000000044005d3e7d017c006a000000000000
-                  0000007c01190000000000000000007d027c026a01000000000000000074
-                  04000000000000000000006a0300000000000000006b0200000000721a7c
-                  006a040000000000000000a0050000000000000000000000000000000000
-                  0000007c01a6010000ab01000000000000000001008c3f64005300
-                84           0 RESUME                   0
+                  0x97007c006a00000000000000000044005d857d017c006a000000000000
+                  0000007c01190000000000000000007d0209007403000000000000000000
+                  007c026a020000000000000000a6010000ab01000000000000000001007c
+                  026a0200000000000000007402000000000000000000006a030000000000
+                  0000006b0200000000721a7c006a040000000000000000a0050000000000
+                  0000000000000000000000000000007c01a6010000ab0100000000000000
+                  0001008c542300740c00000000000000000000240072250100740e000000
+                  00000000000000a008000000000000000000000000000000000000000064
+                  017c026a0200000000000000009b009d02a6010000ab0100000000000000
+                  00010059008c82770078035900770164005300
+                88           0 RESUME                   0
                
-                85           2 LOAD_FAST                0 (self)
+                89           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (statements)
                             14 GET_ITER
-                       >>   16 FOR_ITER                62 (to 142)
+                       >>   16 FOR_ITER               133 (to 284)
                             18 STORE_FAST               1 (statement)
                
-                86          20 LOAD_FAST                0 (self)
+                90          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (statements)
                             32 LOAD_FAST                1 (statement)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-                87          46 LOAD_FAST                2 (value)
-                            48 LOAD_ATTR                1 (response)
-                            58 LOAD_GLOBAL              4 (StatementResponse)
-                            70 LOAD_ATTR                3 (INCORRECT)
-                            80 COMPARE_OP               2 (==)
-                            86 POP_JUMP_FORWARD_IF_FALSE    26 (to 140)
+                91          46 NOP
                
-                88          88 LOAD_FAST                0 (self)
-                            90 LOAD_ATTR                4 (incorrect_statements)
-                           100 LOAD_METHOD              5 (add)
-                           122 LOAD_FAST                1 (statement)
-                           124 PRECALL                  1
-                           128 CALL                     1
-                           138 POP_TOP
-                       >>  140 JUMP_BACKWARD           63 (to 16)
-               
-                85     >>  142 LOAD_CONST               0 (None)
-                           144 RETURN_VALUE
+                92          48 LOAD_GLOBAL              3 (NULL + StatementResponse)
+                            60 LOAD_FAST                2 (value)
+                            62 LOAD_ATTR                2 (response)
+                            72 PRECALL                  1
+                            76 CALL                     1
+                            86 POP_TOP
+               
+                93          88 LOAD_FAST                2 (value)
+                            90 LOAD_ATTR                2 (response)
+                           100 LOAD_GLOBAL              2 (StatementResponse)
+                           112 LOAD_ATTR                3 (INCORRECT)
+                           122 COMPARE_OP               2 (==)
+                           128 POP_JUMP_FORWARD_IF_FALSE    26 (to 182)
+               
+                94         130 LOAD_FAST                0 (self)
+                           132 LOAD_ATTR                4 (incorrect_statements)
+                           142 LOAD_METHOD              5 (add)
+                           164 LOAD_FAST                1 (statement)
+                           166 PRECALL                  1
+                           170 CALL                     1
+                           180 POP_TOP
+                       >>  182 JUMP_BACKWARD           84 (to 16)
+                       >>  184 PUSH_EXC_INFO
+               
+                95         186 LOAD_GLOBAL             12 (ValueError)
+                           198 CHECK_EXC_MATCH
+                           200 POP_JUMP_FORWARD_IF_FALSE    37 (to 276)
+                           202 POP_TOP
+               
+                97         204 LOAD_GLOBAL             14 (logger)
+                           216 LOAD_METHOD              8 (warning)
+                           238 LOAD_CONST               1 ('Ignoring statement response: ')
+                           240 LOAD_FAST                2 (value)
+                           242 LOAD_ATTR                2 (response)
+                           252 FORMAT_VALUE             0
+                           254 BUILD_STRING             2
+                           256 PRECALL                  1
+                           260 CALL                     1
+                           270 POP_TOP
+               
+                98         272 POP_EXCEPT
+                           274 JUMP_BACKWARD          130 (to 16)
+               
+                95     >>  276 RERAISE                  0
+                       >>  278 COPY                     3
+                           280 POP_EXCEPT
+                           282 RERAISE                  1
+               
+                89     >>  284 LOAD_CONST               0 (None)
+                           286 RETURN_VALUE
+               ExceptionTable:
+                 48 to 180 -> 184 [1]
+                 184 to 270 -> 278 [2] lasti
+                 276 to 276 -> 278 [2] lasti
                consts
                   None
-               names      ('statements', 'response', 'StatementResponse', 'INCORRECT', 'incorrect_statements', 'add')
+                  'Ignoring statement response: '
+               names      ('statements', 'StatementResponse', 'response', 'INCORRECT', 'incorrect_statements', 'add', 'ValueError', 'logger', 'warning')
                varnames   ('self', 'statement', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_incorrect_statements__'
-               firstlineno 84
-               lnotab 0x020112011a012a0136fd
+               firstlineno 88
+               lnotab 0x020112011a01020128012a0138011202440104fd08fa
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d3e7d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721a7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001008c3f64005300
-                90           0 RESUME                   0
+               100           0 RESUME                   0
                
-                91           2 LOAD_FAST                0 (self)
+               101           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (properties)
                             14 GET_ITER
                        >>   16 FOR_ITER                62 (to 142)
                             18 STORE_FAST               1 (property_)
                
-                92          20 LOAD_FAST                0 (self)
+               102          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (properties)
                             32 LOAD_FAST                1 (property_)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-                93          46 LOAD_FAST                2 (value)
+               103          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (necessity)
                             58 LOAD_GLOBAL              4 (Necessity)
                             70 LOAD_ATTR                3 (REQUIRED)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    26 (to 140)
                
-                94          88 LOAD_FAST                0 (self)
+               104          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (required_properties)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                1 (property_)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                        >>  140 JUMP_BACKWARD           63 (to 16)
                
-                91     >>  142 LOAD_CONST               0 (None)
+               101     >>  142 LOAD_CONST               0 (None)
                            144 RETURN_VALUE
                consts
                   None
                names      ('properties', 'necessity', 'Necessity', 'REQUIRED', 'required_properties', 'add')
                varnames   ('self', 'property_', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_required_properties__'
-               firstlineno 90
+               firstlineno 100
                lnotab 0x020112011a012a0136fd
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d3e7d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721a7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001008c3f64005300
-                96           0 RESUME                   0
+               106           0 RESUME                   0
                
-                97           2 LOAD_FAST                0 (self)
+               107           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (properties)
                             14 GET_ITER
                        >>   16 FOR_ITER                62 (to 142)
                             18 STORE_FAST               1 (property_)
                
-                98          20 LOAD_FAST                0 (self)
+               108          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (properties)
                             32 LOAD_FAST                1 (property_)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-                99          46 LOAD_FAST                2 (value)
+               109          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (response)
                             58 LOAD_GLOBAL              4 (PropertyResponse)
                             70 LOAD_ATTR                3 (MISSING)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    26 (to 140)
                
-               100          88 LOAD_FAST                0 (self)
+               110          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (missing_properties)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                1 (property_)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                        >>  140 JUMP_BACKWARD           63 (to 16)
                
-                97     >>  142 LOAD_CONST               0 (None)
+               107     >>  142 LOAD_CONST               0 (None)
                            144 RETURN_VALUE
                consts
                   None
                names      ('properties', 'response', 'PropertyResponse', 'MISSING', 'missing_properties', 'add')
                varnames   ('self', 'property_', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_missing_properties__'
-               firstlineno 96
+               firstlineno 106
                lnotab 0x020112011a012a0136fd
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000007d017401000000000000000000007c006a0200
                   00000000000000a6010000ab0100000000000000007d027c01a003000000
                   00000000000000000000000000000000007c02a6010000ab010000000000
                   0000007c005f04000000000000000064005300
-               102           0 RESUME                   0
+               112           0 RESUME                   0
                
-               103           2 LOAD_GLOBAL              1 (NULL + set)
+               113           2 LOAD_GLOBAL              1 (NULL + set)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (missing_properties)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 STORE_FAST               1 (a)
                
-               104          42 LOAD_GLOBAL              1 (NULL + set)
+               114          42 LOAD_GLOBAL              1 (NULL + set)
                             54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (required_properties)
                             66 PRECALL                  1
                             70 CALL                     1
                             80 STORE_FAST               2 (b)
                
-               107          82 LOAD_FAST                1 (a)
+               117          82 LOAD_FAST                1 (a)
                             84 LOAD_METHOD              3 (intersection)
                            106 LOAD_FAST                2 (b)
                            108 PRECALL                  1
                            112 CALL                     1
                            122 LOAD_FAST                0 (self)
                            124 STORE_ATTR               4 (required_properties_that_are_missing)
                            134 LOAD_CONST               0 (None)
@@ -987,44 +1061,44 @@
                   None
                names      ('set', 'missing_properties', 'required_properties', 'intersection', 'required_properties_that_are_missing')
                varnames   ('self', 'a', 'b')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_required_properties_that_are_missing__'
-               firstlineno 102
+               firstlineno 112
                lnotab 0x020128012803
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab0100000000000000007d017401000000000000000000007c006a0200
                   00000000000000a6010000ab0100000000000000007d027c01a003000000
                   00000000000000000000000000000000007c02a6010000ab010000000000
                   0000007c005f04000000000000000064015300
-               109           0 RESUME                   0
+               119           0 RESUME                   0
                
-               111           2 LOAD_GLOBAL              1 (NULL + set)
+               121           2 LOAD_GLOBAL              1 (NULL + set)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (missing_properties)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 STORE_FAST               1 (a)
                
-               112          42 LOAD_GLOBAL              1 (NULL + set)
+               122          42 LOAD_GLOBAL              1 (NULL + set)
                             54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                2 (required_properties)
                             66 PRECALL                  1
                             70 CALL                     1
                             80 STORE_FAST               2 (b)
                
-               113          82 LOAD_FAST                1 (a)
+               123          82 LOAD_FAST                1 (a)
                             84 LOAD_METHOD              3 (difference)
                            106 LOAD_FAST                2 (b)
                            108 PRECALL                  1
                            112 CALL                     1
                            122 LOAD_FAST                0 (self)
                            124 STORE_ATTR               4 (optional_properties_that_are_missing)
                            134 LOAD_CONST               1 (None)
@@ -1034,193 +1108,192 @@
                   None
                names      ('set', 'missing_properties', 'required_properties', 'difference', 'optional_properties_that_are_missing')
                varnames   ('self', 'a', 'b')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_optional_properties_that_are_missing__'
-               firstlineno 109
+               firstlineno 119
                lnotab 0x020228012801
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d3e7d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721a7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001008c3f64005300
-               115           0 RESUME                   0
+               125           0 RESUME                   0
                
-               116           2 LOAD_FAST                0 (self)
+               126           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (properties)
                             14 GET_ITER
                        >>   16 FOR_ITER                62 (to 142)
                             18 STORE_FAST               1 (property_)
                
-               117          20 LOAD_FAST                0 (self)
+               127          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (properties)
                             32 LOAD_FAST                1 (property_)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-               118          46 LOAD_FAST                2 (value)
+               128          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (response)
                             58 LOAD_GLOBAL              4 (PropertyResponse)
                             70 LOAD_ATTR                3 (NOT_ENOUGH_CORRECT_STATEMENTS)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    26 (to 140)
                
-               119          88 LOAD_FAST                0 (self)
+               129          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (properties_without_enough_correct_statements)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                1 (property_)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                        >>  140 JUMP_BACKWARD           63 (to 16)
                
-               116     >>  142 LOAD_CONST               0 (None)
+               126     >>  142 LOAD_CONST               0 (None)
                            144 RETURN_VALUE
                consts
                   None
                names      ('properties', 'response', 'PropertyResponse', 'NOT_ENOUGH_CORRECT_STATEMENTS', 'properties_without_enough_correct_statements', 'add')
                varnames   ('self', 'property_', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_properties_with_not_enough_correct_statements__'
-               firstlineno 115
+               firstlineno 125
                lnotab 0x020112011a012a0136fd
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d3e7d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721a7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c01a6010000ab01000000000000000001008c3f64005300
-               121           0 RESUME                   0
+               131           0 RESUME                   0
                
-               122           2 LOAD_FAST                0 (self)
+               132           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (properties)
                             14 GET_ITER
                        >>   16 FOR_ITER                62 (to 142)
                             18 STORE_FAST               1 (property_)
                
-               123          20 LOAD_FAST                0 (self)
+               133          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (properties)
                             32 LOAD_FAST                1 (property_)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-               124          46 LOAD_FAST                2 (value)
+               134          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (necessity)
                             58 LOAD_GLOBAL              4 (Necessity)
                             70 LOAD_ATTR                3 (ABSENT)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    26 (to 140)
                
-               125          88 LOAD_FAST                0 (self)
+               135          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (properties_that_are_not_allowed)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                1 (property_)
                            124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                        >>  140 JUMP_BACKWARD           63 (to 16)
                
-               122     >>  142 LOAD_CONST               0 (None)
+               132     >>  142 LOAD_CONST               0 (None)
                            144 RETURN_VALUE
                consts
                   None
                names      ('properties', 'necessity', 'Necessity', 'ABSENT', 'properties_that_are_not_allowed', 'add')
                varnames   ('self', 'property_', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_properties_that_are_not_allowed__'
-               firstlineno 121
+               firstlineno 131
                lnotab 0x020112011a012a0136fd
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000044005d437d017c006a000000000000
                   0000007c01190000000000000000007d027c026a01000000000000000074
                   04000000000000000000006a0300000000000000006b0200000000721f7c
                   006a040000000000000000a0050000000000000000000000000000000000
                   0000007c026a060000000000000000a6010000ab01000000000000000001
                   008c4464005300
-               127           0 RESUME                   0
+               137           0 RESUME                   0
                
-               128           2 LOAD_FAST                0 (self)
+               138           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (statements)
                             14 GET_ITER
                        >>   16 FOR_ITER                67 (to 152)
                             18 STORE_FAST               1 (statement)
                
-               129          20 LOAD_FAST                0 (self)
+               139          20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                0 (statements)
                             32 LOAD_FAST                1 (statement)
                             34 BINARY_SUBSCR
                             44 STORE_FAST               2 (value)
                
-               130          46 LOAD_FAST                2 (value)
+               140          46 LOAD_FAST                2 (value)
                             48 LOAD_ATTR                1 (necessity)
                             58 LOAD_GLOBAL              4 (Necessity)
                             70 LOAD_ATTR                3 (ABSENT)
                             80 COMPARE_OP               2 (==)
                             86 POP_JUMP_FORWARD_IF_FALSE    31 (to 150)
                
-               131          88 LOAD_FAST                0 (self)
+               141          88 LOAD_FAST                0 (self)
                             90 LOAD_ATTR                4 (statements_with_property_that_is_not_allowed)
                            100 LOAD_METHOD              5 (add)
                            122 LOAD_FAST                2 (value)
                            124 LOAD_ATTR                6 (property)
                            134 PRECALL                  1
                            138 CALL                     1
                            148 POP_TOP
                        >>  150 JUMP_BACKWARD           68 (to 16)
                
-               128     >>  152 LOAD_CONST               0 (None)
+               138     >>  152 LOAD_CONST               0 (None)
                            154 RETURN_VALUE
                consts
                   None
                names      ('statements', 'necessity', 'Necessity', 'ABSENT', 'statements_with_property_that_is_not_allowed', 'add', 'property')
                varnames   ('self', 'statement', 'value')
                freevars   ()
                cellvars   ()
                filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
                name       '__find_statements_with_property_that_is_not_allowed__'
-               firstlineno 127
+               firstlineno 137
                lnotab 0x020112011a012a0140fd
             None
-         names      ('__name__', '__module__', '__qualname__', 'general', 'Dict', 'Any', '__annotations__', 'name', 'str', 'properties', 'PropertyValue', 'statements', 'StatementValue', 'set', 'missing_properties', 'Set', 'required_properties', 'incorrect_statements', 'properties_with_too_many_statements', 'analyzed', 'bool', 'required_properties_that_are_missing', 'optional_properties_that_are_missing', 'properties_without_enough_correct_statements', 'properties_that_are_not_allowed', 'statements_with_property_that_is_not_allowed', 'property', 'some_required_properties_are_missing', 'properties_with_too_many_statements_found', 'incorrect_statements_found', 'properties_without_enough_correct_statements_found', 'statements_with_properties_that_are_not_allowed_found', 'is_valid', 'is_empty', 'analyze', '__find_properties_with_too_many_statements__', '__find_incorrect_statements__', '__find_required_properties__', '__find_missing_properties__', '__find_required_properties_that_are_missing__', '__find_optional_properties_that_are_missing__', '__find_properties_with_not_enough_correct_statements__', '__find_properties_that_are_not_allowed__', '__find_statements_with_property_that_is_not_allowed__')
+         names      ('__name__', '__module__', '__qualname__', 'general', 'Dict', 'Any', '__annotations__', 'name', 'str', 'properties', 'PropertyValue', 'statements', 'StatementValue', 'set', 'missing_properties', 'Set', 'required_properties', 'incorrect_statements', 'missing_statements', 'properties_with_too_many_statements', 'analyzed', 'bool', 'required_properties_that_are_missing', 'optional_properties_that_are_missing', 'properties_without_enough_correct_statements', 'properties_that_are_not_allowed', 'statements_with_property_that_is_not_allowed', 'property', 'some_required_properties_are_missing', 'properties_with_too_many_statements_found', 'incorrect_statements_found', 'properties_without_enough_correct_statements_found', 'statements_with_properties_that_are_not_allowed_found', 'is_valid', 'is_empty', 'analyze', '__find_properties_with_too_many_statements__', '__find_incorrect_statements__', '__find_required_properties__', '__find_missing_properties__', '__find_required_properties_that_are_missing__', '__find_optional_properties_that_are_missing__', '__find_properties_with_not_enough_correct_statements__', '__find_properties_that_are_not_allowed__', '__find_statements_with_property_that_is_not_allowed__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
          name       'Result'
-         firstlineno 10
+         firstlineno 13
          lnotab
-            0x0c011e010e011e011e012a012a012a012a010e012a012a012a012a012a
-            02020104ff0e010203020104ff0e010203020104ff0e010203020104ff0e
-            010203020104ff0e01020302010aff0e01020e020104ff0e010203060d06
-            060606060606060607060606060606
+            0x0c011e010e011e011e012a012a012a012a012a010e012a012a012a012a
+            012a02020104ff0e010203020104ff0e010203020104ff0e010203020104
+            ff0e010203020104ff0e01020302010aff0e01020e020104ff0e01020306
+            0d0606060c060606060607060606060606
       'Result'
-      None
-   names      ('typing', 'Any', 'Dict', 'Set', 'pydantic', 'BaseModel', 'Field', 'entityshape.enums', 'Necessity', 'PropertyResponse', 'StatementResponse', 'entityshape.models.property_value', 'PropertyValue', 'entityshape.models.statement_value', 'StatementValue', 'Result')
+   names      ('logging', 'typing', 'Any', 'Dict', 'Set', 'pydantic', 'BaseModel', 'ValidationError', 'entityshape.enums', 'Necessity', 'PropertyResponse', 'StatementResponse', 'entityshape.models.property_value', 'PropertyValue', 'entityshape.models.statement_value', 'StatementValue', 'getLogger', '__name__', 'logger', 'Result')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/dpriskorn/PycharmProjects/entityshape/entityshape/models/result.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02011402100214010c010c03
+   lnotab 0x00ff020108011402100214010c010c022003
```

### Comparing `entityshape-0.0.1/entityshape/models/__pycache__/shape.cpython-311.pyc` & `entityshape-0.0.2/entityshape/models/__pycache__/shape.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x8fa99564 (Fri Jun 23 14:17:51 2023 UTC)
+moddate:  0x8cb99564 (Fri Jun 23 15:26:04 2023 UTC)
 files sz: 14070
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `entityshape-0.0.1/entityshape/models/__pycache__/shape_claim.cpython-311.pyc` & `entityshape-0.0.2/entityshape/models/__pycache__/shape_claim.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.1/entityshape/models/compareshape.py` & `entityshape-0.0.2/entityshape/models/compareshape.py`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.1/entityshape/models/result.py` & `entityshape-0.0.2/entityshape/models/result.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,28 @@
+import logging
 from typing import Any, Dict, Set
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ValidationError
 
 from entityshape.enums import Necessity, PropertyResponse, StatementResponse
 from entityshape.models.property_value import PropertyValue
 from entityshape.models.statement_value import StatementValue
 
+logger = logging.getLogger(__name__)
+
 
 class Result(BaseModel):
     general: Dict[Any, Any] = {}
     name: str = ""
     properties: Dict[str, PropertyValue] = {}
     statements: Dict[Any, StatementValue] = {}
     missing_properties: Set[str] = set()
     required_properties: Set[str] = set()
     incorrect_statements: Set[str] = set()
+    missing_statements: Set[str] = set()
     properties_with_too_many_statements: Set[str] = set()
     analyzed: bool = False
     required_properties_that_are_missing: Set[str] = set()
     optional_properties_that_are_missing: Set[str] = set()
     properties_without_enough_correct_statements: Set[str] = set()
     properties_that_are_not_allowed: Set[str] = set()
     statements_with_property_that_is_not_allowed: Set[str] = set()
@@ -80,16 +84,22 @@
             value: PropertyValue = self.properties[property_]
             if value.response == PropertyResponse.TOO_MANY_STATEMENTS:
                 self.properties_with_too_many_statements.add(property_)
 
     def __find_incorrect_statements__(self):
         for statement in self.statements:
             value: StatementValue = self.statements[statement]
-            if value.response == StatementResponse.INCORRECT:
-                self.incorrect_statements.add(statement)
+            try:
+                StatementResponse(value.response)
+                if value.response == StatementResponse.INCORRECT:
+                    self.incorrect_statements.add(statement)
+            except ValueError:
+                # Ignore responses we cannot predict
+                logger.warning(f"Ignoring statement response: {value.response}")
+                pass
 
     def __find_required_properties__(self):
         for property_ in self.properties:
             value: PropertyValue = self.properties[property_]
             if value.necessity == Necessity.REQUIRED:
                 self.required_properties.add(property_)
```

### Comparing `entityshape-0.0.1/entityshape/models/shape.py` & `entityshape-0.0.2/entityshape/models/shape.py`

 * *Files identical despite different names*

### Comparing `entityshape-0.0.1/pyproject.toml` & `entityshape-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Entityshape"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python library to validate Wikidata items."
 authors = ["Mark Tully aka Teester", "Dennis Priskorn <68460690+dpriskorn@users.noreply.github.com>"]
 license = "GPLv3+"
 readme = "README.md"
 repository = "https://github.com/dpriskorn/entityshape"
 keywords = ["wikidata", "entityschema", "entity validation"]
 classifiers = [
@@ -14,17 +14,17 @@
     { include = "entityshape" },
 ]
 
 [tool.poetry.dependencies]
 pydantic = "^1.10.9"
 python = ">=3.8,<=3.12"
 requests = "^2.28.1"
-# wikibaseintegrator = "^0.12.1"
 
 [tool.poetry.group.dev.dependencies]
+rich = "^13.4.2"
 black = "^22.8.0"
 codespell = "^2.2.1"
 coverage = "^6.5.0"
 dead = "^1.5.0"
 mypy = "^1.1.1"
 pre-commit = "^2.20.0"
 pytest = "^7.1.3"
```

### Comparing `entityshape-0.0.1/PKG-INFO` & `entityshape-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entityshape
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python library to validate Wikidata items.
 Home-page: https://github.com/dpriskorn/entityshape
 License: GPLv3+
 Keywords: wikidata,entityschema,entity validation
 Author: Mark Tully aka Teester
 Requires-Python: >=3.8,<=3.12
 Classifier: License :: Other/Proprietary License
@@ -25,14 +25,22 @@
 Based on https://github.com/Teester/entityshape by Mark Tully 
 and https://github.com/dpriskorn/PyEntityshape by Dennis Priskorn
 
 # Features
 * compare a given wikidata item with an entityschema and dig into missing properties, too many statement, etc.
 * determine whether an item is valid according to a certain schema or not
 
+# Limitations
+The shape and compareshape classes currently only support:
+* cardinality (too many or not enough values)
+* whether the property is allowed or not
+* whether the value of a statement on a given property is correct/incorrect
+
+It is still a bit unclear if and how the qualifier validation works.
+
 # Installation
 Get it from pypi
 
 `$ pip install pyentityshape`
 
 # Usage
 Example:
```

