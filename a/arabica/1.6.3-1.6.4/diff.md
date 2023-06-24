# Comparing `tmp/arabica-1.6.3.tar.gz` & `tmp/arabica-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arabica-1.6.3.tar", last modified: Thu Jun 22 01:06:27 2023, max compression
+gzip compressed data, was "arabica-1.6.4.tar", last modified: Sat Jun 24 21:15:33 2023, max compression
```

## Comparing `arabica-1.6.3.tar` & `arabica-1.6.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 01:06:27.296331 arabica-1.6.3/
--rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 arabica-1.6.3/LICENSE
--rw-rw-rw-   0        0        0     7741 2023-06-22 01:06:27.296331 arabica-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0     6974 2023-06-17 11:44:35.000000 arabica-1.6.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 01:06:27.296331 arabica-1.6.3/arabica/
--rw-rw-rw-   0        0        0      105 2023-05-18 23:17:32.000000 arabica-1.6.3/arabica/__init__.py
--rw-rw-rw-   0        0        0    11892 2023-06-22 00:51:28.000000 arabica-1.6.3/arabica/arabica_freq.py
--rw-rw-rw-   0        0        0    30680 2023-06-22 00:04:37.000000 arabica-1.6.3/arabica/cappuccino.py
--rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.3/arabica/clean_ngram.py
--rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.3/arabica/clean_numbers.py
--rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.3/arabica/coffee_break.py
--rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.3/arabica/group.py
--rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.3/arabica/preprocess.py
--rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.3/arabica/sentiment.py
--rw-rw-rw-   0        0        0      447 2023-06-22 00:51:28.000000 arabica-1.6.3/arabica/stopwords.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:06:27.296331 arabica-1.6.3/arabica.egg-info/
--rw-rw-rw-   0        0        0     7741 2023-06-22 01:06:27.000000 arabica-1.6.3/arabica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      424 2023-06-22 01:06:27.000000 arabica-1.6.3/arabica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 01:06:27.000000 arabica-1.6.3/arabica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2023-06-22 01:06:27.000000 arabica-1.6.3/arabica.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-22 01:06:27.000000 arabica-1.6.3/arabica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      547 2023-06-22 01:06:08.000000 arabica-1.6.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 01:06:27.296331 arabica-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0     1111 2023-06-22 01:06:08.000000 arabica-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:15:33.269831 arabica-1.6.4/
+-rw-rw-rw-   0        0        0       11 2023-05-18 21:22:46.000000 arabica-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0     7741 2023-06-24 21:15:33.269831 arabica-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6974 2023-06-17 11:44:35.000000 arabica-1.6.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 21:15:33.269831 arabica-1.6.4/arabica/
+-rw-rw-rw-   0        0        0      105 2023-06-24 17:39:10.000000 arabica-1.6.4/arabica/__init__.py
+-rw-rw-rw-   0        0        0    11892 2023-06-22 16:47:25.000000 arabica-1.6.4/arabica/arabica_freq.py
+-rw-rw-rw-   0        0        0    31589 2023-06-24 20:46:06.000000 arabica-1.6.4/arabica/cappuccino.py
+-rw-rw-rw-   0        0        0     1684 2022-11-28 19:40:32.000000 arabica-1.6.4/arabica/clean_ngram.py
+-rw-rw-rw-   0        0        0      146 2022-08-31 20:55:29.000000 arabica-1.6.4/arabica/clean_numbers.py
+-rw-rw-rw-   0        0        0     8246 2023-06-17 08:04:35.000000 arabica-1.6.4/arabica/coffee_break.py
+-rw-rw-rw-   0        0        0     2531 2023-03-01 22:21:18.000000 arabica-1.6.4/arabica/group.py
+-rw-rw-rw-   0        0        0      595 2023-03-01 22:21:19.000000 arabica-1.6.4/arabica/preprocess.py
+-rw-rw-rw-   0        0        0      533 2023-06-17 08:02:21.000000 arabica-1.6.4/arabica/sentiment.py
+-rw-rw-rw-   0        0        0      447 2023-06-22 00:51:28.000000 arabica-1.6.4/arabica/stopwords.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:15:33.269831 arabica-1.6.4/arabica.egg-info/
+-rw-rw-rw-   0        0        0     7741 2023-06-24 21:15:33.000000 arabica-1.6.4/arabica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-06-24 21:15:33.000000 arabica-1.6.4/arabica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 21:15:33.000000 arabica-1.6.4/arabica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      186 2023-06-24 21:15:33.000000 arabica-1.6.4/arabica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-24 21:15:33.000000 arabica-1.6.4/arabica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      547 2023-06-24 21:15:19.000000 arabica-1.6.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 21:15:33.269831 arabica-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     1125 2023-06-24 21:15:19.000000 arabica-1.6.4/setup.py
```

### Comparing `arabica-1.6.3/PKG-INFO` & `arabica-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
```

### Comparing `arabica-1.6.3/README.md` & `arabica-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `arabica-1.6.3/arabica/arabica_freq.py` & `arabica-1.6.4/arabica/arabica_freq.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.3/arabica/cappuccino.py` & `arabica-1.6.4/arabica/cappuccino.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
                plot: str = '',             # Chart type: 'wordcloud'/'heatmap'/'line'
                ngram: int = '',            # N-gram size, 1 = unigram, 2 = bigram, 3 = trigram
                time_freq: str = '',        # Aggregation period: 'Y'/'M', if no aggregation: 'ungroup'
                max_words: int = '',        # Max number for most frequent n-grams displayed for each period
                numbers: bool = False,      # Remove numbers
                lower_case: bool = False):  # Lowercase text before cleaning and frequency analysis
 
-
     result = arabica_freq(text = text,
                           time = time,
                           date_format = date_format,
                           time_freq = time_freq,
                           max_words = max_words,
                           stopwords = stopwords,
                           skip = skip,
@@ -88,30 +87,31 @@
                 reshaped_unigram_max = reshaped_unigram.groupby(['unigram'], sort=False)['frequency'].max()
                 reshaped_unigram_max = reshaped_unigram_max.reset_index()
                 reshaped_unigram = reshaped_unigram.merge(reshaped_unigram_max, on = ['unigram','frequency'], how = 'left', indicator=True)
                 reshaped_unigram['label'] = np.where(reshaped_unigram['_merge']=='both', reshaped_unigram['unigram'], '')
                 reshaped_unigram = reshaped_unigram[['unigram', 'frequency', 'period','label']]
 
                 fig = (ggplot(reshaped_unigram, aes('period', 'unigram', fill='frequency'))
-                       + geom_tile(aes(width=.95, height=.95))
+                       + geom_tile(aes(width=1, height=1))
                        + geom_text(aes(label='frequency'), size=10)
                        + theme_minimal()
                        + scale_fill_gradient(name = "frequency",
                                              low = "#f0f4ed",
                                              high = "#496160")
                        + theme(axis_title_x=element_text(colour = "black"),
                                axis_title_y=element_text(colour="black"),
-                               axis_text_x=element_text(colour = "black", rotation=45, hjust=1),
-                               figure_size=(10, 5),
+                               axis_text_x=element_text(colour = "black", rotation=45, hjust= 1),
+                               legend_text = element_text(size = 7),
+                               legend_title = element_text(color = "black", vjust= -1.3, size = 10),
+                               figure_size= (3 + ((len(period) /4)), (3 + (max_words * 1.5))),
                                panel_grid_major = element_line(color='black',size = 0.1),
                                panel_background = element_rect(colour = "white", fill = "white"),
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
-
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
 
 
             elif plot == 'line':
                 reshaped_unigram_wide = pd.pivot(reshaped_unigram, index = 'unigram', columns = 'period', values = 'frequency')
                 reshaped_unigram_wide = reshaped_unigram_wide.fillna(0)
@@ -183,27 +183,29 @@
                 reshaped_unigram_max = reshaped_unigram.groupby(['unigram'], sort=False)['frequency'].max()
                 reshaped_unigram_max = reshaped_unigram_max.reset_index()
                 reshaped_unigram = reshaped_unigram.merge(reshaped_unigram_max, on = ['unigram','frequency'], how = 'left', indicator=True)
                 reshaped_unigram['label'] = np.where(reshaped_unigram['_merge']=='both', reshaped_unigram['unigram'], '')
                 reshaped_unigram = reshaped_unigram[['unigram', 'frequency', 'period','label']]
 
                 fig = (ggplot(reshaped_unigram, aes('period', 'unigram', fill='frequency'))
-                       + geom_tile(aes(width=.95, height=.95))
+                       + geom_tile(aes(width=0.95, height=0.95))
                        + geom_text(aes(label='frequency'), size=10)
                        + theme_minimal()
-                       + scale_fill_gradient(name = "frequency",
-                                             low = "#f0f4ed",
-                                             high = "#496160")
                        + theme(axis_title_x=element_text(colour = "black"),
                                axis_title_y=element_text(colour="black"),
-                               axis_text_x=element_text(colour = "black", rotation=45, hjust='1'),
-                               figure_size=(10, 6),
+                               axis_text_x=element_text(colour = "black", rotation=45, hjust= 1),
+                               legend_text = element_text(size = 7),
+                               legend_title = element_text(color = "black", size = 10),
+                               figure_size= (3 + ((len(period) /4)), (3 + (max_words * 0.5))),
                                panel_grid_major = element_line(color='black',size = 0.1),
                                panel_background = element_rect(colour = "white", fill = "white"),
                                plot_background = element_rect(colour = 'white',fill = "white"))
+                       + scale_fill_gradient(name = "frequency",
+                                             low = "#f0f4ed",
+                                             high = "#496160")
                        ).draw(show=False, return_ggplot=True)
 
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
 
             elif plot == 'line':
                 reshaped_unigram_wide = pd.pivot(reshaped_unigram, index = 'unigram', columns = 'period', values = 'frequency')
@@ -228,15 +230,15 @@
                                axis_title_y=element_text(colour="black", size = 7),
                                axis_title=element_text(face="bold"),
                                axis_text_x=element_text(colour = "black", rotation=45, hjust=1, size = 7),
                                legend_text = element_text(size=7),
                                legend_title = element_text(size=10),
                                legend_key_height = 0.5,
                                legend_key_width = 0.5,
-                               figure_size=(10, 5),
+                               figure_size=(2 + max_words, 5),
                                panel_grid_major = element_blank(),
                                panel_background = element_rect(colour = "white", fill = "white"),
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
 
                 plt.gcf().set_dpi(800)
@@ -307,18 +309,20 @@
                 fig = (ggplot(reshaped_unigram, aes('period', 'bigram', fill='frequency'))
                        + geom_tile(aes(width=.95, height=.95))
                        + geom_text(aes(label='frequency'), size=10)
                        + theme_minimal()
                        + scale_fill_gradient(name = "frequency",
                                              low = "#f0f4ed",
                                              high = "#496160")
-                       + theme(axis_title_x=element_text(colour = "black"),
+                       + theme(axis_title_x=element_text(colour = "black"), # TADY
                                axis_title_y=element_text(colour="black"),
-                               axis_text_x=element_text(colour = "black", rotation=45, hjust=1),
-                               figure_size=(10, 8),
+                               axis_text_x=element_text(colour = "black", rotation=45, hjust= 1),
+                               legend_text = element_text(size = 5,vjust = 0.2),
+                               legend_title = element_text(color = "black", vjust = 0.8, size = 10),
+                               figure_size= (3 + ((len(period) /4)), (2 + (max_words * 2.2))),
                                panel_grid_major = element_line(color='black',size = 0.1),
                                panel_background = element_rect(colour = "white", fill = "white"),
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
 
                 plt.gcf().set_dpi(800)
@@ -398,27 +402,28 @@
                 reshaped_unigram['label'] = np.where(reshaped_unigram['_merge']=='both', reshaped_unigram['bigram'], '')
                 reshaped_unigram = reshaped_unigram[['bigram', 'frequency', 'period','label']]
 
                 fig = (ggplot(reshaped_unigram, aes('period', 'bigram', fill='frequency'))
                        + geom_tile(aes(width=.95, height=.95))
                        + geom_text(aes(label='frequency'), size=10)
                        + theme_minimal()
-                       + scale_fill_gradient(name = "frequency",
-                                             low = "#f0f4ed",
-                                             high = "#496160")
                        + theme(axis_title_x=element_text(colour = "black"),
                                axis_title_y=element_text(colour="black"),
-                               axis_text_x=element_text(colour = "black", rotation=45, hjust=1),
-                               figure_size=(10, 8),
+                               axis_text_x=element_text(colour = "black", rotation=45, hjust= 1),
+                               legend_text = element_text(size = 5,vjust = 0.2),
+                               legend_title = element_text(color = "black", vjust = 0.8, size = 10),
+                               figure_size= (3 + ((len(period) /4)), (2 + (max_words * 1.7))),
                                panel_grid_major = element_line(color='black',size = 0.1),
                                panel_background = element_rect(colour = "white", fill = "white"),
                                plot_background = element_rect(colour = 'white',fill = "white"))
+                       + scale_fill_gradient(name = "frequency",
+                                             low = "#f0f4ed",
+                                             high = "#496160")
                        ).draw(show=False, return_ggplot=True)
 
-
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
 
 
             elif plot == 'line':
                 reshaped_unigram_wide = pd.pivot(reshaped_unigram, index = 'bigram', columns = 'period', values = 'frequency')
                 reshaped_unigram_wide = reshaped_unigram_wide.fillna(0)
@@ -443,15 +448,15 @@
                                axis_title_y=element_text(colour="black", size = 7),
                                axis_title=element_text(face="bold"),
                                axis_text_x=element_text(colour = "black", rotation=45, hjust=1, size = 7),
                                legend_text = element_text(size=7),
                                legend_title = element_text(size=10),
                                legend_key_height = 0.5,
                                legend_key_width = 0.5,
-                               figure_size=(10, 5),
+                               figure_size=(7 + (max_words * 0.8), 5),
                                panel_grid_major = element_blank(),
                                panel_background = element_rect(colour = "white", fill = "white"),
                                plot_background = element_rect(colour = 'white',fill = "white"))
                        ).draw(show=False, return_ggplot=True)
 
                 plt.gcf().set_dpi(800)
                 picture = plt.show()
@@ -489,8 +494,9 @@
 
         else:
             sys.exit('Incorrect value for time_freq parameter. Allowed: "ungroup"')
 
     else:
         sys.exit("Incorrect value for ngram parameter. Allowed: 1,2,3.")
 
-    return picture
+    return picture
+#%%
```

### Comparing `arabica-1.6.3/arabica/clean_ngram.py` & `arabica-1.6.4/arabica/clean_ngram.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.3/arabica/coffee_break.py` & `arabica-1.6.4/arabica/coffee_break.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.3/arabica/group.py` & `arabica-1.6.4/arabica/group.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.3/arabica/preprocess.py` & `arabica-1.6.4/arabica/preprocess.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.3/arabica/sentiment.py` & `arabica-1.6.4/arabica/sentiment.py`

 * *Files identical despite different names*

### Comparing `arabica-1.6.3/arabica.egg-info/PKG-INFO` & `arabica-1.6.4/arabica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arabica
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python package for exploratory text data analysis
 Home-page: https://github.com/PetrKorab/Arabica
 Author: Petr Koráb
 Author-email: Petr Korab <xpetrkorab@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/PetrKorab/Arabica
 Project-URL: Bug Tracker, https://github.com/PetrKorab/Arabica/issues
```

### Comparing `arabica-1.6.3/pyproject.toml` & `arabica-1.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "arabica"
-version = "1.6.3"
+version = "1.6.4"
 authors = [
   { name="Petr Korab", email="xpetrkorab@gmail.com" },
 ]
 description = "Python package for exploratory text data analysis"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8, !=3.11"
```

### Comparing `arabica-1.6.3/setup.py` & `arabica-1.6.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
     setuptools.setup(
         name="arabica",
-        version="1.6.3",
+        version="1.6.4",
         author="Petr Koráb",
         author_email="xpetrkorab@gmail.com",
         packages=["arabica"],
         description="Python package for exploratory text data analysis",
         long_description=description,
         long_description_content_type="text/markdown",
         url="https://github.com/PetrKorab/Arabica",
         python_requires='>=3.8, !=3.11',
         install_requires = ['pandas >=1.4.0',
                             'nltk == 3.6.2',
-                            'regex',
+                            'regex == 2022.10.31',
                             'finvader',
                             'matplotlib == 3.6.0',
                             'matplotlib-inline == 0.1.6',
                             'plotnine == 0.10.1',
                             'wordcloud == 1.8.2.2',
                             'jenkspy == 0.3.2',
                             'vaderSentiment == 3.3.2',
```

