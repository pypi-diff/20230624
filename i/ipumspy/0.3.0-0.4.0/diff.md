# Comparing `tmp/ipumspy-0.3.0.tar.gz` & `tmp/ipumspy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipumspy-0.3.0.tar", max compression
+gzip compressed data, was "ipumspy-0.4.0.tar", max compression
```

## Comparing `ipumspy-0.3.0.tar` & `ipumspy-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
--rw-r--r--   0        0        0    16725 2023-03-02 23:47:57.339161 ipumspy-0.3.0/LICENSE
--rw-r--r--   0        0        0     1875 2023-04-09 00:12:02.422109 ipumspy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       96 2023-03-06 22:01:08.975231 ipumspy-0.3.0/src/ipumspy/__init__.py
--rw-r--r--   0        0        0      184 2023-03-06 17:17:16.405993 ipumspy-0.3.0/src/ipumspy/__version__.py
--rw-r--r--   0        0        0      119 2023-03-06 22:01:08.975231 ipumspy-0.3.0/src/ipumspy/api/__init__.py
--rw-r--r--   0        0        0    21466 2023-04-09 00:12:02.422109 ipumspy-0.3.0/src/ipumspy/api/core.py
--rw-r--r--   0        0        0     1108 2023-03-02 23:47:57.349161 ipumspy-0.3.0/src/ipumspy/api/exceptions.py
--rw-r--r--   0        0        0    25203 2023-04-09 00:12:02.422109 ipumspy-0.3.0/src/ipumspy/api/extract.py
--rw-r--r--   0        0        0     8789 2023-03-27 14:03:52.671184 ipumspy-0.3.0/src/ipumspy/cli.py
--rw-r--r--   0        0        0    14371 2023-04-09 00:12:02.422109 ipumspy-0.3.0/src/ipumspy/ddi.py
--rw-r--r--   0        0        0     6009 2023-03-02 23:47:57.349161 ipumspy-0.3.0/src/ipumspy/fileutils.py
--rw-r--r--   0        0        0    17330 2023-04-09 00:12:02.422109 ipumspy-0.3.0/src/ipumspy/readers.py
--rw-r--r--   0        0        0      348 2023-03-02 23:47:57.349161 ipumspy-0.3.0/src/ipumspy/types.py
--rw-r--r--   0        0        0     1236 2023-04-09 00:12:02.422109 ipumspy-0.3.0/src/ipumspy/utilities.py
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 ipumspy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-03-02 23:47:57.339161 ipumspy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1875 2023-06-24 21:04:23.345033 ipumspy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-03-06 22:01:08.975231 ipumspy-0.4.0/src/ipumspy/__init__.py
+-rw-r--r--   0        0        0      184 2023-03-06 17:17:16.405993 ipumspy-0.4.0/src/ipumspy/__version__.py
+-rw-r--r--   0        0        0      119 2023-03-06 22:01:08.975231 ipumspy-0.4.0/src/ipumspy/api/__init__.py
+-rw-r--r--   0        0        0    21466 2023-04-09 00:12:02.422109 ipumspy-0.4.0/src/ipumspy/api/core.py
+-rw-r--r--   0        0        0     1108 2023-03-02 23:47:57.349161 ipumspy-0.4.0/src/ipumspy/api/exceptions.py
+-rw-r--r--   0        0        0    25203 2023-04-09 00:12:02.422109 ipumspy-0.4.0/src/ipumspy/api/extract.py
+-rw-r--r--   0        0        0     8789 2023-03-27 14:03:52.671184 ipumspy-0.4.0/src/ipumspy/cli.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:23:19.621594 ipumspy-0.4.0/src/ipumspy/data/__init__.py
+-rw-r--r--   0        0        0    19106 2023-06-24 20:23:19.621594 ipumspy-0.4.0/src/ipumspy/data/nyts.yml.gz
+-rw-r--r--   0        0        0    15040 2023-06-24 20:23:19.621594 ipumspy-0.4.0/src/ipumspy/data/yrbss.yml.gz
+-rw-r--r--   0        0        0    14372 2023-06-24 20:23:19.621594 ipumspy-0.4.0/src/ipumspy/ddi.py
+-rw-r--r--   0        0        0     6009 2023-03-02 23:47:57.349161 ipumspy-0.4.0/src/ipumspy/fileutils.py
+-rw-r--r--   0        0        0     4073 2023-06-24 20:23:19.621594 ipumspy-0.4.0/src/ipumspy/noextract.py
+-rw-r--r--   0        0        0    17990 2023-06-24 21:04:23.345033 ipumspy-0.4.0/src/ipumspy/readers.py
+-rw-r--r--   0        0        0      348 2023-03-02 23:47:57.349161 ipumspy-0.4.0/src/ipumspy/types.py
+-rw-r--r--   0        0        0     1236 2023-04-09 00:12:02.422109 ipumspy-0.4.0/src/ipumspy/utilities.py
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 ipumspy-0.4.0/PKG-INFO
```

### Comparing `ipumspy-0.3.0/LICENSE` & `ipumspy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipumspy-0.3.0/pyproject.toml` & `ipumspy-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipumspy"
-version = "0.3.0"
+version = "0.4.0"
 description = "A collection of tools for working with IPUMS data"
 authors = ["Kevin H. Wilson <kevin_wilson@brown.edu>",
            "Renae Rodgers <rodge103@umn.edu>"]
 license = "Mozilla Public License 2.0 (MPL 2.0)"
 packages = [
     { include = "ipumspy", from = "src" }
 ]
```

### Comparing `ipumspy-0.3.0/src/ipumspy/api/core.py` & `ipumspy-0.4.0/src/ipumspy/api/core.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.3.0/src/ipumspy/api/exceptions.py` & `ipumspy-0.4.0/src/ipumspy/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.3.0/src/ipumspy/api/extract.py` & `ipumspy-0.4.0/src/ipumspy/api/extract.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.3.0/src/ipumspy/cli.py` & `ipumspy-0.4.0/src/ipumspy/cli.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.3.0/src/ipumspy/ddi.py` & `ipumspy-0.4.0/src/ipumspy/ddi.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """
 Utilities for working with IPUMS DDI formats
 """
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Literal, Optional, Union
 from xml.etree import ElementTree as ET
 from xml.etree.ElementTree import Element
 
 import numpy as np
 import pandas as pd
 
 
@@ -161,20 +161,19 @@
     that from the XML.
     """
 
     filename: str
     """IPUMS extract ddi file name"""
     description: str
     """IPUMS ddi file description"""
-    structure: str
+    structure: Literal["rectangular", "hierarchical"]
     """
     IPUMS extract data file structure.
-    Valid structures: rectangular, hierarchical
     """
-    rectypes: List
+    rectypes: List[str]
     """
     Record types included in the IPUMS extract.
     This is an empty list for rectangular extracts.
     """
     rectype_idvar: str
     """
     The variable that identifies record types.
```

### Comparing `ipumspy-0.3.0/src/ipumspy/fileutils.py` & `ipumspy-0.4.0/src/ipumspy/fileutils.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.3.0/src/ipumspy/readers.py` & `ipumspy-0.4.0/src/ipumspy/readers.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from pathlib import Path
 from typing import Iterator, List, Optional, Union, Dict
 
 import pandas as pd
 import numpy as np
 import yaml
 
+from ipumspy import noextract
+
 from . import ddi as ddi_definitions
 from . import fileutils
 from .fileutils import open_or_yield
 from .types import FilenameType
 
 
 class CitationWarning(Warning):
@@ -148,87 +150,64 @@
         if not iterator:
             data = [reader(infile, **kwargs)]
         else:
             kwargs.update({"iterator": True, "chunksize": chunksize})
             data = reader(infile, **kwargs)
 
         if dtype is None:
-            yield from (
-                _fix_decimal_expansion(df).astype(
-                    {desc.name: desc.pandas_type for desc in data_description}
-                )
-                for df in data
-            )
+            dtype = {desc.name: desc.pandas_type for desc in data_description}
+            # NOTE(khw): The following line is for specifically handling YRBSS data,
+            # which uses a different .dat format from all other files. This should
+            # be resolved in the future by offering a `.parquet` version of the file
+            # NOTE(rr): Looking at the codebook, I don't _think_ there are similar variables
+            # in the NYTS data.
+            if ddi.ipums_collection == "yrbss":
+                for col in dtype:
+                    if any(name in col for name in ["WEIGHT", "BMIPCTILE"]):
+                        dtype[col] = pd.Float64Dtype()
+            yield from (_fix_decimal_expansion(df).astype(dtype) for df in data)
         else:
             if ".dat" in filename.suffixes:
                 # convert variables from default numpy_type to corresponding type in dtype.
                 yield from (_fix_decimal_expansion(df).astype(dtype) for df in data)
             else:
                 # In contrary to counter condition, df already has right dtype. It would be expensive to call astype for
                 # nothing.
                 yield from (_fix_decimal_expansion(df) for df in data)
 
 
-def _read_hierarchical_microdata(
-    ddi: ddi_definitions.Codebook,
-    filename: Optional[fileutils.FileType] = None,
-    encoding: Optional[str] = None,
-    subset: Optional[List[str]] = None,
-    iterator: bool = False,
-    chunksize: Optional[int] = 100000,
-    dtype: Optional[dict] = None,
-    **kwargs,
-):
-    # TODO: try and speed this up
-    if subset is not None:
-        data_description = [
-            desc for desc in ddi.data_description if desc.name in subset
-        ]
-    else:
-        data_description = ddi.data_description
-
+def _get_common_vars(ddi: ddi_definitions.Codebook, data_description: List):
     # identify common variables
     # these variables have all rectypes listed in the variable-level rectype attribute
     # these are delimited by spaces within the string attribute
     # this list would probably be a useful thing to have as a file-level attribute...
     common_vars = [
         desc.name
         for desc in data_description
         if sorted(desc.rectype.split(" ")) == sorted(ddi.file_description.rectypes)
     ]
-    # seperate variables by rectype
-    rectypes = {}
+    return common_vars
+
+
+def _get_rectype_vars(
+    ddi: ddi_definitions.Codebook,
+    rectype: str,
+    common_vars: List,
+    data_description: List,
+):
     # NB: This might result in empty data frames for some rectypes
     # as the ddi contains all possible collection rectypes, even if only a few
     # are actually represented in the file.
     # TODO: prune empty rectype data frames
-    for rectype in ddi.file_description.rectypes:
-        rectype_vars = []
-        rectype_vars.extend(common_vars)
-        for desc in data_description:
-            if desc.rectype == rectype:
-                rectype_vars.append(desc.name)
-        # read microdata for the relevant rectype variables only
-        # and do it in chunks so it goes quicker
-        rectypes[rectype] = next(
-            read_microdata_chunked(
-                ddi,
-                filename,
-                encoding,
-                # rectype vars are the subset
-                rectype_vars,
-                chunksize,
-                dtype,
-                **kwargs,
-            )
-        )
-        # retain only records from the relevant record type
-        rt_df = rectypes[rectype]
-        rectypes[rectype] = rt_df[rt_df["RECTYPE"] == rectype]
-    return rectypes
+    rectype_vars = []
+    rectype_vars.extend(common_vars)
+    for desc in data_description:
+        if desc.rectype == rectype:
+            rectype_vars.append(desc.name)
+    return rectype_vars
 
 
 def read_microdata(
     ddi: ddi_definitions.Codebook,
     filename: Optional[fileutils.FileType] = None,
     encoding: Optional[str] = None,
     subset: Optional[List[str]] = None,
@@ -307,39 +286,62 @@
             type in the extract data file. Set to True to recieve a dictionary of data frames.
         kwargs: keyword args to be passed to the engine (pd.read_fwf, pd.read_csv, or
             pd.read_parquet depending on the file type)
 
     Returns:
         pandas data frame or a dictionary of pandas data frames
     """
-    # hack for now just to have it in this method - make this a ddi.file_description attribute.
-    common_vars = [
-        desc.name
-        for desc in ddi.data_description
-        if sorted(desc.rectype.split(" ")) == sorted(ddi.file_description.rectypes)
-    ]
     # RECTYPE must be included if subset list is specified
-    if subset is not None and "RECTYPE" not in subset:
-        raise ValueError(
-            "RECTYPE must be included in the subset list for hierarchical extracts."
-        )
+    if subset is not None:
+        if "RECTYPE" not in subset:
+            raise ValueError(
+                "RECTYPE must be included in the subset list for hierarchical extracts."
+            )
+        else:
+            data_description = [
+                desc for desc in ddi.data_description if desc.name in subset
+            ]
+    else:
+        data_description = ddi.data_description
+
     # raise a warning if this is a rectantgular file
     if ddi.file_description.structure == "rectangular":
         raise NotImplementedError(
             "Structure must be hierarchical. Use `read_microdata()` for rectangular extracts."
         )
     else:
-        df_dict = _read_hierarchical_microdata(
-            ddi, filename, encoding, subset, dtype, **kwargs
-        )
+        df_dict = {}
+        common_vars = _get_common_vars(ddi, data_description)
+        for rectype in ddi.file_description.rectypes:
+            rectype_vars = _get_rectype_vars(
+                ddi, rectype, common_vars, data_description
+            )
+            # it feels like there should be a better way to do this bit...
+            rectype_df = pd.concat(
+                [
+                    df
+                    for df in _read_microdata(
+                        ddi, filename, encoding, rectype_vars, dtype, **kwargs
+                    )
+                ]
+            )
+            # filter out non-relevant rectype records
+            df_dict[rectype] = rectype_df[rectype_df["RECTYPE"] == rectype]
         if as_dict:
             return df_dict
         else:
             # read the hierarchical file
-            df = next(_read_microdata(ddi, filename, encoding, subset, dtype, **kwargs))
+            df = pd.concat(
+                [
+                    df
+                    for df in _read_microdata(
+                        ddi, filename, encoding, subset, dtype, **kwargs
+                    )
+                ]
+            )
             # for each rectype, nullify variables that belong to other rectypes
             for rectype in df_dict.keys():
                 # create a list of variables that are for rectypes other than the current rectype
                 # and are not included in the list of varaibles that are common across rectypes
                 non_rt_cols = [
                     cols
                     for rt in df_dict.keys()
@@ -375,19 +377,26 @@
     dtype: Optional[dict] = None,
     **kwargs,
 ) -> Iterator[pd.DataFrame]:
     """
     Read in microdata in chunks as specified by the Codebook.
     As these files are often large, you may wish to filter or read in chunks.
     As an example of how you might do that, consider the following example that
-    filters only for rows in Rhode Island::
+    filters only for rows in Rhode Island:
 
         iter_microdata = read_microdata_chunked(ddi, chunksize=1000)
         df = pd.concat([df[df['STATEFIP'] == 44]] for df in iter_microdata])
 
+    This method also works for large hierarchical files. When reading these files
+    in chunks, users will want to be sure to filter on the RECTYPE variable. For example,
+    the code below reads in only household records in Rhode Island:
+
+        iter_microdata = read_microdata_chunked(ddi, chunksize=1000)
+        df = pd.concat([df[(df['RECTYPE'] == 'H') & (df['STATEFIP'] == 44)] for df in iter_microdata])
+
     Args:
         ddi: The codebook representing the data
         filename: The path to the data file. If not present, gets from
                      ddi and assumes the file is relative to the current working directory
         encoding: The encoding of the data file. If not present, reads from ddi
         subset: A list of variable names to keep. If None, will keep all
         dtype: A dictionary with variable names as keys and variable types as values.
```

### Comparing `ipumspy-0.3.0/src/ipumspy/utilities.py` & `ipumspy-0.4.0/src/ipumspy/utilities.py`

 * *Files identical despite different names*

### Comparing `ipumspy-0.3.0/PKG-INFO` & `ipumspy-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipumspy
-Version: 0.3.0
+Version: 0.4.0
 Summary: A collection of tools for working with IPUMS data
 License: Mozilla Public License 2.0 (MPL 2.0)
 Author: Kevin H. Wilson
 Author-email: kevin_wilson@brown.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

