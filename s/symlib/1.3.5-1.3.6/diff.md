# Comparing `tmp/symlib-1.3.5.tar.gz` & `tmp/symlib-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.3.5.tar", last modified: Fri Jun 16 17:54:04 2023, max compression
+gzip compressed data, was "symlib-1.3.6.tar", last modified: Fri Jun 23 23:11:25 2023, max compression
```

## Comparing `symlib-1.3.5.tar` & `symlib-1.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-16 17:54:04.171974 symlib-1.3.5/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.5/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-16 17:54:04.171862 symlib-1.3.5/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.5/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.5/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-06-16 17:54:04.172009 symlib-1.3.5/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2023-06-16 17:54:01.000000 symlib-1.3.5/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-16 17:54:04.171151 symlib-1.3.5/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     1715 2023-06-16 17:53:43.000000 symlib-1.3.5/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.5/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    53185 2023-06-16 17:53:43.000000 symlib-1.3.5/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)     9008 2023-06-16 17:53:43.000000 symlib-1.3.5/symlib/match.py
--rw-r--r--   0 phil       (501) staff       (20)    36176 2023-06-02 20:23:27.000000 symlib-1.3.5/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)     9876 2023-06-14 22:30:07.000000 symlib-1.3.5/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-16 17:54:04.171686 symlib-1.3.5/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-16 17:54:04.000000 symlib-1.3.5/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      303 2023-06-16 17:54:04.000000 symlib-1.3.5/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-06-16 17:54:04.000000 symlib-1.3.5/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2023-06-16 17:54:04.000000 symlib-1.3.5/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-06-16 17:54:04.000000 symlib-1.3.5/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-23 23:11:25.623422 symlib-1.3.6/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.6/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-23 23:11:25.623304 symlib-1.3.6/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.6/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.6/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-06-23 23:11:25.623457 symlib-1.3.6/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2023-06-23 23:11:21.000000 symlib-1.3.6/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-23 23:11:25.622436 symlib-1.3.6/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     1715 2023-06-16 17:53:43.000000 symlib-1.3.6/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.6/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    53792 2023-06-23 23:11:21.000000 symlib-1.3.6/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)     9008 2023-06-16 17:53:43.000000 symlib-1.3.6/symlib/match.py
+-rw-r--r--   0 phil       (501) staff       (20)    36176 2023-06-02 20:23:27.000000 symlib-1.3.6/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)     9876 2023-06-14 22:30:07.000000 symlib-1.3.6/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-23 23:11:25.623159 symlib-1.3.6/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-23 23:11:25.000000 symlib-1.3.6/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      303 2023-06-23 23:11:25.000000 symlib-1.3.6/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-06-23 23:11:25.000000 symlib-1.3.6/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2023-06-23 23:11:25.000000 symlib-1.3.6/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-06-23 23:11:25.000000 symlib-1.3.6/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.3.5/LICENSE` & `symlib-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.3.5/PKG-INFO` & `symlib-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.5
+Version: 1.3.6
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.3.5/setup.py` & `symlib-1.3.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.3.5"
+version = "1.3.6"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.3.5/symlib/__init__.py` & `symlib-1.3.6/symlib/__init__.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.5/symlib/file_management.py` & `symlib-1.3.6/symlib/file_management.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.5/symlib/lib.py` & `symlib-1.3.6/symlib/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,17 @@
               ("f_core", "f4"), ("f_core_rs", "f4"), ("d_core_mbp", "f4"),
               ("ok", "?"), ("ok_rs", "?"), ("is_err", "?"), ("is_err_rs", "?"),
               ("interp", "?")]
 
 """ SYMFIND_DTYPE is the main numpy datatype returned by read_symfind().
  - x (physical kpc): displacement from the host halo to the subhalo.
  - v (km/s): velocity relative to the host.
- - m (Msun): bound mass of the subhalo.
+ - m (Msun): bound mass of the subhalo. Post-porcessing has been done to reduce
+   noise by enfocing monotonicity (i.e. m(z) = max(m_raw(>= z)))
+ - m_raw (Msun): bound mass of the suhalo with no post-processing.
  - r_half (physical kpc) half-mass radius of the subhalo.
  - r_tidal (physical kpc): tidal radius of the subhalo. Accounts for angular
    momentum and the mass profile of the central halo. Tidal radii can be
    poor approximations if the size of the subhalo is comparable to the
    distance to the host centre or if the subhalo is at pericentre. There is no
    strict criteria for identifying this.
  - m_tidal (Msun): total mass within tidal radius.
@@ -170,14 +172,15 @@
  - d_core_mbp (physical kpc): the distance between the subhalo and the
    most-bound particle. Sometimes the most-bound particle can numerically
    diffuse out of the subhalo.
 """
 SYMFIND_DTYPE = [("x", "f4", (3,)), ("v", "f4", (3,)), ("r_tidal", "f4"),
                  ("r_half", "f4"), ("m_tidal", "f4"),
                  ("m_tidal_bound", "f4"), ("m", "f4"), ("vmax", "f4"),
+                 ("m_raw", "f4"),
                  ("ok", "?"), ("interp", "?"),
                  ("f_core", "f4"), ("f_core_rs", "f4"), ("d_core_mbp", "f4"),
                  ("r_half_rs", "f4"), ("ok_rs", "?"),
                  ("is_err", "?"), ("is_err_rs", "?")]
 
 """ UM_DTYPE is a numpy datatype representing UniverseMachine predictions for
 galaxy properties.
@@ -667,22 +670,37 @@
     h, hist = read_subhalos(dir_name)
     c = read_cores(dir_name)
 
     s = np.zeros(c.shape, dtype=SYMFIND_DTYPE)
     s["x"], s["v"] = c["x"], c["v"]
     s["r_tidal"], s["r_half"] = c["r_tidal"], c["r50_bound"] 
     s["m_tidal_bound"], s["m"] = c["m_tidal_bound"], c["m_bound"]
+    s["m_raw"] = c["m_bound"]
     s["vmax"], s["ok"], s["interp"] = c["vmax"], c["ok"], c["interp"]
     s["f_core"], s["f_core_rs"] = c["f_core"], c["f_core"]
     s["d_core_mbp"] = c["d_core_mbp"]
     s["r_half_rs"], s["ok_rs"] = c["r50_bound_rs"], c["ok_rs"]
     s["is_err"], s["is_err_rs"] = c["is_err"], c["is_err_rs"]
 
+    # Enforce monotonicity to reduce noise in the commonly used "m"
+    for i in range(len(s)):
+        s["m"][i] = monotonic_m(s["m_raw"][i], s["ok"][i])
+
     return s, hist
 
+def monotonic_m(m_in, ok):
+    m_out = np.zeros(len(m_in))
+    idx = np.where(ok)[0]
+
+    prev_max = 0
+    for i in idx[::-1]:
+        m_out[i] = max(m_in[i], prev_max)
+        prev_max = m_out[i]
+
+    return m_out
 
 def read_cores(dir_name, include_false_selections=False, suffix="fid3"):
     """ read_cores read the particle-tracked halo cores of the halo in the
     given directory. The returned array is a structured array of type
     CORE_DTYPE with shape (n_halos, n_snaps).
     """
     if suffix == "":
```

### Comparing `symlib-1.3.5/symlib/match.py` & `symlib-1.3.6/symlib/match.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.5/symlib/star_tagging.py` & `symlib-1.3.6/symlib/star_tagging.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.5/symlib/util.py` & `symlib-1.3.6/symlib/util.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.5/symlib.egg-info/PKG-INFO` & `symlib-1.3.6/symlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.5
+Version: 1.3.6
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

