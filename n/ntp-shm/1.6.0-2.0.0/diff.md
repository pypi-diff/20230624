# Comparing `tmp/ntp-shm-1.6.0.tar.gz` & `tmp/ntp-shm-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntp-shm-1.6.0.tar", last modified: Sat Oct  8 18:33:58 2022, max compression
+gzip compressed data, was "ntp-shm-2.0.0.tar", last modified: Sat Jun 24 14:21:30 2023, max compression
```

## Comparing `ntp-shm-1.6.0.tar` & `ntp-shm-2.0.0.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2022-10-08 18:33:58.990950 ntp-shm-1.6.0/
--rw-r--r--   0 stefan     (501) staff       (20)     1074 2021-09-18 14:48:40.000000 ntp-shm-1.6.0/LICENSE
--rw-r--r--   0 stefan     (501) staff       (20)     4862 2022-10-08 18:33:58.991018 ntp-shm-1.6.0/PKG-INFO
--rw-r--r--   0 stefan     (501) staff       (20)     4080 2022-10-08 18:18:03.000000 ntp-shm-1.6.0/README.md
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2022-10-08 18:33:58.989986 ntp-shm-1.6.0/ntp_shm/
--rw-r--r--   0 stefan     (501) staff       (20)       76 2022-10-08 18:18:03.000000 ntp-shm-1.6.0/ntp_shm/__init__.py
--rw-r--r--   0 stefan     (501) staff       (20)       63 2021-09-19 20:46:30.000000 ntp-shm-1.6.0/ntp_shm/__main__.py
--rw-r--r--   0 stefan     (501) staff       (20)     2313 2021-09-19 20:46:30.000000 ntp-shm-1.6.0/ntp_shm/data.py
--rw-r--r--   0 stefan     (501) staff       (20)     2797 2022-10-08 18:18:03.000000 ntp-shm-1.6.0/ntp_shm/main.py
--rw-r--r--   0 stefan     (501) staff       (20)     4280 2022-10-08 18:18:03.000000 ntp-shm-1.6.0/ntp_shm/memory.py
--rw-r--r--   0 stefan     (501) staff       (20)     4786 2022-10-08 18:18:03.000000 ntp-shm-1.6.0/ntp_shm/nmea.py
--rw-r--r--   0 stefan     (501) staff       (20)     1534 2021-09-19 20:46:30.000000 ntp-shm-1.6.0/ntp_shm/util.py
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2022-10-08 18:33:58.990475 ntp-shm-1.6.0/ntp_shm.egg-info/
--rw-r--r--   0 stefan     (501) staff       (20)     4862 2022-10-08 18:33:58.000000 ntp-shm-1.6.0/ntp_shm.egg-info/PKG-INFO
--rw-r--r--   0 stefan     (501) staff       (20)      313 2022-10-08 18:33:58.000000 ntp-shm-1.6.0/ntp_shm.egg-info/SOURCES.txt
--rw-r--r--   0 stefan     (501) staff       (20)        1 2022-10-08 18:33:58.000000 ntp-shm-1.6.0/ntp_shm.egg-info/dependency_links.txt
--rw-r--r--   0 stefan     (501) staff       (20)        8 2022-10-08 18:33:58.000000 ntp-shm-1.6.0/ntp_shm.egg-info/top_level.txt
--rw-r--r--   0 stefan     (501) staff       (20)       90 2021-09-19 20:46:30.000000 ntp-shm-1.6.0/pyproject.toml
-drwxr-xr-x   0 stefan     (501) staff       (20)        0 2022-10-08 18:33:58.990591 ntp-shm-1.6.0/scripts/
--rwxr-xr-x   0 stefan     (501) staff       (20)       51 2021-09-19 20:46:15.000000 ntp-shm-1.6.0/scripts/ntp-shm
--rw-r--r--   0 stefan     (501) staff       (20)     1024 2022-10-08 18:33:58.991304 ntp-shm-1.6.0/setup.cfg
--rw-r--r--   0 stefan     (501) staff       (20)       37 2021-09-19 02:25:13.000000 ntp-shm-1.6.0/setup.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-24 14:21:30.301836 ntp-shm-2.0.0/
+-rw-r--r--   0 stefan     (501) staff       (20)     1074 2021-09-18 14:48:40.000000 ntp-shm-2.0.0/LICENSE
+-rw-r--r--   0 stefan     (501) staff       (20)     4890 2023-06-24 14:21:30.301689 ntp-shm-2.0.0/PKG-INFO
+-rw-r--r--   0 stefan     (501) staff       (20)     4080 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/README.md
+-rw-r--r--   0 stefan     (501) staff       (20)     1107 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/pyproject.toml
+-rw-r--r--   0 stefan     (501) staff       (20)       38 2023-06-24 14:21:30.301873 ntp-shm-2.0.0/setup.cfg
+-rw-r--r--   0 stefan     (501) staff       (20)       37 2021-09-19 02:25:13.000000 ntp-shm-2.0.0/setup.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-24 14:21:30.297118 ntp-shm-2.0.0/src/
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-24 14:21:30.298444 ntp-shm-2.0.0/src/ntp_shm/
+-rw-r--r--   0 stefan     (501) staff       (20)       76 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/src/ntp_shm/__init__.py
+-rw-r--r--   0 stefan     (501) staff       (20)       63 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/src/ntp_shm/__main__.py
+-rw-r--r--   0 stefan     (501) staff       (20)     2304 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/src/ntp_shm/data.py
+-rw-r--r--   0 stefan     (501) staff       (20)     2763 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/src/ntp_shm/main.py
+-rw-r--r--   0 stefan     (501) staff       (20)     4345 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/src/ntp_shm/memory.py
+-rw-r--r--   0 stefan     (501) staff       (20)     4865 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/src/ntp_shm/nmea.py
+-rw-r--r--   0 stefan     (501) staff       (20)     1627 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/src/ntp_shm/util.py
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-24 14:21:30.300962 ntp-shm-2.0.0/src/ntp_shm.egg-info/
+-rw-r--r--   0 stefan     (501) staff       (20)     4890 2023-06-24 14:21:30.000000 ntp-shm-2.0.0/src/ntp_shm.egg-info/PKG-INFO
+-rw-r--r--   0 stefan     (501) staff       (20)      492 2023-06-24 14:21:30.000000 ntp-shm-2.0.0/src/ntp_shm.egg-info/SOURCES.txt
+-rw-r--r--   0 stefan     (501) staff       (20)        1 2023-06-24 14:21:30.000000 ntp-shm-2.0.0/src/ntp_shm.egg-info/dependency_links.txt
+-rw-r--r--   0 stefan     (501) staff       (20)       46 2023-06-24 14:21:30.000000 ntp-shm-2.0.0/src/ntp_shm.egg-info/entry_points.txt
+-rw-r--r--   0 stefan     (501) staff       (20)       47 2023-06-24 14:21:30.000000 ntp-shm-2.0.0/src/ntp_shm.egg-info/requires.txt
+-rw-r--r--   0 stefan     (501) staff       (20)        8 2023-06-24 14:21:30.000000 ntp-shm-2.0.0/src/ntp_shm.egg-info/top_level.txt
+drwxr-xr-x   0 stefan     (501) staff       (20)        0 2023-06-24 14:21:30.301449 ntp-shm-2.0.0/tests/
+-rw-r--r--   0 stefan     (501) staff       (20)     4529 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/tests/test_data.py
+-rw-r--r--   0 stefan     (501) staff       (20)     5097 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/tests/test_nmea_basic.py
+-rw-r--r--   0 stefan     (501) staff       (20)     1642 2022-10-08 18:18:03.000000 ntp-shm-2.0.0/tests/test_nmea_stream.py
+-rw-r--r--   0 stefan     (501) staff       (20)     1956 2023-06-24 14:21:03.000000 ntp-shm-2.0.0/tests/test_util.py
```

### Comparing `ntp-shm-1.6.0/LICENSE` & `ntp-shm-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ntp-shm-1.6.0/PKG-INFO` & `ntp-shm-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: ntp-shm
-Version: 1.6.0
+Version: 2.0.0
 Summary: Pure Python NTP shared memory library.
-Home-page: https://gitlab.com/srfilipek/ntp-shm
-Author: Stefan R. Filipek
-Author-email: srfilipek@gmail.com
+Author-email: "Stefan R. Filipek" <srfilipek@gmail.com>
+Project-URL: Homepage, https://gitlab.com/srfilipek/ntp-shm
 Project-URL: Bug Tracker, https://gitlab.com/srfilipek/ntp-shm/-/issues
 Keywords: gps,time,chrony,ntp,serial,shm,ntpshm
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking :: Time Synchronization
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Overview
 A pure Python interface to the NTP shared memory segment with no external
 dependencies.
 
 The only platform-dependent part of this library is the `SHM_CREAT` constant,
 which seems to always be the octal value of 01000 (Linux and BSDs). Technically
 the size of `time_t` is also platform-dependent, but it's 2021 and this should
 be 64 bit everywhere.
 
 # Prerequisites
-Python: 3.6+
+Python: 3.7+
 
 OSs: Posix-compliant with the System V shared memory interface.
 
 This uses `ctypes` for direct access to memory and shared memory routines. This
 will dynamically load the system's C library to access `shmget()` and `shmat()`
 functions.
```

### Comparing `ntp-shm-1.6.0/README.md` & `ntp-shm-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 The only platform-dependent part of this library is the `SHM_CREAT` constant,
 which seems to always be the octal value of 01000 (Linux and BSDs). Technically
 the size of `time_t` is also platform-dependent, but it's 2021 and this should
 be 64 bit everywhere.
 
 # Prerequisites
-Python: 3.6+
+Python: 3.7+
 
 OSs: Posix-compliant with the System V shared memory interface.
 
 This uses `ctypes` for direct access to memory and shared memory routines. This
 will dynamically load the system's C library to access `shmget()` and `shmat()`
 functions.
```

### Comparing `ntp-shm-1.6.0/ntp_shm/data.py` & `ntp-shm-2.0.0/src/ntp_shm/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 class ShmTime(ctypes.Structure):
     """Structure for NTP's shared memory segment
 
     See https://docs.ntpsec.org/latest/driver_shm.html
 
     Fields renamed slightly.
     """
+
     _fields_ = (
         ("mode", ctypes.c_int),
         ("count", ctypes.c_int),  # volatile
         ("clock_time_sec", ctypes.c_int64),  # time_t
         ("clock_time_usec", ctypes.c_int),
         ("receive_time_sec", ctypes.c_int64),  # time_t
         ("receive_time_usec", ctypes.c_int),
@@ -24,53 +25,45 @@
         ("valid", ctypes.c_int),  # volatile
         ("clock_time_nsec", ctypes.c_uint),
         ("receive_time_nsec", ctypes.c_uint),
         ("_dummy", ctypes.c_int * 8),
     )
 
     @property
-    def clock_dt(self):
+    def clock_dt(self) -> datetime.datetime:
         """Datetime representation of the clock time.
 
         Note that python datetime does not support nanosecond precision."""
         return util.ns_to_datetime(self.clock_ns)
 
     @property
-    def clock_ns(self):
+    def clock_ns(self) -> int:
         """Clock time in integer nanoseconds"""
-        return util.tuple_to_ns(
-            self.clock_time_sec,
-            self.clock_time_usec,
-            self.clock_time_nsec
-        )
+        return util.tuple_to_ns(self.clock_time_sec, self.clock_time_usec, self.clock_time_nsec)
 
     @clock_ns.setter
-    def clock_ns(self, time_ns):
+    def clock_ns(self, time_ns: int) -> None:
         """Clock time in integer nanoseconds"""
         time_sec, time_usec, time_nsec = util.ns_to_tuple(time_ns)
         self.clock_time_sec = time_sec
         self.clock_time_usec = time_usec
         self.clock_time_nsec = time_nsec
 
     @property
-    def receive_dt(self):
+    def receive_dt(self) -> datetime.datetime:
         """Datetime representation of the receive time.
 
         Note that python datetime does not support nanosecond precision."""
         return util.ns_to_datetime(self.receive_ns)
 
     @property
-    def receive_ns(self):
+    def receive_ns(self) -> int:
         """Receive time in integer nanoseconds."""
-        return util.tuple_to_ns(
-            self.receive_time_sec,
-            self.receive_time_usec,
-            self.receive_time_nsec
-        )
+        return util.tuple_to_ns(self.receive_time_sec, self.receive_time_usec, self.receive_time_nsec)
 
     @receive_ns.setter
-    def receive_ns(self, time_ns):
+    def receive_ns(self, time_ns: int) -> None:
         """Clock time in integer nanoseconds"""
         time_sec, time_usec, time_nsec = util.ns_to_tuple(time_ns)
         self.receive_time_sec = time_sec
         self.receive_time_usec = time_usec
         self.receive_time_nsec = time_nsec
```

### Comparing `ntp-shm-1.6.0/ntp_shm/main.py` & `ntp-shm-2.0.0/src/ntp_shm/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 import argparse
-import datetime
-import select
 import sys
-import time
+from typing import Optional
 
-from . import __version__
-from . import data
-from . import memory
-from . import nmea
-from . import util
+from . import __version__, memory, nmea
 
 
-def dump(segment=0):
+def dump(segment: int = 0):
     """Dump the current contents of the NTP shared memory segment"""
     with memory.NtpShm(segment) as shm:
         snap = shm.read()
         field_names = (fn for fn, _ in snap._fields_)
 
         for field_name in field_names:
             if field_name.startswith("_"):
@@ -25,73 +19,72 @@
         # Special properties
         print(f"clock_ns: {snap.clock_ns}")
         print(f"clock_dt: {snap.clock_dt}")
         print(f"receive_ns: {snap.receive_ns}")
         print(f"receive_dt: {snap.receive_dt}")
 
 
-def bridge(path, segment=0, verbose=False):
-    """Parse NMEA sentences from the given file path and write to NTP SHM
-    """
+def bridge(path: str, segment: int = 0, verbose: bool = False) -> None:
+    """Parse NMEA sentences from the given file path and write to NTP SHM"""
     print(f"ntp_shm v{__version__} bridging {path} to segment {segment}")
 
     shm = memory.NtpShm(segment)
 
     for clock_ns, recv_ns in nmea.nmea_time(path):
         if verbose:
             print(f"Updating segment {shm.segment} with clock {clock_ns} received at {recv_ns}")
 
         shm.update(clock_ns, recv_ns)
-        last_ns = clock_ns
 
 
-def main(args=None):
+def main(args: Optional[list[str]] = None) -> None:
     if args is None:
         args = sys.argv
 
     parser = argparse.ArgumentParser("ntp-shm")
     parser.add_argument(
-        "--version", action="store_true", default=False,
-        help="Print the current version and exit"
+        "--version",
+        action="store_true",
+        default=False,
+        help="Print the current version and exit",
     )
     subparsers = parser.add_subparsers()
 
     # dump command
-    p_dump = subparsers.add_parser(
-        "dump",
-        help="Dump the contents of the given shared memory segment."
-    )
+    p_dump = subparsers.add_parser("dump", help="Dump the contents of the given shared memory segment.")
     p_dump.add_argument(
-        "--segment", "-s", type=int, default=0,
-        help="Shared memory segment index (0-??)."
+        "--segment",
+        "-s",
+        type=int,
+        default=0,
+        help="Shared memory segment index (0-??).",
     )
     p_dump.set_defaults(func=dump)
 
     # bridge command
-    p_bridge = subparsers.add_parser(
-        "bridge",
-        help="Bridge a NMEA0183 stream to the NTP shared memory."
-    )
-    p_bridge.add_argument(
-        "--segment", "-s", type=int, default=0,
-        help="Shared memory segment index (0-??)."
-    )
+    p_bridge = subparsers.add_parser("bridge", help="Bridge a NMEA0183 stream to the NTP shared memory.")
     p_bridge.add_argument(
-        "--path", "-p", type=str, default="/dev/stdin",
-        help="File to read NMEA stream from, defaulting to stdin"
+        "--segment",
+        "-s",
+        type=int,
+        default=0,
+        help="Shared memory segment index (0-??).",
     )
     p_bridge.add_argument(
-        "--verbose", "-v", action="store_true", default=False,
-        help="Verbose output"
+        "--path",
+        "-p",
+        type=str,
+        default="/dev/stdin",
+        help="File to read NMEA stream from, defaulting to stdin",
     )
+    p_bridge.add_argument("--verbose", "-v", action="store_true", default=False, help="Verbose output")
     p_bridge.set_defaults(func=bridge)
 
     # Parse and run
-    args = parser.parse_args(args[1:])
-    arg_dict = args.__dict__
+    arg_dict = parser.parse_args(args[1:]).__dict__
 
     version_flag = arg_dict.pop("version", False)
     if version_flag:
         print(f"ntp-shm v{__version__}")
         exit(0)
 
     func = arg_dict.pop("func", None)
```

### Comparing `ntp-shm-1.6.0/ntp_shm/memory.py` & `ntp-shm-2.0.0/src/ntp_shm/memory.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 
 # Fix issues on 64-bit machines :(
 libc.memmove.restype = ctypes.c_void_p
 libc.memmove.argtypes = ctypes.c_void_p, ctypes.c_void_p, ctypes.c_size_t
 libc.shmat.restype = ctypes.c_void_p
 libc.shmat.argtypes = ctypes.c_int, ctypes.c_void_p, ctypes.c_int
 libc.shmdt.restype = ctypes.c_int
-libc.shmdt.argtypes = ctypes.c_void_p,
+libc.shmdt.argtypes = (ctypes.c_void_p,)
 libc.shmget.restype = ctypes.c_int
 libc.shmget.argtypes = ctypes.c_int, ctypes.c_size_t, ctypes.c_int
 
-NTP_SHM_KEY_BASE = 0x4e545030
+NTP_SHM_KEY_BASE = 0x4E545030
 IPC_CREAT = 0o1000  # Octal. Holds for most systems.
 
 LEAP_NOWARNING = 0
 LEAP_ADDSECOND = 1
 LEAP_DELSECOND = 2
 LEAP_NOTINSYNC = 3
 
 
 class NtpShm:
     """An interface to an NTP Shared Memory time segment.
 
     This wraps up all the scary direct memory access.
     """
 
-    def __init__(self, segment=0, mode=0o666):
+    def __init__(self, segment: int = 0, mode: int = 0o666):
         """Create a shared memory segment.
 
         Args:
-            segment (int): Segment number
-            mode (int): Permission mode to use if creating
+            segment: Segment number
+            mode: Permission mode to use if creating
         """
         if segment < 0:
             raise ValueError("Segment must be a non-negative integer")
 
         self._segment = segment
 
         # Get a reference
@@ -51,64 +51,64 @@
 
         # Memory map
         self._seg = libc.shmat(shmid, None, 0)
         if self._seg == -1:
             errcode = errno.errorcode[ctypes.get_errno()]
             raise OSError(f"shmat failed for segment {segment}, id {shmid}: {errcode}")
 
-    def __enter__(self):
+    def __enter__(self) -> "NtpShm":
         return self
 
-    def __exit__(self, *exc):
+    def __exit__(self, *exc) -> None:
         self.close()
 
-    def close(self):
+    def close(self) -> None:
         libc.shmdt(self._seg)
         self._seg = 0
 
     @property
-    def segment(self):
+    def segment(self) -> int:
         return self._segment
 
     @property
-    def key(self):
+    def key(self) -> int:
         return NTP_SHM_KEY_BASE + self._segment
 
     @property
-    def ref(self):
+    def ref(self) -> ShmTime:
         """Direct memory reference as a ShmTime object.
 
         Returns:
-            ShmTime: Reference to the shared segment
+            Reference to the shared segment
         """
         return ctypes.cast(self._seg, ctypes.POINTER(ShmTime)).contents
 
-    def read(self):
+    def read(self) -> ShmTime:
         """Get a copy of the NTP shm segment.
 
         Note that this is a direct copy and does not abide by any mode.
 
         Returns:
-            ShmTime: Shared memory time structure
+            Shared memory time structure
         """
         shm_time = ShmTime()
         libc.memmove(ctypes.byref(shm_time), self._seg, ctypes.sizeof(ShmTime))
         return shm_time
 
-    def write(self, shm_time):
+    def write(self, shm_time: ShmTime) -> None:
         """Write to the NTP shm segment.
 
         Note that this is a direct copy and does not abide by any mode.
 
         Args:
-            shm_time (ShmTime): Shared memory time structure
+            shm_time: Shared memory time structure
         """
         libc.memmove(self._seg, ctypes.byref(shm_time), ctypes.sizeof(ShmTime))
 
-    def update(self, clock_ns, receive_ns, precision=-1, leap=0):
+    def update(self, clock_ns: int, receive_ns: int, precision: int = -1, leap: int = 0) -> None:
         """Update the shared memory segment with the given time using mode 1.
 
         Note that updating shared memory is rife with pitfalls. Memory barriers
         should normally be used to ensure proper memory ordering and multi-core
         cache synchronization. However, we have no such mechanism in Python.
         Cross your fingers and hope for the best.
 
@@ -120,18 +120,18 @@
         Leap indicates if there's a pending leap event. Examples:
             0: No warning
             1: Adding a second
             2: Deleting a second
             3: Not synchronized
 
         Args:
-            clock_ns (int): Clock time (GPS clock), in ns
-            receive_ns (int): System time when the clock time was received, in ns
-            precision (int): Precision indicator
-            leap (int): Leap second warning
+            clock_ns: Clock time (GPS clock), in ns
+            receive_ns: System time when the clock time was received, in ns
+            precision: Precision indicator
+            leap: Leap second warning
         """
         seg = self.ref
 
         seg.valid = 0
         seg.mode = 1
         seg.count += 1
```

### Comparing `ntp-shm-1.6.0/ntp_shm/nmea.py` & `ntp-shm-2.0.0/src/ntp_shm/nmea.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,93 @@
 import datetime
-import operator
 import re
+from typing import Iterable
 
 from . import util
 
-
 NMEA_MAX_LEN = 128  # Actually 82, but let's not be pedantic
 NTP_MIN_FIX = 3
 
 # Time jumps outside this range are invalid
 MIN_DELTA = datetime.timedelta(seconds=0.5)
 MAX_DELTA = datetime.timedelta(seconds=2)
 
 US_IN_MS = 1000
 US_IN_CS = 10000
 
 
 class InvalidFix(RuntimeError):
     """Indicates the GPS does not have a fix"""
+
     pass
 
 
-def _check(sentence, checksum):
-    """Validate the checksum for the given NMEA sentence.
-    """
+def _check(sentence: str, checksum: int) -> None:
+    """Validate the checksum for the given NMEA sentence."""
     actual = 0
     for c in sentence:
         actual ^= ord(c)
 
     if actual != checksum:
         raise ValueError(f"Checksum error. Given 0x{checksum:02x}, actual 0x{actual:02x}")
 
 
-def _nmea_line_gen(path, msg_type):
-    """Generator that hides a bunch of nasty nested nastyness"""
-    with open(path, 'r') as f:
+def _nmea_line_gen(path: str, msg_type: str) -> Iterable[str]:
+    """Generator that hides a bunch of nasty nested nastiness"""
+    with open(path, "r") as f:
         while True:
             try:
                 line = f.readline(NMEA_MAX_LEN)
                 if not line:
                     break
                 if re.match(r"^\$" + msg_type, line):
                     yield line.strip()
             except UnicodeDecodeError:
                 # Ignore. Just bad data.
                 pass
 
 
-def parse(line):
-    """Parse a given GPS NMEA sentence, returning the message type and its fields.
-    """
+def parse(line: str) -> tuple[str, list[str]]:
+    """Parse a given GPS NMEA sentence, returning the message type and its fields."""
     if len(line) < 5 or not line.startswith("$") or not line[-3] == "*":
         raise ValueError("Not a NMEA sentence")
 
     sentence, checksum = line[1:].rsplit("*", 1)
     _check(sentence, int(checksum, 16))
 
     msg, rest = sentence.split(",", 1)
 
     return msg, rest.split(",")
 
 
-def gprmc_time(fields, differential=False):
+def gprmc_time(fields: list[str], differential: bool = False) -> datetime.datetime:
     """Parse GPRMC time from the given array of fields
 
     This will only accept sentence that have a valid fix, either Autonomous or
     Differential. If differential is True, then it only accepts Differential
     mode.
 
     Args:
-        fields (list): NMEA stentence fields
-        differential (bool): Only accept differential mode
+        fields: NMEA stentence fields
+        differential: Only accept differential mode
 
     Returns:
-        datetime.datetime: Datetime in UTC
+        Datetime in UTC
 
     Raises:
         InvalidFix if the sentence indicates no fix
         ValueError if there's an invalid value for the date or time
     """
     utc_time = fields[0]
     valid = fields[1]
     date = fields[8]
     mode = fields[11] if len(fields) > 11 else None
 
     # Skip if invalid
-    if (valid != 'A' or mode not in (None, 'A', 'D') or (differential and mode != 'D')):
+    if valid != "A" or mode not in (None, "A", "D") or (differential and mode != "D"):
         raise InvalidFix(f"Invalid fix: {valid} | {mode}")
 
     # Parse the date
     if len(date) != 6:
         raise ValueError(f"Invalid date field: {date}")
 
     try:
@@ -102,42 +100,38 @@
     # Parse the time
     if len(utc_time) < 6:
         raise ValueError(f"Invalid time field: {utc_time}")
 
     try:
         hour = int(utc_time[0:2], 10)
         minute = int(utc_time[2:4], 10)
-        str_sec_ms = utc_time[4:].split('.')
+        str_sec_ms = utc_time[4:].split(".")
         second = int(str_sec_ms[0], 10)
         us = 0
         if len(str_sec_ms) > 1:
             if len(str_sec_ms[1]) == 2:
                 us = int(str_sec_ms[1], 10) * US_IN_CS
             elif len(str_sec_ms[1]) == 3:
                 us = int(str_sec_ms[1], 10) * US_IN_MS
             else:
                 raise ValueError("Invalid fractional seconds")
     except ValueError:
         raise ValueError(f"Invalid time field: {utc_time}")
 
-    return datetime.datetime(
-        year, month, day,
-        hour, minute, second, us,
-        datetime.timezone.utc
-    )
+    return datetime.datetime(year, month, day, hour, minute, second, us, datetime.timezone.utc)
 
 
-def nmea_time(path):
+def nmea_time(path: str) -> Iterable[tuple[int, int]]:
     """Fetch time from the NMEA0183 sentences at the given path
 
     Args:
-        path (str): Path to the file-like device spitting out NMEA sentences
+        path: Path to the file-like device spitting out NMEA sentences
 
     Yields:
-        (int, int): Clock and received time, in nanoseconds
+        A tuple of clock and received time, in nanoseconds
     """
     valid_count = 0
     last_clock_dt = None
 
     for line in _nmea_line_gen(path, "G.RMC"):
         utc_now = datetime.datetime.now(datetime.timezone.utc)
         recv_ns = util.datetime_to_ns(utc_now)
```

### Comparing `ntp-shm-1.6.0/ntp_shm/util.py` & `ntp-shm-2.0.0/src/ntp_shm/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 import datetime
 
 NSEC_IN_SEC = 1000000000
 NSEC_IN_USEC = 1000
 
 
-def datetime_to_ns(dt):
+def datetime_to_ns(dt: datetime.datetime) -> int:
     """Fetch the UTC time in nanoseconds from the given datetime.
 
     If the datetime object is naive, the default Python behavior is to assume
     it is in the system timezone.
     """
     # Explicit conversion so we don't rely on the platform's mktime()
     timestamp = dt.astimezone(datetime.timezone.utc).timestamp()
     nsec = int(timestamp) * NSEC_IN_SEC
     nsec += dt.microsecond * NSEC_IN_USEC
     return nsec
 
 
-def ns_to_datetime(time_ns):
-    """Convert nanoseconds to a datetime object (UTC timezone)
-    """
+def ns_to_datetime(time_ns: int) -> datetime.datetime:
+    """Convert nanoseconds to a datetime object (UTC timezone)"""
     time_sec = time_ns / NSEC_IN_SEC
     return datetime.datetime.fromtimestamp(time_sec, datetime.timezone.utc)
 
 
-def ns_to_tuple(time_ns):
+def ns_to_tuple(time_ns: int) -> tuple[int, int, int]:
     """Return a tuple of seconds, microseconds, nanoseconds from the given time.
 
     Note that microseconds and nanoseconds represent the same offset, just with
     different precision. That is, nanoseconds will *also* containe the value in
     microseconds.
     """
     time_sec = time_ns // NSEC_IN_SEC
     time_nsec = time_ns % NSEC_IN_SEC
     time_usec = time_nsec // NSEC_IN_USEC
 
     return time_sec, time_usec, time_nsec
 
 
-def tuple_to_ns(time_sec, time_usec, time_nsec):
-    """Convert a tuple of seconds, microseconds, nanoseconds, to nanoseconds.
-    """
+def tuple_to_ns(time_sec: int, time_usec: int, time_nsec: int) -> int:
+    """Convert a tuple of seconds, microseconds, nanoseconds, to nanoseconds."""
     time_ns = time_sec * NSEC_IN_SEC
 
     # In case this system does not populate properly
     if time_nsec == 0:
         time_ns += time_usec * NSEC_IN_USEC
     else:
         time_ns += time_nsec
```

### Comparing `ntp-shm-1.6.0/ntp_shm.egg-info/PKG-INFO` & `ntp-shm-2.0.0/src/ntp_shm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: ntp-shm
-Version: 1.6.0
+Version: 2.0.0
 Summary: Pure Python NTP shared memory library.
-Home-page: https://gitlab.com/srfilipek/ntp-shm
-Author: Stefan R. Filipek
-Author-email: srfilipek@gmail.com
+Author-email: "Stefan R. Filipek" <srfilipek@gmail.com>
+Project-URL: Homepage, https://gitlab.com/srfilipek/ntp-shm
 Project-URL: Bug Tracker, https://gitlab.com/srfilipek/ntp-shm/-/issues
 Keywords: gps,time,chrony,ntp,serial,shm,ntpshm
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking :: Time Synchronization
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # Overview
 A pure Python interface to the NTP shared memory segment with no external
 dependencies.
 
 The only platform-dependent part of this library is the `SHM_CREAT` constant,
 which seems to always be the octal value of 01000 (Linux and BSDs). Technically
 the size of `time_t` is also platform-dependent, but it's 2021 and this should
 be 64 bit everywhere.
 
 # Prerequisites
-Python: 3.6+
+Python: 3.7+
 
 OSs: Posix-compliant with the System V shared memory interface.
 
 This uses `ctypes` for direct access to memory and shared memory routines. This
 will dynamically load the system's C library to access `shmget()` and `shmat()`
 functions.
```

