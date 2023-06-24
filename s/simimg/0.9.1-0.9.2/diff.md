# Comparing `tmp/simimg-0.9.1.tar.gz` & `tmp/simimg-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simimg-0.9.1.tar", last modified: Sun Sep 27 11:23:07 2020, max compression
+gzip compressed data, was "simimg-0.9.2.tar", last modified: Sat Jun 24 03:36:48 2023, max compression
```

## Comparing `simimg-0.9.1.tar` & `simimg-0.9.2.tar`

### file list

```diff
@@ -1,55 +1,36 @@
-drwxr-xr-x   0 sacha     (1000) sacha     (1000)        0 2020-09-27 11:23:07.600960 simimg-0.9.1/
--rw-r--r--   0 sacha     (1000) sacha     (1000)       75 2019-12-19 11:53:59.000000 simimg-0.9.1/MANIFEST.in
--rw-r--r--   0 sacha     (1000) sacha     (1000)     3659 2020-09-27 11:22:31.000000 simimg-0.9.1/NEWS
--rw-r--r--   0 sacha     (1000) sacha     (1000)    12420 2020-09-27 11:23:07.600960 simimg-0.9.1/PKG-INFO
--rw-r--r--   0 sacha     (1000) sacha     (1000)    10016 2020-01-23 15:31:52.000000 simimg-0.9.1/README.md
--rw-r--r--   0 sacha     (1000) sacha     (1000)        7 2019-12-30 15:35:14.000000 simimg-0.9.1/requirements.txt
--rw-r--r--   0 sacha     (1000) sacha     (1000)       38 2020-09-27 11:23:07.600960 simimg-0.9.1/setup.cfg
--rw-r--r--   0 sacha     (1000) sacha     (1000)      777 2020-09-27 11:22:42.000000 simimg-0.9.1/setup.py
-drwxr-xr-x   0 sacha     (1000) sacha     (1000)        0 2020-09-27 11:23:07.590960 simimg-0.9.1/simimg/
--rw-r--r--   0 sacha     (1000) sacha     (1000)        0 2019-12-16 11:58:18.000000 simimg-0.9.1/simimg/__init__.py
-drwxr-xr-x   0 sacha     (1000) sacha     (1000)        0 2020-09-27 11:23:07.590960 simimg-0.9.1/simimg/classes/
--rw-r--r--   0 sacha     (1000) sacha     (1000)        0 2019-12-16 11:58:20.000000 simimg-0.9.1/simimg/classes/__init__.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)    12594 2020-09-27 09:47:17.000000 simimg-0.9.1/simimg/classes/conditionmodules.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     6198 2020-09-27 11:07:08.000000 simimg-0.9.1/simimg/classes/configuration.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)    23115 2020-09-27 10:49:11.000000 simimg-0.9.1/simimg/classes/controller.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     3216 2020-01-10 16:53:24.000000 simimg-0.9.1/simimg/classes/customscales.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     4353 2020-01-19 21:06:23.000000 simimg-0.9.1/simimg/classes/fileobject.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     4317 2020-09-27 11:11:55.000000 simimg-0.9.1/simimg/classes/imageframe.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     5429 2020-09-27 11:07:33.000000 simimg-0.9.1/simimg/classes/miscmodules.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     1711 2020-01-07 09:17:43.000000 simimg-0.9.1/simimg/classes/scrollframe.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     4100 2020-01-10 15:37:56.000000 simimg-0.9.1/simimg/classes/toolbar.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     3753 2020-01-07 09:17:00.000000 simimg-0.9.1/simimg/classes/tooltip.py
-drwxr-xr-x   0 sacha     (1000) sacha     (1000)        0 2020-09-27 11:23:07.590960 simimg-0.9.1/simimg/dialogs/
--rw-r--r--   0 sacha     (1000) sacha     (1000)        0 2019-12-16 11:58:23.000000 simimg-0.9.1/simimg/dialogs/__init__.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     6559 2020-09-27 11:19:38.000000 simimg-0.9.1/simimg/dialogs/configurationwindow.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     2059 2020-01-07 10:45:47.000000 simimg-0.9.1/simimg/dialogs/confirmdeletedialog.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     1001 2020-01-06 16:38:53.000000 simimg-0.9.1/simimg/dialogs/infowindow.py
--rw-rw-r--   0 sacha     (1000) sacha     (1000)     8529 2020-01-13 14:31:05.000000 simimg-0.9.1/simimg/dialogs/viewer.py
-drwxr-xr-x   0 sacha     (1000) sacha     (1000)        0 2020-09-27 11:23:07.600960 simimg-0.9.1/simimg/icons/
--rw-r--r--   0 sacha     (1000) sacha     (1000)     1033 2020-01-08 17:34:56.000000 simimg-0.9.1/simimg/icons/add.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)      730 2020-01-08 17:34:56.000000 simimg-0.9.1/simimg/icons/delete.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)     1123 2020-01-08 17:34:56.000000 simimg-0.9.1/simimg/icons/exit.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)      203 2020-01-08 17:34:56.000000 simimg-0.9.1/simimg/icons/hide.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)     1399 2020-01-08 17:34:57.000000 simimg-0.9.1/simimg/icons/info.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)      910 2020-01-10 17:05:19.000000 simimg-0.9.1/simimg/icons/move.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)      878 2020-01-08 17:34:57.000000 simimg-0.9.1/simimg/icons/open.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)      359 2020-01-08 17:34:57.000000 simimg-0.9.1/simimg/icons/play.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)     1360 2020-01-08 17:34:57.000000 simimg-0.9.1/simimg/icons/refresh.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)     1483 2020-01-08 17:34:57.000000 simimg-0.9.1/simimg/icons/settings.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)     4584 2020-01-08 17:34:57.000000 simimg-0.9.1/simimg/icons/simimg.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)      579 2020-01-08 17:34:57.000000 simimg-0.9.1/simimg/icons/uncheck.png
--rw-r--r--   0 sacha     (1000) sacha     (1000)     2657 2020-07-10 17:14:22.000000 simimg-0.9.1/simimg/simimg.py
-drwxr-xr-x   0 sacha     (1000) sacha     (1000)        0 2020-09-27 11:23:07.600960 simimg-0.9.1/simimg/utils/
--rw-r--r--   0 sacha     (1000) sacha     (1000)        0 2019-12-16 11:58:25.000000 simimg-0.9.1/simimg/utils/__init__.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     3331 2020-01-07 17:20:22.000000 simimg-0.9.1/simimg/utils/database.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     4338 2020-01-08 16:18:49.000000 simimg-0.9.1/simimg/utils/handyfunctions.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     2839 2020-09-27 10:39:18.000000 simimg-0.9.1/simimg/utils/pillowplus.py
--rw-r--r--   0 sacha     (1000) sacha     (1000)     7140 2020-09-27 10:38:55.000000 simimg-0.9.1/simimg/utils/pooling.py
-drwxr-xr-x   0 sacha     (1000) sacha     (1000)        0 2020-09-27 11:23:07.590960 simimg-0.9.1/simimg.egg-info/
--rw-r--r--   0 sacha     (1000) sacha     (1000)    12420 2020-09-27 11:23:07.000000 simimg-0.9.1/simimg.egg-info/PKG-INFO
--rw-r--r--   0 sacha     (1000) sacha     (1000)     1160 2020-09-27 11:23:07.000000 simimg-0.9.1/simimg.egg-info/SOURCES.txt
--rw-r--r--   0 sacha     (1000) sacha     (1000)        1 2020-09-27 11:23:07.000000 simimg-0.9.1/simimg.egg-info/dependency_links.txt
--rw-r--r--   0 sacha     (1000) sacha     (1000)       47 2020-09-27 11:23:07.000000 simimg-0.9.1/simimg.egg-info/entry_points.txt
--rw-r--r--   0 sacha     (1000) sacha     (1000)        7 2020-09-27 11:23:07.000000 simimg-0.9.1/simimg.egg-info/requires.txt
--rw-r--r--   0 sacha     (1000) sacha     (1000)        7 2020-09-27 11:23:07.000000 simimg-0.9.1/simimg.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1062 2019-10-29 11:23:49.009061 simimg-0.9.2/LICENSE
+-rw-r--r--   0        0        0    10016 2020-01-23 15:31:52.212619 simimg-0.9.2/README.md
+-rw-r--r--   0        0        0      671 2023-06-24 03:36:48.491162 simimg-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-18 06:17:23.000000 simimg-0.9.2/simimg/__init__.py
+-rw-r--r--   0        0        0    12712 2023-03-18 21:50:03.675182 simimg-0.9.2/simimg/classes/conditionmodules.py
+-rw-r--r--   0        0        0     6196 2023-03-18 21:27:34.944551 simimg-0.9.2/simimg/classes/configuration.py
+-rw-r--r--   0        0        0    23234 2023-04-30 05:26:08.894944 simimg-0.9.2/simimg/classes/controller.py
+-rw-r--r--   0        0        0     3203 2023-03-18 21:29:28.487855 simimg-0.9.2/simimg/classes/customscales.py
+-rw-r--r--   0        0        0     3812 2023-03-19 04:54:05.914206 simimg-0.9.2/simimg/classes/fileobject.py
+-rw-r--r--   0        0        0     4317 2023-03-18 22:08:28.487149 simimg-0.9.2/simimg/classes/imageframe.py
+-rw-r--r--   0        0        0     5430 2023-03-18 21:11:46.859036 simimg-0.9.2/simimg/classes/miscmodules.py
+-rw-r--r--   0        0        0     1707 2023-03-18 21:19:05.210193 simimg-0.9.2/simimg/classes/scrollframe.py
+-rw-r--r--   0        0        0     4109 2023-03-18 21:12:17.780117 simimg-0.9.2/simimg/classes/toolbar.py
+-rw-r--r--   0        0        0     3644 2023-03-18 21:23:52.497956 simimg-0.9.2/simimg/classes/tooltip.py
+-rw-r--r--   0        0        0     6560 2023-03-18 21:11:42.556024 simimg-0.9.2/simimg/dialogs/configurationwindow.py
+-rw-r--r--   0        0        0     2059 2023-03-18 21:11:28.162986 simimg-0.9.2/simimg/dialogs/confirmdeletedialog.py
+-rw-r--r--   0        0        0     1001 2023-03-18 21:11:32.179997 simimg-0.9.2/simimg/dialogs/infowindow.py
+-rw-r--r--   0        0        0     8550 2023-03-18 21:18:02.123027 simimg-0.9.2/simimg/dialogs/viewer.py
+-rw-r--r--   0        0        0     1033 2020-01-08 17:34:56.000000 simimg-0.9.2/simimg/icons/add.png
+-rw-r--r--   0        0        0      730 2020-01-08 17:34:56.000000 simimg-0.9.2/simimg/icons/delete.png
+-rw-r--r--   0        0        0     1123 2020-01-08 17:34:56.000000 simimg-0.9.2/simimg/icons/exit.png
+-rw-r--r--   0        0        0      203 2020-01-08 17:34:56.000000 simimg-0.9.2/simimg/icons/hide.png
+-rw-r--r--   0        0        0     1399 2020-01-08 17:34:57.000000 simimg-0.9.2/simimg/icons/info.png
+-rw-r--r--   0        0        0      910 2020-01-10 17:05:19.000000 simimg-0.9.2/simimg/icons/move.png
+-rw-r--r--   0        0        0      878 2020-01-08 17:34:57.000000 simimg-0.9.2/simimg/icons/open.png
+-rw-r--r--   0        0        0      359 2020-01-08 17:34:57.000000 simimg-0.9.2/simimg/icons/play.png
+-rw-r--r--   0        0        0     1360 2020-01-08 17:34:57.000000 simimg-0.9.2/simimg/icons/refresh.png
+-rw-r--r--   0        0        0     1483 2020-01-08 17:34:57.000000 simimg-0.9.2/simimg/icons/settings.png
+-rw-r--r--   0        0        0     4584 2020-01-08 17:34:57.000000 simimg-0.9.2/simimg/icons/simimg.png
+-rw-r--r--   0        0        0      579 2020-01-08 17:34:57.000000 simimg-0.9.2/simimg/icons/uncheck.png
+-rw-r--r--   0        0        0     2675 2023-03-18 07:01:14.000000 simimg-0.9.2/simimg/simimg.py
+-rw-r--r--   0        0        0     2412 2023-03-18 21:16:56.578854 simimg-0.9.2/simimg/utils/database.py
+-rw-r--r--   0        0        0     4249 2023-03-18 21:15:07.682566 simimg-0.9.2/simimg/utils/handyfunctions.py
+-rw-r--r--   0        0        0     2829 2023-03-18 21:59:51.977769 simimg-0.9.2/simimg/utils/pillowplus.py
+-rw-r--r--   0        0        0     7165 2023-03-18 21:31:41.952212 simimg-0.9.2/simimg/utils/pooling.py
+-rw-r--r--   0        0        0    10474 1970-01-01 00:00:00.000000 simimg-0.9.2/PKG-INFO
```

### Comparing `simimg-0.9.1/PKG-INFO` & `simimg-0.9.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,261 +1,246 @@
-Metadata-Version: 2.1
-Name: simimg
-Version: 0.9.1
-Summary: Similar Image Finder
-Home-page: https://github.com/zazaho/SimImg
-Author: Sacha Hony
-Author-email: zazahohonini@gmail.com
-License: UNKNOWN
-Description: # Similar Image Finder (Simimg)
-        ![Simimg in action](doc/demo.gif)
-        
-        # Description
-        This is a python GUI for displaying pictures grouped according to
-        similarity. The main aim of the program is to help identify groups of
-        holiday snaps that resemble each-other and efficiently inspect those
-        groups. It allows you to easily keep only the best photos.
-        
-        The program is **not** designed to identify the same but modified pictures
-        (recompressed jpgs, cropped images or adapted colours, etc.). Although
-        it can be used for this there are many and better solutions available.
-        
-        Upon starting Simimg from the command line, by default it will load
-        the pictures it finds in the startup directory and sub-directories
-        into the GUI. These are settings that can be changed within the GUI by
-        clicking on settings (![](simimg/icons/settings.png)). *In particular
-        in the case you want to use the program by clicking on its icon, you
-        may want to set an empty startup directory.*
-        
-        You can play with different filters that take into account how similar
-        two pictures are. These are the panels in the left section of the
-        finder window below the **Filters** title. You can activate a
-        filter by clicking on its name. The following options exist:
-        
-        * I have implemented measurements of how similar the colours are
-        between two images, as well as between 5 regions (the four corners and
-        the central part). The measurement in HSV (hue-saturation-value)
-        supposedly reflects best how humans perceive image information.
-        
-        * Some gradient metrics adapted from ImageHash (dhash). Basically
-        these measure whether two images have similar patterns of brighter and
-        darker regions.
-        
-        * You can further select the maximum allowed time-span between the
-        moments the pictures were taken in order to be considered a match.
-        
-        * You can match on camera model. This means that two pictures are
-        considered to be a match if they were taken with the same camera.
-          
-        * Finally you can match on image shape. You can choose:
-        
-        	* portrait/landscape: width smaller/larger or equal to height
-        
-        	* exact: width/height are identical
-        
-        	* some percentage difference allowed
-        
-        Some of the selection criteria have additional parameters that you can
-        play with.
-        
-        Each filter has a **Must Match** checkbox. If this is switched on,
-        only those pairs that satisfy this filter are considered matches.
-        Note that:
-        
-        1) **Must Match** has no effect if only one filter is active.
-        
-        2) If some filter(s) have **Must Match** set, other filters without
-        **Must Match** have no effect.
-        
-        3) When multiple filters are active and no **Must Match** is set,
-        two images are considered a matching pair if any of the conditions is
-        satisfied.
-        
-        The actual use is to be able to better drill down the list. For
-        example it allows to show only those groups that have similar colours
-        **and** are taken with the same camera by switching on **Must Match** for
-        both filters.
-        
-        # What matching groups are shown?
-        When the program starts, there are no active filters and thumbnails
-        of all files are shown in a grid sorted by filename.
-        
-        Once some filters are activated or changed the display will be
-        updated.
-        
-        For each picture that has some matches in the collection, the group
-        of matching thumbnails will be shown in a row. The only exception is a
-        group that is already displayed in its entirety as a
-        subgroup on another line.
-        
-        Simimg does its best to maintain the sorting order of the displayed
-        files according to filename. This is chosen for two reasons. 
-        
-        1) It limits the visual changes when modifying parameters or filters.
-        This helps to understand the impact of the modification.
-        
-        2) Many times the filename of holiday pictures represents a natural
-        sorting order; for example the serial photo-number or a prefix chosen
-        to indicate where a picture was taken. Maintaining this order, means
-        related pictures have more chance of being presented close together.
-        
-        Note that completely identical files (exact copies of some image file)
-        will not be shown twice. Instead one thumbnail will be shown with a
-        green border around it.
-        
-        # Available functions
-        ## Thumbnail buttons
-        You can click on the **Hide**, **Move** or **Delete** button below
-        each image.
-        
-        * **Hide** will remove the thumbnail from the display but it will not delete
-        the file from your hard-disk.
-        
-        * **Delete** will remove the file from the display and from your
-        hard-disk.
-        
-        * **Move** will Move the file to the folder selected in the move list
-        on the bottom left. See below.
-        
-        ## (De)selecting thumbnails
-        You can select a thumbnail by clicking on it; its background will turn
-        blue to indicate that it is selected.
-        
-        Pressing the Control (Ctrl) key while clicking will select or deselect
-        the entire line of thumbnails.
-        
-        Pressing the Shift key while clicking will select all thumbnails between
-        the current image and the last selected image.
-        
-        Clicking in an empty part of the thumbnail display area deselects all
-        images.
-        
-        The little red check-mark button  (![](simimg/icons/uncheck.png)) in the toolbar area
-        (top-left) also switches between select-all and unselect-all thumbnails.
-        
-        Pressing Ctrl+a toggles between selecting and unselecting all thumbnails.
-        
-        ## Actions for selected thumbnails
-        The *Play* button (![](simimg/icons/play.png))  in the toolbar will show a window that allows
-        to view the selected images in larger versions (Ctrl+v).
-        
-        The *Minus* button (![](simimg/icons/hide.png)) will hide all selected thumbnails (Ctrl+h)
-        
-        The *Red-X* button (![](simimg/icons/delete.png)) will delete all selected thumbnails (Ctrl+d)
-        
-        The *Two folder* button (![](simimg/icons/move.png)) will move the selected thumbnails (Ctrl+m)
-        
-        ## Photo organisation functions
-        Because the Finder window is also a great way to get an overview, even
-        without using the filtering functions, I have implemented a very basic
-        organisation option into it. These are represented by the *Move*
-        folders.
-        
-        Imagine you have 2 folders defined: "WebAlbum", "EditWithGimp". You
-        peruse you photos, select and delete those that are poor, you select
-        those that are nice but either need better framing or need playing a
-        bit with the brightness. Activate the "EditWithGimp" folder and press
-        *Move* button (![](simimg/icons/move.png)). Next, you have found a
-        number of great pictures that you want to publish. Select those,
-        activate the "WebAlbum" target and press *Move*.
-        
-        ## Actions in the viewer window
-        One design goal is a clean interface with a lot of room for the
-        pictures themselves. Therefore there are no action buttons in the
-        viewer.
-        
-        The follow actions are available in the viewer window:
-        
-        * F1 or i: show a short help window
-        
-        * left mouse button, arrow-right or n: show the next picture
-        
-        * right mouse button, arrow left or p: show the previous picture
-        
-        * scrollwheel: zoom-in on part of the picture
-        
-        * delete or d: delete the picture from disk
-        
-        * m: move the file to the move-target directory selected in the finder
-          window
-        
-        * 1: move the file to the **first** move-target directory
-        
-        * 2: move the file to the **second** move-target directory
-        
-        * 3: move the file to the **third** move-target directory
-        
-        * escape or q: quit the viewer
-        
-        ## Tips
-        There are a few features that are not immediately obvious. *Camera
-        Model* and *Picture Shape* can be set to "different". By themselves
-        these options are not useful because they will show unrelated pictures
-        together. They can become interesting in the following scenario:
-        
-        Several people have taken pictures of the same scene, you select
-        pictures taken close in time or with similar colours. If you impose
-        different *Camera Model* you can concentrate on similar pictures but
-        taken by different people.
-        
-        The Folder select dialog for **move** does not allow to create folders
-        on some platforms. Selecting the parent directoy and adding (by
-        typing) the target folder you would like to create before pressing OK
-        will create the directory.
-        
-        ## Technical remarks
-        I have seen quite a variety of 'success', meaning that some algorithm
-        detects matches that I myself would also call a match. It depends a
-        lot on the set of images that one uses as input. I find it useful to
-        play around a bit with selecting different algorithms and playing with
-        the numerical limits. To help with this, the tooltip of the limit
-        selectors will tell you at which value the first match happens and at
-        which value more than 10 matches are found. 
-        
-        In my experience, for the purpose of detecting the most interesting
-        similar holiday pictures the "Gradient (horizontal)" algorithm can be
-        useful but the "HSV (5 regions)" in the Colours Distance gives the
-        best results.
-        
-        The other filters should be considered optional to further limit the
-        shown matches.
-        
-        Some of the calculations can be time-consuming and Simimg tries to be
-        clever about not recalculating. It will store the calculated values in
-        a database for future use. It recognises the pictures files by their
-        MD5-hash which means that even if you move files or rename them, their
-        image properties will not be recalculated.
-        
-        It attempts to do the most expensive calculations in parallel making
-        optimal use of your computers capabilities.
-        
-        Note that, for reasons of speed, the maximum number of thumbnails that
-        will be shown will not exceed about 300.
-        
-        Note that, for reasons of speed and memory, the maximum number of
-        files that will be loaded when adding a folder is 900.
-        
-        # Credit
-        This project uses the following open source packages:
-        
-        * [Python](https://www.python.org/): version 3
-        
-        * [tkinter](https://docs.python.org/3/library/tkinter.html) that
-        should normally come with your python
-        
-        * [pillow](https://python-pillow.org/) for image reading and processing.
-        
-        * The tooltip code is adapted from an example found on
-          [Daniweb](https://www.daniweb.com/programming/software-development/code/484591/a-tooltip-class-for-tkinter).
-          
-        Some of the algorithms used have been inspired by code found at
-        [imagedupes](https://github.com/ghemsley/imagedupes), 
-        [pyimagesearch](https://www.pyimagesearch.com/2014/12/01/complete-guide-building-image-search-engine-python-opencv/)
-        and [imageHash](https://github.com/JohannesBuchner/imagehash).
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
+# Similar Image Finder (Simimg)
+![Simimg in action](doc/demo.gif)
+
+# Description
+This is a python GUI for displaying pictures grouped according to
+similarity. The main aim of the program is to help identify groups of
+holiday snaps that resemble each-other and efficiently inspect those
+groups. It allows you to easily keep only the best photos.
+
+The program is **not** designed to identify the same but modified pictures
+(recompressed jpgs, cropped images or adapted colours, etc.). Although
+it can be used for this there are many and better solutions available.
+
+Upon starting Simimg from the command line, by default it will load
+the pictures it finds in the startup directory and sub-directories
+into the GUI. These are settings that can be changed within the GUI by
+clicking on settings (![](simimg/icons/settings.png)). *In particular
+in the case you want to use the program by clicking on its icon, you
+may want to set an empty startup directory.*
+
+You can play with different filters that take into account how similar
+two pictures are. These are the panels in the left section of the
+finder window below the **Filters** title. You can activate a
+filter by clicking on its name. The following options exist:
+
+* I have implemented measurements of how similar the colours are
+between two images, as well as between 5 regions (the four corners and
+the central part). The measurement in HSV (hue-saturation-value)
+supposedly reflects best how humans perceive image information.
+
+* Some gradient metrics adapted from ImageHash (dhash). Basically
+these measure whether two images have similar patterns of brighter and
+darker regions.
+
+* You can further select the maximum allowed time-span between the
+moments the pictures were taken in order to be considered a match.
+
+* You can match on camera model. This means that two pictures are
+considered to be a match if they were taken with the same camera.
+  
+* Finally you can match on image shape. You can choose:
+
+	* portrait/landscape: width smaller/larger or equal to height
+
+	* exact: width/height are identical
+
+	* some percentage difference allowed
+
+Some of the selection criteria have additional parameters that you can
+play with.
+
+Each filter has a **Must Match** checkbox. If this is switched on,
+only those pairs that satisfy this filter are considered matches.
+Note that:
+
+1) **Must Match** has no effect if only one filter is active.
+
+2) If some filter(s) have **Must Match** set, other filters without
+**Must Match** have no effect.
+
+3) When multiple filters are active and no **Must Match** is set,
+two images are considered a matching pair if any of the conditions is
+satisfied.
+
+The actual use is to be able to better drill down the list. For
+example it allows to show only those groups that have similar colours
+**and** are taken with the same camera by switching on **Must Match** for
+both filters.
+
+# What matching groups are shown?
+When the program starts, there are no active filters and thumbnails
+of all files are shown in a grid sorted by filename.
+
+Once some filters are activated or changed the display will be
+updated.
+
+For each picture that has some matches in the collection, the group
+of matching thumbnails will be shown in a row. The only exception is a
+group that is already displayed in its entirety as a
+subgroup on another line.
+
+Simimg does its best to maintain the sorting order of the displayed
+files according to filename. This is chosen for two reasons. 
+
+1) It limits the visual changes when modifying parameters or filters.
+This helps to understand the impact of the modification.
+
+2) Many times the filename of holiday pictures represents a natural
+sorting order; for example the serial photo-number or a prefix chosen
+to indicate where a picture was taken. Maintaining this order, means
+related pictures have more chance of being presented close together.
+
+Note that completely identical files (exact copies of some image file)
+will not be shown twice. Instead one thumbnail will be shown with a
+green border around it.
+
+# Available functions
+## Thumbnail buttons
+You can click on the **Hide**, **Move** or **Delete** button below
+each image.
+
+* **Hide** will remove the thumbnail from the display but it will not delete
+the file from your hard-disk.
+
+* **Delete** will remove the file from the display and from your
+hard-disk.
+
+* **Move** will Move the file to the folder selected in the move list
+on the bottom left. See below.
+
+## (De)selecting thumbnails
+You can select a thumbnail by clicking on it; its background will turn
+blue to indicate that it is selected.
+
+Pressing the Control (Ctrl) key while clicking will select or deselect
+the entire line of thumbnails.
+
+Pressing the Shift key while clicking will select all thumbnails between
+the current image and the last selected image.
+
+Clicking in an empty part of the thumbnail display area deselects all
+images.
+
+The little red check-mark button  (![](simimg/icons/uncheck.png)) in the toolbar area
+(top-left) also switches between select-all and unselect-all thumbnails.
+
+Pressing Ctrl+a toggles between selecting and unselecting all thumbnails.
+
+## Actions for selected thumbnails
+The *Play* button (![](simimg/icons/play.png))  in the toolbar will show a window that allows
+to view the selected images in larger versions (Ctrl+v).
+
+The *Minus* button (![](simimg/icons/hide.png)) will hide all selected thumbnails (Ctrl+h)
+
+The *Red-X* button (![](simimg/icons/delete.png)) will delete all selected thumbnails (Ctrl+d)
+
+The *Two folder* button (![](simimg/icons/move.png)) will move the selected thumbnails (Ctrl+m)
+
+## Photo organisation functions
+Because the Finder window is also a great way to get an overview, even
+without using the filtering functions, I have implemented a very basic
+organisation option into it. These are represented by the *Move*
+folders.
+
+Imagine you have 2 folders defined: "WebAlbum", "EditWithGimp". You
+peruse you photos, select and delete those that are poor, you select
+those that are nice but either need better framing or need playing a
+bit with the brightness. Activate the "EditWithGimp" folder and press
+*Move* button (![](simimg/icons/move.png)). Next, you have found a
+number of great pictures that you want to publish. Select those,
+activate the "WebAlbum" target and press *Move*.
+
+## Actions in the viewer window
+One design goal is a clean interface with a lot of room for the
+pictures themselves. Therefore there are no action buttons in the
+viewer.
+
+The follow actions are available in the viewer window:
+
+* F1 or i: show a short help window
+
+* left mouse button, arrow-right or n: show the next picture
+
+* right mouse button, arrow left or p: show the previous picture
+
+* scrollwheel: zoom-in on part of the picture
+
+* delete or d: delete the picture from disk
+
+* m: move the file to the move-target directory selected in the finder
+  window
+
+* 1: move the file to the **first** move-target directory
+
+* 2: move the file to the **second** move-target directory
+
+* 3: move the file to the **third** move-target directory
+
+* escape or q: quit the viewer
+
+## Tips
+There are a few features that are not immediately obvious. *Camera
+Model* and *Picture Shape* can be set to "different". By themselves
+these options are not useful because they will show unrelated pictures
+together. They can become interesting in the following scenario:
+
+Several people have taken pictures of the same scene, you select
+pictures taken close in time or with similar colours. If you impose
+different *Camera Model* you can concentrate on similar pictures but
+taken by different people.
+
+The Folder select dialog for **move** does not allow to create folders
+on some platforms. Selecting the parent directoy and adding (by
+typing) the target folder you would like to create before pressing OK
+will create the directory.
+
+## Technical remarks
+I have seen quite a variety of 'success', meaning that some algorithm
+detects matches that I myself would also call a match. It depends a
+lot on the set of images that one uses as input. I find it useful to
+play around a bit with selecting different algorithms and playing with
+the numerical limits. To help with this, the tooltip of the limit
+selectors will tell you at which value the first match happens and at
+which value more than 10 matches are found. 
+
+In my experience, for the purpose of detecting the most interesting
+similar holiday pictures the "Gradient (horizontal)" algorithm can be
+useful but the "HSV (5 regions)" in the Colours Distance gives the
+best results.
+
+The other filters should be considered optional to further limit the
+shown matches.
+
+Some of the calculations can be time-consuming and Simimg tries to be
+clever about not recalculating. It will store the calculated values in
+a database for future use. It recognises the pictures files by their
+MD5-hash which means that even if you move files or rename them, their
+image properties will not be recalculated.
+
+It attempts to do the most expensive calculations in parallel making
+optimal use of your computers capabilities.
+
+Note that, for reasons of speed, the maximum number of thumbnails that
+will be shown will not exceed about 300.
+
+Note that, for reasons of speed and memory, the maximum number of
+files that will be loaded when adding a folder is 900.
+
+# Credit
+This project uses the following open source packages:
+
+* [Python](https://www.python.org/): version 3
+
+* [tkinter](https://docs.python.org/3/library/tkinter.html) that
+should normally come with your python
+
+* [pillow](https://python-pillow.org/) for image reading and processing.
+
+* The tooltip code is adapted from an example found on
+  [Daniweb](https://www.daniweb.com/programming/software-development/code/484591/a-tooltip-class-for-tkinter).
+  
+Some of the algorithms used have been inspired by code found at
+[imagedupes](https://github.com/ghemsley/imagedupes), 
+[pyimagesearch](https://www.pyimagesearch.com/2014/12/01/complete-guide-building-image-search-engine-python-opencv/)
+and [imageHash](https://github.com/JohannesBuchner/imagehash).
+
```

### Comparing `simimg-0.9.1/README.md` & `simimg-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: simimg
+Version: 0.9.2
+Summary: Similar Image Finder
+Author-Email: sacha <sachahony@gmail.com>, Sacha Hony <zazahohonini@gmail.com>
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Project-URL: Homepage, https://github.com/zazaho/SimImg
+Requires-Python: >=3
+Requires-Dist: Pillow
+Description-Content-Type: text/markdown
+
 # Similar Image Finder (Simimg)
 ![Simimg in action](doc/demo.gif)
 
 # Description
 This is a python GUI for displaying pictures grouped according to
 similarity. The main aim of the program is to help identify groups of
 holiday snaps that resemble each-other and efficiently inspect those
```

### Comparing `simimg-0.9.1/simimg/classes/conditionmodules.py` & `simimg-0.9.2/simimg/classes/conditionmodules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,112 +1,116 @@
-''' Classes that implement different criteria for selecting matching images.
+""" Classes that implement different criteria for selecting matching images.
     It should have at least:
     A name label
     A active switch (click on the name label)
     A switch to make this criterion obligatory (must match)
     A method to do something when _somethingChanged
     A method to determine which imagepairs from a list of pairs match
-'''
-import math
-from operator import add
-import itertools
+"""
 import functools
+import itertools
+import math
 import tkinter as tk
+from operator import add
 from tkinter import ttk
-from . import customscales as CS
-from . import tooltip as TT
+
+import simimg.classes.customscales as CS
+import simimg.classes.tooltip as TT
+
 
 class ConditionModule(ttk.Frame):
-    'A frame that holds one selection criterion with options'
-    name = ''
-    _conditionName = ''
+    "A frame that holds one selection criterion with options"
+    name = ""
+    _conditionName = ""
     _currentConfig = {}
 
     def __init__(self, parent, Controller=None):
         super().__init__(parent)
 
-        self.config(borderwidth=1, relief='sunken')
+        self.config(borderwidth=1, relief="sunken")
 
         # keep a handle of the controller object
         self._Ctrl = Controller
         self.active = False
         self.mustMatch = tk.BooleanVar()
 
         self._currentMatchingGroups = {}
         self._matchingInfo = []
         self._checksums = {}
 
         header_frame = ttk.Frame(self)
-        header_frame.pack(fill='x')
+        header_frame.pack(fill="x")
 
         self._label = ttk.Label(header_frame, text=self._conditionName)
-        self._label.bind('<Button-1>', self._activeToggled)
-        self._label.pack(side='left', fill='x')
+        self._label.bind("<Button-1>", self._activeToggled)
+        self._label.pack(side="left", fill="x")
 
-        self._fold_button = ttk.Label(header_frame, text='^')
-        self._fold_button.bind('<Button-1>', self.toggleFolding)
-        self._fold_button.pack(side='right', fill='x')
+        self._fold_button = ttk.Label(header_frame, text="^")
+        self._fold_button.bind("<Button-1>", self.toggleFolding)
+        self._fold_button.pack(side="right", fill="x")
         self.is_folded = False
 
         self._options_frame = ttk.Frame(self)
-        self._options_frame.pack(fill='x')
+        self._options_frame.pack(fill="x")
         self._mustMatchToggle = ttk.Checkbutton(
             self._options_frame,
-            text='Must Match',
+            text="Must Match",
             variable=self.mustMatch,
             command=self._somethingChanged
         )
-        self._mustMatchToggle.pack(fill='x')
+        self._mustMatchToggle.pack(fill="x")
         self._childWidgets = [self._mustMatchToggle]
         self._makeAdditionalWidgets()
         self._setActive(False)
 
+        self.missingmatches = None
+        self.scalevalue = None
+
     def _makeAdditionalWidgets(self):
         pass
 
     def _setActive(self, value):
         self.active = value
         if self.active:
-            self.config(relief='raised')
+            self.config(relief="raised")
             for widget in self._childWidgets:
-                if widget.winfo_class() == 'TCombobox':
-                    widget.config(state='readonly')
+                if widget.winfo_class() == "TCombobox":
+                    widget.config(state="readonly")
                 else:
-                    widget.config(state='normal')
+                    widget.config(state="normal")
         else:
-            self.config(relief='sunken')
+            self.config(relief="sunken")
             for widget in self._childWidgets:
-                widget.config(state='disabled')
+                widget.config(state="disabled")
 
     def toggleFolding(self, *args):
         self.is_folded = not self.is_folded
         if self.is_folded:
-            self._fold_button.config(text='v')
+            self._fold_button.config(text="v")
             self._options_frame.pack_forget()
         else:
-            self._fold_button.config(text='^')
+            self._fold_button.config(text="^")
             self._options_frame.pack()
 
-
     def _activeToggled(self, *args):
         self._setActive(not self.active)
         self._somethingChanged()
 
     def _somethingChanged(self, *args):
         self._Ctrl.onChange()
 
     def _updateFromPrevious(self, checksums):
         # check that the checksums or the widget parameters changed from before
         # if not simply return false to indicate that nothing is updated
-        foundADifference = (self._checksums != set(checksums))
-        for param in self._currentConfig:
+        foundADifference = self._checksums != set(checksums)
+        for param, value in self._currentConfig.items():
             if foundADifference:
                 # one difference is enough
                 break
-            if getattr(self, param) != self._currentConfig[param]:
+            if getattr(self, param) != value:
                 foundADifference = True
 
         if not foundADifference:
             return False
 
         # store the current values for posterity
         self._checksums = set(checksums)
@@ -148,47 +152,47 @@
         self._postMatching()
         return self._currentMatchingGroups
 
     # this is a trick to make sure that ctrl-a works on the thumbnails
     # even if the Scale has foocus
     def _doSelectAll(self, *args):
         self._Ctrl.toggleSelectAllThumbnails()
-        return 'break'
+        return "break"
 
 
 class HashingCondition(ConditionModule):
-    _currentConfig = {'method': None, 'limit': None}
-    _methods = ['']
-    method = ''
+    _currentConfig = {"method": None, "limit": None}
+    _methods = [""]
+    method = ""
     limit = 1
 
     def _makeAdditionalWidgets(self):
         self._Combo = ttk.Combobox(
             self._options_frame,
             values=self._methods,
             width=15,
-            state='readonly',
+            state="readonly",
         )
         self._Combo.set(self.method)
-        self._Combo.bind('<<ComboboxSelected>>', self._comboChanged)
+        self._Combo.bind("<<ComboboxSelected>>", self._comboChanged)
         self._Combo.pack()
         limitVar = tk.IntVar()
         limitVar.set(self.limit)
         self._Scale = CS.LabelScale(
             self._options_frame,
             from_=1,
             to=50,
             takefocus=1,
             command=self._scaleChanged,
             variable=limitVar,
-            orient='horizontal',
+            orient="horizontal",
         )
-        self._Scale.bind('<Control-a>', self._doSelectAll)
+        self._Scale.bind("<Control-a>", self._doSelectAll)
         self._Scale.pack()
-        self._ScaleTip = TT.Tooltip(self._Scale, text='')
+        self._ScaleTip = TT.Tooltip(self._Scale, text="")
         self._childWidgets.extend([self._Combo, self._Scale])
 
     def _comboChanged(self, *args):
         self.method = self._Combo.get()
         self._Combo.focus_set()
         self._somethingChanged()
 
@@ -200,172 +204,175 @@
     def _preMatching(self):
         # Call this to make sure the hash values for this method are available
         self._Ctrl.setHashes(hashName=self.method)
         self._matchingInfo = []
 
     def _postMatching(self):
         if not self._matchingInfo:
-            self._ScaleTip.text = ''
+            self._ScaleTip.text = ""
         elif len(self._matchingInfo) < 10:
-            self._ScaleTip.text = 'Min: %d' % (math.ceil(min(self._matchingInfo)))
+            self._ScaleTip.text = f"Min: {math.ceil(min(self._matchingInfo))}"
         else:
             self._matchingInfo.sort()
-            self._ScaleTip.text = 'min=%d; >10 pairs=%d' % (math.ceil(min(self._matchingInfo)), math.ceil(self._matchingInfo[9]))
+            self._ScaleTip.text = (
+                f"min={math.ceil(min(self._matchingInfo))}; "
+                f">10 pairs={math.ceil(self._matchingInfo[9])}"
+            )
 
 
 class GradientCondition(HashingCondition):
-    name = 'gradients'
-    _conditionName = 'GRADIENTS'
-    _methods = ['Horizontal', 'Vertical']
-    method = 'Horizontal'
+    name = "gradients"
+    _conditionName = "GRADIENTS"
+    _methods = ["Horizontal", "Vertical"]
+    method = "Horizontal"
     limit = 14
 
     def _theymatch(self, checksumA, checksumB):
         hashA = self._Ctrl.FODict[checksumA][0].hashDict[self.method]
         hashB = self._Ctrl.FODict[checksumB][0].hashDict[self.method]
         dist = functools.reduce(
             add,
-            [format(hashA[i] ^ hashB[i], 'b').count('1') for i in range(len(hashA))]
+            [format(hashA[i] ^ hashB[i], "b").count("1") for i in range(len(hashA))]
         )
         self._matchingInfo.append(dist)
         return dist <= self.limit
 
 
 class ColorCondition(HashingCondition):
-    name = 'colordistance'
-    _conditionName = 'COLOR DISTANCE'
+    name = "colordistance"
+    _conditionName = "COLOR DISTANCE"
     _methods = [
-        'HSV',
-        'HSV (5 regions)',
-        'RGB',
-        'RGB (5 regions)',
-        'Luminosity',
-        'Luminosity (5 regions)'
+        "HSV",
+        "HSV (5 regions)",
+        "RGB",
+        "RGB (5 regions)",
+        "Luminosity",
+        "Luminosity (5 regions)"
     ]
-    method = 'HSV (5 regions)'
+    method = "HSV (5 regions)"
     limit = 10
 
     def _theymatch(self, checksumA, checksumB):
         hashA = self._Ctrl.FODict[checksumA][0].hashDict[self.method]
         hashB = self._Ctrl.FODict[checksumB][0].hashDict[self.method]
         # we need to take care of the median hue value (0, 6, .. th element)
         # when calculating distance because this is a measure that wraps at 255
         # back to 0. The correct distance is the minimum of:
         # (h1-h2) % 255 and (h2-h1) % 255
         # in all other cases use abs(v1 -v2)
-        if self.method in ['HSV', 'HSV (5 regions)']:
+        if self.method in ["HSV", "HSV (5 regions)"]:
             distArr = [
                 abs(hashA[i]-hashB[i]) if i % 6
                 else min((hashA[i]-hashB[i]) % 255, (hashB[i]-hashA[i]) % 255)
                 for i in range(len(hashA))
             ]
         else:
             distArr = [abs(hashA[i]-hashB[i]) for i in range(len(hashA))]
         val = sum(distArr)/len(distArr)
         self._matchingInfo.append(val)
         return val <= self.limit
 
 
 class ExifCondition(ConditionModule):
-    _currentConfig = {'missingmatches': None, 'scalevalue': None}
-    _scaleDict = {'': 0}
-    _initialScaleVal = ''
+    _currentConfig = {"missingmatches": None, "scalevalue": None}
+    _scaleDict = {"": 0}
+    _initialScaleVal = ""
     _showMissingMatches = True
 
     def _makeAdditionalWidgets(self):
         self.missingmatches = False
         self.scalevalue = self._scaleDict[self._initialScaleVal]
         self._missingVar = tk.BooleanVar()
         self._missingMatchesCheck = ttk.Checkbutton(
             self._options_frame,
-            text='Missing Matches',
+            text="Missing Matches",
             variable=self._missingVar,
             command=self._toggleChanged,
         )
         if self._showMissingMatches:
-            self._missingMatchesCheck.pack(fill='x')
+            self._missingMatchesCheck.pack(fill="x")
 
         labels = list(self._scaleDict)
         scaleVar = tk.IntVar()
         scaleVar.set(labels.index(self._initialScaleVal))
         self._Scale = CS.TextScale(
             self._options_frame,
             textLabels=labels,
             command=self._scaleChanged,
             variable=scaleVar,
-            orient='horizontal'
+            orient="horizontal"
         )
-        self._Scale.bind('<Control-a>', self._doSelectAll)
+        self._Scale.bind("<Control-a>", self._doSelectAll)
         self._Scale.pack()
         self._childWidgets.extend([self._missingMatchesCheck, self._Scale])
 
     def _toggleChanged(self, *args):
         self.missingmatches = self._missingVar.get()
         self._somethingChanged()
 
     def _scaleChanged(self, *args):
         self.scalevalue = self._scaleDict[self._Scale.get()]
         self._Scale.focus_set()
         self._somethingChanged()
 
 
 class CameraCondition(ExifCondition):
-    name = 'cameramodel'
-    _conditionName = 'CAMERA MODEL'
-    _scaleDict = {'Same': True, 'Different': False}
-    _initialScaleVal = 'Same'
+    name = "cameramodel"
+    _conditionName = "CAMERA MODEL"
+    _scaleDict = {"Same": True, "Different": False}
+    _initialScaleVal = "Same"
 
     def _theymatch(self, checksumA, checksumB):
         camA = self._Ctrl.FODict[checksumA][0].cameraModel()
         camB = self._Ctrl.FODict[checksumB][0].cameraModel()
-        if camA == '':
+        if camA == "":
             return False
-        if self.missingmatches and camB == '':
+        if self.missingmatches and camB == "":
             return True
         return (camA == camB) == self.scalevalue
 
 
 class DateCondition(ExifCondition):
-    name = 'closeintime'
-    _conditionName = 'CLOSE IN TIME'
+    name = "closeintime"
+    _conditionName = "CLOSE IN TIME"
     _scaleDict = {
-        '1 minute': 60,
-        '10 minutes': 600,
-        '1 hour': 3600,
-        '1 day': 24*3600,
-        '1 week': 7*24*3600,
-        '4 weeks': 4*7*24*3600,
-        '1 year': 365*24*3600
+        "1 minute": 60,
+        "10 minutes": 600,
+        "1 hour": 3600,
+        "1 day": 24*3600,
+        "1 week": 7*24*3600,
+        "4 weeks": 4*7*24*3600,
+        "1 year": 365*24*3600
     }
-    _initialScaleVal = '10 minutes'
+    _initialScaleVal = "10 minutes"
 
     def _theymatch(self, checksumA, checksumB):
         dateA = self._Ctrl.FODict[checksumA][0].dateTime()
         dateB = self._Ctrl.FODict[checksumB][0].dateTime()
-        if dateA == 'Missing':
+        if dateA == "Missing":
             return False
-        if dateB == 'Missing':
+        if dateB == "Missing":
             return self.missingmatches
         return abs((dateA - dateB).total_seconds()) <= self.scalevalue
 
 
 class ShapeCondition(ExifCondition):
-    name = 'pictureshape'
-    _conditionName = 'PICTURE SHAPE'
+    name = "pictureshape"
+    _conditionName = "PICTURE SHAPE"
     _scaleDict = {
-        'Different Size': -2,
-        'Portrait/Landscape': -1,
-        'Exact': 0,
-        '<5%': 5,
-        '<10%': 10,
-        '<20%': 20,
-        '<30%': 30,
-        '<50%': 50
+        "Different Size": -2,
+        "Portrait/Landscape": -1,
+        "Exact": 0,
+        "<5%": 5,
+        "<10%": 10,
+        "<20%": 20,
+        "<30%": 30,
+        "<50%": 50
     }
-    _initialScaleVal = 'Portrait/Landscape'
+    _initialScaleVal = "Portrait/Landscape"
     _showMissingMatches = False
 
     def _theymatch(self, checksumA, checksumB):
         if self.scalevalue == -2:
             sizeA = self._Ctrl.FODict[checksumA][0].size()
             sizeB = self._Ctrl.FODict[checksumB][0].size()
             return set(sizeA) != set(sizeB)
```

### Comparing `simimg-0.9.1/simimg/classes/configuration.py` & `simimg-0.9.2/simimg/classes/configuration.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,154 +1,153 @@
-'''communicate and read/write configuration info'''
+"""communicate and read/write configuration info"""
 import sys
 import os.path
 import configparser
 
 
 def str2bool(S):
-    '''convert a string to a boolean
-    we use only the first letter'''
+    """convert a string to a boolean
+    we use only the first letter"""
     return {
-        '0': False,
-        'n': False,
-        'N': False,
-        'f': False,
-        'F': False,
-        '1': True,
-        'y': True,
-        'Y': True,
-        't': True,
-        'T': True,
+        "0": False,
+        "n": False,
+        "N": False,
+        "f": False,
+        "F": False,
+        "1": True,
+        "y": True,
+        "Y": True,
+        "t": True,
+        "T": True,
     }[S[0]]
 
 
 class Configuration():
-    ' Object that can initialise, change and inform about App configuration'
+    " Object that can initialise, change and inform about App configuration"
 
     def __init__(self, ScriptPath=None):
         # The path of the appdata and ini file
         ConfigPath = os.path.join(
-            os.environ.get('APPDATA') or
-            os.environ.get('XDG_CONFIG_HOME') or
-            os.path.join(os.environ['HOME'], '.config'),
-            'simimg'
+            os.environ.get("APPDATA") or
+            os.environ.get("XDG_CONFIG_HOME") or
+            os.path.join(os.environ["HOME"], ".config"),
+            "simimg"
         )
-        self.IniPath = os.path.join(ConfigPath, 'simimg.ini')
+        self.IniPath = os.path.join(ConfigPath, "simimg.ini")
 
         # dict to store all settings
         self.ConfigurationDict = {}
-        self.set('cmdlinearguments', sys.argv[1:])
-        self.set('iconpath', os.path.join(ScriptPath, 'icons'))
-        self.set('databasename', os.path.join(ConfigPath,'simimg.db'))
+        self.set("cmdlinearguments", sys.argv[1:])
+        self.set("iconpath", os.path.join(ScriptPath, "icons"))
+        self.set("databasename", os.path.join(ConfigPath, "simimg.db"))
 
         self._setDefaultConfiguration()
         self._readConfiguration()
 
     def _setDefaultConfiguration(self):
-        'Default configuration parameters'
+        "Default configuration parameters"
         # not yet? configurable
-        self.set('maxthumbnails', 300)
-        self.set('channeltoshow', 'default')
-        self.set('numfolders', 3)
+        self.set("maxthumbnails", 300)
+        self.set("channeltoshow", "default")
+        self.set("numfolders", 3)
 
         # can be overwritten from ini file
-        self.set('searchinsubfolders', False)
-        self.set('confirmdelete', True)
-        self.set('gzipinsteadofdelete', False)
-        self.set('savesettings', True)
-        self.set('showbuttons', True)
-        self.set('filenameonthumbnail', False)
-        self.set('thumbnailsize', 150)
-        self.set('upscalethumbnails', False)
-        self.set('startupfolder', '')
-        self.set('findergeometry', '1200x800+0+0')
-        self.set('viewergeometry', '1200x800+50+0')
-        self.set('restoremovefolders', False)
-        for i in range(1, self.get('numfolders')+1):
-            self.set('folder'+str(i), '')
+        self.set("searchinsubfolders", False)
+        self.set("confirmdelete", True)
+        self.set("gzipinsteadofdelete", False)
+        self.set("savesettings", True)
+        self.set("showbuttons", True)
+        self.set("filenameonthumbnail", False)
+        self.set("thumbnailsize", 150)
+        self.set("upscalethumbnails", False)
+        self.set("startupfolder", "")
+        self.set("findergeometry", "1200x800+0+0")
+        self.set("viewergeometry", "1200x800+50+0")
+        self.set("restoremovefolders", False)
+        for i in range(1, self.get("numfolders")+1):
+            self.set("folder"+str(i), "")
 
     def _readConfiguration(self):
-        '''Function to get configurable parameters from SimImg.ini.'''
-        config = configparser.ConfigParser(converters={'strbool': str2bool})
+        """Function to get configurable parameters from SimImg.ini."""
+        config = configparser.ConfigParser(converters={"strbool": str2bool})
         if config.read(self.IniPath):
-            default = config['simimg']
-            doRecursive = default.getstrbool('searchinsubfolders', 'no')
-            confirmdelete = default.getstrbool('confirmdelete', 'yes')
-            doGzip = default.getstrbool('gzipinsteadofdelete', 'no')
-            savesettings = default.getstrbool('savesettings', 'yes')
-            showbuttons = default.getstrbool('showbuttons', 'yes')
-            filenameonthumbnail = default.getstrbool('filenameonthumbnail', 'no')
-            thumbSize = default.getint('thumbnailsize', 150)
-            doUpscaleThumbnails = default.getstrbool('upscalethumbnails', 'no')
-            startupDir = default.get('startupfolder', '.')
-            finderGeometry = default.get('findergeometry', '1200x800+0+0')
-            viewerGeometry = default.get('viewergeometry', '1200x800+50+0')
-            restoremovefolders = default.getstrbool('restoremovefolders', 'no')
+            default = config["simimg"]
+            doRecursive = default.getstrbool("searchinsubfolders", "no")
+            confirmdelete = default.getstrbool("confirmdelete", "yes")
+            doGzip = default.getstrbool("gzipinsteadofdelete", "no")
+            savesettings = default.getstrbool("savesettings", "yes")
+            showbuttons = default.getstrbool("showbuttons", "yes")
+            filenameonthumbnail = default.getstrbool("filenameonthumbnail", "no")
+            thumbSize = default.getint("thumbnailsize", 150)
+            doUpscaleThumbnails = default.getstrbool("upscalethumbnails", "no")
+            startupDir = default.get("startupfolder", ".")
+            finderGeometry = default.get("findergeometry", "1200x800+0+0")
+            viewerGeometry = default.get("viewergeometry", "1200x800+50+0")
+            restoremovefolders = default.getstrbool("restoremovefolders", "no")
             # store read values in ConfigurationDict
-            self.set('searchinsubfolders', doRecursive)
-            self.set('confirmdelete', confirmdelete)
-            self.set('gzipinsteadofdelete', doGzip)
-            self.set('savesettings', savesettings)
-            self.set('showbuttons', showbuttons)
-            self.set('filenameonthumbnail', filenameonthumbnail)
-            self.set('thumbnailsize', thumbSize)
-            self.set('upscalethumbnails', doUpscaleThumbnails)
-            self.set('startupfolder', startupDir)
-            self.set('findergeometry', finderGeometry)
-            self.set('viewergeometry', viewerGeometry)
-            self.set('restoremovefolders', restoremovefolders)
+            self.set("searchinsubfolders", doRecursive)
+            self.set("confirmdelete", confirmdelete)
+            self.set("gzipinsteadofdelete", doGzip)
+            self.set("savesettings", savesettings)
+            self.set("showbuttons", showbuttons)
+            self.set("filenameonthumbnail", filenameonthumbnail)
+            self.set("thumbnailsize", thumbSize)
+            self.set("upscalethumbnails", doUpscaleThumbnails)
+            self.set("startupfolder", startupDir)
+            self.set("findergeometry", finderGeometry)
+            self.set("viewergeometry", viewerGeometry)
+            self.set("restoremovefolders", restoremovefolders)
 
             # restore move folders enabled
             if restoremovefolders:
-                for i in range(1, self.get('numfolders')+1):
-                    self.set('folder'+str(i), default.get('folder'+str(i), ''))
+                for i in range(1, self.get("numfolders")+1):
+                    self.set("folder"+str(i), default.get("folder"+str(i), ""))
 
             # restore folded folder state
             for k in default.keys():
-                if k[-7:] == '_folded':
-                    is_folded = default.getstrbool(k, 'no')
+                if k[-7:] == "_folded":
+                    is_folded = default.getstrbool(k, "no")
                     self.set(k, is_folded)
 
-                    
     def writeConfiguration(self):
-        'save configuration info'
+        "save configuration info"
 
         # save settings disabled
-        if not self.get('savesettings'):
+        if not self.get("savesettings"):
             return
 
         config = configparser.ConfigParser()
-        config['simimg'] = {
-            'searchinsubfolders': self.get('searchinsubfolders'),
-            'confirmdelete': self.get('confirmdelete'),
-            'gzipinsteadofdelete': self.get('gzipinsteadofdelete'),
-            'savesettings': self.get('savesettings'),
-            'showbuttons': self.get('showbuttons'),
-            'filenameonthumbnail': self.get('filenameonthumbnail'),
-            'thumbnailsize': self.get('thumbnailsize'),
-            'upscalethumbnails': self.get('upscalethumbnails'),
-            'startupfolder': self.get('startupfolder'),
-            'findergeometry': self.get('findergeometry'),
-            'viewergeometry': self.get('viewergeometry'),
-            'restoremovefolders': self.get('restoremovefolders'),
+        config["simimg"] = {
+            "searchinsubfolders": self.get("searchinsubfolders"),
+            "confirmdelete": self.get("confirmdelete"),
+            "gzipinsteadofdelete": self.get("gzipinsteadofdelete"),
+            "savesettings": self.get("savesettings"),
+            "showbuttons": self.get("showbuttons"),
+            "filenameonthumbnail": self.get("filenameonthumbnail"),
+            "thumbnailsize": self.get("thumbnailsize"),
+            "upscalethumbnails": self.get("upscalethumbnails"),
+            "startupfolder": self.get("startupfolder"),
+            "findergeometry": self.get("findergeometry"),
+            "viewergeometry": self.get("viewergeometry"),
+            "restoremovefolders": self.get("restoremovefolders"),
         }
-        for i in range(1, self.get('numfolders')+1):
-            config['simimg'].update({'folder'+str(i): self.get('folder'+str(i))})
+        for i in range(1, self.get("numfolders")+1):
+            config["simimg"].update({"folder"+str(i): self.get("folder"+str(i))})
 
         # add the folding state of the condition modules
-        folding_dict = self.get('folding_dict')
+        folding_dict = self.get("folding_dict")
         if isinstance(folding_dict, dict):
             for k, v in folding_dict.items():
-                config['simimg'].update({f'{k}_folded': str(v)})
+                config["simimg"].update({f"{k}_folded": str(v)})
 
-        with open(self.IniPath, 'w') as configfile:
+        with open(self.IniPath, "w", encoding="utf-8") as configfile:
             config.write(configfile)
 
     def get(self, parameter):
-        'Return one value of the configuration'
+        "Return one value of the configuration"
         if parameter not in self.ConfigurationDict:
             return None
         return self.ConfigurationDict[parameter]
 
     def set(self, param, value):
-        'Add/Change a configuration parameter'
+        "Add/Change a configuration parameter"
         self.ConfigurationDict[param] = value
```

### Comparing `simimg-0.9.1/simimg/classes/controller.py` & `simimg-0.9.2/simimg/classes/controller.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,183 +1,185 @@
-''' Controller module:
+""" Controller module:
 The main gateway between the information contained in the database,
 the fileinfo objects and the display of the thumbnails.
- '''
-import sys
-import os
+ """
 import glob
+import os
+import sys
 from tkinter import ttk
 from tkinter import filedialog as tkfiledialog
+
 from PIL import ImageTk
-from . import conditionmodules as CM
-from . import fileobject as FO
-from . import imageframe as IF
-from . import miscmodules as MM
-from . import toolbar as TB
-from . import tooltip as TT
-from ..dialogs import confirmdeletedialog as CDD
-from ..dialogs import configurationwindow as CW
-from ..dialogs import infowindow as IW
-from ..dialogs import viewer as VI
-from ..utils import database as DB
-from ..utils import handyfunctions as HF
-from ..utils import pooling as POOL
+
+import simimg.classes.conditionmodules as CM
+import simimg.classes.fileobject as FO
+import simimg.classes.imageframe as IF
+import simimg.classes.miscmodules as MM
+import simimg.classes.toolbar as TB
+import simimg.classes.tooltip as TT
+import simimg.dialogs.configurationwindow as CW
+import simimg.dialogs.confirmdeletedialog as CDD
+import simimg.dialogs.infowindow as IW
+import simimg.dialogs.viewer as VI
+import simimg.utils.database as DB
+import simimg.utils.handyfunctions as HF
+import simimg.utils.pooling as POOL
 
 # decorator to change cursor when calling a method that might take time
 def longrunning(f):
-    ''' Show with the cursor that the program is doing a (long) calculation'''
+    """ Show with the cursor that the program is doing a (long) calculation"""
 
     def wrapper(self, *args, **kwargs):
-        self._busyCursorCount += 1
-        self.TopWindow.config(cursor='watch')
+        self.busyCursorCount += 1
+        self.TopWindow.config(cursor="watch")
         f(self, *args, **kwargs)
-        self._busyCursorCount -= 1
+        self.busyCursorCount -= 1
         # make sure not to go below 0
-        self._busyCursorCount = max(0, self._busyCursorCount)
-        if not self._busyCursorCount:
-            self.TopWindow.config(cursor='')
+        self.busyCursorCount = max(0, self.busyCursorCount)
+        if not self.busyCursorCount:
+            self.TopWindow.config(cursor="")
     return wrapper
 
 
 # decorator to show message in status bar for the duration of a function call
 def tellstatus(msg):
     def decorator_tellstatus(f):
         def wrapper_tellstatus(self, *args, **kwargs):
             if msg:
-                self._showInStatusbar(msg)
+                self.showInStatusbar(msg)
             f(self, *args, **kwargs)
-            self._showInStatusbar('...')
+            self.showInStatusbar("...")
         return wrapper_tellstatus
     return decorator_tellstatus
 
 
 class Controller():
-    'Controller object that initializes the program and reacts to events.'
+    "Controller object that initializes the program and reacts to events."
 
     def __init__(self, parent):
 
         self.TopWindow = parent
         self.Cfg = parent.Cfg
         self.lastSelectedXY = None
 
-        self._maxThumbnails = self.Cfg.get('maxthumbnails')
+        self._maxThumbnails = self.Cfg.get("maxthumbnails")
 
         # empty starting values
         self.FODict = {}
         self._DBConnection = None
         self._fileList = []
-        self._filenameCommon = ''
+        self._filenameCommon = ""
         self._filenameUniqueDict = {}
         self._TPPositionDict = {}
         self._matchingGroups = {}
         self._checksumFilenameDict = {}
         self._filenameChecksumDict = {}
-        self._busyCursorCount = 0
+        self.busyCursorCount = 0
         self._someConditionActive = False
 
         # call the exitProgram function when the user clicks the X
-        self.TopWindow.protocol('WM_DELETE_WINDOW', self.exitProgram)
+        self.TopWindow.protocol("WM_DELETE_WINDOW", self.exitProgram)
         # allow some key actions (Ctrl-A, Ctl-D, Ctrl-H, Ctrl-V and F1)
-        self.TopWindow.bind('<Key>', self._onKeyPress)
+        self.TopWindow.bind("<Key>", self._onKeyPress)
         # bind clicking in an empty area of the thumbPane to unselectThumbnails
-        self.TopWindow.ThumbPane.viewPort.bind('<Button-1>', self.unselectThumbnails)
-        self.TopWindow.ThumbPane.canvas.bind('<Button-1>', self.unselectThumbnails)
+        self.TopWindow.ThumbPane.viewPort.bind("<Button-1>", self.unselectThumbnails)
+        self.TopWindow.ThumbPane.canvas.bind("<Button-1>", self.unselectThumbnails)
 
         # allow some key actions (Ctrl-A, Ctl-D, Ctrl-H, Ctrl-V and F1)
-        self.TopWindow.ThumbPane.bind('<Configure>', self._onConfigure)
+        self.TopWindow.ThumbPane.bind("<Configure>", self._onConfigure)
         self._TPWidth = 0
-        
+
         # put the toolbar in the self.TopWindow.ModulePane
         Toolbar = TB.Toolbar(self.TopWindow.ModulePane, Controller=self)
-        Toolbar.pack(side='top', fill='x')
+        Toolbar.pack(side="top", fill="x")
 
         ttk.Label(
             self.TopWindow.ModulePane,
-            text='Display',
-            style='HeaderText.TLabel'
-        ).pack(fill='x')
+            text="Display",
+            style="HeaderText.TLabel"
+        ).pack(fill="x")
 
         ThumbOpt = MM.ThumbOptions(self.TopWindow.ModulePane, Controller=self)
-        ThumbOpt.pack(side='top', fill='x')
+        ThumbOpt.pack(side="top", fill="x")
 
         ttk.Label(
             self.TopWindow.ModulePane,
-            text='Filters',
-            style='HeaderText.TLabel'
-        ).pack(fill='x')
+            text="Filters",
+            style="HeaderText.TLabel"
+        ).pack(fill="x")
 
         # create the condition modules in the self.TopWindow.ModulePane
         # put them in a list so that we can easily iterate over them
         self._CMList = []
         self._CMList.extend([
             CM.ColorCondition(self.TopWindow.ModulePane, Controller=self),
             CM.GradientCondition(self.TopWindow.ModulePane, Controller=self),
             CM.DateCondition(self.TopWindow.ModulePane, Controller=self),
             CM.CameraCondition(self.TopWindow.ModulePane, Controller=self),
             CM.ShapeCondition(self.TopWindow.ModulePane, Controller=self),
         ])
         for cm in self._CMList:
-            cm.pack(side='top', fill='x')
+            cm.pack(side="top", fill="x")
             # restore the saved folded/unfolded state
-            if self.Cfg.get(f'{cm.name}_folded'):
+            if self.Cfg.get(f"{cm.name}_folded"):
                 cm.toggleFolding()
 
         moveheader = ttk.Label(
             self.TopWindow.ModulePane,
-            text='Move',
-            style='HeaderText.TLabel'
+            text="Move",
+            style="HeaderText.TLabel"
         )
-        moveheader.pack(fill='x')
-        msg = '''Move file(s) to the folder selected below.
+        moveheader.pack(fill="x")
+        msg = """Move file(s) to the folder selected below.
 
 1) Click on the move button below each thumbnail
 
 2) For selected pictures by clicking on the move icon in the toolbar or pressing Ctrl-m
 
 3) Press m in the viewer window
 
-Right click on the folders below to set or change its path'''
+Right click on the folders below to set or change its path"""
         TT.Tooltip(moveheader, text=msg)
 
         self._MovePanel = MM.MovePanel(self.TopWindow.ModulePane, Controller=self)
-        self._MovePanel.pack(side='top', fill='x')
+        self._MovePanel.pack(side="top", fill="x")
 
         self.startDatabase()
         self._getFileList()
         self._processFilelist()
         self.onChange()
 
     def _onConfigure(self, event):
-        thumbW = self.Cfg.get('thumbnailsize') + 2
+        thumbW = self.Cfg.get("thumbnailsize") + 2
         oldTPWidth = self._TPWidth
         self._TPWidth = event.width
         # check of the number of thumb columns will change
         if oldTPWidth // thumbW == self._TPWidth // thumbW:
             return
         if not self._someConditionActive:
             self._createViewWithoutConditions()
 
     def _onKeyPress(self, event):
-        if event.keysym == 'F1':
+        if event.keysym == "F1":
             IW.showInfoDialog()
             return
         if (event.state & 0x4) != 0:
             keyDict = {
-                'a': self.toggleSelectAllThumbnails,
-                'd': self.deleteSelected,
-                'h': self.hideSelected,
-                'm': self.moveSelected,
-                'v': self.viewSelected,
-                'q': self.exitProgram
+                "a": self.toggleSelectAllThumbnails,
+                "d": self.deleteSelected,
+                "h": self.hideSelected,
+                "m": self.moveSelected,
+                "v": self.viewSelected,
+                "q": self.exitProgram
             }
             if event.keysym in keyDict:
                 keyDict[event.keysym]()
                 return
 
-    def _showInStatusbar(self, txt):
+    def showInStatusbar(self, txt):
         self.TopWindow.Statusbar.config(text=txt)
         self.TopWindow.Statusbar.update_idletasks()
 
     def _showThumbXY(self, checksum, X, Y):
         # make sure that if a thumb is currently shown it is removed
         # and deleted
         self._removeThumbXY(X, Y)
@@ -202,59 +204,59 @@
     def _removeAllThumbs(self):
         for ThisThumb in self._TPPositionDict.values():
             ThisThumb.destroy()
         self._TPPositionDict = {}
 
     def startDatabase(self, clear=None):
         self._DBConnection = DB.createConnection(
-            self.Cfg.get('databasename')
+            self.Cfg.get("databasename")
         )
         if not self._DBConnection:
             sys.exit(1)
 
         if not DB.createTables(self._DBConnection, clear=clear):
             sys.exit(1)
 
     def stopDatabase(self):
         DB.closeConnection(self._DBConnection)
 
     def exitProgram(self):
         self.stopDatabase()
-        self.Cfg.set('findergeometry', self.TopWindow.geometry())
+        self.Cfg.set("findergeometry", self.TopWindow.geometry())
         # make a dictionary of cm.name: is_folded
         folding_dict = {cm.name: cm.is_folded for cm in self._CMList}
-        self.Cfg.set('folding_dict', folding_dict)
+        self.Cfg.set("folding_dict", folding_dict)
         self.Cfg.writeConfiguration()
         self.TopWindow.quit()
 
     def configureProgram(self):
-        oldThumbsize = self.Cfg.get('thumbnailsize')
-        oldUpscale = self.Cfg.get('upscalethumbnails')
+        oldThumbsize = self.Cfg.get("thumbnailsize")
+        oldUpscale = self.Cfg.get("upscalethumbnails")
         CW.CfgWindow(self.TopWindow, Controller=self)
         if (
-                self.Cfg.get('thumbnailsize') != oldThumbsize or
-                self.Cfg.get('upscalethumbnails') != oldUpscale
+                self.Cfg.get("thumbnailsize") != oldThumbsize or
+                self.Cfg.get("upscalethumbnails") != oldUpscale
         ):
             self.onThumbParamsChanged()
 
     def addOrOpenFolder(self, action=None):
         selectedFolder = tkfiledialog.askdirectory()
         if not selectedFolder:
             return
         if not os.path.isdir(selectedFolder):
             return
-        if action == 'add':
+        if action == "add":
             self._getFileList(Add=selectedFolder)
         else:
             self._getFileList(Replace=selectedFolder)
         self._processFilelist()
         self.onChange()
 
     @longrunning
-    @tellstatus(msg='Gathering the files to show')
+    @tellstatus(msg="Gathering the files to show")
     def _getFileList(self, Replace=None, Add=None):
         pathList = []
         # determine with which mode we are called
         # from openFolder
         if Replace:
             pathList = [Replace]
             oldFiles = []
@@ -262,35 +264,35 @@
         # from add folder
         if Add:
             pathList = [Add]
             oldFiles = self._fileList
 
         # from startup
         if not Replace and not Add:
-            pathList = self.Cfg.get('cmdlinearguments')
+            pathList = self.Cfg.get("cmdlinearguments")
             oldFiles = []
             self.FODict = {}
 
         # from startup without arguments
         if not pathList:
             oldFiles = []
-            startupFolder = self.Cfg.get('startupfolder')
+            startupFolder = self.Cfg.get("startupfolder")
             # start empty
             if not startupFolder:
                 self._fileList = []
                 return
             pathList = [startupFolder]
 
         # now we know which folders to search
-        doRecurse = self.Cfg.get('searchinsubfolders')
+        doRecurse = self.Cfg.get("searchinsubfolders")
         candidates = []
         for arg in pathList:
             arg = os.path.abspath(arg)
             if os.path.isdir(arg):
-                candidates.extend(glob.glob(arg+'/**', recursive=doRecurse))
+                candidates.extend(glob.glob(arg+"/**", recursive=doRecurse))
             else:
                 candidates.append(arg)
         self._fileList = [c for c in candidates if os.path.isfile(c)]
         # check to make sure that the file list is not excessively long
         # three times more than we can anyway show
         # probably this means the program was started in the wrong directory
         # and or recursive was set wrongly
@@ -303,24 +305,24 @@
 
         # split the _fileList into a common and a unique part
         self._filenameCommon, filenameUniqueList = HF.stringlist2commonunique(self._fileList)
         self._filenameUniqueDict = {}
         self._filenameUniqueDict.update(zip(self._fileList, filenameUniqueList))
 
     @longrunning
-    @tellstatus(msg='Processing file list')
+    @tellstatus(msg="Processing file list")
     def _processFilelist(self):
-        ''' Things to do when starting with new image(s)/path'''
+        """ Things to do when starting with new image(s)/path"""
 
         # calculate checksums in multiprocessing
         self._getChecksums()
 
         self._createFileobjects()
         if not self.FODict:
-            self._showInStatusbar('Warning: no files containing image data found')
+            self.showInStatusbar("Warning: no files containing image data found")
 
         # calculate thumbnails in multiprocessing
         self._setThumbnails()
 
     def _createFileobjects(self):
         # Make list of image file objects with all files PIL can read
         fileObjectList = []
@@ -332,36 +334,36 @@
         missingfilelist = list(set(self._fileList) - set(existingfiles))
         for FilePath in missingfilelist:
             ThisFileObject = FO.FileObject(
                 self,
                 FullPath=FilePath,
                 checksumFilenameDict=self._checksumFilenameDict
             )
-            if ThisFileObject.isImage():
+            if ThisFileObject.isImage:
                 fileObjectList.append(ThisFileObject)
                 # do checksum hash and thumbnails
                 ThisFileObject.checksum()
-                
+
         if not fileObjectList:
             return
 
         # transform into a dict based on uniq checksum
         newFODict = HF.pairlist2dict([(i.checksum(), i) for i in fileObjectList])
         self.FODict.update(newFODict)
 
     def _createViewWithoutConditions(self):
-        'Create an overview of all images without conditions'
+        "Create an overview of all images without conditions"
         self._removeAllThumbs()
 
         # because there are no criteria display thumbnails in order
         # calculate how many thumbs fit in the viewPort
         self.TopWindow.ThumbPane.update_idletasks()
         maxW = self.TopWindow.ThumbPane.winfo_width()
         # 2 extra for the highlight thickness
-        thumbW = self.Cfg.get('thumbnailsize') + 2
+        thumbW = self.Cfg.get("thumbnailsize") + 2
         nx = maxW // thumbW
 
         # maximum nx*ny thumbs to show
         thumbToShow = 0
         for checksum in HF.sortChecksumsByFilename(self.FODict.keys(), self._filenameChecksumDict):
             if not self.FODict[checksum][0].active:
                 continue
@@ -369,16 +371,16 @@
             Y = thumbToShow // nx
             self._showThumbXY(checksum, X, Y)
             thumbToShow += 1
             if thumbToShow >= self._maxThumbnails:
                 break
 
     def _getMatchingGroups(self):
-        ''' given the matching groups returned by each active condition module
-           make a master list of image groups '''
+        """ given the matching groups returned by each active condition module
+           make a master list of image groups """
 
         self._matchingGroups = {}
         matchingGroupDictsList = []
         MMMatchingGroupDictsList = []
         activeChecksums = [checksum for checksum, FO in self.FODict.items() if FO[0].active]
         for cm in self._CMList:
             if not cm.active:
@@ -395,27 +397,34 @@
 
         matchingGroups = HF.removeRedunantSubgroups(matchingGroups)
 
         self._matchingGroups = matchingGroups
 
     def _displayMatchingGroups(self):
         # clear messages from the statusbar
-        self._showInStatusbar('...')
-        sortedGroupsList = HF.sortMatchingGroupsByFilename(self._matchingGroups, self._filenameChecksumDict)
+        self.showInStatusbar("...")
+        sortedGroupsList = HF.sortMatchingGroupsByFilename(
+            self._matchingGroups,
+            self._filenameChecksumDict
+        )
         numThumbsShown = 0
         for Y, group in enumerate(sortedGroupsList):
             for X, checksum in enumerate(group):
                 self._showThumbXY(checksum, X, Y)
                 numThumbsShown += 1
                 # no point showing so many
                 if X > 25:
-                    self._showInStatusbar('Groups found a group with too many matches: truncated to 25')
+                    self.showInStatusbar(
+                        "Groups found a group with too many matches: truncated to 25"
+                    )
                     break
             if numThumbsShown > self._maxThumbnails:
-                self._showInStatusbar('Warning too many matches: truncated to ~%s' % self._maxThumbnails)
+                self.showInStatusbar(
+                    f"Warning too many matches: truncated to ~{self._maxThumbnails}"
+                )
                 return
 
     @longrunning
     def onChange(self):
         # put everything to default
         self._matchingGroups = {}
         # make sure to clean the interface
@@ -476,83 +485,83 @@
 
     def hideSelected(self):
         for fo in self._selectedFOs():
             fo.active = False
         self.onChange()
 
     def _deleteFile(self, Filename):
-        if self.Cfg.get('gzipinsteadofdelete'):
+        if self.Cfg.get("gzipinsteadofdelete"):
             HF.gzipfile(Filename)
         else:
             os.remove(Filename)
 
-    def _moveFile(self, fn, dir):
-        if os.path.dirname(fn) == dir:
+    def _moveFile(self, fn, dirname):
+        if os.path.dirname(fn) == dirname:
             return False
         try:
             os.rename(
                 fn,
-                os.path.join(dir, os.path.basename(fn))
+                os.path.join(dirname, os.path.basename(fn))
             )
         except:
             return False
         return True
-    
+
     def moveFOs(self, FOs, **kwargs):
         # check that a target folder is set
         # if not give a warning and do nothing
         targetDir = self._MovePanel.get(**kwargs)
         if not targetDir:
-            self._showInStatusbar('Warning: no target folder set for moving files')
-            return
-        # check that the target folder 
+            self.showInStatusbar("Warning: no target folder set for moving files")
+            return None
+        # check that the target folder
         # if not give a warning and do nothing
         if not os.path.isdir(targetDir):
-            self._showInStatusbar(
-                'Warning: target folder %s for moving files is not valid' % targetDir
+            self.showInStatusbar(
+                f"Warning: target folder {targetDir} for moving files is not valid"
             )
-            return
+            return None
         somethingMoved = False
         for fo in FOs:
             filename = fo.fullPath
             checksum = fo.checksum()
             if self._moveFile(filename, targetDir):
                 if checksum in self.FODict:
                     del self.FODict[checksum]
                 somethingMoved = True
         if somethingMoved:
             self.onChange()
         return somethingMoved
-    
+
     def deleteFOs(self, FOs, Owner=None):
         if not Owner:
             Owner = self.TopWindow
         somethingDeleted = False
-        mustconfirm = self.Cfg.get('confirmdelete')
+        mustconfirm = self.Cfg.get("confirmdelete")
         onlyOneFO = len(FOs) == 1
         for fo in FOs:
             filename = fo.fullPath
             uniqueFilename = self._filenameUniqueDict[filename]
             checksum = fo.checksum()
             if mustconfirm:
                 answer = CDD.CDDialog(
                     Owner,
                     Filename=uniqueFilename,
                     simple=onlyOneFO
                 ).result
             else:
-                answer = 'yes'
-            if answer == 'abort':
+                answer = "yes"
+            if answer == "abort":
                 break
-            if answer == 'no':
+            if answer == "no":
                 continue
-            if answer == 'yestoall':
+            if answer == "yestoall":
                 mustconfirm = False
-                answer = 'yes'
-            if answer == 'yes':
+                answer = "yes"
+            if answer == "yes":
                 if checksum in self.FODict:
                     del self.FODict[checksum]
                 somethingDeleted = True
                 self._deleteFile(filename)
 
         if somethingDeleted:
             self.onChange()
@@ -577,15 +586,15 @@
                 break
         if isAllSelected:
             for tp in self._TPPositionDict.values():
                 tp.select(False)
         else:
             for tp in self._TPPositionDict.values():
                 tp.select(True)
-                
+
         self.lastSelectedXY = None
 
     def toggleSelectRow(self, Y, value):
         for tp in self._TPPositionDict.values():
             if tp.Y == Y:
                 tp.select(value)
 
@@ -614,28 +623,28 @@
                     gridXYLargerOrEqual((tp.X, tp.Y), fromXY) and
                     gridXYLargerOrEqual(toXY, (tp.X, tp.Y))
             ):
                 tp.select(True)
 
     # some routines related to expensive calculations done in a
     # multiprocessing pool
-    @tellstatus(msg='Calculating File Hash values, please be patient')
+    @tellstatus(msg="Calculating File Hash values, please be patient")
     def _getChecksums(self):
         self._checksumFilenameDict = POOL.getChecksums(self._fileList, self._checksumFilenameDict)
         self._filenameChecksumDict = dict(map(reversed, self._checksumFilenameDict.items()))
 
-    @tellstatus(msg='Making file thumbnails, please be patient')
+    @tellstatus(msg="Making file thumbnails, please be patient")
     def _setThumbnails(self):
         checksumThumbDict = POOL.getThumbnails(
             self.FODict,
-            Thumbsize=self.Cfg.get('thumbnailsize'),
-            channel=self.Cfg.get('channeltoshow'),
-            upscale=self.Cfg.get('upscalethumbnails'),
+            Thumbsize=self.Cfg.get("thumbnailsize"),
+            channel=self.Cfg.get("channeltoshow"),
+            upscale=self.Cfg.get("upscalethumbnails"),
         )
-        self._showInStatusbar('...')
+        self.showInStatusbar("...")
         if not checksumThumbDict:
             return
         for checksum, thumb in checksumThumbDict.items():
             if not thumb:
                 del self.FODict[checksum]
                 continue
 
@@ -646,10 +655,10 @@
                 continue
 
             fo = self.FODict[checksum]
             for afo in fo:
                 afo._thumbnail = pimage
 
     @longrunning
-    @tellstatus(msg='Calculating Image Hash values, please be patient')
+    @tellstatus(msg="Calculating Image Hash values, please be patient")
     def setHashes(self, hashName=None):
         POOL.getHashes(self.FODict, hashName, self._DBConnection)
```

### Comparing `simimg-0.9.1/simimg/classes/customscales.py` & `simimg-0.9.2/simimg/classes/customscales.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from tkinter import ttk
 
 
 class DelayedScale(ttk.Scale):
-    '''A ttk scale widget that only fires the command when the mouse is released
+    """A ttk scale widget that only fires the command when the mouse is released
        if using the mouse to drag the slider
-       We also modify the behaviour to always returns integer values'''
+       We also modify the behaviour to always returns integer values"""
 
     def __init__(self, parent, *args, command=None, resolution=None, **kwargs):
         self.realcommand = command
         self._step = int(resolution) if resolution else 1
         super().__init__(parent, *args, command=self._command, **kwargs)
-        self.bind('<ButtonPress-1>', self._scalePressed)
-        self.bind('<ButtonRelease-1>', self._scaleReleased)
-        self.bind('<Key-Left>', self._leftPressed)
-        self.bind('<Key-Right>', self._rightPressed)
-        self.bind('<ButtonPress-1>', self._scalePressed)
+        self.bind("<ButtonPress-1>", self._scalePressed)
+        self.bind("<ButtonRelease-1>", self._scaleReleased)
+        self.bind("<Key-Left>", self._leftPressed)
+        self.bind("<Key-Right>", self._rightPressed)
+        self.bind("<ButtonPress-1>", self._scalePressed)
         self._mouseIsPressed = False
 
     def _leftPressed(self, *args):
         self.set(int(self.get()-self._step))
-        return 'break'
-    
+        return "break"
+
     def _rightPressed(self, *args):
         self.set(int(self.get()+self._step))
-        return 'break'
-        
+        return "break"
+
     def _scalePressed(self, *args):
         self._mouseIsPressed = True
 
     def _scaleReleased(self, *args):
         self._mouseIsPressed = False
         self._command()
 
@@ -40,30 +40,30 @@
             return
         self.mousedowncommand()
         if self._mouseIsPressed:
             return
         if self.realcommand:
             self.realcommand()
 
-    def get(self):
+    def get(self, *args):
         return int(super().get())
 
-    def set(self, val):
-        super().set(int(val))
+    def set(self, value):
+        super().set(int(value))
 
     def mousedowncommand(self, *args):
         pass
 
 class LabelScale(ttk.Frame):
-    'A scale widget (slider) with a label to indicate its value'
+    "A scale widget (slider) with a label to indicate its value"
 
     def __init__(self, parent, *args, **kwargs):
         super().__init__(parent)
 
-        self._Label = ttk.Label(self, text='')
+        self._Label = ttk.Label(self, text="")
         self._Label.pack()
 
         self._Scale = DelayedScale(self, *args, **kwargs)
         self._Scale.pack()
         self._Scale.mousedowncommand = self._updateLabel
         self._Label.config(text=self._int2label(self._Scale.get()))
 
@@ -81,21 +81,21 @@
         self._Scale.set(val)
 
     def focus_set(self):
         self._Scale.focus_set()
 
     def config(self, *args, **kwargs):
         self._Scale.config(*args, **kwargs)
-            
+
     def bind(self, *args, **kwargs):
         self._Scale.bind(*args, **kwargs)
 
 
 class TextScale(LabelScale):
-    'A scale widget (slider) with text rather than numerical labels'
+    "A scale widget (slider) with text rather than numerical labels"
 
     def __init__(self, parent, *args, textLabels=None, **kwargs):
         self.textLabels = textLabels
         super().__init__(parent, *args, from_=0, to=len(self.textLabels)-1, **kwargs)
 
     def _int2label(self, i):
         return self.textLabels[i]
```

### Comparing `simimg-0.9.1/simimg/classes/fileobject.py` & `simimg-0.9.2/simimg/classes/fileobject.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,129 +1,129 @@
-''' The basic object that represents one file '''
-import os
+""" The basic object that represents one file """
+from functools import cached_property
 import hashlib
+import os
 from datetime import datetime
+
 from PIL import Image, ExifTags
-from ..utils import pillowplus as PP
+
+import simimg.utils.pillowplus as PP
 
 
 class FileObject():
-    ' File object that contains all information relating to one file on disk '
+    " File object that contains all information relating to one file on disk "
 
     def __init__(self, parent, FullPath=None, checksumFilenameDict=None):
         self._Ctrl = parent
         self._Cfg = parent.Cfg
         self.fullPath = FullPath
         self.dirName = os.path.dirname(self.fullPath)
         self.fileName = os.path.basename(self.fullPath)
         dummy, self.fileExtension = os.path.splitext(self.fileName)
 
         self.hashDict = {}
 
-        # These are private variables that allow to call the
-        # corresponding method for cheap
-        # If the variable is None we calculate the value
-        # otherwise we return the value of this private variable
-        self._isImage = None
-        self._checksum = checksumFilenameDict[FullPath] if FullPath in checksumFilenameDict else None
-        self._exifTags = None
-        self._thumbnail = None
-        self._dateTime = None
+        self._checksum = (
+            checksumFilenameDict[FullPath]
+            if FullPath in checksumFilenameDict
+            else None
+        )
         self._size = None
+        self._thumbnail = None
         # It this file active
         self.active = True
 
+    @cached_property
     def isImage(self):
-        ' Set IsImage to True if the file can be read by PIL '
-        if self._isImage is None:
-            try:
-                img = Image.open(self.fullPath)
-                self._isImage = True
-                # do this here to save time
-                self._size = img.size
-            except:
-                self._isImage = False
-        return self._isImage
+        " Set IsImage to True if the file can be read by PIL "
+        try:
+            img = Image.open(self.fullPath)
+            # do this here to save time
+            self._size = img.size
+            return True
+        except:
+            return False
 
     def checksum(self):
         if self._checksum is None:
             hasher = hashlib.sha1()
-            with open(self.fullPath, 'rb') as afile:
+            with open(self.fullPath, "rb") as afile:
                 hasher.update(afile.read())
                 self._checksum = hasher.hexdigest()
         return self._checksum
 
+    @cached_property
     def exifTags(self):
-        if self._exifTags is None:
-            # default to empty basic values
-            self._exifTags = {
-                'Make': '',
-                'Model': '',
-                'DateTimeOriginal': '',
-                'DateTime': '',
-                'DateTimeDigitized': ''
-            }
-            with Image.open(self.fullPath) as image:
-                # image does not have method to get tags
-                if not hasattr(image, '_getexif'):
-                    return self._exifTags
-                exif = image._getexif()
-                # image does not have tags
-                if not exif:
-                    return self._exifTags
-                for key, value in exif.items():
-                    if key in ExifTags.TAGS:
-                        self._exifTags[ExifTags.TAGS[key]] = value
-        return self._exifTags
+        # default to empty basic values
+        exifTags = {
+            "Make": "",
+            "Model": "",
+            "DateTimeOriginal": "",
+            "DateTime": "",
+            "DateTimeDigitized": ""
+        }
+        with Image.open(self.fullPath) as image:
+            # image does not have method to get tags
+            if not hasattr(image, "_getexif"):
+                return exifTags
+            exif = image._getexif()
+            # image does not have tags
+            if not exif:
+                return exifTags
+            for key, value in exif.items():
+                if key in ExifTags.TAGS:
+                    exifTags[ExifTags.TAGS[key]] = value
+            return exifTags
 
     def cameraMake(self):
-        return self.exifTags()['Make']
+        return self.exifTags["Make"]
 
     def cameraModel(self):
-        return self.exifTags()['Model']
+        return self.exifTags["Model"]
 
     def date(self):
-        if self.exifTags()['DateTimeOriginal']:
-            return self.exifTags()['DateTimeOriginal']
-        if self.exifTags()['DateTime']:
-            return self.exifTags()['DateTime']
-        if self.exifTags()['DateTimeDigitized']:
-            return self.exifTags()['DateTimeDigitized']
-        return ''
+        if self.exifTags["DateTimeOriginal"]:
+            return self.exifTags["DateTimeOriginal"]
+        if self.exifTags["DateTime"]:
+            return self.exifTags["DateTime"]
+        if self.exifTags["DateTimeDigitized"]:
+            return self.exifTags["DateTimeDigitized"]
+        return ""
 
+    @cached_property
     def dateTime(self):
-        if self._dateTime is None:
-            thisDateString = self.date()
-            if thisDateString == '':
-                self._dateTime = 'Missing'
-                return self._dateTime
-            try:
-                self._dateTime = datetime.strptime(
-                    thisDateString,
-                    '%Y:%m:%d %H:%M:%S'
-                )
-            except:
-                self._dateTime = 'Missing'
-        return self._dateTime
+        thisDateString = self.date()
+        if thisDateString == "":
+            return "Missing"
+        try:
+            dateTime = datetime.strptime(
+                thisDateString,
+                "%Y:%m:%d %H:%M:%S"
+            )
+        except:
+            return "Missing"
+        return dateTime
 
+    @cached_property
     def size(self):
-        if self._size is None:
-            self._size = (0, 0)
-            with Image.open(self.fullPath) as image:
-                self._size = image.size
-        return self._size
+        if self._size is not None:
+            return self._size
+        my_size = (0, 0)
+        with Image.open(self.fullPath) as image:
+            my_size = image.size
+        return my_size
 
     def shapeParameter(self):
-        w, h = self.size()
+        w, h = self.size
         # (width-height)/(width+height)*100
         # positive for landscape, negative for portait
         return (w-h)/(w+h)*100
 
     def thumbnail(self):
         if self._thumbnail is None:
-            ThumbSize = self._Cfg.get('thumbnailsize')
+            ThumbSize = self._Cfg.get("thumbnailsize")
             self._thumbnail = PP.photoImageOpenAndResizeToFit(
-                self.fullPath,
-                ThumbSize,
-                ThumbSize
-            )
+               self.fullPath,
+               ThumbSize,
+               ThumbSize
+           )
         return self._thumbnail
```

### Comparing `simimg-0.9.1/simimg/classes/imageframe.py` & `simimg-0.9.2/simimg/classes/imageframe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-''' class related to the display of one thumbnail '''
+""" class related to the display of one thumbnail """
 import tkinter as tk
 from tkinter import ttk
 
 
 class ImageFrame(ttk.Frame):
-    ' A frame that holds one image thumbnail with its buttons'
+    " A frame that holds one image thumbnail with its buttons"
 
     def __init__(self, parent, checksum=None, Ctrl=None, X=None, Y=None):
         super().__init__(parent)
 
         self.checksum = checksum
         self.selected = False
         self.X = X
         self.Y = Y
 
         self._Ctrl = Ctrl
-        self._tSize = Ctrl.Cfg.get('thumbnailsize')
+        self._tSize = Ctrl.Cfg.get("thumbnailsize")
         self._text = None
         self._backtext = None
 
         self._thumbCanvas = tk.Canvas(
             self,
             width=self._tSize,
             height=self._tSize
         )
-        self._thumbCanvas.defBgClr = self._thumbCanvas.cget('background')
-        self._thumbCanvas.selBgClr = 'blue'
-        self._thumbCanvas.bind('<Button-1>', self._click)
+        self._thumbCanvas.defBgClr = self._thumbCanvas.cget("background")
+        self._thumbCanvas.selBgClr = "blue"
+        self._thumbCanvas.bind("<Button-1>", self._click)
 
-        self._thumbCanvas.pack(side='top')
+        self._thumbCanvas.pack(side="top")
         self._thumbCanvas.config(highlightthickness=1)
         self._hideButton = ttk.Button(
             self,
-            text='Hide',
+            text="Hide",
             command=self._hide,
-            style='Thumb.TButton'
+            style="Thumb.TButton"
         )
         self._moveButton = ttk.Button(
             self,
-            text='Move',
+            text="Move",
             command=self._move,
-            style='Thumb.TButton'
+            style="Thumb.TButton"
         )
         self._deleteButton = ttk.Button(
             self,
-            text='Delete',
+            text="Delete",
             command=self._delete,
-            style='Thumb.TButton'
+            style="Thumb.TButton"
         )
         self.createThumbContent()
         self.showOptionalElements()
 
     def createThumbContent(self):
-        self._tSize = self._Ctrl.Cfg.get('thumbnailsize')
-        self._thumbCanvas.delete('all')
+        self._tSize = self._Ctrl.Cfg.get("thumbnailsize")
+        self._thumbCanvas.delete("all")
         self._thumbCanvas.config(width=self._tSize, height=self._tSize)
         if self.checksum:
             self._thumbCanvas.create_image(
                 self._tSize/2,
                 self._tSize/2,
-                anchor='center',
+                anchor="center",
                 image=self._Ctrl.FODict[self.checksum][0].thumbnail()
             )
             self._text = self._thumbCanvas.create_text(
                 self._tSize/2,
                 self._tSize,
-                anchor='s',
+                anchor="s",
                 text=self._Ctrl.FODict[self.checksum][0].fileName,
             )
             self._backtext = self._thumbCanvas.create_rectangle(
                 self._thumbCanvas.bbox(self._text),
                 fill=self._thumbCanvas.defBgClr,
                 width=0,
             )
             self._thumbCanvas.tag_lower(self._backtext, self._text)
 
             if len(self._Ctrl.FODict[self.checksum]) > 1:
-                self._thumbCanvas.config(highlightbackground='green', highlightthickness=1)
+                self._thumbCanvas.config(highlightbackground="green", highlightthickness=1)
 
     def showOptionalElements(self):
-        if self._Ctrl.Cfg.get('filenameonthumbnail'):
-            self._thumbCanvas.itemconfigure(self._text, state='normal')
-            self._thumbCanvas.itemconfigure(self._backtext, state='normal')
+        if self._Ctrl.Cfg.get("filenameonthumbnail"):
+            self._thumbCanvas.itemconfigure(self._text, state="normal")
+            self._thumbCanvas.itemconfigure(self._backtext, state="normal")
         else:
-            self._thumbCanvas.itemconfigure(self._text, state='hidden')
-            self._thumbCanvas.itemconfigure(self._backtext, state='hidden')
+            self._thumbCanvas.itemconfigure(self._text, state="hidden")
+            self._thumbCanvas.itemconfigure(self._backtext, state="hidden")
 
-        if self._Ctrl.Cfg.get('showbuttons'):
-            self._hideButton.pack(side='left')
-            self._moveButton.pack(side='left')
-            self._deleteButton.pack(side='left')
+        if self._Ctrl.Cfg.get("showbuttons"):
+            self._hideButton.pack(side="left")
+            self._moveButton.pack(side="left")
+            self._deleteButton.pack(side="left")
         else:
             self._hideButton.pack_forget()
             self._moveButton.pack_forget()
             self._deleteButton.pack_forget()
 
     def _hide(self):
         for fo in self._Ctrl.FODict[self.checksum]:
```

### Comparing `simimg-0.9.1/simimg/classes/miscmodules.py` & `simimg-0.9.2/simimg/classes/miscmodules.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,137 +1,138 @@
-''' Some modules to be put in the left panel that are not related to image matching'''
+""" Some modules to be put in the left panel that are not related to image matching"""
 import os
 import tkinter as tk
 from tkinter import ttk
 from tkinter import filedialog as tkfiledialog
-from ..classes import tooltip as TT
-from . import customscales as CS
+
+import simimg.classes.tooltip as TT
+import simimg.classes.customscales as CS
 
 
 class ThumbOptions(ttk.Frame):
-    ' A frame that holds some options for the thumbnail panels'
+    " A frame that holds some options for the thumbnail panels"
 
     def __init__(self, parent, Controller=None):
         super().__init__(parent)
-        self.config(borderwidth=1, relief='raised')
+        self.config(borderwidth=1, relief="raised")
 
         # keep a handle of the controller object
         self._Ctrl = Controller
 
-        label = ttk.Label(self, text='Output channel')
-        label.pack(fill='x')
-        self.channeltoshow = 'Default'
+        label = ttk.Label(self, text="Output channel")
+        label.pack(fill="x")
+        self.channeltoshow = "Default"
         self._Combo = ttk.Combobox(
             self,
-            values=['Default', 'Hue', 'Saturation', 'Value'],
+            values=["Default", "Hue", "Saturation", "Value"],
             width=15,
         )
         self._Combo.set(self.channeltoshow)
-        self._Combo.config(state='normal')
-        self._Combo.bind('<<ComboboxSelected>>', self._comboChanged)
+        self._Combo.config(state="normal")
+        self._Combo.bind("<<ComboboxSelected>>", self._comboChanged)
         self._Combo.pack()
 
         self.showfilename = tk.BooleanVar()
-        self.showfilename.set(self._Ctrl.Cfg.get('filenameonthumbnail'))
+        self.showfilename.set(self._Ctrl.Cfg.get("filenameonthumbnail"))
         sfn = ttk.Checkbutton(
             self,
-            text='Filenames',
+            text="Filenames",
             variable=self.showfilename,
             command=self._showOptionChanged
         )
-        sfn.pack(fill='x')
-        msg = '''Show the filename on each thumbnail.'''
+        sfn.pack(fill="x")
+        msg = """Show the filename on each thumbnail."""
         TT.Tooltip(sfn, text=msg)
 
         self.showbuttons = tk.BooleanVar()
-        self.showbuttons.set(self._Ctrl.Cfg.get('showbuttons'))
+        self.showbuttons.set(self._Ctrl.Cfg.get("showbuttons"))
         shb = ttk.Checkbutton(
             self,
-            text='Show buttons',
+            text="Show buttons",
             variable=self.showbuttons,
             command=self._showOptionChanged
         )
-        shb.pack(fill='x')
-        msg = 'Show the individual Hide/Move/Delete buttons with each thumbnail'
+        shb.pack(fill="x")
+        msg = "Show the individual Hide/Move/Delete buttons with each thumbnail"
         TT.Tooltip(shb, text=msg)
 
-        label = ttk.Label(self, text='Thumbnail size')
-        label.pack(fill='x')
+        label = ttk.Label(self, text="Thumbnail size")
+        label.pack(fill="x")
 
         sizeVar = tk.IntVar()
-        sizeVar.set(self._Ctrl.Cfg.get('thumbnailsize'))
+        sizeVar.set(self._Ctrl.Cfg.get("thumbnailsize"))
         self._Scale = CS.LabelScale(
             self,
             from_=50,
             to=250,
             resolution=10,
             takefocus=1,
             command=self._scaleChanged,
             variable=sizeVar,
-            orient='horizontal',
+            orient="horizontal",
         )
-        self._Scale.bind('<Control-a>', self._doSelectAll)
+        self._Scale.bind("<Control-a>", self._doSelectAll)
         self._Scale.pack()
 
     def _comboChanged(self, *args):
         self._Combo.focus_set()
         if self.channeltoshow != self._Combo.get():
             self.channeltoshow = self._Combo.get()
-            self._Ctrl.Cfg.set('channeltoshow', self.channeltoshow)
+            self._Ctrl.Cfg.set("channeltoshow", self.channeltoshow)
             self._Ctrl.onThumbParamsChanged()
 
     def _showOptionChanged(self, *args):
-        self._Ctrl.Cfg.set('showbuttons', self.showbuttons.get())
-        self._Ctrl.Cfg.set('filenameonthumbnail', self.showfilename.get())
+        self._Ctrl.Cfg.set("showbuttons", self.showbuttons.get())
+        self._Ctrl.Cfg.set("filenameonthumbnail", self.showfilename.get())
         self._Ctrl.onThumbElementsChanged()
 
     def _scaleChanged(self, *args):
-        self._Ctrl.Cfg.set('thumbnailsize', self._Scale.get())
+        self._Ctrl.Cfg.set("thumbnailsize", self._Scale.get())
         self._Scale.focus_set()
         self._Ctrl.onThumbParamsChanged()
 
     def _doSelectAll(self, *args):
         self._Ctrl.toggleSelectAllThumbnails()
-        return 'break'
+        return "break"
 
 class MovePanel(ttk.Frame):
-    ' A frame that holds a list of target folders for moving files'
+    " A frame that holds a list of target folders for moving files"
 
     def __init__(self, parent, Controller=None):
         super().__init__(parent)
-        self.config(borderwidth=1, relief='raised')
+        self.config(borderwidth=1, relief="raised")
 
         # keep a handle of the controller object
         self._Ctrl = Controller
 
-        self._activeFolder = ''
+        self._activeFolder = ""
         self._folderDict = {}
         self._activeFolderIdx = tk.IntVar()
 
-        for i in range(1, self._Ctrl.Cfg.get('numfolders')+1):
-            txt = 'right-click to set'
-            if self._Ctrl.Cfg.get('restoremovefolders'):
-                fld = self._Ctrl.Cfg.get('folder'+str(i))
+        for i in range(1, self._Ctrl.Cfg.get("numfolders")+1):
+            txt = "right-click to set"
+            if self._Ctrl.Cfg.get("restoremovefolders"):
+                fld = self._Ctrl.Cfg.get("folder"+str(i))
                 if fld:
                     self._folderDict[i] = fld
                     txt = os.path.basename(fld)
             RB = ttk.Radiobutton(
                 self,
                 variable=self._activeFolderIdx,
                 text=txt,
                 command=self._setActiveFolder,
                 value=i
             )
-            RB.pack(anchor='w')
-            RB.bind('<Button-3>', self._changeFolder)
+            RB.pack(anchor="w")
+            RB.bind("<Button-3>", self._changeFolder)
 
     def _setActiveFolder(self):
         if self._activeFolderIdx.get() in self._folderDict:
             self._activeFolder = self._folderDict[self._activeFolderIdx.get()]
-        
+
     def _changeFolder(self, event):
         thisWidgetId = event.widget.cget("value")
         selectedFolder = tkfiledialog.askdirectory(mustexist=False)
         if not selectedFolder:
             return
         # try to create the directory
         if not os.path.isdir(selectedFolder):
@@ -141,15 +142,15 @@
         self._folderDict[thisWidgetId] = selectedFolder
         event.widget.config(text=os.path.basename(selectedFolder))
         # set this button active if none are active
         if self._activeFolderIdx.get() == 0:
             self._activeFolderIdx.set(thisWidgetId)
         # make sure the folder string is updated
         self._setActiveFolder()
-        self._Ctrl.Cfg.set('folder'+str(thisWidgetId), self._activeFolder)
+        self._Ctrl.Cfg.set("folder"+str(thisWidgetId), self._activeFolder)
 
     def get(self, index=None):
         if not index:
             return self._activeFolder
-        if not index in self._folderDict:
+        if index not in self._folderDict:
             return None
         return self._folderDict[index]
```

### Comparing `simimg-0.9.1/simimg/classes/scrollframe.py` & `simimg-0.9.2/simimg/classes/scrollframe.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,47 +3,47 @@
 
 # ************************
 # Scrollable Frame Class
 # ************************
 
 
 class ScrollFrame(ttk.Frame):
-    ''' Frame with two scrollbars
-    to be able to view content bigger than the window. '''
+    """ Frame with two scrollbars
+    to be able to view content bigger than the window. """
 
     def __init__(self, parent):
         super().__init__(parent)
 
         self.canvas = tk.Canvas(self)
         self.viewPort = ttk.Frame(self.canvas)
-        self.hsb = ttk.Scrollbar(self, orient='horizontal', command=self.canvas.xview)
-        self.vsb = ttk.Scrollbar(self, orient='vertical', command=self.canvas.yview)
+        self.hsb = ttk.Scrollbar(self, orient="horizontal", command=self.canvas.xview)
+        self.vsb = ttk.Scrollbar(self, orient="vertical", command=self.canvas.yview)
 
         self.canvas.configure(xscrollcommand=self.hsb.set)
         self.canvas.configure(yscrollcommand=self.vsb.set)
         self.canvas_window = self.canvas.create_window(
             (0, 0),
             window=self.viewPort,
-            anchor='nw',
-            tags='self.viewPort'
+            anchor="nw",
+            tags="self.viewPort"
         )
-        self.viewPort.bind('<Configure>', self._frameConfigure)
-        parent.bind('<MouseWheel>', self._mouseScroll)
-        parent.bind('<Button-4>', self._mouseScroll)
-        parent.bind('<Button-5>', self._mouseScroll)
-        self.hsb.pack(side='bottom', fill='x')
-        self.vsb.pack(side='right', fill='y')
-        self.canvas.pack(side='left', fill='both', expand=True)
-
-    def _frameConfigure(self, event):
-        '''Reset the scroll region to encompass the inner frame'''
-        self.canvas.configure(scrollregion=self.canvas.bbox('all'))
+        self.viewPort.bind("<Configure>", self._frameConfigure)
+        parent.bind("<MouseWheel>", self._mouseScroll)
+        parent.bind("<Button-4>", self._mouseScroll)
+        parent.bind("<Button-5>", self._mouseScroll)
+        self.hsb.pack(side="bottom", fill="x")
+        self.vsb.pack(side="right", fill="y")
+        self.canvas.pack(side="left", fill="both", expand=True)
+
+    def _frameConfigure(self, _):
+        """Reset the scroll region to encompass the inner frame"""
+        self.canvas.configure(scrollregion=self.canvas.bbox("all"))
 
     def _mouseScroll(self, event):
         if event.delta:
-            self.canvas.yview_scroll(int(-1*(event.delta/120)), 'units')
+            self.canvas.yview_scroll(int(-1*(event.delta/120)), "units")
             return
         if event.num == 5:
             move = 1
         else:
             move = -1
-        self.canvas.yview_scroll(move, 'units')
+        self.canvas.yview_scroll(move, "units")
```

### Comparing `simimg-0.9.1/simimg/classes/toolbar.py` & `simimg-0.9.2/simimg/classes/toolbar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,51 @@
-''' Modules that defines a oolbar with action items'''
+""" Modules that defines a oolbar with action items"""
 import os
 from tkinter import ttk
-from . import tooltip as TT
-from ..dialogs import infowindow as IW
-from ..utils import pillowplus as PP
+
+import simimg.classes.tooltip as TT
+import simimg.dialogs.infowindow as IW
+import simimg.utils.pillowplus as PP
 
 
 class Toolbar(ttk.Frame):
-    ' A toolbar frame that holds the action buttons'
+    " A toolbar frame that holds the action buttons"
 
     def __init__(self, parent, Controller=None):
         super().__init__(parent)
 
         self.Ctrl = Controller
-        iconpath = self.Ctrl.Cfg.get('iconpath')
-        self.addImg = PP.photoImageOpen(os.path.join(iconpath, 'add.png'))
-        self.deleteImg = PP.photoImageOpen(os.path.join(iconpath, 'delete.png'))
-        self.moveImg = PP.photoImageOpen(os.path.join(iconpath, 'move.png'))
-        self.exitImg = PP.photoImageOpen(os.path.join(iconpath, 'exit.png'))
-        self.hideImg = PP.photoImageOpen(os.path.join(iconpath, 'hide.png'))
-        self.infoImg = PP.photoImageOpen(os.path.join(iconpath, 'info.png'))
-        self.openImg = PP.photoImageOpen(os.path.join(iconpath, 'open.png'))
-        self.playImg = PP.photoImageOpen(os.path.join(iconpath, 'play.png'))
-        self.refreshImg = PP.photoImageOpen(os.path.join(iconpath, 'refresh.png'))
-        self.settingsImg = PP.photoImageOpen(os.path.join(iconpath, 'settings.png'))
-        self.uncheckImg = PP.photoImageOpen(os.path.join(iconpath, 'uncheck.png'))
+        iconpath = self.Ctrl.Cfg.get("iconpath")
+        self.addImg = PP.photoImageOpen(os.path.join(iconpath, "add.png"))
+        self.deleteImg = PP.photoImageOpen(os.path.join(iconpath, "delete.png"))
+        self.moveImg = PP.photoImageOpen(os.path.join(iconpath, "move.png"))
+        self.exitImg = PP.photoImageOpen(os.path.join(iconpath, "exit.png"))
+        self.hideImg = PP.photoImageOpen(os.path.join(iconpath, "hide.png"))
+        self.infoImg = PP.photoImageOpen(os.path.join(iconpath, "info.png"))
+        self.openImg = PP.photoImageOpen(os.path.join(iconpath, "open.png"))
+        self.playImg = PP.photoImageOpen(os.path.join(iconpath, "play.png"))
+        self.refreshImg = PP.photoImageOpen(os.path.join(iconpath, "refresh.png"))
+        self.settingsImg = PP.photoImageOpen(os.path.join(iconpath, "settings.png"))
+        self.uncheckImg = PP.photoImageOpen(os.path.join(iconpath, "uncheck.png"))
 
-        self.exitButton = ttk.Button(self, image=self.exitImg, style='Picture.TButton', command=self.Ctrl.exitProgram)
-        self.settingsButton = ttk.Button(self, image=self.settingsImg, style='Picture.TButton', command=self.Ctrl.configureProgram)
+        self.exitButton = ttk.Button(self, image=self.exitImg, style="Picture.TButton", command=self.Ctrl.exitProgram)
+        self.settingsButton = ttk.Button(self, image=self.settingsImg, style="Picture.TButton", command=self.Ctrl.configureProgram)
         #
-        self.infoButton = ttk.Button(self, image=self.infoImg, style='Picture.TButton', command=IW.showInfoDialog)
+        self.infoButton = ttk.Button(self, image=self.infoImg, style="Picture.TButton", command=IW.showInfoDialog)
 
-        self.openButton = ttk.Button(self, image=self.openImg, style='Picture.TButton', command=self._openFolder)
-        self.addButton = ttk.Button(self, image=self.addImg, style='Picture.TButton', command=self._addFolder)
+        self.openButton = ttk.Button(self, image=self.openImg, style="Picture.TButton", command=self._openFolder)
+        self.addButton = ttk.Button(self, image=self.addImg, style="Picture.TButton", command=self._addFolder)
         #
-        self.refreshButton = ttk.Button(self, image=self.refreshImg, style='Picture.TButton', command=self.Ctrl.resetThumbnails)
+        self.refreshButton = ttk.Button(self, image=self.refreshImg, style="Picture.TButton", command=self.Ctrl.resetThumbnails)
 
-        self.uncheckButton = ttk.Button(self, image=self.uncheckImg, style='Picture.TButton', command=self.Ctrl.toggleSelectAllThumbnails)
-        self.deleteButton = ttk.Button(self, image=self.deleteImg, style='Picture.TButton', command=self.Ctrl.deleteSelected)
-        self.moveButton = ttk.Button(self, image=self.moveImg, style='Picture.TButton', command=self.Ctrl.moveSelected)
-        self.hideButton = ttk.Button(self, image=self.hideImg, style='Picture.TButton', command=self.Ctrl.hideSelected)
-        self.playButton = ttk.Button(self, image=self.playImg, style='Picture.TButton', command=self.Ctrl.viewSelected)
+        self.uncheckButton = ttk.Button(self, image=self.uncheckImg, style="Picture.TButton", command=self.Ctrl.toggleSelectAllThumbnails)
+        self.deleteButton = ttk.Button(self, image=self.deleteImg, style="Picture.TButton", command=self.Ctrl.deleteSelected)
+        self.moveButton = ttk.Button(self, image=self.moveImg, style="Picture.TButton", command=self.Ctrl.moveSelected)
+        self.hideButton = ttk.Button(self, image=self.hideImg, style="Picture.TButton", command=self.Ctrl.hideSelected)
+        self.playButton = ttk.Button(self, image=self.playImg, style="Picture.TButton", command=self.Ctrl.viewSelected)
 
         self.exitButton.grid(column=0, row=0)
         self.settingsButton.grid(column=1, row=0)
         #
         self.infoButton.grid(column=3, row=0)
 
         self.openButton.grid(column=0, row=1)
@@ -54,24 +55,24 @@
         self.refreshButton.grid(column=3, row=1)
 
         self.deleteButton.grid(column=0, row=2)
         self.moveButton.grid(column=1, row=2)
         self.uncheckButton.grid(column=2, row=2)
         self.playButton.grid(column=3, row=2)
 
-        TT.Tooltip(self.addButton, text='Add folder of images')
-        TT.Tooltip(self.deleteButton, text='Delete Selected Images')
-        TT.Tooltip(self.moveButton, text='Move Selected Images')
-        TT.Tooltip(self.exitButton, text='Quit')
-        TT.Tooltip(self.hideButton, text='Hide Selected Images')
-        TT.Tooltip(self.infoButton, text='Quick instructions')
-        TT.Tooltip(self.openButton, text='Open folder of images')
-        TT.Tooltip(self.playButton, text='View Selected Images')
-        TT.Tooltip(self.refreshButton, text='Start fresh with all images shown')
-        TT.Tooltip(self.settingsButton, text='Settings')
-        TT.Tooltip(self.uncheckButton, text='Select/Unselect all images')
+        TT.Tooltip(self.addButton, text="Add folder of images")
+        TT.Tooltip(self.deleteButton, text="Delete Selected Images")
+        TT.Tooltip(self.moveButton, text="Move Selected Images")
+        TT.Tooltip(self.exitButton, text="Quit")
+        TT.Tooltip(self.hideButton, text="Hide Selected Images")
+        TT.Tooltip(self.infoButton, text="Quick instructions")
+        TT.Tooltip(self.openButton, text="Open folder of images")
+        TT.Tooltip(self.playButton, text="View Selected Images")
+        TT.Tooltip(self.refreshButton, text="Start fresh with all images shown")
+        TT.Tooltip(self.settingsButton, text="Settings")
+        TT.Tooltip(self.uncheckButton, text="Select/Unselect all images")
 
     def _openFolder(self, *args):
-        self.Ctrl.addOrOpenFolder(action='open')
+        self.Ctrl.addOrOpenFolder(action="open")
 
     def _addFolder(self, *args):
-        self.Ctrl.addOrOpenFolder(action='add')
+        self.Ctrl.addOrOpenFolder(action="add")
```

### Comparing `simimg-0.9.1/simimg/classes/tooltip.py` & `simimg-0.9.2/simimg/classes/tooltip.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tkinter as tk
 from tkinter import ttk
 
 
 class Tooltip:
-    '''
+    """
     It creates a tooltip for a given widget as the mouse goes on it.
 
     http://www.daniweb.com/programming/software-development/
            code/484591/a-tooltip-class-for-tkinter
 
     - Originally written by vegaseat on 2014.09.09.
 
@@ -17,36 +17,39 @@
         - to correct extreme right and extreme bottom behavior,
         - to stay inside the screen whenever the tooltip might go out on
           the top but still the screen is higher than the tooltip,
         - to use the more flexible mouse positioning,
         - to add customizable background color, padding, waittime and
           wraplength on creation
       by Alberto Vassena on 2016.11.05.
-    '''
+    """
 
-    def __init__(self, widget,
-                 *,
-                 text='widget info',
-                 waittime=400,
-                 wraplength=250):
+    def __init__(
+            self,
+            widget,
+            *,
+            text="widget info",
+            waittime=400,
+            wraplength=250,
+    ):
 
         self.waittime = waittime  # in miliseconds, originally 500
         self.wraplength = wraplength  # in pixels, originally 180
         self.widget = widget
         self.text = text
-        self.widget.bind('<Enter>', self.onEnter)
-        self.widget.bind('<Leave>', self.onLeave)
-        self.widget.bind('<ButtonPress>', self.onLeave)
+        self.widget.bind("<Enter>", self.onEnter)
+        self.widget.bind("<Leave>", self.onLeave)
+        self.widget.bind("<ButtonPress>", self.onLeave)
         self.id = None
         self.tw = None
 
-    def onEnter(self, event=None):
+    def onEnter(self, _):
         self.schedule()
 
-    def onLeave(self, event=None):
+    def onLeave(self, _):
         self.unschedule()
         self.hide()
 
     def schedule(self):
         self.unschedule()
         self.id = self.widget.after(self.waittime, self.show)
 
@@ -68,20 +71,16 @@
             width, height = (label.winfo_reqwidth(), label.winfo_reqheight())
 
             mouse_x, mouse_y = w.winfo_pointerxy()
 
             x1, y1 = mouse_x + tip_delta[0], mouse_y + tip_delta[1]
             x2, y2 = x1 + width, y1 + height
 
-            x_delta = x2 - s_width
-            if x_delta < 0:
-                x_delta = 0
-            y_delta = y2 - s_height
-            if y_delta < 0:
-                y_delta = 0
+            x_delta = max(x2 - s_width, 0)
+            y_delta = max(y2 - s_height, 0)
 
             offscreen = (x_delta, y_delta) != (0, 0)
 
             if offscreen:
 
                 if x_delta:
                     x1 = mouse_x - tip_delta[0] - width
@@ -113,23 +112,23 @@
         self.tw.wm_overrideredirect(True)
 
         win = ttk.Frame(self.tw)
 
         label = ttk.Label(
             win,
             text=self.text,
-            style='Tooltip.TLabel',
+            style="Tooltip.TLabel",
             wraplength=self.wraplength
         )
 
-        label.grid(sticky='nsew')
+        label.grid(sticky="nsew")
         win.grid()
 
         x, y = tip_pos_calculator(widget, label)
 
-        self.tw.wm_geometry('+%d+%d' % (x, y))
+        self.tw.wm_geometry(f"+{x}+{y}")
 
     def hide(self):
         tw = self.tw
         if tw:
             tw.destroy()
         self.tw = None
```

### Comparing `simimg-0.9.1/simimg/dialogs/configurationwindow.py` & `simimg-0.9.2/simimg/dialogs/configurationwindow.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,167 +1,168 @@
-''' Modules that defines a oolbar with action items'''
+""" Modules that defines a oolbar with action items"""
 import os
 import tkinter as tk
 from tkinter import ttk
 from tkinter import filedialog as tkfiledialog
-from ..classes import tooltip as TT
-from ..utils import pillowplus as PP
+
+import simimg.classes.tooltip as TT
+import simimg.utils.pillowplus as PP
 
 
 class CfgWindow(tk.Toplevel):
     def __init__(self, parent, Controller=None):
         super().__init__()
 
-        self.title('Settings')
+        self.title("Settings")
 
         self.parent = parent
         self.transient(self.parent)
 
         self.Ctrl = Controller
-        iconpath = self.Ctrl.Cfg.get('iconpath')
+        iconpath = self.Ctrl.Cfg.get("iconpath")
 
         self.recurse = tk.BooleanVar()
-        self.recurse.set(self.Ctrl.Cfg.get('searchinsubfolders'))
+        self.recurse.set(self.Ctrl.Cfg.get("searchinsubfolders"))
         self.upscale = tk.BooleanVar()
-        self.upscale.set(self.Ctrl.Cfg.get('upscalethumbnails'))
+        self.upscale.set(self.Ctrl.Cfg.get("upscalethumbnails"))
         self.confirmDel = tk.BooleanVar()
-        self.confirmDel.set(self.Ctrl.Cfg.get('confirmdelete'))
+        self.confirmDel.set(self.Ctrl.Cfg.get("confirmdelete"))
         self.doGzip = tk.BooleanVar()
-        self.doGzip.set(self.Ctrl.Cfg.get('gzipinsteadofdelete'))
+        self.doGzip.set(self.Ctrl.Cfg.get("gzipinsteadofdelete"))
         self.saveSettings = tk.BooleanVar()
-        self.saveSettings.set(self.Ctrl.Cfg.get('savesettings'))
+        self.saveSettings.set(self.Ctrl.Cfg.get("savesettings"))
         self.startupDir = tk.StringVar()
-        self.startupDir.set(self.Ctrl.Cfg.get('startupfolder'))
+        self.startupDir.set(self.Ctrl.Cfg.get("startupfolder"))
         self.restoreFolders = tk.BooleanVar()
-        self.restoreFolders.set(self.Ctrl.Cfg.get('restoremovefolders'))
+        self.restoreFolders.set(self.Ctrl.Cfg.get("restoremovefolders"))
 
         startupFrame = ttk.Frame(self)
-        startupFrame.pack(fill='x', padx=5)
+        startupFrame.pack(fill="x", padx=5)
         startlabel = ttk.Label(
             startupFrame,
-            style='LargeText.TLabel',
-            text='Startup Folder'
+            style="LargeText.TLabel",
+            text="Startup Folder"
         )
         startentry = ttk.Entry(
             startupFrame,
-            font=('', 11),
+            font=("", 11),
             textvariable=self.startupDir
         )
-        self.openImg = PP.photoImageOpenAndResizeToFit(os.path.join(iconpath, 'open.png'), 16 , 16)
+        self.openImg = PP.photoImageOpenAndResizeToFit(os.path.join(iconpath, "open.png"), 16 , 16)
         openbutton = ttk.Button(
             startupFrame,
             image=self.openImg,
-            style='Picture.TButton',
+            style="Picture.TButton",
             command=self._openFolder
         )
-        startlabel.pack(pady=5, side='left')
-        startentry.pack(pady=5, side='left')
-        openbutton.pack(side='left', padx=5)
-        msg = '''Folder to read upon starting the application.
+        startlabel.pack(pady=5, side="left")
+        startentry.pack(pady=5, side="left")
+        openbutton.pack(side="left", padx=5)
+        msg = """Folder to read upon starting the application.
 
 . Means the directory from which the script was started.
 
-Leave empty to start without reading files'''
+Leave empty to start without reading files"""
         TT.Tooltip(startlabel, text=msg)
         TT.Tooltip(startentry, text=msg)
-        TT.Tooltip(openbutton, text='Select Startup Folder')
+        TT.Tooltip(openbutton, text="Select Startup Folder")
 
         clearDBFrame = ttk.Frame(self)
-        clearDBFrame.pack(fill='x', padx=5)
-        self.clearDBImg = PP.photoImageOpen(os.path.join(iconpath, 'refresh.png'))
+        clearDBFrame.pack(fill="x", padx=5)
+        self.clearDBImg = PP.photoImageOpen(os.path.join(iconpath, "refresh.png"))
         clearDBbutton = ttk.Button(
             clearDBFrame,
             image=self.clearDBImg,
-            text='Clear Database',
-            style='LargeText.TButton',
-            compound='left',
+            text="Clear Database",
+            style="LargeText.TButton",
+            compound="left",
             command=self._clearDB
         )
-        clearDBbutton.pack(side='left')
-        msg = 'Empty the database that holds the calculated image properties'
+        clearDBbutton.pack(side="left")
+        msg = "Empty the database that holds the calculated image properties"
         TT.Tooltip(clearDBbutton, text=msg)
 
         toggleFrame = ttk.Frame(self)
-        toggleFrame.pack(fill='x', padx=5)
+        toggleFrame.pack(fill="x", padx=5)
         subdir = ttk.Checkbutton(
             toggleFrame,
-            text='Search in Subfolders',
-            style='LargeText.TCheckbutton',
+            text="Search in Subfolders",
+            style="LargeText.TCheckbutton",
             variable=self.recurse
         )
-        msg = 'Search recursively in the subfolders for image files'
+        msg = "Search recursively in the subfolders for image files"
         TT.Tooltip(subdir, text=msg)
 
         upscale = ttk.Checkbutton(
             toggleFrame,
-            text='Zoom small images as thumbnails',
-            style='LargeText.TCheckbutton',
+            text="Zoom small images as thumbnails",
+            style="LargeText.TCheckbutton",
             variable=self.upscale
         )
-        msg = 'While making thumbnail stretch small images to the thumbnail size'
+        msg = "While making thumbnail stretch small images to the thumbnail size"
         TT.Tooltip(upscale, text=msg)
 
         cnfrm = ttk.Checkbutton(
             toggleFrame,
-            text='Confirm File Delete',
-            style='LargeText.TCheckbutton',
+            text="Confirm File Delete",
+            style="LargeText.TCheckbutton",
             variable=self.confirmDel
         )
-        msg = 'Ask before deleting files'
+        msg = "Ask before deleting files"
         TT.Tooltip(cnfrm, text=msg)
 
         gzp = ttk.Checkbutton(
             toggleFrame,
-            text='Gzip File Instead of Delete',
-            style='LargeText.TCheckbutton',
+            text="Gzip File Instead of Delete",
+            style="LargeText.TCheckbutton",
             variable=self.doGzip
         )
-        msg = 'Instead of deleting the file gzip it (adds .gz to the filename)'
+        msg = "Instead of deleting the file gzip it (adds .gz to the filename)"
         TT.Tooltip(gzp, text=msg)
 
         svs = ttk.Checkbutton(
             toggleFrame,
-            text='Save Settings on Exit',
-            style='LargeText.TCheckbutton',
+            text="Save Settings on Exit",
+            style="LargeText.TCheckbutton",
             variable=self.saveSettings
         )
 
         rfl = ttk.Checkbutton(
             toggleFrame,
-            text='Remember Move Folders',
-            style='LargeText.TCheckbutton',
+            text="Remember Move Folders",
+            style="LargeText.TCheckbutton",
             variable=self.restoreFolders
         )
 
-        subdir.pack(pady=5, anchor='w')
-        upscale.pack(pady=5, anchor='w')
-        cnfrm.pack(pady=5, anchor='w')
-        gzp.pack(pady=5, anchor='w')
-        svs.pack(pady=5, anchor='w')
-        rfl.pack(pady=5, anchor='w')
+        subdir.pack(pady=5, anchor="w")
+        upscale.pack(pady=5, anchor="w")
+        cnfrm.pack(pady=5, anchor="w")
+        gzp.pack(pady=5, anchor="w")
+        svs.pack(pady=5, anchor="w")
+        rfl.pack(pady=5, anchor="w")
 
         btnFrame = ttk.Frame(self)
-        btnFrame.pack(fill='x')
+        btnFrame.pack(fill="x")
         ttk.Button(
             btnFrame,
-            text='Ok',
+            text="Ok",
             width=15,
-            style='LargeText.TButton',
+            style="LargeText.TButton",
             command=self._ok
-        ).pack(padx=10, side='left')
+        ).pack(padx=10, side="left")
         ttk.Button(
             btnFrame,
-            text='Cancel',
+            text="Cancel",
             width=15,
-            style='LargeText.TButton',
+            style="LargeText.TButton",
             command=self._cancel
-        ).pack(padx=10, side='right')
+        ).pack(padx=10, side="right")
 
-        self.bind('<Escape>', self._cancel)
-        self.protocol('WM_DELETE_WINDOW', self._cancel)
+        self.bind("<Escape>", self._cancel)
+        self.protocol("WM_DELETE_WINDOW", self._cancel)
         self.geometry = self.parent.geometry()
         self.grab_set()
         self.wait_window(self)
 
     def _openFolder(self):
         selectedFolder = tkfiledialog.askdirectory()
         if not selectedFolder:
@@ -171,21 +172,21 @@
         self.startupDir.set(selectedFolder)
 
     def _clearDB(self):
         self.Ctrl.stopDatabase()
         self.Ctrl.startDatabase(clear=True)
 
     def _ok(self, *args):
-        self.Ctrl.Cfg.set('searchinsubfolders', self.recurse.get())
-        self.Ctrl.Cfg.set('upscalethumbnails', self.upscale.get())
-        self.Ctrl.Cfg.set('confirmdelete', self.confirmDel.get())
-        self.Ctrl.Cfg.set('gzipinsteadofdelete', self.doGzip.get())
-        self.Ctrl.Cfg.set('savesettings', self.saveSettings.get())
-        self.Ctrl.Cfg.set('restoremovefolders', self.restoreFolders.get())
-        self.Ctrl.Cfg.set('startupfolder', self.startupDir.get())
+        self.Ctrl.Cfg.set("searchinsubfolders", self.recurse.get())
+        self.Ctrl.Cfg.set("upscalethumbnails", self.upscale.get())
+        self.Ctrl.Cfg.set("confirmdelete", self.confirmDel.get())
+        self.Ctrl.Cfg.set("gzipinsteadofdelete", self.doGzip.get())
+        self.Ctrl.Cfg.set("savesettings", self.saveSettings.get())
+        self.Ctrl.Cfg.set("restoremovefolders", self.restoreFolders.get())
+        self.Ctrl.Cfg.set("startupfolder", self.startupDir.get())
         self._returntoparent()
 
     def _cancel(self, *args):
         self._returntoparent()
 
     def _returntoparent(self):
         self.withdraw()
```

### Comparing `simimg-0.9.1/simimg/dialogs/confirmdeletedialog.py` & `simimg-0.9.2/simimg/dialogs/confirmdeletedialog.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 import tkinter as tk
 from tkinter import ttk
 
 
 class CDDialog(tk.Toplevel):
-    def __init__(self, parent, Filename='', simple=False):
+    def __init__(self, parent, Filename="", simple=False):
         super().__init__()
 
-        self.title('Delete File?')
+        self.title("Delete File?")
 
         self.parent = parent
         self.transient(self.parent)
 
         self.result = None
         ttk.Label(
             self,
             text=Filename,
-            style='BoldText.TLabel',
+            style="BoldText.TLabel",
         ).grid(column=0, row=0, columnspan=4, padx=10, pady=10)
         ttk.Button(
             self,
-            text='Yes',
+            text="Yes",
             width=10,
             command=self._yes,
-            style='LargeText.TButton',
-            default='active'
+            style="LargeText.TButton",
+            default="active"
         ).grid(column=0, row=1, padx=10)
         ttk.Button(
             self,
-            text='No',
+            text="No",
             width=10,
-            style='LargeText.TButton',
+            style="LargeText.TButton",
             command=self._no
         ).grid(column=1, row=1, padx=10)
         if not simple:
             ttk.Button(
                 self,
-                text='Yes to All',
+                text="Yes to All",
                 width=10,
-                style='LargeText.TButton',
+                style="LargeText.TButton",
                 command=self._yes_to_all
             ).grid(column=2, row=1, padx=10)
             ttk.Button(
                 self,
-                text='Abort',
+                text="Abort",
                 width=10,
-                style='LargeText.TButton',
+                style="LargeText.TButton",
                 command=self._abort
             ).grid(column=3, row=1, padx=10)
 
-        self.bind('<Return>', self._yes)
-        self.bind('<Escape>', self._abort)
-        self.protocol('WM_DELETE_WINDOW', self._abort)
+        self.bind("<Return>", self._yes)
+        self.bind("<Escape>", self._abort)
+        self.protocol("WM_DELETE_WINDOW", self._abort)
 
         self.grab_set()
         self.wait_window(self)
 
     def _yes(self, *args):
-        self.result = 'yes'
+        self.result = "yes"
         self._returntoparent()
 
     def _yes_to_all(self, *args):
-        self.result = 'yestoall'
+        self.result = "yestoall"
         self._returntoparent()
 
     def _no(self, *args):
-        self.result = 'no'
+        self.result = "no"
         self._returntoparent()
 
     def _abort(self, *args):
-        self.result = 'abort'
+        self.result = "abort"
         self._returntoparent()
 
     def _returntoparent(self):
         self.withdraw()
         self.update_idletasks()
         self.parent.focus_set()
         self.destroy()
```

### Comparing `simimg-0.9.1/simimg/dialogs/infowindow.py` & `simimg-0.9.2/simimg/dialogs/infowindow.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from tkinter import messagebox as tkmessagebox
 
 def showInfoDialog():
-    ''' show basic info about this program '''
-    msg = '''
+    """ show basic info about this program """
+    msg = """
 SiMilar ImaGe finder:
 
 This program is designed to display groups of pictures that are similar.
 In particular, it aims to group together pictures that show the same scene.
 The use case is to be able to quickly inspect these pictures and keep only the best ones.
 
 The program in not designed to find copies of the same image that have been slightly altered or identical copies, although it can be use for this. 
@@ -16,9 +16,9 @@
 * Activate some selection criterion of the left by clicking on its label
 * Adapt the parameters
 * The matching groups are updated
 
 * Select images by clicking on the thumbnail (background turns blue)
 * Click the play button to inspect the selected images
 * Click the delete button to delete selected images
-    '''
-    tkmessagebox.showinfo('Information', msg)
+    """
+    tkmessagebox.showinfo("Information", msg)
```

### Comparing `simimg-0.9.1/simimg/dialogs/viewer.py` & `simimg-0.9.2/simimg/dialogs/viewer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-''' Module for show the viewer window '''
+""" Module for show the viewer window """
 import tkinter as tk
 from tkinter import messagebox as tkmessagebox
-from ..utils import pillowplus as PP
+
+import simimg.utils.pillowplus as PP
 
 
 class Viewer(tk.Toplevel):
-    'A viewer window to display the selected pictures'
+    "A viewer window to display the selected pictures"
 
     def __init__(self, Fileinfo=None, Controller=None):
         super().__init__()
 
         self._checksums, self._filenames = map(list, zip(*Fileinfo))
 
         self._Ctrl = Controller
 
-        self.geometry(self._Ctrl.Cfg.get('viewergeometry'))
-        self.protocol('WM_DELETE_WINDOW', self._exitViewer)
+        self.geometry(self._Ctrl.Cfg.get("viewergeometry"))
+        self.protocol("WM_DELETE_WINDOW", self._exitViewer)
 
         self._ImgDict = {}
         self._ImgIndex = 0
         # the pillow image object (not scaled photoimage)
         self._Img = None
 
         self._zoomLevelDict = {
@@ -31,42 +32,42 @@
             6: 100,
             }
         self._zoomLevel = 0
         self._zoomImg = None
         self._zoomImgId = None
 
         self._keyDict = {
-            'space': self._showNext,
-            'n': self._showNext,
-            'Right': self._showNext,
-            'p': self._showPrevious,
-            'Left': self._showPrevious,
-            'd': self._deleteFile,
-            'Delete': self._deleteFile,
-            'h': self._showHelp,
-            'm': self._moveFile,
-            'F1': self._showHelp,
-            'q': self._exitViewer,
-            'Escape': self._exitViewer
+            "space": self._showNext,
+            "n": self._showNext,
+            "Right": self._showNext,
+            "p": self._showPrevious,
+            "Left": self._showPrevious,
+            "d": self._deleteFile,
+            "Delete": self._deleteFile,
+            "h": self._showHelp,
+            "m": self._moveFile,
+            "F1": self._showHelp,
+            "q": self._exitViewer,
+            "Escape": self._exitViewer
             }
-        for i in range(1, self._Ctrl.Cfg.get('numfolders')+1):
+        for i in range(1, self._Ctrl.Cfg.get("numfolders")+1):
             self._keyDict.update({str(i): lambda idx=i: self._moveFile(index=idx)})
-        self.bind('<Key>', self._key)
+        self.bind("<Key>", self._key)
 
         self._canvas = tk.Canvas(self)
-        self._canvas.pack(fill='both', expand=True)
+        self._canvas.pack(fill="both", expand=True)
         self._canvas.update_idletasks()
-        self._canvas.bind('<Button-1>', self._click)
-        self._canvas.bind('<Button-3>', self._click)
+        self._canvas.bind("<Button-1>", self._click)
+        self._canvas.bind("<Button-3>", self._click)
         self._canvas.bind("<Button-4>", self._changeZoom)
         self._canvas.bind("<Button-5>", self._changeZoom)
         self._canvas.bind("<MouseWheel>", self._changeZoom)
         self._canvas.bind("<Motion>", self._showZoom)
 
-        self.bind('<Configure>', self._showImage)
+        self.bind("<Configure>", self._showImage)
 
     def _fillImgDict(self, Index):
         maxW = self._canvas.winfo_width()
         maxH = self._canvas.winfo_height()
         # check if this image already exists?
         if Index in self._ImgDict:
             File, Img, W, H, targetW, targetH = self._ImgDict[Index]
@@ -101,27 +102,29 @@
     # keys
     def _key(self, event):
         if event.keysym not in self._keyDict:
             return
         self._keyDict[event.keysym]()
 
     def _showImage(self, *args):
-        self._canvas.delete('all')
+        self._canvas.delete("all")
         # unset the Image object
         self._Img = None
         # reset the zoom level
         self._zoomLevel = 0
         self._fillImgDict(self._ImgIndex)
         self._canvas.create_image(
             self._canvas.winfo_width()/2,
             self._canvas.winfo_height()/2,
-            anchor='center',
+            anchor="center",
             image=self._ImgDict[self._ImgIndex][1],
         )
-        self.title('Similar Image Viewer: %s --- Press F1 for Help' % self._ImgDict[self._ImgIndex][0])
+        self.title(
+            f"Similar Image Viewer: {self._ImgDict[self._ImgIndex][0]} --- Press F1 for Help"
+        )
 
     def _showNext(self):
         self._ImgIndex += 1
         self._ImgIndex = self._ImgIndex % len(self._filenames)
         # if the filename is none skip to next
         if self._filenames[self._ImgIndex] is None:
             self._showNext()
@@ -216,20 +219,20 @@
         # take ROI of the original image and scale it
         self._zoomImg = PP.TkPhotoImage(
             PP.imageResize(self._Img.crop((X0, Y0, X1, Y1)), zoomSize, zoomSize)
             )
         self._zoomImgId = self._canvas.create_image(
             event.x,
             event.y,
-            anchor='center',
+            anchor="center",
             image=self._zoomImg
         )
 
     def _showHelp(self):
-        msg = '''
+        msg = """
 SiMilar ImaGe viewer:
 
 This windows show the selected images to be able to compare them.
 The mouse allow to browse though the images:
 Left button: forward
 Right button: backward
 The scrollwheel allow to zoom on part of the image
@@ -238,14 +241,14 @@
 i, F1: show this help
 n, Right, Spacebar: show the next image
 p, Left: show the previous images
 d, Delete: delete the file from your hard disk!
 m: move the file to the folder set in the main window
 <n>: move the file to the folder #n move panel of the main window
 q, Escape: quit the viewer
-'''
-        tkmessagebox.showinfo('Information', msg, parent=self)
+"""
+        tkmessagebox.showinfo("Information", msg, parent=self)
 
     def _exitViewer(self):
-        self._Ctrl.Cfg.set('viewergeometry', self.geometry())
+        self._Ctrl.Cfg.set("viewergeometry", self.geometry())
         del self._ImgDict
         self.destroy()
```

### Comparing `simimg-0.9.1/simimg/icons/add.png` & `simimg-0.9.2/simimg/icons/add.png`

 * *Files identical despite different names*

### Comparing `simimg-0.9.1/simimg/icons/delete.png` & `simimg-0.9.2/simimg/icons/delete.png`

 * *Files identical despite different names*

### Comparing `simimg-0.9.1/simimg/icons/exit.png` & `simimg-0.9.2/simimg/icons/exit.png`

 * *Files identical despite different names*

### Comparing `simimg-0.9.1/simimg/icons/info.png` & `simimg-0.9.2/simimg/icons/info.png`

 * *Files identical despite different names*

### Comparing `simimg-0.9.1/simimg/icons/move.png` & `simimg-0.9.2/simimg/icons/move.png`

 * *Files identical despite different names*

### Comparing `simimg-0.9.1/simimg/icons/open.png` & `simimg-0.9.2/simimg/icons/open.png`

 * *Files identical despite different names*

### Comparing `simimg-0.9.1/simimg/icons/refresh.png` & `simimg-0.9.2/simimg/icons/refresh.png`

 * *Files identical despite different names*

### Comparing `simimg-0.9.1/simimg/icons/settings.png` & `simimg-0.9.2/simimg/icons/settings.png`

 * *Files identical despite different names*

### Comparing `simimg-0.9.1/simimg/icons/simimg.png` & `simimg-0.9.2/simimg/icons/simimg.png`

 * *Files identical despite different names*

### Comparing `simimg-0.9.1/simimg/icons/uncheck.png` & `simimg-0.9.2/simimg/icons/uncheck.png`

 * *Files identical despite different names*

### Comparing `simimg-0.9.1/simimg/simimg.py` & `simimg-0.9.2/simimg/simimg.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,82 @@
-''' Project to display similar images from an image catalog '''
+""" Project to display similar images from an image catalog """
 import os
 import tkinter as tk
 from tkinter import ttk
-from .classes import configuration as CONF
-from .classes import controller as CTRL
-from .classes import scrollframe as SF
+
+import simimg.classes.configuration as CONF
+import simimg.classes.controller as CTRL
+import simimg.classes.scrollframe as SF
 
 
 class simim_app(tk.Tk):
-    ''' Main window for sorting and managing pictures'''
+    """ Main window for sorting and managing pictures"""
 
     def __init__(self, ScriptPath=None):
         # do what any TK app does
         super().__init__()
 
         # Do nothing much but creating the objects
         # it is those objects that will implement the
         # working of the App.
 
         # Object that hold configuration database
         self.Cfg = CONF.Configuration(ScriptPath=ScriptPath)
 
-        self.title('Similar Image Finder')
-        self.tk.call('wm', 'iconphoto', self._w,
+        self.title("Similar Image Finder")
+        self.tk.call("wm", "iconphoto", self._w,
                      tk.PhotoImage(
-                         file=os.path.join(self.Cfg.get('iconpath'),'simimg.png')
+                         file=os.path.join(self.Cfg.get("iconpath"), "simimg.png")
                      )
-        )
-        self.geometry(self.Cfg.get('findergeometry'))
+                     )
+        self.geometry(self.Cfg.get("findergeometry"))
 
         # ttk widget style section
         style = ttk.Style()
-        style.configure('LargeText.TButton', font=('', 11))
-        style.configure('LargeText.TLabel', font=('', 11))
+        style.configure("LargeText.TButton", font=("", 11))
+        style.configure("LargeText.TLabel", font=("", 11))
         style.configure(
-            'HeaderText.TLabel',
-            font=('', 11),
-            foreground=self.cget('background'),
-            background='darkblue',
-            anchor='center',
+            "HeaderText.TLabel",
+            font=("", 11),
+            foreground=self.cget("background"),
+            background="darkblue",
+            anchor="center",
         )
-        style.configure('LargeText.TCheckbutton', font=('', 11))
-        style.configure('BoldText.TLabel', font=('', 12, 'bold'))
+        style.configure("LargeText.TCheckbutton", font=("", 11))
+        style.configure("BoldText.TLabel", font=("", 12, "bold"))
 
-        style.configure('Picture.TButton', relief='flat', padding=0)
+        style.configure("Picture.TButton", relief="flat", padding=0)
         style.configure(
-            'Thumb.TButton',
-            relief='flat',
+            "Thumb.TButton",
+            relief="flat",
             padding=0,
-            font=('', 8),
+            font=("", 8),
             width=-1
         )
 
-        style.configure('Tooltip.TLabel',
-                        background='#FFFFE1',
+        style.configure("Tooltip.TLabel",
+                        background="#FFFFE1",
                         padding=3,
-                        relief='solid',
+                        relief="solid",
                         borderwidth=1,
-                        font=('', 11),
+                        font=("", 11),
                         )
 
-        self.Statusbar = ttk.Label(self, text='...', relief='sunken')
-        self.Statusbar.pack(side='bottom', fill='x')
+        self.Statusbar = ttk.Label(self, text="...", relief="sunken")
+        self.Statusbar.pack(side="bottom", fill="x")
         self.ModulePane = ttk.Frame(self)
-        self.ModulePane.pack(side='left', fill='y')
+        self.ModulePane.pack(side="left", fill="y")
         self.ThumbPane = SF.ScrollFrame(self)
-        self.ThumbPane.pack(side='right', fill='both', expand=True)
+        self.ThumbPane.pack(side="right", fill="both", expand=True)
         # The object responsible for dealing with the data
         # and the display of those data
         self.Ctrl = CTRL.Controller(self)
 
 
 def main():
     scriptpath = os.path.join(os.path.dirname(os.path.realpath(__file__)))
     app = simim_app(ScriptPath=scriptpath)
     app.mainloop()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `simimg-0.9.1/simimg/utils/handyfunctions.py` & `simimg-0.9.2/simimg/utils/handyfunctions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,104 @@
-''' library of little function to make code more readable'''
-import os
+""" library of little function to make code more readable"""
 import gzip
+import os
 import shutil
 
 
 def hexstring2array(hexstring):
-    '''convert a hexstring to an array
-    (each pair of letters represents one element) <255'''
+    """convert a hexstring to an array
+    (each pair of letters represents one element) <255"""
     return [int(hexstring[i:i+2], 16) for i in range(0, len(hexstring), 2)]
 
 
 def array2hexstring(array):
-    '''convert an array to a hexstring
-    (each pair of letters represents one element)'''
-    return ''.join(format(round(i), 'x').zfill(2) for i in array)
+    """convert an array to a hexstring
+    (each pair of letters represents one element)"""
+    return "".join(format(round(i), "x").zfill(2) for i in array)
 
 
 def pairlist2dict(lst):
-    '''take a list containing key,values pairs and return
+    """take a list containing key,values pairs and return
     a dict where each key holds a list of matching values.
-    '''
+    """
     dct = {}
     for ky, vle in lst:
         if ky in dct:
             dct[ky].append(vle)
         else:
             dct[ky] = [vle]
     return dct
 
 
 def stringlist2commonunique(sl):
-    '''split list of strings (filenames) into a common part and unique part
+    """split list of strings (filenames) into a common part and unique part
     like ["/home/user/pictures/pic1.jpg", "/home/user/pictures/pic2.jpg"]
     =>
     ("/home/user/pictures/pic", ["1.jpg","2.jpg"])
-    '''
+    """
 
     # break the list of string into tuples of letters for each position
     letterTupleList = map(list, zip(*sl))
-    common = ''
+    common = ""
     for letterTuple in letterTupleList:
         # if there is more than one letter in the set of letters
         # it means that the filenames start to differ at this position.
         if len(set(letterTuple)) > 1:
             break
         common += letterTuple[0]
     unique = [s[len(common):] for s in sl]
     return (common, unique)
 
 
 def gzipfile(file):
-    try:
-        f_in = open(file, 'rb')
-        f_out = gzip.open(file+'.gz', 'wb')
-        shutil.copyfileobj(f_in, f_out)
-        f_out.close()
-        f_in.close()
-        os.remove(file)
-    except:
-        f_out.close()
-        f_in.close()
+    with open(file, "rb") as f_in:
+        with gzip.open(file+".gz", "wb") as f_out:
+            shutil.copyfileobj(f_in, f_out)
+            os.remove(file)
 
 
 def mergeGroupDicts(ListGDict):
-    ''' this routine takes a list of group dicts
+    """ this routine takes a list of group dicts
     each element containing a dict of matching images
     returned by a condition modules.
 
     So if for example the date module returned:
     GL1 = { 1:{1,2,3}, 2:{2,3,6}, 5:{5,6} }
     and the hash module returned:
     GL2 = { 2:{2,3,4}, 5:{5,6}, 6:{6,7} }
     the ListGDict will be [G1, G2]
 
     This function should return the union of each by element:
     GL = { 1:{1,2,3}, 2:{2,3,4,6}, 5:{5,6}, 6:{6,7} }
-    '''
+    """
     GDict = {}
     for d in ListGDict:
         for m, g in d.items():
             previous = GDict[m] if m in GDict else set()
             GDict[m] = previous | g
     return GDict
 
 
 def applyMMGroupDicts(GDict, ListGDict):
-    ''' this routine take a group dict and a list of group dicts
+    """ this routine take a group dict and a list of group dicts
     The first list contains groups of images that matched at least one
     active condition.
     The list of dicts contains groups that statisfy an mustmatch condition.
     We want to keep only the intersection of both element by element
-    '''
+    """
     for k in GDict:
         for mmDict in ListGDict:
             mmSet = mmDict[k] if k in mmDict else set()
             GDict[k] = GDict[k] & mmSet
     # remove sets with less than two element
     return {k: v for k, v in GDict.items() if len(v) > 1}
 
 
 def removeRedunantSubgroups(GDict):
-    ''' Remove groups that exists entirely as subgroups elsewhere'''
+    """ Remove groups that exists entirely as subgroups elsewhere"""
     # We sort by reverse length of the groups so we know that
     # subgroups can only be found later in the list
     checksums_sorted_by_length_of_group = sorted(
         GDict,
         key=lambda k: len(GDict[k]),
         reverse=True
     )
@@ -114,15 +108,15 @@
         if existsAsSubGroup(GDict[m], cleanedGDict.values()):
             continue
         cleanedGDict[m] = GDict[m]
     return cleanedGDict
 
 
 def existsAsSubGroup(g, GL):
-    'Test whether G exists as a subgroup in any of the groups in GL'
+    "Test whether G exists as a subgroup in any of the groups in GL"
     for G in GL:
         if g - G == set():
             return True
     return False
 
 
 def sortMatchingGroupsByFilename(GDict, filenameChecksumDict):
```

### Comparing `simimg-0.9.1/simimg/utils/pillowplus.py` & `simimg-0.9.2/simimg/utils/pillowplus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-''' Some some utililty for reading and dealing with pillow images'''
+""" Some some utililty for reading and dealing with pillow images"""
 from PIL import Image, ImageTk, ImageChops
 
 pillowplus_table16 = [i/256 for i in range(65536)]
 
 
 def imageOpen(fn):
     try:
         img = Image.open(fn)
         if (
-                img.format == 'PNG' and
-                img.mode == 'I' and
+                img.format == "PNG" and
+                img.mode == "I" and
                 max(img.getdata()) > 255
         ):
-            img = img.point(pillowplus_table16, 'L')
+            img = img.point(pillowplus_table16, "L")
     except:
         return None
     return img
 
 
 def imageResize(img, w, h):
     try:
@@ -35,15 +35,15 @@
     return imageResize(imageOpen(fn), w, h)
 
 
 def imageOpenAndResizeToFit(fn, w, h):
     return imageResizeToFit(imageOpen(fn), w, h)
 
 def TkPhotoImage(img):
-    try: 
+    try:
         return ImageTk.PhotoImage(img)
     except:
         return None
 
 def photoImageOpen(fn):
     img = imageOpen(fn)
     if not img:
@@ -70,50 +70,50 @@
     if not img:
         return None
 
     try:
         # this is needed because thumbnail does not check that the file can
         # be actually loaded
         img.load()
-        # if upscale is true and image is smaller than requested 
+        # if upscale is true and image is smaller than requested
         if upscale and img.size[0] < w and img.size[1] < h:
             # scale up
             img = imageResizeToFit(img, w, h)
         else:
             # scale down
             img.thumbnail((w, h))
-    except Exception:
+    except:
         return None
 
     if (
             not channel or
-            channel == 'Default' or
+            channel == "Default" or
             len(img.getbands()) == 1
     ):
         return img
 
     try:
-        hsv = img.split() if img.getbands() == ('H', 'S', 'V') else img.convert('HSV').split()
+        hsv = img.split() if img.getbands() == ("H", "S", "V") else img.convert("HSV").split()
     except:
         return img
 
-    if channel == 'Hue':
+    if channel == "Hue":
         img = Image.merge(
-            'HSV',
+            "HSV",
             (
                 hsv[0],
                 ImageChops.constant(hsv[0], 255),
                 ImageChops.constant(hsv[0], 255),
             )
             )
-    if channel == 'Saturation':
+    if channel == "Saturation":
         img = hsv[1]
-    if channel == 'Value':
+    if channel == "Value":
         img = hsv[2]
     return img
 
 
 def photoThumbnailOpen(fn, w, h, channel=None, upscale=False):
-    img = thumbnailOpen(fn, w, h, channel=channel, upscale=False)
+    img = thumbnailOpen(fn, w, h, channel=channel, upscale=upscale)
     if not img:
         return None
     return TkPhotoImage(img)
```

### Comparing `simimg-0.9.1/simimg/utils/pooling.py` & `simimg-0.9.2/simimg/utils/pooling.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-''' Functions on the image files that take time.
-    Like file-hashing and image-hashing
-    They are organised to be done in multiprocessing.'''
-import hashlib
-from operator import add
+"""Functions on the image files that take time. Like file-hashing and
+image-hashing They are organised to be done in multiprocessing.
+
+"""
 import functools
+import hashlib
 from multiprocessing import Pool
+from operator import add
+
 from PIL import Image
-from . import database as DB
-from . import pillowplus as PP
+
+import simimg.utils.database as DB
+import simimg.utils.pillowplus as PP
 
 # box that contains the whole image
 onebox = [(0.0, 0.0, 1.0, 1.0)]
 
 # size of boxes that has ~equal amount over overlap between the boxes
 # and the amount of unsampled area
 fiveboxsize = 0.46
@@ -34,43 +37,43 @@
 def statsQuantiles(a):
     aa = sorted(a)
     return [aa[round(len(aa)*i)] for i in [0.25, 0.5, 0.75]]
 
 
 def calculateChecksum(file):
     hasher = hashlib.sha1()
-    with open(file, 'rb') as afile:
+    with open(file, "rb") as afile:
         hasher.update(afile.read())
     return (file, hasher.hexdigest())
 
 
 def getChecksums(filelist, hashValueDict):
-    '''return checksum hashing value for each file the list.'''
+    """return checksum hashing value for each file the list."""
     missingfilelist = list(set(filelist) - set(hashValueDict.keys()))
     with Pool() as pool:
         calculatedHashes = pool.map(calculateChecksum, missingfilelist)
     hashValueDict.update(calculatedHashes)
     return hashValueDict
 
 
 def subImage(Img, FracBox):
-    'return a subImage from Image based on coordinates in dimensionless units'
+    "return a subImage from Image based on coordinates in dimensionless units"
     width, height = Img.size
     left = round(width*FracBox[0])
     right = round(width*FracBox[2])
     bottom = round(height*FracBox[1])
     top = round(height*FracBox[3])
     return Img.crop((left, bottom, right, top))
 
 
 def colorHash(Img, colorspace=None, five=False):
-    ''' Regrouped colour hashing function to avoid repeating code.'''
+    """ Regrouped colour hashing function to avoid repeating code."""
 
     # requested colorspace defaults to HSV
-    cspace = colorspace if colorspace else 'HSV'
+    cspace = colorspace if colorspace else "HSV"
     # one box or five boxes requested
     boxes = fiveboxes if five else onebox
 
     # The image is not in the requested mode, convert
     if not Img.mode == cspace:
         Img = Img.convert(cspace)
 
@@ -82,56 +85,56 @@
 
     values = []
     # get measurements for each box
     for bx in boxes:
         # get a measurement for each channel
         for idx, ch in enumerate(channels):
             data = subImage(ch, bx)
-            if cspace == 'HSV' and idx == 1:
+            if cspace == "HSV" and idx == 1:
                 data = list(data)
                 medianH = statsMedian(data)
                 quant = statsQuantiles([(h-medianH+128) % 255 for h in data])
                 values.append(round(medianH))
                 values.append(round(quant[2] - quant[0]))
             else:
                 quant = statsQuantiles(data)
                 values.append(round(quant[1]))
                 values.append(round(quant[2] - quant[0]))
     return values
 
 
 def hsvHash(Img):
-    return colorHash(Img, colorspace='HSV', five=False)
+    return colorHash(Img, colorspace="HSV", five=False)
 
 
 def hsv5Hash(Img):
-    return colorHash(Img, colorspace='HSV', five=True)
+    return colorHash(Img, colorspace="HSV", five=True)
 
 
 def rgbHash(Img):
-    return colorHash(Img, colorspace='RGB', five=False)
+    return colorHash(Img, colorspace="RGB", five=False)
 
 
 def rgb5Hash(Img):
-    return colorHash(Img, colorspace='RGB', five=True)
+    return colorHash(Img, colorspace="RGB", five=True)
 
 
 def lHash(Img):
-    return colorHash(Img, colorspace='L', five=False)
+    return colorHash(Img, colorspace="L", five=False)
 
 
 def l5Hash(Img):
-    return colorHash(Img, colorspace='L', five=True)
+    return colorHash(Img, colorspace="L", five=True)
 
 
 def dHash(Img, doVertical=False):
     if doVertical:
-        i8x8 = Img.convert('L').resize((8, 9), Image.BOX).transpose(Image.ROTATE_90)
+        i8x8 = Img.convert("L").resize((8, 9), Image.BOX).transpose(Image.ROTATE_90)
     else:
-        i8x8 = Img.convert('L').resize((9, 8), Image.BOX)
+        i8x8 = Img.convert("L").resize((9, 8), Image.BOX)
 
     values = []
     for y in range(8):
         val = functools.reduce(
             add,
             [(i8x8.getpixel((x+1, y)) > i8x8.getpixel((x, y)))*(2**x) for x in range(8)]
         )
@@ -146,29 +149,29 @@
 def dHashVertical(Img):
     return dHash(Img, doVertical=True)
 
 
 def calculateHash(args):
     checksum, fullPath, hashName = args
     funcdict = {
-        'HSV': hsvHash,
-        'HSV (5 regions)': hsv5Hash,
-        'RGB': rgbHash,
-        'RGB (5 regions)': rgb5Hash,
-        'Luminosity': lHash,
-        'Luminosity (5 regions)': l5Hash,
-        'Horizontal': dHashHorizontal,
-        'Vertical': dHashVertical,
-        }
+        "HSV": hsvHash,
+        "HSV (5 regions)": hsv5Hash,
+        "RGB": rgbHash,
+        "RGB (5 regions)": rgb5Hash,
+        "Luminosity": lHash,
+        "Luminosity (5 regions)": l5Hash,
+        "Horizontal": dHashHorizontal,
+        "Vertical": dHashVertical,
+    }
     return (checksum, funcdict[hashName](PP.imageOpen(fullPath)))
 
 
 def getHashes(FODict, hashName, db_connection=None):
-    '''return hashing value according to selected hashName method
-    for each file the (file,checksum) list.'''
+    """return hashing value according to selected hashName method
+    for each file the (file,checksum) list."""
 
     # create an empty dict to hold the results
     hashValueDict = {} # checksum:hashValue
 
     # create an empty list to hold checksum,file,hashName tuples
     # that need to be calculated
     needCalculating = []
@@ -222,15 +225,18 @@
         tsize,
         channel=channel,
         upscale=upscale
     )
     return (checksum, img)
 
 
-def getThumbnails(FODict, Thumbsize=None, channel='Default', upscale=False):
-    '''return thumbnail for each checksum in FODict.'''
-    args = [(checksum, fo[0].fullPath, Thumbsize, channel, upscale) for checksum, fo in FODict.items()]
+def getThumbnails(FODict, Thumbsize=None, channel="Default", upscale=False):
+    """return thumbnail for each checksum in FODict."""
+    args = [
+        (checksum, fo[0].fullPath, Thumbsize, channel, upscale)
+        for checksum, fo in FODict.items()
+    ]
     with Pool() as pool:
         calculatedthumbs = pool.map(getOneThumb, args)
     ThumbDict = {}
     ThumbDict.update(calculatedthumbs)
     return ThumbDict
```

