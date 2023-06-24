# Comparing `tmp/osxphotos-0.60.4.tar.gz` & `tmp/osxphotos-0.60.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.60.4.tar", last modified: Sun Jun 18 23:12:12 2023, max compression
+gzip compressed data, was "osxphotos-0.60.5.tar", last modified: Sat Jun 24 17:51:35 2023, max compression
```

## Comparing `osxphotos-0.60.4.tar` & `osxphotos-0.60.5.tar`

### file list

```diff
@@ -1,233 +1,237 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.857297 osxphotos-0.60.4/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.4/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.4/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-18 23:12:12.857120 osxphotos-0.60.4/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   225512 2023-06-18 23:12:04.000000 osxphotos-0.60.4/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.4/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.823534 osxphotos-0.60.4/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1952 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.4/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15962 2023-06-18 23:09:24.000000 osxphotos-0.60.4/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-06-18 23:11:07.000000 osxphotos-0.60.4/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.4/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.4/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.830564 osxphotos-0.60.4/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3565 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.4/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6869 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9933 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3802 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    27384 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.4/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      713 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   107273 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    22101 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    61649 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.4/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20564 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5674 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     8754 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.4/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3355 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26935 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.4/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28044 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.4/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      692 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5089 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.4/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.830953 osxphotos-0.60.4/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.4/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1460158 2023-06-18 23:12:09.000000 osxphotos-0.60.4/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.4/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.4/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.4/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51790 2023-06-17 04:33:59.000000 osxphotos-0.60.4/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10742 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5121 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.4/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     3787 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    91520 2023-06-17 14:14:35.000000 osxphotos-0.60.4/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    84832 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46258 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     5719 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5332 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.832965 osxphotos-0.60.4/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10393 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7576 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   149944 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.4/osxphotos/phototables.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.4/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-06-18 23:12:03.000000 osxphotos-0.60.4/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.4/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    21858 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.4/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.833967 osxphotos-0.60.4/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.4/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.4/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.4/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.4/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.4/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.4/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.834806 osxphotos-0.60.4/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.4/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3242 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2282 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3442 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)    27213 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    18621 2023-06-17 14:12:56.000000 osxphotos-0.60.4/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.824336 osxphotos-0.60.4/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6400 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-06-18 23:12:12.857334 osxphotos-0.60.4/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.4/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.856639 osxphotos-0.60.4/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.856906 osxphotos-0.60.4/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.4/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.4/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11012 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4849 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5334 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54731 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   273142 2023-06-16 16:22:37.000000 osxphotos-0.60.4/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1798 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4571 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2218 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6798 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.4/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.4/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    29996 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6397 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3450 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.4/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.4/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.4/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.4/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1946 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2748 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.4/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.4/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9781 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18308 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5910 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.4/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10301 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155137 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.4/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4022 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.4/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1270 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.4/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      859 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      930 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.4/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1205 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50393 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4731 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4870 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13430 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5796 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.4/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.4/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.4/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.4/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3376 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7530 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10047 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.4/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)     3017 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.4/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.4/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.4/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      489 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    50016 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.4/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     2032 2023-05-07 13:56:16.000000 osxphotos-0.60.4/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.4/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.4/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.337727 osxphotos-0.60.5/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.5/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.5/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-24 17:51:35.337484 osxphotos-0.60.5/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   225895 2023-06-24 17:51:20.000000 osxphotos-0.60.5/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.5/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.275203 osxphotos-0.60.5/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1955 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.5/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15892 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-06-24 17:51:14.000000 osxphotos-0.60.5/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.5/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.5/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.291701 osxphotos-0.60.5/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3568 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.5/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6899 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9936 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3805 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27388 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.5/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3585 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      715 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   107303 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    22104 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    61930 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.5/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20594 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5845 2023-06-24 17:50:43.000000 osxphotos-0.60.5/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8757 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.5/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3385 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26965 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.5/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28075 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.5/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      695 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1263 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5111 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.5/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.292938 osxphotos-0.60.5/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.5/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1471826 2023-06-24 17:51:29.000000 osxphotos-0.60.5/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.5/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.5/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.5/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51792 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10765 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5124 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.5/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3789 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    91553 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    84853 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46280 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6551 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5335 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.313659 osxphotos-0.60.5/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5388 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10395 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7578 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   149958 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.5/osxphotos/phototables.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.5/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-06-24 17:51:20.000000 osxphotos-0.60.5/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.5/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.5/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21821 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)      696 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/platform.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.5/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.315739 osxphotos-0.60.5/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.5/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.5/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.5/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.5/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.5/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-19 14:34:40.000000 osxphotos-0.60.5/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.5/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.5/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.5/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.317221 osxphotos-0.60.5/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.5/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3245 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2281 2023-06-18 23:22:55.000000 osxphotos-0.60.5/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3445 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.5/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)     2607 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27216 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17290 2023-06-24 17:50:21.000000 osxphotos-0.60.5/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.277108 osxphotos-0.60.5/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6499 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-06-24 17:51:35.000000 osxphotos-0.60.5/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-06-24 17:51:35.337768 osxphotos-0.60.5/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.5/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.336849 osxphotos-0.60.5/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-24 17:51:35.337211 osxphotos-0.60.5/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.5/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.5/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4550 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11011 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4848 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5333 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43711 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54734 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   274105 2023-06-24 17:50:43.000000 osxphotos-0.60.5/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1803 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4575 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2225 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6802 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3675 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.5/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.5/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31269 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6395 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3456 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3056 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.5/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.5/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.5/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.5/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1945 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2750 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2212 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.5/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.5/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9784 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18294 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5913 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.5/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10298 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2485 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155128 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.5/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3633 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4014 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.5/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1271 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.5/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      861 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      931 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.5/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1207 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43641 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50371 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4733 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4872 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3779 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13434 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3080 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_photosalbum_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5795 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.5/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.5/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.5/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.5/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3373 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3695 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7529 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10046 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.5/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3018 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.5/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.5/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.5/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      487 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50020 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.5/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.5/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3158 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2035 2023-06-24 17:50:21.000000 osxphotos-0.60.5/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.5/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.5/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43503 2023-06-18 23:22:55.000000 osxphotos-0.60.5/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.60.4/LICENSE` & `osxphotos-0.60.5/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/PKG-INFO` & `osxphotos-0.60.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.4
+Version: 0.60.5
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.4/README.md` & `osxphotos-0.60.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,22 @@
 * Then type this: `pipx install osxphotos`
 * Now you should be able to run `osxphotos` by typing: `osxphotos`
 
 Once you've installed osxphotos with pipx, to upgrade to the latest version:
 
     pipx upgrade osxphotos
 
+**Note**: When installing other packages with homebrew, homebrew may update the version of Python installed which would then cause any app (including osxphotos) installed with `pipx` to fail. If this happens, the easiest fix is to reinstall osxphotos with:
+
+    pipx reinstall osxphotos
+
+Alternatively, you can reinstall all apps installed with `pipx` with:
+
+    pipx reinstall-all
+
 ### Installation using pip
 
 You can also install directly from [pypi](https://pypi.org/project/osxphotos/):
 
     pip install osxphotos
 
 Once you've installed osxphotos with pip, to upgrade to the latest version:
@@ -2105,15 +2113,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.60.4'
+{osxphotos_version}             The osxphotos version, e.g. '0.60.5'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2592,15 +2600,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.60.4'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.60.5'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
```

### Comparing `osxphotos-0.60.4/README.rst` & `osxphotos-0.60.5/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/__init__.py` & `osxphotos-0.60.5/osxphotos/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 from .photoexporter import ExportOptions, ExportResults, PhotoExporter
 from .photoinfo import PhotoInfo
 from .photosdb import PhotosDB
 from .photosdb._photosdb_process_comments import CommentInfo, LikeInfo
 from .phototables import PhotoTables
 from .phototemplate import PhotoTemplate
 from .placeinfo import PlaceInfo
+from .platform import is_macos
 from .queryoptions import QueryOptions
 from .scoreinfo import ScoreInfo
 from .searchinfo import SearchInfo
-from .utils import is_macos
 
 if is_macos:
     from .photosalbum import PhotosAlbum, PhotosAlbumPhotoScript
 
 # configure logging; every module in osxphotos should use this logger
 logging.basicConfig(
     level=logging.DEBUG,
```

### Comparing `osxphotos-0.60.4/osxphotos/_constants.py` & `osxphotos-0.60.5/osxphotos/_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,14 @@
 
 OSXPHOTOS_URL = "https://github.com/RhetTbull/osxphotos"
 
 # Time delta: add this to Photos times to get unix time
 # Apple Epoch is Jan 1, 2001
 TIME_DELTA = (datetime(2001, 1, 1, 0, 0) - datetime(1970, 1, 1, 0, 0)).total_seconds()
 
-# Unicode format to use for comparing strings
-UNICODE_FORMAT = "NFC"
-
 # which Photos library database versions have been tested
 # Photos 2.0 (10.12.6) == 2622
 # Photos 3.0 (10.13.6) == 3301
 # Photos 4.0 (10.14.5) == 4016
 # Photos 4.0 (10.14.6) == 4025
 # Photos 5.0 (10.15.0) == 6000 or 5001
 _TESTED_DB_VERSIONS = ["6000", "5001", "4025", "4016", "3301", "2622"]
```

### Comparing `osxphotos-0.60.4/osxphotos/adjustmentsinfo.py` & `osxphotos-0.60.5/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/albuminfo.py` & `osxphotos-0.60.5/osxphotos/albuminfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/__init__.py` & `osxphotos-0.60.5/osxphotos/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """cli package for osxphotos"""
 
 import sys
 
 from rich import print
 from rich.traceback import install as install_traceback
 
-from osxphotos.utils import is_macos
 from osxphotos.debug import (
     debug_breakpoint,
     debug_watch,
     get_debug_flags,
     get_debug_options,
     set_debug,
     wrap_function,
 )
+from osxphotos.platform import is_macos
 
 # apply any debug functions
 # need to do this before importing anything else so that the debug functions
 # wrap the right function references
 # if a module does something like "from exiftool import ExifTool" and the user tries
 # to wrap 'osxphotos.exiftool.ExifTool.asdict', the original ExifTool.asdict will be
 # wrapped but the caller will have a reference to the function before it was wrapped
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/about.py` & `osxphotos-0.60.5/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/add_locations.py` & `osxphotos-0.60.5/osxphotos/cli/add_locations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from __future__ import annotations
 
 import datetime
 
 import click
 
 import osxphotos
+from osxphotos.platform import assert_macos
 from osxphotos.queryoptions import IncompatibleQueryOptions, query_options_from_kwargs
-from osxphotos.utils import assert_macos, pluralize
+from osxphotos.utils import pluralize
 
 from .cli_params import QUERY_OPTIONS, THEME_OPTION, TIMESTAMP_OPTION, VERBOSE_OPTION
 from .click_rich_echo import rich_click_echo as echo
 from .click_rich_echo import rich_echo_error as echo_error
 from .param_types import TimeOffset
 from .rich_progress import rich_progress
 from .verbose import get_verbose_console, verbose_print
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/albums.py` & `osxphotos-0.60.5/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/batch_edit.py` & `osxphotos-0.60.5/osxphotos/cli/batch_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import json
 import sys
 
 import click
 
 import osxphotos
 from osxphotos.phototemplate import RenderOptions
+from osxphotos.platform import assert_macos
 from osxphotos.sqlitekvstore import SQLiteKVStore
-from osxphotos.utils import assert_macos
 
 assert_macos()
 
 import photoscript
 
 from .cli_commands import echo, echo_error, selection_command, verbose
 from .kvstore import kvstore
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/cli.py` & `osxphotos-0.60.5/osxphotos/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import io
 import pstats
 
 import click
 
 from osxphotos._constants import PROFILE_SORT_KEYS
 from osxphotos._version import __version__
-from osxphotos.utils import is_macos
+from osxphotos.platform import is_macos
 
 from .about import about
 from .albums import albums
 from .cli_params import DB_OPTION, DEBUG_OPTIONS, JSON_OPTION, VERSION_OPTION
 from .common import OSXPHOTOS_HIDDEN
 from .debug_dump import debug_dump
 from .docs import docs_command
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/cli_commands.py` & `osxphotos-0.60.5/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/cli_params.py` & `osxphotos-0.60.5/osxphotos/cli/cli_params.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Common options & parameters for osxphotos CLI commands"""
 
 
 from __future__ import annotations
 
+import contextlib
 import functools
+from textwrap import dedent
 from typing import Any, Callable
+
 import click
-import contextlib
-from textwrap import dedent
 
-from ..utils import is_macos
+from ..platform import is_macos
 from .common import OSXPHOTOS_HIDDEN, print_version
 from .param_types import *
 
 __all__ = [
     "DB_ARGUMENT",
     "DB_OPTION",
     "DEBUG_OPTIONS",
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.60.5/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/color_themes.py` & `osxphotos-0.60.5/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/common.py` & `osxphotos-0.60.5/osxphotos/cli/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 import click
 from packaging import version
 from xdg import xdg_config_home, xdg_data_home
 
 import osxphotos
 from osxphotos._constants import APP_NAME
 from osxphotos._version import __version__
-from osxphotos.utils import get_latest_version, get_macos_version
+from osxphotos.platform import get_macos_version
+from osxphotos.utils import get_latest_version
 
 # used to show/hide hidden commands
 OSXPHOTOS_HIDDEN = not bool(os.getenv("OSXPHOTOS_SHOW_HIDDEN", default=False))
 
 # used by snap and diff commands
 OSXPHOTOS_SNAPSHOT_DIR = "/private/tmp/osxphotos_snapshots"
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/darkmode.py` & `osxphotos-0.60.5/osxphotos/cli/darkmode.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Detect dark mode on MacOS >= 10.14 or fake it elsewhere"""
 
-from osxphotos.utils import is_macos
-
+from osxphotos.platform import is_macos
 
 if is_macos:
-    import objc
     import Foundation
+    import objc
 
     def theme():
         with objc.autorelease_pool():
             user_defaults = Foundation.NSUserDefaults.standardUserDefaults()
             system_theme = user_defaults.stringForKey_("AppleInterfaceStyle")
             return "dark" if system_theme == "Dark" else "light"
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/debug_dump.py` & `osxphotos-0.60.5/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/docs.py` & `osxphotos-0.60.5/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/dump.py` & `osxphotos-0.60.5/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.60.5/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/export.py` & `osxphotos-0.60.5/osxphotos/cli/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,24 +41,19 @@
 from osxphotos.exiftool import get_exiftool_path
 from osxphotos.export_db import ExportDB, ExportDBInMemory
 from osxphotos.fileutil import FileUtilMacOS, FileUtilNoOp, FileUtilShUtil
 from osxphotos.path_utils import is_valid_filepath, sanitize_filename, sanitize_filepath
 from osxphotos.photoexporter import ExportOptions, ExportResults, PhotoExporter
 from osxphotos.photoinfo import PhotoInfoNone
 from osxphotos.phototemplate import PhotoTemplate, RenderOptions
+from osxphotos.platform import get_macos_version, is_macos
 from osxphotos.queryoptions import load_uuid_from_file, query_options_from_kwargs
+from osxphotos.unicode import normalize_fs_path
 from osxphotos.uti import get_preferred_uti_extension
-from osxphotos.utils import (
-    format_sec_to_hhmmss,
-    get_macos_version,
-    is_macos,
-    normalize_fs_path,
-    pluralize,
-    under_test,
-)
+from osxphotos.utils import format_sec_to_hhmmss, pluralize, under_test
 
 if is_macos:
     from osxmetadata import (
         MDITEM_ATTRIBUTE_DATA,
         MDITEM_ATTRIBUTE_SHORT_NAMES,
         OSXMetaData,
         Tag,
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/exportdb.py` & `osxphotos-0.60.5/osxphotos/cli/exportdb.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,22 +15,22 @@
     OSXPHOTOS_EXPORTDB_VERSION,
     ExportDB,
 )
 from osxphotos.export_db_utils import (
     export_db_backup,
     export_db_check_signatures,
     export_db_get_errors,
+    export_db_get_last_library,
     export_db_get_last_run,
     export_db_get_version,
+    export_db_migrate_photos_library,
     export_db_save_config_to_file,
     export_db_touch_files,
     export_db_update_signatures,
     export_db_vacuum,
-    export_db_migrate_photos_library,
-    export_db_get_last_library,
 )
 from osxphotos.utils import pluralize
 
 from .cli_params import THEME_OPTION, TIMESTAMP_OPTION, VERBOSE_OPTION
 from .click_rich_echo import (
     rich_click_echo,
     rich_echo,
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/grep.py` & `osxphotos-0.60.5/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/help.py` & `osxphotos-0.60.5/osxphotos/cli/help.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 from osxphotos.phototemplate import (
     TEMPLATE_SUBSTITUTIONS,
     TEMPLATE_SUBSTITUTIONS_MULTI_VALUED,
     TEMPLATE_SUBSTITUTIONS_PATHLIB,
     get_template_help,
 )
-from osxphotos.utils import is_macos
+from osxphotos.platform import is_macos
 
 if is_macos:
     from osxmetadata import MDITEM_ATTRIBUTE_DATA, MDITEM_ATTRIBUTE_SHORT_NAMES
 
 from .click_rich_echo import rich_echo_via_pager
 from .color_themes import get_theme
 from .common import OSXPHOTOS_HIDDEN
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/import_cli.py` & `osxphotos-0.60.5/osxphotos/cli/import_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,16 +37,18 @@
     datetime_tz_to_utc,
     datetime_utc_to_local,
 )
 from osxphotos.exiftool import ExifToolCaching, get_exiftool_path
 from osxphotos.photoinfo import PhotoInfoNone
 from osxphotos.photosalbum import PhotosAlbumPhotoScript
 from osxphotos.phototemplate import PhotoTemplate, RenderOptions
+from osxphotos.platform import assert_macos
 from osxphotos.sqlitekvstore import SQLiteKVStore
-from osxphotos.utils import assert_macos, pluralize
+from osxphotos.unicode import normalize_unicode
+from osxphotos.utils import pluralize
 
 assert_macos()
 
 from photoscript import Photo, PhotosLibrary
 
 from .cli_params import THEME_OPTION
 from .click_rich_echo import rich_click_echo, rich_echo_error
@@ -353,19 +355,20 @@
 
 def set_photo_metadata(
     photo: Photo,
     metadata: MetaData,
     merge_keywords: bool,
 ) -> MetaData:
     """Set metadata (title, description, keywords) for a Photo object"""
-    photo.title = metadata.title
-    photo.description = metadata.description
+    photo.title = normalize_unicode(metadata.title)
+    photo.description = normalize_unicode(metadata.description)
     keywords = metadata.keywords.copy()
+    keywords =normalize_unicode(keywords)
     if merge_keywords:
-        if old_keywords := photo.keywords:
+        if old_keywords := normalize_unicode(photo.keywords):
             keywords.extend(old_keywords)
             keywords = list(set(keywords))
     photo.keywords = keywords
     return MetaData(metadata.title, metadata.description, keywords, metadata.location)
 
 
 def set_photo_metadata_from_exiftool(
@@ -416,15 +419,15 @@
             err=True,
         )
         raise click.Abort()
     if title_text:
         verbose(
             f"Setting title of photo [filename]{filepath.name}[/] to '{title_text[0]}'"
         )
-        photo.title = title_text[0]
+        photo.title = normalize_unicode(title_text[0])
         return title_text[0]
     else:
         return ""
 
 
 def set_photo_description(
     photo: Photo,
@@ -444,15 +447,15 @@
             err=True,
         )
         raise click.Abort()
     if description_text:
         verbose(
             f"Setting description of photo [filename]{filepath.name}[/] to '{description_text[0]}'"
         )
-        photo.description = description_text[0]
+        photo.description = normalize_unicode(description_text[0])
         return description_text[0]
     else:
         return ""
 
 
 def set_photo_keywords(
     photo: Photo,
@@ -465,16 +468,17 @@
 ) -> list[str]:
     """Set keywords of photo"""
     keywords = []
     for keyword in keyword_template:
         kw = render_photo_template(filepath, relative_filepath, keyword, exiftool_path)
         keywords.extend(kw)
     if keywords:
+        keywords = normalize_unicode(keywords)
         if merge:
-            if old_keywords := photo.keywords:
+            if old_keywords := normalize_unicode(photo.keywords):
                 keywords.extend(old_keywords)
                 keywords = list(set(keywords))
         verbose(f"Setting keywords of photo [filename]{filepath.name}[/] to {keywords}")
         photo.keywords = keywords
     return keywords
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/info.py` & `osxphotos-0.60.5/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.60.5/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/keywords.py` & `osxphotos-0.60.5/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/kvstore.py` & `osxphotos-0.60.5/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/labels.py` & `osxphotos-0.60.5/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/list.py` & `osxphotos-0.60.5/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/orphans.py` & `osxphotos-0.60.5/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/param_types.py` & `osxphotos-0.60.5/osxphotos/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/persons.py` & `osxphotos-0.60.5/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/photo_inspect.py` & `osxphotos-0.60.5/osxphotos/cli/photo_inspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 from rich.console import Console
 from rich.layout import Layout
 from rich.live import Live
 from rich.panel import Panel
 
 from osxphotos import PhotoInfo, PhotosDB
 from osxphotos._constants import _UNKNOWN_PERSON, search_category_factory
+from osxphotos.platform import assert_macos
 from osxphotos.rich_utils import add_rich_markup_tag
-from osxphotos.utils import assert_macos, dd_to_dms_str
+from osxphotos.utils import dd_to_dms_str
 
 assert_macos()
 
 from applescript import ScriptError
 from photoscript import PhotosLibrary
 
 from osxphotos.text_detection import detect_text as detect_text_in_photo
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/places.py` & `osxphotos-0.60.5/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/print_photo_info.py` & `osxphotos-0.60.5/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/query.py` & `osxphotos-0.60.5/osxphotos/cli/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """query command for osxphotos CLI"""
 
 import sys
+
 import click
 
 import osxphotos
 from osxphotos.cli.click_rich_echo import (
     rich_click_echo,
     set_rich_console,
     set_rich_theme,
 )
 from osxphotos.debug import set_debug
 from osxphotos.phototemplate import RenderOptions
+from osxphotos.platform import assert_macos, is_macos
 from osxphotos.queryoptions import query_options_from_kwargs
-from osxphotos.utils import assert_macos, is_macos
 
 if is_macos:
     from osxphotos.photosalbum import PhotosAlbum
 
 from .cli_params import (
     DB_ARGUMENT,
     DB_OPTION,
@@ -47,14 +48,15 @@
     else []
 )
 
 
 @click.command()
 @DB_OPTION
 @JSON_OPTION
+@click.option("--count", is_flag=True, help="Print count of photos matching query and exit.")
 @QUERY_OPTIONS
 @DELETED_OPTIONS
 @MACOS_OPTIONS
 @click.option(
     "--quiet",
     is_flag=True,
     help="Quiet output; doesn't actually print query results. "
@@ -77,14 +79,15 @@
 @click.pass_context
 def query(
     ctx,
     cli_obj,
     db,
     field,
     json_,
+    count,
     print_template,
     quiet,
     photos_library,
     add_to_album=False,
     **kwargs,
 ):
     """Query the Photos database using 1 or more search options;
@@ -132,14 +135,18 @@
         raise click.BadOptionUsage(
             "query_eval", f"Invalid query-eval CRITERIA: {msg}"
         ) from e
 
     # below needed for to make CliRunner work for testing
     cli_json = cli_obj.json if cli_obj is not None else None
 
+    if count:
+        click.echo(len(photos))
+        return
+
     if add_to_album and photos:
         assert_macos()
 
         album_query = PhotosAlbum(add_to_album, verbose=None)
         photo_len = len(photos)
         photo_word = "photos" if photo_len > 1 else "photo"
         click.echo(
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/repl.py` & `osxphotos-0.60.5/osxphotos/cli/repl.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 from rich import pretty, print
 
 import osxphotos
 from osxphotos._constants import _PHOTOS_4_VERSION
 from osxphotos.cli.click_rich_echo import rich_echo_error as echo_error
 from osxphotos.photoinfo import PhotoInfo
 from osxphotos.photosdb import PhotosDB
+from osxphotos.platform import assert_macos, is_macos
 from osxphotos.pyrepl import embed_repl
 from osxphotos.queryoptions import (
     IncompatibleQueryOptions,
     QueryOptions,
     query_options_from_kwargs,
 )
-from osxphotos.utils import assert_macos, is_macos
 
 if is_macos:
     import photoscript
     from applescript import ScriptError
 
 from .cli_params import DB_ARGUMENT, DB_OPTION, DELETED_OPTIONS, QUERY_OPTIONS
 from .common import get_photos_db
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/report_writer.py` & `osxphotos-0.60.5/osxphotos/cli/report_writer.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/rich_progress.py` & `osxphotos-0.60.5/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/show_command.py` & `osxphotos-0.60.5/osxphotos/cli/show_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import re
 
 import click
 
 from osxphotos._constants import UUID_PATTERN
 from osxphotos.export_db_utils import get_uuid_for_filepath
 from osxphotos.photosdb.photosdb_utils import get_photos_library_version
-from osxphotos.utils import get_last_library_path, assert_macos
+from osxphotos.platform import assert_macos
+from osxphotos.utils import get_last_library_path
 
 assert_macos()
 
 from osxphotos.photoscript_utils import (
     photoscript_object_from_name,
     photoscript_object_from_uuid,
 )
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/snap_diff.py` & `osxphotos-0.60.5/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/sync.py` & `osxphotos-0.60.5/osxphotos/cli/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 import click
 
 from osxphotos import PhotoInfo, PhotosDB, __version__
 from osxphotos.photoinfo import PhotoInfoNone
 from osxphotos.photosalbum import PhotosAlbum
 from osxphotos.photosdb.photosdb_utils import get_db_version
 from osxphotos.phototemplate import PhotoTemplate, RenderOptions
+from osxphotos.platform import assert_macos
 from osxphotos.queryoptions import (
     IncompatibleQueryOptions,
     QueryOptions,
     query_options_from_kwargs,
 )
 from osxphotos.sqlitekvstore import SQLiteKVStore
-from osxphotos.utils import assert_macos, pluralize
+from osxphotos.utils import pluralize
 
 assert_macos()
 
 import photoscript
 
 from .cli_params import (
     DB_OPTION,
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/sync_results.py` & `osxphotos-0.60.5/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/theme.py` & `osxphotos-0.60.5/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/timewarp.py` & `osxphotos-0.60.5/osxphotos/cli/timewarp.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,19 +21,21 @@
     set_photo_date_added,
     set_photo_date_from_filename,
     update_photo_date_time,
     update_photo_from_function,
     update_photo_time_for_new_timezone,
 )
 from osxphotos.phototz import PhotoTimeZone, PhotoTimeZoneUpdater
-from osxphotos.utils import assert_macos, noop, pluralize
+from osxphotos.platform import assert_macos
+from osxphotos.utils import noop, pluralize
 
 assert_macos()
 
 from photoscript import PhotosLibrary
+
 from osxphotos.photosalbum import PhotosAlbumPhotoScript
 
 from .cli_params import THEME_OPTION, TIMESTAMP_OPTION, VERBOSE_OPTION
 from .click_rich_echo import rich_click_echo as echo
 from .click_rich_echo import rich_echo_error as echo_error
 from .color_themes import get_theme
 from .common import OSXPHOTOS_CRASH_LOG
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/tutorial.py` & `osxphotos-0.60.5/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/uuid.py` & `osxphotos-0.60.5/osxphotos/cli/uuid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """uuid command for osxphotos CLI"""
 
 import click
 
-from osxphotos.utils import assert_macos
+from osxphotos.platform import assert_macos
 
 assert_macos()
 
 import photoscript
 
 
 @click.command(name="uuid")
```

### Comparing `osxphotos-0.60.4/osxphotos/cli/verbose.py` & `osxphotos-0.60.5/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/cli/version.py` & `osxphotos-0.60.5/osxphotos/cli/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """about command for osxphotos CLI"""
 
-import click
 import os
+
+import click
+import packaging
+
 from osxphotos._constants import OSXPHOTOS_URL
 from osxphotos._version import __version__
+
 from .common import get_latest_version
-import packaging
 
 
 @click.command(name="version")
 @click.pass_obj
 @click.pass_context
 @click.option(
     "--run",
```

### Comparing `osxphotos-0.60.4/osxphotos/compare_exif.py` & `osxphotos-0.60.5/osxphotos/compare_exif.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,21 @@
 from collections import namedtuple
 from typing import Callable, List, Optional, Tuple
 
 from osxphotos import PhotosDB
 from osxphotos.exiftool import ExifTool
 
 from .datetime_utils import datetime_naive_to_local, datetime_to_new_tz
-from .utils import assert_macos, noop
+from .platform import assert_macos
+from .utils import noop
 
 assert_macos()
 
 from photoscript import Photo
+
 from .exif_datetime_updater import get_exif_date_time_offset
 from .phototz import PhotoTimeZone
 
 ExifDiff = namedtuple(
     "ExifDiff",
     [
         "diff",
```

### Comparing `osxphotos-0.60.4/osxphotos/configoptions.py` & `osxphotos-0.60.5/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/crash_reporter.py` & `osxphotos-0.60.5/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/datetime_formatter.py` & `osxphotos-0.60.5/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/datetime_utils.py` & `osxphotos-0.60.5/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/debug.py` & `osxphotos-0.60.5/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/docs/docs.zip` & `osxphotos-0.60.5/osxphotos/docs/docs.zip`

 * *Files 14% similar despite different names*

#### zipinfo {}

```diff
@@ -1,101 +1,101 @@
-Zip file size: 1460158 bytes, number of entries: 99
+Zip file size: 1471826 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-Jun-18 23:12 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-Jun-24 17:51 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
--rw-r--r--  3.0 unx   324766 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/photoexporter.html
+-rw-r--r--  3.0 unx   324897 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photoexporter.html
 -rw-r--r--  3.0 unx   296439 tx defN 23-May-07 14:38 docs/_modules/osxphotos/phototemplate.html
--rw-r--r--  3.0 unx   201027 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/export_db.html
--rw-r--r--  3.0 unx    14791 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/scoreinfo.html
+-rw-r--r--  3.0 unx   201029 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/export_db.html
+-rw-r--r--  3.0 unx    14791 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
 -rw-r--r--  3.0 unx   284197 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/_photoinfo_export.html
 -rw-r--r--  3.0 unx   195566 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/photoinfo.html
 -rw-r--r--  3.0 unx    33978 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_searchinfo.html
 -rw-r--r--  3.0 unx    17959 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
 -rw-r--r--  3.0 unx    43160 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/searchinfo.html
--rw-r--r--  3.0 unx    52325 tx defN 23-May-07 14:38 docs/_modules/osxphotos/fileutil.html
--rw-r--r--  3.0 unx   313861 tx defN 23-Jun-18 16:54 docs/_modules/osxphotos/photoinfo.html
+-rw-r--r--  3.0 unx    52397 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/fileutil.html
+-rw-r--r--  3.0 unx   313931 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photoinfo.html
 -rw-r--r--  3.0 unx     5599 tx defN 22-Apr-21 04:10 docs/_modules/osxphotos/exifinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-16 03:03 docs/_modules/osxphotos/photosdb/
--rw-r--r--  3.0 unx    29240 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
--rw-r--r--  3.0 unx   526422 tx defN 23-Jun-18 16:54 docs/_modules/osxphotos/photosdb/photosdb.html
--rw-r--r--  3.0 unx    37347 tx defN 23-Jun-18 16:54 docs/_modules/osxphotos/photosalbum.html
--rw-r--r--  3.0 unx    92802 tx defN 23-May-07 14:38 docs/_modules/osxphotos/placeinfo.html
+-rw-r--r--  3.0 unx    29242 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
+-rw-r--r--  3.0 unx   526465 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosdb/photosdb.html
+-rw-r--r--  3.0 unx    39730 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosalbum.html
+-rw-r--r--  3.0 unx    92670 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
 -rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
--rw-r--r--  3.0 unx    61579 tx defN 23-Jun-18 16:54 docs/_modules/osxphotos/queryoptions.html
+-rw-r--r--  3.0 unx    61579 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
--rw-r--r--  3.0 unx    62004 tx defN 23-Jun-18 23:11 docs/_modules/osxphotos/_constants.html
+-rw-r--r--  3.0 unx    61830 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-Jun-18 23:11 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-Jun-24 17:51 docs/_sources/template_help.rst.txt
 -rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
 -rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
 -rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
 -rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
 -rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
 -rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
 -rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
 -rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
 -rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
 -rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
 -rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
 -rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-Jun-18 23:12 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-Jun-24 17:51 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-Jun-18 23:12 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-Jun-24 17:51 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-Jun-18 23:12 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-Jun-24 17:51 docs/_static/language_data.js
 -rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
 -rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
 -rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
 -rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
 -rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-Jun-18 23:12 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-Jun-24 17:51 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-Jun-18 23:12 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-Jun-24 17:51 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   423685 tx defN 23-Jun-18 23:11 docs/cli.html
+-rw-r--r--  3.0 unx   424076 tx defN 23-Jun-24 17:51 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   249535 tx defN 23-Jun-18 23:12 docs/genindex.html
--rw-r--r--  3.0 unx   105318 tx defN 23-Jun-18 23:12 docs/index.html
+-rw-r--r--  3.0 unx   249787 tx defN 23-Jun-24 17:51 docs/genindex.html
+-rw-r--r--  3.0 unx   105318 tx defN 23-Jun-24 17:51 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9610 bx stor 23-Jun-18 23:12 docs/objects.inv
+-rw-r--r--  3.0 unx     9617 bx stor 23-Jun-24 17:51 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-Jun-18 23:11 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-Jun-18 23:11 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-Jun-18 23:12 docs/py-modindex.html
--rw-r--r--  3.0 unx   446001 tx defN 23-Jun-18 23:11 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-Jun-24 17:51 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-Jun-24 17:51 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-Jun-24 17:51 docs/py-modindex.html
+-rw-r--r--  3.0 unx   446001 tx defN 23-Jun-24 17:51 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-Jun-18 23:12 docs/search.html
--rw-r--r--  3.0 unx   113489 tx defN 23-Jun-18 23:12 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-Jun-18 23:12 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-Jun-18 23:12 docs/tutorial.html
-99 files, 6851989 bytes uncompressed, 1441426 bytes compressed:  79.0%
+-rw-r--r--  3.0 unx    10567 tx defN 23-Jun-24 17:51 docs/search.html
+-rw-r--r--  3.0 unx   220745 tx defN 23-Jun-24 17:51 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-Jun-24 17:51 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-Jun-24 17:51 docs/tutorial.html
+99 files, 6962292 bytes uncompressed, 1453094 bytes compressed:  79.1%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.60.4 documentation</title>
+        <title>Overview: module code - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoexporter.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoexporter - osxphotos 0.60.2 documentation</title>
+        <title>osxphotos.photoexporter - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -229,25 +229,25 @@
 <span class="p">)</span>
 <span class="kn">from</span> <span class="nn">._version</span> <span class="kn">import</span> <span class="n">__version__</span>
 <span class="kn">from</span> <span class="nn">.datetime_utils</span> <span class="kn">import</span> <span class="n">datetime_tz_to_utc</span>
 <span class="kn">from</span> <span class="nn">.exiftool</span> <span class="kn">import</span> <span class="n">ExifTool</span><span class="p">,</span> <span class="n">ExifToolCaching</span><span class="p">,</span> <span class="n">exiftool_can_write</span><span class="p">,</span> <span class="n">get_exiftool_path</span>
 <span class="kn">from</span> <span class="nn">.export_db</span> <span class="kn">import</span> <span class="n">ExportDB</span><span class="p">,</span> <span class="n">ExportDBTemp</span>
 <span class="kn">from</span> <span class="nn">.fileutil</span> <span class="kn">import</span> <span class="n">FileUtil</span>
 <span class="kn">from</span> <span class="nn">.phototemplate</span> <span class="kn">import</span> <span class="n">RenderOptions</span>
+<span class="kn">from</span> <span class="nn">.platform</span> <span class="kn">import</span> <span class="n">is_macos</span>
 <span class="kn">from</span> <span class="nn">.rich_utils</span> <span class="kn">import</span> <span class="n">add_rich_markup_tag</span>
+<span class="kn">from</span> <span class="nn">.unicode</span> <span class="kn">import</span> <span class="n">normalize_fs_path</span>
 <span class="kn">from</span> <span class="nn">.uti</span> <span class="kn">import</span> <span class="n">get_preferred_uti_extension</span>
 <span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="p">(</span>
     <span class="n">hexdigest</span><span class="p">,</span>
     <span class="n">increment_filename</span><span class="p">,</span>
     <span class="n">increment_filename_with_count</span><span class="p">,</span>
-    <span class="n">is_macos</span><span class="p">,</span>
     <span class="n">lineno</span><span class="p">,</span>
     <span class="n">list_directory</span><span class="p">,</span>
     <span class="n">lock_filename</span><span class="p">,</span>
-    <span class="n">normalize_fs_path</span><span class="p">,</span>
     <span class="n">unlock_filename</span><span class="p">,</span>
 <span class="p">)</span>
 
 <span class="k">if</span> <span class="n">is_macos</span><span class="p">:</span>
     <span class="kn">import</span> <span class="nn">photoscript</span>
 
     <span class="kn">from</span> <span class="nn">.photokit</span> <span class="kn">import</span> <span class="p">(</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -71,25 +71,25 @@
 from ._version import __version__
 from .datetime_utils import datetime_tz_to_utc
 from .exiftool import ExifTool, ExifToolCaching, exiftool_can_write,
 get_exiftool_path
 from .export_db import ExportDB, ExportDBTemp
 from .fileutil import FileUtil
 from .phototemplate import RenderOptions
+from .platform import is_macos
 from .rich_utils import add_rich_markup_tag
+from .unicode import normalize_fs_path
 from .uti import get_preferred_uti_extension
 from .utils import (
     hexdigest,
     increment_filename,
     increment_filename_with_count,
-    is_macos,
     lineno,
     list_directory,
     lock_filename,
-    normalize_fs_path,
     unlock_filename,
 )
 
 if is_macos:
     import photoscript
 
     from .photokit import (
```

#### docs/_modules/osxphotos/export_db.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.export_db - osxphotos 0.60.2 documentation</title>
+        <title>osxphotos.export_db - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -220,15 +220,15 @@
 <span class="kn">from</span> <span class="nn">tenacity</span> <span class="kn">import</span> <span class="n">retry</span><span class="p">,</span> <span class="n">retry_if_not_exception_type</span><span class="p">,</span> <span class="n">stop_after_attempt</span>
 
 <span class="kn">import</span> <span class="nn">osxphotos</span>
 
 <span class="kn">from</span> <span class="nn">._constants</span> <span class="kn">import</span> <span class="n">OSXPHOTOS_EXPORT_DB</span><span class="p">,</span> <span class="n">SQLITE_CHECK_SAME_THREAD</span>
 <span class="kn">from</span> <span class="nn">._version</span> <span class="kn">import</span> <span class="n">__version__</span>
 <span class="kn">from</span> <span class="nn">.fileutil</span> <span class="kn">import</span> <span class="n">FileUtil</span>
-<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">normalize_fs_path</span>
+<span class="kn">from</span> <span class="nn">.unicode</span> <span class="kn">import</span> <span class="n">normalize_fs_path</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span>
     <span class="s2">&quot;ExportDB&quot;</span><span class="p">,</span>
     <span class="s2">&quot;ExportDBInMemory&quot;</span><span class="p">,</span>
     <span class="s2">&quot;ExportDBTemp&quot;</span><span class="p">,</span>
 <span class="p">]</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -62,15 +62,15 @@
 from tenacity import retry, retry_if_not_exception_type, stop_after_attempt
 
 import osxphotos
 
 from ._constants import OSXPHOTOS_EXPORT_DB, SQLITE_CHECK_SAME_THREAD
 from ._version import __version__
 from .fileutil import FileUtil
-from .utils import normalize_fs_path
+from .unicode import normalize_fs_path
 
 __all__ = [
     "ExportDB",
     "ExportDBInMemory",
     "ExportDBTemp",
 ]
```

#### docs/_modules/osxphotos/scoreinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.scoreinfo - osxphotos 0.60.2 documentation</title>
+        <title>osxphotos.scoreinfo - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -193,15 +193,15 @@
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
           <h1>Source code for osxphotos.scoreinfo</h1><div class="highlight"><pre>
 <span></span><span class="sd">&quot;&quot;&quot; ScoreInfo class to expose computed score info from the library &quot;&quot;&quot;</span>
 
-<span class="kn">from</span> <span class="nn">dataclasses</span> <span class="kn">import</span> <span class="n">dataclass</span><span class="p">,</span> <span class="n">asdict</span>
+<span class="kn">from</span> <span class="nn">dataclasses</span> <span class="kn">import</span> <span class="n">asdict</span><span class="p">,</span> <span class="n">dataclass</span>
 
 <span class="kn">from</span> <span class="nn">._constants</span> <span class="kn">import</span> <span class="n">_PHOTOS_4_VERSION</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;ScoreInfo&quot;</span><span class="p">]</span>
 
 
 <div class="viewcode-block" id="ScoreInfo"><a class="viewcode-back" href="../../reference.html#osxphotos.ScoreInfo">[docs]</a><span class="nd">@dataclass</span><span class="p">(</span><span class="n">frozen</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -34,15 +34,15 @@
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 ****** Source code for osxphotos.scoreinfo ******
 """ ScoreInfo class to expose computed score info from the library """
 
-from dataclasses import dataclass, asdict
+from dataclasses import asdict, dataclass
 
 from ._constants import _PHOTOS_4_VERSION
 
 __all__ = ["ScoreInfo"]
 
 
 [docs]@dataclass(frozen=True)
```

#### docs/_modules/osxphotos/fileutil.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.fileutil - osxphotos 0.60.0 documentation</title>
+        <title>osxphotos.fileutil - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -203,15 +203,16 @@
 <span class="kn">import</span> <span class="nn">stat</span>
 <span class="kn">import</span> <span class="nn">tempfile</span>
 <span class="kn">import</span> <span class="nn">typing</span> <span class="k">as</span> <span class="nn">t</span>
 <span class="kn">from</span> <span class="nn">abc</span> <span class="kn">import</span> <span class="n">ABC</span><span class="p">,</span> <span class="n">abstractmethod</span>
 <span class="kn">from</span> <span class="nn">tempfile</span> <span class="kn">import</span> <span class="n">TemporaryDirectory</span>
 
 <span class="kn">from</span> <span class="nn">.imageconverter</span> <span class="kn">import</span> <span class="n">ImageConverter</span>
-<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">is_macos</span><span class="p">,</span> <span class="n">normalize_fs_path</span>
+<span class="kn">from</span> <span class="nn">.platform</span> <span class="kn">import</span> <span class="n">is_macos</span>
+<span class="kn">from</span> <span class="nn">.unicode</span> <span class="kn">import</span> <span class="n">normalize_fs_path</span>
 
 <span class="k">if</span> <span class="n">is_macos</span><span class="p">:</span>
     <span class="kn">import</span> <span class="nn">Foundation</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;FileUtilABC&quot;</span><span class="p">,</span> <span class="s2">&quot;FileUtilMacOS&quot;</span><span class="p">,</span> <span class="s2">&quot;FileUtilShUtil&quot;</span><span class="p">,</span> <span class="s2">&quot;FileUtil&quot;</span><span class="p">,</span> <span class="s2">&quot;FileUtilNoOp&quot;</span><span class="p">]</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -44,15 +44,16 @@
 import stat
 import tempfile
 import typing as t
 from abc import ABC, abstractmethod
 from tempfile import TemporaryDirectory
 
 from .imageconverter import ImageConverter
-from .utils import is_macos, normalize_fs_path
+from .platform import is_macos
+from .unicode import normalize_fs_path
 
 if is_macos:
     import Foundation
 
 __all__ = ["FileUtilABC", "FileUtilMacOS", "FileUtilShUtil", "FileUtil",
 "FileUtilNoOp"]
```

#### docs/_modules/osxphotos/photoinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoinfo - osxphotos 0.60.3 documentation</title>
+        <title>osxphotos.photoinfo - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -254,19 +254,20 @@
 <span class="kn">from</span> <span class="nn">.exiftool</span> <span class="kn">import</span> <span class="n">ExifToolCaching</span><span class="p">,</span> <span class="n">get_exiftool_path</span>
 <span class="kn">from</span> <span class="nn">.momentinfo</span> <span class="kn">import</span> <span class="n">MomentInfo</span>
 <span class="kn">from</span> <span class="nn">.personinfo</span> <span class="kn">import</span> <span class="n">FaceInfo</span><span class="p">,</span> <span class="n">PersonInfo</span>
 <span class="kn">from</span> <span class="nn">.photoexporter</span> <span class="kn">import</span> <span class="n">ExportOptions</span><span class="p">,</span> <span class="n">PhotoExporter</span>
 <span class="kn">from</span> <span class="nn">.phototables</span> <span class="kn">import</span> <span class="n">PhotoTables</span>
 <span class="kn">from</span> <span class="nn">.phototemplate</span> <span class="kn">import</span> <span class="n">PhotoTemplate</span><span class="p">,</span> <span class="n">RenderOptions</span>
 <span class="kn">from</span> <span class="nn">.placeinfo</span> <span class="kn">import</span> <span class="n">PlaceInfo4</span><span class="p">,</span> <span class="n">PlaceInfo5</span>
+<span class="kn">from</span> <span class="nn">.platform</span> <span class="kn">import</span> <span class="n">assert_macos</span><span class="p">,</span> <span class="n">is_macos</span>
 <span class="kn">from</span> <span class="nn">.query_builder</span> <span class="kn">import</span> <span class="n">get_query</span>
 <span class="kn">from</span> <span class="nn">.scoreinfo</span> <span class="kn">import</span> <span class="n">ScoreInfo</span>
 <span class="kn">from</span> <span class="nn">.searchinfo</span> <span class="kn">import</span> <span class="n">SearchInfo</span>
 <span class="kn">from</span> <span class="nn">.uti</span> <span class="kn">import</span> <span class="n">get_preferred_uti_extension</span><span class="p">,</span> <span class="n">get_uti_for_extension</span>
-<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">_get_resource_loc</span><span class="p">,</span> <span class="n">assert_macos</span><span class="p">,</span> <span class="n">hexdigest</span><span class="p">,</span> <span class="n">is_macos</span><span class="p">,</span> <span class="n">list_directory</span>
+<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">_get_resource_loc</span><span class="p">,</span> <span class="n">hexdigest</span><span class="p">,</span> <span class="n">list_directory</span>
 
 <span class="k">if</span> <span class="n">is_macos</span><span class="p">:</span>
     <span class="kn">from</span> <span class="nn">osxmetadata</span> <span class="kn">import</span> <span class="n">OSXMetaData</span>
 
     <span class="kn">from</span> <span class="nn">.text_detection</span> <span class="kn">import</span> <span class="n">detect_text</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;PhotoInfo&quot;</span><span class="p">,</span> <span class="s2">&quot;PhotoInfoNone&quot;</span><span class="p">,</span> <span class="s2">&quot;frozen_photoinfo_factory&quot;</span><span class="p">]</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -96,20 +96,20 @@
 from .exiftool import ExifToolCaching, get_exiftool_path
 from .momentinfo import MomentInfo
 from .personinfo import FaceInfo, PersonInfo
 from .photoexporter import ExportOptions, PhotoExporter
 from .phototables import PhotoTables
 from .phototemplate import PhotoTemplate, RenderOptions
 from .placeinfo import PlaceInfo4, PlaceInfo5
+from .platform import assert_macos, is_macos
 from .query_builder import get_query
 from .scoreinfo import ScoreInfo
 from .searchinfo import SearchInfo
 from .uti import get_preferred_uti_extension, get_uti_for_extension
-from .utils import _get_resource_loc, assert_macos, hexdigest, is_macos,
-list_directory
+from .utils import _get_resource_loc, hexdigest, list_directory
 
 if is_macos:
     from osxmetadata import OSXMetaData
 
     from .text_detection import detect_text
 
 __all__ = ["PhotoInfo", "PhotoInfoNone", "frozen_photoinfo_factory"]
```

#### docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../../genindex.html" /><link rel="search" title="Search" href="../../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosdb._photosdb_process_comments - osxphotos 0.60.2 documentation</title>
+        <title>osxphotos.photosdb._photosdb_process_comments - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../../index.html"><div class="brand">osxphotos 0.60.2 documentation</div></a>
+      <a href="../../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.2 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -199,16 +199,16 @@
 <span class="sd">    Do not import this module directly &quot;&quot;&quot;</span>
 
 <span class="kn">import</span> <span class="nn">dataclasses</span>
 <span class="kn">import</span> <span class="nn">datetime</span>
 <span class="kn">from</span> <span class="nn">dataclasses</span> <span class="kn">import</span> <span class="n">dataclass</span>
 
 <span class="kn">from</span> <span class="nn">.._constants</span> <span class="kn">import</span> <span class="n">_DB_TABLE_NAMES</span><span class="p">,</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">,</span> <span class="n">TIME_DELTA</span>
-<span class="kn">from</span> <span class="nn">..utils</span> <span class="kn">import</span> <span class="n">normalize_unicode</span>
 <span class="kn">from</span> <span class="nn">..sqlite_utils</span> <span class="kn">import</span> <span class="n">sqlite_open_ro</span>
+<span class="kn">from</span> <span class="nn">..unicode</span> <span class="kn">import</span> <span class="n">normalize_unicode</span>
 
 
 <span class="k">def</span> <span class="nf">_process_comments</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
     <span class="sd">&quot;&quot;&quot;load the comments and likes data from the database</span>
 <span class="sd">    this is a PhotosDB method that should be imported in</span>
 <span class="sd">    the PhotosDB class definition in photosdb.py</span>
 <span class="sd">    &quot;&quot;&quot;</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.2_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -40,16 +40,16 @@
     Do not import this module directly """
 
 import dataclasses
 import datetime
 from dataclasses import dataclass
 
 from .._constants import _DB_TABLE_NAMES, _PHOTOS_4_VERSION, TIME_DELTA
-from ..utils import normalize_unicode
 from ..sqlite_utils import sqlite_open_ro
+from ..unicode import normalize_unicode
 
 
 def _process_comments(self):
     """load the comments and likes data from the database
     this is a PhotosDB method that should be imported in
     the PhotosDB class definition in photosdb.py
     """
```

#### docs/_modules/osxphotos/photosdb/photosdb.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../../genindex.html" /><link rel="search" title="Search" href="../../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.3 documentation</title>
+        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../../index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="../../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -249,25 +249,20 @@
 <span class="kn">from</span> <span class="nn">.._version</span> <span class="kn">import</span> <span class="n">__version__</span>
 <span class="kn">from</span> <span class="nn">..albuminfo</span> <span class="kn">import</span> <span class="n">AlbumInfo</span><span class="p">,</span> <span class="n">FolderInfo</span><span class="p">,</span> <span class="n">ImportInfo</span><span class="p">,</span> <span class="n">ProjectInfo</span>
 <span class="kn">from</span> <span class="nn">..datetime_utils</span> <span class="kn">import</span> <span class="n">datetime_has_tz</span><span class="p">,</span> <span class="n">datetime_naive_to_local</span>
 <span class="kn">from</span> <span class="nn">..fileutil</span> <span class="kn">import</span> <span class="n">FileUtil</span>
 <span class="kn">from</span> <span class="nn">..personinfo</span> <span class="kn">import</span> <span class="n">PersonInfo</span>
 <span class="kn">from</span> <span class="nn">..photoinfo</span> <span class="kn">import</span> <span class="n">PhotoInfo</span>
 <span class="kn">from</span> <span class="nn">..phototemplate</span> <span class="kn">import</span> <span class="n">RenderOptions</span>
+<span class="kn">from</span> <span class="nn">..platform</span> <span class="kn">import</span> <span class="n">get_macos_version</span><span class="p">,</span> <span class="n">is_macos</span>
 <span class="kn">from</span> <span class="nn">..queryoptions</span> <span class="kn">import</span> <span class="n">QueryOptions</span>
 <span class="kn">from</span> <span class="nn">..rich_utils</span> <span class="kn">import</span> <span class="n">add_rich_markup_tag</span>
 <span class="kn">from</span> <span class="nn">..sqlite_utils</span> <span class="kn">import</span> <span class="n">sqlite_db_is_locked</span><span class="p">,</span> <span class="n">sqlite_open_ro</span>
-<span class="kn">from</span> <span class="nn">..utils</span> <span class="kn">import</span> <span class="p">(</span>
-    <span class="n">_check_file_exists</span><span class="p">,</span>
-    <span class="n">is_macos</span><span class="p">,</span>
-    <span class="n">get_macos_version</span><span class="p">,</span>
-    <span class="n">get_last_library_path</span><span class="p">,</span>
-    <span class="n">noop</span><span class="p">,</span>
-    <span class="n">normalize_unicode</span><span class="p">,</span>
-<span class="p">)</span>
+<span class="kn">from</span> <span class="nn">..unicode</span> <span class="kn">import</span> <span class="n">normalize_unicode</span>
+<span class="kn">from</span> <span class="nn">..utils</span> <span class="kn">import</span> <span class="n">_check_file_exists</span><span class="p">,</span> <span class="n">get_last_library_path</span><span class="p">,</span> <span class="n">noop</span>
 <span class="kn">from</span> <span class="nn">.photosdb_utils</span> <span class="kn">import</span> <span class="n">get_db_model_version</span><span class="p">,</span> <span class="n">get_db_version</span>
 
 <span class="k">if</span> <span class="n">is_macos</span><span class="p">:</span>
     <span class="kn">import</span> <span class="nn">photoscript</span>
 
 <span class="n">logger</span> <span class="o">=</span> <span class="n">logging</span><span class="o">.</span><span class="n">getLogger</span><span class="p">(</span><span class="s2">&quot;osxphotos&quot;</span><span class="p">)</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -90,25 +90,20 @@
 from .._version import __version__
 from ..albuminfo import AlbumInfo, FolderInfo, ImportInfo, ProjectInfo
 from ..datetime_utils import datetime_has_tz, datetime_naive_to_local
 from ..fileutil import FileUtil
 from ..personinfo import PersonInfo
 from ..photoinfo import PhotoInfo
 from ..phototemplate import RenderOptions
+from ..platform import get_macos_version, is_macos
 from ..queryoptions import QueryOptions
 from ..rich_utils import add_rich_markup_tag
 from ..sqlite_utils import sqlite_db_is_locked, sqlite_open_ro
-from ..utils import (
-    _check_file_exists,
-    is_macos,
-    get_macos_version,
-    get_last_library_path,
-    noop,
-    normalize_unicode,
-)
+from ..unicode import normalize_unicode
+from ..utils import _check_file_exists, get_last_library_path, noop
 from .photosdb_utils import get_db_model_version, get_db_version
 
 if is_macos:
     import photoscript
 
 logger = logging.getLogger("osxphotos")
```

#### docs/_modules/osxphotos/photosalbum.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosalbum - osxphotos 0.60.3 documentation</title>
+        <title>osxphotos.photosalbum - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -193,42 +193,63 @@
             <i class="icon"><svg><use href="#svg-toc"></use></svg></i>
           </label>
         </div>
         <article role="main">
           <h1>Source code for osxphotos.photosalbum</h1><div class="highlight"><pre>
 <span></span><span class="sd">&quot;&quot;&quot; PhotosAlbum class to create an album in default Photos library and add photos to it &quot;&quot;&quot;</span>
 
+<span class="kn">from</span> <span class="nn">__future__</span> <span class="kn">import</span> <span class="n">annotations</span>
+
+<span class="kn">import</span> <span class="nn">unicodedata</span>
 <span class="kn">from</span> <span class="nn">typing</span> <span class="kn">import</span> <span class="n">List</span><span class="p">,</span> <span class="n">Optional</span>
 
 <span class="kn">from</span> <span class="nn">more_itertools</span> <span class="kn">import</span> <span class="n">chunked</span>
 
 <span class="kn">from</span> <span class="nn">.photoinfo</span> <span class="kn">import</span> <span class="n">PhotoInfo</span>
-<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">assert_macos</span><span class="p">,</span> <span class="n">noop</span><span class="p">,</span> <span class="n">pluralize</span>
+<span class="kn">from</span> <span class="nn">.platform</span> <span class="kn">import</span> <span class="n">assert_macos</span>
+<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">noop</span><span class="p">,</span> <span class="n">pluralize</span>
 
 <span class="n">assert_macos</span><span class="p">()</span>
 
 <span class="kn">import</span> <span class="nn">photoscript</span>
 <span class="kn">from</span> <span class="nn">photoscript</span> <span class="kn">import</span> <span class="n">Album</span><span class="p">,</span> <span class="n">Folder</span><span class="p">,</span> <span class="n">Photo</span><span class="p">,</span> <span class="n">PhotosLibrary</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;PhotosAlbum&quot;</span><span class="p">,</span> <span class="s2">&quot;PhotosAlbumPhotoScript&quot;</span><span class="p">]</span>
 
 
+<span class="k">def</span> <span class="nf">get_unicode_variants</span><span class="p">(</span><span class="n">s</span><span class="p">:</span> <span class="nb">str</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+    <span class="sd">&quot;&quot;&quot;Get all unicode variants of string&quot;&quot;&quot;</span>
+    <span class="n">variants</span> <span class="o">=</span> <span class="p">[]</span>
+    <span class="k">for</span> <span class="n">form</span> <span class="ow">in</span> <span class="p">[</span><span class="s2">&quot;NFC&quot;</span><span class="p">,</span> <span class="s2">&quot;NFD&quot;</span><span class="p">,</span> <span class="s2">&quot;NFKC&quot;</span><span class="p">,</span> <span class="s2">&quot;NFKD&quot;</span><span class="p">]:</span>
+        <span class="n">normalized</span> <span class="o">=</span> <span class="n">unicodedata</span><span class="o">.</span><span class="n">normalize</span><span class="p">(</span><span class="n">form</span><span class="p">,</span> <span class="n">s</span><span class="p">)</span>
+        <span class="n">variants</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">normalized</span><span class="p">)</span>
+    <span class="k">return</span> <span class="n">variants</span>
+
+
 <span class="k">def</span> <span class="nf">folder_by_path</span><span class="p">(</span><span class="n">folders</span><span class="p">:</span> <span class="n">List</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">verbose</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">callable</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">Folder</span><span class="p">:</span>
     <span class="sd">&quot;&quot;&quot;Get (and create if necessary) a Photos Folder by path (passed as list of folder names)&quot;&quot;&quot;</span>
     <span class="n">library</span> <span class="o">=</span> <span class="n">PhotosLibrary</span><span class="p">()</span>
     <span class="n">verbose</span> <span class="o">=</span> <span class="n">verbose</span> <span class="ow">or</span> <span class="n">noop</span>
     <span class="n">top_folder_name</span> <span class="o">=</span> <span class="n">folders</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
-    <span class="n">top_folder</span> <span class="o">=</span> <span class="n">library</span><span class="o">.</span><span class="n">folder</span><span class="p">(</span><span class="n">top_folder_name</span><span class="p">,</span> <span class="n">top_level</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-    <span class="k">if</span> <span class="ow">not</span> <span class="n">top_folder</span><span class="p">:</span>
+
+    <span class="k">for</span> <span class="n">folder_variant</span> <span class="ow">in</span> <span class="n">get_unicode_variants</span><span class="p">(</span><span class="n">top_folder_name</span><span class="p">):</span>
+        <span class="n">top_folder</span> <span class="o">=</span> <span class="n">library</span><span class="o">.</span><span class="n">folder</span><span class="p">(</span><span class="n">folder_variant</span><span class="p">,</span> <span class="n">top_level</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+        <span class="k">if</span> <span class="n">top_folder</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+            <span class="k">break</span>
+    <span class="k">else</span><span class="p">:</span>
         <span class="n">verbose</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating folder &#39;</span><span class="si">{</span><span class="n">top_folder_name</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
         <span class="n">top_folder</span> <span class="o">=</span> <span class="n">library</span><span class="o">.</span><span class="n">create_folder</span><span class="p">(</span><span class="n">top_folder_name</span><span class="p">)</span>
+
     <span class="n">current_folder</span> <span class="o">=</span> <span class="n">top_folder</span>
     <span class="k">for</span> <span class="n">folder_name</span> <span class="ow">in</span> <span class="n">folders</span><span class="p">:</span>
-        <span class="n">folder</span> <span class="o">=</span> <span class="n">current_folder</span><span class="o">.</span><span class="n">folder</span><span class="p">(</span><span class="n">folder_name</span><span class="p">)</span>
-        <span class="k">if</span> <span class="ow">not</span> <span class="n">folder</span><span class="p">:</span>
+        <span class="k">for</span> <span class="n">folder_variant</span> <span class="ow">in</span> <span class="n">get_unicode_variants</span><span class="p">(</span><span class="n">folder_name</span><span class="p">):</span>
+            <span class="n">folder</span> <span class="o">=</span> <span class="n">current_folder</span><span class="o">.</span><span class="n">folder</span><span class="p">(</span><span class="n">folder_variant</span><span class="p">)</span>
+            <span class="k">if</span> <span class="n">folder</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+                <span class="k">break</span>
+        <span class="k">else</span><span class="p">:</span>
             <span class="n">verbose</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating folder &#39;</span><span class="si">{</span><span class="n">folder_name</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
             <span class="n">folder</span> <span class="o">=</span> <span class="n">current_folder</span><span class="o">.</span><span class="n">create_folder</span><span class="p">(</span><span class="n">folder_name</span><span class="p">)</span>
         <span class="n">current_folder</span> <span class="o">=</span> <span class="n">folder</span>
     <span class="k">return</span> <span class="n">current_folder</span>
 
 
 <span class="k">def</span> <span class="nf">album_by_path</span><span class="p">(</span>
@@ -237,23 +258,32 @@
     <span class="sd">&quot;&quot;&quot;Get (and create if necessary) a Photos Album by path (pass as list of folders, album name)&quot;&quot;&quot;</span>
     <span class="n">library</span> <span class="o">=</span> <span class="n">PhotosLibrary</span><span class="p">()</span>
     <span class="n">verbose</span> <span class="o">=</span> <span class="n">verbose</span> <span class="ow">or</span> <span class="n">noop</span>
     <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">folders_album</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">1</span><span class="p">:</span>
         <span class="c1"># have folders</span>
         <span class="n">album_name</span> <span class="o">=</span> <span class="n">folders_album</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
         <span class="n">folder</span> <span class="o">=</span> <span class="n">folder_by_path</span><span class="p">(</span><span class="n">folders_album</span><span class="p">,</span> <span class="n">verbose</span><span class="p">)</span>
-        <span class="n">album</span> <span class="o">=</span> <span class="n">folder</span><span class="o">.</span><span class="n">album</span><span class="p">(</span><span class="n">album_name</span><span class="p">)</span>
-        <span class="k">if</span> <span class="n">album</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="k">for</span> <span class="n">album_variant</span> <span class="ow">in</span> <span class="n">get_unicode_variants</span><span class="p">(</span><span class="n">album_name</span><span class="p">):</span>
+            <span class="c1"># Get album if it exists</span>
+            <span class="c1"># need to check every unicode variant to avoid creating duplicate albums with same visual representation (#1085)</span>
+            <span class="n">album</span> <span class="o">=</span> <span class="n">folder</span><span class="o">.</span><span class="n">album</span><span class="p">(</span><span class="n">album_variant</span><span class="p">)</span>
+            <span class="k">if</span> <span class="n">album</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+                <span class="k">break</span>
+        <span class="k">else</span><span class="p">:</span>
             <span class="n">verbose</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating album &#39;</span><span class="si">{</span><span class="n">album_name</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
             <span class="n">album</span> <span class="o">=</span> <span class="n">folder</span><span class="o">.</span><span class="n">create_album</span><span class="p">(</span><span class="n">album_name</span><span class="p">)</span>
     <span class="k">else</span><span class="p">:</span>
         <span class="c1"># only have album name</span>
         <span class="n">album_name</span> <span class="o">=</span> <span class="n">folders_album</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-        <span class="n">album</span> <span class="o">=</span> <span class="n">library</span><span class="o">.</span><span class="n">album</span><span class="p">(</span><span class="n">album_name</span><span class="p">,</span> <span class="n">top_level</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
-        <span class="k">if</span> <span class="n">album</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
+        <span class="k">for</span> <span class="n">album_variant</span> <span class="ow">in</span> <span class="n">get_unicode_variants</span><span class="p">(</span><span class="n">album_name</span><span class="p">):</span>
+            <span class="n">album</span> <span class="o">=</span> <span class="n">library</span><span class="o">.</span><span class="n">album</span><span class="p">(</span><span class="n">album_variant</span><span class="p">,</span> <span class="n">top_level</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
+            <span class="k">if</span> <span class="n">album</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span><span class="p">:</span>
+                <span class="k">break</span>
+        <span class="k">else</span><span class="p">:</span>
+            <span class="c1"># album doesn&#39;t exist, create it</span>
             <span class="n">verbose</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Creating album &#39;</span><span class="si">{</span><span class="n">album_name</span><span class="si">}</span><span class="s2">&#39;&quot;</span><span class="p">)</span>
             <span class="n">album</span> <span class="o">=</span> <span class="n">library</span><span class="o">.</span><span class="n">create_album</span><span class="p">(</span><span class="n">album_name</span><span class="p">)</span>
 
     <span class="k">return</span> <span class="n">album</span>
 
 
 <div class="viewcode-block" id="PhotosAlbum"><a class="viewcode-back" href="../../reference.html#osxphotos.PhotosAlbum">[docs]</a><span class="k">class</span> <span class="nc">PhotosAlbum</span><span class="p">:</span>
@@ -294,21 +324,18 @@
 
     <span class="k">def</span> <span class="nf">add_list</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">photo_list</span><span class="p">:</span> <span class="n">List</span><span class="p">[</span><span class="n">PhotoInfo</span><span class="p">]):</span>
         <span class="n">photos</span> <span class="o">=</span> <span class="p">[]</span>
         <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photo_list</span><span class="p">:</span>
             <span class="k">try</span><span class="p">:</span>
                 <span class="n">photos</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">photoscript</span><span class="o">.</span><span class="n">Photo</span><span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">uuid</span><span class="p">))</span>
             <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Error creating Photo object for photo </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_format_uuid</span><span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">uuid</span><span class="p">)</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">verbose</span><span class="p">(</span>
                     <span class="sa">f</span><span class="s2">&quot;Error creating Photo object for photo </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_format_uuid</span><span class="p">(</span><span class="n">p</span><span class="o">.</span><span class="n">uuid</span><span class="p">)</span><span class="si">}</span><span class="s2">: </span><span class="si">{</span><span class="n">e</span><span class="si">}</span><span class="s2">&quot;</span>
                 <span class="p">)</span>
-        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;photos: </span><span class="si">{</span><span class="n">photos</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
         <span class="k">for</span> <span class="n">photolist</span> <span class="ow">in</span> <span class="n">chunked</span><span class="p">(</span><span class="n">photos</span><span class="p">,</span> <span class="mi">10</span><span class="p">):</span>
-            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;photolist: </span><span class="si">{</span><span class="n">photolist</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">album</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="n">photolist</span><span class="p">)</span>
         <span class="n">photo_len</span> <span class="o">=</span> <span class="nb">len</span><span class="p">(</span><span class="n">photo_list</span><span class="p">)</span>
         <span class="bp">self</span><span class="o">.</span><span class="n">verbose</span><span class="p">(</span>
             <span class="sa">f</span><span class="s2">&quot;Added </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_format_num</span><span class="p">(</span><span class="n">photo_len</span><span class="p">)</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">pluralize</span><span class="p">(</span><span class="n">photo_len</span><span class="p">,</span> <span class="s1">&#39;photo&#39;</span><span class="p">,</span> <span class="s1">&#39;photos&#39;</span><span class="p">)</span><span class="si">}</span><span class="s2"> to album </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">_format_album</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">name</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
         <span class="p">)</span>
 
     <span class="k">def</span> <span class="nf">photos</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -35,44 +35,65 @@
 
 Toggle table of contents sidebar
 
 ****** Source code for osxphotos.photosalbum ******
 """ PhotosAlbum class to create an album in default Photos library and add
 photos to it """
 
+from __future__ import annotations
+
+import unicodedata
 from typing import List, Optional
 
 from more_itertools import chunked
 
 from .photoinfo import PhotoInfo
-from .utils import assert_macos, noop, pluralize
+from .platform import assert_macos
+from .utils import noop, pluralize
 
 assert_macos()
 
 import photoscript
 from photoscript import Album, Folder, Photo, PhotosLibrary
 
 __all__ = ["PhotosAlbum", "PhotosAlbumPhotoScript"]
 
 
+def get_unicode_variants(s: str) -> list[str]:
+    """Get all unicode variants of string"""
+    variants = []
+    for form in ["NFC", "NFD", "NFKC", "NFKD"]:
+        normalized = unicodedata.normalize(form, s)
+        variants.append(normalized)
+    return variants
+
+
 def folder_by_path(folders: List[str], verbose: Optional[callable] = None) -
 > Folder:
     """Get (and create if necessary) a Photos Folder by path (passed as list of
 folder names)"""
     library = PhotosLibrary()
     verbose = verbose or noop
     top_folder_name = folders.pop(0)
-    top_folder = library.folder(top_folder_name, top_level=True)
-    if not top_folder:
+
+    for folder_variant in get_unicode_variants(top_folder_name):
+        top_folder = library.folder(folder_variant, top_level=True)
+        if top_folder is not None:
+            break
+    else:
         verbose(f"Creating folder '{top_folder_name}'")
         top_folder = library.create_folder(top_folder_name)
+
     current_folder = top_folder
     for folder_name in folders:
-        folder = current_folder.folder(folder_name)
-        if not folder:
+        for folder_variant in get_unicode_variants(folder_name):
+            folder = current_folder.folder(folder_variant)
+            if folder is not None:
+                break
+        else:
             verbose(f"Creating folder '{folder_name}'")
             folder = current_folder.create_folder(folder_name)
         current_folder = folder
     return current_folder
 
 
 def album_by_path(
@@ -82,23 +103,33 @@
 folders, album name)"""
     library = PhotosLibrary()
     verbose = verbose or noop
     if len(folders_album) > 1:
         # have folders
         album_name = folders_album.pop()
         folder = folder_by_path(folders_album, verbose)
-        album = folder.album(album_name)
-        if album is None:
+        for album_variant in get_unicode_variants(album_name):
+            # Get album if it exists
+            # need to check every unicode variant to avoid creating duplicate
+albums with same visual representation (#1085)
+            album = folder.album(album_variant)
+            if album is not None:
+                break
+        else:
             verbose(f"Creating album '{album_name}'")
             album = folder.create_album(album_name)
     else:
         # only have album name
         album_name = folders_album[0]
-        album = library.album(album_name, top_level=True)
-        if album is None:
+        for album_variant in get_unicode_variants(album_name):
+            album = library.album(album_variant, top_level=True)
+            if album is not None:
+                break
+        else:
+            # album doesn't exist, create it
             verbose(f"Creating album '{album_name}'")
             album = library.create_album(album_name)
 
     return album
 
 
 [docs]class PhotosAlbum:
@@ -142,23 +173,19 @@
 
     def add_list(self, photo_list: List[PhotoInfo]):
         photos = []
         for p in photo_list:
             try:
                 photos.append(photoscript.Photo(p.uuid))
             except Exception as e:
-                print(f"Error creating Photo object for photo
-{self._format_uuid(p.uuid)}: {e}")
                 self.verbose(
                     f"Error creating Photo object for photo {self._format_uuid
 (p.uuid)}: {e}"
                 )
-        print(f"photos: {photos}")
         for photolist in chunked(photos, 10):
-            print(f"photolist: {photolist}")
             self.album.add(photolist)
         photo_len = len(photo_list)
         self.verbose(
             f"Added {self._format_num(photo_len)} {pluralize(photo_len,
 'photo', 'photos')} to album {self._format_album(self.name)}"
         )
```

#### docs/_modules/osxphotos/placeinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.placeinfo - osxphotos 0.60.0 documentation</title>
+        <title>osxphotos.placeinfo - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.0 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.0 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -204,16 +204,15 @@
 <span class="sd">&quot;&quot;&quot;</span>
 <span class="kn">from</span> <span class="nn">abc</span> <span class="kn">import</span> <span class="n">ABC</span><span class="p">,</span> <span class="n">abstractmethod</span>
 <span class="kn">from</span> <span class="nn">collections</span> <span class="kn">import</span> <span class="n">namedtuple</span>  <span class="c1"># pylint: disable=syntax-error</span>
 
 <span class="kn">import</span> <span class="nn">yaml</span>
 <span class="kn">from</span> <span class="nn">bpylist2</span> <span class="kn">import</span> <span class="n">archiver</span>
 
-<span class="kn">from</span> <span class="nn">._constants</span> <span class="kn">import</span> <span class="n">UNICODE_FORMAT</span>
-<span class="kn">from</span> <span class="nn">.utils</span> <span class="kn">import</span> <span class="n">normalize_unicode</span>
+<span class="kn">from</span> <span class="nn">.unicode</span> <span class="kn">import</span> <span class="n">normalize_unicode</span>
 
 <span class="n">__all__</span> <span class="o">=</span> <span class="p">[</span>
     <span class="s2">&quot;PLRevGeoLocationInfo&quot;</span><span class="p">,</span>
     <span class="s2">&quot;PLRevGeoMapItem&quot;</span><span class="p">,</span>
     <span class="s2">&quot;PLRevGeoMapItemAdditionalPlaceInfo&quot;</span><span class="p">,</span>
     <span class="s2">&quot;CNPostalAddress&quot;</span><span class="p">,</span>
     <span class="s2">&quot;PlaceInfo&quot;</span><span class="p">,</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.0_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -45,16 +45,15 @@
 """
 from abc import ABC, abstractmethod
 from collections import namedtuple  # pylint: disable=syntax-error
 
 import yaml
 from bpylist2 import archiver
 
-from ._constants import UNICODE_FORMAT
-from .utils import normalize_unicode
+from .unicode import normalize_unicode
 
 __all__ = [
     "PLRevGeoLocationInfo",
     "PLRevGeoMapItem",
     "PLRevGeoMapItemAdditionalPlaceInfo",
     "CNPostalAddress",
     "PlaceInfo",
```

#### docs/_modules/osxphotos/queryoptions.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.queryoptions - osxphotos 0.60.3 documentation</title>
+        <title>osxphotos.queryoptions - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/_constants.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos._constants - osxphotos 0.60.4 documentation</title>
+        <title>osxphotos._constants - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -211,17 +211,14 @@
 
 <span class="n">OSXPHOTOS_URL</span> <span class="o">=</span> <span class="s2">&quot;https://github.com/RhetTbull/osxphotos&quot;</span>
 
 <span class="c1"># Time delta: add this to Photos times to get unix time</span>
 <span class="c1"># Apple Epoch is Jan 1, 2001</span>
 <span class="n">TIME_DELTA</span> <span class="o">=</span> <span class="p">(</span><span class="n">datetime</span><span class="p">(</span><span class="mi">2001</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span> <span class="o">-</span> <span class="n">datetime</span><span class="p">(</span><span class="mi">1970</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">))</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
 
-<span class="c1"># Unicode format to use for comparing strings</span>
-<span class="n">UNICODE_FORMAT</span> <span class="o">=</span> <span class="s2">&quot;NFC&quot;</span>
-
 <span class="c1"># which Photos library database versions have been tested</span>
 <span class="c1"># Photos 2.0 (10.12.6) == 2622</span>
 <span class="c1"># Photos 3.0 (10.13.6) == 3301</span>
 <span class="c1"># Photos 4.0 (10.14.5) == 4016</span>
 <span class="c1"># Photos 4.0 (10.14.6) == 4025</span>
 <span class="c1"># Photos 5.0 (10.15.0) == 6000 or 5001</span>
 <span class="n">_TESTED_DB_VERSIONS</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;6000&quot;</span><span class="p">,</span> <span class="s2">&quot;5001&quot;</span><span class="p">,</span> <span class="s2">&quot;4025&quot;</span><span class="p">,</span> <span class="s2">&quot;4016&quot;</span><span class="p">,</span> <span class="s2">&quot;3301&quot;</span><span class="p">,</span> <span class="s2">&quot;2622&quot;</span><span class="p">]</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -53,17 +53,14 @@
 OSXPHOTOS_URL = "https://github.com/RhetTbull/osxphotos"
 
 # Time delta: add this to Photos times to get unix time
 # Apple Epoch is Jan 1, 2001
 TIME_DELTA = (datetime(2001, 1, 1, 0, 0) - datetime(1970, 1, 1, 0,
 0)).total_seconds()
 
-# Unicode format to use for comparing strings
-UNICODE_FORMAT = "NFC"
-
 # which Photos library database versions have been tested
 # Photos 2.0 (10.12.6) == 2622
 # Photos 3.0 (10.13.6) == 3301
 # Photos 4.0 (10.14.5) == 4016
 # Photos 4.0 (10.14.6) == 4025
 # Photos 5.0 (10.15.0) == 6000 or 5001
 _TESTED_DB_VERSIONS = ["6000", "5001", "4025", "4016", "3301", "2622"]
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.60.4'
+     - The osxphotos version, e.g. '0.60.5'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.60.4',
+    VERSION: '0.60.5',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.4 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -2826,14 +2826,20 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-query-json">
 <span class="sig-name descname"><span class="pre">--json</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-query-json" title="Permalink to this definition">#</a></dt>
 <dd><p>Print output in JSON format.</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-query-count">
+<span class="sig-name descname"><span class="pre">--count</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-query-count" title="Permalink to this definition">#</a></dt>
+<dd><p>Print count of photos matching query and exit.</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-query-keyword">
 <span class="sig-name descname"><span class="pre">--keyword</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;KEYWORD&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-query-keyword" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos with keyword KEYWORD. If more than one keyword, treated as “OR”, e.g. find photos matching any keyword</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-query-no-keyword">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -1619,14 +1619,16 @@
 Options
   --library, --db <PHOTOS_LIBRARY_PATH>#
       Specify path to Photos library. If not provided, will attempt to find the
       library to use in the following order: 1. last opened library, 2. system
       library, 3. ~/Pictures/Photos Library.photoslibrary
   --json#
       Print output in JSON format.
+  --count#
+      Print count of photos matching query and exit.
   --keyword <KEYWORD>#
       Search for photos with keyword KEYWORD. If more than one keyword, treated
       as âORâ, e.g. find photos matching any keyword
   --no-keyword#
       Search for photos with no keyword.
   --person <PERSON>#
       Search for photos with person PERSON. If more than one person, treated as
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.4 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.5 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -422,14 +422,21 @@
     --convert-to-jpeg
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-export-convert-to-jpeg">osxphotos-export command line option</a>
 </li>
         </ul></li>
         <li>
+    --count
+
+        <ul>
+          <li><a href="cli.html#cmdoption-osxphotos-query-count">osxphotos-query command line option</a>
+</li>
+        </ul></li>
+        <li>
     --current-name
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-export-current-name">osxphotos-export command line option</a>
 </li>
         </ul></li>
         <li>
@@ -4759,14 +4766,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-album">--album</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-burst">--burst</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-cloudasset">--cloudasset</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-count">--count</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-query-library">--db</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-deleted">--deleted</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-deleted-only">--deleted-only</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-description">--description</a>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -42,894 +42,897 @@
 
 ***** Symbols *****
     * --add-exported-to-album
           o osxphotos-export_command
             line_option
     * --add-missing-to-album
           o osxphotos-export_command
-            line_option                     * --not-hdr
-    * --add-skipped-to-album                      o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-    * --add-to-album                                line_option
-          o osxphotos-query_command               o osxphotos-query_command
+            line_option
+    * --add-skipped-to-album
+          o osxphotos-export_command        * --not-hdr
+            line_option                           o osxphotos-add-locations
+    * --add-to-album                                command_line_option
+          o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-timewarp_command            o osxphotos-repl_command_line
-            line_option                             option
-    * --added-after                               o osxphotos-sync_command_line
+          o osxphotos-timewarp_command            o osxphotos-query_command
+            line_option                             line_option
+    * --added-after                               o osxphotos-repl_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-hidden
-          o osxphotos-export_command              o osxphotos-add-locations
+            command_line_option                   o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * --not-hidden
+          o osxphotos-query_command               o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
+          o osxphotos-repl_command_line           o osxphotos-export_command
             option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-repl_command_line
-            option                                  option
-    * --added-before                              o osxphotos-sync_command_line
+          o osxphotos-sync_command_line           o osxphotos-query_command
+            option                                  line_option
+    * --added-before                              o osxphotos-repl_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-in-album
-          o osxphotos-export_command              o osxphotos-add-locations
+            command_line_option                   o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * --not-in-album
+          o osxphotos-query_command               o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
+          o osxphotos-repl_command_line           o osxphotos-export_command
             option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-repl_command_line
-            option                                  option
-    * --added-in-last                             o osxphotos-sync_command_line
+          o osxphotos-sync_command_line           o osxphotos-query_command
+            option                                  line_option
+    * --added-in-last                             o osxphotos-repl_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-incloud
-          o osxphotos-export_command              o osxphotos-add-locations
+            command_line_option                   o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * --not-incloud
+          o osxphotos-query_command               o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-repl_command_line           o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-sync_command_line           o osxphotos-query_command
+            option                                  line_option
+    * --album                                     o osxphotos-repl_command_line
+          o osxphotos-add-locations                 option
+            command_line_option                   o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * --not-live
+          o osxphotos-import_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
-    * --album                                     o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option             * --not-live
+    * --album-keyword                             o osxphotos-sync_command_line
+          o osxphotos-exiftool_command              option
+            line_option                     * --not-missing
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-import_command              o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-query_command               o osxphotos-query_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-repl_command_line
-            option                                  option
-          o osxphotos-sync_command_line           o osxphotos-sync_command_line
-            option                                  option
-    * --album-keyword                       * --not-missing
-          o osxphotos-exiftool_command            o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
-            line_option                             line_option
-    * --alt-copy                                  o osxphotos-query_command
+    * --alt-copy                                  o osxphotos-export_command
           o osxphotos-export_command                line_option
-            line_option                           o osxphotos-repl_command_line
-    * --append                                      option
-          o osxphotos-exiftool_command            o osxphotos-sync_command_line
+            line_option                           o osxphotos-query_command
+    * --append                                      line_option
+          o osxphotos-exiftool_command            o osxphotos-repl_command_line
+            line_option                             option
+          o osxphotos-export_command              o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-export_command        * --not-panorama
+          o osxphotos-exportdb_command      * --not-panorama
             line_option                           o osxphotos-add-locations
-          o osxphotos-exportdb_command              command_line_option
+          o osxphotos-import_command                command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-import_command                line_option
-            line_option                           o osxphotos-query_command
           o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-repl_command_line
-    * --burst                                       option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
+            option                                o osxphotos-query_command
+    * --burst                                       line_option
+          o osxphotos-add-locations               o osxphotos-repl_command_line
             command_line_option                     option
-          o osxphotos-export_command        * --not-portrait
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-query_command         * --not-portrait
             line_option                           o osxphotos-add-locations
-          o osxphotos-query_command                 command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-query_command
+          o osxphotos-repl_command_line             command_line_option
+            option                                o osxphotos-export_command
           o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-repl_command_line
-    * --check-signatures                            option
-          o osxphotos-exportdb_command            o osxphotos-sync_command_line
-            line_option                             option
-    * --check-templates                     * --not-reference
-          o osxphotos-import_command              o osxphotos-add-locations
-            line_option                             command_line_option
-    * --cleanup                                   o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-query_command
-    * --clear-location                              line_option
-          o osxphotos-import_command              o osxphotos-repl_command_line
+            option                                o osxphotos-query_command
+    * --check-signatures                            line_option
+          o osxphotos-exportdb_command            o osxphotos-repl_command_line
             line_option                             option
-    * --clear-metadata                            o osxphotos-sync_command_line
+    * --check-templates                           o osxphotos-sync_command_line
           o osxphotos-import_command                option
-            line_option                     * --not-saved-to-library
-    * --clone                                     o osxphotos-add-locations
-          o osxphotos-theme_command                 command_line_option
+            line_option                     * --not-reference
+    * --cleanup                                   o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
-    * --cloudasset                                  line_option
-          o osxphotos-add-locations               o osxphotos-query_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-query_command               o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-repl_command_line     * --not-screenshot
-            option                                o osxphotos-add-locations
-          o osxphotos-sync_command_line             command_line_option
-            option                                o osxphotos-export_command
-    * --compare-exif                                line_option
-          o osxphotos-timewarp_command            o osxphotos-query_command
+    * --clear-location                              line_option
+          o osxphotos-import_command              o osxphotos-query_command
             line_option                             line_option
-    * --config                                    o osxphotos-repl_command_line
-          o osxphotos-theme_command                 option
+    * --clear-metadata                            o osxphotos-repl_command_line
+          o osxphotos-import_command                option
             line_option                           o osxphotos-sync_command_line
-    * --config-only                                 option
-          o osxphotos-export_command        * --not-selfie
+    * --clone                                       option
+          o osxphotos-theme_command         * --not-saved-to-library
             line_option                           o osxphotos-add-locations
-    * --convert-to-jpeg                             command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
-            line_option                             line_option
-    * --current-name                              o osxphotos-query_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-repl_command_line
-    * --date                                        option
-          o osxphotos-timewarp_command            o osxphotos-sync_command_line
-            line_option                             option
-    * --date-added                          * --not-shared
-          o osxphotos-timewarp_command            o osxphotos-add-locations
-            line_option                             command_line_option
-    * --date-added-from-photo                     o osxphotos-export_command
-          o osxphotos-timewarp_command              line_option
-            line_option                           o osxphotos-query_command
-    * --date-delta                                  line_option
-          o osxphotos-timewarp_command            o osxphotos-repl_command_line
-            line_option                             option
-    * --db                                  * --not-slow-mo
-          o osxphotos_command_line                o osxphotos-add-locations
-            option                                  command_line_option
-          o osxphotos-albums_command              o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-batch-edit                  o osxphotos-query_command
+    * --cloudasset                                  command_line_option
+          o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
-          o osxphotos-diff_command_line           o osxphotos-repl_command_line
-            option                                  option
-          o osxphotos-dump_command_line           o osxphotos-sync_command_line
-            option                                  option
-          o osxphotos-exiftool_command      * --not-syndicated
-            line_option                           o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-info_command_line             line_option
-            option                                o osxphotos-query_command
-          o osxphotos-inspect_command               line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-keywords_command              option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-labels_command                option
-            line_option                     * --not-time-lapse
-          o osxphotos-orphans_command             o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-persons_command             o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-places_command              o osxphotos-query_command
+          o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
           o osxphotos-query_command               o osxphotos-repl_command_line
             line_option                             option
           o osxphotos-repl_command_line           o osxphotos-sync_command_line
             option                                  option
-          o osxphotos-show_command_line     * --only-movies
+          o osxphotos-sync_command_line     * --not-screenshot
             option                                o osxphotos-add-locations
-          o osxphotos-snap_command_line             command_line_option
-            option                                o osxphotos-export_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-query_command
-    * --db-config                                   line_option
-          o osxphotos-exiftool_command            o osxphotos-repl_command_line
-            line_option                             option
-    * --default                                   o osxphotos-sync_command_line
-          o osxphotos-theme_command                 option
-            line_option                     * --only-new
-    * --delete                                    o osxphotos-export_command
+    * --compare-exif                                command_line_option
+          o osxphotos-timewarp_command            o osxphotos-export_command
+            line_option                             line_option
+    * --config                                    o osxphotos-query_command
           o osxphotos-theme_command                 line_option
-            line_option                     * --only-photos
-    * --delete-file                               o osxphotos-add-locations
-          o osxphotos-exportdb_command              command_line_option
+            line_option                           o osxphotos-repl_command_line
+    * --config-only                                 option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+    * --convert-to-jpeg                     * --not-selfie
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+    * --count                                     o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-query_command
+    * --current-name                                line_option
+          o osxphotos-export_command              o osxphotos-repl_command_line
+            line_option                             option
+    * --date                                      o osxphotos-sync_command_line
+          o osxphotos-timewarp_command              option
+            line_option                     * --not-shared
+    * --date-added                                o osxphotos-add-locations
+          o osxphotos-timewarp_command              command_line_option
             line_option                           o osxphotos-export_command
-    * --delete-uuid                                 line_option
-          o osxphotos-exportdb_command            o osxphotos-query_command
+    * --date-added-from-photo                       line_option
+          o osxphotos-timewarp_command            o osxphotos-query_command
             line_option                             line_option
-    * --deleted                                   o osxphotos-repl_command_line
-          o osxphotos-dump_command_line             option
+    * --date-delta                                o osxphotos-repl_command_line
+          o osxphotos-timewarp_command              option
+            line_option                     * --not-slow-mo
+    * --db                                        o osxphotos-add-locations
+          o osxphotos_command_line                  command_line_option
+            option                                o osxphotos-export_command
+          o osxphotos-albums_command                line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-batch-edit                    line_option
+            command_line_option                   o osxphotos-repl_command_line
+          o osxphotos-diff_command_line             option
             option                                o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --original-suffix
-          o osxphotos-query_command               o osxphotos-export_command
+          o osxphotos-dump_command_line             option
+            option                          * --not-syndicated
+          o osxphotos-exiftool_command            o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * --overwrite
-            option                                o osxphotos-export_command
-    * --deleted-only                                line_option
-          o osxphotos-dump_command_line     * --panorama
-            option                                o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
+          o osxphotos-info_command_line           o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-inspect_command             o osxphotos-repl_command_line
+            line_option                             option
+          o osxphotos-keywords_command            o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-labels_command        * --not-time-lapse
+            line_option                           o osxphotos-add-locations
+          o osxphotos-orphans_command               command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
+          o osxphotos-persons_command               line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-repl_command_line
-    * --description                                 option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-batch-edit            * --parse-date
-            command_line_option                   o osxphotos-import_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-timewarp_command
-          o osxphotos-import_command                line_option
-            line_option                     * --person
-          o osxphotos-query_command               o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-repl_command_line           o osxphotos-export_command
+          o osxphotos-places_command                line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-query_command                 option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-repl_command_line             option
+            option                          * --only-movies
+          o osxphotos-show_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-snap_command_line           o osxphotos-export_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-query_command
             option                                  line_option
-    * --description-template                      o osxphotos-repl_command_line
+    * --db-config                                 o osxphotos-repl_command_line
           o osxphotos-exiftool_command              option
             line_option                           o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --person-keyword
-    * --detect-text                               o osxphotos-exiftool_command
-          o osxphotos-inspect_command               line_option
+    * --default                                     option
+          o osxphotos-theme_command         * --only-new
             line_option                           o osxphotos-export_command
-    * --directory                                   line_option
-          o osxphotos-export_command        * --place
-            line_option                           o osxphotos-add-locations
-    * --download-missing                            command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
-            line_option                             line_option
-    * --dry-run                                   o osxphotos-query_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-repl_command_line
-          o osxphotos-batch-edit                    option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-exiftool_command              option
-            line_option                     * --plain
-          o osxphotos-export_command              o osxphotos-timewarp_command
-            line_option                             line_option
-          o osxphotos-exportdb_command      * --portrait
+    * --delete                                      line_option
+          o osxphotos-theme_command         * --only-photos
             line_option                           o osxphotos-add-locations
-          o osxphotos-sync_command_line             command_line_option
-            option                                o osxphotos-export_command
-    * --dup-check                                   line_option
-          o osxphotos-import_command              o osxphotos-query_command
-            line_option                             line_option
-    * --duplicate                                 o osxphotos-repl_command_line
-          o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --post-command
-          o osxphotos-query_command               o osxphotos-export_command
+    * --delete-file                                 command_line_option
+          o osxphotos-exportdb_command            o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * --post-function
-            option                                o osxphotos-export_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-import_command
-    * --edit                                        line_option
-          o osxphotos-theme_command         * --preview
-            line_option                           o osxphotos-export_command
-    * --edited                                      line_option
-          o osxphotos-add-locations               o osxphotos-theme_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * --preview-if-missing
+    * --delete-uuid                               o osxphotos-query_command
+          o osxphotos-exportdb_command              line_option
+            line_option                           o osxphotos-repl_command_line
+    * --deleted                                     option
+          o osxphotos-dump_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-export_command        * --original-suffix
             line_option                           o osxphotos-export_command
           o osxphotos-query_command                 line_option
-            line_option                     * --preview-suffix
+            line_option                     * --overwrite
           o osxphotos-repl_command_line           o osxphotos-export_command
             option                                  line_option
-          o osxphotos-sync_command_line     * --print
-            option                                o osxphotos-dump_command_line
-    * --edited-suffix                               option
+    * --deleted-only                        * --panorama
+          o osxphotos-dump_command_line           o osxphotos-add-locations
+            option                                  command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-    * --emacs                                     o osxphotos-query_command
-          o osxphotos-repl_command_line             line_option
-            option                          * --pull-exif
-    * --errors                                    o osxphotos-timewarp_command
-          o osxphotos-exportdb_command              line_option
-            line_option                     * --push-exif
-    * --exif                                      o osxphotos-timewarp_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * --query-eval
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-          o osxphotos-query_command               o osxphotos-export_command
+          o osxphotos-query_command               o osxphotos-query_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-query_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-repl_command_line
+          o osxphotos-repl_command_line           o osxphotos-repl_command_line
             option                                  option
-    * --exiftool                                  o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * --query-function
-          o osxphotos-import_command              o osxphotos-add-locations
-            line_option                             command_line_option
-    * --exiftool-merge-keywords                   o osxphotos-export_command
-          o osxphotos-exiftool_command              line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-repl_command_line
-    * --exiftool-merge-persons                      option
+    * --description                               o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * --parse-date
+          o osxphotos-batch-edit                  o osxphotos-import_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-timewarp_command
+            line_option                             line_option
+          o osxphotos-import_command        * --person
+            line_option                           o osxphotos-add-locations
+          o osxphotos-query_command                 command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-query_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-repl_command_line
+    * --description-template                        option
           o osxphotos-exiftool_command            o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-export_command        * --quiet
+          o osxphotos-export_command        * --person-keyword
+            line_option                           o osxphotos-exiftool_command
+    * --detect-text                                 line_option
+          o osxphotos-inspect_command             o osxphotos-export_command
+            line_option                             line_option
+    * --directory                           * --place
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+    * --download-missing                          o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
-    * --exiftool-option                             line_option
-          o osxphotos-exiftool_command      * --ramdb
-            line_option                           o osxphotos-export_command
+    * --dry-run                                     line_option
+          o osxphotos-add-locations               o osxphotos-repl_command_line
+            command_line_option                     option
+          o osxphotos-batch-edit                  o osxphotos-sync_command_line
+            command_line_option                     option
+          o osxphotos-exiftool_command      * --plain
+            line_option                           o osxphotos-timewarp_command
           o osxphotos-export_command                line_option
-            line_option                     * --raw-output
-    * --exiftool-path                             o osxphotos-diff_command_line
-          o osxphotos-exiftool_command              option
-            line_option                     * --regex
-          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                     * --portrait
+          o osxphotos-exportdb_command            o osxphotos-add-locations
             line_option                             command_line_option
-          o osxphotos-import_command              o osxphotos-export_command
+          o osxphotos-sync_command_line           o osxphotos-export_command
+            option                                  line_option
+    * --dup-check                                 o osxphotos-query_command
+          o osxphotos-import_command                line_option
+            line_option                           o osxphotos-repl_command_line
+    * --duplicate                                   option
+          o osxphotos-add-locations               o osxphotos-sync_command_line
+            command_line_option                     option
+          o osxphotos-export_command        * --post-command
+            line_option                           o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                     * --post-function
+          o osxphotos-repl_command_line           o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-sync_command_line           o osxphotos-import_command
+            option                                  line_option
+    * --edit                                * --preview
+          o osxphotos-theme_command               o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-timewarp_command            o osxphotos-query_command
+    * --edited                                    o osxphotos-theme_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * --preview-if-missing
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-    * --export                                    o osxphotos-repl_command_line
-          o osxphotos-orphans_command               option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-sync_command_line             option
-            option                          * --relative-to
-    * --export-as-hardlink                        o osxphotos-import_command
+          o osxphotos-query_command         * --preview-suffix
+            line_option                           o osxphotos-export_command
+          o osxphotos-repl_command_line             line_option
+            option                          * --print
+          o osxphotos-sync_command_line           o osxphotos-dump_command_line
+            option                                  option
+    * --edited-suffix                             o osxphotos-export_command
           o osxphotos-export_command                line_option
-            line_option                     * --replace-keywords
-    * --export-by-date                            o osxphotos-batch-edit
+            line_option                           o osxphotos-query_command
+    * --emacs                                       line_option
+          o osxphotos-repl_command_line     * --pull-exif
+            option                                o osxphotos-timewarp_command
+    * --errors                                      line_option
+          o osxphotos-exportdb_command      * --push-exif
+            line_option                           o osxphotos-timewarp_command
+    * --exif                                        line_option
+          o osxphotos-add-locations         * --query-eval
+            command_line_option                   o osxphotos-add-locations
           o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-exiftool_command
-    * --export-dir                                  line_option
-          o osxphotos-exportdb_command            o osxphotos-export_command
-            line_option                             line_option
-    * --exportdb                            * --report
-          o osxphotos-exiftool_command            o osxphotos-exiftool_command
+            line_option                           o osxphotos-export_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-repl_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-sync_command_line
+    * --exiftool                                    option
+          o osxphotos-export_command        * --query-function
+            line_option                           o osxphotos-add-locations
+          o osxphotos-import_command                command_line_option
+            line_option                           o osxphotos-export_command
+    * --exiftool-merge-keywords                     line_option
+          o osxphotos-exiftool_command            o osxphotos-query_command
             line_option                             line_option
-          o osxphotos-export_command              o osxphotos-export_command
+          o osxphotos-export_command              o osxphotos-repl_command_line
+            line_option                             option
+    * --exiftool-merge-persons                    o osxphotos-sync_command_line
+          o osxphotos-exiftool_command              option
+            line_option                     * --quiet
+          o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
-    * --external-edit                             o osxphotos-exportdb_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-import_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-query_command                 option
-            line_option                     * --resume
-          o osxphotos-repl_command_line           o osxphotos-import_command
-            option                                  line_option
-          o osxphotos-sync_command_line     * --retry
-            option                                o osxphotos-export_command
-    * --favorite                                    line_option
-          o osxphotos-add-locations         * --run
-            command_line_option                   o osxphotos-version_command
-          o osxphotos-export_command                line_option
-            line_option                     * --save-config
-          o osxphotos-query_command               o osxphotos-exiftool_command
+    * --exiftool-option                     * --ramdb
+          o osxphotos-exiftool_command            o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-exportdb_command
-            option                                  line_option
-    * --favorite-rating                     * --saved-to-library
-          o osxphotos-export_command              o osxphotos-add-locations
-            line_option                             command_line_option
-    * --field                                     o osxphotos-export_command
-          o osxphotos-dump_command_line             line_option
-            option                                o osxphotos-query_command
-          o osxphotos-query_command                 line_option
+          o osxphotos-export_command        * --raw-output
+            line_option                           o osxphotos-diff_command_line
+    * --exiftool-path                               option
+          o osxphotos-exiftool_command      * --regex
+            line_option                           o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+          o osxphotos-import_command                line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-timewarp_command              line_option
             line_option                           o osxphotos-repl_command_line
-    * --filename                                    option
-          o osxphotos-export_command              o osxphotos-sync_command_line
+    * --export                                      option
+          o osxphotos-orphans_command             o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-uuid_command_line     * --screenshot
-            option                                o osxphotos-add-locations
-    * --finder-tag-keywords                         command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
+          o osxphotos-sync_command_line     * --relative-to
+            option                                o osxphotos-import_command
+    * --export-as-hardlink                          line_option
+          o osxphotos-export_command        * --replace-keywords
+            line_option                           o osxphotos-batch-edit
+    * --export-by-date                              command_line_option
+          o osxphotos-export_command              o osxphotos-exiftool_command
             line_option                             line_option
-    * --finder-tag-template                       o osxphotos-query_command
+    * --export-dir                                o osxphotos-export_command
+          o osxphotos-exportdb_command              line_option
+            line_option                     * --report
+    * --exportdb                                  o osxphotos-exiftool_command
+          o osxphotos-exiftool_command              line_option
+            line_option                           o osxphotos-export_command
           o osxphotos-export_command                line_option
-            line_option                           o osxphotos-repl_command_line
-    * --folder                                      option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * --selected
-            line_option                           o osxphotos-add-locations
-          o osxphotos-query_command                 command_line_option
+            line_option                           o osxphotos-exportdb_command
+    * --external-edit                               line_option
+          o osxphotos-add-locations               o osxphotos-import_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-query_command         * --resume
+            line_option                           o osxphotos-import_command
+          o osxphotos-repl_command_line             line_option
+            option                          * --retry
+          o osxphotos-sync_command_line           o osxphotos-export_command
+            option                                  line_option
+    * --favorite                            * --run
+          o osxphotos-add-locations               o osxphotos-version_command
+            command_line_option                     line_option
+          o osxphotos-export_command        * --save-config
+            line_option                           o osxphotos-exiftool_command
+          o osxphotos-query_command                 line_option
             line_option                           o osxphotos-export_command
           o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-query_command
+            option                                o osxphotos-exportdb_command
           o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-repl_command_line
-    * --force                                       option
-          o osxphotos-timewarp_command            o osxphotos-sync_command_line
+            option                          * --saved-to-library
+    * --favorite-rating                           o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+    * --field                                       line_option
+          o osxphotos-dump_command_line           o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-query_command               o osxphotos-repl_command_line
             line_option                             option
-    * --force-update                        * --selfie
+    * --filename                                  o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * --screenshot
+          o osxphotos-uuid_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+    * --finder-tag-keywords                       o osxphotos-export_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-query_command
+    * --finder-tag-template                         line_option
+          o osxphotos-export_command              o osxphotos-repl_command_line
+            line_option                             option
+    * --folder                                    o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * --selected
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
-    * --from-date                                 o osxphotos-export_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-query_command
+          o osxphotos-query_command               o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-sync_command_line           o osxphotos-repl_command_line
+            option                                  option
+    * --force                                     o osxphotos-sync_command_line
+          o osxphotos-timewarp_command              option
+            line_option                     * --selfie
+    * --force-update                              o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+    * --from-date                                   line_option
+          o osxphotos-add-locations               o osxphotos-query_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-repl_command_line
+            line_option                             option
+          o osxphotos-query_command               o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-repl_command_line     * --set
+            option                                o osxphotos-sync_command_line
+          o osxphotos-sync_command_line             option
+            option                          * --shared
+    * --from-time                                 o osxphotos-add-locations
+          o osxphotos-add-locations                 command_line_option
+            command_line_option                   o osxphotos-export_command
           o osxphotos-export_command                line_option
+            line_option                           o osxphotos-query_command
+          o osxphotos-query_command                 line_option
             line_option                           o osxphotos-repl_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-sync_command_line
           o osxphotos-repl_command_line             option
-            option                          * --set
-          o osxphotos-sync_command_line           o osxphotos-sync_command_line
-            option                                  option
-    * --from-time                           * --shared
-          o osxphotos-add-locations               o osxphotos-add-locations
-            command_line_option                     command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
+            option                          * --sidecar
+          o osxphotos-sync_command_line           o osxphotos-export_command
+            option                                  line_option
+    * --function                            * --sidecar-drop-ext
+          o osxphotos-timewarp_command            o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-query_command
+    * --glob                                * --skip-bursts
+          o osxphotos-import_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-repl_command_line
-            option                                  option
-          o osxphotos-sync_command_line     * --sidecar
-            option                                o osxphotos-export_command
-    * --function                                    line_option
-          o osxphotos-timewarp_command      * --sidecar-drop-ext
-            line_option                           o osxphotos-export_command
-    * --glob                                        line_option
-          o osxphotos-import_command        * --skip-bursts
+    * --has-comment                         * --skip-edited
+          o osxphotos-add-locations               o osxphotos-export_command
+            command_line_option                     line_option
+          o osxphotos-export_command        * --skip-live
             line_option                           o osxphotos-export_command
-    * --has-comment                                 line_option
-          o osxphotos-add-locations         * --skip-edited
+          o osxphotos-query_command                 line_option
+            line_option                     * --skip-original-if-edited
+          o osxphotos-repl_command_line           o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-sync_command_line     * --skip-raw
+            option                                o osxphotos-export_command
+    * --has-likes                                   line_option
+          o osxphotos-add-locations         * --skip-uuid
             command_line_option                   o osxphotos-export_command
           o osxphotos-export_command                line_option
-            line_option                     * --skip-live
+            line_option                     * --skip-uuid-from-file
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-repl_command_line     * --skip-original-if-edited
+          o osxphotos-repl_command_line     * --slow-mo
+            option                                o osxphotos-add-locations
+          o osxphotos-sync_command_line             command_line_option
             option                                o osxphotos-export_command
+    * --has-raw                                     line_option
+          o osxphotos-add-locations               o osxphotos-query_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-repl_command_line
+            line_option                             option
+          o osxphotos-query_command               o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-repl_command_line     * --split-folder
+            option                                o osxphotos-import_command
           o osxphotos-sync_command_line             line_option
-            option                          * --skip-raw
-    * --has-likes                                 o osxphotos-export_command
+            option                          * --sql
+    * --hdr                                       o osxphotos-exportdb_command
           o osxphotos-add-locations                 line_option
-            command_line_option             * --skip-uuid
+            command_line_option             * --strip
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command         * --skip-uuid-from-file
-            line_option                           o osxphotos-export_command
+          o osxphotos-query_command         * --style
+            line_option                           o osxphotos-diff_command_line
+          o osxphotos-repl_command_line             option
+            option                          * --syndicated
+          o osxphotos-sync_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+    * --help                                      o osxphotos-export_command
+          o osxphotos-run_command_line              line_option
+            option                                o osxphotos-query_command
+    * --hidden                                      line_option
+          o osxphotos-add-locations               o osxphotos-repl_command_line
+            command_line_option                     option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-query_command         * --template
+            line_option                           o osxphotos-inspect_command
           o osxphotos-repl_command_line             line_option
-            option                          * --slow-mo
+            option                          * --theme
           o osxphotos-sync_command_line           o osxphotos-add-locations
             option                                  command_line_option
-    * --has-raw                                   o osxphotos-export_command
-          o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-query_command
+    * --ignore-case                               o osxphotos-batch-edit
+          o osxphotos-add-locations                 command_line_option
+            command_line_option                   o osxphotos-exiftool_command
           o osxphotos-export_command                line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-repl_command_line             option
-            option                          * --split-folder
-          o osxphotos-sync_command_line           o osxphotos-import_command
-            option                                  line_option
-    * --hdr                                 * --sql
-          o osxphotos-add-locations               o osxphotos-exportdb_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * --strip
             line_option                           o osxphotos-export_command
           o osxphotos-query_command                 line_option
-            line_option                     * --style
+            line_option                           o osxphotos-exportdb_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-import_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-inspect_command
+    * --ignore-date-modified                        line_option
+          o osxphotos-exiftool_command            o osxphotos-orphans_command
+            line_option                             line_option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+    * --ignore-signature                          o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option
+            line_option                     * --time
+    * --import                                    o osxphotos-timewarp_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --time-delta
+    * --in-album                                  o osxphotos-timewarp_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * --time-lapse
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-query_command               o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-sync_command_line           o osxphotos-repl_command_line
+            option                                  option
+    * --incloud                                   o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * --timestamp
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-query_command               o osxphotos-batch-edit
+            line_option                             command_line_option
           o osxphotos-repl_command_line           o osxphotos-diff_command_line
             option                                  option
-          o osxphotos-sync_command_line     * --syndicated
-            option                                o osxphotos-add-locations
-    * --help                                        command_line_option
-          o osxphotos-run_command_line            o osxphotos-export_command
+          o osxphotos-sync_command_line           o osxphotos-exiftool_command
             option                                  line_option
-    * --hidden                                    o osxphotos-query_command
+    * --info                                      o osxphotos-export_command
+          o osxphotos-exportdb_command              line_option
+            line_option                           o osxphotos-exportdb_command
+    * --inspect                                     line_option
+          o osxphotos-timewarp_command            o osxphotos-import_command
+            line_option                             line_option
+    * --is-reference                              o osxphotos-orphans_command
           o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-repl_command_line
+            command_line_option                   o osxphotos-sync_command_line
           o osxphotos-export_command                option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-query_command                 option
-            line_option                     * --template
-          o osxphotos-repl_command_line           o osxphotos-inspect_command
+            line_option                           o osxphotos-timewarp_command
+          o osxphotos-query_command                 line_option, [1]
+            line_option                     * --timezone
+          o osxphotos-repl_command_line           o osxphotos-timewarp_command
             option                                  line_option
-          o osxphotos-sync_command_line     * --theme
+          o osxphotos-sync_command_line     * --title
             option                                o osxphotos-add-locations
-    * --ignore-case                                 command_line_option
-          o osxphotos-add-locations               o osxphotos-batch-edit
-            command_line_option                     command_line_option
-          o osxphotos-export_command              o osxphotos-exiftool_command
+    * --jpeg-ext                                    command_line_option
+          o osxphotos-export_command              o osxphotos-batch-edit
+            line_option                             command_line_option
+    * --jpeg-quality                              o osxphotos-export_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-import_command
+    * --json                                        line_option
+          o osxphotos_command_line                o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-albums_command              o osxphotos-repl_command_line
+            line_option                             option
+          o osxphotos-dump_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-info_command_line     * --tmpdir
+            option                                o osxphotos-export_command
+          o osxphotos-keywords_command              line_option
+            line_option                     * --to-date
+          o osxphotos-labels_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-list_command_line           o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-persons_command             o osxphotos-query_command
             line_option                             line_option
+          o osxphotos-places_command              o osxphotos-repl_command_line
+            line_option                             option
+          o osxphotos-query_command               o osxphotos-sync_command_line
+            line_option                             option
+    * --keep                                * --to-time
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+    * --keyword                                   o osxphotos-export_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-query_command
+          o osxphotos-batch-edit                    line_option
+            command_line_option                   o osxphotos-repl_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-import_command                option
+            line_option                     * --touch-file
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-exportdb_command
             option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-import_command
-            option                                  line_option
-    * --ignore-date-modified                      o osxphotos-inspect_command
-          o osxphotos-exiftool_command              line_option
-            line_option                           o osxphotos-orphans_command
-          o osxphotos-export_command                line_option
+          o osxphotos-sync_command_line     * --undo
+            option                                o osxphotos-batch-edit
+    * --keyword-template                            command_line_option
+          o osxphotos-exiftool_command      * --unmatched
             line_option                           o osxphotos-sync_command_line
-    * --ignore-signature                            option
-          o osxphotos-export_command              o osxphotos-timewarp_command
+          o osxphotos-export_command                option
+            line_option                     * --update
+    * --label                                     o osxphotos-export_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * --update-errors
+          o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
-    * --import                              * --time
-          o osxphotos-sync_command_line           o osxphotos-timewarp_command
+          o osxphotos-query_command         * --update-signatures
+            line_option                           o osxphotos-exportdb_command
+          o osxphotos-repl_command_line             line_option
+            option                          * --upgrade
+          o osxphotos-sync_command_line           o osxphotos-install_command
             option                                  line_option
-    * --in-album                            * --time-delta
-          o osxphotos-add-locations               o osxphotos-timewarp_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * --time-lapse
+    * --last-errors                         * --use-file-time
+          o osxphotos-exportdb_command            o osxphotos-timewarp_command
+            line_option                             line_option
+    * --last-run                            * --use-photokit
+          o osxphotos-exportdb_command            o osxphotos-export_command
+            line_option                             line_option
+    * --library                             * --use-photos-export
+          o osxphotos_command_line                o osxphotos-export_command
+            option                                  line_option
+          o osxphotos-albums_command        * --uti
             line_option                           o osxphotos-add-locations
-          o osxphotos-query_command                 command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
+          o osxphotos-batch-edit                    command_line_option
+            command_line_option                   o osxphotos-export_command
+          o osxphotos-diff_command_line             line_option
             option                                o osxphotos-query_command
-          o osxphotos-sync_command_line             line_option
+          o osxphotos-dump_command_line             line_option
             option                                o osxphotos-repl_command_line
-    * --incloud                                     option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * --timestamp
-            line_option                           o osxphotos-add-locations
-          o osxphotos-query_command                 command_line_option
-            line_option                           o osxphotos-batch-edit
-          o osxphotos-repl_command_line             command_line_option
-            option                                o osxphotos-diff_command_line
-          o osxphotos-sync_command_line             option
-            option                                o osxphotos-exiftool_command
-    * --info                                        line_option
-          o osxphotos-exportdb_command            o osxphotos-export_command
-            line_option                             line_option
-    * --inspect                                   o osxphotos-exportdb_command
-          o osxphotos-timewarp_command              line_option
-            line_option                           o osxphotos-import_command
-    * --is-reference                                line_option
-          o osxphotos-add-locations               o osxphotos-orphans_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-query_command               o osxphotos-timewarp_command
-            line_option                             line_option, [1]
-          o osxphotos-repl_command_line     * --timezone
-            option                                o osxphotos-timewarp_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --title
-    * --jpeg-ext                                  o osxphotos-add-locations
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-batch-edit
-    * --jpeg-quality                                command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
+          o osxphotos-exiftool_command              option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * --uuid
+          o osxphotos-info_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+          o osxphotos-inspect_command             o osxphotos-export_command
             line_option                             line_option
-    * --json                                      o osxphotos-import_command
-          o osxphotos_command_line                  line_option
-            option                                o osxphotos-query_command
-          o osxphotos-albums_command                line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-dump_command_line             option
-            option                                o osxphotos-sync_command_line
-          o osxphotos-info_command_line             option
-            option                          * --tmpdir
-          o osxphotos-keywords_command            o osxphotos-export_command
+          o osxphotos-keywords_command            o osxphotos-query_command
             line_option                             line_option
-          o osxphotos-labels_command        * --to-date
-            line_option                           o osxphotos-add-locations
-          o osxphotos-list_command_line             command_line_option
-            option                                o osxphotos-export_command
-          o osxphotos-persons_command               line_option
-            line_option                           o osxphotos-query_command
-          o osxphotos-places_command                line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-sync_command_line
-    * --keep                                        option
-          o osxphotos-export_command        * --to-time
-            line_option                           o osxphotos-add-locations
-    * --keyword                                     command_line_option
-          o osxphotos-add-locations               o osxphotos-export_command
-            command_line_option                     line_option
-          o osxphotos-batch-edit                  o osxphotos-query_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-repl_command_line
+          o osxphotos-labels_command              o osxphotos-repl_command_line
             line_option                             option
-          o osxphotos-import_command              o osxphotos-sync_command_line
+          o osxphotos-orphans_command             o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-query_command         * --touch-file
-            line_option                           o osxphotos-export_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-exportdb_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --undo
-    * --keyword-template                          o osxphotos-batch-edit
-          o osxphotos-exiftool_command              command_line_option
-            line_option                     * --unmatched
-          o osxphotos-export_command              o osxphotos-sync_command_line
-            line_option                             option
-    * --label                               * --update
-          o osxphotos-add-locations               o osxphotos-export_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * --update-errors
-            line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                     * --update-signatures
-          o osxphotos-repl_command_line           o osxphotos-exportdb_command
+          o osxphotos-persons_command       * --uuid-files
+            line_option                           o osxphotos-exportdb_command
+          o osxphotos-places_command                line_option
+            line_option                     * --uuid-from-file
+          o osxphotos-query_command               o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-repl_command_line           o osxphotos-export_command
             option                                  line_option
-          o osxphotos-sync_command_line     * --upgrade
-            option                                o osxphotos-install_command
-    * --last-errors                                 line_option
-          o osxphotos-exportdb_command      * --use-file-time
-            line_option                           o osxphotos-timewarp_command
-    * --last-run                                    line_option
-          o osxphotos-exportdb_command      * --use-photokit
-            line_option                           o osxphotos-export_command
-    * --library                                     line_option
-          o osxphotos_command_line          * --use-photos-export
-            option                                o osxphotos-export_command
-          o osxphotos-albums_command                line_option
-            line_option                     * --uti
-          o osxphotos-batch-edit                  o osxphotos-add-locations
+          o osxphotos-show_command_line           o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-snap_command_line           o osxphotos-repl_command_line
+            option                                  option
+          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-timewarp_command      * --uuid-info
+            line_option                           o osxphotos-exportdb_command
+    * --limit                                       line_option
+          o osxphotos-export_command        * --vacuum
+            line_option                           o osxphotos-exportdb_command
+    * --list                                        line_option
+          o osxphotos-theme_command         * --verbose
+            line_option                           o osxphotos-add-locations
+    * --live                                        command_line_option
+          o osxphotos-add-locations               o osxphotos-batch-edit
             command_line_option                     command_line_option
-          o osxphotos-diff_command_line           o osxphotos-export_command
+          o osxphotos-export_command              o osxphotos-diff_command_line
+            line_option                             option
+          o osxphotos-query_command               o osxphotos-exiftool_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-export_command
             option                                  line_option
-          o osxphotos-dump_command_line           o osxphotos-query_command
+          o osxphotos-sync_command_line           o osxphotos-exportdb_command
             option                                  line_option
-          o osxphotos-exiftool_command            o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-export_command              o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-info_command_line     * --uuid
+    * --load-config                               o osxphotos-import_command
+          o osxphotos-exiftool_command              line_option
+            line_option                           o osxphotos-orphans_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-sync_command_line
+    * --location                                    option
+          o osxphotos-add-locations               o osxphotos-timewarp_command
+            command_line_option                     line_option
+          o osxphotos-batch-edit            * --version
+            command_line_option                   o osxphotos_command_line
+          o osxphotos-export_command                option
+            line_option                           o osxphotos-exportdb_command
+          o osxphotos-import_command                line_option
+            line_option                     * --walk
+          o osxphotos-query_command               o osxphotos-import_command
+            line_option                             line_option
+          o osxphotos-repl_command_line     * --window
             option                                o osxphotos-add-locations
-          o osxphotos-inspect_command               command_line_option
-            line_option                           o osxphotos-export_command
-          o osxphotos-keywords_command              line_option
+          o osxphotos-sync_command_line             command_line_option
+            option                          * --xattr-template
+    * --match-time                                o osxphotos-export_command
+          o osxphotos-timewarp_command              line_option
+            line_option                     * --year
+    * --max-size                                  o osxphotos-add-locations
+          o osxphotos-add-locations                 command_line_option
+            command_line_option                   o osxphotos-export_command
+          o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
-          o osxphotos-labels_command                line_option
+          o osxphotos-query_command                 line_option
             line_option                           o osxphotos-repl_command_line
-          o osxphotos-orphans_command               option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-persons_command               option
-            line_option                     * --uuid-files
-          o osxphotos-places_command              o osxphotos-exportdb_command
-            line_option                             line_option
-          o osxphotos-query_command         * --uuid-from-file
-            line_option                           o osxphotos-add-locations
-          o osxphotos-repl_command_line             command_line_option
-            option                                o osxphotos-export_command
-          o osxphotos-show_command_line             line_option
-            option                                o osxphotos-query_command
-          o osxphotos-snap_command_line             line_option
-            option                                o osxphotos-repl_command_line
-          o osxphotos-sync_command_line             option
+          o osxphotos-repl_command_line             option
             option                                o osxphotos-sync_command_line
-          o osxphotos-timewarp_command              option
-            line_option                     * --uuid-info
-    * --limit                                     o osxphotos-exportdb_command
-          o osxphotos-export_command                line_option
-            line_option                     * --vacuum
-    * --list                                      o osxphotos-exportdb_command
-          o osxphotos-theme_command                 line_option
-            line_option                     * --verbose
-    * --live                                      o osxphotos-add-locations
-          o osxphotos-add-locations                 command_line_option
-            command_line_option                   o osxphotos-batch-edit
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-diff_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-exiftool_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-export_command
+          o osxphotos-sync_command_line             option
+            option                          * --yes
+    * --merge                                     o osxphotos-uninstall_command
           o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-exportdb_command
-    * --load-config                                 line_option
-          o osxphotos-exiftool_command            o osxphotos-import_command
-            line_option                             line_option
-          o osxphotos-export_command              o osxphotos-orphans_command
-            line_option                             line_option
-    * --location                                  o osxphotos-sync_command_line
-          o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-timewarp_command
-          o osxphotos-batch-edit                    line_option
-            command_line_option             * --version
-          o osxphotos-export_command              o osxphotos_command_line
-            line_option                             option
-          o osxphotos-import_command              o osxphotos-exportdb_command
-            line_option                             line_option
-          o osxphotos-query_command         * --walk
-            line_option                           o osxphotos-import_command
-          o osxphotos-repl_command_line             line_option
-            option                          * --window
-          o osxphotos-sync_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-    * --match-time                          * --xattr-template
-          o osxphotos-timewarp_command            o osxphotos-export_command
-            line_option                             line_option
-    * --max-size                            * --year
-          o osxphotos-add-locations               o osxphotos-add-locations
-            command_line_option                     command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
-            line_option                             line_option
-          o osxphotos-query_command               o osxphotos-query_command
-            line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-repl_command_line
-            option                                  option
-          o osxphotos-sync_command_line           o osxphotos-sync_command_line
-            option                                  option
-    * --merge                               * --yes
-          o osxphotos-sync_command_line           o osxphotos-uninstall_command
-            option                                  line_option
-    * --merge-keywords                      * -A
-          o osxphotos-import_command              o osxphotos-sync_command_line
-            line_option                             option
-    * --migrate                             * -a
-          o osxphotos-exportdb_command            o osxphotos-import_command
-            line_option                             line_option
-    * --migrate-photos-library                    o osxphotos-timewarp_command
+            option                          * -A
+    * --merge-keywords                            o osxphotos-sync_command_line
+          o osxphotos-import_command                option
+            line_option                     * -a
+    * --migrate                                   o osxphotos-import_command
           o osxphotos-exportdb_command              line_option
-            line_option                     * -C
-    * --min-size                                  o osxphotos-import_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * -c
-          o osxphotos-export_command              o osxphotos-timewarp_command
-            line_option                             line_option
-          o osxphotos-query_command         * -D
+            line_option                           o osxphotos-timewarp_command
+    * --migrate-photos-library                      line_option
+          o osxphotos-exportdb_command      * -C
             line_option                           o osxphotos-import_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-timewarp_command
-          o osxphotos-sync_command_line             line_option
-            option                          * -d
-    * --missing                                   o osxphotos-import_command
-          o osxphotos-add-locations                 line_option
+    * --min-size                                    line_option
+          o osxphotos-add-locations         * -c
             command_line_option                   o osxphotos-timewarp_command
           o osxphotos-export_command                line_option
-            line_option                     * -e
+            line_option                     * -D
           o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-sync_command_line
-            option                                  option
-          o osxphotos-sync_command_line           o osxphotos-timewarp_command
-            option                                  line_option
-    * --name                                * -F
-          o osxphotos-add-locations               o osxphotos-timewarp_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * -f
-            line_option                           o osxphotos-dump_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-import_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-query_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-timewarp_command
-    * --no-comment                                  line_option
-          o osxphotos-add-locations               o osxphotos-uuid_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * -g
-            line_option                           o osxphotos-import_command
-          o osxphotos-query_command                 line_option
-            line_option                     * -h
-          o osxphotos-repl_command_line           o osxphotos-run_command_line
-            option                                  option
-          o osxphotos-sync_command_line     * -i
-            option                                o osxphotos-add-locations
-    * --no-description                              command_line_option
-          o osxphotos-add-locations               o osxphotos-export_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-query_command
-            line_option                             line_option
-          o osxphotos-query_command               o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-repl_command_line           o osxphotos-sync_command_line
-            option                                  option, [1]
-          o osxphotos-sync_command_line           o osxphotos-timewarp_command
-            option                                  line_option
-    * --no-keyword                          * -k
-          o osxphotos-add-locations               o osxphotos-import_command
-            command_line_option                     line_option
-          o osxphotos-export_command        * -L
-            line_option                           o osxphotos-import_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-timewarp_command
-          o osxphotos-repl_command_line             line_option
-            option                          * -l
-          o osxphotos-sync_command_line           o osxphotos-import_command
+          o osxphotos-repl_command_line           o osxphotos-timewarp_command
             option                                  line_option
-    * --no-likes                            * -M
+          o osxphotos-sync_command_line     * -d
+            option                                o osxphotos-import_command
+    * --missing                                     line_option
           o osxphotos-add-locations               o osxphotos-timewarp_command
             command_line_option                     line_option
-          o osxphotos-export_command        * -m
+          o osxphotos-export_command        * -e
             line_option                           o osxphotos-import_command
           o osxphotos-query_command                 line_option
             line_option                           o osxphotos-sync_command_line
           o osxphotos-repl_command_line             option
             option                                o osxphotos-timewarp_command
           o osxphotos-sync_command_line             line_option
-            option                          * -P
-    * --no-location                               o osxphotos-import_command
+            option                          * -F
+    * --name                                      o osxphotos-timewarp_command
           o osxphotos-add-locations                 line_option
-            command_line_option                   o osxphotos-timewarp_command
-          o osxphotos-export_command                line_option
-            line_option                     * -p
+            command_line_option             * -f
+          o osxphotos-export_command              o osxphotos-dump_command_line
+            line_option                             option
           o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-timewarp_command
+          o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
-          o osxphotos-sync_command_line     * -R
-            option                                o osxphotos-import_command
-    * --no-place                                    line_option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * -r
-            line_option                           o osxphotos-diff_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-import_command
-          o osxphotos-repl_command_line             line_option
-            option                          * -s
-          o osxphotos-sync_command_line           o osxphotos-diff_command_line
-            option                                  option
-    * --no-progress                               o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * -T
-          o osxphotos-import_command              o osxphotos-inspect_command
+          o osxphotos-sync_command_line           o osxphotos-timewarp_command
+            option                                  line_option
+    * --no-comment                                o osxphotos-uuid_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * -g
+          o osxphotos-export_command              o osxphotos-import_command
             line_option                             line_option
-    * --no-title                                  o osxphotos-timewarp_command
+          o osxphotos-query_command         * -h
+            line_option                           o osxphotos-run_command_line
+          o osxphotos-repl_command_line             option
+            option                          * -i
+          o osxphotos-sync_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+    * --no-description                            o osxphotos-export_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-query_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-repl_command_line
+          o osxphotos-query_command                 option
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-repl_command_line             option, [1]
+            option                                o osxphotos-timewarp_command
+          o osxphotos-sync_command_line             line_option
+            option                          * -k
+    * --no-keyword                                o osxphotos-import_command
           o osxphotos-add-locations                 line_option
-            command_line_option             * -t
+            command_line_option             * -L
           o osxphotos-export_command              o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-inspect_command
+          o osxphotos-query_command               o osxphotos-timewarp_command
             line_option                             line_option
+          o osxphotos-repl_command_line     * -l
+            option                                o osxphotos-import_command
+          o osxphotos-sync_command_line             line_option
+            option                          * -M
+    * --no-likes                                  o osxphotos-timewarp_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * -m
+          o osxphotos-export_command              o osxphotos-import_command
+            line_option                             line_option
+          o osxphotos-query_command               o osxphotos-sync_command_line
+            line_option                             option
           o osxphotos-repl_command_line           o osxphotos-timewarp_command
             option                                  line_option
-          o osxphotos-sync_command_line     * -U
-            option                                o osxphotos-install_command
-    * --not-burst                                   line_option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * -V
-            line_option                           o osxphotos-add-locations
-          o osxphotos-query_command                 command_line_option
-            line_option                           o osxphotos-batch-edit
-          o osxphotos-repl_command_line             command_line_option
-            option                                o osxphotos-diff_command_line
-          o osxphotos-sync_command_line             option
-            option                                o osxphotos-exiftool_command
-    * --not-cloudasset                              line_option
-          o osxphotos-add-locations               o osxphotos-export_command
+          o osxphotos-sync_command_line     * -P
+            option                                o osxphotos-import_command
+    * --no-location                                 line_option
+          o osxphotos-add-locations               o osxphotos-timewarp_command
             command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-exportdb_command
-            line_option                             line_option
+          o osxphotos-export_command        * -p
+            line_option                           o osxphotos-import_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-timewarp_command
+          o osxphotos-repl_command_line             line_option
+            option                          * -R
+          o osxphotos-sync_command_line           o osxphotos-import_command
+            option                                  line_option
+    * --no-place                                  o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * -r
+          o osxphotos-export_command              o osxphotos-diff_command_line
+            line_option                             option
           o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-orphans_command
+          o osxphotos-repl_command_line     * -s
+            option                                o osxphotos-diff_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-sync_command_line
+    * --no-progress                                 option
+          o osxphotos-export_command        * -T
+            line_option                           o osxphotos-inspect_command
+          o osxphotos-import_command                line_option
+            line_option                           o osxphotos-timewarp_command
+    * --no-title                                    line_option
+          o osxphotos-add-locations         * -t
+            command_line_option                   o osxphotos-import_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-inspect_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-timewarp_command
+          o osxphotos-repl_command_line             line_option
+            option                          * -U
+          o osxphotos-sync_command_line           o osxphotos-install_command
             option                                  line_option
-          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+    * --not-burst                                 o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * -V
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-query_command               o osxphotos-batch-edit
+            line_option                             command_line_option
+          o osxphotos-repl_command_line           o osxphotos-diff_command_line
             option                                  option
-    * --not-edited                                o osxphotos-timewarp_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * -v
-          o osxphotos-export_command              o osxphotos_command_line
-            line_option                             option
-          o osxphotos-query_command         * -w
-            line_option                           o osxphotos-add-locations
-          o osxphotos-repl_command_line             command_line_option
-            option                                o osxphotos-import_command
-          o osxphotos-sync_command_line             line_option
-            option                          * -y
-    * --not-favorite                              o osxphotos-uninstall_command
+          o osxphotos-sync_command_line           o osxphotos-exiftool_command
+            option                                  line_option
+    * --not-cloudasset                            o osxphotos-export_command
           o osxphotos-add-locations                 line_option
-            command_line_option             * -z
-          o osxphotos-export_command              o osxphotos-timewarp_command
-            line_option                             line_option
+            command_line_option                   o osxphotos-exportdb_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-import_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-orphans_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-sync_command_line
+          o osxphotos-sync_command_line             option
+            option                                o osxphotos-timewarp_command
+    * --not-edited                                  line_option
+          o osxphotos-add-locations         * -v
+            command_line_option                   o osxphotos_command_line
+          o osxphotos-export_command                option
+            line_option                     * -w
+          o osxphotos-query_command               o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-repl_command_line           o osxphotos-import_command
+            option                                  line_option
+          o osxphotos-sync_command_line     * -y
+            option                                o osxphotos-uninstall_command
+    * --not-favorite                                line_option
+          o osxphotos-add-locations         * -z
+            command_line_option                   o osxphotos-timewarp_command
+          o osxphotos-export_command                line_option
+            line_option
           o osxphotos-query_command
             line_option
           o osxphotos-repl_command_line
             option
           o osxphotos-sync_command_line
             option
 
@@ -1258,76 +1261,77 @@
                                               (osxphotos.QueryOptions
                                               attribute)
 
 ***** O *****
                                             * osxphotos-info command line
                                               option
                                                   o --db
-    * orientation_(osxphotos.PhotoInfo            o --json
-      property)                                   o --library
-    * original_filename_                          o PHOTOS_LIBRARY
-      (osxphotos.PhotoInfo_property)        * osxphotos-inspect command line
-    * original_filesize_                      option
-      (osxphotos.PhotoInfo_property)              o --db
-    * original_height_                            o --detect-text
-      (osxphotos.PhotoInfo_property)              o --library
-    * original_orientation_                       o --template
-      (osxphotos.PhotoInfo_property)              o --theme
-    * original_width_                             o -t
-      (osxphotos.PhotoInfo_property)              o -T
-    * osxphotos                             * osxphotos-install command line
-          o module                            option
-    * osxphotos command line option               o --upgrade
-          o --db                                  o -U
-          o --json                                o PACKAGES
-          o --library                       * osxphotos-keywords command line
-          o --version                         option
-          o -v                                    o --db
-    * osxphotos-add-locations command             o --json
-      line option                                 o --library
-          o --added-after                         o PHOTOS_LIBRARY
-          o --added-before                  * osxphotos-labels command line
-          o --added-in-last                   option
-          o --album                               o --db
-          o --burst                               o --json
-          o --cloudasset                          o --library
-          o --description                         o PHOTOS_LIBRARY
-          o --dry-run                       * osxphotos-list command line
-          o --duplicate                       option
-          o --edited                              o --json
-          o --exif                          * osxphotos-orphans command line
-          o --external-edit                   option
-          o --favorite                            o --db
-          o --folder                              o --export
-          o --from-date                           o --library
-          o --from-time                           o --theme
-          o --has-comment                         o --timestamp
-          o --has-likes                           o --verbose
-          o --has-raw                             o -V
-          o --hdr                           * osxphotos-persons command line
-          o --hidden                          option
-          o --ignore-case                         o --db
-          o --in-album                            o --json
-          o --incloud                             o --library
-          o --is-reference                        o PHOTOS_LIBRARY
-          o --keyword                       * osxphotos-places command line
-          o --label                           option
-          o --live                                o --db
-          o --location                            o --json
-          o --max-size                            o --library
-          o --min-size                            o PHOTOS_LIBRARY
-          o --missing                       * osxphotos-query command line
-          o --name                            option
-          o --no-comment                          o --add-to-album
-          o --no-description                      o --added-after
-          o --no-keyword                          o --added-before
-          o --no-likes                            o --added-in-last
-          o --no-location                         o --album
-          o --no-place                            o --burst
-          o --no-title                            o --cloudasset
+                                                  o --json
+    * orientation_(osxphotos.PhotoInfo            o --library
+      property)                                   o PHOTOS_LIBRARY
+    * original_filename_                    * osxphotos-inspect command line
+      (osxphotos.PhotoInfo_property)          option
+    * original_filesize_                          o --db
+      (osxphotos.PhotoInfo_property)              o --detect-text
+    * original_height_                            o --library
+      (osxphotos.PhotoInfo_property)              o --template
+    * original_orientation_                       o --theme
+      (osxphotos.PhotoInfo_property)              o -t
+    * original_width_                             o -T
+      (osxphotos.PhotoInfo_property)        * osxphotos-install command line
+    * osxphotos                               option
+          o module                                o --upgrade
+    * osxphotos command line option               o -U
+          o --db                                  o PACKAGES
+          o --json                          * osxphotos-keywords command line
+          o --library                         option
+          o --version                             o --db
+          o -v                                    o --json
+    * osxphotos-add-locations command             o --library
+      line option                                 o PHOTOS_LIBRARY
+          o --added-after                   * osxphotos-labels command line
+          o --added-before                    option
+          o --added-in-last                       o --db
+          o --album                               o --json
+          o --burst                               o --library
+          o --cloudasset                          o PHOTOS_LIBRARY
+          o --description                   * osxphotos-list command line
+          o --dry-run                         option
+          o --duplicate                           o --json
+          o --edited                        * osxphotos-orphans command line
+          o --exif                            option
+          o --external-edit                       o --db
+          o --favorite                            o --export
+          o --folder                              o --library
+          o --from-date                           o --theme
+          o --from-time                           o --timestamp
+          o --has-comment                         o --verbose
+          o --has-likes                           o -V
+          o --has-raw                       * osxphotos-persons command line
+          o --hdr                             option
+          o --hidden                              o --db
+          o --ignore-case                         o --json
+          o --in-album                            o --library
+          o --incloud                             o PHOTOS_LIBRARY
+          o --is-reference                  * osxphotos-places command line
+          o --keyword                         option
+          o --label                               o --db
+          o --live                                o --json
+          o --location                            o --library
+          o --max-size                            o PHOTOS_LIBRARY
+          o --min-size                      * osxphotos-query command line
+          o --missing                         option
+          o --name                                o --add-to-album
+          o --no-comment                          o --added-after
+          o --no-description                      o --added-before
+          o --no-keyword                          o --added-in-last
+          o --no-likes                            o --album
+          o --no-location                         o --burst
+          o --no-place                            o --cloudasset
+          o --no-title                            o --count
           o --not-burst                           o --db
           o --not-cloudasset                      o --deleted
           o --not-edited                          o --deleted-only
           o --not-favorite                        o --description
           o --not-hdr                             o --duplicate
           o --not-hidden                          o --edited
           o --not-in-album                        o --exif
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.60.4 documentation</title>
+        <title>osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/objects.inv

##### Sphinx inventory

```diff
@@ -861,14 +861,15 @@
 osxphotos-query.--add-to-album std:cmdoption 1 cli.html#cmdoption-osxphotos-query-add-to-album -
 osxphotos-query.--added-after std:cmdoption 1 cli.html#cmdoption-osxphotos-query-added-after -
 osxphotos-query.--added-before std:cmdoption 1 cli.html#cmdoption-osxphotos-query-added-before -
 osxphotos-query.--added-in-last std:cmdoption 1 cli.html#cmdoption-osxphotos-query-added-in-last -
 osxphotos-query.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-query-album -
 osxphotos-query.--burst std:cmdoption 1 cli.html#cmdoption-osxphotos-query-burst -
 osxphotos-query.--cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-query-cloudasset -
+osxphotos-query.--count std:cmdoption 1 cli.html#cmdoption-osxphotos-query-count -
 osxphotos-query.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-query-library -
 osxphotos-query.--deleted std:cmdoption 1 cli.html#cmdoption-osxphotos-query-deleted -
 osxphotos-query.--deleted-only std:cmdoption 1 cli.html#cmdoption-osxphotos-query-deleted-only -
 osxphotos-query.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-query-description -
 osxphotos-query.--duplicate std:cmdoption 1 cli.html#cmdoption-osxphotos-query-duplicate -
 osxphotos-query.--edited std:cmdoption 1 cli.html#cmdoption-osxphotos-query-edited -
 osxphotos-query.--exif std:cmdoption 1 cli.html#cmdoption-osxphotos-query-exif -
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.60.4 documentation</title>
+        <title>OSXPhotos - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.60.4 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.4 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.5 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.60.4 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.4 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.5 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/searchindex.js

##### js-beautify {}

```diff
@@ -1373,15 +1373,15 @@
         "path_sep": 4,
         "separ": [0, 4, 5, 6],
         "model": [4, 5],
         "photoscript": 4,
         "_skip_searchinfo": 4,
         "extract": [4, 5],
         "4": [4, 5, 6],
-        "count": [4, 5],
+        "count": [0, 4, 5],
         "descend": 4,
         "initi": 4,
         "liglob": 4,
         "tabl": 4,
         "statement": [4, 5, 6],
         "cursor": 4,
         "wed": 4,
@@ -3170,14 +3170,15 @@
             [0, 6, 1, "cmdoption-osxphotos-query-add-to-album", "--add-to-album"],
             [0, 6, 1, "cmdoption-osxphotos-query-added-after", "--added-after"],
             [0, 6, 1, "cmdoption-osxphotos-query-added-before", "--added-before"],
             [0, 6, 1, "cmdoption-osxphotos-query-added-in-last", "--added-in-last"],
             [0, 6, 1, "cmdoption-osxphotos-query-album", "--album"],
             [0, 6, 1, "cmdoption-osxphotos-query-burst", "--burst"],
             [0, 6, 1, "cmdoption-osxphotos-query-cloudasset", "--cloudasset"],
+            [0, 6, 1, "cmdoption-osxphotos-query-count", "--count"],
             [0, 6, 1, "cmdoption-osxphotos-query-library", "--db"],
             [0, 6, 1, "cmdoption-osxphotos-query-deleted", "--deleted"],
             [0, 6, 1, "cmdoption-osxphotos-query-deleted-only", "--deleted-only"],
             [0, 6, 1, "cmdoption-osxphotos-query-description", "--description"],
             [0, 6, 1, "cmdoption-osxphotos-query-duplicate", "--duplicate"],
             [0, 6, 1, "cmdoption-osxphotos-query-edited", "--edited"],
             [0, 6, 1, "cmdoption-osxphotos-query-exif", "--exif"],
@@ -4111,9 +4112,3279 @@
         "Color Themes": [
             [6, "color-themes"]
         ],
         "Conclusion": [
             [6, "conclusion"]
         ]
     },
-    "indexentries": {}
+    "indexentries": {
+        "--add-exported-to-album": [
+            [0, "cmdoption-osxphotos-export-add-exported-to-album"]
+        ],
+        "--add-missing-to-album": [
+            [0, "cmdoption-osxphotos-export-add-missing-to-album"]
+        ],
+        "--add-skipped-to-album": [
+            [0, "cmdoption-osxphotos-export-add-skipped-to-album"]
+        ],
+        "--add-to-album": [
+            [0, "cmdoption-osxphotos-query-add-to-album"],
+            [0, "cmdoption-osxphotos-timewarp-a"]
+        ],
+        "--added-after": [
+            [0, "cmdoption-osxphotos-add-locations-added-after"],
+            [0, "cmdoption-osxphotos-export-added-after"],
+            [0, "cmdoption-osxphotos-query-added-after"],
+            [0, "cmdoption-osxphotos-repl-added-after"],
+            [0, "cmdoption-osxphotos-sync-added-after"]
+        ],
+        "--added-before": [
+            [0, "cmdoption-osxphotos-add-locations-added-before"],
+            [0, "cmdoption-osxphotos-export-added-before"],
+            [0, "cmdoption-osxphotos-query-added-before"],
+            [0, "cmdoption-osxphotos-repl-added-before"],
+            [0, "cmdoption-osxphotos-sync-added-before"]
+        ],
+        "--added-in-last": [
+            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
+            [0, "cmdoption-osxphotos-export-added-in-last"],
+            [0, "cmdoption-osxphotos-query-added-in-last"],
+            [0, "cmdoption-osxphotos-repl-added-in-last"],
+            [0, "cmdoption-osxphotos-sync-added-in-last"]
+        ],
+        "--album": [
+            [0, "cmdoption-osxphotos-add-locations-album"],
+            [0, "cmdoption-osxphotos-export-album"],
+            [0, "cmdoption-osxphotos-import-a"],
+            [0, "cmdoption-osxphotos-query-album"],
+            [0, "cmdoption-osxphotos-repl-album"],
+            [0, "cmdoption-osxphotos-sync-album"]
+        ],
+        "--album-keyword": [
+            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
+            [0, "cmdoption-osxphotos-export-album-keyword"]
+        ],
+        "--alt-copy": [
+            [0, "cmdoption-osxphotos-export-alt-copy"]
+        ],
+        "--append": [
+            [0, "cmdoption-osxphotos-exiftool-append"],
+            [0, "cmdoption-osxphotos-export-append"],
+            [0, "cmdoption-osxphotos-exportdb-append"],
+            [0, "cmdoption-osxphotos-import-append"],
+            [0, "cmdoption-osxphotos-sync-A"]
+        ],
+        "--burst": [
+            [0, "cmdoption-osxphotos-add-locations-burst"],
+            [0, "cmdoption-osxphotos-export-burst"],
+            [0, "cmdoption-osxphotos-query-burst"],
+            [0, "cmdoption-osxphotos-repl-burst"],
+            [0, "cmdoption-osxphotos-sync-burst"]
+        ],
+        "--check-signatures": [
+            [0, "cmdoption-osxphotos-exportdb-check-signatures"]
+        ],
+        "--check-templates": [
+            [0, "cmdoption-osxphotos-import-check-templates"]
+        ],
+        "--cleanup": [
+            [0, "cmdoption-osxphotos-export-cleanup"]
+        ],
+        "--clear-location": [
+            [0, "cmdoption-osxphotos-import-L"]
+        ],
+        "--clear-metadata": [
+            [0, "cmdoption-osxphotos-import-C"]
+        ],
+        "--clone": [
+            [0, "cmdoption-osxphotos-theme-clone"]
+        ],
+        "--cloudasset": [
+            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
+            [0, "cmdoption-osxphotos-export-cloudasset"],
+            [0, "cmdoption-osxphotos-query-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-cloudasset"]
+        ],
+        "--compare-exif": [
+            [0, "cmdoption-osxphotos-timewarp-c"]
+        ],
+        "--config": [
+            [0, "cmdoption-osxphotos-theme-config"]
+        ],
+        "--config-only": [
+            [0, "cmdoption-osxphotos-export-config-only"]
+        ],
+        "--convert-to-jpeg": [
+            [0, "cmdoption-osxphotos-export-convert-to-jpeg"]
+        ],
+        "--count": [
+            [0, "cmdoption-osxphotos-query-count"]
+        ],
+        "--current-name": [
+            [0, "cmdoption-osxphotos-export-current-name"]
+        ],
+        "--date": [
+            [0, "cmdoption-osxphotos-timewarp-d"]
+        ],
+        "--date-added": [
+            [0, "cmdoption-osxphotos-timewarp-date-added"]
+        ],
+        "--date-added-from-photo": [
+            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"]
+        ],
+        "--date-delta": [
+            [0, "cmdoption-osxphotos-timewarp-D"]
+        ],
+        "--db": [
+            [0, "cmdoption-osxphotos-albums-library"],
+            [0, "cmdoption-osxphotos-batch-edit-library"],
+            [0, "cmdoption-osxphotos-diff-library"],
+            [0, "cmdoption-osxphotos-dump-library"],
+            [0, "cmdoption-osxphotos-exiftool-library"],
+            [0, "cmdoption-osxphotos-export-library"],
+            [0, "cmdoption-osxphotos-info-library"],
+            [0, "cmdoption-osxphotos-inspect-library"],
+            [0, "cmdoption-osxphotos-keywords-library"],
+            [0, "cmdoption-osxphotos-labels-library"],
+            [0, "cmdoption-osxphotos-library"],
+            [0, "cmdoption-osxphotos-orphans-library"],
+            [0, "cmdoption-osxphotos-persons-library"],
+            [0, "cmdoption-osxphotos-places-library"],
+            [0, "cmdoption-osxphotos-query-library"],
+            [0, "cmdoption-osxphotos-repl-library"],
+            [0, "cmdoption-osxphotos-show-library"],
+            [0, "cmdoption-osxphotos-snap-library"],
+            [0, "cmdoption-osxphotos-sync-library"]
+        ],
+        "--db-config": [
+            [0, "cmdoption-osxphotos-exiftool-db-config"]
+        ],
+        "--default": [
+            [0, "cmdoption-osxphotos-theme-default"]
+        ],
+        "--delete": [
+            [0, "cmdoption-osxphotos-theme-delete"]
+        ],
+        "--delete-file": [
+            [0, "cmdoption-osxphotos-exportdb-delete-file"]
+        ],
+        "--delete-uuid": [
+            [0, "cmdoption-osxphotos-exportdb-delete-uuid"]
+        ],
+        "--deleted": [
+            [0, "cmdoption-osxphotos-dump-deleted"],
+            [0, "cmdoption-osxphotos-export-deleted"],
+            [0, "cmdoption-osxphotos-query-deleted"],
+            [0, "cmdoption-osxphotos-repl-deleted"]
+        ],
+        "--deleted-only": [
+            [0, "cmdoption-osxphotos-dump-deleted-only"],
+            [0, "cmdoption-osxphotos-export-deleted-only"],
+            [0, "cmdoption-osxphotos-query-deleted-only"],
+            [0, "cmdoption-osxphotos-repl-deleted-only"]
+        ],
+        "--description": [
+            [0, "cmdoption-osxphotos-add-locations-description"],
+            [0, "cmdoption-osxphotos-batch-edit-description"],
+            [0, "cmdoption-osxphotos-export-description"],
+            [0, "cmdoption-osxphotos-import-d"],
+            [0, "cmdoption-osxphotos-query-description"],
+            [0, "cmdoption-osxphotos-repl-description"],
+            [0, "cmdoption-osxphotos-sync-description"]
+        ],
+        "--description-template": [
+            [0, "cmdoption-osxphotos-exiftool-description-template"],
+            [0, "cmdoption-osxphotos-export-description-template"]
+        ],
+        "--detect-text": [
+            [0, "cmdoption-osxphotos-inspect-t"]
+        ],
+        "--directory": [
+            [0, "cmdoption-osxphotos-export-directory"]
+        ],
+        "--download-missing": [
+            [0, "cmdoption-osxphotos-export-download-missing"]
+        ],
+        "--dry-run": [
+            [0, "cmdoption-osxphotos-add-locations-dry-run"],
+            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
+            [0, "cmdoption-osxphotos-exiftool-dry-run"],
+            [0, "cmdoption-osxphotos-export-dry-run"],
+            [0, "cmdoption-osxphotos-exportdb-dry-run"],
+            [0, "cmdoption-osxphotos-sync-dry-run"]
+        ],
+        "--dup-check": [
+            [0, "cmdoption-osxphotos-import-D"]
+        ],
+        "--duplicate": [
+            [0, "cmdoption-osxphotos-add-locations-duplicate"],
+            [0, "cmdoption-osxphotos-export-duplicate"],
+            [0, "cmdoption-osxphotos-query-duplicate"],
+            [0, "cmdoption-osxphotos-repl-duplicate"],
+            [0, "cmdoption-osxphotos-sync-duplicate"]
+        ],
+        "--edit": [
+            [0, "cmdoption-osxphotos-theme-edit"]
+        ],
+        "--edited": [
+            [0, "cmdoption-osxphotos-add-locations-edited"],
+            [0, "cmdoption-osxphotos-export-edited"],
+            [0, "cmdoption-osxphotos-query-edited"],
+            [0, "cmdoption-osxphotos-repl-edited"],
+            [0, "cmdoption-osxphotos-sync-edited"]
+        ],
+        "--edited-suffix": [
+            [0, "cmdoption-osxphotos-export-edited-suffix"]
+        ],
+        "--emacs": [
+            [0, "cmdoption-osxphotos-repl-emacs"]
+        ],
+        "--errors": [
+            [0, "cmdoption-osxphotos-exportdb-errors"]
+        ],
+        "--exif": [
+            [0, "cmdoption-osxphotos-add-locations-exif"],
+            [0, "cmdoption-osxphotos-export-exif"],
+            [0, "cmdoption-osxphotos-query-exif"],
+            [0, "cmdoption-osxphotos-repl-exif"],
+            [0, "cmdoption-osxphotos-sync-exif"]
+        ],
+        "--exiftool": [
+            [0, "cmdoption-osxphotos-export-exiftool"],
+            [0, "cmdoption-osxphotos-import-e"]
+        ],
+        "--exiftool-merge-keywords": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"]
+        ],
+        "--exiftool-merge-persons": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"]
+        ],
+        "--exiftool-option": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
+            [0, "cmdoption-osxphotos-export-exiftool-option"]
+        ],
+        "--exiftool-path": [
+            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
+            [0, "cmdoption-osxphotos-export-exiftool-path"],
+            [0, "cmdoption-osxphotos-import-0"],
+            [0, "cmdoption-osxphotos-timewarp-e"]
+        ],
+        "--export": [
+            [0, "cmdoption-osxphotos-orphans-export"],
+            [0, "cmdoption-osxphotos-sync-e"]
+        ],
+        "--export-as-hardlink": [
+            [0, "cmdoption-osxphotos-export-export-as-hardlink"]
+        ],
+        "--export-by-date": [
+            [0, "cmdoption-osxphotos-export-export-by-date"]
+        ],
+        "--export-dir": [
+            [0, "cmdoption-osxphotos-exportdb-export-dir"]
+        ],
+        "--exportdb": [
+            [0, "cmdoption-osxphotos-exiftool-exportdb"],
+            [0, "cmdoption-osxphotos-export-exportdb"]
+        ],
+        "--external-edit": [
+            [0, "cmdoption-osxphotos-add-locations-external-edit"],
+            [0, "cmdoption-osxphotos-export-external-edit"],
+            [0, "cmdoption-osxphotos-query-external-edit"],
+            [0, "cmdoption-osxphotos-repl-external-edit"],
+            [0, "cmdoption-osxphotos-sync-external-edit"]
+        ],
+        "--favorite": [
+            [0, "cmdoption-osxphotos-add-locations-favorite"],
+            [0, "cmdoption-osxphotos-export-favorite"],
+            [0, "cmdoption-osxphotos-query-favorite"],
+            [0, "cmdoption-osxphotos-repl-favorite"],
+            [0, "cmdoption-osxphotos-sync-favorite"]
+        ],
+        "--favorite-rating": [
+            [0, "cmdoption-osxphotos-export-favorite-rating"]
+        ],
+        "--field": [
+            [0, "cmdoption-osxphotos-dump-f"],
+            [0, "cmdoption-osxphotos-query-f"]
+        ],
+        "--filename": [
+            [0, "cmdoption-osxphotos-export-filename"],
+            [0, "cmdoption-osxphotos-uuid-f"]
+        ],
+        "--finder-tag-keywords": [
+            [0, "cmdoption-osxphotos-export-finder-tag-keywords"]
+        ],
+        "--finder-tag-template": [
+            [0, "cmdoption-osxphotos-export-finder-tag-template"]
+        ],
+        "--folder": [
+            [0, "cmdoption-osxphotos-add-locations-folder"],
+            [0, "cmdoption-osxphotos-export-folder"],
+            [0, "cmdoption-osxphotos-query-folder"],
+            [0, "cmdoption-osxphotos-repl-folder"],
+            [0, "cmdoption-osxphotos-sync-folder"]
+        ],
+        "--force": [
+            [0, "cmdoption-osxphotos-timewarp-force"]
+        ],
+        "--force-update": [
+            [0, "cmdoption-osxphotos-export-force-update"]
+        ],
+        "--from-date": [
+            [0, "cmdoption-osxphotos-add-locations-from-date"],
+            [0, "cmdoption-osxphotos-export-from-date"],
+            [0, "cmdoption-osxphotos-query-from-date"],
+            [0, "cmdoption-osxphotos-repl-from-date"],
+            [0, "cmdoption-osxphotos-sync-from-date"]
+        ],
+        "--from-time": [
+            [0, "cmdoption-osxphotos-add-locations-from-time"],
+            [0, "cmdoption-osxphotos-export-from-time"],
+            [0, "cmdoption-osxphotos-query-from-time"],
+            [0, "cmdoption-osxphotos-repl-from-time"],
+            [0, "cmdoption-osxphotos-sync-from-time"]
+        ],
+        "--function": [
+            [0, "cmdoption-osxphotos-timewarp-F"]
+        ],
+        "--glob": [
+            [0, "cmdoption-osxphotos-import-g"]
+        ],
+        "--has-comment": [
+            [0, "cmdoption-osxphotos-add-locations-has-comment"],
+            [0, "cmdoption-osxphotos-export-has-comment"],
+            [0, "cmdoption-osxphotos-query-has-comment"],
+            [0, "cmdoption-osxphotos-repl-has-comment"],
+            [0, "cmdoption-osxphotos-sync-has-comment"]
+        ],
+        "--has-likes": [
+            [0, "cmdoption-osxphotos-add-locations-has-likes"],
+            [0, "cmdoption-osxphotos-export-has-likes"],
+            [0, "cmdoption-osxphotos-query-has-likes"],
+            [0, "cmdoption-osxphotos-repl-has-likes"],
+            [0, "cmdoption-osxphotos-sync-has-likes"]
+        ],
+        "--has-raw": [
+            [0, "cmdoption-osxphotos-add-locations-has-raw"],
+            [0, "cmdoption-osxphotos-export-has-raw"],
+            [0, "cmdoption-osxphotos-query-has-raw"],
+            [0, "cmdoption-osxphotos-repl-has-raw"],
+            [0, "cmdoption-osxphotos-sync-has-raw"]
+        ],
+        "--hdr": [
+            [0, "cmdoption-osxphotos-add-locations-hdr"],
+            [0, "cmdoption-osxphotos-export-hdr"],
+            [0, "cmdoption-osxphotos-query-hdr"],
+            [0, "cmdoption-osxphotos-repl-hdr"],
+            [0, "cmdoption-osxphotos-sync-hdr"]
+        ],
+        "--help": [
+            [0, "cmdoption-osxphotos-run-h"]
+        ],
+        "--hidden": [
+            [0, "cmdoption-osxphotos-add-locations-hidden"],
+            [0, "cmdoption-osxphotos-export-hidden"],
+            [0, "cmdoption-osxphotos-query-hidden"],
+            [0, "cmdoption-osxphotos-repl-hidden"],
+            [0, "cmdoption-osxphotos-sync-hidden"]
+        ],
+        "--ignore-case": [
+            [0, "cmdoption-osxphotos-add-locations-i"],
+            [0, "cmdoption-osxphotos-export-i"],
+            [0, "cmdoption-osxphotos-query-i"],
+            [0, "cmdoption-osxphotos-repl-i"],
+            [0, "cmdoption-osxphotos-sync-0"]
+        ],
+        "--ignore-date-modified": [
+            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
+            [0, "cmdoption-osxphotos-export-ignore-date-modified"]
+        ],
+        "--ignore-signature": [
+            [0, "cmdoption-osxphotos-export-ignore-signature"]
+        ],
+        "--import": [
+            [0, "cmdoption-osxphotos-sync-i"]
+        ],
+        "--in-album": [
+            [0, "cmdoption-osxphotos-add-locations-in-album"],
+            [0, "cmdoption-osxphotos-export-in-album"],
+            [0, "cmdoption-osxphotos-query-in-album"],
+            [0, "cmdoption-osxphotos-repl-in-album"],
+            [0, "cmdoption-osxphotos-sync-in-album"]
+        ],
+        "--incloud": [
+            [0, "cmdoption-osxphotos-add-locations-incloud"],
+            [0, "cmdoption-osxphotos-export-incloud"],
+            [0, "cmdoption-osxphotos-query-incloud"],
+            [0, "cmdoption-osxphotos-repl-incloud"],
+            [0, "cmdoption-osxphotos-sync-incloud"]
+        ],
+        "--info": [
+            [0, "cmdoption-osxphotos-exportdb-info"]
+        ],
+        "--inspect": [
+            [0, "cmdoption-osxphotos-timewarp-i"]
+        ],
+        "--is-reference": [
+            [0, "cmdoption-osxphotos-add-locations-is-reference"],
+            [0, "cmdoption-osxphotos-export-is-reference"],
+            [0, "cmdoption-osxphotos-query-is-reference"],
+            [0, "cmdoption-osxphotos-repl-is-reference"],
+            [0, "cmdoption-osxphotos-sync-is-reference"]
+        ],
+        "--jpeg-ext": [
+            [0, "cmdoption-osxphotos-export-jpeg-ext"]
+        ],
+        "--jpeg-quality": [
+            [0, "cmdoption-osxphotos-export-jpeg-quality"]
+        ],
+        "--json": [
+            [0, "cmdoption-osxphotos-albums-json"],
+            [0, "cmdoption-osxphotos-dump-json"],
+            [0, "cmdoption-osxphotos-info-json"],
+            [0, "cmdoption-osxphotos-json"],
+            [0, "cmdoption-osxphotos-keywords-json"],
+            [0, "cmdoption-osxphotos-labels-json"],
+            [0, "cmdoption-osxphotos-list-json"],
+            [0, "cmdoption-osxphotos-persons-json"],
+            [0, "cmdoption-osxphotos-places-json"],
+            [0, "cmdoption-osxphotos-query-json"]
+        ],
+        "--keep": [
+            [0, "cmdoption-osxphotos-export-keep"]
+        ],
+        "--keyword": [
+            [0, "cmdoption-osxphotos-add-locations-keyword"],
+            [0, "cmdoption-osxphotos-batch-edit-keyword"],
+            [0, "cmdoption-osxphotos-export-keyword"],
+            [0, "cmdoption-osxphotos-import-k"],
+            [0, "cmdoption-osxphotos-query-keyword"],
+            [0, "cmdoption-osxphotos-repl-keyword"],
+            [0, "cmdoption-osxphotos-sync-keyword"]
+        ],
+        "--keyword-template": [
+            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
+            [0, "cmdoption-osxphotos-export-keyword-template"]
+        ],
+        "--label": [
+            [0, "cmdoption-osxphotos-add-locations-label"],
+            [0, "cmdoption-osxphotos-export-label"],
+            [0, "cmdoption-osxphotos-query-label"],
+            [0, "cmdoption-osxphotos-repl-label"],
+            [0, "cmdoption-osxphotos-sync-label"]
+        ],
+        "--last-errors": [
+            [0, "cmdoption-osxphotos-exportdb-last-errors"]
+        ],
+        "--last-run": [
+            [0, "cmdoption-osxphotos-exportdb-last-run"]
+        ],
+        "--library": [
+            [0, "cmdoption-osxphotos-albums-library"],
+            [0, "cmdoption-osxphotos-batch-edit-library"],
+            [0, "cmdoption-osxphotos-diff-library"],
+            [0, "cmdoption-osxphotos-dump-library"],
+            [0, "cmdoption-osxphotos-exiftool-library"],
+            [0, "cmdoption-osxphotos-export-library"],
+            [0, "cmdoption-osxphotos-info-library"],
+            [0, "cmdoption-osxphotos-inspect-library"],
+            [0, "cmdoption-osxphotos-keywords-library"],
+            [0, "cmdoption-osxphotos-labels-library"],
+            [0, "cmdoption-osxphotos-library"],
+            [0, "cmdoption-osxphotos-orphans-library"],
+            [0, "cmdoption-osxphotos-persons-library"],
+            [0, "cmdoption-osxphotos-places-library"],
+            [0, "cmdoption-osxphotos-query-library"],
+            [0, "cmdoption-osxphotos-repl-library"],
+            [0, "cmdoption-osxphotos-show-library"],
+            [0, "cmdoption-osxphotos-snap-library"],
+            [0, "cmdoption-osxphotos-sync-library"],
+            [0, "cmdoption-osxphotos-timewarp-L"]
+        ],
+        "--limit": [
+            [0, "cmdoption-osxphotos-export-limit"]
+        ],
+        "--list": [
+            [0, "cmdoption-osxphotos-theme-list"]
+        ],
+        "--live": [
+            [0, "cmdoption-osxphotos-add-locations-live"],
+            [0, "cmdoption-osxphotos-export-live"],
+            [0, "cmdoption-osxphotos-query-live"],
+            [0, "cmdoption-osxphotos-repl-live"],
+            [0, "cmdoption-osxphotos-sync-live"]
+        ],
+        "--load-config": [
+            [0, "cmdoption-osxphotos-exiftool-load-config"],
+            [0, "cmdoption-osxphotos-export-load-config"]
+        ],
+        "--location": [
+            [0, "cmdoption-osxphotos-add-locations-location"],
+            [0, "cmdoption-osxphotos-batch-edit-location"],
+            [0, "cmdoption-osxphotos-export-location"],
+            [0, "cmdoption-osxphotos-import-l"],
+            [0, "cmdoption-osxphotos-query-location"],
+            [0, "cmdoption-osxphotos-repl-location"],
+            [0, "cmdoption-osxphotos-sync-location"]
+        ],
+        "--match-time": [
+            [0, "cmdoption-osxphotos-timewarp-0"]
+        ],
+        "--max-size": [
+            [0, "cmdoption-osxphotos-add-locations-max-size"],
+            [0, "cmdoption-osxphotos-export-max-size"],
+            [0, "cmdoption-osxphotos-query-max-size"],
+            [0, "cmdoption-osxphotos-repl-max-size"],
+            [0, "cmdoption-osxphotos-sync-max-size"]
+        ],
+        "--merge": [
+            [0, "cmdoption-osxphotos-sync-m"]
+        ],
+        "--merge-keywords": [
+            [0, "cmdoption-osxphotos-import-m"]
+        ],
+        "--migrate": [
+            [0, "cmdoption-osxphotos-exportdb-migrate"]
+        ],
+        "--migrate-photos-library": [
+            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"]
+        ],
+        "--min-size": [
+            [0, "cmdoption-osxphotos-add-locations-min-size"],
+            [0, "cmdoption-osxphotos-export-min-size"],
+            [0, "cmdoption-osxphotos-query-min-size"],
+            [0, "cmdoption-osxphotos-repl-min-size"],
+            [0, "cmdoption-osxphotos-sync-min-size"]
+        ],
+        "--missing": [
+            [0, "cmdoption-osxphotos-add-locations-missing"],
+            [0, "cmdoption-osxphotos-export-missing"],
+            [0, "cmdoption-osxphotos-query-missing"],
+            [0, "cmdoption-osxphotos-repl-missing"],
+            [0, "cmdoption-osxphotos-sync-missing"]
+        ],
+        "--name": [
+            [0, "cmdoption-osxphotos-add-locations-name"],
+            [0, "cmdoption-osxphotos-export-name"],
+            [0, "cmdoption-osxphotos-query-name"],
+            [0, "cmdoption-osxphotos-repl-name"],
+            [0, "cmdoption-osxphotos-sync-name"]
+        ],
+        "--no-comment": [
+            [0, "cmdoption-osxphotos-add-locations-no-comment"],
+            [0, "cmdoption-osxphotos-export-no-comment"],
+            [0, "cmdoption-osxphotos-query-no-comment"],
+            [0, "cmdoption-osxphotos-repl-no-comment"],
+            [0, "cmdoption-osxphotos-sync-no-comment"]
+        ],
+        "--no-description": [
+            [0, "cmdoption-osxphotos-add-locations-no-description"],
+            [0, "cmdoption-osxphotos-export-no-description"],
+            [0, "cmdoption-osxphotos-query-no-description"],
+            [0, "cmdoption-osxphotos-repl-no-description"],
+            [0, "cmdoption-osxphotos-sync-no-description"]
+        ],
+        "--no-keyword": [
+            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
+            [0, "cmdoption-osxphotos-export-no-keyword"],
+            [0, "cmdoption-osxphotos-query-no-keyword"],
+            [0, "cmdoption-osxphotos-repl-no-keyword"],
+            [0, "cmdoption-osxphotos-sync-no-keyword"]
+        ],
+        "--no-likes": [
+            [0, "cmdoption-osxphotos-add-locations-no-likes"],
+            [0, "cmdoption-osxphotos-export-no-likes"],
+            [0, "cmdoption-osxphotos-query-no-likes"],
+            [0, "cmdoption-osxphotos-repl-no-likes"],
+            [0, "cmdoption-osxphotos-sync-no-likes"]
+        ],
+        "--no-location": [
+            [0, "cmdoption-osxphotos-add-locations-no-location"],
+            [0, "cmdoption-osxphotos-export-no-location"],
+            [0, "cmdoption-osxphotos-query-no-location"],
+            [0, "cmdoption-osxphotos-repl-no-location"],
+            [0, "cmdoption-osxphotos-sync-no-location"]
+        ],
+        "--no-place": [
+            [0, "cmdoption-osxphotos-add-locations-no-place"],
+            [0, "cmdoption-osxphotos-export-no-place"],
+            [0, "cmdoption-osxphotos-query-no-place"],
+            [0, "cmdoption-osxphotos-repl-no-place"],
+            [0, "cmdoption-osxphotos-sync-no-place"]
+        ],
+        "--no-progress": [
+            [0, "cmdoption-osxphotos-export-no-progress"],
+            [0, "cmdoption-osxphotos-import-no-progress"]
+        ],
+        "--no-title": [
+            [0, "cmdoption-osxphotos-add-locations-no-title"],
+            [0, "cmdoption-osxphotos-export-no-title"],
+            [0, "cmdoption-osxphotos-query-no-title"],
+            [0, "cmdoption-osxphotos-repl-no-title"],
+            [0, "cmdoption-osxphotos-sync-no-title"]
+        ],
+        "--not-burst": [
+            [0, "cmdoption-osxphotos-add-locations-not-burst"],
+            [0, "cmdoption-osxphotos-export-not-burst"],
+            [0, "cmdoption-osxphotos-query-not-burst"],
+            [0, "cmdoption-osxphotos-repl-not-burst"],
+            [0, "cmdoption-osxphotos-sync-not-burst"]
+        ],
+        "--not-cloudasset": [
+            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
+            [0, "cmdoption-osxphotos-export-not-cloudasset"],
+            [0, "cmdoption-osxphotos-query-not-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-not-cloudasset"]
+        ],
+        "--not-edited": [
+            [0, "cmdoption-osxphotos-add-locations-not-edited"],
+            [0, "cmdoption-osxphotos-export-not-edited"],
+            [0, "cmdoption-osxphotos-query-not-edited"],
+            [0, "cmdoption-osxphotos-repl-not-edited"],
+            [0, "cmdoption-osxphotos-sync-not-edited"]
+        ],
+        "--not-favorite": [
+            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
+            [0, "cmdoption-osxphotos-export-not-favorite"],
+            [0, "cmdoption-osxphotos-query-not-favorite"],
+            [0, "cmdoption-osxphotos-repl-not-favorite"],
+            [0, "cmdoption-osxphotos-sync-not-favorite"]
+        ],
+        "--not-hdr": [
+            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
+            [0, "cmdoption-osxphotos-export-not-hdr"],
+            [0, "cmdoption-osxphotos-query-not-hdr"],
+            [0, "cmdoption-osxphotos-repl-not-hdr"],
+            [0, "cmdoption-osxphotos-sync-not-hdr"]
+        ],
+        "--not-hidden": [
+            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
+            [0, "cmdoption-osxphotos-export-not-hidden"],
+            [0, "cmdoption-osxphotos-query-not-hidden"],
+            [0, "cmdoption-osxphotos-repl-not-hidden"],
+            [0, "cmdoption-osxphotos-sync-not-hidden"]
+        ],
+        "--not-in-album": [
+            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
+            [0, "cmdoption-osxphotos-export-not-in-album"],
+            [0, "cmdoption-osxphotos-query-not-in-album"],
+            [0, "cmdoption-osxphotos-repl-not-in-album"],
+            [0, "cmdoption-osxphotos-sync-not-in-album"]
+        ],
+        "--not-incloud": [
+            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
+            [0, "cmdoption-osxphotos-export-not-incloud"],
+            [0, "cmdoption-osxphotos-query-not-incloud"],
+            [0, "cmdoption-osxphotos-repl-not-incloud"],
+            [0, "cmdoption-osxphotos-sync-not-incloud"]
+        ],
+        "--not-live": [
+            [0, "cmdoption-osxphotos-add-locations-not-live"],
+            [0, "cmdoption-osxphotos-export-not-live"],
+            [0, "cmdoption-osxphotos-query-not-live"],
+            [0, "cmdoption-osxphotos-repl-not-live"],
+            [0, "cmdoption-osxphotos-sync-not-live"]
+        ],
+        "--not-missing": [
+            [0, "cmdoption-osxphotos-add-locations-not-missing"],
+            [0, "cmdoption-osxphotos-export-not-missing"],
+            [0, "cmdoption-osxphotos-query-not-missing"],
+            [0, "cmdoption-osxphotos-repl-not-missing"],
+            [0, "cmdoption-osxphotos-sync-not-missing"]
+        ],
+        "--not-panorama": [
+            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
+            [0, "cmdoption-osxphotos-export-not-panorama"],
+            [0, "cmdoption-osxphotos-query-not-panorama"],
+            [0, "cmdoption-osxphotos-repl-not-panorama"],
+            [0, "cmdoption-osxphotos-sync-not-panorama"]
+        ],
+        "--not-portrait": [
+            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
+            [0, "cmdoption-osxphotos-export-not-portrait"],
+            [0, "cmdoption-osxphotos-query-not-portrait"],
+            [0, "cmdoption-osxphotos-repl-not-portrait"],
+            [0, "cmdoption-osxphotos-sync-not-portrait"]
+        ],
+        "--not-reference": [
+            [0, "cmdoption-osxphotos-add-locations-not-reference"],
+            [0, "cmdoption-osxphotos-export-not-reference"],
+            [0, "cmdoption-osxphotos-query-not-reference"],
+            [0, "cmdoption-osxphotos-repl-not-reference"],
+            [0, "cmdoption-osxphotos-sync-not-reference"]
+        ],
+        "--not-saved-to-library": [
+            [0, "cmdoption-osxphotos-add-locations-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-export-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-query-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-repl-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-sync-not-saved-to-library"]
+        ],
+        "--not-screenshot": [
+            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
+            [0, "cmdoption-osxphotos-export-not-screenshot"],
+            [0, "cmdoption-osxphotos-query-not-screenshot"],
+            [0, "cmdoption-osxphotos-repl-not-screenshot"],
+            [0, "cmdoption-osxphotos-sync-not-screenshot"]
+        ],
+        "--not-selfie": [
+            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
+            [0, "cmdoption-osxphotos-export-not-selfie"],
+            [0, "cmdoption-osxphotos-query-not-selfie"],
+            [0, "cmdoption-osxphotos-repl-not-selfie"],
+            [0, "cmdoption-osxphotos-sync-not-selfie"]
+        ],
+        "--not-shared": [
+            [0, "cmdoption-osxphotos-add-locations-not-shared"],
+            [0, "cmdoption-osxphotos-export-not-shared"],
+            [0, "cmdoption-osxphotos-query-not-shared"],
+            [0, "cmdoption-osxphotos-repl-not-shared"]
+        ],
+        "--not-slow-mo": [
+            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
+            [0, "cmdoption-osxphotos-export-not-slow-mo"],
+            [0, "cmdoption-osxphotos-query-not-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-not-slow-mo"]
+        ],
+        "--not-syndicated": [
+            [0, "cmdoption-osxphotos-add-locations-not-syndicated"],
+            [0, "cmdoption-osxphotos-export-not-syndicated"],
+            [0, "cmdoption-osxphotos-query-not-syndicated"],
+            [0, "cmdoption-osxphotos-repl-not-syndicated"],
+            [0, "cmdoption-osxphotos-sync-not-syndicated"]
+        ],
+        "--not-time-lapse": [
+            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
+            [0, "cmdoption-osxphotos-export-not-time-lapse"],
+            [0, "cmdoption-osxphotos-query-not-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-not-time-lapse"]
+        ],
+        "--only-movies": [
+            [0, "cmdoption-osxphotos-add-locations-only-movies"],
+            [0, "cmdoption-osxphotos-export-only-movies"],
+            [0, "cmdoption-osxphotos-query-only-movies"],
+            [0, "cmdoption-osxphotos-repl-only-movies"],
+            [0, "cmdoption-osxphotos-sync-only-movies"]
+        ],
+        "--only-new": [
+            [0, "cmdoption-osxphotos-export-only-new"]
+        ],
+        "--only-photos": [
+            [0, "cmdoption-osxphotos-add-locations-only-photos"],
+            [0, "cmdoption-osxphotos-export-only-photos"],
+            [0, "cmdoption-osxphotos-query-only-photos"],
+            [0, "cmdoption-osxphotos-repl-only-photos"],
+            [0, "cmdoption-osxphotos-sync-only-photos"]
+        ],
+        "--original-suffix": [
+            [0, "cmdoption-osxphotos-export-original-suffix"]
+        ],
+        "--overwrite": [
+            [0, "cmdoption-osxphotos-export-overwrite"]
+        ],
+        "--panorama": [
+            [0, "cmdoption-osxphotos-add-locations-panorama"],
+            [0, "cmdoption-osxphotos-export-panorama"],
+            [0, "cmdoption-osxphotos-query-panorama"],
+            [0, "cmdoption-osxphotos-repl-panorama"],
+            [0, "cmdoption-osxphotos-sync-panorama"]
+        ],
+        "--parse-date": [
+            [0, "cmdoption-osxphotos-import-P"],
+            [0, "cmdoption-osxphotos-timewarp-M"]
+        ],
+        "--person": [
+            [0, "cmdoption-osxphotos-add-locations-person"],
+            [0, "cmdoption-osxphotos-export-person"],
+            [0, "cmdoption-osxphotos-query-person"],
+            [0, "cmdoption-osxphotos-repl-person"],
+            [0, "cmdoption-osxphotos-sync-person"]
+        ],
+        "--person-keyword": [
+            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
+            [0, "cmdoption-osxphotos-export-person-keyword"]
+        ],
+        "--place": [
+            [0, "cmdoption-osxphotos-add-locations-place"],
+            [0, "cmdoption-osxphotos-export-place"],
+            [0, "cmdoption-osxphotos-query-place"],
+            [0, "cmdoption-osxphotos-repl-place"],
+            [0, "cmdoption-osxphotos-sync-place"]
+        ],
+        "--plain": [
+            [0, "cmdoption-osxphotos-timewarp-plain"]
+        ],
+        "--portrait": [
+            [0, "cmdoption-osxphotos-add-locations-portrait"],
+            [0, "cmdoption-osxphotos-export-portrait"],
+            [0, "cmdoption-osxphotos-query-portrait"],
+            [0, "cmdoption-osxphotos-repl-portrait"],
+            [0, "cmdoption-osxphotos-sync-portrait"]
+        ],
+        "--post-command": [
+            [0, "cmdoption-osxphotos-export-post-command"]
+        ],
+        "--post-function": [
+            [0, "cmdoption-osxphotos-export-post-function"],
+            [0, "cmdoption-osxphotos-import-post-function"]
+        ],
+        "--preview": [
+            [0, "cmdoption-osxphotos-export-preview"],
+            [0, "cmdoption-osxphotos-theme-preview"]
+        ],
+        "--preview-if-missing": [
+            [0, "cmdoption-osxphotos-export-preview-if-missing"]
+        ],
+        "--preview-suffix": [
+            [0, "cmdoption-osxphotos-export-preview-suffix"]
+        ],
+        "--print": [
+            [0, "cmdoption-osxphotos-dump-print"],
+            [0, "cmdoption-osxphotos-export-print"],
+            [0, "cmdoption-osxphotos-query-print"]
+        ],
+        "--pull-exif": [
+            [0, "cmdoption-osxphotos-timewarp-P"]
+        ],
+        "--push-exif": [
+            [0, "cmdoption-osxphotos-timewarp-p"]
+        ],
+        "--query-eval": [
+            [0, "cmdoption-osxphotos-add-locations-query-eval"],
+            [0, "cmdoption-osxphotos-export-query-eval"],
+            [0, "cmdoption-osxphotos-query-query-eval"],
+            [0, "cmdoption-osxphotos-repl-query-eval"],
+            [0, "cmdoption-osxphotos-sync-query-eval"]
+        ],
+        "--query-function": [
+            [0, "cmdoption-osxphotos-add-locations-query-function"],
+            [0, "cmdoption-osxphotos-export-query-function"],
+            [0, "cmdoption-osxphotos-query-query-function"],
+            [0, "cmdoption-osxphotos-repl-query-function"],
+            [0, "cmdoption-osxphotos-sync-query-function"]
+        ],
+        "--quiet": [
+            [0, "cmdoption-osxphotos-query-quiet"]
+        ],
+        "--ramdb": [
+            [0, "cmdoption-osxphotos-export-ramdb"]
+        ],
+        "--raw-output": [
+            [0, "cmdoption-osxphotos-diff-r"]
+        ],
+        "--regex": [
+            [0, "cmdoption-osxphotos-add-locations-regex"],
+            [0, "cmdoption-osxphotos-export-regex"],
+            [0, "cmdoption-osxphotos-query-regex"],
+            [0, "cmdoption-osxphotos-repl-regex"],
+            [0, "cmdoption-osxphotos-sync-regex"]
+        ],
+        "--relative-to": [
+            [0, "cmdoption-osxphotos-import-r"]
+        ],
+        "--replace-keywords": [
+            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
+            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
+            [0, "cmdoption-osxphotos-export-replace-keywords"]
+        ],
+        "--report": [
+            [0, "cmdoption-osxphotos-exiftool-report"],
+            [0, "cmdoption-osxphotos-export-report"],
+            [0, "cmdoption-osxphotos-exportdb-report"],
+            [0, "cmdoption-osxphotos-import-report"],
+            [0, "cmdoption-osxphotos-sync-R"]
+        ],
+        "--resume": [
+            [0, "cmdoption-osxphotos-import-R"]
+        ],
+        "--retry": [
+            [0, "cmdoption-osxphotos-export-retry"]
+        ],
+        "--run": [
+            [0, "cmdoption-osxphotos-version-run"]
+        ],
+        "--save-config": [
+            [0, "cmdoption-osxphotos-exiftool-save-config"],
+            [0, "cmdoption-osxphotos-export-save-config"],
+            [0, "cmdoption-osxphotos-exportdb-save-config"]
+        ],
+        "--saved-to-library": [
+            [0, "cmdoption-osxphotos-add-locations-saved-to-library"],
+            [0, "cmdoption-osxphotos-export-saved-to-library"],
+            [0, "cmdoption-osxphotos-query-saved-to-library"],
+            [0, "cmdoption-osxphotos-repl-saved-to-library"],
+            [0, "cmdoption-osxphotos-sync-saved-to-library"]
+        ],
+        "--screenshot": [
+            [0, "cmdoption-osxphotos-add-locations-screenshot"],
+            [0, "cmdoption-osxphotos-export-screenshot"],
+            [0, "cmdoption-osxphotos-query-screenshot"],
+            [0, "cmdoption-osxphotos-repl-screenshot"],
+            [0, "cmdoption-osxphotos-sync-screenshot"]
+        ],
+        "--selected": [
+            [0, "cmdoption-osxphotos-add-locations-selected"],
+            [0, "cmdoption-osxphotos-export-selected"],
+            [0, "cmdoption-osxphotos-query-selected"],
+            [0, "cmdoption-osxphotos-repl-selected"],
+            [0, "cmdoption-osxphotos-sync-selected"]
+        ],
+        "--selfie": [
+            [0, "cmdoption-osxphotos-add-locations-selfie"],
+            [0, "cmdoption-osxphotos-export-selfie"],
+            [0, "cmdoption-osxphotos-query-selfie"],
+            [0, "cmdoption-osxphotos-repl-selfie"],
+            [0, "cmdoption-osxphotos-sync-selfie"]
+        ],
+        "--set": [
+            [0, "cmdoption-osxphotos-sync-s"]
+        ],
+        "--shared": [
+            [0, "cmdoption-osxphotos-add-locations-shared"],
+            [0, "cmdoption-osxphotos-export-shared"],
+            [0, "cmdoption-osxphotos-query-shared"],
+            [0, "cmdoption-osxphotos-repl-shared"]
+        ],
+        "--sidecar": [
+            [0, "cmdoption-osxphotos-export-sidecar"]
+        ],
+        "--sidecar-drop-ext": [
+            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"]
+        ],
+        "--skip-bursts": [
+            [0, "cmdoption-osxphotos-export-skip-bursts"]
+        ],
+        "--skip-edited": [
+            [0, "cmdoption-osxphotos-export-skip-edited"]
+        ],
+        "--skip-live": [
+            [0, "cmdoption-osxphotos-export-skip-live"]
+        ],
+        "--skip-original-if-edited": [
+            [0, "cmdoption-osxphotos-export-skip-original-if-edited"]
+        ],
+        "--skip-raw": [
+            [0, "cmdoption-osxphotos-export-skip-raw"]
+        ],
+        "--skip-uuid": [
+            [0, "cmdoption-osxphotos-export-skip-uuid"]
+        ],
+        "--skip-uuid-from-file": [
+            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"]
+        ],
+        "--slow-mo": [
+            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
+            [0, "cmdoption-osxphotos-export-slow-mo"],
+            [0, "cmdoption-osxphotos-query-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-slow-mo"]
+        ],
+        "--split-folder": [
+            [0, "cmdoption-osxphotos-import-f"]
+        ],
+        "--sql": [
+            [0, "cmdoption-osxphotos-exportdb-sql"]
+        ],
+        "--strip": [
+            [0, "cmdoption-osxphotos-export-strip"]
+        ],
+        "--style": [
+            [0, "cmdoption-osxphotos-diff-s"]
+        ],
+        "--syndicated": [
+            [0, "cmdoption-osxphotos-add-locations-syndicated"],
+            [0, "cmdoption-osxphotos-export-syndicated"],
+            [0, "cmdoption-osxphotos-query-syndicated"],
+            [0, "cmdoption-osxphotos-repl-syndicated"],
+            [0, "cmdoption-osxphotos-sync-syndicated"]
+        ],
+        "--template": [
+            [0, "cmdoption-osxphotos-inspect-T"]
+        ],
+        "--theme": [
+            [0, "cmdoption-osxphotos-add-locations-theme"],
+            [0, "cmdoption-osxphotos-batch-edit-theme"],
+            [0, "cmdoption-osxphotos-exiftool-theme"],
+            [0, "cmdoption-osxphotos-export-theme"],
+            [0, "cmdoption-osxphotos-exportdb-theme"],
+            [0, "cmdoption-osxphotos-import-theme"],
+            [0, "cmdoption-osxphotos-inspect-theme"],
+            [0, "cmdoption-osxphotos-orphans-theme"],
+            [0, "cmdoption-osxphotos-sync-theme"],
+            [0, "cmdoption-osxphotos-timewarp-theme"]
+        ],
+        "--time": [
+            [0, "cmdoption-osxphotos-timewarp-t"]
+        ],
+        "--time-delta": [
+            [0, "cmdoption-osxphotos-timewarp-T"]
+        ],
+        "--time-lapse": [
+            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
+            [0, "cmdoption-osxphotos-export-time-lapse"],
+            [0, "cmdoption-osxphotos-query-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-time-lapse"]
+        ],
+        "--timestamp": [
+            [0, "cmdoption-osxphotos-add-locations-timestamp"],
+            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
+            [0, "cmdoption-osxphotos-diff-timestamp"],
+            [0, "cmdoption-osxphotos-exiftool-timestamp"],
+            [0, "cmdoption-osxphotos-export-timestamp"],
+            [0, "cmdoption-osxphotos-exportdb-timestamp"],
+            [0, "cmdoption-osxphotos-import-timestamp"],
+            [0, "cmdoption-osxphotos-orphans-timestamp"],
+            [0, "cmdoption-osxphotos-sync-timestamp"],
+            [0, "cmdoption-osxphotos-timewarp-2"],
+            [0, "cmdoption-osxphotos-timewarp-timestamp"]
+        ],
+        "--timezone": [
+            [0, "cmdoption-osxphotos-timewarp-z"]
+        ],
+        "--title": [
+            [0, "cmdoption-osxphotos-add-locations-title"],
+            [0, "cmdoption-osxphotos-batch-edit-title"],
+            [0, "cmdoption-osxphotos-export-title"],
+            [0, "cmdoption-osxphotos-import-t"],
+            [0, "cmdoption-osxphotos-query-title"],
+            [0, "cmdoption-osxphotos-repl-title"],
+            [0, "cmdoption-osxphotos-sync-title"]
+        ],
+        "--tmpdir": [
+            [0, "cmdoption-osxphotos-export-tmpdir"]
+        ],
+        "--to-date": [
+            [0, "cmdoption-osxphotos-add-locations-to-date"],
+            [0, "cmdoption-osxphotos-export-to-date"],
+            [0, "cmdoption-osxphotos-query-to-date"],
+            [0, "cmdoption-osxphotos-repl-to-date"],
+            [0, "cmdoption-osxphotos-sync-to-date"]
+        ],
+        "--to-time": [
+            [0, "cmdoption-osxphotos-add-locations-to-time"],
+            [0, "cmdoption-osxphotos-export-to-time"],
+            [0, "cmdoption-osxphotos-query-to-time"],
+            [0, "cmdoption-osxphotos-repl-to-time"],
+            [0, "cmdoption-osxphotos-sync-to-time"]
+        ],
+        "--touch-file": [
+            [0, "cmdoption-osxphotos-export-touch-file"],
+            [0, "cmdoption-osxphotos-exportdb-touch-file"]
+        ],
+        "--undo": [
+            [0, "cmdoption-osxphotos-batch-edit-undo"]
+        ],
+        "--unmatched": [
+            [0, "cmdoption-osxphotos-sync-U"]
+        ],
+        "--update": [
+            [0, "cmdoption-osxphotos-export-update"]
+        ],
+        "--update-errors": [
+            [0, "cmdoption-osxphotos-export-update-errors"]
+        ],
+        "--update-signatures": [
+            [0, "cmdoption-osxphotos-exportdb-update-signatures"]
+        ],
+        "--upgrade": [
+            [0, "cmdoption-osxphotos-install-U"]
+        ],
+        "--use-file-time": [
+            [0, "cmdoption-osxphotos-timewarp-1"]
+        ],
+        "--use-photokit": [
+            [0, "cmdoption-osxphotos-export-use-photokit"]
+        ],
+        "--use-photos-export": [
+            [0, "cmdoption-osxphotos-export-use-photos-export"]
+        ],
+        "--uti": [
+            [0, "cmdoption-osxphotos-add-locations-uti"],
+            [0, "cmdoption-osxphotos-export-uti"],
+            [0, "cmdoption-osxphotos-query-uti"],
+            [0, "cmdoption-osxphotos-repl-uti"],
+            [0, "cmdoption-osxphotos-sync-uti"]
+        ],
+        "--uuid": [
+            [0, "cmdoption-osxphotos-add-locations-uuid"],
+            [0, "cmdoption-osxphotos-export-uuid"],
+            [0, "cmdoption-osxphotos-query-uuid"],
+            [0, "cmdoption-osxphotos-repl-uuid"],
+            [0, "cmdoption-osxphotos-sync-uuid"]
+        ],
+        "--uuid-files": [
+            [0, "cmdoption-osxphotos-exportdb-uuid-files"]
+        ],
+        "--uuid-from-file": [
+            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
+            [0, "cmdoption-osxphotos-export-uuid-from-file"],
+            [0, "cmdoption-osxphotos-query-uuid-from-file"],
+            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
+            [0, "cmdoption-osxphotos-sync-uuid-from-file"]
+        ],
+        "--uuid-info": [
+            [0, "cmdoption-osxphotos-exportdb-uuid-info"]
+        ],
+        "--vacuum": [
+            [0, "cmdoption-osxphotos-exportdb-vacuum"]
+        ],
+        "--verbose": [
+            [0, "cmdoption-osxphotos-add-locations-V"],
+            [0, "cmdoption-osxphotos-batch-edit-V"],
+            [0, "cmdoption-osxphotos-diff-V"],
+            [0, "cmdoption-osxphotos-exiftool-V"],
+            [0, "cmdoption-osxphotos-export-V"],
+            [0, "cmdoption-osxphotos-exportdb-V"],
+            [0, "cmdoption-osxphotos-import-V"],
+            [0, "cmdoption-osxphotos-orphans-V"],
+            [0, "cmdoption-osxphotos-sync-V"],
+            [0, "cmdoption-osxphotos-timewarp-V"]
+        ],
+        "--version": [
+            [0, "cmdoption-osxphotos-exportdb-version"],
+            [0, "cmdoption-osxphotos-v"]
+        ],
+        "--walk": [
+            [0, "cmdoption-osxphotos-import-w"]
+        ],
+        "--window": [
+            [0, "cmdoption-osxphotos-add-locations-w"]
+        ],
+        "--xattr-template": [
+            [0, "cmdoption-osxphotos-export-xattr-template"]
+        ],
+        "--year": [
+            [0, "cmdoption-osxphotos-add-locations-year"],
+            [0, "cmdoption-osxphotos-export-year"],
+            [0, "cmdoption-osxphotos-query-year"],
+            [0, "cmdoption-osxphotos-repl-year"],
+            [0, "cmdoption-osxphotos-sync-year"]
+        ],
+        "--yes": [
+            [0, "cmdoption-osxphotos-uninstall-y"]
+        ],
+        "-a": [
+            [0, "cmdoption-osxphotos-sync-A"],
+            [0, "cmdoption-osxphotos-import-a"],
+            [0, "cmdoption-osxphotos-timewarp-a"]
+        ],
+        "-c": [
+            [0, "cmdoption-osxphotos-import-C"],
+            [0, "cmdoption-osxphotos-timewarp-c"]
+        ],
+        "-d": [
+            [0, "cmdoption-osxphotos-import-D"],
+            [0, "cmdoption-osxphotos-timewarp-D"],
+            [0, "cmdoption-osxphotos-import-d"],
+            [0, "cmdoption-osxphotos-timewarp-d"]
+        ],
+        "-f": [
+            [0, "cmdoption-osxphotos-timewarp-F"],
+            [0, "cmdoption-osxphotos-dump-f"],
+            [0, "cmdoption-osxphotos-import-f"],
+            [0, "cmdoption-osxphotos-query-f"],
+            [0, "cmdoption-osxphotos-timewarp-1"],
+            [0, "cmdoption-osxphotos-uuid-f"]
+        ],
+        "-l": [
+            [0, "cmdoption-osxphotos-import-L"],
+            [0, "cmdoption-osxphotos-timewarp-L"],
+            [0, "cmdoption-osxphotos-import-l"]
+        ],
+        "-m": [
+            [0, "cmdoption-osxphotos-timewarp-M"],
+            [0, "cmdoption-osxphotos-import-m"],
+            [0, "cmdoption-osxphotos-sync-m"],
+            [0, "cmdoption-osxphotos-timewarp-0"]
+        ],
+        "-p": [
+            [0, "cmdoption-osxphotos-import-P"],
+            [0, "cmdoption-osxphotos-timewarp-P"],
+            [0, "cmdoption-osxphotos-import-0"],
+            [0, "cmdoption-osxphotos-timewarp-p"]
+        ],
+        "-r": [
+            [0, "cmdoption-osxphotos-import-R"],
+            [0, "cmdoption-osxphotos-sync-R"],
+            [0, "cmdoption-osxphotos-diff-r"],
+            [0, "cmdoption-osxphotos-import-r"]
+        ],
+        "-t": [
+            [0, "cmdoption-osxphotos-inspect-T"],
+            [0, "cmdoption-osxphotos-timewarp-T"],
+            [0, "cmdoption-osxphotos-import-t"],
+            [0, "cmdoption-osxphotos-inspect-t"],
+            [0, "cmdoption-osxphotos-timewarp-t"]
+        ],
+        "-u": [
+            [0, "cmdoption-osxphotos-install-U"],
+            [0, "cmdoption-osxphotos-sync-U"]
+        ],
+        "-v": [
+            [0, "cmdoption-osxphotos-add-locations-V"],
+            [0, "cmdoption-osxphotos-batch-edit-V"],
+            [0, "cmdoption-osxphotos-diff-V"],
+            [0, "cmdoption-osxphotos-exiftool-V"],
+            [0, "cmdoption-osxphotos-export-V"],
+            [0, "cmdoption-osxphotos-exportdb-V"],
+            [0, "cmdoption-osxphotos-import-V"],
+            [0, "cmdoption-osxphotos-orphans-V"],
+            [0, "cmdoption-osxphotos-sync-V"],
+            [0, "cmdoption-osxphotos-timewarp-V"],
+            [0, "cmdoption-osxphotos-v"]
+        ],
+        "-e": [
+            [0, "cmdoption-osxphotos-import-e"],
+            [0, "cmdoption-osxphotos-sync-e"],
+            [0, "cmdoption-osxphotos-timewarp-e"]
+        ],
+        "-g": [
+            [0, "cmdoption-osxphotos-import-g"]
+        ],
+        "-h": [
+            [0, "cmdoption-osxphotos-run-h"]
+        ],
+        "-i": [
+            [0, "cmdoption-osxphotos-add-locations-i"],
+            [0, "cmdoption-osxphotos-export-i"],
+            [0, "cmdoption-osxphotos-query-i"],
+            [0, "cmdoption-osxphotos-repl-i"],
+            [0, "cmdoption-osxphotos-sync-0"],
+            [0, "cmdoption-osxphotos-sync-i"],
+            [0, "cmdoption-osxphotos-timewarp-i"]
+        ],
+        "-k": [
+            [0, "cmdoption-osxphotos-import-k"]
+        ],
+        "-s": [
+            [0, "cmdoption-osxphotos-diff-s"],
+            [0, "cmdoption-osxphotos-sync-s"]
+        ],
+        "-w": [
+            [0, "cmdoption-osxphotos-add-locations-w"],
+            [0, "cmdoption-osxphotos-import-w"]
+        ],
+        "-y": [
+            [0, "cmdoption-osxphotos-uninstall-y"]
+        ],
+        "-z": [
+            [0, "cmdoption-osxphotos-timewarp-z"]
+        ],
+        "args": [
+            [0, "cmdoption-osxphotos-run-arg-ARGS"]
+        ],
+        "db2": [
+            [0, "cmdoption-osxphotos-diff-arg-DB2"]
+        ],
+        "dest": [
+            [0, "cmdoption-osxphotos-export-arg-DEST"]
+        ],
+        "export_database": [
+            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"]
+        ],
+        "export_directory": [
+            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"]
+        ],
+        "files": [
+            [0, "cmdoption-osxphotos-import-arg-FILES"]
+        ],
+        "packages": [
+            [0, "cmdoption-osxphotos-install-arg-PACKAGES"],
+            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"]
+        ],
+        "photos_library": [
+            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"]
+        ],
+        "python_file": [
+            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"]
+        ],
+        "subtopic": [
+            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"]
+        ],
+        "topic": [
+            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
+        ],
+        "uuid_or_name": [
+            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"]
+        ],
+        "width": [
+            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
+        ],
+        "osxphotos command line option": [
+            [0, "cmdoption-osxphotos-json"],
+            [0, "cmdoption-osxphotos-library"],
+            [0, "cmdoption-osxphotos-v"]
+        ],
+        "osxphotos-add-locations command line option": [
+            [0, "cmdoption-osxphotos-add-locations-V"],
+            [0, "cmdoption-osxphotos-add-locations-added-after"],
+            [0, "cmdoption-osxphotos-add-locations-added-before"],
+            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
+            [0, "cmdoption-osxphotos-add-locations-album"],
+            [0, "cmdoption-osxphotos-add-locations-burst"],
+            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
+            [0, "cmdoption-osxphotos-add-locations-description"],
+            [0, "cmdoption-osxphotos-add-locations-dry-run"],
+            [0, "cmdoption-osxphotos-add-locations-duplicate"],
+            [0, "cmdoption-osxphotos-add-locations-edited"],
+            [0, "cmdoption-osxphotos-add-locations-exif"],
+            [0, "cmdoption-osxphotos-add-locations-external-edit"],
+            [0, "cmdoption-osxphotos-add-locations-favorite"],
+            [0, "cmdoption-osxphotos-add-locations-folder"],
+            [0, "cmdoption-osxphotos-add-locations-from-date"],
+            [0, "cmdoption-osxphotos-add-locations-from-time"],
+            [0, "cmdoption-osxphotos-add-locations-has-comment"],
+            [0, "cmdoption-osxphotos-add-locations-has-likes"],
+            [0, "cmdoption-osxphotos-add-locations-has-raw"],
+            [0, "cmdoption-osxphotos-add-locations-hdr"],
+            [0, "cmdoption-osxphotos-add-locations-hidden"],
+            [0, "cmdoption-osxphotos-add-locations-i"],
+            [0, "cmdoption-osxphotos-add-locations-in-album"],
+            [0, "cmdoption-osxphotos-add-locations-incloud"],
+            [0, "cmdoption-osxphotos-add-locations-is-reference"],
+            [0, "cmdoption-osxphotos-add-locations-keyword"],
+            [0, "cmdoption-osxphotos-add-locations-label"],
+            [0, "cmdoption-osxphotos-add-locations-live"],
+            [0, "cmdoption-osxphotos-add-locations-location"],
+            [0, "cmdoption-osxphotos-add-locations-max-size"],
+            [0, "cmdoption-osxphotos-add-locations-min-size"],
+            [0, "cmdoption-osxphotos-add-locations-missing"],
+            [0, "cmdoption-osxphotos-add-locations-name"],
+            [0, "cmdoption-osxphotos-add-locations-no-comment"],
+            [0, "cmdoption-osxphotos-add-locations-no-description"],
+            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
+            [0, "cmdoption-osxphotos-add-locations-no-likes"],
+            [0, "cmdoption-osxphotos-add-locations-no-location"],
+            [0, "cmdoption-osxphotos-add-locations-no-place"],
+            [0, "cmdoption-osxphotos-add-locations-no-title"],
+            [0, "cmdoption-osxphotos-add-locations-not-burst"],
+            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
+            [0, "cmdoption-osxphotos-add-locations-not-edited"],
+            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
+            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
+            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
+            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
+            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
+            [0, "cmdoption-osxphotos-add-locations-not-live"],
+            [0, "cmdoption-osxphotos-add-locations-not-missing"],
+            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
+            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
+            [0, "cmdoption-osxphotos-add-locations-not-reference"],
+            [0, "cmdoption-osxphotos-add-locations-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
+            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
+            [0, "cmdoption-osxphotos-add-locations-not-shared"],
+            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
+            [0, "cmdoption-osxphotos-add-locations-not-syndicated"],
+            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
+            [0, "cmdoption-osxphotos-add-locations-only-movies"],
+            [0, "cmdoption-osxphotos-add-locations-only-photos"],
+            [0, "cmdoption-osxphotos-add-locations-panorama"],
+            [0, "cmdoption-osxphotos-add-locations-person"],
+            [0, "cmdoption-osxphotos-add-locations-place"],
+            [0, "cmdoption-osxphotos-add-locations-portrait"],
+            [0, "cmdoption-osxphotos-add-locations-query-eval"],
+            [0, "cmdoption-osxphotos-add-locations-query-function"],
+            [0, "cmdoption-osxphotos-add-locations-regex"],
+            [0, "cmdoption-osxphotos-add-locations-saved-to-library"],
+            [0, "cmdoption-osxphotos-add-locations-screenshot"],
+            [0, "cmdoption-osxphotos-add-locations-selected"],
+            [0, "cmdoption-osxphotos-add-locations-selfie"],
+            [0, "cmdoption-osxphotos-add-locations-shared"],
+            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
+            [0, "cmdoption-osxphotos-add-locations-syndicated"],
+            [0, "cmdoption-osxphotos-add-locations-theme"],
+            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
+            [0, "cmdoption-osxphotos-add-locations-timestamp"],
+            [0, "cmdoption-osxphotos-add-locations-title"],
+            [0, "cmdoption-osxphotos-add-locations-to-date"],
+            [0, "cmdoption-osxphotos-add-locations-to-time"],
+            [0, "cmdoption-osxphotos-add-locations-uti"],
+            [0, "cmdoption-osxphotos-add-locations-uuid"],
+            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
+            [0, "cmdoption-osxphotos-add-locations-w"],
+            [0, "cmdoption-osxphotos-add-locations-year"]
+        ],
+        "osxphotos-albums command line option": [
+            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-albums-json"],
+            [0, "cmdoption-osxphotos-albums-library"]
+        ],
+        "osxphotos-batch-edit command line option": [
+            [0, "cmdoption-osxphotos-batch-edit-V"],
+            [0, "cmdoption-osxphotos-batch-edit-description"],
+            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
+            [0, "cmdoption-osxphotos-batch-edit-keyword"],
+            [0, "cmdoption-osxphotos-batch-edit-library"],
+            [0, "cmdoption-osxphotos-batch-edit-location"],
+            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
+            [0, "cmdoption-osxphotos-batch-edit-theme"],
+            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
+            [0, "cmdoption-osxphotos-batch-edit-title"],
+            [0, "cmdoption-osxphotos-batch-edit-undo"]
+        ],
+        "osxphotos-diff command line option": [
+            [0, "cmdoption-osxphotos-diff-V"],
+            [0, "cmdoption-osxphotos-diff-arg-DB2"],
+            [0, "cmdoption-osxphotos-diff-library"],
+            [0, "cmdoption-osxphotos-diff-r"],
+            [0, "cmdoption-osxphotos-diff-s"],
+            [0, "cmdoption-osxphotos-diff-timestamp"]
+        ],
+        "osxphotos-dump command line option": [
+            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-dump-deleted"],
+            [0, "cmdoption-osxphotos-dump-deleted-only"],
+            [0, "cmdoption-osxphotos-dump-f"],
+            [0, "cmdoption-osxphotos-dump-json"],
+            [0, "cmdoption-osxphotos-dump-library"],
+            [0, "cmdoption-osxphotos-dump-print"]
+        ],
+        "osxphotos-exiftool command line option": [
+            [0, "cmdoption-osxphotos-exiftool-V"],
+            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
+            [0, "cmdoption-osxphotos-exiftool-append"],
+            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"],
+            [0, "cmdoption-osxphotos-exiftool-db-config"],
+            [0, "cmdoption-osxphotos-exiftool-description-template"],
+            [0, "cmdoption-osxphotos-exiftool-dry-run"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
+            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
+            [0, "cmdoption-osxphotos-exiftool-exportdb"],
+            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
+            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
+            [0, "cmdoption-osxphotos-exiftool-library"],
+            [0, "cmdoption-osxphotos-exiftool-load-config"],
+            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
+            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
+            [0, "cmdoption-osxphotos-exiftool-report"],
+            [0, "cmdoption-osxphotos-exiftool-save-config"],
+            [0, "cmdoption-osxphotos-exiftool-theme"],
+            [0, "cmdoption-osxphotos-exiftool-timestamp"]
+        ],
+        "osxphotos-export command line option": [
+            [0, "cmdoption-osxphotos-export-V"],
+            [0, "cmdoption-osxphotos-export-add-exported-to-album"],
+            [0, "cmdoption-osxphotos-export-add-missing-to-album"],
+            [0, "cmdoption-osxphotos-export-add-skipped-to-album"],
+            [0, "cmdoption-osxphotos-export-added-after"],
+            [0, "cmdoption-osxphotos-export-added-before"],
+            [0, "cmdoption-osxphotos-export-added-in-last"],
+            [0, "cmdoption-osxphotos-export-album"],
+            [0, "cmdoption-osxphotos-export-album-keyword"],
+            [0, "cmdoption-osxphotos-export-alt-copy"],
+            [0, "cmdoption-osxphotos-export-append"],
+            [0, "cmdoption-osxphotos-export-arg-DEST"],
+            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-export-burst"],
+            [0, "cmdoption-osxphotos-export-cleanup"],
+            [0, "cmdoption-osxphotos-export-cloudasset"],
+            [0, "cmdoption-osxphotos-export-config-only"],
+            [0, "cmdoption-osxphotos-export-convert-to-jpeg"],
+            [0, "cmdoption-osxphotos-export-current-name"],
+            [0, "cmdoption-osxphotos-export-deleted"],
+            [0, "cmdoption-osxphotos-export-deleted-only"],
+            [0, "cmdoption-osxphotos-export-description"],
+            [0, "cmdoption-osxphotos-export-description-template"],
+            [0, "cmdoption-osxphotos-export-directory"],
+            [0, "cmdoption-osxphotos-export-download-missing"],
+            [0, "cmdoption-osxphotos-export-dry-run"],
+            [0, "cmdoption-osxphotos-export-duplicate"],
+            [0, "cmdoption-osxphotos-export-edited"],
+            [0, "cmdoption-osxphotos-export-edited-suffix"],
+            [0, "cmdoption-osxphotos-export-exif"],
+            [0, "cmdoption-osxphotos-export-exiftool"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"],
+            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"],
+            [0, "cmdoption-osxphotos-export-exiftool-option"],
+            [0, "cmdoption-osxphotos-export-exiftool-path"],
+            [0, "cmdoption-osxphotos-export-export-as-hardlink"],
+            [0, "cmdoption-osxphotos-export-export-by-date"],
+            [0, "cmdoption-osxphotos-export-exportdb"],
+            [0, "cmdoption-osxphotos-export-external-edit"],
+            [0, "cmdoption-osxphotos-export-favorite"],
+            [0, "cmdoption-osxphotos-export-favorite-rating"],
+            [0, "cmdoption-osxphotos-export-filename"],
+            [0, "cmdoption-osxphotos-export-finder-tag-keywords"],
+            [0, "cmdoption-osxphotos-export-finder-tag-template"],
+            [0, "cmdoption-osxphotos-export-folder"],
+            [0, "cmdoption-osxphotos-export-force-update"],
+            [0, "cmdoption-osxphotos-export-from-date"],
+            [0, "cmdoption-osxphotos-export-from-time"],
+            [0, "cmdoption-osxphotos-export-has-comment"],
+            [0, "cmdoption-osxphotos-export-has-likes"],
+            [0, "cmdoption-osxphotos-export-has-raw"],
+            [0, "cmdoption-osxphotos-export-hdr"],
+            [0, "cmdoption-osxphotos-export-hidden"],
+            [0, "cmdoption-osxphotos-export-i"],
+            [0, "cmdoption-osxphotos-export-ignore-date-modified"],
+            [0, "cmdoption-osxphotos-export-ignore-signature"],
+            [0, "cmdoption-osxphotos-export-in-album"],
+            [0, "cmdoption-osxphotos-export-incloud"],
+            [0, "cmdoption-osxphotos-export-is-reference"],
+            [0, "cmdoption-osxphotos-export-jpeg-ext"],
+            [0, "cmdoption-osxphotos-export-jpeg-quality"],
+            [0, "cmdoption-osxphotos-export-keep"],
+            [0, "cmdoption-osxphotos-export-keyword"],
+            [0, "cmdoption-osxphotos-export-keyword-template"],
+            [0, "cmdoption-osxphotos-export-label"],
+            [0, "cmdoption-osxphotos-export-library"],
+            [0, "cmdoption-osxphotos-export-limit"],
+            [0, "cmdoption-osxphotos-export-live"],
+            [0, "cmdoption-osxphotos-export-load-config"],
+            [0, "cmdoption-osxphotos-export-location"],
+            [0, "cmdoption-osxphotos-export-max-size"],
+            [0, "cmdoption-osxphotos-export-min-size"],
+            [0, "cmdoption-osxphotos-export-missing"],
+            [0, "cmdoption-osxphotos-export-name"],
+            [0, "cmdoption-osxphotos-export-no-comment"],
+            [0, "cmdoption-osxphotos-export-no-description"],
+            [0, "cmdoption-osxphotos-export-no-keyword"],
+            [0, "cmdoption-osxphotos-export-no-likes"],
+            [0, "cmdoption-osxphotos-export-no-location"],
+            [0, "cmdoption-osxphotos-export-no-place"],
+            [0, "cmdoption-osxphotos-export-no-progress"],
+            [0, "cmdoption-osxphotos-export-no-title"],
+            [0, "cmdoption-osxphotos-export-not-burst"],
+            [0, "cmdoption-osxphotos-export-not-cloudasset"],
+            [0, "cmdoption-osxphotos-export-not-edited"],
+            [0, "cmdoption-osxphotos-export-not-favorite"],
+            [0, "cmdoption-osxphotos-export-not-hdr"],
+            [0, "cmdoption-osxphotos-export-not-hidden"],
+            [0, "cmdoption-osxphotos-export-not-in-album"],
+            [0, "cmdoption-osxphotos-export-not-incloud"],
+            [0, "cmdoption-osxphotos-export-not-live"],
+            [0, "cmdoption-osxphotos-export-not-missing"],
+            [0, "cmdoption-osxphotos-export-not-panorama"],
+            [0, "cmdoption-osxphotos-export-not-portrait"],
+            [0, "cmdoption-osxphotos-export-not-reference"],
+            [0, "cmdoption-osxphotos-export-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-export-not-screenshot"],
+            [0, "cmdoption-osxphotos-export-not-selfie"],
+            [0, "cmdoption-osxphotos-export-not-shared"],
+            [0, "cmdoption-osxphotos-export-not-slow-mo"],
+            [0, "cmdoption-osxphotos-export-not-syndicated"],
+            [0, "cmdoption-osxphotos-export-not-time-lapse"],
+            [0, "cmdoption-osxphotos-export-only-movies"],
+            [0, "cmdoption-osxphotos-export-only-new"],
+            [0, "cmdoption-osxphotos-export-only-photos"],
+            [0, "cmdoption-osxphotos-export-original-suffix"],
+            [0, "cmdoption-osxphotos-export-overwrite"],
+            [0, "cmdoption-osxphotos-export-panorama"],
+            [0, "cmdoption-osxphotos-export-person"],
+            [0, "cmdoption-osxphotos-export-person-keyword"],
+            [0, "cmdoption-osxphotos-export-place"],
+            [0, "cmdoption-osxphotos-export-portrait"],
+            [0, "cmdoption-osxphotos-export-post-command"],
+            [0, "cmdoption-osxphotos-export-post-function"],
+            [0, "cmdoption-osxphotos-export-preview"],
+            [0, "cmdoption-osxphotos-export-preview-if-missing"],
+            [0, "cmdoption-osxphotos-export-preview-suffix"],
+            [0, "cmdoption-osxphotos-export-print"],
+            [0, "cmdoption-osxphotos-export-query-eval"],
+            [0, "cmdoption-osxphotos-export-query-function"],
+            [0, "cmdoption-osxphotos-export-ramdb"],
+            [0, "cmdoption-osxphotos-export-regex"],
+            [0, "cmdoption-osxphotos-export-replace-keywords"],
+            [0, "cmdoption-osxphotos-export-report"],
+            [0, "cmdoption-osxphotos-export-retry"],
+            [0, "cmdoption-osxphotos-export-save-config"],
+            [0, "cmdoption-osxphotos-export-saved-to-library"],
+            [0, "cmdoption-osxphotos-export-screenshot"],
+            [0, "cmdoption-osxphotos-export-selected"],
+            [0, "cmdoption-osxphotos-export-selfie"],
+            [0, "cmdoption-osxphotos-export-shared"],
+            [0, "cmdoption-osxphotos-export-sidecar"],
+            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"],
+            [0, "cmdoption-osxphotos-export-skip-bursts"],
+            [0, "cmdoption-osxphotos-export-skip-edited"],
+            [0, "cmdoption-osxphotos-export-skip-live"],
+            [0, "cmdoption-osxphotos-export-skip-original-if-edited"],
+            [0, "cmdoption-osxphotos-export-skip-raw"],
+            [0, "cmdoption-osxphotos-export-skip-uuid"],
+            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"],
+            [0, "cmdoption-osxphotos-export-slow-mo"],
+            [0, "cmdoption-osxphotos-export-strip"],
+            [0, "cmdoption-osxphotos-export-syndicated"],
+            [0, "cmdoption-osxphotos-export-theme"],
+            [0, "cmdoption-osxphotos-export-time-lapse"],
+            [0, "cmdoption-osxphotos-export-timestamp"],
+            [0, "cmdoption-osxphotos-export-title"],
+            [0, "cmdoption-osxphotos-export-tmpdir"],
+            [0, "cmdoption-osxphotos-export-to-date"],
+            [0, "cmdoption-osxphotos-export-to-time"],
+            [0, "cmdoption-osxphotos-export-touch-file"],
+            [0, "cmdoption-osxphotos-export-update"],
+            [0, "cmdoption-osxphotos-export-update-errors"],
+            [0, "cmdoption-osxphotos-export-use-photokit"],
+            [0, "cmdoption-osxphotos-export-use-photos-export"],
+            [0, "cmdoption-osxphotos-export-uti"],
+            [0, "cmdoption-osxphotos-export-uuid"],
+            [0, "cmdoption-osxphotos-export-uuid-from-file"],
+            [0, "cmdoption-osxphotos-export-xattr-template"],
+            [0, "cmdoption-osxphotos-export-year"]
+        ],
+        "osxphotos-exportdb command line option": [
+            [0, "cmdoption-osxphotos-exportdb-V"],
+            [0, "cmdoption-osxphotos-exportdb-append"],
+            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"],
+            [0, "cmdoption-osxphotos-exportdb-check-signatures"],
+            [0, "cmdoption-osxphotos-exportdb-delete-file"],
+            [0, "cmdoption-osxphotos-exportdb-delete-uuid"],
+            [0, "cmdoption-osxphotos-exportdb-dry-run"],
+            [0, "cmdoption-osxphotos-exportdb-errors"],
+            [0, "cmdoption-osxphotos-exportdb-export-dir"],
+            [0, "cmdoption-osxphotos-exportdb-info"],
+            [0, "cmdoption-osxphotos-exportdb-last-errors"],
+            [0, "cmdoption-osxphotos-exportdb-last-run"],
+            [0, "cmdoption-osxphotos-exportdb-migrate"],
+            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"],
+            [0, "cmdoption-osxphotos-exportdb-report"],
+            [0, "cmdoption-osxphotos-exportdb-save-config"],
+            [0, "cmdoption-osxphotos-exportdb-sql"],
+            [0, "cmdoption-osxphotos-exportdb-theme"],
+            [0, "cmdoption-osxphotos-exportdb-timestamp"],
+            [0, "cmdoption-osxphotos-exportdb-touch-file"],
+            [0, "cmdoption-osxphotos-exportdb-update-signatures"],
+            [0, "cmdoption-osxphotos-exportdb-uuid-files"],
+            [0, "cmdoption-osxphotos-exportdb-uuid-info"],
+            [0, "cmdoption-osxphotos-exportdb-vacuum"],
+            [0, "cmdoption-osxphotos-exportdb-version"]
+        ],
+        "osxphotos-help command line option": [
+            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"],
+            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
+        ],
+        "osxphotos-import command line option": [
+            [0, "cmdoption-osxphotos-import-0"],
+            [0, "cmdoption-osxphotos-import-C"],
+            [0, "cmdoption-osxphotos-import-D"],
+            [0, "cmdoption-osxphotos-import-L"],
+            [0, "cmdoption-osxphotos-import-P"],
+            [0, "cmdoption-osxphotos-import-R"],
+            [0, "cmdoption-osxphotos-import-V"],
+            [0, "cmdoption-osxphotos-import-a"],
+            [0, "cmdoption-osxphotos-import-append"],
+            [0, "cmdoption-osxphotos-import-arg-FILES"],
+            [0, "cmdoption-osxphotos-import-check-templates"],
+            [0, "cmdoption-osxphotos-import-d"],
+            [0, "cmdoption-osxphotos-import-e"],
+            [0, "cmdoption-osxphotos-import-f"],
+            [0, "cmdoption-osxphotos-import-g"],
+            [0, "cmdoption-osxphotos-import-k"],
+            [0, "cmdoption-osxphotos-import-l"],
+            [0, "cmdoption-osxphotos-import-m"],
+            [0, "cmdoption-osxphotos-import-no-progress"],
+            [0, "cmdoption-osxphotos-import-post-function"],
+            [0, "cmdoption-osxphotos-import-r"],
+            [0, "cmdoption-osxphotos-import-report"],
+            [0, "cmdoption-osxphotos-import-t"],
+            [0, "cmdoption-osxphotos-import-theme"],
+            [0, "cmdoption-osxphotos-import-timestamp"],
+            [0, "cmdoption-osxphotos-import-w"]
+        ],
+        "osxphotos-info command line option": [
+            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-info-json"],
+            [0, "cmdoption-osxphotos-info-library"]
+        ],
+        "osxphotos-inspect command line option": [
+            [0, "cmdoption-osxphotos-inspect-T"],
+            [0, "cmdoption-osxphotos-inspect-library"],
+            [0, "cmdoption-osxphotos-inspect-t"],
+            [0, "cmdoption-osxphotos-inspect-theme"]
+        ],
+        "osxphotos-install command line option": [
+            [0, "cmdoption-osxphotos-install-U"],
+            [0, "cmdoption-osxphotos-install-arg-PACKAGES"]
+        ],
+        "osxphotos-keywords command line option": [
+            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-keywords-json"],
+            [0, "cmdoption-osxphotos-keywords-library"]
+        ],
+        "osxphotos-labels command line option": [
+            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-labels-json"],
+            [0, "cmdoption-osxphotos-labels-library"]
+        ],
+        "osxphotos-list command line option": [
+            [0, "cmdoption-osxphotos-list-json"]
+        ],
+        "osxphotos-orphans command line option": [
+            [0, "cmdoption-osxphotos-orphans-V"],
+            [0, "cmdoption-osxphotos-orphans-export"],
+            [0, "cmdoption-osxphotos-orphans-library"],
+            [0, "cmdoption-osxphotos-orphans-theme"],
+            [0, "cmdoption-osxphotos-orphans-timestamp"]
+        ],
+        "osxphotos-persons command line option": [
+            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-persons-json"],
+            [0, "cmdoption-osxphotos-persons-library"]
+        ],
+        "osxphotos-places command line option": [
+            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-places-json"],
+            [0, "cmdoption-osxphotos-places-library"]
+        ],
+        "osxphotos-query command line option": [
+            [0, "cmdoption-osxphotos-query-add-to-album"],
+            [0, "cmdoption-osxphotos-query-added-after"],
+            [0, "cmdoption-osxphotos-query-added-before"],
+            [0, "cmdoption-osxphotos-query-added-in-last"],
+            [0, "cmdoption-osxphotos-query-album"],
+            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"],
+            [0, "cmdoption-osxphotos-query-burst"],
+            [0, "cmdoption-osxphotos-query-cloudasset"],
+            [0, "cmdoption-osxphotos-query-count"],
+            [0, "cmdoption-osxphotos-query-deleted"],
+            [0, "cmdoption-osxphotos-query-deleted-only"],
+            [0, "cmdoption-osxphotos-query-description"],
+            [0, "cmdoption-osxphotos-query-duplicate"],
+            [0, "cmdoption-osxphotos-query-edited"],
+            [0, "cmdoption-osxphotos-query-exif"],
+            [0, "cmdoption-osxphotos-query-external-edit"],
+            [0, "cmdoption-osxphotos-query-f"],
+            [0, "cmdoption-osxphotos-query-favorite"],
+            [0, "cmdoption-osxphotos-query-folder"],
+            [0, "cmdoption-osxphotos-query-from-date"],
+            [0, "cmdoption-osxphotos-query-from-time"],
+            [0, "cmdoption-osxphotos-query-has-comment"],
+            [0, "cmdoption-osxphotos-query-has-likes"],
+            [0, "cmdoption-osxphotos-query-has-raw"],
+            [0, "cmdoption-osxphotos-query-hdr"],
+            [0, "cmdoption-osxphotos-query-hidden"],
+            [0, "cmdoption-osxphotos-query-i"],
+            [0, "cmdoption-osxphotos-query-in-album"],
+            [0, "cmdoption-osxphotos-query-incloud"],
+            [0, "cmdoption-osxphotos-query-is-reference"],
+            [0, "cmdoption-osxphotos-query-json"],
+            [0, "cmdoption-osxphotos-query-keyword"],
+            [0, "cmdoption-osxphotos-query-label"],
+            [0, "cmdoption-osxphotos-query-library"],
+            [0, "cmdoption-osxphotos-query-live"],
+            [0, "cmdoption-osxphotos-query-location"],
+            [0, "cmdoption-osxphotos-query-max-size"],
+            [0, "cmdoption-osxphotos-query-min-size"],
+            [0, "cmdoption-osxphotos-query-missing"],
+            [0, "cmdoption-osxphotos-query-name"],
+            [0, "cmdoption-osxphotos-query-no-comment"],
+            [0, "cmdoption-osxphotos-query-no-description"],
+            [0, "cmdoption-osxphotos-query-no-keyword"],
+            [0, "cmdoption-osxphotos-query-no-likes"],
+            [0, "cmdoption-osxphotos-query-no-location"],
+            [0, "cmdoption-osxphotos-query-no-place"],
+            [0, "cmdoption-osxphotos-query-no-title"],
+            [0, "cmdoption-osxphotos-query-not-burst"],
+            [0, "cmdoption-osxphotos-query-not-cloudasset"],
+            [0, "cmdoption-osxphotos-query-not-edited"],
+            [0, "cmdoption-osxphotos-query-not-favorite"],
+            [0, "cmdoption-osxphotos-query-not-hdr"],
+            [0, "cmdoption-osxphotos-query-not-hidden"],
+            [0, "cmdoption-osxphotos-query-not-in-album"],
+            [0, "cmdoption-osxphotos-query-not-incloud"],
+            [0, "cmdoption-osxphotos-query-not-live"],
+            [0, "cmdoption-osxphotos-query-not-missing"],
+            [0, "cmdoption-osxphotos-query-not-panorama"],
+            [0, "cmdoption-osxphotos-query-not-portrait"],
+            [0, "cmdoption-osxphotos-query-not-reference"],
+            [0, "cmdoption-osxphotos-query-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-query-not-screenshot"],
+            [0, "cmdoption-osxphotos-query-not-selfie"],
+            [0, "cmdoption-osxphotos-query-not-shared"],
+            [0, "cmdoption-osxphotos-query-not-slow-mo"],
+            [0, "cmdoption-osxphotos-query-not-syndicated"],
+            [0, "cmdoption-osxphotos-query-not-time-lapse"],
+            [0, "cmdoption-osxphotos-query-only-movies"],
+            [0, "cmdoption-osxphotos-query-only-photos"],
+            [0, "cmdoption-osxphotos-query-panorama"],
+            [0, "cmdoption-osxphotos-query-person"],
+            [0, "cmdoption-osxphotos-query-place"],
+            [0, "cmdoption-osxphotos-query-portrait"],
+            [0, "cmdoption-osxphotos-query-print"],
+            [0, "cmdoption-osxphotos-query-query-eval"],
+            [0, "cmdoption-osxphotos-query-query-function"],
+            [0, "cmdoption-osxphotos-query-quiet"],
+            [0, "cmdoption-osxphotos-query-regex"],
+            [0, "cmdoption-osxphotos-query-saved-to-library"],
+            [0, "cmdoption-osxphotos-query-screenshot"],
+            [0, "cmdoption-osxphotos-query-selected"],
+            [0, "cmdoption-osxphotos-query-selfie"],
+            [0, "cmdoption-osxphotos-query-shared"],
+            [0, "cmdoption-osxphotos-query-slow-mo"],
+            [0, "cmdoption-osxphotos-query-syndicated"],
+            [0, "cmdoption-osxphotos-query-time-lapse"],
+            [0, "cmdoption-osxphotos-query-title"],
+            [0, "cmdoption-osxphotos-query-to-date"],
+            [0, "cmdoption-osxphotos-query-to-time"],
+            [0, "cmdoption-osxphotos-query-uti"],
+            [0, "cmdoption-osxphotos-query-uuid"],
+            [0, "cmdoption-osxphotos-query-uuid-from-file"],
+            [0, "cmdoption-osxphotos-query-year"]
+        ],
+        "osxphotos-repl command line option": [
+            [0, "cmdoption-osxphotos-repl-added-after"],
+            [0, "cmdoption-osxphotos-repl-added-before"],
+            [0, "cmdoption-osxphotos-repl-added-in-last"],
+            [0, "cmdoption-osxphotos-repl-album"],
+            [0, "cmdoption-osxphotos-repl-burst"],
+            [0, "cmdoption-osxphotos-repl-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-deleted"],
+            [0, "cmdoption-osxphotos-repl-deleted-only"],
+            [0, "cmdoption-osxphotos-repl-description"],
+            [0, "cmdoption-osxphotos-repl-duplicate"],
+            [0, "cmdoption-osxphotos-repl-edited"],
+            [0, "cmdoption-osxphotos-repl-emacs"],
+            [0, "cmdoption-osxphotos-repl-exif"],
+            [0, "cmdoption-osxphotos-repl-external-edit"],
+            [0, "cmdoption-osxphotos-repl-favorite"],
+            [0, "cmdoption-osxphotos-repl-folder"],
+            [0, "cmdoption-osxphotos-repl-from-date"],
+            [0, "cmdoption-osxphotos-repl-from-time"],
+            [0, "cmdoption-osxphotos-repl-has-comment"],
+            [0, "cmdoption-osxphotos-repl-has-likes"],
+            [0, "cmdoption-osxphotos-repl-has-raw"],
+            [0, "cmdoption-osxphotos-repl-hdr"],
+            [0, "cmdoption-osxphotos-repl-hidden"],
+            [0, "cmdoption-osxphotos-repl-i"],
+            [0, "cmdoption-osxphotos-repl-in-album"],
+            [0, "cmdoption-osxphotos-repl-incloud"],
+            [0, "cmdoption-osxphotos-repl-is-reference"],
+            [0, "cmdoption-osxphotos-repl-keyword"],
+            [0, "cmdoption-osxphotos-repl-label"],
+            [0, "cmdoption-osxphotos-repl-library"],
+            [0, "cmdoption-osxphotos-repl-live"],
+            [0, "cmdoption-osxphotos-repl-location"],
+            [0, "cmdoption-osxphotos-repl-max-size"],
+            [0, "cmdoption-osxphotos-repl-min-size"],
+            [0, "cmdoption-osxphotos-repl-missing"],
+            [0, "cmdoption-osxphotos-repl-name"],
+            [0, "cmdoption-osxphotos-repl-no-comment"],
+            [0, "cmdoption-osxphotos-repl-no-description"],
+            [0, "cmdoption-osxphotos-repl-no-keyword"],
+            [0, "cmdoption-osxphotos-repl-no-likes"],
+            [0, "cmdoption-osxphotos-repl-no-location"],
+            [0, "cmdoption-osxphotos-repl-no-place"],
+            [0, "cmdoption-osxphotos-repl-no-title"],
+            [0, "cmdoption-osxphotos-repl-not-burst"],
+            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
+            [0, "cmdoption-osxphotos-repl-not-edited"],
+            [0, "cmdoption-osxphotos-repl-not-favorite"],
+            [0, "cmdoption-osxphotos-repl-not-hdr"],
+            [0, "cmdoption-osxphotos-repl-not-hidden"],
+            [0, "cmdoption-osxphotos-repl-not-in-album"],
+            [0, "cmdoption-osxphotos-repl-not-incloud"],
+            [0, "cmdoption-osxphotos-repl-not-live"],
+            [0, "cmdoption-osxphotos-repl-not-missing"],
+            [0, "cmdoption-osxphotos-repl-not-panorama"],
+            [0, "cmdoption-osxphotos-repl-not-portrait"],
+            [0, "cmdoption-osxphotos-repl-not-reference"],
+            [0, "cmdoption-osxphotos-repl-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-repl-not-screenshot"],
+            [0, "cmdoption-osxphotos-repl-not-selfie"],
+            [0, "cmdoption-osxphotos-repl-not-shared"],
+            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-not-syndicated"],
+            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-only-movies"],
+            [0, "cmdoption-osxphotos-repl-only-photos"],
+            [0, "cmdoption-osxphotos-repl-panorama"],
+            [0, "cmdoption-osxphotos-repl-person"],
+            [0, "cmdoption-osxphotos-repl-place"],
+            [0, "cmdoption-osxphotos-repl-portrait"],
+            [0, "cmdoption-osxphotos-repl-query-eval"],
+            [0, "cmdoption-osxphotos-repl-query-function"],
+            [0, "cmdoption-osxphotos-repl-regex"],
+            [0, "cmdoption-osxphotos-repl-saved-to-library"],
+            [0, "cmdoption-osxphotos-repl-screenshot"],
+            [0, "cmdoption-osxphotos-repl-selected"],
+            [0, "cmdoption-osxphotos-repl-selfie"],
+            [0, "cmdoption-osxphotos-repl-shared"],
+            [0, "cmdoption-osxphotos-repl-slow-mo"],
+            [0, "cmdoption-osxphotos-repl-syndicated"],
+            [0, "cmdoption-osxphotos-repl-time-lapse"],
+            [0, "cmdoption-osxphotos-repl-title"],
+            [0, "cmdoption-osxphotos-repl-to-date"],
+            [0, "cmdoption-osxphotos-repl-to-time"],
+            [0, "cmdoption-osxphotos-repl-uti"],
+            [0, "cmdoption-osxphotos-repl-uuid"],
+            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
+            [0, "cmdoption-osxphotos-repl-year"]
+        ],
+        "osxphotos-run command line option": [
+            [0, "cmdoption-osxphotos-run-arg-ARGS"],
+            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"],
+            [0, "cmdoption-osxphotos-run-h"]
+        ],
+        "osxphotos-show command line option": [
+            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"],
+            [0, "cmdoption-osxphotos-show-library"]
+        ],
+        "osxphotos-snap command line option": [
+            [0, "cmdoption-osxphotos-snap-library"]
+        ],
+        "osxphotos-sync command line option": [
+            [0, "cmdoption-osxphotos-sync-0"],
+            [0, "cmdoption-osxphotos-sync-A"],
+            [0, "cmdoption-osxphotos-sync-R"],
+            [0, "cmdoption-osxphotos-sync-U"],
+            [0, "cmdoption-osxphotos-sync-V"],
+            [0, "cmdoption-osxphotos-sync-added-after"],
+            [0, "cmdoption-osxphotos-sync-added-before"],
+            [0, "cmdoption-osxphotos-sync-added-in-last"],
+            [0, "cmdoption-osxphotos-sync-album"],
+            [0, "cmdoption-osxphotos-sync-burst"],
+            [0, "cmdoption-osxphotos-sync-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-description"],
+            [0, "cmdoption-osxphotos-sync-dry-run"],
+            [0, "cmdoption-osxphotos-sync-duplicate"],
+            [0, "cmdoption-osxphotos-sync-e"],
+            [0, "cmdoption-osxphotos-sync-edited"],
+            [0, "cmdoption-osxphotos-sync-exif"],
+            [0, "cmdoption-osxphotos-sync-external-edit"],
+            [0, "cmdoption-osxphotos-sync-favorite"],
+            [0, "cmdoption-osxphotos-sync-folder"],
+            [0, "cmdoption-osxphotos-sync-from-date"],
+            [0, "cmdoption-osxphotos-sync-from-time"],
+            [0, "cmdoption-osxphotos-sync-has-comment"],
+            [0, "cmdoption-osxphotos-sync-has-likes"],
+            [0, "cmdoption-osxphotos-sync-has-raw"],
+            [0, "cmdoption-osxphotos-sync-hdr"],
+            [0, "cmdoption-osxphotos-sync-hidden"],
+            [0, "cmdoption-osxphotos-sync-i"],
+            [0, "cmdoption-osxphotos-sync-in-album"],
+            [0, "cmdoption-osxphotos-sync-incloud"],
+            [0, "cmdoption-osxphotos-sync-is-reference"],
+            [0, "cmdoption-osxphotos-sync-keyword"],
+            [0, "cmdoption-osxphotos-sync-label"],
+            [0, "cmdoption-osxphotos-sync-library"],
+            [0, "cmdoption-osxphotos-sync-live"],
+            [0, "cmdoption-osxphotos-sync-location"],
+            [0, "cmdoption-osxphotos-sync-m"],
+            [0, "cmdoption-osxphotos-sync-max-size"],
+            [0, "cmdoption-osxphotos-sync-min-size"],
+            [0, "cmdoption-osxphotos-sync-missing"],
+            [0, "cmdoption-osxphotos-sync-name"],
+            [0, "cmdoption-osxphotos-sync-no-comment"],
+            [0, "cmdoption-osxphotos-sync-no-description"],
+            [0, "cmdoption-osxphotos-sync-no-keyword"],
+            [0, "cmdoption-osxphotos-sync-no-likes"],
+            [0, "cmdoption-osxphotos-sync-no-location"],
+            [0, "cmdoption-osxphotos-sync-no-place"],
+            [0, "cmdoption-osxphotos-sync-no-title"],
+            [0, "cmdoption-osxphotos-sync-not-burst"],
+            [0, "cmdoption-osxphotos-sync-not-cloudasset"],
+            [0, "cmdoption-osxphotos-sync-not-edited"],
+            [0, "cmdoption-osxphotos-sync-not-favorite"],
+            [0, "cmdoption-osxphotos-sync-not-hdr"],
+            [0, "cmdoption-osxphotos-sync-not-hidden"],
+            [0, "cmdoption-osxphotos-sync-not-in-album"],
+            [0, "cmdoption-osxphotos-sync-not-incloud"],
+            [0, "cmdoption-osxphotos-sync-not-live"],
+            [0, "cmdoption-osxphotos-sync-not-missing"],
+            [0, "cmdoption-osxphotos-sync-not-panorama"],
+            [0, "cmdoption-osxphotos-sync-not-portrait"],
+            [0, "cmdoption-osxphotos-sync-not-reference"],
+            [0, "cmdoption-osxphotos-sync-not-saved-to-library"],
+            [0, "cmdoption-osxphotos-sync-not-screenshot"],
+            [0, "cmdoption-osxphotos-sync-not-selfie"],
+            [0, "cmdoption-osxphotos-sync-not-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-not-syndicated"],
+            [0, "cmdoption-osxphotos-sync-not-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-only-movies"],
+            [0, "cmdoption-osxphotos-sync-only-photos"],
+            [0, "cmdoption-osxphotos-sync-panorama"],
+            [0, "cmdoption-osxphotos-sync-person"],
+            [0, "cmdoption-osxphotos-sync-place"],
+            [0, "cmdoption-osxphotos-sync-portrait"],
+            [0, "cmdoption-osxphotos-sync-query-eval"],
+            [0, "cmdoption-osxphotos-sync-query-function"],
+            [0, "cmdoption-osxphotos-sync-regex"],
+            [0, "cmdoption-osxphotos-sync-s"],
+            [0, "cmdoption-osxphotos-sync-saved-to-library"],
+            [0, "cmdoption-osxphotos-sync-screenshot"],
+            [0, "cmdoption-osxphotos-sync-selected"],
+            [0, "cmdoption-osxphotos-sync-selfie"],
+            [0, "cmdoption-osxphotos-sync-slow-mo"],
+            [0, "cmdoption-osxphotos-sync-syndicated"],
+            [0, "cmdoption-osxphotos-sync-theme"],
+            [0, "cmdoption-osxphotos-sync-time-lapse"],
+            [0, "cmdoption-osxphotos-sync-timestamp"],
+            [0, "cmdoption-osxphotos-sync-title"],
+            [0, "cmdoption-osxphotos-sync-to-date"],
+            [0, "cmdoption-osxphotos-sync-to-time"],
+            [0, "cmdoption-osxphotos-sync-uti"],
+            [0, "cmdoption-osxphotos-sync-uuid"],
+            [0, "cmdoption-osxphotos-sync-uuid-from-file"],
+            [0, "cmdoption-osxphotos-sync-year"]
+        ],
+        "osxphotos-theme command line option": [
+            [0, "cmdoption-osxphotos-theme-clone"],
+            [0, "cmdoption-osxphotos-theme-config"],
+            [0, "cmdoption-osxphotos-theme-default"],
+            [0, "cmdoption-osxphotos-theme-delete"],
+            [0, "cmdoption-osxphotos-theme-edit"],
+            [0, "cmdoption-osxphotos-theme-list"],
+            [0, "cmdoption-osxphotos-theme-preview"]
+        ],
+        "osxphotos-timewarp command line option": [
+            [0, "cmdoption-osxphotos-timewarp-0"],
+            [0, "cmdoption-osxphotos-timewarp-1"],
+            [0, "cmdoption-osxphotos-timewarp-2"],
+            [0, "cmdoption-osxphotos-timewarp-D"],
+            [0, "cmdoption-osxphotos-timewarp-F"],
+            [0, "cmdoption-osxphotos-timewarp-L"],
+            [0, "cmdoption-osxphotos-timewarp-M"],
+            [0, "cmdoption-osxphotos-timewarp-P"],
+            [0, "cmdoption-osxphotos-timewarp-T"],
+            [0, "cmdoption-osxphotos-timewarp-V"],
+            [0, "cmdoption-osxphotos-timewarp-a"],
+            [0, "cmdoption-osxphotos-timewarp-c"],
+            [0, "cmdoption-osxphotos-timewarp-d"],
+            [0, "cmdoption-osxphotos-timewarp-date-added"],
+            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"],
+            [0, "cmdoption-osxphotos-timewarp-e"],
+            [0, "cmdoption-osxphotos-timewarp-force"],
+            [0, "cmdoption-osxphotos-timewarp-i"],
+            [0, "cmdoption-osxphotos-timewarp-p"],
+            [0, "cmdoption-osxphotos-timewarp-plain"],
+            [0, "cmdoption-osxphotos-timewarp-t"],
+            [0, "cmdoption-osxphotos-timewarp-theme"],
+            [0, "cmdoption-osxphotos-timewarp-timestamp"],
+            [0, "cmdoption-osxphotos-timewarp-z"]
+        ],
+        "osxphotos-tutorial command line option": [
+            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
+        ],
+        "osxphotos-uninstall command line option": [
+            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"],
+            [0, "cmdoption-osxphotos-uninstall-y"]
+        ],
+        "osxphotos-uuid command line option": [
+            [0, "cmdoption-osxphotos-uuid-f"]
+        ],
+        "osxphotos-version command line option": [
+            [0, "cmdoption-osxphotos-version-run"]
+        ],
+        "albuminfo (class in osxphotos)": [
+            [4, "osxphotos.AlbumInfo"]
+        ],
+        "albumsortorder (class in osxphotos)": [
+            [4, "osxphotos.AlbumSortOrder"]
+        ],
+        "commentinfo (class in osxphotos)": [
+            [4, "osxphotos.CommentInfo"]
+        ],
+        "exifinfo (class in osxphotos)": [
+            [4, "osxphotos.ExifInfo"]
+        ],
+        "exiftool (class in osxphotos)": [
+            [4, "osxphotos.ExifTool"]
+        ],
+        "exportdb (class in osxphotos)": [
+            [4, "osxphotos.ExportDB"]
+        ],
+        "exportdbtemp (class in osxphotos)": [
+            [4, "osxphotos.ExportDBTemp"]
+        ],
+        "exportoptions (class in osxphotos)": [
+            [4, "osxphotos.ExportOptions"]
+        ],
+        "exportresults (class in osxphotos)": [
+            [4, "osxphotos.ExportResults"]
+        ],
+        "fileutil (class in osxphotos)": [
+            [4, "osxphotos.FileUtil"]
+        ],
+        "fileutilnoop (class in osxphotos)": [
+            [4, "osxphotos.FileUtilNoOp"]
+        ],
+        "folderinfo (class in osxphotos)": [
+            [4, "osxphotos.FolderInfo"]
+        ],
+        "importinfo (class in osxphotos)": [
+            [4, "osxphotos.ImportInfo"]
+        ],
+        "likeinfo (class in osxphotos)": [
+            [4, "osxphotos.LikeInfo"]
+        ],
+        "momentinfo (class in osxphotos)": [
+            [4, "osxphotos.MomentInfo"]
+        ],
+        "personinfo (class in osxphotos)": [
+            [4, "osxphotos.PersonInfo"]
+        ],
+        "photoexporter (class in osxphotos)": [
+            [4, "osxphotos.PhotoExporter"]
+        ],
+        "photoinfo (class in osxphotos)": [
+            [4, "osxphotos.PhotoInfo"]
+        ],
+        "phototemplate (class in osxphotos)": [
+            [4, "osxphotos.PhotoTemplate"]
+        ],
+        "photosalbum (class in osxphotos)": [
+            [4, "osxphotos.PhotosAlbum"]
+        ],
+        "photosalbumphotoscript (class in osxphotos)": [
+            [4, "osxphotos.PhotosAlbumPhotoScript"]
+        ],
+        "photosdb (class in osxphotos)": [
+            [4, "osxphotos.PhotosDB"]
+        ],
+        "placeinfo (class in osxphotos)": [
+            [4, "osxphotos.PlaceInfo"]
+        ],
+        "projectinfo (class in osxphotos)": [
+            [4, "osxphotos.ProjectInfo"]
+        ],
+        "queryoptions (class in osxphotos)": [
+            [4, "osxphotos.QueryOptions"]
+        ],
+        "scoreinfo (class in osxphotos)": [
+            [4, "osxphotos.ScoreInfo"]
+        ],
+        "searchinfo (class in osxphotos)": [
+            [4, "osxphotos.SearchInfo"]
+        ],
+        "activities (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.activities"]
+        ],
+        "added_after (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.added_after"]
+        ],
+        "added_before (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.added_before"]
+        ],
+        "added_in_last (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.added_in_last"]
+        ],
+        "addvalues() (osxphotos.exiftool method)": [
+            [4, "osxphotos.ExifTool.addvalues"]
+        ],
+        "adjustments (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.adjustments"]
+        ],
+        "album (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.album"]
+        ],
+        "album_info (osxphotos.folderinfo property)": [
+            [4, "osxphotos.FolderInfo.album_info"]
+        ],
+        "album_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.album_info"]
+        ],
+        "album_info (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.album_info"]
+        ],
+        "album_info_shared (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.album_info_shared"]
+        ],
+        "albums (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.albums"]
+        ],
+        "albums (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.albums"]
+        ],
+        "albums_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.albums_as_dict"]
+        ],
+        "albums_shared (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.albums_shared"]
+        ],
+        "albums_shared_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.albums_shared_as_dict"]
+        ],
+        "all (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.all"]
+        ],
+        "all_files() (osxphotos.exportresults method)": [
+            [4, "osxphotos.ExportResults.all_files"]
+        ],
+        "asdict() (osxphotos.albuminfo method)": [
+            [4, "osxphotos.AlbumInfo.asdict"]
+        ],
+        "asdict() (osxphotos.exiftool method)": [
+            [4, "osxphotos.ExifTool.asdict"]
+        ],
+        "asdict() (osxphotos.folderinfo method)": [
+            [4, "osxphotos.FolderInfo.asdict"]
+        ],
+        "asdict() (osxphotos.importinfo method)": [
+            [4, "osxphotos.ImportInfo.asdict"]
+        ],
+        "asdict() (osxphotos.momentinfo method)": [
+            [4, "osxphotos.MomentInfo.asdict"]
+        ],
+        "asdict() (osxphotos.personinfo method)": [
+            [4, "osxphotos.PersonInfo.asdict"]
+        ],
+        "asdict() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.asdict"]
+        ],
+        "asdict() (osxphotos.scoreinfo method)": [
+            [4, "osxphotos.ScoreInfo.asdict"]
+        ],
+        "asdict() (osxphotos.searchinfo method)": [
+            [4, "osxphotos.SearchInfo.asdict"]
+        ],
+        "attributes (osxphotos.exportresults property)": [
+            [4, "osxphotos.ExportResults.attributes"]
+        ],
+        "bit_flags (osxphotos.exportoptions property)": [
+            [4, "osxphotos.ExportOptions.bit_flags"]
+        ],
+        "bodies_of_water (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.bodies_of_water"]
+        ],
+        "burst (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst"]
+        ],
+        "burst (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.burst"]
+        ],
+        "burst_album_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_album_info"]
+        ],
+        "burst_albums (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_albums"]
+        ],
+        "burst_default_pick (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_default_pick"]
+        ],
+        "burst_key (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_key"]
+        ],
+        "burst_photos (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_photos"]
+        ],
+        "burst_photos (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.burst_photos"]
+        ],
+        "burst_selected (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.burst_selected"]
+        ],
+        "camera (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.camera"]
+        ],
+        "city (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.city"]
+        ],
+        "close() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.close"]
+        ],
+        "cloud_guid (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.cloud_guid"]
+        ],
+        "cloud_metadata (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.cloud_metadata"]
+        ],
+        "cloud_owner_hashed_id (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.cloud_owner_hashed_id"]
+        ],
+        "cloudasset (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.cloudasset"]
+        ],
+        "comments (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.comments"]
+        ],
+        "connection (osxphotos.exportdb property)": [
+            [4, "osxphotos.ExportDB.connection"]
+        ],
+        "convert_to_jpeg (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.convert_to_jpeg"]
+        ],
+        "convert_to_jpeg() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.convert_to_jpeg"]
+        ],
+        "copy() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.copy"]
+        ],
+        "country (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.country"]
+        ],
+        "create_file_record() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.create_file_record"]
+        ],
+        "create_or_get_file_record() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.create_or_get_file_record"]
+        ],
+        "date (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.date"]
+        ],
+        "date (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.date"]
+        ],
+        "date_added (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.date_added"]
+        ],
+        "date_modified (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.date_modified"]
+        ],
+        "date_trashed (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.date_trashed"]
+        ],
+        "datetime (osxphotos.exportresults property)": [
+            [4, "osxphotos.ExportResults.datetime"]
+        ],
+        "db_path (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.db_path"]
+        ],
+        "db_version (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.db_version"]
+        ],
+        "delete_data_for_filepath() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.delete_data_for_filepath"]
+        ],
+        "delete_data_for_uuid() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.delete_data_for_uuid"]
+        ],
+        "deleted (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.deleted"]
+        ],
+        "deleted_only (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.deleted_only"]
+        ],
+        "description (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.description"]
+        ],
+        "description (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.description"]
+        ],
+        "description_template (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.description_template"]
+        ],
+        "detected_text (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.detected_text"]
+        ],
+        "detected_text() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.detected_text"]
+        ],
+        "download_missing (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.download_missing"]
+        ],
+        "dry_run (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.dry_run"]
+        ],
+        "duplicate (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.duplicate"]
+        ],
+        "duplicates (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.duplicates"]
+        ],
+        "edited (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.edited"]
+        ],
+        "edited (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.edited"]
+        ],
+        "end_date (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.end_date"]
+        ],
+        "execute() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.execute"]
+        ],
+        "exif (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.exif"]
+        ],
+        "exif_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.exif_info"]
+        ],
+        "exiftool (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.exiftool"]
+        ],
+        "exiftool (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.exiftool"]
+        ],
+        "exiftool_flags (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.exiftool_flags"]
+        ],
+        "exiftool_json_sidecar() (osxphotos.photoexporter method)": [
+            [4, "osxphotos.PhotoExporter.exiftool_json_sidecar"]
+        ],
+        "expand_variables() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.expand_variables"]
+        ],
+        "expand_variables_to_str() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.expand_variables_to_str"]
+        ],
+        "export() (osxphotos.photoexporter method)": [
+            [4, "osxphotos.PhotoExporter.export"]
+        ],
+        "export() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.export"]
+        ],
+        "export_as_hardlink (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.export_as_hardlink"]
+        ],
+        "export_db (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.export_db"]
+        ],
+        "export_dir (osxphotos.exportdb property)": [
+            [4, "osxphotos.ExportDB.export_dir"]
+        ],
+        "external_edit (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.external_edit"]
+        ],
+        "external_edit (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.external_edit"]
+        ],
+        "face_info (osxphotos.personinfo property)": [
+            [4, "osxphotos.PersonInfo.face_info"]
+        ],
+        "face_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.face_info"]
+        ],
+        "face_regions (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.face_regions"]
+        ],
+        "favorite (osxphotos.personinfo property)": [
+            [4, "osxphotos.PersonInfo.favorite"]
+        ],
+        "favorite (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.favorite"]
+        ],
+        "favorite (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.favorite"]
+        ],
+        "favorite_rating (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.favorite_rating"]
+        ],
+        "feature_less (osxphotos.personinfo property)": [
+            [4, "osxphotos.PersonInfo.feature_less"]
+        ],
+        "file_sig() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.file_sig"]
+        ],
+        "filename (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.filename"]
+        ],
+        "fileutil (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.fileutil"]
+        ],
+        "filter_predicate() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.filter_predicate"]
+        ],
+        "fingerprint (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.fingerprint"]
+        ],
+        "folder (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.folder"]
+        ],
+        "folder_info (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.folder_info"]
+        ],
+        "folder_list (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.folder_list"]
+        ],
+        "folder_list (osxphotos.projectinfo property)": [
+            [4, "osxphotos.ProjectInfo.folder_list"]
+        ],
+        "folder_names (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.folder_names"]
+        ],
+        "folder_names (osxphotos.projectinfo property)": [
+            [4, "osxphotos.ProjectInfo.folder_names"]
+        ],
+        "folders (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.folders"]
+        ],
+        "force_update (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.force_update"]
+        ],
+        "from_date (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.from_date"]
+        ],
+        "function (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.function"]
+        ],
+        "get_db_connection() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.get_db_connection"]
+        ],
+        "get_export_results() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_export_results"]
+        ],
+        "get_exported_files() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_exported_files"]
+        ],
+        "get_field_values() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_field_values"]
+        ],
+        "get_file_record() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_file_record"]
+        ],
+        "get_files_for_uuid() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_files_for_uuid"]
+        ],
+        "get_filter_values() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_filter_values"]
+        ],
+        "get_format_values() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_format_values"]
+        ],
+        "get_media_type() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_media_type"]
+        ],
+        "get_photo() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.get_photo"]
+        ],
+        "get_photo_bool_attribute() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_photo_bool_attribute"]
+        ],
+        "get_photo_video_type() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_photo_video_type"]
+        ],
+        "get_photoinfo_for_uuid() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_photoinfo_for_uuid"]
+        ],
+        "get_previous_uuids() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_previous_uuids"]
+        ],
+        "get_target_for_file() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_target_for_file"]
+        ],
+        "get_template_value() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value"]
+        ],
+        "get_template_value_exiftool() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value_exiftool"]
+        ],
+        "get_template_value_filter_function() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value_filter_function"]
+        ],
+        "get_template_value_function() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value_function"]
+        ],
+        "get_template_value_multi() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value_multi"]
+        ],
+        "get_template_value_pathlib() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.get_template_value_pathlib"]
+        ],
+        "get_uuid_for_file() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.get_uuid_for_file"]
+        ],
+        "hardlink() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.hardlink"]
+        ],
+        "has_comment (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.has_comment"]
+        ],
+        "has_likes (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.has_likes"]
+        ],
+        "has_raw (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.has_raw"]
+        ],
+        "has_raw (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.has_raw"]
+        ],
+        "hasadjustments (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.hasadjustments"]
+        ],
+        "hdr (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.hdr"]
+        ],
+        "hdr (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.hdr"]
+        ],
+        "height (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.height"]
+        ],
+        "hexdigest (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.hexdigest"]
+        ],
+        "hidden (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.hidden"]
+        ],
+        "hidden (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.hidden"]
+        ],
+        "holidays (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.holidays"]
+        ],
+        "ignore_case (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.ignore_case"]
+        ],
+        "ignore_date_modified (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.ignore_date_modified"]
+        ],
+        "ignore_signature (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.ignore_signature"]
+        ],
+        "import_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.import_info"]
+        ],
+        "import_info (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.import_info"]
+        ],
+        "in_album (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.in_album"]
+        ],
+        "incloud (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.incloud"]
+        ],
+        "incloud (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.incloud"]
+        ],
+        "increment (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.increment"]
+        ],
+        "intrash (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.intrash"]
+        ],
+        "is_debug() (in module osxphotos)": [
+            [4, "osxphotos.is_debug"]
+        ],
+        "is_reference (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.is_reference"]
+        ],
+        "iscloudasset (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.iscloudasset"]
+        ],
+        "ismissing (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.ismissing"]
+        ],
+        "ismovie (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.ismovie"]
+        ],
+        "isphoto (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.isphoto"]
+        ],
+        "israw (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.israw"]
+        ],
+        "isreference (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.isreference"]
+        ],
+        "jpeg_ext (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.jpeg_ext"]
+        ],
+        "jpeg_quality (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.jpeg_quality"]
+        ],
+        "json() (osxphotos.exiftool method)": [
+            [4, "osxphotos.ExifTool.json"]
+        ],
+        "json() (osxphotos.personinfo method)": [
+            [4, "osxphotos.PersonInfo.json"]
+        ],
+        "json() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.json"]
+        ],
+        "keyword (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.keyword"]
+        ],
+        "keyword_template (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.keyword_template"]
+        ],
+        "keywords (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.keywords"]
+        ],
+        "keywords (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.keywords"]
+        ],
+        "keywords_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.keywords_as_dict"]
+        ],
+        "label (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.label"]
+        ],
+        "labels (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.labels"]
+        ],
+        "labels (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.labels"]
+        ],
+        "labels (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.labels"]
+        ],
+        "labels_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.labels_as_dict"]
+        ],
+        "labels_normalized (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.labels_normalized"]
+        ],
+        "labels_normalized (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.labels_normalized"]
+        ],
+        "labels_normalized_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.labels_normalized_as_dict"]
+        ],
+        "library_path (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.library_path"]
+        ],
+        "likes (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.likes"]
+        ],
+        "live (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.live"]
+        ],
+        "live_photo (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.live_photo"]
+        ],
+        "live_photo (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.live_photo"]
+        ],
+        "locality_names (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.locality_names"]
+        ],
+        "location (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.location"]
+        ],
+        "location (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.location"]
+        ],
+        "location (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.location"]
+        ],
+        "location (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.location"]
+        ],
+        "max_size (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.max_size"]
+        ],
+        "media_types (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.media_types"]
+        ],
+        "merge_exif_keywords (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.merge_exif_keywords"]
+        ],
+        "merge_exif_persons (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.merge_exif_persons"]
+        ],
+        "min_size (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.min_size"]
+        ],
+        "missing (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.missing"]
+        ],
+        "missing_bursts (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.missing_bursts"]
+        ],
+        "modification_date (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.modification_date"]
+        ],
+        "module": [
+            [4, "module-osxphotos"]
+        ],
+        "moment_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.moment_info"]
+        ],
+        "month (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.month"]
+        ],
+        "movies (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.movies"]
+        ],
+        "name (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.name"]
+        ],
+        "neighborhoods (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.neighborhoods"]
+        ],
+        "no_comment (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_comment"]
+        ],
+        "no_description (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_description"]
+        ],
+        "no_keyword (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_keyword"]
+        ],
+        "no_likes (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_likes"]
+        ],
+        "no_location (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_location"]
+        ],
+        "no_place (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_place"]
+        ],
+        "no_title (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.no_title"]
+        ],
+        "not_burst (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_burst"]
+        ],
+        "not_cloudasset (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_cloudasset"]
+        ],
+        "not_edited (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_edited"]
+        ],
+        "not_favorite (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_favorite"]
+        ],
+        "not_hdr (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_hdr"]
+        ],
+        "not_hidden (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_hidden"]
+        ],
+        "not_in_album (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_in_album"]
+        ],
+        "not_incloud (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_incloud"]
+        ],
+        "not_live (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_live"]
+        ],
+        "not_missing (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_missing"]
+        ],
+        "not_panorama (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_panorama"]
+        ],
+        "not_portrait (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_portrait"]
+        ],
+        "not_reference (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_reference"]
+        ],
+        "not_saved_to_library (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_saved_to_library"]
+        ],
+        "not_screenshot (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_screenshot"]
+        ],
+        "not_selfie (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_selfie"]
+        ],
+        "not_shared (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_shared"]
+        ],
+        "not_slow_mo (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_slow_mo"]
+        ],
+        "not_syndicated (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_syndicated"]
+        ],
+        "not_time_lapse (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_time_lapse"]
+        ],
+        "orientation (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.orientation"]
+        ],
+        "original_filename (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.original_filename"]
+        ],
+        "original_filesize (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.original_filesize"]
+        ],
+        "original_height (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.original_height"]
+        ],
+        "original_orientation (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.original_orientation"]
+        ],
+        "original_width (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.original_width"]
+        ],
+        "osxphotos": [
+            [4, "module-osxphotos"]
+        ],
+        "overwrite (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.overwrite"]
+        ],
+        "owner (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.owner"]
+        ],
+        "panorama (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.panorama"]
+        ],
+        "panorama (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.panorama"]
+        ],
+        "parent (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.parent"]
+        ],
+        "parent (osxphotos.folderinfo property)": [
+            [4, "osxphotos.FolderInfo.parent"]
+        ],
+        "path (osxphotos.exportdb property)": [
+            [4, "osxphotos.ExportDB.path"]
+        ],
+        "path (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path"]
+        ],
+        "path_derivatives (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path_derivatives"]
+        ],
+        "path_edited (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path_edited"]
+        ],
+        "path_edited_live_photo (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path_edited_live_photo"]
+        ],
+        "path_live_photo (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path_live_photo"]
+        ],
+        "path_raw (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.path_raw"]
+        ],
+        "person (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.person"]
+        ],
+        "person_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.person_info"]
+        ],
+        "person_info (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.person_info"]
+        ],
+        "persons (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.persons"]
+        ],
+        "persons (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.persons"]
+        ],
+        "persons (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.persons"]
+        ],
+        "persons_as_dict (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.persons_as_dict"]
+        ],
+        "photo_index() (osxphotos.albuminfo method)": [
+            [4, "osxphotos.AlbumInfo.photo_index"]
+        ],
+        "photos (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.photos"]
+        ],
+        "photos (osxphotos.importinfo property)": [
+            [4, "osxphotos.ImportInfo.photos"]
+        ],
+        "photos (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.photos"]
+        ],
+        "photos (osxphotos.personinfo property)": [
+            [4, "osxphotos.PersonInfo.photos"]
+        ],
+        "photos (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.photos"]
+        ],
+        "photos() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.photos"]
+        ],
+        "photos_by_uuid() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.photos_by_uuid"]
+        ],
+        "photos_version (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.photos_version"]
+        ],
+        "pid (osxphotos.exiftool property)": [
+            [4, "osxphotos.ExifTool.pid"]
+        ],
+        "pk (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.pk"]
+        ],
+        "place (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.place"]
+        ],
+        "place (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.place"]
+        ],
+        "place_names (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.place_names"]
+        ],
+        "portrait (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.portrait"]
+        ],
+        "portrait (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.portrait"]
+        ],
+        "preview (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.preview"]
+        ],
+        "preview_suffix (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.preview_suffix"]
+        ],
+        "project_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.project_info"]
+        ],
+        "project_info (osxphotos.photosdb property)": [
+            [4, "osxphotos.PhotosDB.project_info"]
+        ],
+        "query() (osxphotos.photosdb method)": [
+            [4, "osxphotos.PhotosDB.query"]
+        ],
+        "query_eval (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.query_eval"]
+        ],
+        "raw_original (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.raw_original"]
+        ],
+        "raw_photo (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.raw_photo"]
+        ],
+        "regex (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.regex"]
+        ],
+        "rename() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.rename"]
+        ],
+        "render() (osxphotos.phototemplate method)": [
+            [4, "osxphotos.PhotoTemplate.render"]
+        ],
+        "render_options (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.render_options"]
+        ],
+        "render_template() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.render_template"]
+        ],
+        "replace_keywords (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.replace_keywords"]
+        ],
+        "rich (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.rich"]
+        ],
+        "rmdir() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.rmdir"]
+        ],
+        "run_commands() (osxphotos.exiftool method)": [
+            [4, "osxphotos.ExifTool.run_commands"]
+        ],
+        "saved_to_library (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.saved_to_library"]
+        ],
+        "saved_to_library (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.saved_to_library"]
+        ],
+        "score (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.score"]
+        ],
+        "screenshot (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.screenshot"]
+        ],
+        "screenshot (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.screenshot"]
+        ],
+        "search_info (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.search_info"]
+        ],
+        "search_info_normalized (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.search_info_normalized"]
+        ],
+        "season (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.season"]
+        ],
+        "selected (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.selected"]
+        ],
+        "selfie (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.selfie"]
+        ],
+        "selfie (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.selfie"]
+        ],
+        "set_config() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.set_config"]
+        ],
+        "set_debug() (in module osxphotos)": [
+            [4, "osxphotos.set_debug"]
+        ],
+        "set_export_results() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.set_export_results"]
+        ],
+        "set_photoinfo_for_uuid() (osxphotos.exportdb method)": [
+            [4, "osxphotos.ExportDB.set_photoinfo_for_uuid"]
+        ],
+        "setvalue() (osxphotos.exiftool method)": [
+            [4, "osxphotos.ExifTool.setvalue"]
+        ],
+        "shared (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.shared"]
+        ],
+        "shared (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.shared"]
+        ],
+        "sidecar (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.sidecar"]
+        ],
+        "sidecar_drop_ext (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.sidecar_drop_ext"]
+        ],
+        "slow_mo (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.slow_mo"]
+        ],
+        "slow_mo (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.slow_mo"]
+        ],
+        "sort_order (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.sort_order"]
+        ],
+        "sort_order (osxphotos.personinfo property)": [
+            [4, "osxphotos.PersonInfo.sort_order"]
+        ],
+        "source (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.source"]
+        ],
+        "start_date (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.start_date"]
+        ],
+        "state (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.state"]
+        ],
+        "state_abbreviation (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.state_abbreviation"]
+        ],
+        "streets (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.streets"]
+        ],
+        "strip (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.strip"]
+        ],
+        "subfolders (osxphotos.folderinfo property)": [
+            [4, "osxphotos.FolderInfo.subfolders"]
+        ],
+        "subtitle (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.subtitle"]
+        ],
+        "syndicated (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.syndicated"]
+        ],
+        "syndicated (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.syndicated"]
+        ],
+        "tables() (osxphotos.photoinfo method)": [
+            [4, "osxphotos.PhotoInfo.tables"]
+        ],
+        "text_found (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.text_found"]
+        ],
+        "time_lapse (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.time_lapse"]
+        ],
+        "time_lapse (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.time_lapse"]
+        ],
+        "timeout (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.timeout"]
+        ],
+        "title (osxphotos.albuminfo property)": [
+            [4, "osxphotos.AlbumInfo.title"]
+        ],
+        "title (osxphotos.folderinfo property)": [
+            [4, "osxphotos.FolderInfo.title"]
+        ],
+        "title (osxphotos.importinfo property)": [
+            [4, "osxphotos.ImportInfo.title"]
+        ],
+        "title (osxphotos.momentinfo property)": [
+            [4, "osxphotos.MomentInfo.title"]
+        ],
+        "title (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.title"]
+        ],
+        "title (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.title"]
+        ],
+        "tmpdir (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.tmpdir"]
+        ],
+        "tmpdir() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.tmpdir"]
+        ],
+        "to_date (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.to_date"]
+        ],
+        "touch_file (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.touch_file"]
+        ],
+        "tzoffset (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.tzoffset"]
+        ],
+        "unlink() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.unlink"]
+        ],
+        "update (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.update"]
+        ],
+        "update_errors (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.update_errors"]
+        ],
+        "use_albums_as_keywords (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.use_albums_as_keywords"]
+        ],
+        "use_persons_as_keywords (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.use_persons_as_keywords"]
+        ],
+        "use_photokit (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.use_photokit"]
+        ],
+        "use_photos_export (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.use_photos_export"]
+        ],
+        "uti (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.uti"]
+        ],
+        "uti (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.uti"]
+        ],
+        "uti_edited (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.uti_edited"]
+        ],
+        "uti_original (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.uti_original"]
+        ],
+        "uti_raw (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.uti_raw"]
+        ],
+        "utime() (osxphotos.fileutilnoop class method)": [
+            [4, "osxphotos.FileUtilNoOp.utime"]
+        ],
+        "uuid (osxphotos.folderinfo property)": [
+            [4, "osxphotos.FolderInfo.uuid"]
+        ],
+        "uuid (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.uuid"]
+        ],
+        "uuid (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.uuid"]
+        ],
+        "venue_types (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.venue_types"]
+        ],
+        "venues (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.venues"]
+        ],
+        "verbose (osxphotos.exportoptions attribute)": [
+            [4, "osxphotos.ExportOptions.verbose"]
+        ],
+        "version (osxphotos.exiftool property)": [
+            [4, "osxphotos.ExifTool.version"]
+        ],
+        "visible (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.visible"]
+        ],
+        "width (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.width"]
+        ],
+        "write_exiftool_metadata_to_file() (osxphotos.photoexporter method)": [
+            [4, "osxphotos.PhotoExporter.write_exiftool_metadata_to_file"]
+        ],
+        "year (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.year"]
+        ],
+        "year (osxphotos.searchinfo property)": [
+            [4, "osxphotos.SearchInfo.year"]
+        ]
+    }
 })
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.60.4 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.60.4’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.60.5’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.60.4â
+{osxphotos_version}            The osxphotos version, e.g. â0.60.5â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.60.4 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.60.5 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.4_documentation
+osxphotos_0.60.5_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.60.4/osxphotos/exif_datetime_updater.py` & `osxphotos-0.60.5/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/exifinfo.py` & `osxphotos-0.60.5/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/exiftool.py` & `osxphotos-0.60.5/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/exiftool_filetypes.json` & `osxphotos-0.60.5/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/export_db.py` & `osxphotos-0.60.5/osxphotos/export_db.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from tenacity import retry, retry_if_not_exception_type, stop_after_attempt
 
 import osxphotos
 
 from ._constants import OSXPHOTOS_EXPORT_DB, SQLITE_CHECK_SAME_THREAD
 from ._version import __version__
 from .fileutil import FileUtil
-from .utils import normalize_fs_path
+from .unicode import normalize_fs_path
 
 __all__ = [
     "ExportDB",
     "ExportDBInMemory",
     "ExportDBTemp",
 ]
```

### Comparing `osxphotos-0.60.4/osxphotos/export_db_utils.py` & `osxphotos-0.60.5/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/fileutil.py` & `osxphotos-0.60.5/osxphotos/fileutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 import stat
 import tempfile
 import typing as t
 from abc import ABC, abstractmethod
 from tempfile import TemporaryDirectory
 
 from .imageconverter import ImageConverter
-from .utils import is_macos, normalize_fs_path
+from .platform import is_macos
+from .unicode import normalize_fs_path
 
 if is_macos:
     import Foundation
 
 __all__ = ["FileUtilABC", "FileUtilMacOS", "FileUtilShUtil", "FileUtil", "FileUtilNoOp"]
```

### Comparing `osxphotos-0.60.4/osxphotos/frozen_photoinfo.py` & `osxphotos-0.60.5/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/imageconverter.py` & `osxphotos-0.60.5/osxphotos/imageconverter.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 import pathlib
 import sys
 
 # needed to capture system-level stderr
 from wurlitzer import pipes
 
-from .utils import is_macos
+from .platform import is_macos
 
 if is_macos:
-    import objc
     import Metal
+    import objc
     import Quartz
     from Cocoa import NSURL
     from Foundation import NSDictionary
 
 __all__ = ["ImageConversionError", "ImageConverter"]
```

### Comparing `osxphotos-0.60.4/osxphotos/momentinfo.py` & `osxphotos-0.60.5/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/path_utils.py` & `osxphotos-0.60.5/osxphotos/path_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 This causes problems on other platforms, so we normalize as part of filename
 sanitization functions and rely on them being called every time a unique
 filename is needed.
 """
 
 import pathvalidate
 
-from osxphotos.utils import normalize_unicode
+from osxphotos.unicode import normalize_unicode
 
 from ._constants import MAX_DIRNAME_LEN, MAX_FILENAME_LEN
 
 __all__ = [
     "sanitize_filepath",
     "is_valid_filepath",
     "sanitize_filename",
```

### Comparing `osxphotos-0.60.4/osxphotos/personinfo.py` & `osxphotos-0.60.5/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/photodates.py` & `osxphotos-0.60.5/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/photoexporter.py` & `osxphotos-0.60.5/osxphotos/photoexporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,25 +32,25 @@
 )
 from ._version import __version__
 from .datetime_utils import datetime_tz_to_utc
 from .exiftool import ExifTool, ExifToolCaching, exiftool_can_write, get_exiftool_path
 from .export_db import ExportDB, ExportDBTemp
 from .fileutil import FileUtil
 from .phototemplate import RenderOptions
+from .platform import is_macos
 from .rich_utils import add_rich_markup_tag
+from .unicode import normalize_fs_path
 from .uti import get_preferred_uti_extension
 from .utils import (
     hexdigest,
     increment_filename,
     increment_filename_with_count,
-    is_macos,
     lineno,
     list_directory,
     lock_filename,
-    normalize_fs_path,
     unlock_filename,
 )
 
 if is_macos:
     import photoscript
 
     from .photokit import (
```

### Comparing `osxphotos-0.60.4/osxphotos/photoinfo.py` & `osxphotos-0.60.5/osxphotos/photoinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,19 +57,20 @@
 from .exiftool import ExifToolCaching, get_exiftool_path
 from .momentinfo import MomentInfo
 from .personinfo import FaceInfo, PersonInfo
 from .photoexporter import ExportOptions, PhotoExporter
 from .phototables import PhotoTables
 from .phototemplate import PhotoTemplate, RenderOptions
 from .placeinfo import PlaceInfo4, PlaceInfo5
+from .platform import assert_macos, is_macos
 from .query_builder import get_query
 from .scoreinfo import ScoreInfo
 from .searchinfo import SearchInfo
 from .uti import get_preferred_uti_extension, get_uti_for_extension
-from .utils import _get_resource_loc, assert_macos, hexdigest, is_macos, list_directory
+from .utils import _get_resource_loc, hexdigest, list_directory
 
 if is_macos:
     from osxmetadata import OSXMetaData
 
     from .text_detection import detect_text
 
 __all__ = ["PhotoInfo", "PhotoInfoNone", "frozen_photoinfo_factory"]
```

### Comparing `osxphotos-0.60.4/osxphotos/photokit.py` & `osxphotos-0.60.5/osxphotos/photokit.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,29 +19,31 @@
 
 import copy
 import pathlib
 import sys
 import threading
 import time
 
+from .platform import get_macos_version
+
 assert sys.platform == "darwin"
 
 import AVFoundation
 import CoreServices
 import Foundation
 import objc
 import Photos
 import Quartz
 from Foundation import NSNotificationCenter, NSObject
 from PyObjCTools import AppHelper
 from wurlitzer import pipes
 
 from .fileutil import FileUtil
 from .uti import get_preferred_uti_extension
-from .utils import get_macos_version, increment_filename
+from .utils import increment_filename
 
 __all__ = [
     "NSURL_to_path",
     "path_to_NSURL",
     "check_photokit_authorization",
     "request_photokit_authorization",
     "PhotoKitError",
```

### Comparing `osxphotos-0.60.4/osxphotos/photosalbum.py` & `osxphotos-0.60.5/osxphotos/photosalbum.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,58 @@
 """ PhotosAlbum class to create an album in default Photos library and add photos to it """
 
+from __future__ import annotations
+
+import unicodedata
 from typing import List, Optional
 
 from more_itertools import chunked
 
 from .photoinfo import PhotoInfo
-from .utils import assert_macos, noop, pluralize
+from .platform import assert_macos
+from .utils import noop, pluralize
 
 assert_macos()
 
 import photoscript
 from photoscript import Album, Folder, Photo, PhotosLibrary
 
 __all__ = ["PhotosAlbum", "PhotosAlbumPhotoScript"]
 
 
+def get_unicode_variants(s: str) -> list[str]:
+    """Get all unicode variants of string"""
+    variants = []
+    for form in ["NFC", "NFD", "NFKC", "NFKD"]:
+        normalized = unicodedata.normalize(form, s)
+        variants.append(normalized)
+    return variants
+
+
 def folder_by_path(folders: List[str], verbose: Optional[callable] = None) -> Folder:
     """Get (and create if necessary) a Photos Folder by path (passed as list of folder names)"""
     library = PhotosLibrary()
     verbose = verbose or noop
     top_folder_name = folders.pop(0)
-    top_folder = library.folder(top_folder_name, top_level=True)
-    if not top_folder:
+
+    for folder_variant in get_unicode_variants(top_folder_name):
+        top_folder = library.folder(folder_variant, top_level=True)
+        if top_folder is not None:
+            break
+    else:
         verbose(f"Creating folder '{top_folder_name}'")
         top_folder = library.create_folder(top_folder_name)
+
     current_folder = top_folder
     for folder_name in folders:
-        folder = current_folder.folder(folder_name)
-        if not folder:
+        for folder_variant in get_unicode_variants(folder_name):
+            folder = current_folder.folder(folder_variant)
+            if folder is not None:
+                break
+        else:
             verbose(f"Creating folder '{folder_name}'")
             folder = current_folder.create_folder(folder_name)
         current_folder = folder
     return current_folder
 
 
 def album_by_path(
@@ -40,23 +61,32 @@
     """Get (and create if necessary) a Photos Album by path (pass as list of folders, album name)"""
     library = PhotosLibrary()
     verbose = verbose or noop
     if len(folders_album) > 1:
         # have folders
         album_name = folders_album.pop()
         folder = folder_by_path(folders_album, verbose)
-        album = folder.album(album_name)
-        if album is None:
+        for album_variant in get_unicode_variants(album_name):
+            # Get album if it exists
+            # need to check every unicode variant to avoid creating duplicate albums with same visual representation (#1085)
+            album = folder.album(album_variant)
+            if album is not None:
+                break
+        else:
             verbose(f"Creating album '{album_name}'")
             album = folder.create_album(album_name)
     else:
         # only have album name
         album_name = folders_album[0]
-        album = library.album(album_name, top_level=True)
-        if album is None:
+        for album_variant in get_unicode_variants(album_name):
+            album = library.album(album_variant, top_level=True)
+            if album is not None:
+                break
+        else:
+            # album doesn't exist, create it
             verbose(f"Creating album '{album_name}'")
             album = library.create_album(album_name)
 
     return album
 
 
 class PhotosAlbum:
@@ -97,21 +127,18 @@
 
     def add_list(self, photo_list: List[PhotoInfo]):
         photos = []
         for p in photo_list:
             try:
                 photos.append(photoscript.Photo(p.uuid))
             except Exception as e:
-                print(f"Error creating Photo object for photo {self._format_uuid(p.uuid)}: {e}")
                 self.verbose(
                     f"Error creating Photo object for photo {self._format_uuid(p.uuid)}: {e}"
                 )
-        print(f"photos: {photos}")
         for photolist in chunked(photos, 10):
-            print(f"photolist: {photolist}")
             self.album.add(photolist)
         photo_len = len(photo_list)
         self.verbose(
             f"Added {self._format_num(photo_len)} {pluralize(photo_len, 'photo', 'photos')} to album {self._format_album(self.name)}"
         )
 
     def photos(self):
```

### Comparing `osxphotos-0.60.4/osxphotos/photoscript_utils.py` & `osxphotos-0.60.5/osxphotos/photoscript_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Utilities for creating photoscript objects from a name or UUID"""
 
 from __future__ import annotations
 
 import sqlite3
 
-from .utils import assert_macos
+from .platform import assert_macos
 
 assert_macos()
 
 import photoscript
 
 from ._constants import _DB_TABLE_NAMES, _PHOTOS_5_ALBUM_KIND, _PHOTOS_5_FOLDER_KIND
 from .photosdb.photosdb_utils import get_db_path_for_library, get_photos_library_version
```

### Comparing `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
     Do not import this module directly """
 
 import dataclasses
 import datetime
 from dataclasses import dataclass
 
 from .._constants import _DB_TABLE_NAMES, _PHOTOS_4_VERSION, TIME_DELTA
-from ..utils import normalize_unicode
 from ..sqlite_utils import sqlite_open_ro
+from ..unicode import normalize_unicode
 
 
 def _process_comments(self):
     """load the comments and likes data from the database
     this is a PhotosDB method that should be imported in
     the PhotosDB class definition in photosdb.py
     """
```

### Comparing `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ PhotosDB method for processing exif info 
     Do not import this module directly """
 
 import logging
 
 from .._constants import _DB_TABLE_NAMES, _PHOTOS_4_VERSION
-from ..sqlite_utils import sqlite_open_ro, sqlite_db_is_locked
+from ..sqlite_utils import sqlite_db_is_locked, sqlite_open_ro
 from .photosdb_utils import get_db_version
 
 
 def _process_exifinfo(self):
     """load the exif data from the database
     this is a PhotosDB method that should be imported in
     the PhotosDB class definition in photosdb.py
```

### Comparing `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Methods for PhotosDB to add Photos face info 
 """
 
 
 from .._constants import _DB_TABLE_NAMES, _PHOTOS_4_VERSION
 from ..sqlite_utils import sqlite_open_ro
-from ..utils import normalize_unicode
+from ..unicode import normalize_unicode
 from .photosdb_utils import get_db_version
 
 """
     This module should be imported in the class defintion of PhotosDB in photosdb.py
     Do not import this module directly
     This module adds the following method to PhotosDB:
         _process_faceinfo: process photo face info
```

### Comparing `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import logging
 import pathlib
 import uuid as uuidlib
 from functools import lru_cache
 
 from .._constants import _PHOTOS_4_VERSION, search_category_factory
 from ..sqlite_utils import sqlite_db_is_locked, sqlite_open_ro
-from ..utils import normalize_unicode
+from ..unicode import normalize_unicode
 
 """
     This module should be imported in the class defintion of PhotosDB in photosdb.py
     Do not import this module directly
     This module adds the following method to PhotosDB:
         _process_searchinfo: process search terms from psi.sqlite
```

### Comparing `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_syndicationinfo.py` & `osxphotos-0.60.5/osxphotos/photosdb/_photosdb_process_syndicationinfo.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Methods for PhotosDB to process Syndication info (#1054) """
 
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 from .._constants import _DB_TABLE_NAMES
 from ..sqlite_utils import sqlite_open_ro
 
-from typing import TYPE_CHECKING
-
 if TYPE_CHECKING:
     from osxphotos.photosdb import PhotosDB
 
 
 def _process_syndicationinfo(self: PhotosDB):
     """Process syndication information"""
```

### Comparing `osxphotos-0.60.4/osxphotos/photosdb/photosdb.py` & `osxphotos-0.60.5/osxphotos/photosdb/photosdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,25 +52,20 @@
 from .._version import __version__
 from ..albuminfo import AlbumInfo, FolderInfo, ImportInfo, ProjectInfo
 from ..datetime_utils import datetime_has_tz, datetime_naive_to_local
 from ..fileutil import FileUtil
 from ..personinfo import PersonInfo
 from ..photoinfo import PhotoInfo
 from ..phototemplate import RenderOptions
+from ..platform import get_macos_version, is_macos
 from ..queryoptions import QueryOptions
 from ..rich_utils import add_rich_markup_tag
 from ..sqlite_utils import sqlite_db_is_locked, sqlite_open_ro
-from ..utils import (
-    _check_file_exists,
-    is_macos,
-    get_macos_version,
-    get_last_library_path,
-    noop,
-    normalize_unicode,
-)
+from ..unicode import normalize_unicode
+from ..utils import _check_file_exists, get_last_library_path, noop
 from .photosdb_utils import get_db_model_version, get_db_version
 
 if is_macos:
     import photoscript
 
 logger = logging.getLogger("osxphotos")
```

### Comparing `osxphotos-0.60.4/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.60.5/osxphotos/photosdb/photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/phototables.py` & `osxphotos-0.60.5/osxphotos/phototables.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/phototemplate.cog.md` & `osxphotos-0.60.5/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/phototemplate.md` & `osxphotos-0.60.5/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/phototemplate.py` & `osxphotos-0.60.5/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/phototemplate.tx` & `osxphotos-0.60.5/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/phototz.py` & `osxphotos-0.60.5/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/placeinfo.py` & `osxphotos-0.60.5/osxphotos/placeinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 """
 from abc import ABC, abstractmethod
 from collections import namedtuple  # pylint: disable=syntax-error
 
 import yaml
 from bpylist2 import archiver
 
-from ._constants import UNICODE_FORMAT
-from .utils import normalize_unicode
+from .unicode import normalize_unicode
 
 __all__ = [
     "PLRevGeoLocationInfo",
     "PLRevGeoMapItem",
     "PLRevGeoMapItemAdditionalPlaceInfo",
     "CNPostalAddress",
     "PlaceInfo",
```

### Comparing `osxphotos-0.60.4/osxphotos/pyrepl.py` & `osxphotos-0.60.5/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.60.5/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/query_builder.py` & `osxphotos-0.60.5/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/queryoptions.py` & `osxphotos-0.60.5/osxphotos/queryoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/scoreinfo.py` & `osxphotos-0.60.5/osxphotos/scoreinfo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ ScoreInfo class to expose computed score info from the library """
 
-from dataclasses import dataclass, asdict
+from dataclasses import asdict, dataclass
 
 from ._constants import _PHOTOS_4_VERSION
 
 __all__ = ["ScoreInfo"]
 
 
 @dataclass(frozen=True)
```

### Comparing `osxphotos-0.60.4/osxphotos/searchinfo.py` & `osxphotos-0.60.5/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/sqlgrep.py` & `osxphotos-0.60.5/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/sqlite_utils.py` & `osxphotos-0.60.5/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/sqlitekvstore.py` & `osxphotos-0.60.5/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/template_counter.py` & `osxphotos-0.60.5/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.60.5/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.60.5/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/text_detection.py` & `osxphotos-0.60.5/osxphotos/text_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Use Apple's Vision Framework via PyObjC to perform text detection on images (macOS 10.15+ only) """
 
 import logging
 import sys
 from typing import List, Optional
 
-from .utils import assert_macos, get_macos_version
+from .platform import assert_macos, get_macos_version
 
 assert_macos()
 
 import objc
 import Quartz
 from Cocoa import NSURL
 from Foundation import NSDictionary
```

### Comparing `osxphotos-0.60.4/osxphotos/timeutils.py` & `osxphotos-0.60.5/osxphotos/timeutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Utilities for working with datetimes"""
 
 import datetime
-from typing import Optional
-
 import re
+from typing import Optional
 
 
 def utc_offset_string_to_seconds(utc_offset: str) -> int:
     """match a UTC offset in format ±[hh]:[mm], ±[h]:[mm], or ±[hh][mm] and return number of seconds offset"""
     patterns = [r"^([+-]?)(\d{1,2}):(\d{2})$", r"^([+-]?)(\d{2})(\d{2})$"]
     for pattern in patterns:
         match = re.match(pattern, utc_offset)
```

### Comparing `osxphotos-0.60.4/osxphotos/timezones.py` & `osxphotos-0.60.5/osxphotos/timezones.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Get list of valid timezones on macOS"""
 
 from typing import Union
 
-from .utils import is_macos
+from .platform import is_macos
 
 
 def format_offset_time(offset: int) -> str:
     """Format offset time to exiftool format: -04:00"""
     sign = "-" if offset < 0 else "+"
     hours, remainder = divmod(abs(offset), 3600)
     minutes, _ = divmod(remainder, 60)
```

### Comparing `osxphotos-0.60.4/osxphotos/tutorial.md` & `osxphotos-0.60.5/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/osxphotos/uti.py` & `osxphotos-0.60.5/osxphotos/uti.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import csv
 import re
 import subprocess
 import sys
 import tempfile
 
-from .utils import assert_macos, is_macos, get_macos_version
+from .platform import assert_macos, get_macos_version, is_macos
 
 if is_macos:
     import CoreServices
     import objc
 
 __all__ = ["get_preferred_uti_extension", "get_uti_for_extension"]
```

### Comparing `osxphotos-0.60.4/osxphotos/utils.py` & `osxphotos-0.60.5/osxphotos/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,70 +1,62 @@
 """ Utility functions used in osxphotos """
 
+from __future__ import annotations
+
 import datetime
 import fnmatch
 import hashlib
 import importlib
 import inspect
 import logging
 import os
 import os.path
 import pathlib
-import platform
 import re
 import subprocess
 import sys
-import unicodedata
 import urllib.parse
 from plistlib import load as plistload
-from typing import Any, Callable, List, Optional, Tuple, TypeVar, Union
+from typing import Callable, List, Optional, Tuple, TypeVar, Union
 from uuid import UUID
 
 import requests
 import shortuuid
 
-from ._constants import UNICODE_FORMAT
+from osxphotos.platform import get_macos_version, is_macos
+from osxphotos.unicode import normalize_fs_path
+
+T = TypeVar("T", bound=Union[str, pathlib.Path])
 
 logger = logging.getLogger("osxphotos")
 
+
 __all__ = [
-    "is_macos",
-    "assert_macos",
     "dd_to_dms_str",
     "expand_and_validate_filepath",
     "get_last_library_path",
-    "get_macos_version",
     "get_system_library_path",
     "hexdigest",
     "increment_filename_with_count",
     "increment_filename",
     "lineno",
     "list_directory",
     "list_photo_libraries",
     "load_function",
     "lock_filename",
     "noop",
-    "normalize_fs_path",
-    "normalize_unicode",
     "pluralize",
     "shortuuid_to_uuid",
     "uuid_to_shortuuid",
 ]
 
 
 VERSION_INFO_URL = "https://pypi.org/pypi/osxphotos/json"
 
 
-is_macos = sys.platform == "darwin"
-
-
-def assert_macos():
-    assert is_macos, "This feature only runs on macOS"
-
-
 if is_macos:
     import CoreFoundation
 
 
 def noop(*args, **kwargs):
     """do nothing (no operation)"""
     pass
@@ -74,33 +66,14 @@
     """Returns string with filename and current line number in caller as '(filename): line_num'
     Will trim filename to just the name, dropping path, if any."""
     line = inspect.currentframe().f_back.f_lineno
     filename = pathlib.Path(filename).name
     return f"{filename}: {line}"
 
 
-def get_macos_version():
-    assert_macos()
-    # returns tuple of str containing OS version
-    # e.g. 10.13.6 = ("10", "13", "6")
-    version = platform.mac_ver()[0].split(".")
-    if len(version) == 2:
-        (ver, major) = version
-        minor = "0"
-    elif len(version) == 3:
-        (ver, major, minor) = version
-    else:
-        raise (
-            ValueError(
-                f"Could not parse version string: {platform.mac_ver()} {version}"
-            )
-        )
-    return (ver, major, minor)
-
-
 def _check_file_exists(filename):
     """returns true if file exists and is not a directory
     otherwise returns false"""
     filename = os.path.abspath(filename)
     return os.path.exists(filename) and not os.path.isdir(filename)
 
 
@@ -276,24 +249,14 @@
     ).splitlines()
     for lib in output:
         lib_list.append(lib.decode("utf-8"))
     lib_list = sorted(set(lib_list))
     return lib_list
 
 
-T = TypeVar("T", bound=Union[str, pathlib.Path])
-
-
-def normalize_fs_path(path: T) -> T:
-    """Normalize filesystem paths with unicode in them"""
-    form = "NFD" if is_macos else "NFC"
-    if isinstance(path, pathlib.Path):
-        return pathlib.Path(unicodedata.normalize(form, str(path)))
-    else:
-        return unicodedata.normalize(form, path)
 
 
 # def findfiles(pattern, path):
 #     """Returns list of filenames from path matched by pattern
 #     shell pattern. Matching is case-insensitive.
 #     If 'path_' is invalid/doesn't exist, returns []."""
 #     if not os.path.isdir(path):
@@ -374,26 +337,14 @@
         files = [os.path.join(directory, f) for f in files]
     if is_pathlib:
         files = [pathlib.Path(f) for f in files]
 
     return files
 
 
-def normalize_unicode(value) -> Any:
-    """normalize unicode data"""
-    if value is None:
-        return None
-    if isinstance(value, (tuple, list)):
-        return tuple(unicodedata.normalize(UNICODE_FORMAT, v) for v in value)
-    elif isinstance(value, str):
-        return unicodedata.normalize(UNICODE_FORMAT, value)
-    else:
-        return value
-
-
 def increment_filename_with_count(
     filepath: Union[str, pathlib.Path], count: int = 0, lock: bool = False
 ) -> Tuple[str, int]:
     """Return filename (1).ext, etc if filename.ext exists
 
         If file exists in filename's parent folder with same stem as filename,
         add (1), (2), etc. until a non-existing filename is found.
```

### Comparing `osxphotos-0.60.4/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.60.5/osxphotos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.4
+Version: 0.60.5
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.4/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.60.5/osxphotos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,28 +36,30 @@
 osxphotos/phototables.py
 osxphotos/phototemplate.cog.md
 osxphotos/phototemplate.md
 osxphotos/phototemplate.py
 osxphotos/phototemplate.tx
 osxphotos/phototz.py
 osxphotos/placeinfo.py
+osxphotos/platform.py
 osxphotos/pyrepl.py
 osxphotos/query_builder.py
 osxphotos/queryoptions.py
 osxphotos/rich_utils.py
 osxphotos/scoreinfo.py
 osxphotos/searchinfo.py
 osxphotos/sqlgrep.py
 osxphotos/sqlite_utils.py
 osxphotos/sqlitekvstore.py
 osxphotos/template_counter.py
 osxphotos/text_detection.py
 osxphotos/timeutils.py
 osxphotos/timezones.py
 osxphotos/tutorial.md
+osxphotos/unicode.py
 osxphotos/uti.py
 osxphotos/utils.py
 osxphotos.egg-info/PKG-INFO
 osxphotos.egg-info/SOURCES.txt
 osxphotos.egg-info/dependency_links.txt
 osxphotos.egg-info/entry_points.txt
 osxphotos.egg-info/requires.txt
@@ -184,14 +186,15 @@
 tests/test_monterey_12_0_1.py
 tests/test_monterey_dev_beta_12_0_0.py
 tests/test_movies_4_0.py
 tests/test_movies_5_0.py
 tests/test_path_utils.py
 tests/test_personinfo.py
 tests/test_photokit.py
+tests/test_photosalbum_unicode.py
 tests/test_photosdb_utils.py
 tests/test_placeinfo.py
 tests/test_places_catalina_10_15_1.py
 tests/test_places_high_sierra_10_13_6.py
 tests/test_places_mojave_10_14_6.py
 tests/test_projects_catalina.py
 tests/test_projects_sierra.py
@@ -209,13 +212,14 @@
 tests/test_specials_mojave_10_14_6.py
 tests/test_specials_sierra_10_12.py
 tests/test_sqlite_utils.py
 tests/test_sqlitekvstore.py
 tests/test_template.py
 tests/test_template_counter.py
 tests/test_template_today.py
+tests/test_unicode.py
 tests/test_uti.py
 tests/test_utils.py
 tests/test_ventura_13_0_0.py
 tests/test_ventura_dev_preview_13_0_0.py
 tests/plugins/__init__.py
 tests/plugins/env_vars.py
```

### Comparing `osxphotos-0.60.4/osxphotos.egg-info/requires.txt` & `osxphotos-0.60.5/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/setup.py` & `osxphotos-0.60.5/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_10_12_6.py` & `osxphotos-0.60.5/tests/test_10_12_6.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 
 
 def test_photos_version(photosdb):
     assert photosdb.photos_version == 2
 
 
 def test_persons(photosdb):
-
     assert "Katie" in photosdb.persons
     assert collections.Counter(PERSONS) == collections.Counter(photosdb.persons)
 
 
 def test_keywords(photosdb):
     assert "wedding" in photosdb.keywords
     assert collections.Counter(KEYWORDS) == collections.Counter(photosdb.keywords)
```

### Comparing `osxphotos-0.60.4/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.60.5/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
 import osxphotos
-
 from osxphotos._constants import _UNKNOWN_PERSON, AlbumSortOrder
 
 PHOTOS_DB = "./tests/Test-10.15.7.photoslibrary/database/photos.db"
 
 TOP_LEVEL_FOLDERS = ["Folder1", "Folder2", "Pumpkin Farm"]
 
 TOP_LEVEL_CHILDREN = ["SubFolder1", "SubFolder2"]
```

### Comparing `osxphotos-0.60.4/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.60.5/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
 import osxphotos
-
 from osxphotos._constants import _UNKNOWN_PERSON
 
 PHOTOS_DB = "./tests/Test-10.13.6.photoslibrary/database/photos.db"
 
 TOP_LEVEL_FOLDERS = ["Folder1", "TestFolder"]
 
 TOP_LEVEL_CHILDREN = ["SubFolder1", "SubFolder2"]
```

### Comparing `osxphotos-0.60.4/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.60.5/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
 import osxphotos
-
 from osxphotos._constants import _UNKNOWN_PERSON
 
 PHOTOS_DB = "./tests/Test-10.14.6.photoslibrary/database/photos.db"
 
 TOP_LEVEL_FOLDERS = ["Folder1"]
 
 TOP_LEVEL_CHILDREN = ["SubFolder1", "SubFolder2"]
```

### Comparing `osxphotos-0.60.4/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.60.5/tests/test_bigsur_10_16_0_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,14 +222,15 @@
         assert osxphotos.PhotosDB(PHOTOS_DB, dbfile=PHOTOS_DB)
 
 
 def test_init4():
     # test invalid db
     import os
     import tempfile
+
     import osxphotos
 
     (bad_db, bad_db_name) = tempfile.mkstemp(suffix=".db", prefix="osxphotos-")
     os.close(bad_db)
 
     with pytest.raises(Exception):
         assert osxphotos.PhotosDB(bad_db_name)
@@ -602,15 +603,14 @@
 
 def test_keyword_2(photosdb):
     photos = photosdb.photos(keywords=["wedding"])
     assert len(photos) == 2  # won't show the one in the trash
 
 
 def test_keyword_not_in_album(photosdb):
-
     # find all photos with keyword "Kids" not in the album "Pumpkin Farm"
     photos1 = photosdb.photos(albums=["Pumpkin Farm"])
     photos2 = photosdb.photos(keywords=["Kids"])
     photos3 = [p for p in photos2 if p not in photos1]
     assert len(photos3) == 1
     assert photos3[0].uuid == "A1DD1F98-2ECD-431F-9AC9-5AFEFE2D3A5C"
 
@@ -1020,14 +1020,15 @@
     assert len(photos) == 4
 
 
 def test_date_invalid():
     """Test date is invalid"""
     # doesn't run correctly with the module-level fixture
     from datetime import datetime, timedelta, timezone
+
     import osxphotos
 
     # UUID_DICT["date_invalid"] has an invalid date that's
     # been manually adjusted in the database
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     photos = photosdb.photos(uuid=[UUID_DICT["date_invalid"]])
     assert len(photos) == 1
```

### Comparing `osxphotos-0.60.4/tests/test_catalina_10_15_7.py` & `osxphotos-0.60.5/tests/test_catalina_10_15_7.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from collections import Counter, namedtuple
 
 import pytest
 
 import osxphotos
 from osxphotos._constants import _UNKNOWN_PERSON
 from osxphotos.photoexporter import PhotoExporter
-from osxphotos.utils import is_macos, get_macos_version
+from osxphotos.platform import get_macos_version, is_macos
 
 OS_VERSION = get_macos_version() if is_macos else (None, None, None)
 SKIP_TEST = "OSXPHOTOS_TEST_EXPORT" not in os.environ or OS_VERSION[1] != "15"
 PHOTOS_DB_LOCAL = os.path.expanduser("~/Pictures/Photos Library.photoslibrary")
 
 PHOTOS_DB = "tests/Test-10.15.7.photoslibrary/database/photos.db"
 PHOTOS_DB_PATH = "/Test-10.15.7.photoslibrary/database/photos.db"
```

### Comparing `osxphotos-0.60.4/tests/test_cli.py` & `osxphotos-0.60.5/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 import re
 import shutil
 import sqlite3
 import subprocess
 import tempfile
 import time
 from tempfile import TemporaryDirectory
-from bitmath import contextlib
 
 import pytest
+from bitmath import contextlib
 from click.testing import CliRunner
 
 import osxphotos
 from osxphotos._constants import OSXPHOTOS_EXPORT_DB
 from osxphotos._version import __version__
 from osxphotos.cli import (
     about,
@@ -32,15 +32,17 @@
     labels,
     persons,
     places,
     query,
 )
 from osxphotos.exiftool import ExifTool, get_exiftool_path
 from osxphotos.fileutil import FileUtil
-from osxphotos.utils import is_macos, noop, normalize_fs_path, normalize_unicode
+from osxphotos.platform import is_macos
+from osxphotos.unicode import normalize_fs_path, normalize_unicode
+from osxphotos.utils import noop
 
 if is_macos:
     from osxmetadata import OSXMetaData, Tag
 
 from .conftest import copy_photos_library_to_path
 from .locale_util import setlocale
 
@@ -8170,14 +8172,54 @@
             "--added-in-last",
             "10 years",
         ],
     )
     assert results.exit_code == 0
 
 
+def test_query_count():
+    """Test query --count"""
+
+    runner = CliRunner()
+    cwd = os.getcwd()
+    # pylint: disable=not-context-manager
+    results = runner.invoke(
+        query,
+        [
+            "--library",
+            os.path.join(cwd, PHOTOS_DB_15_7),
+            "--added-before",
+            "2019-07-28",
+            "--count",
+        ],
+    )
+    assert results.exit_code == 0
+    assert results.output.strip() == "7"
+
+
+def test_query_count_0():
+    """Test query --count with zero results"""
+
+    runner = CliRunner()
+    cwd = os.getcwd()
+    # pylint: disable=not-context-manager
+    results = runner.invoke(
+        query,
+        [
+            "--library",
+            os.path.join(cwd, PHOTOS_DB_15_7),
+            "--added-before",
+            "1900-01-01",
+            "--count",
+        ],
+    )
+    assert results.exit_code == 0
+    assert results.output.strip() == "0"
+
+
 def test_export_export_dir_template():
     """Test {export_dir} template"""
 
     runner = CliRunner()
     cwd = os.getcwd()
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
```

### Comparing `osxphotos-0.60.4/tests/test_cli_add_locations.py` & `osxphotos-0.60.5/tests/test_cli_add_locations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Test osxphotos add-locations command"""
 
 import pytest
 from click.testing import CliRunner
 
-from osxphotos.utils import is_macos
+from osxphotos.platform import is_macos
+
 if is_macos:
     import photoscript
+
     from osxphotos.cli.add_locations import add_locations
 else:
     pytest.skip(allow_module_level=True)
 
 UUID_TEST_PHOTO_1 = "F12384F6-CD17-4151-ACBA-AE0E3688539E"  # Pumkins1.jpg
 UUID_TEST_PHOTO_LOCATION = "D79B8D77-BFFC-460B-9312-034F2877D35B"  # Pumkins2.jpg
 TEST_LOCATION = (41.26067, -95.94056)  # Omaha, NE
```

### Comparing `osxphotos-0.60.4/tests/test_cli_add_to_album.py` & `osxphotos-0.60.5/tests/test_cli_add_to_album.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ Test --add-exported-to-album """
 
 import os
 
 import pytest
 from click.testing import CliRunner
 
-from osxphotos.utils import is_macos
+from osxphotos.platform import is_macos
+
 if is_macos:
     import photoscript
 else:
     pytest.skip(allow_module_level=True)
 
 UUID_EXPORT = {"3DD2C897-F19E-4CA6-8C22-B027D5A71907": {"filename": "IMG_4547.jpg"}}
 UUID_MISSING = {
```

### Comparing `osxphotos-0.60.4/tests/test_cli_all_commands.py` & `osxphotos-0.60.5/tests/test_cli_all_commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 TEST_RUN_SCRIPT = "examples/cli_example_1.py"
 
 
 @pytest.fixture(scope="module")
 def runner() -> CliRunner:
     return CliRunner()
 
+
 from osxphotos.cli import (
     about,
     albums,
     debug_dump,
     docs_command,
     dump,
     grep,
@@ -39,16 +40,15 @@
     orphans,
     persons,
     places,
     theme,
     tutorial,
     version,
 )
-
-from osxphotos.utils import is_macos
+from osxphotos.platform import is_macos
 
 if is_macos:
     from osxphotos.cli import uuid
 
 
 def test_about(runner: CliRunner):
     with runner.isolated_filesystem():
@@ -68,15 +68,16 @@
         labels,
         list_libraries,
         orphans,
         persons,
         places,
         tutorial,
         version,
-    ] + ([uuid] if is_macos else []),
+    ]
+    + ([uuid] if is_macos else []),
 )
 def test_cli_comands(runner: CliRunner, command: Callable[..., Any]):
     with runner.isolated_filesystem():
         result = runner.invoke(albums, ["--db", TEST_DB])
         assert result.exit_code == 0
```

### Comparing `osxphotos-0.60.4/tests/test_cli_batch_edit.py` & `osxphotos-0.60.5/tests/test_cli_batch_edit.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 import os
 import time
 
 import pytest
 from click.testing import CliRunner
 
 import osxphotos
-from osxphotos.utils import is_macos
+from osxphotos.platform import is_macos
 
 if is_macos:
     import photoscript
+
     from osxphotos.cli.batch_edit import batch_edit
 else:
     pytest.skip(allow_module_level=True)
 
 # set timezone to avoid issues with comparing dates
 os.environ["TZ"] = "US/Pacific"
 time.tzset()
```

### Comparing `osxphotos-0.60.4/tests/test_cli_dump.py` & `osxphotos-0.60.5/tests/test_cli_dump.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,19 +87,20 @@
                 "--field",
                 "uuid",
                 "{uuid}",
                 "--field",
                 "name",
                 "{photo.original_filename}",
             ],
-                   )
+        )
         assert result.exit_code == 0
         for photo in photos:
             assert f"{photo.uuid},{photo.original_filename}" in result.output
 
+
 def test_dump_field_json(photos):
     """Test osxphotos dump --field --jso"""
     runner = CliRunner()
     cwd = os.getcwd()
     db_path = os.path.join(cwd, CLI_PHOTOS_DB)
     # pylint: disable=not-context-manager
     with runner.isolated_filesystem():
@@ -113,13 +114,13 @@
                 "uuid",
                 "{uuid}",
                 "--field",
                 "name",
                 "{photo.original_filename}",
                 "--json",
             ],
-                   )
+        )
         assert result.exit_code == 0
         json_data = {record["uuid"]: record for record in json.loads(result.output)}
         for photo in photos:
             assert photo.uuid in json_data
             assert json_data[photo.uuid]["name"] == photo.original_filename
```

### Comparing `osxphotos-0.60.4/tests/test_cli_exiftool.py` & `osxphotos-0.60.5/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_cli_export_cloud.py` & `osxphotos-0.60.5/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_cli_export_projects.py` & `osxphotos-0.60.5/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_cli_exportdb.py` & `osxphotos-0.60.5/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_cli_import.py` & `osxphotos-0.60.5/tests/test_cli_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 import os
 import os.path
 import pathlib
 import re
 import shutil
 import sqlite3
 import time
+import unicodedata
 from datetime import datetime
 from tempfile import TemporaryDirectory
 from typing import Dict
 
 import pytest
-
 from click.testing import CliRunner
 from pytest import MonkeyPatch, approx
 
 from osxphotos import PhotosDB, QueryOptions
 from osxphotos._constants import UUID_PATTERN
 from osxphotos.datetime_utils import datetime_remove_tz
 from osxphotos.exiftool import get_exiftool_path
-from osxphotos.utils import is_macos
+from osxphotos.platform import is_macos
 from tests.conftest import get_os_version
 
 if is_macos:
     from photoscript import Photo
+
     from osxphotos.cli.import_cli import import_cli
 else:
     pytest.skip(allow_module_level=True)
 
 TERMINAL_WIDTH = 250
 
 TEST_IMAGES_DIR = "tests/test-images"
@@ -40,25 +41,25 @@
 TEST_VIDEO_1 = "tests/test-images/Jellyfish.mov"
 TEST_VIDEO_2 = "tests/test-images/IMG_0670B_NOGPS.MOV"
 
 TEST_DATA = {
     TEST_IMAGE_1: {
         "title": "Waves crashing on rocks",
         "description": "Used for testing osxphotos",
-        "keywords": ["osxphotos"],
+        "keywords": ["osxphotos", "Sümmer"],
         "lat": 33.7150638888889,
         "lon": -118.319672222222,
         "check_templates": [
             "exiftool title: Waves crashing on rocks",
             "exiftool description: Used for testing osxphotos",
-            "exiftool keywords: ['osxphotos']",
+            "exiftool keywords: ['osxphotos', 'Sümmer']",
             "exiftool location: (33.7150638888889, -118.319672222222)",
             "title: {exiftool:XMP:Title}: Waves crashing on rocks",
             "description: {exiftool:IPTC:Caption-Abstract}: Used for testing osxphotos",
-            "keyword: {exiftool:IPTC:Keywords}: ['osxphotos']",
+            "keyword: {exiftool:IPTC:Keywords}: ['osxphotos', 'Sümmer']",
             "album: {filepath.parent}: test-images",
         ],
     },
     TEST_VIDEO_1: {
         "title": "Jellyfish",
         "description": "Jellyfish Video",
         # "keywords": ["Travel"], # exiftool doesn't seem to support the binary QuickTime:Keywords
@@ -532,15 +533,52 @@
 
     import_data = parse_import_output(result.output)
     file_1 = pathlib.Path(test_image_1).name
     uuid_1 = import_data[file_1]
     photo_1 = Photo(uuid_1)
 
     assert photo_1.filename == file_1
-    assert sorted(photo_1.keywords) == ["Bar", "Foo", "osxphotos"]
+    assert sorted(photo_1.keywords) == sorted(list(set(["Bar", "Foo"] + TEST_DATA[TEST_IMAGE_1]["keywords"])))
+
+@pytest.mark.skipif(exiftool_path is None, reason="exiftool not installed")
+@pytest.mark.test_import
+def test_import_keyword_merge_unicode():
+    """Test import with --keyword and --merge-keywords with unicode keywords (#1085)"""
+    cwd = os.getcwd()
+    test_image_1 = os.path.join(cwd, TEST_IMAGE_1)
+    runner = CliRunner()
+    result = runner.invoke(
+        import_cli,
+        [
+            "--verbose",
+            "--clear-metadata",
+            "--exiftool",
+            "--keyword",
+            "Bar",
+            "--keyword",
+            "Foo",
+            "--keyword",
+            unicodedata.normalize("NFD", "Sümmer"),
+            "--keyword",
+            unicodedata.normalize("NFC", "Sümmer"),
+            "--merge-keywords",
+            test_image_1,
+        ],
+        terminal_width=TERMINAL_WIDTH,
+    )
+
+    assert result.exit_code == 0
+
+    import_data = parse_import_output(result.output)
+    file_1 = pathlib.Path(test_image_1).name
+    uuid_1 = import_data[file_1]
+    photo_1 = Photo(uuid_1)
+
+    assert photo_1.filename == file_1
+    assert sorted(photo_1.keywords) == sorted(list(set(["Bar", "Foo"] + TEST_DATA[TEST_IMAGE_1]["keywords"])))
 
 
 @pytest.mark.test_import
 def test_import_location():
     """Test import file with --location"""
     cwd = os.getcwd()
     test_image_1 = os.path.join(cwd, TEST_IMAGE_1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `osxphotos-0.60.4/tests/test_cli_orphans.py` & `osxphotos-0.60.5/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_cli_param_types.py` & `osxphotos-0.60.5/tests/test_cli_param_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 """ Test custom click paramater types used by osxphotos CLI"""
 
 import datetime
-from bitmath import MB
 
 import pytest
-
-from osxphotos.timezones import Timezone
-
+from bitmath import MB
 from click.exceptions import BadParameter
 
 from osxphotos.cli.param_types import (
     BitMathSize,
     DateOffset,
     DateTimeISO8601,
     ExportDBType,
     FunctionCall,
     TemplateString,
     TimeISO8601,
     TimeOffset,
     TimeString,
     UTCOffset,
 )
+from osxphotos.timezones import Timezone
 
 
 def test_date_offset():
     """Test DateOffset"""
     date_offset_data = {
         "1": datetime.timedelta(days=1),
         "1 day": datetime.timedelta(days=1),
```

### Comparing `osxphotos-0.60.4/tests/test_cli_sync.py` & `osxphotos-0.60.5/tests/test_cli_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """Test osxphotos sync command"""
 
-import os
 import json
+import os
+
 import pytest
 from click.testing import CliRunner
 
-from osxphotos.utils import is_macos
+from osxphotos.platform import is_macos
+
 if is_macos:
     import photoscript
+
     from osxphotos.cli.sync import sync
 else:
     pytest.skip(allow_module_level=True)
 
 UUID_TEST_PHOTO_1 = "D79B8D77-BFFC-460B-9312-034F2877D35B"  # Pumkins2.jpg
 UUID_TEST_PHOTO_2 = "E9BC5C36-7CD1-40A1-A72B-8B8FAC227D51"  # wedding.jpg
```

### Comparing `osxphotos-0.60.4/tests/test_cli_timewarp.py` & `osxphotos-0.60.5/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_cli_utils.py` & `osxphotos-0.60.5/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_cli_verbose.py` & `osxphotos-0.60.5/tests/test_cli_verbose.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """Test verbose functions"""
 
 import re
 from io import StringIO
 
-
 from osxphotos.cli.verbose import (
+    _reset_verbose_globals,
     get_verbose_level,
     set_verbose_level,
     verbose,
     verbose_print,
-    _reset_verbose_globals,
 )
 
 
 def test_set_get_verbose_level(capsys):
     """Test verbose_print"""
     set_verbose_level(2)
     assert get_verbose_level() == 2
```

### Comparing `osxphotos-0.60.4/tests/test_cloud_owner_catalina.py` & `osxphotos-0.60.5/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_comments.py` & `osxphotos-0.60.5/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_concurrent_export.py` & `osxphotos-0.60.5/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_configoptions.py` & `osxphotos-0.60.5/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_datetime_formatter.py` & `osxphotos-0.60.5/tests/test_datetime_formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """ test datetime_formatter.DateTimeFormatter """
 import pytest
 
 from .locale_util import setlocale
 
 
 def test_datetime_formatter_1():
-    """Test DateTimeFormatter """
+    """Test DateTimeFormatter"""
     import datetime
     import locale
+
     from osxphotos.datetime_formatter import DateTimeFormatter
 
     setlocale(locale.LC_ALL, "en_US")
 
     dt = datetime.datetime(2020, 5, 23, 12, 42, 33)
     dtf = DateTimeFormatter(dt)
 
@@ -25,17 +26,18 @@
     assert dtf.doy == "144"
     assert dtf.hour == "12"
     assert dtf.min == "42"
     assert dtf.sec == "33"
 
 
 def test_datetime_formatter_2():
-    """Test DateTimeFormatter with hour > 12 """
+    """Test DateTimeFormatter with hour > 12"""
     import datetime
     import locale
+
     from osxphotos.datetime_formatter import DateTimeFormatter
 
     setlocale(locale.LC_ALL, "en_US")
 
     dt = datetime.datetime(2020, 5, 23, 14, 42, 33)
     dtf = DateTimeFormatter(dt)
 
@@ -49,17 +51,18 @@
     assert dtf.doy == "144"
     assert dtf.hour == "14"
     assert dtf.min == "42"
     assert dtf.sec == "33"
 
 
 def test_datetime_formatter_3():
-    """Test DateTimeFormatter zero-padding  """
+    """Test DateTimeFormatter zero-padding"""
     import datetime
     import locale
+
     from osxphotos.datetime_formatter import DateTimeFormatter
 
     setlocale(locale.LC_ALL, "en_US")
 
     dt = datetime.datetime(2020, 5, 2, 9, 3, 6)
     dtf = DateTimeFormatter(dt)
```

### Comparing `osxphotos-0.60.4/tests/test_datetime_utils.py` & `osxphotos-0.60.5/tests/test_datetime_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import date, timezone
+
 import pytest
 
 from osxphotos.datetime_utils import *
 
 
 def test_get_local_tz():
     import datetime
@@ -89,8 +90,8 @@
     import os
 
     os.environ["TZ"] = "CEST"
 
     tz = datetime.timezone(offset=datetime.timedelta(seconds=7200))
     utc = datetime.datetime(2020, 9, 1, 19, 0, 0, tzinfo=datetime.timezone.utc)
     dt = datetime_utc_to_local(utc)
-    assert dt == datetime.datetime(2020, 9, 1, 21, 0, 0, tzinfo=tz)
+    assert dt == datetime.datetime(2020, 9, 1, 21, 0, 0, tzinfo=tz)
```

### Comparing `osxphotos-0.60.4/tests/test_debug.py` & `osxphotos-0.60.5/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_empty_library_4_0.py` & `osxphotos-0.60.5/tests/test_empty_library_4_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,33 +26,36 @@
 
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     assert photosdb.db_version in osxphotos._constants._TESTED_DB_VERSIONS
     assert photosdb.db_version == "4025"
 
 
 def test_persons():
-    import osxphotos
     import collections
 
+    import osxphotos
+
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     assert photosdb.persons == []
 
 
 def test_keywords():
-    import osxphotos
     import collections
 
+    import osxphotos
+
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     assert photosdb.keywords == []
 
 
 def test_album_names():
-    import osxphotos
     import collections
 
+    import osxphotos
+
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     assert photosdb.albums == []
 
 
 def test_keywords_dict():
     import osxphotos
```

### Comparing `osxphotos-0.60.4/tests/test_exif_info.py` & `osxphotos-0.60.5/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_exiftool.py` & `osxphotos-0.60.5/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_exiftool_caching.py` & `osxphotos-0.60.5/tests/test_exiftool_caching.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from osxphotos.exiftool import get_exiftool_path
 
 TEST_FILE_ONE_KEYWORD = "tests/test-images/wedding.jpg"
 TEST_FILE_BAD_IMAGE = "tests/test-images/badimage.jpeg"
 TEST_FILE_WARNING = "tests/test-images/exiftool_warning.heic"
 TEST_FILE_MULTI_KEYWORD = "tests/test-images/Tulips.jpg"
 TEST_MULTI_KEYWORDS = [
@@ -103,15 +104,15 @@
 
     exif = osxphotos.exiftool.ExifToolCaching(TEST_FILE_ONE_KEYWORD)
     assert exif.version is not None
     assert isinstance(exif.version, str)
 
 
 def test_singleton():
-    """ tests per-file singleton behavior """
+    """tests per-file singleton behavior"""
     import osxphotos.exiftool
 
     exif1 = osxphotos.exiftool.ExifToolCaching(TEST_FILE_ONE_KEYWORD)
     exif2 = osxphotos.exiftool.ExifToolCaching(TEST_FILE_ONE_KEYWORD)
     assert exif1 is exif2
 
     exif3 = osxphotos.exiftool.ExifToolCaching(TEST_FILE_MULTI_KEYWORD)
@@ -127,14 +128,15 @@
     assert exif.data["IPTC:Keywords"] == "wedding"
 
 
 def test_setvalue_1():
     # test setting a tag value
     import os.path
     import tempfile
+
     import osxphotos.exiftool
     from osxphotos.fileutil import FileUtil
 
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     tempfile = os.path.join(tempdir.name, os.path.basename(TEST_FILE_ONE_KEYWORD))
     FileUtil.copy(TEST_FILE_ONE_KEYWORD, tempfile)
 
@@ -143,14 +145,15 @@
         exif.setvalue("IPTC:Keywords", "test")
 
 
 def test_setvalue_cache():
     # test setting a tag value doesn't affect cached value
     import os.path
     import tempfile
+
     import osxphotos.exiftool
     from osxphotos.fileutil import FileUtil
 
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     tempfile = os.path.join(tempdir.name, os.path.basename(TEST_FILE_ONE_KEYWORD))
     FileUtil.copy(TEST_FILE_ONE_KEYWORD, tempfile)
 
@@ -170,14 +173,15 @@
     assert exifcache.asdict()["IPTC:Keywords"] == "foo"
 
 
 def test_setvalue_context_manager():
     # test setting a tag value as context manager
     import os.path
     import tempfile
+
     import osxphotos.exiftool
     from osxphotos.fileutil import FileUtil
 
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     tempfile = os.path.join(tempdir.name, os.path.basename(TEST_FILE_ONE_KEYWORD))
     FileUtil.copy(TEST_FILE_ONE_KEYWORD, tempfile)
 
@@ -186,14 +190,15 @@
             exif.setvalue("IPTC:Keywords", "test1")
 
 
 def test_flags():
     # test that flags raise error
     import os.path
     import tempfile
+
     import osxphotos.exiftool
     from osxphotos.fileutil import FileUtil
 
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     tempfile = os.path.join(tempdir.name, os.path.basename(TEST_FILE_WARNING))
     FileUtil.copy(TEST_FILE_WARNING, tempfile)
 
@@ -203,14 +208,15 @@
             exif.setvalue("XMP:Subject", "foo/ba    r")
 
 
 def test_clear_value():
     # test clearing a tag value
     import os.path
     import tempfile
+
     import osxphotos.exiftool
     from osxphotos.fileutil import FileUtil
 
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     tempfile = os.path.join(tempdir.name, os.path.basename(TEST_FILE_ONE_KEYWORD))
     FileUtil.copy(TEST_FILE_ONE_KEYWORD, tempfile)
 
@@ -220,14 +226,15 @@
         exif.setvalue("IPTC:Keywords", None)
 
 
 def test_addvalues_1():
     # test setting a tag value
     import os.path
     import tempfile
+
     import osxphotos.exiftool
     from osxphotos.fileutil import FileUtil
 
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     tempfile = os.path.join(tempdir.name, os.path.basename(TEST_FILE_ONE_KEYWORD))
     FileUtil.copy(TEST_FILE_ONE_KEYWORD, tempfile)
 
@@ -272,45 +279,46 @@
 
     exif1 = osxphotos.exiftool.ExifToolCaching(TEST_FILE_ONE_KEYWORD)
     exifdata = exif1.asdict(tag_groups=False)
     assert exifdata["TagsList"] == "wedding"
 
 
 def test_json():
-    import osxphotos.exiftool
     import json
 
+    import osxphotos.exiftool
+
     exif1 = osxphotos.exiftool.ExifToolCaching(TEST_FILE_ONE_KEYWORD)
     exifdata = json.loads(exif1.json())
     assert exifdata[0]["XMP:TagsList"] == "wedding"
 
 
 def test_str():
     import osxphotos.exiftool
 
     exif1 = osxphotos.exiftool.ExifToolCaching(TEST_FILE_ONE_KEYWORD)
     assert "file: " in str(exif1)
     assert "exiftool: " in str(exif1)
 
 
 def test_photoinfo_exiftool():
-    """ test PhotoInfo.exiftool which returns ExifTool object for photo """
+    """test PhotoInfo.exiftool which returns ExifTool object for photo"""
     import osxphotos
 
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     for uuid in EXIF_UUID:
         photo = photosdb.photos(uuid=[uuid])[0]
         exiftool = photo.exiftool
         exif_dict = exiftool.asdict()
         for key, val in EXIF_UUID[uuid].items():
             assert exif_dict[key] == val
 
 
 def test_photoinfo_exiftool_no_groups():
-    """ test PhotoInfo.exiftool which returns ExifTool object for photo without tag group names"""
+    """test PhotoInfo.exiftool which returns ExifTool object for photo without tag group names"""
     import osxphotos
 
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     for uuid in EXIF_UUID_NO_GROUPS:
         photo = photosdb.photos(uuid=[uuid])[0]
         exiftool = photo.exiftool
         exif_dict = exiftool.asdict(tag_groups=False)
```

### Comparing `osxphotos-0.60.4/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.60.5/tests/test_export_catalina_10_15_7.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,69 +353,63 @@
 
     with pytest.raises(Exception) as e:
         assert photos[0].export(dest)
     assert e.type == type(FileNotFoundError())
 
 
 def test_dd_to_dms_str_1():
-
     lat_str, lon_str = dd_to_dms_str(
         34.559331096, 69.206499174
     )  # Kabul, 34°33'33.59" N 69°12'23.40" E
 
     assert lat_str == "34 deg 33' 33.59\" N"
     assert lon_str == "69 deg 12' 23.40\" E"
 
 
 def test_dd_to_dms_str_2():
-
     lat_str, lon_str = dd_to_dms_str(
         -34.601997592, -58.375665164
     )  # Buenos Aires, 34°36'7.19" S 58°22'32.39" W
 
     assert lat_str == "34 deg 36' 7.19\" S"
     assert lon_str == "58 deg 22' 32.39\" W"
 
 
 def test_dd_to_dms_str_3():
-
     lat_str, lon_str = dd_to_dms_str(
         -1.2666656, 36.7999968
     )  # Nairobi, 1°15'60.00" S 36°47'59.99" E
 
     assert lat_str == "1 deg 15' 60.00\" S"
     assert lon_str == "36 deg 47' 59.99\" E"
 
 
 def test_dd_to_dms_str_4():
-
     lat_str, lon_str = dd_to_dms_str(
         38.889248, -77.050636
     )  # DC: 38° 53' 21.2928" N, 77° 3' 2.2896" W
 
     assert lat_str == "38 deg 53' 21.29\" N"
     assert lon_str == "77 deg 3' 2.29\" W"
 
 
 def test_exiftool_json_sidecar(photosdb):
-
     uuid = EXIF_JSON_UUID
     photo = photosdb.get_photo(uuid)
 
     with open(str(pathlib.Path(SIDECAR_DIR) / f"{uuid}.json"), "r") as fp:
         json_expected = json.load(fp)[0]
 
     json_got = PhotoExporter(photo).exiftool_json_sidecar()
     json_got = json.loads(json_got)[0]
 
     assert json_got == json_expected
 
 
 def test_exiftool_json_sidecar_ignore_date_modified(photosdb):
-
     uuid = EXIF_JSON_UUID
     photo = photosdb.get_photo(uuid)
 
     with open(
         str(pathlib.Path(SIDECAR_DIR) / f"{uuid}_ignore_date_modified.json"), "r"
     ) as fp:
         json_expected = json.load(fp)[0]
@@ -465,17 +459,15 @@
     for k, v in json_expected.items():
         if type(v) in (list, tuple):
             assert sorted(json_got[k]) == sorted(v)
         else:
             assert json_got[k] == v
 
 
-
 def test_exiftool_json_sidecar_keyword_template(photosdb):
-
     uuid = EXIF_JSON_UUID
     photo = photosdb.get_photo(uuid)
 
     with open(
         str(pathlib.Path(SIDECAR_DIR) / f"{uuid}_keyword_template.json"), "r"
     ) as fp:
         json_expected = json.load(fp)
@@ -484,15 +476,14 @@
     )
     json_got = json.loads(json_got)
 
     assert json_got == json_expected
 
 
 def test_exiftool_json_sidecar_use_persons_keyword(photosdb):
-
     uuid = UUID_DICT["xmp"]
     photo = photosdb.get_photo(uuid)
 
     with open(
         str(pathlib.Path(SIDECAR_DIR) / f"{uuid}_persons_as_keywords.json"), "r"
     ) as fp:
         json_expected = json.load(fp)[0]
@@ -502,15 +493,14 @@
     )
     json_got = json.loads(json_got)[0]
 
     assert json_got == json_expected
 
 
 def test_exiftool_json_sidecar_use_albums_keywords(photosdb):
-
     uuid = UUID_DICT["xmp"]
     photo = photosdb.get_photo(uuid)
 
     with open(
         str(pathlib.Path(SIDECAR_DIR) / f"{uuid}_albums_as_keywords.json"), "r"
     ) as fp:
         json_expected = json.load(fp)
@@ -546,15 +536,14 @@
     assert xmp_file.is_file()
     exiftool = ExifTool(str(xmp_file))
     output, _, _ = exiftool.run_commands("-validate", "-warning")
     assert output == b"[ExifTool]      Validate                        : 0 0 0"
 
 
 def test_xmp_sidecar(photosdb):
-
     uuid = UUID_DICT["xmp"]
     photos = photosdb.photos(uuid=[uuid])
 
     with open(f"tests/sidecars/{uuid}.xmp", "r") as file:
         xmp_expected = file.read()
     xmp_got = PhotoExporter(photos[0])._xmp_sidecar(extension="jpg")
     assert xmp_got == xmp_expected
@@ -571,29 +560,27 @@
         xmp_expected_lines = [line.strip() for line in xmp_expected.split("\n")]
 
     xmp_got = PhotoExporter(photos[0])._xmp_sidecar()
     assert xmp_got == xmp_expected
 
 
 def test_xmp_sidecar_use_persons_keyword(photosdb):
-
     uuid = UUID_DICT["xmp"]
     photo = photosdb.get_photo(uuid)
 
     with open(pathlib.Path(SIDECAR_DIR) / f"{uuid}_persons_as_keywords.xmp") as fp:
         xmp_expected = fp.read()
 
     xmp_got = PhotoExporter(photo)._xmp_sidecar(
         ExportOptions(use_persons_as_keywords=True), extension="jpg"
     )
     assert xmp_got == xmp_expected
 
 
 def test_xmp_sidecar_use_albums_keyword(photosdb):
-
     uuid = UUID_DICT["xmp"]
     photo = photosdb.get_photo(uuid)
 
     with open(pathlib.Path(SIDECAR_DIR) / f"{uuid}_albums_as_keywords.xmp") as fp:
         xmp_expected = fp.read()
 
     xmp_got = PhotoExporter(photo)._xmp_sidecar(
@@ -612,15 +599,14 @@
         xmp_expected = fp.read()
 
     xmp_got = PhotoExporter(photo)._xmp_sidecar()
     assert xmp_got == xmp_expected
 
 
 def test_xmp_sidecar_keyword_template(photosdb):
-
     uuid = UUID_DICT["location"]
     photo = photosdb.get_photo(uuid)
 
     with open(pathlib.Path(SIDECAR_DIR) / f"{uuid}_keyword_template.xmp") as fp:
         xmp_expected = fp.read()
 
     xmp_got = PhotoExporter(photo)._xmp_sidecar(
```

### Comparing `osxphotos-0.60.4/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.60.5/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
+
 import pytest
 
 from osxphotos._constants import _UNKNOWN_PERSON
-from osxphotos.utils import is_macos, get_macos_version
+from osxphotos.platform import get_macos_version, is_macos
 
 OS_VERSION = get_macos_version() if is_macos else (None, None, None)
 SKIP_TEST = "OSXPHOTOS_TEST_EXPORT" not in os.environ or OS_VERSION[1] != "15"
 PHOTOS_DB = os.path.expanduser("~/Pictures/Photos Library.photoslibrary")
 pytestmark = pytest.mark.skipif(
     SKIP_TEST, reason="These tests only run against system photos library"
 )
@@ -119,24 +120,23 @@
 
     assert got_dest == expected_dest
     assert os.path.isfile(expected_dest)
 
 
 def test_export_edited_exiftool(photosdb):
     # test export edited file
+    import logging
     import os
     import os.path
     import pathlib
     import tempfile
 
     import osxphotos
     import osxphotos.exiftool
 
-    import logging
-
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     dest = tempdir.name
     photos = photosdb.photos(uuid=[UUID_DICT["has_adjustments"]])
 
     got_dest = photos[0].export(
         dest, use_photos_export=True, edited=True, exiftool=True
     )
```

### Comparing `osxphotos-0.60.4/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.60.5/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_export_db.py` & `osxphotos-0.60.5/tests/test_export_db.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Test ExportDB """
 
 import os
 import pathlib
+import shutil
 import sqlite3
 import tempfile
-import shutil
 
 import pytest
 
 from osxphotos._version import __version__
 from osxphotos.export_db import (
     OSXPHOTOS_EXPORTDB_VERSION,
     ExportDB,
```

### Comparing `osxphotos-0.60.4/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.60.5/tests/test_export_mojave_10_14_6.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,42 +326,39 @@
 
     with pytest.raises(Exception) as e:
         assert photos[0].export(dest)[0]
     assert e.type == type(FileNotFoundError())
 
 
 def test_exiftool_json_sidecar(photosdb):
-
     uuid = UUID_DICT["location"]
     photo = photosdb.get_photo(uuid)
 
     with open(str(pathlib.Path(SIDECAR_DIR) / f"{uuid}.json"), "r") as fp:
         json_expected = json.load(fp)[0]
 
     json_got = PhotoExporter(photo).exiftool_json_sidecar()
     json_got = json.loads(json_got)[0]
 
     assert json_got == json_expected
 
 
 def test_xmp_sidecar(photosdb):
-
     uuid = UUID_DICT["xmp"]
     photo = photosdb.get_photo(uuid)
 
     with open(pathlib.Path(SIDECAR_DIR) / f"{uuid}_ext.xmp") as fp:
         xmp_expected = fp.read()
 
     xmp_got = PhotoExporter(photo)._xmp_sidecar(extension="jpg")
 
     assert xmp_got == xmp_expected
 
 
 def test_xmp_sidecar_keyword_template(photosdb):
-
     uuid = UUID_DICT["xmp"]
     photo = photosdb.get_photo(uuid)
 
     with open(pathlib.Path(SIDECAR_DIR) / f"{uuid}_keyword_template.xmp") as fp:
         xmp_expected = fp.read()
 
     xmp_got = PhotoExporter(photo)._xmp_sidecar(
```

### Comparing `osxphotos-0.60.4/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.60.5/tests/test_export_raw_catalina_10_15_1.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -62,17 +62,17 @@
     assert pathlib.Path(got_dest).name == FILENAME_DICT["original"]
 
 
 def test_export_edited_name():
     # export edited file with name provided
     import os
     import os.path
+    import pathlib
     import tempfile
     import time
-    import pathlib
 
     import osxphotos
 
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     dest = tempdir.name
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     photos = photosdb.photos(uuid=[UUID_DICT["has_adjustments"]])
@@ -105,18 +105,18 @@
 
 
 def test_export_edited_wrong_suffix():
     # export edited file with name provided but wrong suffix
     # should produce a warning via logging.warning
     import os
     import os.path
+    import pathlib
     import sys
     import tempfile
     import time
-    import pathlib
 
     import osxphotos
 
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     dest = tempdir.name
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     photos = photosdb.photos(uuid=[UUID_DICT["has_adjustments"]])
```

### Comparing `osxphotos-0.60.4/tests/test_exportresults.py` & `osxphotos-0.60.5/tests/test_exportresults.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ test ExportResults class """
 
 import pytest
+
 from osxphotos.photoexporter import ExportResults
 
 EXPORT_RESULT_ATTRIBUTES = ExportResults().attributes
 
 
 def test_exportresults_init():
     results = ExportResults()
```

### Comparing `osxphotos-0.60.4/tests/test_faceinfo.py` & `osxphotos-0.60.5/tests/test_faceinfo.py`

 * *Files 0% similar despite different names*

```diff
@@ -4070,53 +4070,53 @@
     import osxphotos
 
     return osxphotos.PhotosDB(dbfile=PHOTOS_DB_4)
 
 
 @pytest.mark.parametrize("uuid_dict", UUID_LIST_5)
 def test_faceinfo_v5(photosdb5, uuid_dict):
-    """ Test FaceInfo object """
+    """Test FaceInfo object"""
     import json
 
     for uuid in uuid_dict:
         photo = photosdb5.get_photo(uuid)
         faces = photo.face_info
         assert len(faces) == len(uuid_dict[uuid])
         for face in faces:
             assert face.uuid in uuid_dict[uuid]
             # test by keys instead of dict == dict because Monterey+ dropped support for some of the face details
-            # and I didn't want to regenerate all the test data (e.g.eye, mouth coordinates) 
+            # and I didn't want to regenerate all the test data (e.g.eye, mouth coordinates)
             face_dict = face.asdict()
             for key in face_dict:
                 if key == "yaw":
-                    continue # yaw set to 0 as it's not in Ventura
+                    continue  # yaw set to 0 as it's not in Ventura
                 assert face_dict[key] == uuid_dict[uuid][face.uuid][key]
 
 
 def test_faceinfo_v5_no_face(photosdb5):
-    """ Test FaceInfo on image with no faces """
+    """Test FaceInfo on image with no faces"""
     photo = photosdb5.get_photo(UUID_NO_FACE_5)
     assert photo.face_info == []
 
 
 @pytest.mark.parametrize("uuid_dict", UUID_LIST_4)
 def test_faceinfo_v4(photosdb4, uuid_dict):
-    """ Test FaceInfo object """
+    """Test FaceInfo object"""
     import json
 
     for uuid in uuid_dict:
         photo = photosdb4.get_photo(uuid)
         faces = photo.face_info
         assert len(faces) == len(uuid_dict[uuid])
         for face in faces:
             assert face.uuid in uuid_dict[uuid]
             # test by keys instead of dict == dict because Monterey+ dropped support for some of the face details
-            # and I didn't want to regenerate all the test data (e.g.eye, mouth coordinates) 
+            # and I didn't want to regenerate all the test data (e.g.eye, mouth coordinates)
             face_dict = face.asdict()
             for key in face_dict:
                 assert face_dict[key] == uuid_dict[uuid][face.uuid][key]
 
 
 def test_faceinfo_v4_no_face(photosdb4):
-    """ Test FaceInfo on image with no faces """
+    """Test FaceInfo on image with no faces"""
     photo = photosdb4.get_photo(UUID_NO_FACE_4)
     assert photo.face_info == []
```

### Comparing `osxphotos-0.60.4/tests/test_fileutil.py` & `osxphotos-0.60.5/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_highsierra.py` & `osxphotos-0.60.5/tests/test_highsierra.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import pytest
 
 import osxphotos
-
 from osxphotos._constants import _UNKNOWN_PERSON
 
 PHOTOS_DB = "./tests/Test-10.13.6.photoslibrary/database/photos.db"
 KEYWORDS = [
     "Kids",
     "wedding",
     "flowers",
```

### Comparing `osxphotos-0.60.4/tests/test_image_converter.py` & `osxphotos-0.60.5/tests/test_image_converter.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,27 +15,28 @@
 TEST_JPEG = "tests/test-images/IMG_3984.jpeg"
 TEST_IMAGES = [TEST_HEIC, TEST_RAW, TEST_JPEG]
 TEST_NOT_AN_IMAGE = "tests/README.md"
 TEST_IMAGE_DOES_NOT_EXIST = "tests/test-images/NOT-A-FILE.heic"
 
 
 def test_image_converter_singleton():
-    """ test that ImageConverter is a singleton """
+    """test that ImageConverter is a singleton"""
     from osxphotos.imageconverter import ImageConverter
 
     convert1 = ImageConverter()
     convert2 = ImageConverter()
 
     assert convert1 == convert2
 
 
 def test_image_converter():
-    """ test conversion of different image types """
+    """test conversion of different image types"""
     import pathlib
     import tempfile
+
     from osxphotos.imageconverter import ImageConverter
 
     converter = ImageConverter()
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     with tempdir:
         for imgfile in TEST_IMAGES:
             imgfile = pathlib.Path(imgfile)
@@ -46,17 +47,18 @@
             assert converter.write_jpeg(imgfile, outfile)
             assert converter.write_jpeg(str(imgfile), str(outfile2))
             assert outfile.is_file()
             assert outfile2.is_file()
 
 
 def test_image_converter_compression_quality():
-    """ test conversion of different image types with custom compression quality """
+    """test conversion of different image types with custom compression quality"""
     import pathlib
     import tempfile
+
     from osxphotos.imageconverter import ImageConverter
 
     converter = ImageConverter()
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     with tempdir:
         for imgfile in TEST_IMAGES:
             imgfile = pathlib.Path(imgfile)
@@ -65,52 +67,54 @@
             # call write_jpeg with both pathlib.Path and str arguments
             assert converter.write_jpeg(imgfile, outfile, compression_quality=0.1)
             assert outfile.is_file()
             assert outfile.stat().st_size < 1000000
 
 
 def test_image_converter_bad_compression_quality():
-    """ test illegal compression quality """
+    """test illegal compression quality"""
     import pathlib
     import tempfile
+
     from osxphotos.imageconverter import ImageConverter
 
     converter = ImageConverter()
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     with tempdir:
         imgfile = pathlib.Path(TEST_HEIC)
         outfile = pathlib.Path(tempdir.name) / f"{imgfile.stem}.jpeg"
         with pytest.raises(ValueError):
             converter.write_jpeg(imgfile, outfile, compression_quality=2.0)
         with pytest.raises(ValueError):
             converter.write_jpeg(imgfile, outfile, compression_quality=-1.0)
 
 
 def test_image_converter_bad_file():
-    """ Try to convert a file that's not an image """
+    """Try to convert a file that's not an image"""
     import pathlib
     import tempfile
-    from osxphotos.imageconverter import ImageConverter, ImageConversionError
+
+    from osxphotos.imageconverter import ImageConversionError, ImageConverter
 
     converter = ImageConverter()
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     with tempdir:
         imgfile = pathlib.Path(TEST_NOT_AN_IMAGE)
         outfile = pathlib.Path(tempdir.name) / f"{imgfile.stem}.jpeg"
         with pytest.raises(ImageConversionError):
             converter.write_jpeg(imgfile, outfile)
 
 
 def test_image_converter_missing_file():
-    """ Try to convert a file that's not an image """
+    """Try to convert a file that's not an image"""
     import pathlib
     import tempfile
+
     from osxphotos.imageconverter import ImageConverter
 
     converter = ImageConverter()
     tempdir = tempfile.TemporaryDirectory(prefix="osxphotos_")
     with tempdir:
         imgfile = pathlib.Path(TEST_IMAGE_DOES_NOT_EXIST)
         outfile = pathlib.Path(tempdir.name) / f"{imgfile.stem}.jpeg"
         with pytest.raises(FileNotFoundError):
             converter.write_jpeg(imgfile, outfile)
-
```

### Comparing `osxphotos-0.60.4/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.60.5/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.60.5/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.60.5/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.60.5/tests/test_incloud_mojave_10_14_6.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 }
 
 
 @pytest.fixture(scope="module")
 def photosdb():
     return osxphotos.PhotosDB(dbfile=PHOTOS_DB_CLOUD)
 
+
 def test_incloud(photosdb):
     photos = photosdb.photos(uuid=[UUID_DICT["incloud"]])
 
     assert photos[0].incloud
 
 
 def test_not_incloud(photosdb):
```

### Comparing `osxphotos-0.60.4/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.60.5/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.60.5/tests/test_modified_date_catalina_10_15_7.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 PHOTOS_DB = "./tests/Test-10.15.7.photoslibrary/database/photos.db"
 
 UUID_DICT = {
     "modified": "E9BC5C36-7CD1-40A1-A72B-8B8FAC227D51",
     "not_modified": "D05A5FE3-15FB-49A1-A15D-AB3DA6F8B068",
 }
 
+
 @pytest.fixture(scope="module")
 def photosdb():
     return osxphotos.PhotosDB(dbfile=PHOTOS_DB)
 
+
 def test_modified(photosdb):
     import datetime
 
     photos = photosdb.photos(uuid=[UUID_DICT["modified"]])
     assert photos[0].date_modified is not None
     assert photos[0].date_modified == datetime.datetime(
         2019,
```

### Comparing `osxphotos-0.60.4/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.60.5/tests/test_modified_date_mojave_10_14_6.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 PHOTOS_LIBRARY_PATH = "/Test-Shared-10.14.6.photoslibrary"
 
 UUID_DICT = {
     "modified": "3Jn73XpSQQCluzRBMWRsMA",
     "not_modified": "35243F7D-88C4-4408-B516-C74406E90C15",
 }
 
+
 @pytest.fixture(scope="module")
 def photosdb():
     return osxphotos.PhotosDB(dbfile=PHOTOS_DB)
 
 
 def test_modified(photosdb):
     photos = photosdb.photos(uuid=[UUID_DICT["modified"]])
```

### Comparing `osxphotos-0.60.4/tests/test_mojave_10_14_6.py` & `osxphotos-0.60.5/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.60.5/tests/test_mojave_10_14_6_path_edited.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,30 @@
     "standard_00_path": "3Jn73XpSQQCluzRBMWRsMA",
 }
 
 
 def test_path_edited1():
     # test a valid edited path
     import os.path
+
     import osxphotos
 
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     photos = photosdb.photos(uuid=[UUID_DICT["standard_00_path"]])
     assert len(photos) == 1
     p = photos[0]
     path = p.path_edited
     assert path.endswith("resources/media/version/00/00/fullsizeoutput_d.jpeg")
     assert os.path.exists(path)
 
 
 def test_path_edited2():
     # test a non-standard (not 00) edited path
     import os.path
+
     import osxphotos
 
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     photos = photosdb.photos(uuid=[UUID_DICT["non_00_path"]])
     assert len(photos) == 1
     p = photos[0]
     path = p.path_edited
```

### Comparing `osxphotos-0.60.4/tests/test_monterey_12_0_1.py` & `osxphotos-0.60.5/tests/test_monterey_12_0_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,14 +228,15 @@
         assert osxphotos.PhotosDB(PHOTOS_DB, dbfile=PHOTOS_DB)
 
 
 def test_init4():
     # test invalid db
     import os
     import tempfile
+
     import osxphotos
 
     (bad_db, bad_db_name) = tempfile.mkstemp(suffix=".db", prefix="osxphotos-")
     os.close(bad_db)
 
     with pytest.raises(Exception):
         assert osxphotos.PhotosDB(bad_db_name)
@@ -604,15 +605,14 @@
 
 def test_keyword_2(photosdb):
     photos = photosdb.photos(keywords=["wedding"])
     assert len(photos) == 2  # won't show the one in the trash
 
 
 def test_keyword_not_in_album(photosdb):
-
     # find all photos with keyword "Kids" not in the album "Pumpkin Farm"
     photos1 = photosdb.photos(albums=["Pumpkin Farm"])
     photos2 = photosdb.photos(keywords=["Kids"])
     photos3 = [p for p in photos2 if p not in photos1]
     assert len(photos3) == 1
     assert photos3[0].uuid == "A1DD1F98-2ECD-431F-9AC9-5AFEFE2D3A5C"
 
@@ -1022,14 +1022,15 @@
     assert len(photos) == 4
 
 
 def test_date_invalid():
     """Test date is invalid"""
     # doesn't run correctly with the module-level fixture
     from datetime import datetime, timedelta, timezone
+
     import osxphotos
 
     # UUID_DICT["date_invalid"] has an invalid date that's
     # been manually adjusted in the database
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     photos = photosdb.photos(uuid=[UUID_DICT["date_invalid"]])
     assert len(photos) == 1
```

### Comparing `osxphotos-0.60.4/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.60.5/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from collections import Counter, namedtuple
 
 import pytest
 
 import osxphotos
 from osxphotos._constants import _UNKNOWN_PERSON
 from osxphotos.photoexporter import PhotoExporter
-from osxphotos.utils import is_macos, get_macos_version
+from osxphotos.platform import get_macos_version, is_macos
 
 OS_VERSION = get_macos_version() if is_macos else (None, None, None)
 # SKIP_TEST = "OSXPHOTOS_TEST_EXPORT" not in os.environ or OS_VERSION[1] != "17"
 SKIP_TEST = True  # don't run any of the local library tests
 PHOTOS_DB_LOCAL = os.path.expanduser("~/Pictures/Photos Library.photoslibrary")
 
 PHOTOS_DB = "tests/Test-12.0.0.dev-beta.photoslibrary/database/photos.db"
@@ -287,86 +287,75 @@
     mocker.patch("osxphotos.photosdb.photosdb.get_last_library_path", new=bad_library)
 
     with pytest.raises(Exception):
         assert osxphotos.PhotosDB()
 
 
 def test_db_len(photosdb):
-
     # assert photosdb.db_version in osxphotos._TESTED_DB_VERSIONS
     assert len(photosdb) == PHOTOS_DB_LEN
 
 
 def test_db_version(photosdb):
-
     # assert photosdb.db_version in osxphotos._TESTED_DB_VERSIONS
     assert photosdb.db_version == "6000"
 
 
 def test_photos_version(photosdb):
     assert photosdb.photos_version == 7
 
 
 def test_persons(photosdb):
-
     assert "Katie" in photosdb.persons
     assert Counter(PERSONS) == Counter(photosdb.persons)
 
 
 def test_keywords(photosdb):
-
     assert "wedding" in photosdb.keywords
     assert Counter(KEYWORDS) == Counter(photosdb.keywords)
 
 
 def test_album_names(photosdb):
-
     assert "Pumpkin Farm" in photosdb.albums
     assert Counter(ALBUMS) == Counter(photosdb.albums)
 
 
 def test_keywords_dict(photosdb):
-
     keywords = photosdb.keywords_as_dict
     assert keywords["wedding"] == 3
     assert keywords == KEYWORDS_DICT
 
 
 def test_persons_as_dict(photosdb):
-
     persons = photosdb.persons_as_dict
     assert persons["Maria"] == 2
     assert persons == PERSONS_DICT
 
 
 def test_albums_as_dict(photosdb):
-
     albums = photosdb.albums_as_dict
     assert albums["Pumpkin Farm"] == 3
     assert albums == ALBUM_DICT
 
 
 def test_album_sort_order(photosdb):
-
     album = [a for a in photosdb.album_info if a.title == "Pumpkin Farm"][0]
     photos = album.photos
 
     uuids = [p.uuid for p in photos]
     assert uuids == ALBUM_SORT_ORDER
 
 
 def test_album_empty_album(photosdb):
-
     album = [a for a in photosdb.album_info if a.title == "EmptyAlbum"][0]
     photos = album.photos
     assert photos == []
 
 
 def test_attributes(photosdb):
-
     photos = photosdb.photos(uuid=["D79B8D77-BFFC-460B-9312-034F2877D35B"])
     assert len(photos) == 1
     p = photos[0]
     assert p.keywords == ["Kids"]
     assert p.original_filename == "Pumkins2.jpg"
     assert p.filename == "D79B8D77-BFFC-460B-9312-034F2877D35B.jpeg"
     assert p.date == datetime.datetime(
@@ -430,48 +419,43 @@
     assert p.original_width == 2048
     assert p.orientation == 1
     assert p.original_orientation == 1
     assert p.original_filesize == 460483
 
 
 def test_missing(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["missing"]])
     assert len(photos) == 1
     p = photos[0]
     assert p.path is None
     assert p.ismissing == True
 
 
 def test_favorite(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["favorite"]])
     assert len(photos) == 1
     p = photos[0]
     assert p.favorite == True
 
 
 def test_not_favorite(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["not_favorite"]])
     assert len(photos) == 1
     p = photos[0]
     assert p.favorite == False
 
 
 def test_hidden(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["hidden"]])
     assert len(photos) == 1
     p = photos[0]
     assert p.hidden == True
 
 
 def test_not_hidden(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["not_hidden"]])
     assert len(photos) == 1
     p = photos[0]
     assert p.hidden == False
 
 
 def test_visible(photosdb):
@@ -602,15 +586,14 @@
 
     photos = photosdb.photos(uuid=[UUID_DICT["no_adjustments"]])
     p = photos[0]
     assert not p.ismovie
 
 
 def test_count(photosdb):
-
     photos = photosdb.photos()
     assert len(photos) == PHOTOS_NOT_IN_TRASH_LEN
 
 
 def test_photos_intrash_1(photosdb):
     """test PhotosDB.photos(intrash=True)"""
 
@@ -681,21 +664,19 @@
 
     p = photosdb.photos(uuid=[UUID_DICT["not_intrash"]])[0]
     assert not p.intrash
     assert p.date_trashed is None
 
 
 def test_keyword_2(photosdb):
-
     photos = photosdb.photos(keywords=["wedding"])
     assert len(photos) == 2  # won't show the one in the trash
 
 
 def test_keyword_not_in_album(photosdb):
-
     # find all photos with keyword "Kids" not in the album "Pumpkin Farm"
     photos1 = photosdb.photos(albums=["Pumpkin Farm"])
     photos2 = photosdb.photos(keywords=["Kids"])
     photos3 = [p for p in photos2 if p not in photos1]
     assert len(photos3) == 1
     assert photos3[0].uuid == "A1DD1F98-2ECD-431F-9AC9-5AFEFE2D3A5C"
 
@@ -704,28 +685,25 @@
     """Test query with album name same as a folder name"""
 
     photos = photosdb.photos(albums=["Pumpkin Farm"])
     assert sorted(p.uuid for p in photos) == sorted(UUID_PUMPKIN_FARM)
 
 
 def test_multi_person(photosdb):
-
     photos = photosdb.photos(persons=["Katie", "Suzy"])
 
     assert len(photos) == 3
 
 
 def test_get_db_path(photosdb):
-
     db_path = photosdb.db_path
     assert db_path.endswith(PHOTOS_DB_PATH)
 
 
 def test_get_library_path(photosdb):
-
     lib_path = photosdb.library_path
     assert lib_path.endswith(PHOTOS_LIBRARY_PATH)
 
 
 def test_get_db_connection(photosdb):
     """Test PhotosDB.get_db_connection"""
 
@@ -1024,33 +1002,30 @@
     albums = photos1[0].albums
     assert albums
 
     assert photos1[0] == photos2[0]
 
 
 def test_not_eq(photosdb):
-
     photos1 = photosdb.photos(uuid=[UUID_DICT["export"]])
     photos2 = photosdb.photos(uuid=[UUID_DICT["missing"]])
     assert photos1[0] != photos2[0]
 
 
 def test_photosdb_repr():
-
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     photosdb2 = eval(repr(photosdb))
 
     ignore_keys = ["_tmp_db", "_tempdir", "_tempdir_name", "_db_connection"]
     assert {k: v for k, v in photosdb.__dict__.items() if k not in ignore_keys} == {
         k: v for k, v in photosdb2.__dict__.items() if k not in ignore_keys
     }
 
 
 def test_photosinfo_repr(photosdb):
-
     photos = photosdb.photos(uuid=[UUID_DICT["favorite"]])
     photo = photos[0]
     photo2 = eval(repr(photo))
 
     assert {k: str(v).encode("utf-8") for k, v in photo.__dict__.items()} == {
         k: str(v).encode("utf-8") for k, v in photo2.__dict__.items()
     }
```

### Comparing `osxphotos-0.60.4/tests/test_movies_4_0.py` & `osxphotos-0.60.5/tests/test_movies_4_0.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,23 +29,25 @@
 
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     assert photosdb.db_version in osxphotos._constants._TESTED_DB_VERSIONS
     assert photosdb.db_version == "4025"
 
 
 def test_keywords():
-    import osxphotos
     import collections
 
+    import osxphotos
+
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     assert "test" in photosdb.keywords
 
 
 def test_attributes():
     import datetime
+
     import osxphotos
 
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     photos = photosdb.photos(uuid=[UUID_DICT["movie"]], movies=True)
     assert len(photos) == 1
     p = photos[0]
     assert p.keywords == ["test"]
```

### Comparing `osxphotos-0.60.4/tests/test_movies_5_0.py` & `osxphotos-0.60.5/tests/test_movies_5_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,23 +32,25 @@
 
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     assert photosdb.db_version in osxphotos._constants._TESTED_DB_VERSIONS
     assert photosdb.db_version == "6000"
 
 
 def test_keywords():
-    import osxphotos
     import collections
 
+    import osxphotos
+
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     assert "test" in photosdb.keywords
 
 
 def test_attributes():
     import datetime
+
     import osxphotos
 
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     photos = photosdb.photos(uuid=[UUID_DICT["movie"]], movies=True)
     assert len(photos) == 1
     p = photos[0]
     assert p.keywords == ["test"]
```

### Comparing `osxphotos-0.60.4/tests/test_path_utils.py` & `osxphotos-0.60.5/tests/test_path_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """ Test path_utils.py """
 
 from osxphotos._constants import _OSXPHOTOS_LOCK_EXTENSION, MAX_FILENAME_LEN
 from osxphotos.path_utils import sanitize_filename
 
 
 def test_sanitize_filename():
-
     # basic sanitize
     filenames = {
         "Foobar.txt": "Foobar.txt",
         "Foo:bar.txt": "Foo:bar.txt",
         "Foo/bar.txt": "Foo:bar.txt",
         "Foo//.txt": "Foo::.txt",
     }
```

### Comparing `osxphotos-0.60.4/tests/test_personinfo.py` & `osxphotos-0.60.5/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_photokit.py` & `osxphotos-0.60.5/tests/test_photokit.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 import os
 import pathlib
 import tempfile
 
 import pytest
 
-from osxphotos.utils import is_macos
+from osxphotos.platform import is_macos
+
 if is_macos:
     from osxphotos.photokit import (
+        PHOTOS_VERSION_CURRENT,
+        PHOTOS_VERSION_ORIGINAL,
+        PHOTOS_VERSION_UNADJUSTED,
         LivePhotoAsset,
         PhotoAsset,
         PhotoLibrary,
         VideoAsset,
-        PHOTOS_VERSION_CURRENT,
-        PHOTOS_VERSION_ORIGINAL,
-        PHOTOS_VERSION_UNADJUSTED,
     )
 else:
     pytest.skip(allow_module_level=True)
 
 skip_test = "OSXPHOTOS_TEST_EXPORT" not in os.environ
 pytestmark = pytest.mark.skipif(
     skip_test, reason="Skip if not running with author's personal library."
```

### Comparing `osxphotos-0.60.4/tests/test_photosdb_utils.py` & `osxphotos-0.60.5/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_placeinfo.py` & `osxphotos-0.60.5/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.60.5/tests/test_places_catalina_10_15_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """ Test PlaceInfo """
 import pytest
 
-
 PHOTOS_DB = "./tests/Test-Places-Catalina-10_15_1.photoslibrary/database/photos.db"
 
 UUID_DICT = {
     "place_dc": "128FB4C6-0B16-4E7D-9108-FB2E90DA1546",
     "place_maui": "FF7AFE2C-49B0-4C9B-B0D7-7E1F8B8F2F0C",
     "no_place": "A9B73E13-A6F2-4915-8D67-7213B39BAE9F",
 }
```

### Comparing `osxphotos-0.60.4/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.60.5/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.60.5/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_projects_catalina.py` & `osxphotos-0.60.5/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_projects_sierra.py` & `osxphotos-0.60.5/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_score_info.py` & `osxphotos-0.60.5/tests/test_score_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Test ScoreInfo """
 
 from math import isclose
+
 import pytest
 
 from osxphotos.scoreinfo import ScoreInfo
 
 PHOTOS_DB_5 = "tests/Test-10.15.5.photoslibrary"
 PHOTOS_DB_4 = "tests/Test-10.14.6.photoslibrary"
 
@@ -74,24 +75,24 @@
 def photosdb():
     import osxphotos
 
     return osxphotos.PhotosDB(dbfile=PHOTOS_DB_5)
 
 
 def test_score_info_v5(photosdb):
-    """ test score """
+    """test score"""
     # use math.isclose to compare floats
     # on MacOS x64 these can probably compared for equality but would possibly
     # fail if osxphotos ever ported to other platforms
     for uuid in SCORE_DICT:
         photo = photosdb.photos(uuid=[uuid], movies=True)[0]
         for attr in photo.score.__dict__:
             assert isclose(getattr(photo.score, attr), getattr(SCORE_DICT[uuid], attr))
 
 
 def test_score_info_v4():
-    """ test version 4, score should be None """
+    """test version 4, score should be None"""
     import osxphotos
 
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB_4)
     for photo in photosdb.photos():
         assert photo.score is None
```

### Comparing `osxphotos-0.60.4/tests/test_search_info_10_14_6.py` & `osxphotos-0.60.5/tests/test_search_info_10_14_6.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 # On 10.14.6, SearchInfo is not valid and returns None
 
 import pytest
 
 from osxphotos._constants import _UNKNOWN_PERSON
 
-
 PHOTOS_DB = "./tests/Test-10.14.6.photoslibrary/database/photos.db"
 
 LABELS_DICT = {
     # 8SOE9s0XQVGsuq4ONohTng Pumkins1.jpg Can we carry this? Girls with pumpkins [] False
     "8SOE9s0XQVGsuq4ONohTng": [],
     # HrK3ZQdlQ7qpDA0FgOYXLA Pumpkins3.jpg None Kids in pumpkin field [] False
     "HrK3ZQdlQ7qpDA0FgOYXLA": [],
```

### Comparing `osxphotos-0.60.4/tests/test_search_info_10_15_4.py` & `osxphotos-0.60.5/tests/test_search_info_10_15_4.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ test PhotoInfo.search_info """
 
 import pytest
 
 from osxphotos._constants import _UNKNOWN_PERSON
 
-
 PHOTOS_DB = "./tests/Test-10.15.4.photoslibrary/database/photos.db"
 PHOTOS_DB_PATH = "/Test-10.15.4.photoslibrary/database/photos.db"
 PHOTOS_LIBRARY_PATH = "/Test-10.15.4.photoslibrary"
 
 LABELS_DICT = {
     # A92D9C26-3A50-4197-9388-CB5F7DB9FA91 IMG_1994.JPG None RAW + JPEG, JPEG Original [] False
     "A92D9C26-3A50-4197-9388-CB5F7DB9FA91": [],
```

### Comparing `osxphotos-0.60.4/tests/test_search_info_10_15_5.py` & `osxphotos-0.60.5/tests/test_search_info_10_15_5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ test PhotoInfo.search_info """
 
 import pytest
 
 from osxphotos._constants import _UNKNOWN_PERSON
 
-
 PHOTOS_DB = "./tests/Test-10.15.5.photoslibrary/database/photos.db"
 PHOTOS_DB_PATH = "/Test-10.15.5.photoslibrary/database/photos.db"
 PHOTOS_LIBRARY_PATH = "/Test-10.15.5.photoslibrary"
 
 LABELS_DICT = {
     # A92D9C26-3A50-4197-9388-CB5F7DB9FA91 IMG_1994.JPG None RAW + JPEG, JPEG Original [] False
     "A92D9C26-3A50-4197-9388-CB5F7DB9FA91": [
```

### Comparing `osxphotos-0.60.4/tests/test_search_info_10_15_7.py` & `osxphotos-0.60.5/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.60.5/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.60.5/tests/test_shared_mojave_10_14_6.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pytest
 
-
 PHOTOS_DB = "./tests/Test-10.14.6.photoslibrary/database/photos.db"
 PHOTOS_DB_PATH = "/Test-10.14.6.photoslibrary/database/photos.db"
 PHOTOS_LIBRARY_PATH = "/Test-10.14.6.photoslibrary"
 
 ALBUMS = ["Pumpkin Farm", "AlbumInFolder", "Test Album", "Test Album (1)"]
 ALBUM_DICT = {
     "Pumpkin Farm": 3,
@@ -14,14 +13,15 @@
 }
 
 
 PHOTOS_DB_LEN = 13
 PHOTOS_NOT_IN_TRASH_LEN = 12
 PHOTOS_IN_TRASH_LEN = 1
 
+
 def test_album_names():
     import osxphotos
 
     photosdb = osxphotos.PhotosDB(dbfile=PHOTOS_DB)
     albums = photosdb.albums
 
     assert len(albums) == len(ALBUMS)
```

### Comparing `osxphotos-0.60.4/tests/test_sidecar_xmp.py` & `osxphotos-0.60.5/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.60.5/tests/test_specials_bigsur_10_16_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     assert not photos[0].selfie
     assert not photos[0].time_lapse
     assert not photos[0].panorama
 
     photos = photosdb.photos(uuid=[UUID_DICT["no_specials"]])
     assert not photos[0].portrait
 
+
 def test_portrait2():
     import osxphotos
 
     photosdb = osxphotos.PhotosDB(PHOTOS_DB_CLOUD)
     photos = photosdb.photos(uuid=[UUID_DICT["portrait2"]])
 
     assert photos[0].portrait
```

### Comparing `osxphotos-0.60.4/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.60.5/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.60.5/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_specials_sierra_10_12.py` & `osxphotos-0.60.5/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_sqlitekvstore.py` & `osxphotos-0.60.5/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_template.py` & `osxphotos-0.60.5/tests/test_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 import re
 
 import pytest
 
 import osxphotos
 from osxphotos.exiftool import get_exiftool_path
 from osxphotos.export_db import ExportDBInMemory
+from osxphotos.photoinfo import PhotoInfoNone
 from osxphotos.phototemplate import (
     PUNCTUATION,
     TEMPLATE_SUBSTITUTIONS,
     TEMPLATE_SUBSTITUTIONS_MULTI_VALUED,
     PhotoTemplate,
     RenderOptions,
 )
-from osxphotos.photoinfo import PhotoInfoNone
-from osxphotos.utils import is_macos
-from .photoinfo_mock import PhotoInfoMock
+from osxphotos.platform import is_macos
+
 from .locale_util import setlocale
+from .photoinfo_mock import PhotoInfoMock
 
 try:
     exiftool = get_exiftool_path()
 except:
     exiftool = None
 
 PHOTOS_DB_PLACES = (
```

### Comparing `osxphotos-0.60.4/tests/test_template_counter.py` & `osxphotos-0.60.5/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_template_today.py` & `osxphotos-0.60.5/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_uti.py` & `osxphotos-0.60.5/tests/test_uti.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """ test uti.py """
 
 import pytest
 
 import osxphotos.uti
+from osxphotos.platform import is_macos
 from osxphotos.uti import (
     _get_uti_from_mdls,
     get_preferred_uti_extension,
     get_uti_for_extension,
 )
-from osxphotos.utils import is_macos
 
 EXT_DICT = {"heic": "public.heic", "jpg": "public.jpeg", ".jpg": "public.jpeg"}
 UTI_DICT = {"public.heic": "heic", "public.jpeg": "jpeg"}
 
 
 def test_get_preferred_uti_extension():
     """test get_preferred_uti_extension"""
```

### Comparing `osxphotos-0.60.4/tests/test_utils.py` & `osxphotos-0.60.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_ventura_13_0_0.py` & `osxphotos-0.60.5/tests/test_ventura_13_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.4/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.60.5/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files 0% similar despite different names*

```diff
@@ -604,15 +604,14 @@
 
 def test_keyword_2(photosdb):
     photos = photosdb.photos(keywords=["wedding"])
     assert len(photos) == 2  # won't show the one in the trash
 
 
 def test_keyword_not_in_album(photosdb):
-
     # find all photos with keyword "Kids" not in the album "Pumpkin Farm"
     photos1 = photosdb.photos(albums=["Pumpkin Farm"])
     photos2 = photosdb.photos(keywords=["Kids"])
     photos3 = [p for p in photos2 if p not in photos1]
     assert len(photos3) == 1
     assert photos3[0].uuid == "A1DD1F98-2ECD-431F-9AC9-5AFEFE2D3A5C"
```

