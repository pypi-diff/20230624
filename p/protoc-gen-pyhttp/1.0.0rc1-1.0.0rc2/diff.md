# Comparing `tmp/protoc_gen_pyhttp-1.0.0rc1-py3-none-any.whl.zip` & `tmp/protoc_gen_pyhttp-1.0.0rc2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 12059 bytes, number of entries: 11
+Zip file size: 12063 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-13 12:15 protoc_gen_pyhttp/__init__.py
 -rw-rw-rw-  2.0 fat    12894 b- defN 23-Jun-13 12:17 protoc_gen_pyhttp/http.py
--rw-rw-rw-  2.0 fat      922 b- defN 23-Jun-13 12:17 protoc_gen_pyhttp/main.py
--rw-rw-rw-  2.0 fat     6411 b- defN 23-Jun-13 12:15 protoc_gen_pyhttp/template.py
+-rw-rw-rw-  2.0 fat      928 b- defN 23-Jun-24 08:19 protoc_gen_pyhttp/main.py
+-rw-rw-rw-  2.0 fat     6431 b- defN 23-Jun-24 08:22 protoc_gen_pyhttp/template.py
 -rw-rw-rw-  2.0 fat      665 b- defN 23-Jun-13 12:15 protoc_gen_pyhttp/util.py
--rw-rw-rw-  2.0 fat    11357 b- defN 23-Jun-13 12:23 protoc_gen_pyhttp-1.0.0rc1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      488 b- defN 23-Jun-13 12:23 protoc_gen_pyhttp-1.0.0rc1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-13 12:23 protoc_gen_pyhttp-1.0.0rc1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       66 b- defN 23-Jun-13 12:23 protoc_gen_pyhttp-1.0.0rc1.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-13 12:23 protoc_gen_pyhttp-1.0.0rc1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      973 b- defN 23-Jun-13 12:23 protoc_gen_pyhttp-1.0.0rc1.dist-info/RECORD
-11 files, 33886 bytes uncompressed, 10381 bytes compressed:  69.4%
+-rw-rw-rw-  2.0 fat    11357 b- defN 23-Jun-24 08:27 protoc_gen_pyhttp-1.0.0rc2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      488 b- defN 23-Jun-24 08:27 protoc_gen_pyhttp-1.0.0rc2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-24 08:27 protoc_gen_pyhttp-1.0.0rc2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       66 b- defN 23-Jun-24 08:27 protoc_gen_pyhttp-1.0.0rc2.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-24 08:27 protoc_gen_pyhttp-1.0.0rc2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      973 b- defN 23-Jun-24 08:27 protoc_gen_pyhttp-1.0.0rc2.dist-info/RECORD
+11 files, 33912 bytes uncompressed, 10385 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: protoc_gen_pyhttp/template.py
 Comment: 
 
 Filename: protoc_gen_pyhttp/util.py
 Comment: 
 
-Filename: protoc_gen_pyhttp-1.0.0rc1.dist-info/LICENSE
+Filename: protoc_gen_pyhttp-1.0.0rc2.dist-info/LICENSE
 Comment: 
 
-Filename: protoc_gen_pyhttp-1.0.0rc1.dist-info/METADATA
+Filename: protoc_gen_pyhttp-1.0.0rc2.dist-info/METADATA
 Comment: 
 
-Filename: protoc_gen_pyhttp-1.0.0rc1.dist-info/WHEEL
+Filename: protoc_gen_pyhttp-1.0.0rc2.dist-info/WHEEL
 Comment: 
 
-Filename: protoc_gen_pyhttp-1.0.0rc1.dist-info/entry_points.txt
+Filename: protoc_gen_pyhttp-1.0.0rc2.dist-info/entry_points.txt
 Comment: 
 
-Filename: protoc_gen_pyhttp-1.0.0rc1.dist-info/top_level.txt
+Filename: protoc_gen_pyhttp-1.0.0rc2.dist-info/top_level.txt
 Comment: 
 
-Filename: protoc_gen_pyhttp-1.0.0rc1.dist-info/RECORD
+Filename: protoc_gen_pyhttp-1.0.0rc2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## protoc_gen_pyhttp/main.py

```diff
@@ -5,31 +5,29 @@
 from google.protobuf.descriptor_pool import DescriptorPool
 
 if __package__ is None and not hasattr(sys, "frozen"):
     path = os.path.realpath(os.path.abspath(__file__))
     sys.path.insert(0, os.path.dirname(os.path.dirname(path)))
 from protoc_gen_pyhttp import http
 
-__version__ = "1.0.0rc1"
+__version__ = "1.0.0rc2"
 
 
-def main() -> None:
+def main():
     request = plugin.CodeGeneratorRequest.FromString(sys.stdin.buffer.read())
 
-    response = plugin.CodeGeneratorResponse()
-    response.supported_features = plugin.CodeGeneratorResponse.FEATURE_PROTO3_OPTIONAL
-
     pool = DescriptorPool()
     for proto in request.proto_file:
         pool.Add(proto)
 
-    gen = response.file.add()
-
     for proto_file in request.proto_file:
+        response = plugin.CodeGeneratorResponse()
+        response.supported_features = plugin.CodeGeneratorResponse.FEATURE_PROTO3_OPTIONAL
+
+        gen = response.file.add()
         http.generate_file(proto_file, pool, gen)
 
-    sys.stdout.buffer.write(response.SerializeToString())
+        sys.stdout.buffer.write(response.SerializeToString())
 
 
 if __name__ == "__main__":
     main()
-
```

## protoc_gen_pyhttp/template.py

```diff
@@ -80,17 +80,17 @@
 {%- if has_vars %}
 from google.protobuf.json_format import ParseDict as _ParseDict
 {%- endif %}
 {% for use in uses %}
 {{ use }}
 {%- endfor %}
 
-_RegisterMethod = _Callable[[str, str, _Callable[[_Dict[str, _Any], bytes], _Any]], _Any]
-_RequestDeserializerMethod = _Callable[[_Any, bytes], _Any]
-_ResponseSerializerMethod = _Callable[[_Any], _Any]
+_RegisterFunction = _Callable[[str, str, _Callable[[_Dict[str, _Any], bytes], _Any]], _Any]
+_RequestDeserializerFunction = _Callable[[_Any, bytes], _Any]
+_ResponseSerializerFunction = _Callable[[_Any], _Any]
 
 
 {%- for service in services %}
 
 
 class {{ service.name }}Servicer(object):
     """
@@ -110,34 +110,34 @@
         {% endfor -%}
         """
         raise NotImplementedError('Method not implemented!')
     {%- endfor %}
 
 
 def register_{{ service.snake_case_name }}_http_server(
-        register: _RegisterMethod,
+        register: _RegisterFunction,
         servicer: {{ service.name }}Servicer,
-        request_deserializer: _RequestDeserializerMethod,
-        response_serializer: _ResponseSerializerMethod):
+        request_deserializer: _RequestDeserializerFunction,
+        response_serializer: _ResponseSerializerFunction):
     service = {{ service.pascal_case_name }}(servicer, request_deserializer, response_serializer)
     {%- for method in service.methods %}
     register("{{ method.method }}", "{{ method.path }}", service.{{ method.snake_case_name }})
     {%- endfor %}
 
 
 class {{ service.pascal_case_name }}(object):
     servicer: {{ service.name }}Servicer
-    request_deserializer: _RequestDeserializerMethod
-    response_serializer: _ResponseSerializerMethod
+    request_deserializer: _RequestDeserializerFunction
+    response_serializer: _ResponseSerializerFunction
 
     def __init__(
             self,
             servicer: {{ service.name }}Servicer,
-            request_deserializer: _RequestDeserializerMethod,
-            response_serializer: _ResponseSerializerMethod):
+            request_deserializer: _RequestDeserializerFunction,
+            response_serializer: _ResponseSerializerFunction):
         self.servicer = servicer
         self.request_deserializer = request_deserializer
         self.response_serializer = response_serializer
 
     {%- for method in service.methods %}
 
     def {{ method.snake_case_name }}(self, {{- ' ' -}}
```

## Comparing `protoc_gen_pyhttp-1.0.0rc1.dist-info/LICENSE` & `protoc_gen_pyhttp-1.0.0rc2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `protoc_gen_pyhttp-1.0.0rc1.dist-info/RECORD` & `protoc_gen_pyhttp-1.0.0rc2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 protoc_gen_pyhttp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 protoc_gen_pyhttp/http.py,sha256=TplHhE6dt-2oxiSObSl8BPBWLEtF75f2BsJ1UXm5OUw,12894
-protoc_gen_pyhttp/main.py,sha256=C-AmNQ77YCgE_CTtiYLK1dS5sQYwPCr-R7BpNNSIUtI,922
-protoc_gen_pyhttp/template.py,sha256=tdYapdfgb3dQ-zmFl-dVWasfDrB_Sa6cL2bLImA4oCI,6411
+protoc_gen_pyhttp/main.py,sha256=T19_S-F2d3BjAiLliXNOpejxF6CMqi1IGULT94AmLg4,928
+protoc_gen_pyhttp/template.py,sha256=jvuGQt7OE1_MT98uV3FnXtOzEOyth4oeIMW_DdrcIhI,6431
 protoc_gen_pyhttp/util.py,sha256=6E8rO4TNA8m_2LbtPitoTdvn9X09BMvAl1t3ioI1Ovw,665
-protoc_gen_pyhttp-1.0.0rc1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-protoc_gen_pyhttp-1.0.0rc1.dist-info/METADATA,sha256=9rp0VLNE70ZJfoPUulRQcgpUjvqy8TKlOxUXt91jJXo,488
-protoc_gen_pyhttp-1.0.0rc1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-protoc_gen_pyhttp-1.0.0rc1.dist-info/entry_points.txt,sha256=BwDuxzLn1n-mRoQ1A8RwTLkFoQieQLit6Ylw4VkhjN4,66
-protoc_gen_pyhttp-1.0.0rc1.dist-info/top_level.txt,sha256=4MQv_8FVmS7cnuezsnCo4EVb9_sdsy-deIXuxVR6K2E,18
-protoc_gen_pyhttp-1.0.0rc1.dist-info/RECORD,,
+protoc_gen_pyhttp-1.0.0rc2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+protoc_gen_pyhttp-1.0.0rc2.dist-info/METADATA,sha256=WphIigzG2kf1ER8PBzVdGdKUc32OO8GQUfrhzykOuA8,488
+protoc_gen_pyhttp-1.0.0rc2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+protoc_gen_pyhttp-1.0.0rc2.dist-info/entry_points.txt,sha256=BwDuxzLn1n-mRoQ1A8RwTLkFoQieQLit6Ylw4VkhjN4,66
+protoc_gen_pyhttp-1.0.0rc2.dist-info/top_level.txt,sha256=4MQv_8FVmS7cnuezsnCo4EVb9_sdsy-deIXuxVR6K2E,18
+protoc_gen_pyhttp-1.0.0rc2.dist-info/RECORD,,
```

