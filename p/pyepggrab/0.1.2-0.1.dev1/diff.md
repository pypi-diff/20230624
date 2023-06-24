# Comparing `tmp/pyepggrab-0.1.2.tar.gz` & `tmp/pyepggrab-0.1.dev1.tar.gz`

## Comparing `pyepggrab-0.1.2.tar` & `pyepggrab-0.1.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/__about__.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/__init__.py
--rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/args.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/ask.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/configbase.py
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/configmanager.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/log.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/pyepggrab.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/utils.py
--rw-r--r--   0        0        0    21711 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/xmltv.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/xmlwriter.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/grabbers/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/__init__.py
--rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/catmap.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/config.py
--rwxr-xr-x   0        0        0    16506 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/hu_porthu.py
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/request_proc.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/utils.py
--rw-r--r--   0        0        0    17363 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/xml_utils.py
--rw-r--r--   0        0        0    27085 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyepggrab/resources/xmltv.dtd
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/README.md
--rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 pyepggrab-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/__about__.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/__init__.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/args.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/ask.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/configbase.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/configmanager.py
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/log.py
+-rw-r--r--   0        0        0     5961 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/pyepggrab.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/utils.py
+-rw-r--r--   0        0        0    21711 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/xmltv.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/xmlwriter.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/__init__.py
+-rw-r--r--   0        0        0    14813 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/catmap.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/config.py
+-rwxr-xr-x   0        0        0    15937 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/hu_porthu.py
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/request_proc.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/utils.py
+-rw-r--r--   0        0        0    17379 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/xml_utils.py
+-rw-r--r--   0        0        0    27085 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyepggrab/resources/xmltv.dtd
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/LICENSE.txt
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/README.md
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2757 2020-02-02 00:00:00.000000 pyepggrab-0.1.dev1/PKG-INFO
```

### Comparing `pyepggrab-0.1.2/pyepggrab/ask.py` & `pyepggrab-0.1.dev1/pyepggrab/ask.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.2/pyepggrab/configbase.py` & `pyepggrab-0.1.dev1/pyepggrab/configbase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Base classes used in the configuration management.
 
 These also provides the default config functionality
 """
 
+# from __future__ import annotations
+
 from dataclasses import dataclass
 from json import JSONEncoder
 from typing import Any, Dict, Type, TypeVar
 
 try:
     from typing import override  # type: ignore # noqa: F401, RUF100
 except ImportError:
@@ -39,8 +41,9 @@
 
 
 class ConfigEncoder(JSONEncoder):
     """Default config encoder. Saves every member variable of the class."""
 
     @override
     def default(self, o: Any) -> dict:
+        ConfigRootBase.from_dict({})
         return vars(o)
```

### Comparing `pyepggrab-0.1.2/pyepggrab/configmanager.py` & `pyepggrab-0.1.dev1/pyepggrab/configmanager.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,16 @@
         self._root = root
         self._encoder = encoder
         self._decoder = decoder
 
         if path:
             self._path = Path(path)
         else:
-            self._path = self.get_default_config_path()
+            confname = Path(sys.argv[0]).stem + ".conf"
+            self._path = Path(Path.home(), ".xmltv", confname)
 
     def get_config_path(self) -> Path:
         """Return the path to the config file."""
         return self._path
 
     def is_config_exists(self) -> bool:
         """Return true is the config file exists."""
@@ -68,25 +69,7 @@
             return self._root.from_dict(conf)
 
     def write_config(self, config: T) -> None:
         """Write the `root` type config to the config file."""
         configstr = json.dumps(config, cls=self._encoder, indent=2, ensure_ascii=False)
         with self._path.open("w", encoding="UTF-8") as file:
             file.write(configstr)
-
-    @staticmethod
-    def get_default_config_directory() -> Path:
-        """Get the default configuration directory."""
-        return Path(Path.home(), ".xmltv")
-
-    @staticmethod
-    def get_default_config_name() -> str:
-        """Get the default configuration file name."""
-        return Path(sys.argv[0]).stem + ".conf"
-
-    @classmethod
-    def get_default_config_path(cls) -> Path:
-        """Get the default configuration path (dir+name)."""
-        return Path(
-            cls.get_default_config_directory(),
-            cls.get_default_config_name(),
-        )
```

### Comparing `pyepggrab-0.1.2/pyepggrab/log.py` & `pyepggrab-0.1.dev1/pyepggrab/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 Loggers created with `create_logger()` are treated as manged loggers.
 The managed loggers are benefit from the delayed logging feature if the loggers
 are not finalized to avoid outputting unwanted log messages.
 """
 
 import logging
 import sys
-from typing import ClassVar, Dict, List, Union
+from typing import Dict, List, Union
 
 from .utils import grabber_name
 
 
 class Log:
     """Logger of pyepggrab."""
 
-    _finalized: ClassVar[bool] = False
-    _delayedlogs: ClassVar[Dict[str, List[logging.LogRecord]]] = {}
-    _managed_loggers: ClassVar[List[logging.Logger]] = []
+    _finalized: bool = False
+    _delayedlogs: Dict[str, List[logging.LogRecord]] = {}
+    _managed_loggers: List[logging.Logger] = []
 
     @classmethod
     def disable_loggers(cls) -> None:
         """Disable any logging output."""
         logging.disable(logging.CRITICAL)
 
     @classmethod
```

### Comparing `pyepggrab-0.1.2/pyepggrab/pyepggrab.py` & `pyepggrab-0.1.dev1/pyepggrab/pyepggrab.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,32 +16,32 @@
 Writing grabber that not using these are possible but not recommended (if you
 still want to do, use this as a reference).
 """
 
 import sys
 from argparse import Namespace
 from json import JSONDecoder, JSONEncoder
-from typing import Callable, ClassVar, List, NoReturn, Optional, Type
+from typing import Callable, List, NoReturn, Optional, Type
 
 from pyepggrab import __about__
 from pyepggrab.configbase import ConfigEncoder, ConfigRootBase, T
 from pyepggrab.log import Log
 
 from .args import ArgParser, ExtraargsType
 from .configmanager import ConfigManager
 
 MainType = Callable[[Namespace, ConfigManager], Optional[int]]
 
 
 class Pyepggrab:
     """Pyepggrab convenience functions and decorators."""
 
-    _grabber_main: ClassVar[Optional[MainType]] = None
-    _grabber_config: ClassVar[Optional[MainType]] = None
-    _grabber_extraargs: ClassVar[Optional[ExtraargsType]] = None
+    _grabber_main: Optional[MainType] = None
+    _grabber_config: Optional[MainType] = None
+    _grabber_extraargs: Optional[ExtraargsType] = None
 
     @classmethod
     def grabber_main(cls, func: MainType) -> MainType:
         """Decorate the grabber main function with this.
 
         Called when grabber starts in normal operation.
```

### Comparing `pyepggrab-0.1.2/pyepggrab/utils.py` & `pyepggrab-0.1.dev1/pyepggrab/utils.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.2/pyepggrab/xmltv.py` & `pyepggrab-0.1.dev1/pyepggrab/xmltv.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.2/pyepggrab/xmlwriter.py` & `pyepggrab-0.1.dev1/pyepggrab/xmlwriter.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/catmap.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/catmap.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/config.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Classes used in the configuration file."""
 
+# from __future__ import annotations
+
 from dataclasses import asdict, dataclass
-from json import JSONEncoder
-from typing import Any, List, Type
+from typing import List, Type
 
 from pyepggrab.configbase import ConfigBase, ConfigRootBase, T
-from pyepggrab.utils import remove_suffix
 
 try:
     from typing import override  # type: ignore # noqa: F401, RUF100
 except ImportError:
     from typing_extensions import override  # type: ignore # noqa: F401, RUF100
 
 
@@ -20,15 +20,15 @@
     id_: str
     name: str
     enabled: bool
 
     @override
     @classmethod
     def from_dict(cls: Type[T], d: dict) -> "Channel":
-        id_ = d.get("id", "")  # Stored without '_' in config
+        id_ = d.get("id", "")
         name = d.get("name", "")
         enabled = d.get("enabled", False)
         return Channel(id_, name, enabled)
 
 
 @dataclass
 class GrabberConfig(ConfigRootBase):
@@ -38,16 +38,7 @@
 
     @override
     @classmethod
     def from_dict(cls: Type[T], d: dict) -> "GrabberConfig":
         channels = [Channel.from_dict(ch) for ch in d.get("channels", [])]
         conf = ConfigRootBase.from_dict(d)
         return GrabberConfig(**asdict(conf), channels=channels)
-
-
-class GrabberConfigEncoder(JSONEncoder):
-    """Save every member variable of the class, but without the '_' suffixes."""
-
-    @override
-    def default(self, o: Any) -> dict:
-        """Encode keys without '_' suffixes."""
-        return {remove_suffix(k, "_"): v for k, v in vars(o).items()}
```

### Comparing `pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/hu_porthu.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/hu_porthu.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 from typing import Dict, List, NoReturn, Optional, Tuple
 
 import requests
 from fake_useragent import UserAgent  # type: ignore[import]
 
 from pyepggrab.ask import ask_boolean, ask_many_boolean
 from pyepggrab.configmanager import ConfigManager
-from pyepggrab.grabbers.hu_porthu.config import (
-    Channel,
-    GrabberConfig,
-    GrabberConfigEncoder,
-)
+from pyepggrab.grabbers.hu_porthu.config import Channel, GrabberConfig
 from pyepggrab.grabbers.hu_porthu.request_proc import ProcessCtx
 from pyepggrab.grabbers.hu_porthu.utils import (
     INIT_URL,
     PROGLIST_URL,
     portid_to_xmlid,
     xmlid_to_portid,
 )
@@ -417,32 +413,16 @@
 
 @Pyepggrab.grabber_extraargs
 def extraargs(argp: argparse.ArgumentParser) -> None:
     """Add grabber specific arguments to argparser.
 
     Called by pyepggrab
     """
-    argp.add_argument(
-        "--slow",
-        action="store_true",
-        help=(
-            "Use a significantly slower, but more detailed mode to download the guide. "
-            "This adds information like description, actors, etc"
-        ),
-    )
-    argp.add_argument(
-        "--jobs",
-        type=int,
-        default=1,
-        help=(
-            "Number of parallel processes used to download the guide. "
-            "Only used in --slow mode. Setting this value too high may result in "
-            "high resource usage and/or getting banned from port.hu"
-        ),
-    )
+    argp.add_argument("--slow", action="store_true")
+    argp.add_argument("--jobs", type=int, default=1)
 
 
 @Pyepggrab.grabber_main
 def main(
     args: argparse.Namespace,
     confman: ConfigManager[GrabberConfig],
 ) -> Optional[int]:
@@ -515,14 +495,13 @@
 def run(**kwargs) -> NoReturn:
     """Entrypoint to start the grabber by calling `pyepggrab_main()`."""
     Pyepggrab.main(
         version=GRABBER_VERSION,
         description=GRABBER_DESCRIPTION,
         caps=GRABBER_CAPABILITIES,
         config_root=GrabberConfig,
-        config_encoder=GrabberConfigEncoder,
         **kwargs,
     )
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/request_proc.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/request_proc.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/utils.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/utils.py`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.2/pyepggrab/grabbers/hu_porthu/xml_utils.py` & `pyepggrab-0.1.dev1/pyepggrab/grabbers/hu_porthu/xml_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,16 @@
     if season_num in (None, ""):
         subt = append_if_not_empty(subt, ", ", episode_num, ". rész")
     else:
         subt = append_if_not_empty(subt, "/", episode_num, ". rész")
     subt = append_if_not_empty(subt, ", ", release_date)
     if subt not in (None, ""):
         subt = f"({subt})"
-    return append_if_not_empty(episode_title, " - ", subt)
+    subt = append_if_not_empty(episode_title, " - ", subt)
+    return subt
 
 
 def create_xprogramme(  # noqa: PLR0912, PLR0915
     progjsons: List[Dict],
     response: Optional[requests.Response] = None,
 ) -> List[XmltvProgramme]:
     """Build an XMLTV program from json and by scraping the page of the program."""
```

### Comparing `pyepggrab-0.1.2/pyepggrab/resources/xmltv.dtd` & `pyepggrab-0.1.dev1/pyepggrab/resources/xmltv.dtd`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.2/.gitignore` & `pyepggrab-0.1.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.2/LICENSE.txt` & `pyepggrab-0.1.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.2/README.md` & `pyepggrab-0.1.dev1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,65 +9,40 @@
 original XMLTV project, and any software uses the original XMLTV project
 can use these grabbers without any modification.
 
 To avoid name conflicts, pyepggrab grabbers use the prefix `tv_grab_pyepg_`.
 
 ## Installation
 
+Currently, there are no premade packages available, but this expected to change
+in the future.
+
 If the functionality of `tv_find_grabbers` is required the one in the
 original [XMLTV][xmltv] project can be used until we provide an alternative.
 (On the [Roadmap](#roadmap))
 
-### From package
-
-pyepggrab is available on PyPi: https://pypi.org/project/pyepggrab/
-
-Install it with your preferred package manager.
-
-For example, with `pip`
-```
-pip install pyepggrab
-```
-
-or with `pipx`
-```
-pipx install pyepggrab
-```
+To install from source, create a wheel package (this requires `hatch`):
 
-### From source
+> `hatch build`
 
-To install from source, create a wheel package (this requires `hatch`):
+and install it with your preferred package manager (`pipx` in the example):
 
-```
-hatch build
-```
-
-and install it with your preferred package manager.
-
-For example, with `pip`
-```
-pip install dist/pyepggrab-*.whl
-```
-
-or with `pipx`
-```
-pipx install dist/pyepggrab-*.whl
-```
+> `pipx install dist/pyepggrab-*.whl`
 
 ## Available grabbers:
 
 | Country | Guide source      | Grabber                |
 |:-------:|-------------------|------------------------|
 | HU      | [port.hu][porthu] | [hu_porthu][hu_porthu] |
 
 [porthu]: https://port.hu
 [hu_porthu]: pyepggrab/grabbers/hu_porthu
 
 ## Roadmap
 
 In no particular order
 
-- [x] Upload a package to PyPi
+- [ ] Upload a package to PyPi
 - [ ] Write an example grabber to demonstrate the usage of pyepggrab
 - [ ] Write tools to make it standalone (`tv_find_grabbers`, `tv_validate_*`)
 
 [xmltv]: https://github.com/XMLTV/xmltv
```

### Comparing `pyepggrab-0.1.2/pyproject.toml` & `pyepggrab-0.1.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyepggrab-0.1.2/PKG-INFO` & `pyepggrab-0.1.dev1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyepggrab
-Version: 0.1.2
+Version: 0.1.dev1
 Summary: Drop in replacement/extension to xmltv grabbers
 Project-URL: Documentation, https://github.com/pyepggrab/pyepggrab#readme
 Project-URL: Issues, https://github.com/pyepggrab/pyepggrab/issues
 Project-URL: Source, https://github.com/pyepggrab/pyepggrab
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: XMLTV,epg,tv
@@ -43,65 +43,40 @@
 original XMLTV project, and any software uses the original XMLTV project
 can use these grabbers without any modification.
 
 To avoid name conflicts, pyepggrab grabbers use the prefix `tv_grab_pyepg_`.
 
 ## Installation
 
+Currently, there are no premade packages available, but this expected to change
+in the future.
+
 If the functionality of `tv_find_grabbers` is required the one in the
 original [XMLTV][xmltv] project can be used until we provide an alternative.
 (On the [Roadmap](#roadmap))
 
-### From package
-
-pyepggrab is available on PyPi: https://pypi.org/project/pyepggrab/
-
-Install it with your preferred package manager.
-
-For example, with `pip`
-```
-pip install pyepggrab
-```
-
-or with `pipx`
-```
-pipx install pyepggrab
-```
+To install from source, create a wheel package (this requires `hatch`):
 
-### From source
+> `hatch build`
 
-To install from source, create a wheel package (this requires `hatch`):
+and install it with your preferred package manager (`pipx` in the example):
 
-```
-hatch build
-```
-
-and install it with your preferred package manager.
-
-For example, with `pip`
-```
-pip install dist/pyepggrab-*.whl
-```
-
-or with `pipx`
-```
-pipx install dist/pyepggrab-*.whl
-```
+> `pipx install dist/pyepggrab-*.whl`
 
 ## Available grabbers:
 
 | Country | Guide source      | Grabber                |
 |:-------:|-------------------|------------------------|
 | HU      | [port.hu][porthu] | [hu_porthu][hu_porthu] |
 
 [porthu]: https://port.hu
 [hu_porthu]: pyepggrab/grabbers/hu_porthu
 
 ## Roadmap
 
 In no particular order
 
-- [x] Upload a package to PyPi
+- [ ] Upload a package to PyPi
 - [ ] Write an example grabber to demonstrate the usage of pyepggrab
 - [ ] Write tools to make it standalone (`tv_find_grabbers`, `tv_validate_*`)
 
 [xmltv]: https://github.com/XMLTV/xmltv
```

