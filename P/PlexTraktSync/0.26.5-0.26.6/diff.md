# Comparing `tmp/PlexTraktSync-0.26.5.tar.gz` & `tmp/PlexTraktSync-0.26.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-y7kxfii4/PlexTraktSync-0.26.5.tar", last modified: Mon May 22 17:56:10 2023, max compression
+gzip compressed data, was "/home/runner/work/PlexTraktSync/PlexTraktSync/dist/.tmp-qk_kp6uh/PlexTraktSync-0.26.6.tar", last modified: Sat Jun 24 17:51:46 2023, max compression
```

## Comparing `PlexTraktSync-0.26.5.tar` & `PlexTraktSync-0.26.6.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/PlexTraktSync.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/bug_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/clear_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/imdb_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/plex_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/self_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/trakt_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/unmatched.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/watch.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/commands/watched_shows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/config/
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/ConfigLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/ConfigMergeMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/HttpCacheConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/PlexServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/RunConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/ServerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/SyncConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/config.default.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/flatten.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/http_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/measure_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/memoize.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/nocache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/decorators/time_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/logger/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/logger/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/mixin/ChangeNotifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/plex/
--rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexApi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexAudioCodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexGuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexLibraryItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexLibrarySection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexRatings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexServerConnection.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/PlexWatchList.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/SessionCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/plex/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/pytrakt_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/queue/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/queue/BackgroundTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/queue/Queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/queue/TraktBatchWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/queue/TraktMarkWatchedWorker.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/rich_addons.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/servers.default.yml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/style.py
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/PartialTraktMedia.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/ScrobblerCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/ScrobblerProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/TraktApi.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/TraktItem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/TraktLookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/TraktRatingCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/TraktWatchlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/trakt_set.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/trakt_list_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/util/
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/Factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/Path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/Timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/Version.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/execp.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/execx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/expand_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/git_version_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/local_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/openurl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/parse_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/util/remove_empty_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/plextraktsync/watch/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/EventFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/WatchStateUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/WebSocketListener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/plextraktsync/watch/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-22 17:56:02.000000 PlexTraktSync-0.26.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:56:10.000000 PlexTraktSync-0.26.5/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_collection_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_events.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_new_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_plex_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_threading.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_timer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_trakt_progress.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_tv_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-05-22 17:55:59.000000 PlexTraktSync-0.26.5/tests/test_walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/PlexTraktSync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19069 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/PlexTraktSync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/PlexTraktSync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/PlexTraktSync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/PlexTraktSync.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/PlexTraktSync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/PlexTraktSync.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/plextraktsync/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-24 17:51:36.000000 PlexTraktSync-0.26.6/plextraktsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/plextraktsync/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/bug_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/clear_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/imdb_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/plex_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/self_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/trakt_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/unmatched.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/commands/watched_shows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/plextraktsync/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/config/ConfigLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/config/ConfigMergeMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/config/HttpCacheConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/config/PlexServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/config/RunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/config/ServerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/config/SyncConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/config.default.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/plextraktsync/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/decorators/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/decorators/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/decorators/http_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/decorators/measure_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/decorators/memoize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/decorators/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/decorators/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/decorators/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/decorators/time_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/plextraktsync/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/logger/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/plextraktsync/mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/mixin/ChangeNotifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/plextraktsync/plex/
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/plex/PlexApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/plex/PlexAudioCodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/plex/PlexGuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/plex/PlexLibraryItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/plex/PlexLibrarySection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/plex/PlexRatings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/plex/PlexServerConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/plex/PlexWatchList.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/plex/SessionCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/plex/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/pytrakt_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/plextraktsync/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/queue/BackgroundTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/queue/Queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/queue/TraktBatchWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/queue/TraktMarkWatchedWorker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/rich_addons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/servers.default.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/plextraktsync/trakt/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/trakt/PartialTraktMedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/trakt/ScrobblerCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/trakt/ScrobblerProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/trakt/TraktApi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/trakt/TraktItem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/trakt/TraktLookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/trakt/TraktRatingCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/trakt/TraktWatchlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/trakt/trakt_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/trakt/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/trakt_list_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/plextraktsync/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/Factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/Timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/Version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/execp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/execx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/expand_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/git_version_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/local_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/openurl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/parse_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/util/remove_empty_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/plextraktsync/watch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/watch/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/watch/EventFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/watch/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/watch/WatchStateUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/watch/WebSocketListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/plextraktsync/watch/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-24 17:51:38.000000 PlexTraktSync-0.26.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 17:51:46.000000 PlexTraktSync-0.26.6/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1923 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/tests/test_collection_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1443 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/tests/test_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2703 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/tests/test_events.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/tests/test_logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      977 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/tests/test_new_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/tests/test_plex_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      503 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/tests/test_threading.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/tests/test_timer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      572 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/tests/test_trakt_progress.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3584 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/tests/test_tv_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1926 2023-06-24 17:51:35.000000 PlexTraktSync-0.26.6/tests/test_walker.py
```

### Comparing `PlexTraktSync-0.26.5/LICENSE` & `PlexTraktSync-0.26.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/PKG-INFO` & `PlexTraktSync-0.26.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.5
+Version: 0.26.6
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.26.5/PlexTraktSync.egg-info/PKG-INFO` & `PlexTraktSync-0.26.6/PlexTraktSync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PlexTraktSync
-Version: 0.26.5
+Version: 0.26.6
 Summary: Plex-Trakt-Sync is a two-way-sync between trakt.tv and Plex Media Server
 Home-page: https://github.com/Taxel/PlexTraktSync
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Taxel/PlexTraktSync/issues
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `PlexTraktSync-0.26.5/PlexTraktSync.egg-info/SOURCES.txt` & `PlexTraktSync-0.26.6/PlexTraktSync.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 plextraktsync/watch/ProgressBar.py
 plextraktsync/watch/WatchStateUpdater.py
 plextraktsync/watch/WebSocketListener.py
 plextraktsync/watch/events.py
 tests/test_collection_metadata.py
 tests/test_config.py
 tests/test_events.py
+tests/test_logger.py
 tests/test_new_agent.py
 tests/test_plex_search.py
 tests/test_threading.py
 tests/test_timer.py
 tests/test_trakt_progress.py
 tests/test_tv_lookup.py
 tests/test_walker.py
```

### Comparing `PlexTraktSync-0.26.5/PlexTraktSync.egg-info/requires.txt` & `PlexTraktSync-0.26.6/PlexTraktSync.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 attrs==23.1.0
 certifi==2023.5.7
 charset-normalizer==3.1.0
 click==8.1.3
-deprecated==1.2.13
+deprecated==1.2.14
 inquirerpy==0.3.4
 oauthlib==3.2.2
-plexapi==4.13.4
+plexapi==4.14.0
 prompt-toolkit==3.0.38
 pygments==2.15.1
 python-dotenv==0.21.1
 python-git-info==0.8.3
 pytimeparse==1.1.8
 pytrakt==3.4.23
 pyyaml==6.0
 requests-cache==1.0.0b1
-requests==2.30.0
-rich==13.3.5
+requests==2.31.0
+rich==13.4.2
 tqdm==4.65.0
-urllib3==2.0.2
+urllib3==2.0.3
 wcwidth==0.2.6
-websocket-client==1.5.1
+websocket-client==1.6.0
 
 [:python_version <= "3.7"]
 backports.cached-property==1.0.2
 
 [:python_version >= "3.4"]
 requests-oauthlib==1.3.1
 six==1.16.0
@@ -32,14 +32,14 @@
 idna==3.4
 wrapt==1.15.0
 
 [:python_version >= "3.6"]
 url-normalize==1.4.3
 
 [:python_version >= "3.7"]
-cattrs==22.2.0
+cattrs==23.1.2
 markdown-it-py==2.2.0
 mdurl==0.1.2
-platformdirs==3.5.0
+platformdirs==3.7.0
 
 [:python_version >= "3.7" and python_version < "4.0"]
 pfzy==0.3.4
```

### Comparing `PlexTraktSync-0.26.5/README.md` & `PlexTraktSync-0.26.6/README.md`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/cli.py` & `PlexTraktSync-0.26.6/plextraktsync/cli.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/bug_report.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/bug_report.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/cache.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/cache.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/clear_collections.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/clear_collections.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/config.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/download.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/download.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/imdb_import.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/imdb_import.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/info.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/info.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/inspect.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/login.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/plex_login.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/plex_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/self_update.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/self_update.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/sync.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/trakt_login.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/trakt_login.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/unmatched.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/unmatched.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/watch.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/watch.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/commands/watched_shows.py` & `PlexTraktSync-0.26.6/plextraktsync/commands/watched_shows.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/config/Config.py` & `PlexTraktSync-0.26.6/plextraktsync/config/Config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/config/ConfigLoader.py` & `PlexTraktSync-0.26.6/plextraktsync/config/ConfigLoader.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/config/HttpCacheConfig.py` & `PlexTraktSync-0.26.6/plextraktsync/config/HttpCacheConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/config/ServerConfig.py` & `PlexTraktSync-0.26.6/plextraktsync/config/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/config/SyncConfig.py` & `PlexTraktSync-0.26.6/plextraktsync/config/SyncConfig.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/config.default.yml` & `PlexTraktSync-0.26.6/plextraktsync/config.default.yml`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/decorators/rate_limit.py` & `PlexTraktSync-0.26.6/plextraktsync/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/decorators/retry.py` & `PlexTraktSync-0.26.6/plextraktsync/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/logger/filter.py` & `PlexTraktSync-0.26.6/plextraktsync/logger/filter.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/logging.py` & `PlexTraktSync-0.26.6/plextraktsync/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,16 @@
         from plexapi import loghandler
 
         logger.removeHandler(loghandler)
         logger.setLevel(logging.DEBUG)
 
 
 class CustomFormatter(logging.Formatter):
-    def format(self, record):
-        record.msg = self.remove_markup(record.msg)
-        return super().format(record)
+    MARKUP_PATTERN = re.compile(r'\[link=[^\]]*\]|(\[green\])|(\[\/\])')
 
-    def remove_markup(self, text):
-        pattern = r'\[link=[^\]]*\]|(\[green\])|(\[\/\])'
-        return re.sub(pattern, '', text)
+    def formatMessage(self, record):
+        record.message = self.remove_markup(record.message)
+        return super().formatMessage(record)
+
+    @classmethod
+    def remove_markup(cls, text: str) -> str:
+        return cls.MARKUP_PATTERN.sub('', text)
```

### Comparing `PlexTraktSync-0.26.5/plextraktsync/media.py` & `PlexTraktSync-0.26.6/plextraktsync/media.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/mixin/ChangeNotifier.py` & `PlexTraktSync-0.26.6/plextraktsync/mixin/ChangeNotifier.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/plex/PlexApi.py` & `PlexTraktSync-0.26.6/plextraktsync/plex/PlexApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/plex/PlexAudioCodec.py` & `PlexTraktSync-0.26.6/plextraktsync/plex/PlexAudioCodec.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/plex/PlexGuid.py` & `PlexTraktSync-0.26.6/plextraktsync/plex/PlexGuid.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/plex/PlexLibraryItem.py` & `PlexTraktSync-0.26.6/plextraktsync/plex/PlexLibraryItem.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/plex/PlexLibrarySection.py` & `PlexTraktSync-0.26.6/plextraktsync/plex/PlexLibrarySection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/plex/PlexRatings.py` & `PlexTraktSync-0.26.6/plextraktsync/plex/PlexRatings.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/plex/PlexServerConnection.py` & `PlexTraktSync-0.26.6/plextraktsync/plex/PlexServerConnection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/plex/PlexWatchList.py` & `PlexTraktSync-0.26.6/plextraktsync/plex/PlexWatchList.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/plex/SessionCollection.py` & `PlexTraktSync-0.26.6/plextraktsync/plex/SessionCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/pytrakt_extensions.py` & `PlexTraktSync-0.26.6/plextraktsync/pytrakt_extensions.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/queue/BackgroundTask.py` & `PlexTraktSync-0.26.6/plextraktsync/queue/BackgroundTask.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/queue/Queue.py` & `PlexTraktSync-0.26.6/plextraktsync/queue/Queue.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/queue/TraktBatchWorker.py` & `PlexTraktSync-0.26.6/plextraktsync/queue/TraktBatchWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/queue/TraktMarkWatchedWorker.py` & `PlexTraktSync-0.26.6/plextraktsync/queue/TraktMarkWatchedWorker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/rich_addons.py` & `PlexTraktSync-0.26.6/plextraktsync/rich_addons.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/sync.py` & `PlexTraktSync-0.26.6/plextraktsync/sync.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/trakt/ScrobblerCollection.py` & `PlexTraktSync-0.26.6/plextraktsync/trakt/ScrobblerCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/trakt/ScrobblerProxy.py` & `PlexTraktSync-0.26.6/plextraktsync/trakt/ScrobblerProxy.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/trakt/TraktApi.py` & `PlexTraktSync-0.26.6/plextraktsync/trakt/TraktApi.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/trakt/TraktItem.py` & `PlexTraktSync-0.26.6/plextraktsync/trakt/TraktItem.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/trakt/TraktLookup.py` & `PlexTraktSync-0.26.6/plextraktsync/trakt/TraktLookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/trakt/TraktRatingCollection.py` & `PlexTraktSync-0.26.6/plextraktsync/trakt/TraktRatingCollection.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/trakt/TraktWatchlist.py` & `PlexTraktSync-0.26.6/plextraktsync/trakt/TraktWatchlist.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/trakt_list_util.py` & `PlexTraktSync-0.26.6/plextraktsync/trakt_list_util.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/util/Factory.py` & `PlexTraktSync-0.26.6/plextraktsync/util/Factory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/util/Path.py` & `PlexTraktSync-0.26.6/plextraktsync/util/Path.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/util/Timer.py` & `PlexTraktSync-0.26.6/plextraktsync/util/Timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/util/Version.py` & `PlexTraktSync-0.26.6/plextraktsync/util/Version.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/util/expand_id.py` & `PlexTraktSync-0.26.6/plextraktsync/util/expand_id.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/util/local_url.py` & `PlexTraktSync-0.26.6/plextraktsync/util/local_url.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/util/openurl.py` & `PlexTraktSync-0.26.6/plextraktsync/util/openurl.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/util/packaging.py` & `PlexTraktSync-0.26.6/plextraktsync/util/packaging.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/util/remove_empty_values.py` & `PlexTraktSync-0.26.6/plextraktsync/util/remove_empty_values.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/walker.py` & `PlexTraktSync-0.26.6/plextraktsync/walker.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/watch/EventDispatcher.py` & `PlexTraktSync-0.26.6/plextraktsync/watch/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/watch/EventFactory.py` & `PlexTraktSync-0.26.6/plextraktsync/watch/EventFactory.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/watch/ProgressBar.py` & `PlexTraktSync-0.26.6/plextraktsync/watch/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/watch/WatchStateUpdater.py` & `PlexTraktSync-0.26.6/plextraktsync/watch/WatchStateUpdater.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/watch/WebSocketListener.py` & `PlexTraktSync-0.26.6/plextraktsync/watch/WebSocketListener.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/plextraktsync/watch/events.py` & `PlexTraktSync-0.26.6/plextraktsync/watch/events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/requirements.txt` & `PlexTraktSync-0.26.6/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 # To regenerate from the project's Pipfile, run:
 #
 #    pipenv lock --requirements
 #
 
 attrs==23.1.0
 backports.cached-property==1.0.2; python_version <= '3.7'
-cattrs==22.2.0; python_version >= '3.7'
+cattrs==23.1.2; python_version >= '3.7'
 certifi==2023.5.7
 charset-normalizer==3.1.0
 click==8.1.3
-deprecated==1.2.13
+deprecated==1.2.14
 idna==3.4; python_version >= '3.5'
 inquirerpy==0.3.4
 markdown-it-py==2.2.0; python_version >= '3.7'
 mdurl==0.1.2; python_version >= '3.7'
 oauthlib==3.2.2
 pfzy==0.3.4; python_version >= '3.7' and python_version < '4.0'
-platformdirs==3.5.0; python_version >= '3.7'
-plexapi==4.13.4
+platformdirs==3.7.0; python_version >= '3.7'
+plexapi==4.14.0
 prompt-toolkit==3.0.38
 pygments==2.15.1
 python-dotenv==0.21.1
 python-git-info==0.8.3
 pytimeparse==1.1.8
 pytrakt==3.4.23
 pyyaml==6.0
 requests-cache==1.0.0b1
 requests-oauthlib==1.3.1; python_version >= '3.4'
-requests==2.30.0
-rich==13.3.5
+requests==2.31.0
+rich==13.4.2
 six==1.16.0; python_version >= '3.4'
 tqdm==4.65.0
 url-normalize==1.4.3; python_version >= '3.6'
-urllib3==2.0.2
+urllib3==2.0.3
 wcwidth==0.2.6
-websocket-client==1.5.1
+websocket-client==1.6.0
 wrapt==1.15.0; python_version >= '3.5'
```

### Comparing `PlexTraktSync-0.26.5/setup.cfg` & `PlexTraktSync-0.26.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/tests/test_collection_metadata.py` & `PlexTraktSync-0.26.6/tests/test_collection_metadata.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/tests/test_config.py` & `PlexTraktSync-0.26.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/tests/test_events.py` & `PlexTraktSync-0.26.6/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/tests/test_new_agent.py` & `PlexTraktSync-0.26.6/tests/test_new_agent.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/tests/test_timer.py` & `PlexTraktSync-0.26.6/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/tests/test_trakt_progress.py` & `PlexTraktSync-0.26.6/tests/test_trakt_progress.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/tests/test_tv_lookup.py` & `PlexTraktSync-0.26.6/tests/test_tv_lookup.py`

 * *Files identical despite different names*

### Comparing `PlexTraktSync-0.26.5/tests/test_walker.py` & `PlexTraktSync-0.26.6/tests/test_walker.py`

 * *Files identical despite different names*

