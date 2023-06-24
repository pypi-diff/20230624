# Comparing `tmp/pwl_writer-1.1.0.tar.gz` & `tmp/pwl_writer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl_writer-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pwl_writer-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pwl_writer-1.1.0.tar` & `pwl_writer-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1497 2023-06-23 13:23:50.038539 pwl_writer-1.1.0/.gitignore
--rw-r--r--   0        0        0     1111 2023-06-23 12:40:45.054972 pwl_writer-1.1.0/LICENSE
--rw-r--r--   0        0        0     3934 2023-06-24 11:49:16.390169 pwl_writer-1.1.0/README.md
--rw-r--r--   0        0        0   167381 2023-06-24 11:47:54.591001 pwl_writer-1.1.0/docs/pwl_writer.html
--rw-r--r--   0        0        0     7070 2023-06-24 11:47:54.296800 pwl_writer-1.1.0/docs/pycco.css
--rw-r--r--   0        0        0      184 2023-06-24 11:50:37.701578 pwl_writer-1.1.0/pwl_writer/__init__.py
--rw-r--r--   0        0        0    43854 2023-06-24 11:47:51.787460 pwl_writer-1.1.0/pwl_writer/pwl_writer.py
--rw-r--r--   0        0        0      685 2023-06-24 11:51:38.147038 pwl_writer-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 pwl_writer-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-23 13:23:50.038539 pwl_writer-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1111 2023-06-23 12:40:45.054972 pwl_writer-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3934 2023-06-24 11:49:16.390169 pwl_writer-1.1.1/README.md
+-rw-r--r--   0        0        0   168194 2023-06-24 12:06:32.205647 pwl_writer-1.1.1/docs/pwl_writer.html
+-rw-r--r--   0        0        0     7070 2023-06-24 12:06:31.890674 pwl_writer-1.1.1/docs/pycco.css
+-rw-r--r--   0        0        0      184 2023-06-24 12:05:23.141586 pwl_writer-1.1.1/pwl_writer/__init__.py
+-rw-r--r--   0        0        0    44085 2023-06-24 12:05:36.194808 pwl_writer-1.1.1/pwl_writer/pwl_writer.py
+-rw-r--r--   0        0        0      685 2023-06-24 11:51:38.147038 pwl_writer-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 pwl_writer-1.1.1/PKG-INFO
```

### Comparing `pwl_writer-1.1.0/.gitignore` & `pwl_writer-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.0/LICENSE` & `pwl_writer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.0/README.md` & `pwl_writer-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.0/docs/pwl_writer.html` & `pwl_writer-1.1.1/docs/pwl_writer.html`

 * *Files 0% similar despite different names*

```diff
@@ -1653,22 +1653,27 @@
 <p>Class method that takes all instances of the <code>PWL</code> class and plots them on the same time axis.</p>
 <h3>Arguments</h3>
 <ul>
 <li><code>merge</code> (<code>bool</code>, optional) : Flag indicating if all signals should be ploted on the same strip or separeted. If not set, defaults to False.</li>
 </ul>
 <h3>Raises</h3>
 <ul>
+<li><code>TypeError</code> : Raised if <code>merge</code> is not a boolean.</li>
 <li><code>ImportError</code> : Raised if the matplotlib package is not installed.</li>
 </ul>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="n">_has_matplotlib</span><span class="p">:</span>
             <span class="k">raise</span> <span class="ne">ImportError</span><span class="p">(</span>
                 <span class="s2">&quot;Optional features are deactivated. Install matplotlib to use.&quot;</span><span class="p">)</span>
 
+        <span class="k">if</span> <span class="ow">not</span> <span class="nb">isinstance</span><span class="p">(</span><span class="n">merge</span><span class="p">,</span> <span class="nb">bool</span><span class="p">):</span>
+            <span class="k">raise</span> <span class="ne">TypeError</span><span class="p">(</span>
+                <span class="sa">f</span><span class="s2">&quot;Argument &#39;merge&#39; should be a boolean but has type &#39;</span><span class="si">{</span><span class="nb">type</span><span class="p">(</span><span class="n">merge</span><span class="p">)</span><span class="o">.</span><span class="vm">__name__</span><span class="si">}</span><span class="s2">&#39;.&quot;</span><span class="p">)</span>
+
         <span class="n">dict_of_objects</span> <span class="o">=</span> <span class="bp">cls</span><span class="o">.</span><span class="n">__dict_of_objects</span>
 
         <span class="k">if</span> <span class="ow">not</span> <span class="n">dict_of_objects</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">None</span>
 
         <span class="k">if</span> <span class="n">merge</span><span class="p">:</span>
             <span class="n">fig</span><span class="p">,</span> <span class="n">axs</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">subplots</span><span class="p">(</span><span class="n">nrows</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">sharex</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">squeeze</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
```

#### html2text {}

```diff
@@ -941,20 +941,26 @@
 **** Summary ****
 Class method that takes all instances of the PWL class and plots them on the
 same time axis.
 **** Arguments ****
     * merge (bool, optional) : Flag indicating if all signals should be ploted
       on the same strip or separeted. If not set, defaults to False.
 **** Raises ****
+    * TypeError : Raised if merge is not a boolean.
     * ImportError : Raised if the matplotlib package is not installed.
         if not _has_matplotlib:
             raise ImportError(
                 "Optional features are deactivated. Install matplotlib to
 use.")
 
+        if not isinstance(merge, bool):
+            raise TypeError(
+                f"Argument 'merge' should be a boolean but has type '{type
+(merge).__name__}'.")
+
         dict_of_objects = cls.__dict_of_objects
 
         if not dict_of_objects:
             return None
 
         if merge:
             fig, axs = plt.subplots(nrows=1, sharex=True, squeeze=False)
```

### Comparing `pwl_writer-1.1.0/docs/pycco.css` & `pwl_writer-1.1.1/docs/pycco.css`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.0/pwl_writer/pwl_writer.py` & `pwl_writer-1.1.1/pwl_writer/pwl_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -943,21 +943,26 @@
 
         ### Arguments
 
         * `merge` (`bool`, optional) : Flag indicating if all signals should be ploted on the same strip or separeted. If not set, defaults to False.
 
         ### Raises
 
+        * `TypeError` : Raised if `merge` is not a boolean.
         * `ImportError` : Raised if the matplotlib package is not installed.
         """
 
         if not _has_matplotlib:
             raise ImportError(
                 "Optional features are deactivated. Install matplotlib to use.")
 
+        if not isinstance(merge, bool):
+            raise TypeError(
+                f"Argument 'merge' should be a boolean but has type '{type(merge).__name__}'.")
+
         dict_of_objects = cls.__dict_of_objects
 
         if not dict_of_objects:
             return None
 
         if merge:
             fig, axs = plt.subplots(nrows=1, sharex=True, squeeze=False)
```

### Comparing `pwl_writer-1.1.0/pyproject.toml` & `pwl_writer-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.1.0/PKG-INFO` & `pwl_writer-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwl_writer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Package to generate PWL incrementally using little 'events' like rectangular pulses and exponential rising or falling edges.
 Author-email: "Victor Sabiá P. Carpes" <victorscarpes@gmail.com>
 Requires-Python: >=3.6.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy
 Requires-Dist: pycco ; extra == "doc"
```

