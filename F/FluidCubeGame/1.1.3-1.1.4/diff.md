# Comparing `tmp/FluidCubeGame-1.1.3.tar.gz` & `tmp/FluidCubeGame-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FluidCubeGame-1.1.3.tar", last modified: Sat Jun 24 14:13:36 2023, max compression
+gzip compressed data, was "FluidCubeGame-1.1.4.tar", last modified: Sat Jun 24 14:30:08 2023, max compression
```

## Comparing `FluidCubeGame-1.1.3.tar` & `FluidCubeGame-1.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:13:36.658473 FluidCubeGame-1.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:13:36.658473 FluidCubeGame-1.1.3/FluidCubeGame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-24 14:13:36.000000 FluidCubeGame-1.1.3/FluidCubeGame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-24 14:13:36.000000 FluidCubeGame-1.1.3/FluidCubeGame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:13:36.000000 FluidCubeGame-1.1.3/FluidCubeGame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 14:13:36.000000 FluidCubeGame-1.1.3/FluidCubeGame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-24 14:13:36.000000 FluidCubeGame-1.1.3/FluidCubeGame.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-24 14:13:36.658473 FluidCubeGame-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-24 14:12:07.000000 FluidCubeGame-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:13:36.658473 FluidCubeGame-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-24 14:12:07.000000 FluidCubeGame-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:13:36.654472 FluidCubeGame-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:13:36.658473 FluidCubeGame-1.1.3/src/FluidCubeGame/
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-24 14:12:07.000000 FluidCubeGame-1.1.3/src/FluidCubeGame/FluidCube.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-24 14:12:07.000000 FluidCubeGame-1.1.3/src/FluidCubeGame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-24 14:12:07.000000 FluidCubeGame-1.1.3/src/FluidCubeGame/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:30:07.995787 FluidCubeGame-1.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:30:07.995787 FluidCubeGame-1.1.4/FluidCubeGame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-24 14:30:07.000000 FluidCubeGame-1.1.4/FluidCubeGame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-24 14:30:07.000000 FluidCubeGame-1.1.4/FluidCubeGame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:30:07.000000 FluidCubeGame-1.1.4/FluidCubeGame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-24 14:30:07.000000 FluidCubeGame-1.1.4/FluidCubeGame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-24 14:30:07.000000 FluidCubeGame-1.1.4/FluidCubeGame.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-24 14:30:07.995787 FluidCubeGame-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-24 14:28:43.000000 FluidCubeGame-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:30:07.995787 FluidCubeGame-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-24 14:28:43.000000 FluidCubeGame-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:30:07.995787 FluidCubeGame-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:30:07.995787 FluidCubeGame-1.1.4/src/FluidCubeGame/
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-24 14:28:43.000000 FluidCubeGame-1.1.4/src/FluidCubeGame/FluidCube.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-24 14:28:43.000000 FluidCubeGame-1.1.4/src/FluidCubeGame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-24 14:28:43.000000 FluidCubeGame-1.1.4/src/FluidCubeGame/main.py
```

### Comparing `FluidCubeGame-1.1.3/README.md` & `FluidCubeGame-1.1.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 
 ----------------------------------------------------------------
 
 ## Запуск приложения
 <br>
 
 > Для установки приложения Вам необходимо создать любую папку
-> Запустить командную строку Windows
-> Ввести последовательно команды:
-  1) cd C:\Путь до папки
-  2) python -m venv env
-  3) cd C:\Путь до папки\env\Scripts
-  4) activate.bat
-  5) pip install fluidCube
-  6) Затем зайди в любой компилятор Python и ввести код:
-     from fluidCube import main
+> Открыть эту папку через любой компилятор, например, VS Code
+> Создать новый терминал и ввести последовательно команды:
+  1) python -m venv env
+  3) cd ./env/Scripts
+  4) ./activate.bat
+  5) pip install FluidCubeGame
+  6) Затем в этой же папке создать любой файл *.py с следющим содержанием:
+     
+     from src.FluidCubeGame.main import main
 
      main()
-  7) Запустить программу
+  8) Запустить программу
 
 ### Docker-образ
 > Ссылка на скачивание - https://hub.docker.com/r/megasear/fluidcube
 >
 > Для самостоятельной сборки Docker образа можно использовать Dockerfile.
 > 
 > $ docker build . -t fluidSimulator
```

### Comparing `FluidCubeGame-1.1.3/src/FluidCubeGame/FluidCube.py` & `FluidCubeGame-1.1.4/src/FluidCubeGame/FluidCube.py`

 * *Files identical despite different names*

### Comparing `FluidCubeGame-1.1.3/src/FluidCubeGame/main.py` & `FluidCubeGame-1.1.4/src/FluidCubeGame/main.py`

 * *Files identical despite different names*

