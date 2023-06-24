# Comparing `tmp/glimy-4.2.5.tar.gz` & `tmp/glimy-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glimy-4.2.5.tar", last modified: Wed Mar 22 01:13:37 2023, max compression
+gzip compressed data, was "glimy-5.0.0.tar", last modified: Sat Jun 24 21:26:30 2023, max compression
```

## Comparing `glimy-4.2.5.tar` & `glimy-5.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-03-22 01:13:37.701613 glimy-4.2.5/
--rw-rw-r--   0 ali       (1000) ali       (1000)       47 2022-11-11 09:33:29.000000 glimy-4.2.5/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)    21664 2023-03-22 01:13:37.701613 glimy-4.2.5/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)    21000 2023-03-22 01:12:57.000000 glimy-4.2.5/README.md
--rw-rw-r--   0 ali       (1000) ali       (1000)      739 2023-03-22 01:13:24.000000 glimy-4.2.5/pyproject.toml
--rw-rw-r--   0 ali       (1000) ali       (1000)       38 2023-03-22 01:13:37.701613 glimy-4.2.5/setup.cfg
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-03-22 01:13:37.629600 glimy-4.2.5/src/
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-03-22 01:13:37.697613 glimy-4.2.5/src/glimy/
--rw-rw-r--   0 ali       (1000) ali       (1000)    53957 2023-03-22 01:05:33.000000 glimy-4.2.5/src/glimy/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    26917 2023-03-11 21:34:12.000000 glimy-4.2.5/src/glimy/geo.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-03-22 01:13:37.701613 glimy-4.2.5/src/glimy.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)    21664 2023-03-22 01:13:37.000000 glimy-4.2.5/src/glimy.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      235 2023-03-22 01:13:37.000000 glimy-4.2.5/src/glimy.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-03-22 01:13:37.000000 glimy-4.2.5/src/glimy.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       17 2023-03-22 01:13:37.000000 glimy-4.2.5/src/glimy.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        6 2023-03-22 01:13:37.000000 glimy-4.2.5/src/glimy.egg-info/top_level.txt
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:26:30.654988 glimy-5.0.0/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       47 2022-11-11 09:33:29.000000 glimy-5.0.0/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)    21684 2023-06-24 21:26:30.650988 glimy-5.0.0/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)    21000 2023-03-22 01:12:57.000000 glimy-5.0.0/README.md
+-rw-rw-r--   0 ali       (1000) ali       (1000)      769 2023-06-24 21:25:04.000000 glimy-5.0.0/pyproject.toml
+-rw-rw-r--   0 ali       (1000) ali       (1000)       38 2023-06-24 21:26:30.654988 glimy-5.0.0/setup.cfg
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:26:30.650988 glimy-5.0.0/src/
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:26:30.650988 glimy-5.0.0/src/glimy/
+-rw-rw-r--   0 ali       (1000) ali       (1000)    67803 2023-06-24 21:23:50.000000 glimy-5.0.0/src/glimy/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    26917 2023-05-05 09:58:12.000000 glimy-5.0.0/src/glimy/geo.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:26:30.650988 glimy-5.0.0/src/glimy.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)    21684 2023-06-24 21:26:30.000000 glimy-5.0.0/src/glimy.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      235 2023-06-24 21:26:30.000000 glimy-5.0.0/src/glimy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-24 21:26:30.000000 glimy-5.0.0/src/glimy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       25 2023-06-24 21:26:30.000000 glimy-5.0.0/src/glimy.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        6 2023-06-24 21:26:30.000000 glimy-5.0.0/src/glimy.egg-info/top_level.txt
```

### Comparing `glimy-4.2.5/PKG-INFO` & `glimy-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: glimy
-Version: 4.2.5
-Summary: Computational Electromagnetics Package with Dielectic, Magnetic Materials and Gravity
+Version: 5.0.0
+Summary: Computational Electromagnetics Package with Dielectic, Magnetic, Anisotropic, Lossy Materials and Gravity
 Author-email: Ali Hakim Taskiran <alihakimxyz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
         
 Project-URL: Homepage, https://github.com/alihakimtaskiran/Glimy
 Project-URL: Bug Tracker, https://github.com/alihakimtaskiran/Glimy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Glimy
 ## FDTD Simulator
 <img src="https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/logo.png" width="200"></img>
```

### Comparing `glimy-4.2.5/README.md` & `glimy-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `glimy-4.2.5/pyproject.toml` & `glimy-5.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "glimy"
-version = "4.2.5"
+version = "5.0.0"
 authors = [
   { name="Ali Hakim Taskiran", email="alihakimxyz@gmail.com" },
 ]
-description = "Computational Electromagnetics Package with Dielectic, Magnetic Materials and Gravity"
+description = "Computational Electromagnetics Package with Dielectic, Magnetic, Anisotropic, Lossy Materials and Gravity"
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.7"
-dependencies=["numpy", "matplotlib"]
+requires-python = ">=3.6"
+dependencies=["numpy", "matplotlib","psutils"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `glimy-4.2.5/src/glimy/__init__.py` & `glimy-5.0.0/src/glimy/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,37 @@
 print("Interacting with reality...")
 import numpy as np
+try:
+    import cupy as cp
+    print("GPU accelerated computing enabled. You can set Render('cupy') to benefit GPU utils.")
+    cupy_enabled=True
+except ImportError:
+    cupy_enabled=False
+    cp=np
+    print("Running in CPU mode, set Render('numpy') to use it.")
+
+
 import sys
 import glimy.geo
-
+import psutil
 import warnings
 import time
 import matplotlib.pyplot as plt
 import itertools
 G=6.6743e-11
 c=299792458
 c_2=c**2
 PI_2=np.pi*2
 Z_0=376.730313
 e_0=8.8541878128e-12
 mu_0=1.25663706212e-6
 
+e_0_2=e_0*2
+mu_0_2=2*mu_0
+
 class Continuum(object):
     def __init__(self, grid_size, ds):
         
         if not isinstance(grid_size,(tuple,list)):
             raise TypeError("# of pixels of grid must be carried by a tuple or a list")
         
         self.__dim=len(grid_size)
@@ -56,14 +69,16 @@
         
         self.__instance=0
         
         self.__bound=None
         self.__bound_bool=False
         self.__rendered=False
         
+        self.__built_for=None
+        
 
         
         
     def add(self, arg):
         
         if isinstance(arg, (set, tuple, list)):
             for element in arg:
@@ -118,59 +133,72 @@
         def gp(*x):
             __=0
             x=np.array(x)
             for l,m in self.__stellar:
                 __+=m/np.linalg.norm(l-x*self.__ds)
             return __
 
-        self.__Jdt=1/np.sqrt(1+g_c_2*np.fromfunction(np.vectorize(gp), self.__grid_size, dtype=float))
+        self.__Jdt=1/(1+g_c_2*np.fromfunction(np.vectorize(gp), self.__grid_size, dtype=float))
+        if self.__cupy_enabled:
+            self.__Jdt_cp=cp.array(self.__Jdt)
         
 
     def __emo_video_creator(self):
         
         if self.__anisotropy:
             shape=self.__grid_size+(self.__dim,self.__dim)
             self.__e=np.full(shape,np.eye(self.__dim))
             self.__mu=np.full(shape,np.eye(self.__dim))
+
         else:
             shape=self.__grid_size
             self.__e=np.ones(shape)
             self.__mu=np.ones(shape)
             
         if self.__conductivity:
             self.__sigma=np.zeros(self.__grid_size)
         
         if self.__conductivity_m:
             self.__sigma_m=np.zeros(self.__grid_size)
+            
+            
+        if self.__cupy_enabled:
+            self.__e_cp=cp.array(self.__e)
+            self.__mu_cp=cp.array(self.__mu)
+            if self.__conductivity:self.__sigma_cp=cp.array(self.__sigma)
+            if self.__conductivity_m:self.__sigma_m_cp=cp.array(self.__sigma_m)
         
         
         
         for element in self.__emo:
             if self.__anisotropy!=element.anisotropy:
                 e=np.zeros((self.__dim,self.__dim))
                 mu=np.zeros((self.__dim,self.__dim))
                 for i in range(self.__dim):
                      e[i,i]=element.fielder[0]
                      mu[i,i]=element.fielder[1]
                 
-                fielder=e,mu,element.fielder[2]
+                fielder=e,mu,element.fielder[2]#Needs Future Action(0): sigma_m fielders are not actually rendered by renderer. If necessary physics both enabled for anisotropic materials, the action should be modified
+
             else:
                 fielder=element.fielder
+
             mfs=[a[1]-a[0] for a in element.coverage]
             if not self.__anisotropy:
                 modified_array=np.full(mfs,False,dtype=bool)
                 ad=True
             else:
                 modified_array=np.full(mfs+[self.__dim, self.__dim],False,dtype=bool)
                 ad=[[True]*self.__dim]*self.__dim
             sl=np.array([element.coverage[i][0] for i in range(self.__dim)])
             for index in itertools.product(*(range(i) for i in mfs)):
                 ind=index+sl
                 if element.isIn(ind):                    
                     modified_array[index]=ad
+
             
 
             action=(element.layer, element.coverage, modified_array, fielder)
             
             if element.eternity:
                 if 0 not in self.__start_frames:
                     self.__start_frames.add(0)
@@ -210,173 +238,240 @@
                     
                     self.__e[indices]*=np.logical_not(action[2])
                     self.__e[indices]+=np.full(mfs+[self.__dim, self.__dim],action[3][0])*action[2]
                     
                     self.__mu[indices]*=np.logical_not(action[2])
                     self.__mu[indices]+=np.full(mfs+[self.__dim, self.__dim],action[3][1])*action[2]
                     
+
                     if self.__conductivity:
                         
                         self.__sigma[indices]*=np.logical_not(action[2][:,:,:,0,0])
                         tg_a=np.full(mfs,action[3][2])*action[2][:,:,:,0,0]
                         self.__sigma[indices]+=tg_a
-                        
+
                     if self.__conductivity_m:
                             
                         self.__sigma_m[indices]*=np.logical_not(action[2][:,:,:,0,0])
                         tg_a=np.full(mfs,action[3][3])*action[2][:,:,:,0,0]
                         self.__sigma_m[indices]+=tg_a
 
-                    
+      
+                    if self.__cupy_enabled:
+                        self.__e_cp[indices]=cp.array(self.__e[indices])
+                        self.__mu_cp[indices]=cp.array(self.__mu[indices])
+                        if self.__conductivity:self.__sigma_cp[indices]=cp.array(self.__sigma[indices])
+                        if self.__conductivity_m:self.__sigma_m_cp[indices]=cp.array(self.__sigma_m[indices])
+
                 else:
                     self.__e[indices]*=np.logical_not(action[2])
                     tg_a=np.full(mfs,action[3][0])*action[2]
                     self.__e[indices]+=tg_a
                     
+                    
                     self.__mu[indices]*=np.logical_not(action[2])
                     tg_a=np.full(mfs,action[3][1])*action[2]
                     self.__mu[indices]+=tg_a
                     
                     if self.__conductivity:    
                         self.__sigma[indices]*=np.logical_not(action[2])
                         tg_a=np.full(mfs,action[3][2])*action[2]
                         self.__sigma[indices]+=tg_a
-                        
+                                                
                     if self.__conductivity_m:    
                         self.__sigma_m[indices]*=np.logical_not(action[2])
                         tg_a=np.full(mfs,action[3][3])*action[2]
                         self.__sigma_m[indices]+=tg_a
+                                                
+                        
+                    if self.__cupy_enabled:
+                        self.__e_cp[indices]=cp.array(self.__e[indices])
+                        self.__mu_cp[indices]=cp.array(self.__mu[indices])
+                        if self.__conductivity:self.__sigma_cp[indices]=cp.array(self.__sigma[indices])
+                        if self.__conductivity_m:self.__sigma_m_cp[indices]=cp.array(self.__sigma_m[indices])
                     
         if self.__conductivity:
-            self.__sigma_ex=self.__sigma*self.__Jdt*self.__dt/2/e_0/self.__e
+            if self.__cupy_enabled:
+                self.__sigma_ex=self.__sigma_cp*self.__Jdt_cp*self.__dt/e_0_2/self.__e_cp
+            else:
+                self.__sigma_ex=self.__sigma*self.__Jdt*self.__dt/e_0_2/self.__e
         if self.__conductivity_m:
-            self.__sigma_mux=self.__sigma_m*self.__Jdt*self.__dt/2/mu_0/self.__mu
+            if self.__cupy_enabled:
+                self.__sigma_mux=self.__sigma_m_cp*self.__Jdt_cp*self.__dt/mu_0_2/self.__mu_cp
+            else:
+                self.__sigma_mux=self.__sigma_m*self.__Jdt*self.__dt/mu_0_2/self.__mu
             
         
-        if self.__anisotropy:            
-            self.__e_inv=np.linalg.inv(self.__e)
-            self.__mu_inv=np.linalg.inv(self.__mu)
+        if self.__anisotropy:
+            if self.__cupy_enabled:
+                self.__e_inv=cp.linalg.inv(self.__e_cp)
+                self.__mu_inv=cp.linalg.inv(self.__mu_cp)
+            else:
+                self.__e_inv=np.linalg.inv(self.__e)
+                self.__mu_inv=np.linalg.inv(self.__mu)
+
+        if self.__cupy_enabled:
+            cp._default_memory_pool.free_all_blocks()
+
             
             
                     
     def __update_grid(self):
 
         self.__instance+=1
         
         change=False
         
-        if self.__instance in self.__start_frames:
+        if self.__instance in self.__end_frames:
             change=True
-            for action in self.__video_starters[self.__instance]:
+            for action in self.__video_terminators[self.__instance]:
+                
                 mfs=[a[1]-a[0] for a in action[1]]
                 indices=tuple([slice(k[0], k[1]) for k in action[1]])
-
                 if self.__anisotropy:
-
                     self.__e[indices]*=np.logical_not(action[2])
-                    self.__e[indices]+=np.full(mfs+[self.__dim, self.__dim],action[3][0])*action[2]
+                    self.__e[indices]+=np.full(mfs+[self.__dim, self.__dim],np.eye(self.__dim))*action[2]
                     
                     self.__mu[indices]*=np.logical_not(action[2])
-                    self.__mu[indices]+=np.full(mfs+[self.__dim, self.__dim],action[3][1])*action[2]
+                    self.__mu[indices]+=np.full(mfs+[self.__dim, self.__dim],np.eye(self.__dim))*action[2]
                     
-                    if self.__conductivity:
+                    if self.__conductivity:   
                         self.__sigma[indices]*=np.logical_not(action[2][:,:,:,0,0])
-                        tg_a=np.full(mfs,action[3][2])*action[2][:,:,:,0,0]
+                        tg_a=np.full(mfs,0)*action[2][:,:,:,0,0]
                         self.__sigma[indices]+=tg_a
                         
-                    if self.__conductivity_m:
+                    if self.__conductivity_m:   
                         self.__sigma_m[indices]*=np.logical_not(action[2][:,:,:,0,0])
-                        tg_a=np.full(mfs,action[3][3])*action[2][:,:,:,0,0]
-                        self.__sigma_m[indices]+=tg_a
+                        tg_a=np.full(mfs,0)*action[2][:,:,:,0,0]
+                        self.__sigma_m[indices]+=tg_a 
+
                     
                 else:
-                    
                     self.__e[indices]*=np.logical_not(action[2])
-                    tg_a=np.full(mfs,action[3][0])*action[2]
+                    tg_a=np.full(mfs,1.)*action[2]
                     self.__e[indices]+=tg_a
                     
                     self.__mu[indices]*=np.logical_not(action[2])
-                    tg_a=np.full(mfs,action[3][1])*action[2]
+                    tg_a=np.full(mfs,1.)*action[2]
                     self.__mu[indices]+=tg_a
                     
-                    if self.__conductivity:    
+                    if self.__conductivity:
                         self.__sigma[indices]*=np.logical_not(action[2])
-                        tg_a=np.full(mfs,action[3][2])*action[2]
-                        self.__sigma[indices]+=tg_a
+                        tg_a=np.full(mfs,0)*action[2]
+                        self.__sigma[indices]+=tg_a  
                         
-                    if self.__conductivity_m:    
+                    if self.__conductivity_m:
                         self.__sigma_m[indices]*=np.logical_not(action[2])
-                        tg_a=np.full(mfs,action[3][3])*action[2]
+                        tg_a=np.full(mfs,0)*action[2]
                         self.__sigma_m[indices]+=tg_a
-                    
-                    
-        if self.__instance in self.__end_frames:
+
+                if self.__cupy_enabled:
+                    self.__e_cp[indices]=cp.array(self.__e[indices])
+                    self.__mu_cp[indices]=cp.array(self.__mu[indices])
+                    if self.__conductivity:self.__sigma_cp[indices]=cp.array(self.__sigma[indices])
+                    if self.__conductivity_m:self.__sigma_m_cp[indices]=cp.array(self.__sigma_m[indices])
+
+        
+        if self.__instance in self.__start_frames:
             change=True
-            for action in self.__video_terminators[self.__instance]:
-                
+            for action in self.__video_starters[self.__instance]:
                 mfs=[a[1]-a[0] for a in action[1]]
                 indices=tuple([slice(k[0], k[1]) for k in action[1]])
+
                 if self.__anisotropy:
+
                     self.__e[indices]*=np.logical_not(action[2])
-                    self.__e[indices]+=np.full(mfs+[self.__dim, self.__dim],np.eye(self.__dim))*action[2]
+                    self.__e[indices]+=np.full(mfs+[self.__dim, self.__dim],action[3][0])*action[2]
                     
                     self.__mu[indices]*=np.logical_not(action[2])
-                    self.__mu[indices]+=np.full(mfs+[self.__dim, self.__dim],np.eye(self.__dim))*action[2]
+                    self.__mu[indices]+=np.full(mfs+[self.__dim, self.__dim],action[3][1])*action[2]
                     
-                    if self.__conductivity:   
+                    if self.__conductivity:
                         self.__sigma[indices]*=np.logical_not(action[2][:,:,:,0,0])
-                        tg_a=np.full(mfs,0)*action[2][:,:,:,0,0]
+                        tg_a=np.full(mfs,action[3][2])*action[2][:,:,:,0,0]
                         self.__sigma[indices]+=tg_a
                         
-                    if self.__conductivity_m:   
+                    if self.__conductivity_m:
                         self.__sigma_m[indices]*=np.logical_not(action[2][:,:,:,0,0])
-                        tg_a=np.full(mfs,0)*action[2][:,:,:,0,0]
-                        self.__sigma_m[indices]+=tg_a 
+                        tg_a=np.full(mfs,action[3][3])*action[2][:,:,:,0,0]
+                        self.__sigma_m[indices]+=tg_a
 
-                    
                 else:
+                    
                     self.__e[indices]*=np.logical_not(action[2])
-                    tg_a=np.full(mfs,1.)*action[2]
+                    tg_a=np.full(mfs,action[3][0])*action[2]
                     self.__e[indices]+=tg_a
                     
                     self.__mu[indices]*=np.logical_not(action[2])
-                    tg_a=np.full(mfs,1.)*action[2]
+                    tg_a=np.full(mfs,action[3][1])*action[2]
                     self.__mu[indices]+=tg_a
                     
-                    if self.__conductivity:
+                    if self.__conductivity:    
                         self.__sigma[indices]*=np.logical_not(action[2])
-                        tg_a=np.full(mfs,0)*action[2]
-                        self.__sigma[indices]+=tg_a  
+                        tg_a=np.full(mfs,action[3][2])*action[2]
+                        self.__sigma[indices]+=tg_a
                         
-                    if self.__conductivity_m:
+                    if self.__conductivity_m:    
                         self.__sigma_m[indices]*=np.logical_not(action[2])
-                        tg_a=np.full(mfs,0)*action[2]
+                        tg_a=np.full(mfs,action[3][3])*action[2]
                         self.__sigma_m[indices]+=tg_a
+                        
+                if self.__cupy_enabled:
+                    self.__e_cp[indices]=cp.array(self.__e[indices])
+                    self.__mu_cp[indices]=cp.array(self.__mu[indices])
+                    if self.__conductivity:self.__sigma_cp[indices]=cp.array(self.__sigma[indices])
+                    if self.__conductivity_m:self.__sigma_m_cp[indices]=cp.array(self.__sigma_m[indices])
+
         
                 
         if change:
             if self.__conductivity:
-                self.__sigma_ex=self.__sigma*self.__Jdt*self.__dt/2/e_0/self.__e
+                if self.__cupy_enabled:
+                    self.__sigma_ex=self.__sigma_cp*self.__Jdt*self.__dt/e_0_2/self.__e
+                else:
+                    self.__sigma_ex=self.__sigma*self.__Jdt*self.__dt/e_0_2/self.__e
             if self.__conductivity_m:
-                self.__sigma_mux=self.__sigma_m*self.__Jdt*self.__dt/2/mu_0/self.__mu
-            
+                if self.__cupy_enabled:
+                    self.__sigma_mux=self.__sigma_m_cp*self.__Jdt*self.__dt/mu_0_2/self.__mu
+                else:
+                    self.__sigma_mux=self.__sigma_m*self.__Jdt*self.__dt/mu_0_2/self.__mu
+                
             
             if self.__anisotropy:
-                self.__e_inv=np.linalg.inv(self.__e)
-                self.__mu_inv=np.linalg.inv(self.__mu)
+                if self.__cupy_enabled:
+                    self.__e_inv=cp.linalg.inv(self.__e_cp)
+                    self.__mu_inv=cp.linalg.inv(self.__mu_cp)
+                else:
+                    self.__e_inv=np.linalg.inv(self.__e)
+                    self.__mu_inv=np.linalg.inv(self.__mu)
+                    
+        if self.__cupy_enabled:
+            cp._default_memory_pool.free_all_blocks()
+
             
         
 
     def export_grid(self):
         return self.__e, self.__mu
     
     def export_field(self):
         return self.__E, self.__H
 
-    def build(self,verbose=1):
+    def build(self,verbose=1,gpu_flag=False):
+        if (not cupy_enabled and gpu_flag):
+            raise NotImplementedError("GPU resources are not available. Set gpu_flag=False")
+        
+        self.__cupy_enabled=bool(gpu_flag)
+        
+        if gpu_flag==True:
+            try:device=cp.cuda.Device(0);print(f"Building for GPU{device} Render stream.\n{int(device.mem_info[0]/1048576)}MiB({device.mem_info[0]/device.mem_info[1]*100:.1f}%) VRAM available");self.__built_for="cupy";
+            except:pass
+        else:mem=psutil.virtual_memory();print(f"Building for CPU Render stream.\n{int(mem.available/1048576)}MiB({100-mem.percent}%) RAM available");self.__built_for="numpy";
+        if cupy_enabled and not gpu_flag:warnings.warn("GPU is available. You can use GPU for accelerating the computations significantly faster. Call build(gpu_flag=1) for utilizing GPU resources", UserWarning)
+        
         if verbose:
             start=time.time()
         self.__bound=None
         self.__categorizer()
         self.__gravitonics()
         self.__emo_video_creator()
         self.__rendered=False
@@ -388,14 +483,18 @@
         if self.__anisotropy and (self.__conductivity or self.__conductivity_m):
             raise NotImplementedError("Both conductive and anisotropic materials are not permitted.")
         self.__instance=0
 
         self.__E=np.zeros((3,)+self.__grid_size)
         self.__H=np.zeros((3,)+self.__grid_size)
         
+        if gpu_flag==True:
+            self.__E_cp=cp.zeros((3,)+self.__grid_size)
+            self.__H_cp=cp.zeros((3,)+self.__grid_size)
+        
         if verbose:
             rt=time.time()-start
 
             print(f"Built in {self.__convert_to_time(rt)}  {self.__prefix_quantifier(np.prod(self.__grid_size)/rt)}Points/s\n")
     
     @staticmethod
     def __prefix_quantifier(quantity):
@@ -967,15 +1066,15 @@
             
             
             for t in range(args[0]):
                 
                 
                 if self.__conductivity_m:
                     
-                    self.__H=self.__H *(1-self.__sigma_mux)/(1+self.__sigma_mux)+ pre_E()*Z_c2/self.__e/(1+self.__sigma_mux)
+                    self.__H=self.__H *(1-self.__sigma_mux)/(1+self.__sigma_mux)+ pre_E()*Z_c2/self.__mu/(1+self.__sigma_mux)
                 else:
                     self.__H+=pre_E()*Z_c2/self.__mu
                     
                     
                     
                 if self.__conductivity:
                     self.__E=self.__E*(1-self.__sigma_ex)/(1+self.__sigma_ex)+pre_H()*Z_c1/self.__e/(1+self.__sigma_ex)
@@ -1118,14 +1217,204 @@
                         self.__E[:, :, :, -2] = -self.__E[:, :, :, -3]
                         self.__H[:, :, :, -2] = -self.__H[:, :, :, -3]
 
 
                             
         if obs:
             return obs_array
+        
+    def __cupy_renderer(self, *args):
+        if args[1]:
+            obs=True
+            n_obs=len(args[1])
+            obs_array=np.empty((args[0],n_obs,3))
+            
+        else:
+            obs=False
+            
+        if self.__dim==2:
+            Z_c1=Z_0/2**.5*self.__Jdt_cp
+            Z_c2=1/Z_0/2**.5*self.__Jdt_cp
+            arr_shape=self.__E.shape
+
+
+            def pre_E():
+                ind = cp.zeros(arr_shape)
+            
+                ind[0,:,:-1] += self.__E_cp[2,:,1:] - self.__E_cp[2,:,:-1]
+                ind[1,:-1,:] -= self.__E_cp[2,1:,:] - self.__E_cp[2,:-1,:]
+            
+                return ind
+            
+            
+            def pre_H():
+                ind = cp.zeros(arr_shape)
+                
+                ind[2,:,1:] += self.__H_cp[0,:,1:] - self.__H_cp[0,:,:-1]
+                ind[2,1:,:] -= self.__H_cp[1,1:,:] - self.__H_cp[1,:-1,:]
+                return ind
+            
+            start_time=time.time()
+            
+            
+            for t in range(args[0]):
+                
+                
+                if self.__conductivity_m:
+                    
+                    self.__H_cp=self.__H_cp *(1-self.__sigma_mux)/(1+self.__sigma_mux)+ pre_E()*Z_c2/self.__mu_cp/(1+self.__sigma_mux)
+                else:
+                    self.__H_cp+=pre_E()*Z_c2/self.__mu_cp
+                                        
+                    
+                    
+                if self.__conductivity:
+                    self.__E_cp=self.__E_cp*(1-self.__sigma_ex)/(1+self.__sigma_ex)+pre_H()*Z_c1/self.__e_cp/(1+self.__sigma_ex)
+                    
+                else:
+                    self.__E_cp+=pre_H()*Z_c1/self.__e_cp
+
+
+                for energizer in self.__energizers:
+                    self.__E_cp[:,energizer.location[0],energizer.location[1]]=cp.array(energizer(t))
+                
+                self.__update_grid()
+
+                
+                if t%10==0:
+                    self.__create_progress_bar_with_ETA(start_time,t,args[0])
+                    
+                if obs:
+                    for i in range(n_obs):
+                        for ind in range(3):
+                            obs_array[t,i,ind]=self.__E_cp[ind][args[1][i]]
+                            
+                if self.__bound_bool:
+                    if self.__bound[2]==1:
+                        self.__E_cp[2,:,0]=-self.__E_cp[2,:,1]
+                        self.__H_cp[0,:,0]=-self.__H_cp[0,:,1]
+                    
+                    if self.__bound[3]==1:
+                        self.__E_cp[2,:,-1]=-self.__E_cp[2,:,-2]
+                        self.__H_cp[0,:,-2]=-self.__H_cp[0,:,-3]
+                        
+                    if self.__bound[1]==1:
+                        self.__E_cp[2,-1]=-self.__E_cp[2,-2]
+                        self.__H_cp[1,-2]=-self.__H_cp[1,-3]
+                        
+                    if self.__bound[0]==1:
+                        self.__E_cp[2,0]=-self.__E_cp[2,1]
+                        self.__H_cp[1,0]=-self.__H_cp[1,1]
+
+
+
+        elif self.__dim==3:
+            
+            
+            Z_c1=Z_0/3**.5
+            Z_c2=1/Z_0/3**.5
+            arr_shape=self.__E.shape
+            
+            def pre_E():
+                ind = cp.zeros(arr_shape)
+            
+                ind[0,:,:-1,:] += self.__E_cp[2,:,1:,:] - self.__E_cp[2,:,:-1,:]
+                ind[0,:,:,:-1] -= self.__E_cp[1,:,:,1:] - self.__E_cp[1,:,:,:-1]
+                ind[1,:,:,:-1] += self.__E_cp[0,:,:,1:] - self.__E_cp[0,:,:,:-1]
+                ind[1,:-1,:,:] -= self.__E_cp[2,1:,:,:] - self.__E_cp[2,:-1,:,:]
+                ind[2,:-1,:,:] += self.__E_cp[1,1:,:,:] - self.__E_cp[1,:-1,:,:]
+                ind[2,:,:-1,:] -= self.__E_cp[0,:,1:,:] - self.__E_cp[0,:,:-1,:]
+            
+                return ind
+            
+            
+            def pre_H():
+                ind = cp.zeros(arr_shape)
+                
+                ind[0,:,:,1:] += self.__H_cp[1,:,:,1:] - self.__H_cp[1,:,:,:-1]
+                ind[0,:,1:,:] -= self.__H_cp[2,:,1:,:] - self.__H_cp[2,:,:-1,:]
+                ind[1,1:,:,:] += self.__H_cp[2,1:,:,:] - self.__H_cp[2,:-1,:,:]
+                ind[1,:,:,1:] -= self.__H_cp[0,:,:,1:] - self.__H_cp[0,:,:,:-1]
+                ind[2,:,1:,:] += self.__H_cp[0,:,1:,:] - self.__H_cp[0,:,:-1,:]
+                ind[2,1:,:,:] -= self.__H_cp[1,1:,:,:] - self.__H_cp[1,:-1,:,:]        
+                return ind
+            
+            start_time=time.time()
+            
+            coord_E=self.__Jdt_cp*Z_c1
+            coord_H=self.__Jdt_cp*Z_c2
+                
+            
+            
+            for t in range(args[0]):
+                    
+                if self.__anisotropy:
+                    self.__H_cp+=cp.einsum("klmij,jklm->iklm",self.__mu_inv,pre_E())*coord_H
+                    self.__E_cp+=cp.einsum("klmij,jklm->iklm",self.__e_inv,pre_H())*coord_E
+                        
+                else:
+                    if self.__conductivity_m:
+                        self.__H_cp=self.__H_cp*(1-self.__sigma_mux)/(1+self.__sigma_mux)+pre_E()*coord_H/self.__mu_cp/(1+self.__sigma_mux)
+
+                    else:
+                        self.__H_cp+=pre_E()*coord_H/self.__mu_cp
+                        
+                        
+                    if self.__conductivity:
+                        self.__E_cp=self.__E_cp*(1-self.__sigma_ex)/(1+self.__sigma_ex)+pre_H()*coord_E/self.__e_cp/(1+self.__sigma_ex)
+                    else:
+                        self.__E_cp+=pre_H()*coord_E/self.__e_cp
+                
+                
+                for energizer in self.__energizers:
+                    self.__E_cp[:,energizer.location[0],energizer.location[1],energizer.location[2]]=cp.array(energizer(t))
+                
+                self.__update_grid()
+                
+                self.__create_progress_bar_with_ETA(start_time,t,args[0])
+                    
+                if obs:
+                    for i in range(n_obs):
+                        for ind in range(3):
+                            obs_array[t,i,ind]=self.__E_cp[ind][args[1][i]]
+                            
+        
+                if self.__bound_bool:
+                    # Boundaries in the x-direction
+                    if self.__bound[0] == 1:
+                        self.__E_cp[:, 0, :, :] = self.__E_cp[:, 1, :, :]
+                        self.__H_cp[:, 0, :, :] = self.__H_cp[:, 1, :, :]
+                
+                    if self.__bound[1] == 1:
+                        self.__E_cp[:, -2, :, :] = -self.__E_cp[:, -3, :, :]
+                        self.__H_cp[:, -2, :, :] = -self.__H_cp[:, -3, :, :]
+                
+                    # Boundaries in the y-direction
+                    if self.__bound[2] == 1:
+                        self.__E_cp[:, :, 0, :] = self.__E_cp[:, :, 1, :]
+                        self.__H_cp[:, :, 0, :] = self.__H_cp[:, :, 1, :]
+                
+                    if self.__bound[3] == 1:
+                        self.__E_cp[:, :, -2, :] = -self.__E_cp[:, :, -3, :]
+                        self.__H_cp[:, :, -2, :] = -self.__H_cp[:, :, -3, :]
+                
+                    # Boundaries in the z-direction
+                    if self.__bound[4] == 1:
+                        self.__E_cp[:, :, :, 0] = self.__E_cp[:, :, :, 1]
+                        self.__H_cp[:, :, :, 0] = self.__H_cp[:, :, :, 1]
+
+                
+                    if self.__bound[5] == 1:
+                        self.__E_cp[:, :, :, -2] = -self.__E_cp[:, :, :, -3]
+                        self.__H_cp[:, :, :, -2] = -self.__H_cp[:, :, :, -3]
+
+
+                            
+        if obs:
+            return obs_array
                 
 
     def Render(self, time_steps, backend="numpy", observers=None):
         
         if type(time_steps)!=int:
             raise TypeError("time_steps must be an int")
         
@@ -1150,35 +1439,49 @@
         
         if not self.__built:
             raise NotImplementedError("The Continuum should be built first. Call build() method first.")
         
         start_time=time.time()
 
         if backend.upper()=="NUMPY":
+            if self.__cupy_enabled==True and (self.__conductivity or self.__conductivity_m or self.__anisotropy):
+                raise NotImplementedError("Prebuilt anisotropic or conductive medium for GPU is not available for NUMPY renderer.\nBuild for non-GPU or use 'cupy' as backend")
             obs=self.__numpy_renderer(time_steps, observers)
+            time_elapsed=time.time()-start_time
+            print(f"\nRendered Succesfully\nElapsed Time : {self.__convert_to_time(time_elapsed)} , {time_elapsed/time_steps} s/step\nRender Stream Rate : {self.__prefix_quantifier(np.prod(self.__grid_size)/time_elapsed*time_steps)}Points/s")
+            
+        elif backend.upper()=="CUPY":
+            if self.__built_for!="cupy":
+                raise ValueError("set build(gpu_flag=1) for utilizing GPU resources")
+            obs=self.__cupy_renderer(time_steps, observers)
+            time_elapsed=time.time()-start_time
+            print(f"\nRendered Succesfully\nElapsed Time : {self.__convert_to_time(time_elapsed)} , {time_elapsed/time_steps} s/step\nRender Stream Rate : {self.__prefix_quantifier(np.prod(self.__grid_size)/time_elapsed*time_steps)}Points/s")
+            cp._default_memory_pool.free_all_blocks()
+
+            print("Transfering from GPU to host memory...")
+            start_t=time.time()
+            self.__E=self.__E_cp.get()
+            self.__H=self.__H_cp.get()
+            end_t=time.time()
+            print(f"Data transferred in {end_t-start_t} secs")
         
         elif backend.upper()=="C++":
             raise ValueError("C++ renderer will be added in future releases")#self.__cpp_renderer(time_steps, observers)
         
         elif backend.upper()=="CUDA":
             raise ValueError("CUDA based GPU enabled renderer will be added in future releases")#self.__nvcc_render(time_steps, observers)
         
         elif backend.upper()=="FPGA":
             raise ValueError("FPGA based hardware accelerator will be added in future releases")#self.__fpga_renderer(time_steps, observers)
         
         else:
             raise ValueError(f"'{backend}' is not a recognized backend. Check for any typo. Supported background is:\n'numpy'")#raise ValueError(f"{backend} is not a recognized backend. Check for any typo. Supported backgrounds are:\n'numpy','C++','CUDA', 'FPGA")
-       
-        
-       
-       
+
         
-        time_elapsed=time.time()-start_time
 
-        print(f"\nRendered Succesfully\nElapsed Time : {self.__convert_to_time(time_elapsed)} , {time_elapsed/time_steps} s/step\nRender Stream Rate : {self.__prefix_quantifier(np.prod(self.__grid_size)/time_elapsed*time_steps)}Points/s")
         self.__rendered=True
         return obs
     
 
     
     @property
     def isbuilt(self):
@@ -1379,8 +1682,7 @@
     def __validator(inn):
         if inn not in {"ABC","PEC"}:
             raise ValueError("boundary type must be ABC, PBC or PEC.\nBoundary Types:\nPEC(Perfect Electric Conductor): Reflects all waves perfectly\nABC(Absorbing Boundary Conditions): Absorbs all waves.\n")
         return True
     @property
     def dimensionality(self):
         return self.__dim
-
```

### Comparing `glimy-4.2.5/src/glimy/geo.py` & `glimy-5.0.0/src/glimy/geo.py`

 * *Files identical despite different names*

### Comparing `glimy-4.2.5/src/glimy.egg-info/PKG-INFO` & `glimy-5.0.0/src/glimy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: glimy
-Version: 4.2.5
-Summary: Computational Electromagnetics Package with Dielectic, Magnetic Materials and Gravity
+Version: 5.0.0
+Summary: Computational Electromagnetics Package with Dielectic, Magnetic, Anisotropic, Lossy Materials and Gravity
 Author-email: Ali Hakim Taskiran <alihakimxyz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
         
 Project-URL: Homepage, https://github.com/alihakimtaskiran/Glimy
 Project-URL: Bug Tracker, https://github.com/alihakimtaskiran/Glimy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Glimy
 ## FDTD Simulator
 <img src="https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/logo.png" width="200"></img>
```

