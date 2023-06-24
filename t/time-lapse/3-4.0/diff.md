# Comparing `tmp/time-lapse-3.tar.gz` & `tmp/time_lapse-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time-lapse-3.tar", last modified: Fri Sep 30 06:59:25 2022, max compression
+gzip compressed data, was "time_lapse-4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `time-lapse-3.tar` & `time_lapse-4.0.tar`

### file list

```diff
@@ -1,30 +1,93 @@
-drwxr-xr-x   0 arne       (501) staff       (20)        0 2022-09-30 06:59:25.068195 time-lapse-3/
--rw-r--r--   0 arne       (501) staff       (20)      274 2022-01-17 10:30:52.000000 time-lapse-3/.editorconfig
--rw-r--r--   0 arne       (501) staff       (20)     1069 2022-01-17 10:30:52.000000 time-lapse-3/LICENSE
--rw-r--r--   0 arne       (501) staff       (20)      167 2022-01-17 10:30:52.000000 time-lapse-3/MANIFEST.in
--rw-r--r--   0 arne       (501) staff       (20)      607 2022-01-17 10:30:52.000000 time-lapse-3/Makefile
--rw-r--r--   0 arne       (501) staff       (20)     4664 2022-09-30 06:59:25.068270 time-lapse-3/PKG-INFO
--rw-r--r--   0 arne       (501) staff       (20)     3974 2022-09-11 11:43:07.000000 time-lapse-3/README.md
--rw-r--r--   0 arne       (501) staff       (20)     1273 2022-09-30 06:59:25.068648 time-lapse-3/setup.cfg
--rwxr-xr-x   0 arne       (501) staff       (20)       38 2022-01-17 10:30:52.000000 time-lapse-3/setup.py
-drwxr-xr-x   0 arne       (501) staff       (20)        0 2022-09-30 06:59:25.065911 time-lapse-3/tests/
--rw-r--r--   0 arne       (501) staff       (20)        0 2022-01-17 10:30:52.000000 time-lapse-3/tests/__init__.py
-drwxr-xr-x   0 arne       (501) staff       (20)        0 2022-09-30 06:59:25.065999 time-lapse-3/tests/__pycache__/
--rw-r--r--   0 arne       (501) staff       (20)      145 2022-09-30 06:59:22.000000 time-lapse-3/tests/__pycache__/__init__.cpython-310.pyc
-drwxr-xr-x   0 arne       (501) staff       (20)        0 2022-09-30 06:59:25.066690 time-lapse-3/time_lapse/
--rw-r--r--   0 arne       (501) staff       (20)       61 2022-01-17 10:30:52.000000 time-lapse-3/time_lapse/__init__.py
--rw-r--r--   0 arne       (501) staff       (20)     3529 2022-09-30 06:58:06.000000 time-lapse-3/time_lapse/check_interval.py
--rw-r--r--   0 arne       (501) staff       (20)     1693 2022-01-17 10:30:52.000000 time-lapse-3/time_lapse/cli.py
--rw-r--r--   0 arne       (501) staff       (20)      244 2022-01-17 10:30:52.000000 time-lapse-3/time_lapse/detect_audio.py
-drwxr-xr-x   0 arne       (501) staff       (20)        0 2022-09-30 06:59:25.067383 time-lapse-3/time_lapse/fonts/
--rwxr-xr-x   0 arne       (501) staff       (20)    98228 2022-01-17 10:30:52.000000 time-lapse-3/time_lapse/fonts/Jost-400-Book.ttf
--rw-r--r--   0 arne       (501) staff       (20)     2095 2022-06-11 10:30:05.000000 time-lapse-3/time_lapse/output.py
--rw-r--r--   0 arne       (501) staff       (20)      769 2022-01-17 10:30:52.000000 time-lapse-3/time_lapse/source.py
--rw-r--r--   0 arne       (501) staff       (20)      540 2022-01-17 10:30:52.000000 time-lapse-3/time_lapse/watermark.py
-drwxr-xr-x   0 arne       (501) staff       (20)        0 2022-09-30 06:59:25.067280 time-lapse-3/time_lapse.egg-info/
--rw-r--r--   0 arne       (501) staff       (20)     4664 2022-09-30 06:59:25.000000 time-lapse-3/time_lapse.egg-info/PKG-INFO
--rw-r--r--   0 arne       (501) staff       (20)      536 2022-09-30 06:59:25.000000 time-lapse-3/time_lapse.egg-info/SOURCES.txt
--rw-r--r--   0 arne       (501) staff       (20)        1 2022-09-30 06:59:25.000000 time-lapse-3/time_lapse.egg-info/dependency_links.txt
--rw-r--r--   0 arne       (501) staff       (20)       98 2022-09-30 06:59:25.000000 time-lapse-3/time_lapse.egg-info/entry_points.txt
--rw-r--r--   0 arne       (501) staff       (20)       91 2022-09-30 06:59:25.000000 time-lapse-3/time_lapse.egg-info/requires.txt
--rw-r--r--   0 arne       (501) staff       (20)       11 2022-09-30 06:59:25.000000 time-lapse-3/time_lapse.egg-info/top_level.txt
+-rw-r--r--   0        0        0      274 2022-01-17 10:30:52.246163 time_lapse-4.0/.editorconfig
+-rw-r--r--   0        0        0      250 2023-06-23 06:58:58.776606 time_lapse-4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      432 2022-12-16 18:40:51.232478 time_lapse-4.0/.github/workflows/demo.yml
+-rw-r--r--   0        0        0      983 2023-06-16 15:03:59.334837 time_lapse-4.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       72 2022-01-17 10:30:52.246658 time_lapse-4.0/.gitignore
+-rw-r--r--   0        0        0     1069 2022-01-17 10:30:52.246784 time_lapse-4.0/LICENSE
+-rw-r--r--   0        0        0      781 2023-06-16 15:03:59.335188 time_lapse-4.0/Makefile
+-rw-r--r--   0        0        0     3972 2022-12-16 18:40:51.288312 time_lapse-4.0/README.md
+-rw-r--r--   0        0        0      106 2022-01-17 10:30:52.247371 time_lapse-4.0/demo/Makefile
+-rw-r--r--   0        0        0    47653 2022-01-17 10:30:52.247772 time_lapse-4.0/demo/source/S60_050504_181349.jpg
+-rw-r--r--   0        0        0    47989 2022-01-17 10:30:52.248224 time_lapse-4.0/demo/source/S60_050504_181449.jpg
+-rw-r--r--   0        0        0    48213 2022-01-17 10:30:52.248657 time_lapse-4.0/demo/source/S60_050504_181549.jpg
+-rw-r--r--   0        0        0    48206 2022-01-17 10:30:52.249109 time_lapse-4.0/demo/source/S60_050504_181649.jpg
+-rw-r--r--   0        0        0    48291 2022-01-17 10:30:52.249544 time_lapse-4.0/demo/source/S60_050504_181749.jpg
+-rw-r--r--   0        0        0    48140 2022-01-17 10:30:52.249879 time_lapse-4.0/demo/source/S60_050504_181849.jpg
+-rw-r--r--   0        0        0    48733 2022-01-17 10:30:52.250320 time_lapse-4.0/demo/source/S60_050504_181949.jpg
+-rw-r--r--   0        0        0    49385 2022-01-17 10:30:52.250787 time_lapse-4.0/demo/source/S60_050504_182049.jpg
+-rw-r--r--   0        0        0    49778 2022-01-17 10:30:52.251132 time_lapse-4.0/demo/source/S60_050504_182149.jpg
+-rw-r--r--   0        0        0    50554 2022-01-17 10:30:52.251491 time_lapse-4.0/demo/source/S60_050504_182249.jpg
+-rw-r--r--   0        0        0    51313 2022-01-17 10:30:52.252097 time_lapse-4.0/demo/source/S60_050504_182349.jpg
+-rw-r--r--   0        0        0    51550 2022-01-17 10:30:52.252669 time_lapse-4.0/demo/source/S60_050504_182449.jpg
+-rw-r--r--   0        0        0    51972 2022-01-17 10:30:52.253049 time_lapse-4.0/demo/source/S60_050504_182549.jpg
+-rw-r--r--   0        0        0    52344 2022-01-17 10:30:52.253503 time_lapse-4.0/demo/source/S60_050504_182649.jpg
+-rw-r--r--   0        0        0    52423 2022-01-17 10:30:52.253818 time_lapse-4.0/demo/source/S60_050504_182749.jpg
+-rw-r--r--   0        0        0    52739 2022-01-17 10:30:52.254242 time_lapse-4.0/demo/source/S60_050504_182849.jpg
+-rw-r--r--   0        0        0    52795 2022-01-17 10:30:52.254679 time_lapse-4.0/demo/source/S60_050504_182949.jpg
+-rw-r--r--   0        0        0    52615 2022-01-17 10:30:52.255101 time_lapse-4.0/demo/source/S60_050504_183049.jpg
+-rw-r--r--   0        0        0    52194 2022-01-17 10:30:52.255424 time_lapse-4.0/demo/source/S60_050504_183149.jpg
+-rw-r--r--   0        0        0    51880 2022-01-17 10:30:52.255828 time_lapse-4.0/demo/source/S60_050504_183249.jpg
+-rw-r--r--   0        0        0    52125 2022-01-17 10:30:52.256144 time_lapse-4.0/demo/source/S60_050504_183349.jpg
+-rw-r--r--   0        0        0    52215 2022-01-17 10:30:52.256552 time_lapse-4.0/demo/source/S60_050504_183449.jpg
+-rw-r--r--   0        0        0    52445 2022-01-17 10:30:52.256862 time_lapse-4.0/demo/source/S60_050504_183549.jpg
+-rw-r--r--   0        0        0    52529 2022-01-17 10:30:52.257276 time_lapse-4.0/demo/source/S60_050504_183649.jpg
+-rw-r--r--   0        0        0    52935 2022-01-17 10:30:52.257600 time_lapse-4.0/demo/source/S60_050504_183749.jpg
+-rw-r--r--   0        0        0    52965 2022-01-17 10:30:52.257930 time_lapse-4.0/demo/source/S60_050504_184017.jpg
+-rw-r--r--   0        0        0    52445 2022-01-17 10:30:52.258247 time_lapse-4.0/demo/source/S60_050504_184117.jpg
+-rw-r--r--   0        0        0    52212 2022-01-17 10:30:52.258555 time_lapse-4.0/demo/source/S60_050504_184217.jpg
+-rw-r--r--   0        0        0    52202 2022-01-17 10:30:52.258963 time_lapse-4.0/demo/source/S60_050504_184317.jpg
+-rw-r--r--   0        0        0    51929 2022-01-17 10:30:52.259366 time_lapse-4.0/demo/source/S60_050504_184417.jpg
+-rw-r--r--   0        0        0    52125 2022-01-17 10:30:52.259678 time_lapse-4.0/demo/source/S60_050504_184517.jpg
+-rw-r--r--   0        0        0    51591 2022-01-17 10:30:52.259984 time_lapse-4.0/demo/source/S60_050504_184617.jpg
+-rw-r--r--   0        0        0    51855 2022-01-17 10:30:52.260285 time_lapse-4.0/demo/source/S60_050504_184717.jpg
+-rw-r--r--   0        0        0    51873 2022-01-17 10:30:52.260580 time_lapse-4.0/demo/source/S60_050504_184817.jpg
+-rw-r--r--   0        0        0    52124 2022-01-17 10:30:52.260883 time_lapse-4.0/demo/source/S60_050504_184917.jpg
+-rw-r--r--   0        0        0    52149 2022-01-17 10:30:52.261183 time_lapse-4.0/demo/source/S60_050504_185017.jpg
+-rw-r--r--   0        0        0    51641 2022-01-17 10:30:52.261451 time_lapse-4.0/demo/source/S60_050504_185117.jpg
+-rw-r--r--   0        0        0    52029 2022-01-17 10:30:52.261786 time_lapse-4.0/demo/source/S60_050504_185217.jpg
+-rw-r--r--   0        0        0    52155 2022-01-17 10:30:52.262164 time_lapse-4.0/demo/source/S60_050504_185317.jpg
+-rw-r--r--   0        0        0    51904 2022-01-17 10:30:52.262459 time_lapse-4.0/demo/source/S60_050504_185417.jpg
+-rw-r--r--   0        0        0    51874 2022-01-17 10:30:52.262749 time_lapse-4.0/demo/source/S60_050504_185517.jpg
+-rw-r--r--   0        0        0    52336 2022-01-17 10:30:52.263016 time_lapse-4.0/demo/source/S60_050504_185617.jpg
+-rw-r--r--   0        0        0    52336 2022-01-17 10:30:52.263278 time_lapse-4.0/demo/source/S60_050504_185717.jpg
+-rw-r--r--   0        0        0    51972 2022-01-17 10:30:52.263557 time_lapse-4.0/demo/source/S60_050504_185817.jpg
+-rw-r--r--   0        0        0    51917 2022-01-17 10:30:52.263837 time_lapse-4.0/demo/source/S60_050504_185917.jpg
+-rw-r--r--   0        0        0    51871 2022-01-17 10:30:52.264111 time_lapse-4.0/demo/source/S60_050504_190017.jpg
+-rw-r--r--   0        0        0    52177 2022-01-17 10:30:52.264378 time_lapse-4.0/demo/source/S60_050504_190117.jpg
+-rw-r--r--   0        0        0    52092 2022-01-17 10:30:52.264649 time_lapse-4.0/demo/source/S60_050504_190217.jpg
+-rw-r--r--   0        0        0    51864 2022-01-17 10:30:52.264925 time_lapse-4.0/demo/source/S60_050504_190317.jpg
+-rw-r--r--   0        0        0    52200 2022-01-17 10:30:52.265199 time_lapse-4.0/demo/source/S60_050504_190417.jpg
+-rw-r--r--   0        0        0    51954 2022-01-17 10:30:52.265462 time_lapse-4.0/demo/source/S60_050504_190517.jpg
+-rw-r--r--   0        0        0    52033 2022-01-17 10:30:52.265730 time_lapse-4.0/demo/source/S60_050504_190617.jpg
+-rw-r--r--   0        0        0    52688 2022-01-17 10:30:52.265994 time_lapse-4.0/demo/source/S60_050504_190717.jpg
+-rw-r--r--   0        0        0    52338 2022-01-17 10:30:52.266273 time_lapse-4.0/demo/source/S60_050504_190817.jpg
+-rw-r--r--   0        0        0    52243 2022-01-17 10:30:52.266545 time_lapse-4.0/demo/source/S60_050504_190917.jpg
+-rw-r--r--   0        0        0    52578 2022-01-17 10:30:52.266809 time_lapse-4.0/demo/source/S60_050504_191017.jpg
+-rw-r--r--   0        0        0    53033 2022-01-17 10:30:52.267093 time_lapse-4.0/demo/source/S60_050504_191117.jpg
+-rw-r--r--   0        0        0    52802 2022-01-17 10:30:52.267357 time_lapse-4.0/demo/source/S60_050504_191217.jpg
+-rw-r--r--   0        0        0    52858 2022-01-17 10:30:52.267639 time_lapse-4.0/demo/source/S60_050504_191417.jpg
+-rw-r--r--   0        0        0    52802 2022-01-17 10:30:52.267922 time_lapse-4.0/demo/source/S60_050504_191517.jpg
+-rw-r--r--   0        0        0    52941 2022-01-17 10:30:52.268192 time_lapse-4.0/demo/source/S60_050504_191617.jpg
+-rw-r--r--   0        0        0    52973 2022-01-17 10:30:52.268468 time_lapse-4.0/demo/source/S60_050504_191717.jpg
+-rw-r--r--   0        0        0    53037 2022-01-17 10:30:52.268760 time_lapse-4.0/demo/source/S60_050504_191817.jpg
+-rw-r--r--   0        0        0    52912 2022-01-17 10:30:52.269032 time_lapse-4.0/demo/source/S60_050504_191917.jpg
+-rw-r--r--   0        0        0    52819 2022-01-17 10:30:52.269288 time_lapse-4.0/demo/source/S60_050504_192017.jpg
+-rw-r--r--   0        0        0    53355 2022-01-17 10:30:52.269541 time_lapse-4.0/demo/source/S60_050504_192117.jpg
+-rw-r--r--   0        0        0    53243 2022-01-17 10:30:52.269788 time_lapse-4.0/demo/source/S60_050504_192217.jpg
+-rw-r--r--   0        0        0    53250 2022-01-17 10:30:52.270037 time_lapse-4.0/demo/source/S60_050504_192317.jpg
+-rw-r--r--   0        0        0    53299 2022-01-17 10:30:52.270277 time_lapse-4.0/demo/source/S60_050504_192417.jpg
+-rw-r--r--   0        0        0    53519 2022-01-17 10:30:52.270532 time_lapse-4.0/demo/source/S60_050504_192517.jpg
+-rw-r--r--   0        0        0     2538 2023-06-24 13:07:45.049828 time_lapse-4.0/pyproject.toml
+-rw-r--r--   0        0        0       14 2023-06-23 13:01:19.764663 time_lapse-4.0/requirements-ruff.txt
+-rw-r--r--   0        0        0        0 2022-01-17 10:30:52.274345 time_lapse-4.0/tests/__init__.py
+-rw-r--r--   0        0        0       61 2022-01-17 10:30:52.274470 time_lapse-4.0/time_lapse/__init__.py
+-rw-r--r--   0        0        0     3629 2023-06-16 15:03:59.335692 time_lapse-4.0/time_lapse/check_interval.py
+-rw-r--r--   0        0        0     1834 2023-06-16 15:14:40.513817 time_lapse-4.0/time_lapse/cli.py
+-rw-r--r--   0        0        0      306 2023-06-16 15:03:59.336314 time_lapse-4.0/time_lapse/detect_audio.py
+-rwxr-xr-x   0        0        0    98228 2022-01-17 10:30:52.275448 time_lapse-4.0/time_lapse/fonts/Jost-400-Book.ttf
+-rwxr-xr-x   0        0        0     3627 2022-01-17 10:30:52.275875 time_lapse-4.0/time_lapse/fonts/LICENSE.md
+-rw-r--r--   0        0        0     2271 2023-06-16 15:03:59.336503 time_lapse-4.0/time_lapse/output.py
+-rw-r--r--   0        0        0        0 2023-06-16 15:03:59.336545 time_lapse-4.0/time_lapse/py.typed
+-rw-r--r--   0        0        0     1131 2023-06-16 15:03:59.336751 time_lapse-4.0/time_lapse/source.py
+-rw-r--r--   0        0        0      693 2023-06-16 15:03:59.336913 time_lapse-4.0/time_lapse/watermark.py
+-rw-r--r--   0        0        0     4941 1970-01-01 00:00:00.000000 time_lapse-4.0/PKG-INFO
```

### Comparing `time-lapse-3/LICENSE` & `time_lapse-4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `time-lapse-3/Makefile` & `time_lapse-4.0/Makefile`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,34 @@
+.PHONY: ruffinstall
+ruffinstall:
+	pip install --upgrade pip
+	pip install --upgrade --upgrade-strategy eager -r requirements-ruff.txt
+
 .PHONY: devinstall
 devinstall:
 	pip install --upgrade pip
 	pip install --upgrade --upgrade-strategy eager --editable .[dev]
 
 .PHONY: test
-test: flaketest checksetup unittests
+test: rufftest mypytest checksetup unittests
 
-.PHONY: flaketest
-flaketest:
-	flake8
+.PHONY: rufftest
+rufftest:
+	ruff .
+
+.PHONY: mypytest
+mypytest:
+	mypy .
 
 .PHONY: checksetup
 checksetup:
 	python setup.py check -ms
 
-.PHONY: unittests
-unittests:
+.PHONY: unittest
+unittest:
 	python -m unittest discover --catch --start-directory tests --top-level-directory .
 
 .PHONY: clean
 clean:
 	rm -rf build dist
 
 .PHONY: build
```

### Comparing `time-lapse-3/PKG-INFO` & `time_lapse-4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: time-lapse
-Version: 3
+Version: 4.0
 Summary: Time-lapse movie assembly
-Home-page: https://github.com/153957/time-lapse
-Author: Arne de Laat
-Author-email: arne@delaat.net
-Maintainer: Arne de Laat
-Maintainer-email: arne@delaat.net
-License: MIT
 Keywords: ffmpeg,photography,time-lapse
+Author-email: Arne de Laat <arne@delaat.net>
+Maintainer-email: Arne de Laat <arne@delaat.net>
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Video :: Conversion
-Description-Content-Type: text/markdown
-Provides-Extra: graph
+Requires-Dist: exifreader==0.1.1
+Requires-Dist: ffmpeg-python==0.2.0
+Requires-Dist: coverage ; extra == "dev"
+Requires-Dist: flit ; extra == "dev"
+Requires-Dist: mypy ; extra == "dev"
+Requires-Dist: graphviz ; extra == "graph"
+Project-URL: Homepage, https://arne.delaat.net/timelapse.html
+Project-URL: Repository, https://github.com/153957/time-lapse
 Provides-Extra: dev
-License-File: LICENSE
+Provides-Extra: graph
 
 Time-Lapse assembling
 =====================
 
 [![PyPI](https://img.shields.io/pypi/v/time-lapse)](https://pypi.org/project/time-lapse/)
-[![License](https://img.shields.io/github/license/153957/time-lapse)](https://github.com/153957/time-lapse/blob/master/LICENSE)
-[![Build](https://img.shields.io/github/workflow/status/153957/time-lapse/Run%20tests)](https://github.com/153957/time-lapse/actions)
+[![License](https://img.shields.io/github/license/153957/time-lapse)](https://github.com/153957/time-lapse/blob/main/LICENSE)
+[![Build](https://img.shields.io/github/actions/workflow/status/153957/time-lapse/tests.yml?branch=main)](https://github.com/153957/time-lapse/actions)
 
 This repo contains tools used to compile Time-lapse movies using
 ffmpeg. The ffmpeg utility is controlled via the ffmpeg-python wrapper.
 
 Example usage of this package can be found in the
 [time-lapse scripts](https://github.com/153957/time-lapse-scripts) repository.
 
@@ -103,27 +107,27 @@
 should be given using `-framerate 30`.
 
 Filters
 =======
 
 Commonly used filters:
 
--   Deflicker <https://ffmpeg.org/ffmpeg-filters.html#toc-deflicker>
--   Scale <https://ffmpeg.org/ffmpeg-filters.html#scale>
--   Crop <https://ffmpeg.org/ffmpeg-filters.html#crop>
--   Drawtext <https://ffmpeg.org/ffmpeg-filters.html#drawtext-1>
--   Video sizes <https://ffmpeg.org/ffmpeg-utils.html#video-size-syntax>
+- Deflicker <https://ffmpeg.org/ffmpeg-filters.html#toc-deflicker>
+- Scale <https://ffmpeg.org/ffmpeg-filters.html#scale>
+- Crop <https://ffmpeg.org/ffmpeg-filters.html#crop>
+- Drawtext <https://ffmpeg.org/ffmpeg-filters.html#drawtext-1>
+- Video sizes <https://ffmpeg.org/ffmpeg-utils.html#video-size-syntax>
 
 Steps
 -----
 
--   First deflicker the video to ensure it is equally deflickered for
-    all outputs
--   Then scale and crop the videos to fit the desired final resolutions
--   Then add the watermark (which should not be deflickered)
+- First deflicker the video to ensure it is equally deflickered for
+  all outputs
+- Then scale and crop the videos to fit the desired final resolutions
+- Then add the watermark (which should not be deflickered)
 
 Scale video
 -----------
 
 Add scaling to ensure it fits in given dimensions. Negative values for
 width or height make the encoder figure out the size by itself, keeping
 the aspect ratio of the source. The integer of the negative value, i.e.
@@ -153,7 +157,8 @@
 Show the ffmpeg command options ffmpeg-python would use:
 
     .get_args()
 
 By using graphviz the graph from input to output can be shown using:
 
     .view()
+
```

### Comparing `time-lapse-3/README.md` & `time_lapse-4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Time-Lapse assembling
 =====================
 
 [![PyPI](https://img.shields.io/pypi/v/time-lapse)](https://pypi.org/project/time-lapse/)
-[![License](https://img.shields.io/github/license/153957/time-lapse)](https://github.com/153957/time-lapse/blob/master/LICENSE)
-[![Build](https://img.shields.io/github/workflow/status/153957/time-lapse/Run%20tests)](https://github.com/153957/time-lapse/actions)
+[![License](https://img.shields.io/github/license/153957/time-lapse)](https://github.com/153957/time-lapse/blob/main/LICENSE)
+[![Build](https://img.shields.io/github/actions/workflow/status/153957/time-lapse/tests.yml?branch=main)](https://github.com/153957/time-lapse/actions)
 
 This repo contains tools used to compile Time-lapse movies using
 ffmpeg. The ffmpeg utility is controlled via the ffmpeg-python wrapper.
 
 Example usage of this package can be found in the
 [time-lapse scripts](https://github.com/153957/time-lapse-scripts) repository.
 
@@ -81,27 +81,27 @@
 should be given using `-framerate 30`.
 
 Filters
 =======
 
 Commonly used filters:
 
--   Deflicker <https://ffmpeg.org/ffmpeg-filters.html#toc-deflicker>
--   Scale <https://ffmpeg.org/ffmpeg-filters.html#scale>
--   Crop <https://ffmpeg.org/ffmpeg-filters.html#crop>
--   Drawtext <https://ffmpeg.org/ffmpeg-filters.html#drawtext-1>
--   Video sizes <https://ffmpeg.org/ffmpeg-utils.html#video-size-syntax>
+- Deflicker <https://ffmpeg.org/ffmpeg-filters.html#toc-deflicker>
+- Scale <https://ffmpeg.org/ffmpeg-filters.html#scale>
+- Crop <https://ffmpeg.org/ffmpeg-filters.html#crop>
+- Drawtext <https://ffmpeg.org/ffmpeg-filters.html#drawtext-1>
+- Video sizes <https://ffmpeg.org/ffmpeg-utils.html#video-size-syntax>
 
 Steps
 -----
 
--   First deflicker the video to ensure it is equally deflickered for
-    all outputs
--   Then scale and crop the videos to fit the desired final resolutions
--   Then add the watermark (which should not be deflickered)
+- First deflicker the video to ensure it is equally deflickered for
+  all outputs
+- Then scale and crop the videos to fit the desired final resolutions
+- Then add the watermark (which should not be deflickered)
 
 Scale video
 -----------
 
 Add scaling to ensure it fits in given dimensions. Negative values for
 width or height make the encoder figure out the size by itself, keeping
 the aspect ratio of the source. The integer of the negative value, i.e.
```

### Comparing `time-lapse-3/time_lapse/check_interval.py` & `time_lapse-4.0/time_lapse/check_interval.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,121 +1,126 @@
 import argparse
 import datetime
 import pathlib
 
+from dataclasses import dataclass
 from glob import glob
+from operator import attrgetter
 
 import exifreader
 
 MARGIN = datetime.timedelta(seconds=0.2)
-MIN_IMAGES_SEQUENCE = 5
+MIN_INTERVAL = datetime.timedelta(seconds=0.4)
+MIN_IMAGES_SEQUENCE = 20
 
 
-def get_image_date(image_path):
+def get_image_date(image_path: str) -> datetime.datetime:
     """Get EXIF image date from an image as a datetime"""
-    with open(image_path, 'rb') as _file:
+    with pathlib.Path(image_path).open('rb') as _file:
         tags = exifreader.process_file(_file, details=False)
     date_time = tags['EXIF DateTimeOriginal'].values
     subsec = tags['EXIF SubSecTimeOriginal'].values
-    full_date_time = f'{date_time}.{subsec}'
-    image_date = datetime.datetime.strptime(full_date_time, '%Y:%m:%d %H:%M:%S.%f')
+    full_date_time = f'{date_time}.{subsec}+0000'
+    image_date = datetime.datetime.strptime(full_date_time, '%Y:%m:%d %H:%M:%S.%f%z')
     return image_date
 
 
-def find_sequences(pattern, shots_per_interval):
+@dataclass
+class ImageInfo:
+    path: pathlib.Path
+    date: datetime.datetime
+
+
+def find_sequences(pattern: str, shots_per_interval: int, group: bool) -> None:
     skip = shots_per_interval
     files = sorted(glob(pattern))
-    image_dates = [
-        {'path': pathlib.Path(path).name, 'date': get_image_date(path)}
-        for path in files[::skip]
-    ]
 
-    n_same_interval = 1
-    start_of_sequence = image_dates[0]['path']
+    if not files:
+        print(f'Found no matching files the pattern "{pattern}"')
+        return
+
+    image_dates = sorted(
+        (ImageInfo(path=pathlib.Path(path), date=get_image_date(path)) for path in files[::skip]),
+        key=attrgetter('date'),
+    )
+
+    start_of_sequence = image_dates[0].path
+    sequence = [start_of_sequence]
+    nth_sequence = 1
 
     print(
+        ' seq',
         '   n',
         'interval',
         'sequence',
-        sep='\t'
+        sep='\t',
     )
 
-    for i, (previous, current, following) in enumerate(zip(image_dates[:-2], image_dates[1:-1], image_dates[2:]), 1):
-        n_same_interval += 1
+    for previous, current, following in zip(image_dates[:-2], image_dates[1:-1], image_dates[2:], strict=True):
+        sequence.append(current.path)
 
-        interval = current['date'] - previous['date']
-        new_interval = following['date'] - current['date']
+        interval = current.date - previous.date
+        new_interval = following.date - current.date
 
-        if abs(interval - new_interval) > MARGIN:
-            if n_same_interval > MIN_IMAGES_SEQUENCE:
+        if interval < MIN_INTERVAL or abs(interval - new_interval) > MARGIN:
+            if len(sequence) > MIN_IMAGES_SEQUENCE:
                 print(
-                    f'{n_same_interval:4}',
+                    f'{nth_sequence:4}',
+                    f'{len(sequence):4}',
                     f'{interval.total_seconds():7}s',
-                    f'{start_of_sequence} → {current["path"]}',
-                    sep='\t'
+                    f'{sequence[0]} → {sequence[-1]}',
+                    sep='\t',
                 )
-            start_of_sequence = current['path']
-            n_same_interval = 1
-
-    n_same_interval += 1
+                if group:
+                    group_sequence(sequence, nth_sequence)
+                nth_sequence += 1
+            sequence = [current.path]
 
-    if n_same_interval > MIN_IMAGES_SEQUENCE:
+    sequence.append(following.path)
+    if len(sequence) > MIN_IMAGES_SEQUENCE:
         print(
-            f'{n_same_interval:4}',
+            f'{len(sequence):4}',
             f'{new_interval.total_seconds():7}s',
-            f'{start_of_sequence} → {following["path"]}',
-            sep='\t'
+            f'{sequence[0]} → {sequence[-1]}',
+            sep='\t',
         )
+        if group:
+            group_sequence(sequence, nth_sequence)
 
 
-def find_outliers(pattern, shots_per_interval):
-    skip = shots_per_interval
-    files = sorted(glob(pattern))
-    image_dates = [
-        {'path': pathlib.Path(path).name, 'date': get_image_date(path)}
-        for path in files[::skip]
-    ]
-    outliers = []
-
-    n_since_last_change = 0
-    previous_interval = datetime.timedelta()
-
-    for i, (previous, current) in enumerate(zip(image_dates[:-1], image_dates[1:]), 1):
-        n_since_last_change += 1
-        interval = current['date'] - previous['date']
-        if previous_interval and abs(interval - previous_interval) > MARGIN:
-            outliers.append((interval, previous['path'], current['path']))
-            print(
-                f'{i:5} – '
-                f'{n_since_last_change:4} – '
-                f'{previous_interval.total_seconds():6}s → {interval.total_seconds():6}s – '
-                f'{previous["path"]} → {current["path"]}'
-            )
-            n_since_last_change = 0
-        previous_interval = interval
+def group_sequence(sequence: list[pathlib.Path], sequence_number: int) -> None:
+    """Group all files in the sequence into a subdirectory in the working directory"""
 
-    return outliers
+    pathlib.Path(f'sequence_{sequence_number}').mkdir()
+    for path in sequence:
+        path.rename(f'sequence_{sequence_number}/{path.name}')
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser(description='.')
     parser.add_argument(
         '--pattern',
         default='*.NEF',
-        help='Regex pattern with which to find the input frames.',
+        help='Glob pattern with which to find the input frames.',
     )
     parser.add_argument(
         '--shots_per_interval',
         type=int,
         default=1,
         help='Number of images per interval, e.g. in case of HDR shots.',
     )
+    parser.add_argument(
+        '--group',
+        action='store_true',
+        help='Group images in the same interval into directories.',
+    )
     args = parser.parse_args()
 
     find_sequences(
         args.pattern,
         args.shots_per_interval,
+        args.group,
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `time-lapse-3/time_lapse/cli.py` & `time_lapse-4.0/time_lapse/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 import argparse
 
 from time_lapse import output, source
 
 
-def make_movie(name, patterns, fps, deflicker, watermark, verbose, dryrun):
-    source_input = source.get_input(patterns, fps, deflicker)
+def make_movie(
+    name: str,
+    patterns: list[str],
+    fps: int,
+    deflicker: int,
+    watermark: list[str],
+    verbose: bool,
+    dryrun: bool,
+    filters: list[tuple[str, dict[str, str]]] | None = None,
+) -> None:
+    source_input = source.get_input(patterns, fps, deflicker, filters)
     output.create_outputs(source_input, name, watermark=watermark, verbose=verbose, dryrun=dryrun)
 
 
-def main():
+def main() -> None:
     parser = argparse.ArgumentParser(description='Combine frames into a movie.')
     parser.add_argument(
         '--name',
         help='Output name of the movie, without file extension.',
         default='output',
     )
     parser.add_argument(
         '--pattern',
         help='Glob pattern(s) with which to find the input frames.',
         default='*.tiff',
         nargs='+',
+        dest='patterns',
     )
     parser.add_argument(
         '--fps',
         help='Frame rate of the created movie.',
         type=int,
         default=30,
         choices=[1, 2, 6, 12, 15, 24, 25, 30, 48, 50, 60, 120, 240, 300],
@@ -39,20 +49,21 @@
         help='Do not perform the ffmpeg command, only show it.',
         action='store_true',
     )
     parser.add_argument(
         '--quiet',
         help='Produce less output, i.e. no graph and ffmpeg command.',
         action='store_false',
+        dest='verbose',
     )
     parser.add_argument(
         '--watermark',
         help='Add watermark, provide two value, one main text and the subtext.',
         nargs=2,
     )
-    args = parser.parse_args()
+    kwargs = vars(parser.parse_args())
 
-    make_movie(args.name, args.pattern, args.fps, args.deflicker, args.watermark, args.quiet, args.dryrun)
+    make_movie(**kwargs)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `time-lapse-3/time_lapse/fonts/Jost-400-Book.ttf` & `time_lapse-4.0/time_lapse/fonts/Jost-400-Book.ttf`

 * *Files identical despite different names*

### Comparing `time-lapse-3/time_lapse/output.py` & `time_lapse-4.0/time_lapse/output.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import ffmpeg
 
 from .watermark import add_watermark
 
-OUTPUT_OPTIONS = {
+OUTPUT_OPTIONS: dict[str, str | int] = {
     'crf': 20,
     'preset': 'slower',
     'movflags': 'faststart',
-    'pix_fmt': 'yuv420p'
+    'pix_fmt': 'yuv420p',
 }
 
 
 def create_outputs(
-    source_input,
-    name,
-    framerate=None,
-    watermark=True,
-    verbose=False,
-    dryrun=False,
-):
+    source_input: ffmpeg.nodes.FilterNode,
+    name: str,
+    framerate: int | None = None,
+    watermark: bool | list[str] = True,
+    verbose: bool = False,
+    dryrun: bool = False,
+) -> ffmpeg.nodes.OutputNode:
     """Create output at multiple sizes (FHD and qHD)
 
     :param source_input: ffmpeg input node ready for scaling and conversion.
     :param name: name of the output.
     :param watermark: if True the default watermark will be added to the movie,
         if a tuple is provided the contained strings are used for the main an sub lines.
     :param verbose: if True output the ffmpeg CLI command which will be used.
@@ -38,28 +38,29 @@
         else:
             text, subtext = watermark
         watermarked_input = add_watermark(fhd_input, text, subtext, fontsize=32)
         split_input = watermarked_input.split()
     else:
         split_input = fhd_input.split()
 
+    output_options: dict[str, str | int]
     if framerate:
         output_options = {'r': framerate, **OUTPUT_OPTIONS}
     else:
-        output_options = OUTPUT_OPTIONS
+        output_options = {**OUTPUT_OPTIONS}
 
     output = ffmpeg.merge_outputs(
         # 1920x1080 (1920x1280)
         split_input[0].output(f'{name}.mp4', **output_options),
         # 960x540 (960x640)
         (
             split_input[1]
             .filter_('scale', size='qhd', force_original_aspect_ratio='increase')
             .output(f'{name}_960.mp4', **output_options)
-        )
+        ),
     )
 
     if verbose:
         print('ffmpeg ' + ' '.join(output.get_args()))
         try:
             output.view(filename=f'{name}')  # Automatically suffixed with .pdf
         except ImportError:
```

