# Comparing `tmp/instagram-archiver-0.0.5.tar.gz` & `tmp/instagram_archiver-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instagram-archiver-0.0.5.tar", last modified: Sun Apr  2 01:57:32 2023, max compression
+gzip compressed data, was "instagram_archiver-0.2.0.tar", max compression
```

## Comparing `instagram-archiver-0.0.5.tar` & `instagram_archiver-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,10 @@
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2023-04-02 01:57:32.834031 instagram-archiver-0.0.5/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      613 2023-04-02 01:57:32.834031 instagram-archiver-0.0.5/PKG-INFO
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      310 2023-04-02 01:53:21.000000 instagram-archiver-0.0.5/README.md
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2023-04-02 01:57:32.834031 instagram-archiver-0.0.5/instagram_archiver/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       44 2023-04-02 01:54:39.000000 instagram-archiver-0.0.5/instagram_archiver/__init__.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      885 2023-04-02 01:22:25.000000 instagram-archiver-0.0.5/instagram_archiver/constants.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      572 2022-06-08 17:37:24.000000 instagram-archiver-0.0.5/instagram_archiver/ig_typing.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     7614 2023-04-02 01:45:12.000000 instagram-archiver-0.0.5/instagram_archiver/main.py
--rw-r-----   0 tatsh     (1000) tatsh     (1000)     2495 2023-04-02 01:24:29.000000 instagram-archiver-0.0.5/instagram_archiver/utils.py
-drwxr-x---   0 tatsh     (1000) tatsh     (1000)        0 2023-04-02 01:57:32.834031 instagram-archiver-0.0.5/instagram_archiver.egg-info/
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      613 2023-04-02 01:57:32.000000 instagram-archiver-0.0.5/instagram_archiver.egg-info/PKG-INFO
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      422 2023-04-02 01:57:32.000000 instagram-archiver-0.0.5/instagram_archiver.egg-info/SOURCES.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)        1 2023-04-02 01:57:32.000000 instagram-archiver-0.0.5/instagram_archiver.egg-info/dependency_links.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       47 2023-04-02 01:57:32.000000 instagram-archiver-0.0.5/instagram_archiver.egg-info/entry_points.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      131 2023-04-02 01:57:32.000000 instagram-archiver-0.0.5/instagram_archiver.egg-info/requires.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       19 2023-04-02 01:57:32.000000 instagram-archiver-0.0.5/instagram_archiver.egg-info/top_level.txt
--rw-r-----   0 tatsh     (1000) tatsh     (1000)       38 2023-04-02 01:57:32.834031 instagram-archiver-0.0.5/setup.cfg
--rw-r-----   0 tatsh     (1000) tatsh     (1000)      919 2023-04-02 01:56:36.000000 instagram-archiver-0.0.5/setup.py
+-rw-r--r--   0        0        0     1080 2023-04-09 18:35:32.311409 instagram_archiver-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0      310 2023-04-02 01:53:21.596308 instagram_archiver-0.2.0/README.md
+-rw-r--r--   0        0        0       44 2023-04-02 01:54:39.428228 instagram_archiver-0.2.0/instagram_archiver/__init__.py
+-rw-r--r--   0        0        0    14066 2023-06-24 03:51:06.849364 instagram_archiver-0.2.0/instagram_archiver/client.py
+-rw-r--r--   0        0        0     3490 2023-04-13 17:30:33.623333 instagram_archiver-0.2.0/instagram_archiver/constants.py
+-rw-r--r--   0        0        0     2361 2023-04-13 21:34:35.792248 instagram_archiver-0.2.0/instagram_archiver/ig_typing.py
+-rw-r--r--   0        0        0     2463 2023-04-13 21:41:21.669932 instagram_archiver-0.2.0/instagram_archiver/main.py
+-rw-r--r--   0        0        0     3169 2023-04-13 21:41:38.791929 instagram_archiver-0.2.0/instagram_archiver/utils.py
+-rw-r--r--   0        0        0      978 2023-06-24 03:51:06.849364 instagram_archiver-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 instagram_archiver-0.2.0/PKG-INFO
```

### Comparing `instagram-archiver-0.0.5/instagram_archiver/utils.py` & `instagram_archiver-0.2.0/instagram_archiver/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,49 @@
+from contextlib import contextmanager
+from os import chdir as os_chdir, getcwd
 from os.path import isfile
 from pathlib import Path
 from types import FrameType
-from typing import (Literal, Optional, Union)
+from typing import Generic, Iterator, Literal, TypeVar
+import json
 import logging
 import sys
 
 from loguru import logger
 import click
 
-__all__ = ('UnknownMimetypeError', 'get_extension', 'write_if_new')
+__all__ = ('UnknownMimetypeError', 'chdir', 'get_extension', 'json_dumps_formatted', 'write_if_new')
 
+T = TypeVar('T')
 
-def write_if_new(target: Union[Path, str],
-                 content: Union[str, bytes],
-                 mode: str = 'w') -> None:
+
+class JSONFormattedString(Generic[T]):  # pylint: disable=too-few-public-methods
+    def __init__(self, formatted: str, original: T) -> None:
+        self.formatted = formatted
+        self.original_value = original
+
+    def __str__(self) -> str:
+        return self.formatted
+
+
+def json_dumps_formatted(obj: T) -> JSONFormattedString[T]:
+    return JSONFormattedString(json.dumps(obj, sort_keys=True, indent=2), obj)
+
+
+@contextmanager
+def chdir(path: str | Path) -> Iterator[None]:
+    old_path = getcwd()
+    os_chdir(path)
+    try:
+        yield
+    finally:
+        chdir(old_path)
+
+
+def write_if_new(target: Path | str, content: str | bytes, mode: str = 'w') -> None:
     if not isfile(target):
         with click.open_file(str(target), mode) as f:
             f.write(content)
 
 
 class UnknownMimetypeError(Exception):
     pass
@@ -30,36 +56,35 @@
         return 'png'
     raise UnknownMimetypeError(mimetype)
 
 
 class InterceptHandler(logging.Handler):  # pragma: no cover
     """Intercept handler taken from Loguru's documentation."""
     def emit(self, record: logging.LogRecord) -> None:
-        level: Union[str, int]
+        level: str | int
         # Get corresponding Loguru level if it exists
         try:
             level = logger.level(record.levelname).name
         except ValueError:
             level = record.levelno
         # Find caller from where originated the logged message
-        frame: Optional[FrameType] = logging.currentframe()
+        frame: FrameType | None = logging.currentframe()
         depth = 2
         while frame and frame.f_code.co_filename == logging.__file__:
             frame = frame.f_back
             depth += 1
-        logger.opt(depth=depth, exception=record.exc_info).log(
-            level, record.getMessage())
+        logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
 
 def setup_log_intercept_handler() -> None:  # pragma: no cover
     """Sets up Loguru to intercept records from the logging module."""
     logging.basicConfig(handlers=(InterceptHandler(),), level=0)
 
 
-def setup_logging(debug: Optional[bool] = False) -> None:
+def setup_logging(debug: bool | None = False) -> None:
     """Shared function to enable logging."""
     if debug:  # pragma: no cover
         setup_log_intercept_handler()
         logger.enable('')
     else:
         logger.configure(handlers=(dict(
             format='<level>{message}</level>',
@@ -71,15 +96,15 @@
 class YoutubeDLLogger:
     def debug(self, message: str) -> None:
         if message.startswith('[debug] '):
             logger.debug(message)
         else:
             logger.info(message)
 
-    def info(self, _: str) -> None:
+    def info(self, message: str) -> None:
         pass
 
     def warning(self, message: str) -> None:
         logger.warning(message)
 
     def error(self, message: str) -> None:
         logger.error(message)
```

