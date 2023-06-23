# Comparing `tmp/pycsbinarywriter-0.0.4.tar.gz` & `tmp/pycsbinarywriter-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycsbinarywriter-0.0.4.tar", max compression
+gzip compressed data, was "pycsbinarywriter-0.1.0.tar", max compression
```

## Comparing `pycsbinarywriter-0.0.4.tar` & `pycsbinarywriter-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1072 2022-06-15 23:10:16.533160 pycsbinarywriter-0.0.4/LICENSE
--rw-r--r--   0        0        0      555 2022-06-15 23:09:50.657374 pycsbinarywriter-0.0.4/README.md
--rw-r--r--   0        0        0        0 2021-01-26 00:59:15.546467 pycsbinarywriter-0.0.4/pycsbinarywriter/__init__.py
--rw-r--r--   0        0        0      129 2022-10-06 23:55:24.113631 pycsbinarywriter-0.0.4/pycsbinarywriter/consts.py
--rw-r--r--   0        0        0     2800 2022-06-15 22:49:49.635167 pycsbinarywriter-0.0.4/pycsbinarywriter/csharpserializable.py
--rw-r--r--   0        0        0      106 2022-06-15 22:52:03.367104 pycsbinarywriter-0.0.4/pycsbinarywriter/cstypes/__init__.py
--rw-r--r--   0        0        0     1352 2022-06-15 22:51:54.503108 pycsbinarywriter-0.0.4/pycsbinarywriter/cstypes/cstype.py
--rw-r--r--   0        0        0     6960 2022-06-15 22:51:36.735115 pycsbinarywriter-0.0.4/pycsbinarywriter/cstypes/decimal.py
--rw-r--r--   0        0        0     1514 2022-06-15 22:51:02.895130 pycsbinarywriter-0.0.4/pycsbinarywriter/cstypes/seven_bit_int.py
--rw-r--r--   0        0        0     1614 2022-10-06 23:55:24.013632 pycsbinarywriter-0.0.4/pycsbinarywriter/cstypes/simple.py
--rw-r--r--   0        0        0     3003 2022-06-15 22:50:28.199146 pycsbinarywriter-0.0.4/pycsbinarywriter/cstypes/strings.py
--rw-r--r--   0        0        0      148 2021-01-26 00:59:15.550467 pycsbinarywriter-0.0.4/pycsbinarywriter/test/__init__.py
--rw-r--r--   0        0        0     5402 2022-10-06 23:55:24.105631 pycsbinarywriter-0.0.4/pycsbinarywriter/test/simple.py
--rw-r--r--   0        0        0     1565 2022-06-15 22:58:01.038200 pycsbinarywriter-0.0.4/pycsbinarywriter/test/strings.py
--rw-r--r--   0        0        0      680 2022-10-06 23:55:19.217692 pycsbinarywriter-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1367 1970-01-01 00:00:00.000000 pycsbinarywriter-0.0.4/setup.py
--rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 pycsbinarywriter-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-06-15 23:10:16.533160 pycsbinarywriter-0.1.0/LICENSE
+-rw-r--r--   0        0        0      721 2023-06-23 19:07:53.543053 pycsbinarywriter-0.1.0/README.md
+-rw-r--r--   0        0        0       48 2023-06-23 21:58:59.304345 pycsbinarywriter-0.1.0/pycsbinarywriter/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-23 21:58:22.228527 pycsbinarywriter-0.1.0/pycsbinarywriter/consts.py
+-rw-r--r--   0        0        0     2895 2023-06-23 21:54:32.701665 pycsbinarywriter-0.1.0/pycsbinarywriter/csharpserializable.py
+-rw-r--r--   0        0        0      106 2022-06-15 22:52:03.367104 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/__init__.py
+-rw-r--r--   0        0        0     2093 2023-06-23 19:45:47.670489 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/cstype.py
+-rw-r--r--   0        0        0     3917 2023-06-23 21:53:32.829965 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/decimal.py
+-rw-r--r--   0        0        0     2489 2023-06-23 21:43:21.333176 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/seven_bit_int.py
+-rw-r--r--   0        0        0     1615 2023-06-23 21:58:22.152527 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/simple.py
+-rw-r--r--   0        0        0     4412 2023-06-23 21:43:11.093234 pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/strings.py
+-rw-r--r--   0        0        0      148 2021-01-26 00:59:15.550467 pycsbinarywriter-0.1.0/pycsbinarywriter/test/__init__.py
+-rw-r--r--   0        0        0     5411 2023-06-23 21:58:22.224527 pycsbinarywriter-0.1.0/pycsbinarywriter/test/simple.py
+-rw-r--r--   0        0        0     1565 2022-06-15 22:58:01.038200 pycsbinarywriter-0.1.0/pycsbinarywriter/test/strings.py
+-rw-r--r--   0        0        0      800 2023-06-23 19:36:17.833631 pycsbinarywriter-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1383 1970-01-01 00:00:00.000000 pycsbinarywriter-0.1.0/PKG-INFO
```

### Comparing `pycsbinarywriter-0.0.4/LICENSE` & `pycsbinarywriter-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycsbinarywriter-0.0.4/pycsbinarywriter/csharpserializable.py` & `pycsbinarywriter-0.1.0/pycsbinarywriter/csharpserializable.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 import pytz
 
 from pycsbinarywriter import cstypes
 from pycsbinarywriter.cstypes.simple import SimpleCSType
 
 NUL: bytes = bytes([0x00])
 
-
+'''
+Don't worry, I am still debating whether this class should still exist. :weeping-smile:
+'''
 class CSharpSerializable(object):
     def __init__(self) -> None:
         self.pos: int = 0
         self.fh: BinaryIO = None
 
     def unpackSpecified(self, cstype: SimpleCSType) -> Any:
         sz: int = cstype.calcsize()
```

### Comparing `pycsbinarywriter-0.0.4/pycsbinarywriter/cstypes/cstype.py` & `pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/cstype.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from asyncio import StreamReader, StreamWriter
 import struct
 from typing import Type, TypeVar, Generic, BinaryIO, Optional
 
-__all__ = ['CSTypes']
+__all__ = ['BaseCSType', 'SimpleCSType']
 
 T = TypeVar('T')
 
 
 class BaseCSType(Generic[T]):
     def __init__(self, name: str, pytype: Type) -> None:
         self.name: str = name
@@ -13,20 +14,29 @@
 
     def unpack(self, data: bytes) -> Optional[T]:
         return None
 
     def pack(self, value: T) -> bytes:
         return b''
 
+    def packTo(self, value: T, f: BinaryIO) -> None:
+        pass
+
+    async def asyncPackTo(self, value: T, f: StreamWriter) -> None:
+        pass
+
     def calcsize(self) -> int:
         return -1
 
     def unpackFrom(self, f: BinaryIO) -> Optional[T]:
         return None
 
+    async def asyncUnpackFrom(self, f: StreamReader) -> Optional[T]:
+        return None
+
 
 class SimpleCSType(BaseCSType[T]):
     def __init__(self, name: str, fmt: str, size: int, pytype: Type) -> None:
         super().__init__(name, pytype)
         self.format: str = fmt
         self.size: int = size
 
@@ -35,14 +45,27 @@
         if len(data) < sz:
             return None
         return struct.unpack(self.format, data[:sz])[0]
 
     def pack(self, value: T) -> bytes:
         return struct.pack(self.format, value)
 
+    def packTo(self, value: T, f: BinaryIO) -> None:
+        f.write(self.pack(value))
+
+    async def asyncPackTo(self, value: T, f: StreamWriter) -> None:
+        f.write(self.pack(value))
+
+    async def asyncUnpackFrom(self, f: StreamReader) -> Optional[T]:
+        sz: int = self.calcsize()
+        data: bytes = await f.read(sz)
+        if len(data) < sz:
+            return None
+        return struct.unpack(self.format, data)[0]
+
     def calcsize(self) -> int:
         return self.size if self.size > 0 else struct.calcsize(self.format)
 
     def unpackFrom(self, f: BinaryIO) -> Optional[T]:
         sz: int = self.calcsize()
         data: bytes = f.read(sz)
         if len(data) < sz:
```

### Comparing `pycsbinarywriter-0.0.4/pycsbinarywriter/cstypes/simple.py` & `pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/simple.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # @GENERATED by build/buildTypes.py (see data/types.yml)
-# Generated at 2022-10-06T23:55:23.990860+00:00
+# Generated at 2023-06-23T21:58:22.121936+00:00
 import builtins
 from pycsbinarywriter.cstypes.cstype import SimpleCSType
-__all__ = ['bool', 'double', 'float', 'int16', 'int32', 'int64', 'int8', 'uint16', 'uint32', 'uint64', 'uint8']
-uint8: SimpleCSType[builtins.int] = SimpleCSType('uint8', '<B', 1, builtins.int)
+
+__all__ = ["bool", "double", "float", "int16", "int32", "int64", "int8", "uint16", "uint32", "uint64", "uint8"]
+uint8: SimpleCSType[builtins.int] = SimpleCSType("uint8", "<B", 1, builtins.int)
 byte: SimpleCSType[builtins.int] = uint8
-int8: SimpleCSType[builtins.int] = SimpleCSType('int8', '<b', 1, builtins.int)
+int8: SimpleCSType[builtins.int] = SimpleCSType("int8", "<b", 1, builtins.int)
 sbyte: SimpleCSType[builtins.int] = int8
-int16: SimpleCSType[builtins.int] = SimpleCSType('int16', '<h', 2, builtins.int)
+int16: SimpleCSType[builtins.int] = SimpleCSType("int16", "<h", 2, builtins.int)
 short: SimpleCSType[builtins.int] = int16
-uint16: SimpleCSType[builtins.int] = SimpleCSType('uint16', '<H', 2, builtins.int)
+uint16: SimpleCSType[builtins.int] = SimpleCSType("uint16", "<H", 2, builtins.int)
 ushort: SimpleCSType[builtins.int] = uint16
-int32: SimpleCSType[builtins.int] = SimpleCSType('int32', '<i', 4, builtins.int)
+int32: SimpleCSType[builtins.int] = SimpleCSType("int32", "<i", 4, builtins.int)
 int: SimpleCSType[builtins.int] = int32
-uint32: SimpleCSType[builtins.int] = SimpleCSType('uint32', '<I', 4, builtins.int)
+uint32: SimpleCSType[builtins.int] = SimpleCSType("uint32", "<I", 4, builtins.int)
 uint: SimpleCSType[builtins.int] = uint32
-int64: SimpleCSType[builtins.int] = SimpleCSType('int64', '<q', 8, builtins.int)
+int64: SimpleCSType[builtins.int] = SimpleCSType("int64", "<q", 8, builtins.int)
 long: SimpleCSType[builtins.int] = int64
-uint64: SimpleCSType[builtins.int] = SimpleCSType('uint64', '<Q', 8, builtins.int)
+uint64: SimpleCSType[builtins.int] = SimpleCSType("uint64", "<Q", 8, builtins.int)
 ulong: SimpleCSType[builtins.int] = uint64
-float: SimpleCSType[builtins.float] = SimpleCSType('float', 'f', 4, builtins.float)
+float: SimpleCSType[builtins.float] = SimpleCSType("float", "f", 4, builtins.float)
 single: SimpleCSType[builtins.float] = float
-double: SimpleCSType[builtins.float] = SimpleCSType('double', 'd', 8, builtins.float)
-bool: SimpleCSType[builtins.bool] = SimpleCSType('bool', '<?', 1, builtins.bool)
+double: SimpleCSType[builtins.float] = SimpleCSType("double", "d", 8, builtins.float)
+bool: SimpleCSType[builtins.bool] = SimpleCSType("bool", "<?", 1, builtins.bool)
 bool_: SimpleCSType[builtins.bool] = bool
```

### Comparing `pycsbinarywriter-0.0.4/pycsbinarywriter/cstypes/strings.py` & `pycsbinarywriter-0.1.0/pycsbinarywriter/cstypes/strings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import struct
+from asyncio import StreamReader, StreamWriter
 from typing import BinaryIO, Optional
 
-from .cstype import BaseCSType
-from .seven_bit_int import int7
+from pycsbinarywriter.cstypes.cstype import BaseCSType
+from pycsbinarywriter.cstypes.seven_bit_int import int7
 
 __all__ = ['char', 'cstring', 'string']
 
 
 class CharType(BaseCSType[str]):
     def __init__(self) -> None:
         super().__init__('char', str)
@@ -22,15 +23,22 @@
     def pack(self, value: str) -> bytes:
         return struct.pack('<b', ord(value[0]))
 
     def unpackFrom(self, f: BinaryIO) -> Optional[str]:
         data: bytes = f.read(1)
         if len(data) < 1:
             return None
-        return struct.unpack(self.format, data)[0]
+        return struct.unpack('<b', data)[0]
+
+    async def asyncPackTo(self, value: str, f: StreamWriter) -> None:
+        f.write(self.pack(value))
+
+    async def asyncUnpackFrom(self, f: StreamReader) -> Optional[str]:
+        data: bytes = await f.readexactly(1)
+        return struct.unpack('<b', data)[0]
 
 
 class CStringType(BaseCSType[str]):
     def __init__(self) -> None:
         super().__init__('cstring', str)
         self.bytesRead: int = 0
 
@@ -50,34 +58,48 @@
 
     def pack(self, value: str, encoding='utf-8') -> bytes:
         return value.encode(encoding)+b'\x00'
 
     def calcsize(self) -> int:
         return -1
 
-    def unpackFrom(self, f: BinaryIO, encoding='utf-8') -> Optional[str]:
+    def unpackFrom(self, f: BinaryIO, encoding: str = 'utf-8') -> Optional[str]:
         self.bytesRead = 0
         buffer = b''
         while True:
             b = f.read(1)
             if b is None:
                 break
             self.bytesRead += 1
             if b == b'\x00':
                 break
             buffer += b
         return buffer.decode(encoding)
 
+    async def asyncPackTo(self, value: str, f: StreamWriter, encoding: str = 'utf-8') -> None:
+        f.write(self.pack(value, encoding=encoding))
+
+    async def asyncUnpackFrom(self, f: StreamReader, encoding: str = 'utf-8') -> Optional[str]:
+        self.bytesRead = 0
+        buffer = b''
+        while True:
+            b = await f.readexactly(1)
+            self.bytesRead += 1
+            if b == b'\x00':
+                break
+            buffer += b
+        return buffer.decode(encoding)
+
 
 class CSStringType(BaseCSType[str]):
     def __init__(self) -> None:
         super().__init__('string', str)
         self.bytesRead: int = 0
 
-    def unpack(self, data: bytes, start: int = 0, encoding='utf-8') -> Optional[str]:
+    def unpack(self, data: bytes, start: int = 0, encoding: str = 'utf-8') -> Optional[str]:
         self.bytesRead = 0
         nbytes: int = int7.unpack(data, start)
         self.bytesRead += int7.bytesRead
         start += int7.bytesRead
         ob: bytes = data[start:start+nbytes]
         assert len(ob) == nbytes
         o: str = data[start:start+nbytes].decode(encoding)
@@ -86,22 +108,36 @@
 
     def pack(self, value: str, encoding='utf-8') -> bytes:
         return int7.pack(len(value))+value.encode(encoding)
 
     def calcsize(self) -> int:
         return -1
 
-    def unpackFrom(self, f: BinaryIO, encoding='utf-8') -> Optional[str]:
+    def unpackFrom(self, f: BinaryIO, encoding: str = 'utf-8') -> Optional[str]:
         self.bytesRead = 0
         nbytes = int7.unpackFrom(f)
         self.bytesRead += int7.bytesRead
 
         ob: bytes = f.read(nbytes)
         assert len(ob) == nbytes
         o: str = ob.decode(encoding)
         self.bytesRead += nbytes
         return o
 
+    async def asyncPackTo(self, value: str, f: StreamWriter, encoding: str = 'utf-8') -> None:
+        f.write(self.pack(value, encoding=encoding))
+
+    async def asyncUnpackFrom(self, f: StreamReader, encoding: str = 'utf-8') -> Optional[str]:
+        self.bytesRead = 0
+        nbytes: int = await int7.asyncUnpackFrom(f)
+        self.bytesRead += int7.bytesRead
+
+        ob: bytes = await f.readexactly(nbytes)
+        assert len(ob) == nbytes
+        o: str = ob.decode(encoding)
+        self.bytesRead += nbytes
+        return o
+
 
 char: CharType = CharType()
 cstring: CStringType = CStringType()
 string: CSStringType = CSStringType()
```

### Comparing `pycsbinarywriter-0.0.4/pycsbinarywriter/test/simple.py` & `pycsbinarywriter-0.1.0/pycsbinarywriter/test/simple.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,145 +1,145 @@
 # @GENERATED by build/buildTypes.py (see data/types.yml)
-# Generated at 2022-10-06T23:55:24.018021+00:00
+# Generated at 2023-06-23T21:58:22.154918+00:00
 import builtins
 import unittest
 from pycsbinarywriter import cstypes
-__all__ = ['TestSimpleSerializers']
+
+__all__ = ["TestSimpleSerializers"]
 
 
 class TestSimpleSerializers(unittest.TestCase):
     def test_uint8_pack(self) -> None:
         input_value: builtins.int = 127
-        expected: bytes = b'\x7f'
+        expected: bytes = b"\x7f"
         actual: bytes = cstypes.uint8.pack(input_value)
         self.assertEqual(actual, expected)
 
     def test_uint8_unpack(self) -> None:
-        input_bytes: bytes = b'\x7f'
+        input_bytes: bytes = b"\x7f"
         expected: builtins.int = 127
-        actual: bytes = cstypes.uint8.unpack(input_bytes)
+        actual: builtins.int = cstypes.uint8.unpack(input_bytes)
         self.assertEqual(actual, expected)
 
     def test_int8_pack(self) -> None:
         input_value: builtins.int = -127
-        expected: bytes = b'\x81'
+        expected: bytes = b"\x81"
         actual: bytes = cstypes.int8.pack(input_value)
         self.assertEqual(actual, expected)
 
     def test_int8_unpack(self) -> None:
-        input_bytes: bytes = b'\x81'
+        input_bytes: bytes = b"\x81"
         expected: builtins.int = -127
-        actual: bytes = cstypes.int8.unpack(input_bytes)
+        actual: builtins.int = cstypes.int8.unpack(input_bytes)
         self.assertEqual(actual, expected)
 
     def test_int16_pack(self) -> None:
         input_value: builtins.int = -1234
-        expected: bytes = b'\x2e\xfb'
+        expected: bytes = b".\xfb"
         actual: bytes = cstypes.int16.pack(input_value)
         self.assertEqual(actual, expected)
 
     def test_int16_unpack(self) -> None:
-        input_bytes: bytes = b'\x2e\xfb'
+        input_bytes: bytes = b".\xfb"
         expected: builtins.int = -1234
-        actual: bytes = cstypes.int16.unpack(input_bytes)
+        actual: builtins.int = cstypes.int16.unpack(input_bytes)
         self.assertEqual(actual, expected)
 
     def test_uint16_pack(self) -> None:
         input_value: builtins.int = 1234
-        expected: bytes = b'\xd2\x04'
+        expected: bytes = b"\xd2\x04"
         actual: bytes = cstypes.uint16.pack(input_value)
         self.assertEqual(actual, expected)
 
     def test_uint16_unpack(self) -> None:
-        input_bytes: bytes = b'\xd2\x04'
+        input_bytes: bytes = b"\xd2\x04"
         expected: builtins.int = 1234
-        actual: bytes = cstypes.uint16.unpack(input_bytes)
+        actual: builtins.int = cstypes.uint16.unpack(input_bytes)
         self.assertEqual(actual, expected)
 
     def test_int32_pack(self) -> None:
         input_value: builtins.int = -1234567
-        expected: bytes = b'\x79\x29\xed\xff'
+        expected: bytes = b"y)\xed\xff"
         actual: bytes = cstypes.int32.pack(input_value)
         self.assertEqual(actual, expected)
 
     def test_int32_unpack(self) -> None:
-        input_bytes: bytes = b'\x79\x29\xed\xff'
+        input_bytes: bytes = b"y)\xed\xff"
         expected: builtins.int = -1234567
-        actual: bytes = cstypes.int32.unpack(input_bytes)
+        actual: builtins.int = cstypes.int32.unpack(input_bytes)
         self.assertEqual(actual, expected)
 
     def test_uint32_pack(self) -> None:
         input_value: builtins.int = 1234567
-        expected: bytes = b'\x87\xd6\x12\x00'
+        expected: bytes = b"\x87\xd6\x12\x00"
         actual: bytes = cstypes.uint32.pack(input_value)
         self.assertEqual(actual, expected)
 
     def test_uint32_unpack(self) -> None:
-        input_bytes: bytes = b'\x87\xd6\x12\x00'
+        input_bytes: bytes = b"\x87\xd6\x12\x00"
         expected: builtins.int = 1234567
-        actual: bytes = cstypes.uint32.unpack(input_bytes)
+        actual: builtins.int = cstypes.uint32.unpack(input_bytes)
         self.assertEqual(actual, expected)
 
     def test_int64_pack(self) -> None:
         input_value: builtins.int = -1234567890
-        expected: bytes = b'\x2e\xfd\x69\xb6\xff\xff\xff\xff'
+        expected: bytes = b".\xfdi\xb6\xff\xff\xff\xff"
         actual: bytes = cstypes.int64.pack(input_value)
         self.assertEqual(actual, expected)
 
     def test_int64_unpack(self) -> None:
-        input_bytes: bytes = b'\x2e\xfd\x69\xb6\xff\xff\xff\xff'
+        input_bytes: bytes = b".\xfdi\xb6\xff\xff\xff\xff"
         expected: builtins.int = -1234567890
-        actual: bytes = cstypes.int64.unpack(input_bytes)
+        actual: builtins.int = cstypes.int64.unpack(input_bytes)
         self.assertEqual(actual, expected)
 
     def test_uint64_pack(self) -> None:
         input_value: builtins.int = 1234567890
-        expected: bytes = b'\xd2\x02\x96\x49\x00\x00\x00\x00'
+        expected: bytes = b"\xd2\x02\x96I\x00\x00\x00\x00"
         actual: bytes = cstypes.uint64.pack(input_value)
         self.assertEqual(actual, expected)
 
     def test_uint64_unpack(self) -> None:
-        input_bytes: bytes = b'\xd2\x02\x96\x49\x00\x00\x00\x00'
+        input_bytes: bytes = b"\xd2\x02\x96I\x00\x00\x00\x00"
         expected: builtins.int = 1234567890
-        actual: bytes = cstypes.uint64.unpack(input_bytes)
+        actual: builtins.int = cstypes.uint64.unpack(input_bytes)
         self.assertEqual(actual, expected)
 
     def test_float_pack(self) -> None:
         input_value: builtins.float = 1.5
-        expected: bytes = b'\x00\x00\xc0\x3f'
+        expected: bytes = b"\x00\x00\xc0?"
         actual: bytes = cstypes.float.pack(input_value)
         self.assertEqual(actual, expected)
 
     def test_float_unpack(self) -> None:
-        input_bytes: bytes = b'\x00\x00\xc0\x3f'
+        input_bytes: bytes = b"\x00\x00\xc0?"
         expected: builtins.float = 1.5
-        actual: bytes = cstypes.float.unpack(input_bytes)
+        actual: builtins.float = cstypes.float.unpack(input_bytes)
         self.assertEqual(actual, expected)
 
     def test_double_pack(self) -> None:
         input_value: builtins.float = 1.0000005
-        expected: bytes = b'\x06\xbd\x37\x86\x00\x00\xf0\x3f'
+        expected: bytes = b"\x06\xbd7\x86\x00\x00\xf0?"
         actual: bytes = cstypes.double.pack(input_value)
         self.assertEqual(actual, expected)
 
     def test_double_unpack(self) -> None:
-        input_bytes: bytes = b'\x06\xbd\x37\x86\x00\x00\xf0\x3f'
+        input_bytes: bytes = b"\x06\xbd7\x86\x00\x00\xf0?"
         expected: builtins.float = 1.0000005
-        actual: bytes = cstypes.double.unpack(input_bytes)
+        actual: builtins.float = cstypes.double.unpack(input_bytes)
         self.assertEqual(actual, expected)
 
     def test_bool_pack(self) -> None:
         input_value: builtins.bool = True
-        expected: bytes = b'\x01'
+        expected: bytes = b"\x01"
         actual: bytes = cstypes.bool.pack(input_value)
         self.assertEqual(actual, expected)
 
     def test_bool_unpack(self) -> None:
-        input_bytes: bytes = b'\x01'
+        input_bytes: bytes = b"\x01"
         expected: builtins.bool = True
-        actual: bytes = cstypes.bool.unpack(input_bytes)
+        actual: builtins.bool = cstypes.bool.unpack(input_bytes)
         self.assertEqual(actual, expected)
 
 
-if __name__ == '__main__':
-    import unittest
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `pycsbinarywriter-0.0.4/pycsbinarywriter/test/strings.py` & `pycsbinarywriter-0.1.0/pycsbinarywriter/test/strings.py`

 * *Files identical despite different names*

### Comparing `pycsbinarywriter-0.0.4/pyproject.toml` & `pycsbinarywriter-0.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "pycsbinarywriter"
-version = "0.0.4"
-description = "Helpers for parsing binary data created by dotnet BinaryWriters."
+version = "0.1.0"
+description = "Helpers for parsing and writing binary data created by dotnet System.IO.BinaryWriters."
 authors = ["Rob Nelson <nexisentertainment@gmail.com>"]
 license = "MIT"
 readme="README.md"
 repository="https://gitlab.com/N3X15/pycsbinarywriter"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-pytz = "^2022.2.1"
-
-[tool.poetry.dev-dependencies]
-isort = "^5.10.1"
-mypy = "^0.971"
-autopep8 = "^1.7.0"
-pybuildtools = "^0.5.3"
-"ruamel.yaml" = "^0.17.21"
-poetryup = "^0.12.0"
-twine = "^4.0.1"
+python = ">=3.10,<4.0"
+pytz = "^2023.3"
 
 [tool.poetry.group.dev.dependencies]
-poetryup = "^0.12.2"
+isort = "^5.12.0"
+mypy = {extras = ["d"], version = "^1.4.0"}
+autopep8 = "^2.0.2"
+pybuildtools = "^0.5.12"
+"ruamel.yaml" = "^0.17.32"
+twine = "^4.0.2"
+mkast = {git = "https://gitlab.com/N3X15/python-mkast.git"}
+astor = "^0.8.1"
+black = {extras = ["d"], version = "^23.3.0"}
+autoflake = "^2.1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pycsbinarywriter-0.0.4/PKG-INFO` & `pycsbinarywriter-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: pycsbinarywriter
-Version: 0.0.4
-Summary: Helpers for parsing binary data created by dotnet BinaryWriters.
+Version: 0.1.0
+Summary: Helpers for parsing and writing binary data created by dotnet System.IO.BinaryWriters.
 Home-page: https://gitlab.com/N3X15/pycsbinarywriter
 License: MIT
 Author: Rob Nelson
 Author-email: nexisentertainment@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: pytz (>=2022.2.1,<2023.0.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pytz (>=2023.3,<2024.0)
 Project-URL: Repository, https://gitlab.com/N3X15/pycsbinarywriter
 Description-Content-Type: text/markdown
 
 # pyCSBinaryWriter
 
 A simple library for .NET binary (de)serialization.
 
+This package gives developers access to simple method calls from decoding
+binary data written by .NET BinaryWriter.
+
 ## Limitations
 
 * Decimal is not implemented yet. Pull requests are welcome.
+* asyncio support is brand new and may be buggy.
 
 ## Installation
 
 ```shell
 $ pip install -U pycsbinarywriter
 ```
```

