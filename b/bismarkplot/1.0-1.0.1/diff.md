# Comparing `tmp/bismarkplot-1.0.tar.gz` & `tmp/bismarkplot-1.0.1.tar.gz`

## Comparing `bismarkplot-1.0.tar` & `bismarkplot-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bismarkplot-1.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 bismarkplot-1.0/.github/workflows/publish.yaml
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/.gitignore
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/BismarkPlot.iml
--rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/dbnavigator.xml
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/misc.xml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/modules.xml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/vcs.xml
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 bismarkplot-1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/.nojekyll
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/Makefile
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/conf.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/index.rst
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/make.bat
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/requirements.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/_templates/module.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bismarkplot-1.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/BarPlot.py
--rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/Bismark.py
--rw-r--r--   0        0        0    16328 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/BismarkFiles.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/BoxPlot.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/HeatMap.py
--rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/LinePlot.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/__init__.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/read_bismark.py
--rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 bismarkplot-1.0/src/bismarkplot/read_genome.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 bismarkplot-1.0/LICENSE.txt
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 bismarkplot-1.0/README.md
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 bismarkplot-1.0/pyproject.toml
--rw-r--r--   0        0        0    43599 2020-02-02 00:00:00.000000 bismarkplot-1.0/PKG-INFO
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/.idea/.gitignore
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/.idea/BismarkPlot.iml
+-rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/.idea/dbnavigator.xml
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/.idea/misc.xml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/.idea/modules.xml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/.idea/vcs.xml
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/docs/.nojekyll
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/docs/index.rst
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/docs/requirements.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/docs/_templates/module.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/src/bismarkplot/BarPlot.py
+-rw-r--r--   0        0        0     2439 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/src/bismarkplot/Bismark.py
+-rw-r--r--   0        0        0    16997 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/src/bismarkplot/BismarkFiles.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/src/bismarkplot/BoxPlot.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/src/bismarkplot/HeatMap.py
+-rw-r--r--   0        0        0     2819 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/src/bismarkplot/LinePlot.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/src/bismarkplot/__init__.py
+-rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/src/bismarkplot/__main__.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/src/bismarkplot/read_bismark.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/src/bismarkplot/read_genome.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/README.md
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    43601 2020-02-02 00:00:00.000000 bismarkplot-1.0.1/PKG-INFO
```

### Comparing `bismarkplot-1.0/.github/workflows/publish.yaml` & `bismarkplot-1.0.1/.github/workflows/publish.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         build
         --user
     - name: Build a binary wheel and a source tarball
       run: >-
         python -m
         build
     - name: Publish distribution 📦 to Test PyPI
+      if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.TEST_PYPI_API_TOKEN }}
         repository-url: https://test.pypi.org/legacy/
     - name: Publish distribution 📦 to PyPI
       if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `bismarkplot-1.0/.idea/dbnavigator.xml` & `bismarkplot-1.0.1/.idea/dbnavigator.xml`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/.idea/inspectionProfiles/Project_Default.xml` & `bismarkplot-1.0.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/docs/Makefile` & `bismarkplot-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/docs/conf.py` & `bismarkplot-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/docs/make.bat` & `bismarkplot-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/src/bismarkplot/BarPlot.py` & `bismarkplot-1.0.1/src/bismarkplot/BarPlot.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/src/bismarkplot/Bismark.py` & `bismarkplot-1.0.1/src/bismarkplot/Bismark.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/src/bismarkplot/BismarkFiles.py` & `bismarkplot-1.0.1/src/bismarkplot/BismarkFiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,25 +97,27 @@
             strand: str = '+',
             smooth: float = .05,
             labels: list[str] = None,
             linewidth: float = 1.0,
             linestyle: str = '-',
             title: str = None,
             out_dir: str = '',
-            dpi: int = 300
+            dpi: int = 300,
+            file_format: str = 'png'
     ):
         """
         Method to plot selected context and strand
 
+        :param file_format: Format of output image
         :param context: Methylation context to filter
         :param strand: Strand to filter
         :param smooth: Smooth * len(density) = window_length for SavGol filter
         :param labels: Labels for files data
         :param linewidth: Line width
-        :param linestyle: Line width see Linestyles_
+        :param linestyle: See Linestyles_
         :param title: Title of the plot
         :param out_dir: directory to save plots to
         :param dpi: DPI of output pic
 
         .. _Linestyles: https://matplotlib.org/stable/gallery/lines_bars_and_markers/linestyles.html/
         """
 
@@ -134,31 +136,33 @@
         if len(set(labels)) and list(set(labels))[0] is not None:
             axes.legend(loc='best')
 
         axes.set_title(title.replace('_', ' '), fontstyle='italic')
         self.__add_flank_lines(axes)
 
         self.__set_single_fig_dim()
-        file_name = f'{title}_{self.__current_time()}.png'
+        file_name = f'{title}_{self.__current_time()}.{file_format}'
         self.__logger.info(f'Line plot on {context}{strand} saved as {file_name}')
-        plt.savefig(f'{out_dir}/{file_name}', dpi=dpi)
+        plt.savefig(f'{out_dir}/{file_name}', dpi=dpi, format=file_format)
 
     def draw_heat_maps_filtered(
             self,
             context: str = 'CG',
             strand: str = '+',
             resolution: int = 100,
             labels: list[str] = None,
             title: str = None,
             out_dir: str = '',
-            dpi: int = 300
+            dpi: int = 300,
+            file_format: str = 'png'
     ):
         """
         Method to plot heatmap for selected context and strand
 
+        :param file_format: Format of output image
         :param context: Methylation context to filter
         :param strand: Strand to filter
         :param resolution:
         :param labels: Labels for files data
         :param title: Title of the plot
         :param out_dir: directory to save plots to
         :param dpi: DPI of output pic
@@ -202,79 +206,85 @@
                 ax.set_xlabel('Position')
                 ax.set_ylabel('')
                 self.__add_flank_lines(ax)
                 plt.colorbar(image, ax=ax, label='Methylation density')
 
         plt.suptitle(title.replace('_', ' '), fontstyle='italic')
         fig.set_size_inches(6 * subplots_x, 5 * subplots_y)
-        file_name = f'{title}_{self.__current_time()}.png'
+        file_name = f'{title}_{self.__current_time()}.{file_format}'
         self.__logger.info(f'Heat Map on {context}{strand} saved as {file_name}')
-        plt.savefig(f'{out_dir}/{file_name}', dpi=dpi)
+        plt.savefig(f'{out_dir}/{file_name}', dpi=dpi, format=file_format)
 
     def draw_line_plots_all(
             self,
             smooth: float = .05,
             labels: list[str] = None,
             linewidth: float = 1.0,
             linestyle: str = '-',
             out_dir: str = '',
-            dpi: int = 300
+            dpi: int = 300,
+            file_format: str = 'png'
     ):
         """
         Method to plot all contexts and strands
 
+        :param file_format: Format of output image
         :param smooth: ``smooth * len(density) = window_length`` for SavGol filter
         :param labels: Labels for files data
         :param linewidth: Line width
         :param linestyle: Line style
         :param out_dir: directory to save plots to
         :param dpi: DPI of output pic
         """
         out_dir = self.__format_dir(out_dir)
         if not self.__check_data(self.line_plots, 'LinePlots'):
             return
 
         filters = [(context, strand) for context in ['CG', 'CHG', 'CHH'] for strand in ['+', '-']]
 
         for context, strand in filters:
-            self.draw_line_plots_filtered(context, strand, smooth, labels, linewidth, linestyle, None, out_dir, dpi)
+            self.draw_line_plots_filtered(context, strand, smooth, labels, linewidth, linestyle, None, out_dir, dpi, file_format)
 
     def draw_heat_maps_all(
             self,
             resolution: int = 100,
             labels: list[str] = None,
             out_dir: str = '',
-            dpi: int = 300
+            dpi: int = 300,
+            file_format: str = 'png'
     ):
         """
         Method to plot all heatmaps and strands
 
+        :param file_format: Format of output image
         :param resolution: Number of vertical rows in the resulting image
         :param labels: Labels for files data
         :param out_dir: directory to save plots to
         :param dpi: DPI of output pic
         """
         out_dir = self.__format_dir(out_dir)
         if not self.__check_data(self.heat_maps, 'HeatMaps'):
             return
 
         filters = [(context, strand) for context in ['CG', 'CHG', 'CHH'] for strand in ['+', '-']]
 
         for context, strand in filters:
-            self.draw_heat_maps_filtered(context, strand, resolution, labels, None, out_dir, dpi)
+            self.draw_heat_maps_filtered(context, strand, resolution, labels, None, out_dir, dpi, file_format)
 
     def draw_bar_plot(
             self,
             labels: list[str] = None,
             out_dir: str = '',
-            dpi: int = 300
+            dpi: int = 300,
+            file_format: str = 'png'
     ):
         """
         Method to plot data for all contexts as bar plot. The plot isn't strand specific.
 
+        :param file_format: Format of output image
         :param labels: Labels for files data
         :param out_dir: directory to save plots to
         :param dpi: DPI of output pic
         """
         out_dir = self.__format_dir(out_dir)
         if not self.__check_data(self.bar_plots, 'BarPlots'):
             return
@@ -288,29 +298,31 @@
             df[label] = bar_plot.bismark.with_columns(pl.col('context').cast(pl.Utf8)).sort('context')['density'].to_list()
 
         self.__set_single_fig_dim()
 
         df.plot(x='context', kind='bar', stacked=False, edgecolor='k', linewidth=1)
         plt.xlabel('Context')
         plt.ylabel('Methylation density')
-        file_name = f'bar_{self.__current_time()}.png'
+        file_name = f'bar_{self.__current_time()}.{file_format}'
         self.__logger.info(f'Bar Plot saved as {file_name}')
-        plt.savefig(f'{out_dir}/{file_name}', dpi=dpi, bbox_inches='tight')
+        plt.savefig(f'{out_dir}/{file_name}', dpi=dpi, bbox_inches='tight', format=file_format)
 
     def draw_box_plot(
             self,
             strand_specific: bool = False,
             widths: float = .6,
             labels: list[str] = None,
             out_dir: str = '',
-            dpi: int = 300
+            dpi: int = 300,
+            file_format: str = 'png'
     ):
         """
         Method to plot data for all contexts as box plot
 
+        :param file_format: Format of output image
         :param strand_specific: Distinguish strand or not
         :param widths: Widths of bars
         :param labels: Labels for files data
         :param out_dir: directory to save plots to
         :param dpi: DPI of output pic
         """
         out_dir = self.__format_dir(out_dir)
@@ -363,17 +375,17 @@
         plt.legend(lines, labels)
         [line.set_visible(False) for line in lines]
 
         self.__set_single_fig_dim()
 
         plt.xlabel('Context')
         plt.ylabel('Methylation density')
-        file_name = f'box_{self.__current_time()}.png'
+        file_name = f'box_{self.__current_time()}.{file_format}'
         self.__logger.info(f'Box Plot saved as {file_name}')
-        plt.savefig(f'{out_dir}/{file_name}', dpi=dpi, bbox_inches='tight')
+        plt.savefig(f'{out_dir}/{file_name}', dpi=dpi, bbox_inches='tight', format=file_format)
 
     def __add_flank_lines(self, axes: plt.Axes):
         """
         Add flank lines to the given axis (for line plot)
         """
         if self.__flank_windows:
             x_ticks = [self.__flank_windows - 1, self.__gene_windows + self.__flank_windows]
```

### Comparing `bismarkplot-1.0/src/bismarkplot/BoxPlot.py` & `bismarkplot-1.0.1/src/bismarkplot/BoxPlot.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,9 +44,9 @@
         :return: List of density of filtered Dataframe
         """
         if strand is not None:
             filter_expr = (pl.col('context') == context) & (pl.col('strand') == strand)
             return self.bismark.filter(filter_expr)['density'].to_list()[0]
         else:
             filter_expr = pl.col('context') == context
-            return self.bismark.groupby('context').agg(pl.sum('density')).filter(filter_expr)['density'].to_list()[0]
+            return self.bismark.explode('density').groupby('context').agg(pl.col('density')).filter(filter_expr)['density'].to_list()[0]
```

### Comparing `bismarkplot-1.0/src/bismarkplot/HeatMap.py` & `bismarkplot-1.0.1/src/bismarkplot/HeatMap.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/src/bismarkplot/LinePlot.py` & `bismarkplot-1.0.1/src/bismarkplot/LinePlot.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/src/bismarkplot/read_bismark.py` & `bismarkplot-1.0.1/src/bismarkplot/read_bismark.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/src/bismarkplot/read_genome.py` & `bismarkplot-1.0.1/src/bismarkplot/read_genome.py`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/LICENSE.txt` & `bismarkplot-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bismarkplot-1.0/README.md` & `bismarkplot-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # BismarkPlot
-A small library to plot Bismark ``methylation_exctractor`` reports.
+A small library to plot Bismark ``methylation_extractor`` reports.
 
 See the docs: https://shitohana.github.io/BismarkPlot
 
 Right now only ``coverage2cytosine`` input is supported, but support for ``bismark2bedGraph`` will be added soon.
 
 ## Installation
 
@@ -69,8 +69,8 @@
 
 For box plot or bar plot use
 ```python
 bismark.draw_box_plot(strand_specific=True, labels=['exp1', 'exp2'])
 bismark.draw_bar_plot(labels=['exp1', 'exp2'])
 ```
 <img alt="box_05_07_23:54.png" height="400" src="https://user-images.githubusercontent.com/43905117/236703689-9eaaa28a-1a98-4300-a0d0-83039ed9a541.png"/>
-<img alt="bar_05_07_23:54.png" height="400" src="https://user-images.githubusercontent.com/43905117/236703687-f3fd1225-1ad1-45b0-9318-b2282a694e68.png"/>
+<img alt="bar_05_07_23:54.png" height="400" src="https://user-images.githubusercontent.com/43905117/236703687-f3fd1225-1ad1-45b0-9318-b2282a694e68.png"/>
```

### Comparing `bismarkplot-1.0/pyproject.toml` & `bismarkplot-1.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bismarkplot"
-version = "1.0"
+version = "1.0.1"
 authors = [
   { name="shitohana", email="kyudytskiy@gmail.com" },
 ]
 keywords = ['bismark', 'methylation', 'plot']
 license = {file = "LICENSE.txt"}
 dependencies = [
     "matplotlib>=3.7.1",
@@ -29,8 +29,11 @@
 
 [project.urls]
 Homepage = "https://github.com/shitohana/BismarkPlot"
 Documentation = "https://shitohana.github.io/BismarkPlot/"
 "Bug Tracker" = "https://github.com/shitohana/BismarkPlot/issues"
 
 [tool.hatch.build]
-exclude = ["/venv", "/dist", "/test"]
+exclude = ["/venv", "/dist", "/test"]
+
+[project.scripts]
+bismarkplot = "bismarkplot.__main__:main"
```

### Comparing `bismarkplot-1.0/PKG-INFO` & `bismarkplot-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bismarkplot
-Version: 1.0
+Version: 1.0.1
 Summary: A small library to plot Bismark methylation_exctractor reports.
 Project-URL: Homepage, https://github.com/shitohana/BismarkPlot
 Project-URL: Documentation, https://shitohana.github.io/BismarkPlot/
 Project-URL: Bug Tracker, https://github.com/shitohana/BismarkPlot/issues
 Author-email: shitohana <kyudytskiy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -690,15 +690,15 @@
 Requires-Dist: numpy>=1.24.2
 Requires-Dist: pandas>=2.0.0
 Requires-Dist: polars>=0.17.5
 Requires-Dist: scipy>=1.10.1
 Description-Content-Type: text/markdown
 
 # BismarkPlot
-A small library to plot Bismark ``methylation_exctractor`` reports.
+A small library to plot Bismark ``methylation_extractor`` reports.
 
 See the docs: https://shitohana.github.io/BismarkPlot
 
 Right now only ``coverage2cytosine`` input is supported, but support for ``bismark2bedGraph`` will be added soon.
 
 ## Installation
 
@@ -764,8 +764,8 @@
 
 For box plot or bar plot use
 ```python
 bismark.draw_box_plot(strand_specific=True, labels=['exp1', 'exp2'])
 bismark.draw_bar_plot(labels=['exp1', 'exp2'])
 ```
 <img alt="box_05_07_23:54.png" height="400" src="https://user-images.githubusercontent.com/43905117/236703689-9eaaa28a-1a98-4300-a0d0-83039ed9a541.png"/>
-<img alt="bar_05_07_23:54.png" height="400" src="https://user-images.githubusercontent.com/43905117/236703687-f3fd1225-1ad1-45b0-9318-b2282a694e68.png"/>
+<img alt="bar_05_07_23:54.png" height="400" src="https://user-images.githubusercontent.com/43905117/236703687-f3fd1225-1ad1-45b0-9318-b2282a694e68.png"/>
```

