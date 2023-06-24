# Comparing `tmp/w3bstream-client-python-0.1.0.tar.gz` & `tmp/w3bstream_client_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w3bstream-client-python-0.1.0.tar", last modified: Sat Jun 24 06:04:40 2023, max compression
+gzip compressed data, was "w3bstream_client_python-0.2.0.tar", last modified: Sat Jun 24 06:13:49 2023, max compression
```

## Comparing `w3bstream-client-python-0.1.0.tar` & `w3bstream_client_python-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 06:04:40.817942 w3bstream-client-python-0.1.0/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      184 2023-06-24 06:04:40.817942 w3bstream-client-python-0.1.0/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-06-24 06:04:40.817942 w3bstream-client-python-0.1.0/setup.cfg
--rw-r--r--   0 haaai     (1000) haaai     (1000)      201 2023-06-24 06:04:36.000000 w3bstream-client-python-0.1.0/setup.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 06:04:40.817942 w3bstream-client-python-0.1.0/w3bstream-client-python/
--rw-r--r--   0 haaai     (1000) haaai     (1000)       49 2023-06-24 01:11:11.000000 w3bstream-client-python-0.1.0/w3bstream-client-python/__init__.py
--rw-r--r--   0 haaai     (1000) haaai     (1000)      875 2023-06-24 06:02:38.000000 w3bstream-client-python-0.1.0/w3bstream-client-python/client.py
-drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 06:04:40.817942 w3bstream-client-python-0.1.0/w3bstream_client_python.egg-info/
--rw-r--r--   0 haaai     (1000) haaai     (1000)      184 2023-06-24 06:04:40.000000 w3bstream-client-python-0.1.0/w3bstream_client_python.egg-info/PKG-INFO
--rw-r--r--   0 haaai     (1000) haaai     (1000)      266 2023-06-24 06:04:40.000000 w3bstream-client-python-0.1.0/w3bstream_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-06-24 06:04:40.000000 w3bstream-client-python-0.1.0/w3bstream_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-06-24 06:04:40.000000 w3bstream-client-python-0.1.0/w3bstream_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 06:13:49.407914 w3bstream_client_python-0.2.0/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-24 06:13:49.407914 w3bstream_client_python-0.2.0/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       38 2023-06-24 06:13:49.407914 w3bstream_client_python-0.2.0/setup.cfg
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      205 2023-06-24 06:13:35.000000 w3bstream_client_python-0.2.0/setup.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 06:13:49.407914 w3bstream_client_python-0.2.0/w3bstream_client_python/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       49 2023-06-24 01:11:11.000000 w3bstream_client_python-0.2.0/w3bstream_client_python/__init__.py
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      875 2023-06-24 06:07:28.000000 w3bstream_client_python-0.2.0/w3bstream_client_python/client.py
+drwxr-xr-x   0 haaai     (1000) haaai     (1000)        0 2023-06-24 06:13:49.407914 w3bstream_client_python-0.2.0/w3bstream_client_python.egg-info/
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      188 2023-06-24 06:13:49.000000 w3bstream_client_python-0.2.0/w3bstream_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 haaai     (1000) haaai     (1000)      266 2023-06-24 06:13:49.000000 w3bstream_client_python-0.2.0/w3bstream_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)        1 2023-06-24 06:13:49.000000 w3bstream_client_python-0.2.0/w3bstream_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 haaai     (1000) haaai     (1000)       24 2023-06-24 06:13:49.000000 w3bstream_client_python-0.2.0/w3bstream_client_python.egg-info/top_level.txt
```

### Comparing `w3bstream-client-python-0.1.0/w3bstream-client-python/client.py` & `w3bstream_client_python-0.2.0/w3bstream_client_python/client.py`

 * *Files identical despite different names*

