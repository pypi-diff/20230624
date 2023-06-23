# Comparing `tmp/redis_purse-1.0.0.tar.gz` & `tmp/redis_purse-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_purse-1.0.0.tar", max compression
+gzip compressed data, was "redis_purse-1.1.0.tar", max compression
```

## Comparing `redis_purse-1.0.0.tar` & `redis_purse-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11380 2021-10-25 12:47:57.000000 redis_purse-1.0.0/LICENSE
--rw-r--r--   0        0        0     6999 2023-04-20 13:58:16.641280 redis_purse-1.0.0/README.md
--rw-r--r--   0        0        0     1442 2023-04-20 13:40:10.467231 redis_purse-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      370 2022-01-02 14:59:19.000000 redis_purse-1.0.0/src/purse/__init__.py
--rw-r--r--   0        0        0    40776 2023-04-20 13:51:55.485451 redis_purse-1.0.0/src/purse/collections.py
--rw-r--r--   0        0        0        0 2021-09-15 18:36:12.000000 redis_purse-1.0.0/src/purse/py.typed
--rw-r--r--   0        0        0    13525 2023-04-20 13:52:56.094040 redis_purse-1.0.0/src/purse/redlock.py
--rw-r--r--   0        0        0     7966 1970-01-01 00:00:00.000000 redis_purse-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11380 2021-10-25 12:47:57.000000 redis_purse-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6924 2023-06-23 23:31:29.466987 redis_purse-1.1.0/README.md
+-rw-r--r--   0        0        0     1442 2023-06-23 23:31:29.466987 redis_purse-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      370 2022-01-02 14:59:19.000000 redis_purse-1.1.0/src/purse/__init__.py
+-rw-r--r--   0        0        0    40776 2023-04-20 13:51:55.485451 redis_purse-1.1.0/src/purse/collections.py
+-rw-r--r--   0        0        0        0 2021-09-15 18:36:12.000000 redis_purse-1.1.0/src/purse/py.typed
+-rw-r--r--   0        0        0    14095 2023-06-23 23:31:29.466987 redis_purse-1.1.0/src/purse/redlock.py
+-rw-r--r--   0        0        0     7891 1970-01-01 00:00:00.000000 redis_purse-1.1.0/PKG-INFO
```

### Comparing `redis_purse-1.0.0/LICENSE` & `redis_purse-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_purse-1.0.0/README.md` & `redis_purse-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 High-Level Async-IO Python interface for Redis 6.0.x that provides useful Pythonic abstractions to simplify 
 the usage of Redis as a non-blocking Caching layer, or even as a first-class non-blocking datastore.
 
 Influenced and Inspired by the great library [pottery](https://github.com/brainix/pottery), with
 a few differences in objectives and implementation detail.
 
-* ``purse`` is strictly an Async-IO library that utilizes the excellent Python Redis driver library [aioredis](https://github.com/aio-libs/aioredis-py)
+* ``purse`` is strictly an Async-IO library that utilizes the redis library.
 * ``purse`` tries to adhere as much as possible to familiar APIs and idioms used with familiar python structures
   (``dict``, ``set``, ``list`` among others), but deviates from those conventions in many instances:
   * Due to the ``async/await`` nature of the API, it is difficult and sometimes impossible to use python language constructs such as ``myhash["key"] = "value"`` - 
     as of Python 3.10, the language simply doesn't provide async-io methods for those operations and idioms 
   * ``purse`` tries to expose, as much as possible, Redis rich features such as key TTL and pattern matching, among others
 
 Optionally, collections in this library use [pydantic](https://github.com/samuelcolvin/pydantic)
```

### Comparing `redis_purse-1.0.0/pyproject.toml` & `redis_purse-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "redis-purse"
-version = "1.0.0"
+version = "1.1.0"
 description = "High Level Asyncio interface to redis"
 license = "Apache-2.0"
 authors = ["mk <mk@plataux.com>"]
 maintainers = []
 readme = "README.md"
 homepage = "https://plataux.com"
 repository = "https://github.com/plataux/purse"
```

### Comparing `redis_purse-1.0.0/src/purse/collections.py` & `redis_purse-1.1.0/src/purse/collections.py`

 * *Files identical despite different names*

### Comparing `redis_purse-1.0.0/src/purse/redlock.py` & `redis_purse-1.1.0/src/purse/redlock.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                  'masters',
                  'raise_on_redis_errors',
                  'auto_release_time',
                  'num_extensions',
                  'context_manager_blocking',
                  'context_manager_timeout',
                  '_uuid',
-                 '_extension_num',)
+                 '_current_extension_count',)
 
     @property
     def key(self) -> str:
         return self._key
 
     @key.setter
     def key(self, value: str) -> None:
@@ -83,27 +83,38 @@
 
     def __init__(self, key, masters: List[Redis], raise_on_redis_errors=False,
                  auto_release_time: int = AUTO_RELEASE_TIME,
                  num_extensions: int = NUM_EXTENSIONS,
                  context_manager_blocking: bool = True,
                  context_manager_timeout: float = -1,
                  ):
+        """
+        Create a distributed lock object
+
+        :param key:
+        :param masters: a list of redis connection objects
+        :param raise_on_redis_errors:
+        :param auto_release_time: milliseconds to auto-release the lock if not extended
+        :param num_extensions: -1 for infinite extensions
+        :param context_manager_blocking: block if locked
+        :param context_manager_timeout: optional timeout, or -1 for infinite
+        """
         if not context_manager_blocking and context_manager_timeout != -1:
             raise ValueError("can't specify a timeout for a non-blocking call")
 
         self.key = key
         self.masters = masters
         self.raise_on_redis_errors = raise_on_redis_errors
 
         self.auto_release_time = auto_release_time
         self.num_extensions = num_extensions
         self.context_manager_blocking = context_manager_blocking
         self.context_manager_timeout = context_manager_timeout
         self._uuid = ''
-        self._extension_num = 0
+        self._current_extension_count = 0
 
         self.__reg_scripts()
 
     def __reg_scripts(self):
         """
         register LOA scripts with any of the master clients, and store them in class fields
         It seems that this doesn't actually do any networking, but it does assume that all masters
@@ -149,15 +160,15 @@
         Return False if the lock was not successfully set with the majority of Redis Masters, or
         Raise an Exception if ``raise_on_redis_errors`` parameter is set
 
         :param raise_on_redis_errors:
         :return:
         """
         self._uuid = str(uuid4())
-        self._extension_num = 0
+        self._current_extension_count = 0
 
         aws = [asyncio.create_task(self.__acquire_master(m)) for m in self.masters]
 
         num_masters_acquired, redis_errors = 0, []
 
         timer = MilliTimer()
 
@@ -313,30 +324,32 @@
                         return max(validity_time, 0)
 
         self._check_enough_masters_up(raise_on_redis_errors, redis_errors)
         return 0
 
     async def extend(self, *, raise_on_redis_errors: Optional[bool] = None) -> None:
 
-        if self._extension_num >= self.num_extensions:
+        if self.num_extensions <= -1:
+            pass
+        elif self._current_extension_count >= self.num_extensions:
             raise RuntimeError("Exceeded Number of Extensions cap")
 
         aws = [asyncio.create_task(self.__extend_master(m)) for m in self.masters]
 
         num_masters_extended, redis_errors = 0, []
 
         for aw in asyncio.as_completed(aws):
             try:
                 res = await aw  # that's a bool
                 num_masters_extended += res
             except RedisError as error:
                 redis_errors.append(error)
             else:
                 if num_masters_extended > len(self.masters) // 2:
-                    self._extension_num += 1
+                    self._current_extension_count += 1
                     return
 
         self._check_enough_masters_up(raise_on_redis_errors, redis_errors)
         raise RuntimeError("Trying to extend an unlocked lock")
 
     async def release(self, *, raise_on_redis_errors: Optional[bool] = None) -> None:
```

### Comparing `redis_purse-1.0.0/PKG-INFO` & `redis_purse-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-purse
-Version: 1.0.0
+Version: 1.1.0
 Summary: High Level Asyncio interface to redis
 Home-page: https://plataux.com
 License: Apache-2.0
 Keywords: key-value,caching,messaging
 Author: mk
 Author-email: mk@plataux.com
 Requires-Python: >=3.8,<4
@@ -28,15 +28,15 @@
 
 High-Level Async-IO Python interface for Redis 6.0.x that provides useful Pythonic abstractions to simplify 
 the usage of Redis as a non-blocking Caching layer, or even as a first-class non-blocking datastore.
 
 Influenced and Inspired by the great library [pottery](https://github.com/brainix/pottery), with
 a few differences in objectives and implementation detail.
 
-* ``purse`` is strictly an Async-IO library that utilizes the excellent Python Redis driver library [aioredis](https://github.com/aio-libs/aioredis-py)
+* ``purse`` is strictly an Async-IO library that utilizes the redis library.
 * ``purse`` tries to adhere as much as possible to familiar APIs and idioms used with familiar python structures
   (``dict``, ``set``, ``list`` among others), but deviates from those conventions in many instances:
   * Due to the ``async/await`` nature of the API, it is difficult and sometimes impossible to use python language constructs such as ``myhash["key"] = "value"`` - 
     as of Python 3.10, the language simply doesn't provide async-io methods for those operations and idioms 
   * ``purse`` tries to expose, as much as possible, Redis rich features such as key TTL and pattern matching, among others
 
 Optionally, collections in this library use [pydantic](https://github.com/samuelcolvin/pydantic)
```

