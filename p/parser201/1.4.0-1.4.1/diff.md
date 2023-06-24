# Comparing `tmp/parser201-1.4.0.tar.gz` & `tmp/parser201-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parser201-1.4.0.tar", max compression
+gzip compressed data, was "parser201-1.4.1.tar", max compression
```

## Comparing `parser201-1.4.0.tar` & `parser201-1.4.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1074 2023-04-30 20:20:31.148592 parser201-1.4.0/LICENSE
--rw-r--r--   0        0        0     4454 2023-04-30 22:23:05.969168 parser201-1.4.0/README.md
--rw-r--r--   0        0        0     1657 2023-04-30 20:20:31.152590 parser201-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      399 2023-04-30 20:20:31.156589 parser201-1.4.0/src/parser201/__init__.py
--rw-r--r--   0        0        0    10446 2023-04-30 20:29:04.112043 parser201-1.4.0/src/parser201/classes.py
--rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 parser201-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-30 22:26:53.844809 parser201-1.4.1/LICENSE
+-rw-r--r--   0        0        0     4523 2023-06-22 20:40:04.197867 parser201-1.4.1/README.md
+-rw-r--r--   0        0        0     1655 2023-06-22 20:40:04.197867 parser201-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      399 2023-06-22 20:40:04.197867 parser201-1.4.1/src/parser201/__init__.py
+-rw-r--r--   0        0        0    10412 2023-06-22 20:40:04.197867 parser201-1.4.1/src/parser201/classes.py
+-rw-r--r--   0        0        0     5927 1970-01-01 00:00:00.000000 parser201-1.4.1/PKG-INFO
```

### Comparing `parser201-1.4.0/LICENSE` & `parser201-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parser201-1.4.0/README.md` & `parser201-1.4.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
 ## Documentation
 
 See: [parser201 Documentation](https://geozeke.github.io/parser201).
 
 ## Version History
 
+* 1.4.1 (2023-06-22)
+  * Migrated code formatter to *black*.<br><br>
 * 1.4.0 (2023-04-30)
   * Strengthened regular expression parsing to handle log lines that
     contain a wider array of malicious attacks.
   * Added support for access logs that contain both IPv4 and IPv6
     addresses.
   * Minimum supported Python version is now 3.8 (^3.8).
   * Miscellaneous optimizations.<br><br>
```

### Comparing `parser201-1.4.0/pyproject.toml` & `parser201-1.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "parser201"
-version = "1.4.0"
+version = "1.4.1"
 description = "Extract individual fields from lines in Apache access logs"
 authors = ["Peter Nardi <pete@nardi.com>"]
 maintainers = ["Peter Nardi <pete@nardi.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "parser201", from = "src" }]
 homepage = "https://github.com/geozeke/parser201"
@@ -44,19 +44,19 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.5.0"
 pytest = "^7.1.3"
-autopep8 = "^1.7.0"
 flake8 = "^5.0.4"
 flake8-docstrings = "^1.6.0"
 mypy = "^0.982"
 pdoc3 = "^0.10.0"
+black = "^23.3.0"
 
 [tool.pytest.ini_options]
 pythonpath = [".", "./src", "./src/parser201"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `parser201-1.4.0/src/parser201/classes.py` & `parser201-1.4.1/src/parser201/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,59 +144,58 @@
     # Behold the power of generative AI. I provided the following query to
     # ChatGPT: "Write a regular expression that recognizes a line from an
     # apache access log". I had to have a "conversation" with ChatGPT to refine
     # the regex with a few examples, but after a brief exchange, it produced
     # what you see below. This regex cleaned up my previous solution and
     # replace several lines of code. I split the regex into individual match
     # groups here to make it easier to follow.
-    _ip = r'^([^ ]+)'
-    _ui = r'(\S+)'
-    _un = r'(\S+)'
-    _ts = r'\[([^\]]+)\]'
+    _ip = r"^([^ ]+)"
+    _ui = r"(\S+)"
+    _un = r"(\S+)"
+    _ts = r"\[([^\]]+)\]"
     _rl = r'"(.*?)"'
-    _sc = r'(\d{3})'
-    _ds = r'(\S+)'
+    _sc = r"(\d{3})"
+    _ds = r"(\S+)"
     _re = r'"((?:[^"]|\")*?)"'
     _ua = r'"((?:[^"]|\")*?|-)"'
-    _regex = fr'{_ip} {_ui} {_un} {_ts} {_rl} {_sc} {_ds} {_re} {_ua}'
+    _regex = rf"{_ip} {_ui} {_un} {_ts} {_rl} {_sc} {_ds} {_re} {_ua}"
 
     # A list of labels (in the correct order) used to render string
     # representations of LogParser objects. Also calculate the length of the
     # longest label so we can use f-strings to right-justify all the labels.
     _labels = [
-        'ipaddress',
-        'userid',
-        'username',
-        'timestamp',
-        'requestline',
-        'statuscode',
-        'datasize',
-        'referrer',
-        'useragent'
+        "ipaddress",
+        "userid",
+        "username",
+        "timestamp",
+        "requestline",
+        "statuscode",
+        "datasize",
+        "referrer",
+        "useragent",
     ]
     _pad = len(max(_labels, key=len))
 
     def __init__(self, line, timezone=TZ.original, dts_format=FMT.string):
-
         # Initialize data fields
-        self.ipaddress: str = ''
-        self.userid: str = ''
-        self.username: str = ''
-        self.timestamp: str = ''
-        self.requestline: str = ''
+        self.ipaddress: str = ""
+        self.userid: str = ""
+        self.username: str = ""
+        self.timestamp: str = ""
+        self.requestline: str = ""
         self.statuscode: int = 0
         self.datasize: int = 0
-        self.referrer: str = ''
-        self.useragent: str = ''
+        self.referrer: str = ""
+        self.useragent: str = ""
 
         if type(line) != str:
             self.__none_fields()
             return
 
-        if (groups := re.match(LogParser._regex, line)):
+        if groups := re.match(LogParser._regex, line):
             self.ipaddress = groups.group(1)
             self.userid = groups.group(2)
             self.username = groups.group(3)
             self.timestamp = groups.group(4)
             self.requestline = groups.group(5)
             self.statuscode = int(groups.group(6))
             try:
@@ -209,42 +208,41 @@
             self.__none_fields()
             return
 
         # This takes the work of ensuring valid date-time stamps from the regex
         # and guarantees things like "Feb 31" will be handled as an invalid
         # date.
         try:
-            date_obj = dt.datetime.strptime(self.timestamp,
-                                            '%d/%b/%Y:%H:%M:%S %z')
+            date_obj = dt.datetime.strptime(self.timestamp, "%d/%b/%Y:%H:%M:%S %z")
         except ValueError:
             self.__none_fields()
             return
 
         # Process date/time stamp and adjust timezone/dts_format as indicated
         sign, hh, mm = self.__decomposeTZ(self.timestamp)
         if timezone == TZ.original:
             if dts_format == FMT.string:
                 return
         elif timezone == TZ.local:
-            zone_str = time.strftime('%z')
+            zone_str = time.strftime("%z")
             # First convert to GMT
-            date_obj = date_obj + (-1*sign*dt.timedelta(hours=hh, minutes=mm))
+            date_obj = date_obj + (-1 * sign * dt.timedelta(hours=hh, minutes=mm))
             # Now convert to local time and replace tzinfo
             sign, hh, mm = self.__decomposeTZ(zone_str)
-            zone_obj = dt.timezone(dt.timedelta(hours=hh*sign, minutes=mm))
-            date_obj = date_obj + (sign*dt.timedelta(hours=hh, minutes=mm))
+            zone_obj = dt.timezone(dt.timedelta(hours=hh * sign, minutes=mm))
+            date_obj = date_obj + (sign * dt.timedelta(hours=hh, minutes=mm))
             date_obj = date_obj.replace(tzinfo=zone_obj)
         else:  # TZ == utc
-            date_obj = date_obj + (-1*sign*dt.timedelta(hours=hh, minutes=mm))
-            sign, hh, mm = self.__decomposeTZ('+0000')
+            date_obj = date_obj + (-1 * sign * dt.timedelta(hours=hh, minutes=mm))
+            sign, hh, mm = self.__decomposeTZ("+0000")
             zone_obj = dt.timezone(dt.timedelta(hours=0, minutes=0))
             date_obj = date_obj.replace(tzinfo=zone_obj)
 
         if dts_format == FMT.string:
-            self.timestamp = date_obj.strftime('%d/%b/%Y:%H:%M:%S %z')
+            self.timestamp = date_obj.strftime("%d/%b/%Y:%H:%M:%S %z")
         else:  # dts_format == FMT.date_obj
             self.timestamp = date_obj
 
         return
 
     def __none_fields(self):
         """Set all properties to None."""
@@ -277,16 +275,16 @@
          statuscode: 304
            datasize: 2454
            referrer: -
           useragent: Mozilla/4.0 compatible; MSIE 7.0; Windows NT 5.1;
         """
         lp_str = []
         for label in LogParser._labels:
-            lp_str.append(f'{label:>{LogParser._pad}}: {getattr(self, label)}')
-        return '\n'.join(lp_str)
+            lp_str.append(f"{label:>{LogParser._pad}}: {getattr(self, label)}")
+        return "\n".join(lp_str)
 
     def __eq__(self, other):
         """Determine if two `LogParser` objects are equal.
 
         The class provides a `__eq__` method to test for equality
         between two `LogParser` objects.
 
@@ -303,13 +301,13 @@
         if type(self) != type(other):
             return False
         return vars(self) == vars(other)
 
     def __decomposeTZ(self, zone):
         """Decompose a time zone into +/-, hrs, and mins."""
         leader, hrs, mins = zone[-5], zone[-4:-2], zone[-2:]
-        sign = -1 if leader == '-' else 1
+        sign = -1 if leader == "-" else 1
         return sign, int(hrs), int(mins)
 
 
-if __name__ == '__main__':  # pragma no cover
+if __name__ == "__main__":  # pragma no cover
     pass
```

### Comparing `parser201-1.4.0/PKG-INFO` & `parser201-1.4.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parser201
-Version: 1.4.0
+Version: 1.4.1
 Summary: Extract individual fields from lines in Apache access logs
 Home-page: https://github.com/geozeke/parser201
 License: MIT
 Keywords: parser201,apache,log,parse,parser,scanner,web,server
 Author: Peter Nardi
 Author-email: pete@nardi.com
 Maintainer: Peter Nardi
@@ -18,18 +18,14 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Education
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Logging
 Classifier: Topic :: System :: Systems Administration
 Project-URL: Bug Tracker, https://github.com/geozeke/parser201/issues
 Project-URL: Documentation, https://geozeke.github.io/parser201
@@ -77,14 +73,16 @@
 
 ## Documentation
 
 See: [parser201 Documentation](https://geozeke.github.io/parser201).
 
 ## Version History
 
+* 1.4.1 (2023-06-22)
+  * Migrated code formatter to *black*.<br><br>
 * 1.4.0 (2023-04-30)
   * Strengthened regular expression parsing to handle log lines that
     contain a wider array of malicious attacks.
   * Added support for access logs that contain both IPv4 and IPv6
     addresses.
   * Minimum supported Python version is now 3.8 (^3.8).
   * Miscellaneous optimizations.<br><br>
```

