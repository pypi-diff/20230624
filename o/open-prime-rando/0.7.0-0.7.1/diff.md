# Comparing `tmp/open-prime-rando-0.7.0.tar.gz` & `tmp/open-prime-rando-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-prime-rando-0.7.0.tar", last modified: Fri Jun 23 11:18:52 2023, max compression
+gzip compressed data, was "open-prime-rando-0.7.1.tar", last modified: Sat Jun 24 00:44:49 2023, max compression
```

## Comparing `open-prime-rando-0.7.0.tar` & `open-prime-rando-0.7.1.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.932643 open-prime-rando-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.916643 open-prime-rando-0.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.916643 open-prime-rando-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-23 11:18:52.932643 open-prime-rando-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-23 11:18:52.932643 open-prime-rando-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.916643 open-prime-rando-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.920643 open-prime-rando-0.7.0/src/open_prime_rando/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.920643 open-prime-rando-0.7.0/src/open_prime_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.920643 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/all_prime_dol_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.920643 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/corruption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/corruption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/corruption/dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/corruption/dol_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/dol_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.924643 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/beam_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/dol_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/dol_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/user_preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.924643 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/prime1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/prime1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/prime1/dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/prime1/dol_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/dynamic_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.924643 open-prime-rando-0.7.0/src/open_prime_rando/echoes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.924643 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/agon_wastes.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/great_temple.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/m02_spires.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/m04_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
--rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/temple_grounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/torvus_bog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.916643 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.928643 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/doors/
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.928643 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/rubiks/
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.928643 open-prime-rando-0.7.0/src/open_prime_rando/echoes/dock_lock_rando/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/dock_lock_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20626 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.928643 open-prime-rando-0.7.0/src/open_prime_rando/echoes/elevators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/elevators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/elevators/elevator_rando.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.928643 open-prime-rando-0.7.0/src/open_prime_rando/echoes/inverted/
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/inverted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/inverted/area_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.928643 open-prime-rando-0.7.0/src/open_prime_rando/echoes/small_randomizations/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/small_randomizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/small_randomizations/echo_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/small_randomizations/rubiks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/specific_area_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes/vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/echoes_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/p1r_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.928643 open-prime-rando-0.7.0/src/open_prime_rando/prime_remastered/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/prime_remastered/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/unique_area_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/src/open_prime_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 11:18:52.000000 open-prime-rando-0.7.0/src/open_prime_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.920643 open-prime-rando-0.7.0/src/open_prime_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-23 11:18:52.000000 open-prime-rando-0.7.0/src/open_prime_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-23 11:18:52.000000 open-prime-rando-0.7.0/src/open_prime_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:18:52.000000 open-prime-rando-0.7.0/src/open_prime_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 11:18:52.000000 open-prime-rando-0.7.0/src/open_prime_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 11:18:52.000000 open-prime-rando-0.7.0/src/open_prime_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 11:18:52.000000 open-prime-rando-0.7.0/src/open_prime_rando.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.928643 open-prime-rando-0.7.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.928643 open-prime-rando-0.7.0/tests/dol_patching/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/tests/dol_patching/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/tests/dol_patching/test_all_prime_dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/tests/dol_patching/test_dol_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/tests/dol_patching/test_echoes_dol_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    17803 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/tests/dol_patching/test_echoes_dol_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/tests/test_echoes_custom_Assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:18:52.932643 open-prime-rando-0.7.0/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-23 11:18:36.000000 open-prime-rando-0.7.0/tools/asset_id_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.970483 open-prime-rando-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/all_prime_dol_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/corruption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/corruption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/corruption/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/corruption/dol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/dol_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/beam_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/user_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.978483 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/dol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/dynamic_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.978483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.978483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/agon_wastes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/great_temple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m02_spires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m04_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/temple_grounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/torvus_bog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.970483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.978483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.978483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20626 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/elevator_rando.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/inverted/
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/inverted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/inverted/area_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/echo_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/rubiks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/specific_area_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes/vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/echoes_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/p1r_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/src/open_prime_rando/prime_remastered/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/prime_remastered/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/unique_area_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/src/open_prime_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.974483 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-24 00:44:49.000000 open-prime-rando-0.7.1/src/open_prime_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/tests/dol_patching/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/dol_patching/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/dol_patching/test_all_prime_dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/dol_patching/test_dol_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/dol_patching/test_echoes_dol_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17803 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/dol_patching/test_echoes_dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tests/test_echoes_custom_Assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 00:44:49.982483 open-prime-rando-0.7.1/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-24 00:44:32.000000 open-prime-rando-0.7.1/tools/asset_id_files.py
```

### Comparing `open-prime-rando-0.7.0/.github/dependabot.yml` & `open-prime-rando-0.7.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/.github/workflows/python.yml` & `open-prime-rando-0.7.1/.github/workflows/python.yml`

 * *Files 2% similar despite different names*

```diff
@@ -98,20 +98,21 @@
         run: venv/bin/python -m pip install --upgrade pip
 
       - name: install built wheel
         run: venv/bin/python -m pip install -e .[test]
 
       - name: Run Tests
         run:
-          venv/bin/python -m pytest --cov --durations=100
+          venv/bin/python -m pytest --cov src --cov-report=xml --durations=100
 
       - name: codecov
         uses: codecov/codecov-action@v3
         with:
-          fail_ci_if_error: true
+          fail_ci_if_error: false
+          files: ./coverage.xml
         env:
           CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
 
   ruff:
     runs-on: 'ubuntu-latest'
 
     steps:
```

### Comparing `open-prime-rando-0.7.0/.gitignore` & `open-prime-rando-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/LICENSE` & `open-prime-rando-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/PKG-INFO` & `open-prime-rando-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.7.0
+Version: 0.7.1
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
 Author: Henrique Gemignani
 Project-URL: Homepage, https://github.com/randovania/open-prime-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `open-prime-rando-0.7.0/pyproject.toml` & `open-prime-rando-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/cli.py` & `open-prime-rando-0.7.1/src/open_prime_rando/cli.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/all_prime_dol_patches.py` & `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/all_prime_dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/corruption/dol_versions.py` & `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/corruption/dol_versions.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/dol_version.py` & `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/dol_version.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/beam_configuration.py` & `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/beam_configuration.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/dol_patcher.py` & `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_patcher.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/dol_patches.py` & `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/dol_versions.py` & `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/dol_versions.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/echoes/user_preferences.py` & `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/echoes/user_preferences.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/prime1/dol_patches.py` & `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/dol_patching/prime1/dol_versions.py` & `open-prime-rando-0.7.1/src/open_prime_rando/dol_patching/prime1/dol_versions.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/dynamic_schema.py` & `open-prime-rando-0.7.1/src/open_prime_rando/dynamic_schema.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/agon_wastes.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/agon_wastes.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/great_temple.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/great_temple.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/temple_grounds.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/temple_grounds.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/torvus_bog.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/torvus_bog.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/asset_ids/world.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/asset_ids/world.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/custom_assets.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/custom_assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/dock_lock_rando/__init__.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/__init__.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/elevators/elevator_rando.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/elevators/elevator_rando.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/inverted/__init__.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/inverted/__init__.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/inverted/area_pairs.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/inverted/area_pairs.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/schema.json` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/schema.json`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/small_randomizations/__init__.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/__init__.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/small_randomizations/echo_locks.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/echo_locks.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/specific_area_patches.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/specific_area_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes/vulnerabilities.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/echoes_patcher.py` & `open-prime-rando-0.7.1/src/open_prime_rando/echoes_patcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 import json
 import logging
 from collections.abc import Callable
 from pathlib import Path
 
 from retro_data_structures.asset_manager import FileProvider
 from retro_data_structures.formats.mrea import Area
@@ -93,14 +94,34 @@
                 paks = editor.find_paks(old_strg)
                 new_strg = editor.add_file(f"custom_name_for_{area.internal_name}.STRG", strg, paks)
                 area._raw.area_name_id = new_strg
 
             area.build_mlvl_dependencies(only_modified=True)
 
 
+def apply_corrupted_memory_card_change(editor: PatcherEditor):
+    # STRG_MemoryCard_0
+    table = editor.get_file(0x88E242D6, Strg)
+
+    name_to_index = {
+        table.raw.name_table.name_array[entry.offset].string: entry.index
+        for entry in table.raw.name_table.name_entries
+    }
+
+    table.set_string(
+        name_to_index["CorruptedFile"],
+        """The save file was created using a different
+Randomizer ISO and must be deleted."""
+    )
+    table.set_string(
+        name_to_index["ChoiceDeleteCorruptedFile"],
+        "Delete Incompatible File"
+    )
+
+
 def patch_paks(file_provider: FileProvider,
                output_path: Path,
                configuration: dict,
                status_update: Callable[[str, float], None] = lambda s, _: LOG.info(s)):
     status_update(f"Will patch files at {file_provider}", 0)
 
     editor = PatcherEditor(file_provider, Game.ECHOES)
@@ -113,14 +134,15 @@
 
     status_update("Applying small patches", 0)
     dock_lock_rando.add_custom_models(editor)
     if configuration["auto_enabled_elevators"]:
         auto_enabled_elevator_patches.apply_auto_enabled_elevators_patch(editor)
     specific_area_patches.specific_patches(editor, configuration["area_patches"])
     apply_small_randomizations(editor, configuration["small_randomizations"])
+    apply_corrupted_memory_card_change(editor)
     apply_area_modifications(editor, configuration["worlds"], status_update)
 
     if configuration["inverted"]:
         apply_inverted(editor)
 
     # Save our changes
     editor.flush_modified_assets()
```

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/p1r_patcher.py` & `open-prime-rando-0.7.1/src/open_prime_rando/p1r_patcher.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/patcher_editor.py` & `open-prime-rando-0.7.1/src/open_prime_rando/patcher_editor.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando/validator_with_default.py` & `open-prime-rando-0.7.1/src/open_prime_rando/validator_with_default.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando.egg-info/PKG-INFO` & `open-prime-rando-0.7.1/src/open_prime_rando.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.7.0
+Version: 0.7.1
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
 Author: Henrique Gemignani
 Project-URL: Homepage, https://github.com/randovania/open-prime-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `open-prime-rando-0.7.0/src/open_prime_rando.egg-info/SOURCES.txt` & `open-prime-rando-0.7.1/src/open_prime_rando.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
+codecov.yml
 pyproject.toml
 setup.cfg
 .github/dependabot.yml
 .github/workflows/python.yml
 src/open_prime_rando/__init__.py
 src/open_prime_rando/__main__.py
 src/open_prime_rando/cli.py
```

### Comparing `open-prime-rando-0.7.0/tests/dol_patching/conftest.py` & `open-prime-rando-0.7.1/tests/dol_patching/conftest.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/tests/dol_patching/test_all_prime_dol_patches.py` & `open-prime-rando-0.7.1/tests/dol_patching/test_all_prime_dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/tests/dol_patching/test_dol_version.py` & `open-prime-rando-0.7.1/tests/dol_patching/test_dol_version.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/tests/dol_patching/test_echoes_dol_patcher.py` & `open-prime-rando-0.7.1/tests/dol_patching/test_echoes_dol_patcher.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/tests/dol_patching/test_echoes_dol_patches.py` & `open-prime-rando-0.7.1/tests/dol_patching/test_echoes_dol_patches.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/tests/test_echoes_custom_Assets.py` & `open-prime-rando-0.7.1/tests/test_echoes_custom_Assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.7.0/tools/asset_id_files.py` & `open-prime-rando-0.7.1/tools/asset_id_files.py`

 * *Files identical despite different names*

