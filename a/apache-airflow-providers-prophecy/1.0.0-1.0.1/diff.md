# Comparing `tmp/apache-airflow-providers-prophecy-1.0.0.tar.gz` & `tmp/apache-airflow-providers-prophecy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-prophecy-1.0.0.tar", last modified: Fri Jun 23 09:49:51 2023, max compression
+gzip compressed data, was "apache-airflow-providers-prophecy-1.0.1.tar", last modified: Sat Jun 24 10:21:21 2023, max compression
```

## Comparing `apache-airflow-providers-prophecy-1.0.0.tar` & `apache-airflow-providers-prophecy-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sumit      (501) staff       (20)        0 2023-06-23 09:49:51.147466 apache-airflow-providers-prophecy-1.0.0/
--rw-r--r--   0 sumit      (501) staff       (20)      308 2023-06-23 09:49:51.147329 apache-airflow-providers-prophecy-1.0.0/PKG-INFO
--rw-r--r--   0 sumit      (501) staff       (20)       27 2023-06-23 05:14:33.000000 apache-airflow-providers-prophecy-1.0.0/README.md
-drwxr-xr-x   0 sumit      (501) staff       (20)        0 2023-06-23 09:49:51.146621 apache-airflow-providers-prophecy-1.0.0/apache_airflow_providers_prophecy.egg-info/
--rw-r--r--   0 sumit      (501) staff       (20)      308 2023-06-23 09:49:51.000000 apache-airflow-providers-prophecy-1.0.0/apache_airflow_providers_prophecy.egg-info/PKG-INFO
--rw-r--r--   0 sumit      (501) staff       (20)      421 2023-06-23 09:49:51.000000 apache-airflow-providers-prophecy-1.0.0/apache_airflow_providers_prophecy.egg-info/SOURCES.txt
--rw-r--r--   0 sumit      (501) staff       (20)        1 2023-06-23 09:49:51.000000 apache-airflow-providers-prophecy-1.0.0/apache_airflow_providers_prophecy.egg-info/dependency_links.txt
--rw-r--r--   0 sumit      (501) staff       (20)       87 2023-06-23 09:49:51.000000 apache-airflow-providers-prophecy-1.0.0/apache_airflow_providers_prophecy.egg-info/entry_points.txt
--rw-r--r--   0 sumit      (501) staff       (20)       22 2023-06-23 09:49:51.000000 apache-airflow-providers-prophecy-1.0.0/apache_airflow_providers_prophecy.egg-info/requires.txt
--rw-r--r--   0 sumit      (501) staff       (20)       18 2023-06-23 09:49:51.000000 apache-airflow-providers-prophecy-1.0.0/apache_airflow_providers_prophecy.egg-info/top_level.txt
-drwxr-xr-x   0 sumit      (501) staff       (20)        0 2023-06-23 09:49:51.146999 apache-airflow-providers-prophecy-1.0.0/prophecy_provider/
--rw-r--r--   0 sumit      (501) staff       (20)      243 2023-06-23 07:46:16.000000 apache-airflow-providers-prophecy-1.0.0/prophecy_provider/__init__.py
--rw-r--r--   0 sumit      (501) staff       (20)     1838 2023-06-23 09:06:01.000000 apache-airflow-providers-prophecy-1.0.0/prophecy_provider/emailer.py
--rw-r--r--   0 sumit      (501) staff       (20)       38 2023-06-23 09:49:51.147516 apache-airflow-providers-prophecy-1.0.0/setup.cfg
--rw-r--r--   0 sumit      (501) staff       (20)      708 2023-06-23 08:59:38.000000 apache-airflow-providers-prophecy-1.0.0/setup.py
+drwxr-xr-x   0 sumit      (501) staff       (20)        0 2023-06-24 10:21:21.715056 apache-airflow-providers-prophecy-1.0.1/
+-rw-r--r--   0 sumit      (501) staff       (20)      308 2023-06-24 10:21:21.714923 apache-airflow-providers-prophecy-1.0.1/PKG-INFO
+-rw-r--r--   0 sumit      (501) staff       (20)       27 2023-06-23 05:14:33.000000 apache-airflow-providers-prophecy-1.0.1/README.md
+drwxr-xr-x   0 sumit      (501) staff       (20)        0 2023-06-24 10:21:21.714194 apache-airflow-providers-prophecy-1.0.1/apache_airflow_providers_prophecy.egg-info/
+-rw-r--r--   0 sumit      (501) staff       (20)      308 2023-06-24 10:21:21.000000 apache-airflow-providers-prophecy-1.0.1/apache_airflow_providers_prophecy.egg-info/PKG-INFO
+-rw-r--r--   0 sumit      (501) staff       (20)      421 2023-06-24 10:21:21.000000 apache-airflow-providers-prophecy-1.0.1/apache_airflow_providers_prophecy.egg-info/SOURCES.txt
+-rw-r--r--   0 sumit      (501) staff       (20)        1 2023-06-24 10:21:21.000000 apache-airflow-providers-prophecy-1.0.1/apache_airflow_providers_prophecy.egg-info/dependency_links.txt
+-rw-r--r--   0 sumit      (501) staff       (20)       87 2023-06-24 10:21:21.000000 apache-airflow-providers-prophecy-1.0.1/apache_airflow_providers_prophecy.egg-info/entry_points.txt
+-rw-r--r--   0 sumit      (501) staff       (20)       22 2023-06-24 10:21:21.000000 apache-airflow-providers-prophecy-1.0.1/apache_airflow_providers_prophecy.egg-info/requires.txt
+-rw-r--r--   0 sumit      (501) staff       (20)       18 2023-06-24 10:21:21.000000 apache-airflow-providers-prophecy-1.0.1/apache_airflow_providers_prophecy.egg-info/top_level.txt
+drwxr-xr-x   0 sumit      (501) staff       (20)        0 2023-06-24 10:21:21.714663 apache-airflow-providers-prophecy-1.0.1/prophecy_provider/
+-rw-r--r--   0 sumit      (501) staff       (20)      243 2023-06-23 07:46:16.000000 apache-airflow-providers-prophecy-1.0.1/prophecy_provider/__init__.py
+-rw-r--r--   0 sumit      (501) staff       (20)     1793 2023-06-24 10:20:32.000000 apache-airflow-providers-prophecy-1.0.1/prophecy_provider/emailer.py
+-rw-r--r--   0 sumit      (501) staff       (20)       38 2023-06-24 10:21:21.715093 apache-airflow-providers-prophecy-1.0.1/setup.cfg
+-rw-r--r--   0 sumit      (501) staff       (20)      708 2023-06-24 10:21:14.000000 apache-airflow-providers-prophecy-1.0.1/setup.py
```

### Comparing `apache-airflow-providers-prophecy-1.0.0/prophecy_provider/emailer.py` & `apache-airflow-providers-prophecy-1.0.1/prophecy_provider/emailer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 import smtplib
-import logging
-from typing import Iterable, Any
+from typing import Any, Dict, Iterable, List, Union
 
 from airflow.utils.email import build_mime_message
 from airflow.configuration import conf
 from airflow.hooks.base import BaseHook
 
-log = logging.getLogger(__name__)
-
 
 def send_email(
-        to: list[str] | Iterable[str],
-        subject: str,
-        html_content: str,
-        files: list[str] | None = None,
-        dryrun: bool = False,
-        cc: str | Iterable[str] | None = None,
-        bcc: str | Iterable[str] | None = None,
-        mime_subtype: str = 'mixed',
-        mime_charset: str = 'utf-8',
-        conn_id: str | None = None,
-        custom_headers: dict[str, Any] | None = None,
-        **kwargs,
+    to: Union[List[str], Iterable[str]],
+    subject: str,
+    html_content: str,
+    files: Union[List[str], None] = None,
+    dryrun: bool = False,
+    cc: Union[str, Iterable[str], None] = None,
+    bcc: Union[str, Iterable[str], None] = None,
+    mime_subtype: str = 'mixed',
+    mime_charset: str = 'utf-8',
+    conn_id: Union[str, None] = None,
+    custom_headers: Union[Dict[str, Any], None] = None,
+    **kwargs,
 ):
     backend_conn_id = conn_id or conf.get("email", "email_conn_id", fallback=None)
     from_email = conf.get('email', 'from_email', fallback=None)
 
     if backend_conn_id is None:
         raise Exception(
             "Please set email.email_conn_id Airflow configuration"
```

### Comparing `apache-airflow-providers-prophecy-1.0.0/setup.py` & `apache-airflow-providers-prophecy-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='apache-airflow-providers-prophecy',
-    version='1.0.0',
+    version='1.0.1',
     description='Your provider package for Apache Airflow',
     packages=find_packages(),
     install_requires=[
         'apache-airflow>=2.2.0'
         # Add any additional dependencies required by your provider
     ],
     classifiers=[
```

