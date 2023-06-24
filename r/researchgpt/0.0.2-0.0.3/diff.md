# Comparing `tmp/researchgpt-0.0.2.tar.gz` & `tmp/researchgpt-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "researchgpt-0.0.2.tar", last modified: Sat Jun 24 18:21:40 2023, max compression
+gzip compressed data, was "researchgpt-0.0.3.tar", last modified: Sat Jun 24 18:44:03 2023, max compression
```

## Comparing `researchgpt-0.0.2.tar` & `researchgpt-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:21:40.673682 researchgpt-0.0.2/
--rw-rw-rw-   0        0        0      108 2023-06-24 18:21:40.672681 researchgpt-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-06-10 11:21:53.000000 researchgpt-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 18:21:40.663685 researchgpt-0.0.2/researchgpt/
--rw-rw-rw-   0        0        0       48 2023-06-24 18:20:51.000000 researchgpt-0.0.2/researchgpt/__init__.py
--rw-rw-rw-   0        0        0     1513 2023-06-24 03:55:58.000000 researchgpt-0.0.2/researchgpt/cli.py
--rw-rw-rw-   0        0        0      624 2023-06-24 10:39:43.000000 researchgpt-0.0.2/researchgpt/config.py
--rw-rw-rw-   0        0        0     3048 2023-06-24 18:20:54.000000 researchgpt-0.0.2/researchgpt/main.py
--rw-rw-rw-   0        0        0      678 2023-06-24 18:20:54.000000 researchgpt-0.0.2/researchgpt/modes.py
--rw-rw-rw-   0        0        0     2387 2023-06-24 18:20:54.000000 researchgpt-0.0.2/researchgpt/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:21:40.671682 researchgpt-0.0.2/researchgpt/writers/
--rw-rw-rw-   0        0        0      111 2023-06-21 06:45:07.000000 researchgpt-0.0.2/researchgpt/writers/__init__.py
--rw-rw-rw-   0        0        0      700 2023-06-24 03:05:57.000000 researchgpt-0.0.2/researchgpt/writers/base.py
--rw-rw-rw-   0        0        0     2335 2023-06-24 18:20:54.000000 researchgpt-0.0.2/researchgpt/writers/latex.py
--rw-rw-rw-   0        0        0     1979 2023-06-24 18:20:54.000000 researchgpt-0.0.2/researchgpt/writers/text.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:21:40.668684 researchgpt-0.0.2/researchgpt.egg-info/
--rw-rw-rw-   0        0        0      108 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 18:21:40.673682 researchgpt-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-06-24 18:21:01.000000 researchgpt-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:44:03.486146 researchgpt-0.0.3/
+-rw-rw-rw-   0        0        0      108 2023-06-24 18:44:03.485146 researchgpt-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-06-24 18:41:17.000000 researchgpt-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 18:44:03.478146 researchgpt-0.0.3/researchgpt/
+-rw-rw-rw-   0        0        0       48 2023-06-24 18:30:30.000000 researchgpt-0.0.3/researchgpt/__init__.py
+-rw-rw-rw-   0        0        0     1699 2023-06-24 18:43:19.000000 researchgpt-0.0.3/researchgpt/cli.py
+-rw-rw-rw-   0        0        0      624 2023-06-24 10:39:43.000000 researchgpt-0.0.3/researchgpt/config.py
+-rw-rw-rw-   0        0        0     3050 2023-06-24 18:37:46.000000 researchgpt-0.0.3/researchgpt/main.py
+-rw-rw-rw-   0        0        0      680 2023-06-24 18:36:40.000000 researchgpt-0.0.3/researchgpt/modes.py
+-rw-rw-rw-   0        0        0     2387 2023-06-24 18:20:54.000000 researchgpt-0.0.3/researchgpt/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:44:03.485146 researchgpt-0.0.3/researchgpt/writers/
+-rw-rw-rw-   0        0        0       97 2023-06-24 18:37:07.000000 researchgpt-0.0.3/researchgpt/writers/__init__.py
+-rw-rw-rw-   0        0        0      700 2023-06-24 03:05:57.000000 researchgpt-0.0.3/researchgpt/writers/base.py
+-rw-rw-rw-   0        0        0     2335 2023-06-24 18:20:54.000000 researchgpt-0.0.3/researchgpt/writers/latex.py
+-rw-rw-rw-   0        0        0     1979 2023-06-24 18:20:54.000000 researchgpt-0.0.3/researchgpt/writers/text.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:44:03.482147 researchgpt-0.0.3/researchgpt.egg-info/
+-rw-rw-rw-   0        0        0      108 2023-06-24 18:44:03.000000 researchgpt-0.0.3/researchgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-06-24 18:44:03.000000 researchgpt-0.0.3/researchgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:44:03.000000 researchgpt-0.0.3/researchgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-24 18:44:03.000000 researchgpt-0.0.3/researchgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2023-06-24 18:44:03.000000 researchgpt-0.0.3/researchgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 18:44:03.486146 researchgpt-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      489 2023-06-24 18:35:26.000000 researchgpt-0.0.3/setup.py
```

### Comparing `researchgpt-0.0.2/researchgpt/cli.py` & `researchgpt-0.0.3/researchgpt/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 import argparse
 import json
 
 from loopgpt.aifunc import create_empty_agent
-from main import research, write_book
-from modes import get_research_args
-from config import model, emb
-
-
-research_agent = create_empty_agent(model=model, embedding_provider=emb)
-writer_agent = create_empty_agent(model=model, embedding_provider=emb)
-
-parser = argparse.ArgumentParser()
-
-parser.add_argument("topic", help="Topic to research")
-parser.add_argument(
-    "filename",
-    help="Filename to write the research.",
-)
-parser.add_argument(
-    "--mode",
-    choices=["short", "long"],
-    help="Mode of research.",
-    default="short",
-)
-parser.add_argument(
-    "--latex",
-    help="Latex mode",
-    action="store_true",
-)
-parser.add_argument(
-    "--breadth",
-    help="Breadth of research.",
-)
-parser.add_argument(
-    "--depth",
-    help="Depth of research.",
-)
-
-args = parser.parse_args()
-
-topic = args.topic
-filename = args.filename
-mode = args.mode
-
-if args.latex:
-    mode = "latex-" + mode
-
-
-research_agent = create_empty_agent(model=model, embedding_provider=emb)
-writer_agent = create_empty_agent(model=model, embedding_provider=emb)
-
-writer_agent.memory = research_agent.memory
-
-research_args = get_research_args(mode)
-if args.breadth:
-    research_args["breadth"] = int(args.breadth)
-if args.depth:
-    research_args["depth"] = int(args.depth)
+from .main import research, write_book
+from .modes import get_research_args
+from .config import model, emb
+
+
+def main():
+    research_agent = create_empty_agent(model=model, embedding_provider=emb)
+    writer_agent = create_empty_agent(model=model, embedding_provider=emb)
+
+    parser = argparse.ArgumentParser()
+
+    parser.add_argument("topic", help="Topic to research")
+    parser.add_argument(
+        "filename",
+        help="Filename to write the research.",
+    )
+    parser.add_argument(
+        "--mode",
+        choices=["short", "long"],
+        help="Mode of research.",
+        default="short",
+    )
+    parser.add_argument(
+        "--latex",
+        help="Latex mode",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--breadth",
+        help="Breadth of research.",
+    )
+    parser.add_argument(
+        "--depth",
+        help="Depth of research.",
+    )
+
+    args = parser.parse_args()
+
+    topic = args.topic
+    filename = args.filename
+    mode = args.mode
+
+    if args.latex:
+        mode = "latex-" + mode
+
+    research_agent = create_empty_agent(model=model, embedding_provider=emb)
+    writer_agent = create_empty_agent(model=model, embedding_provider=emb)
+
+    writer_agent.memory = research_agent.memory
+
+    research_args = get_research_args(mode)
+    if args.breadth:
+        research_args["breadth"] = int(args.breadth)
+    if args.depth:
+        research_args["depth"] = int(args.depth)
 
-index = research(topic, research_agent, **research_args)
-write_book(topic, index, writer_agent, filename, mode)
+    index = research(topic, research_agent, **research_args)
+    write_book(topic, index, writer_agent, filename, mode)
```

### Comparing `researchgpt-0.0.2/researchgpt/config.py` & `researchgpt-0.0.3/researchgpt/config.py`

 * *Files identical despite different names*

### Comparing `researchgpt-0.0.2/researchgpt/main.py` & `researchgpt-0.0.3/researchgpt/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections import defaultdict, OrderedDict
 
-from utils import (
+from .utils import (
     get_keywords_and_questions,
     generate_index,
 )
 from loopgpt.tools import GoogleSearch, Browser
-from modes import get_writer, get_template
+from .modes import get_writer, get_template
 from datetime import date
 
 
 def research(topic, research_agent, breadth=3, depth=1):
     keywords_and_questions = get_keywords_and_questions(topic)[:breadth]
 
     google_search = GoogleSearch()
```

### Comparing `researchgpt-0.0.2/researchgpt/modes.py` & `researchgpt-0.0.3/researchgpt/modes.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from writers import *
-from writers.latex import LATEX_TEMPLATE
+from .writers import *
+from .writers.latex import LATEX_TEMPLATE
 
 
 def get_research_args(mode):
     if mode.endswith("short"):
         return {"breadth": 4, "depth": 1}
     else:
         return {"breadth": 4, "depth": 2}
```

### Comparing `researchgpt-0.0.2/researchgpt/utils.py` & `researchgpt-0.0.3/researchgpt/utils.py`

 * *Files identical despite different names*

### Comparing `researchgpt-0.0.2/researchgpt/writers/base.py` & `researchgpt-0.0.3/researchgpt/writers/base.py`

 * *Files identical despite different names*

### Comparing `researchgpt-0.0.2/researchgpt/writers/latex.py` & `researchgpt-0.0.3/researchgpt/writers/latex.py`

 * *Files identical despite different names*

### Comparing `researchgpt-0.0.2/researchgpt/writers/text.py` & `researchgpt-0.0.3/researchgpt/writers/text.py`

 * *Files identical despite different names*

