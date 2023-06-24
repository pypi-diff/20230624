# Comparing `tmp/researchgpt-0.0.1.tar.gz` & `tmp/researchgpt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "researchgpt-0.0.1.tar", last modified: Sat Jun 24 18:17:55 2023, max compression
+gzip compressed data, was "researchgpt-0.0.2.tar", last modified: Sat Jun 24 18:21:40 2023, max compression
```

## Comparing `researchgpt-0.0.1.tar` & `researchgpt-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:17:55.496616 researchgpt-0.0.1/
--rw-rw-rw-   0        0        0       95 2023-06-24 18:17:55.495614 researchgpt-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       57 2023-06-10 11:21:53.000000 researchgpt-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 18:17:55.487611 researchgpt-0.0.1/researchgpt/
--rw-rw-rw-   0        0        0       21 2023-06-24 05:44:37.000000 researchgpt-0.0.1/researchgpt/__init__.py
--rw-rw-rw-   0        0        0     1513 2023-06-24 03:55:58.000000 researchgpt-0.0.1/researchgpt/cli.py
--rw-rw-rw-   0        0        0      624 2023-06-24 10:39:43.000000 researchgpt-0.0.1/researchgpt/config.py
--rw-rw-rw-   0        0        0     3052 2023-06-24 17:55:23.000000 researchgpt-0.0.1/researchgpt/main.py
--rw-rw-rw-   0        0        0      676 2023-06-24 03:35:00.000000 researchgpt-0.0.1/researchgpt/modes.py
--rw-rw-rw-   0        0        0     2391 2023-06-24 17:55:46.000000 researchgpt-0.0.1/researchgpt/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:17:55.494614 researchgpt-0.0.1/researchgpt/writers/
--rw-rw-rw-   0        0        0      111 2023-06-21 06:45:07.000000 researchgpt-0.0.1/researchgpt/writers/__init__.py
--rw-rw-rw-   0        0        0      700 2023-06-24 03:05:57.000000 researchgpt-0.0.1/researchgpt/writers/base.py
--rw-rw-rw-   0        0        0     2341 2023-06-24 17:02:52.000000 researchgpt-0.0.1/researchgpt/writers/latex.py
--rw-rw-rw-   0        0        0     2049 2023-06-24 12:57:48.000000 researchgpt-0.0.1/researchgpt/writers/text.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:17:55.492609 researchgpt-0.0.1/researchgpt.egg-info/
--rw-rw-rw-   0        0        0       95 2023-06-24 18:17:55.000000 researchgpt-0.0.1/researchgpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      474 2023-06-24 18:17:55.000000 researchgpt-0.0.1/researchgpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:17:55.000000 researchgpt-0.0.1/researchgpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-24 18:17:55.000000 researchgpt-0.0.1/researchgpt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-06-24 18:17:55.000000 researchgpt-0.0.1/researchgpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-24 18:17:55.000000 researchgpt-0.0.1/researchgpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 18:17:55.496616 researchgpt-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      486 2023-06-24 18:01:28.000000 researchgpt-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:21:40.673682 researchgpt-0.0.2/
+-rw-rw-rw-   0        0        0      108 2023-06-24 18:21:40.672681 researchgpt-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2023-06-10 11:21:53.000000 researchgpt-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-24 18:21:40.663685 researchgpt-0.0.2/researchgpt/
+-rw-rw-rw-   0        0        0       48 2023-06-24 18:20:51.000000 researchgpt-0.0.2/researchgpt/__init__.py
+-rw-rw-rw-   0        0        0     1513 2023-06-24 03:55:58.000000 researchgpt-0.0.2/researchgpt/cli.py
+-rw-rw-rw-   0        0        0      624 2023-06-24 10:39:43.000000 researchgpt-0.0.2/researchgpt/config.py
+-rw-rw-rw-   0        0        0     3048 2023-06-24 18:20:54.000000 researchgpt-0.0.2/researchgpt/main.py
+-rw-rw-rw-   0        0        0      678 2023-06-24 18:20:54.000000 researchgpt-0.0.2/researchgpt/modes.py
+-rw-rw-rw-   0        0        0     2387 2023-06-24 18:20:54.000000 researchgpt-0.0.2/researchgpt/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:21:40.671682 researchgpt-0.0.2/researchgpt/writers/
+-rw-rw-rw-   0        0        0      111 2023-06-21 06:45:07.000000 researchgpt-0.0.2/researchgpt/writers/__init__.py
+-rw-rw-rw-   0        0        0      700 2023-06-24 03:05:57.000000 researchgpt-0.0.2/researchgpt/writers/base.py
+-rw-rw-rw-   0        0        0     2335 2023-06-24 18:20:54.000000 researchgpt-0.0.2/researchgpt/writers/latex.py
+-rw-rw-rw-   0        0        0     1979 2023-06-24 18:20:54.000000 researchgpt-0.0.2/researchgpt/writers/text.py
+drwxrwxrwx   0        0        0        0 2023-06-24 18:21:40.668684 researchgpt-0.0.2/researchgpt.egg-info/
+-rw-rw-rw-   0        0        0      108 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-24 18:21:40.000000 researchgpt-0.0.2/researchgpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-24 18:21:40.673682 researchgpt-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-06-24 18:21:01.000000 researchgpt-0.0.2/setup.py
```

### Comparing `researchgpt-0.0.1/researchgpt/cli.py` & `researchgpt-0.0.2/researchgpt/cli.py`

 * *Files identical despite different names*

### Comparing `researchgpt-0.0.1/researchgpt/config.py` & `researchgpt-0.0.2/researchgpt/config.py`

 * *Files identical despite different names*

### Comparing `researchgpt-0.0.1/researchgpt/main.py` & `researchgpt-0.0.2/researchgpt/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                     next_keywords = subtopics[:breadth]
 
                 keywords_map[i + 1].append(next_level[:])
                 new_keywords.extend(next_keywords[:])
             keywords_and_questions = new_keywords[:]
             depth -= 1
             i += 1
-    
+
     keywords_map.pop(i)
 
     heading_map = ""
 
     def print_section(depth, section, lst):
         nonlocal heading_map
         heading_map += f"{'    ' * depth}{lst[section]}\n"
```

### Comparing `researchgpt-0.0.1/researchgpt/modes.py` & `researchgpt-0.0.2/researchgpt/modes.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,12 +17,13 @@
     elif mode == "latex-long":
         return LatexWriter
     elif mode == "latex-short":
         return ShortLatexWriter
     else:
         raise ValueError("Invalid mode.")
 
+
 def get_template(mode):
     if mode.startswith("latex"):
         return LATEX_TEMPLATE
     else:
         return "{content}"
```

### Comparing `researchgpt-0.0.1/researchgpt/utils.py` & `researchgpt-0.0.2/researchgpt/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,26 +49,27 @@
     Args:
         context (str): The context to generate headings for.
 
     Returns:
         List[str]: The list of headings generated.
     """
 
+
 @loopgpt.aifunc()
 def generate_index(bad_index: str) -> str:
-    """This is a semantic function. Given is an index for a book, but it has many problems, for example, duplicate sections, 
-    bad section names, subsections that don't match their sections, missing numbering or sections without subsections. 
+    """This is a semantic function. Given is an index for a book, but it has many problems, for example, duplicate sections,
+    bad section names, subsections that don't match their sections, missing numbering or sections without subsections.
     This function fixes all of these problems and returns a properly numbered good index without duplicate sections or missing subsections.
 
     Examples:
         1. Section 1
             1.1. Subsection 1
             1.2. Subsection 2
         2. Section 2
             3.1. Subsection 1
-    
+
     Args:
         bad_index (str): The bad index to be fixed.
 
     Returns:
         str: The generated good index.
     """
```

### Comparing `researchgpt-0.0.1/researchgpt/writers/base.py` & `researchgpt-0.0.2/researchgpt/writers/base.py`

 * *Files identical despite different names*

### Comparing `researchgpt-0.0.1/researchgpt/writers/latex.py` & `researchgpt-0.0.2/researchgpt/writers/latex.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 """
 
 
 class LatexWriter(Writer):
     @staticmethod
     @loopgpt.aifunc()
     def write_section(section: str) -> str:
-        """Writes a latex \section{} command with the section name and then a short section about the given topic without going into specific details 
-        as there will be future subsections for that. The section should be less than 50 words long and should mention at least 3 subtopics 
+        """Writes a latex \section{} command with the section name and then a short section about the given topic without going into specific details
+        as there will be future subsections for that. The section should be less than 50 words long and should mention at least 3 subtopics
         that will be covered in future subsections.
 
         Args:
             section (str): The section to write the introduction for.
 
         Returns:
             str: The introduction written in LaTeX format.
         """
 
     @staticmethod
     @loopgpt.aifunc()
     def write_subsection(subsection: str) -> str:
-        """Writes a latex \subsection{} command with the subsection name and then a detailed subsection about the given topic that should contain as much 
-        details as possible including reference links. The subsection should be between 500 and 1000 words long and should cover the topic in depth. 
+        """Writes a latex \subsection{} command with the subsection name and then a detailed subsection about the given topic that should contain as much
+        details as possible including reference links. The subsection should be between 500 and 1000 words long and should cover the topic in depth.
         It must be in valid LaTeX with correct escaping.
 
         Args:
             subsection (str): The subsection to write about.
 
         Returns:
             str: The section written in LaTeX format.
@@ -51,16 +51,16 @@
 
 class ShortLatexWriter(LatexWriter):
     @staticmethod
     @loopgpt.aifunc()
     def write_subsection(subsection: str) -> str:
         """This is a semantic function. It writes a latex subsection command followed by the subsection name and then a very short subsection
         content including links to relevant websites.
-        Writes a latex \subsection{} command with the subsection name and then a short subsection about the given topic that should be between 100 and 200 
-        words long. It must be in valid LaTeX with correct escaping. Includes any relevant links that were found previously where the reader can 
+        Writes a latex \subsection{} command with the subsection name and then a short subsection about the given topic that should be between 100 and 200
+        words long. It must be in valid LaTeX with correct escaping. Includes any relevant links that were found previously where the reader can
         find more information.
 
         Args:
             subsection (str): The subsection to write about.
 
         Returns:
             str: The section written in LaTeX format.
```

### Comparing `researchgpt-0.0.1/researchgpt/writers/text.py` & `researchgpt-0.0.2/researchgpt/writers/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,55 +8,49 @@
 
 {content}
 """
 
 
 class TextWriter(Writer):
     @staticmethod
-    @format(
-        lambda heading, content: f"\n{heading}\n{'=' * len(heading)}\n\n{content}"
-    )
+    @format(lambda heading, content: f"\n{heading}\n{'=' * len(heading)}\n\n{content}")
     @loopgpt.aifunc()
     def write_section(section: str) -> str:
         """Writes a short section about the given topic without going into specific details as there will be future subsections for that.
         The section should be less than 50 words long and should mention at least 3 subtopics that will be covered in future subsections.
 
         Args:
             section (str): The topic of the section.
-        
+
         Returns:
             str: The section content.
         """
-    
+
     @staticmethod
-    @format(
-        lambda heading, content: f"\n{heading}\n{'-' * len(heading)}\n\n{content}"
-    )
+    @format(lambda heading, content: f"\n{heading}\n{'-' * len(heading)}\n\n{content}")
     @loopgpt.aifunc()
     def write_subsection(subsection: str) -> str:
         """Writes a detailed subsection about the given topic that should contain as much details as possible including reference links.
-        The subsection should be between 500 and 1000 words long and should cover the topic in depth. Please include at least 1 reference link 
+        The subsection should be between 500 and 1000 words long and should cover the topic in depth. Please include at least 1 reference link
         from a reputable source.
 
         Args:
             subsection (str): The topic of the subsection.
-        
+
         Returns:
             str: The subsection content.
         """
 
 
 class ShortTextWriter(TextWriter):
     @staticmethod
     @loopgpt.aifunc()
-    @format(
-        lambda heading, content: f"\n{heading}\n{'-' * len(heading)}\n\n{content}"
-    )
+    @format(lambda heading, content: f"\n{heading}\n{'-' * len(heading)}\n\n{content}")
     def write_subsection(subsection: str) -> str:
-        """Writes a short subsection about the given topic that should be between 100 and 200 words long. Inlcudes any relevant links that were found 
+        """Writes a short subsection about the given topic that should be between 100 and 200 words long. Inlcudes any relevant links that were found
         previously where the reader can find more information.
 
         Args:
             subsection (str): The topic of the subsection.
 
         Returns:
             str: The subsection content.
```

