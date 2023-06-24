# Comparing `tmp/jaraco.abode-5.0.1.tar.gz` & `tmp/jaraco.abode-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.abode-5.0.1.tar", last modified: Fri Apr  7 01:14:34 2023, max compression
+gzip compressed data, was "jaraco.abode-5.1.0.tar", last modified: Sat Jun 24 00:17:56 2023, max compression
```

## Comparing `jaraco.abode-5.0.1.tar` & `jaraco.abode-5.1.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.195859 jaraco.abode-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.163859 jaraco.abode-5.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.163859 jaraco.abode-5.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-04-07 01:14:34.195859 jaraco.abode-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.163859 jaraco.abode-5.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.155859 jaraco.abode-5.0.1/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.171859 jaraco.abode-5.0.1/jaraco/abode/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/automation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.179859 jaraco.abode-5.0.1/jaraco/abode/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/devices/valve.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/event_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.179859 jaraco.abode-5.0.1/jaraco/abode/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/helpers/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/helpers/events.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/helpers/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/helpers/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/socketio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/jaraco/abode/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.167859 jaraco.abode-5.0.1/jaraco.abode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-04-07 01:14:34.000000 jaraco.abode-5.0.1/jaraco.abode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-07 01:14:34.000000 jaraco.abode-5.0.1/jaraco.abode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 01:14:34.000000 jaraco.abode-5.0.1/jaraco.abode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-07 01:14:34.000000 jaraco.abode-5.0.1/jaraco.abode.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-07 01:14:34.000000 jaraco.abode-5.0.1/jaraco.abode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-07 01:14:34.000000 jaraco.abode-5.0.1/jaraco.abode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-07 01:14:34.195859 jaraco.abode-5.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.187859 jaraco.abode-5.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.191859 jaraco.abode-5.0.1/tests/mock/
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/automation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 01:14:34.195859 jaraco.abode-5.0.1/tests/mock/devices/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/door_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/door_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/glass.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/hue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/ipcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/ir_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/keypad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/pir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/power_switch_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/power_switch_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/remote_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/secure_barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/status_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/unknown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/valve.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/devices/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/oauth_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/mock/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    20675 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_abode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_automation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_door_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_event_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_hue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_power_switch_meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_power_switch_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_secure_barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tests/test_valve.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-07 01:14:13.000000 jaraco.abode-5.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.511628 jaraco.abode-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.487625 jaraco.abode-5.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.491625 jaraco.abode-5.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-06-24 00:17:56.511628 jaraco.abode-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.491625 jaraco.abode-5.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.483624 jaraco.abode-5.1.0/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.499626 jaraco.abode-5.1.0/jaraco/abode/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.503627 jaraco.abode-5.1.0/jaraco/abode/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/devices/valve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/event_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.503627 jaraco.abode-5.1.0/jaraco/abode/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/helpers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/helpers/events.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/helpers/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/helpers/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/socketio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/jaraco/abode/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.495626 jaraco.abode-5.1.0/jaraco.abode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 2023-06-24 00:17:56.000000 jaraco.abode-5.1.0/jaraco.abode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-06-24 00:17:56.000000 jaraco.abode-5.1.0/jaraco.abode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 00:17:56.000000 jaraco.abode-5.1.0/jaraco.abode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-24 00:17:56.000000 jaraco.abode-5.1.0/jaraco.abode.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-24 00:17:56.000000 jaraco.abode-5.1.0/jaraco.abode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-24 00:17:56.000000 jaraco.abode-5.1.0/jaraco.abode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-24 00:17:56.511628 jaraco.abode-5.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.507627 jaraco.abode-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.507627 jaraco.abode-5.1.0/tests/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/automation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:17:56.511628 jaraco.abode-5.1.0/tests/mock/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/door_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/door_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/glass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/hue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/ipcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/ir_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/keypad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/pir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/power_switch_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/power_switch_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/remote_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/secure_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/status_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/valve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/devices/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/oauth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/mock/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20675 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_abode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11978 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13234 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_door_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18432 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_event_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_hue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_power_switch_meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_power_switch_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_secure_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tests/test_valve.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-24 00:17:31.000000 jaraco.abode-5.1.0/tox.ini
```

### Comparing `jaraco.abode-5.0.1/.github/workflows/main.yml` & `jaraco.abode-5.1.0/.github/workflows/main.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 name: tests
 
 on: [push, pull_request]
 
+permissions:
+  contents: read
+
 env:
   # Environment variables to support color support (jaraco/skeleton#66):
   # Request colored output from CLI tools supporting it. Different tools
   # interpret the value differently. For some, just being set is sufficient.
   # For others, it must be a non-zero integer. For yet others, being set
   # to a non-empty value is sufficient. For tox, it must be one of
   # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
@@ -35,57 +38,51 @@
 
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-        - "3.7"
+        - "3.8"
         - "3.11"
         - "3.12"
-        # Workaround for actions/setup-python#508
-        dev:
-        - -dev
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
-        - python: "3.8"
-          platform: ubuntu-latest
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
         - python: pypy3.9
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.12' }}
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
+          python-version: ${{ matrix.python }}
+          allow-prereleases: true
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   docs:
     runs-on: ubuntu-latest
     env:
       TOXENV: docs
     steps:
       - uses: actions/checkout@v3
       - name: Setup Python
         uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python }}${{ matrix.dev }}
       - name: Install tox
         run: |
           python -m pip install tox
       - name: Run tests
         run: tox
 
   check:  # This job does nothing and is only used for the branch protection
@@ -100,14 +97,16 @@
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
         jobs: ${{ toJSON(needs) }}
 
   release:
+    permissions:
+      contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `jaraco.abode-5.0.1/CHANGES.rst` & `jaraco.abode-5.1.0/NEWS.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.1.0
+======
+
+Features
+--------
+
+- Require Python 3.8 or later.
+
+
 v5.0.1
 ======
 
 Minor bugfixes and test updates.
 
 v5.0.0
 ======
```

### Comparing `jaraco.abode-5.0.1/LICENSE` & `jaraco.abode-5.1.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.abode-5.0.1/PKG-INFO` & `jaraco.abode-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: jaraco.abode
-Version: 5.0.1
+Version: 5.1.0
 Summary: A library interfacing to the Abode home security system
 Home-page: https://github.com/jaraco/jaraco.abode
 Author: Wil Schrader
 Author-email: wilrader@gmail.com
 Maintainer: Jason R. Coombs
 Maintainer-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 Provides-Extra: docs
 License-File: LICENSE
 
 .. image:: https://img.shields.io/pypi/v/jaraco.abode.svg
    :target: https://pypi.org/project/jaraco.abode
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.abode.svg
 
 .. image:: https://github.com/jaraco/jaraco.abode/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.abode/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracoabode/badge/?version=latest
    :target: https://jaracoabode.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.abode-5.0.1/README.rst` & `jaraco.abode-5.1.0/jaraco.abode.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,39 @@
+Metadata-Version: 2.1
+Name: jaraco.abode
+Version: 5.1.0
+Summary: A library interfacing to the Abode home security system
+Home-page: https://github.com/jaraco/jaraco.abode
+Author: Wil Schrader
+Author-email: wilrader@gmail.com
+Maintainer: Jason R. Coombs
+Maintainer-email: jaraco@jaraco.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.8
+Provides-Extra: testing
+Provides-Extra: docs
+License-File: LICENSE
+
 .. image:: https://img.shields.io/pypi/v/jaraco.abode.svg
    :target: https://pypi.org/project/jaraco.abode
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.abode.svg
 
 .. image:: https://github.com/jaraco/jaraco.abode/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.abode/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracoabode/badge/?version=latest
    :target: https://jaracoabode.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.abode-5.0.1/conftest.py` & `jaraco.abode-5.1.0/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/docs/api.rst` & `jaraco.abode-5.1.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/docs/conf.py` & `jaraco.abode-5.1.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 master_doc = "index"
 html_theme = "furo"
 
 # Link dates and other references in the changelog
 extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
```

### Comparing `jaraco.abode-5.0.1/jaraco/abode/automation.py` & `jaraco.abode-5.1.0/jaraco/abode/automation.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/cli.py` & `jaraco.abode-5.1.0/jaraco/abode/cli.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/client.py` & `jaraco.abode-5.1.0/jaraco/abode/client.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/devices/alarm.py` & `jaraco.abode-5.1.0/jaraco/abode/devices/alarm.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/devices/base.py` & `jaraco.abode-5.1.0/jaraco/abode/devices/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     tags: Tuple[str, ...] = ()
     _desc_t = '{name} (ID: {id}, UUID: {uuid}) - {type} - {status}'
     _url_t = urls.DEVICE
 
     @property
     def _control_url(self):
         if not self._state['control_url']:
-            raise jaraco.abode.Exception("Control URL required")
+            raise jaraco.abode.Exception(("Control URL required",))
         return self._state['control_url']
 
     def set_status(self, status) -> None:
         """Set device status."""
         response = self._client.send_request(
             method="put",
             path=self._control_url,
```

### Comparing `jaraco.abode-5.0.1/jaraco/abode/devices/binary_sensor.py` & `jaraco.abode-5.1.0/jaraco/abode/devices/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/devices/camera.py` & `jaraco.abode-5.1.0/jaraco/abode/devices/camera.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/devices/cover.py` & `jaraco.abode-5.1.0/jaraco/abode/devices/cover.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/devices/light.py` & `jaraco.abode-5.1.0/jaraco/abode/devices/light.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/devices/lock.py` & `jaraco.abode-5.1.0/jaraco/abode/devices/lock.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/devices/sensor.py` & `jaraco.abode-5.1.0/jaraco/abode/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/devices/status.py` & `jaraco.abode-5.1.0/jaraco/abode/devices/status.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/devices/switch.py` & `jaraco.abode-5.1.0/jaraco/abode/devices/switch.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/devices/valve.py` & `jaraco.abode-5.1.0/jaraco/abode/devices/valve.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/event_controller.py` & `jaraco.abode-5.1.0/jaraco/abode/event_controller.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/exceptions.py` & `jaraco.abode-5.1.0/jaraco/abode/exceptions.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/helpers/errors.py` & `jaraco.abode-5.1.0/jaraco/abode/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/helpers/events.csv` & `jaraco.abode-5.1.0/jaraco/abode/helpers/events.csv`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/helpers/timeline.py` & `jaraco.abode-5.1.0/jaraco/abode/helpers/timeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Timeline event constants."""
 
 import csv
 
 from importlib_resources import files
-from jaraco.functools import call_aside
+from jaraco.functools import invoke
 from jaraco.collections import RangeMap
 
 
 class Groups:
     """Event groups."""
 
     ALARM = 'abode_alarm'
@@ -62,15 +62,15 @@
 
 
 def _read_events():
     with files().joinpath('events.csv').open(encoding='utf-8') as strm:
         yield from csv.DictReader(strm, quoting=csv.QUOTE_NONE, skipinitialspace=True)
 
 
-@call_aside
+@invoke
 def _load_events():
     def var_name(event):
         default = (
             event['text']
             .replace(' - ', '_')
             .replace(' ', '_')
             .replace('/', '_')
```

### Comparing `jaraco.abode-5.0.1/jaraco/abode/helpers/urls.py` & `jaraco.abode-5.1.0/jaraco/abode/helpers/urls.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/settings.py` & `jaraco.abode-5.1.0/jaraco/abode/settings.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/socketio.py` & `jaraco.abode-5.1.0/jaraco/abode/socketio.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco/abode/state.py` & `jaraco.abode-5.1.0/jaraco/abode/state.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/jaraco.abode.egg-info/PKG-INFO` & `jaraco.abode-5.1.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,20 @@
-Metadata-Version: 2.1
-Name: jaraco.abode
-Version: 5.0.1
-Summary: A library interfacing to the Abode home security system
-Home-page: https://github.com/jaraco/jaraco.abode
-Author: Wil Schrader
-Author-email: wilrader@gmail.com
-Maintainer: Jason R. Coombs
-Maintainer-email: jaraco@jaraco.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
-Provides-Extra: testing
-Provides-Extra: docs
-License-File: LICENSE
-
 .. image:: https://img.shields.io/pypi/v/jaraco.abode.svg
    :target: https://pypi.org/project/jaraco.abode
 
 .. image:: https://img.shields.io/pypi/pyversions/jaraco.abode.svg
 
 .. image:: https://github.com/jaraco/jaraco.abode/workflows/tests/badge.svg
    :target: https://github.com/jaraco/jaraco.abode/actions?query=workflow%3A%22tests%22
    :alt: tests
 
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
+
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Code style: Black
 
 .. image:: https://readthedocs.org/projects/jaracoabode/badge/?version=latest
    :target: https://jaracoabode.readthedocs.io/en/latest/?badge=latest
```

### Comparing `jaraco.abode-5.0.1/jaraco.abode.egg-info/SOURCES.txt` & `jaraco.abode-5.1.0/jaraco.abode.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
 .readthedocs.yaml
-CHANGES.rst
 LICENSE
+NEWS.rst
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 setup.cfg
+towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/api.rst
 docs/conf.py
 docs/history.rst
 docs/index.rst
```

### Comparing `jaraco.abode-5.0.1/jaraco.abode.egg-info/requires.txt` & `jaraco.abode-5.1.0/jaraco.abode.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -8,31 +8,29 @@
 jaraco.classes
 jaraco.net>=9
 more_itertools
 importlib_resources>=5.10
 bx_py_utils
 platformdirs
 jaraco.itertools
+jaraco.functools>=3.6
 
 [docs]
 sphinx>=3.5
 jaraco.packaging>=9
 rst.linker>=1.9
 furo
 sphinx-lint
 
 [testing]
 pytest>=6
 pytest-checkdocs>=2.4
-flake8<5
 pytest-cov
 pytest-enabler>=1.3
+pytest-ruff
 requests_mock
 types-requests
 jaraco.collections>=4.1
 
 [testing:platform_python_implementation != "PyPy"]
 pytest-black>=0.3.7
 pytest-mypy>=0.9.1
-
-[testing:python_version < "3.12"]
-pytest-flake8
```

### Comparing `jaraco.abode-5.0.1/pytest.ini` & `jaraco.abode-5.1.0/pytest.ini`

 * *Files 26% similar despite different names*

```diff
@@ -3,30 +3,25 @@
 addopts=--doctest-modules
 filterwarnings=
 	## upstream
 
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
-	# Suppress deprecation warning in flake8
-	ignore:SelectableGroups dict interface is deprecated::flake8
-
 	# shopkeep/pytest-black#55
 	ignore:<class 'pytest_black.BlackItem'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
 	ignore:The \(fspath. py.path.local\) argument to BlackItem is deprecated.:pytest.PytestDeprecationWarning
 	ignore:BlackItem is an Item subclass and should not be a collector:pytest.PytestWarning
 
-	# tholo/pytest-flake8#83
-	ignore:<class 'pytest_flake8.Flake8Item'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
-	ignore:The \(fspath. py.path.local\) argument to Flake8Item is deprecated.:pytest.PytestDeprecationWarning
-	ignore:Flake8Item is an Item subclass and should not be a collector:pytest.PytestWarning
-
 	# shopkeep/pytest-black#67
 	ignore:'encoding' argument not specified::pytest_black
 
 	# realpython/pytest-mypy#152
 	ignore:'encoding' argument not specified::pytest_mypy
 
 	# python/cpython#100750
 	ignore:'encoding' argument not specified::platform
 
+	# pypa/build#615
+	ignore:'encoding' argument not specified::build.env
+
 	## end upstream
```

### Comparing `jaraco.abode-5.0.1/setup.cfg` & `jaraco.abode-5.1.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find_namespace:
 include_package_data = true
-python_requires = >=3.7
+python_requires = >=3.8
 install_requires = 
 	requests >= 2.12.4
 	lomond >= 0.3.3
 	colorlog >= 3.0.1
 	keyring
 	requests_toolbelt
 	jaraco.collections
@@ -29,35 +29,34 @@
 	jaraco.classes
 	jaraco.net >= 9
 	more_itertools
 	importlib_resources >= 5.10
 	bx_py_utils
 	platformdirs
 	jaraco.itertools
+	jaraco.functools >= 3.6
 
 [options.packages.find]
 exclude = 
 	build*
 	dist*
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8; \
-	python_version < "3.12"
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 1.3
+	pytest-ruff
 	
 	requests_mock
 	types-requests
 	jaraco.collections >= 4.1
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
```

### Comparing `jaraco.abode-5.0.1/tests/mock/__init__.py` & `jaraco.abode-5.1.0/tests/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/automation.py` & `jaraco.abode-5.1.0/tests/mock/automation.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/__init__.py` & `jaraco.abode-5.1.0/tests/mock/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/dimmer.py` & `jaraco.abode-5.1.0/tests/mock/devices/dimmer.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/door_contact.py` & `jaraco.abode-5.1.0/tests/mock/devices/door_contact.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/door_lock.py` & `jaraco.abode-5.1.0/tests/mock/devices/door_lock.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/glass.py` & `jaraco.abode-5.1.0/tests/mock/devices/glass.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/hue.py` & `jaraco.abode-5.1.0/tests/mock/devices/hue.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/ipcam.py` & `jaraco.abode-5.1.0/tests/mock/devices/ipcam.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/ir_camera.py` & `jaraco.abode-5.1.0/tests/mock/devices/ir_camera.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/keypad.py` & `jaraco.abode-5.1.0/tests/mock/devices/keypad.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/lm.py` & `jaraco.abode-5.1.0/tests/mock/devices/lm.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/pir.py` & `jaraco.abode-5.1.0/tests/mock/devices/pir.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/power_switch_meter.py` & `jaraco.abode-5.1.0/tests/mock/devices/power_switch_meter.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/power_switch_sensor.py` & `jaraco.abode-5.1.0/tests/mock/devices/power_switch_sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/remote_controller.py` & `jaraco.abode-5.1.0/tests/mock/devices/remote_controller.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/secure_barrier.py` & `jaraco.abode-5.1.0/tests/mock/devices/secure_barrier.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/siren.py` & `jaraco.abode-5.1.0/tests/mock/devices/siren.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/status_display.py` & `jaraco.abode-5.1.0/tests/mock/devices/status_display.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/unknown.py` & `jaraco.abode-5.1.0/tests/mock/devices/unknown.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/valve.py` & `jaraco.abode-5.1.0/tests/mock/devices/valve.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/devices/water_sensor.py` & `jaraco.abode-5.1.0/tests/mock/devices/water_sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/login.py` & `jaraco.abode-5.1.0/tests/mock/login.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/panel.py` & `jaraco.abode-5.1.0/tests/mock/panel.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/mock/user.py` & `jaraco.abode-5.1.0/tests/mock/user.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_abode.py` & `jaraco.abode-5.1.0/tests/test_abode.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_alarm.py` & `jaraco.abode-5.1.0/tests/test_alarm.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_automation.py` & `jaraco.abode-5.1.0/tests/test_automation.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_binary_sensor.py` & `jaraco.abode-5.1.0/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_camera.py` & `jaraco.abode-5.1.0/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_device.py` & `jaraco.abode-5.1.0/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_dimmer.py` & `jaraco.abode-5.1.0/tests/test_dimmer.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_door_lock.py` & `jaraco.abode-5.1.0/tests/test_door_lock.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_event_controller.py` & `jaraco.abode-5.1.0/tests/test_event_controller.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_hue.py` & `jaraco.abode-5.1.0/tests/test_hue.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_lm.py` & `jaraco.abode-5.1.0/tests/test_lm.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_power_switch_meter.py` & `jaraco.abode-5.1.0/tests/test_power_switch_meter.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_power_switch_sensor.py` & `jaraco.abode-5.1.0/tests/test_power_switch_sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_secure_barrier.py` & `jaraco.abode-5.1.0/tests/test_secure_barrier.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tests/test_valve.py` & `jaraco.abode-5.1.0/tests/test_valve.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.0.1/tox.ini` & `jaraco.abode-5.1.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,8 @@
 [tox]
-envlist = python
-minversion = 3.2
-# https://github.com/jaraco/skeleton/issues/6
-tox_pip_extensions_ext_venv_update = true
 toxworkdir={env:TOX_WORK_DIR:.tox}
 
 
 [testenv]
 deps =
 	# workaround for jamielennox/requests-mock#17
 	requests_mock@git+https://github.com/jaraco/requests-mock@bugfix-17
@@ -23,14 +19,24 @@
 	docs
 	testing
 changedir = docs
 commands =
 	python -m sphinx -W --keep-going . {toxinidir}/build/html
 	python -m sphinxlint
 
+[testenv:finalize]
+skip_install = True
+deps =
+	towncrier
+	jaraco.develop >= 7.23
+passenv = *
+commands =
+	python -m jaraco.develop.finalize
+
+
 [testenv:release]
 skip_install = True
 deps =
 	build
 	twine>=3
 	jaraco.develop>=7.1
 passenv =
```

