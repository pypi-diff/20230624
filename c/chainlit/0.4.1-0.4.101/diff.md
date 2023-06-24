# Comparing `tmp/chainlit-0.4.1.tar.gz` & `tmp/chainlit-0.4.101.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlit-0.4.1.tar", max compression
+gzip compressed data, was "chainlit-0.4.101.tar", max compression
```

## Comparing `chainlit-0.4.1.tar` & `chainlit-0.4.101.tar`

### file list

```diff
@@ -1,37 +1,38 @@
--rw-r--r--   0        0        0     2586 2023-06-20 13:11:34.219457 chainlit-0.4.1/README.md
--rw-r--r--   0        0        0     7489 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/__init__.py
--rw-r--r--   0        0        0       87 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/__main__.py
--rw-r--r--   0        0        0     1316 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/action.py
--rw-r--r--   0        0        0     1343 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cache.py
--rw-r--r--   0        0        0     3882 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cli/__init__.py
--rw-r--r--   0        0        0     4093 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cli/auth.py
--rw-r--r--   0        0        0     2594 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cli/deploy.py
--rw-r--r--   0        0        0     1147 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cli/mock.py
--rw-r--r--   0        0        0      716 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/cli/utils.py
--rw-r--r--   0        0        0     9838 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/client.py
--rw-r--r--   0        0        0     7430 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/config.py
--rw-r--r--   0        0        0     6060 2023-06-20 13:10:49.871691 chainlit-0.4.1/chainlit/element.py
--rw-r--r--   0        0        0     5113 2023-06-20 13:10:49.875692 chainlit-0.4.1/chainlit/emitter.py
--rw-r--r--   0        0        0   614554 2023-06-20 13:11:58.387330 chainlit-0.4.1/chainlit/frontend/dist/assets/index-51a1a88f.js
--rw-r--r--   0        0        0  1521126 2023-06-20 13:11:58.387330 chainlit-0.4.1/chainlit/frontend/dist/assets/index-68c36c96.js
--rw-r--r--   0        0        0     5697 2023-06-20 13:11:58.387330 chainlit-0.4.1/chainlit/frontend/dist/assets/index-f93cc942.css
--rw-r--r--   0        0        0     8889 2023-06-20 13:11:58.379330 chainlit-0.4.1/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
--rw-r--r--   0        0        0     8891 2023-06-20 13:11:58.387330 chainlit-0.4.1/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
--rw-r--r--   0        0        0     6455 2023-06-20 13:11:57.255335 chainlit-0.4.1/chainlit/frontend/dist/favicon.svg
--rw-r--r--   0        0        0      793 2023-06-20 13:11:58.387330 chainlit-0.4.1/chainlit/frontend/dist/index.html
--rw-r--r--   0        0        0      417 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/hello.py
--rw-r--r--   0        0        0      292 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/lc/__init__.py
--rw-r--r--   0        0        0     1080 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/lc/agent.py
--rw-r--r--   0        0        0    13195 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/lc/callbacks.py
--rw-r--r--   0        0        0      398 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/logger.py
--rw-r--r--   0        0        0     1623 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/markdown.py
--rw-r--r--   0        0        0    11948 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/message.py
--rw-r--r--   0        0        0    14332 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/server.py
--rw-r--r--   0        0        0      884 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/session.py
--rw-r--r--   0        0        0      950 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/sync.py
--rw-r--r--   0        0        0     2358 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/telemetry.py
--rw-r--r--   0        0        0     1525 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/types.py
--rw-r--r--   0        0        0     1213 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/user_session.py
--rw-r--r--   0        0        0      196 2023-06-20 13:10:49.879691 chainlit-0.4.1/chainlit/version.py
--rw-r--r--   0        0        0     1022 2023-06-20 13:10:49.879691 chainlit-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     4044 1970-01-01 00:00:00.000000 chainlit-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2827 2023-06-24 18:00:08.473588 chainlit-0.4.101/README.md
+-rw-r--r--   0        0        0     7502 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/__init__.py
+-rw-r--r--   0        0        0       87 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/__main__.py
+-rw-r--r--   0        0        0     1209 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/action.py
+-rw-r--r--   0        0        0     1343 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/cache.py
+-rw-r--r--   0        0        0     3550 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/cli/__init__.py
+-rw-r--r--   0        0        0     4093 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/cli/auth.py
+-rw-r--r--   0        0        0     2594 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/cli/deploy.py
+-rw-r--r--   0        0        0     1147 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/cli/mock.py
+-rw-r--r--   0        0        0      716 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/cli/utils.py
+-rw-r--r--   0        0        0     9838 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/client.py
+-rw-r--r--   0        0        0     7430 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/config.py
+-rw-r--r--   0        0        0      709 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/context.py
+-rw-r--r--   0        0        0     5971 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/element.py
+-rw-r--r--   0        0        0     4178 2023-06-24 17:59:20.832978 chainlit-0.4.101/chainlit/emitter.py
+-rw-r--r--   0        0        0   614554 2023-06-24 18:00:34.893916 chainlit-0.4.101/chainlit/frontend/dist/assets/index-51a1a88f.js
+-rw-r--r--   0        0        0  1521126 2023-06-24 18:00:34.893916 chainlit-0.4.101/chainlit/frontend/dist/assets/index-68c36c96.js
+-rw-r--r--   0        0        0     5697 2023-06-24 18:00:34.889916 chainlit-0.4.101/chainlit/frontend/dist/assets/index-f93cc942.css
+-rw-r--r--   0        0        0     8889 2023-06-24 18:00:34.885916 chainlit-0.4.101/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg
+-rw-r--r--   0        0        0     8891 2023-06-24 18:00:34.889916 chainlit-0.4.101/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg
+-rw-r--r--   0        0        0     6455 2023-06-24 18:00:33.605900 chainlit-0.4.101/chainlit/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0      793 2023-06-24 18:00:34.893916 chainlit-0.4.101/chainlit/frontend/dist/index.html
+-rw-r--r--   0        0        0      417 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/hello.py
+-rw-r--r--   0        0        0      292 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/lc/__init__.py
+-rw-r--r--   0        0        0     1121 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/lc/agent.py
+-rw-r--r--   0        0        0    12783 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/lc/callbacks.py
+-rw-r--r--   0        0        0      398 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/logger.py
+-rw-r--r--   0        0        0     1623 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/markdown.py
+-rw-r--r--   0        0        0    11832 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/message.py
+-rw-r--r--   0        0        0    14081 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/server.py
+-rw-r--r--   0        0        0      807 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/session.py
+-rw-r--r--   0        0        0      539 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/sync.py
+-rw-r--r--   0        0        0     2358 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/telemetry.py
+-rw-r--r--   0        0        0     1525 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/types.py
+-rw-r--r--   0        0        0     1213 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/user_session.py
+-rw-r--r--   0        0        0      196 2023-06-24 17:59:20.836978 chainlit-0.4.101/chainlit/version.py
+-rw-r--r--   0        0        0     1000 2023-06-24 17:59:20.836978 chainlit-0.4.101/pyproject.toml
+-rw-r--r--   0        0        0     4242 1970-01-01 00:00:00.000000 chainlit-0.4.101/PKG-INFO
```

### Comparing `chainlit-0.4.1/README.md` & `chainlit-0.4.101/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -52,15 +52,18 @@
 $ chainlit run demo.py -w
 ```
 
 <img src="/images/quick-start.png" alt="Quick Start"></img>
 
 ### 🔗 With LangChain
 
-Checkout our plug and play [integration](https://docs.chainlit.io/langchain) with LangChain!
+Check out our plug-and-play [integration](https://docs.chainlit.io/langchain) with LangChain!
+
+### 📚 More Examples - Cookbook
+You can find various examples of Chainlit apps [here](https://github.com/Chainlit/cookbook) that leverage tools and services such as OpenAI, Anthropiс, LangChain, LlamaIndex, ChromaDB, Pinecone and more.
 
 ## 🛣 Roadmap
 - [ ] New UI elements (spreadsheet, video, carousel...)
 - [ ] Create your own UI elements via component framework
 - [ ] DAG-based chain-of-thought interface
 - [ ] Support more LLMs in the prompt playground
 - [ ] App deployment
```

### Comparing `chainlit-0.4.1/chainlit/__init__.py` & `chainlit-0.4.101/chainlit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from chainlit.message import ErrorMessage
 from chainlit.action import Action
 from chainlit.element import Image, Text, Pdf, Avatar, Pyplot
 from chainlit.message import Message, ErrorMessage, AskUserMessage, AskFileMessage
 from chainlit.user_session import user_session
 from chainlit.sync import run_sync, make_async
 from chainlit.cache import cache
+from chainlit.context import emitter_var
 
 if LANGCHAIN_INSTALLED:
     from chainlit.lc.callbacks import (
         ChainlitCallbackHandler,
         AsyncChainlitCallbackHandler,
     )
 
@@ -39,40 +40,42 @@
     Args:
         user_function (Callable): The user-defined function to wrap.
 
     Returns:
         Callable: The wrapped function.
     """
 
-    async def wrapper(*args, __chainlit_emitter__: ChainlitEmitter):
+    async def wrapper(*args):
         # Get the parameter names of the user-defined function
         user_function_params = list(inspect.signature(user_function).parameters.keys())
 
         # Create a dictionary of parameter names and their corresponding values from *args
         params_values = {
             param_name: arg for param_name, arg in zip(user_function_params, args)
         }
 
+        emitter = emitter_var.get()
+
         if with_task:
-            await __chainlit_emitter__.task_start()
+            await emitter.task_start()
 
         try:
             # Call the user-defined function with the arguments
             if inspect.iscoroutinefunction(user_function):
                 return await user_function(**params_values)
             else:
                 return user_function(**params_values)
         except InterruptedError:
             pass
         except Exception as e:
             logger.exception(e)
             await ErrorMessage(content=str(e), author="Error").send()
         finally:
             if with_task:
-                await __chainlit_emitter__.task_end()
+                await emitter.task_end()
 
     return wrapper
 
 
 @trace
 def langchain_factory(use_async: bool) -> Callable:
     """
```

### Comparing `chainlit-0.4.1/chainlit/action.py` & `chainlit-0.4.101/chainlit/action.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pydantic.dataclasses import dataclass
 from dataclasses_json import dataclass_json
 
-from chainlit.emitter import get_emit_fn
+from chainlit.context import get_emitter
 from chainlit.telemetry import trace_event
 
 
 @dataclass_json
 @dataclass
 class Action:
     # Name of the action, this should be used in the action_callback
@@ -17,17 +17,15 @@
     # The description of the action. This is what the user will see when they hover the action.
     description: str = ""
     # This should not be set manually, only used internally.
     forId: str = None
 
     def __post_init__(self) -> None:
         trace_event(f"init {self.__class__.__name__}")
-        self.emit = get_emit_fn()
-        if not self.emit:
-            raise RuntimeError("Action should be instantiated in a Chainlit context")
+        self.emit = get_emitter().emit
 
     async def send(self, for_id: str):
         trace_event(f"send {self.__class__.__name__}")
         self.forId = for_id
         await self.emit("action", self.to_dict())
 
     async def remove(self):
```

### Comparing `chainlit-0.4.1/chainlit/cache.py` & `chainlit-0.4.101/chainlit/cache.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/cli/__init__.py` & `chainlit-0.4.101/chainlit/cli/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 import click
 import os
 import sys
 import uvicorn
-import asyncio
-import nest_asyncio
-
-nest_asyncio.apply()
 
 from chainlit.config import (
     config,
     init_config,
     load_module,
     PACKAGE_ROOT,
     DEFAULT_HOST,
@@ -48,23 +44,15 @@
     init_markdown(config.root)
 
     # Initialize the LangChain cache if installed and enabled
     init_lc_cache()
 
     log_level = "debug" if config.run.debug else "error"
 
-    # Start the server
-    async def start():
-        config = uvicorn.Config(app, host=host, port=port, log_level=log_level)
-        server = uvicorn.Server(config)
-        await server.serve()
-
-    # Run the asyncio event loop instead of uvloop to enable re entrance
-    asyncio.run(start())
-    # uvicorn.run(app, host=host, port=port)
+    uvicorn.run(app, host=host, port=port, log_level=log_level)
 
 
 # Define the "run" command for Chainlit CLI
 @cli.command("run")
 @click.argument("target", required=True, envvar="RUN_TARGET")
 @click.option("-w", "--watch", default=False, is_flag=True, envvar="WATCH")
 @click.option("-h", "--headless", default=False, is_flag=True, envvar="HEADLESS")
```

### Comparing `chainlit-0.4.1/chainlit/cli/auth.py` & `chainlit-0.4.101/chainlit/cli/auth.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/cli/deploy.py` & `chainlit-0.4.101/chainlit/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/cli/mock.py` & `chainlit-0.4.101/chainlit/cli/mock.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/cli/utils.py` & `chainlit-0.4.101/chainlit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/client.py` & `chainlit-0.4.101/chainlit/client.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/config.py` & `chainlit-0.4.101/chainlit/config.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/element.py` & `chainlit-0.4.101/chainlit/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pydantic.dataclasses import dataclass
 from dataclasses_json import dataclass_json
 from typing import Dict, Union, Any
 import uuid
 import aiofiles
 from io import BytesIO
 
-from chainlit.emitter import get_emitter, BaseClient
+from chainlit.context import get_emitter
+from chainlit.client import BaseClient
 from chainlit.telemetry import trace_event
 from chainlit.types import ElementType, ElementDisplay, ElementSize
 
 type_to_mime = {
     "image": "binary/octet-stream",
     "text": "text/plain",
     "pdf": "application/pdf",
@@ -37,16 +38,14 @@
     tempId: str = None
     # The ID of the message this element is associated with.
     forId: str = None
 
     def __post_init__(self) -> None:
         trace_event(f"init {self.__class__.__name__}")
         self.emitter = get_emitter()
-        if not self.emitter:
-            raise RuntimeError("Element should be instantiated in a Chainlit context")
 
         if not self.url and not self.path and not self.content:
             raise ValueError("Must provide url, path or content to instantiate element")
 
         self.tempId = uuid.uuid4().hex
 
     async def preprocess_content(self):
```

### Comparing `chainlit-0.4.1/chainlit/emitter.py` & `chainlit-0.4.101/chainlit/emitter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union, Dict
 from chainlit.session import Session
 from chainlit.types import AskSpec
 from chainlit.client import BaseClient
+from chainlit.context import emitter_var
 from socketio.exceptions import TimeoutError
-import inspect
 
 
 class ChainlitEmitter:
     """
     Chainlit Emitter class. The Emitter is not directly exposed to the developer.
     Instead, the developer interacts with the Emitter through the methods and classes exposed in the __init__ file.
     """
@@ -125,35 +125,7 @@
             "stream_start",
             msg_dict,
         )
 
     def send_token(self, id: Union[str, int], token: str):
         """Send a message token to the UI."""
         return self.emit("stream_token", {"id": id, "token": token})
-
-
-def get_emitter() -> Union[ChainlitEmitter, None]:
-    """
-    Get the Chainlit Emitter instance from the current call stack.
-    This unusual approach is necessary because:
-     - we need to get the right Emitter instance with the right websocket connection
-     - to preserve a lean developer experience, we do not pass the Emitter instance to every function call
-
-    What happens is that we set __chainlit_emitter__ in the local variables when we receive a websocket message.
-    Then we can retrieve it from the call stack when we need it, even if the developer's code has no idea about it.
-    """
-    attr = "__chainlit_emitter__"
-    candidates = [i[0].f_locals.get(attr) for i in inspect.stack()]
-    emitter = None
-    for candidate in candidates:
-        if candidate:
-            emitter = candidate
-            break
-
-    return emitter
-
-
-def get_emit_fn():
-    emitter = get_emitter()
-    if emitter:
-        return emitter.emit
-    return None
```

### Comparing `chainlit-0.4.1/chainlit/frontend/dist/assets/index-51a1a88f.js` & `chainlit-0.4.101/chainlit/frontend/dist/assets/index-51a1a88f.js`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/frontend/dist/assets/index-68c36c96.js` & `chainlit-0.4.101/chainlit/frontend/dist/assets/index-68c36c96.js`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/frontend/dist/assets/index-f93cc942.css` & `chainlit-0.4.101/chainlit/frontend/dist/assets/index-f93cc942.css`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg` & `chainlit-0.4.101/chainlit/frontend/dist/assets/logo_dark-bc7401f6.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg` & `chainlit-0.4.101/chainlit/frontend/dist/assets/logo_light-f19fc2ea.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/frontend/dist/favicon.svg` & `chainlit-0.4.101/chainlit/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/frontend/dist/index.html` & `chainlit-0.4.101/chainlit/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/lc/agent.py` & `chainlit-0.4.101/chainlit/lc/agent.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any
 from chainlit.lc.callbacks import ChainlitCallbackHandler, AsyncChainlitCallbackHandler
 from chainlit.sync import make_async
+from chainlit.context import emitter_var
 
 
 async def run_langchain_agent(agent: Any, input_str: str, use_async: bool):
     if hasattr(agent, "input_keys"):
         input_key = agent.input_keys[0]
         if use_async:
             raw_res = await agent.acall(
```

### Comparing `chainlit-0.4.1/chainlit/lc/callbacks.py` & `chainlit-0.4.101/chainlit/lc/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 from langchain.callbacks.base import BaseCallbackHandler, AsyncCallbackHandler
 from langchain.schema import (
     AgentAction,
     AgentFinish,
     BaseMessage,
     LLMResult,
 )
-from chainlit.emitter import get_emitter, ChainlitEmitter
+from chainlit.emitter import ChainlitEmitter
+from chainlit.context import get_emitter
 from chainlit.message import Message, ErrorMessage
 from chainlit.config import config
 from chainlit.types import LLMSettings
 from chainlit.sync import run_sync
 
 IGNORE_LIST = ["AgentExecutor"]
 
@@ -103,22 +104,18 @@
     def start_stream(self):
         author, indent, llm_settings = self.get_message_params()
 
         if author in IGNORE_LIST:
             return
 
         if config.code.lc_rename:
-            author = run_sync(
-                config.code.lc_rename(author, __chainlit_emitter__=self.emitter)
-            )
+            author = run_sync(config.code.lc_rename(author))
 
         self.pop_prompt()
 
-        __chainlit_emitter__ = self.emitter
-
         streamed_message = Message(
             author=author,
             indent=indent,
             llm_settings=llm_settings,
             prompt=self.consume_last_prompt(),
             content="",
         )
@@ -131,19 +128,15 @@
     def add_message(self, message, prompt: str = None, error=False):
         author, indent, llm_settings = self.get_message_params()
 
         if author in IGNORE_LIST:
             return
 
         if config.code.lc_rename:
-            author = run_sync(
-                config.code.lc_rename(author, __chainlit_emitter__=self.emitter)
-            )
-
-        __chainlit_emitter__ = self.emitter
+            author = run_sync(config.code.lc_rename(author))
 
         if error:
             run_sync(ErrorMessage(author=author, content=message).send())
             self.end_stream()
             return
 
         if self.stream:
@@ -263,22 +256,18 @@
     async def start_stream(self):
         author, indent, llm_settings = self.get_message_params()
 
         if author in IGNORE_LIST:
             return
 
         if config.code.lc_rename:
-            author = await config.code.lc_rename(
-                author, __chainlit_emitter__=self.emitter
-            )
+            author = await config.code.lc_rename(author)
 
         self.pop_prompt()
 
-        __chainlit_emitter__ = self.emitter
-
         streamed_message = Message(
             author=author,
             indent=indent,
             prompt=self.consume_last_prompt(),
             llm_settings=llm_settings,
             content="",
         )
@@ -291,19 +280,15 @@
     async def add_message(self, message, prompt: str = None, error=False):
         author, indent, llm_settings = self.get_message_params()
 
         if author in IGNORE_LIST:
             return
 
         if config.code.lc_rename:
-            author = await config.code.lc_rename(
-                author, __chainlit_emitter__=self.emitter
-            )
-
-        __chainlit_emitter__ = self.emitter
+            author = await config.code.lc_rename(author)
 
         if error:
             await ErrorMessage(author=author, content=message).send()
             self.end_stream()
             return
 
         if self.stream:
```

### Comparing `chainlit-0.4.1/chainlit/markdown.py` & `chainlit-0.4.101/chainlit/markdown.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/message.py` & `chainlit-0.4.101/chainlit/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Dict, Union
 from abc import ABC, abstractmethod
 import uuid
 import time
 import asyncio
 
 from chainlit.telemetry import trace_event
-from chainlit.emitter import get_emitter
+from chainlit.context import get_emitter
 from chainlit.config import config
 from chainlit.types import (
     LLMSettings,
     AskSpec,
     AskFileSpec,
     AskFileResponse,
     AskResponse,
@@ -30,16 +30,14 @@
     created_at: int = None
 
     def __post_init__(self) -> None:
         trace_event(f"init {self.__class__.__name__}")
         self.temp_id = uuid.uuid4().hex
         self.created_at = current_milli_time()
         self.emitter = get_emitter()
-        if not self.emitter:
-            raise RuntimeError("Message should be instantiated in a Chainlit context")
 
     @abstractmethod
     def to_dict(self):
         pass
 
     async def _create(self):
         msg_dict = self.to_dict()
```

### Comparing `chainlit-0.4.1/chainlit/server.py` & `chainlit-0.4.101/chainlit/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     FileResponse,
     PlainTextResponse,
 )
 from fastapi_socketio import SocketManager
 from starlette.middleware.cors import CORSMiddleware
 import asyncio
 
+from chainlit.context import emitter_var, loop_var
 from chainlit.config import config, load_module, reload_config, DEFAULT_HOST
 from chainlit.session import Session, sessions
 from chainlit.user_session import user_sessions
 from chainlit.client import CloudClient
 from chainlit.emitter import ChainlitEmitter
 from chainlit.markdown import get_markdown_str
 from chainlit.action import Action
@@ -291,36 +292,37 @@
 
     session = {
         "id": sid,
         "emit": emit_fn,
         "ask_user": ask_user_fn,
         "client": cloud_client,
         "user_env": user_env,
-        "running_sync": False,
         "should_stop": False,
     }  # type: Session
 
     sessions[sid] = session
 
     trace_event("connection_successful")
     return True
 
 
 @socket.on("connection_successful")
 async def connection_successful(sid):
     session = need_session(sid)
-    __chainlit_emitter__ = ChainlitEmitter(session)
+    emitter_var.set(ChainlitEmitter(session))
+    loop_var.set(asyncio.get_event_loop())
+
     if config.code.lc_factory:
         """Instantiate the langchain agent and store it in the session."""
-        agent = await config.code.lc_factory(__chainlit_emitter__=__chainlit_emitter__)
+        agent = await config.code.lc_factory()
         session["agent"] = agent
 
     if config.code.on_chat_start:
         """Call the on_chat_start function provided by the developer."""
-        await config.code.on_chat_start(__chainlit_emitter__=__chainlit_emitter__)
+        await config.code.on_chat_start()
 
 
 @socket.on("disconnect")
 async def disconnect(sid):
     if sid in sessions:
         # Clean up the session
         sessions.pop(sid)
@@ -332,30 +334,34 @@
 
 @socket.on("stop")
 async def stop(sid):
     if sid in sessions:
         trace_event("stop_task")
         session = sessions[sid]
 
-        __chainlit_emitter__ = ChainlitEmitter(session)
+        emitter_var.set(ChainlitEmitter(session))
+        loop_var.set(asyncio.get_event_loop())
 
         await Message(author="System", content="Task stopped by the user.").send()
 
         session["should_stop"] = True
 
         if config.code.on_stop:
             await config.code.on_stop()
 
 
 async def process_message(session: Session, author: str, input_str: str):
     """Process a message from the user."""
 
     try:
-        __chainlit_emitter__ = ChainlitEmitter(session)
-        await __chainlit_emitter__.task_start()
+        emitter = ChainlitEmitter(session)
+        emitter_var.set(emitter)
+        loop_var.set(asyncio.get_event_loop())
+
+        await emitter.task_start()
 
         if session["client"]:
             # If cloud is enabled, persist the message
             await session["client"].create_message(
                 {
                     "author": author,
                     "content": input_str,
@@ -369,75 +375,70 @@
 
             # If a langchain agent is available, run it
             if config.code.lc_run:
                 # If the developer provided a custom run function, use it
                 await config.code.lc_run(
                     langchain_agent,
                     input_str,
-                    __chainlit_emitter__=__chainlit_emitter__,
                 )
                 return
             else:
                 # Otherwise, use the default run function
                 raw_res, output_key = await run_langchain_agent(
                     langchain_agent, input_str, use_async=config.code.lc_agent_is_async
                 )
 
                 if config.code.lc_postprocess:
                     # If the developer provided a custom postprocess function, use it
-                    await config.code.lc_postprocess(
-                        raw_res, __chainlit_emitter__=__chainlit_emitter__
-                    )
+                    await config.code.lc_postprocess(raw_res)
                     return
                 elif output_key is not None:
                     # Use the output key if provided
                     res = raw_res[output_key]
                 else:
                     # Otherwise, use the raw response
                     res = raw_res
             # Finally, send the response to the user
             await Message(author=config.ui.name, content=res).send()
 
         elif config.code.on_message:
             # If no langchain agent is available, call the on_message function provided by the developer
-            await config.code.on_message(
-                input_str, __chainlit_emitter__=__chainlit_emitter__
-            )
+            await config.code.on_message(input_str)
     except InterruptedError:
         pass
     except Exception as e:
         logger.exception(e)
         await ErrorMessage(author="Error", content=str(e)).send()
     finally:
-        await __chainlit_emitter__.task_end()
+        await emitter.task_end()
 
 
 @socket.on("ui_message")
 async def message(sid, data):
     """Handle a message sent by the User."""
     session = need_session(sid)
     session["should_stop"] = False
 
     input_str = data["content"].strip()
     author = data["author"]
 
     await process_message(session, author, input_str)
 
 
-async def process_action(session: Session, action: Action):
-    __chainlit_emitter__ = ChainlitEmitter(session)
+async def process_action(action: Action):
     callback = config.code.action_callbacks.get(action.name)
     if callback:
-        await callback(action, __chainlit_emitter__=__chainlit_emitter__)
+        await callback(action)
     else:
         logger.warning("No callback found for action %s", action.name)
 
 
 @socket.on("action_call")
 async def call_action(sid, action):
     """Handle an action call from the UI."""
     session = need_session(sid)
+    emitter_var.set(ChainlitEmitter(session))
+    loop_var.set(asyncio.get_event_loop())
 
-    __chainlit_emitter__ = ChainlitEmitter(session)
     action = Action(**action)
 
-    await process_action(session, action)
+    await process_action(action)
```

### Comparing `chainlit-0.4.1/chainlit/session.py` & `chainlit-0.4.101/chainlit/session.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,16 +12,14 @@
     ask_user: Callable[[Any, Optional[int]], Union[AskResponse, None]]
     # Function to emit a message to the user
     emit: Callable[[str, Any], None]
     # User specific environment variables. Empty if no user environment variables are required.
     user_env: Dict[str, str]
     # Optional langchain agent
     agent: Any
-    # If the session is currently running a sync task
-    running_sync: bool
     # Whether the current task should be stopped
     should_stop: bool
     # Optional client to persist messages and files
     client: Optional[BaseClient]
 
 
 sessions: Dict[str, Session] = {}
```

### Comparing `chainlit-0.4.1/chainlit/telemetry.py` & `chainlit-0.4.101/chainlit/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/types.py` & `chainlit-0.4.101/chainlit/types.py`

 * *Files identical despite different names*

### Comparing `chainlit-0.4.1/chainlit/user_session.py` & `chainlit-0.4.101/chainlit/user_session.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict
-from chainlit.emitter import get_emitter
+from chainlit.context import get_emitter
 
 user_sessions: Dict[str, Dict] = {}
 
 
 class UserSession:
     """
     Developer facing user session class.
```

### Comparing `chainlit-0.4.1/pyproject.toml` & `chainlit-0.4.101/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlit"
-version = "0.4.1"
+version = "0.4.101"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'langchain']
 description = "A faster way to build chatbot UIs."
 authors = ["Chainlit"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
@@ -18,15 +18,14 @@
 # command_name = module_for_handler : function_for_handler
 chainlit = 'chainlit.cli:cli'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dataclasses_json = "^0.5.7"
 uvicorn = "^0.22.0"
-nest-asyncio = "^1.5.6"
 fastapi = "^0.96.0"
 fastapi-socketio = "^0.0.10"
 aiohttp = "^3.8.4"
 aiofiles = "^23.1.0"
 syncer = "^2.0.3"
 asyncer = "^0.0.2"
 click = "^8.1.3"
```

### Comparing `chainlit-0.4.1/PKG-INFO` & `chainlit-0.4.101/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlit
-Version: 0.4.1
+Version: 0.4.101
 Summary: A faster way to build chatbot UIs.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,langchain
 Author: Chainlit
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -17,15 +17,14 @@
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: asyncer (>=0.0.2,<0.0.3)
 Requires-Dist: auth0-python (>=4.1.1,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dataclasses_json (>=0.5.7,<0.6.0)
 Requires-Dist: fastapi (>=0.96.0,<0.97.0)
 Requires-Dist: fastapi-socketio (>=0.0.10,<0.0.11)
-Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: pydantic (>=1.10.8,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-graphql-client (>=0.4.3,<0.5.0)
 Requires-Dist: syncer (>=2.0.3,<3.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: uptrace (>=1.18.0,<2.0.0)
@@ -88,15 +87,18 @@
 $ chainlit run demo.py -w
 ```
 
 <img src="/images/quick-start.png" alt="Quick Start"></img>
 
 ### 🔗 With LangChain
 
-Checkout our plug and play [integration](https://docs.chainlit.io/langchain) with LangChain!
+Check out our plug-and-play [integration](https://docs.chainlit.io/langchain) with LangChain!
+
+### 📚 More Examples - Cookbook
+You can find various examples of Chainlit apps [here](https://github.com/Chainlit/cookbook) that leverage tools and services such as OpenAI, Anthropiс, LangChain, LlamaIndex, ChromaDB, Pinecone and more.
 
 ## 🛣 Roadmap
 - [ ] New UI elements (spreadsheet, video, carousel...)
 - [ ] Create your own UI elements via component framework
 - [ ] DAG-based chain-of-thought interface
 - [ ] Support more LLMs in the prompt playground
 - [ ] App deployment
```

