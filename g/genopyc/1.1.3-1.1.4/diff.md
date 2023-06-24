# Comparing `tmp/genopyc-1.1.3-py3-none-any.whl.zip` & `tmp/genopyc-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 424167 bytes, number of entries: 8
+Zip file size: 424193 bytes, number of entries: 8
 -rwxrwxrwx  2.0 unx      978 b- defN 23-Jun-24 20:45 genopyc/__init__.py
--rwxrwxrwx  2.0 unx    42339 b- defN 23-Jun-24 20:43 genopyc/genopyc.py
+-rwxrwxrwx  2.0 unx    42535 b- defN 23-Jun-24 21:02 genopyc/genopyc.py
 -rwxrwxrwx  2.0 unx  1302100 b- defN 23-Jun-21 11:17 genopyc/data/hippie_interactome.sif
--rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-24 20:49 genopyc-1.1.3.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-24 20:49 genopyc-1.1.3.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-24 20:49 genopyc-1.1.3.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-24 20:49 genopyc-1.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-24 20:49 genopyc-1.1.3.dist-info/RECORD
-8 files, 1381271 bytes uncompressed, 423067 bytes compressed:  69.4%
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-24 21:02 genopyc-1.1.4.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-24 21:02 genopyc-1.1.4.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-24 21:02 genopyc-1.1.4.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-24 21:02 genopyc-1.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-24 21:02 genopyc-1.1.4.dist-info/RECORD
+8 files, 1381467 bytes uncompressed, 423093 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: genopyc/genopyc.py
 Comment: 
 
 Filename: genopyc/data/hippie_interactome.sif
 Comment: 
 
-Filename: genopyc-1.1.3.dist-info/LICENSE.txt
+Filename: genopyc-1.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-1.1.3.dist-info/METADATA
+Filename: genopyc-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-1.1.3.dist-info/WHEEL
+Filename: genopyc-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-1.1.3.dist-info/top_level.txt
+Filename: genopyc-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-1.1.3.dist-info/RECORD
+Filename: genopyc-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genopyc/genopyc.py

```diff
@@ -1,14 +1,15 @@
 import requests
 import pandas as pd
 import biomapy as bp
 import os
 import networkx as nx
 import numpy as np
 import pandas as pd
+import matplotlib
 import requests
 from gprofiler import GProfiler
 import igraph as ig 
 import warnings
 warnings.filterwarnings('ignore')
 import dash
 import dash_core_components as dcc
@@ -866,60 +867,60 @@
 
             # If one rectangle is above other
             if(r1.y >= l2.y or r2.y >= l1.y):
                 return False
 
             return True
 
-    annotations_coord=[]
-    for i, dot in enumerate(y):
-        x_coords=x[i]
-        y_coords=y[i]
-        annotation=ax.annotate(str(list_of_annotations[i]),
-                                xy=(x[i],y[i]),
-                                 xytext=(x_coords,y_coords),
-                                    **kwargs)
-
-        ax.figure.canvas.draw()
-        bbox=matplotlib.text.Text.get_window_extent(annotation)
-        bbox_data = ax.transData.inverted().transform(bbox)
-        factor=0.2*(bbox_data[0,0]-bbox_data[1,0])
-        annotations_coord.append(bbox_data)
-        ##BUILD THE SPIRAL##
-        theta=np.radians(np.linspace(1,360*200,500))
-        r=np.linspace(0,max(max(zip(x,y))),len(theta))
-        x_2 = r*np.cos(theta)+x_coords#move the spiral onto the data point
-        y_2 = r*np.sin(theta)+y_coords
-        n=0
-        keep_cycling=True
-        while keep_cycling:
-            keep_cycling=False
-            if verbose==True:
-                print('start checking box %s'% i)
-            for ind, box in enumerate (annotations_coord[0:-1]):
-                if verbose:
-                    print('checking %s and %s' % (i,ind))
-                if doOverlap(box,bbox_data):
+        annotations_coord=[]
+        for i, dot in enumerate(y):
+            x_coords=x[i]
+            y_coords=y[i]
+            annotation=ax.annotate(str(list_of_annotations[i]),
+                                    xy=(x[i],y[i]),
+                                    xytext=(x_coords,y_coords),
+                                        **kwargs)
+
+            ax.figure.canvas.draw()
+            bbox=matplotlib.text.Text.get_window_extent(annotation)
+            bbox_data = ax.transData.inverted().transform(bbox)
+            factor=0.2*(bbox_data[0,0]-bbox_data[1,0])
+            annotations_coord.append(bbox_data)
+            ##BUILD THE SPIRAL##
+            theta=np.radians(np.linspace(1,360*200,500))
+            r=np.linspace(0,max(max(zip(x,y))),len(theta))
+            x_2 = r*np.cos(theta)+x_coords#move the spiral onto the data point
+            y_2 = r*np.sin(theta)+y_coords
+            n=0
+            keep_cycling=True
+            while keep_cycling:
+                keep_cycling=False
+                if verbose==True:
+                    print('start checking box %s'% i)
+                for ind, box in enumerate (annotations_coord[0:-1]):
                     if verbose:
-                        print('%s and %s overlap' % (i,ind))
-                    annotation.set_x(x_2[n])
-                    annotation.set_y(y_2[n])
-                    n+=1
-                    ax.figure.canvas.draw()
-                    bbox=matplotlib.text.Text.get_window_extent(annotation)
-                    bbox_data = ax.transData.inverted().transform(bbox)
-                    annotations_coord.pop()
-                    annotations_coord.append(bbox_data)
-                    if verbose:
-                        print('new coords (x=%i,y=%i)'%(x_coords,y_coords))
-                        print('new bbox data',bbox_data)
-                        print('annotation coordinates',box)
-                        print('restart iteration')
-                    keep_cycling=True
-                    break
+                        print('checking %s and %s' % (i,ind))
+                    if doOverlap(box,bbox_data):
+                        if verbose:
+                            print('%s and %s overlap' % (i,ind))
+                        annotation.set_x(x_2[n])
+                        annotation.set_y(y_2[n])
+                        n+=1
+                        ax.figure.canvas.draw()
+                        bbox=matplotlib.text.Text.get_window_extent(annotation)
+                        bbox_data = ax.transData.inverted().transform(bbox)
+                        annotations_coord.pop()
+                        annotations_coord.append(bbox_data)
+                        if verbose:
+                            print('new coords (x=%i,y=%i)'%(x_coords,y_coords))
+                            print('new bbox data',bbox_data)
+                            print('annotation coordinates',box)
+                            print('restart iteration')
+                        keep_cycling=True
+                        break
 
 
     gp = GProfiler(return_dataframe=True)
     df=gp.profile(organism='hsapiens',
                     query=list_of_genes,
                     significance_threshold_method='bonferroni',
                     no_iea=True,
@@ -1054,8 +1055,8 @@
             axis.set_ylim([factor*y for y in axis.get_ylim()])
             plt.tight_layout()
             if savefig:
                 plt.savefig(str(s)+'enrichment_analysis.jpeg', dpi=300,bbox_inches='tight')
             
             
             
-            plt.show()
+            plt.show()
```

## Comparing `genopyc-1.1.3.dist-info/LICENSE.txt` & `genopyc-1.1.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `genopyc-1.1.3.dist-info/METADATA` & `genopyc-1.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genopyc
-Version: 1.1.3
+Version: 1.1.4
 Author: Francesco Gualdi
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: numpy
```

