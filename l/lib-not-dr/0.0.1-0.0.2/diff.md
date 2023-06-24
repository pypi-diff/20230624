# Comparing `tmp/lib-not-dr-0.0.1.tar.gz` & `tmp/lib-not-dr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-not-dr-0.0.1.tar", last modified: Sat Jun 24 12:31:11 2023, max compression
+gzip compressed data, was "lib-not-dr-0.0.2.tar", last modified: Sat Jun 24 13:01:22 2023, max compression
```

## Comparing `lib-not-dr-0.0.1.tar` & `lib-not-dr-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 12:31:11.148639 lib-not-dr-0.0.1/
--rw-rw-rw-   0        0        0    17098 2023-06-09 16:24:01.000000 lib-not-dr-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    20517 2023-06-24 12:31:11.147637 lib-not-dr-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       67 2023-06-09 16:24:01.000000 lib-not-dr-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 12:31:11.127638 lib-not-dr-0.0.1/lib_not_dr/
--rw-rw-rw-   0        0        0      205 2023-06-17 04:45:09.000000 lib-not-dr-0.0.1/lib_not_dr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 12:31:11.138639 lib-not-dr-0.0.1/lib_not_dr/nuitka/
--rw-rw-rw-   0        0        0     5758 2023-06-17 06:41:41.000000 lib-not-dr-0.0.1/lib_not_dr/nuitka/compile.py
-drwxrwxrwx   0        0        0        0 2023-06-24 12:31:11.145636 lib-not-dr-0.0.1/lib_not_dr/types/
--rw-rw-rw-   0        0        0      785 2023-06-17 04:51:13.000000 lib-not-dr-0.0.1/lib_not_dr/types/__init__.py
--rw-rw-rw-   0        0        0     8958 2023-06-17 04:45:09.000000 lib-not-dr-0.0.1/lib_not_dr/types/options.py
--rw-rw-rw-   0        0        0     8114 2023-06-17 04:49:52.000000 lib-not-dr-0.0.1/lib_not_dr/types/version.py
-drwxrwxrwx   0        0        0        0 2023-06-24 12:31:11.135638 lib-not-dr-0.0.1/lib_not_dr.egg-info/
--rw-rw-rw-   0        0        0    20517 2023-06-24 12:31:11.000000 lib-not-dr-0.0.1/lib_not_dr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-06-24 12:31:11.000000 lib-not-dr-0.0.1/lib_not_dr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 12:31:11.000000 lib-not-dr-0.0.1/lib_not_dr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 12:31:11.000000 lib-not-dr-0.0.1/lib_not_dr.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      383 2023-06-24 12:31:05.000000 lib-not-dr-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-24 12:31:11.148639 lib-not-dr-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 13:01:22.186917 lib-not-dr-0.0.2/
+-rw-rw-rw-   0        0        0    17098 2023-06-09 16:24:01.000000 lib-not-dr-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0    21199 2023-06-24 13:01:22.185917 lib-not-dr-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      749 2023-06-24 12:58:45.000000 lib-not-dr-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 13:01:22.134799 lib-not-dr-0.0.2/lib_not_dr/
+-rw-rw-rw-   0        0        0      205 2023-06-17 04:45:09.000000 lib-not-dr-0.0.2/lib_not_dr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:01:22.159798 lib-not-dr-0.0.2/lib_not_dr/nuitka/
+-rw-rw-rw-   0        0        0     6464 2023-06-24 12:56:32.000000 lib-not-dr-0.0.2/lib_not_dr/nuitka/compile.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:01:22.174799 lib-not-dr-0.0.2/lib_not_dr/types/
+-rw-rw-rw-   0        0        0      785 2023-06-17 04:51:13.000000 lib-not-dr-0.0.2/lib_not_dr/types/__init__.py
+-rw-rw-rw-   0        0        0     8958 2023-06-17 04:45:09.000000 lib-not-dr-0.0.2/lib_not_dr/types/options.py
+-rw-rw-rw-   0        0        0     8114 2023-06-17 04:49:52.000000 lib-not-dr-0.0.2/lib_not_dr/types/version.py
+drwxrwxrwx   0        0        0        0 2023-06-24 13:01:22.154798 lib-not-dr-0.0.2/lib_not_dr.egg-info/
+-rw-rw-rw-   0        0        0    21199 2023-06-24 13:01:22.000000 lib-not-dr-0.0.2/lib_not_dr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-06-24 13:01:22.000000 lib-not-dr-0.0.2/lib_not_dr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 13:01:22.000000 lib-not-dr-0.0.2/lib_not_dr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-24 13:01:22.000000 lib-not-dr-0.0.2/lib_not_dr.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      393 2023-06-24 13:00:19.000000 lib-not-dr-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-24 13:01:22.187918 lib-not-dr-0.0.2/setup.cfg
```

### Comparing `lib-not-dr-0.0.1/LICENSE` & `lib-not-dr-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.1/PKG-INFO` & `lib-not-dr-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-not-dr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python lib created from Difficult Rocket development
 Author-email: shenjackyuanjie <3695888@qq.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -380,8 +380,43 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lib-not-dr
-A python lib came from Difficult Rocket development
+
+A python lib came from [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) development
+
+一个在 [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) 开发中 分离出来的 python 库
+
+## Information/信息
+
+- Version/版本: 0.0.2
+
+### Author/作者
+
+[shenjackyuanjie](https://github/shenjackyuanjie)
+
+### License/许可证
+
+[MPL-2.0](https://www.mozilla.org/en-US/MPL/2.0/)
+
+## 安装/Install
+
+```bash
+pip install lib-not-dr
+```
+
+## 使用/Usage
+
+### Nuitka Compiler Helper
+
+```python
+import subprocess
+from lib_not_dr.nuitka import CompilerHelper
+
+compiler = CompilerHelper("main.py")
+
+print(compiler)
+subprocess.run(compiler.gen_subprocess_cmd())
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lib-not-dr-0.0.1/lib_not_dr/nuitka/compile.py` & `lib-not-dr-0.0.2/lib_not_dr/nuitka/compile.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 def _add_cmd(cmd: List[str], string: Optional[str]) -> List[str]:
     if string is not None and string:
         cmd.append(string)
     return cmd
 
 
 class CompilerHelper(Options):
+    """
+    用于帮助生成 nuitka 构建脚本的类
+    Use to help generate nuitka build script
+    
+    """
     name = 'Nuitka Compiler Helper'
 
     output_path: Path = Path('./build')
     src_file: Path
 
     python_cmd: str = 'python'
 
@@ -71,19 +76,40 @@
             self.use_mingw = self.use_mingw and not self.use_msvc
             # Windows 平台下使用 msvc 时不使用 mingw
 
     def __str__(self):
         return self.as_markdown()
 
     def as_markdown(self, longest: Optional[int] = None) -> str:
+        """
+        输出编译器帮助信息
+        Output compiler help information
+        
+        Args:
+            longest (Optional[int], optional): 
+                输出信息的最大长度限制 The maximum length of output information. 
+                Defaults to None.
+
+        Returns:
+            str: 以 markdown 格式输出的编译器帮助信息
+                Compile helper information in markdown format
+        """
         front = super().as_markdown(longest)
         gen_cmd = self.gen_subprocess_cmd()
         return f"{front}\n\n```bash\n{' '.join(gen_cmd)}\n```"
 
     def gen_subprocess_cmd(self) -> List[str]:
+        """生成 nuitka 构建脚本
+        Generate nuitka build script
+
+        Returns:
+            List[str]: 
+                生成的 nuitka 构建脚本
+                Generated nuitka build script
+        """
         cmd_list = [self.python_cmd, '-m', 'nuitka']
         # macos 和 非 macos icon 参数不同
         if platform.system() == 'Darwin':
             cmd_list.append(f"--macos-app-version={self.product_version}")
             _add_cmd(cmd_list, f'--macos-app-icon={self.icon_path.absolute()}' if self.icon_path else None)
         elif platform.system() == 'Windows':
             _add_cmd(cmd_list, f'--windows-icon-from-ico={self.icon_path.absolute()}' if self.icon_path else None)
@@ -119,13 +145,7 @@
         if self.include_data_dir:
             cmd_list += [f"--include-data-dir={src}={dst}" for src, dst in self.include_data_dir]
         if self.include_packages:
             cmd_list += [f"--include-package={package}" for package in self.include_packages]
 
         cmd_list.append(f"{self.src_file}")
         return cmd_list
-
-
-if __name__ == '__main__':
-    cp = CompilerHelper(src_file = Path('test.py'))
-    print(cp)
-
```

### Comparing `lib-not-dr-0.0.1/lib_not_dr/types/__init__.py` & `lib-not-dr-0.0.2/lib_not_dr/types/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.1/lib_not_dr/types/options.py` & `lib-not-dr-0.0.2/lib_not_dr/types/options.py`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.1/lib_not_dr/types/version.py` & `lib-not-dr-0.0.2/lib_not_dr/types/version.py`

 * *Files identical despite different names*

### Comparing `lib-not-dr-0.0.1/lib_not_dr.egg-info/PKG-INFO` & `lib-not-dr-0.0.2/lib_not_dr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-not-dr
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python lib created from Difficult Rocket development
 Author-email: shenjackyuanjie <3695888@qq.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -380,8 +380,43 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lib-not-dr
-A python lib came from Difficult Rocket development
+
+A python lib came from [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) development
+
+一个在 [Difficult Rocket](https://github.com/shenjackyuanjie/Difficult-Rocket) 开发中 分离出来的 python 库
+
+## Information/信息
+
+- Version/版本: 0.0.2
+
+### Author/作者
+
+[shenjackyuanjie](https://github/shenjackyuanjie)
+
+### License/许可证
+
+[MPL-2.0](https://www.mozilla.org/en-US/MPL/2.0/)
+
+## 安装/Install
+
+```bash
+pip install lib-not-dr
+```
+
+## 使用/Usage
+
+### Nuitka Compiler Helper
+
+```python
+import subprocess
+from lib_not_dr.nuitka import CompilerHelper
+
+compiler = CompilerHelper("main.py")
+
+print(compiler)
+subprocess.run(compiler.gen_subprocess_cmd())
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

