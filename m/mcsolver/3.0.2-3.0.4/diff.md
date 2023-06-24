# Comparing `tmp/mcsolver-3.0.2.tar.gz` & `tmp/mcsolver-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mcsolver-3.0.2.tar", last modified: Tue May 23 16:30:41 2023, max compression
+gzip compressed data, was "dist\mcsolver-3.0.4.tar", last modified: Sat Jun 24 17:47:55 2023, max compression
```

## Comparing `mcsolver-3.0.2.tar` & `mcsolver-3.0.4.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 16:30:41.344514 mcsolver-3.0.2/
--rw-rw-rw-   0        0        0    35823 2019-12-13 12:05:28.000000 mcsolver-3.0.2/LICENSE
--rw-rw-rw-   0        0        0       72 2021-05-31 04:17:53.000000 mcsolver-3.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     8308 2023-05-23 16:30:41.343511 mcsolver-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6844 2023-05-23 15:21:53.000000 mcsolver-3.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-23 16:30:41.318511 mcsolver-3.0.2/mcsolver/
--rw-rw-rw-   0        0        0    14449 2023-05-23 15:54:54.000000 mcsolver-3.0.2/mcsolver/Lattice.py
--rw-rw-rw-   0        0        0    16327 2020-11-19 06:14:17.000000 mcsolver-3.0.2/mcsolver/WannierKit.py
--rw-rw-rw-   0        0        0      536 2023-05-23 16:29:59.000000 mcsolver-3.0.2/mcsolver/__init__.py
--rw-rw-rw-   0        0        0     8390 2023-05-22 11:26:05.000000 mcsolver-3.0.2/mcsolver/auxiliary.py
--rw-rw-rw-   0        0        0    13828 2023-05-23 14:42:07.000000 mcsolver-3.0.2/mcsolver/fileio.py
--rw-rw-rw-   0        0        0    18917 2023-05-21 12:26:44.000000 mcsolver-3.0.2/mcsolver/guiMain.py
--rw-rw-rw-   0        0        0    33812 2023-05-23 12:36:14.000000 mcsolver-3.0.2/mcsolver/heisenbergLib.c
--rw-rw-rw-   0        0        0    73138 2023-05-23 14:53:37.000000 mcsolver-3.0.2/mcsolver/heisenberglib.so
--rw-rw-rw-   0        0        0     1187 2021-01-29 17:10:03.000000 mcsolver-3.0.2/mcsolver/input.py
--rw-rw-rw-   0        0        0    11504 2021-01-21 13:51:41.000000 mcsolver-3.0.2/mcsolver/interface2swt.py
--rw-rw-rw-   0        0        0    20702 2021-01-29 17:13:41.000000 mcsolver-3.0.2/mcsolver/isingLib.c
--rw-rw-rw-   0        0        0    63552 2021-01-29 17:13:48.000000 mcsolver-3.0.2/mcsolver/isinglib.so
--rw-rw-rw-   0        0        0    25045 2023-05-23 14:28:57.000000 mcsolver-3.0.2/mcsolver/mcMain.py
--rw-rw-rw-   0        0        0     3540 2019-12-14 04:31:12.000000 mcsolver-3.0.2/mcsolver/toolbox.py
--rw-rw-rw-   0        0        0     8720 2023-05-23 15:14:43.000000 mcsolver-3.0.2/mcsolver/win.py
--rw-rw-rw-   0        0        0    29702 2023-05-23 12:13:30.000000 mcsolver-3.0.2/mcsolver/xyLib.c
--rw-rw-rw-   0        0        0    68339 2023-05-23 14:53:57.000000 mcsolver-3.0.2/mcsolver/xylib.so
-drwxrwxrwx   0        0        0        0 2023-05-23 16:30:41.339516 mcsolver-3.0.2/mcsolver.egg-info/
--rw-rw-rw-   0        0        0     8308 2023-05-23 16:30:41.000000 mcsolver-3.0.2/mcsolver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2023-05-23 16:30:41.000000 mcsolver-3.0.2/mcsolver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 16:30:41.000000 mcsolver-3.0.2/mcsolver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-23 16:30:41.000000 mcsolver-3.0.2/mcsolver.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 16:30:41.000000 mcsolver-3.0.2/mcsolver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-23 16:30:41.344514 mcsolver-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1965 2023-05-23 16:28:57.000000 mcsolver-3.0.2/setup.py
--rw-rw-rw-   0        0        0      972 2023-05-23 16:28:45.000000 mcsolver-3.0.2/setup2.py
-drwxrwxrwx   0        0        0        0 2023-05-23 16:30:41.341513 mcsolver-3.0.2/test/
--rw-rw-rw-   0        0        0      659 2019-12-09 13:48:42.000000 mcsolver-3.0.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:47:55.032680 mcsolver-3.0.4/
+-rw-rw-rw-   0        0        0    35823 2019-12-13 12:05:28.000000 mcsolver-3.0.4/LICENSE
+-rw-rw-rw-   0        0        0       72 2021-05-31 04:17:53.000000 mcsolver-3.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     8459 2023-06-24 17:47:55.031682 mcsolver-3.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6979 2023-05-24 09:15:09.000000 mcsolver-3.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 17:47:55.003681 mcsolver-3.0.4/mcsolver/
+-rw-rw-rw-   0        0        0    14449 2023-05-23 15:54:54.000000 mcsolver-3.0.4/mcsolver/Lattice.py
+-rw-rw-rw-   0        0        0    18263 2023-05-26 06:04:35.000000 mcsolver-3.0.4/mcsolver/WannierKit.py
+-rw-rw-rw-   0        0        0      536 2023-05-23 16:29:59.000000 mcsolver-3.0.4/mcsolver/__init__.py
+-rw-rw-rw-   0        0        0     8390 2023-05-22 11:26:05.000000 mcsolver-3.0.4/mcsolver/auxiliary.py
+-rw-rw-rw-   0        0        0    13828 2023-05-23 14:42:07.000000 mcsolver-3.0.4/mcsolver/fileio.py
+-rw-rw-rw-   0        0        0    18944 2023-05-26 06:02:12.000000 mcsolver-3.0.4/mcsolver/guiMain.py
+-rw-rw-rw-   0        0        0    14059 2023-06-05 04:40:28.000000 mcsolver-3.0.4/mcsolver/guiPyQt5.py
+-rw-rw-rw-   0        0        0     4020 2023-06-05 04:16:17.000000 mcsolver-3.0.4/mcsolver/guiPyQt5_toolbox.py
+-rw-rw-rw-   0        0        0    39878 2023-06-24 15:15:05.000000 mcsolver-3.0.4/mcsolver/heisenbergLib.c
+-rw-rw-rw-   0        0        0     1185 2023-06-24 17:02:47.000000 mcsolver-3.0.4/mcsolver/input.py
+-rw-rw-rw-   0        0        0    11504 2021-01-21 13:51:41.000000 mcsolver-3.0.4/mcsolver/interface2swt.py
+-rw-rw-rw-   0        0        0    25649 2023-06-24 17:10:24.000000 mcsolver-3.0.4/mcsolver/isingLib.c
+-rw-rw-rw-   0        0        0    36491 2023-06-24 17:13:23.000000 mcsolver-3.0.4/mcsolver/mcMain.py
+-rw-rw-rw-   0        0        0     3540 2019-12-14 04:31:12.000000 mcsolver-3.0.4/mcsolver/toolbox.py
+-rw-rw-rw-   0        0        0     8720 2023-06-24 16:02:37.000000 mcsolver-3.0.4/mcsolver/win.py
+-rw-rw-rw-   0        0        0    35728 2023-06-24 13:34:21.000000 mcsolver-3.0.4/mcsolver/xyLib.c
+drwxrwxrwx   0        0        0        0 2023-06-24 17:47:55.027682 mcsolver-3.0.4/mcsolver.egg-info/
+-rw-rw-rw-   0        0        0     8459 2023-06-24 17:47:54.000000 mcsolver-3.0.4/mcsolver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-06-24 17:47:54.000000 mcsolver-3.0.4/mcsolver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 17:47:54.000000 mcsolver-3.0.4/mcsolver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-24 17:47:54.000000 mcsolver-3.0.4/mcsolver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 17:47:54.000000 mcsolver-3.0.4/mcsolver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 17:47:55.033686 mcsolver-3.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1384 2023-06-24 17:42:44.000000 mcsolver-3.0.4/setup.py
+-rw-rw-rw-   0        0        0      974 2023-06-24 17:45:50.000000 mcsolver-3.0.4/setup2.py
+drwxrwxrwx   0        0        0        0 2023-06-24 17:47:55.029688 mcsolver-3.0.4/test/
+-rw-rw-rw-   0        0        0      283 2023-05-25 14:57:33.000000 mcsolver-3.0.4/test/test.py
```

### Comparing `mcsolver-3.0.2/LICENSE` & `mcsolver-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.2/PKG-INFO` & `mcsolver-3.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 1.2
 Name: mcsolver
-Version: 3.0.2
+Version: 3.0.4
 Summary: A user friendly program to do Monte Carlo sims for magnetic systems
 Home-page: https://github.com/golddoushi/mcsolver
 Author: Liang Liu
 Author-email: liangliu@main.sdu.edu.cn
 License: UNKNOWN
 Description: # mcsolver
         A user friendly and efficient tool implementing Monte Carlo simulations to estimate Curie/Neel temperature
         
         Support multiple ocassions, e.g. standard ferromangetic/anti-ferromagnetic systems, DMI, Kiteav non-diagonal exchange interactions, dipole-dipole long-range couplings, with external fields.
         
+        The newest version is 3, which supports the calculations on topological charges (the number of (anti-)Skyrmions and (anti-)Merons).
+        
         Original version contributor: Dr. Liang Liu* 1.Shenzheng University 2.Shandong University
         Email: liangliu@mail.sdu.edu.cn
         
         You can download the packed .exe (only tested in Windows 10 platform) from the following link. Wish it can find something helpful for you. And if it was used for publication, please cite:
         [1] Magnetic switches via electric field in BN nanoribbons. Applied Surface Science 480(2019)
         
         Link for exe: https://pan.baidu.com/s/1EaDqOOdB7AP9WXrwEIEaxQ
```

### Comparing `mcsolver-3.0.2/README.md` & `mcsolver-3.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # mcsolver
 A user friendly and efficient tool implementing Monte Carlo simulations to estimate Curie/Neel temperature
 
 Support multiple ocassions, e.g. standard ferromangetic/anti-ferromagnetic systems, DMI, Kiteav non-diagonal exchange interactions, dipole-dipole long-range couplings, with external fields.
 
+The newest version is 3, which supports the calculations on topological charges (the number of (anti-)Skyrmions and (anti-)Merons).
+
 Original version contributor: Dr. Liang Liu* 1.Shenzheng University 2.Shandong University
 Email: liangliu@mail.sdu.edu.cn
 
 You can download the packed .exe (only tested in Windows 10 platform) from the following link. Wish it can find something helpful for you. And if it was used for publication, please cite:
 [1] Magnetic switches via electric field in BN nanoribbons. Applied Surface Science 480(2019)
 
 Link for exe: https://pan.baidu.com/s/1EaDqOOdB7AP9WXrwEIEaxQ
```

### Comparing `mcsolver-3.0.2/mcsolver/Lattice.py` & `mcsolver-3.0.4/mcsolver/Lattice.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.2/mcsolver/WannierKit.py` & `mcsolver-3.0.4/mcsolver/WannierKit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 '''
 Created on 2018 12 8 
 
 @author: Andrew
 '''
 import numpy as np
-import re
+from time import time
 from matplotlib.figure import Figure
-from mpl_toolkits.mplot3d.axes3d import Axes3D
 import matplotlib.pyplot as plt
 try:
     from . import auxiliary as aux
 except:
     import auxiliary as aux
 
 class TBmodel(object):
     Ham=[]
     Ham_k=[]
     lattice=[]
     reci_lattice=[]
     norbital=0
     orbital_coor=[]
+    spin_list=[]
     onsite_energy=[]
     
     nhoppings=0
     hopping=[]
     
     kpath=[]
     kmesh=[]
@@ -73,15 +73,15 @@
         
         hopping=[]
         nhoppings=0
         for iinter_cell, interior_cell in enumerate(interior_cell_list):
             for iorb0, orb0 in enumerate(self.orbital_coor):
                 # add coordinates
                 orb_sc=np.dot(orb0[0]+interior_cell,invTmatrix)
-                sc_orbital_coor.append([orb_sc,orb0[1],orb0[2]])
+                sc_orbital_coor.append([orb_sc,orb0[1],orb0[2],orb0[3]])
                 norbital+=1
                 # add hopping
                 for hopping_ele in self.hopping:
                     if(hopping_ele[0]==iorb0):
                         iorb0_sc=iinter_cell*self.norbital+iorb0
                         #hopping_orb0=[iorb0_sc]
                         iorb1, aug_vec, amplify, color, linewidth= hopping_ele[1], hopping_ele[2], hopping_ele[3], hopping_ele[4], hopping_ele[5]
@@ -178,14 +178,50 @@
         ax.set_xticks([])
         ax.set_yticks([])
         ax.set_zticks([])
         ax.grid(False)
         ax.axis('off')
         return f, ax
 
+    def viewStructure_maya(self,ax):
+        '''visualize the orbital and bonding's spatial configuration'''
+        
+        def dragLineWithTwoPoints(pt0, pt1, c=(0,0,0), linewidth=None):
+            ax.plot3d([pt0[0],pt1[0]],[pt0[1],pt1[1]],[pt0[2],pt1[2]], color=c, tube_radius=linewidth)
+         
+        # draw the boder of unit cell   
+        pt0=np.zeros(3)
+        a1,a2,a3=self.lattice[0],self.lattice[1],self.lattice[2]
+
+        ax.quiver3d(*pt0,*a1,color=(0,0,0),line_width=20,mode='2darrow')
+        ax.quiver3d(*pt0,*a2,color=(0,0,0),line_width=20,mode='2darrow')
+        ax.quiver3d(*pt0,*a3,color=(0,0,0),line_width=20,mode='2darrow')
+        time0=time()
+        for iorb, orb in enumerate(self.orbital_coor):
+            #if iorb>=50:
+            #    print('num. of orb >=50, some orbs will not be illustrated')
+            #    break
+            orb_xyz=orb[0]@self.lattice
+            ax.points3d(orb_xyz[0],orb_xyz[1],orb_xyz[2],color=orb[2],scale_factor=orb[1],mode='sphere')#,s=orb[1])
+            ax.quiver3d(*orb_xyz,*orb[3],color=(0,0,1),mode='arrow')
+            #ax.text(orb_xyz[0],orb_xyz[1],orb_xyz[2],str(iorb))
+        print("Draw orbitals and mag.moms.: %.3fs"%(time()-time0))
+        time0=time()
+        for ihopping, hopping in enumerate(self.hopping):
+            #if ihopping>=200:
+            #    print('num. of hopping >=200, some hoppings will not be illustrated')
+            #    break
+            iorb0, iorb1, Rextra, amp, color, linewidth=hopping[0], hopping[1], hopping[2], hopping[3], hopping[4], hopping[5]
+            if np.dot(Rextra,Rextra)>0:
+                continue
+            orb0_xyz=np.dot(self.orbital_coor[iorb0][0],self.lattice)
+            orb1_xyz=np.dot((self.orbital_coor[iorb1][0]+Rextra),self.lattice)
+            dragLineWithTwoPoints(orb0_xyz,orb1_xyz,c=color,linewidth=linewidth)
+        print("Draw couplings: %.3fs"%(time()-time0))
+
     def genReciLattice(self):
         # generate the 3rd lattice vector if input 2D model
         def antiSymmMatrix(a):
             return np.array([
                 [ 0   ,-a[2], a[1]],
                 [ a[2], 0   ,-a[0]],
                 [-a[1], a[0], 0   ]
```

### Comparing `mcsolver-3.0.2/mcsolver/__init__.py` & `mcsolver-3.0.4/mcsolver/__init__.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.2/mcsolver/auxiliary.py` & `mcsolver-3.0.4/mcsolver/auxiliary.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.2/mcsolver/fileio.py` & `mcsolver-3.0.4/mcsolver/fileio.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.2/mcsolver/guiMain.py` & `mcsolver-3.0.4/mcsolver/guiMain.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,15 +239,15 @@
     IDandTypeOfBondNote=toolbox.NoteFrm(id_base, init_notes=['ID:','J:','','','','','','','',''],init_data=[1,-1,-1,-1,0,0,0,0,0,0],row=True,entryWidth=3)
     IDandTypeOfBondNote.entry_list[0].config(state='disabled')
 
     detail_base=Frame(addBondFrameBase)
     detail_base.grid(row=2,column=0,sticky=(W,E))
     BondDetailNote=toolbox.NoteFrm(detail_base, init_notes=['s','t','over lat.','',''],init_data=[0,0,1,0,0],row=True,entryWidth=3)
 
-    unitLabel=Label(BondFrame,text='Note all energy units are in Kelvin (1meV=11.58875K)')
+    unitLabel=Label(BondFrame,text='Note all energy units are in Kelvin (1meV=11.604609K)')
     unitLabel.grid(row=3,column=0,sticky=(W,E))
 
     #reviewBtn=Button(addBondFrameBase,text='review',command=reviewBond)
     #reviewBtn.grid(row=1,column=1,sticky='E')
     addBtn=Button(addBondFrameBase,text='add',command=addBond)
     addBtn.grid(row=2,column=2,rowspan=1,sticky='E')
     resetBtn=Button(addBondFrameBase,text='reset',command=resetBond)
@@ -323,15 +323,15 @@
     structureFrame.grid(row=0,column=1,rowspan=2)
 
     tb=wan.TBmodel()
     a1=latticeGui[0].report()
     a2=latticeGui[1].report()
     a3=latticeGui[2].report()
     tb.lattice=np.array([a1,a2,a3])
-    tb.orbital_coor=[[np.array(ele[3]),50,'red'] for ele in OrbListBox.infoData]
+    tb.orbital_coor=[[np.array(ele[3]),50,'red',(0,0,ele[2])] for ele in OrbListBox.infoData]
     tb.norbital=len(tb.orbital_coor)
     tb.hopping=[[bond_data[2][0],bond_data[2][1],np.array(bond_data[2][2]),bond_data[1][0],'green', 2] for bond_data in BondBox.infoData]
     tb.nhoppings=len(tb.hopping)
     Lx, Ly, Lz=[4 if x>1 else 1 for x in supercellGui.report() ]
     tb.make_supercell([Lx,0,0],[0,Ly,0],[0,0,Lz])
     f, structureAxis=tb.viewStructure()
     
@@ -361,15 +361,15 @@
     z0, z1 = structureAxis.get_zlim()
 
     tb=wan.TBmodel()
     a1=latticeGui[0].report()
     a2=latticeGui[1].report()
     a3=latticeGui[2].report()
     tb.lattice=np.array([a1,a2,a3])
-    tb.orbital_coor=[[np.array(ele[3]),100 if ele[0]==lightOrb else 50,'yellow' if ele[0]==lightOrb else 'red' ] for ele in OrbListBox.infoData]
+    tb.orbital_coor=[[np.array(ele[3]),100 if ele[0]==lightOrb else 50,'yellow' if ele[0]==lightOrb else 'red',(0,0,ele[2]) ] for ele in OrbListBox.infoData]
     tb.norbital=len(tb.orbital_coor)
     tb.hopping=[[bond_data[2][0],bond_data[2][1],np.array(bond_data[2][2]),bond_data[1][0],'yellow' if bond_data[0]==lightID else 'green', 6 if bond_data[0]==lightID else 2] for bond_data in BondBox.infoData]
     tb.nhoppings=len(tb.hopping)
     Lx, Ly, Lz=[4 if x>1 else 1 for x in supercellGui.report() ]
     tb.make_supercell([Lx,0,0],[0,Ly,0],[0,0,Lz])
     f, structureAxis=tb.viewStructure()
     structureAxis.view_init(elev=elev,azim=azim)
```

### Comparing `mcsolver-3.0.2/mcsolver/heisenbergLib.c` & `mcsolver-3.0.4/mcsolver/xyLib.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,208 +1,161 @@
+#define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #include <stdio.h>
 #include <stdlib.h>
 #include <math.h>
-#define PI 3.1415926535
+
 typedef struct Vec
 {
     int dimension;
-    double len;
-    double x,y,z;
+    double x,y;
 }Vec;
-typedef struct Vec9
+typedef struct Vec4
 {
     int dimension;
-    double xx,yy,zz,xy,xz,yz,yx,zx,zy;
-}Vec9;
+    double xx,yy,xy,yx;
+}Vec4;
 // vec1=abs(vec1)
 void normalize(Vec *vec1){
-    double len=sqrt(vec1->x*vec1->x+vec1->y*vec1->y+vec1->z*vec1->z);
+    double len=sqrt(vec1->x*vec1->x+vec1->y*vec1->y);
     if (len<1e-5) return;
     vec1->x/=len;
     vec1->y/=len;
-    vec1->z/=len;
 }
 // vec1=vec2
 void equal(Vec *vec1, Vec vec2){
     vec1->x=vec2.x;
     vec1->y=vec2.y;
-    vec1->z=vec2.z;
+}
+// vec1*=c
+void cTimes(Vec *vec1, double c){
+    vec1->x*=c;
+    vec1->y*=c;
 }
 // vec1=fabs(vec1)
 void vabs(Vec *vec1){
     vec1->x=fabs(vec1->x);
     vec1->y=fabs(vec1->y);
-    vec1->z=fabs(vec1->z);
 }
 // vec1/=c
 void cDivides(Vec *vec1, double c){
     vec1->x/=c;
     vec1->y/=c;
-    vec1->z/=c;
-}
-// vec1*=c
-void cTimes(Vec *vec1, double c){
-    vec1->x*=c;
-    vec1->y*=c;
-    vec1->z*=c;
 }
 // vec1+=vec2
 void plusEqual(Vec *vec1, Vec vec2){
     vec1->x+=vec2.x;
     vec1->y+=vec2.y;
-    vec1->z+=vec2.z;
 }
 // vec1-=vec2
 void minusEqual(Vec *vec1, Vec vec2){
     vec1->x-=vec2.x;
     vec1->y-=vec2.y;
-    vec1->z-=vec2.z;
 }
 // vec1 dot vec2
 double dot(Vec vec1, Vec vec2){
-    return vec1.x*vec2.x+vec1.y*vec2.y+vec1.z*vec2.z;
+    return vec1.x*vec2.x+vec1.y*vec2.y;
+}
+
+double diagonalDot(Vec vec1, Vec vec2, Vec4 matrix){
+    return vec1.x*vec2.x*matrix.xx+
+           vec1.y*vec2.y*matrix.yy+
+           vec1.x*vec2.y*matrix.xy+
+           vec1.y*vec2.x*matrix.yx;
 }
-// vec1 cross vec2
-Vec* cross(Vec vec1, Vec vec2){
-    Vec *vec3=(Vec*)malloc(sizeof(Vec));
-    vec3->x=vec1.y*vec2.z - vec1.z*vec2.y;
-    vec3->y=vec1.z*vec2.x - vec1.x*vec2.z;
-    vec3->z=vec1.x*vec2.y - vec1.y*vec2.x;
-    return vec3;
-}
-
-double (*p_diagonalDot)(Vec vec1, Vec vec2, Vec9 J);
-
-double diagonalDot(Vec vec1, Vec vec2, Vec9 J){
-    return vec1.x*vec2.x*J.xx+
-           vec1.y*vec2.y*J.yy+
-           vec1.z*vec2.z*J.zz+
-           vec1.x*vec2.y*J.xy+
-           vec1.x*vec2.z*J.xz+
-           vec1.y*vec2.z*J.yz+
-           vec1.y*vec2.x*J.yx+
-           vec1.z*vec2.x*J.zx+
-           vec1.z*vec2.y*J.zy;
-}
-
-double diagonalDot_simple(Vec vec1, Vec vec2, Vec9 J){
-    return vec1.x*vec2.x*J.xx+
-           vec1.y*vec2.y*J.yy+
-           vec1.z*vec2.z*J.zz;
+double diagonalDot_simple(Vec vec1, Vec vec2, Vec4 matrix){
+    return vec1.x*vec2.x*matrix.xx+
+           vec1.y*vec2.y*matrix.yy;
 }
+double (*p_diagonalDot)(Vec vec1, Vec vec2, Vec4 matrix);
+
+double gaussian_distr[RAND_MAX];
 
 Vec *generateRandomVec(void){
     double x=rand()/(double) RAND_MAX-0.5;
     double y=rand()/(double) RAND_MAX-0.5;
-    double z=rand()/(double) RAND_MAX-0.5;
-    double len2=(x*x+y*y+z*z);
+    double len2=(x*x+y*y);
     if (len2>0.25)
     {
         return generateRandomVec();
     }else
     {
         double len=sqrt(len2);
         Vec *direction=(Vec*)malloc(sizeof(Vec));
         direction->x=x/len;
         direction->y=y/len;
-        direction->z=z/len;
         return direction;
     }
 }
 
-double calcSignedArea(Vec s1, Vec s2, Vec s3){
-    double s1s2=dot(s1,s2)/s1.len/s2.len;
-    double s2s3=dot(s2,s3)/s2.len/s3.len;
-    double s3s1=dot(s3,s1)/s3.len/s1.len;
-    Vec* s2xs3=cross(s2,s3);
-    double realPart = 1+s1s2+s2s3+s3s1;
-    double imagPart = dot(s1, *s2xs3)/s1.len/s2.len/s3.len;
-    free(s2xs3);
-    if(fabs(realPart)<1e-6){
-        if(imagPart>0)return PI;
-        return -PI;
-    }
-    return 2*atan(imagPart/realPart);
-}
-
 typedef struct Orb
 {
     int id;
-    double S; 
+    double S; // maximum spin number
     Vec spin;
     Vec transSpin;
     Vec perpenSpin;
     int nlink;
-    Vec9 *linkStrength;
+    Vec4 *linkStrength;
     int inBlock;
     struct Orb **linkedOrb;
     struct Orb **linkedOrb_rnorm;
     Vec onsiteAnisotropy;
 
     double d_onsiteEnergy;
     double sDotN;
     int isProjected;
     int chosen;
     int nOrbInCluster;
     struct Orb **orb_cluster;
-    
+
     double h;
+    
 }Orb;
 
 //establishLattice(lattice, totOrbs, initSpin, maxNLinking, nlink, linkStrength);
-void establishLattice(Orb *lattice, int totOrbs, double initSpin[totOrbs], double initD[totOrbs][3], double h, double flunc, int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking][9],
+void establishLattice(Orb *lattice, int totOrbs, double initSpin[totOrbs], double initD[totOrbs][3], double flunc, int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking][9], double h,
                       int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm][nOrbInCluster]){
     //printf("establishing whole lattice with %d orbs and %d linkings for each orb\n",totOrbs,maxNLinking);
-    for(int i=0;i<totOrbs;i++){
+    int i;
+    for(i=0;i<totOrbs;i++){
         //printf("check point-1, entering setting %d",i);
         lattice[i].id=i;
         lattice[i].S=initSpin[i];
-        //lattice[i].spin.coor=(double*)malloc(3*sizeof(double));  // allocate spin vector for each orb
         lattice[i].spin.x=initSpin[i];
         lattice[i].spin.y=0;
-        lattice[i].spin.z=0;
-        lattice[i].spin.len=fabs(initSpin[i]);
 
         Vec *fluncSpin=generateRandomVec();
         cTimes(fluncSpin, flunc);
         plusEqual(&lattice[i].spin,*fluncSpin);
         normalize(&lattice[i].spin);
         cTimes(&lattice[i].spin,fabs(initSpin[i]));
         free(fluncSpin);
-        //printf("%.3f %.3f \n",lattice[i].spin.x, fabs(initSpin[i]));
+
         lattice[i].onsiteAnisotropy.x=initD[i][0];
         lattice[i].onsiteAnisotropy.y=initD[i][1];
-        lattice[i].onsiteAnisotropy.z=initD[i][2];
 
         lattice[i].h=h;
         //printf("orb %d spin: %.3f %.3f %.3f\n",i,lattice[i].spin.coor[0],lattice[i].spin.coor[1],lattice[i].spin.coor[2]);
         lattice[i].transSpin.x=0;  // allocate trans spin vector for each orb
         lattice[i].transSpin.y=0;
-        lattice[i].transSpin.z=0;
         lattice[i].perpenSpin.x=0;
         lattice[i].perpenSpin.y=0;
-        lattice[i].perpenSpin.z=0;
         lattice[i].nlink=nlink[i];
         //printf("check point 1, orb: %d\n",lattice[i].id);
-        lattice[i].linkStrength=(Vec9*)malloc(nlink[i]*sizeof(Vec9)); // allocate strength for each linking
+        lattice[i].linkStrength=(Vec4*)malloc(lattice[i].nlink*sizeof(Vec4)); // allocate strength for each linking
         //printf("check point 2, total links:%d\n",nlink[i]);
         for(int j=0;j<nlink[i];j++){
             //lattice[i].linkStrength[j].coor=(double*)malloc(3*sizeof(double));
             //printf("check point 3\n");
             lattice[i].linkStrength[j].xx=linkStrength[i][j][0];
             lattice[i].linkStrength[j].yy=linkStrength[i][j][1];
-            lattice[i].linkStrength[j].zz=linkStrength[i][j][2];
             lattice[i].linkStrength[j].xy=linkStrength[i][j][3];
-            lattice[i].linkStrength[j].xz=linkStrength[i][j][4];
-            lattice[i].linkStrength[j].yz=linkStrength[i][j][5];
             lattice[i].linkStrength[j].yx=linkStrength[i][j][6];
-            lattice[i].linkStrength[j].zx=linkStrength[i][j][7];
-            lattice[i].linkStrength[j].zy=linkStrength[i][j][8];
-            //printf("check point 4, link:%d, strength: %.3f %.3f %.3f\n",j,lattice[i].linkStrength[j].coor[0],lattice[i].linkStrength[j].coor[1],lattice[i].linkStrength[j].coor[2]);
+            //printf("check point 4, link:%d, strength: %.3f %.3f\n",j,lattice[i].linkStrength[j].x,lattice[i].linkStrength[j].y);
         }
         lattice[i].chosen=0;
     }
     //printf("now checking the orb cluster\n");
     for(int i=0;i<totOrb_rnorm;i++){
         int id=rOrb[i];
         lattice[id].chosen=1;
@@ -216,98 +169,92 @@
     }
     //printf("orbitals successfully built\n");
 }
 
 void establishLinking(Orb *lattice, int totOrbs, int maxNLinking, int nlink[totOrbs], int linkedOrb[totOrbs][maxNLinking],
                       int totOrb_rnorm, int rOrb[totOrb_rnorm], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking]){
     for(int iorb=0;iorb<totOrbs;iorb++){
-        lattice[iorb].linkedOrb=(Orb**)malloc(nlink[iorb]*sizeof(Orb*));
+        lattice[iorb].linkedOrb=(Orb**)malloc(lattice[iorb].nlink*sizeof(Orb*));
         for(int ilink=0;ilink<nlink[iorb];ilink++){
             lattice[iorb].linkedOrb[ilink]=lattice+linkedOrb[iorb][ilink];
         }
     }
     for(int i=0;i<totOrb_rnorm;i++){
         int iorb=rOrb[i];
         lattice[iorb].linkedOrb_rnorm=(Orb**)malloc(nlink[iorb]*sizeof(Orb*));
         for(int ilink=0;ilink<nlink[iorb];ilink++){
             lattice[iorb].linkedOrb_rnorm[ilink]=lattice+linkedOrb_rnorm[i][ilink];
         }
     }
+    //printf("bonds successfully built\n");
 }
 
 double getCorrEnergy(Orb *source){
-    //printf("start calc corr. energy\n");
     double corr=0;
     for(int i=0;i<source->nlink;i++){
+        //printf("getCorrEnergy\n");
         corr+=(*p_diagonalDot)(source->spin,source->linkedOrb[i]->spin,source->linkStrength[i]);
-        //printf("J=%.3f S1=%.3f S2=%.3f\n",source->linkStrength[i],source->spin,source->linkedOrb[i]->spin);
-        //printf("corr=%.3f\n",corr);
     }
     return corr;
 }
 
-double getOnsiteEnergy(Orb *source){  // onsite term
+double getOnsiteEnergy(Orb *source){
     return source->onsiteAnisotropy.x*source->spin.x*source->spin.x+
-           source->onsiteAnisotropy.y*source->spin.y*source->spin.y+
-           source->onsiteAnisotropy.z*source->spin.z*source->spin.z-source->h*source->spin.z;
+           source->onsiteAnisotropy.y*source->spin.y*source->spin.y-
+           source->h*source->spin.x;
 }
 
-Vec getMajoritySpin(Orb*_orb){ // core algorithm for renormalization
+Vec getMajoritySpin(Orb*_orb){  // core algorithm for renormalization
     //return _orb->spin; // decimation algorithm
     Vec avgSpin;
     avgSpin.x=0;
     avgSpin.y=0;
-    avgSpin.z=0;
     for(int iorb=0;iorb<_orb->nOrbInCluster;iorb++){
         plusEqual(&avgSpin,_orb->orb_cluster[iorb]->spin);
     }
+    //cDivides(&avgSpin,_orb->nOrbInCluster);
     normalize(&avgSpin);
     cTimes(&avgSpin, _orb->S);
     return avgSpin; // majority algorithm
 }
 
-double getCorrEnergy_rnorm(Orb *source, double (*p_diagonalFunc)()){
+double getCorrEnergy_rnorm(Orb *source){
     double corr=0;
     Vec avgSpin_source=getMajoritySpin(source);
     for(int i=0;i<source->nlink;i++){
         //printf("link to orb%d\n",source->linkedOrb_rnorm[i]->id);
         Vec avgSpin_target=getMajoritySpin(source->linkedOrb_rnorm[i]);
-        corr+=(*p_diagonalFunc)(avgSpin_source,avgSpin_target,source->linkStrength[i]);
+        corr+=(*p_diagonalDot)(avgSpin_source,avgSpin_target,source->linkStrength[i]);
     }
     //printf("Ecorr=%.3f\n",corr);
     return corr;
 }
 
 double getOnsiteEnergy_rnorm(Orb *source){
     Vec avgSpin_source=getMajoritySpin(source);
     return source->onsiteAnisotropy.x*avgSpin_source.x*avgSpin_source.x+
-           source->onsiteAnisotropy.y*avgSpin_source.y*avgSpin_source.y+
-           source->onsiteAnisotropy.z*avgSpin_source.z*avgSpin_source.z-source->h*avgSpin_source.z;
+           source->onsiteAnisotropy.y*avgSpin_source.y*avgSpin_source.y-
+           source->h*avgSpin_source.x;
 }
 
-double getDeltaCorrEnergy(Orb *source){//, double (*p_diagonalFunc)()){
+double getDeltaCorrEnergy(Orb *source){
     double corr=0;
-    //printf("centre orb%d, trial trans %.3f %.3f %.3f, len %.3f\n",source->id,source->transSpin.x,source->transSpin.y,source->transSpin.z,sqrt(dot(source->transSpin,source->transSpin)));
     for(int i=0;i<source->nlink;i++){
-        //printf("corr to orb%d, J %.3f %.3f %.3f S %.3f %.3f %.3f, \n",source->linkedOrb[i]->id,source->linkStrength[i].x,source->linkStrength[i].y,source->linkStrength[i].z,source->linkedOrb[i]->spin.x,source->linkedOrb[i]->spin.y,source->linkedOrb[i]->spin.z);
+        //printf("getDeltaCorrEnergy\n");
         corr+=(*p_diagonalDot)(source->transSpin,source->linkedOrb[i]->spin,source->linkStrength[i]);
     }
-    //printf("total corr %.6f\n",corr);
     return corr;
 }
 
 double getDeltaOnsiteEnergy(Orb *source){
     double s1x=source->spin.x+source->transSpin.x;
     double s1y=source->spin.y+source->transSpin.y;
-    double s1z=source->spin.z+source->transSpin.z;
-    //printf("h %.3f, transSpin %.3f\n",source->h,source->transSpin.z);
     return source->onsiteAnisotropy.x*(s1x*s1x-source->spin.x*source->spin.x)+
-           source->onsiteAnisotropy.y*(s1y*s1y-source->spin.y*source->spin.y)+
-           source->onsiteAnisotropy.z*(s1z*s1z-source->spin.z*source->spin.z)-
-           source->h*source->transSpin.z;
+           source->onsiteAnisotropy.y*(s1y*s1y-source->spin.y*source->spin.y)-
+           source->h*source->transSpin.x;
 }
 
 int expandBlock(int*beginIndex, int*endIndex, Orb *buffer[], int*blockLen, Orb *block[], Vec refDirection){
     //printf("  Buffer: now start and end pt is %d, %d.\n",*beginIndex, *endIndex);
     if(*beginIndex>*endIndex) return 0;
 
     // FIFO
@@ -315,30 +262,29 @@
     *beginIndex+=1; // pop out the first element
     
     //FILO
     //Orb *outOrb=buffer[*endIndex];
     //*endIndex-=1; // pop out the last element
 
     if(outOrb->isProjected==0){
-        // calc. perpendicular and transverse parts (to refDirection)
         outOrb->sDotN=-dot(outOrb->spin,refDirection);
         equal(&outOrb->transSpin, refDirection);
         cTimes(&outOrb->transSpin, outOrb->sDotN);
         equal(&outOrb->perpenSpin,outOrb->spin);
         plusEqual(&outOrb->perpenSpin,outOrb->transSpin);
         outOrb->isProjected=1;
     }
     //printf("center orb: %d\n", outOrb->id);
     //printf("projection along axis: %.3f\n", -s1n/2);
-    //printf("variation of spin: %.3f %.3f %.3f\n",outOrb->transSpin.coor[0],outOrb->transSpin.coor[1],outOrb->transSpin.coor[2]);
+    //printf("variation of spin: %.3f %.3f\n",outOrb->transSpin.x,outOrb->transSpin.y);
     //printf("it has %d neighbor orbs\n",outOrb->nlink);
     int i;
     for(i=0;i<outOrb->nlink;i++){
         //double effectiveJ=diagonalDot(outOrb->linkStrength[i], refDirection, refDirection);
-        //printf("the %d linking has strength %.3f %.3f %.3f (original) %.3f (effective)\n",i,outOrb->linkStrength[i].coor[0],outOrb->linkStrength[i].coor[1],outOrb->linkStrength[i].coor[2],effectiveJ);
+        //printf("the %d linking has strength %.3f %.3f (original) %.3f (effective)\n",i,outOrb->linkStrength[i].x,outOrb->linkStrength[i].y,effectiveJ);
         Orb *linkedOrb=outOrb->linkedOrb[i];
         //printf("consider to add orb %d\n",linkedOrb->id);
         //printf("      considering the %d orb which is linking to %d orb, it is %d in block \n", linkedOrb->id, outOrb->id, linkedOrb->inBlock);
         if(linkedOrb->inBlock==0){
             //printf("projection along axis: %.3f\n", s2n);
             //double corr=-s1n*diagonalDot(refDirection,outOrb->linkStrength[i],linkedOrb->spin); // bond strength
             //printf("      spin of orb %d is %.3f %.3f %.3f and bond strength is %.3f\n",linkedOrb->id,linkedOrb->spin.coor[0],linkedOrb->spin.coor[1],linkedOrb->spin.coor[2],corr);
@@ -347,14 +293,15 @@
                 linkedOrb->sDotN=-dot(linkedOrb->spin,refDirection);
                 equal(&linkedOrb->transSpin, refDirection);
                 cTimes(&linkedOrb->transSpin, linkedOrb->sDotN);
                 equal(&linkedOrb->perpenSpin, linkedOrb->spin);
                 plusEqual(&linkedOrb->perpenSpin, linkedOrb->transSpin);
                 linkedOrb->isProjected=1;
             }
+            //printf("229\n");
             double corr=2*outOrb->sDotN*linkedOrb->sDotN*(*p_diagonalDot)(refDirection,refDirection,outOrb->linkStrength[i]);
             
             //linkedOrb->d_onsiteEnergy=getDeltaOnsiteEnergy(linkedOrb);
             if(corr<0 && (1-exp(corr))>rand()/(double) RAND_MAX){
                 //printf("          -->>fortunately it is added to block with possibility %f\n",(1-exp(2*corr)));
                 // update block
                 *blockLen+=1;
@@ -384,17 +331,17 @@
 
     Vec *refDirection=generateRandomVec();
     //refDirection.coor=(double*)malloc(3*sizeof(double));
     //equal(&refDirection, &block[0]->spin);
     //normalize(&refDirection);
     //printf("-------------------\n");
     //printf("the seed Orb is %d\n",block[0]->id);
-    //printf("trial normal direction %.3f %.3f %.3f\n",refDirection.coor[0],refDirection.coor[1],refDirection.coor[2]);
-    //double effectiveJ=diagonalDot(block[0]->linkStrength[0], refDirection, refDirection);
-    //printf("the 0 linking has strength %.3f %.3f %.3f (original) %.3f (effective)\n",block[0]->linkStrength[0].coor[0],block[0]->linkStrength[1].coor[1],block[0]->linkStrength[2].coor[2],effectiveJ);
+    //printf("trial normal direction %.3f %.3f\n",refDirection->x,refDirection->y);
+    //double effectiveJ=diagonalDot(block[0]->linkStrength[0], *refDirection, *refDirection);
+    //printf("the 0 linking has strength %.3f %.3f (original) %.3f (effective)\n",block[0]->linkStrength[0].x,block[0]->linkStrength[1].y,effectiveJ);
     while (expandBlock(p_beginIndex, p_endIndex, buffer, p_blockLen, block, *refDirection)==1)
     {
         // no code here
     }
     
     //printf("    Block size is %d\n",*p_blockLen);
     double tot_d_onsiteEnergy=0;
@@ -410,17 +357,14 @@
                 tot_d_onsiteEnergy+=source_anisotropy;
             }
         }
     }
     // single-ion anisotropy
     for(i=0;i<*p_blockLen;i++) tot_d_onsiteEnergy+=getDeltaOnsiteEnergy(block[i]);
     // process the onsite anisotropy
-    //printf("tot_d_onsiteEnergy=%.6f\n",tot_d_onsiteEnergy);
-    //tot_d_onsiteEnergy=0;
-    //if(fabs(tot_d_onsiteEnergy)>1e-5) printf("Anisotropy energy=%.3f\n",tot_d_onsiteEnergy);
     if(tot_d_onsiteEnergy<=0 || exp(-tot_d_onsiteEnergy)>rand()/(double) RAND_MAX){
         for(i=0;i<*p_blockLen;i++){
             cTimes(&block[i]->transSpin,2);
             plusEqual(&block[i]->spin, block[i]->transSpin);
             //printf("    after update orb %d spin converted to %.3f %.3f %.3f\n",block[i]->id,block[i]->spin.coor[0],block[i]->spin.coor[1],block[i]->spin.coor[2]);
             //block[i]->inBlock=0;
             plusEqual(p_totSpin,block[i]->transSpin);
@@ -433,100 +377,202 @@
     }
     // clean
     free(refDirection);
 }
 
 void localUpdate(int totOrbs, Orb lattice[], double *p_energy, Vec *p_totSpin){
     //printf("start local updating\n");
-    int seedID=rand()%totOrbs;  // chose one orb
-    //printf("considering %d orb, its spin is %.3f %.3f %.3f\n",
-    //         seedID,lattice[seedID].spin.coor[0],lattice[seedID].spin.coor[1],lattice[seedID].spin.coor[2]);
+    int seedID=rand()%totOrbs;  // chose one orb Note that WE CANNOT CHOOSE GHOST SPIN, since it's not compatible with local statistics
+    //int seedID=totOrbs;
+    //printf("considering %d orb, its spin is %.3f %.3f\n",
+    //         seedID,lattice[seedID].spin.x,lattice[seedID].spin.y);
     Vec *refDirection=generateRandomVec(); // chose new direction
-    //printf("try new spin direction, ref: %.3f %.3f %.3f\n",
-    //       refDirection.coor[0],refDirection.coor[1],refDirection.coor[2]);
+    //printf("try new spin direction, ref: %.3f %.3f\n",
+    //       refDirection->x,refDirection->y);
     double s1n=-2*dot(lattice[seedID].spin,*refDirection);
     //printf("projection s1n: %.3f\n",s1n);
     equal(&lattice[seedID].transSpin,*refDirection);
     cTimes(&lattice[seedID].transSpin,s1n);
-    double corr=getDeltaCorrEnergy(lattice+seedID);//,p_diagonalFunc);
+    double corr=getDeltaCorrEnergy(lattice+seedID);
     corr+=getDeltaOnsiteEnergy(lattice+seedID);
     
-    //printf("lead to the translation spin vector: %.3f %.3f %.3f and delta Ecorr: %.3f\n",
-    //      lattice[seedID].transSpin.x,lattice[seedID].transSpin.y,lattice[seedID].transSpin.z,corr);
+    //printf("lead to the translation spin vector: %.3f %.3f and delta Ecorr: %.3f, transition possibility %.3f P\n",
+    //      lattice[seedID].transSpin.x,lattice[seedID].transSpin.y,corr,100*exp(-corr));
     
     if(corr<=0 || exp(-corr)>rand()/(double) RAND_MAX){  // new direction is energertically favoured thus accept directly
         plusEqual(p_totSpin,lattice[seedID].transSpin);
         plusEqual(&lattice[seedID].spin,lattice[seedID].transSpin);
         *p_energy+=corr;
-        //printf("since new direction is energertically lowerd thus we accept, energy: %.3f\n",*p_energy);
-        //double energy_tmp=0;
-        //for(int i=0;i<totOrbs;i++) energy_tmp+=getCorrEnergy(lattice+i);
-        //energy_tmp/=2;
-        //printf("ref energy (with out onsite) %.3f\n",energy_tmp);
+        //printf("Luckily we accept the transition, energy: %.3f\n",*p_energy);
     }
     free(refDirection);
     return;
 }
 
-// interface to block update and local update algorithm
-void (*p_mcUpdate)(int totOrbs, Orb lattice[], double *p_energy, Vec *p_totSpin);
+void (*p_mcUpdate)(int totOrbs, Orb lattice[], double*p_energy, Vec *p_totSpin);
+
+//PyObject * MCMainFunction(int algorithm, int totOrbs, double initSpin[totOrbs], double initD[totOrbs][3], int nthermal, int nsweep, 
+//                   int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking][9], int linkedOrb[totOrbs][maxNLinking], int nLocalCircuits, int localCircuits[nLocalCircuits][3],
+//                   int ninterval, int nLat, int corrOrbPair[nLat][2], int nOrbGroup, int maxOrbGroupSize, int orbGroupList[nOrbGroup][maxOrbGroupSize], double flunc, double h,
+//                   int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm][nOrbInCluster], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking],
+//                   int spinFrame,
+//                   int ignoreNonDiagonalJ){
+PyObject * MCMainFunction(PyObject* self, PyObject* args){
+    // read in all parameters
+    PyObject* py_algorithm;
+    PyObject* py_initSpin;
+    PyObject* py_initD;
+    PyObject* py_nthermal;
+    PyObject* py_nsweep;
+    PyObject* py_maxNLinking;
+    PyObject* py_ninterval;
+    PyObject* py_nlink;
+    PyObject* py_linkStrength;
+    PyObject* py_linkedOrb;
+    PyObject* py_localCircuits;
+    PyObject* py_corrOrbPair;
+    PyObject* py_nOrbGroup;
+    PyObject* py_maxOrbGroupSize;
+    PyObject* py_orbGroupList;
+    PyObject* py_flunc; 
+    PyObject* py_h;
+    PyObject* py_rOrb;
+    PyObject* py_rOrbCluster;
+    PyObject* py_linkedOrb_rnorm;
+    PyObject* py_spinFrame;
+    PyObject* py_ignoreNonDiagonalJ;
+    PyObject* callback;  // callback function
+    PyArg_ParseTuple(args,"OOOOOOOOOOOOOOOOOOOOOOO",
+                    &py_algorithm,&py_initSpin,&py_initD,&py_nthermal,&py_nsweep,&py_ninterval,
+                    &py_maxNLinking,&py_nlink,&py_linkStrength,&py_linkedOrb,&py_localCircuits,
+                    &py_corrOrbPair,
+                    &py_nOrbGroup,&py_maxOrbGroupSize,&py_orbGroupList,
+                    &py_flunc,&py_h,
+                    &py_rOrb,&py_rOrbCluster,&py_linkedOrb_rnorm,
+                    &py_spinFrame,&py_ignoreNonDiagonalJ,
+                    &callback);
+
+    int algorithm=(int)PyLong_AsLong(py_algorithm); 
+    //printf("%d\n",algorithm);
+    int nthermal=(int)PyLong_AsLong(py_nthermal);
+    int nsweep=(int)PyLong_AsLong(py_nsweep);
+    int maxNLinking=(int)PyLong_AsLong(py_maxNLinking);
+    int ninterval=(int)PyLong_AsLong(py_ninterval);
+    int spinFrame=(int)PyLong_AsLong(py_spinFrame);
+    int ignoreNonDiagonalJ=(int)PyLong_AsLong(py_ignoreNonDiagonalJ);
+
+    int totOrbs=(int)PyTuple_Size(py_initSpin);
+    double initSpin[totOrbs];
+    for(int iorb=0;iorb<totOrbs;iorb++)initSpin[iorb]=PyFloat_AsDouble(PyTuple_GetItem(py_initSpin,iorb));
+
+    double initD[totOrbs][3];
+    for(int iorb=0;iorb<totOrbs;iorb++)for(int idir=0;idir<3;idir++)
+        initD[iorb][idir]=PyFloat_AsDouble(PyTuple_GetItem(py_initD,iorb*3+idir));
+    
+    
+    int nlink[totOrbs];
+    double linkStrength[totOrbs][maxNLinking][9];
+    int linkedOrb[totOrbs][maxNLinking];
+    for(int iorb=0;iorb<totOrbs;iorb++){
+        nlink[iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_nlink,iorb));
+        for(int ilink=0;ilink<maxNLinking;ilink++){
+            linkedOrb[iorb][ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb,iorb*maxNLinking+ilink));
+            for(int icomp=0;icomp<9;icomp++)
+            linkStrength[iorb][ilink][icomp]=PyFloat_AsDouble(PyTuple_GetItem(py_linkStrength,iorb*maxNLinking*9+ilink*9+icomp));
+        }
+    }
+    //printf("totOrbs=%d s0=%f D0x=%f nther=%d nst=%d tau=%d maxLink=%d link0=%d J0x=%f\n",totOrbs,initSpin[0],initD[0][0],nthermal,nsweep,ninterval,maxNLinking,nlink[0],linkStrength[0][0][0]);
+    //printf("spinFrame: %d only diagonal: %d\n",spinFrame,ignoreNonDiagonalJ);
+    //for(int iorb=0;iorb<nlink[0];iorb++)printf("orb0-orb%d\n",linkedOrb[0][iorb]);
+    
+    int nLocalCircuits=(int)PyTuple_Size(py_localCircuits)/3;
+    int minimalLocalCircuits=1;if(nLocalCircuits>minimalLocalCircuits)minimalLocalCircuits=nLocalCircuits;
+    int localCircuits[minimalLocalCircuits][3];
+    for(int icircuit=0;icircuit<nLocalCircuits;icircuit++)for(int icomp=0;icomp<3;icomp++)
+        localCircuits[icircuit][icomp]=(int)PyLong_AsLong(PyTuple_GetItem(py_localCircuits,icircuit*3+icomp));
+    //printf("num. of local circuit for topo: %d\n",nLocalCircuits);
+
+    int nLat=(int)PyTuple_Size(py_corrOrbPair)/2;
+    int corrOrbPair[nLat][2];
+    for(int ilat=0;ilat<nLat;ilat++){
+        for(int icomp=0;icomp<2;icomp++)
+        corrOrbPair[ilat][icomp]=(int)PyLong_AsLong(PyTuple_GetItem(py_corrOrbPair,ilat*2+icomp));
+        //printf("pair%d orb%d-orb%d\n",ilat,corrOrbPair[ilat][0],corrOrbPair[ilat][1]);
+    }
+    
+    int nOrbGroup=(int)PyLong_AsLong(py_nOrbGroup);
+    int maxOrbGroupSize=(int)PyLong_AsLong(py_maxOrbGroupSize);
+    //printf("nOrbGroup=%d maxOrbGroupSize=%d\n",nOrbGroup,maxOrbGroupSize);
+    int orbGroupList[nOrbGroup][maxOrbGroupSize];
+    for(int iorbGroup=0;iorbGroup<nOrbGroup;iorbGroup++)for(int iorb=0;iorb<maxOrbGroupSize;iorb++)
+        orbGroupList[iorbGroup][iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_orbGroupList,iorbGroup*maxOrbGroupSize+iorb));
+    
+    double flunc = PyFloat_AsDouble(py_flunc);
+    double h = PyFloat_AsDouble(py_h);
+    //printf("flunc=%f h=%f\n",flunc,h);
+
+    int totOrb_rnorm=(int)PyTuple_Size(py_rOrb);
+    int nOrbInCluster=(int)PyTuple_Size(py_rOrbCluster)/totOrb_rnorm;
+    //printf("totOrb renorm=%d grain size=%d\n",totOrb_rnorm,nOrbInCluster);
+    int rOrb[totOrb_rnorm];
+    int rOrbCluster[totOrb_rnorm][nOrbInCluster];
+    int linkedOrb_rnorm[totOrb_rnorm][maxNLinking];
+    for(int iorb=0;iorb<totOrb_rnorm;iorb++){
+        rOrb[iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrb,iorb));
+        for(int iorb_cluster=0;iorb_cluster<nOrbInCluster;iorb_cluster++)
+            rOrbCluster[iorb][iorb_cluster]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrbCluster,iorb*nOrbInCluster+iorb_cluster));
+        for(int ilink=0;ilink<maxNLinking;ilink++)
+            linkedOrb_rnorm[iorb][ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb_rnorm,iorb*maxNLinking+ilink));
+    }
 
-PyObject * MCMainFunction(int algorithm, int totOrbs, double initSpin[totOrbs], double initD[totOrbs][3], int nthermal, int nsweep, 
-                   int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking][9], int linkedOrb[totOrbs][maxNLinking],  int nLocalCircuits, int localCircuits[nLocalCircuits][3],
-                   int ninterval, int nLat, int corrOrbPair[nLat][2], int nOrbGroup, int maxOrbGroupSize, int orbGroupList[nOrbGroup][maxOrbGroupSize], double flunc, double h,
-                   int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm][nOrbInCluster], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking],
-                   int spinFrame,
-                   int ignoreNonDiagonalJ){
     // set algorithm
     p_mcUpdate=localUpdate;
-    if (algorithm==1) p_mcUpdate=blockUpdate;
+    if(algorithm==1) p_mcUpdate=blockUpdate;
 
-    // set diagonal dot version
+    // set diagonal dot function
     p_diagonalDot=diagonalDot;
     if (ignoreNonDiagonalJ>0) p_diagonalDot=diagonalDot_simple;
-    
-    // initialize lattice
+
+    // initialize lattice add one ghost spin for mimicing external field
     Orb lattice[totOrbs];
     //printf("hello here is C lib\n");
-    establishLattice(lattice, totOrbs, initSpin, initD, h, flunc, maxNLinking, nlink, linkStrength, totOrb_rnorm, nOrbInCluster, rOrb, rOrbCluster);
+    establishLattice(lattice, totOrbs, initSpin, initD, flunc, maxNLinking, nlink, linkStrength, h, totOrb_rnorm, nOrbInCluster, rOrb, rOrbCluster);
     establishLinking(lattice, totOrbs, maxNLinking, nlink, linkedOrb, totOrb_rnorm, rOrb, linkedOrb_rnorm);
 
     // initialize measurement
     double energy=0;
     double *p_energy=&energy;
     for(int i=0;i<totOrbs;i++)*p_energy+=getCorrEnergy(lattice+i);
     *p_energy/=2; // double counting
     for(int i=0;i<totOrbs;i++)*p_energy+=getOnsiteEnergy(lattice+i);
-    //printf("gournd energy=%.3f nLat=%d\n",*p_energy, nLat);
 
     Vec totSpin;
-    totSpin.x=0;totSpin.y=0;totSpin.z=0;
+    totSpin.x=0;totSpin.y=0;
     Vec*p_totSpin=&totSpin;
     for(int i=0;i<totOrbs;i++) plusEqual(p_totSpin, lattice[i].spin);
-
+    
     for(int i=0;i<nthermal*ninterval;i++) (*p_mcUpdate)(totOrbs, lattice, p_energy, p_totSpin); //thermalization
 
-    // printf("start sweeping\n");
     Vec spin_i, spin_i_r;
     Vec spin_j, spin_j_r;
-    spin_i.x=0;spin_i.y=0;spin_i.z=0;spin_i_r.x=0;spin_i_r.y=0;spin_i_r.z=0;
-    spin_j.x=0;spin_j.y=0;spin_j.z=0;spin_j_r.x=0;spin_j_r.y=0;spin_j_r.z=0;
+    spin_i.x=0;spin_i.y=0;spin_i_r.x=0;spin_i_r.y=0;
+    spin_j.x=0;spin_j.y=0;spin_j_r.x=0;spin_j_r.y=0;
     double spin_ij, spin_ij_r;
     spin_ij=0;spin_ij_r=0;
 
     double totEnergy=0, totEnergy_r=0;
     double E2=0, E2_r=0;
     double M=0,M2=0,M4=0;
     double M_tmp=0,MdotM_tmp=0,M_tot=0;
-    
+
     double topological_q=0; // total vortice number
 
     Vec spin_direction;
-    double spin_i_z, spin_j_z, spin_tot_z; // spin projected to net-spin
-    double spin_i_h, spin_j_h, spin_tot_h; // spin projected to z aixis
+    double spin_i_z, spin_j_z, spin_tot_z;
+    double spin_i_h, spin_j_h, spin_tot_h;
     spin_i_z=0;spin_j_z=0;spin_tot_z=0;
     spin_i_h=0;spin_j_h=0;spin_tot_h=0;
 
     // prepare for output spin frame
     int output_per_sweep=nsweep;
     int iFrame=0;
     PyObject *spinFrameData;
@@ -538,87 +584,81 @@
     }
 
     // prepare for orb group statistics
     double spinDotSpinBetweenGroup[(nOrbGroup+1)*(nOrbGroup+1)];
     for(int i=0;i<(nOrbGroup+1)*(nOrbGroup+1);i++) spinDotSpinBetweenGroup[i]=0.0;
     double spin4Order[nOrbGroup+1];
     for(int i=0;i<nOrbGroup+1;i++) spin4Order[i]=0.0;
-    
+
     for(int i=0;i<nsweep;i++){
         for(int j=0;j<ninterval;j++) (*p_mcUpdate)(totOrbs, lattice, p_energy, p_totSpin);
         // record the spin vector field distribution
         if((spinFrame>0) & (i%output_per_sweep==0)){
             PyObject *spinDistribution=PyTuple_New(totOrbs);
             for(int j=0;j<totOrbs;j++){
                 PyObject *spinJVec=PyTuple_New(3);
                 PyTuple_SetItem(spinJVec, 0, PyFloat_FromDouble(lattice[j].spin.x));
                 PyTuple_SetItem(spinJVec, 1, PyFloat_FromDouble(lattice[j].spin.y));
-                PyTuple_SetItem(spinJVec, 2, PyFloat_FromDouble(lattice[j].spin.z));
+                PyTuple_SetItem(spinJVec, 2, PyFloat_FromDouble(0));
                 PyTuple_SetItem(spinDistribution, j, spinJVec);
             }
             PyTuple_SetItem(spinFrameData, iFrame, spinDistribution);
             iFrame+=1;
         }
 
         // find the main axis
         spin_direction.x=p_totSpin->x;
         spin_direction.y=p_totSpin->y;
-        spin_direction.z=p_totSpin->z;
         normalize(&spin_direction);
 
         // spin statistics over space in each frame
         Vec spin_i_avg;
         Vec spin_j_avg;
         spin_i_avg.x=0;
         spin_i_avg.y=0;
-        spin_i_avg.z=0;
         spin_j_avg.x=0;
         spin_j_avg.y=0;
-        spin_j_avg.z=0;
         double spin_ij_avg=0.0;
 
         double spin_i_z_avg, spin_j_z_avg;
         double spin_i_h_avg, spin_j_h_avg;
         spin_i_z_avg=0;spin_j_z_avg=0;
         spin_i_h_avg=0;spin_j_h_avg=0;
         for(int j=0;j<nLat;j++){
             plusEqual(&spin_i_avg, lattice[corrOrbPair[j][0]].spin);
             plusEqual(&spin_j_avg, lattice[corrOrbPair[j][1]].spin);
             spin_ij_avg+=dot(lattice[corrOrbPair[j][0]].spin,lattice[corrOrbPair[j][1]].spin);
-            
+
             // spin along main axis
             spin_i_z_avg+=dot(spin_direction,lattice[corrOrbPair[j][0]].spin);
             spin_j_z_avg+=dot(spin_direction,lattice[corrOrbPair[j][1]].spin);
 
             // spin projected to z axis
-            spin_i_h_avg+=lattice[corrOrbPair[j][0]].spin.z;
-            spin_j_h_avg+=lattice[corrOrbPair[j][1]].spin.z;
+            spin_i_h_avg+=lattice[corrOrbPair[j][0]].spin.x;
+            spin_j_h_avg+=lattice[corrOrbPair[j][1]].spin.x;
+            
         }
 
-        double topological_q_local=0;
-        for(int icircuit=0;icircuit<nLocalCircuits;icircuit++){
-            topological_q_local+=calcSignedArea(lattice[localCircuits[icircuit][0]].spin, lattice[localCircuits[icircuit][1]].spin, lattice[localCircuits[icircuit][2]].spin);
-        }
-        topological_q+=topological_q_local/PI/4;
+        double topological_q_local=0; // xy-model posess no topological charge
+        topological_q+=topological_q_local;
 
         spin_i_z+=spin_i_z_avg/nLat;
         spin_j_z+=spin_j_z_avg/nLat;
         spin_tot_z+=(dot(spin_direction,*p_totSpin)/nLat);
         //if(h<0.00001){// avoid faults time reversal symmetry
         //    spin_i_h+=fabs(spin_i_h_avg)/nLat;
         //    spin_j_h+=fabs(spin_j_h_avg)/nLat;
-        //    spin_tot_h+=fabs(p_totSpin->z/nLat);
+        //    spin_tot_h+=fabs(p_totSpin->x/nLat);
         //}else{
             spin_i_h+=spin_i_h_avg/nLat;
             spin_j_h+=spin_j_h_avg/nLat;
-            spin_tot_h+=p_totSpin->z/nLat;
+            spin_tot_h+=p_totSpin->x/nLat;
         //}
 
-
-        M=sqrt(dot(*p_totSpin,*p_totSpin))/nLat;
+        M=sqrt(dot(spin_i_avg,spin_i_avg))/nLat;
         M2+=M*M;
         M4+=M*M*M*M;
         //calc auto-correlation
         M_tot+=M;
         MdotM_tmp+=M_tmp*M;
         M_tmp=M;
 
@@ -627,22 +667,23 @@
         vabs(&spin_i_avg);
         vabs(&spin_j_avg);
         plusEqual(&spin_i,spin_i_avg);
         plusEqual(&spin_j,spin_j_avg);
         spin_ij+=spin_ij_avg/nLat;
 
         double e_avg=*p_energy/totOrbs;
+        //printf("e_avg=%.5f\n",e_avg);
         totEnergy+=e_avg;
         E2+=e_avg*e_avg;
 
         // *************** statistics on renormalized lattice
         // spin statistics over space in each frame
         Vec spin_i_r_avg, spin_j_r_avg;
-        spin_i_r_avg.x=0;spin_i_r_avg.y=0;spin_i_r_avg.z=0;
-        spin_j_r_avg.x=0;spin_j_r_avg.y=0;spin_j_r_avg.z=0;
+        spin_i_r_avg.x=0;spin_i_r_avg.y=0;
+        spin_j_r_avg.x=0;spin_j_r_avg.y=0;
         int chosed_spin_i=0;
         int chosed_spin_j=0;
         int chosed_spin_ij=0;
         double spin_ij_r_avg=0.0;
         for(int j=0;j<nLat;j++){
             Orb *_orb_i=lattice+corrOrbPair[j][0];
             Orb *_orb_j=lattice+corrOrbPair[j][1];
@@ -679,98 +720,114 @@
         plusEqual(&spin_i_r,spin_i_r_avg);
         plusEqual(&spin_j_r,spin_j_r_avg);
         spin_ij_r+=spin_ij_r_avg/chosed_spin_ij;
 
         // energy statistics
         double e_avg_rnorm=0;
         for(int j=0;j<totOrbs;j++){ // calc. bond energy in renormalized system
-            if(lattice[j].chosen>0) e_avg_rnorm+=getCorrEnergy_rnorm(lattice+j, p_diagonalDot);
+            if(lattice[j].chosen>0) e_avg_rnorm+=getCorrEnergy_rnorm(lattice+j);
         }
         e_avg_rnorm/=2; // double counting
         for(int j=0;j<totOrbs;j++){ // onsite part
             if(lattice[j].chosen>0) e_avg_rnorm+=getOnsiteEnergy(lattice+j);
         }
         e_avg_rnorm/=totOrb_rnorm;
         totEnergy_r+=e_avg_rnorm;
         E2_r+=e_avg_rnorm*e_avg_rnorm;
 
         // orb group statistics
         Vec summedSpinOfGroup[nOrbGroup+1];
         int iOrbGroup, jOrbGroup;
         for(iOrbGroup=0;iOrbGroup<nOrbGroup;iOrbGroup++){
             Vec summedSpin;
-            summedSpin.x=0;summedSpin.y=0;summedSpin.z=0;
+            summedSpin.x=0;summedSpin.y=0;
             int k;
             for(k=0;k<maxOrbGroupSize;k++){
                 if(orbGroupList[iOrbGroup][k]<0) break;
                 plusEqual(&summedSpin,lattice[orbGroupList[iOrbGroup][k]].spin);
             }
             summedSpinOfGroup[iOrbGroup].x=summedSpin.x;
             summedSpinOfGroup[iOrbGroup].y=summedSpin.y;
-            summedSpinOfGroup[iOrbGroup].z=summedSpin.z;
         }
         summedSpinOfGroup[iOrbGroup].x=p_totSpin->x/nLat;
         summedSpinOfGroup[iOrbGroup].y=p_totSpin->y/nLat;
-        summedSpinOfGroup[iOrbGroup].z=p_totSpin->z/nLat;
         //printf("nOrbGroup: %d\n",nOrbGroup);
         for(iOrbGroup=0;iOrbGroup<(nOrbGroup+1);iOrbGroup++){
             for(jOrbGroup=0;jOrbGroup<(nOrbGroup+1);jOrbGroup++){
                 double spin_i_dot_spin_j=dot(summedSpinOfGroup[iOrbGroup],summedSpinOfGroup[jOrbGroup]);
                 spinDotSpinBetweenGroup[iOrbGroup*(nOrbGroup+1)+jOrbGroup]+=spin_i_dot_spin_j;
                 //printf("i=%d, j=%d, spin_i_dot_j=%.6f\n",iOrbGroup,jOrbGroup,spin_i_dot_spin_j);
                 if(iOrbGroup==jOrbGroup) spin4Order[iOrbGroup]+=spin_i_dot_spin_j*spin_i_dot_spin_j;
             }
         }
     }
+    //printf("%.3f %.3f\n",spin_i_r.x,spin_i_r.y);
     double U4=(M2/nsweep)*(M2/nsweep)/(M4/nsweep);
-    double autoCorr=(MdotM_tmp/nsweep-M_tot/nsweep*M_tot/nsweep);
+    double autoCorr=(MdotM_tmp/nsweep-(M_tot/nsweep)*(M_tot/nsweep));
     PyObject *spinDotSpinBetweenGroup_Tuple;
     spinDotSpinBetweenGroup_Tuple=PyTuple_New((nOrbGroup+2)*(nOrbGroup+1));
     for(int iOrbGroup=0;iOrbGroup<(nOrbGroup+1);iOrbGroup++){
         for(int jOrbGroup=0;jOrbGroup<(nOrbGroup+1);jOrbGroup++){
             int index=iOrbGroup*(nOrbGroup+1)+jOrbGroup;
             double result=spinDotSpinBetweenGroup[index]/nsweep;
             PyTuple_SetItem(spinDotSpinBetweenGroup_Tuple, index, PyFloat_FromDouble(result));
         }
     }
     for(int iOrbGroup=0;iOrbGroup<(nOrbGroup+1);iOrbGroup++){
         int index=(nOrbGroup+1)*(nOrbGroup+1)+iOrbGroup;
         double result=spin4Order[iOrbGroup]/nsweep;
         PyTuple_SetItem(spinDotSpinBetweenGroup_Tuple, index, PyFloat_FromDouble(result));
     }
-    if(nOrbGroup==0){
-        spinDotSpinBetweenGroup_Tuple=PyFloat_FromDouble(0);
-    }
-
+    if(nOrbGroup==0) spinDotSpinBetweenGroup_Tuple=PyFloat_FromDouble(0);
     PyObject *Data;
     Data=PyTuple_New(29);
     PyTuple_SetItem(Data, 0, PyFloat_FromDouble(spin_i.x/nsweep));
     PyTuple_SetItem(Data, 1, PyFloat_FromDouble(spin_i.y/nsweep));
-    PyTuple_SetItem(Data, 2, PyFloat_FromDouble(spin_i.z/nsweep));
+    PyTuple_SetItem(Data, 2, PyFloat_FromDouble(0));
     PyTuple_SetItem(Data, 3, PyFloat_FromDouble(spin_j.x/nsweep));
     PyTuple_SetItem(Data, 4, PyFloat_FromDouble(spin_j.y/nsweep));
-    PyTuple_SetItem(Data, 5, PyFloat_FromDouble(spin_j.z/nsweep));
+    PyTuple_SetItem(Data, 5, PyFloat_FromDouble(0));
     PyTuple_SetItem(Data, 6, PyFloat_FromDouble(spin_ij/nsweep));
     PyTuple_SetItem(Data, 7, PyFloat_FromDouble(autoCorr));
     PyTuple_SetItem(Data, 8, PyFloat_FromDouble(totEnergy/nsweep));
     PyTuple_SetItem(Data, 9, PyFloat_FromDouble(E2/nsweep));
     PyTuple_SetItem(Data,10, PyFloat_FromDouble(U4));
     PyTuple_SetItem(Data,11, PyFloat_FromDouble(spin_i_r.x/nsweep));
     PyTuple_SetItem(Data,12, PyFloat_FromDouble(spin_i_r.y/nsweep));
-    PyTuple_SetItem(Data,13, PyFloat_FromDouble(spin_i_r.z/nsweep));
+    PyTuple_SetItem(Data,13, PyFloat_FromDouble(0));
     PyTuple_SetItem(Data,14, PyFloat_FromDouble(spin_j_r.x/nsweep));
     PyTuple_SetItem(Data,15, PyFloat_FromDouble(spin_j_r.y/nsweep));
-    PyTuple_SetItem(Data,16, PyFloat_FromDouble(spin_j_r.z/nsweep));
+    PyTuple_SetItem(Data,16, PyFloat_FromDouble(0));
     PyTuple_SetItem(Data,17, PyFloat_FromDouble(spin_ij_r/nsweep));
     PyTuple_SetItem(Data,18, PyFloat_FromDouble(totEnergy_r/nsweep));
     PyTuple_SetItem(Data,19, PyFloat_FromDouble(E2_r/nsweep));
     PyTuple_SetItem(Data,20, PyFloat_FromDouble(spin_i_z/nsweep));
     PyTuple_SetItem(Data,21, PyFloat_FromDouble(spin_j_z/nsweep));
     PyTuple_SetItem(Data,22, PyFloat_FromDouble(spin_tot_z/nsweep));
     PyTuple_SetItem(Data,23, PyFloat_FromDouble(spin_i_h/nsweep));
     PyTuple_SetItem(Data,24, PyFloat_FromDouble(spin_j_h/nsweep));
     PyTuple_SetItem(Data,25, PyFloat_FromDouble(spin_tot_h/nsweep));
     PyTuple_SetItem(Data,26, PyFloat_FromDouble(topological_q/nsweep));
     PyTuple_SetItem(Data, 27, spinFrameData);
     PyTuple_SetItem(Data, 28, spinDotSpinBetweenGroup_Tuple);
     return Data;
+}
+
+static PyMethodDef module_methods[] = {
+    {"MCMainFunction", MCMainFunction, METH_VARARGS, "the only function in our c lib"},
+    {NULL, NULL, 0, NULL} // neccessary to tell python compiler stop here
+};
+
+static PyModuleDef moduledef = {
+    PyModuleDef_HEAD_INIT,
+    "xylib",
+    "Used to execute the Monte Carlo simulations of xy-model, that is, the O(2) spin model.",
+    -1,
+    module_methods
+};
+
+PyMODINIT_FUNC PyInit_xylib(void) {
+    printf("Initializing xylib...\n");
+    PyObject* m;
+    m= PyModule_Create(&moduledef);
+    return m;
 }
```

### Comparing `mcsolver-3.0.2/mcsolver/input.py` & `mcsolver-3.0.4/mcsolver/input.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import numpy as np
 import Lattice as lat
 import mcMain as mc
 import matplotlib.pyplot as plt
 import time
+
 ## magnetic crystal part
 LMatrix=[[1,0,0],
          [0,1,0],
          [0,0,1]]
 # magnetic orbitals in fractional coordinates
 pos=[[0,0,0]] 
 # spin number
 Spin=[1]
 # single ion anisotropy
-D=np.array([[0.0,0.0,0.0]])
+D=np.array([[0.5,0.0,0.0]])
 # couplings   #source #target #edge  #J(meV) negative for FM coupling
 bond1=lat.Bond(0,0,np.array([1,0,0]),-1,-1,-1, 0, 0, 0, 0, 0, 0, False)
 bond2=lat.Bond(0,0,np.array([0,1,0]),-1,-1,-1, 0, 0, 0, 0, 0, 0, False)
 
 bondList=[bond1,bond2]
 
 time0=time.time()
-mcslave=mc.MC(0,LMatrix,pos=pos,S=Spin,D=D,bondList=bondList,T=2.4,Lx=128,Ly=128,Lz=1,ki_s=0,ki_t=0,ki_overLat=[2,0,0],orbGroupList=[[0]],groupInSC=True,h=0.0,dipoleAlpha=0.0,On=1,spinFrame=0)
+mcslave=mc.MC(0,LMatrix,pos=pos,S=Spin,D=D,bondList=bondList,T=1.0,Lx=8,Ly=8,Lz=1,ki_s=0,ki_t=0,ki_overLat=[2,0,0],orbGroupList=[[0]],groupInSC=True,h=0.0,dipoleAlpha=0.0,On=1,spinFrame=0)
 # Check MC part
-#data=mcslave.mainLoopViaCLib_On(nsweep=80000,nthermal=40000,ninterval=20,algo='Wolff',On=2,flunc=0.0)
 data=mcslave.mainLoopViaCLib(nsweep=80000,nthermal=40000,ninterval=1,algo='Wolff')
+#data=mcslave.mainLoopViaCLib_On(nsweep=80000,nthermal=40000,ninterval=20,algo='Wolff',On=2,flunc=0.0)
 print(data)
 #mean=np.mean(abs(np.array(totSpin)))/mcslave.totOrbs
 #print(np.mean(abs(np.array(corr)))-mean**2)
 
 # Spin-wave part
 
 print('time elapsed: %.3f s'%(time.time()-time0))
```

### Comparing `mcsolver-3.0.2/mcsolver/interface2swt.py` & `mcsolver-3.0.4/mcsolver/interface2swt.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.2/mcsolver/mcMain.py` & `mcsolver-3.0.4/mcsolver/mcMain.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from ctypes import c_double, c_int, CDLL, py_object, c_double, cdll
+#from ctypes import c_double, c_int, CDLL, py_object, c_double, cdll
 from random import random, randint
 import numpy.fft as fft
 import numpy as np
 import matplotlib.pyplot as plt
 import time
-import sys,os
+#import sys,os
 try:
     from . import win
     from . import Lattice as lat
 except:
     import win
     import Lattice as lat
 
@@ -46,16 +46,16 @@
         self.Sz=Lx*Ly*Lz*sum(S)
         self.Energy=0.
         self.blockLen=0
         self.ki_s=ki_s
         self.ki_t=ki_t
         self.h=h
         self.spinFrame=spinFrame
-
-    def mainLoopViaCLib(self,nsweep=1000,nthermal=500,ninterval=-1,algo='Wolff'):
+    '''
+    def __mainLoopViaCLib(self,nsweep=1000,nthermal=500,ninterval=-1,algo='Wolff'):
         self.nsweep=nsweep
         self.nthermal=nthermal
         ninterval=self.totOrbs if ninterval<=0 else ninterval
 
         # initial spin
         initSpin=(c_double*self.totOrbs)()
         nlinking=(c_int*self.totOrbs)()
@@ -179,15 +179,15 @@
         with open('./out','a') as fout:
             fout.write("%.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.6f\n"%(
                 self.T, self.h,   spin_i,    spin_j,  spin_tot,   spin_ij,        E,        E2,   E_rnorm,    E2_rnorm, U4))
         if self.spinFrame>0:
             self.outputSpinDistributionForIsing(spinDistributionList)
         return spin_i, spin_j, spin_ij, autoCorr, E, E2, U4
 
-    def mainLoopViaCLib_On(self,nsweep=1000,nthermal=5000,ninterval=-1,algo='Metroplis',On=3,flunc=0.0,h=0.,binGraph=False):
+    def __mainLoopViaCLib_On(self,nsweep=1000,nthermal=5000,ninterval=-1,algo='Metroplis',On=3,flunc=0.0,h=0.,binGraph=False):
         self.nsweep=nsweep
         self.nthermal=nthermal
         ninterval=self.totOrbs if ninterval<=0 else ninterval
 
         # initial spin, single ion anisotropy and number of linking
         initSpin=(c_double*self.totOrbs)()
         initD=(c_double*(3*self.totOrbs))()
@@ -381,15 +381,239 @@
         # FFT on the MC random data makes no sense
         #if self.spinFrame==nsweep:self.outputSpinWaveSpetra(spinDistributionList) 
         
         if self.spinFrame>0:self.outputSpinDistributionForOn(spinDistributionList)
         
         if len(self.orbGroup)>0:self.outputSpinGroup(spinDotSpinBetweenGroups)
         return spin_i, spin_j, spin_ij, autoCorr, E, E2, U4, topologicalQ
+    '''     
+    
+    def mainLoopViaCLib(self,nsweep=1000,nthermal=500,ninterval=-1,algo='Wolff'):
+        self.nsweep=nsweep
+        self.nthermal=nthermal
+        ninterval=self.totOrbs if ninterval<=0 else ninterval
+
+        # initial spin
+        initSpin=[]
+        nlinking=[]
+        nlinking_list=[]
+        for iorb, orb in enumerate(self.lattice):
+            initSpin.append(orb.spin)
+            nlinking.append(len(orb.linkedOrb))
+            nlinking_list.append(len(orb.linkedOrb))
         
+        # link strength
+        maxNLinking=max(nlinking_list)
+        #nlinking=len(orb.linkedOrb)
+        linkStrength,linkData=[],[]
+        #linkStrength_rnorm=(c_double*(self.totOrbs*maxNLinking))() # linking for renormalization
+        for iorb, orb in enumerate(self.lattice):
+            for ilinking in range(maxNLinking):
+                if ilinking>=nlinking_list[iorb]:
+                    linkData.append(-1)
+                    linkStrength.append(0.)
+                    #linkStrength_rnorm[cnt]=c_double(0.)
+                else:
+                    linkData.append(orb.linkedOrb[ilinking].id)
+                    linkStrength.append(orb.linkStrength[ilinking])
+
+        #-------------------------------------------------------------------------------#
+        # linking info. for renormalized lattice
+        # count total sites in shrinked lat.
+        
+        #print("total %d orbs in renormalized lattice"%totOrb_rnorm)
+        rOrb,rOrbCluster,linkData_rnorm=[],[],[] # store id of renormalized orbs in cluster
+        for orb in self.lattice:
+            if orb.chosen:
+                rOrb.append(orb.id)
+                #print("orb%d is chosen"%orb.id)
+                for orbInCluster in orb.orb_cluster:
+                    rOrbCluster.append(orbInCluster.id)
+
+                for iorb in range(maxNLinking):
+                    if iorb<len(orb.linkedOrb_rnorm):
+                        linkData_rnorm.append(orb.linkedOrb_rnorm[iorb].id) 
+                    else:
+                        linkData_rnorm.append(-1)
+                    #print("orb%d ~ orb%d, linkeData_rnorm[%d]= %d"%(orb.id,orb.linkedOrb_rnorm[iorb].id,cnt,linkData_rnorm[cnt]))
+        #for cnt in range(totOrb_rnorm*maxNLinking):
+        #    print(linkData_rnorm[cnt])
+        #-------------------------------------------------------------------------------#
+        
+        # correlated info.
+        corrOrbitalPair=[]
+        for pair in self.correlatedOrbitalPair: corrOrbitalPair+=pair
+
+        updateAlgorithm=0 # default Metropolis algorithm
+        if algo=='Wolff': updateAlgorithm=1
+
+        try:
+            from isinglib import MCMainFunction
+        except:
+            from mcsolver.lib.isinglib import MCMainFunction
+
+        def callback(k):
+            print("callbak function of python is reporting, recived parameter is:")
+            print(k)
+            return
+        data=MCMainFunction(updateAlgorithm, tuple(initSpin), nthermal, nsweep, ninterval, 
+                            maxNLinking, tuple(nlinking), tuple(linkStrength), tuple(linkData), 
+                            tuple(corrOrbitalPair), self.h/self.T,
+                            tuple(rOrb), tuple(rOrbCluster), tuple(linkData_rnorm),
+                            self.spinFrame,
+                            callback)
+        #print('data has been returned successfully, dim=%d'%len(data))
+        spin_i, spin_j, spin_ij, autoCorr, E, E2, E_rnorm, E2_rnorm, U4, spin_tot, spinDistributionList = data
+        E*=self.T;E2*=self.T**2;E_rnorm*=self.T;E2_rnorm*=self.T**2 # recover the real energies
+        print("%.3f %.3f %.3f %.3f %.3f %.3f %.6f %.3f %.3f %.3f %.3f %.6f %.6f %.6f"%(
+               self.T, self.h,   spin_i,    spin_j,  spin_tot,   spin_ij,        autoCorr,    E,        E2,   E_rnorm,    E2_rnorm, E2-E**2, E2_rnorm-E_rnorm**2, U4))
+        with open('./out','a') as fout:
+            fout.write("%.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.6f\n"%(
+                self.T, self.h,   spin_i,    spin_j,  spin_tot,   spin_ij,        E,        E2,   E_rnorm,    E2_rnorm, U4))
+        if self.spinFrame>0:
+            self.outputSpinDistributionForIsing(spinDistributionList)
+        return spin_i, spin_j, spin_ij, autoCorr, E, E2, U4
+
+    def mainLoopViaCLib_On(self,nsweep=1000,nthermal=5000,ninterval=-1,algo='Metroplis',On=3,flunc=0.0,h=0.,binGraph=False):
+        def callback(k):
+            print("callbak function of python is reporting, recived parameter is:")
+            print(k)
+            return
+        
+        self.nsweep=nsweep
+        self.nthermal=nthermal
+        ninterval=self.totOrbs if ninterval<=0 else ninterval
+
+        updateAlgorithm=0 # default Metropolis algorithm
+        if algo=='Wolff': updateAlgorithm=1
+
+        initSpin,initD,nlinking=[],[],[]
+        for orb in self.lattice:
+            initSpin.append(orb.spin)
+            for i in range(3):
+                initD.append(orb.D[i])
+            nlinking.append(len(orb.linkedOrb))
+        
+        # link strength
+        ignoreNonDiagonalJ=1
+        maxNLinking=max(nlinking)
+        linkStrength,linkData=[],[] # thus the nlinking of every orbs are the same
+        
+        for iorb, orb in enumerate(self.lattice):
+            #print("orb%d"%orb.id)
+            for ilinking in range(maxNLinking):
+                if ilinking>=nlinking[iorb]:
+                    linkData.append(-1)
+                    for i in range(9):  # set the redundant bond strength to zero
+                        linkStrength.append(0.)
+                else:
+                    linkData.append(orb.linkedOrb[ilinking].id)
+                    #print("link %d :"%ilinking,orb.linkStrength[ilinking])
+                    for i in range(9):  # set the bond strength
+                        linkStrength.append(orb.linkStrength[ilinking][i])
+                        if abs(orb.linkStrength[ilinking][i]) > 1e-6 and i>=3: ignoreNonDiagonalJ=0
+
+        # topological circuits
+        localCircuits=[]
+        for circuit in self.localCircuit:
+            for orb in circuit: localCircuits+=[orb.id]
+        
+        # correlated info.
+        corrOrbitalPair=[]
+        for pair in self.correlatedOrbitalPair:corrOrbitalPair+=pair
+
+        # orb group
+        nOrbGroup=len(self.orbGroup)
+        maxOrbGroupSize=1
+        if nOrbGroup>0:
+            maxOrbGroupSize=len(self.orbGroup[0])
+        if nOrbGroup>1:
+            maxOrbGroupSize=np.max([len(subGroup) for subGroup in self.orbGroup])
+        orbGroupList=[]
+        for subGroup in self.orbGroup:
+            for iorb in range(maxOrbGroupSize):
+                if iorb<len(subGroup):
+                    orbGroupList.append(subGroup[iorb].id)
+                else:
+                    orbGroupList.append(-1)
+        #print(nOrbGroup,maxOrbGroupSize)
+        #exit()
+
+        #-------------------------------------------------------------------------------#
+        # linking info. for renormalized lattice
+        # count total sites in shrinked lat.
+        
+        #print("total %d orbs in renormalized lattice"%totOrb_rnorm)
+        rOrb,rOrbCluster,linkData_rnorm=[],[],[] # store id of renormalized orbs
+        #print("checking while preparing info.>>>>")
+        for orb in self.lattice:
+            if orb.chosen:
+                #print("orb%d is chosen"%orb.id)
+                rOrb.append(orb.id)
+                for orbInCluster in orb.orb_cluster:
+                    rOrbCluster.append(orbInCluster.id)
+                    #print("    orb%d"%orbInCluster.id)
+            
+                for iorb in range(maxNLinking):
+                    if iorb<len(orb.linkedOrb_rnorm):
+                        linkData_rnorm.append(orb.linkedOrb_rnorm[iorb].id)  
+                    else:
+                        linkData_rnorm.append(-1)
+                    #print("orb%d ~ orb%d, linkeData_rnorm[%d]= %d"%(orb.id,orb.linkedOrb_rnorm[iorb].id,cnt,linkData_rnorm[cnt]))
+        #print("<<<<")
+                
+        #for cnt in range(totOrb_rnorm*maxNLinking):
+        #    print(linkData_rnorm[cnt])
+        #-------------------------------------------------------------------------------#
+        if On==2:
+            try:
+                from xylib import MCMainFunction
+            except:
+                from mcsolver.lib.xylib import MCMainFunction
+        elif On==3:
+            try:
+                from heisenberglib import MCMainFunction
+            except:
+                from mcsolver.lib.heisenberglib import MCMainFunction
+        
+        data = MCMainFunction(updateAlgorithm,tuple(initSpin),tuple(initD),nthermal,nsweep,ninterval,
+                             maxNLinking,tuple(nlinking),tuple(linkStrength),tuple(linkData),
+                             tuple(localCircuits),
+                             tuple(corrOrbitalPair),
+                             nOrbGroup, maxOrbGroupSize, tuple(orbGroupList),
+                             flunc, self.h/self.T,
+                             tuple(rOrb), tuple(rOrbCluster), tuple(linkData_rnorm),
+                             self.spinFrame,
+                             ignoreNonDiagonalJ,
+                             callback)
+        
+        spin_i_x, spin_i_y, spin_i_z, spin_j_x, spin_j_y, spin_j_z, spin_ij, autoCorr, E, E2, U4, spin_i_r_x, spin_i_r_y, spin_i_r_z, spin_j_r_x, spin_j_r_y, spin_j_r_z, spin_ij_r, E_r, E2_r, spin_i_tot_z,spin_j_tot_z,spin_tot_z,spin_i_h,spin_j_h,spin_tot_h, topologicalQ, spinDistributionList, spinDotSpinBetweenGroups=data
+        E*=self.T;E2*=self.T**2;E_r*=self.T;E2_r*=self.T**2 # recover the real energies
+        C=E2-E*E
+        C_r=E2_r-E_r*E_r
+        spin_i=np.array([spin_i_x, spin_i_y, spin_i_z])
+        spin_j=np.array([spin_j_x, spin_j_y, spin_j_z])
+        spin_i_len=np.sqrt(np.dot(spin_i,spin_i))
+        spin_j_len=np.sqrt(np.dot(spin_j,spin_j))
+        spin_i_r=np.array([spin_i_r_x, spin_i_r_y, spin_i_r_z])
+        spin_j_r=np.array([spin_j_r_x, spin_j_r_y, spin_j_r_z])
+        #      T       <i><j>     <ij>      <autoCorr>      <E>      <E2>      <U4>      <E_r>      <E2_r>  C  C_v
+        print('%.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.6f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f'%(
+               self.T,self.h,spin_i_tot_z,spin_j_tot_z,spin_tot_z,spin_i_h,spin_j_h,spin_tot_h,spin_i_len,spin_j_len,spin_ij,np.dot(spin_i,spin_j),E,E2,       U4,spin_ij_r,np.dot(spin_i_r,spin_j_r),       E_r,      E2_r, topologicalQ))
+        with open('./out','a') as fout:
+            fout.write('%.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.6f %.3f %.3f %.3f %.3f %.3f %.3f %.3f %.3f\n'%(
+                   self.T,self.h,spin_i_tot_z,spin_j_tot_z,spin_tot_z,spin_i_h,spin_j_h,spin_tot_h,spin_i_len,spin_j_len,spin_ij,np.dot(spin_i,spin_j),E,E2,       U4,spin_ij_r,np.dot(spin_i_r,spin_j_r),       E_r,      E2_r, topologicalQ))
+        # FFT on the MC random data makes no sense
+        #if self.spinFrame==nsweep:self.outputSpinWaveSpetra(spinDistributionList) 
+        
+        if self.spinFrame>0:self.outputSpinDistributionForOn(spinDistributionList)
+        
+        if len(self.orbGroup)>0:self.outputSpinGroup(spinDotSpinBetweenGroups)
+        return spin_i, spin_j, spin_ij, autoCorr, E, E2, U4, topologicalQ
+
     def outputSpinGroup(self,spinDotSpinData):
         with open('./spinDotSpin.txt','a') as fout:
             # title
             fout.write('%.3f %.3f '%(self.T,self.h))
             cnt=0
             for i in range(len(self.orbGroup)+1):
                 for j in range(len(self.orbGroup)+1):
```

### Comparing `mcsolver-3.0.2/mcsolver/toolbox.py` & `mcsolver-3.0.4/mcsolver/toolbox.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.2/mcsolver/win.py` & `mcsolver-3.0.4/mcsolver/win.py`

 * *Files identical despite different names*

### Comparing `mcsolver-3.0.2/mcsolver/xyLib.c` & `mcsolver-3.0.4/mcsolver/heisenbergLib.c`

 * *Files 15% similar despite different names*

```diff
@@ -1,160 +1,209 @@
+#define PY_SSIZE_T_CLEAN
 #include "Python.h"
 #include <stdio.h>
 #include <stdlib.h>
 #include <math.h>
-
+#define PI 3.1415926535
 typedef struct Vec
 {
     int dimension;
-    double x,y;
+    double len;
+    double x,y,z;
 }Vec;
-typedef struct Vec4
+typedef struct Vec9
 {
     int dimension;
-    double xx,yy,xy,yx;
-}Vec4;
+    double xx,yy,zz,xy,xz,yz,yx,zx,zy;
+}Vec9;
 // vec1=abs(vec1)
 void normalize(Vec *vec1){
-    double len=sqrt(vec1->x*vec1->x+vec1->y*vec1->y);
+    double len=sqrt(vec1->x*vec1->x+vec1->y*vec1->y+vec1->z*vec1->z);
     if (len<1e-5) return;
     vec1->x/=len;
     vec1->y/=len;
+    vec1->z/=len;
 }
 // vec1=vec2
 void equal(Vec *vec1, Vec vec2){
     vec1->x=vec2.x;
     vec1->y=vec2.y;
-}
-// vec1*=c
-void cTimes(Vec *vec1, double c){
-    vec1->x*=c;
-    vec1->y*=c;
+    vec1->z=vec2.z;
 }
 // vec1=fabs(vec1)
 void vabs(Vec *vec1){
     vec1->x=fabs(vec1->x);
     vec1->y=fabs(vec1->y);
+    vec1->z=fabs(vec1->z);
 }
 // vec1/=c
 void cDivides(Vec *vec1, double c){
     vec1->x/=c;
     vec1->y/=c;
+    vec1->z/=c;
+}
+// vec1*=c
+void cTimes(Vec *vec1, double c){
+    vec1->x*=c;
+    vec1->y*=c;
+    vec1->z*=c;
 }
 // vec1+=vec2
 void plusEqual(Vec *vec1, Vec vec2){
     vec1->x+=vec2.x;
     vec1->y+=vec2.y;
+    vec1->z+=vec2.z;
 }
 // vec1-=vec2
 void minusEqual(Vec *vec1, Vec vec2){
     vec1->x-=vec2.x;
     vec1->y-=vec2.y;
+    vec1->z-=vec2.z;
 }
 // vec1 dot vec2
 double dot(Vec vec1, Vec vec2){
-    return vec1.x*vec2.x+vec1.y*vec2.y;
-}
-
-double diagonalDot(Vec vec1, Vec vec2, Vec4 matrix){
-    return vec1.x*vec2.x*matrix.xx+
-           vec1.y*vec2.y*matrix.yy+
-           vec1.x*vec2.y*matrix.xy+
-           vec1.y*vec2.x*matrix.yx;
+    return vec1.x*vec2.x+vec1.y*vec2.y+vec1.z*vec2.z;
 }
-double diagonalDot_simple(Vec vec1, Vec vec2, Vec4 matrix){
-    return vec1.x*vec2.x*matrix.xx+
-           vec1.y*vec2.y*matrix.yy;
+// vec1 cross vec2
+Vec* cross(Vec vec1, Vec vec2){
+    Vec *vec3=(Vec*)malloc(sizeof(Vec));
+    vec3->x=vec1.y*vec2.z - vec1.z*vec2.y;
+    vec3->y=vec1.z*vec2.x - vec1.x*vec2.z;
+    vec3->z=vec1.x*vec2.y - vec1.y*vec2.x;
+    return vec3;
+}
+
+double (*p_diagonalDot)(Vec vec1, Vec vec2, Vec9 J);
+
+double diagonalDot(Vec vec1, Vec vec2, Vec9 J){
+    return vec1.x*vec2.x*J.xx+
+           vec1.y*vec2.y*J.yy+
+           vec1.z*vec2.z*J.zz+
+           vec1.x*vec2.y*J.xy+
+           vec1.x*vec2.z*J.xz+
+           vec1.y*vec2.z*J.yz+
+           vec1.y*vec2.x*J.yx+
+           vec1.z*vec2.x*J.zx+
+           vec1.z*vec2.y*J.zy;
+}
+
+double diagonalDot_simple(Vec vec1, Vec vec2, Vec9 J){
+    return vec1.x*vec2.x*J.xx+
+           vec1.y*vec2.y*J.yy+
+           vec1.z*vec2.z*J.zz;
 }
-double (*p_diagonalDot)(Vec vec1, Vec vec2, Vec4 matrix);
-
-double gaussian_distr[RAND_MAX];
 
 Vec *generateRandomVec(void){
     double x=rand()/(double) RAND_MAX-0.5;
     double y=rand()/(double) RAND_MAX-0.5;
-    double len2=(x*x+y*y);
+    double z=rand()/(double) RAND_MAX-0.5;
+    double len2=(x*x+y*y+z*z);
     if (len2>0.25)
     {
         return generateRandomVec();
     }else
     {
         double len=sqrt(len2);
         Vec *direction=(Vec*)malloc(sizeof(Vec));
         direction->x=x/len;
         direction->y=y/len;
+        direction->z=z/len;
         return direction;
     }
 }
 
+double calcSignedArea(Vec s1, Vec s2, Vec s3){
+    double s1s2=dot(s1,s2)/s1.len/s2.len;
+    double s2s3=dot(s2,s3)/s2.len/s3.len;
+    double s3s1=dot(s3,s1)/s3.len/s1.len;
+    Vec* s2xs3=cross(s2,s3);
+    double realPart = 1+s1s2+s2s3+s3s1;
+    double imagPart = dot(s1, *s2xs3)/s1.len/s2.len/s3.len;
+    free(s2xs3);
+    if(fabs(realPart)<1e-6){
+        if(imagPart>0)return PI;
+        return -PI;
+    }
+    return 2*atan(imagPart/realPart);
+}
+
 typedef struct Orb
 {
     int id;
-    double S; // maximum spin number
+    double S; 
     Vec spin;
     Vec transSpin;
     Vec perpenSpin;
     int nlink;
-    Vec4 *linkStrength;
+    Vec9 *linkStrength;
     int inBlock;
     struct Orb **linkedOrb;
     struct Orb **linkedOrb_rnorm;
     Vec onsiteAnisotropy;
 
     double d_onsiteEnergy;
     double sDotN;
     int isProjected;
     int chosen;
     int nOrbInCluster;
     struct Orb **orb_cluster;
-
-    double h;
     
+    double h;
 }Orb;
 
 //establishLattice(lattice, totOrbs, initSpin, maxNLinking, nlink, linkStrength);
-void establishLattice(Orb *lattice, int totOrbs, double initSpin[totOrbs], double initD[totOrbs][3], double flunc, int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking][9], double h,
+void establishLattice(Orb *lattice, int totOrbs, double initSpin[totOrbs], double initD[totOrbs][3], double h, double flunc, int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking][9],
                       int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm][nOrbInCluster]){
     //printf("establishing whole lattice with %d orbs and %d linkings for each orb\n",totOrbs,maxNLinking);
-    int i;
-    for(i=0;i<totOrbs;i++){
+    for(int i=0;i<totOrbs;i++){
         //printf("check point-1, entering setting %d",i);
         lattice[i].id=i;
         lattice[i].S=initSpin[i];
+        //lattice[i].spin.coor=(double*)malloc(3*sizeof(double));  // allocate spin vector for each orb
         lattice[i].spin.x=initSpin[i];
         lattice[i].spin.y=0;
+        lattice[i].spin.z=0;
+        lattice[i].spin.len=fabs(initSpin[i]);
 
         Vec *fluncSpin=generateRandomVec();
         cTimes(fluncSpin, flunc);
         plusEqual(&lattice[i].spin,*fluncSpin);
         normalize(&lattice[i].spin);
         cTimes(&lattice[i].spin,fabs(initSpin[i]));
         free(fluncSpin);
-
+        //printf("%.3f %.3f \n",lattice[i].spin.x, fabs(initSpin[i]));
         lattice[i].onsiteAnisotropy.x=initD[i][0];
         lattice[i].onsiteAnisotropy.y=initD[i][1];
+        lattice[i].onsiteAnisotropy.z=initD[i][2];
 
         lattice[i].h=h;
         //printf("orb %d spin: %.3f %.3f %.3f\n",i,lattice[i].spin.coor[0],lattice[i].spin.coor[1],lattice[i].spin.coor[2]);
         lattice[i].transSpin.x=0;  // allocate trans spin vector for each orb
         lattice[i].transSpin.y=0;
+        lattice[i].transSpin.z=0;
         lattice[i].perpenSpin.x=0;
         lattice[i].perpenSpin.y=0;
+        lattice[i].perpenSpin.z=0;
         lattice[i].nlink=nlink[i];
         //printf("check point 1, orb: %d\n",lattice[i].id);
-        lattice[i].linkStrength=(Vec4*)malloc(lattice[i].nlink*sizeof(Vec4)); // allocate strength for each linking
+        lattice[i].linkStrength=(Vec9*)malloc(nlink[i]*sizeof(Vec9)); // allocate strength for each linking
         //printf("check point 2, total links:%d\n",nlink[i]);
         for(int j=0;j<nlink[i];j++){
             //lattice[i].linkStrength[j].coor=(double*)malloc(3*sizeof(double));
             //printf("check point 3\n");
             lattice[i].linkStrength[j].xx=linkStrength[i][j][0];
             lattice[i].linkStrength[j].yy=linkStrength[i][j][1];
+            lattice[i].linkStrength[j].zz=linkStrength[i][j][2];
             lattice[i].linkStrength[j].xy=linkStrength[i][j][3];
+            lattice[i].linkStrength[j].xz=linkStrength[i][j][4];
+            lattice[i].linkStrength[j].yz=linkStrength[i][j][5];
             lattice[i].linkStrength[j].yx=linkStrength[i][j][6];
-            //printf("check point 4, link:%d, strength: %.3f %.3f\n",j,lattice[i].linkStrength[j].x,lattice[i].linkStrength[j].y);
+            lattice[i].linkStrength[j].zx=linkStrength[i][j][7];
+            lattice[i].linkStrength[j].zy=linkStrength[i][j][8];
+            //printf("check point 4, link:%d, strength: %.3f %.3f %.3f\n",j,lattice[i].linkStrength[j].coor[0],lattice[i].linkStrength[j].coor[1],lattice[i].linkStrength[j].coor[2]);
         }
         lattice[i].chosen=0;
     }
     //printf("now checking the orb cluster\n");
     for(int i=0;i<totOrb_rnorm;i++){
         int id=rOrb[i];
         lattice[id].chosen=1;
@@ -168,92 +217,98 @@
     }
     //printf("orbitals successfully built\n");
 }
 
 void establishLinking(Orb *lattice, int totOrbs, int maxNLinking, int nlink[totOrbs], int linkedOrb[totOrbs][maxNLinking],
                       int totOrb_rnorm, int rOrb[totOrb_rnorm], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking]){
     for(int iorb=0;iorb<totOrbs;iorb++){
-        lattice[iorb].linkedOrb=(Orb**)malloc(lattice[iorb].nlink*sizeof(Orb*));
+        lattice[iorb].linkedOrb=(Orb**)malloc(nlink[iorb]*sizeof(Orb*));
         for(int ilink=0;ilink<nlink[iorb];ilink++){
             lattice[iorb].linkedOrb[ilink]=lattice+linkedOrb[iorb][ilink];
         }
     }
     for(int i=0;i<totOrb_rnorm;i++){
         int iorb=rOrb[i];
         lattice[iorb].linkedOrb_rnorm=(Orb**)malloc(nlink[iorb]*sizeof(Orb*));
         for(int ilink=0;ilink<nlink[iorb];ilink++){
             lattice[iorb].linkedOrb_rnorm[ilink]=lattice+linkedOrb_rnorm[i][ilink];
         }
     }
-    //printf("bonds successfully built\n");
 }
 
 double getCorrEnergy(Orb *source){
+    //printf("start calc corr. energy\n");
     double corr=0;
     for(int i=0;i<source->nlink;i++){
-        //printf("getCorrEnergy\n");
         corr+=(*p_diagonalDot)(source->spin,source->linkedOrb[i]->spin,source->linkStrength[i]);
+        //printf("J=%.3f S1=%.3f S2=%.3f\n",source->linkStrength[i],source->spin,source->linkedOrb[i]->spin);
+        //printf("corr=%.3f\n",corr);
     }
     return corr;
 }
 
-double getOnsiteEnergy(Orb *source){
+double getOnsiteEnergy(Orb *source){  // onsite term
     return source->onsiteAnisotropy.x*source->spin.x*source->spin.x+
-           source->onsiteAnisotropy.y*source->spin.y*source->spin.y-
-           source->h*source->spin.x;
+           source->onsiteAnisotropy.y*source->spin.y*source->spin.y+
+           source->onsiteAnisotropy.z*source->spin.z*source->spin.z-source->h*source->spin.z;
 }
 
-Vec getMajoritySpin(Orb*_orb){  // core algorithm for renormalization
+Vec getMajoritySpin(Orb*_orb){ // core algorithm for renormalization
     //return _orb->spin; // decimation algorithm
     Vec avgSpin;
     avgSpin.x=0;
     avgSpin.y=0;
+    avgSpin.z=0;
     for(int iorb=0;iorb<_orb->nOrbInCluster;iorb++){
         plusEqual(&avgSpin,_orb->orb_cluster[iorb]->spin);
     }
-    //cDivides(&avgSpin,_orb->nOrbInCluster);
     normalize(&avgSpin);
     cTimes(&avgSpin, _orb->S);
     return avgSpin; // majority algorithm
 }
 
-double getCorrEnergy_rnorm(Orb *source){
+double getCorrEnergy_rnorm(Orb *source, double (*p_diagonalFunc)()){
     double corr=0;
     Vec avgSpin_source=getMajoritySpin(source);
     for(int i=0;i<source->nlink;i++){
         //printf("link to orb%d\n",source->linkedOrb_rnorm[i]->id);
         Vec avgSpin_target=getMajoritySpin(source->linkedOrb_rnorm[i]);
-        corr+=(*p_diagonalDot)(avgSpin_source,avgSpin_target,source->linkStrength[i]);
+        corr+=(*p_diagonalFunc)(avgSpin_source,avgSpin_target,source->linkStrength[i]);
     }
     //printf("Ecorr=%.3f\n",corr);
     return corr;
 }
 
 double getOnsiteEnergy_rnorm(Orb *source){
     Vec avgSpin_source=getMajoritySpin(source);
     return source->onsiteAnisotropy.x*avgSpin_source.x*avgSpin_source.x+
-           source->onsiteAnisotropy.y*avgSpin_source.y*avgSpin_source.y-
-           source->h*avgSpin_source.x;
+           source->onsiteAnisotropy.y*avgSpin_source.y*avgSpin_source.y+
+           source->onsiteAnisotropy.z*avgSpin_source.z*avgSpin_source.z-source->h*avgSpin_source.z;
 }
 
-double getDeltaCorrEnergy(Orb *source){
+double getDeltaCorrEnergy(Orb *source){//, double (*p_diagonalFunc)()){
     double corr=0;
+    //printf("centre orb%d, trial trans %.3f %.3f %.3f, len %.3f\n",source->id,source->transSpin.x,source->transSpin.y,source->transSpin.z,sqrt(dot(source->transSpin,source->transSpin)));
     for(int i=0;i<source->nlink;i++){
-        //printf("getDeltaCorrEnergy\n");
+        //printf("corr to orb%d, J %.3f %.3f %.3f S %.3f %.3f %.3f, \n",source->linkedOrb[i]->id,source->linkStrength[i].x,source->linkStrength[i].y,source->linkStrength[i].z,source->linkedOrb[i]->spin.x,source->linkedOrb[i]->spin.y,source->linkedOrb[i]->spin.z);
         corr+=(*p_diagonalDot)(source->transSpin,source->linkedOrb[i]->spin,source->linkStrength[i]);
     }
+    //printf("total corr %.6f\n",corr);
     return corr;
 }
 
 double getDeltaOnsiteEnergy(Orb *source){
     double s1x=source->spin.x+source->transSpin.x;
     double s1y=source->spin.y+source->transSpin.y;
+    double s1z=source->spin.z+source->transSpin.z;
+    //printf("h %.3f, transSpin %.3f\n",source->h,source->transSpin.z);
     return source->onsiteAnisotropy.x*(s1x*s1x-source->spin.x*source->spin.x)+
-           source->onsiteAnisotropy.y*(s1y*s1y-source->spin.y*source->spin.y)-
-           source->h*source->transSpin.x;
+           source->onsiteAnisotropy.y*(s1y*s1y-source->spin.y*source->spin.y)+
+           source->onsiteAnisotropy.z*(s1z*s1z-source->spin.z*source->spin.z)-
+           source->h*source->transSpin.z;
 }
 
 int expandBlock(int*beginIndex, int*endIndex, Orb *buffer[], int*blockLen, Orb *block[], Vec refDirection){
     //printf("  Buffer: now start and end pt is %d, %d.\n",*beginIndex, *endIndex);
     if(*beginIndex>*endIndex) return 0;
 
     // FIFO
@@ -261,29 +316,30 @@
     *beginIndex+=1; // pop out the first element
     
     //FILO
     //Orb *outOrb=buffer[*endIndex];
     //*endIndex-=1; // pop out the last element
 
     if(outOrb->isProjected==0){
+        // calc. perpendicular and transverse parts (to refDirection)
         outOrb->sDotN=-dot(outOrb->spin,refDirection);
         equal(&outOrb->transSpin, refDirection);
         cTimes(&outOrb->transSpin, outOrb->sDotN);
         equal(&outOrb->perpenSpin,outOrb->spin);
         plusEqual(&outOrb->perpenSpin,outOrb->transSpin);
         outOrb->isProjected=1;
     }
     //printf("center orb: %d\n", outOrb->id);
     //printf("projection along axis: %.3f\n", -s1n/2);
-    //printf("variation of spin: %.3f %.3f\n",outOrb->transSpin.x,outOrb->transSpin.y);
+    //printf("variation of spin: %.3f %.3f %.3f\n",outOrb->transSpin.coor[0],outOrb->transSpin.coor[1],outOrb->transSpin.coor[2]);
     //printf("it has %d neighbor orbs\n",outOrb->nlink);
     int i;
     for(i=0;i<outOrb->nlink;i++){
         //double effectiveJ=diagonalDot(outOrb->linkStrength[i], refDirection, refDirection);
-        //printf("the %d linking has strength %.3f %.3f (original) %.3f (effective)\n",i,outOrb->linkStrength[i].x,outOrb->linkStrength[i].y,effectiveJ);
+        //printf("the %d linking has strength %.3f %.3f %.3f (original) %.3f (effective)\n",i,outOrb->linkStrength[i].coor[0],outOrb->linkStrength[i].coor[1],outOrb->linkStrength[i].coor[2],effectiveJ);
         Orb *linkedOrb=outOrb->linkedOrb[i];
         //printf("consider to add orb %d\n",linkedOrb->id);
         //printf("      considering the %d orb which is linking to %d orb, it is %d in block \n", linkedOrb->id, outOrb->id, linkedOrb->inBlock);
         if(linkedOrb->inBlock==0){
             //printf("projection along axis: %.3f\n", s2n);
             //double corr=-s1n*diagonalDot(refDirection,outOrb->linkStrength[i],linkedOrb->spin); // bond strength
             //printf("      spin of orb %d is %.3f %.3f %.3f and bond strength is %.3f\n",linkedOrb->id,linkedOrb->spin.coor[0],linkedOrb->spin.coor[1],linkedOrb->spin.coor[2],corr);
@@ -292,15 +348,14 @@
                 linkedOrb->sDotN=-dot(linkedOrb->spin,refDirection);
                 equal(&linkedOrb->transSpin, refDirection);
                 cTimes(&linkedOrb->transSpin, linkedOrb->sDotN);
                 equal(&linkedOrb->perpenSpin, linkedOrb->spin);
                 plusEqual(&linkedOrb->perpenSpin, linkedOrb->transSpin);
                 linkedOrb->isProjected=1;
             }
-            //printf("229\n");
             double corr=2*outOrb->sDotN*linkedOrb->sDotN*(*p_diagonalDot)(refDirection,refDirection,outOrb->linkStrength[i]);
             
             //linkedOrb->d_onsiteEnergy=getDeltaOnsiteEnergy(linkedOrb);
             if(corr<0 && (1-exp(corr))>rand()/(double) RAND_MAX){
                 //printf("          -->>fortunately it is added to block with possibility %f\n",(1-exp(2*corr)));
                 // update block
                 *blockLen+=1;
@@ -330,17 +385,17 @@
 
     Vec *refDirection=generateRandomVec();
     //refDirection.coor=(double*)malloc(3*sizeof(double));
     //equal(&refDirection, &block[0]->spin);
     //normalize(&refDirection);
     //printf("-------------------\n");
     //printf("the seed Orb is %d\n",block[0]->id);
-    //printf("trial normal direction %.3f %.3f\n",refDirection->x,refDirection->y);
-    //double effectiveJ=diagonalDot(block[0]->linkStrength[0], *refDirection, *refDirection);
-    //printf("the 0 linking has strength %.3f %.3f (original) %.3f (effective)\n",block[0]->linkStrength[0].x,block[0]->linkStrength[1].y,effectiveJ);
+    //printf("trial normal direction %.3f %.3f %.3f\n",refDirection.coor[0],refDirection.coor[1],refDirection.coor[2]);
+    //double effectiveJ=diagonalDot(block[0]->linkStrength[0], refDirection, refDirection);
+    //printf("the 0 linking has strength %.3f %.3f %.3f (original) %.3f (effective)\n",block[0]->linkStrength[0].coor[0],block[0]->linkStrength[1].coor[1],block[0]->linkStrength[2].coor[2],effectiveJ);
     while (expandBlock(p_beginIndex, p_endIndex, buffer, p_blockLen, block, *refDirection)==1)
     {
         // no code here
     }
     
     //printf("    Block size is %d\n",*p_blockLen);
     double tot_d_onsiteEnergy=0;
@@ -356,14 +411,17 @@
                 tot_d_onsiteEnergy+=source_anisotropy;
             }
         }
     }
     // single-ion anisotropy
     for(i=0;i<*p_blockLen;i++) tot_d_onsiteEnergy+=getDeltaOnsiteEnergy(block[i]);
     // process the onsite anisotropy
+    //printf("tot_d_onsiteEnergy=%.6f\n",tot_d_onsiteEnergy);
+    //tot_d_onsiteEnergy=0;
+    //if(fabs(tot_d_onsiteEnergy)>1e-5) printf("Anisotropy energy=%.3f\n",tot_d_onsiteEnergy);
     if(tot_d_onsiteEnergy<=0 || exp(-tot_d_onsiteEnergy)>rand()/(double) RAND_MAX){
         for(i=0;i<*p_blockLen;i++){
             cTimes(&block[i]->transSpin,2);
             plusEqual(&block[i]->spin, block[i]->transSpin);
             //printf("    after update orb %d spin converted to %.3f %.3f %.3f\n",block[i]->id,block[i]->spin.coor[0],block[i]->spin.coor[1],block[i]->spin.coor[2]);
             //block[i]->inBlock=0;
             plusEqual(p_totSpin,block[i]->transSpin);
@@ -376,94 +434,208 @@
     }
     // clean
     free(refDirection);
 }
 
 void localUpdate(int totOrbs, Orb lattice[], double *p_energy, Vec *p_totSpin){
     //printf("start local updating\n");
-    int seedID=rand()%totOrbs;  // chose one orb Note that WE CANNOT CHOOSE GHOST SPIN, since it's not compatible with local statistics
-    //int seedID=totOrbs;
-    //printf("considering %d orb, its spin is %.3f %.3f\n",
-    //         seedID,lattice[seedID].spin.x,lattice[seedID].spin.y);
+    int seedID=rand()%totOrbs;  // chose one orb
+    //printf("considering %d orb, its spin is %.3f %.3f %.3f\n",
+    //         seedID,lattice[seedID].spin.coor[0],lattice[seedID].spin.coor[1],lattice[seedID].spin.coor[2]);
     Vec *refDirection=generateRandomVec(); // chose new direction
-    //printf("try new spin direction, ref: %.3f %.3f\n",
-    //       refDirection->x,refDirection->y);
+    //printf("try new spin direction, ref: %.3f %.3f %.3f\n",
+    //       refDirection.coor[0],refDirection.coor[1],refDirection.coor[2]);
     double s1n=-2*dot(lattice[seedID].spin,*refDirection);
     //printf("projection s1n: %.3f\n",s1n);
     equal(&lattice[seedID].transSpin,*refDirection);
     cTimes(&lattice[seedID].transSpin,s1n);
-    double corr=getDeltaCorrEnergy(lattice+seedID);
+    double corr=getDeltaCorrEnergy(lattice+seedID);//,p_diagonalFunc);
     corr+=getDeltaOnsiteEnergy(lattice+seedID);
     
-    //printf("lead to the translation spin vector: %.3f %.3f and delta Ecorr: %.3f, transition possibility %.3f P\n",
-    //      lattice[seedID].transSpin.x,lattice[seedID].transSpin.y,corr,100*exp(-corr));
+    //printf("lead to the translation spin vector: %.3f %.3f %.3f and delta Ecorr: %.3f\n",
+    //      lattice[seedID].transSpin.x,lattice[seedID].transSpin.y,lattice[seedID].transSpin.z,corr);
     
     if(corr<=0 || exp(-corr)>rand()/(double) RAND_MAX){  // new direction is energertically favoured thus accept directly
         plusEqual(p_totSpin,lattice[seedID].transSpin);
         plusEqual(&lattice[seedID].spin,lattice[seedID].transSpin);
         *p_energy+=corr;
-        //printf("Luckily we accept the transition, energy: %.3f\n",*p_energy);
+        //printf("since new direction is energertically lowerd thus we accept, energy: %.3f\n",*p_energy);
+        //double energy_tmp=0;
+        //for(int i=0;i<totOrbs;i++) energy_tmp+=getCorrEnergy(lattice+i);
+        //energy_tmp/=2;
+        //printf("ref energy (with out onsite) %.3f\n",energy_tmp);
     }
     free(refDirection);
     return;
 }
 
-void (*p_mcUpdate)(int totOrbs, Orb lattice[], double*p_energy, Vec *p_totSpin);
+// interface to block update and local update algorithm
+void (*p_mcUpdate)(int totOrbs, Orb lattice[], double *p_energy, Vec *p_totSpin);
 
-PyObject * MCMainFunction(int algorithm, int totOrbs, double initSpin[totOrbs], double initD[totOrbs][3], int nthermal, int nsweep, 
-                   int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking][9], int linkedOrb[totOrbs][maxNLinking], int nLocalCircuits, int localCircuits[nLocalCircuits][3],
-                   int ninterval, int nLat, int corrOrbPair[nLat][2], int nOrbGroup, int maxOrbGroupSize, int orbGroupList[nOrbGroup][maxOrbGroupSize], double flunc, double h,
-                   int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm][nOrbInCluster], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking],
-                   int spinFrame,
-                   int ignoreNonDiagonalJ){
+//PyObject * MCMainFunction(int algorithm, int totOrbs, double initSpin[totOrbs], double initD[totOrbs][3], int nthermal, int nsweep, 
+//                   int maxNLinking, int nlink[totOrbs], double linkStrength[totOrbs][maxNLinking][9], int linkedOrb[totOrbs][maxNLinking],  int nLocalCircuits, int localCircuits[nLocalCircuits][3],
+//                   int ninterval, int nLat, int corrOrbPair[nLat][2], int nOrbGroup, int maxOrbGroupSize, int orbGroupList[nOrbGroup][maxOrbGroupSize], double flunc, double h,
+//                   int totOrb_rnorm, int nOrbInCluster, int rOrb[totOrb_rnorm], int rOrbCluster[totOrb_rnorm][nOrbInCluster], int linkedOrb_rnorm[totOrb_rnorm][maxNLinking],
+//                   int spinFrame,
+//                   int ignoreNonDiagonalJ){
+PyObject * MCMainFunction(PyObject* self, PyObject* args){
+    // read in all parameters
+    PyObject* py_algorithm;
+    PyObject* py_initSpin;
+    PyObject* py_initD;
+    PyObject* py_nthermal;
+    PyObject* py_nsweep;
+    PyObject* py_maxNLinking;
+    PyObject* py_ninterval;
+    PyObject* py_nlink;
+    PyObject* py_linkStrength;
+    PyObject* py_linkedOrb;
+    PyObject* py_localCircuits;
+    PyObject* py_corrOrbPair;
+    PyObject* py_nOrbGroup;
+    PyObject* py_maxOrbGroupSize;
+    PyObject* py_orbGroupList;
+    PyObject* py_flunc; 
+    PyObject* py_h;
+    PyObject* py_rOrb;
+    PyObject* py_rOrbCluster;
+    PyObject* py_linkedOrb_rnorm;
+    PyObject* py_spinFrame;
+    PyObject* py_ignoreNonDiagonalJ;
+    PyObject* callback;  // callback function
+    PyArg_ParseTuple(args,"OOOOOOOOOOOOOOOOOOOOOOO",
+                    &py_algorithm,&py_initSpin,&py_initD,&py_nthermal,&py_nsweep,&py_ninterval,
+                    &py_maxNLinking,&py_nlink,&py_linkStrength,&py_linkedOrb,&py_localCircuits,
+                    &py_corrOrbPair,
+                    &py_nOrbGroup,&py_maxOrbGroupSize,&py_orbGroupList,
+                    &py_flunc,&py_h,
+                    &py_rOrb,&py_rOrbCluster,&py_linkedOrb_rnorm,
+                    &py_spinFrame,&py_ignoreNonDiagonalJ,
+                    &callback);
+
+    int algorithm=(int)PyLong_AsLong(py_algorithm); 
+    //printf("%d\n",algorithm);
+    int nthermal=(int)PyLong_AsLong(py_nthermal);
+    int nsweep=(int)PyLong_AsLong(py_nsweep);
+    int maxNLinking=(int)PyLong_AsLong(py_maxNLinking);
+    int ninterval=(int)PyLong_AsLong(py_ninterval);
+    int spinFrame=(int)PyLong_AsLong(py_spinFrame);
+    int ignoreNonDiagonalJ=(int)PyLong_AsLong(py_ignoreNonDiagonalJ);
+
+    int totOrbs=(int)PyTuple_Size(py_initSpin);
+    double initSpin[totOrbs];
+    for(int iorb=0;iorb<totOrbs;iorb++)initSpin[iorb]=PyFloat_AsDouble(PyTuple_GetItem(py_initSpin,iorb));
+
+    double initD[totOrbs][3];
+    for(int iorb=0;iorb<totOrbs;iorb++)for(int idir=0;idir<3;idir++)
+        initD[iorb][idir]=PyFloat_AsDouble(PyTuple_GetItem(py_initD,iorb*3+idir));
+    
+    
+    int nlink[totOrbs];
+    double linkStrength[totOrbs][maxNLinking][9];
+    int linkedOrb[totOrbs][maxNLinking];
+    for(int iorb=0;iorb<totOrbs;iorb++){
+        nlink[iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_nlink,iorb));
+        for(int ilink=0;ilink<maxNLinking;ilink++){
+            linkedOrb[iorb][ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb,iorb*maxNLinking+ilink));
+            for(int icomp=0;icomp<9;icomp++)
+            linkStrength[iorb][ilink][icomp]=PyFloat_AsDouble(PyTuple_GetItem(py_linkStrength,iorb*maxNLinking*9+ilink*9+icomp));
+        }
+    }
+    //printf("totOrbs=%d s0=%f D0x=%f nther=%d nst=%d tau=%d maxLink=%d link0=%d J0x=%f\n",totOrbs,initSpin[0],initD[0][0],nthermal,nsweep,ninterval,maxNLinking,nlink[0],linkStrength[0][0][0]);
+    //printf("spinFrame: %d only diagonal: %d\n",spinFrame,ignoreNonDiagonalJ);
+    //for(int iorb=0;iorb<nlink[0];iorb++)printf("orb0-orb%d\n",linkedOrb[0][iorb]);
+    
+    int nLocalCircuits=(int)PyTuple_Size(py_localCircuits)/3;
+    int minimalLocalCircuits=1;if(nLocalCircuits>minimalLocalCircuits)minimalLocalCircuits=nLocalCircuits;
+    int localCircuits[minimalLocalCircuits][3];
+    for(int icircuit=0;icircuit<nLocalCircuits;icircuit++)for(int icomp=0;icomp<3;icomp++)
+        localCircuits[icircuit][icomp]=(int)PyLong_AsLong(PyTuple_GetItem(py_localCircuits,icircuit*3+icomp));
+    //printf("num. of local circuit for topo: %d\n",nLocalCircuits);
+
+    int nLat=(int)PyTuple_Size(py_corrOrbPair)/2;
+    int corrOrbPair[nLat][2];
+    for(int ilat=0;ilat<nLat;ilat++){
+        for(int icomp=0;icomp<2;icomp++)
+        corrOrbPair[ilat][icomp]=(int)PyLong_AsLong(PyTuple_GetItem(py_corrOrbPair,ilat*2+icomp));
+        //printf("pair%d orb%d-orb%d\n",ilat,corrOrbPair[ilat][0],corrOrbPair[ilat][1]);
+    }
+    
+    int nOrbGroup=(int)PyLong_AsLong(py_nOrbGroup);
+    int maxOrbGroupSize=(int)PyLong_AsLong(py_maxOrbGroupSize);
+    //printf("nOrbGroup=%d maxOrbGroupSize=%d\n",nOrbGroup,maxOrbGroupSize);
+    int orbGroupList[nOrbGroup][maxOrbGroupSize];
+    for(int iorbGroup=0;iorbGroup<nOrbGroup;iorbGroup++)for(int iorb=0;iorb<maxOrbGroupSize;iorb++)
+        orbGroupList[iorbGroup][iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_orbGroupList,iorbGroup*maxOrbGroupSize+iorb));
+    
+    double flunc = PyFloat_AsDouble(py_flunc);
+    double h = PyFloat_AsDouble(py_h);
+    //printf("flunc=%f h=%f\n",flunc,h);
+
+    int totOrb_rnorm=(int)PyTuple_Size(py_rOrb);
+    int nOrbInCluster=(int)PyTuple_Size(py_rOrbCluster)/totOrb_rnorm;
+    //printf("totOrb renorm=%d grain size=%d\n",totOrb_rnorm,nOrbInCluster);
+    int rOrb[totOrb_rnorm];
+    int rOrbCluster[totOrb_rnorm][nOrbInCluster];
+    int linkedOrb_rnorm[totOrb_rnorm][maxNLinking];
+    for(int iorb=0;iorb<totOrb_rnorm;iorb++){
+        rOrb[iorb]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrb,iorb));
+        for(int iorb_cluster=0;iorb_cluster<nOrbInCluster;iorb_cluster++)
+            rOrbCluster[iorb][iorb_cluster]=(int)PyLong_AsLong(PyTuple_GetItem(py_rOrbCluster,iorb*nOrbInCluster+iorb_cluster));
+        for(int ilink=0;ilink<maxNLinking;ilink++)
+            linkedOrb_rnorm[iorb][ilink]=(int)PyLong_AsLong(PyTuple_GetItem(py_linkedOrb_rnorm,iorb*maxNLinking+ilink));
+    }    
+    
     // set algorithm
     p_mcUpdate=localUpdate;
-    if(algorithm==1) p_mcUpdate=blockUpdate;
+    if (algorithm==1) p_mcUpdate=blockUpdate;
 
-    // set diagonal dot function
+    // set diagonal dot version
     p_diagonalDot=diagonalDot;
     if (ignoreNonDiagonalJ>0) p_diagonalDot=diagonalDot_simple;
-
-    // initialize lattice add one ghost spin for mimicing external field
+    
+    // initialize lattice
     Orb lattice[totOrbs];
     //printf("hello here is C lib\n");
-    establishLattice(lattice, totOrbs, initSpin, initD, flunc, maxNLinking, nlink, linkStrength, h, totOrb_rnorm, nOrbInCluster, rOrb, rOrbCluster);
+    establishLattice(lattice, totOrbs, initSpin, initD, h, flunc, maxNLinking, nlink, linkStrength, totOrb_rnorm, nOrbInCluster, rOrb, rOrbCluster);
     establishLinking(lattice, totOrbs, maxNLinking, nlink, linkedOrb, totOrb_rnorm, rOrb, linkedOrb_rnorm);
 
     // initialize measurement
     double energy=0;
     double *p_energy=&energy;
     for(int i=0;i<totOrbs;i++)*p_energy+=getCorrEnergy(lattice+i);
     *p_energy/=2; // double counting
     for(int i=0;i<totOrbs;i++)*p_energy+=getOnsiteEnergy(lattice+i);
+    //printf("gournd energy=%.3f nLat=%d\n",*p_energy, nLat);
 
     Vec totSpin;
-    totSpin.x=0;totSpin.y=0;
+    totSpin.x=0;totSpin.y=0;totSpin.z=0;
     Vec*p_totSpin=&totSpin;
     for(int i=0;i<totOrbs;i++) plusEqual(p_totSpin, lattice[i].spin);
-    
+
     for(int i=0;i<nthermal*ninterval;i++) (*p_mcUpdate)(totOrbs, lattice, p_energy, p_totSpin); //thermalization
 
+    // printf("start sweeping\n");
     Vec spin_i, spin_i_r;
     Vec spin_j, spin_j_r;
-    spin_i.x=0;spin_i.y=0;spin_i_r.x=0;spin_i_r.y=0;
-    spin_j.x=0;spin_j.y=0;spin_j_r.x=0;spin_j_r.y=0;
+    spin_i.x=0;spin_i.y=0;spin_i.z=0;spin_i_r.x=0;spin_i_r.y=0;spin_i_r.z=0;
+    spin_j.x=0;spin_j.y=0;spin_j.z=0;spin_j_r.x=0;spin_j_r.y=0;spin_j_r.z=0;
     double spin_ij, spin_ij_r;
     spin_ij=0;spin_ij_r=0;
 
     double totEnergy=0, totEnergy_r=0;
     double E2=0, E2_r=0;
     double M=0,M2=0,M4=0;
     double M_tmp=0,MdotM_tmp=0,M_tot=0;
-
+    
     double topological_q=0; // total vortice number
 
     Vec spin_direction;
-    double spin_i_z, spin_j_z, spin_tot_z;
-    double spin_i_h, spin_j_h, spin_tot_h;
+    double spin_i_z, spin_j_z, spin_tot_z; // spin projected to net-spin
+    double spin_i_h, spin_j_h, spin_tot_h; // spin projected to z aixis
     spin_i_z=0;spin_j_z=0;spin_tot_z=0;
     spin_i_h=0;spin_j_h=0;spin_tot_h=0;
 
     // prepare for output spin frame
     int output_per_sweep=nsweep;
     int iFrame=0;
     PyObject *spinFrameData;
@@ -475,81 +647,87 @@
     }
 
     // prepare for orb group statistics
     double spinDotSpinBetweenGroup[(nOrbGroup+1)*(nOrbGroup+1)];
     for(int i=0;i<(nOrbGroup+1)*(nOrbGroup+1);i++) spinDotSpinBetweenGroup[i]=0.0;
     double spin4Order[nOrbGroup+1];
     for(int i=0;i<nOrbGroup+1;i++) spin4Order[i]=0.0;
-
+    
     for(int i=0;i<nsweep;i++){
         for(int j=0;j<ninterval;j++) (*p_mcUpdate)(totOrbs, lattice, p_energy, p_totSpin);
         // record the spin vector field distribution
         if((spinFrame>0) & (i%output_per_sweep==0)){
             PyObject *spinDistribution=PyTuple_New(totOrbs);
             for(int j=0;j<totOrbs;j++){
                 PyObject *spinJVec=PyTuple_New(3);
                 PyTuple_SetItem(spinJVec, 0, PyFloat_FromDouble(lattice[j].spin.x));
                 PyTuple_SetItem(spinJVec, 1, PyFloat_FromDouble(lattice[j].spin.y));
-                PyTuple_SetItem(spinJVec, 2, PyFloat_FromDouble(0));
+                PyTuple_SetItem(spinJVec, 2, PyFloat_FromDouble(lattice[j].spin.z));
                 PyTuple_SetItem(spinDistribution, j, spinJVec);
             }
             PyTuple_SetItem(spinFrameData, iFrame, spinDistribution);
             iFrame+=1;
         }
 
         // find the main axis
         spin_direction.x=p_totSpin->x;
         spin_direction.y=p_totSpin->y;
+        spin_direction.z=p_totSpin->z;
         normalize(&spin_direction);
 
         // spin statistics over space in each frame
         Vec spin_i_avg;
         Vec spin_j_avg;
         spin_i_avg.x=0;
         spin_i_avg.y=0;
+        spin_i_avg.z=0;
         spin_j_avg.x=0;
         spin_j_avg.y=0;
+        spin_j_avg.z=0;
         double spin_ij_avg=0.0;
 
         double spin_i_z_avg, spin_j_z_avg;
         double spin_i_h_avg, spin_j_h_avg;
         spin_i_z_avg=0;spin_j_z_avg=0;
         spin_i_h_avg=0;spin_j_h_avg=0;
         for(int j=0;j<nLat;j++){
             plusEqual(&spin_i_avg, lattice[corrOrbPair[j][0]].spin);
             plusEqual(&spin_j_avg, lattice[corrOrbPair[j][1]].spin);
             spin_ij_avg+=dot(lattice[corrOrbPair[j][0]].spin,lattice[corrOrbPair[j][1]].spin);
-
+            
             // spin along main axis
             spin_i_z_avg+=dot(spin_direction,lattice[corrOrbPair[j][0]].spin);
             spin_j_z_avg+=dot(spin_direction,lattice[corrOrbPair[j][1]].spin);
 
             // spin projected to z axis
-            spin_i_h_avg+=lattice[corrOrbPair[j][0]].spin.x;
-            spin_j_h_avg+=lattice[corrOrbPair[j][1]].spin.x;
-            
+            spin_i_h_avg+=lattice[corrOrbPair[j][0]].spin.z;
+            spin_j_h_avg+=lattice[corrOrbPair[j][1]].spin.z;
         }
 
-        double topological_q_local=0; // xy-model posess no topological charge
-        topological_q+=topological_q_local;
+        double topological_q_local=0;
+        for(int icircuit=0;icircuit<nLocalCircuits;icircuit++){
+            topological_q_local+=calcSignedArea(lattice[localCircuits[icircuit][0]].spin, lattice[localCircuits[icircuit][1]].spin, lattice[localCircuits[icircuit][2]].spin);
+        }
+        topological_q+=topological_q_local/PI/4;
 
         spin_i_z+=spin_i_z_avg/nLat;
         spin_j_z+=spin_j_z_avg/nLat;
         spin_tot_z+=(dot(spin_direction,*p_totSpin)/nLat);
         //if(h<0.00001){// avoid faults time reversal symmetry
         //    spin_i_h+=fabs(spin_i_h_avg)/nLat;
         //    spin_j_h+=fabs(spin_j_h_avg)/nLat;
-        //    spin_tot_h+=fabs(p_totSpin->x/nLat);
+        //    spin_tot_h+=fabs(p_totSpin->z/nLat);
         //}else{
             spin_i_h+=spin_i_h_avg/nLat;
             spin_j_h+=spin_j_h_avg/nLat;
-            spin_tot_h+=p_totSpin->x/nLat;
+            spin_tot_h+=p_totSpin->z/nLat;
         //}
 
-        M=sqrt(dot(spin_i_avg,spin_i_avg))/nLat;
+
+        M=sqrt(dot(*p_totSpin,*p_totSpin))/nLat;
         M2+=M*M;
         M4+=M*M*M*M;
         //calc auto-correlation
         M_tot+=M;
         MdotM_tmp+=M_tmp*M;
         M_tmp=M;
 
@@ -558,23 +736,22 @@
         vabs(&spin_i_avg);
         vabs(&spin_j_avg);
         plusEqual(&spin_i,spin_i_avg);
         plusEqual(&spin_j,spin_j_avg);
         spin_ij+=spin_ij_avg/nLat;
 
         double e_avg=*p_energy/totOrbs;
-        //printf("e_avg=%.5f\n",e_avg);
         totEnergy+=e_avg;
         E2+=e_avg*e_avg;
 
         // *************** statistics on renormalized lattice
         // spin statistics over space in each frame
         Vec spin_i_r_avg, spin_j_r_avg;
-        spin_i_r_avg.x=0;spin_i_r_avg.y=0;
-        spin_j_r_avg.x=0;spin_j_r_avg.y=0;
+        spin_i_r_avg.x=0;spin_i_r_avg.y=0;spin_i_r_avg.z=0;
+        spin_j_r_avg.x=0;spin_j_r_avg.y=0;spin_j_r_avg.z=0;
         int chosed_spin_i=0;
         int chosed_spin_j=0;
         int chosed_spin_ij=0;
         double spin_ij_r_avg=0.0;
         for(int j=0;j<nLat;j++){
             Orb *_orb_i=lattice+corrOrbPair[j][0];
             Orb *_orb_j=lattice+corrOrbPair[j][1];
@@ -611,94 +788,118 @@
         plusEqual(&spin_i_r,spin_i_r_avg);
         plusEqual(&spin_j_r,spin_j_r_avg);
         spin_ij_r+=spin_ij_r_avg/chosed_spin_ij;
 
         // energy statistics
         double e_avg_rnorm=0;
         for(int j=0;j<totOrbs;j++){ // calc. bond energy in renormalized system
-            if(lattice[j].chosen>0) e_avg_rnorm+=getCorrEnergy_rnorm(lattice+j);
+            if(lattice[j].chosen>0) e_avg_rnorm+=getCorrEnergy_rnorm(lattice+j, p_diagonalDot);
         }
         e_avg_rnorm/=2; // double counting
         for(int j=0;j<totOrbs;j++){ // onsite part
             if(lattice[j].chosen>0) e_avg_rnorm+=getOnsiteEnergy(lattice+j);
         }
         e_avg_rnorm/=totOrb_rnorm;
         totEnergy_r+=e_avg_rnorm;
         E2_r+=e_avg_rnorm*e_avg_rnorm;
 
         // orb group statistics
         Vec summedSpinOfGroup[nOrbGroup+1];
         int iOrbGroup, jOrbGroup;
         for(iOrbGroup=0;iOrbGroup<nOrbGroup;iOrbGroup++){
             Vec summedSpin;
-            summedSpin.x=0;summedSpin.y=0;
+            summedSpin.x=0;summedSpin.y=0;summedSpin.z=0;
             int k;
             for(k=0;k<maxOrbGroupSize;k++){
                 if(orbGroupList[iOrbGroup][k]<0) break;
                 plusEqual(&summedSpin,lattice[orbGroupList[iOrbGroup][k]].spin);
             }
             summedSpinOfGroup[iOrbGroup].x=summedSpin.x;
             summedSpinOfGroup[iOrbGroup].y=summedSpin.y;
+            summedSpinOfGroup[iOrbGroup].z=summedSpin.z;
         }
         summedSpinOfGroup[iOrbGroup].x=p_totSpin->x/nLat;
         summedSpinOfGroup[iOrbGroup].y=p_totSpin->y/nLat;
+        summedSpinOfGroup[iOrbGroup].z=p_totSpin->z/nLat;
         //printf("nOrbGroup: %d\n",nOrbGroup);
         for(iOrbGroup=0;iOrbGroup<(nOrbGroup+1);iOrbGroup++){
             for(jOrbGroup=0;jOrbGroup<(nOrbGroup+1);jOrbGroup++){
                 double spin_i_dot_spin_j=dot(summedSpinOfGroup[iOrbGroup],summedSpinOfGroup[jOrbGroup]);
                 spinDotSpinBetweenGroup[iOrbGroup*(nOrbGroup+1)+jOrbGroup]+=spin_i_dot_spin_j;
                 //printf("i=%d, j=%d, spin_i_dot_j=%.6f\n",iOrbGroup,jOrbGroup,spin_i_dot_spin_j);
                 if(iOrbGroup==jOrbGroup) spin4Order[iOrbGroup]+=spin_i_dot_spin_j*spin_i_dot_spin_j;
             }
         }
     }
-    //printf("%.3f %.3f\n",spin_i_r.x,spin_i_r.y);
     double U4=(M2/nsweep)*(M2/nsweep)/(M4/nsweep);
-    double autoCorr=(MdotM_tmp/nsweep-(M_tot/nsweep)*(M_tot/nsweep));
+    double autoCorr=(MdotM_tmp/nsweep-M_tot/nsweep*M_tot/nsweep);
     PyObject *spinDotSpinBetweenGroup_Tuple;
     spinDotSpinBetweenGroup_Tuple=PyTuple_New((nOrbGroup+2)*(nOrbGroup+1));
     for(int iOrbGroup=0;iOrbGroup<(nOrbGroup+1);iOrbGroup++){
         for(int jOrbGroup=0;jOrbGroup<(nOrbGroup+1);jOrbGroup++){
             int index=iOrbGroup*(nOrbGroup+1)+jOrbGroup;
             double result=spinDotSpinBetweenGroup[index]/nsweep;
             PyTuple_SetItem(spinDotSpinBetweenGroup_Tuple, index, PyFloat_FromDouble(result));
         }
     }
     for(int iOrbGroup=0;iOrbGroup<(nOrbGroup+1);iOrbGroup++){
         int index=(nOrbGroup+1)*(nOrbGroup+1)+iOrbGroup;
         double result=spin4Order[iOrbGroup]/nsweep;
         PyTuple_SetItem(spinDotSpinBetweenGroup_Tuple, index, PyFloat_FromDouble(result));
     }
-    if(nOrbGroup==0) spinDotSpinBetweenGroup_Tuple=PyFloat_FromDouble(0);
+    if(nOrbGroup==0){
+        spinDotSpinBetweenGroup_Tuple=PyFloat_FromDouble(0);
+    }
+
     PyObject *Data;
     Data=PyTuple_New(29);
     PyTuple_SetItem(Data, 0, PyFloat_FromDouble(spin_i.x/nsweep));
     PyTuple_SetItem(Data, 1, PyFloat_FromDouble(spin_i.y/nsweep));
-    PyTuple_SetItem(Data, 2, PyFloat_FromDouble(0));
+    PyTuple_SetItem(Data, 2, PyFloat_FromDouble(spin_i.z/nsweep));
     PyTuple_SetItem(Data, 3, PyFloat_FromDouble(spin_j.x/nsweep));
     PyTuple_SetItem(Data, 4, PyFloat_FromDouble(spin_j.y/nsweep));
-    PyTuple_SetItem(Data, 5, PyFloat_FromDouble(0));
+    PyTuple_SetItem(Data, 5, PyFloat_FromDouble(spin_j.z/nsweep));
     PyTuple_SetItem(Data, 6, PyFloat_FromDouble(spin_ij/nsweep));
     PyTuple_SetItem(Data, 7, PyFloat_FromDouble(autoCorr));
     PyTuple_SetItem(Data, 8, PyFloat_FromDouble(totEnergy/nsweep));
     PyTuple_SetItem(Data, 9, PyFloat_FromDouble(E2/nsweep));
     PyTuple_SetItem(Data,10, PyFloat_FromDouble(U4));
     PyTuple_SetItem(Data,11, PyFloat_FromDouble(spin_i_r.x/nsweep));
     PyTuple_SetItem(Data,12, PyFloat_FromDouble(spin_i_r.y/nsweep));
-    PyTuple_SetItem(Data,13, PyFloat_FromDouble(0));
+    PyTuple_SetItem(Data,13, PyFloat_FromDouble(spin_i_r.z/nsweep));
     PyTuple_SetItem(Data,14, PyFloat_FromDouble(spin_j_r.x/nsweep));
     PyTuple_SetItem(Data,15, PyFloat_FromDouble(spin_j_r.y/nsweep));
-    PyTuple_SetItem(Data,16, PyFloat_FromDouble(0));
+    PyTuple_SetItem(Data,16, PyFloat_FromDouble(spin_j_r.z/nsweep));
     PyTuple_SetItem(Data,17, PyFloat_FromDouble(spin_ij_r/nsweep));
     PyTuple_SetItem(Data,18, PyFloat_FromDouble(totEnergy_r/nsweep));
     PyTuple_SetItem(Data,19, PyFloat_FromDouble(E2_r/nsweep));
     PyTuple_SetItem(Data,20, PyFloat_FromDouble(spin_i_z/nsweep));
     PyTuple_SetItem(Data,21, PyFloat_FromDouble(spin_j_z/nsweep));
     PyTuple_SetItem(Data,22, PyFloat_FromDouble(spin_tot_z/nsweep));
     PyTuple_SetItem(Data,23, PyFloat_FromDouble(spin_i_h/nsweep));
     PyTuple_SetItem(Data,24, PyFloat_FromDouble(spin_j_h/nsweep));
     PyTuple_SetItem(Data,25, PyFloat_FromDouble(spin_tot_h/nsweep));
     PyTuple_SetItem(Data,26, PyFloat_FromDouble(topological_q/nsweep));
     PyTuple_SetItem(Data, 27, spinFrameData);
     PyTuple_SetItem(Data, 28, spinDotSpinBetweenGroup_Tuple);
     return Data;
+}
+
+static PyMethodDef module_methods[] = {
+    {"MCMainFunction", MCMainFunction, METH_VARARGS, "the only function in our c lib"},
+    {NULL, NULL, 0, NULL} // neccessary to tell python compiler stop here
+};
+
+static PyModuleDef moduledef = {
+    PyModuleDef_HEAD_INIT,
+    "heisenberglib",
+    "Used to execute the Monte Carlo simulations of Heisenberg model, that is, the O(3) spin model.",
+    -1,
+    module_methods
+};
+
+PyMODINIT_FUNC PyInit_heisenberglib(void) {
+    printf("Initializing heisenberglib...\n");
+    PyObject* m;
+    m= PyModule_Create(&moduledef);
+    return m;
 }
```

### Comparing `mcsolver-3.0.2/mcsolver.egg-info/PKG-INFO` & `mcsolver-3.0.4/mcsolver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 1.2
 Name: mcsolver
-Version: 3.0.2
+Version: 3.0.4
 Summary: A user friendly program to do Monte Carlo sims for magnetic systems
 Home-page: https://github.com/golddoushi/mcsolver
 Author: Liang Liu
 Author-email: liangliu@main.sdu.edu.cn
 License: UNKNOWN
 Description: # mcsolver
         A user friendly and efficient tool implementing Monte Carlo simulations to estimate Curie/Neel temperature
         
         Support multiple ocassions, e.g. standard ferromangetic/anti-ferromagnetic systems, DMI, Kiteav non-diagonal exchange interactions, dipole-dipole long-range couplings, with external fields.
         
+        The newest version is 3, which supports the calculations on topological charges (the number of (anti-)Skyrmions and (anti-)Merons).
+        
         Original version contributor: Dr. Liang Liu* 1.Shenzheng University 2.Shandong University
         Email: liangliu@mail.sdu.edu.cn
         
         You can download the packed .exe (only tested in Windows 10 platform) from the following link. Wish it can find something helpful for you. And if it was used for publication, please cite:
         [1] Magnetic switches via electric field in BN nanoribbons. Applied Surface Science 480(2019)
         
         Link for exe: https://pan.baidu.com/s/1EaDqOOdB7AP9WXrwEIEaxQ
```

### Comparing `mcsolver-3.0.2/mcsolver.egg-info/SOURCES.txt` & `mcsolver-3.0.4/mcsolver.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 setup2.py
 mcsolver/Lattice.py
 mcsolver/WannierKit.py
 mcsolver/__init__.py
 mcsolver/auxiliary.py
 mcsolver/fileio.py
 mcsolver/guiMain.py
+mcsolver/guiPyQt5.py
+mcsolver/guiPyQt5_toolbox.py
 mcsolver/heisenbergLib.c
-mcsolver/heisenberglib.so
 mcsolver/input.py
 mcsolver/interface2swt.py
 mcsolver/isingLib.c
-mcsolver/isinglib.so
 mcsolver/mcMain.py
 mcsolver/toolbox.py
 mcsolver/win.py
 mcsolver/xyLib.c
-mcsolver/xylib.so
 mcsolver.egg-info/PKG-INFO
 mcsolver.egg-info/SOURCES.txt
 mcsolver.egg-info/dependency_links.txt
 mcsolver.egg-info/requires.txt
 mcsolver.egg-info/top_level.txt
 test/test.py
```

### Comparing `mcsolver-3.0.2/setup2.py` & `mcsolver-3.0.4/setup2.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mcsolver",
-    version="3.0.2",
+    version="3.0.4",
     author="Liang Liu",
     author_email="liangliu@main.sdu.edu.cn",
     description="A user friendly program to do Monte Carlo sims for magnetic systems",
     long_description=long_description,
     python_requires='>=3.7',
     install_requires = ['matplotlib','numpy'],
     url="https://github.com/golddoushi/mcsolver",
     packages=["mcsolver"],
-    package_data={'mcsolver': ['./*.so']},
-    include_package_data=True,
+    #package_data={'mcsolver': ['./*.so']},
+    #include_package_data=True,
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Development Status :: 4 - Beta",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Scientific/Engineering :: Visualization",
```

