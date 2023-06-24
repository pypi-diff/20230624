# Comparing `tmp/adataset-0.1.1.tar.gz` & `tmp/adataset-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adataset-0.1.1.tar", last modified: Sat Jun 10 11:50:55 2023, max compression
+gzip compressed data, was "adataset-0.1.2.tar", last modified: Sat Jun 24 03:44:07 2023, max compression
```

## Comparing `adataset-0.1.1.tar` & `adataset-0.1.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.498804 adataset-0.1.1/
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-06-10 11:50:55.498561 adataset-0.1.1/PKG-INFO
--rw-r--r--   0 wangfanghao   (502) staff       (20)     3875 2023-05-20 04:47:09.000000 adataset-0.1.1/README.md
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.475995 adataset-0.1.1/adataset/
--rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/__init__.py
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.470794 adataset-0.1.1/adataset/calibration_meta/
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.477464 adataset-0.1.1/adataset/calibration_meta/camera_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      207 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/camera_params/camera_extrinsics.yaml
--rw-r--r--   0 wangfanghao   (502) staff       (20)      939 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/camera_params/camera_intrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.477940 adataset-0.1.1/adataset/calibration_meta/gnss_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      273 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/gnss_params/ant_imu_leverarm.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.478409 adataset-0.1.1/adataset/calibration_meta/radar_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      203 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/radar_params/radar_extrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.478943 adataset-0.1.1/adataset/calibration_meta/vehicle_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)      115 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/vehicle_params/vehicle_imu_extrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.480285 adataset-0.1.1/adataset/calibration_meta/velodyne_params/
--rw-r--r--   0 wangfanghao   (502) staff       (20)       59 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/velodyne_params/lidar_height.yaml
--rw-r--r--   0 wangfanghao   (502) staff       (20)      214 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/calibration_meta/velodyne_params/lidar_novatel_extrinsics.yaml
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.487923 adataset-0.1.1/adataset/kitti/
--rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/__init__.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)    12153 2023-06-10 11:44:42.000000 adataset-0.1.1/adataset/kitti/calibration_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1348 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/common.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     3707 2023-06-10 11:46:05.000000 adataset-0.1.1/adataset/kitti/dataset_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     5514 2023-06-10 11:44:59.000000 adataset-0.1.1/adataset/kitti/geometry.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4198 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/kitti.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1892 2023-06-10 11:45:15.000000 adataset-0.1.1/adataset/kitti/params.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1397 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/pcd_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1579 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/proj_helper.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     3861 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/kitti/sensor.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4051 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/main.py
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.493162 adataset-0.1.1/adataset/nuscenes/
--rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/nuscenes/__init__.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)    12194 2023-06-10 11:48:19.000000 adataset-0.1.1/adataset/nuscenes/calibration_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     3956 2023-06-10 11:33:09.000000 adataset-0.1.1/adataset/nuscenes/dataset_converter.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     5514 2023-06-10 10:39:20.000000 adataset-0.1.1/adataset/nuscenes/geometry.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     6886 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/nuscenes/nuscenes.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     2363 2023-06-10 11:09:08.000000 adataset-0.1.1/adataset/nuscenes/params.py
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1444 2023-05-20 04:47:09.000000 adataset-0.1.1/adataset/nuscenes/pcd_converter.py
-drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-10 11:50:55.498263 adataset-0.1.1/adataset.egg-info/
--rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/PKG-INFO
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1276 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/SOURCES.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)        1 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/dependency_links.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)       48 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/entry_points.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)       37 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/requires.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)        9 2023-06-10 11:50:55.000000 adataset-0.1.1/adataset.egg-info/top_level.txt
--rw-r--r--   0 wangfanghao   (502) staff       (20)       38 2023-06-10 11:50:55.498877 adataset-0.1.1/setup.cfg
--rw-r--r--   0 wangfanghao   (502) staff       (20)     1353 2023-06-10 09:41:03.000000 adataset-0.1.1/setup.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.466546 adataset-0.1.2/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-06-24 03:44:07.466371 adataset-0.1.2/PKG-INFO
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3875 2023-05-20 04:47:09.000000 adataset-0.1.2/README.md
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.440810 adataset-0.1.2/adataset/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/__init__.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.436638 adataset-0.1.2/adataset/calibration_meta/
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.442123 adataset-0.1.2/adataset/calibration_meta/camera_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      207 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/camera_params/camera_extrinsics.yaml
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      939 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/camera_params/camera_intrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.442797 adataset-0.1.2/adataset/calibration_meta/gnss_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      273 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/gnss_params/ant_imu_leverarm.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.443381 adataset-0.1.2/adataset/calibration_meta/radar_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      203 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/radar_params/radar_extrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.443968 adataset-0.1.2/adataset/calibration_meta/vehicle_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      115 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/vehicle_params/vehicle_imu_extrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.445358 adataset-0.1.2/adataset/calibration_meta/velodyne_params/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       59 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/velodyne_params/lidar_height.yaml
+-rw-r--r--   0 wangfanghao   (502) staff       (20)      214 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/calibration_meta/velodyne_params/lidar_novatel_extrinsics.yaml
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.453576 adataset-0.1.2/adataset/kitti/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/__init__.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)    12153 2023-06-10 11:44:42.000000 adataset-0.1.2/adataset/kitti/calibration_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1348 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/common.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3626 2023-06-24 03:19:09.000000 adataset-0.1.2/adataset/kitti/dataset_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     5514 2023-06-10 11:44:59.000000 adataset-0.1.2/adataset/kitti/geometry.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4198 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/kitti.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1892 2023-06-10 11:45:15.000000 adataset-0.1.2/adataset/kitti/params.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1397 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/pcd_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1579 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/proj_helper.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3861 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/kitti/sensor.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4051 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/main.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.458943 adataset-0.1.2/adataset/nuscenes/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        0 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/nuscenes/__init__.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)    12194 2023-06-10 11:48:19.000000 adataset-0.1.2/adataset/nuscenes/calibration_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     3880 2023-06-24 03:19:48.000000 adataset-0.1.2/adataset/nuscenes/dataset_converter.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     5514 2023-06-10 10:39:20.000000 adataset-0.1.2/adataset/nuscenes/geometry.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     6886 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/nuscenes/nuscenes.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     2363 2023-06-10 11:09:08.000000 adataset-0.1.2/adataset/nuscenes/params.py
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1444 2023-05-20 04:47:09.000000 adataset-0.1.2/adataset/nuscenes/pcd_converter.py
+drwxr-xr-x   0 wangfanghao   (502) staff       (20)        0 2023-06-24 03:44:07.466094 adataset-0.1.2/adataset.egg-info/
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     4411 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/PKG-INFO
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1276 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/SOURCES.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        1 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/dependency_links.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       48 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/entry_points.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       37 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/requires.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)        9 2023-06-24 03:44:07.000000 adataset-0.1.2/adataset.egg-info/top_level.txt
+-rw-r--r--   0 wangfanghao   (502) staff       (20)       38 2023-06-24 03:44:07.466607 adataset-0.1.2/setup.cfg
+-rw-r--r--   0 wangfanghao   (502) staff       (20)     1353 2023-06-24 03:43:46.000000 adataset-0.1.2/setup.py
```

### Comparing `adataset-0.1.1/PKG-INFO` & `adataset-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adataset
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dataset conversion to Apollo record tool
 Home-page: https://github.com/ApolloAuto/apollo/tree/master/modules/tools/adataset
 Author: apollo-team
 Author-email: apollo-support@baidu.com
 Project-URL: Bug Tracker, https://github.com/ApolloAuto/apollo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `adataset-0.1.1/README.md` & `adataset-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/calibration_meta/camera_params/camera_intrinsics.yaml` & `adataset-0.1.2/adataset/calibration_meta/camera_params/camera_intrinsics.yaml`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/kitti/calibration_converter.py` & `adataset-0.1.2/adataset/kitti/calibration_converter.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/kitti/common.py` & `adataset-0.1.2/adataset/kitti/common.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/kitti/dataset_converter.py` & `adataset-0.1.2/adataset/kitti/dataset_converter.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ###############################################################################
 '''Generate apollo record file by kitti raw sensor data.'''
 
 import logging
+import math
 
 from cyber_record.record import Record
 from record_msg.builder import (
   ImageBuilder,
   PointCloudBuilder,
   LocalizationBuilder,
   TransformBuilder)
@@ -67,24 +68,23 @@
         record.write(channel_name, pb_msg, int(t*1e9))
 
       if ego_pose:
         rotation = ego_pose.rotation
         quat = Quaternion(rotation[0], rotation[1], rotation[2], rotation[3])
         heading = quat.to_euler().yaw
 
+        # Apollo coordinate system conversion
+        world_to_imu_q = Euler(0, 0, -math.pi/2).to_quaternion()
+        quat *= world_to_imu_q
+
         pb_msg = localization_builder.build(
-          ego_pose.translation, ego_pose.rotation, heading, t)
+          ego_pose.translation, [quat.w, quat.x, quat.y, quat.z], heading, t)
         if pb_msg:
           record.write(LOCALIZATION_TOPIC, pb_msg, int(t*1e9))
 
-        # Apollo coordinate system conversion
-        r_array = kitti2apollo_imu[:3,:3]
-        roll, pitch, yaw = rotation_matrix_to_euler(r_array)
-        kitti2apollo_q = Euler(roll, pitch, yaw).to_quaternion()
-        quat = quat * kitti2apollo_q
         pb_msg = transform_builder.build('world', 'localization',
           ego_pose.translation, [quat.w, quat.x, quat.y, quat.z], t)
         if pb_msg:
           record.write(TF_TOPIC, pb_msg, int(t*1e9))
 
 
 def convert_dataset(dataset_path, record_path):
```

### Comparing `adataset-0.1.1/adataset/kitti/geometry.py` & `adataset-0.1.2/adataset/kitti/geometry.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/kitti/kitti.py` & `adataset-0.1.2/adataset/kitti/kitti.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/kitti/params.py` & `adataset-0.1.2/adataset/kitti/params.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/kitti/pcd_converter.py` & `adataset-0.1.2/adataset/kitti/pcd_converter.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/kitti/proj_helper.py` & `adataset-0.1.2/adataset/kitti/proj_helper.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/kitti/sensor.py` & `adataset-0.1.2/adataset/kitti/sensor.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/main.py` & `adataset-0.1.2/adataset/main.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/nuscenes/calibration_converter.py` & `adataset-0.1.2/adataset/nuscenes/calibration_converter.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/nuscenes/dataset_converter.py` & `adataset-0.1.2/adataset/nuscenes/dataset_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 ###############################################################################
 '''Generate apollo record file by nuscenes raw sensor data.'''
 
 import os
 import logging
+import math
 
 from cyber_record.record import Record
 from record_msg.builder import (
   ImageBuilder,
   PointCloudBuilder,
   LocalizationBuilder,
   TransformBuilder)
@@ -70,27 +71,27 @@
       if pb_msg:
         record.write(channel_name, pb_msg, t*1000)
 
       rotation = ego_pose['rotation']
       quat = Quaternion(rotation[0], rotation[1], rotation[2], rotation[3])
       heading = quat.to_euler().yaw
 
+      # Apollo coordinate system conversion
+      world_to_imu_q = Euler(0, 0, -math.pi/2).to_quaternion()
+      quat *= world_to_imu_q
       ego_pose_t = ego_pose['timestamp']
       pb_msg = localization_builder.build(
-        ego_pose['translation'], ego_pose['rotation'], heading, ego_pose_t/1e6)
+        ego_pose['translation'], [quat.w, quat.x, quat.y, quat.z], heading,
+        ego_pose_t/1e6)
       if pb_msg:
         record.write(LOCALIZATION_TOPIC, pb_msg, ego_pose_t*1000)
 
-      # Apollo coordinate system conversion
-      r_matrix = nuscenes2apollo_imu[:3,:3]
-      roll, pitch, yaw = rotation_matrix_to_euler(r_matrix)
-      nuscenes2apollo_q = Euler(roll, pitch, yaw).to_quaternion()
-      quat = quat * nuscenes2apollo_q
       pb_msg = transform_builder.build('world', 'localization',
-        ego_pose['translation'], [quat.w, quat.x, quat.y, quat.z], ego_pose_t/1e6)
+        ego_pose['translation'], [quat.w, quat.x, quat.y, quat.z],
+        ego_pose_t/1e6)
       if pb_msg:
         record.write(TF_TOPIC, pb_msg, ego_pose_t*1000)
 
 def convert_dataset(dataset_path, record_path):
   """Generate apollo record file by nuscenes dataset
 
   Args:
```

### Comparing `adataset-0.1.1/adataset/nuscenes/geometry.py` & `adataset-0.1.2/adataset/nuscenes/geometry.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/nuscenes/nuscenes.py` & `adataset-0.1.2/adataset/nuscenes/nuscenes.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/nuscenes/params.py` & `adataset-0.1.2/adataset/nuscenes/params.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset/nuscenes/pcd_converter.py` & `adataset-0.1.2/adataset/nuscenes/pcd_converter.py`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/adataset.egg-info/PKG-INFO` & `adataset-0.1.2/adataset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adataset
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dataset conversion to Apollo record tool
 Home-page: https://github.com/ApolloAuto/apollo/tree/master/modules/tools/adataset
 Author: apollo-team
 Author-email: apollo-support@baidu.com
 Project-URL: Bug Tracker, https://github.com/ApolloAuto/apollo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `adataset-0.1.1/adataset.egg-info/SOURCES.txt` & `adataset-0.1.2/adataset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adataset-0.1.1/setup.py` & `adataset-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="adataset",
-    version="0.1.1",
+    version="0.1.2",
     author="apollo-team",
     author_email="apollo-support@baidu.com",
     description="Dataset conversion to Apollo record tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ApolloAuto/apollo/tree/master/modules/tools/adataset",
     project_urls={
```

