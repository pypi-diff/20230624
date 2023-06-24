# Comparing `tmp/leuci-geo-0.0.8.tar.gz` & `tmp/leuci-geo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leuci-geo-0.0.8.tar", last modified: Mon Jun 19 19:29:36 2023, max compression
+gzip compressed data, was "leuci-geo-0.0.9.tar", last modified: Sat Jun 24 19:21:34 2023, max compression
```

## Comparing `leuci-geo-0.0.8.tar` & `leuci-geo-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-19 19:29:36.027644 leuci-geo-0.0.8/
--rw-r--r--   0 rachel    (1000) rachel    (1000)    35149 2023-05-25 20:00:31.000000 leuci-geo-0.0.8/LICENSE
--rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-19 19:29:36.027644 leuci-geo-0.0.8/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)       22 2023-05-25 20:00:31.000000 leuci-geo-0.0.8/README.md
--rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-geo-0.0.8/pyproject.toml
--rw-r--r--   0 rachel    (1000) rachel    (1000)      656 2023-06-19 19:29:36.027644 leuci-geo-0.0.8/setup.cfg
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-19 19:29:36.017644 leuci-geo-0.0.8/src/
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-19 19:29:36.017644 leuci-geo-0.0.8/src/leuci_geo/
--rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-geo-0.0.8/src/leuci_geo/__init__.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     2963 2023-05-29 13:51:47.000000 leuci-geo-0.0.8/src/leuci_geo/geocalculator.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)    27123 2023-06-04 18:16:10.000000 leuci-geo-0.0.8/src/leuci_geo/pdbgeometry.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     2844 2023-05-29 13:40:46.000000 leuci-geo-0.0.8/src/leuci_geo/pdbloader.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     9405 2023-06-04 13:05:42.000000 leuci-geo-0.0.8/src/leuci_geo/pdbobject.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-05-29 10:54:24.000000 leuci-geo-0.0.8/src/leuci_geo/pdbspace.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)    22826 2023-06-19 19:28:31.000000 leuci-geo-0.0.8/src/leuci_geo/reportmaker.py
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-19 19:29:36.027644 leuci-geo-0.0.8/src/leuci_geo.egg-info/
--rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-19 19:29:35.000000 leuci-geo-0.0.8/src/leuci_geo.egg-info/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)      385 2023-06-19 19:29:36.000000 leuci-geo-0.0.8/src/leuci_geo.egg-info/SOURCES.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-06-19 19:29:35.000000 leuci-geo-0.0.8/src/leuci_geo.egg-info/dependency_links.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-06-19 19:29:35.000000 leuci-geo-0.0.8/src/leuci_geo.egg-info/top_level.txt
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-24 19:21:34.805450 leuci-geo-0.0.9/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    35149 2023-05-25 20:00:31.000000 leuci-geo-0.0.9/LICENSE
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-24 19:21:34.805450 leuci-geo-0.0.9/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       22 2023-05-25 20:00:31.000000 leuci-geo-0.0.9/README.md
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-geo-0.0.9/pyproject.toml
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      656 2023-06-24 19:21:34.805450 leuci-geo-0.0.9/setup.cfg
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-24 19:21:34.795450 leuci-geo-0.0.9/src/
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-24 19:21:34.805450 leuci-geo-0.0.9/src/leuci_geo/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-geo-0.0.9/src/leuci_geo/__init__.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     2963 2023-05-29 13:51:47.000000 leuci-geo-0.0.9/src/leuci_geo/geocalculator.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    27123 2023-06-04 18:16:10.000000 leuci-geo-0.0.9/src/leuci_geo/pdbgeometry.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     2844 2023-05-29 13:40:46.000000 leuci-geo-0.0.9/src/leuci_geo/pdbloader.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     9405 2023-06-04 13:05:42.000000 leuci-geo-0.0.9/src/leuci_geo/pdbobject.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-05-29 10:54:24.000000 leuci-geo-0.0.9/src/leuci_geo/pdbspace.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    23124 2023-06-24 19:21:16.000000 leuci-geo-0.0.9/src/leuci_geo/reportmaker.py
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-24 19:21:34.805450 leuci-geo-0.0.9/src/leuci_geo.egg-info/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-24 19:21:34.000000 leuci-geo-0.0.9/src/leuci_geo.egg-info/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      385 2023-06-24 19:21:34.000000 leuci-geo-0.0.9/src/leuci_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-06-24 19:21:34.000000 leuci-geo-0.0.9/src/leuci_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-06-24 19:21:34.000000 leuci-geo-0.0.9/src/leuci_geo.egg-info/top_level.txt
```

### Comparing `leuci-geo-0.0.8/LICENSE` & `leuci-geo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.8/PKG-INFO` & `leuci-geo-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-geo
-Version: 0.0.8
+Version: 0.0.9
 Summary: geometric paramaters and searches of protein structures
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `leuci-geo-0.0.8/setup.cfg` & `leuci-geo-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = leuci-geo
-version = 0.0.8
+version = 0.0.9
 author = Rachel Alcraft
 author_email = rachelalcraft@gmail.com
 description = geometric paramaters and searches of protein structures
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `leuci-geo-0.0.8/src/leuci_geo/geocalculator.py` & `leuci-geo-0.0.9/src/leuci_geo/geocalculator.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.8/src/leuci_geo/pdbgeometry.py` & `leuci-geo-0.0.9/src/leuci_geo/pdbgeometry.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.8/src/leuci_geo/pdbloader.py` & `leuci-geo-0.0.9/src/leuci_geo/pdbloader.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.8/src/leuci_geo/pdbobject.py` & `leuci-geo-0.0.9/src/leuci_geo/pdbobject.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.8/src/leuci_geo/reportmaker.py` & `leuci-geo-0.0.9/src/leuci_geo/reportmaker.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,14 +118,20 @@
             # COLOR LEGEND (FIRST guess at size ITEMS) we don;t want to plot the distanceinc
             huelen = len(data.sort_values(by=hue, ascending=True)[hue].unique()) + 1
             col_lgd = plt.legend(h[:huelen], l[:huelen], loc='upper left', bbox_to_anchor=(1.05, 1), fancybox=True, shadow=True, ncol=1)
             plt.gca().add_artist(col_lgd)
             self.ax.set_xlabel('')
             self.ax.set_ylabel('')
             plt.legend(title=hue,bbox_to_anchor=(1.05, 1), loc=2, borderaxespad=0.)  # Put the legend out of the figure
+        elif plottype == 'barplot':
+            if palette == "viridis":
+                palette = 'b'            
+            self.ax.bar(data[geo_x],data[geo_y],color=palette,width=0.5)        
+            self.ax.set_xlabel('')
+            self.ax.set_ylabel('')            
         elif plottype == 'hist2d':
             x = data[geo_x]
             y = data[geo_y]
             bins=100
             gridsize=50
             hb = plt.hexbin(x, y, bins=bins, cmap=palette, gridsize=gridsize,extent=[minx,maxx,miny,maxy])
         elif plottype == 'probability':
@@ -152,14 +158,15 @@
             self.ax.set_axisbelow(True)
 
         self.ax.set_xlabel(geo_x + "\nCount=" + str(count))
         self.ax.set_ylabel(geo_y)
         plt.title(title)
         plt.xlim([minx, maxx])
         plt.ylim([miny, maxy])
+        plt.xticks(rotation=45)   
         #Having plotted we now need to get the image data from the plt
         if not overlay:
             encoded = self.getPlotImage(self.fig, self.ax)
             htmlstring = '<img src="data:image/png;base64, {}">'.format(encoded.decode('utf-8')) + '\n'
             self.HTMLIncrement()
             self.html_string += '<td width=' + str(int(100/self.cols)) + '%>' + htmlstring + '</td>\n'
 
@@ -210,15 +217,15 @@
             g = plt.hist(mydata, edgecolor='k', bins=bins, color=palette, alpha=alpha, label='geo_x',range=axisrange,cumulative=cumulative,density=density,histtype='step')
         elif plottype == 'stepfilled':
             g = plt.hist(mydata, edgecolor='k', bins=bins, color=palette, alpha=alpha, label='geo_x',range=axisrange,cumulative=cumulative,density=density,histtype='stepfilled')
         elif plottype == 'barstacked':
             g = plt.hist(mydata, edgecolor='k', bins=bins, color=palette, alpha=alpha, label='geo_x',range=axisrange,cumulative=cumulative,density=density,histtype='barstacked')
         elif plottype == 'violin':
             g = plt.violinplot(mydata,showmeans=False,showextrema=True,showmedians=True,quantiles=[0.25,0.75])
-
+        
         #cb = plt.colorbar(g)
         #hue is used to find the outliers
         if hue != '':
             geos = []
             if len(geo_x[0]) > 1:  # todo evident bug if the x is a 1 lne stingf
                 geos = geo_x
             else:
@@ -247,26 +254,26 @@
         # Having plotted we now need to get the image data from the plt
         if not overlay:
             encoded = self.getPlotImage(self.fig, self.ax)
             htmlstring = '<img src="data:image/png;base64, {}">'.format(encoded.decode('utf-8')) + '\n'
             self.HTMLIncrement()
             self.html_string += '<td width=' + str(int(100 / self.cols)) + '%>' + htmlstring + '</td>\n'
 
-    def addPlotPi(self, data,geo_x,hue,title='',colors=[],overlay=False,alpha=1,percent=False):
+    def addPlotPi(self, data,geo_x,hue,title='',colors = [],overlay=False,percent=False):
         self.incrementOverlay(overlay)
         if colors == []:
             if percent:
                 plt.pie(data[geo_x],labels=data[hue], autopct='%1.1f%%')
             else:
                 plt.pie(data[geo_x],labels=data[hue])
         else:
             if percent:
-                plt.pie(data[geo_x], labels=data[hue],colors=colors,alpha=alpha, autopct='%1.1f%%')
+                plt.pie(data[geo_x], labels=data[hue],colors=colors,autopct='%1.1f%%')
             else:
-                plt.pie(data[geo_x], labels=data[hue],colors=colors,alpha=alpha)
+                plt.pie(data[geo_x], labels=data[hue],colors=colors)        
         plt.title(title)
         # Having plotted we now need to get the image data from the plt
         if not overlay:
             encoded = self.getPlotImage(self.fig, self.ax)
             htmlstring = '<img src="data:image/png;base64, {}">'.format(encoded.decode('utf-8')) + '\n'
             self.HTMLIncrement()
             self.html_string += '<td width=' + str(int(100 / self.cols)) + '%>' + htmlstring + '</td>\n'
```

### Comparing `leuci-geo-0.0.8/src/leuci_geo.egg-info/PKG-INFO` & `leuci-geo-0.0.9/src/leuci_geo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-geo
-Version: 0.0.8
+Version: 0.0.9
 Summary: geometric paramaters and searches of protein structures
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

