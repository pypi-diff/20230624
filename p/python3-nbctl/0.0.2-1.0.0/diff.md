# Comparing `tmp/python3-nbctl-0.0.2.tar.gz` & `tmp/python3-nbctl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-nbctl-0.0.2.tar", last modified: Sat Jun 24 07:12:54 2023, max compression
+gzip compressed data, was "python3-nbctl-1.0.0.tar", last modified: Sat Jun 24 08:54:31 2023, max compression
```

## Comparing `python3-nbctl-0.0.2.tar` & `python3-nbctl-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 07:12:54.457710 python3-nbctl-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 07:12:54.453710 python3-nbctl-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 07:12:54.457710 python3-nbctl-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/.github/workflows/actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/.github/workflows/greetings.yml
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/.github/workflows/label.yml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-24 07:12:54.000000 python3-nbctl-0.0.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-24 07:12:54.000000 python3-nbctl-0.0.2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-24 07:12:54.457710 python3-nbctl-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/entrypoint.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 07:12:54.457710 python3-nbctl-0.0.2/nbctl/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/nbctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/nbctl/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/nbctl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/nbctl/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 07:12:54.457710 python3-nbctl-0.0.2/python3_nbctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-24 07:12:54.000000 python3-nbctl-0.0.2/python3_nbctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-24 07:12:54.000000 python3-nbctl-0.0.2/python3_nbctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 07:12:54.000000 python3-nbctl-0.0.2/python3_nbctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-24 07:12:54.000000 python3-nbctl-0.0.2/python3_nbctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 07:12:54.000000 python3-nbctl-0.0.2/python3_nbctl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-24 07:12:54.000000 python3-nbctl-0.0.2/python3_nbctl.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 07:12:54.000000 python3-nbctl-0.0.2/python3_nbctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 07:12:54.000000 python3-nbctl-0.0.2/python3_nbctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-24 07:12:54.457710 python3-nbctl-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-24 07:12:40.000000 python3-nbctl-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:54:31.157979 python3-nbctl-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:54:31.153979 python3-nbctl-1.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:54:31.153979 python3-nbctl-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/.github/workflows/actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/.github/workflows/greetings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/.github/workflows/label.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-24 08:54:31.000000 python3-nbctl-1.0.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-24 08:54:31.000000 python3-nbctl-1.0.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-24 08:54:31.157979 python3-nbctl-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/entrypoint.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:54:31.157979 python3-nbctl-1.0.0/nbctl/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/nbctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/nbctl/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/nbctl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/nbctl/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:54:31.157979 python3-nbctl-1.0.0/python3_nbctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-24 08:54:31.000000 python3-nbctl-1.0.0/python3_nbctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-24 08:54:31.000000 python3-nbctl-1.0.0/python3_nbctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:54:31.000000 python3-nbctl-1.0.0/python3_nbctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-24 08:54:31.000000 python3-nbctl-1.0.0/python3_nbctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:54:31.000000 python3-nbctl-1.0.0/python3_nbctl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-24 08:54:31.000000 python3-nbctl-1.0.0/python3_nbctl.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-24 08:54:31.000000 python3-nbctl-1.0.0/python3_nbctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-24 08:54:31.000000 python3-nbctl-1.0.0/python3_nbctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-24 08:54:31.157979 python3-nbctl-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-24 08:54:19.000000 python3-nbctl-1.0.0/setup.py
```

### Comparing `python3-nbctl-0.0.2/.github/workflows/publish.yml` & `python3-nbctl-1.0.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `python3-nbctl-0.0.2/Dockerfile` & `python3-nbctl-1.0.0/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 ENV LC_ALL C.UTF-8
 ENV LANG en_US.UTF-8
 ENV LANGUAGE en_US.UTF-8
 
 # apt install -y docker-ce docker-ce-cli containerd.io; systemctl start docker
 RUN apt update && \
-    apt install -y git python3 python3-pip skopeo jq && \
+    apt install -y git python3 python3-pip && \
     cd ~ && \
     git clone https://github.com/x-actions/python3-nbctl.git && \
     cd python3-nbctl && \
     git checkout v1 && \
     pip3 install -r requirements.txt && \
     python3 setup.py --version && \
     python3 setup.py install
```

### Comparing `python3-nbctl-0.0.2/LICENSE` & `python3-nbctl-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python3-nbctl-0.0.2/PKG-INFO` & `python3-nbctl-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: python3-nbctl
-Version: 0.0.2
-Summary: Convert ipynb to hugo markdown files
+Version: 1.0.0
+Summary: convert jupyter *.ipynb file to markdown files
 Home-page: https://www.xiexianbin.cn/
 Author: xiexianbin
 Author-email: me@xiexianbin.cn
 Project-URL: Bug Tracker, https://github.com/x-actions/python3-nbctl/issues
 Project-URL: Source Code, https://github.com/x-actions/python3-nbctl
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -16,39 +16,42 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # python3-nbctl
 
-将ipynb文件转化为hugo markdown文件/Convert ipynb to hugo markdown files
+将ipynb文件转化为markdown文件/convert jupyter *.ipynb file to markdown files
 
 [![PyPI-python3-nbctl](https://img.shields.io/pypi/v/python3-nbctl.svg?maxAge=3600)](https://pypi.org/project/python3-nbctl/)
 
 Github Actions for [Container ipynb to markdown](https://github.com/marketplace/actions/nbctl)
 
 ## How to Use by Github Actions
 
 ```
-      - name: install nbctl
+      - name: convert jupyter *.ipynb file to markdown
         uses: x-actions/python3-nbctl@v1
-      - name: convert ipynb to hugo markdown
-        run: |
-          find static/code/ai -type f -name "*.ipynb" | grep -v ".ipynb_checkpoints" | xargs -I{} nbctl --input {} -f
+        with:
+          script: >
+            find <path> -type f -name "*.ipynb" | grep -v ".ipynb_checkpoints" | xargs -I{} nbctl --input {} --force --debug
 ```
 
 ## Dev and Test
 
 - local run
 
 ```
 # install
 pip3 install -r requirements.txt
 python3 setup.py install
 
 # or
 pip3 install python3-nbctl
+```
+
+- help
 
-# run
-nbctl
+```
+nbctl --help
 ```
```

### Comparing `python3-nbctl-0.0.2/README.md` & `python3-nbctl-1.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # python3-nbctl
 
-将ipynb文件转化为hugo markdown文件/Convert ipynb to hugo markdown files
+将ipynb文件转化为markdown文件/convert jupyter *.ipynb file to markdown files
 
 [![PyPI-python3-nbctl](https://img.shields.io/pypi/v/python3-nbctl.svg?maxAge=3600)](https://pypi.org/project/python3-nbctl/)
 
 Github Actions for [Container ipynb to markdown](https://github.com/marketplace/actions/nbctl)
 
 ## How to Use by Github Actions
 
 ```
-      - name: install nbctl
+      - name: convert jupyter *.ipynb file to markdown
         uses: x-actions/python3-nbctl@v1
-      - name: convert ipynb to hugo markdown
-        run: |
-          find static/code/ai -type f -name "*.ipynb" | grep -v ".ipynb_checkpoints" | xargs -I{} nbctl --input {} -f
+        with:
+          script: >
+            find <path> -type f -name "*.ipynb" | grep -v ".ipynb_checkpoints" | xargs -I{} nbctl --input {} --force --debug
 ```
 
 ## Dev and Test
 
 - local run
 
 ```
 # install
 pip3 install -r requirements.txt
 python3 setup.py install
 
 # or
 pip3 install python3-nbctl
+```
+
+- help
 
-# run
-nbctl
+```
+nbctl --help
 ```
```

### Comparing `python3-nbctl-0.0.2/nbctl/__init__.py` & `python3-nbctl-1.0.0/nbctl/__init__.py`

 * *Files identical despite different names*

### Comparing `python3-nbctl-0.0.2/nbctl/constants.py` & `python3-nbctl-1.0.0/nbctl/constants.py`

 * *Files identical despite different names*

### Comparing `python3-nbctl-0.0.2/nbctl/logger.py` & `python3-nbctl-1.0.0/nbctl/logger.py`

 * *Files identical despite different names*

### Comparing `python3-nbctl-0.0.2/nbctl/shell.py` & `python3-nbctl-1.0.0/nbctl/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 #         http://www.apache.org/licenses/LICENSE-2.0
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
-"""convert ipynb to hugo markdown."""
+"""convert jupyter *.ipynb file to markdown"""
 
 import argparse
 import os
 import sys
 from typing import Dict
 
 import nbformat
 from nbconvert import MarkdownExporter
 from traitlets.config import Config
 
 from nbctl import constants
 from nbctl import logger
 
 
-parser = argparse.ArgumentParser(description='convert ipynb to hugo markdown.')
+parser = argparse.ArgumentParser(description='convert jupyter *.ipynb file to markdown')
 parser.add_argument('--debug', '-d', help='show debug info, default is INFO',
                     action="store_true")
 parser.add_argument('--input', '-i', help='input *.ipynb file or dir', 
                     required=True, default='', type=str)
 parser.add_argument('--output', '-o', help='output file or dir', 
                     required=False, default='', type=str)
 parser.add_argument('--force', '-f', help='force overwrite output file', 
@@ -109,15 +109,15 @@
         return True
 
 
     def do(self):
         # check param
         if os.path.exists(self.input):
             if os.path.isdir(self.input):
-                for (dirpath, dirnames, filenames) in os.walk():
+                for (dirpath, dirnames, filenames) in os.walk(self.input):
                     self.logger.debug(f'dirpath: {dirpath}, dirnames: {dirnames}, filenames: {filenames}')
             else:
                 self.render_one(ipynb_path=self.input, markdown_dir=self.output)
         else:
             print(f'dir {self.input} not exists, exit 1.')
             sys.exit(1)
```

### Comparing `python3-nbctl-0.0.2/python3_nbctl.egg-info/PKG-INFO` & `python3-nbctl-1.0.0/python3_nbctl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: python3-nbctl
-Version: 0.0.2
-Summary: Convert ipynb to hugo markdown files
+Version: 1.0.0
+Summary: convert jupyter *.ipynb file to markdown files
 Home-page: https://www.xiexianbin.cn/
 Author: xiexianbin
 Author-email: me@xiexianbin.cn
 Project-URL: Bug Tracker, https://github.com/x-actions/python3-nbctl/issues
 Project-URL: Source Code, https://github.com/x-actions/python3-nbctl
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
@@ -16,39 +16,42 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # python3-nbctl
 
-将ipynb文件转化为hugo markdown文件/Convert ipynb to hugo markdown files
+将ipynb文件转化为markdown文件/convert jupyter *.ipynb file to markdown files
 
 [![PyPI-python3-nbctl](https://img.shields.io/pypi/v/python3-nbctl.svg?maxAge=3600)](https://pypi.org/project/python3-nbctl/)
 
 Github Actions for [Container ipynb to markdown](https://github.com/marketplace/actions/nbctl)
 
 ## How to Use by Github Actions
 
 ```
-      - name: install nbctl
+      - name: convert jupyter *.ipynb file to markdown
         uses: x-actions/python3-nbctl@v1
-      - name: convert ipynb to hugo markdown
-        run: |
-          find static/code/ai -type f -name "*.ipynb" | grep -v ".ipynb_checkpoints" | xargs -I{} nbctl --input {} -f
+        with:
+          script: >
+            find <path> -type f -name "*.ipynb" | grep -v ".ipynb_checkpoints" | xargs -I{} nbctl --input {} --force --debug
 ```
 
 ## Dev and Test
 
 - local run
 
 ```
 # install
 pip3 install -r requirements.txt
 python3 setup.py install
 
 # or
 pip3 install python3-nbctl
+```
+
+- help
 
-# run
-nbctl
+```
+nbctl --help
 ```
```

### Comparing `python3-nbctl-0.0.2/python3_nbctl.egg-info/SOURCES.txt` & `python3-nbctl-1.0.0/python3_nbctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3-nbctl-0.0.2/setup.cfg` & `python3-nbctl-1.0.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-nbctl
-summary = Convert ipynb to hugo markdown files
+summary = convert jupyter *.ipynb file to markdown files
 description_file = 
 	README.md
 author = xiexianbin
 author_email = me@xiexianbin.cn
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.xiexianbin.cn/
```

### Comparing `python3-nbctl-0.0.2/setup.py` & `python3-nbctl-1.0.0/setup.py`

 * *Files identical despite different names*

