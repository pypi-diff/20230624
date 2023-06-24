# Comparing `tmp/sleepeeg-0.2.3.tar.gz` & `tmp/sleepeeg-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepeeg-0.2.3.tar", last modified: Mon Jun 19 10:06:15 2023, max compression
+gzip compressed data, was "sleepeeg-0.3.0.tar", last modified: Sat Jun 24 13:04:15 2023, max compression
```

## Comparing `sleepeeg-0.2.3.tar` & `sleepeeg-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 10:06:15.322218 sleepeeg-0.2.3/
--rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     1728 2023-06-19 10:06:15.322218 sleepeeg-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1306 2023-06-09 12:52:22.000000 sleepeeg-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 10:06:15.292298 sleepeeg-0.2.3/docs/
--rw-rw-rw-   0        0        0     2495 2023-06-06 06:12:53.000000 sleepeeg-0.2.3/docs/conf.py
--rw-rw-rw-   0        0        0      861 2023-06-19 08:41:56.000000 sleepeeg-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-19 10:06:15.323215 sleepeeg-0.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-19 10:06:15.298281 sleepeeg-0.2.3/sleepeeg/
--rw-rw-rw-   0        0        0    51888 2023-06-19 06:26:07.000000 sleepeeg-0.2.3/sleepeeg/base.py
--rw-rw-rw-   0        0        0    12356 2023-06-19 09:06:55.000000 sleepeeg-0.2.3/sleepeeg/dashboard.py
--rw-rw-rw-   0        0        0    34242 2023-06-19 06:53:17.000000 sleepeeg-0.2.3/sleepeeg/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-06-19 10:06:15.319225 sleepeeg-0.2.3/sleepeeg.egg-info/
--rw-rw-rw-   0        0        0     1728 2023-06-19 10:06:15.000000 sleepeeg-0.2.3/sleepeeg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-06-19 10:06:15.000000 sleepeeg-0.2.3/sleepeeg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 10:06:15.000000 sleepeeg-0.2.3/sleepeeg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      132 2023-06-19 10:06:15.000000 sleepeeg-0.2.3/sleepeeg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       33 2023-06-19 10:06:15.000000 sleepeeg-0.2.3/sleepeeg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 13:04:15.672348 sleepeeg-0.3.0/
+-rw-rw-rw-   0        0        0     1088 2023-03-20 20:54:05.000000 sleepeeg-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0     1728 2023-06-24 13:04:15.671350 sleepeeg-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1306 2023-06-09 12:52:22.000000 sleepeeg-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 13:04:15.643424 sleepeeg-0.3.0/docs/
+-rw-rw-rw-   0        0        0     2433 2023-06-24 10:09:30.000000 sleepeeg-0.3.0/docs/conf.py
+-rw-rw-rw-   0        0        0      839 2023-06-24 12:45:44.000000 sleepeeg-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:04:15.673344 sleepeeg-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 13:04:15.651403 sleepeeg-0.3.0/sleepeeg/
+-rw-rw-rw-   0        0        0    48299 2023-06-24 12:09:58.000000 sleepeeg-0.3.0/sleepeeg/base.py
+-rw-rw-rw-   0        0        0    12311 2023-06-24 12:39:28.000000 sleepeeg-0.3.0/sleepeeg/dashboard.py
+-rw-rw-rw-   0        0        0    28327 2023-06-24 12:51:40.000000 sleepeeg-0.3.0/sleepeeg/pipeline.py
+-rw-rw-rw-   0        0        0     2005 2023-06-24 08:52:40.000000 sleepeeg-0.3.0/sleepeeg/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:04:15.669355 sleepeeg-0.3.0/sleepeeg.egg-info/
+-rw-rw-rw-   0        0        0     1728 2023-06-24 13:04:15.000000 sleepeeg-0.3.0/sleepeeg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-06-24 13:04:15.000000 sleepeeg-0.3.0/sleepeeg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:04:15.000000 sleepeeg-0.3.0/sleepeeg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-06-24 13:04:15.000000 sleepeeg-0.3.0/sleepeeg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-24 13:04:15.000000 sleepeeg-0.3.0/sleepeeg.egg-info/top_level.txt
```

### Comparing `sleepeeg-0.2.3/LICENSE` & `sleepeeg-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.2.3/PKG-INFO` & `sleepeeg-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.2.3
+Version: 0.3.0
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
 Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
 Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
 Keywords: sleep,eeg
 Requires-Python: >=3.10
```

### Comparing `sleepeeg-0.2.3/README.md` & `sleepeeg-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sleepeeg-0.2.3/docs/conf.py` & `sleepeeg-0.3.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 html_theme = "furo"
 html_static_path = ["_static"]
 
 intersphinx_mapping = {
     "mne": ("https://mne.tools/stable/", None),
     "yasa": ("https://raphaelvallat.com/yasa/build/html/", None),
     "mpl": ("https://matplotlib.org/stable/", None),
-    "fooof": ("https://fooof-tools.github.io/fooof/", None),
 }
 
 intersphinx_disabled_reftypes = ["*"]
 
 
 def linkcode_resolve(domain, info):
     """Determine the URL corresponding to a Python object.
```

### Comparing `sleepeeg-0.2.3/pyproject.toml` & `sleepeeg-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 exclude = ["notebooks"]  # empty by default
 
 [project]
 name = "sleepeeg"
-version = "0.2.3"
+version = "0.3.0"
 authors = [
     {name = "Gennadiy Belonosov", email = "gennadiyb@mail.tau.ac.il"},
 ]
 description = "Sleep EEG preprocessing and analysis"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
@@ -20,18 +20,17 @@
     "attrs",
     "mne>=1.4.1",
     "mne-qt-browser",
     "pyqt5",
     "yasa==0.6.3",
     "lspopt",
     "ipympl",
-    "numpy<=1.23.5",
+    "numpy",
     "pandas",
     "scipy",
-    "fooof",
     "natsort",
     "more-itertools",
     "h5io",
     "loguru"
 ]
 
 [project.urls]
```

### Comparing `sleepeeg-0.2.3/sleepeeg/base.py` & `sleepeeg-0.3.0/sleepeeg/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,31 @@
+import errno
 import os
 import sys
-import errno
-
-from loguru import logger
 from abc import ABC, abstractmethod
 from collections.abc import Iterable
 from pathlib import Path
-import functools
-
-from typing import TypeVar, Type
-from attrs import define, field
-from tqdm import tqdm
+from typing import Type, TypeVar
 
 import matplotlib.pyplot as plt
-import numpy as np
 import mne
+import numpy as np
+from attrs import define, field
+from loguru import logger
+from tqdm import tqdm
 
+from .utils import logger_wraps
 
 # For type annotation of pipe elements.
 BasePipeType = TypeVar("BasePipeType", bound="BasePipe")
 
 
-def logger_wraps(*, level="DEBUG"):
-    def wrapper(func):
-        name = func.__name__
-
-        @functools.wraps(func)
-        def wrapped(self, *args, **kwargs):
-            logger_ = logger.opt(depth=1)
-            logger_.log(
-                level,
-                f"Entering '{self.__class__.__name__}.{name}' (args={args}, kwargs={kwargs})",
-            )
-            result = func(self, *args, **kwargs)
-
-            return result
-
-        return wrapped
-
-    return wrapper
-
-
 @define(kw_only=True, slots=False)
 class BasePipe(ABC):
-    """A template class for the pipeline segments."""
+    """A base class for all per-subject pipeline segments."""
 
     prec_pipe: Type[BasePipeType] = field(default=None)
     """Preceding pipe that hands over mne_raw attribute."""
 
     path_to_eeg: Path = field(converter=Path)
     """Can be any file type supported by :py:func:`mne:mne.io.read_raw`.
     """
@@ -64,17 +42,17 @@
             raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), value)
 
     output_dir: Path = field(converter=Path)
     """Path to the directory where the output will be saved."""
 
     @output_dir.default
     def _set_output_dir(self):
-        return (
-            self.prec_pipe.output_dir if self.prec_pipe else self.path_to_eeg.parents[0]
-        )
+        if self.prec_pipe:
+            return self.prec_pipe.output_dir
+        raise TypeError("missing 1 required keyword-only argument: 'output_dir'")
 
     @output_dir.validator
     def _validate_output_dir(self, attr, value):
         self.output_dir.mkdir(exist_ok=True)
         (self.output_dir / self.__class__.__name__).mkdir(exist_ok=True)
         logger.remove()
         logger.add(self.output_dir / "pipeline.log")
@@ -83,57 +61,38 @@
     """An instanse of :py:class:`mne:mne.io.Raw`.
     """
 
     @mne_raw.default
     def _read_mne_raw(self):
         if self.prec_pipe:
             return self.prec_pipe.mne_raw
+
         try:
             return mne.io.read_raw(self.path_to_eeg)
         except RuntimeError as err:
             if "EGI epoch first/last samps" in str(err):
-                import re
-                from ast import literal_eval
-                from itertools import chain
-                import shutil
+                from .utils import fix_mff_epochs_xml
 
                 logger.warning(
-                    "Fixing epochs.xml from the .mff, original file is saved as epochs_old.xml"
+                    "Trying to fix epochs.xml from the .mff, "
+                    "original file will be saved as epochs_old.xml"
                 )
-                values = chain.from_iterable(
-                    zip(
-                        range(-1000, -6000, -1000),
-                        range(1000, 6000, 1000),
+
+                value = fix_mff_epochs_xml(self.path_to_eeg)
+
+                if value:
+                    logger.info(
+                        f"epochs.xml were fixed successfully (endTime {value}), "
+                        "proceeding with loading the .mff file."
                     )
-                )
-                shutil.copyfile(
-                    self.path_to_eeg / "epochs.xml",
-                    self.path_to_eeg / "epochs_old.xml",
-                )
-                for value in values:
-                    operation = (
-                        f"subtract {abs(value)} from"
-                        if value < 0
-                        else f"add {abs(value)} to"
+                else:
+                    logger.error(
+                        "No success in fixing epochs.xml, try to debug it manually"
                     )
-                    logger.info(f"Trying to {operation} the last 'endTime' tag")
-                    with open(self.path_to_eeg / "epochs.xml", "r+") as epochs_f:
-                        orig_xml = epochs_f.read()
-                        matches = re.findall(r"<endTime>(\d+)<\/endTime>", orig_xml)
-                        new_xml = orig_xml.replace(
-                            matches[-1], str(literal_eval(matches[-1]) + value)
-                        )
-                        epochs_f.seek(0)
-                        epochs_f.write(new_xml)
-                        epochs_f.truncate()
-                    try:
-                        return mne.io.read_raw(self.path_to_eeg)
-                    except:
-                        with open(self.path_to_eeg / "epochs.xml", "w") as epochs_f:
-                            epochs_f.write(orig_xml)
+                    raise err
 
             else:
                 raise
         except Exception as err:
             print(f"Unexpected {err=}, {type(err)=}")
             raise
 
@@ -142,14 +101,32 @@
         """A wrapper for :py:class:`raw.info["sfreq"] <mne:mne.Info>`.
 
         Returns:
             float: sampling frequency
         """
         return self.mne_raw.info["sfreq"]
 
+    @property
+    def bad_data_percent(self):
+        """Calculates percent of data segments annotated as BAD.
+
+        Returns:
+            float: percent of bad data spans in raw data
+        """
+        df = self.mne_raw.annotations.to_data_frame()
+        return round(
+            100
+            * (
+                df[df.description.str.contains("bad", case=False)].duration.sum()
+                * self.sf
+            )
+            / self.mne_raw.n_times,
+            2,
+        )
+
     def plot(
         self,
         save_annotations: bool = False,
         save_bad_channels: bool = False,
         overwrite: bool = False,
         **kwargs,
     ):
@@ -161,41 +138,44 @@
             overwrite: Whether to overwrite annotations and bad_channels files if exist.
                 Defaults to False.
             **kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.plot`.
         """
         kwargs.setdefault("theme", "dark")
         kwargs.setdefault("bad_color", "r")
         kwargs.setdefault("scalings", "auto")
-        kwargs.setdefault("block", True)
+        kwargs["block"] = True
 
         self.mne_raw.plot(**kwargs)
 
         if save_annotations:
             self.mne_raw.annotations.save(
                 self.output_dir / self.__class__.__name__ / "annotations.txt",
                 overwrite=overwrite,
             )
+
         if save_bad_channels:
-            from natsort import natsorted
+            new_bads = self.mne_raw.info["bads"]
 
-            if overwrite:
-                with open(
-                    self.output_dir / self.__class__.__name__ / "bad_channels.txt", "w"
-                ) as f:
-                    for bad in natsorted(self.mne_raw.info["bads"]):
-                        f.write(f"{bad}\n")
-            else:
-                with open(
-                    self.output_dir / self.__class__.__name__ / "bad_channels.txt", "a+"
-                ) as f:
-                    bads = natsorted(set(f.read().split() + self.mne_raw.info["bads"]))
-                    f.seek(0)
+            if new_bads:
+                from natsort import natsorted
+
+                fpath = self.output_dir / self.__class__.__name__ / "bad_channels.txt"
+                old_bads = []
+                if fpath.exists():
+                    with open(fpath, "r") as f:
+                        old_bads = f.read().split()
+
+                with open(fpath, "w") as f:
+                    bads = (
+                        natsorted(new_bads)
+                        if overwrite
+                        else natsorted(set(old_bads + new_bads))
+                    )
                     for bad in bads:
                         f.write(f"{bad}\n")
-                    f.truncate()
 
     def plot_sensors(
         self, legend: Iterable[str] = None, legend_args: dict = None, **kwargs
     ):
         """A wrapper for :py:func:`mne:mne.viz.plot_sensors` with a legend.
 
         Args:
@@ -220,15 +200,14 @@
         if legend:
             if not len(legend) == len(ch_groups):
                 raise ValueError(
                     "Length of the legend and of the ch_groups should be equal"
                 )
 
             patches = []
-            # if legend:
             colors = np.linspace(0, 1, len(ch_groups))
             color_vals = [plt.cm.jet(colors[i]) for i in range(len(ch_groups))]
             for i, color in enumerate(color_vals):
                 if legend[i]:
                     patches.append(mpatches.Patch(color=color, label=legend[i]))
             if self.mne_raw.info["bads"]:
                 patches.append(mpatches.Patch(color="red", label="Bad"))
@@ -260,15 +239,15 @@
         self.mne_raw.load_data().set_eeg_reference(
             ref_channels=ref_channels, projection=projection, **kwargs
         )
 
 
 @define(kw_only=True, slots=False)
 class BaseHypnoPipe(BasePipe, ABC):
-    """A template class for the sleep stage analysis pipeline segments."""
+    """A base class for the sleep stage analysis pipeline segments."""
 
     path_to_hypno: Path = field(converter=Path)
     """Path to hypnogram. Must be text file with every 
     row being int representing sleep stage for the epoch.
     """
 
     @path_to_hypno.default
@@ -299,30 +278,30 @@
     """
 
     @hypno.default
     def _import_hypno(self):
         if self.prec_pipe and isinstance(self.prec_pipe, BaseHypnoPipe):
             return self.prec_pipe.hypno
         if self.path_to_hypno == Path("/"):
-            return np.empty(0)
+            return None
         return np.loadtxt(self.path_to_hypno)
 
-    hypno_up: np.array = field()
+    hypno_up: np.array = field(init=False)
     """ Hypnogram upsampled to the sampling frequency of the raw data.
     """
 
     @hypno_up.default
     def _set_hypno_up(self):
         return self.hypno
 
     def __attrs_post_init__(self):
-        if self.hypno.any():
-            self.__upsample_hypno()
+        if self.hypno is not None:
+            self._upsample_hypno()
 
-    def __upsample_hypno(self):
+    def _upsample_hypno(self):
         """Adapted from YASA."""
         repeats = self.sf / self.hypno_freq
         if self.hypno_freq > self.sf:
             raise ValueError(
                 "Sampling frequency of hypnogram must be smaller than that of eeg signal."
             )
         if not repeats.is_integer():
@@ -358,15 +337,15 @@
         self,
         eeg_name: str = "E183",
         eog_name: str = "E252",
         emg_name: str = "E247",
         ref_name: str = "E26",
         save: bool = True,
     ):
-        """Runs YASA's automatic sleep staging
+        """Runs YASA's automatic sleep staging.
 
         Args:
             eeg_name: Preferentially a central electrode. Defaults to "E183".
             eog_name: Preferentially, the left LOC channel. Defaults to "E252".
             emg_name: Preferentially a chin electrode. Defaults to "E247".
             ref_name: Reference channel, preferentially a mastoid. Defaults to "E26".
             save: Whether to save the hypnogram to file. Defaults to True.
@@ -378,15 +357,15 @@
             eeg_name=eeg_name,
             eog_name=eog_name,
             emg_name=emg_name,
         )
         hypno = sls.predict()
         self.hypno = hypno_str_to_int(hypno)
         self.hypno_freq = 1 / 30
-        self.__upsample_hypno()
+        self._upsample_hypno()
         sls.plot_predict_proba()
         if save:
             np.savetxt(
                 self.output_dir / self.__class__.__name__ / "predicted_hypno.txt",
                 self.hypno,
                 fmt="%d",
             )
@@ -399,18 +378,20 @@
     def sleep_stats(self, save: bool = False):
         """A wrapper for :py:func:`yasa:yasa.sleep_statistics`.
 
         Args:
             save: Whether to save the stats to csv. Defaults to False.
         """
 
-        from yasa import sleep_statistics
         from csv import DictWriter
 
-        assert self.hypno.any(), "There is no hypnogram to get stats from."
+        from yasa import sleep_statistics
+
+        if self.hypno is None:
+            raise ValueError("There is no hypnogram to get stats from.")
         stats = sleep_statistics(self.hypno, self.hypno_freq)
         if save:
             with open(
                 self.output_dir / self.__class__.__name__ / "sleep_stats.csv",
                 "w",
                 newline="",
             ) as csv_file:
@@ -444,15 +425,15 @@
             ax=axis,
             **cbar_args,
         )
 
 
 @define(kw_only=True, slots=False)
 class BaseEventPipe(BaseHypnoPipe, BaseTopomap, ABC):
-    """A template class for event detection."""
+    """A base class for event detection."""
 
     results = field(init=False)
     """Event detection results as returned by YASA's event detection methods. 
     Depending on the child class can be instance of either 
     :py:class:`yasa:yasa.SpindlesResults`, :py:class:`yasa:yasa.SWResults` or :py:class:`yasa:yasa.REMResults` classes. 
     """
 
@@ -516,16 +497,16 @@
             axis: Instance of :py:class:`mpl:matplotlib.axes.Axes`.
                 Defaults to None.
             save: Whether to save the figure. Defaults to False.
             topomap_args: Arguments passed to :py:func:`mne:mne.viz.plot_topomap`.Defaults to None.
             cbar_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.colorbar`.Defaults to None.
             subplots_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.subplots`.Defaults to None.
         """
-        from natsort import natsort_keygen
         from more_itertools import collapse
+        from natsort import natsort_keygen
         from seaborn import color_palette
 
         topomap_args = topomap_args or dict()
         cbar_args = cbar_args or dict()
         subplots_args = subplots_args or dict()
         topomap_args.setdefault("cmap", color_palette("rocket_r", as_cmap=True))
         cbar_args.setdefault("label", prop)
@@ -599,16 +580,16 @@
                 Defaults to 95.
             save: Whether to save the figure. Defaults to False.
             topomap_args: Arguments passed to :py:func:`mne:mne.viz.plot_topomap`.Defaults to None.
             cbar_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.colorbar`.Defaults to None.
             figure_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.figure`.Defaults to None.
 
         """
-        from natsort import natsort_keygen
         from more_itertools import collapse
+        from natsort import natsort_keygen
 
         topomap_args = topomap_args or dict()
         cbar_args = cbar_args or dict()
         figure_args = figure_args or dict()
         topomap_args.setdefault("cmap", "plasma")
         topomap_args.setdefault("vlim", [None, None])
 
@@ -687,15 +668,15 @@
                 axes[col_index].set_title(f"{prop}")
             n_spindles = int(
                 self.results.summary(grp_chan=False, grp_stage=True).loc[
                     sleep_stages[stage]
                 ]["Count"]
             )
             subfigs[row_index].suptitle(
-                f"{stage}, {n_spindles} {self.__class__.__name__[:-4].lower()}",
+                f"{stage}, n={n_spindles}",
                 fontsize="xx-large",
             )
 
         fig.suptitle(f"{self.__class__.__name__[:-4]}", fontsize="xx-large")
         if save:
             fig.savefig(
                 self.output_dir
@@ -713,15 +694,15 @@
         method: str = "morlet",
         save: bool = False,
         **tfr_kwargs,
     ):
         """Transforms the events signal to time-frequency representation.
 
         Args:
-            freqs: Lower and upper bounds of frequencies of interest in Hz, e.g., (10,20)
+            freqs: Lower and upper bounds of frequencies of interest in Hz, e.g., (10,20).
             n_freqs: Frequency resolution in TFR.
             time_before: Seconds before the event peak to get from the real data.
             time_after: Seconds after the event peak to get from the real data
             method: TFR transform method. Defaults to "morlet".
             save: Whether to save the TFRs to file. Defaults to False.
             **tfr_kwargs: Arguments passed to :py:func:`mne:mne.time_frequency.tfr_array_morlet`
                 or :py:func:`mne:mne.time_frequency.tfr_array_multitaper`.
@@ -796,15 +777,15 @@
                     for channel, v in tqdm(for_tfrs.items())
                 }
             # Sort and combine
             data = np.squeeze(
                 np.array([tfr for channel, tfr in natsorted(tfrs.items())])
             )
 
-            # Matrix should be 3D, so if there was only one channel need to expand.
+            # Matrix should be 3D, so if there was only one channel - need to expand.
             if data.ndim == 2:
                 data = np.expand_dims(data, axis=0)
             self.tfrs[sleep_stages[stage]] = mne.time_frequency.AverageTFR(
                 info=self.mne_raw.copy().pick(list(tfrs.keys())).info,
                 data=data,
                 times=np.linspace(
                     -time_before,
@@ -838,41 +819,46 @@
         self.tfrs = dict()
         dirpath = (
             Path(dirpath) if dirpath else self.output_dir / self.__class__.__name__
         )
         for p in dirpath.glob("*tfr.h5"):
             m = re.search(r, str(p))
             if m:
-                self.tfrs[m.groups()[0]] = mne.time_frequency.read_tfrs(p)
+                self.tfrs[m.groups()[0]] = mne.time_frequency.read_tfrs(p)[0]
 
 
 @define(kw_only=True, slots=False)
 class SpectrumPlots(BaseTopomap, ABC):
     """Plotting spectral data."""
 
+    psds: dict = field(init=False, factory=dict)
+    """Instances of :class:`.SleepSpectrum` per sleep stage.
+    """
+
     @logger_wraps()
     def plot_psds(
         self,
-        picks,
+        picks: Iterable[str] | str,
         psd_range: tuple = (-40, 60),
         freq_range: tuple = (0, 60),
         dB=True,
         xscale: str = "linear",
         axis: plt.axis = None,
         plot_sensors: bool = False,
         save: bool = False,
         legend_args: dict = None,
         **subplots_kw,
     ):
         """Plot PSD per sleep stage.
 
         Args:
+            picks: Channels to plot PSDs for. Refer to :py:meth:`mne:mne.io.Raw.pick`.
             psd_range: Range of y axis on PSD plot. Defaults to (-40, 60).
             freq_range: Range of x axis on PSD plot. Defaults to (0, 40).
-            dB:
+            dB: Whether transform PSD to dB. Defaults to True.
             xscale: Scale of the X axis, check available values at
                 :py:meth:`mpl:matplotlib.axes.Axes.set_xscale`. Defaults to "linear".
             axis: Instance of :py:class:`mpl:matplotlib.axes.Axes`.
                 Defaults to None.
             plot_sensors: Whether to plot sensor map showing which channels were used for
                 computing PSD. Defaults to False.
             save: Whether to save the figure. Defaults to False.
@@ -893,15 +879,15 @@
             psds = np.mean(
                 spectrum._data[_picks_to_idx(spectrum.info, picks=picks), :], axis=0
             )
             psds = 10 * np.log10(10**12 * psds) if dB else 10**12 * psds
             axis.plot(
                 spectrum._freqs,
                 psds,
-                label=f"{stage} ({spectrum.info.description}%)",
+                label=f"{stage} ({spectrum.info['description']}%)",
             )
 
         axis.set_xlim(freq_range)
         axis.set_ylim(psd_range)
         axis.set_xscale(xscale)
         units = r"$\mu V^{2}/Hz$ (dB)" if dB else r"$\mu V^{2}/Hz$"
         axis.set_ylabel(f"Power ({units})")
@@ -910,34 +896,31 @@
             if xscale == "linear"
             else f"{xscale} frequency [Hz]".capitalize()
         )
         axis.set_xlabel(xlabel)
         axis.legend(**legend_args)
 
         if plot_sensors:
-            from mpl_toolkits.axes_grid1.inset_locator import inset_axes
-            from more_itertools import flatten
             from ast import literal_eval
 
+            from mpl_toolkits.axes_grid1.inset_locator import inset_axes
+
             # color = "cyan"
             axins = inset_axes(axis, width="30%", height="30%", loc="lower left")
             psd_channels = _picks_to_idx(self.mne_raw.info, picks)
 
-            # Parse log to get interpolated channels
+            try:
+                interpolated = literal_eval(self.mne_raw.info["description"])
+            except:
+                interpolated = None
 
-            reg = r"(?:.*) \| (?:.*) \| (?:.*) Interpolated channels: (?P<channels>.*)"
-            interpolated = [
-                literal_eval(e["channels"])
-                for e in logger.parse(self.output_dir / "pipeline.log", reg)
-            ]
             interpolated = (
-                _picks_to_idx(self.mne_raw.info, list(flatten(interpolated)))
-                if interpolated
-                else None
+                _picks_to_idx(self.mne_raw.info, interpolated) if interpolated else None
             )
+
             ch_groups = {
                 k: v
                 for k, v in {"PSD": psd_channels, "Interpolated": interpolated}.items()
                 if v is not None
             }
             self.plot_sensors(
                 legend=list(ch_groups.keys()),
@@ -957,84 +940,67 @@
     @logger_wraps()
     def plot_topomap(
         self,
         stage: str = "REM",
         band: dict = {"Delta": (0, 4)},
         dB: bool = False,
         axis: plt.axis = None,
-        fooof: bool = False,
         save: bool = False,
         topomap_args: dict = None,
         cbar_args: dict = None,
-        fooof_group_args: dict = None,
-        fooof_get_band_peak_fg_args: dict = None,
         subplots_args: dict = None,
     ):
         """Plots topomap for a sleep stage and a frequency band.
 
         Args:
             stage: One of the sleep_stages keys. Defaults to "REM".
             band: Name-value pair - with name=arbitrary name
                 and value=(l_freq, h_freq).
                 Defaults to {"Delta": (0, 4)}.
             dB: Whether transform PSD to dB. Defaults to False.
             axis: Instance of :py:class:`mpl:matplotlib.axes.Axes`.
                 Defaults to None.
-            fooof: Whether to plot parametrised spectra.
-                More at :std:doc:`fooof:auto_examples/analyses/plot_mne_example`.
-                Defaults to False.
             save: Whether to save the figure. Defaults to False.
             topomap_args: Arguments passed to :py:func:`mne:mne.viz.plot_topomap`.Defaults to None.
             cbar_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.colorbar`.Defaults to None.
             subplots_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.subplots`.Defaults to None.
-            fooof_group_args: Arguments passed to :py:class:`fooof:fooof.FOOOFGroup`. Defaults to None.
-            fooof_get_band_peak_fg_args: Arguments passed to the :py:func:`fooof:fooof.analysis.get_band_peak_fg`. Defaults to None.
         """
         topomap_args = topomap_args or dict()
         cbar_args = cbar_args or dict()
         subplots_args = subplots_args or dict()
         topomap_args.setdefault("cmap", "plasma")
         cbar_args.setdefault(
             "label",
-            r"$\mu V^{2}/Hz$ (dB)" if dB else r"$\mu V^{2}/Hz$" if not fooof else None,
+            r"$\mu V^{2}/Hz$ (dB)" if dB else r"$\mu V^{2}/Hz$",
         )
         assert stage in self.psds, f"{stage} is not in self.psds"
 
         is_new_axis = False
 
         if axis is None:
             fig, axis = plt.subplots(**subplots_args)
             is_new_axis = True
 
         [(_, b)] = band.items()
 
-        if fooof:
-            psds = self._fooof(
-                band=band,
-                stage=stage,
-                fooof_group_args=fooof_group_args,
-                get_band_peak_fg_args=fooof_get_band_peak_fg_args,
-            )
-
-        else:
-            psds = (
-                10 * np.log10(10**12 * self.psds[stage]._data)
-                if dB
-                else 10**12 * self.psds[stage]._data
-            )
-            psds = np.take(
-                psds,
-                np.where(
-                    np.logical_and(
-                        self.psds[stage]._freqs >= b[0],
-                        self.psds[stage]._freqs <= b[1],
-                    )
-                )[0],
-                axis=1,
-            ).sum(axis=1)
+        psds = (
+            10 * np.log10(10**12 * self.psds[stage]._data)
+            if dB
+            else 10**12 * self.psds[stage]._data
+        )
+        psds = np.take(
+            psds,
+            np.where(
+                np.logical_and(
+                    self.psds[stage]._freqs >= b[0],
+                    self.psds[stage]._freqs <= b[1],
+                )
+            )[0],
+            axis=1,
+        ).sum(axis=1)
 
         self._plot_topomap(
             data=psds,
             axis=axis,
             topomap_args=topomap_args,
             cbar_args=cbar_args,
         )
@@ -1057,22 +1023,19 @@
             "Theta": (4, 7.99),
             "Alpha": (8, 12.49),
             "SMR": (12.5, 15),
             "Beta": (12.5, 29.99),
             "Gamma": (30, 60),
         },
         dB: bool = False,
-        fooof: bool = False,
         low_percentile: float = 5,
         high_percentile: float = 95,
         save: bool = False,
         topomap_args: dict = None,
         cbar_args: dict = None,
-        fooof_group_args: dict = None,
-        fooof_get_band_peak_fg_args: dict = None,
         figure_args: dict = None,
     ):
         """Plots topomap collage for multiple sleep stages and bands.
 
         Args:
             stages_to_plot: Tuple of strings representing names from sleep_stages,
                 e.g., ("REM", "N1").
@@ -1081,36 +1044,31 @@
             bands: Dict of name-value pairs - with name=arbitrary name
                 and value=(l_freq, h_freq).
                 Defaults to { "Delta": (0, 3.99), "Theta": (4, 7.99), "Alpha": (8, 12.49),
                 "SMR": (12.5, 15), "Beta": (12.5, 29.99), "Gamma": (30, 60), }.
             dB: Whether transform PSD to dB. Defaults to False.
             sleep_stages: Mapping between sleep stages names and their integer representations.
                 Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
-            fooof: Whether to plot parametrised spectra.
-                More at :std:doc:`fooof:auto_examples/analyses/plot_mne_example`.
-                Defaults to False.
             low_percentile: Set min color value by percentile of the band data.
                 Defaults to 5.
             high_percentile: Set max color value by percentile of the band data.
                 Defaults to 95.
             save: Whether to save the figure. Defaults to False.
             topomap_args: Arguments passed to :py:func:`mne:mne.viz.plot_topomap`.Defaults to None.
             cbar_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.colorbar`.Defaults to None.
             figure_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.figure`.Defaults to None.
-            fooof_group_args: Arguments passed to :py:class:`fooof:fooof.FOOOFGroup`. Defaults to None.
-            fooof_get_band_peak_fg_args: Arguments passed to the :py:func:`fooof:fooof.analysis.get_band_peak_fg`. Defaults to None.
         """
         topomap_args = topomap_args or dict()
         cbar_args = cbar_args or dict()
         figure_args = figure_args or dict()
         topomap_args.setdefault("cmap", "plasma")
         topomap_args.setdefault("vlim", [None, None])
         cbar_args.setdefault(
             "label",
-            r"$\mu V^{2}/Hz$ (dB)" if dB else r"$\mu V^{2}/Hz$" if not fooof else None,
+            r"$\mu V^{2}/Hz$ (dB)" if dB else r"$\mu V^{2}/Hz$",
         )
 
         if stages_to_plot == "all":
             stages_to_plot = self.psds.keys()
         n_rows = len(stages_to_plot)
         n_cols = len(bands)
 
@@ -1127,37 +1085,29 @@
 
         psds_per_stage_per_band = np.empty(
             (len(stages_to_plot), len(bands)), dtype=object
         )
         for col_index, (band_key, b) in enumerate(bands.items()):
             for_perc = []
             for row_index, stage in enumerate(self.psds):
-                if fooof:
-                    psds = self._fooof(
-                        band={band_key: b},
-                        stage=stage,
-                        fooof_group_args=fooof_group_args,
-                        get_band_peak_fg_args=fooof_get_band_peak_fg_args,
-                    )
-                else:
-                    psds = (
-                        10 * np.log10(10**12 * self.psds[stage]._data)
-                        if dB
-                        else 10**12 * self.psds[stage]._data
-                    )
-                    psds = np.take(
-                        psds,
-                        np.where(
-                            np.logical_and(
-                                self.psds[stage]._freqs >= b[0],
-                                self.psds[stage]._freqs <= b[1],
-                            )
-                        )[0],
-                        axis=1,
-                    ).sum(axis=1)
+                psds = (
+                    10 * np.log10(10**12 * self.psds[stage]._data)
+                    if dB
+                    else 10**12 * self.psds[stage]._data
+                )
+                psds = np.take(
+                    psds,
+                    np.where(
+                        np.logical_and(
+                            self.psds[stage]._freqs >= b[0],
+                            self.psds[stage]._freqs <= b[1],
+                        )
+                    )[0],
+                    axis=1,
+                ).sum(axis=1)
                 for_perc.append(psds)
                 psds_per_stage_per_band[row_index, col_index] = psds
             if low_percentile:
                 perc_low[band_key] = np.percentile(for_perc, low_percentile)
             if high_percentile:
                 perc_high[band_key] = np.percentile(for_perc, high_percentile)
 
@@ -1177,56 +1127,33 @@
                     cbar_args=cbar_args,
                 )
                 axes[col_index].set_title(
                     f"{band_key} ({bands[band_key][0]}-{bands[band_key][1]} Hz)"
                 )
 
             subfigs[row_index].suptitle(
-                f"{stage} ({self.psds[stage].info.description}%)", fontsize="xx-large"
+                f"{stage} ({self.psds[stage].info['description']}%)",
+                fontsize="xx-large",
             )
 
         if save:
             fig.savefig(
                 self.output_dir / self.__class__.__name__ / f"topomap_psd_collage.png"
             )
 
-    def _fooof(self, band, stage, fooof_group_args=None, get_band_peak_fg_args=None):
-        from fooof import FOOOFGroup
-        from fooof.bands import Bands
-        from fooof.analysis import get_band_peak_fg
-
-        fooof_group_args = fooof_group_args or dict()
-        get_band_peak_fg_args = get_band_peak_fg_args or dict()
-        fooof_group_args.setdefault("peak_width_limits", (1, 6))
-        fooof_group_args.setdefault("min_peak_height", 0.15)
-        fooof_group_args.setdefault("peak_threshold", 2.0)
-        fooof_group_args.setdefault("verbose", False)
-        # Initialize a FOOOFGroup object, with desired settings
-        fg = FOOOFGroup(**fooof_group_args)
-
-        # Define the frequency range to fit
-        freq_range = [1, 45]
-
-        fg.fit(
-            self.psds[stage]._freqs,
-            self.psds[stage]._data,
-            freq_range=freq_range,
-        )
-
-        # Define frequency bands of interest
-        bands = Bands(band)
-
-        # Extract peaks
-        peaks = get_band_peak_fg(fg, bands[list(band)[0]], **get_band_peak_fg_args)
-
-        peaks[np.where(np.isnan(peaks))] = 0
-        # Extract the power values from the detected peaks
-        psds = peaks[:, 1]
+    @logger_wraps()
+    def _save_psds(self, overwrite):
+        import re
 
-        return psds
+        for stage, spectrum in self.psds.items():
+            stage = re.sub(r"[^\w\s-]", "_", stage)
+            spectrum.save(
+                self.output_dir / self.__class__.__name__ / f"{stage}-psd.h5",
+                overwrite=overwrite,
+            )
 
 
 @define(kw_only=True, slots=False)
 class SleepSpectrum(mne.time_frequency.spectrum.BaseSpectrum):
     """Spectral representation of sleep stage data.
 
     Adapted from `MNE <https://mne.tools/stable/index.html>`_.
@@ -1281,49 +1208,54 @@
         del self._shape
         # save memory
         del self.inst
 
     def __add__(self, other):
         if isinstance(other, self.__class__):
             from copy import deepcopy
-            from ast import literal_eval
 
             spectrum_cp = deepcopy(self)
             spectrum_cp._data = np.add(self._data, other._data)
-            descr = literal_eval(self.info.description)
-            spectrum_cp.info.description = str(
-                descr + literal_eval(other.info.description)
-            )
+            try:
+                stage_percent = float(self.info["description"])
+                other_stage_percent = float(other.info["description"])
+                spectrum_cp.info["description"] = str(
+                    stage_percent + other_stage_percent
+                )
+            except:
+                pass
             return spectrum_cp
         else:
             return NotImplemented
 
     def __truediv__(self, other):
         if isinstance(other, (int, float)):
             from copy import deepcopy
-            from ast import literal_eval
 
             spectrum_cp = deepcopy(self)
             spectrum_cp._data = self._data / other
-            spectrum_cp.info.description = str(
-                round(literal_eval(self.info.description) / other, 2)
-            )
+            try:
+                spectrum_cp.info["description"] = str(
+                    round(float(self.info["description"]) / other, 2)
+                )
+            except:
+                pass
             return spectrum_cp
         else:
             return NotImplemented
 
     def _compute_spectra(
         self, method, data, hypno, stage_idx, fmin, fmax, n_jobs, verbose
     ):
         """
         Weighted average for Welch's PSD.
         Average of uniform sample regions for Multitaper's PSD.
         """
-        from scipy import ndimage
         from more_itertools import collapse
+        from scipy import ndimage
 
         n_samples_total = np.count_nonzero(~np.isnan(data), axis=1)[0]
         psds_list = []
         weights = []
         n_samples = 0
         try:
             regions = collapse(
@@ -1372,15 +1304,15 @@
             np.array(psds_list), np.isnan(np.array(psds_list))
         )
         average = np.ma.average(masked_data, weights=weights, axis=0)
         avg_psds = average.filled(np.nan)
 
         self._data = avg_psds
         self._freqs = freqs
-        self.info.description = str(round(n_samples / n_samples_total * 100, 2))
+        self.info["description"] = str(round(n_samples / n_samples_total * 100, 2))
         # this is *expected* shape, it gets asserted later in _check_values()
         # (and then deleted afterwards)
         self._shape = (len(self.ch_names), len(self.freqs))
         # we don't need these anymore, and they make save/load harder
         del self._picks
         del self._psd_func
         del self._time_mask
```

### Comparing `sleepeeg-0.2.3/sleepeeg/dashboard.py` & `sleepeeg-0.3.0/sleepeeg/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 def _init_s_pipe(prec_pipe, path_to_hypnogram, hypno_freq):
     if path_to_hypnogram is None:
         s_pipe = SpectralPipe(
             prec_pipe=prec_pipe,
         )
         s_pipe.hypno = np.zeros(s_pipe.mne_raw.n_times)
         s_pipe.hypno_freq = s_pipe.sf
-        s_pipe._BaseHypnoPipe__upsample_hypno()
+        s_pipe._upsample_hypno()
         sleep_stages = {"All": 0}
     else:
         s_pipe = SpectralPipe(
             prec_pipe=prec_pipe,
             path_to_hypno=path_to_hypnogram,
             hypno_freq=hypno_freq,
         )
@@ -61,15 +61,15 @@
         fmax = lp
     else:
         pipe.filter(l_freq=None, h_freq=fmax, n_jobs=-1)
 
     if fmax > 50:
         pipe.notch(freqs=notch_freqs, n_jobs=-1)
     else:
-        notch_freqs = None
+        notch_freqs = [None]
 
     return sfreq, fmin, fmax, notch_freqs
 
 
 def _hypno_psd(
     s_pipe,
     sleep_stages,
@@ -342,15 +342,15 @@
         (
             f"Recording duration: {recording_time}",
             f"Sampling frequency: {sfreq} Hz",
             f"Bad epochs: {bad_epochs_percent}%",
             f"Interpolated channels: {interpolated_channels_percent}%",
             f"EEG reference: {reference}",
             f"Band-pass filter: [{round(fmin, 2)}, {round(fmax, 2)}] Hz",
-            f"Notch filter: {set(notch_freqs) if notch_freqs else notch_freqs} Hz",
+            f"Notch filter: {set(notch_freqs)} Hz",
             f"ICA performed: {'Yes' if is_ica else 'No'}",
             f"Adaptive topomaps: {'Yes' if is_adaptive_topo else 'No'}",
         )
     )
     info_axes[1].set_axis_off()
     info_axes[1].text(
         0,
```

### Comparing `sleepeeg-0.2.3/sleepeeg/pipeline.py` & `sleepeeg-0.3.0/sleepeeg/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,45 @@
 """This module contains and describes pipe elements for sleep eeg analysis.
 """
 
-from attrs import define, field
-from loguru import logger
-from typing import TypeVar
-from pathlib import Path
-from collections.abc import Iterable
 from collections import defaultdict
+from collections.abc import Iterable
+from pathlib import Path
+from typing import TypeVar
 
-import numpy as np
-import pandas as pd
 import matplotlib.pyplot as plt
 import mne
+import numpy as np
+import pandas as pd
+from attrs import define, field
+from loguru import logger
 
-
-from .base import (
-    BasePipe,
-    BaseHypnoPipe,
-    BaseEventPipe,
-    BaseTopomap,
-    SpectrumPlots,
-    SleepSpectrum,
-    logger_wraps,
-)
+from .base import BaseEventPipe, BaseHypnoPipe, BasePipe, SleepSpectrum, SpectrumPlots
+from .utils import logger_wraps
 
 # For type annotation of pipe elements.
 BasePipeType = TypeVar("BasePipeType", bound="BasePipe")
 
 
 @define(kw_only=True)
 class CleaningPipe(BasePipe):
     """The cleaning pipeline element.
 
     Contains resampling function, band and notch filters,
-    browser for manual selection of bad channels
+    mne browser for manual selection of bad channels
     and bad data spans.
     """
 
     @logger_wraps()
     def resample(self, sfreq: float = 250, save: bool = False, **resample_kwargs):
         """A wrapper for :py:meth:`mne:mne.io.Raw.resample`
-        with an additional option to save the resampled data.
+        with an additional option to save the resampled data to file.
 
         Args:
+            sfreq: Desired new frequency. Defaults to 250.
             save: Whether to save a resampled data to a fif file. Defaults to False.
             **resample_kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.resample`.
         """
         self.mne_raw.resample(sfreq=sfreq, **resample_kwargs)
         if save:
             self.save_raw(
                 "_".join(
@@ -64,23 +57,28 @@
     @logger_wraps()
     def filter(
         self, l_freq: float | None = 0.3, h_freq: float | None = None, **filter_kwargs
     ):
         """A wrapper for :py:meth:`mne:mne.io.Raw.filter`.
 
         Args:
+            l_freq: Lower pass-band edge in Hz. Defaults to 0.3.
+            h_freq: Upper pass-band edge in Hz. Defaults to None.
             **filter_kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.filter`.
         """
         self.mne_raw.load_data().filter(l_freq=l_freq, h_freq=h_freq, **filter_kwargs)
 
     @logger_wraps()
     def notch(self, freqs: str | Iterable[float] = "50s", **notch_kwargs):
         """A wrapper for :py:meth:`mne:mne.io.Raw.notch_filter`.
 
         Args:
+            freqs: Frequencies to notch filter in Hz. Can be either array of floats,
+                or '50s' or '60s' to filter harmonics of 50 and 60 Hz, respectively.
+                Defaults to '50s'.
             **notch_kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.notch_filter`.
         """
         if isinstance(freqs, str):
             if freqs == "50s":
                 freqs = np.arange(50, int(self.sf / 2), 50)
             elif freqs == "60s":
                 freqs = np.arange(50, int(self.sf / 2), 50)
@@ -120,16 +118,25 @@
     @logger_wraps()
     def interpolate_bads(self, **interp_kwargs):
         """A wrapper for :py:meth:`mne:mne.io.Raw.interpolate_bads`
 
         Args:
             **interp_kwargs: Arguments passed to :py:meth:`mne:mne.io.Raw.interpolate_bads`.
         """
+        from ast import literal_eval
+
+        from natsort import natsorted
+
         bads = self.mne_raw.info["bads"]
-        self.mne_raw.interpolate_bads(**interp_kwargs)
+        self.mne_raw.load_data().interpolate_bads(**interp_kwargs)
+        try:
+            old_interp = literal_eval(self.mne_raw.info["description"])
+        except:
+            old_interp = []
+        self.mne_raw.info["description"] = str(natsorted(set(old_interp + bads)))
         logger.info(f"Interpolated channels: {bads}")
 
 
 @define(kw_only=True)
 class ICAPipe(BasePipe):
     """The ICA pipeline element.
 
@@ -168,15 +175,15 @@
                 Additional parameters passed to the ICA estimator as specified by method.
                 Allowed entries are determined by the various algorithm implementations:
                 see `FastICA <https://scikit-learn.org/stable/modules/generated/sklearn.
                 decomposition. FastICA.html#sklearn.decomposition.FastICA>`_,
                 `picard <https://pierreablin.github.io/picard/generated/picard.picard.html#picard.picard>`_ and
                 `infomax <https://mne.tools/stable/generated/mne.preprocessing.infomax.html#mne.preprocessing.infomax>`_.
                 Defaults to None.
-            path_to_ica: Path to the saved -ica.fif file you want to continue work with.
+            path_to_ica: Path to the saved -ica.fif file you want to continue work with. Defaults to None.
             **ica_kwargs: Arguments passed to :py:class:`mne:mne.preprocessing.ICA`.
         """
         if path_to_ica is not None:
             ica = mne.preprocessing.read_ica(path_to_ica)
         else:
             ica = mne.preprocessing.ICA(
                 n_components=n_components,
@@ -192,19 +199,19 @@
                 output_dir=output_dir,
                 mne_ica=ica,
             )
         self.mne_raw.load_data()
 
     @logger_wraps()
     def fit(self, filter_kwargs: dict = None, **fit_kwargs):
-        """Highpass-filters (1 Hz) a copy of the mne_raw object
-        and then runs :py:meth:`mne:mne.preprocessing.ICA.fit`.
+        """High-pass filters (1 Hz) a copy of the mne_raw object
+        and then runs :py:meth:`mne:mne.preprocessing.ICA.fit` on it.
 
         Args:
-            filter_args: Arguments passed to :py:meth:`mne:mne.io.Raw.filter`.
+            filter_args: Arguments passed to :py:meth:`mne:mne.io.Raw.filter`. Defaults to None.
             **fit_kwargs: Arguments passed to :py:meth:`mne:mne.preprocessing.ICA.fit`.
         """
         filter_kwargs = filter_kwargs or dict()
         filter_kwargs.setdefault("l_freq", 1.0)
         filter_kwargs.setdefault("h_freq", None)
         if self.mne_raw.info["highpass"] < 1.0:
             filtered_raw = self.mne_raw.copy()
@@ -250,18 +257,14 @@
 class SpectralPipe(BaseHypnoPipe, SpectrumPlots):
     """The spectral analyses pipeline element.
 
     Contains methods for computing and plotting PSD,
     spectrogram and topomaps per sleep stage.
     """
 
-    psds: dict = field(init=False, factory=dict)
-    """Instances of :class:`.SleepSpectrum` per sleep stage.
-    """
-
     @logger_wraps()
     def compute_psds_per_stage(
         self,
         sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
         reference: Iterable[str] | str | None = None,
         method: str = "welch",
         fmin: float = 0,
@@ -277,25 +280,27 @@
         """For each sleep stage creates a :class:`.SleepSpectrum` object.
 
         Args:
             sleep_stages: Sleep stages mapping in hypnogram.
                 Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
             reference: Which eeg reference to compute PSD with.
                 If None, the reference isn't changed. Defaults to None.
-            method: Spectral estimation method.. Defaults to "welch".
+            method: Spectral estimation method. Defaults to "welch".
             fmin: Lower frequency bound. Defaults to 0.
             fmax: Upper frequency bound. Defaults to 60.
             picks: Channels to compute spectra for. Refer to :py:meth:`mne:mne.io.Raw.pick`.
                 Defaults to "eeg".
             reject_by_annotation: Whether to not use the annotations for the spectra computation.
                 Defaults to True.
             save: Whether to save the spectra in .h5 files. Defaults to False.
             overwrite: Whether to overwrite the file. Defaults to False.
-            n_jobs: _description_. Defaults to -1.
-            verbose: _description_. Defaults to False.
+            n_jobs: The number of jobs to run in parallel. If -1,
+                it is set to the number of CPU cores. Defaults to -1.
+            verbose: Control verbosity of the logging output.
+                If None, use the default verbosity level. Defaults to False.
             **psd_kwargs: Additional arguments passed to :py:func:`mne:mne.time_frequency.psd_array_welch`
                 or :py:func:`mne:mne.time_frequency.psd_array_multitaper`.
         """
         inst = self.mne_raw.copy().load_data()
         if reference is not None:
             inst.set_eeg_reference(ref_channels=reference)
         for stage, stage_idx in sleep_stages.items():
@@ -312,35 +317,29 @@
                 proj=False,
                 reject_by_annotation=reject_by_annotation,
                 n_jobs=n_jobs,
                 verbose=verbose,
                 **psd_kwargs,
             )
         if save:
-            import re
-
-            for stage, spectrum in self.psds.items():
-                stage = re.sub(r"[^\w\s-]", "_", stage)
-                spectrum.save(
-                    self.output_dir / self.__class__.__name__ / f"{stage}-psd.h5",
-                    overwrite=overwrite,
-                )
+            self._save_psds(overwrite)
 
     @logger_wraps()
     def read_spectra(self, dirpath: str | None = None):
         """Loads spectra stored in hdf5 files.
 
         Filenames should end with {sleep_stage}-psd.h5
 
         Args:
             dirpath: Path to the directory containing hdf5 files. Defaults to None.
         """
-        from mne.time_frequency import read_spectrum
-        from pathlib import Path
         import re
+        from pathlib import Path
+
+        from mne.time_frequency import read_spectrum
 
         r = f"(.+)(?:-psd.h5)"
         self.tfrs = dict()
         dirpath = (
             Path(dirpath) if dirpath else self.output_dir / self.__class__.__name__
         )
         for p in dirpath.glob("*psd.h5"):
@@ -348,55 +347,59 @@
             if m:
                 self.psds[m.groups()[0]] = read_spectrum(p)
 
     @logger_wraps()
     def plot_hypnospectrogram(
         self,
         picks: str | Iterable[str] = ("E101",),
-        win_sec: float = 30,
+        win_sec: float = 10,
         trimperc: float = 2.5,
         freq_range: tuple = (0, 40),
         cmap: str = "Spectral_r",
         overlap: bool = False,
         save: bool = False,
         axis: plt.Axes = None,
     ):
         """Plots hypnogram and spectrogram.
 
-        Adapted from yasa.
+        Adapted from YASA.
 
         Args:
             picks: Channels to compute the spectrogram on. Defaults to ("E101",).
-            win_sec: The length of the sliding window, in seconds, used for multitaper PSD calculation. Defaults to 30.
-            trimperc: The amount of data to trim on both ends of the distribution when normalizing the colormap. Defaults to 2.5.
+            win_sec: The length of the sliding window, in seconds, used for multitaper PSD calculation.
+                Defaults to 30.
+            trimperc: The amount of data to trim on both ends of the distribution
+                when normalizing the colormap. Defaults to 2.5.
             freq_range: Range of x axis on spectrogram plot. Defaults to (0, 40).
-            cmap: Matplotlib colormap. :std:doc:`mpl:tutorials/colors/colormaps`. Defaults to "Spectral_r".
-            overlap: Whether to plot hypnogram over the spectrogram or on top of it. Defaults to False.
+            cmap: Matplotlib colormap. :std:doc:`mpl:tutorials/colors/colormaps`.
+                Defaults to "Spectral_r".
+            overlap: Whether to plot hypnogram over the spectrogram or on top of it.
+                Defaults to False.
             save: Whether to save the figure. Defaults to False.
             axis: Instance of :py:class:`mpl:matplotlib.axes.Axes`.
                 Defaults to None.
         """
         # Import data from the raw mne file.
         data = self.mne_raw.get_data(picks, units="uV", reject_by_annotation="NaN")[0]
         # Create a plot figure
-        if overlap or not self.hypno_up.any():
+        if overlap or self.hypno_up is None:
             if axis is None:
                 fig, axis = plt.subplots(nrows=1, figsize=(12, 4))
 
             im = self.__plot_spectrogram(
                 data,
                 self.sf,
                 win_sec,
                 freq_range[0],
                 freq_range[1],
                 trimperc,
                 cmap,
                 axis,
             )
-            if self.hypno_up.any():
+            if self.hypno_up is not None:
                 ax_hypno = axis.twinx()
                 self.__plot_hypnogram(self.sf, self.hypno_up, ax_hypno)
             # Add colorbar
             cbar = plt.colorbar(im, ax=axis, shrink=0.95, fraction=0.1, aspect=25)
             cbar.ax.set_ylabel(r"$\mu V^{2}/Hz$ (dB)", rotation=90)
             return None if axis is not None else fig
         else:
@@ -405,15 +408,15 @@
                     nrows=2, figsize=(12, 6), gridspec_kw={"height_ratios": [1, 2]}
                 )
                 plt.subplots_adjust(hspace=0.1)
             else:
                 ax0 = axis[0]
                 ax1 = axis[1]
 
-            if self.hypno_up.any():
+            if self.hypno_up is not None:
                 # Hypnogram (top axis)
                 self.__plot_hypnogram(self.sf, self.hypno_up, ax0)
             # Spectrogram (bottom axis)
             self.__plot_spectrogram(
                 data,
                 self.sf,
                 win_sec,
@@ -469,17 +472,17 @@
         ax0.spines["right"].set_visible(False)
         ax0.spines["top"].set_visible(False)
         return ax0
 
     @staticmethod
     def __plot_spectrogram(data, sf, win_sec, fmin, fmax, trimperc, cmap, ax):
         """Adapted from :py:func:`yasa:yasa.plot_spectrogram`."""
-        from matplotlib.colors import Normalize
-        from lspopt import spectrogram_lspopt
         import numpy as np
+        from lspopt import spectrogram_lspopt
+        from matplotlib.colors import Normalize
 
         # Calculate multi-taper spectrogram
         nperseg = int(win_sec * sf)
         f, t, Sxx = spectrogram_lspopt(data, sf, nperseg=nperseg, noverlap=0)
         Sxx = 10 * np.log10(
             Sxx, out=np.full(Sxx.shape, np.nan), where=(Sxx != 0)
         )  # Convert uV^2 / Hz --> dB / Hz
@@ -639,42 +642,37 @@
     def plot_topomap_collage(self):
         raise AttributeError(
             "'RapidEyeMovementsPipe' object has no attribute 'plot_topomap'"
         )
 
 
 @define(kw_only=True)
-class GrandPipe(SpectrumPlots, BaseTopomap):
+class GrandSpectralPipe(SpectrumPlots):
     """The pipeline element combining results from multiple subjects.
 
     Contains methods for computing and plotting combined PSD,
     spectrogram and topomaps, per sleep stage.
     """
 
+    pipes: Iterable[SpectralPipe] = field()
+    """Stores SpectralPipes for multiple subjects.
+    """
+
     output_dir: Path = field(converter=Path)
     """Path to the directory where the output will be saved."""
 
     @output_dir.validator
     def _validate_output_dir(self, attr, value):
         self.output_dir.mkdir(exist_ok=True)
         (self.output_dir / self.__class__.__name__).mkdir(exist_ok=True)
         logger.remove()
         logger.add(self.output_dir / "pipeline.log")
 
-    psds: dict = field(init=False, factory=dict)
-    """Instances of :class:`.SleepSpectrum` per sleep stage.
-    """
-
-    pipes: Iterable[BaseHypnoPipe] = field()
-    """Stores pipeline elements for multiple subjects.
-    """
-
     mne_raw: mne.io.Raw = field(init=False)
-
-    detection_results = field(init=False, factory=lambda: defaultdict(pd.DataFrame))
+    """Representative raw object to infer montage"""
 
     @mne_raw.default
     def _get_mne_raw_from_pipe(self):
         return self.pipes[0].mne_raw
 
     @logger_wraps()
     def compute_psds_per_stage(
@@ -712,179 +710,29 @@
             n_jobs: _description_. Defaults to -1.
             verbose: _description_. Defaults to False.
             **psd_kwargs: Additional arguments passed to :py:func:`mne:mne.time_frequency.psd_array_welch`
                 or :py:func:`mne:mne.time_frequency.psd_array_multitaper`.
         """
 
         avg_func = np.median if average == "median" else np.mean
-        psds = defaultdict(list)
         for pipe in self.pipes:
-            inst = pipe.mne_raw.copy().load_data()
-            if reference is not None:
-                inst.set_eeg_reference(ref_channels=reference)
-            for stage, stage_idx in sleep_stages.items():
-                psds[stage].append(
-                    SleepSpectrum(
-                        inst,
-                        hypno=pipe.hypno_up,
-                        stage_idx=stage_idx,
-                        method=method,
-                        fmin=fmin,
-                        fmax=fmax,
-                        tmin=None,
-                        tmax=None,
-                        picks=picks,
-                        proj=False,
-                        reject_by_annotation=reject_by_annotation,
-                        n_jobs=n_jobs,
-                        verbose=verbose,
-                        **psd_kwargs,
-                    )
-                )
-
-        for stage, spectra in psds.items():
-            self.psds[stage] = avg_func(spectra, axis=0)
-
-        if save:
-            import re
-
-            for stage, spectrum in self.psds.items():
-                stage = re.sub(r"[^\w\s-]", "_", stage)
-                spectrum.save(
-                    self.output_dir / self.__class__.__name__ / f"{stage}-psd.h5",
-                    overwrite=overwrite,
-                )
-
-    @logger_wraps()
-    def spindles_detect(
-        self,
-        picks: str | Iterable[str] = ("eeg"),
-        reference: Iterable[str] | str = "average",
-        include: Iterable[int] = (1, 2, 3),
-        freq_sp: Iterable[float] = (12, 15),
-        freq_broad: Iterable[float] = (1, 30),
-        duration: Iterable[float] = (0.5, 2),
-        min_distance: int = 500,
-        thresh: dict = {"corr": 0.65, "rel_pow": 0.2, "rms": 1.5},
-        multi_only: bool = False,
-        remove_outliers: bool = False,
-        average: str = "mean",
-        verbose: bool = False,
-        save: bool = False,
-        get_sync_events_args=None,
-    ):
-        """A wrapper around :py:func:`yasa:yasa.spindles_detect` with option to save."""
-        from yasa import spindles_detect
-
-        get_sync_events_args = get_sync_events_args or dict()
-        for pipe_index, pipe in enumerate(self.pipes):
-            inst = pipe.mne_raw.copy().load_data()
-            if reference is not None:
-                inst.set_eeg_reference(ref_channels=reference)
-            detection_results = spindles_detect(
-                data=inst.pick(picks),
-                hypno=pipe.hypno_up,
+            pipe.compute_psds_per_stage(
+                sleep_stages=sleep_stages,
+                reference=reference,
+                method=method,
+                fmin=fmin,
+                fmax=fmax,
+                picks=picks,
+                reject_by_annotation=reject_by_annotation,
+                save=False,
+                overwrite=overwrite,
+                n_jobs=n_jobs,
                 verbose=verbose,
-                include=include,
-                freq_sp=freq_sp,
-                freq_broad=freq_broad,
-                duration=duration,
-                min_distance=min_distance,
-                thresh=thresh,
-                multi_only=multi_only,
-                remove_outliers=remove_outliers,
-            )
-            self.detection_results["summary"] = pd.concat(
-                [self.detection_results["summary"], detection_results.summary()]
-            )
-            events_signal = detection_results.get_sync_events()
-            events_signal["pipe_index"] = pipe_index
-            self.detection_results["events"] = pd.concat(
-                [self.detection_results["events"], events_signal]
+                **psd_kwargs,
             )
-        if save:
-            self._save_to_csv()
 
-    @logger_wraps()
-    def plot_topomap(
-        self,
-        prop: str,
-        stage: str = "N2",
-        aggfunc: str = "mean",
-        sleep_stages: dict = {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4},
-        axis: plt.axis = None,
-        save: bool = False,
-        topomap_args: dict = None,
-        cbar_args: dict = None,
-        subplots_args: dict = None,
-    ):
-        """Plots topomap for a sleep stage and some property of detected events.
-
-        Args:
-            prop: Any event property returned by self.results.summary().
-            stage: One of the sleep_stages keys. Defaults to "N2".
-            aggfunc: Averaging function, "mean" or "median". Defaults to "mean".
-            sleep_stages: Mapping between sleep stages names and their integer representations.
-                Defaults to {"Wake": 0, "N1": 1, "N2": 2, "N3": 3, "REM": 4}.
-            axis: Instance of :py:class:`mpl:matplotlib.axes.Axes`.
-                Defaults to None.
-            save: Whether to save the figure. Defaults to False.
-            topomap_args: Arguments passed to :py:func:`mne:mne.viz.plot_topomap`.Defaults to None.
-            cbar_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.colorbar`.Defaults to None.
-            subplots_args: Arguments passed to :py:func:`mpl:matplotlib.pyplot.subplots`.Defaults to None.
-        """
-        from natsort import natsort_keygen
-        from more_itertools import collapse
-        from seaborn import color_palette
-
-        topomap_args = topomap_args or dict()
-        cbar_args = cbar_args or dict()
-        subplots_args = subplots_args or dict()
-        topomap_args.setdefault("cmap", color_palette("rocket_r", as_cmap=True))
-        cbar_args.setdefault("label", prop)
-
-        grouped_summary = self.detection_results["summary"].groupby(
-            ["Channel", "Stage"]
-        )
-        grouped_summary = (
-            grouped_summary.mean() if aggfunc == "mean" else grouped_summary.median()
-        )
-        grouped_summary = grouped_summary.sort_values(
-            "Channel", key=natsort_keygen()
-        ).reset_index()
-
-        assert np.isin(
-            sleep_stages[stage], grouped_summary["Stage"].unique()
-        ).all(), "No such stage in the detected events, was it included in the detect method?"
-
-        is_new_axis = False
-        if not axis:
-            fig, axis = plt.subplots(**subplots_args)
-            is_new_axis = True
-
-        per_stage = grouped_summary.loc[
-            grouped_summary["Stage"].isin(collapse([sleep_stages[stage]]))
-        ].groupby("Channel")
-        per_stage = per_stage.mean() if aggfunc == "mean" else per_stage.median()
-        per_stage = per_stage.sort_values("Channel", key=natsort_keygen()).reset_index()
-
-        info = self.mne_raw.copy().pick(list(per_stage["Channel"].unique())).info
-
-        topomap_args.setdefault("vlim", (per_stage[prop].min(), per_stage[prop].max()))
-        self._plot_topomap(
-            data=per_stage[prop],
-            axis=axis,
-            info=info,
-            topomap_args=topomap_args,
-            cbar_args=cbar_args,
-        )
-        if is_new_axis:
-            fig.suptitle(f"{stage} {self.__class__.__name__[:-4]} ({prop})")
-        if save and is_new_axis:
-            fig.savefig(
-                self.output_dir
-                / self.__class__.__name__
-                / f"topomap_{self.__class__.__name__[:-4].lower()}_{prop.lower()}.png"
-            )
+        for stage in sleep_stages:
+            spectra = [pipe.psds[stage] for pipe in self.pipes]
+            self.psds[stage] = avg_func(spectra, axis=0)
 
-    def detect(self):
-        raise AttributeError("'GrandPipe' object has no attribute 'detect'")
+        if save:
+            self._save_psds(overwrite)
```

### Comparing `sleepeeg-0.2.3/sleepeeg.egg-info/PKG-INFO` & `sleepeeg-0.3.0/sleepeeg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepeeg
-Version: 0.2.3
+Version: 0.3.0
 Summary: Sleep EEG preprocessing and analysis
 Author-email: Gennadiy Belonosov <gennadiyb@mail.tau.ac.il>
 License: MIT
 Project-URL: Homepage, https://github.com/NirLab-TAU/sleepeeg
 Project-URL: Documentation, https://nirlab-tau.github.io/sleepeeg/
 Keywords: sleep,eeg
 Requires-Python: >=3.10
```

