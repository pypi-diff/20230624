# Comparing `tmp/jam_ai-0.1.6.tar.gz` & `tmp/jam_ai-0.1.7.tar.gz`

## Comparing `jam_ai-0.1.6.tar` & `jam_ai-0.1.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/cmd/__init__.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.1.6/cmd/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/personnel/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/personnel/albert-einstein.json
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/personnel/homer-simpson.json
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/personnel/marie-curie.json
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.1.6/example/personnel/walter-white.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/base.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/core.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/version.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/instrument/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/instrument/base.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/instrument/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/instrument/text.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/interface/__init__.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/interface/base.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/interface/openai.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/interface/stability_ai.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/interface/writesonic.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/persistence/__init__.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/persistence/base.py
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/persistence/memory.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/persistence/model.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/persistence/sqlite.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/personnel/__init__.py
--rw-r--r--   0        0        0     6950 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/personnel/base.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/personnel/personnel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/util/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/util/generate.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.1.6/jam/util/search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/tests/instrument/__init__.py
--rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.1.6/tests/instrument/test_base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.6/tests/interface/__init__.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 jam_ai-0.1.6/tests/interface/test_base.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.1.6/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.1.6/LICENSE
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 jam_ai-0.1.6/README.md
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 jam_ai-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 jam_ai-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/cmd/__init__.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 jam_ai-0.1.7/cmd/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/personnel/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/personnel/albert-einstein.json
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/personnel/homer-simpson.json
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/personnel/marie-curie.json
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jam_ai-0.1.7/example/personnel/walter-white.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/base.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/core.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/version.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/instrument/__init__.py
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/instrument/base.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/instrument/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/instrument/text.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/interface/__init__.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/interface/base.py
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/interface/openai.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/interface/stability_ai.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/interface/writesonic.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/persistence/__init__.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/persistence/base.py
+-rw-r--r--   0        0        0     3730 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/persistence/memory.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/persistence/model.py
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/persistence/sqlite.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/personnel/__init__.py
+-rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/personnel/base.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/personnel/personnel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/util/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/util/generate.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jam_ai-0.1.7/jam/util/search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/tests/instrument/__init__.py
+-rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 jam_ai-0.1.7/tests/instrument/test_base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jam_ai-0.1.7/tests/interface/__init__.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 jam_ai-0.1.7/tests/interface/test_base.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 jam_ai-0.1.7/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jam_ai-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 jam_ai-0.1.7/README.md
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 jam_ai-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    16417 2020-02-02 00:00:00.000000 jam_ai-0.1.7/PKG-INFO
```

### Comparing `jam_ai-0.1.6/cmd/main.py` & `jam_ai-0.1.7/cmd/main.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/example/personnel/albert-einstein.json` & `jam_ai-0.1.7/example/personnel/albert-einstein.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/example/personnel/homer-simpson.json` & `jam_ai-0.1.7/example/personnel/homer-simpson.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/example/personnel/marie-curie.json` & `jam_ai-0.1.7/example/personnel/marie-curie.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/example/personnel/walter-white.json` & `jam_ai-0.1.7/example/personnel/walter-white.json`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/jam/base.py` & `jam_ai-0.1.7/jam/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/jam/core.py` & `jam_ai-0.1.7/jam/core.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/jam/instrument/base.py` & `jam_ai-0.1.7/jam/instrument/base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/jam/instrument/image.py` & `jam_ai-0.1.7/jam/instrument/image.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Union, Dict, AnyStr
 
 from jam.instrument.base import BaseInstrument, BaseParameter, BaseProperty
 from jam.interface.base import BaseInterface
 from jam.interface.openai import OpenAIImageGen
 
-_OpenAIImageGen = OpenAIImageGen()
 _PromptPainterPromptProperty = BaseProperty(
     name='prompt', description='The text prompt to generate the image'
 )
 _PromptPainterParameters = BaseParameter(
     properties=[_PromptPainterPromptProperty],
     required=[_PromptPainterPromptProperty]
 )
@@ -16,16 +15,18 @@
 
 class PromptPainter(BaseInstrument):
 
     def __init__(self,
                  name: str = 'prompt_painter',
                  description: str = 'Generates image from text prompt',
                  parameters: Union[BaseParameter, Dict] = _PromptPainterParameters,
-                 interface: BaseInterface = _OpenAIImageGen):
+                 interface: BaseInterface = None):
         super().__init__(name, description, parameters, interface)
+        if self.interface is None:
+            self.interface = OpenAIImageGen()
 
     def activate(self, prompt: AnyStr = None):
         if prompt is None:
             return
 
         response = self.interface.call(prompt)
         return response
```

### Comparing `jam_ai-0.1.6/jam/interface/base.py` & `jam_ai-0.1.7/jam/interface/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from typing import Any, AnyStr
 
 
+class JIError(Exception):
+
+    def __init__(self, message: str):
+        self.message = message
+
+
 class JIOutput(object):
     JIO_TEXT = 'text'
     JIO_IMAGE = 'image'
     JIO_AUDIO = 'audio'
     JIO_VIDEO = 'video'
     JIO_FILE = 'file'
     JIO_OTHER = 'other'
```

### Comparing `jam_ai-0.1.6/jam/interface/openai.py` & `jam_ai-0.1.7/jam/interface/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 import warnings
 from typing import AnyStr, Tuple, List, Dict
 
 import openai
 import requests
 from PIL import Image
 
-from jam.interface.base import BaseInterface, JIOutput
+from jam.interface.base import BaseInterface, JIOutput, JIError
 from jam.util.generate import generate_id
 
 warnings.filterwarnings('ignore')
 
 
 class OpenAIBase(BaseInterface):
 
     def __init__(self, token: str = None, model: str = None):
         super(OpenAIBase, self).__init__()
         self._token = token
         if self._token is None:
             self._token = os.getenv('OPENAI_KEY', '')
 
+        if self._token == '':
+            raise JIError(f"Unfulfilled credentials for {self.__class__.__name__} in parameters or environment.")
+
         openai.api_key = self._token
         self.open_ai = openai
 
         self.model = model
 
 
 class OpenAIChat(OpenAIBase):
```

### Comparing `jam_ai-0.1.6/jam/interface/stability_ai.py` & `jam_ai-0.1.7/jam/interface/stability_ai.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import io
 import warnings
 from typing import AnyStr, Tuple
 
-from jam.interface.base import BaseInterface, JIOutput
+from jam.interface.base import BaseInterface, JIOutput, JIError
 
 from PIL import Image
 from stability_sdk import client
 import stability_sdk.interfaces.gooseai.generation.generation_pb2 as generation
 
 
 class StabilityAIBase(BaseInterface):
@@ -29,14 +29,17 @@
         if self._api_key is None:
             self._api_key = os.getenv('STABILITY_KEY', '')
 
         self._host = host
         if self._host is None:
             self._host = os.getenv('STABILITY_HOST', '')
 
+        if self._api_key == '':
+            raise JIError(f"Unfulfilled credentials for {self.__class__.__name__} in parameters or environment.")
+
         self.verbose = verbose
         self.stability_api = client.StabilityInference(
             key=self._api_key,
             verbose=self.verbose,
             engine=self.engine,
         )
```

### Comparing `jam_ai-0.1.6/jam/interface/writesonic.py` & `jam_ai-0.1.7/jam/interface/writesonic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import os
 from typing import AnyStr, Tuple
 
-from jam.interface.base import BaseInterface, JIOutput
+from jam.interface.base import BaseInterface, JIOutput, JIError
 from jam.util.generate import generate_id
 
 import requests
 from PIL import Image
 
 
 class WriteSonicBase(BaseInterface):
@@ -17,14 +17,17 @@
                  engine: str = None,
                  language: str = 'en'):
         super(WriteSonicBase, self).__init__()
         self._api_key = api_key
         if self._api_key is None:
             self._api_key = os.getenv('WRITESONIC_KEY', '')
 
+        if self._api_key == '':
+            raise JIError(f"Unfulfilled credentials for {self.__class__.__name__} in parameters or environment.")
+
         self.headers = {
             "accept": "application/json",
             "content-type": "application/json",
             "X-API-KEY": self._api_key
         }
 
         self.product = product
```

### Comparing `jam_ai-0.1.6/jam/persistence/memory.py` & `jam_ai-0.1.7/jam/persistence/memory.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,23 +19,27 @@
     def __init__(self):
         self.head: Optional[Node] = None
         self.tail: Optional[Node] = None
         self.length = 0
 
     def append(self, data: PersistenceObject):
         new_node = Node(data)
-        if self.head is None:
+        if not self.head:
             self.head = new_node
             self.tail = new_node
         else:
-            current = self.head
-            while current.next:
-                current = current.next
+            # current = self.head
+            # while current.next:
+            #     current = current.next
+            # current.next = new_node
+            # new_node.prev = current
+            # self.tail = new_node
+            current = self.tail
             current.next = new_node
-            new_node.prev = current
+            new_node.prev = self.tail
             self.tail = new_node
         self.length += 1
 
     def find(self, key: str, value: List[str], limit: int = 5):
         result = []
         current = self.tail
         if current is None:
@@ -51,14 +55,35 @@
         result = []
         current = self.tail
         while current is not None:
             result.append(current.data)
             current = current.prev
         return result
 
+    def clear(self, key: str = None, value: List[str] = None):
+        if key is None or value is None:
+            self.head = self.tail = None
+            self.length = 0
+        else:
+            current = self.tail
+            while current:
+                if current.data.__dict__[key] in value:
+                    if current.prev:
+                        current.prev.next = current.next
+                    else:
+                        self.head = current.next
+
+                    if current.next:
+                        current.next.prev = current.prev
+                    else:
+                        self.tail = current.prev
+                    self.length -= 1
+
+                current = current.prev
+
 
 class MemoryPersistence(BasePersistence):
 
     def __init__(self):
         super(MemoryPersistence, self).__init__()
         self.db: DoubleLinkedList = DoubleLinkedList()
 
@@ -94,7 +119,12 @@
 
     def all(self):
         result = self.db.all()
         return result
 
     def count(self):
         return self.db.length
+
+    def clear(self, key: str = None, value: List[str] = None):
+        self.db.clear(key=key, value=value)
+        return
+
```

### Comparing `jam_ai-0.1.6/jam/persistence/model.py` & `jam_ai-0.1.7/jam/persistence/model.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/jam/persistence/sqlite.py` & `jam_ai-0.1.7/jam/persistence/sqlite.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,8 +90,23 @@
             return list(map(self.transform, result))
 
     def count(self):
         with Session(self.db) as session:
             result = session.query(ConversationHistory).count()
             return result
 
+    def clear(self, key: str = None, value: List[str] = None):
+        with Session(self.db) as session:
+            if key is None or value is None:
+                session.query(ConversationHistory).delete()
+                session.commit()
+                return
+
+            filter_conditions = [getattr(ConversationHistory, key) == val for val in value]
+            filter_conditions = or_(*filter_conditions)
+
+            session.query(ConversationHistory).filter(filter_conditions).delete()
+            session.commit()
+            return
+
+
```

### Comparing `jam_ai-0.1.6/jam/personnel/base.py` & `jam_ai-0.1.7/jam/personnel/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         f_call = self.function_map[f_name]
         f_args = json.loads(x['function_call']['arguments'])
         f_response = f_call(**f_args)
 
         return f_name, f_response
 
     @classmethod
-    def get_template(cls, filepath: str = 'new-agent.json'):
+    def get_template(cls, filepath: str = 'new-personnel.json'):
         filename, file_extension = os.path.splitext(filepath)
         if file_extension == '.json':
             with open(filepath, 'w') as f:
                 json.dump(cls.BASE_TEMPLATE, f)
             return True
         return False
```

### Comparing `jam_ai-0.1.6/tests/instrument/test_base.py` & `jam_ai-0.1.7/tests/instrument/test_base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/tests/interface/test_base.py` & `jam_ai-0.1.7/tests/interface/test_base.py`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/.gitignore` & `jam_ai-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/LICENSE` & `jam_ai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jam_ai-0.1.6/pyproject.toml` & `jam_ai-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jam-ai"
-version = "0.1.6"
+version = "0.1.7"
 version_pattern = "MAJOR.MINOR.PATCH"
 authors = [
   { name="Abhishta Gatya", email="abhishtagatya@yahoo.com" },
 ]
-description = "Experimental collaboration tool to use multiple AI personnel together equipped with instructed function calls."
+description = "Engaging with Multiple AI Agents with Jam."
 keywords = ["openai", "multi agent", "chat engine", "collaboration", "machine learning", "data science"]
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
     'openai',
     'Pillow',
```

### Comparing `jam_ai-0.1.6/PKG-INFO` & `jam_ai-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: jam-ai
-Version: 0.1.6
-Summary: Experimental collaboration tool to use multiple AI personnel together equipped with instructed function calls.
+Version: 0.1.7
+Summary: Engaging with Multiple AI Agents with Jam.
 Project-URL: homepage, https://github.com/abhishtagatya/jam
 Project-URL: documentation, https://github.com/abhishtagatya/jam
 Project-URL: changelog, https://github.com/abhishtagatya/jam/blob/master/CHANGELOG.md
 Author-email: Abhishta Gatya <abhishtagatya@yahoo.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -269,14 +269,21 @@
 prompt = jam_room.compose(
     message='Give me a question',
     multi=True
 )
 
 ```
 
+Don't forget to use your credentials. Primarily for OpenAI, the core engine of this project. 
+https://platform.openai.com/account/api-keys
+
+```bash
+export OPENAI_KEY=YOUR_KEY
+```
+
 ## Installation
 
 ```bash
 pip install jam-ai --upgrade
 ```
 You need to use Pip to install jam. Conda package is currently unavailable.
 
@@ -285,9 +292,20 @@
 * OpenAI
 
 Extra Requirements for Function Calls
 * Requests
 * Stability SDK
 * Pillow
 
+### Extension
+
+For the use of other libraries, please consider to always feed in your API Keys respectively. See below for example.
+
+```bash
+export STABILITY_KEY=YOUR_STABILITY_AI_KEY # If you are using Stability SDK
+export WRITESONIC_KEY=YOUR_WRITE_SONIC_KEY # If you are using WriteSonic API
+export CUSTOM_KEY=YOUR_CUSTOM_KEY          # If there are any other added functionalities
+```
+
+
 ## Author
 * Abhishta Gatya ([Email](mailto:abhishtagatya@yahoo.com)) - Software and Machine Learning Engineer
```

