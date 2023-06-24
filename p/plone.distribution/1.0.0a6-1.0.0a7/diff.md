# Comparing `tmp/plone.distribution-1.0.0a6.tar.gz` & `tmp/plone.distribution-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.distribution-1.0.0a6.tar", last modified: Fri Jun 23 23:11:01 2023, max compression
+gzip compressed data, was "plone.distribution-1.0.0a7.tar", last modified: Sat Jun 24 19:48:29 2023, max compression
```

## Comparing `plone.distribution-1.0.0a6.tar` & `plone.distribution-1.0.0a7.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.125752 plone.distribution-1.0.0a6/
--rw-r--r--   0 ericof     (501) staff       (20)     1342 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/.editorconfig
--rw-r--r--   0 ericof     (501) staff       (20)      540 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/.flake8
--rw-r--r--   0 ericof     (501) staff       (20)      663 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/.gitignore
--rw-r--r--   0 ericof     (501) staff       (20)      557 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/.meta.toml
--rw-r--r--   0 ericof     (501) staff       (20)     1740 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/.pre-commit-config.yaml
--rw-r--r--   0 ericof     (501) staff       (20)     1919 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/CHANGES.md
--rw-r--r--   0 ericof     (501) staff       (20)       95 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/CONTRIBUTING.md
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/LICENSE
--rw-r--r--   0 ericof     (501) staff       (20)      269 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)     5109 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/Makefile
--rw-r--r--   0 ericof     (501) staff       (20)     9765 2023-06-23 23:11:01.125558 plone.distribution-1.0.0a6/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     6639 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/README.md
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/constraints.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.114061 plone.distribution-1.0.0a6/docs/
--rw-r--r--   0 ericof     (501) staff       (20)     7078 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/Makefile
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.114502 plone.distribution-1.0.0a6/docs/_static/
--rw-r--r--   0 ericof     (501) staff       (20)     5430 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/_static/favicon.ico
--rw-r--r--   0 ericof     (501) staff       (20)     3775 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/_static/logo.svg
--rw-r--r--   0 ericof     (501) staff       (20)       30 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/_static/print.css
--rw-r--r--   0 ericof     (501) staff       (20)     7814 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/_static/styles.css
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.114823 plone.distribution-1.0.0a6/docs/api/
--rw-r--r--   0 ericof     (501) staff       (20)      469 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/api/distribution.md
--rw-r--r--   0 ericof     (501) staff       (20)      709 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/api/index.md
--rw-r--r--   0 ericof     (501) staff       (20)      439 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/api/site.md
--rw-r--r--   0 ericof     (501) staff       (20)     2813 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/conf.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.114935 plone.distribution-1.0.0a6/docs/development/
--rw-r--r--   0 ericof     (501) staff       (20)       26 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/development/index.md
--rw-r--r--   0 ericof     (501) staff       (20)     1329 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/index.md
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.115262 plone.distribution-1.0.0a6/docs/usage/
--rw-r--r--   0 ericof     (501) staff       (20)     2560 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/usage/code-examples.md
--rw-r--r--   0 ericof     (501) staff       (20)     2010 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/usage/index.md
--rw-r--r--   0 ericof     (501) staff       (20)     4505 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/usage/package-structure.md
--rw-r--r--   0 ericof     (501) staff       (20)      172 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/instance.yaml
--rw-r--r--   0 ericof     (501) staff       (20)      577 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/mx.ini
--rw-r--r--   0 ericof     (501) staff       (20)     4112 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)      393 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/requirements-docs.txt
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/requirements.txt
--rw-r--r--   0 ericof     (501) staff       (20)       38 2023-06-23 23:11:01.125787 plone.distribution-1.0.0a6/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2155 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.109537 plone.distribution-1.0.0a6/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.115378 plone.distribution-1.0.0a6/src/plone/
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.117278 plone.distribution-1.0.0a6/src/plone/distribution/
--rw-r--r--   0 ericof     (501) staff       (20)      127 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.117601 plone.distribution-1.0.0a6/src/plone/distribution/api/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/api/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1912 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/api/distribution.py
--rw-r--r--   0 ericof     (501) staff       (20)     5231 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/api/site.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.118129 plone.distribution-1.0.0a6/src/plone/distribution/browser/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     2547 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/admin.py
--rw-r--r--   0 ericof     (501) staff       (20)      970 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1286 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/image.py
--rw-r--r--   0 ericof     (501) staff       (20)     1055 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/overrides.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.118862 plone.distribution-1.0.0a6/src/plone/distribution/browser/static/
--rw-r--r--   0 ericof     (501) staff       (20)     1185 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-logo.png
--rw-r--r--   0 ericof     (501) staff       (20)      712 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-overview.min.css
--rw-r--r--   0 ericof     (501) staff       (20)   521416 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-overview.min.js
--rw-r--r--   0 ericof     (501) staff       (20)      812 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone.svg
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.118980 plone.distribution-1.0.0a6/src/plone/distribution/browser/templates/
--rw-r--r--   0 ericof     (501) staff       (20)     1431 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/templates/plone-overview.pt
--rw-r--r--   0 ericof     (501) staff       (20)      446 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     3618 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/core.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.110287 plone.distribution-1.0.0a6/src/plone/distribution/distributions/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.119484 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.120078 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/
--rw-r--r--   0 ericof     (501) staff       (20)     9565 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/content.json
--rw-r--r--   0 ericof     (501) staff       (20)      336 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/defaultpages.json
--rw-r--r--   0 ericof     (501) staff       (20)      257 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/ordering.json
--rw-r--r--   0 ericof     (501) staff       (20)     5160 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/portal.json
--rw-r--r--   0 ericof     (501) staff       (20)      613 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/portlets.json
--rw-r--r--   0 ericof     (501) staff       (20)   293282 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/image.png
--rw-r--r--   0 ericof     (501) staff       (20)      148 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/profiles.json
--rw-r--r--   0 ericof     (501) staff       (20)     1280 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/schema.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.120540 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.120661 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/content/
--rw-r--r--   0 ericof     (501) staff       (20)    25846 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/content/portal.json
--rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/image.png
--rw-r--r--   0 ericof     (501) staff       (20)      175 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/profiles.json
--rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/schema.json
--rw-r--r--   0 ericof     (501) staff       (20)      491 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.121443 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1266 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4259 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/dist_export.py
--rw-r--r--   0 ericof     (501) staff       (20)     3054 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/dist_import.py
--rw-r--r--   0 ericof     (501) staff       (20)     2486 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/helpers.py
--rw-r--r--   0 ericof     (501) staff       (20)      241 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/interfaces.py
--rw-r--r--   0 ericof     (501) staff       (20)     2735 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/serializer.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.121679 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/templates/
--rw-r--r--   0 ericof     (501) staff       (20)     2290 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/templates/export_all.pt
--rw-r--r--   0 ericof     (501) staff       (20)     1371 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/templates/import_all.pt
--rw-r--r--   0 ericof     (501) staff       (20)     1334 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/handler.py
--rw-r--r--   0 ericof     (501) staff       (20)      698 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/interfaces.py
--rw-r--r--   0 ericof     (501) staff       (20)      391 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/meta.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     2950 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/metaconfigure.py
--rw-r--r--   0 ericof     (501) staff       (20)     4174 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/registry.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.121881 plone.distribution-1.0.0a6/src/plone/distribution/services/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.122201 plone.distribution-1.0.0a6/src/plone/distribution/services/auth/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/auth/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      348 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/auth/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1301 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/auth/login.py
--rw-r--r--   0 ericof     (501) staff       (20)      334 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.122675 plone.distribution-1.0.0a6/src/plone/distribution/services/sites/
--rw-r--r--   0 ericof     (501) staff       (20)       77 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/sites/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1784 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/sites/add.py
--rw-r--r--   0 ericof     (501) staff       (20)      895 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/sites/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4340 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/sites/get.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.123043 plone.distribution-1.0.0a6/src/plone/distribution/testing/
--rw-r--r--   0 ericof     (501) staff       (20)      149 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/testing/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     3123 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/testing/layer.py
--rw-r--r--   0 ericof     (501) staff       (20)     1017 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/testing/testing.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.123434 plone.distribution-1.0.0a6/src/plone/distribution/utils/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/utils/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      914 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/utils/request.py
--rw-r--r--   0 ericof     (501) staff       (20)     4402 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/utils/schema.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.116285 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)     9765 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     4348 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)       40 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/namespace_packages.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/not-zip-safe
--rw-r--r--   0 ericof     (501) staff       (20)      208 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/top_level.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.123637 plone.distribution-1.0.0a6/tests/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.123873 plone.distribution-1.0.0a6/tests/api/
--rw-r--r--   0 ericof     (501) staff       (20)     1524 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/api/test_api_distribution.py
--rw-r--r--   0 ericof     (501) staff       (20)     2166 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/api/test_api_site.py
--rw-r--r--   0 ericof     (501) staff       (20)      363 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/conftest.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.124315 plone.distribution-1.0.0a6/tests/distributions/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/distributions/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      322 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/distributions/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)     1895 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/distributions/test_distributions_classic.py
--rw-r--r--   0 ericof     (501) staff       (20)     1765 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/distributions/test_distributions_default.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.124537 plone.distribution-1.0.0a6/tests/exportimport/
--rw-r--r--   0 ericof     (501) staff       (20)    12736 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/exportimport/portal.json
--rw-r--r--   0 ericof     (501) staff       (20)     3279 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/exportimport/test_exportimport_helpers.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.124846 plone.distribution-1.0.0a6/tests/services/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/services/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      243 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/services/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)     3170 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/services/test_services_site.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.125149 plone.distribution-1.0.0a6/tests/utils/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/utils/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.125370 plone.distribution-1.0.0a6/tests/utils/data/
--rw-r--r--   0 ericof     (501) staff       (20)      969 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/utils/data/invalid.json
--rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/utils/data/valid.json
--rw-r--r--   0 ericof     (501) staff       (20)     1205 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/utils/test_utils_request.py
--rw-r--r--   0 ericof     (501) staff       (20)     2519 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/utils/test_utils_schema.py
--rw-r--r--   0 ericof     (501) staff       (20)     3740 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tox.ini
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.241056 plone.distribution-1.0.0a7/
+-rw-r--r--   0 ericof     (501) staff       (20)     1342 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)      540 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/.flake8
+-rw-r--r--   0 ericof     (501) staff       (20)      663 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/.gitignore
+-rw-r--r--   0 ericof     (501) staff       (20)      557 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/.meta.toml
+-rw-r--r--   0 ericof     (501) staff       (20)     1740 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/.pre-commit-config.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)     2006 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/CHANGES.md
+-rw-r--r--   0 ericof     (501) staff       (20)       95 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/CONTRIBUTING.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/LICENSE
+-rw-r--r--   0 ericof     (501) staff       (20)      269 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     5109 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/Makefile
+-rw-r--r--   0 ericof     (501) staff       (20)     9852 2023-06-24 19:48:29.240886 plone.distribution-1.0.0a7/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     6639 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/constraints.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.229493 plone.distribution-1.0.0a7/docs/
+-rw-r--r--   0 ericof     (501) staff       (20)     7078 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/Makefile
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.229915 plone.distribution-1.0.0a7/docs/_static/
+-rw-r--r--   0 ericof     (501) staff       (20)     5430 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/_static/favicon.ico
+-rw-r--r--   0 ericof     (501) staff       (20)     3775 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/_static/logo.svg
+-rw-r--r--   0 ericof     (501) staff       (20)       30 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/_static/print.css
+-rw-r--r--   0 ericof     (501) staff       (20)     7814 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/_static/styles.css
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.230236 plone.distribution-1.0.0a7/docs/api/
+-rw-r--r--   0 ericof     (501) staff       (20)      469 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/api/distribution.md
+-rw-r--r--   0 ericof     (501) staff       (20)      709 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/api/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)      439 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/api/site.md
+-rw-r--r--   0 ericof     (501) staff       (20)     2813 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/conf.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.230358 plone.distribution-1.0.0a7/docs/development/
+-rw-r--r--   0 ericof     (501) staff       (20)       26 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/development/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)     1329 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/index.md
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.230682 plone.distribution-1.0.0a7/docs/usage/
+-rw-r--r--   0 ericof     (501) staff       (20)     2560 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/usage/code-examples.md
+-rw-r--r--   0 ericof     (501) staff       (20)     2010 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/usage/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)     4505 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/docs/usage/package-structure.md
+-rw-r--r--   0 ericof     (501) staff       (20)      172 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/instance.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)      577 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/mx.ini
+-rw-r--r--   0 ericof     (501) staff       (20)     4112 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)      393 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/requirements-docs.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2023-06-24 19:48:29.241090 plone.distribution-1.0.0a7/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2155 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.225493 plone.distribution-1.0.0a7/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.230794 plone.distribution-1.0.0a7/src/plone/
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.232641 plone.distribution-1.0.0a7/src/plone/distribution/
+-rw-r--r--   0 ericof     (501) staff       (20)      127 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.232947 plone.distribution-1.0.0a7/src/plone/distribution/api/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/api/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1912 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/api/distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5231 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/api/site.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.233471 plone.distribution-1.0.0a7/src/plone/distribution/browser/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/browser/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2547 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/browser/admin.py
+-rw-r--r--   0 ericof     (501) staff       (20)      970 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/browser/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1286 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/browser/image.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1055 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/browser/overrides.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.234194 plone.distribution-1.0.0a7/src/plone/distribution/browser/static/
+-rw-r--r--   0 ericof     (501) staff       (20)     1185 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/browser/static/plone-logo.png
+-rw-r--r--   0 ericof     (501) staff       (20)      712 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/browser/static/plone-overview.min.css
+-rw-r--r--   0 ericof     (501) staff       (20)   521416 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/browser/static/plone-overview.min.js
+-rw-r--r--   0 ericof     (501) staff       (20)      812 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/browser/static/plone.svg
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.234311 plone.distribution-1.0.0a7/src/plone/distribution/browser/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)     1431 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/browser/templates/plone-overview.pt
+-rw-r--r--   0 ericof     (501) staff       (20)      446 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     3618 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/core.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.226080 plone.distribution-1.0.0a7/src/plone/distribution/distributions/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.234802 plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.235362 plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/content/
+-rw-r--r--   0 ericof     (501) staff       (20)     9565 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/content/content.json
+-rw-r--r--   0 ericof     (501) staff       (20)      336 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/content/defaultpages.json
+-rw-r--r--   0 ericof     (501) staff       (20)      257 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/content/ordering.json
+-rw-r--r--   0 ericof     (501) staff       (20)     5160 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/content/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)      613 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/content/portlets.json
+-rw-r--r--   0 ericof     (501) staff       (20)   293282 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      148 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1280 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/schema.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.235970 plone.distribution-1.0.0a7/src/plone/distribution/distributions/default/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.236077 plone.distribution-1.0.0a7/src/plone/distribution/distributions/default/content/
+-rw-r--r--   0 ericof     (501) staff       (20)    25846 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/default/content/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/default/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      175 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/default/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions/default/schema.json
+-rw-r--r--   0 ericof     (501) staff       (20)      491 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/distributions.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.236839 plone.distribution-1.0.0a7/src/plone/distribution/exportimport/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/exportimport/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1266 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/exportimport/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4276 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/exportimport/dist_export.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3054 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/exportimport/dist_import.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2486 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/exportimport/helpers.py
+-rw-r--r--   0 ericof     (501) staff       (20)      241 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/exportimport/interfaces.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2735 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/exportimport/serializer.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.237062 plone.distribution-1.0.0a7/src/plone/distribution/exportimport/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)     2290 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/exportimport/templates/export_all.pt
+-rw-r--r--   0 ericof     (501) staff       (20)     1371 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/exportimport/templates/import_all.pt
+-rw-r--r--   0 ericof     (501) staff       (20)     1334 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/handler.py
+-rw-r--r--   0 ericof     (501) staff       (20)      698 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/interfaces.py
+-rw-r--r--   0 ericof     (501) staff       (20)      391 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/meta.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     2950 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/metaconfigure.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4174 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/registry.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.237253 plone.distribution-1.0.0a7/src/plone/distribution/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/services/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.237557 plone.distribution-1.0.0a7/src/plone/distribution/services/auth/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/services/auth/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      348 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/services/auth/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1301 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/services/auth/login.py
+-rw-r--r--   0 ericof     (501) staff       (20)      334 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/services/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.237990 plone.distribution-1.0.0a7/src/plone/distribution/services/sites/
+-rw-r--r--   0 ericof     (501) staff       (20)       77 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/services/sites/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1784 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/services/sites/add.py
+-rw-r--r--   0 ericof     (501) staff       (20)      895 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/services/sites/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4340 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/services/sites/get.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.238310 plone.distribution-1.0.0a7/src/plone/distribution/testing/
+-rw-r--r--   0 ericof     (501) staff       (20)      149 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/testing/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3123 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/testing/layer.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1017 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/testing/testing.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.238621 plone.distribution-1.0.0a7/src/plone/distribution/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/utils/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      914 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/utils/request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4402 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/src/plone/distribution/utils/schema.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.231668 plone.distribution-1.0.0a7/src/plone.distribution.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)     9852 2023-06-24 19:48:29.000000 plone.distribution-1.0.0a7/src/plone.distribution.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     4348 2023-06-24 19:48:29.000000 plone.distribution-1.0.0a7/src/plone.distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-24 19:48:29.000000 plone.distribution-1.0.0a7/src/plone.distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       40 2023-06-24 19:48:29.000000 plone.distribution-1.0.0a7/src/plone.distribution.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-06-24 19:48:29.000000 plone.distribution-1.0.0a7/src/plone.distribution.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-24 19:48:29.000000 plone.distribution-1.0.0a7/src/plone.distribution.egg-info/not-zip-safe
+-rw-r--r--   0 ericof     (501) staff       (20)      208 2023-06-24 19:48:29.000000 plone.distribution-1.0.0a7/src/plone.distribution.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-06-24 19:48:29.000000 plone.distribution-1.0.0a7/src/plone.distribution.egg-info/top_level.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.238820 plone.distribution-1.0.0a7/tests/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.239041 plone.distribution-1.0.0a7/tests/api/
+-rw-r--r--   0 ericof     (501) staff       (20)     1524 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/api/test_api_distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2166 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/api/test_api_site.py
+-rw-r--r--   0 ericof     (501) staff       (20)      363 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.239498 plone.distribution-1.0.0a7/tests/distributions/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/distributions/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      322 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/distributions/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1895 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/distributions/test_distributions_classic.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1765 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/distributions/test_distributions_default.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.239751 plone.distribution-1.0.0a7/tests/exportimport/
+-rw-r--r--   0 ericof     (501) staff       (20)    12736 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/exportimport/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)     3279 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/exportimport/test_exportimport_helpers.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.240075 plone.distribution-1.0.0a7/tests/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/services/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      243 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/services/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3170 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/services/test_services_site.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.240445 plone.distribution-1.0.0a7/tests/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/utils/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-24 19:48:29.240665 plone.distribution-1.0.0a7/tests/utils/data/
+-rw-r--r--   0 ericof     (501) staff       (20)      969 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/utils/data/invalid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/utils/data/valid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1205 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/utils/test_utils_request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2519 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tests/utils/test_utils_schema.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3740 2023-06-24 19:48:28.000000 plone.distribution-1.0.0a7/tox.ini
```

### Comparing `plone.distribution-1.0.0a6/.editorconfig` & `plone.distribution-1.0.0a7/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/.flake8` & `plone.distribution-1.0.0a7/.flake8`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/.gitignore` & `plone.distribution-1.0.0a7/.gitignore`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/.meta.toml` & `plone.distribution-1.0.0a7/.meta.toml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/.pre-commit-config.yaml` & `plone.distribution-1.0.0a7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/CHANGES.md` & `plone.distribution-1.0.0a7/CHANGES.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a7 (2023-06-24)
+
+
+### Bug fixes:
+
+- Fix content export to json [@ericof] #33
+
+
 ## 1.0.0a6 (2023-06-23)
 
 
 ### New features:
 
 - Improve support for testing distributions [@ericof] #24
 - Allow export only for distributions still in development [@ericof] #28
```

### Comparing `plone.distribution-1.0.0a6/LICENSE` & `plone.distribution-1.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/Makefile` & `plone.distribution-1.0.0a7/Makefile`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/PKG-INFO` & `plone.distribution-1.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -272,14 +272,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a7 (2023-06-24)
+
+
+### Bug fixes:
+
+- Fix content export to json [@ericof] #33
+
+
 ## 1.0.0a6 (2023-06-23)
 
 
 ### New features:
 
 - Improve support for testing distributions [@ericof] #24
 - Allow export only for distributions still in development [@ericof] #28
```

### Comparing `plone.distribution-1.0.0a6/README.md` & `plone.distribution-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/docs/Makefile` & `plone.distribution-1.0.0a7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/docs/_static/favicon.ico` & `plone.distribution-1.0.0a7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/docs/_static/logo.svg` & `plone.distribution-1.0.0a7/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/docs/_static/styles.css` & `plone.distribution-1.0.0a7/docs/_static/styles.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/docs/api/index.md` & `plone.distribution-1.0.0a7/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/docs/conf.py` & `plone.distribution-1.0.0a7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/docs/index.md` & `plone.distribution-1.0.0a7/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/docs/usage/code-examples.md` & `plone.distribution-1.0.0a7/docs/usage/code-examples.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/docs/usage/index.md` & `plone.distribution-1.0.0a7/docs/usage/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/docs/usage/package-structure.md` & `plone.distribution-1.0.0a7/docs/usage/package-structure.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/mx.ini` & `plone.distribution-1.0.0a7/mx.ini`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/pyproject.toml` & `plone.distribution-1.0.0a7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/setup.py` & `plone.distribution-1.0.0a7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
     name="plone.distribution",
-    version="1.0.0a6",
+    version="1.0.0a7",
     description="Plone distribution support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/api/distribution.py` & `plone.distribution-1.0.0a7/src/plone/distribution/api/distribution.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/api/site.py` & `plone.distribution-1.0.0a7/src/plone/distribution/api/site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/browser/admin.py` & `plone.distribution-1.0.0a7/src/plone/distribution/browser/admin.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/browser/configure.zcml` & `plone.distribution-1.0.0a7/src/plone/distribution/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/browser/image.py` & `plone.distribution-1.0.0a7/src/plone/distribution/browser/image.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/browser/overrides.zcml` & `plone.distribution-1.0.0a7/src/plone/distribution/browser/overrides.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-logo.png` & `plone.distribution-1.0.0a7/src/plone/distribution/browser/static/plone-logo.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-overview.min.css` & `plone.distribution-1.0.0a7/src/plone/distribution/browser/static/plone-overview.min.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-overview.min.js` & `plone.distribution-1.0.0a7/src/plone/distribution/browser/static/plone-overview.min.js`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone.svg` & `plone.distribution-1.0.0a7/src/plone/distribution/browser/static/plone.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/browser/templates/plone-overview.pt` & `plone.distribution-1.0.0a7/src/plone/distribution/browser/templates/plone-overview.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/core.py` & `plone.distribution-1.0.0a7/src/plone/distribution/core.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/content.json` & `plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/content/content.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/portal.json` & `plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/content/portal.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/portlets.json` & `plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/content/portlets.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/image.png` & `plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/schema.json` & `plone.distribution-1.0.0a7/src/plone/distribution/distributions/classic/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/content/portal.json` & `plone.distribution-1.0.0a7/src/plone/distribution/distributions/default/content/portal.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/image.png` & `plone.distribution-1.0.0a7/src/plone/distribution/distributions/default/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/schema.json` & `plone.distribution-1.0.0a7/src/plone/distribution/distributions/default/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/exportimport/configure.zcml` & `plone.distribution-1.0.0a7/src/plone/distribution/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/exportimport/dist_export.py` & `plone.distribution-1.0.0a7/src/plone/distribution/exportimport/dist_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             download_to_server,
             migration,
             include_revisions,
         )
 
     def global_dict_hook(self, item, obj):
         """Clean up data before export."""
-        item = remove_site_root(item)
+        item = remove_site_root(item, self.PORTAL_URL)
         if item["@type"] == "Plone Site":
             # To avoid a conflict between @id and id
             item["@id"] = f"/{item['id']}"
         if "blocks" in item:
             blocks = item["blocks"]
             item["blocks"] = parse_blocks(blocks)
         return item
```

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/exportimport/dist_import.py` & `plone.distribution-1.0.0a7/src/plone/distribution/exportimport/dist_import.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/exportimport/helpers.py` & `plone.distribution-1.0.0a7/src/plone/distribution/exportimport/helpers.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/exportimport/serializer.py` & `plone.distribution-1.0.0a7/src/plone/distribution/exportimport/serializer.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/exportimport/templates/export_all.pt` & `plone.distribution-1.0.0a7/src/plone/distribution/exportimport/templates/export_all.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/exportimport/templates/import_all.pt` & `plone.distribution-1.0.0a7/src/plone/distribution/exportimport/templates/import_all.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/handler.py` & `plone.distribution-1.0.0a7/src/plone/distribution/handler.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/interfaces.py` & `plone.distribution-1.0.0a7/src/plone/distribution/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/metaconfigure.py` & `plone.distribution-1.0.0a7/src/plone/distribution/metaconfigure.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/registry.py` & `plone.distribution-1.0.0a7/src/plone/distribution/registry.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/services/auth/login.py` & `plone.distribution-1.0.0a7/src/plone/distribution/services/auth/login.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/services/sites/add.py` & `plone.distribution-1.0.0a7/src/plone/distribution/services/sites/add.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/services/sites/configure.zcml` & `plone.distribution-1.0.0a7/src/plone/distribution/services/sites/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/services/sites/get.py` & `plone.distribution-1.0.0a7/src/plone/distribution/services/sites/get.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/testing/layer.py` & `plone.distribution-1.0.0a7/src/plone/distribution/testing/layer.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/testing/testing.py` & `plone.distribution-1.0.0a7/src/plone/distribution/testing/testing.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/utils/request.py` & `plone.distribution-1.0.0a7/src/plone/distribution/utils/request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone/distribution/utils/schema.py` & `plone.distribution-1.0.0a7/src/plone/distribution/utils/schema.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/src/plone.distribution.egg-info/PKG-INFO` & `plone.distribution-1.0.0a7/src/plone.distribution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -272,14 +272,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a7 (2023-06-24)
+
+
+### Bug fixes:
+
+- Fix content export to json [@ericof] #33
+
+
 ## 1.0.0a6 (2023-06-23)
 
 
 ### New features:
 
 - Improve support for testing distributions [@ericof] #24
 - Allow export only for distributions still in development [@ericof] #28
```

### Comparing `plone.distribution-1.0.0a6/src/plone.distribution.egg-info/SOURCES.txt` & `plone.distribution-1.0.0a7/src/plone.distribution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tests/api/test_api_distribution.py` & `plone.distribution-1.0.0a7/tests/api/test_api_distribution.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tests/api/test_api_site.py` & `plone.distribution-1.0.0a7/tests/api/test_api_site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tests/distributions/test_distributions_classic.py` & `plone.distribution-1.0.0a7/tests/distributions/test_distributions_classic.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tests/distributions/test_distributions_default.py` & `plone.distribution-1.0.0a7/tests/distributions/test_distributions_default.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tests/exportimport/portal.json` & `plone.distribution-1.0.0a7/tests/exportimport/portal.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tests/exportimport/test_exportimport_helpers.py` & `plone.distribution-1.0.0a7/tests/exportimport/test_exportimport_helpers.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tests/services/test_services_site.py` & `plone.distribution-1.0.0a7/tests/services/test_services_site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tests/utils/data/invalid.json` & `plone.distribution-1.0.0a7/tests/utils/data/invalid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tests/utils/data/valid.json` & `plone.distribution-1.0.0a7/tests/utils/data/valid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tests/utils/test_utils_request.py` & `plone.distribution-1.0.0a7/tests/utils/test_utils_request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tests/utils/test_utils_schema.py` & `plone.distribution-1.0.0a7/tests/utils/test_utils_schema.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a6/tox.ini` & `plone.distribution-1.0.0a7/tox.ini`

 * *Files identical despite different names*

