# Comparing `tmp/neon-skill-device_controls-0.3.1a2.tar.gz` & `tmp/neon-skill-device_controls-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-device_controls-0.3.1a2.tar", last modified: Thu Jun 15 20:52:41 2023, max compression
+gzip compressed data, was "neon-skill-device_controls-1.0.0.tar", last modified: Fri Jun 23 23:42:23 2023, max compression
```

## Comparing `neon-skill-device_controls-0.3.1a2.tar` & `neon-skill-device_controls-1.0.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:41.875504 neon-skill-device_controls-0.3.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-15 20:52:41.875504 neon-skill-device_controls-0.3.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:41.867503 neon-skill-device_controls-0.3.1a2/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:41.867503 neon-skill-device_controls-0.3.1a2/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:41.871504 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/action_not_confirmed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/already_requiring.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/already_skipping.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/ask_disable_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/ask_exit_shutdown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/ask_start_requiring.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/ask_start_skipping.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_brain_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_brain_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_cancel.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_exiting.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_listening_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_listening_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_require_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_restarting.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_shutdown.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_skip_ww.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_ww_changed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_ww_changing.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/confirm_ww_disabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/error_invalid_ww_requested.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/error_no_ww_api.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/error_no_ww_heard.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/error_ww_already_enabled.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/error_ww_change_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/dialog/not_doing_anything.dialog
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:41.871504 neon-skill-device_controls-0.3.1a2/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/intent/exit.intent
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/intent/restart.intent
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/intent/shutdown.intent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:41.871504 neon-skill-device_controls-0.3.1a2/locale/en-us/regex/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/regex/wakeword.rx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:41.875504 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/debug.voc
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/disable.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/enable.voc
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/exit.voc
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/listening.voc
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/mycroft.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/neon.voc
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/no.voc
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/request.voc
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/restart.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/shutdown.voc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/solo.voc
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/start.voc
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/start_sww.voc
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/stop.voc
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/stop_sww.voc
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/locale/en-us/vocab/ww.voc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:41.875504 neon-skill-device_controls-0.3.1a2/neon_skill_device_controls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-15 20:52:41.000000 neon-skill-device_controls-0.3.1a2/neon_skill_device_controls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-15 20:52:41.000000 neon-skill-device_controls-0.3.1a2/neon_skill_device_controls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:52:41.000000 neon-skill-device_controls-0.3.1a2/neon_skill_device_controls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-15 20:52:41.000000 neon-skill-device_controls-0.3.1a2/neon_skill_device_controls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 20:52:41.000000 neon-skill-device_controls-0.3.1a2/neon_skill_device_controls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-15 20:52:41.000000 neon-skill-device_controls-0.3.1a2/neon_skill_device_controls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:52:41.875504 neon-skill-device_controls-0.3.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:52:41.875504 neon-skill-device_controls-0.3.1a2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    27790 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-15 20:52:37.000000 neon-skill-device_controls-0.3.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:23.241448 neon-skill-device_controls-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-23 23:42:23.241448 neon-skill-device_controls-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14983 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:23.225448 neon-skill-device_controls-1.0.0/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:23.225448 neon-skill-device_controls-1.0.0/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:23.233447 neon-skill-device_controls-1.0.0/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/action_not_confirmed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/already_requiring.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/already_skipping.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/ask_disable_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/ask_exit_shutdown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/ask_start_requiring.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/ask_start_skipping.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_brain_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_brain_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_cancel.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_exiting.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_listening_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_listening_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_require_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_restarting.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_shutdown.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_skip_ww.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_ww_changed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_ww_changing.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/confirm_ww_disabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/error_invalid_ww_requested.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/error_no_ww_api.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/error_no_ww_heard.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/error_ww_already_enabled.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/error_ww_change_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/dialog/not_doing_anything.dialog
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:23.233447 neon-skill-device_controls-1.0.0/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/intent/exit.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/intent/restart.intent
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/intent/shutdown.intent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:23.233447 neon-skill-device_controls-1.0.0/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/regex/wakeword.rx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:23.237448 neon-skill-device_controls-1.0.0/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/debug.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/disable.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/enable.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/exit.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/listening.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/mycroft.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/no.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/request.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/restart.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/shutdown.voc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/solo.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/start.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/start_sww.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/stop.voc
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/stop_sww.voc
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/locale/en-us/vocab/ww.voc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:23.241448 neon-skill-device_controls-1.0.0/neon_skill_device_controls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-23 23:42:23.000000 neon-skill-device_controls-1.0.0/neon_skill_device_controls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-23 23:42:23.000000 neon-skill-device_controls-1.0.0/neon_skill_device_controls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 23:42:23.000000 neon-skill-device_controls-1.0.0/neon_skill_device_controls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-23 23:42:23.000000 neon-skill-device_controls-1.0.0/neon_skill_device_controls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 23:42:23.000000 neon-skill-device_controls-1.0.0/neon_skill_device_controls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 23:42:23.000000 neon-skill-device_controls-1.0.0/neon_skill_device_controls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 23:42:23.241448 neon-skill-device_controls-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 23:42:23.241448 neon-skill-device_controls-1.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    27790 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-23 23:42:20.000000 neon-skill-device_controls-1.0.0/version.py
```

### Comparing `neon-skill-device_controls-0.3.1a2/LICENSE.md` & `neon-skill-device_controls-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-0.3.1a2/PKG-INFO` & `neon-skill-device_controls-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-device_controls
-Version: 0.3.1a2
+Version: 1.0.0
 Home-page: https://github.com/NeonGeckoCom/skill-device_controls
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-device_controls-0.3.1a2/README.md` & `neon-skill-device_controls-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-0.3.1a2/__init__.py` & `neon-skill-device_controls-1.0.0/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-0.3.1a2/neon_skill_device_controls.egg-info/PKG-INFO` & `neon-skill-device_controls-1.0.0/neon_skill_device_controls.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-device-controls
-Version: 0.3.1a2
+Version: 1.0.0
 Home-page: https://github.com/NeonGeckoCom/skill-device_controls
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-device_controls-0.3.1a2/neon_skill_device_controls.egg-info/SOURCES.txt` & `neon-skill-device_controls-1.0.0/neon_skill_device_controls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-0.3.1a2/setup.py` & `neon-skill-device_controls-1.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-0.3.1a2/skill.json` & `neon-skill-device_controls-1.0.0/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-0.3.1a2/test/test_skill.py` & `neon-skill-device_controls-1.0.0/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-device_controls-0.3.1a2/version.py` & `neon-skill-device_controls-1.0.0/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.3.1a2"
+__version__ = "1.0.0"
```

