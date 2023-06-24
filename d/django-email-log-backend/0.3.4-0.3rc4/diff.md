# Comparing `tmp/django-email-log-backend-0.3.4.tar.gz` & `tmp/django-email-log-backend-0.3rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-email-log-backend-0.3.4.tar", last modified: Sat Jun 24 05:54:58 2023, max compression
+gzip compressed data, was "dist/django-email-log-backend-0.3rc4.tar", last modified: Sat Apr  3 19:12:24 2021, max compression
```

## Comparing `django-email-log-backend-0.3.4.tar` & `django-email-log-backend-0.3rc4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.913991 django-email-log-backend-0.3.4/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2017-10-20 12:24:14.000000 django-email-log-backend-0.3.4/.editorconfig
--rw-r--r--   0 mirec     (1000) mirec     (1000)       84 2023-05-15 09:56:03.000000 django-email-log-backend-0.3.4/.gitignore
--rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2017-10-20 12:24:14.000000 django-email-log-backend-0.3.4/AUTHORS
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1060 2021-04-03 16:00:19.000000 django-email-log-backend-0.3.4/LICENSE
--rw-r--r--   0 mirec     (1000) mirec     (1000)      291 2017-10-20 12:24:14.000000 django-email-log-backend-0.3.4/MANIFEST.in
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1672 2023-06-24 05:54:58.913991 django-email-log-backend-0.3.4/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)      973 2023-05-30 04:07:47.000000 django-email-log-backend-0.3.4/README.rst
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.912991 django-email-log-backend-0.3.4/django_email_log/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      104 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1827 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/admin.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      344 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/apps.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1693 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/backends.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1282 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/checks.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.910991 django-email-log-backend-0.3.4/django_email_log/locale/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.910991 django-email-log-backend-0.3.4/django_email_log/locale/sk_SK/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.912991 django-email-log-backend-0.3.4/django_email_log/locale/sk_SK/LC_MESSAGES/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1527 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/locale/sk_SK/LC_MESSAGES/django.mo
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1886 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/locale/sk_SK/LC_MESSAGES/django.po
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.912991 django-email-log-backend-0.3.4/django_email_log/migrations/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1023 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/migrations/0001_initial.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     3442 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/migrations/0002_auto_20210321_1145.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/migrations/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     5053 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/models.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      387 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/settings.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.910991 django-email-log-backend-0.3.4/django_email_log/static/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.910991 django-email-log-backend-0.3.4/django_email_log/static/django_email_log/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.912991 django-email-log-backend-0.3.4/django_email_log/static/django_email_log/css/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2420 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/static/django_email_log/css/admin.css
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.912991 django-email-log-backend-0.3.4/django_email_log/status_handlers/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/status_handlers/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      522 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/status_handlers/base.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1200 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/status_handlers/celery.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.910991 django-email-log-backend-0.3.4/django_email_log/templates/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.910991 django-email-log-backend-0.3.4/django_email_log/templates/admin/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.910991 django-email-log-backend-0.3.4/django_email_log/templates/admin/django_email_log/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.912991 django-email-log-backend-0.3.4/django_email_log/templates/admin/django_email_log/email/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4074 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/templates/admin/django_email_log/email/change_form.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      210 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/templates/admin/django_email_log/email/change_list.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      431 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/templates/admin/django_email_log/email/part_tree.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      368 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/urls.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      546 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/utils.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2191 2023-06-24 05:52:15.000000 django-email-log-backend-0.3.4/django_email_log/views.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-06-24 05:54:58.913991 django-email-log-backend-0.3.4/django_email_log_backend.egg-info/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1672 2023-06-24 05:54:58.000000 django-email-log-backend-0.3.4/django_email_log_backend.egg-info/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1177 2023-06-24 05:54:58.000000 django-email-log-backend-0.3.4/django_email_log_backend.egg-info/SOURCES.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-06-24 05:54:58.000000 django-email-log-backend-0.3.4/django_email_log_backend.egg-info/dependency_links.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       17 2023-06-24 05:54:58.000000 django-email-log-backend-0.3.4/django_email_log_backend.egg-info/top_level.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-06-24 05:54:58.913991 django-email-log-backend-0.3.4/setup.cfg
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1964 2023-06-24 05:54:52.000000 django-email-log-backend-0.3.4/setup.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.236062 django-email-log-backend-0.3rc4/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2017-10-20 12:24:14.000000 django-email-log-backend-0.3rc4/.editorconfig
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       78 2021-04-03 15:44:24.000000 django-email-log-backend-0.3rc4/.gitignore
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2017-10-20 12:24:14.000000 django-email-log-backend-0.3rc4/AUTHORS
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1060 2021-04-03 16:00:19.000000 django-email-log-backend-0.3rc4/LICENSE
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      291 2017-10-20 12:24:14.000000 django-email-log-backend-0.3rc4/MANIFEST.in
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1992 2021-04-03 19:12:24.236062 django-email-log-backend-0.3rc4/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      936 2021-04-03 19:11:39.000000 django-email-log-backend-0.3rc4/README.rst
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.234063 django-email-log-backend-0.3rc4/django_email_log/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       55 2017-10-20 12:24:14.000000 django-email-log-backend-0.3rc4/django_email_log/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1827 2021-03-21 20:19:19.000000 django-email-log-backend-0.3rc4/django_email_log/admin.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      344 2021-04-03 15:23:07.000000 django-email-log-backend-0.3rc4/django_email_log/apps.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1633 2021-04-03 15:35:04.000000 django-email-log-backend-0.3rc4/django_email_log/backends.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1282 2021-04-03 15:58:37.000000 django-email-log-backend-0.3rc4/django_email_log/checks.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.231063 django-email-log-backend-0.3rc4/django_email_log/locale/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.231063 django-email-log-backend-0.3rc4/django_email_log/locale/sk_SK/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.234063 django-email-log-backend-0.3rc4/django_email_log/locale/sk_SK/LC_MESSAGES/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1527 2021-04-03 19:11:57.000000 django-email-log-backend-0.3rc4/django_email_log/locale/sk_SK/LC_MESSAGES/django.mo
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1886 2021-03-21 19:40:09.000000 django-email-log-backend-0.3rc4/django_email_log/locale/sk_SK/LC_MESSAGES/django.po
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.234063 django-email-log-backend-0.3rc4/django_email_log/migrations/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1023 2020-01-23 09:18:27.000000 django-email-log-backend-0.3rc4/django_email_log/migrations/0001_initial.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1831 2021-03-21 21:02:49.000000 django-email-log-backend-0.3rc4/django_email_log/migrations/0002_auto_20210321_1145.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2017-10-20 12:24:14.000000 django-email-log-backend-0.3rc4/django_email_log/migrations/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     5056 2021-04-03 13:57:42.000000 django-email-log-backend-0.3rc4/django_email_log/models.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      387 2021-04-03 06:52:01.000000 django-email-log-backend-0.3rc4/django_email_log/settings.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.231063 django-email-log-backend-0.3rc4/django_email_log/static/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.231063 django-email-log-backend-0.3rc4/django_email_log/static/django_email_log/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.234063 django-email-log-backend-0.3rc4/django_email_log/static/django_email_log/css/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2420 2021-03-21 20:17:36.000000 django-email-log-backend-0.3rc4/django_email_log/static/django_email_log/css/admin.css
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.235062 django-email-log-backend-0.3rc4/django_email_log/status_handlers/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2021-04-03 06:42:44.000000 django-email-log-backend-0.3rc4/django_email_log/status_handlers/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      456 2021-04-03 06:43:48.000000 django-email-log-backend-0.3rc4/django_email_log/status_handlers/base.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1144 2021-04-03 15:12:27.000000 django-email-log-backend-0.3rc4/django_email_log/status_handlers/celery.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.231063 django-email-log-backend-0.3rc4/django_email_log/templates/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.231063 django-email-log-backend-0.3rc4/django_email_log/templates/admin/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.231063 django-email-log-backend-0.3rc4/django_email_log/templates/admin/django_email_log/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.235062 django-email-log-backend-0.3rc4/django_email_log/templates/admin/django_email_log/email/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4069 2021-03-21 19:58:56.000000 django-email-log-backend-0.3rc4/django_email_log/templates/admin/django_email_log/email/change_form.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      191 2021-03-21 20:10:25.000000 django-email-log-backend-0.3rc4/django_email_log/templates/admin/django_email_log/email/change_list.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      431 2021-03-21 18:52:13.000000 django-email-log-backend-0.3rc4/django_email_log/templates/admin/django_email_log/email/part_tree.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      368 2021-03-21 14:45:11.000000 django-email-log-backend-0.3rc4/django_email_log/urls.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      546 2021-04-03 15:32:50.000000 django-email-log-backend-0.3rc4/django_email_log/utils.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2191 2021-03-21 21:06:56.000000 django-email-log-backend-0.3rc4/django_email_log/views.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2021-04-03 19:12:24.236062 django-email-log-backend-0.3rc4/django_email_log_backend.egg-info/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1992 2021-04-03 19:12:24.000000 django-email-log-backend-0.3rc4/django_email_log_backend.egg-info/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1177 2021-04-03 19:12:24.000000 django-email-log-backend-0.3rc4/django_email_log_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2021-04-03 19:12:24.000000 django-email-log-backend-0.3rc4/django_email_log_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       17 2021-04-03 19:12:24.000000 django-email-log-backend-0.3rc4/django_email_log_backend.egg-info/top_level.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2021-04-03 19:12:24.236062 django-email-log-backend-0.3rc4/setup.cfg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1965 2021-04-03 19:12:09.000000 django-email-log-backend-0.3rc4/setup.py
```

### Comparing `django-email-log-backend-0.3.4/LICENSE` & `django-email-log-backend-0.3rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-email-log-backend-0.3.4/PKG-INFO` & `django-email-log-backend-0.3rc4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,64 @@
 Metadata-Version: 2.1
 Name: django-email-log-backend
-Version: 0.3.4
+Version: 0.3rc4
 Summary: Django email log backend
 Home-page: https://github.com/mireq/django-email-log-backend
 Author: Miroslav Bendík
 Author-email: miroslav.bendik@gmail.com
+License: UNKNOWN
+Description: ============================
+        Django database email logger
+        ============================
+        
+        Install
+        -------
+        
+        `pip install django-email-log-backend.git`
+        
+        or
+        
+        `pip install -e 'git+https://github.com/mireq/django-email-log-backend.git#egg=django_email_log_backend'`
+        
+        Usage
+        -----
+        
+        Settings
+        ^^^^^^^^
+        
+        .. code:: python
+        
+        	INSTALLED_APPS = (
+        		# ...
+        		'django_email_log',
+        	)
+        
+        	EMAIL_BACKEND = 'django_email_log.backends.EmailBackend'
+        	EMAIL_LOG_BACKEND = 'django.core.mail.backends.console.EmailBackend'
+        
+        Emails are forwarded to `EMAIL_LOG_BACKEND`.
+        
+        .. code:: python
+        
+        	# urls.py
+        	urlpatterns = [
+        		# ...
+        		url(r'^django-email-log/', include('django_email_log.urls')),
+        	]
+        
+        .. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg1.png?v2020-04-03
+        
+        .. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg2.png?v2020-04-03
+        
+        .. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg3.png?v2020-04-03
+        
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS
-
-============================
-Django database email logger
-============================
-
-Install
--------
-
-.. code:: bash
-
-	pip install django-email-log-backend
-
-or
-
-.. code:: bash
-
-	pip install -e 'git+https://github.com/mireq/django-email-log-backend.git#egg=django_email_log_backend'
-
-Settings
-^^^^^^^^
-
-.. code:: python
-
-	INSTALLED_APPS = (
-		# ...
-		'django_email_log',
-	)
-
-	EMAIL_BACKEND = 'django_email_log.backends.EmailBackend'
-	EMAIL_LOG_BACKEND = 'django.core.mail.backends.console.EmailBackend'
-
-Emails are forwarded to `EMAIL_LOG_BACKEND`.
-
-.. code:: python
-
-	# urls.py
-	urlpatterns = [
-		# ...
-		path('django-email-log/', include('django_email_log.urls')),
-	]
-
-Screenshots
-^^^^^^^^^^^
-
-.. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg1.png?v2020-04-03
-
-.. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg2.png?v2020-04-03
-
-.. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg3.png?v2020-04-03
```

### Comparing `django-email-log-backend-0.3.4/README.rst` & `django-email-log-backend-0.3rc4/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 ============================
 Django database email logger
 ============================
 
 Install
 -------
 
-.. code:: bash
-
-	pip install django-email-log-backend
+`pip install django-email-log-backend.git`
 
 or
 
-.. code:: bash
+`pip install -e 'git+https://github.com/mireq/django-email-log-backend.git#egg=django_email_log_backend'`
 
-	pip install -e 'git+https://github.com/mireq/django-email-log-backend.git#egg=django_email_log_backend'
+Usage
+-----
 
 Settings
 ^^^^^^^^
 
 .. code:: python
 
 	INSTALLED_APPS = (
@@ -31,18 +30,15 @@
 Emails are forwarded to `EMAIL_LOG_BACKEND`.
 
 .. code:: python
 
 	# urls.py
 	urlpatterns = [
 		# ...
-		path('django-email-log/', include('django_email_log.urls')),
+		url(r'^django-email-log/', include('django_email_log.urls')),
 	]
 
-Screenshots
-^^^^^^^^^^^
-
 .. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg1.png?v2020-04-03
 
 .. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg2.png?v2020-04-03
 
 .. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg3.png?v2020-04-03
```

### Comparing `django-email-log-backend-0.3.4/django_email_log/admin.py` & `django-email-log-backend-0.3rc4/django_email_log/admin.py`

 * *Files identical despite different names*

### Comparing `django-email-log-backend-0.3.4/django_email_log/backends.py` & `django-email-log-backend-0.3rc4/django_email_log/backends.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,15 @@
 			message.connection = self.connection
 			email = self.get_email_instance(message)
 			current_message.set(email)
 			try:
 				num_sent += self.process_status(message.send(), email)
 			except Exception:
 				logger.exception("Wrong e-mail status value", extra={'value': num_sent})
-			if email is not None:
-				email.save()
+			email.save()
 		return num_sent
 
 	def get_email_instance(self, message):
 		if hasattr(message, 'model_instance'):
 			model_instance = message.model_instance
 		else:
 			try:
@@ -47,10 +46,9 @@
 				extra = {'email': message}
 				logger.exception("E-mail message not serialized", extra=extra)
 				model_instance = Email(
 					subject='<error>',
 					date_sent=timezone.now(),
 					status=Email.STATUS_FAIL
 				)
-		if model_instance is not None:
-			model_instance.original_message = message
+		model_instance.original_message = message
 		return model_instance
```

### Comparing `django-email-log-backend-0.3.4/django_email_log/checks.py` & `django-email-log-backend-0.3rc4/django_email_log/checks.py`

 * *Files identical despite different names*

### Comparing `django-email-log-backend-0.3.4/django_email_log/locale/sk_SK/LC_MESSAGES/django.mo` & `django-email-log-backend-0.3rc4/django_email_log/locale/sk_SK/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-email-log-backend-0.3.4/django_email_log/locale/sk_SK/LC_MESSAGES/django.po` & `django-email-log-backend-0.3rc4/django_email_log/locale/sk_SK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-email-log-backend-0.3.4/django_email_log/migrations/0001_initial.py` & `django-email-log-backend-0.3rc4/django_email_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-email-log-backend-0.3.4/django_email_log/models.py` & `django-email-log-backend-0.3rc4/django_email_log/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 	def save(self, *args, **kwargs):
 		if not self.id and not self.date_sent:
 			self.date_sent = timezone.now()
 		return super().save(*args, **kwargs)
 
 	@property
 	def parsed_message(self):
-		return email.message_from_bytes(bytes(self.message_data))
+		return email.message_from_bytes(self.message_data.tobytes())
 
 	@property
 	def payload_tree(self):
 		return self.__preprocessed_message['tree']
 
 	@property
 	def payload_list(self):
```

### Comparing `django-email-log-backend-0.3.4/django_email_log/static/django_email_log/css/admin.css` & `django-email-log-backend-0.3rc4/django_email_log/static/django_email_log/css/admin.css`

 * *Files identical despite different names*

### Comparing `django-email-log-backend-0.3.4/django_email_log/status_handlers/celery.py` & `django-email-log-backend-0.3rc4/django_email_log/status_handlers/celery.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,15 @@
 				success = (status == 'SUCCESS' and int(retval) > 0)
 				email_status = Email.STATUS_SUCCESS if success else Email.STATUS_FAIL
 			except Exception:
 				email_status = Email.STATUS_FAIL
 			Email.objects.filter(pk=kwargs['email_id']).update(status=email_status)
 
 	def delay(self, *args, **kwargs):
-		email_id = 0
-		email = current_message.get()
-		if email is not None:
-			email_id = email.pk
+		email_id = current_message.get().pk
 		kwargs['email_id'] = email_id
 		return super().delay(*args, **kwargs)
 
 
 def djcelery_email_handler(status, email):
 	"""
 	Handles e-mail status if backend directly returns number of sent messages or
```

### Comparing `django-email-log-backend-0.3.4/django_email_log/templates/admin/django_email_log/email/change_form.html` & `django-email-log-backend-0.3rc4/django_email_log/templates/admin/django_email_log/email/change_form.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {% extends "admin/change_form.html" %}
 
-{% load i18n static %}
+{% load static %}
 
 {% block extrastyle %}
 {{ block.super }}
 <link rel="stylesheet" type="text/css" href="{% static "django_email_log/css/admin.css" %}" />
 {% endblock %}
 
 {% block object-tools %}{% endblock %}
```

### Comparing `django-email-log-backend-0.3.4/django_email_log/utils.py` & `django-email-log-backend-0.3rc4/django_email_log/utils.py`

 * *Files identical despite different names*

### Comparing `django-email-log-backend-0.3.4/django_email_log/views.py` & `django-email-log-backend-0.3rc4/django_email_log/views.py`

 * *Files identical despite different names*

### Comparing `django-email-log-backend-0.3.4/django_email_log_backend.egg-info/PKG-INFO` & `django-email-log-backend-0.3rc4/django_email_log_backend.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,64 @@
 Metadata-Version: 2.1
 Name: django-email-log-backend
-Version: 0.3.4
+Version: 0.3rc4
 Summary: Django email log backend
 Home-page: https://github.com/mireq/django-email-log-backend
 Author: Miroslav Bendík
 Author-email: miroslav.bendik@gmail.com
+License: UNKNOWN
+Description: ============================
+        Django database email logger
+        ============================
+        
+        Install
+        -------
+        
+        `pip install django-email-log-backend.git`
+        
+        or
+        
+        `pip install -e 'git+https://github.com/mireq/django-email-log-backend.git#egg=django_email_log_backend'`
+        
+        Usage
+        -----
+        
+        Settings
+        ^^^^^^^^
+        
+        .. code:: python
+        
+        	INSTALLED_APPS = (
+        		# ...
+        		'django_email_log',
+        	)
+        
+        	EMAIL_BACKEND = 'django_email_log.backends.EmailBackend'
+        	EMAIL_LOG_BACKEND = 'django.core.mail.backends.console.EmailBackend'
+        
+        Emails are forwarded to `EMAIL_LOG_BACKEND`.
+        
+        .. code:: python
+        
+        	# urls.py
+        	urlpatterns = [
+        		# ...
+        		url(r'^django-email-log/', include('django_email_log.urls')),
+        	]
+        
+        .. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg1.png?v2020-04-03
+        
+        .. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg2.png?v2020-04-03
+        
+        .. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg3.png?v2020-04-03
+        
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
-License-File: LICENSE
-License-File: AUTHORS
-
-============================
-Django database email logger
-============================
-
-Install
--------
-
-.. code:: bash
-
-	pip install django-email-log-backend
-
-or
-
-.. code:: bash
-
-	pip install -e 'git+https://github.com/mireq/django-email-log-backend.git#egg=django_email_log_backend'
-
-Settings
-^^^^^^^^
-
-.. code:: python
-
-	INSTALLED_APPS = (
-		# ...
-		'django_email_log',
-	)
-
-	EMAIL_BACKEND = 'django_email_log.backends.EmailBackend'
-	EMAIL_LOG_BACKEND = 'django.core.mail.backends.console.EmailBackend'
-
-Emails are forwarded to `EMAIL_LOG_BACKEND`.
-
-.. code:: python
-
-	# urls.py
-	urlpatterns = [
-		# ...
-		path('django-email-log/', include('django_email_log.urls')),
-	]
-
-Screenshots
-^^^^^^^^^^^
-
-.. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg1.png?v2020-04-03
-
-.. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg2.png?v2020-04-03
-
-.. image:: https://raw.github.com/wiki/mireq/django-email-log-backend/msg3.png?v2020-04-03
```

### Comparing `django-email-log-backend-0.3.4/django_email_log_backend.egg-info/SOURCES.txt` & `django-email-log-backend-0.3rc4/django_email_log_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-email-log-backend-0.3.4/setup.py` & `django-email-log-backend-0.3rc4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 with open('README.rst', 'r') as fh:
 	long_description = fh.read()
 
 
 setuptools.setup(
 	name='django-email-log-backend',
-	version='0.3.4',
+	version='0.3rc4',
 	author='Miroslav Bendík',
 	author_email='miroslav.bendik@gmail.com',
 	description="Django email log backend",
 	long_description=long_description,
 	long_description_content_type='text/x-rst',
 	url='https://github.com/mireq/django-email-log-backend',
 	packages=setuptools.find_packages(),
```

