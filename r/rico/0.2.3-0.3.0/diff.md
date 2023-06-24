# Comparing `tmp/rico-0.2.3.tar.gz` & `tmp/rico-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rico-0.2.3.tar", last modified: Thu Jun 15 16:18:20 2023, max compression
+gzip compressed data, was "rico-0.3.0.tar", last modified: Sat Jun 24 08:02:03 2023, max compression
```

## Comparing `rico-0.2.3.tar` & `rico-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-06-15 16:17:52.853613 rico-0.2.3/LICENSE
--rw-r--r--   0        0        0      706 2023-06-15 16:17:52.853613 rico-0.2.3/README.md
--rw-r--r--   0        0        0     2870 2023-06-15 16:18:20.949893 rico-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      491 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/__init__.py
--rw-r--r--   0        0        0     5471 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/_config.py
--rw-r--r--   0        0        0     5605 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/_container.py
--rw-r--r--   0        0        0    14794 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/_content.py
--rw-r--r--   0        0        0     7015 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/_html.py
--rw-r--r--   0        0        0      340 2023-06-15 16:17:52.853613 rico-0.2.3/src/rico/_version.py
--rw-r--r--   0        0        0       18 2023-06-15 16:17:52.853613 rico-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     1476 2023-06-15 16:17:52.853613 rico-0.2.3/tests/test__config.py
--rw-r--r--   0        0        0    10251 2023-06-15 16:17:52.853613 rico-0.2.3/tests/test__container.py
--rw-r--r--   0        0        0    17097 2023-06-15 16:17:52.853613 rico-0.2.3/tests/test__content.py
--rw-r--r--   0        0        0     9501 2023-06-15 16:17:52.853613 rico-0.2.3/tests/test__html.py
--rw-r--r--   0        0        0      730 2023-06-15 16:17:52.853613 rico-0.2.3/tests/test__version.py
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 rico-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-24 08:01:28.246842 rico-0.3.0/LICENSE
+-rw-r--r--   0        0        0    15333 2023-06-24 08:01:28.246842 rico-0.3.0/README.md
+-rw-r--r--   0        0        0     2955 2023-06-24 08:02:03.107859 rico-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      710 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/__init__.py
+-rw-r--r--   0        0        0     5469 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/_config.py
+-rw-r--r--   0        0        0     5629 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/_container.py
+-rw-r--r--   0        0        0    14852 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/_content.py
+-rw-r--r--   0        0        0     7031 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/_html.py
+-rw-r--r--   0        0        0      340 2023-06-24 08:01:28.246842 rico-0.3.0/src/rico/_version.py
+-rw-r--r--   0        0        0       18 2023-06-24 08:01:28.246842 rico-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1476 2023-06-24 08:01:28.246842 rico-0.3.0/tests/test__config.py
+-rw-r--r--   0        0        0    10248 2023-06-24 08:01:28.246842 rico-0.3.0/tests/test__container.py
+-rw-r--r--   0        0        0    17099 2023-06-24 08:01:28.246842 rico-0.3.0/tests/test__content.py
+-rw-r--r--   0        0        0     8907 2023-06-24 08:01:28.246842 rico-0.3.0/tests/test__html.py
+-rw-r--r--   0        0        0      730 2023-06-24 08:01:28.246842 rico-0.3.0/tests/test__version.py
+-rw-r--r--   0        0        0    16989 1970-01-01 00:00:00.000000 rico-0.3.0/PKG-INFO
```

### Comparing `rico-0.2.3/LICENSE` & `rico-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rico-0.2.3/pyproject.toml` & `rico-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [project]
 name = "rico"
 dynamic = []
-description = "Rich content to HTML as easy as Doc(df, plot)."
+description = "A Python package for creating HTML documents from rich content: dataframes, plots, images, markdown etc. It provides a high-level, easy-to-use API with reasonable defaults, as well as low-level access for better control."
 authors = [
     { name = "Evgeny Ivanov", email = "ivanov.evgeny.n@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: HTML",
     "Topic :: Text Processing :: Markup :: Markdown",
 ]
-version = "0.2.3"
+version = "0.3.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 source = "https://github.com/e10v/rico"
 "release notes" = "https://github.com/e10v/rico/releases"
@@ -93,15 +93,14 @@
 exclude_lines = [
     "if TYPE_CHECKING:",
     "pragma: no cover",
 ]
 
 [tool.pyright]
 typeCheckingMode = "strict"
-reportIncompatibleMethodOverride = false
 reportMissingTypeStubs = false
 
 [tool.ruff]
 select = [
     "A",
     "ANN",
     "ARG",
@@ -163,13 +162,10 @@
 lines-after-imports = 2
 known-local-folder = [
     "rico",
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
-ignore-decorators = [
-    "typing.overload",
-]
 
 [tool.ruff.pylint]
 max-args = 8
```

### Comparing `rico-0.2.3/src/rico/_config.py` & `rico-0.3.0/src/rico/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     Args:
         bootstrap_css: A link to a bootstrap css file.
             If empty then bootstrap css is not loaded.
         bootstrap_js: A link to a bootstrap javascript file.
             If empty then bootstrap javascript is not loaded.
         dataframe_style: A dataframe table stylesheet.
             If empty then it's not used.
-        image_format: Default chart image format.
+        image_format: Default plot image format.
         indent_html: Indent HTML elements in serialization methods.
         indent_space: Default indent space.
         inline_scripts: If True then scripts are loaded inline.
         inline_styles: If True then styles are loaded inline.
         meta_charset: An HTML document charset.
             If empty then it's not used.
         meta_viewport: An HTML document viewport property.
@@ -144,15 +144,15 @@
     Args:
         bootstrap_css: A link to a bootstrap css file.
             If empty then bootstrap css is not loaded.
         bootstrap_js: A link to a bootstrap javascript file.
             If empty then bootstrap javascript is not loaded.
         dataframe_style: A dataframe table stylesheet.
             If empty then it's not used.
-        image_format: Default chart image format.
+        image_format: Default plot image format.
         indent_html: Indent HTML elements in serialization methods.
         indent_space: Default indent space.
         inline_scripts: If True then scripts are loaded inline.
         inline_styles: If True then styles are loaded inline.
         meta_charset: An HTML document charset.
             If empty then it's not used.
         meta_viewport: An HTML document viewport property.
```

### Comparing `rico-0.2.3/src/rico/_container.py` & `rico-0.3.0/src/rico/_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 
     append_tag = _append(rico._content.Tag, rico._content.Tag.__init__)
     append_text = _append(rico._content.Text, rico._content.Text.__init__)
     append_code = _append(rico._content.Code, rico._content.Code.__init__)
     append_html = _append(rico._content.HTML, rico._content.HTML.__init__)
     append_markdown = _append(rico._content.Markdown, rico._content.Markdown.__init__)
     append_image = _append(rico._content.Image, rico._content.Image.__init__)
+    append_plot = _append(rico._content.Plot, rico._content.Plot.__init__)
     append_chart = _append(rico._content.Chart, rico._content.Chart.__init__)
     append = _append(rico._content.Obj, rico._content.Obj.__init__)
 
 
 class Doc(Div):
     """Creates an HTML document.
 
@@ -127,21 +128,18 @@
         if bootstrap.lower() in {"css", "full"}:
             styles.append(rico._content.Style(src=global_config["bootstrap_css"]))
         if bootstrap.lower() == "full":
             scripts.append(rico._content.Script(src=global_config["bootstrap_js"]))
         if global_config["dataframe_style"]:
             styles.append(rico._content.Style(text=global_config["dataframe_style"]))
 
-        styles = [*styles, *extra_styles]
-        scripts = [*scripts, *extra_scripts]
-
-        for style in styles:
+        for style in (*styles, *extra_styles):
             self.head.append(style.container)
 
-        for script in scripts:
+        for script in (*scripts, *extra_scripts):
             if script.footer:
                 self.body.append(script.container)
             else:
                 self.head.append(script.container)
 
     def serialize(
         self,
```

### Comparing `rico-0.2.3/src/rico/_content.py` & `rico-0.3.0/src/rico/_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,68 +248,65 @@
     """An Image content definition.
 
     Creates content elements using an image data and appends them to the container.
     """
     def __init__(
         self,
         data: bytes | str,
-        format: str,  # noqa: A002
+        mime_subtype: str,
         class_: str | None = None,
     ):
         """Create content using image data.
 
         Args:
             data: The image data.
-            format: The image format.
+            mime_subtype: The image MIME subtype. Examples: "png", "svg+xml".
             class_: The container class attribute.
         """
         super().__init__(class_)
 
         if isinstance(data, str):
             data = data.encode()
         encoded_image = base64.b64encode(data).decode()
 
-        if format == "svg":
-            format = "svg+xml"  # noqa: A001
-
         element = ET.Element(
             "img",
-            attrib={"src": f"data:image/{format};base64,{encoded_image}"},
+            attrib={"src": f"data:image/{mime_subtype};base64,{encoded_image}"},
         )
         self.container.append(element)
 
 
-class Chart(ContentBase):
-    """An Chart content definition.
+class Plot(ContentBase):
+    """A Plot content definition.
 
-    Creates content elements from a chart object and appends them to the container.
+    Creates content elements from a plot object and appends them to the container.
 
-    The supported chart types are the following:
+    The supported plot types are the following:
     - Altair Chart,
     - Pyplot Axes and Figure,
     - Seaborn Plot (seaborn.objects interface).
     """
     def __init__(
         self,
         obj: Any,
         format: Literal["svg", "png"] | None = None,  # noqa: A002
         class_: str | None = None,
         **kwargs: Any,
     ):
-        """Create content from a chart object.
+        """Create content from a plot object.
 
         Args:
-            obj: The chart object.
+            obj: The plot object.
             format: The image format.
             class_: The container class attribute.
             **kwargs: Keyword arguments passed to a function
                 which converts object to an image.
 
         Raises:
-            TypeError: Chart type is not supported
+            TypeError: Plot type is not supported
                 or required extra package is not installed.
         """
         if format is None:
             format = rico._config.get_config("image_format")  # noqa: A001
 
         if plt is not None and isinstance(obj, plt.Axes):
             obj = obj.figure
@@ -327,22 +324,25 @@
             image = convert(  # type: ignore
                 obj.to_json(),  # type: ignore
                 vl_version="_".join(alt.SCHEMA_VERSION.split(".")[:2]),
                 **kwargs,
             )
         else:
             error_msg = (
-                f"Chart type {type(obj)} is not supported "
+                f"Plot type {type(obj)} is not supported "
                 "or required extra package is not installed."
             )
             raise TypeError(error_msg)
 
-        content = Image(data=image, format=format, class_=class_)  # type: ignore
+        mime_subtype = "svg+xml" if format == "svg" else format
+        content = Image(data=image, mime_subtype=mime_subtype, class_=class_)  # type: ignore  # noqa: E501
         self.container = content.container
 
+Chart = Plot
+
 
 class Obj(ContentBase):
     """An arbitrary content definition.
 
     Creates content elements from arbitrary objects and appends them to the container.
 
     Automatically determines the content type.
@@ -359,15 +359,15 @@
             if isinstance(obj, ContentBase):
                 elements = (obj.container,)
             elif (
                 alt is not None and isinstance(obj, alt.TopLevelMixin) or
                 plt is not None and isinstance(obj, plt.Axes | plt.Figure) or  # type: ignore  # noqa: E501
                 so is not None and isinstance(obj, so.Plot)
             ):
-                elements = Chart(obj).container
+                elements = Plot(obj).container
             elif hasattr(obj, "_repr_html_") and callable(obj._repr_html_):
                 elements = HTML(
                     obj._repr_html_(),
                     strip_dataframe_borders=True,
                 ).container
             else:
                 elements = Text(obj).container
```

### Comparing `rico-0.2.3/src/rico/_html.py` & `rico-0.3.0/src/rico/_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def handle_endtag(self, tag: str) -> None:
         self._builder.end(tag)
 
     def handle_data(self, data: str) -> None:
         self._builder.data(data)
 
-    def close(self) -> tuple[ET.Element]:
+    def close(self) -> tuple[ET.Element]:  # type: ignore
         super().close()
         self._builder.end(self._root)
         return tuple(self._builder.close())
 
 
 def parse_html(data: str) -> tuple[ET.Element]:
     """Parse an HTML document from a string.
```

### Comparing `rico-0.2.3/tests/test__config.py` & `rico-0.3.0/tests/test__config.py`

 * *Files identical despite different names*

### Comparing `rico-0.2.3/tests/test__container.py` & `rico-0.3.0/tests/test__container.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,17 +114,17 @@
         {"x": "B", "y": 3},
         {"x": "C", "y": 6},
         {"x": "D", "y": 7},
         {"x": "E", "y": 2},
     ]),
 ).mark_bar().encode(x="x:N", y="y:Q")
 
-def test_div_append_chart(div_container: rico._container.Div):
-    div_container.append_chart(altair_chart)
-    content = rico._content.Chart(altair_chart)
+def test_div_append_plot(div_container: rico._container.Div):
+    div_container.append_plot(altair_chart)
+    content = rico._content.Plot(altair_chart)
     assert str(div_container) == f"<div>{content}</div>"
 
 
 def test_div_append(div_container: rico._container.Div):
     div_container.append("Hello world", altair_chart)
     content = rico._content.Obj("Hello world", altair_chart)
     assert str(div_container) == f"<div>{content}</div>"
```

### Comparing `rico-0.2.3/tests/test__content.py` & `rico-0.3.0/tests/test__content.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,15 +311,15 @@
     'width="16" height="16" fill="currentColor" class="bi bi-dash">'
     '<path d="M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z"/>'
     "</svg>"
 )
 
 @pytest.mark.parametrize("data", [svg_data, svg_data.encode()], ids=["str", "bytes"])
 def test_image_svg(data: str | bytes):
-    content = rico._content.Image(data, format="svg", class_="row")
+    content = rico._content.Image(data, mime_subtype="svg+xml", class_="row")
 
     if isinstance(data, str):
         data = data.encode()
     encoded_image = base64.b64encode(data).decode()
 
     div = content.container
     assert isinstance(div, ET.Element)
@@ -336,15 +336,15 @@
     assert img.text is None
     assert img.tail is None
     assert len(img) == 0
 
 
 @pytest.mark.parametrize("data", [svg_data, svg_data.encode()], ids=["str", "bytes"])
 def test_image_png(data: str | bytes):
-    content = rico._content.Image(data, format="png")
+    content = rico._content.Image(data, mime_subtype="png")
 
     if isinstance(data, str):
         data = data.encode()
     encoded_image = base64.b64encode(data).decode()
 
     div = content.container
     assert isinstance(div, ET.Element)
@@ -375,21 +375,21 @@
 
 pyplot_figure, pyplot_axes = plt.subplots()  # type: ignore
 pyplot_axes.plot([1, 2, 3, 4], [1, 4, 2, 3])  # type: ignore
 
 seaborn_plot = so.Plot({"x": [1, 2, 3, 4], "y": [1, 4, 2, 3]})  # type: ignore
 
 @pytest.mark.parametrize(
-    "chart",
+    "plot",
     [altair_chart, pyplot_axes, pyplot_figure, seaborn_plot],
     ids=["altair", "pyplot_axes", "pyplot_figure", "seaborn_plot"],
 )
 @pytest.mark.parametrize("format", [None, "png"], ids=["svg", "png"])
-def test_chart_complete(chart: Any, format: Literal["svg", "png"] | None):  # noqa: A002
-    content = rico._content.Chart(chart, format=format, class_="row")
+def test_plot_complete(plot: Any, format: Literal["svg", "png"] | None):  # noqa: A002
+    content = rico._content.Plot(plot, format=format, class_="row")
 
     div = content.container
     assert isinstance(div, ET.Element)
     assert div.tag == "div"
     assert div.attrib == {"class": "row"}
     assert div.text is None
     assert div.tail is None
@@ -397,28 +397,28 @@
 
     img = tuple(div)[0]
     assert isinstance(img, ET.Element)
     assert img.tag == "img"
 
 
 @pytest.mark.parametrize(
-    ("module", "err_chart", "chart"),
+    ("module", "err_plot", "plot"),
     [
         ("alt", altair_chart, seaborn_plot),
         ("plt", pyplot_axes, altair_chart),
         ("so", seaborn_plot, pyplot_axes),
     ],
     ids=["alt", "plt", "so"],
 )
-def test_chart_error(module: str, err_chart: Any, chart: Any):
+def test_plot_error(module: str, err_plot: Any, plot: Any):
     with unittest.mock.patch.object(rico._content, module, None):
         with pytest.raises(TypeError):
-            rico._content.Chart(err_chart)
+            rico._content.Plot(err_plot)
 
-        content = rico._content.Chart(chart, class_="row")
+        content = rico._content.Plot(plot, class_="row")
         div = content.container
         assert isinstance(div, ET.Element)
 
 
 def test_obj():
     class ReprHTML:
         def _repr_html_(self) -> str:
```

### Comparing `rico-0.2.3/tests/test__html.py` & `rico-0.3.0/tests/test__html.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,17 @@
 
 def elem_to_string(elem: ET.Element | tuple[ET.Element], sep: str = "") -> str:
     if isinstance(elem, tuple):
         return sep.join(elem_to_string(e) for e in elem)
     return ET.tostring(elem, encoding="unicode", method="html")
 
 
-def test_html_parser_two_elements():
+def test_parse_html_two_elements():
     text = "<p>Hello</p><p>world</p>"
-    parser = rico._html.HTMLParser()
-    parser.feed(text)
-    elements = parser.close()
+    elements = rico._html.parse_html(text)
 
     assert elem_to_string(elements) == text
     assert isinstance(elements, tuple)
     assert len(elements) == 2
 
     p0 = elements[0]
     assert isinstance(p0, ET.Element)
@@ -37,19 +35,17 @@
     assert p1.tag == "p"
     assert p1.attrib == {}
     assert p1.text == "world"
     assert p1.tail is None
     assert len(p1) == 0
 
 
-def test_html_parser_nested_tags():
+def test_parse_html_nested_tags():
     text = "<div><p>Hello <strong>world</strong>!</p></div>"
-    parser = rico._html.HTMLParser()
-    parser.feed(text)
-    elements = parser.close()
+    elements = rico._html.parse_html(text)
 
     assert elem_to_string(elements) == text
     assert isinstance(elements, tuple)
     assert len(elements) == 1
 
     div = elements[0]
     assert isinstance(div, ET.Element)
@@ -72,20 +68,18 @@
     assert strong.tag == "strong"
     assert strong.attrib == {}
     assert strong.text == "world"
     assert strong.tail == "!"
     assert len(strong) == 0
 
 
-def test_html_parser_attributes():
+def test_parse_html_attributes():
     script_src = "https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"
     text = f"<script defer src='{script_src}' crossorigin='anonymous'></script>"
-    parser = rico._html.HTMLParser()
-    parser.feed(text)
-    elements = parser.close()
+    elements = rico._html.parse_html(text)
 
     assert isinstance(elements, tuple)
     assert len(elements) == 1
 
     script = elements[0]
     assert isinstance(script, ET.Element)
     assert script.tag == "script"
@@ -95,25 +89,23 @@
         "crossorigin": "anonymous",
     }
     assert script.text is None
     assert script.tail is None
     assert len(script) == 0
 
 
-def test_html_parser_svg():
+def test_parse_html_svg():
     text = (
         '<svg xmlns="http://www.w3.org/2000/svg" '
         'xmlns:xlink="http://www.w3.org/1999/xlink" '
         'width="16" height="16" fill="currentColor" class="bi bi-dash">'
         '<path d="M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z"/>'
         "</svg>"
     )
-    parser = rico._html.HTMLParser()
-    parser.feed(text)
-    elements = parser.close()
+    elements = rico._html.parse_html(text)
 
     assert isinstance(elements, tuple)
     assert len(elements) == 1
 
     svg = elements[0]
     assert isinstance(svg, ET.Element)
     assert svg.tag == "svg"
@@ -136,31 +128,14 @@
         "d": "M4 8a.5.5 0 0 1 .5-.5h7a.5.5 0 0 1 0 1h-7A.5.5 0 0 1 4 8z",
     }
     assert path.text is None
     assert path.tail is None
     assert len(path) == 0
 
 
-def test_parse_html():
-    text = "<p>Hello world</p>"
-    elements = rico._html.parse_html(text)
-
-    assert elem_to_string(elements) == text
-    assert isinstance(elements, tuple)
-    assert len(elements) == 1
-
-    p = elements[0]
-    assert isinstance(p, ET.Element)
-    assert p.tag == "p"
-    assert p.attrib == {}
-    assert p.text == "Hello world"
-    assert p.tail is None
-    assert len(p) == 0
-
-
 @pytest.fixture
 def sample_elem():
     div0 = ET.Element("div", {"class": "container"})
     div0.text = "\n"
     p0 = ET.SubElement(div0, "p")
     p0.text = " Hello "
     p0.tail = "\n"
```

### Comparing `rico-0.2.3/tests/test__version.py` & `rico-0.3.0/tests/test__version.py`

 * *Files identical despite different names*

