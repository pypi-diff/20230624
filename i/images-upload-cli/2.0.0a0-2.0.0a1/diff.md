# Comparing `tmp/images_upload_cli-2.0.0a0.tar.gz` & `tmp/images_upload_cli-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "images_upload_cli-2.0.0a0.tar", max compression
+gzip compressed data, was "images_upload_cli-2.0.0a1.tar", max compression
```

## Comparing `images_upload_cli-2.0.0a0.tar` & `images_upload_cli-2.0.0a1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/LICENSE
--rw-r--r--   0        0        0     5236 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/README.md
--rw-r--r--   0        0        0     2557 2023-06-21 20:13:37.943695 images_upload_cli-2.0.0a0/pyproject.toml
--rwxr-xr-x   0        0        0      175 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/src/images_upload_cli/__init__.py
--rwxr-xr-x   0        0        0      178 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/src/images_upload_cli/__main__.py
--rwxr-xr-x   0        0        0     2453 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/src/images_upload_cli/cli.py
--rwxr-xr-x   0        0        0    10781 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/src/images_upload_cli/upload.py
--rwxr-xr-x   0        0        0     3090 2023-06-21 20:13:21.051465 images_upload_cli-2.0.0a0/src/images_upload_cli/util.py
--rw-r--r--   0        0        0     6197 1970-01-01 00:00:00.000000 images_upload_cli-2.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0     5236 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/README.md
+-rw-r--r--   0        0        0     2557 2023-06-22 20:02:25.238057 images_upload_cli-2.0.0a1/pyproject.toml
+-rwxr-xr-x   0        0        0      175 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/src/images_upload_cli/__init__.py
+-rwxr-xr-x   0        0        0      178 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/src/images_upload_cli/__main__.py
+-rwxr-xr-x   0        0        0     2407 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/src/images_upload_cli/cli.py
+-rwxr-xr-x   0        0        0    10763 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/src/images_upload_cli/upload.py
+-rwxr-xr-x   0        0        0     3133 2023-06-22 20:02:09.801887 images_upload_cli-2.0.0a1/src/images_upload_cli/util.py
+-rw-r--r--   0        0        0     6197 1970-01-01 00:00:00.000000 images_upload_cli-2.0.0a1/PKG-INFO
```

### Comparing `images_upload_cli-2.0.0a0/LICENSE` & `images_upload_cli-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `images_upload_cli-2.0.0a0/README.md` & `images_upload_cli-2.0.0a1/README.md`

 * *Files identical despite different names*

### Comparing `images_upload_cli-2.0.0a0/pyproject.toml` & `images_upload_cli-2.0.0a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "images-upload-cli"
-version = "2.0.0-alpha.0"
+version = "2.0.0-alpha.1"
 description = "Upload images via APIs"
 authors = ["DeadNews <aurczpbgr@mozmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DeadNews/images-upload-cli"
 repository = "https://github.com/DeadNews/images-upload-cli"
 keywords = ["cli", "imgur", "image-upload", "upload-images", "upload-pictures"]
@@ -25,15 +25,15 @@
 pyperclip = "^1.8.2"
 python-dotenv = "^1.0.0"
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
 mypy = "^1.4.0"
 poethepoet = "^0.20.0"
-ruff = "^0.0.274"
+ruff = "^0.0.275"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 pytest-asyncio = "^0.21.0"
 pytest-httpx = "^0.22.0"
```

### Comparing `images_upload_cli-2.0.0a0/src/images_upload_cli/cli.py` & `images_upload_cli-2.0.0a1/src/images_upload_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     notify: bool,
     clipboard: bool,
 ) -> None:
     """Upload images via APIs."""
     # loading .env variables
     load_dotenv(dotenv_path=get_config_path())
 
-    # images upload
+    # async images upload
     links = asyncio.run(
         upload_images(
             upload_func=UPLOAD[hosting],
             images=images,
             bbcode=bbcode,
             thumbnail=thumbnail,
         )
@@ -72,25 +72,24 @@
 
 async def upload_images(
     upload_func: Callable,
     images: tuple[Path],
     bbcode: bool,
     thumbnail: bool,
 ) -> list[str]:
-    """Upload images."""
+    """Upload images coroutine."""
     links = []
 
     async with AsyncClient() as client:
         for img_path in images:
             img = img_path.read_bytes()
 
+            img_link = await upload_func(client, img)
             if not thumbnail:
-                img_link = await upload_func(client, img)
                 link = f"[img]{img_link}[/img]" if bbcode else img_link
             else:
-                img_link = await upload_func(client, img)
                 thumb_link = await upload_func(client, make_thumbnail(img))
                 link = f"[url={img_link}][img]{thumb_link}[/img][/url]"
 
             links.append(link)
 
     return links
```

### Comparing `images_upload_cli-2.0.0a0/src/images_upload_cli/upload.py` & `images_upload_cli-2.0.0a1/src/images_upload_cli/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     response.raise_for_status()
 
     match = search(r"<imagepath>(.+?)</imagepath>", response.text)
     if match is None:
         msg = "Image link not found in response."
         raise HTTPError(msg)
 
-    return match.group(1).strip()
+    return match[1].strip()
 
 
 async def filecoffee_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to file.coffee."""
     response = await client.post(
         url="https://file.coffee/api/file/upload",
         files={"file": img},
@@ -118,15 +118,15 @@
     response.raise_for_status()
 
     match = search(r"url:(.+?)$", response.text)
     if match is None:
         msg = "Image link not found in response."
         raise HTTPError(msg)
 
-    return match.group(1).strip()
+    return match[1].strip()
 
 
 async def imgbb_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to imgbb.com."""
     key = get_env("IMGBB_KEY")
 
     response = await client.post(
@@ -207,15 +207,15 @@
     # get direct link
     get_resp = await client.get(show_url)
     u = urlparse(show_url)
     match = search(
         rf"({u.scheme}://(.+?){u.netloc}/images/{u.path.removeprefix('/show/')})",
         get_resp.text,
     )
-    image_link = None if match is None else match.group(0).strip()
+    image_link = None if match is None else match[0].strip()
 
     return show_url if image_link is None else image_link
 
 
 async def ptpimg_upload(client: AsyncClient, img: bytes) -> str:
     """Upload to ptpimg.me."""
     key = get_env("PTPIMG_KEY")
```

### Comparing `images_upload_cli-2.0.0a0/src/images_upload_cli/util.py` & `images_upload_cli-2.0.0a1/src/images_upload_cli/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 """Utils."""
 
+from functools import lru_cache
 from io import BytesIO
 from os import getenv
 from pathlib import Path
 from shutil import which
 from subprocess import Popen
 
 import click
@@ -40,14 +41,15 @@
 
 
 def get_img_ext(img: bytes) -> str:
     """Get image extension from bytes."""
     return Image.open(BytesIO(img)).format.lower()
 
 
+@lru_cache
 def get_font() -> ImageFont.FreeTypeFont:
     """Attempt to retrieve a reasonably-looking TTF font from the system."""
     font_names = [
         "Helvetica",
         "NotoSerif-Regular",
         "Menlo",
         "DejaVuSerif",
```

### Comparing `images_upload_cli-2.0.0a0/PKG-INFO` & `images_upload_cli-2.0.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: images-upload-cli
-Version: 2.0.0a0
+Version: 2.0.0a1
 Summary: Upload images via APIs
 Home-page: https://github.com/DeadNews/images-upload-cli
 License: MIT
 Keywords: cli,imgur,image-upload,upload-images,upload-pictures
 Author: DeadNews
 Author-email: aurczpbgr@mozmail.com
 Requires-Python: >=3.9,<4.0
```

