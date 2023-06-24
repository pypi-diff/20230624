# Comparing `tmp/pyUbersolar-0.1.2.tar.gz` & `tmp/pyUbersolar-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyUbersolar-0.1.2.tar", last modified: Fri Feb  3 05:37:01 2023, max compression
+gzip compressed data, was "pyUbersolar-0.1.3.tar", last modified: Sat Jun 24 18:25:49 2023, max compression
```

## Comparing `pyUbersolar-0.1.2.tar` & `pyUbersolar-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 05:37:01.313187 pyUbersolar-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-02-03 05:37:01.313187 pyUbersolar-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 05:37:01.309187 pyUbersolar-0.1.2/pyUbersolar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-02-03 05:37:01.000000 pyUbersolar-0.1.2/pyUbersolar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-03 05:37:01.000000 pyUbersolar-0.1.2/pyUbersolar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 05:37:01.000000 pyUbersolar-0.1.2/pyUbersolar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-03 05:37:01.000000 pyUbersolar-0.1.2/pyUbersolar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-03 05:37:01.000000 pyUbersolar-0.1.2/pyUbersolar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 05:37:01.313187 pyUbersolar-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 05:37:01.309187 pyUbersolar-0.1.2/ubersolar/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/ubersolar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/ubersolar/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 05:37:01.309187 pyUbersolar-0.1.2/ubersolar/adv_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/ubersolar/adv_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/ubersolar/adv_parsers/ubersmart.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/ubersolar/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 05:37:01.309187 pyUbersolar-0.1.2/ubersolar/devices/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/ubersolar/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14356 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/ubersolar/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/ubersolar/devices/ubersmart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/ubersolar/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-02-03 05:36:50.000000 pyUbersolar-0.1.2/ubersolar/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:25:49.476057 pyUbersolar-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-24 18:25:49.476057 pyUbersolar-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:25:49.472057 pyUbersolar-0.1.3/pyUbersolar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-24 18:25:49.000000 pyUbersolar-0.1.3/pyUbersolar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-24 18:25:49.000000 pyUbersolar-0.1.3/pyUbersolar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 18:25:49.000000 pyUbersolar-0.1.3/pyUbersolar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-24 18:25:49.000000 pyUbersolar-0.1.3/pyUbersolar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-24 18:25:49.000000 pyUbersolar-0.1.3/pyUbersolar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 18:25:49.476057 pyUbersolar-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:25:49.472057 pyUbersolar-0.1.3/ubersolar/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/ubersolar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/ubersolar/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:25:49.476057 pyUbersolar-0.1.3/ubersolar/adv_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/ubersolar/adv_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/ubersolar/adv_parsers/ubersmart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/ubersolar/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 18:25:49.476057 pyUbersolar-0.1.3/ubersolar/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/ubersolar/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14279 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/ubersolar/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/ubersolar/devices/ubersmart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/ubersolar/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-24 18:25:39.000000 pyUbersolar-0.1.3/ubersolar/models.py
```

### Comparing `pyUbersolar-0.1.2/LICENSE` & `pyUbersolar-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyUbersolar-0.1.2/PKG-INFO` & `pyUbersolar-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyUbersolar
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library to communicate with UberSolar devices
 Home-page: https://github.com/RenierM26/pyUbersolar
 Author: Renier Moorcroft
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `pyUbersolar-0.1.2/pyUbersolar.egg-info/PKG-INFO` & `pyUbersolar-0.1.3/pyUbersolar.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyUbersolar
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library to communicate with UberSolar devices
 Home-page: https://github.com/RenierM26/pyUbersolar
 Author: Renier Moorcroft
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `pyUbersolar-0.1.2/setup.py` & `pyUbersolar-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name = "pyUbersolar",
     packages = ["ubersolar", "ubersolar.devices", "ubersolar.adv_parsers"],
     install_requires=["async_timeout>=4.0.1", "bleak>=0.17.0", "bleak-retry-connector>=2.9.0", "cryptography>=38.0.3"],
-    version = "0.1.2",
+    version = "0.1.3",
     description = "A library to communicate with UberSolar devices",
     long_description= "API for accessing UberSolar UberSmart devices. Communication to/from the device via Bluetooth. Please view readme on github",
     author="Renier Moorcroft",
     url="https://github.com/RenierM26/pyUbersolar",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `pyUbersolar-0.1.2/ubersolar/__main__.py` & `pyUbersolar-0.1.3/ubersolar/__main__.py`

 * *Files identical despite different names*

### Comparing `pyUbersolar-0.1.2/ubersolar/adv_parsers/ubersmart.py` & `pyUbersolar-0.1.3/ubersolar/adv_parsers/ubersmart.py`

 * *Files identical despite different names*

### Comparing `pyUbersolar-0.1.2/ubersolar/devices/device.py` & `pyUbersolar-0.1.3/ubersolar/devices/device.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Library to handle connection with UberSolar."""
 from __future__ import annotations
 
 import asyncio
 from collections.abc import Callable
 import logging
 import time
-from typing import Any
+from typing import Any, TypeVar, cast
 from uuid import UUID
 
 from bleak import BleakError
 from bleak.backends.device import BLEDevice
 from bleak.backends.service import BleakGATTCharacteristic, BleakGATTServiceCollection
 from bleak.exc import BleakDBusError
 from bleak_retry_connector import (
@@ -58,14 +58,29 @@
 
 
 READ_CHAR_UUID = _uuid(comms_type="tx")
 WRITE_CHAR_UUID = _uuid(comms_type="rx")
 SERVICE_CHAR_UUID = _uuid()
 FW_CHAR_UUID = _uuid(comms_type="FWVersion")
 
+WrapFuncType = TypeVar("WrapFuncType", bound=Callable[..., Any])
+
+
+def update_after_operation(func: WrapFuncType) -> WrapFuncType:
+    """Define a wrapper to update after an operation."""
+
+    async def _async_update_after_operation_wrap(
+        self: UberSolarBaseDevice, *args: Any, **kwargs: Any
+    ) -> None:
+        ret = await func(self, *args, **kwargs)
+        await self.update()
+        return ret
+
+    return cast(WrapFuncType, _async_update_after_operation_wrap)
+
 
 class UberSolarBaseDevice:
     """Base Representation of a UberSolar Device."""
 
     def __init__(
         self,
         device: BLEDevice,
@@ -84,67 +99,63 @@
         self._disconnect_timer: asyncio.TimerHandle | None = None
         self._expected_disconnect = False
         self.loop = asyncio.get_event_loop()
         self._callbacks: list[Callable[[], None]] = []
         self._notify_future: asyncio.Future[bytearray] | None = None
         self.status_data: dict[str, Any] = {device.address: {}}
         self._last_full_update: float = -POLL_INTERVAL
+        self._timed_disconnect_task: asyncio.Task[None] | None = None
 
     async def _send_command(
         self, key: str = "", retry: int | None = None
     ) -> bytes | None:
         """Send command to device and read response."""
         if retry is None:
             retry = self._retry_count
 
         command = bytearray.fromhex(key)
         _LOGGER.debug("%s: Scheduling command %s", self.name, key)
         max_attempts = retry + 1
         if self._operation_lock.locked():
             _LOGGER.debug(
-                "%s: Operation already in progress, waiting for it to complete; RSSI: %s",
+                "%s: Operation already in progress, waiting for it to complete",
                 self.name,
-                self.rssi,
             )
         async with self._operation_lock:
             for attempt in range(max_attempts):
                 try:
                     return await self._send_command_locked(command)
                 except BleakNotFoundError:
                     _LOGGER.error(
-                        "%s: device not found, no longer in range, or poor RSSI: %s",
+                        "%s: device not found, no longer in range, or poor RSSI",
                         self.name,
-                        self.rssi,
                         exc_info=True,
                     )
                     raise
                 except CharacteristicMissingError as ex:
                     if attempt == retry:
                         _LOGGER.error(
-                            "%s: characteristic missing: %s; Stopping trying; RSSI: %s",
+                            "%s: characteristic missing: %s; Stopping trying",
                             self.name,
                             ex,
-                            self.rssi,
                             exc_info=True,
                         )
                         raise
 
                     _LOGGER.debug(
-                        "%s: characteristic missing: %s; RSSI: %s",
+                        "%s: characteristic missing: %s",
                         self.name,
                         ex,
-                        self.rssi,
                         exc_info=True,
                     )
                 except BLEAK_RETRY_EXCEPTIONS:
                     if attempt == retry:
                         _LOGGER.error(
-                            "%s: communication failed; Stopping trying; RSSI: %s",
+                            "%s: communication failed; Stopping trying",
                             self.name,
-                            self.rssi,
                             exc_info=True,
                         )
                         raise
 
                     _LOGGER.debug(
                         "%s: communication failed with:", self.name, exc_info=True
                     )
@@ -152,54 +163,47 @@
         raise RuntimeError("Unreachable")
 
     @property
     def name(self) -> str:
         """Return device name."""
         return f"{self._device.name} ({self._device.address})"
 
-    @property
-    def rssi(self) -> int:
-        """Return RSSI of device."""
-        return self._device.rssi
-
     async def _ensure_connected(self) -> None:
         """Ensure connection to device is established."""
         if self._connect_lock.locked():
             _LOGGER.debug(
-                "%s: Connection already in progress, waiting for it to complete; RSSI: %s",
+                "%s: Connection already in progress, waiting for it to complete",
                 self.name,
-                self.rssi,
             )
         if self._client and self._client.is_connected:
             self._reset_disconnect_timer()
             return
         async with self._connect_lock:
             # Check again while holding the lock
             if self._client and self._client.is_connected:
                 self._reset_disconnect_timer()
                 return
-            _LOGGER.debug("%s: Connecting; RSSI: %s", self.name, self.rssi)
+            _LOGGER.debug("%s: Connecting", self.name)
             client: BleakClientWithServiceCache = await establish_connection(
                 BleakClientWithServiceCache,
                 self._device,
                 self.name,
                 self._disconnected,
                 use_services_cache=True,
                 ble_device_callback=lambda: self._device,
             )
-            _LOGGER.debug("%s: Connected; RSSI: %s", self.name, self.rssi)
+            _LOGGER.debug("%s: Connected", self.name)
 
             try:
                 self._resolve_characteristics(client.services)
             except CharacteristicMissingError as ex:
                 _LOGGER.debug(
-                    "%s: characteristic missing, clearing cache: %s; RSSI: %s",
+                    "%s: characteristic missing, clearing cache: %s",
                     self.name,
                     ex,
-                    self.rssi,
                     exc_info=True,
                 )
                 await client.clear_cache()
                 await self._execute_forced_disconnect()
                 raise
 
             self._client = client
@@ -222,36 +226,34 @@
         self._disconnect_timer = self.loop.call_later(
             DISCONNECT_DELAY, self._disconnect_from_timer
         )
 
     def _disconnected(self, client: BleakClientWithServiceCache) -> None:
         """Disconnected callback."""
         if self._expected_disconnect:
-            _LOGGER.debug(
-                "%s: Disconnected from device; RSSI: %s", self.name, self.rssi
-            )
+            _LOGGER.debug("%s: Disconnected from device", self.name)
             return
         _LOGGER.warning(
-            "%s: Device unexpectedly disconnected; RSSI: %s",
+            "%s: Device unexpectedly disconnected",
             self.name,
-            self.rssi,
         )
 
     def _disconnect_from_timer(self) -> None:
         """Disconnect from device."""
         if self._operation_lock.locked() and self._client.is_connected:
             _LOGGER.debug(
-                "%s: Operation in progress, resetting disconnect timer; RSSI: %s",
+                "%s: Operation in progress, resetting disconnect timer",
                 self.name,
-                self.rssi,
             )
             self._reset_disconnect_timer()
             return
         self._cancel_disconnect_timer()
-        asyncio.create_task(self._execute_timed_disconnect())
+        self._timed_disconnect_task = asyncio.create_task(
+            self._execute_timed_disconnect()
+        )
 
     def _cancel_disconnect_timer(self) -> None:
         """Cancel disconnect timer."""
         if self._disconnect_timer:
             self._disconnect_timer.cancel()
             self._disconnect_timer = None
 
@@ -294,41 +296,39 @@
         if command != b"":
             try:
                 return await self._execute_command_locked(command)
             except BleakDBusError as ex:
                 # Disconnect so we can reset state and try again
                 await asyncio.sleep(0.25)
                 _LOGGER.debug(
-                    "%s: RSSI: %s; Backing off %ss; Disconnecting due to error: %s",
+                    "%s: Backing off %ss; Disconnecting due to error: %s",
                     self.name,
-                    self.rssi,
                     0.25,
                     ex,
                 )
                 await self._execute_forced_disconnect()
                 raise
             except BleakError as ex:
                 # Disconnect so we can reset state and try again
                 _LOGGER.debug(
-                    "%s: RSSI: %s; Disconnecting due to error: %s",
+                    "%s: Disconnecting due to error: %s",
                     self.name,
-                    self.rssi,
                     ex,
                 )
                 await self._execute_forced_disconnect()
                 raise
 
     def _notification_handler(self, _sender: int, data: bytearray) -> None:
         """Handle notification responses."""
         _LOGGER.debug("%s: Received notification: %s", self.name, data)
         self.status_data[self._device.address].update(process_ubersmart(data))
 
     async def _start_notify(self) -> None:
         """Start notification."""
-        _LOGGER.debug("%s: Subscribe to notifications; RSSI: %s", self.name, self.rssi)
+        _LOGGER.debug("%s: Subscribe to notifications", self.name)
 
         await self._client.start_notify(self._read_char, self._notification_handler)
         await asyncio.sleep(3)
 
     async def _execute_command_locked(self, command: bytes) -> None:
         """Execute command and read response."""
         assert self._client is not None
@@ -391,10 +391,10 @@
     def _check_command_result(
         self, result: bytes | None, index: int, values: set[int]
     ) -> bool:
         """Check command result."""
         if not result or len(result) - 1 < index:
             result_hex = result.hex() if result else "None"
             raise UberSmartOperationError(
-                f"{self.name}: Sending command failed (result={result_hex} index={index} expected={values} rssi={self.rssi})"
+                f"{self.name}: Sending command failed (result={result_hex} index={index} expected={values})"
             )
         return result[index] in values
```

### Comparing `pyUbersolar-0.1.2/ubersolar/devices/ubersmart.py` & `pyUbersolar-0.1.3/ubersolar/devices/ubersmart.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,203 +2,214 @@
 from __future__ import annotations
 
 import logging
 import struct
 import time
 from typing import Any
 
-from .device import UberSolarBaseDevice
+from .device import UberSolarBaseDevice, update_after_operation
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class UberSmart(UberSolarBaseDevice):
     """Representation of a UberSmart Device."""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         """UberSolar UberSmart constructor."""
 
         super().__init__(*args, **kwargs)
 
+    @update_after_operation
     async def toggle_switches_all(self, switches: str) -> None:
         """Set all switches from hex string."""
 
         # 1st byte is message id, use 06 to toggle switches.
         # need to send  all switches.
         # elementToggle, pumpToggle, holidayModeToggle, solenoidMode = 0 - off, 1 - on, 2 - auto
         # example 0600000002
-        if not len(switches) == 8:
+        if len(switches) != 8:
             _LOGGER.error("Switch length has to be 8")
 
         await self._send_command(key=f"06{switches}")
         _LOGGER.info("%s: Toggle switches", self.name)
 
     async def enable_wifi_ap(self) -> None:
         """Enable Wifi ap mode on device."""
         # intended for firmware update but who knows.
         await self._send_command(key="14")
         _LOGGER.info("%s: Enable Wifi AP on device", self.name)
 
+    @update_after_operation
     async def set_current_time(self) -> None:
         """Set current datetime on device."""
 
         current_time = int(time.time())
         ct_to_bytearray = bytearray(struct.pack("<Qxxxx", current_time))
         ct_to_bytearray[9] = 2  # add utc offset on byte 9
 
         await self._send_command(key=f"09{ct_to_bytearray.hex()}")
         _LOGGER.info("%s: Send current time to device", self.name)
 
+    @update_after_operation
     async def turn_on_element(self) -> None:
         """Turn element switch on."""
 
         if not self.status_data:
             await self.update()
 
         current_switches = self.status_data[self._device.address]["AllSwitches"]
 
-        if not len(current_switches) == 5:
+        if len(current_switches) != 5:
             _LOGGER.error("Switch length has to be 5 bytes")
 
         current_switches[0] = 6
         current_switches[1] = 1
-        current_switches[2] = 0 # Pump can't be on as well.
+        current_switches[2] = 0  # Pump can't be on as well.
 
         await self._send_command(key=current_switches.hex())
         _LOGGER.info("%s: Turn Element On", self.name)
 
+    @update_after_operation
     async def turn_off_element(self) -> None:
         """Turn element switch off."""
 
         if not self.status_data:
             await self.update()
 
         current_switches = self.status_data[self._device.address]["AllSwitches"]
 
-        if not len(current_switches) == 5:
+        if len(current_switches) != 5:
             _LOGGER.error("Switch length has to be 5 bytes")
 
         current_switches[0] = 6
         current_switches[1] = 0
 
         await self._send_command(key=current_switches.hex())
         _LOGGER.info("%s: Turn Element Off", self.name)
 
+    @update_after_operation
     async def turn_on_pump(self) -> None:
         """Turn pump switch on."""
 
         if not self.status_data:
             await self.update()
 
         current_switches = self.status_data[self._device.address]["AllSwitches"]
 
-        if not len(current_switches) == 5:
+        if len(current_switches) != 5:
             _LOGGER.error("Switch length has to be 5 bytes")
 
         current_switches[0] = 6
-        current_switches[1] = 0 # Pump and element can't be on at same time.
+        current_switches[1] = 0  # Pump and element can't be on at same time.
         current_switches[2] = 1
 
         await self._send_command(key=current_switches.hex())
         _LOGGER.info("%s: Turn Pump On", self.name)
 
+    @update_after_operation
     async def turn_off_pump(self) -> None:
         """Turn pump switch off."""
 
         if not self.status_data:
             await self.update()
 
         current_switches = self.status_data[self._device.address]["AllSwitches"]
 
-        if not len(current_switches) == 5:
+        if len(current_switches) != 5:
             _LOGGER.error("Switch length has to be 5 bytes")
 
         current_switches[0] = 6
         current_switches[2] = 0
 
         await self._send_command(key=current_switches.hex())
         _LOGGER.info("%s: Turn Pump Off", self.name)
 
+    @update_after_operation
     async def turn_on_holiday(self) -> None:
         """Turn holiday switch on."""
 
         if not self.status_data:
             await self.update()
 
         current_switches = self.status_data[self._device.address]["AllSwitches"]
 
-        if not len(current_switches) == 5:
+        if len(current_switches) != 5:
             _LOGGER.error("Switch length has to be 5 bytes")
 
         current_switches[0] = 6
         current_switches[3] = 1
 
         await self._send_command(key=current_switches.hex())
         _LOGGER.info("%s: Turn Holiday On", self.name)
 
+    @update_after_operation
     async def turn_off_holiday(self) -> None:
         """Turn holiday switch off."""
 
         if not self.status_data:
             await self.update()
 
         current_switches = self.status_data[self._device.address]["AllSwitches"]
 
-        if not len(current_switches) == 5:
+        if len(current_switches) != 5:
             _LOGGER.error("Switch length has to be 5 bytes")
 
         current_switches[0] = 6
         current_switches[3] = 0
 
         await self._send_command(key=current_switches.hex())
         _LOGGER.info("%s: Turn Holiday Off", self.name)
 
+    @update_after_operation
     async def set_solinoid_off(self) -> None:
         """Turn Solinoid off."""
 
         if not self.status_data:
             await self.update()
 
         current_switches = self.status_data[self._device.address]["AllSwitches"]
 
-        if not len(current_switches) == 5:
+        if len(current_switches) != 5:
             _LOGGER.error("Switch length has to be 5 bytes")
 
         current_switches[0] = 6
         current_switches[4] = 0
 
         await self._send_command(key=current_switches.hex())
         _LOGGER.info("%s: Turn Solinoid Off", self.name)
 
+    @update_after_operation
     async def set_solinoid_on(self) -> None:
         """Turn Solinoid on."""
 
         if not self.status_data:
             await self.update()
 
         current_switches = self.status_data[self._device.address]["AllSwitches"]
 
-        if not len(current_switches) == 5:
+        if len(current_switches) != 5:
             _LOGGER.error("Switch length has to be 5 bytes")
 
         current_switches[0] = 6
         current_switches[4] = 1
 
         await self._send_command(key=current_switches.hex())
         _LOGGER.info("%s: Turn Solinoid On", self.name)
 
+    @update_after_operation
     async def set_solinoid_auto(self) -> None:
         """Set Solinoid to Auto."""
 
         if not self.status_data:
             await self.update()
 
         current_switches = self.status_data[self._device.address]["AllSwitches"]
 
-        if not len(current_switches) == 5:
+        if len(current_switches) != 5:
             _LOGGER.error("Switch length has to be 5 bytes")
 
         current_switches[0] = 6
         current_switches[4] = 2
 
         await self._send_command(key=current_switches.hex())
         _LOGGER.info("%s: Turn Solinoid to Auto", self.name)
```

### Comparing `pyUbersolar-0.1.2/ubersolar/discovery.py` & `pyUbersolar-0.1.3/ubersolar/discovery.py`

 * *Files identical despite different names*

