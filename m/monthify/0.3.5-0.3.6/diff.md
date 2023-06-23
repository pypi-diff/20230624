# Comparing `tmp/monthify-0.3.5.tar.gz` & `tmp/monthify-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monthify-0.3.5.tar", max compression
+gzip compressed data, was "monthify-0.3.6.tar", max compression
```

## Comparing `monthify-0.3.5.tar` & `monthify-0.3.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1133 2023-05-18 06:24:22.438685 monthify-0.3.5/README.md
--rw-r--r--   0        0        0      435 2023-05-28 05:00:16.109215 monthify-0.3.5/monthify/__init__.py
--rw-r--r--   0        0        0       68 2023-05-18 06:24:22.439685 monthify-0.3.5/monthify/__main__.py
--rw-r--r--   0        0        0     1610 2023-06-13 20:30:31.505128 monthify-0.3.5/monthify/args.py
--rw-r--r--   0        0        0     1103 2023-05-28 04:45:17.054980 monthify-0.3.5/monthify/auth.py
--rw-r--r--   0        0        0      811 2023-05-28 04:59:34.295576 monthify-0.3.5/monthify/config.py
--rw-r--r--   0        0        0     2916 2023-06-13 20:36:34.279834 monthify-0.3.5/monthify/main.py
--rw-r--r--   0        0        0    19056 2023-06-17 20:47:51.409566 monthify-0.3.5/monthify/script.py
--rw-r--r--   0        0        0      769 2023-06-13 20:30:31.506127 monthify-0.3.5/monthify/track.py
--rw-r--r--   0        0        0     1185 2023-05-27 02:42:22.456255 monthify-0.3.5/monthify/utils.py
--rw-r--r--   0        0        0      815 2023-05-28 04:27:43.087494 monthify-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 monthify-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-05-18 06:24:22.438685 monthify-0.3.6/README.md
+-rw-r--r--   0        0        0      435 2023-06-17 20:51:52.540666 monthify-0.3.6/monthify/__init__.py
+-rw-r--r--   0        0        0       68 2023-05-18 06:24:22.439685 monthify-0.3.6/monthify/__main__.py
+-rw-r--r--   0        0        0     1610 2023-06-17 20:51:52.540666 monthify-0.3.6/monthify/args.py
+-rw-r--r--   0        0        0     1103 2023-06-17 20:51:52.540666 monthify-0.3.6/monthify/auth.py
+-rw-r--r--   0        0        0      811 2023-06-17 20:51:52.540666 monthify-0.3.6/monthify/config.py
+-rw-r--r--   0        0        0     2916 2023-06-17 20:51:52.540666 monthify-0.3.6/monthify/main.py
+-rw-r--r--   0        0        0    18736 2023-06-23 22:28:01.461301 monthify-0.3.6/monthify/script.py
+-rw-r--r--   0        0        0      769 2023-06-17 20:51:52.541666 monthify-0.3.6/monthify/track.py
+-rw-r--r--   0        0        0     1185 2023-05-27 02:42:22.456255 monthify-0.3.6/monthify/utils.py
+-rw-r--r--   0        0        0      815 2023-06-23 22:28:01.462301 monthify-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1792 1970-01-01 00:00:00.000000 monthify-0.3.6/PKG-INFO
```

### Comparing `monthify-0.3.5/README.md` & `monthify-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `monthify-0.3.5/monthify/args.py` & `monthify-0.3.6/monthify/args.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.5/monthify/auth.py` & `monthify-0.3.6/monthify/auth.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.5/monthify/config.py` & `monthify-0.3.6/monthify/config.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.5/monthify/main.py` & `monthify-0.3.6/monthify/main.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.5/monthify/script.py` & `monthify-0.3.6/monthify/script.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 # Script
 import sys
-
-# from collections.abc import Iterable
 from datetime import datetime
 from os import makedirs, remove, stat
 from os.path import exists
 from pathlib import Path
-from typing import Any, Generator, Iterable, List, Reversible, Tuple
+from typing import Any, Generator, Iterable, List, Optional, Reversible, Tuple
 
 from cachetools import TTLCache, cached
 from loguru import logger
 
 from monthify import ERROR, SUCCESS, appdata_location, console
 from monthify.auth import Auth
 from monthify.track import Track
 from monthify.utils import conditional_decorator, normalize_text, sort_chronologically
 
 MAX_RESULTS = 10000
 CACHE_LIFETIME = 30
 
 makedirs(f"{appdata_location}/logs", exist_ok=True)
-logger.add(
-    sys.stderr, format="{time} {level} {message}", filter="monthify", level="INFO"
-)
+logger.add(sys.stderr, format="{time} {level} {message}", filter="monthify", level="INFO")
 logger.remove()
 logger.add(f"{appdata_location}/logs/monthify.log", rotation="00:00", compression="zip")
 existing_playlists_file = f"{appdata_location}/existing_playlists_file.dat"
 last_run_file = f"{appdata_location}/last_run.txt"
 last_run_format = "%Y-%m-%d %H:%M:%S"
 saved_tracks_cache: TTLCache = TTLCache(maxsize=1000, ttl=86400)
 saved_playlists_cache: TTLCache = TTLCache(maxsize=1000, ttl=86400)
@@ -50,21 +46,17 @@
         self.SKIP_PLAYLIST_CREATION = SKIP_PLAYLIST_CREATION
         self.CREATE_PLAYLIST = CREATE_PLAYLIST
         self.has_created_playlists = False
         self.current_username: str
         self.current_display_name: str
         self.playlist_names: List[Tuple[str, str]]
         self.already_created_playlists_exists = False
-        if (
-            exists(existing_playlists_file)
-            and stat(existing_playlists_file).st_size != 0
-        ):
+        if exists(existing_playlists_file) and stat(existing_playlists_file).st_size != 0:
             if (
-                datetime.now()
-                - datetime.fromtimestamp(Path(existing_playlists_file).stat().st_ctime)
+                datetime.now() - datetime.fromtimestamp(Path(existing_playlists_file).stat().st_ctime)
             ).days >= CACHE_LIFETIME:
                 remove(existing_playlists_file)
                 self.already_created_playlists = []
                 self.already_created_playlists_exists = False
             else:
                 with open(existing_playlists_file, "r", encoding="utf_8") as f:
                     self.already_created_playlists = list(f.read().splitlines())
@@ -109,88 +101,94 @@
                 sys.exit(0)
 
     def starting(self) -> None:
         """
         Staring function
         Displays project name and current username
         """
+
         logger.info("Starting script execution")
         console.print(self.name, style="green")
         with console.status("Retrieving user information"):
             self.current_display_name = self.get_username()["display_name"]
             self.current_username = self.get_username()["uri"][13:]
         console.print(f"Username: [cyan]{self.current_display_name}[/cyan]\n")
 
     def update_last_run(self) -> None:
         """
         Updates last run time to current time
         """
+
         self.last_run = datetime.now().strftime(last_run_format)
         with open(last_run_file, "w", encoding="utf_8") as f:
             f.write(self.last_run)
 
     def get_results(self, result):
         """
         Retrieves all results from a spotify api call
         """
+
         results = []
         while result:
             results += [*result["items"]]
             if result["next"]:
                 result = self.sp.next(result)
             else:
                 result = None
         return results
 
     @cached(user_cache)
     def get_username(self) -> dict:
         """
         Retrieves the current user's spotify information
         """
+
         return self.sp.current_user()
 
     @cached(saved_tracks_cache)
     def get_user_saved_tracks(self) -> List[dict]:
         """
         Retrieves the current user's saved spotify tracks
         """
+
         logger.info("Starting user saved tracks fetch")
         results = self.get_results(self.sp.current_user_saved_tracks(limit=50))
         logger.info("Ending user saved tracks fetch")
         return results
 
     @conditional_decorator(cached(saved_playlists_cache), "has_created_playlists")
     def get_user_saved_playlists(self):
         """
         Retrieves the current user's created or liked spotify playlists
         """
+
         logger.info("Starting user saved playlists fetch")
         results = self.get_results(self.sp.current_user_playlists(limit=50))
         logger.info("Ending user saved playlists fetch")
         return results
 
     def get_playlist_items(self, playlist_id: str) -> List[dict]:
         """
         Retrieves all the tracks in a specified spotify playlist identified by playlist id
         """
+
         logger.info(f"Starting playlist item fetch\n id: {playlist_id}", playlist_id)
-        results = self.get_results(
-            self.sp.playlist_items(playlist_id=playlist_id, fields=None, limit=20)
-        )
+        results = self.get_results(self.sp.playlist_items(playlist_id=playlist_id, fields=None, limit=20))
         logger.info(f"Ending playlist item fetch\n id: {playlist_id}")
         return results
 
     def create_playlist(self, name: str) -> None:
         """
         Creates playlist with name var checking if the playlist already exists in the user's library,
         if it does the user is informed
         """
+
         sp = self.sp
         playlists = self.get_user_saved_playlists()
-        already_created_playlists = []
+        already_created_playlists: List[str] = []
         created_playlists = []
         count = 0
         logger.info(f"Playlist creation called {name}")
         for item in playlists:
             if normalize_text(item["name"]) == normalize_text(name):
                 count += 1
                 console.print(f"Playlist {name} already exists")
@@ -215,21 +213,23 @@
         self.has_created_playlists = True if len(created_playlists) > 0 else False
         self.already_created_playlists_inter = already_created_playlists
 
     def get_saved_track_info(self) -> None:
         """
         Calls the get_saved_track_gen function at program's start to cache the user's saved tracks
         """
+
         with console.status("Retrieving user saved tracks"):
             self.get_saved_track_gen()
 
     def get_saved_track_gen(self) -> Generator[Track, Any, None]:
         """
         Collates the user's saved tracks and adds them to a list as a Track type
         """
+
         tracks = self.get_user_saved_tracks()
         logger.info("Retrieving saved track info")
         track_list = (
             Track(
                 title=item["track"]["name"],
                 artist=item["track"]["artists"][0]["name"],
                 added_at=item["added_at"],
@@ -239,196 +239,184 @@
         )
         return track_list
 
     def get_playlist_names_names(self):
         """
         Generates month playlist names using the added_at attribute of the Track type
         """
+
         logger.info("Generating playlist names")
-        self.playlist_names = tuple(
-            track.track_month for track in self.get_saved_track_gen()
-        )
+        self.playlist_names = tuple(track.track_month for track in self.get_saved_track_gen())
         unsorted_playlist_names = [*set(self.playlist_names)]
         self.playlist_names = sort_chronologically(unsorted_playlist_names)
         logger.info("Removing duplicate playlist names")
         logger.info(f"Final list: {self.playlist_names}")
 
     def get_monthly_playlist_ids(self):
         """
         Retrieves playlist ids of already created month playlists
         """
+
         logger.info("Retrieving playlist ids")
         with console.status("Retrieving relevant playlist information"):
             playlists = self.get_user_saved_playlists()
             for month, year in self.playlist_names:
                 for item in playlists:
-                    if normalize_text((month + " '" + year[2:])) == normalize_text(
-                        item["name"]
-                    ):
+                    if normalize_text((month + " '" + year[2:])) == normalize_text(item["name"]):
                         self.playlist_names_with_id.append((month, year, item["id"]))
                         logger.info(
                             "Playlist name: {name} id: {id}",
                             name=str(month + " '" + year[2:]),
                             id=str(item["id"]),
                         )
 
-    def skip(self, status: bool, playlists: Iterable = None) -> None:
+    def skip(self, status: bool, playlists: Optional[Iterable] = None) -> None:
+        """
+        Skips playlist generation if status is True
+        """
+
         if status is True:
             console.print("Playlist generation skipped")
             logger.info("Playlist generation skipped")
         else:
             logger.info("Playlist generation starting")
             if playlists is None:
                 RuntimeError("Playlists have not passed been passed to skip function")
             for month, year in reversed(self.playlist_names):
                 playlist_name = str(month + " '" + year[2:])
-                if (
-                    playlist_name in self.already_created_playlists
-                    and playlist_name in playlists
-                ):
+                if playlist_name in self.already_created_playlists and playlist_name in playlists:
                     console.print(f"{month} '{year[2:]} playlist already exists")
                 else:
                     name = month + " '" + year[2:]
                     self.create_playlist(name)
 
     def create_monthly_playlists(self):
         """
         Creates playlists in user's library based on generated playlist names
         """
+
         logger.info("Creating playlists")
         with console.status("Generating playlists"):
-            spotify_playlists = [
-                item["name"] for item in self.get_user_saved_playlists()
-            ]
+            spotify_playlists = [item["name"] for item in self.get_user_saved_playlists()]
 
         monthly_ran = False
-        last_run = (
-            datetime.now().strftime(last_run_format)
-            if not self.last_run
-            else self.last_run
-        )
+        last_run = datetime.now().strftime(last_run_format) if not self.last_run else self.last_run
 
-        has_month_passed = datetime.strptime(last_run, last_run_format).strftime(
-            "%B"
-        ) != datetime.now().strftime("%B")
+        has_month_passed = datetime.strptime(last_run, last_run_format).strftime("%B") != datetime.now().strftime("%B")
         if has_month_passed and self.already_created_playlists_exists is False:
             self.skip(False, spotify_playlists)
         elif has_month_passed is False and self.already_created_playlists_exists:
             monthly_ran = True
 
         if self.CREATE_PLAYLIST is False:
             if self.SKIP_PLAYLIST_CREATION is False and monthly_ran is False:
+                console.print("Playlist generation has not occured this month, Generating Playlists...")
+                logger.info("Requesting playlist creation")
+                self.skip(False, spotify_playlists)
+
+            elif self.SKIP_PLAYLIST_CREATION is False and monthly_ran is True:
                 console.print(
                     "Playlist generation has already occurred this month, do you still want to generate "
                     "playlists? (yes/no)"
                 )
                 logger.info("Requesting playlist creation")
 
                 if not console.input("> ").lower().startswith("y"):
                     self.skip(True)
                 else:
                     self.skip(False, spotify_playlists)
 
             elif self.already_created_playlists_exists is False:
-                console.print(
-                    "Somehow the playlists do not exist. Generating Playlists..."
-                )
+                console.print("Somehow the playlists do not exist. Generating Playlists...")
                 logger.info("Requesting playlist creation")
                 self.skip(False, spotify_playlists)
 
             else:
                 self.skip(True)
 
         else:
             self.skip(False, spotify_playlists)
 
         if self.already_created_playlists_inter:
             self.already_created_playlists = [
                 *self.already_created_playlists,
                 *self.already_created_playlists_inter,
             ]
-            self.already_created_playlists = list(
-                dict.fromkeys(self.already_created_playlists)
-            )
+            self.already_created_playlists = list(dict.fromkeys(self.already_created_playlists))
 
         if self.already_created_playlists:
             with open(existing_playlists_file, "w", encoding="utf_8") as f:
                 f.write("\n".join(self.already_created_playlists))
 
     def add_to_playlist(self, tracks: Reversible[Track], playlist_id: str) -> None:
         """
         Add a list of tracks to a specified playlist using playlist id
         """
+
         logger.info(
             "Attempting to add tracks to playlist: {playlist}\ntracks: {tracks} ",
             tracks=tracks,
             playlist=str(playlist_id),
         )
         playlist_items = self.get_playlist_items(playlist_id)
         to_be_added_uris: list[str] = []
 
-        playlist_uris: Iterable[str] = tuple(
-            item["track"]["uri"] for item in playlist_items
-        )
+        playlist_uris: Iterable[str] = tuple(item["track"]["uri"] for item in playlist_items)
 
         for track in reversed(tracks):
             if track.uri in playlist_uris:
                 logger.info(f"Track: {track} already in playlist: {str(playlist_id)}")
                 track_url = f'https://open.{track.uri.replace(":", "/").replace("spotify", "spotify.com")}'
                 console.print(
                     f"[bold red][-][/bold red]\t[link={track_url}][cyan]{track.title} by {track.artist}[/cyan][/link]"
                     " already exists in the playlist"
                 )
             else:
-                logger.info(
-                    f"Track: {track} will be added to playlist: {str(playlist_id)}"
-                )
+                logger.info(f"Track: {track} will be added to playlist: {str(playlist_id)}")
                 track_url = f'https://open.{track.uri.replace(":", "/").replace("spotify", "spotify.com")}'
                 console.print(
                     f"[bold green][+][/bold green]\t[link={track_url}][bold green]{track.title} by {track.artist}"
                     "[/bold green][/link]"
                     " will be added to the playlist "
                 )
                 to_be_added_uris.append(track.uri)
+
         if not to_be_added_uris:
-            logger.info(
-                "No tracks to add to playlist: {playlist}", playlist=playlist_id
-            )
+            logger.info("No tracks to add to playlist: {playlist}", playlist=playlist_id)
             console.print("\t\n")
         else:
             logger.info(
                 "Adding tracks: {tracks} to playlist: {playlist}",
                 tracks=(" ".join(to_be_added_uris)),
                 playlist=playlist_id,
             )
-            to_be_added_uris_chunks = tuple(
-                to_be_added_uris[x : x + 100]
-                for x in range(0, len(to_be_added_uris), 100)
-            )
+            to_be_added_uris_chunks = tuple(to_be_added_uris[x : x + 100] for x in range(0, len(to_be_added_uris), 100))
             for chunk in to_be_added_uris_chunks:
                 self.sp.playlist_add_items(playlist_id=playlist_id, items=chunk)
             console.print("\n")
             self.total_tracks_added += len(to_be_added_uris)
+
         logger.info("Ended track addition")
 
     def sort_tracks_by_month(self):
         """
         Sorts saved tracks into appropriate monthly playlist
         """
+
         log = logger.bind(
             playlist_names=self.playlist_names_with_id,
             tracks=[track.title for track in self.get_saved_track_gen()],
         )
+
         log.info("Started sort")
+
         console.print("\nBeginning playlist sort")
         try:
             if len(self.playlist_names) != len(self.playlist_names_with_id):
-                raise RuntimeError(
-                    "playlist_names and playlist_names_with_id are not the same length"
-                )
+                raise RuntimeError("playlist_names and playlist_names_with_id are not the same length")
         except RuntimeError as error:
             log.error(
                 "playlist_names and playlist_names_with_id are not the same length",
                 playlist_names_length=self.playlist_names.__len__(),
                 playlist_names_with_id_length=self.playlist_names_with_id.__len__(),
                 error=error,
             )
@@ -437,29 +425,21 @@
                 " please run the program again with the --create-playlists flag",
                 style=ERROR,
             )
             sys.exit(1)
 
         with console.status("Sorting Tracks"):
             for month, year, playlist_id in self.playlist_names_with_id:
-                logger.info(
-                    "Sorting into playlist: {playlist}", playlist=(month, year[2:])
-                )
+                logger.info("Sorting into playlist: {playlist}", playlist=(month, year[2:]))
                 playlist_url = f"https://open.spotify.com/playlist/{playlist_id}"
                 playlist_name = f"{month} '{year[2:]}"
 
-                console.rule(
-                    f"Sorting into playlist [link={playlist_url}]{playlist_name}[/link]"
-                )
+                console.rule(f"Sorting into playlist [link={playlist_url}]{playlist_name}[/link]")
                 console.print("\t\n")
-                tracks = tuple(
-                    track
-                    for track in self.get_saved_track_gen()
-                    if track.track_month == (month, year)
-                )
+                tracks = tuple(track for track in self.get_saved_track_gen() if track.track_month == (month, year))
                 if not tracks:
                     break
                 else:
                     logger.info(
                         "Adding tracks to playlist: {playlist}",
                         playlist=str(playlist_id),
                     )
```

### Comparing `monthify-0.3.5/monthify/track.py` & `monthify-0.3.6/monthify/track.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.5/monthify/utils.py` & `monthify-0.3.6/monthify/utils.py`

 * *Files identical despite different names*

### Comparing `monthify-0.3.5/pyproject.toml` & `monthify-0.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monthify"
-version = "0.3.5"
+version = "0.3.6"
 description = "Sorts liked spotify tracks into playlists by the month they were liked."
 authors = ["Madiba Hudson-Quansah <mhquansah@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 loguru = "^0.6.0"
```

### Comparing `monthify-0.3.5/PKG-INFO` & `monthify-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monthify
-Version: 0.3.5
+Version: 0.3.6
 Summary: Sorts liked spotify tracks into playlists by the month they were liked.
 Author: Madiba Hudson-Quansah
 Author-email: mhquansah@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

