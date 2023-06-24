# Comparing `tmp/pybash-0.3.3.tar.gz` & `tmp/pybash-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybash-0.3.3.tar", max compression
+gzip compressed data, was "pybash-0.3.4.tar", max compression
```

## Comparing `pybash-0.3.3.tar` & `pybash-0.3.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1060 2023-06-09 02:00:03.224966 pybash-0.3.3/LICENSE
--rw-r--r--   0        0        0     4055 2023-06-09 02:00:03.224966 pybash-0.3.3/README.md
--rw-r--r--   0        0        0        0 2023-06-09 02:00:03.224966 pybash-0.3.3/pybash/__init__.py
--rw-r--r--   0        0        0      684 2023-06-09 02:00:03.224966 pybash-0.3.3/pybash/__main__.py
--rw-r--r--   0        0        0      531 2023-06-09 02:00:03.224966 pybash-0.3.3/pybash/hook.py
--rw-r--r--   0        0        0    15694 2023-06-09 02:00:03.224966 pybash-0.3.3/pybash/transformer.py
--rw-r--r--   0        0        0      792 2023-06-09 02:00:03.224966 pybash-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 pybash-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-24 20:45:14.853931 pybash-0.3.4/LICENSE
+-rw-r--r--   0        0        0     4055 2023-06-24 20:45:14.853931 pybash-0.3.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 20:45:14.857931 pybash-0.3.4/pybash/__init__.py
+-rw-r--r--   0        0        0      684 2023-06-24 20:45:14.857931 pybash-0.3.4/pybash/__main__.py
+-rw-r--r--   0        0        0      531 2023-06-24 20:45:14.857931 pybash-0.3.4/pybash/hook.py
+-rw-r--r--   0        0        0    15774 2023-06-24 20:45:14.857931 pybash-0.3.4/pybash/transformer.py
+-rw-r--r--   0        0        0      792 2023-06-24 20:45:14.857931 pybash-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 pybash-0.3.4/PKG-INFO
```

### Comparing `pybash-0.3.3/LICENSE` & `pybash-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybash-0.3.3/README.md` & `pybash-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pybash-0.3.3/pybash/__main__.py` & `pybash-0.3.4/pybash/__main__.py`

 * *Files identical despite different names*

### Comparing `pybash-0.3.3/pybash/hook.py` & `pybash-0.3.4/pybash/hook.py`

 * *Files identical despite different names*

### Comparing `pybash-0.3.3/pybash/transformer.py` & `pybash-0.3.4/pybash/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,61 +50,64 @@
 
         for sub in subs:
             parsed_command = re.sub(pattern, '" + f\"\"\"{' + sub + '}\"\"\" + "', parsed_command, 1)
 
         return parsed_command.replace('"" + f"""', 'f"""').replace('""" + ""', '"""')
 
     @staticmethod
-    def direct_interpolate(string: str) -> str:
+    def direct_interpolate(token_string: str) -> str:
         """Process {{ static interpolations }} and substitute.
             Static interpolations are denotated by a {{ }} with a variable or a function call inside.
             Substitution happens directly on the parsed command string. Therefore, certain characters
             cannot be interpolated as they get parsed out before substitution.
 
         Args:
             string (str): String to interpolate
 
         Returns:
-            str: Interpolated string
+            str: Interpolated or given token string
         """
 
         # validate interpolation
         invalid_chars = [' ', '"', "'"]
-        matches = re.findall(r'{{(.+?)}}', string)
-        if matches and any(any(bad_char in match for bad_char in invalid_chars) for match in matches):
+        matches = re.findall(r'{{(.+?)}}', token_string)
+        if not matches:
+            return token_string
+
+        if any(any(bad_char in match for bad_char in invalid_chars) for match in matches):
             raise InvalidInterpolation
 
-        interpolated = re.sub(r'{{(.+?)}}', r'" + \1 + "', string)
-        return interpolated.replace('"" + ', '').replace(' + ""', '')
+        interpolated = re.sub(r'{{(.+?)}}', r'" + \1 + "', token_string)
+        return interpolated.replace(',"" + ', ',').replace(' + ""', '')
 
 
 class Shelled(Processor):
-    # $ls .github/*
+    # >ls .github/*
     command_char = ">"
 
     def transform(self) -> token_utils.Token:
         command_str = " ".join(self.command)
         self.token.string = Commander.build_subprocess_str_cmd("run", command_str, shell=True) + '\n'
         return self.token
 
 
 class Execed(Processor):
-    # >ls -la
+    # $ls -la
     def transform(self) -> token_utils.Token:
         pipeline_command = Pipeline(self.command).parse_command()
         if pipeline_command != self.command:
             self.token.string = pipeline_command + '\n'
         else:
             # no pipers
             self.token.string = Commander.build_subprocess_list_cmd("run", self.command) + '\n'
         return self.token
 
 
 class Variablized(Processor):
-    # a = >cat test.txt
+    # a = $cat test.txt
     def parse(self) -> None:
         self.parsed_line = shlex.split(self.token.line)
         self.start_index = Commander.get_start_index(self.parsed_line)
         self.command = Commander.get_bash_command(self.parsed_line, start_index=self.start_index)
 
     def transform(self) -> None:
         pipeline_command = Pipeline(self.command).parse_command(variablized=True)
@@ -115,15 +118,15 @@
             self.token.string += ' '.join(self.parsed_line[: self.start_index]) + ' cmd1\n'
         else:
             self.token.string = ' '.join(self.parsed_line[: self.start_index]) + ' '
             self.token.string += Commander.build_subprocess_list_cmd("check_output", self.command) + '\n'
 
 
 class Wrapped(Processor):
-    # print(>cat test.txt)
+    # print($cat test.txt)
     def parse(self) -> None:
         self.parsed_line = shlex.split(self.token.line)
         self.raw_line = [tok for tok in self.token.line.split(' ') if tok]
         self.start_index = Commander.get_start_index(self.parsed_line)
         self.command = Commander.get_bash_command(self.parsed_line, start_index=self.start_index, wrapped=True)
 
     def transform(self) -> token_utils.Token:
@@ -185,25 +188,25 @@
 
         out = f"{fvar} = {fout}; cmd1 = {cmd1};"
         while pipeline:
             idx, piper = pipeline[0]
             fvar = f"fout{idx}"
             cmd = ""
             if piper == '>':
-                # >sort < test.txt > test2.txt
+                # $sort < test.txt > test2.txt
                 cmd = cls.write_to_file(
                     command, pipeline, reader='cmd1.stdout.read()', start_index=first_idx + 1, fmode="wb"
                 )
             elif piper == '>>':
-                # >sort < test.txt >> test2.txt
+                # $sort < test.txt >> test2.txt
                 cmd = cls.write_to_file(
                     command, pipeline, reader='cmd1.stdout.read()', start_index=first_idx + 1, fmode="ab"
                 )
             elif piper == '|':
-                # >sort < test.txt | grep "HELLO"
+                # $sort < test.txt | grep "HELLO"
                 cmd = cls.get_piper(piper)(
                     command, pipeline, start_index=first_idx + 1, stdin="cmd1.stdout", chained=True
                 )
             out += cmd
             first_idx = idx
 
         return out
@@ -349,23 +352,23 @@
             parsed_line (list): line to parse
             start_index (int, optional): index to start parsing command from. Defaults to None.
             wrapped (bool, optional): input is surrounded by parentheses
 
         Returns:
             list: parsed command list
         """
-        # find which arg index the > is at
+        # find which arg index the $ is at
         if not start_index:
             start_index = Commander.get_start_index(parsed_line)
 
         # strip everything before that index-- not part of the command
         command = parsed_line[start_index:]
 
-        # > may be at the beginning or somewhere in the middle of this arg
-        # examples: >ls, print(>cat => strip up to and including >
+        # $ may be at the beginning or somewhere in the middle of this arg
+        # examples: $ls, print(>cat => strip up to and including >
         command[0] = command[0][command[0].index(command_char) + 1 :].strip()
         if command[0] == '':
             del command[0]
 
         # remove everything after and including first )- not part of the command
         if wrapped:
             if ')' not in command[-1]:
```

### Comparing `pybash-0.3.3/pyproject.toml` & `pybash-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyBash"
-version = "0.3.3"
+version = "0.3.4"
 description = ">execute bash commands from python easily"
 authors = ["Jay <jay.github0@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pybash"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pybash-0.3.3/PKG-INFO` & `pybash-0.3.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybash
-Version: 0.3.3
+Version: 0.3.4
 Summary: >execute bash commands from python easily
 Author: Jay
 Author-email: jay.github0@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

