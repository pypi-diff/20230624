# Comparing `tmp/pyxboxcontroller-0.7.1.tar.gz` & `tmp/pyxboxcontroller-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxboxcontroller-0.7.1.tar", last modified: Thu May  4 19:59:28 2023, max compression
+gzip compressed data, was "pyxboxcontroller-0.7.3.tar", last modified: Sat Jun 24 13:53:53 2023, max compression
```

## Comparing `pyxboxcontroller-0.7.1.tar` & `pyxboxcontroller-0.7.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 19:59:28.406313 pyxboxcontroller-0.7.1/
--rw-rw-rw-   0        0        0     1086 2022-10-20 14:56:56.000000 pyxboxcontroller-0.7.1/LICENCE
--rw-rw-rw-   0        0        0      797 2023-05-04 19:59:28.406313 pyxboxcontroller-0.7.1/PKG-INFO
--rw-rw-rw-   0        0        0     1234 2023-04-13 22:41:35.000000 pyxboxcontroller-0.7.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 19:59:28.393301 pyxboxcontroller-0.7.1/pyxboxcontroller/
--rw-rw-rw-   0        0        0     1559 2023-05-04 17:45:21.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/XInput.py
--rw-rw-rw-   0        0        0      168 2023-05-04 17:28:58.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/__init__.py
--rw-rw-rw-   0        0        0    11425 2023-05-04 19:59:09.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/controller.py
-drwxrwxrwx   0        0        0        0 2023-05-04 19:59:28.404310 pyxboxcontroller-0.7.1/pyxboxcontroller/examples/
--rw-rw-rw-   0        0        0      104 2023-04-13 22:37:04.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/examples/__init__.py
--rw-rw-rw-   0        0        0     1082 2023-04-13 22:20:17.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/examples/example_print_state.py
--rw-rw-rw-   0        0        0     4607 2023-04-13 22:20:32.000000 pyxboxcontroller-0.7.1/pyxboxcontroller/examples/example_state_gui.py
-drwxrwxrwx   0        0        0        0 2023-05-04 19:59:28.401307 pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/
--rw-rw-rw-   0        0        0      797 2023-05-04 19:59:28.000000 pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-05-04 19:59:28.000000 pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 19:59:28.000000 pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-04 19:59:28.000000 pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 19:59:28.407313 pyxboxcontroller-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1107 2023-05-04 19:59:17.000000 pyxboxcontroller-0.7.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-04 19:59:28.405311 pyxboxcontroller-0.7.1/tests/
--rw-rw-rw-   0        0        0     1517 2023-05-04 19:58:32.000000 pyxboxcontroller-0.7.1/tests/test_controller.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:53:53.158688 pyxboxcontroller-0.7.3/
+-rw-rw-rw-   0        0        0     1086 2022-10-20 14:56:56.000000 pyxboxcontroller-0.7.3/LICENCE
+-rw-rw-rw-   0        0        0      797 2023-06-24 13:53:53.157686 pyxboxcontroller-0.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1234 2023-04-13 22:41:35.000000 pyxboxcontroller-0.7.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 13:53:53.145676 pyxboxcontroller-0.7.3/pyxboxcontroller/
+-rw-rw-rw-   0        0        0     1686 2023-06-24 13:27:14.000000 pyxboxcontroller-0.7.3/pyxboxcontroller/XInput.py
+-rw-rw-rw-   0        0        0      168 2023-06-24 13:08:00.000000 pyxboxcontroller-0.7.3/pyxboxcontroller/__init__.py
+-rw-rw-rw-   0        0        0    11868 2023-06-24 13:30:13.000000 pyxboxcontroller-0.7.3/pyxboxcontroller/controller.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:53:53.155685 pyxboxcontroller-0.7.3/pyxboxcontroller/examples/
+-rw-rw-rw-   0        0        0      104 2023-04-13 22:37:04.000000 pyxboxcontroller-0.7.3/pyxboxcontroller/examples/__init__.py
+-rw-rw-rw-   0        0        0     1082 2023-04-13 22:20:17.000000 pyxboxcontroller-0.7.3/pyxboxcontroller/examples/example_print_state.py
+-rw-rw-rw-   0        0        0     4607 2023-04-13 22:20:32.000000 pyxboxcontroller-0.7.3/pyxboxcontroller/examples/example_state_gui.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:53:53.152682 pyxboxcontroller-0.7.3/pyxboxcontroller.egg-info/
+-rw-rw-rw-   0        0        0      797 2023-06-24 13:53:53.000000 pyxboxcontroller-0.7.3/pyxboxcontroller.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-06-24 13:53:53.000000 pyxboxcontroller-0.7.3/pyxboxcontroller.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:53:53.000000 pyxboxcontroller-0.7.3/pyxboxcontroller.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 13:53:53.000000 pyxboxcontroller-0.7.3/pyxboxcontroller.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:53:53.158688 pyxboxcontroller-0.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1107 2023-06-24 13:16:37.000000 pyxboxcontroller-0.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:53:53.156685 pyxboxcontroller-0.7.3/tests/
+-rw-rw-rw-   0        0        0     1657 2023-06-24 11:58:59.000000 pyxboxcontroller-0.7.3/tests/test_controller.py
```

### Comparing `pyxboxcontroller-0.7.1/LICENCE` & `pyxboxcontroller-0.7.3/LICENCE`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.7.1/PKG-INFO` & `pyxboxcontroller-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxboxcontroller
-Version: 0.7.1
+Version: 0.7.3
 Summary: Allows simple access to the current state of connected Xbox controllers on Windows.
 Home-page: https://github.com/SimpleHydrogen/pyxboxcontroller
 Author: Dan Forbes
 Author-email: danielforbes.123412@gmail.com
 License: MIT
 Keywords: xbox controller,XInput,xbox,controller,python,xbox-controller,xboxcontroller
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pyxboxcontroller-0.7.1/README.md` & `pyxboxcontroller-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.7.1/pyxboxcontroller/XInput.py` & `pyxboxcontroller-0.7.3/pyxboxcontroller/XInput.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 C_Structs and other objects for communicating with XInput DLL.
 
 - Dan Forbes - Mid October 2022
 """
 import ctypes
+from enum import IntEnum
 
 # Get link to XInput library
 XINPUT_DLL = ctypes.windll.xinput1_4
 
 
 # Define ctype structs for accessing XInput functions
 class XINPUT_GAMEPAD(ctypes.Structure):
@@ -35,21 +36,27 @@
 
 class Codes:
     """XInput Communication codes"""
     NOT_CONNECTED = 1167
     SUCCESS = 0
 
 
+class DeviceTypes(IntEnum):
+    """XInput devType"""
+    GAMEPAD = 0
+    HEADSET = 1
+
+
 def GetState(id: int, state: XINPUT_STATE) -> Codes:
     return XINPUT_DLL.XInputGetState(id, ctypes.byref(state))
 
 
 def GetBatteryInformation(
         id: int,
-        device_type: int,
+        device_type: DeviceTypes,
         battery_state: XINPUT_BATTERY_INFORMATION
         ) -> Codes:
     return XINPUT_DLL.XInputGetBatteryInformation(
         id,
         device_type,
         ctypes.byref(battery_state))
```

### Comparing `pyxboxcontroller-0.7.1/pyxboxcontroller/controller.py` & `pyxboxcontroller-0.7.3/pyxboxcontroller/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,20 +53,18 @@
         gamepad: XInput.XINPUT_GAMEPAD = state.gamepad
 
         # # NOTE FOR DEBUG
         # if buttons not in self.BUTTON_MAP.values():
         #     print(f"Unknown button or combination: {buttons}")
 
         # Get states of each button
-        self.buttons: dict[str, bool] = {
-            btn : self._get_button_state(btn, gamepad.buttons)
-            for btn in self._BUTTON_MAP}
+        self.buttons: dict[str, bool] = self._get_button_states(gamepad.buttons)
 
         # Thumbsticks
-        # TODO add deadzone checking
+        # TODO add deadzones
         # round to 4 decimal places
         # rounding ignores the error with converting signed 32-bit int to float
         # (-32768 to 32767) to (-1.0 to 1.0)
         self.l_thumb_x: float = round(gamepad.l_thumb_x / 32767., 4)
         self.l_thumb_y: float = round(gamepad.l_thumb_y / 32767., 4)
         self.r_thumb_x: float = round(gamepad.r_thumb_x / 32767., 4)
         self.r_thumb_y: float = round(gamepad.r_thumb_y / 32767., 4)
@@ -77,53 +75,62 @@
 
     @classmethod
     def default_state(cls):
         """Returns a default state of XboxControllerState"""
         class XInputSpoofState:
             """Spoof an XInput state packet"""
             packet_number: int = -1
+
             class gamepad:
                 buttons: int = 0
                 l_thumb: float = 0.
                 l_thumb_x: float = 0.
                 l_thumb_y: float = 0.
                 r_thumb: float = 0.
                 r_thumb_x: float = 0.
                 r_thumb_y: float = 0.
                 left_trigger: float = 0.
                 right_trigger: float = 0.
         return cls(XInputSpoofState())
 
     def __repr__(self) -> str:
-        return f"""
-    Packet number:{self.packet_number},
-    Buttons:{self.buttons},
-    Left thumbstick: {(self.l_thumb_x, self.l_thumb_y)},
-    Right thumbstick: {(self.r_thumb_x, self.r_thumb_y)},
-    Left trigger: {self.l_trigger}, 
-    Right trigger: {self.r_trigger}
-    """
+        return (
+            f"Packet number:{self.packet_number}\n"
+            f"Buttons:{self.buttons}\n"
+            f"Left thumbstick: {(self.l_thumb_x, self.l_thumb_y)}\n"
+            f"Right thumbstick: {(self.r_thumb_x, self.r_thumb_y)}\n"
+            f"Left trigger: {self.l_trigger}\n"
+            f"Right trigger: {self.r_trigger}")
 
     def _get_button_state(self, button: str, buttons: int) -> bool:
         """Returns True or False if the given button was pressed.
         bitwise and (&) of the bitmask and gamepad.buttons number"""
         mask: int = self._BUTTON_MAP[button]
         pressed: bool = (mask & buttons) != 0
         return pressed
 
+    def _get_button_states(self, gamepad_buttons: int) -> dict[str, bool]:
+        """Returns a dict with True or False for each button.
+        The value will be True if the button was pressed.
+        bitwise and (&) of the bitmask and gamepad.buttons number"""
+        return {
+            btn: (bitmask & gamepad_buttons) != 0
+            for btn, bitmask in self._BUTTON_MAP.items()}
+
     # Thumbstick getter
     @property
     def l_thumb(self) -> tuple[float, float]:
         """Returns the state of (X,Y) for the left thumbstick"""
         return (self.l_thumb_x, self.l_thumb_y)
     @property
     def r_thumb(self) -> tuple[float, float]:
         """Returns the state of (X,Y) for the right thumbstick"""
         return (self.r_thumb_x, self.r_thumb_y)
 
+    # Triggers
     @property
     def triggers(self) -> tuple[float, float]:
         """Returns the position of triggers (L,R)"""
         return (self.l_trigger, self.r_trigger)
 
     # Individual button getters
     @property
@@ -170,28 +177,29 @@
         return self.buttons["r3"]
 
     @classmethod
     @property
     @cache
     # Default buttons dict
     def buttons(cls) -> dict[str, bool]:
-        """dict containing current state of buttons"""
-        return {btn:False for btn in cls._BUTTON_MAP}
+        """dict representing the current state of buttons"""
+        return {btn: False for btn in cls._BUTTON_MAP}
 
 
 class BatteryLevel(IntEnum):
     """Different battery levels.\n
     EMPTY = 0, LOW = 1, MEDIUM = 2, FULL = 3"""
     EMPTY = 0
     LOW = 1
     MEDIUM = 2
     FULL = 3
 
     def __str__(self) -> str:
-        return self.name
+        return f"Battery Level: {self.name}"
+
 
 class BatteryType(IntEnum):
     """Different battery types"""
     DISCONNECTED = 0
     WIRED = 1
     ALKALINE = 2
     NIMH = 3  # nickel metal hydride
@@ -219,18 +227,17 @@
         class XInputSpoofBatteryInfo:
             """Spoof an XInput battery info packet"""
             battery_type = BatteryType.DISCONNECTED
             battery_level = BatteryLevel.EMPTY
         return cls(XInputSpoofBatteryInfo())
 
     def __repr__(self) -> str:
-        return f"""
-    Battery level: {self.level.name},
-    Battery type: {self.battery_type.name}
-    """
+        return (
+            f"Battery level: {self.level.name}\n"
+            f"Battery type: {self.battery_type.name}")
 
 
 class XboxController:
     """
     Provides access to the current state of a connected xbox controller.\n
 
     Connect to a controller with:
@@ -260,15 +267,15 @@
     """
 
     # TODO
     # Deadzones
     # Rumble
 
     # Specifies this is a controller for getting battery info
-    _battery_device_type: int = 0
+    device_type = XInput.DeviceTypes.GAMEPAD
 
     def __init__(self, controller_id: int):
         self.id = controller_id
         self._state = XInput.XINPUT_STATE()
         self._battery_info = XInput.XINPUT_BATTERY_INFORMATION()
         self._last_packet_number: int = -1
         self._last_state: XboxControllerState = XboxControllerState.default_state()
@@ -299,15 +306,15 @@
         return new_state
 
     @property
     def battery_info(self) -> XboxBatteryInfo:
         """Get the battery information of the controller"""
         response = XInput.GetBatteryInformation(
             self.id,
-            self._battery_device_type,
+            self.device_type,
             self._battery_info)
 
         # Handle response from XInput
         self.handle_response_code(response, "get battery info")
 
         # Convert the XInput struct into a sensible response
         battery_info = XboxBatteryInfo(self._battery_info)
```

### Comparing `pyxboxcontroller-0.7.1/pyxboxcontroller/examples/example_print_state.py` & `pyxboxcontroller-0.7.3/pyxboxcontroller/examples/example_print_state.py`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.7.1/pyxboxcontroller/examples/example_state_gui.py` & `pyxboxcontroller-0.7.3/pyxboxcontroller/examples/example_state_gui.py`

 * *Files identical despite different names*

### Comparing `pyxboxcontroller-0.7.1/pyxboxcontroller.egg-info/PKG-INFO` & `pyxboxcontroller-0.7.3/pyxboxcontroller.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxboxcontroller
-Version: 0.7.1
+Version: 0.7.3
 Summary: Allows simple access to the current state of connected Xbox controllers on Windows.
 Home-page: https://github.com/SimpleHydrogen/pyxboxcontroller
 Author: Dan Forbes
 Author-email: danielforbes.123412@gmail.com
 License: MIT
 Keywords: xbox controller,XInput,xbox,controller,python,xbox-controller,xboxcontroller
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `pyxboxcontroller-0.7.1/setup.py` & `pyxboxcontroller-0.7.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.7.1"
-DESCRIPTION = 'Allows simple access to the current state of connected Xbox controllers on Windows.'
+VERSION = "0.7.3"
+DESCRIPTION = "Allows simple access to the current state of connected Xbox controllers on Windows."
 
-setup(name='pyxboxcontroller',
+setup(name="pyxboxcontroller",
     version = VERSION,
     description = DESCRIPTION,
     license = "MIT",
-    author = 'Dan Forbes',
-    author_email = 'danielforbes.123412@gmail.com',
-    url = 'https://github.com/SimpleHydrogen/pyxboxcontroller',
+    author = "Dan Forbes",
+    author_email = "danielforbes.123412@gmail.com",
+    url = "https://github.com/SimpleHydrogen/pyxboxcontroller",
     packages = find_packages(),
     keywords = ["xbox controller",
                 "XInput",
                 "xbox",
                 "controller",
                 "python",
                 "xbox-controller",
```

### Comparing `pyxboxcontroller-0.7.1/tests/test_controller.py` & `pyxboxcontroller-0.7.3/tests/test_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import os, sys
+# Ensure pyxboxcontroller is discoverable on PATH
+import os
+import sys
 sys.path.append(os.path.dirname(__name__))
 
 
 def test_default_state() -> None:
     """Test creation of default controller state"""
     from pyxboxcontroller.controller import XboxControllerState
 
@@ -12,14 +14,15 @@
 
     assert isinstance(default_state, XboxControllerState)
 
     assert isinstance(XboxControllerState.buttons, dict)
 
 
 def test_XboxController() -> None:
+    """Test XboxControllerState produced by XboxController.state"""
     from pyxboxcontroller import XboxController, XboxControllerState
 
     controller = XboxController(0)
 
     state = controller.state
 
     assert isinstance(state, XboxControllerState)
@@ -43,15 +46,15 @@
     state.r3
     state.packet_number
     state.select
     state.start
 
 
 def test_XboxBatteryInfo():
-    # Connect to conttoller
+    """Test BatteryInfo functionality"""
     from pyxboxcontroller import XboxController, XboxBatteryInfo
 
     controller = XboxController(0)
 
     battery_info = controller.battery_info
 
     assert isinstance(battery_info, XboxBatteryInfo)
```

