# Comparing `tmp/genopyc-1.1.0-py3-none-any.whl.zip` & `tmp/genopyc-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 424126 bytes, number of entries: 8
+Zip file size: 424144 bytes, number of entries: 8
 -rwxrwxrwx  2.0 unx      917 b- defN 23-Jun-21 11:24 genopyc/__init__.py
--rwxrwxrwx  2.0 unx    42070 b- defN 23-Jun-24 20:35 genopyc/genopyc.py
+-rwxrwxrwx  2.0 unx    42339 b- defN 23-Jun-24 20:43 genopyc/genopyc.py
 -rwxrwxrwx  2.0 unx  1302100 b- defN 23-Jun-21 11:17 genopyc/data/hippie_interactome.sif
--rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-24 20:36 genopyc-1.1.0.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-24 20:36 genopyc-1.1.0.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-24 20:36 genopyc-1.1.0.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-24 20:36 genopyc-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-24 20:36 genopyc-1.1.0.dist-info/RECORD
-8 files, 1380941 bytes uncompressed, 423026 bytes compressed:  69.4%
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-24 20:43 genopyc-1.1.1.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      596 b- defN 23-Jun-24 20:43 genopyc-1.1.1.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-24 20:43 genopyc-1.1.1.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-24 20:43 genopyc-1.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      635 b- defN 23-Jun-24 20:43 genopyc-1.1.1.dist-info/RECORD
+8 files, 1381210 bytes uncompressed, 423044 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: genopyc/genopyc.py
 Comment: 
 
 Filename: genopyc/data/hippie_interactome.sif
 Comment: 
 
-Filename: genopyc-1.1.0.dist-info/LICENSE.txt
+Filename: genopyc-1.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-1.1.0.dist-info/METADATA
+Filename: genopyc-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-1.1.0.dist-info/WHEEL
+Filename: genopyc-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-1.1.0.dist-info/top_level.txt
+Filename: genopyc-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-1.1.0.dist-info/RECORD
+Filename: genopyc-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genopyc/genopyc.py

```diff
@@ -836,15 +836,15 @@
     Enrichment = EnrichmentAnalisys(ListOfGenes)
     BuildGraph(SubG,Enrichment)
 
 
 #use this function#
 
 
-def plot_enrichment_analisys_network(df,pvalue,colormap='cividis',edgecolor='red',mkcolor='grey',mkfsize=10000,layout='spring',
+def plot_enrichment_analisys_network(list_of_genes,pvalue,colormap='cividis',edgecolor='red',mkcolor='grey',mkfsize=10000,layout='spring',
                                      mklinewidths=2,alpha=1,figsize=(40,20),savefig=False,factor=1,k=10,
                                      cbarfontsize=10,labelling=True,legend=False, legend_fontsize = 20, legend_titlefontsize = 25,
                                      legend_location = (0.5,0.0), legend_col = 6, legend_labelspacing = 1.5, legend_title = '',
                                      legend_columnspacing=1.5, legend_handlelength = 3, size_legend_nofelements=3, cbar_orientation= 'horizontal',
                                      cbar_loc=(1, 0.5),**kwargs):
     def labelling_without_overlapping(x,y,list_of_annotations,ax,verbose=False,**kwargs):
     
@@ -914,15 +914,20 @@
                         print('new bbox data',bbox_data)
                         print('annotation coordinates',box)
                         print('restart iteration')
                     keep_cycling=True
                     break
 
 
-
+    gp = GProfiler(return_dataframe=True)
+    df=gp.profile(organism='hsapiens',
+                    query=list_of_genes,
+                    significance_threshold_method='bonferroni',
+                    no_iea=True,
+                    no_evidences=False)
     maxpv=max([-np.log10(p) for p in df.p_value.tolist()])
     for i, (s,v) in enumerate(zip(df.source.value_counts().index,df.source.value_counts())):
         data=df[(df.source==s)&(-np.log10(df.p_value)>pvalue)].reset_index()
         if data.shape[0]==0:
             continue
         else:
```

## Comparing `genopyc-1.1.0.dist-info/LICENSE.txt` & `genopyc-1.1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `genopyc-1.1.0.dist-info/METADATA` & `genopyc-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genopyc
-Version: 1.1.0
+Version: 1.1.1
 Author: Francesco Gualdi
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: numpy
```

## Comparing `genopyc-1.1.0.dist-info/RECORD` & `genopyc-1.1.1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 genopyc/__init__.py,sha256=Evc18XwNN4kPqHdq62q_qSYtBIQmYeKZQORuF99rXz8,917
-genopyc/genopyc.py,sha256=vnv8vJTYiwI5uy_lm-uMvkLLxJnI6lSBaI705i-0unU,42070
+genopyc/genopyc.py,sha256=3vw1e-rk4Gim95VvxhiVKcRHO-FerVgcW8odIuWXEiI,42339
 genopyc/data/hippie_interactome.sif,sha256=iqdnCWTnTXIs43-jMLNijQ2PJWd7CRSVMHnh8miE1vs,1302100
-genopyc-1.1.0.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-genopyc-1.1.0.dist-info/METADATA,sha256=msDqOdtTMdfRM7AV8l2EDp53D1cFP2JJc4kkn4hz_kU,596
-genopyc-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-genopyc-1.1.0.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
-genopyc-1.1.0.dist-info/RECORD,,
+genopyc-1.1.1.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+genopyc-1.1.1.dist-info/METADATA,sha256=w-TTg0p9_HGbD_FJkmBqLEoVFCDBL126HkzX7onDF0o,596
+genopyc-1.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+genopyc-1.1.1.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
+genopyc-1.1.1.dist-info/RECORD,,
```

