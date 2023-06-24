# Comparing `tmp/MDbrew-2.3.6.tar.gz` & `tmp/MDbrew-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDbrew-2.3.6.tar", last modified: Thu Jun  8 11:08:00 2023, max compression
+gzip compressed data, was "MDbrew-2.3.7.tar", last modified: Sat Jun 24 09:44:21 2023, max compression
```

## Comparing `MDbrew-2.3.6.tar` & `MDbrew-2.3.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 11:08:00.826433 MDbrew-2.3.6/
--rw-r--r--   0 minu       (501) staff       (20)       25 2023-06-08 05:19:02.000000 MDbrew-2.3.6/MANIFEST.in
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 11:08:00.822207 MDbrew-2.3.6/MDbrew/
--rw-r--r--   0 minu       (501) staff       (20)      182 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/__init__.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 11:08:00.823647 MDbrew-2.3.6/MDbrew/analysis/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/analysis/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     4477 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/analysis/msd.py
--rw-r--r--   0 minu       (501) staff       (20)     6171 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/analysis/rdf.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 11:08:00.824005 MDbrew-2.3.6/MDbrew/application/
--rw-r--r--   0 minu       (501) staff       (20)       20 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/application/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)    10136 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/application/cp2k.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 11:08:00.824624 MDbrew-2.3.6/MDbrew/main/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/main/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     5712 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/main/brewery.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 11:08:00.825685 MDbrew-2.3.6/MDbrew/main/filetype/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/main/filetype/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)      940 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/main/filetype/gro.py
--rw-r--r--   0 minu       (501) staff       (20)      904 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/main/filetype/lmps.py
--rw-r--r--   0 minu       (501) staff       (20)      848 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/main/filetype/pdb.py
--rw-r--r--   0 minu       (501) staff       (20)     4427 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/main/filetype/trr.py
--rw-r--r--   0 minu       (501) staff       (20)     2959 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/main/filetype/vasp.py
--rw-r--r--   0 minu       (501) staff       (20)     1226 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/main/filetype/xyz.py
--rw-r--r--   0 minu       (501) staff       (20)     1695 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/main/opener.py
--rw-r--r--   0 minu       (501) staff       (20)     1353 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/main/writer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 11:08:00.826312 MDbrew-2.3.6/MDbrew/tool/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/tool/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     3618 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/tool/colorfont.py
--rw-r--r--   0 minu       (501) staff       (20)     1578 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/tool/decorator.py
--rw-r--r--   0 minu       (501) staff       (20)      765 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/tool/doctor.py
--rw-r--r--   0 minu       (501) staff       (20)      695 2023-06-08 11:07:40.000000 MDbrew-2.3.6/MDbrew/tool/spacer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-08 11:08:00.823036 MDbrew-2.3.6/MDbrew.egg-info/
--rw-r--r--   0 minu       (501) staff       (20)      340 2023-06-08 11:08:00.000000 MDbrew-2.3.6/MDbrew.egg-info/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)      758 2023-06-08 11:08:00.000000 MDbrew-2.3.6/MDbrew.egg-info/SOURCES.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-06-08 11:08:00.000000 MDbrew-2.3.6/MDbrew.egg-info/dependency_links.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-06-08 11:08:00.000000 MDbrew-2.3.6/MDbrew.egg-info/not-zip-safe
--rw-r--r--   0 minu       (501) staff       (20)        7 2023-06-08 11:08:00.000000 MDbrew-2.3.6/MDbrew.egg-info/top_level.txt
--rw-r--r--   0 minu       (501) staff       (20)      340 2023-06-08 11:08:00.826496 MDbrew-2.3.6/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)       62 2023-06-08 05:19:02.000000 MDbrew-2.3.6/requirement.txt
--rw-r--r--   0 minu       (501) staff       (20)       79 2023-06-08 11:08:00.826704 MDbrew-2.3.6/setup.cfg
--rw-r--r--   0 minu       (501) staff       (20)      664 2023-06-08 11:07:52.000000 MDbrew-2.3.6/setup.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.650387 MDbrew-2.3.7/
+-rw-r--r--   0 minu       (501) staff       (20)       25 2023-06-08 05:19:02.000000 MDbrew-2.3.7/MANIFEST.in
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.646122 MDbrew-2.3.7/MDbrew/
+-rw-r--r--   0 minu       (501) staff       (20)      182 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/__init__.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.647844 MDbrew-2.3.7/MDbrew/analysis/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/analysis/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     4477 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/analysis/msd.py
+-rw-r--r--   0 minu       (501) staff       (20)     6171 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/analysis/rdf.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.648211 MDbrew-2.3.7/MDbrew/application/
+-rw-r--r--   0 minu       (501) staff       (20)       20 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/application/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)    10136 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/application/cp2k.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.648756 MDbrew-2.3.7/MDbrew/main/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     5769 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/brewery.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.649635 MDbrew-2.3.7/MDbrew/main/filetype/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)      940 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/gro.py
+-rw-r--r--   0 minu       (501) staff       (20)      933 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/lmps.py
+-rw-r--r--   0 minu       (501) staff       (20)      848 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/pdb.py
+-rw-r--r--   0 minu       (501) staff       (20)     4427 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/trr.py
+-rw-r--r--   0 minu       (501) staff       (20)     2959 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/vasp.py
+-rw-r--r--   0 minu       (501) staff       (20)     1226 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/filetype/xyz.py
+-rw-r--r--   0 minu       (501) staff       (20)     1695 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/opener.py
+-rw-r--r--   0 minu       (501) staff       (20)     1353 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/main/writer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.650260 MDbrew-2.3.7/MDbrew/tool/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/tool/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     3618 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/tool/colorfont.py
+-rw-r--r--   0 minu       (501) staff       (20)     1579 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/tool/decorator.py
+-rw-r--r--   0 minu       (501) staff       (20)      765 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/tool/doctor.py
+-rw-r--r--   0 minu       (501) staff       (20)      695 2023-06-24 09:43:53.000000 MDbrew-2.3.7/MDbrew/tool/spacer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-06-24 09:44:21.647081 MDbrew-2.3.7/MDbrew.egg-info/
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-06-24 09:44:21.000000 MDbrew-2.3.7/MDbrew.egg-info/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)      758 2023-06-24 09:44:21.000000 MDbrew-2.3.7/MDbrew.egg-info/SOURCES.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-06-24 09:44:21.000000 MDbrew-2.3.7/MDbrew.egg-info/dependency_links.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-06-08 11:08:00.000000 MDbrew-2.3.7/MDbrew.egg-info/not-zip-safe
+-rw-r--r--   0 minu       (501) staff       (20)        7 2023-06-24 09:44:21.000000 MDbrew-2.3.7/MDbrew.egg-info/top_level.txt
+-rw-r--r--   0 minu       (501) staff       (20)      340 2023-06-24 09:44:21.650483 MDbrew-2.3.7/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)       62 2023-06-08 05:19:02.000000 MDbrew-2.3.7/requirement.txt
+-rw-r--r--   0 minu       (501) staff       (20)       79 2023-06-24 09:44:21.650768 MDbrew-2.3.7/setup.cfg
+-rw-r--r--   0 minu       (501) staff       (20)      665 2023-06-24 09:44:10.000000 MDbrew-2.3.7/setup.py
```

### Comparing `MDbrew-2.3.6/MDbrew/analysis/msd.py` & `MDbrew-2.3.7/MDbrew/analysis/msd.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/analysis/rdf.py` & `MDbrew-2.3.7/MDbrew/analysis/rdf.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/application/cp2k.py` & `MDbrew-2.3.7/MDbrew/application/cp2k.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/main/brewery.py` & `MDbrew-2.3.7/MDbrew/main/brewery.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,25 +7,24 @@
 from .filetype.pdb import pdbOpener
 from .filetype.vasp import vaspOpener, POSCARWriter
 from .filetype.xyz import xyzOpener, xyzWriter
 from .filetype.trr import trrOpener
 from ..tool.colorfont import color
 from ..tool.decorator import color_print_verbose
 
-
 class Brewery(object):
-    __support_opener__: dict["str":Opener] = {
+    __support_opener__ = {
         "auto": None,
         "pdb": pdbOpener,
         "xyz": xyzOpener,
         "vasp": vaspOpener,
         "lmps": lmpsOpener,
         "trr": trrOpener,
     }
-    __support_writer__: dict["str":Writer] = {"xyz": xyzWriter, "vasp_poscar": POSCARWriter}
+    __support_writer__ = {"xyz": xyzWriter, "vasp_poscar": POSCARWriter}
     __print_option__ = {
         "brewery": f" #OPEN  {color.font_yellow}Brewery {color.reset}",
         "b_brewing": f" #BREW  {color.font_yellow}Some...  {color.reset}",
         "b_coords": f" #BREW  {color.font_yellow}Coords     {color.reset}",
         "b_atominfo": f" #BREW  {color.font_yellow}Atom Info  {color.reset}",
     }
 
@@ -103,37 +102,38 @@
 
     def _check_fmt(self, fmt: str):
         fmt_list = list(self.__support_opener__.keys())
         assert fmt in fmt_list, f"fmt should be in {fmt_list}"
         if fmt == "auto":
             file_name = self._path.split("/")[-1]
             fmt = file_name.split(".")[-1]
+            fmt = "lmps" if "lamm" in file_name else fmt
         return fmt
 
     def _check_path(self, path, **kwrgs):
         path = os.path.join(os.getcwd(), path)
         assert os.path.isfile(path=path), f"Check your path || not {path}"
         return path
 
     @color_print_verbose(name=__print_option__["b_brewing"])
-    def brew(self, cols: list[str] = None, what: str = None, dtype: str = "float32", verbose: bool = False):
+    def brew(self, cols = None, what: str = None, dtype: str = "float64", verbose: bool = False):
         data = pd.DataFrame(data=self.data, columns=self.columns)
         data = data.query(self._what) if self._what is not None else data
         data = data.query(what) if what is not None else data
         data = data.loc[:, cols] if cols is not None else data
         return data.to_numpy(dtype=dtype)
 
     def reset(self):
         self._opener.reset()
 
-    def order(self, what: str = None):
-        return Brewery(trj_file=self._path, fmt=self._fmt, what=what)
+    def order(self, what: str = None, verbose:bool=False):
+        return Brewery(trj_file=self._path, fmt=self._fmt, what=what, verbose=verbose)
 
     def reorder(self):
-        return Brewery(trj_file=self._path, fmt=self._fmt, what=self._what)
+        return Brewery(trj_file=self._path, fmt=self._fmt, what=self._what, verbose=False)
 
     def frange(self, start: int = 0, end: int = None, step: int = 1):
         self.move_frame(num=start)
         if end != None:
             assert start < end, "start should be lower than end"
         while True:
             try:
```

### Comparing `MDbrew-2.3.6/MDbrew/main/filetype/gro.py` & `MDbrew-2.3.7/MDbrew/main/filetype/gro.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/main/filetype/lmps.py` & `MDbrew-2.3.7/MDbrew/main/filetype/lmps.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         self._atom_keyword = "type"
         super().gen_db()
 
     def _make_one_frame_data(self, file):
         self.skip_line(file=file, num=3)
         atom_num = int(file.readline().split()[0])
         self.skip_line(file=file, num=1)
-        self.box_size = [sum([abs(float(box_length)) for box_length in file.readline().split()]) for _ in range(3)]
+        self.box_size = [sum([float(box_length) * ((-1)**(idx+1)) for idx, box_length in enumerate(file.readline().split())]) for _ in range(3)]
         self.column = file.readline().split()[2:]
         self.total_line_num = 9 + atom_num
         return [self.str2float_list(file.readline().split()) for _ in range(atom_num)]
 
     def skip_line(self, file, num):
         for _ in range(num):
             file.readline()
```

### Comparing `MDbrew-2.3.6/MDbrew/main/filetype/pdb.py` & `MDbrew-2.3.7/MDbrew/main/filetype/pdb.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/main/filetype/trr.py` & `MDbrew-2.3.7/MDbrew/main/filetype/trr.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/main/filetype/vasp.py` & `MDbrew-2.3.7/MDbrew/main/filetype/vasp.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/main/filetype/xyz.py` & `MDbrew-2.3.7/MDbrew/main/filetype/xyz.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/main/opener.py` & `MDbrew-2.3.7/MDbrew/main/opener.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/main/writer.py` & `MDbrew-2.3.7/MDbrew/main/writer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/tool/colorfont.py` & `MDbrew-2.3.7/MDbrew/tool/colorfont.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/tool/decorator.py` & `MDbrew-2.3.7/MDbrew/tool/decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     return deco
 
 
 # Wrapper of count the function execution time
 def color_print_verbose(name):
     def deco(func):
         def inner(*args, **kwrgs):
-            verbose = kwrgs.pop("verbose", True)
+            verbose = kwrgs.pop("verbose", False)
             if verbose:
                 print(f"[ {color.font_green}RUNN{color.reset} ] {name}", end="\r")
                 start = time()
             result = func(verbose=verbose, *args, **kwrgs)
             if verbose:
                 end = time()
                 end_string = f"[ {color.font_red}DONE{color.reset} ] {name}"
```

### Comparing `MDbrew-2.3.6/MDbrew/tool/doctor.py` & `MDbrew-2.3.7/MDbrew/tool/doctor.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew/tool/spacer.py` & `MDbrew-2.3.7/MDbrew/tool/spacer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/MDbrew.egg-info/SOURCES.txt` & `MDbrew-2.3.7/MDbrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.6/setup.py` & `MDbrew-2.3.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="MDbrew",
-    version="2.3.6",
+    version="2.3.7",
     author="Knu",
     author_email="minu928@snu.ac.kr",
     url="https://github.com/MyKnu/MDbrew",
-    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.3.6.tar.gz",
+    download_url="https://github.com/MyKnu/MDbrew/install_file/MDbrew-2.3.7.tar.gz",
     install_requies=[
-        "numpy>=1.0.0",
+        "numpy>=1.19.0",
         "pandas>=1.0.0",
         "matplotlib>=1.0.0",
         "tqdm>=1.0.0",
     ],
     description="Postprocessing tools for the MD simulation results (ex. lammps)",
     packages=find_packages(),
     keywords=["MD", "LAMMPS", "GROMACS"],
```

