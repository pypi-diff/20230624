# Comparing `tmp/pwl_writer-1.0.0.tar.gz` & `tmp/pwl_writer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwl_writer-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pwl_writer-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pwl_writer-1.0.0.tar` & `pwl_writer-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1497 2023-06-23 13:23:50.038539 pwl_writer-1.0.0/.gitignore
--rw-r--r--   0        0        0     1111 2023-06-23 12:40:45.054972 pwl_writer-1.0.0/LICENSE
--rw-r--r--   0        0        0     3911 2023-06-23 13:37:30.640689 pwl_writer-1.0.0/README.md
--rw-r--r--   0        0        0   159569 2023-06-23 13:12:43.607017 pwl_writer-1.0.0/docs/pwl_writer.html
--rw-r--r--   0        0        0     7070 2023-06-23 13:12:43.437701 pwl_writer-1.0.0/docs/pycco.css
--rw-r--r--   0        0        0      184 2023-06-23 13:15:48.492071 pwl_writer-1.0.0/pwl_writer/__init__.py
--rw-r--r--   0        0        0    41934 2023-06-23 13:07:21.783945 pwl_writer-1.0.0/pwl_writer/pwl_writer.py
--rw-r--r--   0        0        0     1027 2023-06-23 13:10:47.769030 pwl_writer-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      376 2023-06-23 09:23:47.134006 pwl_writer-1.0.0/setup.py
--rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 pwl_writer-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-06-23 13:23:50.038539 pwl_writer-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1111 2023-06-23 12:40:45.054972 pwl_writer-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3934 2023-06-24 11:49:16.390169 pwl_writer-1.1.0/README.md
+-rw-r--r--   0        0        0   167381 2023-06-24 11:47:54.591001 pwl_writer-1.1.0/docs/pwl_writer.html
+-rw-r--r--   0        0        0     7070 2023-06-24 11:47:54.296800 pwl_writer-1.1.0/docs/pycco.css
+-rw-r--r--   0        0        0      184 2023-06-24 11:50:37.701578 pwl_writer-1.1.0/pwl_writer/__init__.py
+-rw-r--r--   0        0        0    43854 2023-06-24 11:47:51.787460 pwl_writer-1.1.0/pwl_writer/pwl_writer.py
+-rw-r--r--   0        0        0      685 2023-06-24 11:51:38.147038 pwl_writer-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4588 1970-01-01 00:00:00.000000 pwl_writer-1.1.0/PKG-INFO
```

### Comparing `pwl_writer-1.0.0/.gitignore` & `pwl_writer-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.0.0/LICENSE` & `pwl_writer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.0.0/README.md` & `pwl_writer-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 # pwl_writer
 
 *by Victor Sabiá P. Carpes*
 
-Tested on python version `3.6.6` with numpy version `1.19.5` and python version `3.11.1` with numpy version `1.25.0`. Type stubs for older numpy versions for mypy checking can be found [here](https://github.com/numpy/numpy-stubs).
+Tested on:
+
+* python `3.6.6`
+  * numpy `1.19.5`
+  * matplotlib `3.3.4`
+* python `3.11.1`
+  * numpy `1.25.0`
+  * matplotlib `3.7.1`
+
+Type stubs for older numpy versions for mypy checking can be found [here](https://github.com/numpy/numpy-stubs).
 
 ## Summary
 
 This package defines a class `PWL` to generate objects that represent time dependent signals $x(t)$ that need to be coded in a PWL file. Those objects are built using little components such as rectangular pulses and sawtooth pulses that can be chained together.
 
 ## Motivation
```

### Comparing `pwl_writer-1.0.0/docs/pwl_writer.html` & `pwl_writer-1.1.0/docs/pwl_writer.html`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,28 @@
   <div class='clearall'>
   <div class='section' id='section-0'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-0'>#</a>
       </div>
       <p><em>by Victor Sabiá P. Carpes</em></p>
-<p>Tested on python version <code>3.6.6</code> with numpy version <code>1.19.5</code> and python version <code>3.11.1</code> with numpy version <code>1.25.0</code>. Type stubs for older numpy versions for mypy checking can be found <a href="https://github.com/numpy/numpy-stubs">here</a>.</p>
+<p>Tested on:</p>
+<ul>
+<li>python <code>3.6.6</code><ul>
+<li>numpy <code>1.19.5</code></li>
+<li>matplotlib <code>3.3.4</code></li>
+</ul>
+</li>
+<li>python <code>3.11.1</code><ul>
+<li>numpy <code>1.25.0</code></li>
+<li>matplotlib <code>3.7.1</code></li>
+</ul>
+</li>
+</ul>
+<p>Type stubs for older numpy versions for mypy checking can be found <a href="https://github.com/numpy/numpy-stubs">here</a>.</p>
 <hr />
 <h1>Index</h1>
 <ul>
 <li><a href="#package-summary">Package Summary</a></li>
 <li><a href="#precision-related-exception">Precision Related Exception</a></li>
 <li><a href="#pwl-class">PWL Class</a><ul>
 <li>Dunder Methods<ul>
@@ -44,14 +57,15 @@
 <li><a href="#linear-transition">Linear Transition</a></li>
 <li><a href="#rectangular-pulse">Rectangular Pulse</a></li>
 <li><a href="#sawtooth-pulse">Sawtooth Pulse</a></li>
 <li><a href="#exponential-transition">Exponential Transition</a></li>
 <li><a href="#half-sine-transition">Half Sine Transition</a></li>
 <li><a href="#smoothstep-transition">Smoothstep Transition</a></li>
 <li><a href="#pwl-file-writer">PWL File Writer</a></li>
+<li><a href="#pwl-plotter">PWL Plotter</a> <em>(optional feature: requires matplotlib)</em></li>
 </ul>
 </li>
 <li>Private Methods <em>(minimal documentation)</em><ul>
 <li><a href="#pwl-point-adder">PWL Point Adder</a></li>
 <li><a href="#colinear-points-eliminator">Colinear Points Eliminator</a></li>
 <li><a href="#nested-linear-transition">Nested Linear Transition</a></li>
 </ul>
@@ -98,17 +112,26 @@
    idle_state(1)
    mode2_state(5)
 </code></pre>
     </div>
     <div class='code'>
       <div class="highlight"><pre><span></span><span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s1">&#39;PrecisionError&#39;</span><span class="p">,</span> <span class="s1">&#39;PWL&#39;</span><span class="p">]</span>
 
+<span class="kn">from</span> <span class="nn">warnings</span> <span class="kn">import</span> <span class="n">warn</span>
 <span class="kn">from</span> <span class="nn">numbers</span> <span class="kn">import</span> <span class="n">Real</span>
 <span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">Callable</span><span class="p">,</span> <span class="n">Dict</span><span class="p">,</span> <span class="n">List</span><span class="p">,</span> <span class="n">Optional</span>
-<span class="kn">import</span> <span class="nn">numpy</span></pre></div>
+<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
+
+<span class="k">try</span><span class="p">:</span>
+    <span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>  <span class="c1"># type: ignore</span>
+<span class="k">except</span> <span class="ne">ImportError</span><span class="p">:</span>
+    <span class="n">_has_matplotlib</span> <span class="o">=</span> <span class="kc">False</span>
+    <span class="n">warn</span><span class="p">(</span><span class="s2">&quot;Matplotlib package not found. Optional features deactivated.&quot;</span><span class="p">,</span> <span class="ne">ImportWarning</span><span class="p">)</span>
+<span class="k">else</span><span class="p">:</span>
+    <span class="n">_has_matplotlib</span> <span class="o">=</span> <span class="kc">True</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-1'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-1'>#</a>
@@ -1235,15 +1258,15 @@
 
         <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">last_x</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
 
         <span class="n">f</span> <span class="o">=</span> <span class="n">_exp_transition_func</span><span class="p">(</span><span class="n">tau</span><span class="o">=</span><span class="n">tau</span><span class="p">,</span> <span class="n">t1</span><span class="o">=</span><span class="n">last_t</span><span class="p">,</span> <span class="n">t2</span><span class="o">=</span><span class="n">last_t</span> <span class="o">+</span>
                                  <span class="n">duration</span><span class="p">,</span> <span class="n">f1</span><span class="o">=</span><span class="n">last_x</span><span class="p">,</span> <span class="n">f2</span><span class="o">=</span><span class="n">target</span><span class="p">)</span>
 
-        <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">numpy</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
+        <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-64'>
@@ -1355,15 +1378,15 @@
 
         <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">last_x</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
 
         <span class="n">f</span> <span class="o">=</span> <span class="n">_sin_transition_func</span><span class="p">(</span>
             <span class="n">t1</span><span class="o">=</span><span class="n">last_t</span><span class="p">,</span> <span class="n">t2</span><span class="o">=</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">f1</span><span class="o">=</span><span class="n">last_x</span><span class="p">,</span> <span class="n">f2</span><span class="o">=</span><span class="n">target</span><span class="p">)</span>
 
-        <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">numpy</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
+        <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-68'>
@@ -1474,15 +1497,15 @@
 
         <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">last_x</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
 
         <span class="n">f</span> <span class="o">=</span> <span class="n">_smoothstep_transition_func</span><span class="p">(</span>
             <span class="n">t1</span><span class="o">=</span><span class="n">last_t</span><span class="p">,</span> <span class="n">t2</span><span class="o">=</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">f1</span><span class="o">=</span><span class="n">last_x</span><span class="p">,</span> <span class="n">f2</span><span class="o">=</span><span class="n">target</span><span class="p">)</span>
 
-        <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">numpy</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
+        <span class="k">for</span> <span class="n">t</span> <span class="ow">in</span> <span class="n">np</span><span class="o">.</span><span class="n">arange</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">t_step</span><span class="p">,</span> <span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">t_step</span><span class="p">):</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">t</span><span class="p">,</span> <span class="n">f</span><span class="p">(</span><span class="n">t</span><span class="p">))</span>
 
         <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-72'>
@@ -1559,24 +1582,24 @@
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
             <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">: Writing PWL file to </span><span class="si">{</span><span class="n">filename</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 
         <span class="n">t_list</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span>
         <span class="n">x_list</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span>
 
         <span class="k">with</span> <span class="nb">open</span><span class="p">(</span><span class="n">filename</span><span class="p">,</span> <span class="s2">&quot;w&quot;</span><span class="p">)</span> <span class="k">as</span> <span class="n">file</span><span class="p">:</span>
-            <span class="n">ti_str</span> <span class="o">=</span> <span class="n">numpy</span><span class="o">.</span><span class="n">format_float_scientific</span><span class="p">(</span>
+            <span class="n">ti_str</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">format_float_scientific</span><span class="p">(</span>
                 <span class="n">t_list</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">precision</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="n">unique</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">sign</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-            <span class="n">xi_str</span> <span class="o">=</span> <span class="n">numpy</span><span class="o">.</span><span class="n">format_float_scientific</span><span class="p">(</span>
+            <span class="n">xi_str</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">format_float_scientific</span><span class="p">(</span>
                 <span class="n">x_list</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">precision</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="n">unique</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">sign</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
             <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">ti_str</span><span class="si">}</span><span class="s2">    </span><span class="si">{</span><span class="n">xi_str</span><span class="si">}</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
             <span class="n">last_t</span> <span class="o">=</span> <span class="n">ti_str</span>
             <span class="k">for</span> <span class="n">ti</span><span class="p">,</span> <span class="n">xi</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">t_list</span><span class="p">[</span><span class="mi">1</span><span class="p">:],</span> <span class="n">x_list</span><span class="p">[</span><span class="mi">1</span><span class="p">:]):</span>
-                <span class="n">ti_str</span> <span class="o">=</span> <span class="n">numpy</span><span class="o">.</span><span class="n">format_float_scientific</span><span class="p">(</span>
+                <span class="n">ti_str</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">format_float_scientific</span><span class="p">(</span>
                     <span class="n">ti</span><span class="p">,</span> <span class="n">precision</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="n">unique</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">sign</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
-                <span class="n">xi_str</span> <span class="o">=</span> <span class="n">numpy</span><span class="o">.</span><span class="n">format_float_scientific</span><span class="p">(</span>
+                <span class="n">xi_str</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">format_float_scientific</span><span class="p">(</span>
                     <span class="n">xi</span><span class="p">,</span> <span class="n">precision</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="n">unique</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> <span class="n">sign</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
                 <span class="k">if</span> <span class="n">ti_str</span> <span class="o">==</span> <span class="n">last_t</span><span class="p">:</span>
                     <span class="k">raise</span> <span class="n">PrecisionError</span><span class="p">(</span>
                         <span class="s2">&quot;The chosen precision level caused the written time coordinates to not be strictly increasing.&quot;</span><span class="p">)</span>
                 <span class="n">file</span><span class="o">.</span><span class="n">write</span><span class="p">(</span>
                     <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">ti_str</span><span class="si">}</span><span class="s2">    </span><span class="si">{</span><span class="n">xi_str</span><span class="si">}</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
                 <span class="n">last_t</span> <span class="o">=</span> <span class="n">ti_str</span></pre></div>
@@ -1596,74 +1619,149 @@
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-77'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-77'>#</a>
       </div>
-      <h1><span id="private-methods-and-functions" href="private-methods-and-functions"> Private Methods and Functions </span></h1>
+      <h2><span id="pwl-plotter" href="pwl-plotter"> PWL Plotter </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-78'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-78'>#</a>
       </div>
-      <p>From this point forward, all listed methods and functions are not intended to be used by the user. Brief descriptions will be provided, but documentation will be kept to a minimum.</p>
+      <p><strong><code>plot</code> class method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre></pre></div>
+      <div class="highlight"><pre>    <span class="nd">@classmethod</span>
+    <span class="k">def</span> <span class="nf">plot</span><span class="p">(</span><span class="bp">cls</span><span class="p">,</span> <span class="n">merge</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-79'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-79'>#</a>
       </div>
-      <hr />
+      <p><em>Optional feature: Requires matplotlib</em></p>
+<h3>Summary</h3>
+<p>Class method that takes all instances of the <code>PWL</code> class and plots them on the same time axis.</p>
+<h3>Arguments</h3>
+<ul>
+<li><code>merge</code> (<code>bool</code>, optional) : Flag indicating if all signals should be ploted on the same strip or separeted. If not set, defaults to False.</li>
+</ul>
+<h3>Raises</h3>
+<ul>
+<li><code>ImportError</code> : Raised if the matplotlib package is not installed.</li>
+</ul>
     </div>
     <div class='code'>
-      <div class="highlight"><pre></pre></div>
+      <div class="highlight"><pre>        <span class="k">if</span> <span class="ow">not</span> <span class="n">_has_matplotlib</span><span class="p">:</span>
+            <span class="k">raise</span> <span class="ne">ImportError</span><span class="p">(</span>
+                <span class="s2">&quot;Optional features are deactivated. Install matplotlib to use.&quot;</span><span class="p">)</span>
+
+        <span class="n">dict_of_objects</span> <span class="o">=</span> <span class="bp">cls</span><span class="o">.</span><span class="n">__dict_of_objects</span>
+
+        <span class="k">if</span> <span class="ow">not</span> <span class="n">dict_of_objects</span><span class="p">:</span>
+            <span class="k">return</span> <span class="kc">None</span>
+
+        <span class="k">if</span> <span class="n">merge</span><span class="p">:</span>
+            <span class="n">fig</span><span class="p">,</span> <span class="n">axs</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">subplots</span><span class="p">(</span><span class="n">nrows</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">sharex</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">squeeze</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+            <span class="n">axs</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">repeat</span><span class="p">(</span><span class="n">axs</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">dict_of_objects</span><span class="p">))</span>
+        <span class="k">else</span><span class="p">:</span>
+            <span class="n">fig</span><span class="p">,</span> <span class="n">axs</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">subplots</span><span class="p">(</span>
+                <span class="n">nrows</span><span class="o">=</span><span class="nb">len</span><span class="p">(</span><span class="n">dict_of_objects</span><span class="p">),</span> <span class="n">sharex</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">squeeze</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
+            <span class="n">axs</span> <span class="o">=</span> <span class="n">axs</span><span class="o">.</span><span class="n">flatten</span><span class="p">()</span>
+        <span class="n">x_max</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">0</span>
+
+        <span class="k">for</span> <span class="n">key</span><span class="p">,</span> <span class="n">ax</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">dict_of_objects</span><span class="p">,</span> <span class="n">axs</span><span class="p">):</span>
+            <span class="n">pwl</span> <span class="o">=</span> <span class="n">dict_of_objects</span><span class="p">[</span><span class="n">key</span><span class="p">]</span>
+            <span class="n">x_list</span> <span class="o">=</span> <span class="n">pwl</span><span class="o">.</span><span class="n">t_list</span>
+            <span class="n">x_max</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="n">x_max</span><span class="p">,</span> <span class="nb">max</span><span class="p">(</span><span class="n">x_list</span><span class="p">))</span>
+            <span class="n">y_list</span> <span class="o">=</span> <span class="n">pwl</span><span class="o">.</span><span class="n">x_list</span>
+            <span class="n">label</span> <span class="o">=</span> <span class="n">pwl</span><span class="o">.</span><span class="n">name</span>
+            <span class="n">ax</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">x_list</span><span class="p">,</span> <span class="n">y_list</span><span class="p">)</span>
+            <span class="n">ax</span><span class="o">.</span><span class="n">set_ylabel</span><span class="p">(</span><span class="n">label</span><span class="p">)</span>
+
+        <span class="n">axs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">set_xlim</span><span class="p">(</span><span class="n">xmin</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">xmax</span><span class="o">=</span><span class="n">x_max</span><span class="p">)</span>
+        <span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-80'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-80'>#</a>
       </div>
-      <h2><span id="pwl-point-adder" href="pwl-point-adder"> PWL Point Adder </span></h2>
+      <h1><span id="private-methods-and-functions" href="private-methods-and-functions"> Private Methods and Functions </span></h1>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-81'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-81'>#</a>
       </div>
-      <p><strong><code>_add</code> private method of <code>PWL</code> class</strong></p>
+      <p>From this point forward, all listed methods and functions are not intended to be used by the user. Brief descriptions will be provided, but documentation will be kept to a minimum.</p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">x</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
+      <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
   <div class='section' id='section-82'>
     <div class='docs'>
       <div class='octowrap'>
         <a class='octothorpe' href='#section-82'>#</a>
       </div>
+      <hr />
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-83'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-83'>#</a>
+      </div>
+      <h2><span id="pwl-point-adder" href="pwl-point-adder"> PWL Point Adder </span></h2>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-84'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-84'>#</a>
+      </div>
+      <p><strong><code>_add</code> private method of <code>PWL</code> class</strong></p>
+    </div>
+    <div class='code'>
+      <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">x</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
+    </div>
+  </div>
+  <div class='clearall'></div>
+  <div class='section' id='section-85'>
+    <div class='docs'>
+      <div class='octowrap'>
+        <a class='octothorpe' href='#section-85'>#</a>
+      </div>
       <p>Private method that adds a <code>(t, x)</code> point to a <code>PWL</code> object of any size.</p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">)</span> <span class="o">&gt;=</span> <span class="mi">1</span> <span class="ow">and</span> <span class="n">t</span> <span class="o">&lt;=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]:</span>
             <span class="k">raise</span> <span class="n">PrecisionError</span><span class="p">(</span>
                 <span class="sa">f</span><span class="s2">&quot;Internal Python rounding caused the time coordinates to not be strictly increasing when adding points to </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_name</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
 
@@ -1671,54 +1769,54 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">t</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">x</span><span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_colinear_eliminator</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">t</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-83'>
+  <div class='section' id='section-86'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-83'>#</a>
+        <a class='octothorpe' href='#section-86'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-84'>
+  <div class='section' id='section-87'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-84'>#</a>
+        <a class='octothorpe' href='#section-87'>#</a>
       </div>
       <h2><span id="colinear-points-eliminator" href="colinear-points-eliminator"> Colinear Points Eliminator </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-85'>
+  <div class='section' id='section-88'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-85'>#</a>
+        <a class='octothorpe' href='#section-88'>#</a>
       </div>
       <p><strong><code>_colinear_eliminator</code> private method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_colinear_eliminator</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">x</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-86'>
+  <div class='section' id='section-89'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-86'>#</a>
+        <a class='octothorpe' href='#section-89'>#</a>
       </div>
       <p>Private method that adds a <code>(t, x)</code> point to a <code>PWL</code> object with 2 or more points without consecutive colinear points.</p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="n">t_n_1</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="n">t_n_2</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">2</span><span class="p">]</span>
 
@@ -1733,54 +1831,54 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span> <span class="o">=</span> <span class="n">x</span>
         <span class="k">else</span><span class="p">:</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">t</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_x_list</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">x</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-87'>
+  <div class='section' id='section-90'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-87'>#</a>
+        <a class='octothorpe' href='#section-90'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-88'>
+  <div class='section' id='section-91'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-88'>#</a>
+        <a class='octothorpe' href='#section-91'>#</a>
       </div>
       <h2><span id="nested-linear-transition" href="nested-linear-transition"> Nested Linear Transition </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-89'>
+  <div class='section' id='section-92'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-89'>#</a>
+        <a class='octothorpe' href='#section-92'>#</a>
       </div>
       <p><strong><code>_lin_transition</code> private method of <code>PWL</code> class</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">_lin_transition</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">target</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">duration</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">n</span><span class="p">:</span> <span class="nb">int</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="kc">None</span><span class="p">:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-90'>
+  <div class='section' id='section-93'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-90'>#</a>
+        <a class='octothorpe' href='#section-93'>#</a>
       </div>
       <p>Private method to generate a linear transition. The difference between this method and the <a href="#linear-transition">public linear transition</a> method is that this method prints indented verbose output when called from within any of the public methods that revert to a linear transition in certain conditions.</p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_verbose</span><span class="p">:</span>
             <span class="k">if</span> <span class="n">n</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
                 <span class="nb">print</span><span class="p">(</span>
@@ -1795,236 +1893,242 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span>
 
         <span class="n">last_t</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_t_list</span><span class="p">[</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">_add</span><span class="p">(</span><span class="n">last_t</span><span class="o">+</span><span class="n">duration</span><span class="p">,</span> <span class="n">target</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-91'>
+  <div class='section' id='section-94'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-91'>#</a>
+        <a class='octothorpe' href='#section-94'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-92'>
+  <div class='section' id='section-95'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-92'>#</a>
+        <a class='octothorpe' href='#section-95'>#</a>
       </div>
       <h2><span id="exponential-function-generator" href="exponential-function-generator"> Exponential Function Generator </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-93'>
+  <div class='section' id='section-96'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-93'>#</a>
+        <a class='octothorpe' href='#section-96'>#</a>
       </div>
       <p><strong><code>_exp_transition_func</code> private function</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre><span class="k">def</span> <span class="nf">_exp_transition_func</span><span class="p">(</span><span class="n">tau</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-94'>
+  <div class='section' id='section-97'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-94'>#</a>
+        <a class='octothorpe' href='#section-97'>#</a>
       </div>
       <p>Private function that generates an exponential function passing trough 2 fixed points.</p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="n">A</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span><span class="o">*</span><span class="n">numpy</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">f2</span><span class="o">*</span><span class="n">numpy</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span> <span class="o">/</span> \
-        <span class="p">(</span><span class="n">numpy</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">numpy</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span>
-    <span class="n">B</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span> <span class="o">-</span> <span class="n">f2</span><span class="p">)</span><span class="o">/</span><span class="p">(</span><span class="n">numpy</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">numpy</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span></pre></div>
+      <div class="highlight"><pre>    <span class="n">A</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">f2</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span> <span class="o">/</span> \
+        <span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span>
+    <span class="n">B</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span> <span class="o">-</span> <span class="n">f2</span><span class="p">)</span><span class="o">/</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t1</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span> <span class="o">-</span> <span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t2</span><span class="o">/</span><span class="n">tau</span><span class="p">))</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-95'>
+  <div class='section' id='section-98'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-95'>#</a>
+        <a class='octothorpe' href='#section-98'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">f</span><span class="p">(</span><span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-        <span class="n">result</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">A</span> <span class="o">+</span> <span class="n">B</span><span class="o">*</span><span class="n">numpy</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span>
+        <span class="n">result</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">A</span> <span class="o">+</span> <span class="n">B</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">exp</span><span class="p">(</span><span class="o">-</span><span class="n">t</span><span class="o">/</span><span class="n">tau</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">result</span>
 
     <span class="k">return</span> <span class="n">f</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-96'>
+  <div class='section' id='section-99'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-96'>#</a>
+        <a class='octothorpe' href='#section-99'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-97'>
+  <div class='section' id='section-100'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-97'>#</a>
+        <a class='octothorpe' href='#section-100'>#</a>
       </div>
       <h2><span id="sinusoidal-function-generator" href="sinusoidal-function-generator"> Sinusoidal Function Generator </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-98'>
+  <div class='section' id='section-101'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-98'>#</a>
+        <a class='octothorpe' href='#section-101'>#</a>
       </div>
       <p><strong><code>_sin_transition_func</code> private function</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre><span class="k">def</span> <span class="nf">_sin_transition_func</span><span class="p">(</span><span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-99'>
+  <div class='section' id='section-102'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-99'>#</a>
+        <a class='octothorpe' href='#section-102'>#</a>
       </div>
       <p>Private function that generates a sinusoidal function passing trough 2 fixed points.</p>
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="n">fm</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">f1</span><span class="o">+</span><span class="n">f2</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span>
     <span class="n">tm</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="p">(</span><span class="n">t1</span><span class="o">+</span><span class="n">t2</span><span class="p">)</span><span class="o">/</span><span class="mi">2</span>
     <span class="n">T</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">2</span><span class="o">*</span><span class="p">(</span><span class="n">t2</span><span class="o">-</span><span class="n">t1</span><span class="p">)</span>
-    <span class="n">w</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">2</span><span class="o">*</span><span class="n">numpy</span><span class="o">.</span><span class="n">pi</span><span class="o">/</span><span class="n">T</span>
+    <span class="n">w</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="mi">2</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">pi</span><span class="o">/</span><span class="n">T</span>
     <span class="n">phi</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">w</span><span class="o">*</span><span class="n">tm</span>
     <span class="n">A</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">f2</span><span class="o">-</span><span class="n">fm</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-100'>
+  <div class='section' id='section-103'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-100'>#</a>
+        <a class='octothorpe' href='#section-103'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">f</span><span class="p">(</span><span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
-        <span class="n">result</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">fm</span> <span class="o">+</span> <span class="n">A</span><span class="o">*</span><span class="n">numpy</span><span class="o">.</span><span class="n">sin</span><span class="p">(</span><span class="n">w</span><span class="o">*</span><span class="n">t</span> <span class="o">-</span> <span class="n">phi</span><span class="p">)</span>
+        <span class="n">result</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">fm</span> <span class="o">+</span> <span class="n">A</span><span class="o">*</span><span class="n">np</span><span class="o">.</span><span class="n">sin</span><span class="p">(</span><span class="n">w</span><span class="o">*</span><span class="n">t</span> <span class="o">-</span> <span class="n">phi</span><span class="p">)</span>
         <span class="k">return</span> <span class="n">result</span>
 
     <span class="k">return</span> <span class="n">f</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-101'>
+  <div class='section' id='section-104'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-101'>#</a>
+        <a class='octothorpe' href='#section-104'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-102'>
+  <div class='section' id='section-105'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-102'>#</a>
+        <a class='octothorpe' href='#section-105'>#</a>
       </div>
       <h2><span id="smoothstep-function-generator" href="smoothstep-function-generator"> Smoothstep Function Generator </span></h2>
     </div>
     <div class='code'>
       <div class="highlight"><pre></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-103'>
+  <div class='section' id='section-106'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-103'>#</a>
+        <a class='octothorpe' href='#section-106'>#</a>
       </div>
       <p><strong><code>_smoothstep_transition_func</code> private function</strong></p>
     </div>
     <div class='code'>
       <div class="highlight"><pre><span class="k">def</span> <span class="nf">_smoothstep_transition_func</span><span class="p">(</span><span class="n">t1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f1</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">t2</span><span class="p">:</span> <span class="nb">float</span><span class="p">,</span> <span class="n">f2</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Callable</span><span class="p">[[</span><span class="nb">float</span><span class="p">],</span> <span class="nb">float</span><span class="p">]:</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-104'>
+  <div class='section' id='section-107'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-104'>#</a>
+        <a class='octothorpe' href='#section-107'>#</a>
       </div>
       <p>Private function that generates a smoothstep function passing trough 2 fixed points.</p>
     </div>
     <div class='code'>
-      <div class="highlight"><pre>    <span class="n">Am</span> <span class="o">=</span> <span class="n">numpy</span><span class="o">.</span><span class="n">array</span><span class="p">([[</span><span class="mi">1</span><span class="p">,</span> <span class="n">t1</span><span class="p">,</span> <span class="n">t1</span><span class="o">**</span><span class="mi">2</span><span class="p">,</span> <span class="n">t1</span><span class="o">**</span><span class="mi">3</span><span class="p">],</span>
-                      <span class="p">[</span><span class="mi">1</span><span class="p">,</span> <span class="n">t2</span><span class="p">,</span> <span class="n">t2</span><span class="o">**</span><span class="mi">2</span><span class="p">,</span> <span class="n">t2</span><span class="o">**</span><span class="mi">3</span><span class="p">],</span>
-                      <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="o">*</span><span class="n">t1</span><span class="p">,</span> <span class="mi">3</span><span class="o">*</span><span class="n">t1</span><span class="o">**</span><span class="mi">2</span><span class="p">],</span>
-                      <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="o">*</span><span class="n">t2</span><span class="p">,</span> <span class="mi">3</span><span class="o">*</span><span class="n">t2</span><span class="o">**</span><span class="mi">2</span><span class="p">]])</span>
-    <span class="n">Bm</span> <span class="o">=</span> <span class="n">numpy</span><span class="o">.</span><span class="n">array</span><span class="p">([</span><span class="n">f1</span><span class="p">,</span> <span class="n">f2</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">])</span>
-    <span class="n">A</span><span class="p">,</span> <span class="n">B</span><span class="p">,</span> <span class="n">C</span><span class="p">,</span> <span class="n">D</span> <span class="o">=</span> <span class="n">numpy</span><span class="o">.</span><span class="n">linalg</span><span class="o">.</span><span class="n">solve</span><span class="p">(</span><span class="n">Am</span><span class="p">,</span> <span class="n">Bm</span><span class="p">)</span></pre></div>
+      <div class="highlight"><pre>    <span class="n">Am</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">([[</span><span class="mi">1</span><span class="p">,</span> <span class="n">t1</span><span class="p">,</span> <span class="n">t1</span><span class="o">**</span><span class="mi">2</span><span class="p">,</span> <span class="n">t1</span><span class="o">**</span><span class="mi">3</span><span class="p">],</span>
+                   <span class="p">[</span><span class="mi">1</span><span class="p">,</span> <span class="n">t2</span><span class="p">,</span> <span class="n">t2</span><span class="o">**</span><span class="mi">2</span><span class="p">,</span> <span class="n">t2</span><span class="o">**</span><span class="mi">3</span><span class="p">],</span>
+                   <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="o">*</span><span class="n">t1</span><span class="p">,</span> <span class="mi">3</span><span class="o">*</span><span class="n">t1</span><span class="o">**</span><span class="mi">2</span><span class="p">],</span>
+                   <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">2</span><span class="o">*</span><span class="n">t2</span><span class="p">,</span> <span class="mi">3</span><span class="o">*</span><span class="n">t2</span><span class="o">**</span><span class="mi">2</span><span class="p">]])</span>
+    <span class="n">Bm</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">([</span><span class="n">f1</span><span class="p">,</span> <span class="n">f2</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">])</span>
+    <span class="n">A</span><span class="p">,</span> <span class="n">B</span><span class="p">,</span> <span class="n">C</span><span class="p">,</span> <span class="n">D</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">linalg</span><span class="o">.</span><span class="n">solve</span><span class="p">(</span><span class="n">Am</span><span class="p">,</span> <span class="n">Bm</span><span class="p">)</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-105'>
+  <div class='section' id='section-108'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-105'>#</a>
+        <a class='octothorpe' href='#section-108'>#</a>
       </div>
       
     </div>
     <div class='code'>
       <div class="highlight"><pre>    <span class="k">def</span> <span class="nf">f</span><span class="p">(</span><span class="n">t</span><span class="p">:</span> <span class="nb">float</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">float</span><span class="p">:</span>
         <span class="n">result</span><span class="p">:</span> <span class="nb">float</span> <span class="o">=</span> <span class="n">A</span> <span class="o">+</span> <span class="n">B</span><span class="o">*</span><span class="n">t</span> <span class="o">+</span> <span class="n">C</span><span class="o">*</span><span class="n">t</span><span class="o">**</span><span class="mi">2</span> <span class="o">+</span> <span class="n">D</span><span class="o">*</span><span class="n">t</span><span class="o">**</span><span class="mi">3</span>
         <span class="k">return</span> <span class="n">result</span>
 
     <span class="k">return</span> <span class="n">f</span></pre></div>
     </div>
   </div>
   <div class='clearall'></div>
-  <div class='section' id='section-106'>
+  <div class='section' id='section-109'>
     <div class='docs'>
       <div class='octowrap'>
-        <a class='octothorpe' href='#section-106'>#</a>
+        <a class='octothorpe' href='#section-109'>#</a>
       </div>
       <hr />
     </div>
     <div class='code'>
       <div class="highlight"><pre><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-    <span class="n">pwl</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="n">verbose</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">t_step</span><span class="o">=</span><span class="mf">0.1</span><span class="p">)</span>
-    <span class="n">pwl</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
-    <span class="n">pwl</span><span class="o">.</span><span class="n">sin_transition</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
-    <span class="n">pwl</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
-    <span class="n">pwl</span><span class="o">.</span><span class="n">smoothstep_transition</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
-    <span class="n">pwl</span><span class="o">.</span><span class="n">rect_pulse</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
-    <span class="n">pwl</span><span class="o">.</span><span class="n">lin_transition</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
-    <span class="n">pwl</span><span class="o">.</span><span class="n">sin_transition</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mf">0.01</span><span class="p">)</span>
-    <span class="n">pwl</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+    <span class="n">pwl0</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="mf">0.001</span><span class="p">)</span>
+    <span class="n">pwl1</span> <span class="o">=</span> <span class="n">PWL</span><span class="p">(</span><span class="mf">0.001</span><span class="p">)</span>
+
+    <span class="n">pwl0</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+    <span class="n">pwl1</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+
+    <span class="n">pwl0</span><span class="o">.</span><span class="n">sin_transition</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
+    <span class="n">pwl1</span><span class="o">.</span><span class="n">sin_transition</span><span class="p">(</span><span class="o">-</span><span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
+
+    <span class="n">pwl0</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+    <span class="n">pwl1</span><span class="o">.</span><span class="n">hold</span><span class="p">(</span><span class="mi">1</span><span class="p">)</span>
+
+    <span class="n">pwl0</span><span class="o">.</span><span class="n">sin_transition</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
+
+    <span class="n">PWL</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">merge</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
 
 </pre></div>
     </div>
   </div>
   <div class='clearall'></div>
 </div>
 </body>
```

#### html2text {}

```diff
@@ -1,13 +1,18 @@
 ****** pwl_writer.py ******
 #
 by Victor Sabiá P. Carpes
-Tested on python version 3.6.6 with numpy version 1.19.5 and python version
-3.11.1 with numpy version 1.25.0. Type stubs for older numpy versions for mypy
-checking can be found here.
+Tested on:
+    * python 3.6.6
+          o numpy 1.19.5
+          o matplotlib 3.3.4
+    * python 3.11.1
+          o numpy 1.25.0
+          o matplotlib 3.7.1
+Type stubs for older numpy versions for mypy checking can be found here.
 ===============================================================================
 ****** Index ******
     * Package_Summary
     * Precision_Related_Exception
     * PWL_Class
           o Dunder Methods
                 # Initializer
@@ -24,14 +29,15 @@
                 # Linear_Transition
                 # Rectangular_Pulse
                 # Sawtooth_Pulse
                 # Exponential_Transition
                 # Half_Sine_Transition
                 # Smoothstep_Transition
                 # PWL_File_Writer
+                # PWL_Plotter (optional feature: requires matplotlib)
           o Private Methods (minimal documentation)
                 # PWL_Point_Adder
                 # Colinear_Points_Eliminator
                 # Nested_Linear_Transition
     * Private Functions (minimal documentation)
           o Exponential_Function_Generator
           o Sinusoidal_Function_Generator
@@ -88,17 +94,27 @@
 system to be at mode 1 for 3 seconds, idle for 1 second and at mode 2 for 5
 seconds, we could write something like the following:
    mode1_state(3)
    idle_state(1)
    mode2_state(5)
 __all__ = ['PrecisionError', 'PWL']
 
+from warnings import warn
 from numbers import Real
 from typing import Callable, Dict, List, Optional
-import numpy
+import numpy as np
+
+try:
+    import matplotlib.pyplot as plt  # type: ignore
+except ImportError:
+    _has_matplotlib = False
+    warn("Matplotlib package not found. Optional features deactivated.",
+ImportWarning)
+else:
+    _has_matplotlib = True
 #
 ===============================================================================
 #
 ***** Precision Related Exception *****
 #
 PrecisionError exception class
 class PrecisionError(Exception):
@@ -650,15 +666,15 @@
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
         f = _exp_transition_func(tau=tau, t1=last_t, t2=last_t +
                                  duration, f1=last_x, f2=target)
 
-        for t in numpy.arange(last_t+t_step, last_t+duration, t_step):
+        for t in np.arange(last_t+t_step, last_t+duration, t_step):
             self._add(t, f(t))
 
         self._add(last_t+duration, target)
 #
 ===============================================================================
 #
 ***** Half Sine Transition *****
@@ -745,15 +761,15 @@
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
         f = _sin_transition_func(
             t1=last_t, t2=last_t+duration, f1=last_x, f2=target)
 
-        for t in numpy.arange(last_t+t_step, last_t+duration, t_step):
+        for t in np.arange(last_t+t_step, last_t+duration, t_step):
             self._add(t, f(t))
 
         self._add(last_t+duration, target)
 #
 ===============================================================================
 #
 ***** Smoothstep Transition *****
@@ -837,15 +853,15 @@
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
         f = _smoothstep_transition_func(
             t1=last_t, t2=last_t+duration, f1=last_x, f2=target)
 
-        for t in numpy.arange(last_t+t_step, last_t+duration, t_step):
+        for t in np.arange(last_t+t_step, last_t+duration, t_step):
             self._add(t, f(t))
 
         self._add(last_t+duration, target)
 #
 ===============================================================================
 #
 ***** PWL File Writer *****
@@ -890,35 +906,81 @@
         if self._verbose:
             print(f"{self._name}: Writing PWL file to {filename}.")
 
         t_list = self._t_list
         x_list = self._x_list
 
         with open(filename, "w") as file:
-            ti_str = numpy.format_float_scientific(
+            ti_str = np.format_float_scientific(
                 t_list[0], precision-1, unique=False, sign=False)
-            xi_str = numpy.format_float_scientific(
+            xi_str = np.format_float_scientific(
                 x_list[0], precision-1, unique=False, sign=True)
             file.write(f"{ti_str}    {xi_str}\n")
             last_t = ti_str
             for ti, xi in zip(t_list[1:], x_list[1:]):
-                ti_str = numpy.format_float_scientific(
+                ti_str = np.format_float_scientific(
                     ti, precision-1, unique=False, sign=False)
-                xi_str = numpy.format_float_scientific(
+                xi_str = np.format_float_scientific(
                     xi, precision-1, unique=False, sign=True)
                 if ti_str == last_t:
                     raise PrecisionError(
                         "The chosen precision level caused the written time
 coordinates to not be strictly increasing.")
                 file.write(
                     f"{ti_str}    {xi_str}\n")
                 last_t = ti_str
 #
 ===============================================================================
 #
+***** PWL Plotter *****
+#
+plot class method of PWL class
+    @classmethod
+    def plot(cls, merge: bool = False) -> None:
+#
+Optional feature: Requires matplotlib
+**** Summary ****
+Class method that takes all instances of the PWL class and plots them on the
+same time axis.
+**** Arguments ****
+    * merge (bool, optional) : Flag indicating if all signals should be ploted
+      on the same strip or separeted. If not set, defaults to False.
+**** Raises ****
+    * ImportError : Raised if the matplotlib package is not installed.
+        if not _has_matplotlib:
+            raise ImportError(
+                "Optional features are deactivated. Install matplotlib to
+use.")
+
+        dict_of_objects = cls.__dict_of_objects
+
+        if not dict_of_objects:
+            return None
+
+        if merge:
+            fig, axs = plt.subplots(nrows=1, sharex=True, squeeze=False)
+            axs = np.repeat(axs, len(dict_of_objects))
+        else:
+            fig, axs = plt.subplots(
+                nrows=len(dict_of_objects), sharex=True, squeeze=False)
+            axs = axs.flatten()
+        x_max: float = 0
+
+        for key, ax in zip(dict_of_objects, axs):
+            pwl = dict_of_objects[key]
+            x_list = pwl.t_list
+            x_max = max(x_max, max(x_list))
+            y_list = pwl.x_list
+            label = pwl.name
+            ax.plot(x_list, y_list)
+            ax.set_ylabel(label)
+
+        axs[0].set_xlim(xmin=0, xmax=x_max)
+        plt.show()
+#
 ****** Private Methods and Functions ******
 #
 From this point forward, all listed methods and functions are not intended to
 be used by the user. Brief descriptions will be provided, but documentation
 will be kept to a minimum.
 #
 ===============================================================================
@@ -1001,20 +1063,20 @@
 #
 _exp_transition_func private function
 def _exp_transition_func(tau: float, t1: float, f1: float, t2: float, f2:
 float) -> Callable[[float], float]:
 #
 Private function that generates an exponential function passing trough 2 fixed
 points.
-    A: float = (f1*numpy.exp(t1/tau) - f2*numpy.exp(t2/tau)) / \
-        (numpy.exp(t1/tau) - numpy.exp(t2/tau))
-    B: float = (f1 - f2)/(numpy.exp(-t1/tau) - numpy.exp(-t2/tau))
+    A: float = (f1*np.exp(t1/tau) - f2*np.exp(t2/tau)) / \
+        (np.exp(t1/tau) - np.exp(t2/tau))
+    B: float = (f1 - f2)/(np.exp(-t1/tau) - np.exp(-t2/tau))
 #
     def f(t: float) -> float:
-        result: float = A + B*numpy.exp(-t/tau)
+        result: float = A + B*np.exp(-t/tau)
         return result
 
     return f
 #
 ===============================================================================
 #
 ***** Sinusoidal Function Generator *****
@@ -1024,51 +1086,57 @@
 > Callable[[float], float]:
 #
 Private function that generates a sinusoidal function passing trough 2 fixed
 points.
     fm: float = (f1+f2)/2
     tm: float = (t1+t2)/2
     T: float = 2*(t2-t1)
-    w: float = 2*numpy.pi/T
+    w: float = 2*np.pi/T
     phi: float = w*tm
     A: float = f2-fm
 #
     def f(t: float) -> float:
-        result: float = fm + A*numpy.sin(w*t - phi)
+        result: float = fm + A*np.sin(w*t - phi)
         return result
 
     return f
 #
 ===============================================================================
 #
 ***** Smoothstep Function Generator *****
 #
 _smoothstep_transition_func private function
 def _smoothstep_transition_func(t1: float, f1: float, t2: float, f2: float) -
 > Callable[[float], float]:
 #
 Private function that generates a smoothstep function passing trough 2 fixed
 points.
-    Am = numpy.array([[1, t1, t1**2, t1**3],
-                      [1, t2, t2**2, t2**3],
-                      [0, 1, 2*t1, 3*t1**2],
-                      [0, 1, 2*t2, 3*t2**2]])
-    Bm = numpy.array([f1, f2, 0, 0])
-    A, B, C, D = numpy.linalg.solve(Am, Bm)
+    Am = np.array([[1, t1, t1**2, t1**3],
+                   [1, t2, t2**2, t2**3],
+                   [0, 1, 2*t1, 3*t1**2],
+                   [0, 1, 2*t2, 3*t2**2]])
+    Bm = np.array([f1, f2, 0, 0])
+    A, B, C, D = np.linalg.solve(Am, Bm)
 #
     def f(t: float) -> float:
         result: float = A + B*t + C*t**2 + D*t**3
         return result
 
     return f
 #
 ===============================================================================
 if __name__ == "__main__":
-    pwl = PWL(verbose=True, t_step=0.1)
-    pwl.hold(1)
-    pwl.sin_transition(1, 1)
-    pwl.hold(1)
-    pwl.smoothstep_transition(0, 1)
-    pwl.rect_pulse(1, 1)
-    pwl.lin_transition(0, 1)
-    pwl.sin_transition(1, 0.01)
-    pwl.hold(1)
+    pwl0 = PWL(0.001)
+    pwl1 = PWL(0.001)
+
+    pwl0.hold(1)
+    pwl1.hold(1)
+
+    pwl0.sin_transition(1, 1)
+    pwl1.sin_transition(-1, 1)
+
+    pwl0.hold(1)
+    pwl1.hold(1)
+
+    pwl0.sin_transition(0, 1)
+
+    PWL.plot(merge=True)
```

### Comparing `pwl_writer-1.0.0/docs/pycco.css` & `pwl_writer-1.1.0/docs/pycco.css`

 * *Files identical despite different names*

### Comparing `pwl_writer-1.0.0/pwl_writer/pwl_writer.py` & `pwl_writer-1.1.0/pwl_writer/pwl_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 """
 *by Victor Sabiá P. Carpes*
 
-Tested on python version `3.6.6` with numpy version `1.19.5` and python version `3.11.1` with numpy version `1.25.0`. Type stubs for older numpy versions for mypy checking can be found [here](https://github.com/numpy/numpy-stubs).
+Tested on:
+
+* python `3.6.6`
+        * numpy `1.19.5`
+        * matplotlib `3.3.4`
+* python `3.11.1`
+        * numpy `1.25.0`
+        * matplotlib `3.7.1`
+
+Type stubs for older numpy versions for mypy checking can be found [here](https://github.com/numpy/numpy-stubs).
 
 ----
 
 # Index
 
 * [Package Summary](#package-summary)
 * [Precision Related Exception](#precision-related-exception)
@@ -25,14 +34,15 @@
             * [Linear Transition](#linear-transition)
             * [Rectangular Pulse](#rectangular-pulse)
             * [Sawtooth Pulse](#sawtooth-pulse)
             * [Exponential Transition](#exponential-transition)
             * [Half Sine Transition](#half-sine-transition)
             * [Smoothstep Transition](#smoothstep-transition)
             * [PWL File Writer](#pwl-file-writer)
+            * [PWL Plotter](#pwl-plotter) *(optional feature: requires matplotlib)*
         * Private Methods *(minimal documentation)*
             * [PWL Point Adder](#pwl-point-adder)
             * [Colinear Points Eliminator](#colinear-points-eliminator)
             * [Nested Linear Transition](#nested-linear-transition)
 * Private Functions *(minimal documentation)*
         * [Exponential Function Generator](#exponential-function-generator)
         * [Sinusoidal Function Generator](#sinusoidal-function-generator)
@@ -69,17 +79,26 @@
         mode1_state(3)
         idle_state(1)
         mode2_state(5)
 """
 
 __all__ = ['PrecisionError', 'PWL']
 
+from warnings import warn
 from numbers import Real
 from typing import Callable, Dict, List, Optional
-import numpy
+import numpy as np
+
+try:
+    import matplotlib.pyplot as plt  # type: ignore
+except ImportError:
+    _has_matplotlib = False
+    warn("Matplotlib package not found. Optional features deactivated.", ImportWarning)
+else:
+    _has_matplotlib = True
 
 # ----
 
 # == Precision Related Exception ==
 
 
 class PrecisionError(Exception):
@@ -658,15 +677,15 @@
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
         f = _exp_transition_func(tau=tau, t1=last_t, t2=last_t +
                                  duration, f1=last_x, f2=target)
 
-        for t in numpy.arange(last_t+t_step, last_t+duration, t_step):
+        for t in np.arange(last_t+t_step, last_t+duration, t_step):
             self._add(t, f(t))
 
         self._add(last_t+duration, target)
 
     # ----
 
     # == Half Sine Transition ==
@@ -748,15 +767,15 @@
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
         f = _sin_transition_func(
             t1=last_t, t2=last_t+duration, f1=last_x, f2=target)
 
-        for t in numpy.arange(last_t+t_step, last_t+duration, t_step):
+        for t in np.arange(last_t+t_step, last_t+duration, t_step):
             self._add(t, f(t))
 
         self._add(last_t+duration, target)
 
     # ----
 
     # == Smoothstep Transition ==
@@ -836,15 +855,15 @@
 
         last_t = self._t_list[-1]
         last_x = self._x_list[-1]
 
         f = _smoothstep_transition_func(
             t1=last_t, t2=last_t+duration, f1=last_x, f2=target)
 
-        for t in numpy.arange(last_t+t_step, last_t+duration, t_step):
+        for t in np.arange(last_t+t_step, last_t+duration, t_step):
             self._add(t, f(t))
 
         self._add(last_t+duration, target)
 
     # ----
 
     # == PWL File Writer ==
@@ -887,34 +906,84 @@
         if self._verbose:
             print(f"{self._name}: Writing PWL file to {filename}.")
 
         t_list = self._t_list
         x_list = self._x_list
 
         with open(filename, "w") as file:
-            ti_str = numpy.format_float_scientific(
+            ti_str = np.format_float_scientific(
                 t_list[0], precision-1, unique=False, sign=False)
-            xi_str = numpy.format_float_scientific(
+            xi_str = np.format_float_scientific(
                 x_list[0], precision-1, unique=False, sign=True)
             file.write(f"{ti_str}    {xi_str}\n")
             last_t = ti_str
             for ti, xi in zip(t_list[1:], x_list[1:]):
-                ti_str = numpy.format_float_scientific(
+                ti_str = np.format_float_scientific(
                     ti, precision-1, unique=False, sign=False)
-                xi_str = numpy.format_float_scientific(
+                xi_str = np.format_float_scientific(
                     xi, precision-1, unique=False, sign=True)
                 if ti_str == last_t:
                     raise PrecisionError(
                         "The chosen precision level caused the written time coordinates to not be strictly increasing.")
                 file.write(
                     f"{ti_str}    {xi_str}\n")
                 last_t = ti_str
 
     # ----
 
+    # == PWL Plotter ==
+
+    @classmethod
+    def plot(cls, merge: bool = False) -> None:
+        """**`plot` class method of `PWL` class**
+        *Optional feature: Requires matplotlib*
+
+        ### Summary
+
+        Class method that takes all instances of the `PWL` class and plots them on the same time axis.
+
+        ### Arguments
+
+        * `merge` (`bool`, optional) : Flag indicating if all signals should be ploted on the same strip or separeted. If not set, defaults to False.
+
+        ### Raises
+
+        * `ImportError` : Raised if the matplotlib package is not installed.
+        """
+
+        if not _has_matplotlib:
+            raise ImportError(
+                "Optional features are deactivated. Install matplotlib to use.")
+
+        dict_of_objects = cls.__dict_of_objects
+
+        if not dict_of_objects:
+            return None
+
+        if merge:
+            fig, axs = plt.subplots(nrows=1, sharex=True, squeeze=False)
+            axs = np.repeat(axs, len(dict_of_objects))
+        else:
+            fig, axs = plt.subplots(
+                nrows=len(dict_of_objects), sharex=True, squeeze=False)
+            axs = axs.flatten()
+        x_max: float = 0
+
+        for key, ax in zip(dict_of_objects, axs):
+            pwl = dict_of_objects[key]
+            x_list = pwl.t_list
+            x_max = max(x_max, max(x_list))
+            y_list = pwl.x_list
+            label = pwl.name
+            ax.plot(x_list, y_list)
+            ax.set_ylabel(label)
+
+        axs[0].set_xlim(xmin=0, xmax=x_max)
+        plt.show()
+
     # = Private Methods and Functions =
 
     # From this point forward, all listed methods and functions are not intended to be used by the user. Brief descriptions will be provided, but documentation will be kept to a minimum.
 
     # ----
 
     # == PWL Point Adder ==
@@ -994,20 +1063,20 @@
 
 def _exp_transition_func(tau: float, t1: float, f1: float, t2: float, f2: float) -> Callable[[float], float]:
     """**`_exp_transition_func` private function**
 
     Private function that generates an exponential function passing trough 2 fixed points.
     """
 
-    A: float = (f1*numpy.exp(t1/tau) - f2*numpy.exp(t2/tau)) / \
-        (numpy.exp(t1/tau) - numpy.exp(t2/tau))
-    B: float = (f1 - f2)/(numpy.exp(-t1/tau) - numpy.exp(-t2/tau))
+    A: float = (f1*np.exp(t1/tau) - f2*np.exp(t2/tau)) / \
+        (np.exp(t1/tau) - np.exp(t2/tau))
+    B: float = (f1 - f2)/(np.exp(-t1/tau) - np.exp(-t2/tau))
 
     def f(t: float) -> float:
-        result: float = A + B*numpy.exp(-t/tau)
+        result: float = A + B*np.exp(-t/tau)
         return result
 
     return f
 
 # ----
 
 # == Sinusoidal Function Generator ==
@@ -1018,20 +1087,20 @@
 
     Private function that generates a sinusoidal function passing trough 2 fixed points.
     """
 
     fm: float = (f1+f2)/2
     tm: float = (t1+t2)/2
     T: float = 2*(t2-t1)
-    w: float = 2*numpy.pi/T
+    w: float = 2*np.pi/T
     phi: float = w*tm
     A: float = f2-fm
 
     def f(t: float) -> float:
-        result: float = fm + A*numpy.sin(w*t - phi)
+        result: float = fm + A*np.sin(w*t - phi)
         return result
 
     return f
 
 # ----
 
 # == Smoothstep Function Generator ==
@@ -1039,33 +1108,39 @@
 
 def _smoothstep_transition_func(t1: float, f1: float, t2: float, f2: float) -> Callable[[float], float]:
     """**`_smoothstep_transition_func` private function**
 
     Private function that generates a smoothstep function passing trough 2 fixed points.
     """
 
-    Am = numpy.array([[1, t1, t1**2, t1**3],
-                      [1, t2, t2**2, t2**3],
-                      [0, 1, 2*t1, 3*t1**2],
-                      [0, 1, 2*t2, 3*t2**2]])
-    Bm = numpy.array([f1, f2, 0, 0])
-    A, B, C, D = numpy.linalg.solve(Am, Bm)
+    Am = np.array([[1, t1, t1**2, t1**3],
+                   [1, t2, t2**2, t2**3],
+                   [0, 1, 2*t1, 3*t1**2],
+                   [0, 1, 2*t2, 3*t2**2]])
+    Bm = np.array([f1, f2, 0, 0])
+    A, B, C, D = np.linalg.solve(Am, Bm)
 
     def f(t: float) -> float:
         result: float = A + B*t + C*t**2 + D*t**3
         return result
 
     return f
 
 # ----
 
 
 if __name__ == "__main__":
-    pwl = PWL(verbose=True, t_step=0.1)
-    pwl.hold(1)
-    pwl.sin_transition(1, 1)
-    pwl.hold(1)
-    pwl.smoothstep_transition(0, 1)
-    pwl.rect_pulse(1, 1)
-    pwl.lin_transition(0, 1)
-    pwl.sin_transition(1, 0.01)
-    pwl.hold(1)
+    pwl0 = PWL(0.001)
+    pwl1 = PWL(0.001)
+
+    pwl0.hold(1)
+    pwl1.hold(1)
+
+    pwl0.sin_transition(1, 1)
+    pwl1.sin_transition(-1, 1)
+
+    pwl0.hold(1)
+    pwl1.hold(1)
+
+    pwl0.sin_transition(0, 1)
+
+    PWL.plot(merge=True)
```

### Comparing `pwl_writer-1.0.0/PKG-INFO` & `pwl_writer-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 Metadata-Version: 2.1
 Name: pwl_writer
-Version: 1.0.0
+Version: 1.1.0
 Summary: Package to generate PWL incrementally using little 'events' like rectangular pulses and exponential rising or falling edges.
 Author-email: "Victor Sabiá P. Carpes" <victorscarpes@gmail.com>
 Requires-Python: >=3.6.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: numpy >=1.19.5
+Requires-Dist: numpy
+Requires-Dist: pycco ; extra == "doc"
+Requires-Dist: matplotlib ; extra == "plot"
 Project-URL: Documentation, https://htmlpreview.github.io/?https://github.com/victorscarpes/pwl_writer/blob/main/docs/pwl_writer.html
 Project-URL: Source, https://github.com/victorscarpes/pwl_writer
+Provides-Extra: doc
+Provides-Extra: plot
 
 # pwl_writer
 
 *by Victor Sabiá P. Carpes*
 
-Tested on python version `3.6.6` with numpy version `1.19.5` and python version `3.11.1` with numpy version `1.25.0`. Type stubs for older numpy versions for mypy checking can be found [here](https://github.com/numpy/numpy-stubs).
+Tested on:
+
+* python `3.6.6`
+  * numpy `1.19.5`
+  * matplotlib `3.3.4`
+* python `3.11.1`
+  * numpy `1.25.0`
+  * matplotlib `3.7.1`
+
+Type stubs for older numpy versions for mypy checking can be found [here](https://github.com/numpy/numpy-stubs).
 
 ## Summary
 
 This package defines a class `PWL` to generate objects that represent time dependent signals $x(t)$ that need to be coded in a PWL file. Those objects are built using little components such as rectangular pulses and sawtooth pulses that can be chained together.
 
 ## Motivation
```

