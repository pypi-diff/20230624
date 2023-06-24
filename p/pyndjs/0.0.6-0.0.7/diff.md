# Comparing `tmp/pyndjs-0.0.6.tar.gz` & `tmp/pyndjs-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyndjs-0.0.6.tar", last modified: Wed May 31 10:09:26 2023, max compression
+gzip compressed data, was "dist\pyndjs-0.0.7.tar", last modified: Sat Jun 24 13:02:29 2023, max compression
```

## Comparing `pyndjs-0.0.6.tar` & `pyndjs-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 10:09:26.143917 pyndjs-0.0.6/
--rw-rw-rw-   0        0        0      160 2023-05-31 10:09:26.142918 pyndjs-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-31 10:09:26.135535 pyndjs-0.0.6/pyndjs/
--rw-rw-rw-   0        0        0       52 2023-02-08 08:23:02.000000 pyndjs-0.0.6/pyndjs/__init__.py
--rw-rw-rw-   0        0        0     6121 2023-05-31 10:08:45.000000 pyndjs-0.0.6/pyndjs/pyndjs.py
-drwxrwxrwx   0        0        0        0 2023-05-31 10:09:26.141912 pyndjs-0.0.6/pyndjs.egg-info/
--rw-rw-rw-   0        0        0      160 2023-05-31 10:09:26.000000 pyndjs-0.0.6/pyndjs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2023-05-31 10:09:26.000000 pyndjs-0.0.6/pyndjs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 10:09:26.000000 pyndjs-0.0.6/pyndjs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-31 10:09:26.000000 pyndjs-0.0.6/pyndjs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-31 10:09:26.000000 pyndjs-0.0.6/pyndjs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 10:09:26.143917 pyndjs-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      275 2023-05-31 10:09:20.000000 pyndjs-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:02:29.000000 pyndjs-0.0.7/
+-rw-rw-rw-   0        0        0      192 2023-06-24 13:02:29.000000 pyndjs-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-24 13:02:29.000000 pyndjs-0.0.7/pyndjs/
+-rw-rw-rw-   0        0        0       52 2023-02-08 08:23:02.000000 pyndjs-0.0.7/pyndjs/__init__.py
+-rw-rw-rw-   0        0        0     6122 2023-06-24 13:01:25.000000 pyndjs-0.0.7/pyndjs/pyndjs.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:02:29.000000 pyndjs-0.0.7/pyndjs.egg-info/
+-rw-rw-rw-   0        0        0      192 2023-06-24 13:02:29.000000 pyndjs-0.0.7/pyndjs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2023-06-24 13:02:29.000000 pyndjs-0.0.7/pyndjs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:02:29.000000 pyndjs-0.0.7/pyndjs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-24 13:02:29.000000 pyndjs-0.0.7/pyndjs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-24 13:02:29.000000 pyndjs-0.0.7/pyndjs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:02:29.000000 pyndjs-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      275 2023-06-24 13:00:57.000000 pyndjs-0.0.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyndjs-0.0.6/pyndjs/pyndjs.py` & `pyndjs-0.0.7/pyndjs/pyndjs.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     pattern = "|".join(re.escape(k) for k in replacements)
     runner_source = re.sub(pattern, lambda m: replacements[m.group(0)](), runner_source)
     return runner_source
 
 
 def execute(js_code, fun_name, args, node_path=os.popen("where node").read().strip(), encoding='utf-8'):
     js_code = js_code + "\n" + \
-             r"""return eval('('+"{}.apply(this, {})"+')')""".format(fun_name, args)
+             r"""return eval('('+`{}.apply(this, {})`+')');""".format(fun_name, args)
     cmd = [node_path.replace('\\', '/')]
     try:
         p = Popen(cmd, stdin=-1, stdout=-1, stderr=-1, cwd=None, universal_newlines=True, encoding=encoding)
         input = _compile(js_code)
         if six.PY2:
             input = input.encode(sys.getfilesystemencoding())
         stdoutdata, stderrdata = p.communicate(input=input)
```

