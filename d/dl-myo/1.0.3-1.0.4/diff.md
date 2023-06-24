# Comparing `tmp/dl_myo-1.0.3.tar.gz` & `tmp/dl_myo-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_myo-1.0.3.tar", max compression
+gzip compressed data, was "dl_myo-1.0.4.tar", max compression
```

## Comparing `dl_myo-1.0.3.tar` & `dl_myo-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35123 2023-06-22 16:31:30.630862 dl_myo-1.0.3/LICENSE
--rw-r--r--   0        0        0     3837 2023-06-22 16:31:30.630862 dl_myo-1.0.3/README.md
--rw-r--r--   0        0        0      751 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/commands.py
--rw-r--r--   0        0        0      504 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/constants.py
--rw-r--r--   0        0        0    15170 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/core.py
--rw-r--r--   0        0        0     5805 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/profile.py
--rw-r--r--   0        0        0     9074 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/types.py
--rw-r--r--   0        0        0       22 2023-06-22 16:31:30.630862 dl_myo-1.0.3/myo/version.py
--rw-r--r--   0        0        0     3210 2023-06-22 16:31:50.235024 dl_myo-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 dl_myo-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35123 2023-06-24 11:42:42.130414 dl_myo-1.0.4/LICENSE
+-rw-r--r--   0        0        0     3837 2023-06-24 11:42:42.130414 dl_myo-1.0.4/README.md
+-rw-r--r--   0        0        0      751 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/commands.py
+-rw-r--r--   0        0        0      504 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/constants.py
+-rw-r--r--   0        0        0    15170 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/core.py
+-rw-r--r--   0        0        0     5805 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/profile.py
+-rw-r--r--   0        0        0     8991 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/types.py
+-rw-r--r--   0        0        0       22 2023-06-24 11:42:42.130414 dl_myo-1.0.4/myo/version.py
+-rw-r--r--   0        0        0     3210 2023-06-24 11:43:00.134503 dl_myo-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 dl_myo-1.0.4/PKG-INFO
```

### Comparing `dl_myo-1.0.3/LICENSE` & `dl_myo-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.3/README.md` & `dl_myo-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.3/myo/__init__.py` & `dl_myo-1.0.4/myo/__init__.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.3/myo/commands.py` & `dl_myo-1.0.4/myo/commands.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.3/myo/core.py` & `dl_myo-1.0.4/myo/core.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.3/myo/profile.py` & `dl_myo-1.0.4/myo/profile.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.3/myo/types.py` & `dl_myo-1.0.4/myo/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,26 +64,27 @@
         elif self.t == ClassifierEventType.SYNC_FAILED:
             return {"type": self.t.name, "sync-result": self.sync_result.name}
         return {"type": self.t.name}
 
 
 # -> myohw_classifier_event_type_t
 class ClassifierEventType(Enum):
-    ARM_SYNCED = 0x01
-    ARM_UNSYNCED = 0x02
-    POSE = 0x03
-    UNLOCKED = 0x04
-    LOCKED = 0x05
-    SYNC_FAILED = 0x06
+    ARM_SYNCED = 1
+    ARM_UNSYNCED = 2
+    POSE = 3
+    UNLOCKED = 4
+    LOCKED = 5
+    SYNC_FAILED = 6
+    UNKNOWN = 7
 
 
 # -> myohw_classifier_mode_t
 class ClassifierMode(Enum):
-    DISABLED = 0x00
-    ENABLED = 0x01
+    DISABLED = 0
+    ENABLED = 1
 
 
 # -> myohw_classifier_model_type_t
 # fmt: off
 class ClassifierModelType(Enum):
     BUILTIN = 0  # Model built into the classifier package.
     CUSTOM = 1   # Model based on personalized user data.
@@ -124,21 +125,21 @@
         return {"fv": self.fv, "mask": self.mask}
 
 
 # -> myohw_emg_mode_t
 # cf. https://github.com/dzhu/myo-raw/issues/17#issuecomment-913140042
 # fmt: off
 class EMGMode(Enum):
-    NONE = 0x00       # Do not send EMG data.
-    SEND_FILT = 0x01  # Send bandpass-filtered && rectified EMG data.
-    # noqa            #  - This is a hidden mode in myohw.h.
-    # noqa            #  - See FVData for the interpolated type
-    SEND_EMG = 0x02   # Send filtered && unrectified EMG data.
-    SEND_RAW = 0x03   # Send unfiltered and unrectified EMG data.
-    # noqa                  #  - The values are scaled between [-128,127]
+    NONE = 0       # Do not send EMG data.
+    SEND_FILT = 1  # Send bandpass-filtered && rectified EMG data.
+    # noqa         #  - This is a hidden mode in myohw.h.
+    # noqa         #  - See FVData for the interpolated type
+    SEND_EMG = 2   # Send filtered && unrectified EMG data.
+    SEND_RAW = 3   # Send unfiltered and unrectified EMG data.
+    # noqa         #  - The values are scaled between [-128,127]
 # fmt: on
 
 
 # -> myohw_fw_info_t
 class FirmwareInfo:
     def __init__(self, data):
         u = struct.unpack("<6BH12B", data)  # 20 bytes
@@ -227,19 +228,19 @@
             "gyroscope": self.gyroscope,
         }
 
 
 # -> myohw_imu_mode_t
 # fmt: off
 class IMUMode(Enum):
-    NONE = 0x00         # Do not send IMU data or events.
-    SEND_DATA = 0x01    # Send IMU data streams (accel, gyro, and orientation).
-    SEND_EVENTS = 0x02  # Send motion events detected by the IMU (e.g. taps).
-    SEND_ALL = 0x03     # Send both IMU data streams and motion events.
-    SEND_RAW = 0x04     # Send raw IMU data streams.
+    NONE = 0         # Do not send IMU data or events.
+    SEND_DATA = 1    # Send IMU data streams (accel, gyro, and orientation).
+    SEND_EVENTS = 2  # Send motion events detected by the IMU (e.g. taps).
+    SEND_ALL = 3     # Send both IMU data streams and motion events.
+    SEND_RAW = 4     # Send raw IMU data streams.
 # fmt: on
 
 
 # -> myohw_motion_event_t
 class MotionEvent:
     def __init__(self, data):
         t, _, _ = struct.unpack("<3b", data)
@@ -270,17 +271,17 @@
             return {
                 "type": self.t.name,
             }
 
 
 # -> myohw_motion_event_type_t
 class MotionEventType(Enum):
-    TAP = 0x00
-    UNKNOWN1 = 0x01
-    UNKNOWN2 = 0x02
+    TAP = 0
+    UNKNOWN1 = 1
+    UNKNOWN2 = 2
 
 
 # -> myohw_pose_t
 class Pose(Enum):
     REST = 0x0000
     FIST = 0x0001
     WAVE_IN = 0x0002
@@ -301,35 +302,35 @@
 class SleepMode(Enum):
     NORMAL = 0
     NEVER_SLEEP = 1
 
 
 # -> myohw_sync_result_t
 class SyncResult(Enum):
-    FAILED_TOO_HARD = 0x01
+    FAILED_TOO_HARD = 1
 
 
 # -> myohw_unlock_type_t
 class UnlockType(Enum):
-    LOCK = 0x00
-    TIMED = 0x01
-    HOLD = 0x02
+    LOCK = 0
+    TIMED = 1
+    HOLD = 2
 
 
 # -> myohw_user_action_type_t
 class UserActionType(Enum):
     SINGLE = 0
 
 
 # -> myohw_vibration_type_t
 class VibrationType(Enum):
-    NONE = 0x00
-    SHORT = 0x01
-    MEDIUM = 0x02
-    LONG = 0x03
+    NONE = 0
+    SHORT = 1
+    MEDIUM = 2
+    LONG = 3
 
 
 # -> myohw_x_direction_t
 class XDirection(Enum):
     TOWARD_WRIST = 0x01
     TOWARD_ELBOW = 0x02
     DIRECTION_UNKNOWN = 0xFF
```

### Comparing `dl_myo-1.0.3/pyproject.toml` & `dl_myo-1.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.poetry]
 name = "dl-myo"
-version = "1.0.3"
+version = "1.0.4"
 description = "Yet another MyoConnect alternative without dongles"
 authors = ["Iori Mizutani <iomz@sazanka.io>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "myo"}]
 
 [tool.poetry.dependencies]
```

### Comparing `dl_myo-1.0.3/PKG-INFO` & `dl_myo-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dl-myo
-Version: 1.0.3
+Version: 1.0.4
 Summary: Yet another MyoConnect alternative without dongles
 License: GPLv3
 Author: Iori Mizutani
 Author-email: iomz@sazanka.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

