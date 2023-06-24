# Comparing `tmp/isocodes-2023.6.13.tar.gz` & `tmp/isocodes-2023.6.24.tar.gz`

## Comparing `isocodes-2023.6.13.tar` & `isocodes-2023.6.24.tar`

### file list

```diff
@@ -1,1163 +1,1163 @@
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.gitmodules
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.pre-commit-config.yaml
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 isocodes-2023.6.13/tox.ini
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 isocodes-2023.6.13/update.sh
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.github/dependabot.yml
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.github/workflows/publish-test.yaml
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.github/workflows/test.yaml
--rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/__init__.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/py.typed
--rw-r--r--   0        0        0    17097 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_15924.json
--rw-r--r--   0        0        0    43284 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-1.json
--rw-r--r--   0        0        0   501099 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-2.json
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-3.json
--rw-r--r--   0        0        0    16584 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_4217.json
--rw-r--r--   0        0        0    36852 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-2.json
--rw-r--r--   0        0        0   874782 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-3.json
--rw-r--r--   0        0        0     8486 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-5.json
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-15924.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-1.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-2.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-3.json
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-4217.json
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-2.json
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-3.json
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-5.json
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ab/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ab/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ab/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ab/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ace/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ace/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ach/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ach/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    22487 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5414 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ak/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ak/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/an/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/an/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    28339 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    33554 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    31617 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    22752 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22649 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   311331 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ay/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ay/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ba/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ba/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6864 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bar/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bar/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    30045 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   201179 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    27908 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    18766 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    28945 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    15126 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    24471 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bi/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    35751 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    33036 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    96597 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    35713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    10555 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    32879 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    22283 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23927 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9059 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23424 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    25765 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ce/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ce/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ch/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ch/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/chr/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/chr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    21581 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    20258 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   256161 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24094 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24860 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    14412 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/csb/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/csb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cv/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cv/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23789 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    35290 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    15797 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    14506 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10182 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23328 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   135392 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8861 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22920 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    19729 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23454 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   219517 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23574 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   395556 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    11257 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/dv/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/dv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    40229 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/dz/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ee/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ee/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    57390 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    91227 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/en/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/en/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8524 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23042 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    47595 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22133 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    48656 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10493 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23741 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    15724 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23281 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    33190 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     9689 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23059 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22375 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    30637 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23811 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    23772 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    21800 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    20888 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    26404 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ff/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ff/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    22418 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    21391 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    10473 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23844 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24141 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   166186 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9303 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23058 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   407281 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/frp/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/frp/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    23756 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    22913 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fy/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/fy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    23528 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    14446 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22867 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   306888 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gn/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    35101 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    32619 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    44025 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gv/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/gv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ha/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ha/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/haw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    27802 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    35310 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23488 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    26178 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    15454 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    52545 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ht/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ht/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24519 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    69162 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22864 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    37180 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    30567 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/hy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23086 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   165253 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23311 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   292415 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/io/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/io/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24295 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23986 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   149997 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23660 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   163383 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23171 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   369645 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/iu/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/iu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24942 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   100171 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23644 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    16790 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/jam/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/jam/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    36655 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   109788 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    13229 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    14569 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0     6371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ki/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ki/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kl/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    35806 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/km/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/km/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/km/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    21966 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    29606 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    32465 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   390349 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24204 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9975 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24693 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    18040 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kv/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9310 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kw/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/kw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    29069 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lo/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23186 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    75936 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22164 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    31678 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    22888 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    21927 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mai/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mai/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10467 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    27425 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    34752 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    34245 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mo/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    35144 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    32230 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   425099 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/my/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/my/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/na/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/na/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nah/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nah/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23349 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    32389 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ne/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23512 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   213685 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23302 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    86365 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    21966 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nv/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/nv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23749 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    34110 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    32596 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   217560 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    31594 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   410401 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    14875 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pap/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pap/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pi/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23849 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   188055 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9807 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23814 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   121821 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23926 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23190 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    15062 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24079 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23166 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    22866 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    27706 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7042 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23251 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    10854 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro_MD/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ro_MD/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   112174 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    11510 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    29137 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    18412 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     9598 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    21974 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    15826 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    10473 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24430 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   104509 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    23525 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    19985 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sd/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sd/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    31931 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23531 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24319 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    22611 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    79740 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    14346 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/son/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/son/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23866 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24241 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   145300 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    29938 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    17095 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23246 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   122426 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24379 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    14420 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23553 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   164336 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9466 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   398696 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     7984 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/sw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    31984 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    33169 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   438383 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    35338 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    32092 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0    28527 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    33663 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    83632 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    18477 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    53438 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    18029 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    21411 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    10222 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23676 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    77264 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24213 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   343245 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    21810 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0    29812 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ug/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    29887 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   265202 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    12535 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    29090 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0   511201 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-3.mo
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ur/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ur/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uz/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/uz/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    24644 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   135733 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    27170 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    16925 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    22427 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wal/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0    21638 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/wo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/yo/LC_MESSAGES/iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/yo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23425 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0   117078 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24039 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23388 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24126 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639-5.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
--rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_15924.mo
--rw-r--r--   0        0        0    23390 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0    18281 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-2.mo
--rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
--rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_4217.mo
--rw-r--r--   0        0        0    24253 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0    32698 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_3166-1.mo
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_3166-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639-2.mo
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639-3.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/pkgconfig/iso-codes.pc
--rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_15924.xml
--rw-r--r--   0        0        0    40003 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166-1.xml
--rw-r--r--   0        0        0   334692 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166-2.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166-3.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166.xml -> iso_3166-1.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166_2.xml -> iso_3166-2.xml
--rw-r--r--   0        0        0    31649 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_4217.xml
--rw-r--r--   0        0        0    48857 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-2.xml
--rw-r--r--   0        0        0  1016601 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-3.xml
--rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-5.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639.xml -> iso_639-2.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639_3.xml -> iso_639-3.xml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639_5.xml -> iso_639-5.xml
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 isocodes-2023.6.13/requirements/build-requirements.txt
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 isocodes-2023.6.13/requirements/dev-requirements.txt
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 isocodes-2023.6.13/requirements/doc-requirements.txt
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 isocodes-2023.6.13/requirements/requirements.txt
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 isocodes-2023.6.13/requirements/test-requirements.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 isocodes-2023.6.13/tests/__init__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 isocodes-2023.6.13/tests/test_general.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 isocodes-2023.6.13/.gitignore
--rw-r--r--   0        0        0    24477 2020-02-02 00:00:00.000000 isocodes-2023.6.13/LICENSE
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 isocodes-2023.6.13/README.md
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 isocodes-2023.6.13/pyproject.toml
--rw-r--r--   0        0        0    32330 2020-02-02 00:00:00.000000 isocodes-2023.6.13/PKG-INFO
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 isocodes-2023.6.24/.gitmodules
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 isocodes-2023.6.24/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 isocodes-2023.6.24/tox.ini
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 isocodes-2023.6.24/update.sh
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 isocodes-2023.6.24/.github/dependabot.yml
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 isocodes-2023.6.24/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 isocodes-2023.6.24/.github/workflows/publish-test.yaml
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 isocodes-2023.6.24/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 isocodes-2023.6.24/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/__init__.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/py.typed
+-rw-r--r--   0        0        0    17097 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_15924.json
+-rw-r--r--   0        0        0    43284 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_3166-1.json
+-rw-r--r--   0        0        0   501099 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_3166-2.json
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_3166-3.json
+-rw-r--r--   0        0        0    16584 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_4217.json
+-rw-r--r--   0        0        0    36852 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_639-2.json
+-rw-r--r--   0        0        0   874782 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_639-3.json
+-rw-r--r--   0        0        0     8486 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_639-5.json
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-15924.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-3166-1.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-3166-2.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-3166-3.json
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-4217.json
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-639-2.json
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-639-3.json
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-639-5.json
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ab/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ab/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ab/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ab/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ace/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ace/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9088 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ach/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ach/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    22487 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/af/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/af/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/af/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6732 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/af/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5414 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/af/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/af/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/af/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ak/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ak/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6413 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/am/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/am/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/am/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5736 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/am/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/am/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/am/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/am/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/an/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/an/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    28339 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    10214 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    33554 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/as/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4070 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/as/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/as/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    31617 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/as/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/as/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    22752 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22649 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   311331 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ay/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ay/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ba/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ba/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6864 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bar/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bar/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    12701 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    30045 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   201179 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3661 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    12256 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    27908 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    18766 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    28945 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    15126 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    15143 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    24471 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bi/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    35751 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4015 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    33036 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    96597 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    35713 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    10555 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    32879 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    22283 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2593 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5711 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/byn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5632 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/byn/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5693 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/byn/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/byn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/byn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23927 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9059 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23424 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    25765 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    10819 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ce/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ce/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ch/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ch/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5143 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/chr/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/chr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    21581 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    20258 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   256161 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24094 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     9150 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24860 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14412 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/csb/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/csb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cv/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    10906 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cv/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23789 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    35290 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    15797 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14506 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10182 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23328 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   135392 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8861 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22920 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    19729 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10383 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23454 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   219517 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23574 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   395556 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    11257 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/dv/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/dv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    40229 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/dz/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ee/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ee/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9431 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     9080 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    57390 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    91227 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/en/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/en/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8524 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23042 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    47595 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8374 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22133 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    48656 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10493 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23741 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    15724 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23281 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    33190 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9689 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23059 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22375 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    30637 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7437 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23811 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    23772 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2745 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    21800 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    20888 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    26404 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    13407 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ff/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ff/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    22418 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    21391 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    10473 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fil/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23844 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fil/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fil/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     5837 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24141 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   166186 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9303 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23058 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   407281 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/frp/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/frp/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    23756 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    22913 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     9356 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fy/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/fy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    23528 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    14446 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5761 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gez/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gez/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5696 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gez/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gez/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gez/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     8054 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23252 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22867 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   306888 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gn/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    35101 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3904 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    32619 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gu/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    44025 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gu/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     8982 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gv/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/gv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ha/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ha/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/haw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     3410 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    27802 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    34323 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5910 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    35310 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6646 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10432 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23488 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    26178 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    15454 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    52545 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7671 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ht/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ht/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24519 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    69162 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22864 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    37180 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    30567 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3474 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/hy/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8085 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ia/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ia/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23086 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   165253 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23311 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   292415 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     9210 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/io/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/io/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10637 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24295 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4405 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9804 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23986 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   149997 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     8015 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     9447 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23660 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   163383 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9244 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23171 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   369645 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/iu/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/iu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4131 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24942 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   100171 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2724 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    10051 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23644 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    16790 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     8321 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/jam/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/jam/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    36655 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   109788 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    13229 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    14569 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0     6371 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     5119 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ki/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ki/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    29652 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kl/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    35806 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/km/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/km/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/km/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    21966 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kmr/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kmr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    29606 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    32465 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kn/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   390349 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kn/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24204 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3047 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9975 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24693 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    18040 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     6506 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kok/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kok/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kok/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kok/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5803 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kv/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9310 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kw/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/kw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    29069 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ky/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ky/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     5756 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lo/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23186 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    75936 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2767 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22164 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    31678 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9267 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    22888 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    21927 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    10625 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     4535 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mai/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mai/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10467 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mi/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mi/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    27425 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mk/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2178 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mk/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ml/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    34752 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4406 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ml/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    34245 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ml/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ml/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0    10101 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5207 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mo/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    35144 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3916 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    32230 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mr/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   425099 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mr/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ms/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ms/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ms/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ms/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ms/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mt/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mt/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/mt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    15588 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/my/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/my/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/na/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/na/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8116 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nah/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nah/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23349 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8569 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5570 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    32389 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ne/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10224 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23512 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   213685 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23302 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    86365 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    21966 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     7462 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     7830 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nv/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/nv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1713 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23749 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     5714 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0     6852 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    34110 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/or/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/or/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/or/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    32596 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/or/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   217560 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/or/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/or/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/or/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    30504 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3356 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    31594 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   410401 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    14875 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pap/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pap/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9264 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pi/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23849 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   188055 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9807 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23814 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   121821 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7985 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ps/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ps/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ps/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ps/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ps/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23926 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23190 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    15062 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    10363 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24079 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23166 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    17829 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    22866 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    27706 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7042 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23251 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    10854 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro_MD/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ro_MD/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    29823 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   112174 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    11510 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    29137 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    18412 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     9598 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    21974 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     4998 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    15826 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    10473 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24430 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   104509 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    23525 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    19985 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sd/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sd/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/si/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    31931 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/si/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/si/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/si/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23531 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    13211 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24319 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    11443 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    22611 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    79740 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24028 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14346 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0     6066 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     9275 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/son/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/son/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23866 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24241 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    12875 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    28915 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   145300 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3352 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9338 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    29938 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    17095 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     4031 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10451 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23246 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   122426 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24379 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14420 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23553 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   164336 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9466 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    22999 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   398696 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7469 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     7984 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/sw/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    31984 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ta/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    33169 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ta/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   438383 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ta/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ta/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ta/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    35338 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/te/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/te/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/te/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    32092 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/te/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/te/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0    28527 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tg/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tg/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tg/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tg/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0    11584 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    33663 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    83632 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    10193 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    18477 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    53438 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ti/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ti/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ti/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ti/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ti/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tig/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tig/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tig/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tig/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tig/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    18029 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    21411 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tl/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    10222 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23676 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    77264 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24213 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   343245 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    21810 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     7090 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    18209 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     6281 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tzm/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tzm/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tzm/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/tzm/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0    29812 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ug/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    12713 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    29887 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   265202 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    12535 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    29090 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0   511201 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_639-3.mo
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ur/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ur/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8863 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uz/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/uz/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     7913 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    24644 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   135733 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     8278 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    27170 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    16925 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    22427 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    12889 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5713 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wal/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0    21638 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/wo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/xh/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/xh/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/xh/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/xh/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/xh/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0    11032 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/yo/LC_MESSAGES/iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/yo/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     7170 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23425 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0   117078 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24039 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     4992 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23388 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     8815 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24126 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0     7424 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639-5.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639_5.mo -> iso_639-5.mo
+-rw-r--r--   0        0        0    10644 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_15924.mo
+-rw-r--r--   0        0        0    23390 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0    18281 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-2.mo
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166_2.mo -> iso_3166-2.mo
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_4217.mo
+-rw-r--r--   0        0        0    24253 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0    32698 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0     5882 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zu/LC_MESSAGES/iso_3166-1.mo
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zu/LC_MESSAGES/iso_3166-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zu/LC_MESSAGES/iso_3166.mo -> iso_3166-1.mo
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zu/LC_MESSAGES/iso_639-2.mo
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zu/LC_MESSAGES/iso_639-3.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zu/LC_MESSAGES/iso_639.mo -> iso_639-2.mo
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/locale/zu/LC_MESSAGES/iso_639_3.mo -> iso_639-3.mo
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/pkgconfig/iso-codes.pc
+-rw-r--r--   0        0        0    17766 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_15924.xml
+-rw-r--r--   0        0        0    40003 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_3166-1.xml
+-rw-r--r--   0        0        0   334692 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_3166-2.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_3166-3.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_3166.xml -> iso_3166-1.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_3166_2.xml -> iso_3166-2.xml
+-rw-r--r--   0        0        0    31649 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_4217.xml
+-rw-r--r--   0        0        0    48857 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_639-2.xml
+-rw-r--r--   0        0        0  1016601 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_639-3.xml
+-rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_639-5.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_639.xml -> iso_639-2.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_639_3.xml -> iso_639-3.xml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_639_5.xml -> iso_639-5.xml
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 isocodes-2023.6.24/requirements/build-requirements.txt
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 isocodes-2023.6.24/requirements/dev-requirements.txt
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 isocodes-2023.6.24/requirements/doc-requirements.txt
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 isocodes-2023.6.24/requirements/requirements.txt
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 isocodes-2023.6.24/requirements/test-requirements.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 isocodes-2023.6.24/tests/__init__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 isocodes-2023.6.24/tests/test_general.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 isocodes-2023.6.24/.gitignore
+-rw-r--r--   0        0        0    24477 2020-02-02 00:00:00.000000 isocodes-2023.6.24/LICENSE
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 isocodes-2023.6.24/README.md
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 isocodes-2023.6.24/pyproject.toml
+-rw-r--r--   0        0        0    32330 2020-02-02 00:00:00.000000 isocodes-2023.6.24/PKG-INFO
```

### Comparing `isocodes-2023.6.13/.pre-commit-config.yaml` & `isocodes-2023.6.24/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/.github/workflows/codeql.yml` & `isocodes-2023.6.24/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/.github/workflows/publish-test.yaml` & `isocodes-2023.6.24/.github/workflows/publish-test.yaml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/.github/workflows/publish.yaml` & `isocodes-2023.6.24/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/.github/workflows/test.yaml` & `isocodes-2023.6.24/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/__init__.py` & `isocodes-2023.6.24/isocodes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 LOCALES_DIR = f"{BASE_DIR}/share/locale"
 
 
 class ISO:
     def __init__(self, iso_key: str) -> None:
         self.iso_key: str = iso_key
         with open(
-            f"{BASE_DIR}/share/iso-codes/json/iso_{self.iso_key}.json"
+            f"{BASE_DIR}/share/iso-codes/json/iso_{self.iso_key}.json", encoding="utf-8"
         ) as iso_file:
             self.data: List[Dict] = json.load(iso_file)[self.iso_key]
 
     def __len__(self) -> int:
         return len(self.data)
 
     def _name_from_index(self, index: str) -> Generator[tuple, None, None]:
```

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_15924.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_15924.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-1.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_3166-1.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-2.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_3166-2.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_3166-3.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_3166-3.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_4217.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_4217.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-2.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_639-2.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-3.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_639-3.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/iso_639-5.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/iso_639-5.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-15924.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-15924.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-1.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-3166-1.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-2.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-3166-2.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-3166-3.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-3166-3.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-4217.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-4217.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-2.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-639-2.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-3.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-639-3.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/iso-codes/json/schema-639-5.json` & `isocodes-2023.6.24/isocodes/share/iso-codes/json/schema-639-5.json`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ab/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ab/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ace/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ace/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ach/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ach/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/af/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/af/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/af/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/af/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/af/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ak/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ak/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/am/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/am/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/am/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/am/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/an/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/an/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ar/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ar/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/as/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/as/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/as/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/as/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ast/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ast/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ay/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ay/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/az/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/az/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ba/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ba/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bar/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/bar/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/be/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/be/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bg/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/bg/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/bi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn_BD/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/bn_IN/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/br/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/br/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/bs/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/bs/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/byn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/byn/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/byn/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/byn/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ca/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ca/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ce/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ce/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ch/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ch/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/chr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/chr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ckb/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/crh/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/crh/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cs/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/cs/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/csb/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/csb/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cv/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/cv/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/cv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/cy/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/cy/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/da/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/da/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/de/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/de/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/dv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/dv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/dz/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ee/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ee/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/el/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/el/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/en/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/en/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eo/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/eo/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/es/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/es/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/et/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/et/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/eu/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/eu/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fa/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/fa/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ff/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ff/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fi/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/fi/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/fil/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/fil/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/fo/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fr/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/fr/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/frp/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/frp/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fur/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/fur/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/fy/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/fy/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ga/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ga/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/gez/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/gez/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gez/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/gez/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gl/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/gl/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/gn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/gu/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/gu/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gu/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/gu/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/gv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/gv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ha/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ha/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/haw/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/he/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/he/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hi/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/hi/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hr/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/hr/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ht/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ht/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hu/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/hu/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/hy/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/ia/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ia/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/id/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/id/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/io/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/io/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/is/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/is/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/it/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/it/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/iu/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/iu/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ja/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ja/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/jam/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/jam/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ka/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/ka/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kab/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/kab/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ki/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ki/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/kk/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/kl/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/km/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/km/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/km/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/km/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/kmr/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kmr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/kmr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/kn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/kn/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kn/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/kn/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ko/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ko/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/kok/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kok/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/kok/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/kv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/kw/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/kw/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ky/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/lo/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lt/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/lt/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/lv/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/lv/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mai/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/mai/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/mhr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/mi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/mi/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mi/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/mi/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/mk/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/mk/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mk/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/mk/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/ml/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ml/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ml/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ml/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mn/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/mn/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/mo/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/mr/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/mr/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/mr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ms/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ms/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ms/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ms/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/mt/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/mt/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/mt/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/mt/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/my/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/my/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/na/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/na/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nah/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/nah/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nb/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/nb/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/nb_NO/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ne/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nl/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/nl/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nn/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/nn/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nso/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/nso/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/nv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/nv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/oc/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/oc/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/or/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/or/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/or/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/or/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/or/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/pa/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/pa/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pa/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/pa/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/pa_PK/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pap/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/pap/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/pi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pl/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/pl/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ps/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ps/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ps/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ps/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/pt_BR/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ro/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ro/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ro_MD/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ro_MD/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ru/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/ru/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/rw/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/rw/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sc/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/sc/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sd/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/sd/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/si/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/si/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/si/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/si/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sk/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sk/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sl/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sl/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/so/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/so/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/son/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/son/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sq/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sq/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/sr@latin/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sv/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/sv/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/sw/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ta/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ta/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ta/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ta/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/te/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/te/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/te/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/te/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/tg/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tg/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/tg/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/th/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/th/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ti/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ti/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ti/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ti/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/tig/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/tig/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tig/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/tig/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/tk/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/tl/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tr/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/tr/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/tt/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/tt/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tt/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/tt/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/tt@iqtelif/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/tzm/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/tzm/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/tzm/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/tzm/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ug/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/uk/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/uk/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ur/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ur/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/uz/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/uz/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/ve/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/ve/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/vi/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/vi/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/wa/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/wa/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/wal/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/wo/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/xh/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/xh/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/xh/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/xh/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/yo/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/yo/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_CN/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_HK/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_Hans/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639-5.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_Hant/LC_MESSAGES/iso_639-5.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_15924.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_15924.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_3166-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_4217.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_4217.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/zh_TW/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_3166-1.mo` & `isocodes-2023.6.24/isocodes/share/locale/zu/LC_MESSAGES/iso_3166-1.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639-2.mo` & `isocodes-2023.6.24/isocodes/share/locale/zu/LC_MESSAGES/iso_639-2.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/locale/zu/LC_MESSAGES/iso_639-3.mo` & `isocodes-2023.6.24/isocodes/share/locale/zu/LC_MESSAGES/iso_639-3.mo`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_15924.xml` & `isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_15924.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166-1.xml` & `isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_3166-1.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_3166-2.xml` & `isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_3166-2.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_4217.xml` & `isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_4217.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-2.xml` & `isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_639-2.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-3.xml` & `isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_639-3.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/isocodes/share/xml/iso-codes/iso_639-5.xml` & `isocodes-2023.6.24/isocodes/share/xml/iso-codes/iso_639-5.xml`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/requirements/build-requirements.txt` & `isocodes-2023.6.24/requirements/build-requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=build --output-file=requirements/build-requirements.txt --resolver=backtracking pyproject.toml
 #
 anyio==3.6.2
     # via httpcore
-certifi==2022.12.7
+certifi==2023.5.7
     # via
     #   httpcore
     #   httpx
 cffi==1.15.1
     # via cryptography
 click==8.1.3
     # via
@@ -75,15 +75,15 @@
     # via pexpect
 pycparser==2.21
     # via cffi
 pygments==2.15.1
     # via rich
 pyperclip==1.8.2
     # via hatch
-rich==13.3.4
+rich==13.4.2
     # via hatch
 secretstorage==3.3.3
     # via keyring
 shellingham==1.5.0.post1
     # via hatch
 sniffio==1.3.0
     # via
```

### Comparing `isocodes-2023.6.13/requirements/dev-requirements.txt` & `isocodes-2023.6.24/requirements/dev-requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via pre-commit
 distlib==0.3.6
     # via virtualenv
 filelock==3.11.0
     # via virtualenv
 identify==2.5.24
     # via pre-commit
-mypy==1.1.1
+mypy==1.3.0
     # via isocodes (pyproject.toml)
 mypy-extensions==1.0.0
     # via mypy
 nodeenv==1.7.0
     # via pre-commit
 platformdirs==3.5.3
     # via virtualenv
```

### Comparing `isocodes-2023.6.13/requirements/doc-requirements.txt` & `isocodes-2023.6.24/requirements/doc-requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --extra=doc --output-file=requirements/doc-requirements.txt --resolver=backtracking pyproject.toml
 #
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via mkdocs
 colorama==0.4.6
     # via mkdocs-material
```

### Comparing `isocodes-2023.6.13/requirements/test-requirements.txt` & `isocodes-2023.6.24/requirements/test-requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # via
     #   tox
     #   virtualenv
 pluggy==1.0.0
     # via
     #   pytest
     #   tox
-pyproject-api==1.5.1
+pyproject-api==1.5.2
     # via tox
 pytest==7.2.0
     # via isocodes (pyproject.toml)
 tomli==2.0.1
     # via
     #   pyproject-api
     #   pytest
```

### Comparing `isocodes-2023.6.13/.gitignore` & `isocodes-2023.6.24/.gitignore`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/LICENSE` & `isocodes-2023.6.24/LICENSE`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/README.md` & `isocodes-2023.6.24/README.md`

 * *Files identical despite different names*

### Comparing `isocodes-2023.6.13/pyproject.toml` & `isocodes-2023.6.24/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "isocodes"
-version = "2023.06.13"
+version = "2023.06.24"
 description = "This project provides lists of various ISO standards (e.g. country, language, language scripts, and currency names) in one place"
 authors = [{ name = "Atem18", email = "contact@atemlire.io" }]
 license = { file = "LICENSE" }
 readme = "README.md"
 homepage = "https://github.com/Atem18/isocodes"
 repository = "https://github.com/Atem18/isocodes"
 keywords = ["iso"]
@@ -16,14 +16,14 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
 ]
 dependencies = []
 
 [project.optional-dependencies]
-dev = ["pre-commit >=2.17.0,<3.0.0", "ruff == 0.0.254", "mypy == 1.1.1"]
+dev = ["pre-commit >=2.17.0,<3.0.0", "ruff == 0.0.254", "mypy == 1.3.0"]
 
 doc = ["mkdocs == 1.4.2", "mkdocs-material == 9.1.15", "mkdocstrings == 0.19.1"]
 
 test = ["pytest == 7.2.0", "tox == 4.5.1"]
 
 build = ["hatch == 1.7.0"]
```

### Comparing `isocodes-2023.6.13/PKG-INFO` & `isocodes-2023.6.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isocodes
-Version: 2023.6.13
+Version: 2023.6.24
 Summary: This project provides lists of various ISO standards (e.g. country, language, language scripts, and currency names) in one place
 Author-email: Atem18 <contact@atemlire.io>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
@@ -465,15 +465,15 @@
 Keywords: iso
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: build
 Requires-Dist: hatch==1.7.0; extra == 'build'
 Provides-Extra: dev
-Requires-Dist: mypy==1.1.1; extra == 'dev'
+Requires-Dist: mypy==1.3.0; extra == 'dev'
 Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: ruff==0.0.254; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mkdocs-material==9.1.15; extra == 'doc'
 Requires-Dist: mkdocs==1.4.2; extra == 'doc'
 Requires-Dist: mkdocstrings==0.19.1; extra == 'doc'
 Provides-Extra: test
```

