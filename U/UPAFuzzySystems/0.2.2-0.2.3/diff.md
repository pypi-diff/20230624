# Comparing `tmp/UPAFuzzySystems-0.2.2.tar.gz` & `tmp/UPAFuzzySystems-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UPAFuzzySystems-0.2.2.tar", last modified: Wed Jun 21 16:47:30 2023, max compression
+gzip compressed data, was "UPAFuzzySystems-0.2.3.tar", last modified: Sat Jun 24 16:48:50 2023, max compression
```

## Comparing `UPAFuzzySystems-0.2.2.tar` & `UPAFuzzySystems-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 16:47:30.130203 UPAFuzzySystems-0.2.2/
--rw-rw-rw-   0        0        0     1099 2022-10-29 19:07:07.000000 UPAFuzzySystems-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     2498 2023-06-21 16:47:30.128144 UPAFuzzySystems-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1616 2023-06-21 16:45:02.000000 UPAFuzzySystems-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 16:47:30.059993 UPAFuzzySystems-0.2.2/UPAFuzzySystems/
--rw-rw-rw-   0        0        0    34335 2023-06-21 15:14:44.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems/UPAFuzzySystems.py
--rw-rw-rw-   0        0        0      286 2022-11-03 19:51:00.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 16:47:30.118870 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/
--rw-rw-rw-   0        0        0     2498 2023-06-21 16:47:29.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-21 16:47:29.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 16:47:29.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-21 16:47:29.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-21 16:47:29.000000 UPAFuzzySystems-0.2.2/UPAFuzzySystems.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 16:47:30.131203 UPAFuzzySystems-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1574 2023-06-21 16:46:39.000000 UPAFuzzySystems-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:48:50.953575 UPAFuzzySystems-0.2.3/
+-rw-rw-rw-   0        0        0     1099 2022-10-29 19:07:07.000000 UPAFuzzySystems-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     8329 2023-06-24 16:48:50.950592 UPAFuzzySystems-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7273 2023-06-24 16:20:44.000000 UPAFuzzySystems-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 16:48:50.888573 UPAFuzzySystems-0.2.3/UPAFuzzySystems/
+-rw-rw-rw-   0        0        0    34549 2023-06-24 16:22:01.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems/UPAFuzzySystems.py
+-rw-rw-rw-   0        0        0      286 2022-11-03 19:51:00.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 16:48:50.944582 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/
+-rw-rw-rw-   0        0        0     8329 2023-06-24 16:48:50.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-24 16:48:50.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 16:48:50.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-24 16:48:50.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-24 16:48:50.000000 UPAFuzzySystems-0.2.3/UPAFuzzySystems.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 16:48:50.954578 UPAFuzzySystems-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1574 2023-06-24 16:20:55.000000 UPAFuzzySystems-0.2.3/setup.py
```

### Comparing `UPAFuzzySystems-0.2.2/LICENSE` & `UPAFuzzySystems-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `UPAFuzzySystems-0.2.2/UPAFuzzySystems/UPAFuzzySystems.py` & `UPAFuzzySystems-0.2.3/UPAFuzzySystems/UPAFuzzySystems.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 
 from skfuzzy import defuzz, trapmf, trimf, trimf, gaussmf, gbellmf
-from numpy import array, arange, matrix, meshgrid, linspace, radians, fmin, fmax, max, zeros, minimum, maximum, isscalar, sum, prod, multiply, repeat
+from numpy import array, arange, matrix, meshgrid, linspace, radians, fmin, fmax, max, zeros, minimum, maximum, isscalar, sum, prod, multiply, repeat, dot, sum
 import matplotlib.pyplot as plt
 from control import NonlinearIOSystem, sample_system, InterconnectedSystem, LinearIOSystem, tf2ss, tfdata
 
 
 class fuzzy_universe():
     """Create a Universe Discrete or Continuous for Describe Inputs and Outputs in an 
     inference system.
@@ -42,15 +42,16 @@
             `'gbellmf'`: Generalized bell membership function.
             `'eq'`: For specific equation to use in Takagi Sugeno forms, in this vertices is an string equation.
         vertices (list/str): List with the numerical parameters or string equation for the membership functions.
         
         Returns:
         none
         """
-
+        if isinstance(vertices, list):
+            vertices=array(vertices)
         self.structure[name_f] = [mf,vertices]
     def remove_fuzzyset(self,name_f=""):
         """Deletes from the universe the fuzzy set with the given name.
         
         Args:
         name_f (str): String name for the fuzzy set to delete.
         
@@ -67,20 +68,21 @@
         Returns:
             fuzzy_set (dict): Dictionary containing universe and membership values of the fuzzy set.
         """
         membershipvalues=[]
         X = self.structure['universe']
         membershipfuntion = self.structure[name][0]
         vertices = self.structure[name][1]
+        vertilist =list(vertices)
         if membershipfuntion =='gaussmf':
-            exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertices[0])+','+str(vertices[1])+'))')
+            exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertilist[0])+','+str(vertilist[1])+'))')
         elif membershipfuntion == 'raw':
-             exec('membershipvalues.append('+str(vertices)+')')
+             exec('membershipvalues.append('+str(vertilist)+')')
         else:
-            exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertices)+'))')
+            exec('membershipvalues.append('+membershipfuntion+'(X,'+str(vertilist)+'))')
         return {'universe':X,'membership values':membershipvalues[0]}
     def view_fuzzy(self):
 
         """Plots the the corresponding universe with all its fuzzy sets.
         
 
         Args:
@@ -236,47 +238,49 @@
         consequence (obj): Object with a fuzzy universe previously defined.
 
         Returns:
         none
         """
         self.consequences.append(consequence)
         self.output_universes.append(consequence.universe)
-    def add_rule(self,premises_r,conectors_r,consequence_r):
+    def add_rule(self,premises_r,conectors_r,consequences_r):
         """Allows to add a rule to the corresponding inference system with conectors in premises and consequences. All premises and consequences must have the same number of elements in their universes.
         
         Args:
         premises_r (list): List of lists of premises with two strings per premise [[`'Name Premise 1'`,`'Name Fuzzy Set 1'`],[`'Name Premise 2'`,`'Name Fuzzy Set 2'`]].
         conectors_r (list): List of conectors for the premises in the rule `'and'`/`'or'`.
         consequence_r (list): List of lists of consequences with two strings per consequence [[`'Name Consequence 1'`,`'Name Fuzzy Set 1'`],[`'Name Consequence 2'`,`'Name Fuzzy Set 2'`]].
         Returns:
         none
         """
 
-        fuzzy_set = premises_r
+        fuzzy_set_input = premises_r.copy()
         antecedents = []
-        consequences_r = []
+        fuzzy_set_output = consequences_r.copy()
         universes = []
+        consequents = []
         universe = 0
-        while fuzzy_set:
-            premise = fuzzy_set.pop(0)
+        while fuzzy_set_input:
+            premise = fuzzy_set_input.pop(0)
             for i in self.premises:
                 if i.name == premise[0]:
                     provlist = i.structure[premise[1]].copy()
                     provlist.append(i.universe)
                     antecedents.append(provlist)
-        while consequence_r:
-            consequence = consequence_r.pop(0)
+        while fuzzy_set_output:
+            consequence = fuzzy_set_output.pop(0)
             for i in self.consequences:
                 if i.name == consequence[0]:
-                    consequences_r.append(i.structure[consequence[1]])
-                    universes.append(universe)
-                    universe = universe+1
+                    provlist = i.structure[consequence[1]].copy()
+                    provlist.append(i.universe)
+                    universes.append(i.universe)
+                    consequents.append(provlist)
         rule = {'antecedent':antecedents,
                   'conectors':conectors_r,
-                  'consequent':consequences_r,
+                  'consequent':consequents,
                'output_universes':universes}
         self.rules.append(rule)
     def build(self):
         """Built the created system with all the predefined configurations.
         
         Args:
         none
@@ -345,14 +349,17 @@
                 `'mom'`: Mean of maxima.
                 `'som'`: Smallest of maxima.
                 `'lom'`: Largest of maxima.
         Returns:
             defuzzifiedv (float): Defuzzified value.
         """
         try:
+            if func =='centroid':
+                defuzzific = array([dot(universe,i+1e-200)/sum(i+1e-200) for i in sc])
+            else:
                 defuzzific = array([0 if sum(i)==0 else defuzz(universe,i,func)  for i in sc]) 
         except:
             defuzzific = 0
         return defuzzific
 
     def fuzzy_system_sim(self, inputs_val):
         """Simulate an input and returns the output of the defined inference system, rembember to check that all universes of premises and consequences have the same number of elements.
@@ -392,20 +399,20 @@
                     elif conect =='and' and self.structure['AndConector']=='prod':
                         a = multiply(a,self.fuzzification(self.structure['Rules'][i]['antecedent'][j+1][0],self.structure['Rules'][i]['antecedent'][j+1][1],inputs_val[:,j+1],self.structure['Rules'][i]['antecedent'][0][2]))
                     elif conect =='or' and self.structure['OrConector']=='probsum':
                         b = self.fuzzification(self.structure['Rules'][i]['antecedent'][j+1][0],self.structure['Rules'][i]['antecedent'][j+1][1],inputs_val[:,j+1],self.structure['Rules'][i]['antecedent'][0][2])
                         a = (a+b)-multiply(a,b)
                 for k in range(len(self.structure['Rules'][i]['consequent'])):
                     if isinstance(self.structure['Rules'][i]['consequent'][k][0],str) and  self.structure['Defuzz'] != 'centroidTS':
-                        self.structure['Rules'][i]['consequent'][k] = self.fuzzification(self.structure['Rules'][i]['consequent'][k][0],self.structure['Rules'][i]['consequent'][k][1],self.structure['output_universes'][self.structure['Rules'][i]['output_universes'][k]],self.structure['Rules'][i]['antecedent'][0][2])
+                        consequence_vector = self.fuzzification(self.structure['Rules'][i]['consequent'][k][0],self.structure['Rules'][i]['consequent'][k][1],self.structure['output_universes'][k],self.structure['Rules'][i]['consequent'][0][2])
                     if self.structure['Defuzz'] != 'centroidTS':
                         if self.structure['Implication'] =='min':
-                            IM[k][i,:] = fmin(a.reshape(a.shape[0],1),repeat((self.structure['Rules'][i]['consequent'][k]).reshape((1,self.structure['Rules'][i]['consequent'][k].shape[0])),a.shape[0],axis = 0))
+                            IM[k][i,:] = fmin(a.reshape(a.shape[0],1),repeat((consequence_vector).reshape((1,consequence_vector.shape[0])),a.shape[0],axis = 0))
                         elif self.structure['Implication'] =='prod':
-                            IM[k][i,:] = (a.reshape(a.shape[0],1).repeat(len(self.structure['Rules'][i]['consequent'][k]),axis = 1)*self.structure['Rules'][i]['consequent'][k])
+                            IM[k][i,:] = a.reshape(a.shape[0],1).repeat(len(consequence_vector),axis = 1)*consequence_vector
                     else:
                         x = inputs_val
                         if self.structure['Implication'] =='min':
                             IM[k][i,0] = fmin(a,self.fuzzification(self.structure['Rules'][i]['consequent'][k][0],self.structure['Rules'][i]['consequent'][k][1],inputs_val,self.structure['Rules'][i]['antecedent'][0][2]))
                             miuo[k] = miuo[k] + a
                         if self.structure['Implication'] =='prod':
                             IM[k][i,:,0] = multiply(a,self.fuzzification(self.structure['Rules'][i]['consequent'][k][0],self.structure['Rules'][i]['consequent'][k][1],inputs_val,self.structure['Rules'][i]['antecedent'][0][2]))
```

### Comparing `UPAFuzzySystems-0.2.2/setup.py` & `UPAFuzzySystems-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 DESCRIPTION = 'UPAFuzzySystems package for definition and simulation of Fuzzy Inference Systems for general and control applications.'
 LONG_DESCRIPTION = 'UPAFuzzySystems library allows defining Fuzzy Inference Systems for different applications with continuous and discrete universes, it also deploys structures for simulation of fuzzy control with transfer functions and state space models.'
 with open('README.md', 'r', encoding='utf-8') as file:
     LONG_DESCRIPTION = file.read()
 
 # Setting up
 setup(
```

