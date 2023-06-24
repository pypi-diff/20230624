# Comparing `tmp/qsonic-0.7.3.tar.gz` & `tmp/qsonic-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsonic-0.7.3.tar", last modified: Wed Jun 21 22:20:31 2023, max compression
+gzip compressed data, was "qsonic-0.7.4.tar", last modified: Sat Jun 24 15:23:28 2023, max compression
```

## Comparing `qsonic-0.7.3.tar` & `qsonic-0.7.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.965005 qsonic-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-21 22:20:12.000000 qsonic-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-21 22:20:31.965005 qsonic-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-21 22:20:12.000000 qsonic-0.7.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.957005 qsonic-0.7.3/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.961005 qsonic-0.7.3/py/qsonic/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    52579 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/picca_continuum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.961005 qsonic-0.7.3/py/qsonic/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/scripts/qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/scripts/qsonic_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    29973 2023-06-21 22:20:12.000000 qsonic-0.7.3/py/qsonic/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.961005 qsonic-0.7.3/py/qsonic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 22:20:31.000000 qsonic-0.7.3/py/qsonic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 22:20:12.000000 qsonic-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-21 22:20:12.000000 qsonic-0.7.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-21 22:20:31.965005 qsonic-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:20:12.000000 qsonic-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:20:31.965005 qsonic-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_mathtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_mpi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_picca_continuum.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_qsonic_calib.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-21 22:20:12.000000 qsonic-0.7.3/tests/test_spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.047543 qsonic-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-24 15:23:00.000000 qsonic-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-24 15:23:28.047543 qsonic-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-06-24 15:23:00.000000 qsonic-0.7.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.039543 qsonic-0.7.4/py/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.043543 qsonic-0.7.4/py/qsonic/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13560 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17279 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52575 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/picca_continuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.047543 qsonic-0.7.4/py/qsonic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/scripts/qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12088 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/scripts/qsonic_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30200 2023-06-24 15:23:00.000000 qsonic-0.7.4/py/qsonic/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.047543 qsonic-0.7.4/py/qsonic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 15:23:28.000000 qsonic-0.7.4/py/qsonic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-24 15:23:00.000000 qsonic-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-24 15:23:00.000000 qsonic-0.7.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-24 15:23:28.047543 qsonic-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 15:23:00.000000 qsonic-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 15:23:28.047543 qsonic-0.7.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_mathtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_mpi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_picca_continuum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_qsonic_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-24 15:23:00.000000 qsonic-0.7.4/tests/test_spectrum.py
```

### Comparing `qsonic-0.7.3/LICENSE` & `qsonic-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/PKG-INFO` & `qsonic-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.7.3
+Version: 0.7.4
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
```

### Comparing `qsonic-0.7.3/README.rst` & `qsonic-0.7.4/README.rst`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/py/qsonic/calibration.py` & `qsonic-0.7.4/py/qsonic/calibration.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/py/qsonic/catalog.py` & `qsonic-0.7.4/py/qsonic/catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/py/qsonic/io.py` & `qsonic-0.7.4/py/qsonic/io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/py/qsonic/masks.py` & `qsonic-0.7.4/py/qsonic/masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/py/qsonic/mathtools.py` & `qsonic-0.7.4/py/qsonic/mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/py/qsonic/mpi_utils.py` & `qsonic-0.7.4/py/qsonic/mpi_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import warnings
 
 import fitsio
 import numpy as np
 
 from qsonic import QsonicException
 
 
@@ -58,29 +57,14 @@
     fnc: logging method
         Channel to log, usually info or error.
     """
     if mpi_rank == 0:
         getattr(logging, fnc)(msg)
 
 
-def warn_mpi(msg, mpi_rank):
-    """ Warns of RuntimeWarning only on ``mpi_rank=0``.
-
-    Arguments
-    ---------
-    msg: str
-        Message to log.
-    mpi_rank: int
-        Rank of the MPI process.
-    """
-
-    if mpi_rank == 0:
-        warnings.warn(msg, RuntimeWarning)
-
-
 class _INVALID_VALUE(object):
     """ Sentinel for invalid values. """
 
 
 def mpi_fnc_bcast(fnc, comm=None, mpi_rank=0, err_msg="", *args, **kwargs):
     """ Wrapper function to run function then broadcast. Return value of
     ``fnc`` must be broadcastable.
```

### Comparing `qsonic-0.7.3/py/qsonic/picca_continuum.py` & `qsonic-0.7.4/py/qsonic/picca_continuum.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from scipy.interpolate import UnivariateSpline
 from scipy.special import legendre
 
 from mpi4py import MPI
 
 from qsonic import QsonicException
 from qsonic.spectrum import valid_spectra
-from qsonic.mpi_utils import logging_mpi, warn_mpi, mpi_fnc_bcast, MPISaver
+from qsonic.mpi_utils import logging_mpi, mpi_fnc_bcast, MPISaver
 from qsonic.mathtools import (
     mypoly1d, block_covariance_of_square,
     FastLinear1DInterp, FastCubic1DInterp,
     SubsampleCov
 )
 
 
@@ -422,16 +422,14 @@
         spectra_list: list(Spectrum)
             Spectrum objects to fit.
 
         Raises
         ------
         QsonicException
             If there are no valid fits.
-        RuntimeWarning
-            If more than 20% spectra have invalid fits.
         """
         num_valid_fits = 0
         num_invalid_fits = 0
 
         # For each forest fit continuum
         for spec in spectra_list:
             self.fit_continuum(spec)
@@ -448,15 +446,17 @@
                     self.mpi_rank)
 
         if num_valid_fits == 0:
             raise QsonicException("Crucial error: No valid continuum fits!")
 
         invalid_ratio = num_invalid_fits / (num_valid_fits + num_invalid_fits)
         if invalid_ratio > 0.2:
-            warn_mpi("More than 20% spectra have invalid fits.", self.mpi_rank)
+            logging_mpi(
+                "More than 20% spectra have invalid fits.", self.mpi_rank,
+                "warning")
 
     def _project_normalize_meancont(self, new_meancont):
         """ Project out higher order Legendre polynomials from the new mean
         continuum since these are degenerate with the free fitting parameters.
         Returns a normalized mean continuum. Integrals are calculated using
         ``np.trapz`` with ``ln lambda_RF`` as x array.
 
@@ -535,17 +535,17 @@
 
         self.flux_stacker.calculate()
         self.comm.Allreduce(MPI.IN_PLACE, norm_flux)
         self.comm.Allreduce(MPI.IN_PLACE, counts)
         w = counts > 0
 
         if w.sum() != self.nbins:
-            warn_mpi(
+            logging_mpi(
                 "Extrapolating empty bins in the mean continuum.",
-                self.mpi_rank)
+                self.mpi_rank, "warning")
 
         norm_flux[w] /= counts[w]
         norm_flux[~w] = np.mean(norm_flux[w])
         std_flux[w] = 1 / np.sqrt(counts[w])
         std_flux[~w] = 10 * np.mean(std_flux[w])
 
         # Smooth new estimates
@@ -564,15 +564,15 @@
         all_pt_test = np.all(np.abs(norm_flux) < 0.33 * std_flux)
         chi2_change = np.sum((norm_flux / std_flux)**2) / self.nbins
         has_converged = (chi2_change < 1e-3) | all_pt_test
 
         if self.mpi_rank != 0:
             return has_converged
 
-        text = ("Continuum updates\n" "rfwave\t| update\t| error\n")
+        text = ("Continuum updates:\n" "rfwave\t| update\t| error\n")
 
         sl = np.s_[::max(1, self.nbins // 10)]
         for w, n, e in zip(self.rfwave[sl], norm_flux[sl], std_flux[sl]):
             text += f"{w:7.2f}\t| {n:7.2e}\t| +- {e:7.2e}\n"
 
         text += f"Change in chi2: {chi2_change*100:.4e}%"
         logging_mpi(text, 0)
@@ -619,26 +619,26 @@
             self.varlss_interp.reset(y[:, 0], ep=ep[:, 0])
             self.eta_interp.reset(y[:, 1], ep=ep[:, 1])
 
         if self.mpi_rank != 0:
             return
 
         step = max(1, self.varlss_fitter.nwbins // 10)
-        text = ("------------------------------\n"
+        text = ("Variance fitting results:\n"
                 "wave\t| var_lss +-  error \t|   eta   +-  error \n")
 
         for i in range(0, self.varlss_fitter.nwbins, step):
             w = self.varlss_fitter.waveobs[i]
             v = self.varlss_interp.fp[i]
             ve = self.varlss_interp.ep[i]
             n = self.eta_interp.fp[i]
             ne = self.eta_interp.ep[i]
             text += \
                 f"{w:7.2f}\t| {v:7.2e} +- {ve:7.2e}\t| {n:7.2e} +- {ne:7.2e}\n"
-        text += "------------------------------"
+
         logging_mpi(text, 0)
 
     def _normalize_flux(self, spectra_list):
         """Multiplies continuum estimates with stacked values in order to
         normalize flux in the observed grid to be 1 if
         ``--normalize-stacked-flux`` is passed.
 
@@ -706,15 +706,16 @@
             self.update_var_lss_eta(spectra_list)
 
             if has_converged:
                 logging_mpi("Iteration has converged.", self.mpi_rank)
                 break
 
         if not has_converged:
-            warn_mpi("Iteration has NOT converged.", self.mpi_rank)
+            logging_mpi("Iteration has NOT converged.", self.mpi_rank,
+                        "warning")
 
         self._normalize_flux(spectra_list)
 
         self.save(fattr)
         if self.varlss_fitter:
             self.varlss_fitter.write(fattr)
         fattr.close()
@@ -817,16 +818,15 @@
         corder = self.cont_order + 1
 
         dtype = np.dtype([
             ('TARGETID', 'int64'), ('Z', 'f4'), ('HPXPIXEL', 'i8'),
             ('ARMS', 'U5'), ('MEANSNR', 'f4', 3), ('RSNR', 'f4'),
             ('MPI_RANK', 'i4'),
             ('CONT_valid', bool), ('CONT_chi2', 'f4'), ('CONT_dof', 'i4'),
-            ('CONT_x', 'f4', corder),
-            ('CONT_xcov', 'f4', corder**2)
+            ('CONT_x', 'f4', (corder, )), ('CONT_xcov', 'f4', (corder**2, ))
         ])
         local_catalog = np.empty(len(spectra_list), dtype=dtype)
 
         for i, spec in enumerate(spectra_list):
             mean_snrs = np.zeros(3)
             _x = list(spec.mean_snr.values())
             mean_snrs[:len(_x)] = _x
@@ -1200,18 +1200,18 @@
             i1 = iwave * self.nvarbins
             i2 = i1 + self.nvarbins
             wave_slice = np.s_[i1:i2]
             w = w_gtr_min[wave_slice]
 
             if w.sum() == 0:
                 nfails += 1
-                warn_mpi(
+                logging_mpi(
                     "Not enough statistics for VarLSSFitter at"
                     f" wave_obs: {self.waveobs[iwave]:.2f}.",
-                    self.mpi_rank)
+                    self.mpi_rank, "warning")
                 continue
 
             if self.use_cov:
                 err2use = err_base[iwave][:, w][w, :]
             else:
                 err2use = err_base[wave_slice][w]
 
@@ -1224,32 +1224,32 @@
                     sigma=err2use,
                     absolute_sigma=True,
                     check_finite=True,
                     bounds=(0, 2)
                 )
             except Exception as e:
                 nfails += 1
-                warn_mpi(
+                logging_mpi(
                     "VarLSSFitter failed at wave_obs: "
                     f"{self.waveobs[iwave]:.2f}. "
                     f"Reason: {e}. Extrapolating.",
-                    self.mpi_rank)
+                    self.mpi_rank, "warning")
             else:
                 fit_results[iwave] = pfit
                 std_results[iwave] = np.sqrt(np.diag(pcov))
 
         invalid_ratio = nfails / fit_results.shape[0]
         if invalid_ratio > 0.4:
             raise QsonicException(
                 "VarLSSFitter failed at more than 40% points.")
 
         if nfails > 0:
-            warn_mpi(
+            logging_mpi(
                 f"VarLSSFitter failed and extrapolated at {nfails} points.",
-                self.mpi_rank)
+                self.mpi_rank, "warning")
 
         # Smooth new estimates
         if smooth:
             fit_results = self._smooth_fit_results(fit_results, std_results)
 
         return fit_results, std_results
```

### Comparing `qsonic-0.7.3/py/qsonic/scripts/qsonic_calib.py` & `qsonic-0.7.4/py/qsonic/scripts/qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/py/qsonic/scripts/qsonic_fit.py` & `qsonic-0.7.4/py/qsonic/scripts/qsonic_fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,22 +115,30 @@
     spectra_list = []
     # Each process reads its own list
     for cat in local_queue:
         local_specs = qsonic.io.read_spectra_onehealpix(
             cat, args.input_dir, args.arms, args.mock_analysis, skip_resomat,
             args.true_continuum)
 
+        specs_to_keep = []
+
         for spec in local_specs:
             spec.set_forest_region(
                 args.wave1, args.wave2, args.forest_w1, args.forest_w2)
-
             spec.remove_nonforest_pixels()
 
-        spectra_list.extend(
-            [spec for spec in local_specs if spec.rsnr > args.min_rsnr])
+            if not spec.forestwave:
+                continue
+
+            if spec.rsnr < args.min_rsnr:
+                continue
+
+            specs_to_keep.append(spec)
+
+        spectra_list.extend(specs_to_keep)
 
         # if args.skip_resomat:
         #     continue
 
         # w = np.array(
         #     [spec.rsnr > args.min_rsnr for spec in local_specs], dtype=bool)
         # nspec = w.sum()
@@ -360,15 +368,18 @@
     start_time = time.time()
 
     from mpi4py import MPI
     comm = MPI.COMM_WORLD
     mpi_rank = comm.Get_rank()
     mpi_size = comm.Get_size()
 
-    logging.basicConfig(level=logging.DEBUG)
+    logging.basicConfig(
+        format='%(asctime)s - %(levelname)s: %(message)s',
+        datefmt='%Y/%m/%d %I:%M:%S %p',
+        level=logging.DEBUG)
     logging.captureWarnings(True)
 
     try:
         mpi_run_all(comm, mpi_rank, mpi_size)
     except QsonicException as e:
         logging_mpi(e, mpi_rank, "exception")
     except Exception as e:
```

### Comparing `qsonic-0.7.3/py/qsonic/spectrum.py` & `qsonic-0.7.4/py/qsonic/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,27 +214,27 @@
         self._forestivar_sm = {}
         self._forestreso = {}
         self._forestweight = {}
 
         self._smoothing_scale = 0
 
         for arm, wave_arm in self.wave.items():
-            self.flux[arm] = flux[arm][idx]
-            self.ivar[arm] = ivar[arm][idx]
+            self.flux[arm] = flux[arm][idx].copy()
+            self.ivar[arm] = ivar[arm][idx].copy()
             w = (mask[arm][idx] != 0) | np.isnan(self.flux[arm])\
                 | np.isnan(self.ivar[arm])
             self.flux[arm][w] = 0
             self.ivar[arm][w] = 0
 
             if not reso:
                 continue
             elif reso[arm].ndim == 2:
                 self.reso[arm] = reso[arm].copy()
             else:
-                self.reso[arm] = reso[arm][idx]
+                self.reso[arm] = reso[arm][idx].copy()
 
         self.cont_params = {}
         self.cont_params['method'] = ''
         self.cont_params['valid'] = False
         self.cont_params['x'] = np.array([1., 0.])
         self.cont_params['xcov'] = np.eye(2)
         self.cont_params['chi2'] = -1.
@@ -302,19 +302,22 @@
             real_size_arm = np.sum(self.ivar[arm][ii1:ii2] > 0)
             if real_size_arm == 0:
                 continue
 
             self._f1[arm], self._f2[arm] = ii1, ii2
 
             # Does this create a view or copy array?
-            self._forestwave[arm] = wave_arm[ii1:ii2]
-            self._forestflux[arm] = self.flux[arm][ii1:ii2]
-            self._forestivar[arm] = self.ivar[arm][ii1:ii2]
+            # See https://numpy.org/doc/stable/user/basics.copies.html
+            # Slicing creates views, not copies. Bases of views are not removed
+            # from memory!
+            self._forestwave[arm] = wave_arm[ii1:ii2].copy()
+            self._forestflux[arm] = self.flux[arm][ii1:ii2].copy()
+            self._forestivar[arm] = self.ivar[arm][ii1:ii2].copy()
             if self.reso:
-                self._forestreso[arm] = self.reso[arm][:, ii1:ii2]
+                self._forestreso[arm] = self.reso[arm][:, ii1:ii2].copy()
 
         self._forestivar_sm = self._forestivar
         self._forestweight = self._forestivar
         self._set_forest_related_parameters()
 
     def drop_short_arms(self, lya1=0, lya2=0, skip_ratio=0):
         """Arms that have less than ``skip_ratio`` pixels are removed from
```

### Comparing `qsonic-0.7.3/py/qsonic.egg-info/PKG-INFO` & `qsonic-0.7.4/py/qsonic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsonic
-Version: 0.7.3
+Version: 0.7.4
 Summary: Quasar continuum fitter for DESI
 Author: Naim Goksel Karacayli
 Author-email: ngokselk@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/p-slash/qsonic/issues
 Project-URL: Documentation, http://qsonic.readthedocs.io/
 Project-URL: Source, https://github.com/p-slash/qsonic
```

### Comparing `qsonic-0.7.3/py/qsonic.egg-info/SOURCES.txt` & `qsonic-0.7.4/py/qsonic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/setup.cfg` & `qsonic-0.7.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.7.3
+current_version = 0.7.4
 commit = True
 tag = True
 
 [bumpversion:file:py/qsonic/__init__.py]
 search = __version__ = '{current_version}'
 replace = __version__ = '{new_version}'
```

### Comparing `qsonic-0.7.3/tests/test_catalog.py` & `qsonic-0.7.4/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/tests/test_io.py` & `qsonic-0.7.4/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/tests/test_masks.py` & `qsonic-0.7.4/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/tests/test_mathtools.py` & `qsonic-0.7.4/tests/test_mathtools.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/tests/test_mpi_utils.py` & `qsonic-0.7.4/tests/test_mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/tests/test_picca_continuum.py` & `qsonic-0.7.4/tests/test_picca_continuum.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/tests/test_qsonic_calib.py` & `qsonic-0.7.4/tests/test_qsonic_calib.py`

 * *Files identical despite different names*

### Comparing `qsonic-0.7.3/tests/test_spectrum.py` & `qsonic-0.7.4/tests/test_spectrum.py`

 * *Files identical despite different names*

