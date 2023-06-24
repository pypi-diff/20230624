# Comparing `tmp/colour_specio-0.2.8.tar.gz` & `tmp/colour_specio-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colour_specio-0.2.8.tar", max compression
+gzip compressed data, was "colour_specio-0.2.9.tar", max compression
```

## Comparing `colour_specio-0.2.8.tar` & `colour_specio-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     1195 2022-07-20 20:59:12.149887 colour_specio-0.2.8/LICENSE.md
--rw-r--r--   0        0        0      334 2022-10-20 16:37:16.649139 colour_specio-0.2.8/README.md
--rw-r--r--   0        0        0      809 2022-11-30 02:21:00.557860 colour_specio-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     7565 2022-11-01 18:23:28.915569 colour_specio-0.2.8/specio/ColorimetryResearch/CRSpectrometer.py
--rw-r--r--   0        0        0     3119 2022-10-14 16:52:42.719296 colour_specio-0.2.8/specio/ColorimetryResearch/CR_Definitions.py
--rw-r--r--   0        0        0      600 2022-11-01 18:23:28.915763 colour_specio-0.2.8/specio/ColorimetryResearch/__init__.py
--rw-r--r--   0        0        0      978 2022-11-28 21:53:14.239029 colour_specio-0.2.8/specio/__init__.py
--rw-r--r--   0        0        0     4643 2022-12-19 14:33:02.002728 colour_specio-0.2.8/specio/common.py
--rw-r--r--   0        0        0     3975 2022-11-23 23:30:12.821403 colour_specio-0.2.8/specio/fileio.py
--rw-r--r--   0        0        0        0 2022-11-01 18:23:28.915820 colour_specio-0.2.8/specio/protobuf/__init__.py
--rw-r--r--   0        0        0     3346 2022-11-29 22:32:03.380144 colour_specio-0.2.8/specio/protobuf/measurements_pb2.py
--rw-r--r--   0        0        0     5173 2022-11-29 22:32:03.380942 colour_specio-0.2.8/specio/protobuf/measurements_pb2.pyi
--rw-r--r--   0        0        0     1689 2022-11-03 14:54:42.775859 colour_specio-0.2.8/specio/spectrometer.py
--rw-r--r--   0        0        0     1155 1970-01-01 00:00:00.000000 colour_specio-0.2.8/setup.py
--rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 colour_specio-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1195 2023-06-22 23:22:09.646445 colour_specio-0.2.9/LICENSE.md
+-rw-r--r--   0        0        0      334 2023-06-22 23:22:09.647582 colour_specio-0.2.9/README.md
+-rw-r--r--   0        0        0      809 2023-06-24 00:26:13.743335 colour_specio-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     7557 2023-06-23 22:04:49.112303 colour_specio-0.2.9/specio/ColorimetryResearch/CRSpectrometer.py
+-rw-r--r--   0        0        0     3126 2023-06-22 23:22:09.647777 colour_specio-0.2.9/specio/ColorimetryResearch/CR_Definitions.py
+-rw-r--r--   0        0        0      600 2023-06-22 23:22:09.647724 colour_specio-0.2.9/specio/ColorimetryResearch/__init__.py
+-rw-r--r--   0        0        0     1010 2023-06-24 00:26:29.122724 colour_specio-0.2.9/specio/__init__.py
+-rw-r--r--   0        0        0     4375 2023-06-24 00:21:54.575962 colour_specio-0.2.9/specio/fileio.py
+-rw-r--r--   0        0        0     4662 2023-06-23 22:03:42.761928 colour_specio-0.2.9/specio/measurement.py
+-rw-r--r--   0        0        0       31 2023-06-23 19:11:14.267213 colour_specio-0.2.9/specio/protobuf/__init__.py
+-rw-r--r--   0        0        0     1221 2023-06-23 21:58:34.437592 colour_specio-0.2.9/specio/protobuf/measurements.proto
+-rw-r--r--   0        0        0     3486 2023-06-23 22:00:30.947561 colour_specio-0.2.9/specio/protobuf/measurements_pb2.py
+-rw-r--r--   0        0        0     5077 2023-06-23 22:00:30.948033 colour_specio-0.2.9/specio/protobuf/measurements_pb2.pyi
+-rw-r--r--   0        0        0     1694 2023-06-23 21:09:48.066444 colour_specio-0.2.9/specio/spectrometer.py
+-rw-r--r--   0        0        0       23 2023-06-23 21:09:48.064291 colour_specio-0.2.9/specio/utility/__init__.py
+-rw-r--r--   0        0        0     3610 2023-06-23 23:28:15.719627 colour_specio-0.2.9/specio/utility/spectral.py
+-rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 colour_specio-0.2.9/PKG-INFO
```

### Comparing `colour_specio-0.2.8/LICENSE.md` & `colour_specio-0.2.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `colour_specio-0.2.8/pyproject.toml` & `colour_specio-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "colour-specio"
 packages = [
     { include = "specio" },
 ]
-version = "0.2.8"
+version = "0.2.9"
 description = "Instrument control for spectrometers"
 authors = ["Tucker <tucker@tuckerd.info>"]
 keywords = ["colour-science", "spectrometer", "instrument control"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tjdcs/specio"
 repository = "https://github.com/tjdcs/specio"
```

### Comparing `colour_specio-0.2.8/specio/ColorimetryResearch/CRSpectrometer.py` & `colour_specio-0.2.9/specio/ColorimetryResearch/CRSpectrometer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import platform
 import re
 import time
 
 import serial.tools.list_ports
 from colour import SpectralDistribution, SpectralShape
 
-from specio.common import RawMeasurement
+from specio.measurement import RawMeasurement
 from specio.spectrometer import SpecRadiometer
 
 from specio.ColorimetryResearch.CR_Definitions import (
     CommandError,
     CommandResponse,
     InstrumentType,
     MeasurementSpeed,
@@ -39,31 +39,30 @@
     In particular this implementation was developed and tested with the CR300,
     but it should work for CR250 or other spectrometers from CR.
     """
 
     def __initialize_connection__(self, device: str | None = None) -> str:
         if device is None:
             if platform.system() == "Darwin":
-                portlist = list(serial.tools.list_ports.grep("usbmodem"))
+                port_list = list(serial.tools.list_ports.grep("usbmodem"))
             elif platform.system() == "Windows":
-                portlist = list(serial.tools.list_ports.grep("Colorimetry"))
+                port_list = list(serial.tools.list_ports.grep("Colorimetry"))
             elif platform.system() == "Unix":
                 raise NotImplementedError("CR discovery is not implemented for Unix")
             elif platform.system() == "Linux":
-                portlist = list(serial.tools.list_ports.grep("ACM"))
-
-            if len(portlist) == 0:
+                port_list = list(serial.tools.list_ports.grep("ACM"))
+            else:
                 raise OSError("Could not find any candidates for ColorimetryResearch")
 
-            if len(portlist) > 1:
+            if len(port_list) > 1:
                 raise NotImplementedError(
                     "Too many port candidates found, only a single port may be auto discovered."
                 )
 
-            device = portlist[0].device
+            device = port_list[0].device
 
         self.__port = serial.Serial(device, timeout=DEFAULT_TIMEOUT, baudrate=115200)
 
     def __init__(
         self,
         device: str | None = None,
         speed: MeasurementSpeed = MeasurementSpeed.NORMAL,
```

### Comparing `colour_specio-0.2.8/specio/ColorimetryResearch/CR_Definitions.py` & `colour_specio-0.2.9/specio/ColorimetryResearch/CR_Definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any
 
 from aenum import Enum, MultiValueEnum
-from attr import dataclass
+from dataclasses import dataclass
 
 __author__ = "Tucker Downs"
 __copyright__ = "Copyright 2022 Specio Developers"
 __license__ = "MIT License - https://github.com/tjdcs/specio/blob/main/LICENSE.md"
 __maintainer__ = "Tucker Downs"
 __email__ = "tucker@tuckerd.info"
 __status__ = "Development"
```

### Comparing `colour_specio-0.2.8/specio/ColorimetryResearch/__init__.py` & `colour_specio-0.2.9/specio/ColorimetryResearch/__init__.py`

 * *Files identical despite different names*

### Comparing `colour_specio-0.2.8/specio/__init__.py` & `colour_specio-0.2.9/specio/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """
 Specio
 ======
 Provides support for interacting with various hardware spectrometers.
 """
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
-from .common import Measurement, RawMeasurement
+from .measurement import Measurement, RawMeasurement
 from .spectrometer import SpecRadiometer
 
 __all__ = [
     "Measurement",
     "RawMeasurement",
     "SpecRadiometer",
 ]
 
-
 __author__ = "Tucker Downs"
 __copyright__ = "Copyright 2022 Specio Developers"
 __license__ = "MIT License - https://github.com/tjdcs/specio/blob/main/LICENSE.md"
 __maintainer__ = "Tucker Downs"
 __email__ = "tucker@tuckerd.info"
 __status__ = "Development"
 
 
-def config__specio_logger() -> None:
+def _config__specio_logger() -> None:
     """
     Configure the default specio logger "specio"
     """
     import logging
 
     log = logging.getLogger("specio")
 
@@ -35,7 +34,10 @@
     stream_handler.formatter = logging.Formatter(
         fmt="[%(asctime)s.%(msecs)d] %(levelname)s - %(name)s %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
     log.addHandler(stream_handler)
     log.setLevel("DEBUG")
+
+
+_config__specio_logger()
```

### Comparing `colour_specio-0.2.8/specio/common.py` & `colour_specio-0.2.9/specio/measurement.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import textwrap
 from dataclasses import dataclass
 from datetime import datetime
 
-from typing import Any, Tuple
+from typing import Any, Self, Tuple, cast
 import colour
 
 import numpy as np
 from colour import (
     SpectralDistribution,
     SpectralShape,
     XYZ_to_xy,
     dominant_wavelength,
     sd_to_XYZ,
     uv_to_CCT,
     xy_to_UCS_uv,
 )
 from numpy import byte, ndarray, power
-from specio.protobuf import measurements_pb2
+from specio import protobuf
+from specio.utility import buffer_to_sd, sd_to_buffer
 
 __author__ = "Tucker Downs"
 __copyright__ = "Copyright 2022 Specio Developers"
 __license__ = "MIT License - https://github.com/tjdcs/specio/blob/main/LICENSE.md"
 __maintainer__ = "Tucker Downs"
 __email__ = "tucker@tuckerd.info"
 __status__ = "Development"
@@ -30,128 +31,126 @@
 class RawMeasurement:
     spd: SpectralDistribution
     exposure: float
     spectrometer_id: str
     anc_data: None | Any = None
 
 
-@dataclass
 class Measurement:
-    def _from_protobuf(self, data: bytes | measurements_pb2.Measurement):
-        m: measurements_pb2.Measurement
+    def _from_buffer(self, data: bytes | protobuf.Measurement):
+        m: protobuf.Measurement
         if type(data) == bytes:
-            m = measurements_pb2.Measurement()
+            m = protobuf.Measurement()
             m.ParseFromString(data)
         else:
-            m = data
+            m = cast(protobuf.Measurement, data)
 
-        self.spd = SpectralDistribution(
-            data=m.spd.values,
-            domain=SpectralShape(
-                start=m.spd.shape.start, end=m.spd.shape.end, interval=m.spd.shape.step
-            ),
-            name=m.spd.name,
-        )
+        self.spd = buffer_to_sd(m.spd)
         self.exposure = m.exposure
         self.spectrometer_id = m.spectrometer_id
         self.XYZ = np.array([m.XYZ.X, m.XYZ.Y, m.XYZ.Z])
         self.xy = np.array([m.xy.x, m.xy.y])
         self.cct = m.cct.cct
         self.duv = m.cct.duv
         self.dominant_wl = m.dominant_wl
         self.power = m.power
         self.time = datetime.fromisoformat(m.time.timestr)
-        self.anc_data = None
 
-    def to_protobuf(self) -> Tuple[bytes, measurements_pb2.Measurement]:
-        m = measurements_pb2.Measurement()
+    def to_buffer(self, return_pb: bool = False) -> bytes | protobuf.Measurement:
+        m = protobuf.Measurement()
         m.exposure = self.exposure
         m.dominant_wl = self.dominant_wl
         m.power = self.power
         m.spectrometer_id = self.spectrometer_id
 
         m.time.timestr = self.time.isoformat()
 
-        m.spd.values[:] = self.spd.values.tolist()
-        m.spd.shape.start = self.spd.shape.start
-        m.spd.shape.end = self.spd.shape.end
-        m.spd.shape.step = self.spd.shape.interval
-        m.spd.name = self.spd.name
+        m.spd.CopyFrom(
+            cast(protobuf.SpectralDistribution, sd_to_buffer(self.spd, return_pb=True))  # type: ignore
+        )
 
         m.XYZ.X = self.XYZ[0]
         m.XYZ.Y = self.XYZ[1]
         m.XYZ.Z = self.XYZ[2]
 
         m.xy.x = self.xy[0]
         m.xy.y = self.xy[1]
 
         m.cct.cct = self.cct
         m.cct.duv = self.duv
 
-        if self.anc_data is not None:
-            pass
-
-        return (m.SerializeToString(), m)
+        return m if return_pb else m.SerializeToString()
 
     def __init__(
         self,
-        raw_meas: (None | RawMeasurement | bytes | measurements_pb2.Measurement) = None,
+        raw_meas: (None | RawMeasurement | bytes | protobuf.Measurement) = None,
     ):
-        if type(raw_meas) is bytes or type(raw_meas) == measurements_pb2.Measurement:
-            self._from_protobuf(raw_meas)
+        if type(raw_meas) is bytes or type(raw_meas) == protobuf.Measurement:
+            self._from_buffer(raw_meas)
             return
 
         if raw_meas is None:
             self.spd = colour.sd_multi_leds(
                 np.random.randint(400, 700, size=3), np.random.randint(40, 150, size=3)
             )
             self.spd.values / 1000
             self.exposure = 1
             self.spectrometer_id = "Virtual Spectrometer"
             self.anc_data = None
         else:
+            raw_meas = cast(RawMeasurement, raw_meas)
             self.spd = raw_meas.spd
             self.exposure = raw_meas.exposure
             self.spectrometer_id = raw_meas.spectrometer_id
             self.anc_data = raw_meas.anc_data
 
         self.XYZ = sd_to_XYZ(self.spd, k=683)
         self.xy = XYZ_to_xy(self.XYZ)
         _cct = uv_to_CCT(xy_to_UCS_uv(self.xy))
-        self.cct = _cct[0]
-        self.duv = _cct[1]
-        self.dominant_wl = dominant_wavelength(self.xy, [1 / 3, 1 / 3])[0]
+        self.cct: float = _cct[0]
+        self.duv: float = _cct[1]
+        self.dominant_wl = float(dominant_wavelength(self.xy, [1 / 3, 1 / 3])[0])
         self.power = self.spd.values.sum() * 1000
         self.time = datetime.now()
 
-    spd: SpectralDistribution
-    exposure: float
-    spectrometer_id: str
-    XYZ: ndarray
-    xy: ndarray
-    cct: ndarray
-    duv: ndarray
-    dominant_wl: float
-    power: float
-    anc_data: None | Any
-    time: datetime
-
     def __str__(self) -> str:
         return textwrap.dedent(
             f"""
             Spectral Measurement - {self.spectrometer_id}:
                 time: {self.time}
                 XYZ: {np.array2string(self.XYZ, formatter={'float_kind':lambda x: "%.2f" % x})}
                 xy: {np.array2string(self.xy, formatter={'float_kind':lambda x: "%.4f" % x})}
                 CCT: {self.cct:.0f} ± {self.duv:.5f}
                 Dominant WL: {self.dominant_wl:.1f}
                 Exposure: {self.exposure:.3f}
             """
         )
 
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    def __eq__(self, other: Self) -> bool:
+        keys = [
+            "spd",
+            "exposure",
+            "spectrometer_id",
+            "XYZ",
+            "xy",
+            "dominant_wl",
+            "power",
+            "time",
+            "cct",
+            "duv",
+        ]
+        data = [getattr(self, k) == getattr(other, k) for k in keys]
+        for d in data:
+            if not np.all(d):
+                return False
+        return True
+
 
 if __name__ == "__main__":
     m = Measurement()
-    str = m.to_protobuf()[0]
-    print(str)
+    str = m.to_buffer()
     m2 = Measurement(str)
+    print(m2 == m)
     pass
```

### Comparing `colour_specio-0.2.8/specio/fileio.py` & `colour_specio-0.2.9/specio/fileio.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from dataclasses import dataclass, field
 import re
+from textwrap import dedent
 from typing import List
+from click import File
 
 import numpy as np
 from numpy import ndarray
-from specio.common import Measurement
+from specio.measurement import Measurement
 
 from specio.protobuf import measurements_pb2
 
 __author__ = "Tucker Downs"
 __copyright__ = "Copyright 2022 Specio Developers"
 __license__ = "MIT License - https://github.com/tjdcs/specio/blob/main/LICENSE.md"
 __maintainer__ = "Tucker Downs"
@@ -30,34 +32,37 @@
 class MeasurementList:
     measurements: List[Measurement] = field(default_factory=list)
     metadata: MeasurementList_Notes = field(default_factory=MeasurementList_Notes)
     test_colors: ndarray | None = None
     order: List[int] | None = None
 
     def __repr__(self) -> str:
-        return "None"
+        return dedent(
+            f"""MeasurementList
+                {self.metadata.notes}"""
+        )
 
     pass
 
 
 def save_measurements(
     file: str,
     measurements: Measurement | List[Measurement],
     notes: MeasurementList_Notes = MeasurementList_Notes(),
     order: None | List[int] = None,
     testColors: None | ndarray | List[List[float]] = None,
 ):
     if type(measurements) == Measurement:
         measurements = [measurements]
 
-    pbuf = measurements_pb2.Measurement_List()
+    pbuf = measurements_pb2.MeasurementList()
 
     m: Measurement
     for m in measurements:
-        m_pbuf = m.to_protobuf()[1]
+        m_pbuf = m.to_buffer(return_pb=True)
         pbuf.measurements.append(m_pbuf)
 
     if notes.notes:
         pbuf.notes = notes.notes
 
     if notes.author:
         pbuf.author = notes.author
@@ -72,50 +77,57 @@
         pbuf.order[:] = order
 
     if testColors is not None:
         if type(testColors) == list:
             testColors = np.array(testColors)
         if np.ptp(testColors) > 1 and np.all(np.modf(testColors)[0] < 1e-8):
             for color in testColors:
-                tc_buf = measurements_pb2.Measurement_List.TestColor()
+                tc_buf = measurements_pb2.MeasurementList.TestColor()
                 tc_buf.c[:] = [int(value) for value in color.tolist()]
-                pbuf.colors.append(tc_buf)
+                pbuf.test_colors.append(tc_buf)
         else:
             for color in testColors:
                 tc_buf = measurements_pb2.Measurement_List.TestColor()
                 tc_buf.f[:] = color
-                pbuf.colors.append(tc_buf)
+                pbuf.test_colors.append(tc_buf)
 
     data_string = pbuf.SerializeToString()
 
-    with open(file=file + FILE_EXTENSION, mode="wb") as f:
+    if file[-5:] != ".csmf":
+        file += FILE_EXTENSION
+
+    with open(file=file, mode="wb") as f:
         f.write(data_string)
     pass
 
 
 def load_measurements(file: str) -> MeasurementList:
     data_string: bytes
-    file = re.sub(".csmf", "", file)
-    with open(file=file + FILE_EXTENSION, mode="rb") as f:
+    with open(file, mode="rb") as f:
         data_string = f.read()
 
-    pbuf = measurements_pb2.Measurement_List()
+    pbuf = measurements_pb2.MeasurementList()
     pbuf.ParseFromString(data_string)
 
     measurements: List[Measurement] = []
     for mbuf in pbuf.measurements:
         measurements.append(Measurement(mbuf))
 
     tcs = []
     for color in pbuf.test_colors:
         tcs.append(color.c)
     tcs = np.array(tcs)
 
     measurements: MeasurementList = MeasurementList(
-        measurements=measurements, order=pbuf.order, test_colors=tcs
+        measurements=measurements,
+        order=pbuf.order,
+        test_colors=tcs,
+        metadata=MeasurementList_Notes(
+            pbuf.notes, pbuf.author, pbuf.location, pbuf.software
+        ),
     )
 
     return measurements
 
 
 if __name__ == "__main__":
     from time import time
@@ -136,16 +148,21 @@
     for i in range(100):
         measures.append(Measurement())
 
     file = "/Users/tucker/Downloads/test"
 
     @timer_func
     def time_save():
-        save_measurements(file=file, measurements=measures)
+        save_measurements(
+            file=file,
+            measurements=measures,
+            notes=MeasurementList_Notes("Hello", "World", "Burbank"),
+        )
 
     time_save()
 
     @timer_func
     def time_read():
-        load_measurements(file=file)
+        return load_measurements(file=file)
 
-    time_read()
+    m = time_read()
+    pass
```

### Comparing `colour_specio-0.2.8/specio/protobuf/measurements_pb2.py` & `colour_specio-0.2.9/specio/protobuf/measurements_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: measurements.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12measurements.proto\x12\x0especio.protoio\":\n\x0eSpectral_Shape\x12\r\n\x05start\x18\x01 \x01(\x01\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x01\x12\x0c\n\x04step\x18\x03 \x01(\x01\"~\n\nColour_SDS\x12-\n\x05shape\x18\x01 \x01(\x0b\x32\x1e.specio.protoio.Spectral_Shape\x12\x15\n\rvalues_double\x18\x02 \x03(\x01\x12\x0e\n\x06values\x18\x04 \x03(\x02\x12\x11\n\x04name\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x07\n\x05_name\",\n\tXYZ_value\x12\t\n\x01X\x18\x01 \x01(\x01\x12\t\n\x01Y\x18\x02 \x01(\x01\x12\t\n\x01Z\x18\x03 \x01(\x01\" \n\x08xy_value\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"%\n\tcct_value\x12\x0b\n\x03\x63\x63t\x18\x01 \x01(\x01\x12\x0b\n\x03\x64uv\x18\x02 \x01(\x01\"\x1c\n\tTimestamp\x12\x0f\n\x07timestr\x18\x01 \x01(\t\"\xc8\x02\n\x0bMeasurement\x12\'\n\x03spd\x18\x01 \x01(\x0b\x32\x1a.specio.protoio.Colour_SDS\x12\x10\n\x08\x65xposure\x18\x02 \x01(\x01\x12&\n\x03XYZ\x18\x03 \x01(\x0b\x32\x19.specio.protoio.XYZ_value\x12$\n\x02xy\x18\x04 \x01(\x0b\x32\x18.specio.protoio.xy_value\x12&\n\x03\x63\x63t\x18\x05 \x01(\x0b\x32\x19.specio.protoio.cct_value\x12\x13\n\x0b\x64ominant_wl\x18\x06 \x01(\x01\x12\r\n\x05power\x18\x07 \x01(\x01\x12\x17\n\x0fspectrometer_id\x18\x08 \x01(\t\x12\'\n\x04time\x18\t \x01(\x0b\x32\x19.specio.protoio.Timestamp\x12\x15\n\x08\x61nc_data\x18\x10 \x01(\x0cH\x00\x88\x01\x01\x42\x0b\n\t_anc_data\"\x8e\x02\n\x10Measurement_List\x12\x31\n\x0cmeasurements\x18\x01 \x03(\x0b\x32\x1b.specio.protoio.Measurement\x12?\n\x0btest_colors\x18\x03 \x03(\x0b\x32*.specio.protoio.Measurement_List.TestColor\x12\r\n\x05order\x18\x02 \x03(\x05\x12\r\n\x05notes\x18\x10 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x11 \x01(\t\x12\x10\n\x08location\x18\x12 \x01(\t\x12\x10\n\x08software\x18\x13 \x01(\t\x12\x11\n\tancillary\x18\x14 \x01(\x0c\x1a!\n\tTestColor\x12\t\n\x01\x63\x18\x01 \x03(\r\x12\t\n\x01\x66\x18\x02 \x03(\x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12measurements.proto\x12\x06specio\"9\n\rSpectralShape\x12\r\n\x05start\x18\x01 \x01(\x01\x12\x0b\n\x03\x65nd\x18\x02 \x01(\x01\x12\x0c\n\x04step\x18\x03 \x01(\x01\"|\n\x14SpectralDistribution\x12$\n\x05shape\x18\x01 \x01(\x0b\x32\x15.specio.SpectralShape\x12\x0e\n\x06values\x18\x02 \x03(\x01\x12\x12\n\nvalues_old\x18\x04 \x03(\x02\x12\x11\n\x04name\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x07\n\x05_name\",\n\tXYZ_value\x12\t\n\x01X\x18\x01 \x01(\x01\x12\t\n\x01Y\x18\x02 \x01(\x01\x12\t\n\x01Z\x18\x03 \x01(\x01\" \n\x08xy_value\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"%\n\tcct_value\x12\x0b\n\x03\x63\x63t\x18\x01 \x01(\x01\x12\x0b\n\x03\x64uv\x18\x02 \x01(\x01\"\x1c\n\tTimestamp\x12\x0f\n\x07timestr\x18\x01 \x01(\t\"\x8c\x02\n\x0bMeasurement\x12)\n\x03spd\x18\x01 \x01(\x0b\x32\x1c.specio.SpectralDistribution\x12\x10\n\x08\x65xposure\x18\x02 \x01(\x01\x12\x1e\n\x03XYZ\x18\x03 \x01(\x0b\x32\x11.specio.XYZ_value\x12\x1c\n\x02xy\x18\x04 \x01(\x0b\x32\x10.specio.xy_value\x12\x1e\n\x03\x63\x63t\x18\x05 \x01(\x0b\x32\x11.specio.cct_value\x12\x13\n\x0b\x64ominant_wl\x18\x06 \x01(\x01\x12\r\n\x05power\x18\x07 \x01(\x01\x12\x17\n\x0fspectrometer_id\x18\x08 \x01(\t\x12\x1f\n\x04time\x18\t \x01(\x0b\x32\x11.specio.TimestampJ\x04\x08\x10\x10\x11\"\xfc\x01\n\x0fMeasurementList\x12)\n\x0cmeasurements\x18\x01 \x03(\x0b\x32\x13.specio.Measurement\x12\x36\n\x0btest_colors\x18\x03 \x03(\x0b\x32!.specio.MeasurementList.TestColor\x12\r\n\x05order\x18\x02 \x03(\x05\x12\r\n\x05notes\x18\x10 \x01(\t\x12\x0e\n\x06\x61uthor\x18\x11 \x01(\t\x12\x10\n\x08location\x18\x12 \x01(\t\x12\x10\n\x08software\x18\x13 \x01(\t\x12\x11\n\tancillary\x18\x14 \x01(\x0c\x1a!\n\tTestColor\x12\t\n\x01\x63\x18\x01 \x03(\r\x12\t\n\x01\x66\x18\x02 \x03(\x02\x62\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'measurements_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'measurements_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _SPECTRAL_SHAPE._serialized_start=38
-  _SPECTRAL_SHAPE._serialized_end=96
-  _COLOUR_SDS._serialized_start=98
-  _COLOUR_SDS._serialized_end=224
-  _XYZ_VALUE._serialized_start=226
-  _XYZ_VALUE._serialized_end=270
-  _XY_VALUE._serialized_start=272
-  _XY_VALUE._serialized_end=304
-  _CCT_VALUE._serialized_start=306
-  _CCT_VALUE._serialized_end=343
-  _TIMESTAMP._serialized_start=345
-  _TIMESTAMP._serialized_end=373
-  _MEASUREMENT._serialized_start=376
-  _MEASUREMENT._serialized_end=704
-  _MEASUREMENT_LIST._serialized_start=707
-  _MEASUREMENT_LIST._serialized_end=977
-  _MEASUREMENT_LIST_TESTCOLOR._serialized_start=944
-  _MEASUREMENT_LIST_TESTCOLOR._serialized_end=977
+  _globals['_SPECTRALSHAPE']._serialized_start=30
+  _globals['_SPECTRALSHAPE']._serialized_end=87
+  _globals['_SPECTRALDISTRIBUTION']._serialized_start=89
+  _globals['_SPECTRALDISTRIBUTION']._serialized_end=213
+  _globals['_XYZ_VALUE']._serialized_start=215
+  _globals['_XYZ_VALUE']._serialized_end=259
+  _globals['_XY_VALUE']._serialized_start=261
+  _globals['_XY_VALUE']._serialized_end=293
+  _globals['_CCT_VALUE']._serialized_start=295
+  _globals['_CCT_VALUE']._serialized_end=332
+  _globals['_TIMESTAMP']._serialized_start=334
+  _globals['_TIMESTAMP']._serialized_end=362
+  _globals['_MEASUREMENT']._serialized_start=365
+  _globals['_MEASUREMENT']._serialized_end=633
+  _globals['_MEASUREMENTLIST']._serialized_start=636
+  _globals['_MEASUREMENTLIST']._serialized_end=888
+  _globals['_MEASUREMENTLIST_TESTCOLOR']._serialized_start=855
+  _globals['_MEASUREMENTLIST_TESTCOLOR']._serialized_end=888
 # @@protoc_insertion_point(module_scope)
```

### Comparing `colour_specio-0.2.8/specio/protobuf/measurements_pb2.pyi` & `colour_specio-0.2.9/specio/protobuf/measurements_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,111 +1,109 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Colour_SDS(_message.Message):
-    __slots__ = ["name", "shape", "values", "values_double"]
-    NAME_FIELD_NUMBER: _ClassVar[int]
+class SpectralShape(_message.Message):
+    __slots__ = ["start", "end", "step"]
+    START_FIELD_NUMBER: _ClassVar[int]
+    END_FIELD_NUMBER: _ClassVar[int]
+    STEP_FIELD_NUMBER: _ClassVar[int]
+    start: float
+    end: float
+    step: float
+    def __init__(self, start: _Optional[float] = ..., end: _Optional[float] = ..., step: _Optional[float] = ...) -> None: ...
+
+class SpectralDistribution(_message.Message):
+    __slots__ = ["shape", "values", "values_old", "name"]
     SHAPE_FIELD_NUMBER: _ClassVar[int]
-    VALUES_DOUBLE_FIELD_NUMBER: _ClassVar[int]
     VALUES_FIELD_NUMBER: _ClassVar[int]
-    name: str
-    shape: Spectral_Shape
+    VALUES_OLD_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    shape: SpectralShape
     values: _containers.RepeatedScalarFieldContainer[float]
-    values_double: _containers.RepeatedScalarFieldContainer[float]
-    def __init__(self, shape: _Optional[_Union[Spectral_Shape, _Mapping]] = ..., values_double: _Optional[_Iterable[float]] = ..., values: _Optional[_Iterable[float]] = ..., name: _Optional[str] = ...) -> None: ...
+    values_old: _containers.RepeatedScalarFieldContainer[float]
+    name: str
+    def __init__(self, shape: _Optional[_Union[SpectralShape, _Mapping]] = ..., values: _Optional[_Iterable[float]] = ..., values_old: _Optional[_Iterable[float]] = ..., name: _Optional[str] = ...) -> None: ...
+
+class XYZ_value(_message.Message):
+    __slots__ = ["X", "Y", "Z"]
+    X_FIELD_NUMBER: _ClassVar[int]
+    Y_FIELD_NUMBER: _ClassVar[int]
+    Z_FIELD_NUMBER: _ClassVar[int]
+    X: float
+    Y: float
+    Z: float
+    def __init__(self, X: _Optional[float] = ..., Y: _Optional[float] = ..., Z: _Optional[float] = ...) -> None: ...
+
+class xy_value(_message.Message):
+    __slots__ = ["x", "y"]
+    X_FIELD_NUMBER: _ClassVar[int]
+    Y_FIELD_NUMBER: _ClassVar[int]
+    x: float
+    y: float
+    def __init__(self, x: _Optional[float] = ..., y: _Optional[float] = ...) -> None: ...
+
+class cct_value(_message.Message):
+    __slots__ = ["cct", "duv"]
+    CCT_FIELD_NUMBER: _ClassVar[int]
+    DUV_FIELD_NUMBER: _ClassVar[int]
+    cct: float
+    duv: float
+    def __init__(self, cct: _Optional[float] = ..., duv: _Optional[float] = ...) -> None: ...
+
+class Timestamp(_message.Message):
+    __slots__ = ["timestr"]
+    TIMESTR_FIELD_NUMBER: _ClassVar[int]
+    timestr: str
+    def __init__(self, timestr: _Optional[str] = ...) -> None: ...
 
 class Measurement(_message.Message):
-    __slots__ = ["XYZ", "anc_data", "cct", "dominant_wl", "exposure", "power", "spd", "spectrometer_id", "time", "xy"]
-    ANC_DATA_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["spd", "exposure", "XYZ", "xy", "cct", "dominant_wl", "power", "spectrometer_id", "time"]
+    SPD_FIELD_NUMBER: _ClassVar[int]
+    EXPOSURE_FIELD_NUMBER: _ClassVar[int]
+    XYZ_FIELD_NUMBER: _ClassVar[int]
+    XY_FIELD_NUMBER: _ClassVar[int]
     CCT_FIELD_NUMBER: _ClassVar[int]
     DOMINANT_WL_FIELD_NUMBER: _ClassVar[int]
-    EXPOSURE_FIELD_NUMBER: _ClassVar[int]
     POWER_FIELD_NUMBER: _ClassVar[int]
-    SPD_FIELD_NUMBER: _ClassVar[int]
     SPECTROMETER_ID_FIELD_NUMBER: _ClassVar[int]
     TIME_FIELD_NUMBER: _ClassVar[int]
+    spd: SpectralDistribution
+    exposure: float
     XYZ: XYZ_value
-    XYZ_FIELD_NUMBER: _ClassVar[int]
-    XY_FIELD_NUMBER: _ClassVar[int]
-    anc_data: bytes
+    xy: xy_value
     cct: cct_value
     dominant_wl: float
-    exposure: float
     power: float
-    spd: Colour_SDS
     spectrometer_id: str
     time: Timestamp
-    xy: xy_value
-    def __init__(self, spd: _Optional[_Union[Colour_SDS, _Mapping]] = ..., exposure: _Optional[float] = ..., XYZ: _Optional[_Union[XYZ_value, _Mapping]] = ..., xy: _Optional[_Union[xy_value, _Mapping]] = ..., cct: _Optional[_Union[cct_value, _Mapping]] = ..., dominant_wl: _Optional[float] = ..., power: _Optional[float] = ..., spectrometer_id: _Optional[str] = ..., time: _Optional[_Union[Timestamp, _Mapping]] = ..., anc_data: _Optional[bytes] = ...) -> None: ...
+    def __init__(self, spd: _Optional[_Union[SpectralDistribution, _Mapping]] = ..., exposure: _Optional[float] = ..., XYZ: _Optional[_Union[XYZ_value, _Mapping]] = ..., xy: _Optional[_Union[xy_value, _Mapping]] = ..., cct: _Optional[_Union[cct_value, _Mapping]] = ..., dominant_wl: _Optional[float] = ..., power: _Optional[float] = ..., spectrometer_id: _Optional[str] = ..., time: _Optional[_Union[Timestamp, _Mapping]] = ...) -> None: ...
 
-class Measurement_List(_message.Message):
-    __slots__ = ["ancillary", "author", "location", "measurements", "notes", "order", "software", "test_colors"]
+class MeasurementList(_message.Message):
+    __slots__ = ["measurements", "test_colors", "order", "notes", "author", "location", "software", "ancillary"]
     class TestColor(_message.Message):
         __slots__ = ["c", "f"]
         C_FIELD_NUMBER: _ClassVar[int]
         F_FIELD_NUMBER: _ClassVar[int]
         c: _containers.RepeatedScalarFieldContainer[int]
         f: _containers.RepeatedScalarFieldContainer[float]
         def __init__(self, c: _Optional[_Iterable[int]] = ..., f: _Optional[_Iterable[float]] = ...) -> None: ...
-    ANCILLARY_FIELD_NUMBER: _ClassVar[int]
-    AUTHOR_FIELD_NUMBER: _ClassVar[int]
-    LOCATION_FIELD_NUMBER: _ClassVar[int]
     MEASUREMENTS_FIELD_NUMBER: _ClassVar[int]
-    NOTES_FIELD_NUMBER: _ClassVar[int]
+    TEST_COLORS_FIELD_NUMBER: _ClassVar[int]
     ORDER_FIELD_NUMBER: _ClassVar[int]
+    NOTES_FIELD_NUMBER: _ClassVar[int]
+    AUTHOR_FIELD_NUMBER: _ClassVar[int]
+    LOCATION_FIELD_NUMBER: _ClassVar[int]
     SOFTWARE_FIELD_NUMBER: _ClassVar[int]
-    TEST_COLORS_FIELD_NUMBER: _ClassVar[int]
-    ancillary: bytes
-    author: str
-    location: str
+    ANCILLARY_FIELD_NUMBER: _ClassVar[int]
     measurements: _containers.RepeatedCompositeFieldContainer[Measurement]
-    notes: str
+    test_colors: _containers.RepeatedCompositeFieldContainer[MeasurementList.TestColor]
     order: _containers.RepeatedScalarFieldContainer[int]
+    notes: str
+    author: str
+    location: str
     software: str
-    test_colors: _containers.RepeatedCompositeFieldContainer[Measurement_List.TestColor]
-    def __init__(self, measurements: _Optional[_Iterable[_Union[Measurement, _Mapping]]] = ..., test_colors: _Optional[_Iterable[_Union[Measurement_List.TestColor, _Mapping]]] = ..., order: _Optional[_Iterable[int]] = ..., notes: _Optional[str] = ..., author: _Optional[str] = ..., location: _Optional[str] = ..., software: _Optional[str] = ..., ancillary: _Optional[bytes] = ...) -> None: ...
-
-class Spectral_Shape(_message.Message):
-    __slots__ = ["end", "start", "step"]
-    END_FIELD_NUMBER: _ClassVar[int]
-    START_FIELD_NUMBER: _ClassVar[int]
-    STEP_FIELD_NUMBER: _ClassVar[int]
-    end: float
-    start: float
-    step: float
-    def __init__(self, start: _Optional[float] = ..., end: _Optional[float] = ..., step: _Optional[float] = ...) -> None: ...
-
-class Timestamp(_message.Message):
-    __slots__ = ["timestr"]
-    TIMESTR_FIELD_NUMBER: _ClassVar[int]
-    timestr: str
-    def __init__(self, timestr: _Optional[str] = ...) -> None: ...
-
-class XYZ_value(_message.Message):
-    __slots__ = ["X", "Y", "Z"]
-    X: float
-    X_FIELD_NUMBER: _ClassVar[int]
-    Y: float
-    Y_FIELD_NUMBER: _ClassVar[int]
-    Z: float
-    Z_FIELD_NUMBER: _ClassVar[int]
-    def __init__(self, X: _Optional[float] = ..., Y: _Optional[float] = ..., Z: _Optional[float] = ...) -> None: ...
-
-class cct_value(_message.Message):
-    __slots__ = ["cct", "duv"]
-    CCT_FIELD_NUMBER: _ClassVar[int]
-    DUV_FIELD_NUMBER: _ClassVar[int]
-    cct: float
-    duv: float
-    def __init__(self, cct: _Optional[float] = ..., duv: _Optional[float] = ...) -> None: ...
-
-class xy_value(_message.Message):
-    __slots__ = ["x", "y"]
-    X_FIELD_NUMBER: _ClassVar[int]
-    Y_FIELD_NUMBER: _ClassVar[int]
-    x: float
-    y: float
-    def __init__(self, x: _Optional[float] = ..., y: _Optional[float] = ...) -> None: ...
+    ancillary: bytes
+    def __init__(self, measurements: _Optional[_Iterable[_Union[Measurement, _Mapping]]] = ..., test_colors: _Optional[_Iterable[_Union[MeasurementList.TestColor, _Mapping]]] = ..., order: _Optional[_Iterable[int]] = ..., notes: _Optional[str] = ..., author: _Optional[str] = ..., location: _Optional[str] = ..., software: _Optional[str] = ..., ancillary: _Optional[bytes] = ...) -> None: ...
```

### Comparing `colour_specio-0.2.8/specio/spectrometer.py` & `colour_specio-0.2.9/specio/spectrometer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 import numpy as np
 from colour import sd_multi_leds
 
-from specio.common import Measurement, RawMeasurement
+from specio.measurement import Measurement, RawMeasurement
 
 __author__ = "Tucker Downs"
 __copyright__ = "Copyright 2022 Specio Developers"
 __license__ = "MIT License - https://github.com/tjdcs/specio/blob/main/LICENSE.md"
 __maintainer__ = "Tucker Downs"
 __email__ = "tucker@tuckerd.info"
 __status__ = "Development"
```

### Comparing `colour_specio-0.2.8/PKG-INFO` & `colour_specio-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colour-specio
-Version: 0.2.8
+Version: 0.2.9
 Summary: Instrument control for spectrometers
 Home-page: https://github.com/tjdcs/specio
 License: MIT
 Keywords: colour-science,spectrometer,instrument control
 Author: Tucker
 Author-email: tucker@tuckerd.info
 Requires-Python: >=3.10,<3.12
```

