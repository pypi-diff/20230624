# Comparing `tmp/bisque_metadoc-0.6.3.26-py3-none-any.whl.zip` & `tmp/bisque_metadoc-0.6.3.27-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10818 bytes, number of entries: 11
--rw-r--r--  2.0 unx      167 b- defN 23-Jun-14 22:06 bq/__init__.py
--rw-r--r--  2.0 unx       73 b- defN 23-Jun-14 22:06 bq/metadoc/__init__.py
--rw-r--r--  2.0 unx     2467 b- defN 23-Jun-14 22:06 bq/metadoc/etree.py
--rw-r--r--  2.0 unx    24272 b- defN 23-Jun-14 22:06 bq/metadoc/formats.py
--rw-r--r--  2.0 unx     1020 b- defN 23-Jun-14 22:06 bq/metadoc/logging.py
--rw-r--r--  2.0 unx      167 b- defN 23-Jun-14 22:07 bq/metadoc/version.py
--rw-r--r--  2.0 unx     4486 b- defN 23-Jun-14 22:06 bq/metadoc/xmldict.py
--rw-r--r--  2.0 unx      641 b- defN 23-Jun-14 22:07 bisque_metadoc-0.6.3.26.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-14 22:07 bisque_metadoc-0.6.3.26.dist-info/WHEEL
--rw-r--r--  2.0 unx        3 b- defN 23-Jun-14 22:07 bisque_metadoc-0.6.3.26.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      871 b- defN 23-Jun-14 22:07 bisque_metadoc-0.6.3.26.dist-info/RECORD
-11 files, 34259 bytes uncompressed, 9346 bytes compressed:  72.7%
+Zip file size: 10843 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-23 22:57 bq/__init__.py
+-rw-r--r--  2.0 unx       73 b- defN 23-Jun-23 22:57 bq/metadoc/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 23-Jun-23 22:57 bq/metadoc/etree.py
+-rw-r--r--  2.0 unx    24373 b- defN 23-Jun-23 22:57 bq/metadoc/formats.py
+-rw-r--r--  2.0 unx     1020 b- defN 23-Jun-23 22:57 bq/metadoc/logging.py
+-rw-r--r--  2.0 unx      167 b- defN 23-Jun-23 22:57 bq/metadoc/version.py
+-rw-r--r--  2.0 unx     4486 b- defN 23-Jun-23 22:57 bq/metadoc/xmldict.py
+-rw-r--r--  2.0 unx      641 b- defN 23-Jun-23 22:57 bisque_metadoc-0.6.3.27.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 22:57 bisque_metadoc-0.6.3.27.dist-info/WHEEL
+-rw-r--r--  2.0 unx        3 b- defN 23-Jun-23 22:57 bisque_metadoc-0.6.3.27.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      871 b- defN 23-Jun-23 22:57 bisque_metadoc-0.6.3.27.dist-info/RECORD
+11 files, 34393 bytes uncompressed, 9371 bytes compressed:  72.8%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: bq/metadoc/version.py
 Comment: 
 
 Filename: bq/metadoc/xmldict.py
 Comment: 
 
-Filename: bisque_metadoc-0.6.3.26.dist-info/METADATA
+Filename: bisque_metadoc-0.6.3.27.dist-info/METADATA
 Comment: 
 
-Filename: bisque_metadoc-0.6.3.26.dist-info/WHEEL
+Filename: bisque_metadoc-0.6.3.27.dist-info/WHEEL
 Comment: 
 
-Filename: bisque_metadoc-0.6.3.26.dist-info/top_level.txt
+Filename: bisque_metadoc-0.6.3.27.dist-info/top_level.txt
 Comment: 
 
-Filename: bisque_metadoc-0.6.3.26.dist-info/RECORD
+Filename: bisque_metadoc-0.6.3.27.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bq/metadoc/etree.py

```diff
@@ -68,23 +68,23 @@
     def Element(tag, **kw):
         return Metadoc(tag=tag, **kw)
 
     def SubElement(node, tag, **kw):
         return node.add_tag(tag, **kw)
 
     def fromstring(s):
-        return Metadoc.deserialize(s)
+        return Metadoc.from_etree_like_string(s)
 
     def parse(f):
-        return ElementTree(Metadoc.deserialize(f))
+        return ElementTree(Metadoc.from_etree_like_string(f))
 
     XML = fromstring
 
     def tostring(xml, **kw):
-        return xml.serialize()
+        return xml.to_etree_like_string()
 
     class ElementMaker:
         def __call__(self, tag, *children, **attr):
             res = Metadoc(tag=tag, **attr)
             for kid in children:
                 res.add_child(kid)
             return res
```

## bq/metadoc/formats.py

```diff
@@ -664,33 +664,36 @@
         self.node.extend(kid.node for kid in newchildren)
 
     def iter(self, tag=None):
         for node in self.node.iter(tag=tag):
             yield Metadoc(et=node)
 
     @staticmethod
-    def deserialize(s):
+    def from_etree_like_string(s):
         res = anyxml_to_etree(s)
         # fix any escaped empty strings
         for kid in res.iter(tag=etree.Element):
             if kid.attrib.get("value") == "":
                 del kid.attrib["value"]
                 kid.text = ""
         return Metadoc(et=res)
 
-    def serialize(self):
+    def to_etree_like_string(self):
         # escape any empty strings (XML is not round-tripable for empty strings in text nodes!)
         return _tostring_fix_empty(self.node, encoding="unicode")
 
+    deserialize = from_tagxml
+    serialize = to_tagxml
+
     def __str__(self):
-        return self.serialize()
+        return self.to_etree_like_string()
         # TODO: better return as JSON
 
     def __repr__(self):
-        return f"metadoc:{self.serialize()}"
+        return f"metadoc:{self.to_etree_like_string()}"
         # TODO: better return as JSON
 
     def _path_to_xpath(self, path):
         path = path.strip()
         if re.match(
             r"^[\w]", path
         ):  # TODO: right now every tag has to start with '/' otherwise the regex below won't work
```

## bq/metadoc/version.py

```diff
@@ -1,4 +1,4 @@
 # file generated by setuptools_scm
 # don't change, don't track in version control
-__version__ = version = '0.6.3.26'
-__version_tuple__ = version_tuple = (0, 6, 3, 26)
+__version__ = version = '0.6.3.27'
+__version_tuple__ = version_tuple = (0, 6, 3, 27)
```

## Comparing `bisque_metadoc-0.6.3.26.dist-info/METADATA` & `bisque_metadoc-0.6.3.27.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bisque-metadoc
-Version: 0.6.3.26
+Version: 0.6.3.27
 Summary: Bisque Metadoc
 Author: ViQi Inc
 Author-email: devops@viqi.org
 Project-URL: homepage, https://gitlab.com/viqi/viqi-common/bisque_metadoc
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `bisque_metadoc-0.6.3.26.dist-info/RECORD` & `bisque_metadoc-0.6.3.27.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 bq/__init__.py,sha256=xiybI6MFP1EFRXvSb-33FlFs5jN4FImlrmD2D0jWs6g,167
 bq/metadoc/__init__.py,sha256=l9gw3A8XoRuAewpCkNfBA0nFUNnu0PDuTpmhh8w85uk,73
-bq/metadoc/etree.py,sha256=tM0QCHhRryUMl3U6Wb7SNK2niAIANBSiu34x40K3Qwg,2467
-bq/metadoc/formats.py,sha256=doHS1ECzmC0roEqvmwjH1MVnTinDzyipuc0p0Do0Mow,24272
+bq/metadoc/etree.py,sha256=CbHUMxNgs8tKYwaeV3yKjZLRZA82r2sfDPzk1mO_Nrg,2500
+bq/metadoc/formats.py,sha256=sYeEjX--Nk-iEpqtgR5ik49TG9cYUBlxomp2_nsYTe0,24373
 bq/metadoc/logging.py,sha256=vYuf2-OuZFvIw-lAj1R_BWpRbud92vqUxiIFEMF8eOo,1020
-bq/metadoc/version.py,sha256=IMRjnzI_5XF_B0g18HQ1jRMD__bJKcpQP4_Hh1lRjq4,167
+bq/metadoc/version.py,sha256=rgP43_At5s3w3Oz_RSuwtVgQ4f6Mzfn7ns2DDCWBiM8,167
 bq/metadoc/xmldict.py,sha256=ZIk0_XMMfBSe2JDsQhjXBSx4R70qLj-bfjN5Ebufh4c,4486
-bisque_metadoc-0.6.3.26.dist-info/METADATA,sha256=HvhkB8L7gIUhnfw7wb5ekV4OPFKXFIAQjwEd7IVaJPo,641
-bisque_metadoc-0.6.3.26.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-bisque_metadoc-0.6.3.26.dist-info/top_level.txt,sha256=w5z7Un4-v3yqVMurNio-Srl-AUvtPOxZ3tZh4Eb8RHo,3
-bisque_metadoc-0.6.3.26.dist-info/RECORD,,
+bisque_metadoc-0.6.3.27.dist-info/METADATA,sha256=d_qku0WISz5vB-GLsSiwRNVxRfNIwTyLM0pJD80r4ww,641
+bisque_metadoc-0.6.3.27.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+bisque_metadoc-0.6.3.27.dist-info/top_level.txt,sha256=w5z7Un4-v3yqVMurNio-Srl-AUvtPOxZ3tZh4Eb8RHo,3
+bisque_metadoc-0.6.3.27.dist-info/RECORD,,
```

