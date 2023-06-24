# Comparing `tmp/xiaowupkg-1.0.4.tar.gz` & `tmp/xiaowupkg-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaowupkg-1.0.4.tar", last modified: Fri Jun  9 08:08:03 2023, max compression
+gzip compressed data, was "xiaowupkg-1.0.5.tar", last modified: Sat Jun 24 07:16:06 2023, max compression
```

## Comparing `xiaowupkg-1.0.4.tar` & `xiaowupkg-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 08:08:03.417691 xiaowupkg-1.0.4/
--rw-rw-rw-   0        0        0      158 2023-06-09 08:08:03.395745 xiaowupkg-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      105 2023-06-01 09:52:58.000000 xiaowupkg-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-09 08:08:03.418686 xiaowupkg-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      350 2023-06-09 08:07:14.000000 xiaowupkg-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:08:03.380786 xiaowupkg-1.0.4/xiaowupkg/
--rw-rw-rw-   0        0        0      193 2023-06-01 09:50:19.000000 xiaowupkg-1.0.4/xiaowupkg/__init__.py
--rw-rw-rw-   0        0        0      697 2023-06-01 06:46:27.000000 xiaowupkg-1.0.4/xiaowupkg/filefunc.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:08:03.395745 xiaowupkg-1.0.4/xiaowupkg.egg-info/
--rw-rw-rw-   0        0        0      158 2023-06-09 08:08:03.000000 xiaowupkg-1.0.4/xiaowupkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-06-09 08:08:03.000000 xiaowupkg-1.0.4/xiaowupkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 08:08:03.000000 xiaowupkg-1.0.4/xiaowupkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-09 08:08:03.000000 xiaowupkg-1.0.4/xiaowupkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 07:16:06.096831 xiaowupkg-1.0.5/
+-rw-rw-rw-   0        0        0      158 2023-06-24 07:16:06.095834 xiaowupkg-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-06-16 08:20:18.000000 xiaowupkg-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-24 07:16:06.096831 xiaowupkg-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      401 2023-06-24 07:15:43.000000 xiaowupkg-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:16:06.080884 xiaowupkg-1.0.5/xiaowupkg/
+-rw-rw-rw-   0        0        0     6062 2023-06-24 07:05:38.000000 xiaowupkg-1.0.5/xiaowupkg/UIfunc.py
+-rw-rw-rw-   0        0        0      379 2023-06-24 07:09:01.000000 xiaowupkg-1.0.5/xiaowupkg/__init__.py
+-rw-rw-rw-   0        0        0     1229 2023-06-20 07:52:36.000000 xiaowupkg-1.0.5/xiaowupkg/filefunc.py
+drwxrwxrwx   0        0        0        0 2023-06-24 07:16:06.095834 xiaowupkg-1.0.5/xiaowupkg.egg-info/
+-rw-rw-rw-   0        0        0      158 2023-06-24 07:16:06.000000 xiaowupkg-1.0.5/xiaowupkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-24 07:16:06.000000 xiaowupkg-1.0.5/xiaowupkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 07:16:06.000000 xiaowupkg-1.0.5/xiaowupkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-24 07:16:06.000000 xiaowupkg-1.0.5/xiaowupkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-24 07:16:06.000000 xiaowupkg-1.0.5/xiaowupkg.egg-info/top_level.txt
```

