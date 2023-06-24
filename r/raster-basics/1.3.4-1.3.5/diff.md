# Comparing `tmp/raster_basics-1.3.4.tar.gz` & `tmp/raster_basics-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster_basics-1.3.4.tar", last modified: Fri Jun 16 19:27:15 2023, max compression
+gzip compressed data, was "raster_basics-1.3.5.tar", last modified: Sat Jun 24 15:29:19 2023, max compression
```

## Comparing `raster_basics-1.3.4.tar` & `raster_basics-1.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:27:15.834809 raster_basics-1.3.4/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-16 19:27:15.834865 raster_basics-1.3.4/PKG-INFO
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:27:15.834047 raster_basics-1.3.4/raster_basics/
--rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.3.4/raster_basics/BaseFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    42097 2023-06-01 21:15:30.000000 raster_basics-1.3.4/raster_basics/DataPlots.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    24574 2023-06-16 19:26:40.000000 raster_basics-1.3.4/raster_basics/GlacierFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.3.4/raster_basics/RasterBasics.py
--rwxrwxrwx   0 albinwells   (501) staff       (20)    12126 2023-06-13 18:14:16.000000 raster_basics-1.3.4/raster_basics/SmoothingFunctions.py
--rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.4/raster_basics/__init__.py
-drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-16 19:27:15.834704 raster_basics-1.3.4/raster_basics.egg-info/
--rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-16 19:27:15.000000 raster_basics-1.3.4/raster_basics.egg-info/PKG-INFO
--rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-16 19:27:15.000000 raster_basics-1.3.4/raster_basics.egg-info/SOURCES.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-16 19:27:15.000000 raster_basics-1.3.4/raster_basics.egg-info/dependency_links.txt
--rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-16 19:27:15.000000 raster_basics-1.3.4/raster_basics.egg-info/not-zip-safe
--rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-16 19:27:15.000000 raster_basics-1.3.4/raster_basics.egg-info/top_level.txt
--rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-16 19:27:15.835126 raster_basics-1.3.4/setup.cfg
--rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-16 19:26:57.000000 raster_basics-1.3.4/setup.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-24 15:29:19.736894 raster_basics-1.3.5/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-24 15:29:19.737024 raster_basics-1.3.5/PKG-INFO
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-24 15:29:19.735849 raster_basics-1.3.5/raster_basics/
+-rw-rw-r--   0 albinwells   (501) staff       (20)     8661 2023-02-27 17:09:17.000000 raster_basics-1.3.5/raster_basics/BaseFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    42340 2023-06-24 15:28:38.000000 raster_basics-1.3.5/raster_basics/DataPlots.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    24574 2023-06-16 19:26:40.000000 raster_basics-1.3.5/raster_basics/GlacierFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)    12235 2023-03-23 16:41:47.000000 raster_basics-1.3.5/raster_basics/RasterBasics.py
+-rwxrwxrwx   0 albinwells   (501) staff       (20)    12126 2023-06-13 18:14:16.000000 raster_basics-1.3.5/raster_basics/SmoothingFunctions.py
+-rw-rw-r--   0 albinwells   (501) staff       (20)      574 2023-02-03 15:09:59.000000 raster_basics-1.3.5/raster_basics/__init__.py
+drwxr-xr-x   0 albinwells   (501) staff       (20)        0 2023-06-24 15:29:19.736771 raster_basics-1.3.5/raster_basics.egg-info/
+-rw-r--r--   0 albinwells   (501) staff       (20)      184 2023-06-24 15:29:19.000000 raster_basics-1.3.5/raster_basics.egg-info/PKG-INFO
+-rw-r--r--   0 albinwells   (501) staff       (20)      386 2023-06-24 15:29:19.000000 raster_basics-1.3.5/raster_basics.egg-info/SOURCES.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-24 15:29:19.000000 raster_basics-1.3.5/raster_basics.egg-info/dependency_links.txt
+-rw-r--r--   0 albinwells   (501) staff       (20)        1 2023-06-24 15:29:19.000000 raster_basics-1.3.5/raster_basics.egg-info/not-zip-safe
+-rw-r--r--   0 albinwells   (501) staff       (20)       14 2023-06-24 15:29:19.000000 raster_basics-1.3.5/raster_basics.egg-info/top_level.txt
+-rw-rw-r--   0 albinwells   (501) staff       (20)       38 2023-06-24 15:29:19.737383 raster_basics-1.3.5/setup.cfg
+-rw-rw-r--   0 albinwells   (501) staff       (20)      421 2023-06-24 15:28:51.000000 raster_basics-1.3.5/setup.py
```

### Comparing `raster_basics-1.3.4/raster_basics/BaseFunctions.py` & `raster_basics-1.3.5/raster_basics/BaseFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.4/raster_basics/DataPlots.py` & `raster_basics-1.3.5/raster_basics/DataPlots.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,45 +29,49 @@
         ax.add_artist(ScaleBar(dx=res, units='m')) # add scalebar
     fig.colorbar(c, label=ctitle)
     fig.suptitle(title)
     plt.show()
     if savefig == True:
     	fig.savefig(title + '.jpg', dpi=500) # to save the plot as a jpg image
 
-def scatterplot(data, xtitle, ytitle, title, colors, labels, markers, xyLine=False, buff=100, savefig=False):
+def scatterplot(data, xtitle, ytitle, title, colors, labels, markers='.', xyLine=False, buff=100, savefig=False):
     """
 	Create a scatterplot from data
 		data: input data (list of arrays of length 2) (e.g. [[0, 0, 0, 0], [1, 2, 3, 4]] or [[[0, 0, 0], [1, 2, 3]], [[1, 1, 1, 1], [1, 2, 3, 4]]])
 		xtitle, ytitle: axis titles (str)
 		colors: list of colors for each x-y scatterplot dataset (list of str, same length as data)
 		labels: legend label for data (list of str, same length as data) (e.g. ['label1', 'label2'])
-		markers: scatterplot marker (list of str, same length as data)
+		markers: scatterplot marker (list of str, same length as data, or string if all markers should be the same)
 		xyLine: to show the 1-to-1 line (boolean)
 		buff: buffer on axis limits (int or float)
     """
     fig = plt.figure()
     ax = fig.add_subplot(111)
     plt.grid()
+    
+    if type(markers) == str:
+        markers = [markers] * len(data)
 
     for i, xy in enumerate(data):
         ax.scatter(xy[0], xy[1], c=colors[i], alpha=0.7, marker=markers[i], label=labels[i])
     ax.set_xlabel(xtitle)
     ax.set_ylabel(ytitle)
     ax.legend()
     if xyLine == True:
         ax.axline([0, 0], [1, 1], c='k', ls='--', lw=1)
 
-    maximums = []
-    minimums = []
+    maximums_x, minimums_x, maximums_y, minimums_y = [], [], [], []
     for d in np.array(data):
-        maximums.append(max([max(d[0]), max(d[1])]) + buff)
-        minimums.append(min([min(d[0]), min(d[1])]) - buff)
+        maximums_x.append(np.nanmax(d[0]))
+        minimums_x.append(np.nanmin(d[0]))
+        maximums_y.append(np.nanmax(d[1]))
+        minimums_y.append(np.nanmin(d[1]))
 
-    ax.set_xlim([min(minimums), max(maximums)])
-    ax.set_ylim([min(minimums), max(maximums)])
+    ax.set_xlim([min(minimums_x) - buff, max(maximums_x) + buff])
+    ax.set_ylim([min(minimums_y) - buff, max(maximums_y) + buff])
     fig.suptitle(title, size=8)
     
     if savefig == True:
     	figName = title.replace(' ', '_') + '.png'
     	fig.savefig(figName, dpi=250)
```

### Comparing `raster_basics-1.3.4/raster_basics/GlacierFunctions.py` & `raster_basics-1.3.5/raster_basics/GlacierFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.4/raster_basics/RasterBasics.py` & `raster_basics-1.3.5/raster_basics/RasterBasics.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.4/raster_basics/SmoothingFunctions.py` & `raster_basics-1.3.5/raster_basics/SmoothingFunctions.py`

 * *Files identical despite different names*

### Comparing `raster_basics-1.3.4/raster_basics/__init__.py` & `raster_basics-1.3.5/raster_basics/__init__.py`

 * *Files identical despite different names*

