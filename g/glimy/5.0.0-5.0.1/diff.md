# Comparing `tmp/glimy-5.0.0.tar.gz` & `tmp/glimy-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glimy-5.0.0.tar", last modified: Sat Jun 24 21:26:30 2023, max compression
+gzip compressed data, was "glimy-5.0.1.tar", last modified: Sat Jun 24 21:40:46 2023, max compression
```

## Comparing `glimy-5.0.0.tar` & `glimy-5.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:26:30.654988 glimy-5.0.0/
--rw-rw-r--   0 ali       (1000) ali       (1000)       47 2022-11-11 09:33:29.000000 glimy-5.0.0/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)    21684 2023-06-24 21:26:30.650988 glimy-5.0.0/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)    21000 2023-03-22 01:12:57.000000 glimy-5.0.0/README.md
--rw-rw-r--   0 ali       (1000) ali       (1000)      769 2023-06-24 21:25:04.000000 glimy-5.0.0/pyproject.toml
--rw-rw-r--   0 ali       (1000) ali       (1000)       38 2023-06-24 21:26:30.654988 glimy-5.0.0/setup.cfg
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:26:30.650988 glimy-5.0.0/src/
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:26:30.650988 glimy-5.0.0/src/glimy/
--rw-rw-r--   0 ali       (1000) ali       (1000)    67803 2023-06-24 21:23:50.000000 glimy-5.0.0/src/glimy/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    26917 2023-05-05 09:58:12.000000 glimy-5.0.0/src/glimy/geo.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:26:30.650988 glimy-5.0.0/src/glimy.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)    21684 2023-06-24 21:26:30.000000 glimy-5.0.0/src/glimy.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      235 2023-06-24 21:26:30.000000 glimy-5.0.0/src/glimy.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-24 21:26:30.000000 glimy-5.0.0/src/glimy.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       25 2023-06-24 21:26:30.000000 glimy-5.0.0/src/glimy.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        6 2023-06-24 21:26:30.000000 glimy-5.0.0/src/glimy.egg-info/top_level.txt
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:40:46.051267 glimy-5.0.1/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       47 2022-11-11 09:33:29.000000 glimy-5.0.1/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)    22580 2023-06-24 21:40:46.051267 glimy-5.0.1/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)    21896 2023-06-24 21:39:52.000000 glimy-5.0.1/README.md
+-rw-rw-r--   0 ali       (1000) ali       (1000)      768 2023-06-24 21:40:04.000000 glimy-5.0.1/pyproject.toml
+-rw-rw-r--   0 ali       (1000) ali       (1000)       38 2023-06-24 21:40:46.051267 glimy-5.0.1/setup.cfg
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:40:46.047267 glimy-5.0.1/src/
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:40:46.047267 glimy-5.0.1/src/glimy/
+-rw-rw-r--   0 ali       (1000) ali       (1000)    67803 2023-06-24 21:23:50.000000 glimy-5.0.1/src/glimy/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    26917 2023-05-05 09:58:12.000000 glimy-5.0.1/src/glimy/geo.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-24 21:40:46.047267 glimy-5.0.1/src/glimy.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)    22580 2023-06-24 21:40:46.000000 glimy-5.0.1/src/glimy.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      235 2023-06-24 21:40:46.000000 glimy-5.0.1/src/glimy.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-24 21:40:46.000000 glimy-5.0.1/src/glimy.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       24 2023-06-24 21:40:46.000000 glimy-5.0.1/src/glimy.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        6 2023-06-24 21:40:46.000000 glimy-5.0.1/src/glimy.egg-info/top_level.txt
```

### Comparing `glimy-5.0.0/PKG-INFO` & `glimy-5.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glimy
-Version: 5.0.0
+Version: 5.0.1
 Summary: Computational Electromagnetics Package with Dielectic, Magnetic, Anisotropic, Lossy Materials and Gravity
 Author-email: Ali Hakim Taskiran <alihakimxyz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
         
 Project-URL: Homepage, https://github.com/alihakimtaskiran/Glimy
 Project-URL: Bug Tracker, https://github.com/alihakimtaskiran/Glimy/issues
 Classifier: Programming Language :: Python :: 3
@@ -17,23 +17,34 @@
 # Glimy
 ## FDTD Simulator
 <img src="https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/logo.png" width="200"></img>
 
   The electromagnetic field.. Interacts with our reality and the reason that we continue to live. We can live beter, if we know time evolution of electromagnetic field. 
   Moreover, Glimy can simulate behaviour of light near massive objects(i.e neutron stars, blackholes). It utilizes VSL Theory of **Mach-Einstein-Dicke**.
   Glimy can simulate photonic devices with varying refractive index through time.
+### CPU-only
 <pre>
 pip install glimy
 </pre>
+### GPU-only
+Make sure that Nvidia drivers and CUDA is successfully installed. Then proceed with installing cupy.
+
+See ![GPU usage example](https://github.com/alihakimtaskiran/Glimy/blob/main/examples/7-GPU.py)
+<pre>
+pip install cupy # See https://docs.cupy.dev/en/stable/install.html#installing-cupy for more information
+pip install glimy
+</pre>
 ## Capabilities
+-  GPU Support(install **cupy** to access GPU resources)
 -  Electromagnetic waves in dielectric and magnetic materials.
 -  Gravitational effect on electromagnetism
 -  Anisotropic materials
 -  Lossy medium and conductive materials(both electric and magnetic)
 -  Objects can be inserted and omitted through the time
+-  Can be integrated into GPT-4
 ### ![Strong Gravitational Potential](examples/2-Near-Massive-Object.py)
 ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/5.png)     ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/6.png)
 
 ### ![Waveguide Example](examples/1-Dielectric-Wave-Guide.py):
 ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/3.png)     ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/4.png)
 
 <hr/>
@@ -50,15 +61,15 @@
 ### Tree
 <pre>
 |----Continuum(object)----|
 |                         |---__init__(grid_size,ds)
 |                         |---add(arg)
 |                         |---export_grid()
 |                         |---export_field()
-|                         |---build(verbose=1)
+|                         |---build(verbose=1,gpu_flag=False)
 |                         |---impose_grid(e,mu,sigma=False,sigma_m=False,anisotropy=(False,False))
 |                         |---view_(field="t",*args,colorbar=True)
 |                         |---view_structure(field="e",*args,colorbar=True)
 |                         |---view_field(field="E",*args,colorbar=True)
 |                         |---Render(time_steps,backend="numpy",observers=None)
 |
 |
@@ -119,25 +130,26 @@
                                                           |---__init__(A,r,h,layer=0,e=1,mu=1,sigma=0,sigma_m=0,time=None)
           
   </pre>
   
   # Documentation
   <hr/>
   
-  ## Continuum(dim,grid_size,ds)
+  ## Continuum(grid_size,ds)
    Creates electromagnetic field with given dimensions and grid size. Grid spacing is introduced with ds.
    - **grid_size** : Defines grid cell count per axis. It may take a tuple or list. It's 2D or 3D.
    - **ds** : Length of a edge of a grid cell. It may take a float or integer. **All units are SI**.
 
 ### add(arg)
   Adds either new geometries, celestial objects and sources into the Continuum.
   - **arg** : It adds new objects into the grid. It can take either defined object or list/tuple of them(recursively). It can take tuple, list, set, everything in **geo**(**geo.\***) and **DotSource**. As long as dimensionality of object and Continuum is the same, it is added.
-### build(verbose=1)
+### build(verbose=1, gpu_flag=False)
    Builds the dielectric, magnetic and geometrodynamic structure. 
    - **verbose**: Determines whether info is displayed. If 0, nothing displayed. If 1, render time is displayed.
+   - **gpu_flag**: Determines whether the grid is compiled for GPU.
 ### export_field()
   Get Electric and Magnetic Field arrays. It returns a tuple (E, H).
 ### export_grid()
   Get permittivity and permeability arrays. It returns a tuple (e, mu).
 ### impose_grid(e,mu,sigma=False,sigma_m=False,anisotropy=(False,False))
   Embed the electromagnetic grid - generated by other sources -. It is useful for fetching electromagnetic material structure from any optimization algorithm and examining it's electromagnetic properties with **glimy**.
   - **e**: Epsilon of each point of the grid. Shape of the array is (Nx, Ny,...) in isotropic media; (3,Nx,Ny,Nz) in anisotopic media.
@@ -159,15 +171,15 @@
   You can view geometrodynamic curvature due to the massive objects in the grid.
   - **field** : It takes "t" for curvatures in time. No other grids are not compatible yet.
   - **\*args** : Only used in 3D. It used specify axis of view. Plane and and index number can be inserted. For example "z", 10 corresponds z=10 plane in the 3D array. "x","y","z" can be inserted. Also "yz", "xz", "xy" are synonym respectively.
   - **colorbar**: If is is set to **True**, colorbar is displayed.
 ### Render(time_steps,backend="numpy",observers=None)
    Executes FDTD calculations on a Continuum object.
    - **time_steps** : It is number of time steps that field will evolve. It may take an integer. Lenght of time steps is given by ds/c/(<span>&#8730;</span>dim) ; where ds is grid spacing, c is speed of light and dim is number of dimensions of the grid. All units are SI.
-   - **backend** : It sets the backend. Only **numpy** is supported recently. Therefore it is always **numpy**
+   - **backend** : It sets the backend. For CPU-only version, use **backend="numpy"**. IF GPU is enabled, then use **backend=cupy**. Make sure that the Continuum instance was built with gpu_flag=1 for accessing GPU acceleration.
    - **observers** : Determines whether time dependent logging will be the case. If it is set to <code>None</code>, time dependent observation is not the case. However, it is a tuple or list of points e.g <code>[ (0,0), (2,2) ]</code> then it returns E-field amplitude of each given point. Returned array's order is the same as implicit order of the fed list/tuple.
 <hr/> 
 
 
   ## DotSource(location,presence,amplitude,frequency,phase=0)
    Creates a point source on a given place on grid, through given time interval with given amplitude, frequency and phase.
    - **location** : It is location of dot source. It may take a list or tuple. 
@@ -177,20 +189,27 @@
    - **phase** : Phase of the wave. It may take int or float. It is default 0.
 
   ## Boundaries(subject_grid_dim, all_bound="ABC")
   The Boundaries class allows users to define boundary conditions for the grid in 2D or 3D space. There are two supported boundary types:
    PEC (Perfect Electric Conductor): Reflects all waves perfectly
    ABC (Absorbing Boundary Conditions): Absorbs all waves
    
-  -L(self, boundary_type="ABC"): Sets the left boundary condition.
-  -R(self, boundary_type="ABC"): Sets the right boundary condition.
-  -B(self, boundary_type="ABC"): Sets the backward boundary condition.
-  -F(self, boundary_type="ABC"): Sets the forward boundary condition.
-  -D(self, boundary_type="ABC"): Sets the down boundary condition (for 3D grids only).
-  -U(self, boundary_type="ABC"): Sets the up boundary condition (for 3D grids only).
+  - L(self, boundary_type="ABC"): Sets the left boundary condition.
+  - R(self, boundary_type="ABC"): Sets the right boundary condition.
+  - B(self, boundary_type="ABC"): Sets the backward boundary condition.
+  - F(self, boundary_type="ABC"): Sets the forward boundary condition.
+  - D(self, boundary_type="ABC"): Sets the down boundary condition (for 3D grids only).
+  - U(self, boundary_type="ABC"): Sets the up boundary condition (for 3D grids only).
+  A short example:
+  <code>
+  boundaries = Boundaries(3)  # Creates a 3D grid with default ABC boundaries
+  boundaries.L("PEC")  # Sets the left boundary to PEC
+  boundaries.R("PEC")  # Sets the right boundary to PEC
+  </code>
+
   
   ## geo.SingularCelestial(location, mass):
    Creates a point mass.
    - **location** : Sets the location of point mass. Unit is **meters**. It may take tuple, list or np.array. It must bu in form of N-tuple. It may be outside of the grid.
    - **mass** : Stest the mass of the object. Unit is **kg**. It may take float ot int.
   ## geo.MassiveCluster(objects,volatile=False)
   Creates cluster of massive objects. It is used to integrate so many heavy objects.
```

### Comparing `glimy-5.0.0/README.md` & `glimy-5.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 # Glimy
 ## FDTD Simulator
 <img src="https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/logo.png" width="200"></img>
 
   The electromagnetic field.. Interacts with our reality and the reason that we continue to live. We can live beter, if we know time evolution of electromagnetic field. 
   Moreover, Glimy can simulate behaviour of light near massive objects(i.e neutron stars, blackholes). It utilizes VSL Theory of **Mach-Einstein-Dicke**.
   Glimy can simulate photonic devices with varying refractive index through time.
+### CPU-only
 <pre>
 pip install glimy
 </pre>
+### GPU-only
+Make sure that Nvidia drivers and CUDA is successfully installed. Then proceed with installing cupy.
+
+See ![GPU usage example](https://github.com/alihakimtaskiran/Glimy/blob/main/examples/7-GPU.py)
+<pre>
+pip install cupy # See https://docs.cupy.dev/en/stable/install.html#installing-cupy for more information
+pip install glimy
+</pre>
 ## Capabilities
+-  GPU Support(install **cupy** to access GPU resources)
 -  Electromagnetic waves in dielectric and magnetic materials.
 -  Gravitational effect on electromagnetism
 -  Anisotropic materials
 -  Lossy medium and conductive materials(both electric and magnetic)
 -  Objects can be inserted and omitted through the time
+-  Can be integrated into GPT-4
 ### ![Strong Gravitational Potential](examples/2-Near-Massive-Object.py)
 ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/5.png)     ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/6.png)
 
 ### ![Waveguide Example](examples/1-Dielectric-Wave-Guide.py):
 ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/3.png)     ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/4.png)
 
 <hr/>
@@ -34,15 +45,15 @@
 ### Tree
 <pre>
 |----Continuum(object)----|
 |                         |---__init__(grid_size,ds)
 |                         |---add(arg)
 |                         |---export_grid()
 |                         |---export_field()
-|                         |---build(verbose=1)
+|                         |---build(verbose=1,gpu_flag=False)
 |                         |---impose_grid(e,mu,sigma=False,sigma_m=False,anisotropy=(False,False))
 |                         |---view_(field="t",*args,colorbar=True)
 |                         |---view_structure(field="e",*args,colorbar=True)
 |                         |---view_field(field="E",*args,colorbar=True)
 |                         |---Render(time_steps,backend="numpy",observers=None)
 |
 |
@@ -103,25 +114,26 @@
                                                           |---__init__(A,r,h,layer=0,e=1,mu=1,sigma=0,sigma_m=0,time=None)
           
   </pre>
   
   # Documentation
   <hr/>
   
-  ## Continuum(dim,grid_size,ds)
+  ## Continuum(grid_size,ds)
    Creates electromagnetic field with given dimensions and grid size. Grid spacing is introduced with ds.
    - **grid_size** : Defines grid cell count per axis. It may take a tuple or list. It's 2D or 3D.
    - **ds** : Length of a edge of a grid cell. It may take a float or integer. **All units are SI**.
 
 ### add(arg)
   Adds either new geometries, celestial objects and sources into the Continuum.
   - **arg** : It adds new objects into the grid. It can take either defined object or list/tuple of them(recursively). It can take tuple, list, set, everything in **geo**(**geo.\***) and **DotSource**. As long as dimensionality of object and Continuum is the same, it is added.
-### build(verbose=1)
+### build(verbose=1, gpu_flag=False)
    Builds the dielectric, magnetic and geometrodynamic structure. 
    - **verbose**: Determines whether info is displayed. If 0, nothing displayed. If 1, render time is displayed.
+   - **gpu_flag**: Determines whether the grid is compiled for GPU.
 ### export_field()
   Get Electric and Magnetic Field arrays. It returns a tuple (E, H).
 ### export_grid()
   Get permittivity and permeability arrays. It returns a tuple (e, mu).
 ### impose_grid(e,mu,sigma=False,sigma_m=False,anisotropy=(False,False))
   Embed the electromagnetic grid - generated by other sources -. It is useful for fetching electromagnetic material structure from any optimization algorithm and examining it's electromagnetic properties with **glimy**.
   - **e**: Epsilon of each point of the grid. Shape of the array is (Nx, Ny,...) in isotropic media; (3,Nx,Ny,Nz) in anisotopic media.
@@ -143,15 +155,15 @@
   You can view geometrodynamic curvature due to the massive objects in the grid.
   - **field** : It takes "t" for curvatures in time. No other grids are not compatible yet.
   - **\*args** : Only used in 3D. It used specify axis of view. Plane and and index number can be inserted. For example "z", 10 corresponds z=10 plane in the 3D array. "x","y","z" can be inserted. Also "yz", "xz", "xy" are synonym respectively.
   - **colorbar**: If is is set to **True**, colorbar is displayed.
 ### Render(time_steps,backend="numpy",observers=None)
    Executes FDTD calculations on a Continuum object.
    - **time_steps** : It is number of time steps that field will evolve. It may take an integer. Lenght of time steps is given by ds/c/(<span>&#8730;</span>dim) ; where ds is grid spacing, c is speed of light and dim is number of dimensions of the grid. All units are SI.
-   - **backend** : It sets the backend. Only **numpy** is supported recently. Therefore it is always **numpy**
+   - **backend** : It sets the backend. For CPU-only version, use **backend="numpy"**. IF GPU is enabled, then use **backend=cupy**. Make sure that the Continuum instance was built with gpu_flag=1 for accessing GPU acceleration.
    - **observers** : Determines whether time dependent logging will be the case. If it is set to <code>None</code>, time dependent observation is not the case. However, it is a tuple or list of points e.g <code>[ (0,0), (2,2) ]</code> then it returns E-field amplitude of each given point. Returned array's order is the same as implicit order of the fed list/tuple.
 <hr/> 
 
 
   ## DotSource(location,presence,amplitude,frequency,phase=0)
    Creates a point source on a given place on grid, through given time interval with given amplitude, frequency and phase.
    - **location** : It is location of dot source. It may take a list or tuple. 
@@ -161,20 +173,27 @@
    - **phase** : Phase of the wave. It may take int or float. It is default 0.
 
   ## Boundaries(subject_grid_dim, all_bound="ABC")
   The Boundaries class allows users to define boundary conditions for the grid in 2D or 3D space. There are two supported boundary types:
    PEC (Perfect Electric Conductor): Reflects all waves perfectly
    ABC (Absorbing Boundary Conditions): Absorbs all waves
    
-  -L(self, boundary_type="ABC"): Sets the left boundary condition.
-  -R(self, boundary_type="ABC"): Sets the right boundary condition.
-  -B(self, boundary_type="ABC"): Sets the backward boundary condition.
-  -F(self, boundary_type="ABC"): Sets the forward boundary condition.
-  -D(self, boundary_type="ABC"): Sets the down boundary condition (for 3D grids only).
-  -U(self, boundary_type="ABC"): Sets the up boundary condition (for 3D grids only).
+  - L(self, boundary_type="ABC"): Sets the left boundary condition.
+  - R(self, boundary_type="ABC"): Sets the right boundary condition.
+  - B(self, boundary_type="ABC"): Sets the backward boundary condition.
+  - F(self, boundary_type="ABC"): Sets the forward boundary condition.
+  - D(self, boundary_type="ABC"): Sets the down boundary condition (for 3D grids only).
+  - U(self, boundary_type="ABC"): Sets the up boundary condition (for 3D grids only).
+  A short example:
+  <code>
+  boundaries = Boundaries(3)  # Creates a 3D grid with default ABC boundaries
+  boundaries.L("PEC")  # Sets the left boundary to PEC
+  boundaries.R("PEC")  # Sets the right boundary to PEC
+  </code>
+
   
   ## geo.SingularCelestial(location, mass):
    Creates a point mass.
    - **location** : Sets the location of point mass. Unit is **meters**. It may take tuple, list or np.array. It must bu in form of N-tuple. It may be outside of the grid.
    - **mass** : Stest the mass of the object. Unit is **kg**. It may take float ot int.
   ## geo.MassiveCluster(objects,volatile=False)
   Creates cluster of massive objects. It is used to integrate so many heavy objects.
```

### Comparing `glimy-5.0.0/pyproject.toml` & `glimy-5.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "glimy"
-version = "5.0.0"
+version = "5.0.1"
 authors = [
   { name="Ali Hakim Taskiran", email="alihakimxyz@gmail.com" },
 ]
 description = "Computational Electromagnetics Package with Dielectic, Magnetic, Anisotropic, Lossy Materials and Gravity"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
-dependencies=["numpy", "matplotlib","psutils"]
+dependencies=["numpy", "matplotlib","psutil"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `glimy-5.0.0/src/glimy/__init__.py` & `glimy-5.0.1/src/glimy/__init__.py`

 * *Files identical despite different names*

### Comparing `glimy-5.0.0/src/glimy/geo.py` & `glimy-5.0.1/src/glimy/geo.py`

 * *Files identical despite different names*

### Comparing `glimy-5.0.0/src/glimy.egg-info/PKG-INFO` & `glimy-5.0.1/src/glimy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glimy
-Version: 5.0.0
+Version: 5.0.1
 Summary: Computational Electromagnetics Package with Dielectic, Magnetic, Anisotropic, Lossy Materials and Gravity
 Author-email: Ali Hakim Taskiran <alihakimxyz@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
         
 Project-URL: Homepage, https://github.com/alihakimtaskiran/Glimy
 Project-URL: Bug Tracker, https://github.com/alihakimtaskiran/Glimy/issues
 Classifier: Programming Language :: Python :: 3
@@ -17,23 +17,34 @@
 # Glimy
 ## FDTD Simulator
 <img src="https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/logo.png" width="200"></img>
 
   The electromagnetic field.. Interacts with our reality and the reason that we continue to live. We can live beter, if we know time evolution of electromagnetic field. 
   Moreover, Glimy can simulate behaviour of light near massive objects(i.e neutron stars, blackholes). It utilizes VSL Theory of **Mach-Einstein-Dicke**.
   Glimy can simulate photonic devices with varying refractive index through time.
+### CPU-only
 <pre>
 pip install glimy
 </pre>
+### GPU-only
+Make sure that Nvidia drivers and CUDA is successfully installed. Then proceed with installing cupy.
+
+See ![GPU usage example](https://github.com/alihakimtaskiran/Glimy/blob/main/examples/7-GPU.py)
+<pre>
+pip install cupy # See https://docs.cupy.dev/en/stable/install.html#installing-cupy for more information
+pip install glimy
+</pre>
 ## Capabilities
+-  GPU Support(install **cupy** to access GPU resources)
 -  Electromagnetic waves in dielectric and magnetic materials.
 -  Gravitational effect on electromagnetism
 -  Anisotropic materials
 -  Lossy medium and conductive materials(both electric and magnetic)
 -  Objects can be inserted and omitted through the time
+-  Can be integrated into GPT-4
 ### ![Strong Gravitational Potential](examples/2-Near-Massive-Object.py)
 ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/5.png)     ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/6.png)
 
 ### ![Waveguide Example](examples/1-Dielectric-Wave-Guide.py):
 ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/3.png)     ![](https://github.com/alihakimtaskiran/Glimy-FDTD/raw/main/src/4.png)
 
 <hr/>
@@ -50,15 +61,15 @@
 ### Tree
 <pre>
 |----Continuum(object)----|
 |                         |---__init__(grid_size,ds)
 |                         |---add(arg)
 |                         |---export_grid()
 |                         |---export_field()
-|                         |---build(verbose=1)
+|                         |---build(verbose=1,gpu_flag=False)
 |                         |---impose_grid(e,mu,sigma=False,sigma_m=False,anisotropy=(False,False))
 |                         |---view_(field="t",*args,colorbar=True)
 |                         |---view_structure(field="e",*args,colorbar=True)
 |                         |---view_field(field="E",*args,colorbar=True)
 |                         |---Render(time_steps,backend="numpy",observers=None)
 |
 |
@@ -119,25 +130,26 @@
                                                           |---__init__(A,r,h,layer=0,e=1,mu=1,sigma=0,sigma_m=0,time=None)
           
   </pre>
   
   # Documentation
   <hr/>
   
-  ## Continuum(dim,grid_size,ds)
+  ## Continuum(grid_size,ds)
    Creates electromagnetic field with given dimensions and grid size. Grid spacing is introduced with ds.
    - **grid_size** : Defines grid cell count per axis. It may take a tuple or list. It's 2D or 3D.
    - **ds** : Length of a edge of a grid cell. It may take a float or integer. **All units are SI**.
 
 ### add(arg)
   Adds either new geometries, celestial objects and sources into the Continuum.
   - **arg** : It adds new objects into the grid. It can take either defined object or list/tuple of them(recursively). It can take tuple, list, set, everything in **geo**(**geo.\***) and **DotSource**. As long as dimensionality of object and Continuum is the same, it is added.
-### build(verbose=1)
+### build(verbose=1, gpu_flag=False)
    Builds the dielectric, magnetic and geometrodynamic structure. 
    - **verbose**: Determines whether info is displayed. If 0, nothing displayed. If 1, render time is displayed.
+   - **gpu_flag**: Determines whether the grid is compiled for GPU.
 ### export_field()
   Get Electric and Magnetic Field arrays. It returns a tuple (E, H).
 ### export_grid()
   Get permittivity and permeability arrays. It returns a tuple (e, mu).
 ### impose_grid(e,mu,sigma=False,sigma_m=False,anisotropy=(False,False))
   Embed the electromagnetic grid - generated by other sources -. It is useful for fetching electromagnetic material structure from any optimization algorithm and examining it's electromagnetic properties with **glimy**.
   - **e**: Epsilon of each point of the grid. Shape of the array is (Nx, Ny,...) in isotropic media; (3,Nx,Ny,Nz) in anisotopic media.
@@ -159,15 +171,15 @@
   You can view geometrodynamic curvature due to the massive objects in the grid.
   - **field** : It takes "t" for curvatures in time. No other grids are not compatible yet.
   - **\*args** : Only used in 3D. It used specify axis of view. Plane and and index number can be inserted. For example "z", 10 corresponds z=10 plane in the 3D array. "x","y","z" can be inserted. Also "yz", "xz", "xy" are synonym respectively.
   - **colorbar**: If is is set to **True**, colorbar is displayed.
 ### Render(time_steps,backend="numpy",observers=None)
    Executes FDTD calculations on a Continuum object.
    - **time_steps** : It is number of time steps that field will evolve. It may take an integer. Lenght of time steps is given by ds/c/(<span>&#8730;</span>dim) ; where ds is grid spacing, c is speed of light and dim is number of dimensions of the grid. All units are SI.
-   - **backend** : It sets the backend. Only **numpy** is supported recently. Therefore it is always **numpy**
+   - **backend** : It sets the backend. For CPU-only version, use **backend="numpy"**. IF GPU is enabled, then use **backend=cupy**. Make sure that the Continuum instance was built with gpu_flag=1 for accessing GPU acceleration.
    - **observers** : Determines whether time dependent logging will be the case. If it is set to <code>None</code>, time dependent observation is not the case. However, it is a tuple or list of points e.g <code>[ (0,0), (2,2) ]</code> then it returns E-field amplitude of each given point. Returned array's order is the same as implicit order of the fed list/tuple.
 <hr/> 
 
 
   ## DotSource(location,presence,amplitude,frequency,phase=0)
    Creates a point source on a given place on grid, through given time interval with given amplitude, frequency and phase.
    - **location** : It is location of dot source. It may take a list or tuple. 
@@ -177,20 +189,27 @@
    - **phase** : Phase of the wave. It may take int or float. It is default 0.
 
   ## Boundaries(subject_grid_dim, all_bound="ABC")
   The Boundaries class allows users to define boundary conditions for the grid in 2D or 3D space. There are two supported boundary types:
    PEC (Perfect Electric Conductor): Reflects all waves perfectly
    ABC (Absorbing Boundary Conditions): Absorbs all waves
    
-  -L(self, boundary_type="ABC"): Sets the left boundary condition.
-  -R(self, boundary_type="ABC"): Sets the right boundary condition.
-  -B(self, boundary_type="ABC"): Sets the backward boundary condition.
-  -F(self, boundary_type="ABC"): Sets the forward boundary condition.
-  -D(self, boundary_type="ABC"): Sets the down boundary condition (for 3D grids only).
-  -U(self, boundary_type="ABC"): Sets the up boundary condition (for 3D grids only).
+  - L(self, boundary_type="ABC"): Sets the left boundary condition.
+  - R(self, boundary_type="ABC"): Sets the right boundary condition.
+  - B(self, boundary_type="ABC"): Sets the backward boundary condition.
+  - F(self, boundary_type="ABC"): Sets the forward boundary condition.
+  - D(self, boundary_type="ABC"): Sets the down boundary condition (for 3D grids only).
+  - U(self, boundary_type="ABC"): Sets the up boundary condition (for 3D grids only).
+  A short example:
+  <code>
+  boundaries = Boundaries(3)  # Creates a 3D grid with default ABC boundaries
+  boundaries.L("PEC")  # Sets the left boundary to PEC
+  boundaries.R("PEC")  # Sets the right boundary to PEC
+  </code>
+
   
   ## geo.SingularCelestial(location, mass):
    Creates a point mass.
    - **location** : Sets the location of point mass. Unit is **meters**. It may take tuple, list or np.array. It must bu in form of N-tuple. It may be outside of the grid.
    - **mass** : Stest the mass of the object. Unit is **kg**. It may take float ot int.
   ## geo.MassiveCluster(objects,volatile=False)
   Creates cluster of massive objects. It is used to integrate so many heavy objects.
```

