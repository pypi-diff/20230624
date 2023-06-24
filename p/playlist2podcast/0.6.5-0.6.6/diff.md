# Comparing `tmp/playlist2podcast-0.6.5.tar.gz` & `tmp/playlist2podcast-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playlist2podcast-0.6.5.tar", last modified: Sun Mar  5 00:38:42 2023, max compression
+gzip compressed data, was "playlist2podcast-0.6.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `playlist2podcast-0.6.5.tar` & `playlist2podcast-0.6.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4968 2023-03-05 00:37:07.609492 playlist2podcast-0.6.5/README.rst
--rw-r--r--   0        0        0     3806 2023-03-05 00:37:07.613492 playlist2podcast-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      218 2023-03-05 00:37:07.613492 playlist2podcast-0.6.5/src/playlist2podcast/__init__.py
--rw-r--r--   0        0        0    20238 2023-03-05 00:37:07.613492 playlist2podcast-0.6.5/src/playlist2podcast/playlist_2_podcast.py
--rw-r--r--   0        0        0     6822 1970-01-01 00:00:00.000000 playlist2podcast-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0     4968 2023-06-24 04:11:11.240766 playlist2podcast-0.6.6/README.rst
+-rw-r--r--   0        0        0     3806 2023-06-24 04:11:11.244766 playlist2podcast-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-06-24 04:11:11.244766 playlist2podcast-0.6.6/src/playlist2podcast/__init__.py
+-rw-r--r--   0        0        0    20201 2023-06-24 04:11:11.244766 playlist2podcast-0.6.6/src/playlist2podcast/playlist_2_podcast.py
+-rw-r--r--   0        0        0     6822 1970-01-01 00:00:00.000000 playlist2podcast-0.6.6/PKG-INFO
```

### Comparing `playlist2podcast-0.6.5/README.rst` & `playlist2podcast-0.6.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         container_name: playlist2podcast
         tty: true
         stdin_open: true
         environment:
           - DEBUG_LOG_FILE=debug.log    # Optional: If set will create a debug log file
           - UPDATE_INTERVAL=4h          # How long to wait between updates.
        volumes:
-          - <path to direcotry containing config.json file>:/config
+          - <path to directory containing config.json file>:/config
           - podcast-data:/publish       # podcast feed data will be saved here
         restart: unless-stopped
         networks:
           - caddy
         labels:
           caddy: <full hostname podcast>    # DNS for this needs to resolve before starting
           caddy.root: "* /publish"
```

### Comparing `playlist2podcast-0.6.5/pyproject.toml` & `playlist2podcast-0.6.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playlist2podcast-0.6.5/src/playlist2podcast/playlist_2_podcast.py` & `playlist2podcast-0.6.6/src/playlist2podcast/playlist_2_podcast.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
     feed.description("Marvin's Youtube Playlist Podcast")
 
     download_options = YDL_DL_OPTS
     download_options[
         "outtmpl"
     ] = f"{config.publish_dir}/{config.media_dir}/%(id)s.%(ext)s"
     download_options["playlistend"] = config.number_of_episodes * 3
-    if config.youtube_cookie_file and config.youtube_cookie_file != "":
+    if config.youtube_cookie_file:
         download_options["cookiefile"] = config.youtube_cookie_file
 
     for current_play_list in config.play_lists:
         rprint(f"Downloading info for videos on playlist: {current_play_list['url']}")
         logger.debug(
             "Downloading info for videos on playlist: %s", current_play_list["url"]
         )
```

### Comparing `playlist2podcast-0.6.5/PKG-INFO` & `playlist2podcast-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playlist2podcast
-Version: 0.6.5
+Version: 0.6.6
 Summary: Creates podcast feed from playlist URL
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -104,15 +104,15 @@
         container_name: playlist2podcast
         tty: true
         stdin_open: true
         environment:
           - DEBUG_LOG_FILE=debug.log    # Optional: If set will create a debug log file
           - UPDATE_INTERVAL=4h          # How long to wait between updates.
        volumes:
-          - <path to direcotry containing config.json file>:/config
+          - <path to directory containing config.json file>:/config
           - podcast-data:/publish       # podcast feed data will be saved here
         restart: unless-stopped
         networks:
           - caddy
         labels:
           caddy: <full hostname podcast>    # DNS for this needs to resolve before starting
           caddy.root: "* /publish"
```

