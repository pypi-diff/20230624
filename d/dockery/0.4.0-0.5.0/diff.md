# Comparing `tmp/dockery-0.4.0.tar.gz` & `tmp/dockery-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockery-0.4.0.tar", last modified: Tue Jun 20 06:40:59 2023, max compression
+gzip compressed data, was "dockery-0.5.0.tar", last modified: Sat Jun 24 19:04:57 2023, max compression
```

## Comparing `dockery-0.4.0.tar` & `dockery-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1082 2023-06-20 06:40:48.096194 dockery-0.4.0/LICENSE
--rw-r--r--   0        0        0      862 2023-06-20 06:40:48.096194 dockery-0.4.0/README.md
--rw-r--r--   0        0        0      761 2023-06-20 06:40:59.876404 dockery-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 06:40:48.096194 dockery-0.4.0/src/dockery/__init__.py
--rw-r--r--   0        0        0      759 2023-06-20 06:40:48.096194 dockery-0.4.0/src/dockery/buttons.py
--rw-r--r--   0        0        0     2489 2023-06-20 06:40:48.096194 dockery-0.4.0/src/dockery/dockery.py
--rw-r--r--   0        0        0     6628 2023-06-20 06:40:48.096194 dockery-0.4.0/src/dockery/gui.py
--rw-r--r--   0        0        0     1863 2023-06-20 06:40:48.096194 dockery-0.4.0/src/dockery/logs.py
--rw-r--r--   0        0        0     1026 2023-06-20 06:40:48.096194 dockery-0.4.0/src/dockery/style.css
--rw-r--r--   0        0        0      881 2023-06-20 06:40:48.096194 dockery-0.4.0/src/dockery/utils.py
--rw-r--r--   0        0        0     1342 1970-01-01 00:00:00.000000 dockery-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-24 19:04:49.346517 dockery-0.5.0/LICENSE
+-rw-r--r--   0        0        0      865 2023-06-24 19:04:49.346517 dockery-0.5.0/README.md
+-rw-r--r--   0        0        0      761 2023-06-24 19:04:57.986569 dockery-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/__init__.py
+-rw-r--r--   0        0        0     1760 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/custom_widgets.py
+-rw-r--r--   0        0        0     2767 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/dockery.py
+-rw-r--r--   0        0        0     6167 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/gui.py
+-rw-r--r--   0        0        0     1616 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/images.py
+-rw-r--r--   0        0        0     1899 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/logs.py
+-rw-r--r--   0        0        0     1763 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/networks.py
+-rw-r--r--   0        0        0     1070 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/style.css
+-rw-r--r--   0        0        0      881 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/utils.py
+-rw-r--r--   0        0        0     1744 2023-06-24 19:04:49.346517 dockery-0.5.0/src/dockery/volumes.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 dockery-0.5.0/PKG-INFO
```

### Comparing `dockery-0.4.0/LICENSE` & `dockery-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dockery-0.4.0/README.md` & `dockery-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # update only:
 git pull
 ```
 
 ### From pip
 
 ```shell
-pip install dockery
+pip install -U dockery
 ```
 
 ## Usage
 
 Run on your console:
 
 ```shell
```

#### html2text {}

```diff
@@ -2,10 +2,10 @@
 [https://github.com/marianocarrazana/  [https://github.com/marianocarrazana/
 dockery/assets/17238076/3c987e47-2d86- dockery/assets/17238076/26dc43c9-1dd0-
 44ae-a078-73eced62dc11]                4097-ac02-aa006c3ff6b6]
 [https://github.com/marianocarrazana/dockery/assets/17238076/c991ff4b-eebf-
 4495-b67c-2c57e933bd7d]
 ## Installation ### From source ```shell git clone git@github.com:
 marianocarrazana/dockery.git cd dockery pip install -e . # update only: git
-pull ``` ### From pip ```shell pip install dockery ``` ## Usage Run on your
+pull ``` ### From pip ```shell pip install -U dockery ``` ## Usage Run on your
 console: ```shell dockery ``` ## Extra commands ```shell dockery df dockery ps
 dockery volumes dockery images dockery stats ``` ## **Enjoy it!**
```

### Comparing `dockery-0.4.0/pyproject.toml` & `dockery-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dockery"
-version = "0.4.0"
+version = "0.5.0"
 description = "Graphical interface for Docker in your console"
 authors = [
     { name = "Mariano Carrazana", email = "marianocarrazana@gmail.com" },
 ]
 dependencies = [
     "docker>=6.1.3",
     "textual>=0.28.0",
```

### Comparing `dockery-0.4.0/src/dockery/dockery.py` & `dockery-0.5.0/src/dockery/dockery.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import docker
 from docker.models.containers import Container
 from docker.models.volumes import Volume
 from docker.models.images import Image
+from docker.models.networks import Network
 import click
 from rich import print
 
 from .gui import AppGUI
 
 default_options = [
     click.option(
@@ -94,16 +95,24 @@
 @add_options(default_options)
 def images(**kargs):
     client = get_client(**kargs)
     imgs: list[Image] = client.images.list()  # type: ignore
     for i in imgs:
         print(i.attrs)
 
+@click.command
+@add_options(default_options)
+def networks(**kargs):
+    client = get_client(**kargs)
+    netw: list[Network] = client.networks.list()  # type: ignore
+    for i in netw:
+        print(i.attrs)
 
 main.add_command(df)
 main.add_command(volumes)
 main.add_command(ps)
 main.add_command(stats)
 main.add_command(images)
+main.add_command(networks)
 
 if __name__ == "__main__":
     main()
```

### Comparing `dockery-0.4.0/src/dockery/gui.py` & `dockery-0.5.0/src/dockery/gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import threading
-import math
-from rich.text import TextType
 from textual.app import App, ComposeResult
 from textual.widgets import Footer, Static, ContentSwitcher, Tabs, Tab, Label
 from textual.widgets._header import HeaderClock
 from textual.containers import (
     VerticalScroll,
     Horizontal,
     Vertical,
     Container as Group,
-    Grid,
 )
 from textual.reactive import reactive
-from textual.events import Resize
 from docker import DockerClient, errors
 from docker.models.containers import Container
 
 from .utils import get_cpu_usage, get_mem_usage
 from .logs import LogsButton
-from .buttons import CustomButton
+from .custom_widgets import CustomButton, ResponsiveGrid, ReactiveString
+from .images import ImagesList
+from .networks import NetworkList
+from .volumes import VolumesList
 
 
 class AppGUI(App):
     CSS_PATH = "style.css"
     BINDINGS = [
         ("d", "toggle_dark", "Toggle dark mode"),
         ("q", "quit", "Quit"),
@@ -34,47 +33,43 @@
         super().__init__(**kargs)
 
     def compose(self) -> ComposeResult:
         with Horizontal(id="header"):
             yield HeaderClock()
             yield Tabs(
                 Tab("Containers", id="container-list"),
+                Tab("Images", id="image-list"),
+                Tab("Networks", id="network-list"),
+                Tab("Volumes", id="volume-list"),
                 Tab("Logs", id="container-logs"),
                 id="nav",
             )
         yield Footer()
         with ContentSwitcher():
             yield ContainersList(self.docker, id="container-list")
-            with VerticalScroll(id="container-logs"):
-                yield Static("", id="logs")
+            yield VerticalScroll(id="container-logs")
+            yield ImagesList(self.docker, id="image-list")
+            yield NetworkList(self.docker, id="network-list")
+            yield VolumesList(self.docker, id="volume-list")
 
     def on_tabs_tab_activated(self, event: Tabs.TabActivated) -> None:
         self.query_one(ContentSwitcher).current = event.tab.id
 
 
-class ContainersList(VerticalScroll):
+class ContainersList(ResponsiveGrid):
     container_count = reactive(0)
 
     def __init__(self, docker: DockerClient, **kargs):
         self.containers = []
         self.docker = docker
-        self.grid = Grid()
         super().__init__(**kargs)
 
-    def compose(self) -> ComposeResult:
-        yield self.grid
-
     def on_mount(self) -> None:
         self.get_containers()
         self.set_interval(2, self.count_timer)
-        self.resize()
-        self.grid.styles.grid_columns = "1fr"
-        self.grid.styles.grid_rows = "4"
-        self.grid.styles.width = "100%"
-        self.grid.styles.height = "auto"
 
     def count_timer(self) -> None:
         thread = threading.Thread(target=self.get_containers)
         thread.start()
 
     async def watch_container_count(self, count: int) -> None:
         await self.grid.remove_children()
@@ -82,22 +77,14 @@
             cw = ContainerWidget(c, self.docker)  # type: ignore
             self.grid.mount(cw)
 
     def get_containers(self) -> None:
         self.containers = self.docker.containers.list(all=True)
         self.container_count = len(self.containers)
 
-    def on_resize(self, e: Resize):
-        self.resize()
-
-    def resize(self):
-        min_container_width = 75
-        columns = math.floor(self.size.width / min_container_width)
-        self.grid.styles.grid_size_columns = columns
-
 
 class ContainerWidget(Static):
     def __init__(self, container: Container, client: DockerClient, **kargs):
         self.container = container
         self.client = client
         self.container_id = container.id
         super().__init__(**kargs)
@@ -123,20 +110,19 @@
 
     def data_timer(self) -> None:
         thread = threading.Thread(target=self.update_data, daemon=True)
         thread.start()
 
     def update_data(self) -> None:
         try:
-            c: Container = self.client.containers.get(self.container_id)  # type: ignore
+            self.container.reload()
         except errors.NotFound:
             return None
         else:
-            self.container = c
-            status = c.status.capitalize()
+            status = self.container.status.capitalize()
             self.query_one("#status", ReactiveString).text = (
                 "[green]" if status == "Running" else "[bright_black]"
             ) + status
 
     def update_usage(self) -> None:
         c = self.container
         cpu = self.query_one("#cpu", ReactiveString)
@@ -147,24 +133,14 @@
             cpu.text = f"CPU: {get_cpu_usage(stat):.1f}"
             mem.text = f"MEM: {get_mem_usage(stat):.1f}"
 
     def on_unmount(self):
         self.running = False
 
 
-class ReactiveString(Static):
-    text = reactive("")
-
-    def __init__(self, **kargs):
-        super().__init__(shrink=True, expand=True, **kargs)
-
-    def render(self) -> TextType:
-        return self.text
-
-
 class StatusButtons(Static):
     def __init__(self, container: Container, **kargs):
         self.container = container
         super().__init__(**kargs)
 
     def compose(self) -> ComposeResult:
         yield Horizontal(
```

### Comparing `dockery-0.4.0/src/dockery/logs.py` & `dockery-0.5.0/src/dockery/logs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import threading
 import time
 from textual.app import ComposeResult
 from textual.widgets import Static, TextLog, Tabs
 from textual.reactive import reactive
+from textual.containers import VerticalScroll
 from docker.models.containers import Container
 
-from .buttons import CustomButton
+from .custom_widgets import CustomButton
 
 
 class LogsButton(Static):
     def __init__(self, container: Container, **kargs):
         self.container = container
         super().__init__(**kargs)
 
     async def on_click(self) -> None:
-        cl = self.app.query_one("#logs")
+        cl = self.app.query_one("VerticalScroll#container-logs", VerticalScroll)
         await cl.remove_children()
         lc = LogsContainer(self.container)
         await cl.mount(lc)
         self.app.query_one("#nav", Tabs).active = "container-logs"
 
     def compose(self) -> ComposeResult:
         yield CustomButton(":notebook:Logs", color="blue")
 
 
 class LogsContainer(TextLog):
     last_log = reactive("")
 
     def __init__(self, container: Container, **kargs):
         self.container = container
-        self.log_container = self.app.query_one("#logs")
         super().__init__(highlight=True, auto_scroll=True, wrap=True, **kargs)
 
     def on_mount(self) -> None:
         self.running = True
         self.thread = threading.Thread(target=self.update_log, daemon=True)
         self.thread.start()
```

### Comparing `dockery-0.4.0/src/dockery/style.css` & `dockery-0.5.0/src/dockery/style.css`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-ContainerWidget {
+ContainerWidget,
+ImageWidget,
+NetworkWidget,
+VolumeWidget {
     layout: horizontal;
     background: $boost;
     height: 3;
     margin: 1;
     min-width: 50;
     padding: 0 2;
 }
@@ -72,12 +75,12 @@
 }
 
 HeaderClock {
     height: 3;
     background: transparent;
 }
 
-.container-name{
+.container-name {
     overflow-x: hidden;
     max-width: 100%;
     height: 1;
-}
+}
```

### Comparing `dockery-0.4.0/src/dockery/utils.py` & `dockery-0.5.0/src/dockery/utils.py`

 * *Files identical despite different names*

### Comparing `dockery-0.4.0/PKG-INFO` & `dockery-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockery
-Version: 0.4.0
+Version: 0.5.0
 Summary: Graphical interface for Docker in your console
 Author-Email: Mariano Carrazana <marianocarrazana@gmail.com>
 License: MIT
 Project-URL: Bug tracker, https://github.com/marianocarrazana/dockery/issues
 Project-URL: Source code, https://github.com/marianocarrazana/dockery
 Requires-Python: >=3.9
 Requires-Dist: docker>=6.1.3
@@ -37,15 +37,15 @@
 # update only:
 git pull
 ```
 
 ### From pip
 
 ```shell
-pip install dockery
+pip install -U dockery
 ```
 
 ## Usage
 
 Run on your console:
 
 ```shell
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: dockery Version: 0.4.0 Summary: Graphical interface
+Metadata-Version: 2.1 Name: dockery Version: 0.5.0 Summary: Graphical interface
 for Docker in your console Author-Email: Mariano Carrazana
 gmail.com> License: MIT Project-URL: Bug tracker, https://github.com/
 marianocarrazana/dockery/issues Project-URL: Source code, https://github.com/
 marianocarrazana/dockery Requires-Python: >=3.9 Requires-Dist: docker>=6.1.3
 Requires-Dist: textual>=0.28.0 Requires-Dist: click>=8.1.3 Description-Content-
 Type: text/markdown # dockery Graphical interface for Docker in your console
 [https://github.com/marianocarrazana/  [https://github.com/marianocarrazana/
 dockery/assets/17238076/3c987e47-2d86- dockery/assets/17238076/26dc43c9-1dd0-
 44ae-a078-73eced62dc11]                4097-ac02-aa006c3ff6b6]
 [https://github.com/marianocarrazana/dockery/assets/17238076/c991ff4b-eebf-
 4495-b67c-2c57e933bd7d]
 ## Installation ### From source ```shell git clone git@github.com:
 marianocarrazana/dockery.git cd dockery pip install -e . # update only: git
-pull ``` ### From pip ```shell pip install dockery ``` ## Usage Run on your
+pull ``` ### From pip ```shell pip install -U dockery ``` ## Usage Run on your
 console: ```shell dockery ``` ## Extra commands ```shell dockery df dockery ps
 dockery volumes dockery images dockery stats ``` ## **Enjoy it!**
```

