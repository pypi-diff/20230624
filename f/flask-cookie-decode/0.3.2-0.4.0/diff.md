# Comparing `tmp/flask_cookie_decode-0.3.2.tar.gz` & `tmp/flask_cookie_decode-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask_cookie_decode-0.3.2.tar", last modified: Fri Nov 29 21:24:47 2019, max compression
+gzip compressed data, was "flask_cookie_decode-0.4.0.tar", last modified: Sat Jun 24 18:21:07 2023, max compression
```

## Comparing `flask_cookie_decode-0.3.2.tar` & `flask_cookie_decode-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-29 21:24:47.000000 flask_cookie_decode-0.3.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)      262 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/MANIFEST.in
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-29 21:24:47.000000 flask_cookie_decode-0.3.2/flask_cookie_decode.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8710 2019-11-29 21:24:46.000000 flask_cookie_decode-0.3.2/flask_cookie_decode.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-29 21:24:46.000000 flask_cookie_decode-0.3.2/flask_cookie_decode.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2019-11-29 21:24:46.000000 flask_cookie_decode-0.3.2/flask_cookie_decode.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-29 21:24:46.000000 flask_cookie_decode-0.3.2/flask_cookie_decode.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)      754 2019-11-29 21:24:46.000000 flask_cookie_decode-0.3.2/flask_cookie_decode.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2019-11-29 21:24:46.000000 flask_cookie_decode-0.3.2/flask_cookie_decode.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2019-11-29 21:24:46.000000 flask_cookie_decode-0.3.2/flask_cookie_decode.egg-info/entry_points.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-29 21:24:47.000000 flask_cookie_decode-0.3.2/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/authors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)   101870 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/cookie.png
--rw-rw-r--   0 travis    (2000) travis    (2000)       27 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/readme.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6814 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/Makefile
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8760 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       28 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/history.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/usage.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1194 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      303 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       94 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/modules.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      402 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/flask_cookie_decode.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     6485 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/docs/make.bat
--rw-rw-r--   0 travis    (2000) travis    (2000)     4873 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/CONTRIBUTING.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     8710 2019-11-29 21:24:47.000000 flask_cookie_decode-0.3.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      157 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/AUTHORS.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-29 21:24:47.000000 flask_cookie_decode-0.3.2/flask_cookie_decode/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4686 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/flask_cookie_decode/cookie_decode.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      488 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/flask_cookie_decode/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      402 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/flask_cookie_decode/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      317 2019-11-29 21:24:47.000000 flask_cookie_decode-0.3.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1205 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/HISTORY.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1070 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     5054 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     2106 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-29 21:24:47.000000 flask_cookie_decode-0.3.2/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4070 2019-11-29 21:24:14.000000 flask_cookie_decode-0.3.2/tests/test_flask_cookie_decode.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-06-24 18:21:07.810267 flask_cookie_decode-0.4.0/
+-rw-r--r--   0 kyle       (501) staff       (20)      157 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/AUTHORS.rst
+-rw-r--r--   0 kyle       (501) staff       (20)     4873 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 kyle       (501) staff       (20)     1362 2023-06-24 18:19:02.000000 flask_cookie_decode-0.4.0/HISTORY.rst
+-rw-r--r--   0 kyle       (501) staff       (20)     1070 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/LICENSE
+-rw-r--r--   0 kyle       (501) staff       (20)      262 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/MANIFEST.in
+-rw-r--r--   0 kyle       (501) staff       (20)     7308 2023-06-24 18:21:07.810327 flask_cookie_decode-0.4.0/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)     5054 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/README.rst
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-06-24 18:21:07.808130 flask_cookie_decode-0.4.0/docs/
+-rw-r--r--   0 kyle       (501) staff       (20)     6814 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/Makefile
+-rw-r--r--   0 kyle       (501) staff       (20)       28 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/authors.rst
+-rwxr-xr-x   0 kyle       (501) staff       (20)     8760 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/conf.py
+-rw-r--r--   0 kyle       (501) staff       (20)       33 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/contributing.rst
+-rw-r--r--   0 kyle       (501) staff       (20)   101870 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/cookie.png
+-rw-r--r--   0 kyle       (501) staff       (20)      402 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/flask_cookie_decode.rst
+-rw-r--r--   0 kyle       (501) staff       (20)       28 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/history.rst
+-rw-r--r--   0 kyle       (501) staff       (20)      303 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/index.rst
+-rw-r--r--   0 kyle       (501) staff       (20)     1194 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/installation.rst
+-rw-r--r--   0 kyle       (501) staff       (20)     6485 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/make.bat
+-rw-r--r--   0 kyle       (501) staff       (20)       94 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/modules.rst
+-rw-r--r--   0 kyle       (501) staff       (20)       27 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/readme.rst
+-rw-r--r--   0 kyle       (501) staff       (20)       18 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/docs/usage.rst
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-06-24 18:21:07.808951 flask_cookie_decode-0.4.0/flask_cookie_decode/
+-rw-r--r--   0 kyle       (501) staff       (20)      402 2023-06-24 18:19:02.000000 flask_cookie_decode-0.4.0/flask_cookie_decode/__init__.py
+-rw-r--r--   0 kyle       (501) staff       (20)      488 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/flask_cookie_decode/__main__.py
+-rw-r--r--   0 kyle       (501) staff       (20)     4787 2023-06-24 18:19:02.000000 flask_cookie_decode-0.4.0/flask_cookie_decode/cookie_decode.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-06-24 18:21:07.809947 flask_cookie_decode-0.4.0/flask_cookie_decode.egg-info/
+-rw-r--r--   0 kyle       (501) staff       (20)     7308 2023-06-24 18:21:07.000000 flask_cookie_decode-0.4.0/flask_cookie_decode.egg-info/PKG-INFO
+-rw-r--r--   0 kyle       (501) staff       (20)      769 2023-06-24 18:21:07.000000 flask_cookie_decode-0.4.0/flask_cookie_decode.egg-info/SOURCES.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2023-06-24 18:21:07.000000 flask_cookie_decode-0.4.0/flask_cookie_decode.egg-info/dependency_links.txt
+-rw-r--r--   0 kyle       (501) staff       (20)       58 2023-06-24 18:21:07.000000 flask_cookie_decode-0.4.0/flask_cookie_decode.egg-info/entry_points.txt
+-rw-r--r--   0 kyle       (501) staff       (20)        1 2023-06-24 18:21:07.000000 flask_cookie_decode-0.4.0/flask_cookie_decode.egg-info/not-zip-safe
+-rw-r--r--   0 kyle       (501) staff       (20)       27 2023-06-24 18:21:07.000000 flask_cookie_decode-0.4.0/flask_cookie_decode.egg-info/requires.txt
+-rw-r--r--   0 kyle       (501) staff       (20)       20 2023-06-24 18:21:07.000000 flask_cookie_decode-0.4.0/flask_cookie_decode.egg-info/top_level.txt
+-rw-r--r--   0 kyle       (501) staff       (20)      104 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/pyproject.toml
+-rw-r--r--   0 kyle       (501) staff       (20)      317 2023-06-24 18:21:07.810553 flask_cookie_decode-0.4.0/setup.cfg
+-rw-r--r--   0 kyle       (501) staff       (20)     2106 2023-06-23 20:42:45.000000 flask_cookie_decode-0.4.0/setup.py
+drwxr-xr-x   0 kyle       (501) staff       (20)        0 2023-06-24 18:21:07.810058 flask_cookie_decode-0.4.0/tests/
+-rw-r--r--   0 kyle       (501) staff       (20)     4483 2023-06-24 18:19:02.000000 flask_cookie_decode-0.4.0/tests/test_flask_cookie_decode.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `flask_cookie_decode-0.3.2/flask_cookie_decode.egg-info/SOURCES.txt` & `flask_cookie_decode-0.4.0/flask_cookie_decode.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 AUTHORS.rst
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/cookie.png
```

### Comparing `flask_cookie_decode-0.3.2/docs/cookie.png` & `flask_cookie_decode-0.4.0/docs/cookie.png`

 * *Files identical despite different names*

### Comparing `flask_cookie_decode-0.3.2/docs/Makefile` & `flask_cookie_decode-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flask_cookie_decode-0.3.2/docs/conf.py` & `flask_cookie_decode-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `flask_cookie_decode-0.3.2/docs/installation.rst` & `flask_cookie_decode-0.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `flask_cookie_decode-0.3.2/docs/make.bat` & `flask_cookie_decode-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flask_cookie_decode-0.3.2/CONTRIBUTING.rst` & `flask_cookie_decode-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `flask_cookie_decode-0.3.2/flask_cookie_decode/cookie_decode.py` & `flask_cookie_decode-0.4.0/flask_cookie_decode/cookie_decode.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from datetime import datetime, timedelta
 from collections import namedtuple
 import click
 from itsdangerous.timed import TimestampSigner
 from itsdangerous.exc import BadTimeSignature, SignatureExpired
 from flask.cli import AppGroup
 from flask.sessions import SecureCookieSessionInterface
-from flask.helpers import total_seconds
 
 TrustedCookie = namedtuple("TrustedCookie", "contents, expiration")
 UntrustedCookie = namedtuple("UntrustedCookie", "contents, expiration")
 ExpiredCookie = namedtuple("ExpiredCookie", "contents, expiration")
 
 
 class CookieDecode(object):
@@ -47,15 +46,18 @@
     def init_app(self, app):
         """Initalizes the application with the extension."""
         self._session_interface = SecureCookieSessionInterface()
         self._signing_serializer = self._session_interface.get_signing_serializer(app)
         self._timestamp_signer = TimestampSigner(
             app.secret_key, key_derivation="hmac", salt="cookie-session"
         )
-        self._max_age = total_seconds(app.permanent_session_lifetime)
+        if isinstance(app.permanent_session_lifetime, timedelta):
+            self._max_age = app.permanent_session_lifetime.total_seconds()
+        else:
+            self.max_age = app.permanent_session_lifetime
 
         cookie_cli = AppGroup(
             "cookie", help="Tools to inspect the Flask session cookie."
         )
         app.cli.add_command(cookie_cli)
 
         @cookie_cli.command("decode")
@@ -86,27 +88,27 @@
         except BadTimeSignature as bad_sign:
             return UntrustedCookie(
                 *self._unsafe_decode(cookie, date_signed=bad_sign.date_signed)
             )
         return TrustedCookie(*self._safe_decode(cookie))
 
     def _safe_decode(self, cookie):
-        """"Validate the signature in the session cookie, decode the cookie
+        """Validate the signature in the session cookie, decode the cookie
         payload and compute the expiration date based off of the Flask application
         instances PERMANENT_SESSION_LIFETIME config value.
         """
         contents, date_signed = self._signing_serializer.loads(
             cookie, return_timestamp=True
         )
 
         expires_at = (date_signed + timedelta(seconds=self._max_age)).isoformat()
         return (contents, expires_at)
 
     def _unsafe_decode(self, cookie, date_signed=None):
-        """"Ignoring the signature of the session cookies decode the cookies
+        """Ignoring the signature of the session cookies decode the cookies
         payload and the compute the expiration based off of the Flask application
         instances PERMANENT_SESSION_LIFETIME config value.
 
         The data loaded here is *untrusted*."""
         _, contents = self._signing_serializer.loads_unsafe(cookie)
         if date_signed is None:
             return (contents, None)
```

### Comparing `flask_cookie_decode-0.3.2/HISTORY.rst` & `flask_cookie_decode-0.4.0/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 History
 #######
 
 .. towncrier release notes start
 
+Flask_Cookie_Decode 0.4.0 (2023-06-23)
+======================================
+
+Bugfixes
+--------
+
+- remove dependency on flask.helpers.total_seconds (#13)
+
+
 Flask_Cookie_Decode 0.3.2 (2019-11-29)
 ======================================
 
 Bugfixes
 --------
 
 - The `fcd` client now handles compressed cookies. (#10)
```

### Comparing `flask_cookie_decode-0.3.2/LICENSE` & `flask_cookie_decode-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_cookie_decode-0.3.2/README.rst` & `flask_cookie_decode-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `flask_cookie_decode-0.3.2/setup.py` & `flask_cookie_decode-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `flask_cookie_decode-0.3.2/tests/test_flask_cookie_decode.py` & `flask_cookie_decode-0.4.0/tests/test_flask_cookie_decode.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,15 +63,16 @@
     res = fcd_invoke(foo_compressed_cookie)
     assert res.exit_code == 0
     assert "a" in json.loads(res.output).keys()
 
 
 def test_safe_decode(app):
     result = app.extensions["flask_cookie_decode"]._safe_decode(foo_cookie)
-    assert result == rv_foo_cookie
+    assert result[0] == rv_foo_cookie[0]
+    assert result[1].replace("+00:00", "") == rv_foo_cookie[1]
 
 
 def test_unsafe_decode(app):
     result = app.extensions["flask_cookie_decode"]._unsafe_decode(foo_cookie)
     assert result == ({"a": "helloworld"}, None)
 
 
@@ -85,31 +86,34 @@
         foo_cookie_invalid_sign
     )
     assert result == ({"a": "helloworld"}, None)
 
 
 def test_compressed_safe_decode(app):
     result = app.extensions["flask_cookie_decode"]._safe_decode(foo_compressed_cookie)
-
-    assert result == (
-        {
-            "a": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam vestibulum massa eget leo venenatis interdum. Vestibulum ut blandit massa, in porta neque. Aenean viverra facilisis nisl, eget ornare velit vehicula ut. Donec arcu nibh, lacinia ac maximus in, pellentesque non eros. Mauris interdum turpis vel rutrum malesuada. Fusce a tortor eu risus placerat tempus. Nam ut varius magna. Etiam vel purus elit. In et ligula et est viverra egestas."
-        },
-        "2019-01-29T21:34:06",
-    )
+    assert result[0] == {
+        "a": "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam vestibulum massa eget leo venenatis interdum. Vestibulum ut blandit massa, in porta neque. Aenean viverra facilisis nisl, eget ornare velit vehicula ut. Donec arcu nibh, lacinia ac maximus in, pellentesque non eros. Mauris interdum turpis vel rutrum malesuada. Fusce a tortor eu risus placerat tempus. Nam ut varius magna. Etiam vel purus elit. In et ligula et est viverra egestas."
+    }
+    assert result[1].replace("+00:00", "") == "2019-01-29T21:34:06"
 
 
 def test_decode_cookie_trusted(app):
     result = app.extensions["flask_cookie_decode"].decode_cookie(foo_cookie)
-    assert result == TrustedCookie(*rv_foo_cookie)
+    expect = TrustedCookie(*rv_foo_cookie)
+    assert result.contents == expect.contents
+    assert result.expiration.replace("+00:00", "") == expect.expiration
 
 
 def test_decode_cookie_untrusted(app):
     result = app.extensions["flask_cookie_decode"].decode_cookie(
         foo_cookie_invalid_sign
     )
-    assert result == UntrustedCookie(*rv_foo_cookie_invalid_sign)
+    expect = UntrustedCookie(*rv_foo_cookie_invalid_sign)
+    assert result.contents == expect.contents
+    assert result.expiration.replace("+00:00", "") == expect.expiration
 
 
 def test_decode_cookie_expired(app):
     result = app.extensions["flask_cookie_decode"].decode_cookie(foo_cookie_expired)
-    assert result == ExpiredCookie(*rv_foo_cookie_expired)
+    expect = ExpiredCookie(*rv_foo_cookie_expired)
+    assert result.contents == expect.contents
+    assert result.expiration.replace("+00:00", "") == expect.expiration
```

