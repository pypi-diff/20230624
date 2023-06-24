# Comparing `tmp/ovos_ww_plugin_openwakeword-0.2.0a1-py3-none-any.whl.zip` & `tmp/ovos_ww_plugin_openwakeword-0.2.1a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7825 bytes, number of entries: 8
--rw-r--r--  2.0 unx     3482 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword/__init__.py
--rw-r--r--  2.0 unx      177 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword/version.py
--rw-r--r--  2.0 unx    11349 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/LICENSE
--rw-r--r--  2.0 unx      390 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/WHEEL
--rw-r--r--  2.0 unx      101 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       28 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      804 b- defN 23-Apr-22 23:33 ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/RECORD
-8 files, 16423 bytes uncompressed, 6379 bytes compressed:  61.2%
+Zip file size: 7870 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     3579 b- defN 23-Jun-24 17:18 ovos_ww_plugin_openwakeword/__init__.py
+-rw-r--r--  2.0 unx      177 b- defN 23-Jun-24 17:18 ovos_ww_plugin_openwakeword/version.py
+-rw-r--r--  2.0 unx    11349 b- defN 23-Jun-24 17:18 ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      390 b- defN 23-Jun-24 17:18 ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 17:18 ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx      101 b- defN 23-Jun-24 17:18 ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       28 b- defN 23-Jun-24 17:18 ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      804 b- defN 23-Jun-24 17:18 ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/RECORD
+8 files, 16520 bytes uncompressed, 6424 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: ovos_ww_plugin_openwakeword/__init__.py
 Comment: 
 
 Filename: ovos_ww_plugin_openwakeword/version.py
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/LICENSE
+Filename: ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/LICENSE
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/METADATA
+Filename: ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/METADATA
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/WHEEL
+Filename: ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/WHEEL
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/entry_points.txt
+Filename: ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/top_level.txt
+Filename: ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/top_level.txt
 Comment: 
 
-Filename: ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/RECORD
+Filename: ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ovos_ww_plugin_openwakeword/__init__.py

```diff
@@ -53,15 +53,16 @@
             prediction = self.model.predict(self.audio_buffer)
 
             # Clear the buffer after each prediction
             self.audio_buffer = []
 
             # Check for score above threshold
             for mdl_name in self.model_names:
-                if prediction[mdl_name] >= self.config.get("threshold"):
+                # https://github.com/dscripka/openwakeword#threshold-scores-for-activation
+                if prediction[mdl_name] >= self.config.get("threshold", 0.5):
                     # Set flag indicating that a wakeword was detected
                     self.has_found = True
 
                     # Flush recent history of openWakeWord internal audio buffer to avoid re-activations
                     n_frames = self.model.model_inputs[mdl_name]
                     self.model.preprocessor.raw_data_buffer.extend([0.0]*n_frames*1280)
                     self.model.preprocessor.feature_buffer[-n_frames:, :] = np.zeros((n_frames, 96)).astype(np.float32)
```

## ovos_ww_plugin_openwakeword/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 0
 VERSION_MINOR = 2
-VERSION_BUILD = 0
+VERSION_BUILD = 1
 VERSION_ALPHA = 1
 # END_VERSION_BLOCK
```

## Comparing `ovos_ww_plugin_openwakeword-0.2.0a1.dist-info/LICENSE` & `ovos_ww_plugin_openwakeword-0.2.1a1.dist-info/LICENSE`

 * *Files identical despite different names*

