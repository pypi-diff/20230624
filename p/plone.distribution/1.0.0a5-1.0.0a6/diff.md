# Comparing `tmp/plone.distribution-1.0.0a5.tar.gz` & `tmp/plone.distribution-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.distribution-1.0.0a5.tar", last modified: Thu May 18 21:06:20 2023, max compression
+gzip compressed data, was "plone.distribution-1.0.0a6.tar", last modified: Fri Jun 23 23:11:01 2023, max compression
```

## Comparing `plone.distribution-1.0.0a5.tar` & `plone.distribution-1.0.0a6.tar`

### file list

```diff
@@ -1,137 +1,153 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.858627 plone.distribution-1.0.0a5/
--rw-r--r--   0 ericof     (501) staff       (20)      974 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/.editorconfig
--rw-r--r--   0 ericof     (501) staff       (20)      477 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/.gitignore
--rw-r--r--   0 ericof     (501) staff       (20)     1393 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/CHANGES.md
--rw-r--r--   0 ericof     (501) staff       (20)       95 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/CONTRIBUTING.md
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/LICENSE
--rw-r--r--   0 ericof     (501) staff       (20)      269 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)     5797 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/Makefile
--rw-r--r--   0 ericof     (501) staff       (20)     9239 2023-05-18 21:06:20.858460 plone.distribution-1.0.0a5/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     6639 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/README.md
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/constraints.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.847728 plone.distribution-1.0.0a5/docs/
--rw-r--r--   0 ericof     (501) staff       (20)     7078 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/Makefile
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.848173 plone.distribution-1.0.0a5/docs/_static/
--rw-r--r--   0 ericof     (501) staff       (20)     5430 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/_static/favicon.ico
--rw-r--r--   0 ericof     (501) staff       (20)     3775 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/_static/logo.svg
--rw-r--r--   0 ericof     (501) staff       (20)       30 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/_static/print.css
--rw-r--r--   0 ericof     (501) staff       (20)     7814 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/_static/styles.css
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.848517 plone.distribution-1.0.0a5/docs/api/
--rw-r--r--   0 ericof     (501) staff       (20)      469 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/api/distribution.md
--rw-r--r--   0 ericof     (501) staff       (20)      709 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/api/index.md
--rw-r--r--   0 ericof     (501) staff       (20)      439 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/api/site.md
--rw-r--r--   0 ericof     (501) staff       (20)      308 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/changelog_template.jinja
--rw-r--r--   0 ericof     (501) staff       (20)     2813 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/conf.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.848626 plone.distribution-1.0.0a5/docs/development/
--rw-r--r--   0 ericof     (501) staff       (20)       26 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/development/index.md
--rw-r--r--   0 ericof     (501) staff       (20)     1329 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/index.md
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.848956 plone.distribution-1.0.0a5/docs/usage/
--rw-r--r--   0 ericof     (501) staff       (20)     2255 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/usage/code-examples.md
--rw-r--r--   0 ericof     (501) staff       (20)     2010 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/usage/index.md
--rw-r--r--   0 ericof     (501) staff       (20)     4505 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/docs/usage/package-structure.md
--rw-r--r--   0 ericof     (501) staff       (20)      172 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/instance.yaml
--rw-r--r--   0 ericof     (501) staff       (20)      577 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/mx.ini
--rw-r--r--   0 ericof     (501) staff       (20)     1324 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)      393 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/requirements-docs.txt
--rw-r--r--   0 ericof     (501) staff       (20)       13 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/requirements.txt
--rw-r--r--   0 ericof     (501) staff       (20)       38 2023-05-18 21:06:20.858665 plone.distribution-1.0.0a5/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2155 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.844132 plone.distribution-1.0.0a5/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.849065 plone.distribution-1.0.0a5/src/plone/
--rw-r--r--   0 ericof     (501) staff       (20)       56 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.851101 plone.distribution-1.0.0a5/src/plone/distribution/
--rw-r--r--   0 ericof     (501) staff       (20)      127 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.851437 plone.distribution-1.0.0a5/src/plone/distribution/api/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/api/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1912 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/api/distribution.py
--rw-r--r--   0 ericof     (501) staff       (20)     4319 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/api/site.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.852005 plone.distribution-1.0.0a5/src/plone/distribution/browser/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     2547 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/admin.py
--rw-r--r--   0 ericof     (501) staff       (20)      970 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1286 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/image.py
--rw-r--r--   0 ericof     (501) staff       (20)     1055 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/overrides.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.852785 plone.distribution-1.0.0a5/src/plone/distribution/browser/static/
--rw-r--r--   0 ericof     (501) staff       (20)     1185 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-logo.png
--rw-r--r--   0 ericof     (501) staff       (20)      712 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-overview.min.css
--rw-r--r--   0 ericof     (501) staff       (20)   521416 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-overview.min.js
--rw-r--r--   0 ericof     (501) staff       (20)      812 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone.svg
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.852909 plone.distribution-1.0.0a5/src/plone/distribution/browser/templates/
--rw-r--r--   0 ericof     (501) staff       (20)     1306 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/browser/templates/plone-overview.pt
--rw-r--r--   0 ericof     (501) staff       (20)      446 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     3121 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/core.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.844739 plone.distribution-1.0.0a5/src/plone/distribution/distributions/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.853431 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.854212 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/
--rw-r--r--   0 ericof     (501) staff       (20)     9565 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/content.json
--rw-r--r--   0 ericof     (501) staff       (20)      336 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/defaultpages.json
--rw-r--r--   0 ericof     (501) staff       (20)      257 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/ordering.json
--rw-r--r--   0 ericof     (501) staff       (20)     5160 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/portal.json
--rw-r--r--   0 ericof     (501) staff       (20)      613 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/portlets.json
--rw-r--r--   0 ericof     (501) staff       (20)   293282 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/image.png
--rw-r--r--   0 ericof     (501) staff       (20)      148 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/profiles.json
--rw-r--r--   0 ericof     (501) staff       (20)     1280 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/schema.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.854732 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.854856 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/content/
--rw-r--r--   0 ericof     (501) staff       (20)    25845 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/content/portal.json
--rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/image.png
--rw-r--r--   0 ericof     (501) staff       (20)      175 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/profiles.json
--rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/schema.json
--rw-r--r--   0 ericof     (501) staff       (20)      491 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/distributions.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.855433 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      795 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4540 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/exportimport.py
--rw-r--r--   0 ericof     (501) staff       (20)      265 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/interfaces.py
--rw-r--r--   0 ericof     (501) staff       (20)     2735 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/serializer.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.855659 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/templates/
--rw-r--r--   0 ericof     (501) staff       (20)     1807 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/templates/export_all.pt
--rw-r--r--   0 ericof     (501) staff       (20)     1143 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/exportimport/templates/import_all.pt
--rw-r--r--   0 ericof     (501) staff       (20)     1161 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/handler.py
--rw-r--r--   0 ericof     (501) staff       (20)      698 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/interfaces.py
--rw-r--r--   0 ericof     (501) staff       (20)      373 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/meta.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4173 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/registry.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.855876 plone.distribution-1.0.0a5/src/plone/distribution/services/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.856196 plone.distribution-1.0.0a5/src/plone/distribution/services/auth/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/auth/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      348 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/auth/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     1301 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/auth/login.py
--rw-r--r--   0 ericof     (501) staff       (20)      334 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.856643 plone.distribution-1.0.0a5/src/plone/distribution/services/sites/
--rw-r--r--   0 ericof     (501) staff       (20)       77 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/sites/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1784 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/sites/add.py
--rw-r--r--   0 ericof     (501) staff       (20)      895 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/sites/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     4340 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/services/sites/get.py
--rw-r--r--   0 ericof     (501) staff       (20)      813 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/testing.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.856958 plone.distribution-1.0.0a5/src/plone/distribution/utils/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/utils/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      914 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/utils/request.py
--rw-r--r--   0 ericof     (501) staff       (20)     4396 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/utils/schema.py
--rw-r--r--   0 ericof     (501) staff       (20)     2950 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone/distribution/zcml.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.849987 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)     9239 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     3887 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)       40 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/namespace_packages.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/not-zip-safe
--rw-r--r--   0 ericof     (501) staff       (20)      208 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/src/plone.distribution.egg-info/top_level.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.857158 plone.distribution-1.0.0a5/tests/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.857379 plone.distribution-1.0.0a5/tests/api/
--rw-r--r--   0 ericof     (501) staff       (20)     1524 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/api/test_api_distribution.py
--rw-r--r--   0 ericof     (501) staff       (20)     1247 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/api/test_api_site.py
--rw-r--r--   0 ericof     (501) staff       (20)      363 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/conftest.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.857689 plone.distribution-1.0.0a5/tests/services/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/services/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      243 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/services/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)     3170 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/services/test_services_site.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.858000 plone.distribution-1.0.0a5/tests/utils/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/utils/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-05-18 21:06:20.858220 plone.distribution-1.0.0a5/tests/utils/data/
--rw-r--r--   0 ericof     (501) staff       (20)      969 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/utils/data/invalid.json
--rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/utils/data/valid.json
--rw-r--r--   0 ericof     (501) staff       (20)     1167 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/utils/test_utils_request.py
--rw-r--r--   0 ericof     (501) staff       (20)     2519 2023-05-18 21:06:20.000000 plone.distribution-1.0.0a5/tests/utils/test_utils_schema.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.125752 plone.distribution-1.0.0a6/
+-rw-r--r--   0 ericof     (501) staff       (20)     1342 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)      540 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/.flake8
+-rw-r--r--   0 ericof     (501) staff       (20)      663 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/.gitignore
+-rw-r--r--   0 ericof     (501) staff       (20)      557 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/.meta.toml
+-rw-r--r--   0 ericof     (501) staff       (20)     1740 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/.pre-commit-config.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)     1919 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/CHANGES.md
+-rw-r--r--   0 ericof     (501) staff       (20)       95 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/CONTRIBUTING.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/LICENSE
+-rw-r--r--   0 ericof     (501) staff       (20)      269 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     5109 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/Makefile
+-rw-r--r--   0 ericof     (501) staff       (20)     9765 2023-06-23 23:11:01.125558 plone.distribution-1.0.0a6/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     6639 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/constraints.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.114061 plone.distribution-1.0.0a6/docs/
+-rw-r--r--   0 ericof     (501) staff       (20)     7078 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/Makefile
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.114502 plone.distribution-1.0.0a6/docs/_static/
+-rw-r--r--   0 ericof     (501) staff       (20)     5430 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/_static/favicon.ico
+-rw-r--r--   0 ericof     (501) staff       (20)     3775 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/_static/logo.svg
+-rw-r--r--   0 ericof     (501) staff       (20)       30 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/_static/print.css
+-rw-r--r--   0 ericof     (501) staff       (20)     7814 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/_static/styles.css
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.114823 plone.distribution-1.0.0a6/docs/api/
+-rw-r--r--   0 ericof     (501) staff       (20)      469 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/api/distribution.md
+-rw-r--r--   0 ericof     (501) staff       (20)      709 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/api/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)      439 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/api/site.md
+-rw-r--r--   0 ericof     (501) staff       (20)     2813 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/conf.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.114935 plone.distribution-1.0.0a6/docs/development/
+-rw-r--r--   0 ericof     (501) staff       (20)       26 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/development/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)     1329 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/index.md
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.115262 plone.distribution-1.0.0a6/docs/usage/
+-rw-r--r--   0 ericof     (501) staff       (20)     2560 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/usage/code-examples.md
+-rw-r--r--   0 ericof     (501) staff       (20)     2010 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/usage/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)     4505 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/docs/usage/package-structure.md
+-rw-r--r--   0 ericof     (501) staff       (20)      172 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/instance.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)      577 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/mx.ini
+-rw-r--r--   0 ericof     (501) staff       (20)     4112 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)      393 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/requirements-docs.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       13 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2023-06-23 23:11:01.125787 plone.distribution-1.0.0a6/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2155 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.109537 plone.distribution-1.0.0a6/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.115378 plone.distribution-1.0.0a6/src/plone/
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.117278 plone.distribution-1.0.0a6/src/plone/distribution/
+-rw-r--r--   0 ericof     (501) staff       (20)      127 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.117601 plone.distribution-1.0.0a6/src/plone/distribution/api/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/api/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1912 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/api/distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5231 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/api/site.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.118129 plone.distribution-1.0.0a6/src/plone/distribution/browser/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2547 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/admin.py
+-rw-r--r--   0 ericof     (501) staff       (20)      970 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1286 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/image.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1055 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/overrides.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.118862 plone.distribution-1.0.0a6/src/plone/distribution/browser/static/
+-rw-r--r--   0 ericof     (501) staff       (20)     1185 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-logo.png
+-rw-r--r--   0 ericof     (501) staff       (20)      712 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-overview.min.css
+-rw-r--r--   0 ericof     (501) staff       (20)   521416 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-overview.min.js
+-rw-r--r--   0 ericof     (501) staff       (20)      812 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone.svg
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.118980 plone.distribution-1.0.0a6/src/plone/distribution/browser/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)     1431 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/browser/templates/plone-overview.pt
+-rw-r--r--   0 ericof     (501) staff       (20)      446 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     3618 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/core.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.110287 plone.distribution-1.0.0a6/src/plone/distribution/distributions/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.119484 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.120078 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/
+-rw-r--r--   0 ericof     (501) staff       (20)     9565 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/content.json
+-rw-r--r--   0 ericof     (501) staff       (20)      336 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/defaultpages.json
+-rw-r--r--   0 ericof     (501) staff       (20)      257 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/ordering.json
+-rw-r--r--   0 ericof     (501) staff       (20)     5160 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)      613 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/portlets.json
+-rw-r--r--   0 ericof     (501) staff       (20)   293282 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      148 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1280 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/schema.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.120540 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.120661 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/content/
+-rw-r--r--   0 ericof     (501) staff       (20)    25846 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/content/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)   218233 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/image.png
+-rw-r--r--   0 ericof     (501) staff       (20)      175 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/profiles.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/schema.json
+-rw-r--r--   0 ericof     (501) staff       (20)      491 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/distributions.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.121443 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1266 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4259 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/dist_export.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3054 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/dist_import.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2486 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/helpers.py
+-rw-r--r--   0 ericof     (501) staff       (20)      241 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/interfaces.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2735 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/serializer.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.121679 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/templates/
+-rw-r--r--   0 ericof     (501) staff       (20)     2290 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/templates/export_all.pt
+-rw-r--r--   0 ericof     (501) staff       (20)     1371 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/exportimport/templates/import_all.pt
+-rw-r--r--   0 ericof     (501) staff       (20)     1334 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/handler.py
+-rw-r--r--   0 ericof     (501) staff       (20)      698 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/interfaces.py
+-rw-r--r--   0 ericof     (501) staff       (20)      391 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/meta.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     2950 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/metaconfigure.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4174 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/registry.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.121881 plone.distribution-1.0.0a6/src/plone/distribution/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.122201 plone.distribution-1.0.0a6/src/plone/distribution/services/auth/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/auth/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      348 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/auth/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     1301 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/auth/login.py
+-rw-r--r--   0 ericof     (501) staff       (20)      334 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.122675 plone.distribution-1.0.0a6/src/plone/distribution/services/sites/
+-rw-r--r--   0 ericof     (501) staff       (20)       77 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/sites/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1784 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/sites/add.py
+-rw-r--r--   0 ericof     (501) staff       (20)      895 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/sites/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     4340 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/services/sites/get.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.123043 plone.distribution-1.0.0a6/src/plone/distribution/testing/
+-rw-r--r--   0 ericof     (501) staff       (20)      149 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/testing/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3123 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/testing/layer.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1017 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/testing/testing.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.123434 plone.distribution-1.0.0a6/src/plone/distribution/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/utils/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      914 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/utils/request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4402 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/src/plone/distribution/utils/schema.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.116285 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)     9765 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     4348 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       40 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/not-zip-safe
+-rw-r--r--   0 ericof     (501) staff       (20)      208 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2023-06-23 23:11:01.000000 plone.distribution-1.0.0a6/src/plone.distribution.egg-info/top_level.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.123637 plone.distribution-1.0.0a6/tests/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.123873 plone.distribution-1.0.0a6/tests/api/
+-rw-r--r--   0 ericof     (501) staff       (20)     1524 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/api/test_api_distribution.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2166 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/api/test_api_site.py
+-rw-r--r--   0 ericof     (501) staff       (20)      363 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.124315 plone.distribution-1.0.0a6/tests/distributions/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/distributions/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      322 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/distributions/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1895 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/distributions/test_distributions_classic.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1765 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/distributions/test_distributions_default.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.124537 plone.distribution-1.0.0a6/tests/exportimport/
+-rw-r--r--   0 ericof     (501) staff       (20)    12736 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/exportimport/portal.json
+-rw-r--r--   0 ericof     (501) staff       (20)     3279 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/exportimport/test_exportimport_helpers.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.124846 plone.distribution-1.0.0a6/tests/services/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/services/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      243 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/services/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3170 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/services/test_services_site.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.125149 plone.distribution-1.0.0a6/tests/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/utils/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2023-06-23 23:11:01.125370 plone.distribution-1.0.0a6/tests/utils/data/
+-rw-r--r--   0 ericof     (501) staff       (20)      969 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/utils/data/invalid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1267 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/utils/data/valid.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1205 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/utils/test_utils_request.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2519 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tests/utils/test_utils_schema.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3740 2023-06-23 23:11:00.000000 plone.distribution-1.0.0a6/tox.ini
```

### Comparing `plone.distribution-1.0.0a5/.editorconfig` & `plone.distribution-1.0.0a6/.editorconfig`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-# EditorConfig Configurtaion file, for more details see:
-# https://EditorConfig.org
+# Generated from:
+# https://github.com/plone/meta/tree/master/config/default
+# See the inline comments on how to expand/tweak this configuration file
+#
+# EditorConfig Configuration file, for more details see:
+# http://EditorConfig.org
 # EditorConfig is a convention description, that could be interpreted
 # by multiple editors to enforce common coding conventions for specific
 # file types
 
 # top-most EditorConfig file:
 # Will ignore other EditorConfig files in Home directory or upper tree level.
 root = true
 
+
 [*]  # For All Files
 # Unix-style newlines with a newline ending every file
 end_of_line = lf
 insert_final_newline = true
 trim_trailing_whitespace = true
 # Set default charset
 charset = utf-8
@@ -20,16 +25,29 @@
 # Max Line Length - a hard line wrap, should be disabled
 max_line_length = off
 
 [*.{py,cfg,ini}]
 # 4 space indentation
 indent_size = 4
 
-[*.{html,dtml,pt,zpt,xml,zcml,js,json,less,css,yml,yaml,ts}]
+[*.{yml,zpt,pt,dtml,zcml}]
+# 2 space indentation
+indent_size = 2
+
+[*.{json,jsonl,js,jsx,ts,tsx,css,less,scss,html}]  # Frontend development
 # 2 space indentation
 indent_size = 2
 
 [{Makefile,.gitmodules}]
 # Tab indentation (no size specified, but view as 4 spaces)
 indent_style = tab
 indent_size = unset
 tab_width = unset
+
+
+##
+# Add extra configuration options in .meta.toml:
+#  [editorconfig]
+#  extra_lines = """
+#  _your own configuration lines_
+#  """
+##
```

### Comparing `plone.distribution-1.0.0a5/CHANGES.md` & `plone.distribution-1.0.0a6/CHANGES.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,36 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a6 (2023-06-23)
+
+
+### New features:
+
+- Improve support for testing distributions [@ericof] #24
+- Allow export only for distributions still in development [@ericof] #28
+- Create a report for Plone sites created from a distribution [@ericof] #30
+- Clean up exported content to remove references to portal.absolute_url() [@ericof] #32
+
+
+### Bug fixes:
+
+- Content language should be allowed in portal configuration [@ericof] #23
+
+
+### Internal:
+
+- Update configuration files.
+  [plone devs] 047ec50d, 55bda5c9, d7e9e748
+
+
 ## 1.0.0a5 (2023-05-18)
 
 
 ### Bug fixes:
 
 - Import did not import any steps except content and portal. [pbauer] #22
```

### Comparing `plone.distribution-1.0.0a5/LICENSE` & `plone.distribution-1.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/Makefile` & `plone.distribution-1.0.0a6/Makefile`

 * *Files 26% similar despite different names*

```diff
@@ -29,22 +29,16 @@
 # version ok?
 PYTHON_VERSION_MIN=3.8
 PYTHON_VERSION_OK=$(shell $(PYTHON) -c "import sys; print((int(sys.version_info[0]), int(sys.version_info[1])) >= tuple(map(int, '$(PYTHON_VERSION_MIN)'.split('.'))))")
 ifeq ($(PYTHON_VERSION_OK),0)
   $(error "Need python $(PYTHON_VERSION) >= $(PYTHON_VERSION_MIN)")
 endif
 
-CODE_QUALITY_VERSION=2
-ifndef LOG_LEVEL
-	LOG_LEVEL=INFO
-endif
-CURRENT_USER=$$(whoami)
-USER_INFO=$$(id -u ${CURRENT_USER}):$$(getent group ${CURRENT_USER}|cut -d: -f3)
-LINT=docker run --rm -e LOG_LEVEL="${LOG_LEVEL}" -v "${BACKEND_FOLDER}":/github/workspace plone/code-quality:${CODE_QUALITY_VERSION} check
-FORMAT=docker run --rm --user="${USER_INFO}" -e LOG_LEVEL="${LOG_LEVEL}" -v "${BACKEND_FOLDER}":/github/workspace plone/code-quality:${CODE_QUALITY_VERSION} format
+# Set distributions still in development
+DISTRIBUTIONS="default,classic"
 
 all: build
 
 # Add the following 'help' target to your Makefile
 # And add help text after each target name starting with '\#\#'
 .PHONY: help
 help: ## This help message
@@ -59,15 +53,15 @@
 
 .PHONY: clean-instance
 clean-instance: ## remove existing instance
 	rm -fr instance etc inituser var
 
 .PHONY: clean-venv
 clean-venv: ## remove virtual environment
-	rm -fr bin include lib lib64
+	rm -fr bin include lib lib64 env pyvenv.cfg .tox .pytest_cache requirements-mxdev.txt
 
 .PHONY: clean-build
 clean-build: ## remove build artifacts
 	rm -fr build/
 	rm -fr dist/
 	rm -fr .eggs/
 	find . -name '*.egg-info' -exec rm -fr {} +
@@ -81,18 +75,19 @@
 	find . -name '__pycache__' -exec rm -fr {} +
 
 .PHONY: clean-test
 clean-test: ## remove test and coverage artifacts
 	rm -f .coverage
 	rm -fr htmlcov/
 
-bin/pip:
+bin/pip bin/tox bin/mxdev:
 	@echo "$(GREEN)==> Setup Virtual Env$(RESET)"
 	$(PYTHON) -m venv .
-	bin/pip install -U "pip" "wheel" "cookiecutter" "mxdev"
+	bin/pip install -U "pip" "wheel" "cookiecutter" "mxdev" "tox" "pre-commit"
+	bin/pre-commit install
 
 .PHONY: config
 config: bin/pip  ## Create instance configuration
 	@echo "$(GREEN)==> Create instance configuration$(RESET)"
 	bin/cookiecutter -f --no-input --config-file instance.yaml gh:plone/cookiecutter-zope-instance
 
 .PHONY: install-plone-6.0
@@ -112,82 +107,59 @@
 
 .PHONY: build-frontend
 build-frontend:
 	@echo "$(GREEN)==> Build the frontend code$(RESET)"
 	(cd frontend && pnpm build)
 	(mv frontend/dist/* src/plone/distribution/browser/static/)
 
-.PHONY: clean
-clean: ## Remove old virtualenv and creates a new one
-	@echo "$(RED)==> Cleaning environment and build$(RESET)"
-	rm -rf bin lib lib64 include share etc var inituser pyvenv.cfg .installed.cfg
-	rm -rf frontend/dist frontend/node_modules
-
 .PHONY: start
 start: ## Start a Plone instance on localhost:8080
-	PYTHONWARNINGS=ignore ./bin/runwsgi instance/etc/zope.ini
+	DEVELOP_DISTRIBUTIONS=$(DISTRIBUTIONS) PYTHONWARNINGS=ignore ./bin/runwsgi instance/etc/zope.ini
 
 .PHONY: format-frontend
 format-frontend: ## Format frontend codebase
 	@echo "$(GREEN)==> Format frontend codebase$(RESET)"
 	(cd frontend && pnpm lint:fix)
 	(cd frontend && pnpm prettier:fix)
 
 .PHONY: format
-format: ## Format the codebase according to our standards
+format: bin/tox ## Format the codebase according to our standards
 	@echo "$(GREEN)==> Format codebase$(RESET)"
-	$(FORMAT)
+	bin/tox -e format
 	make format-frontend
 
 .PHONY: lint-frontend
 lint-frontend: ## Lint frontend codebase
 	@echo "$(GREEN)==> Lint frontend codebase$(RESET)"
 	(cd frontend && pnpm lint)
 	(cd frontend && pnpm prettier)
 
 .PHONY: lint
 lint: ## check code style
-	$(LINT)
+	bin/tox -e lint
 	make lint-frontend
 
-.PHONY: lint-black
-lint-black: ## validate black formating
-	$(LINT) black
-
-.PHONY: lint-flake8
-lint-flake8: ## validate black formating
-	$(LINT) flake8
-
-.PHONY: lint-isort
-lint-isort: ## validate using isort
-	$(LINT) isort
-
-.PHONY: lint-pyroma
-lint-pyroma: ## validate using pyroma
-	$(LINT) pyroma
-
-.PHONY: lint-zpretty
-lint-zpretty: ## validate ZCML/XML using zpretty
-	$(LINT) zpretty
-
 # i18n
 bin/i18ndude:	bin/pip
 	@echo "$(GREEN)==> Install translation tools$(RESET)"
 	bin/pip install i18ndude
 
 .PHONY: i18n
 i18n: bin/i18ndude ## Update locales
 	@echo "$(GREEN)==> Updating locales$(RESET)"
 	bin/update_locale
 
 # Tests
 .PHONY: test
-test: ## run tests
-	bin/pytest --disable-warnings
+test: bin/tox ## run tests
+	DEVELOP_DISTRIBUTIONS=$(DISTRIBUTIONS) bin/tox -e test
 
+.PHONY: test-coverage
+test-coverage: bin/tox ## run tests with coverage
+	DEVELOP_DISTRIBUTIONS=$(DISTRIBUTIONS) bin/tox -e coverage
 
 # Docs
 bin/sphinx-build: bin/pip
 	bin/pip install -r requirements-docs.txt
 
 .PHONY: build-docs
 build-docs: bin/sphinx-build  ## Build the documentation
```

### Comparing `plone.distribution-1.0.0a5/PKG-INFO` & `plone.distribution-1.0.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -272,14 +272,36 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a6 (2023-06-23)
+
+
+### New features:
+
+- Improve support for testing distributions [@ericof] #24
+- Allow export only for distributions still in development [@ericof] #28
+- Create a report for Plone sites created from a distribution [@ericof] #30
+- Clean up exported content to remove references to portal.absolute_url() [@ericof] #32
+
+
+### Bug fixes:
+
+- Content language should be allowed in portal configuration [@ericof] #23
+
+
+### Internal:
+
+- Update configuration files.
+  [plone devs] 047ec50d, 55bda5c9, d7e9e748
+
+
 ## 1.0.0a5 (2023-05-18)
 
 
 ### Bug fixes:
 
 - Import did not import any steps except content and portal. [pbauer] #22
```

### Comparing `plone.distribution-1.0.0a5/README.md` & `plone.distribution-1.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/docs/Makefile` & `plone.distribution-1.0.0a6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/docs/_static/favicon.ico` & `plone.distribution-1.0.0a6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/docs/_static/logo.svg` & `plone.distribution-1.0.0a6/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/docs/_static/styles.css` & `plone.distribution-1.0.0a6/docs/_static/styles.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/docs/api/index.md` & `plone.distribution-1.0.0a6/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/docs/conf.py` & `plone.distribution-1.0.0a6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/docs/index.md` & `plone.distribution-1.0.0a6/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/docs/usage/code-examples.md` & `plone.distribution-1.0.0a6/docs/usage/code-examples.md`

 * *Files 12% similar despite different names*

```diff
@@ -65,14 +65,28 @@
 ```python
 from plone.distribution.api import site as site_api
 
 
 sites = site_api.get_sites(app)
 ```
 
+
+(api-site-get_creation_report-example)=
+
+### Get creation report for a site
+
+To get a report of the creation of the site use the method {meth}`api.site.get_creation_report`.
+
+```python
+from plone.distribution.api import site as site_api
+
+site = app.Plone
+report = site_api.get_creation_report(site)
+```
+
 (api-site-create-example)=
 
 ### Create a new site
 
 Create a new Plone site using one of the available distributions using the method {meth}`api.site.create`.
 
 ```python
```

### Comparing `plone.distribution-1.0.0a5/docs/usage/index.md` & `plone.distribution-1.0.0a6/docs/usage/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/docs/usage/package-structure.md` & `plone.distribution-1.0.0a6/docs/usage/package-structure.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/mx.ini` & `plone.distribution-1.0.0a6/mx.ini`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/setup.py` & `plone.distribution-1.0.0a6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
     name="plone.distribution",
-    version="1.0.0a5",
+    version="1.0.0a6",
     description="Plone distribution support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/api/distribution.py` & `plone.distribution-1.0.0a6/src/plone/distribution/api/distribution.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/api/site.py` & `plone.distribution-1.0.0a6/src/plone/distribution/api/site.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from AccessControl import getSecurityManager
 from AccessControl.Permissions import view as View
+from datetime import datetime
+from datetime import timezone
 from plone.base.interfaces import IPloneSiteRoot
 from plone.distribution.api import distribution as dist_api
+from plone.distribution.core import SiteCreationReport
 from plone.distribution.handler import default_handler
 from plone.registry.interfaces import IRegistry
 from Products.CMFPlone.events import SiteManagerCreatedEvent
 from Products.CMFPlone.Portal import PloneSite
 from Products.GenericSetup.tool import SetupTool
 from typing import List
+from typing import Union
 from ZODB.broken import Broken
+from zope.annotation.interfaces import IAnnotations
 from zope.component import queryUtility
 from zope.component.hooks import setSite
 from zope.event import notify
 from zope.lifecycleevent import ObjectCreatedEvent
 
 
 _TOOL_ID = "portal_setup"
 _DEFAULT_PROFILE = "Products.CMFPlone:plone"
 
 
+SITE_REPORT_ANNO = "__plone_distribution_report__"
+
+
 def _required_str_value(answers: dict, key: str) -> str:
     try:
         return answers[key]
     except KeyError:
         raise KeyError(f"A value for {key} is required.")
 
 
@@ -48,14 +56,27 @@
             if secman.checkPermission(View, obj):
                 result.append(obj)
         elif obj.getId() in getattr(context, "_mount_points", {}):
             result.extend(get_sites(context=obj))
     return result
 
 
+def get_creation_report(site: PloneSite) -> Union[SiteCreationReport, None]:
+    """Return a site creation report for a Plone site.
+
+    :param site: Plone Site.
+    :returns: SiteCreationReport with distribution name, creation date and
+              answers used to create the site.
+
+    :Example: :ref:`api-site-get_creation_report-example`
+    """
+    annotations = IAnnotations(site)
+    return annotations.get(SITE_REPORT_ANNO, None)
+
+
 def create(
     context,
     distribution_name: str,
     answers: dict,
     profile_id: str = _DEFAULT_PROFILE,
 ) -> PloneSite:
     """Create a new Plone site using one of the distributions.
@@ -112,8 +133,14 @@
     reg["plone.available_languages"] = [default_language]
     reg["plone.site_title"] = title
     # Run the Distribution handler
     site = handler(distribution, site, answers)
     # Run the Distribution post_handler
     if post_handler:
         site = post_handler(distribution, site, answers)
+    # Create a report of a site creation
+    annotations = IAnnotations(site)
+    report = SiteCreationReport(
+        distribution_name, datetime.now(tz=timezone.utc), answers
+    )
+    annotations[SITE_REPORT_ANNO] = report
     return site
```

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/browser/admin.py` & `plone.distribution-1.0.0a6/src/plone/distribution/browser/admin.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/browser/configure.zcml` & `plone.distribution-1.0.0a6/src/plone/distribution/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/browser/image.py` & `plone.distribution-1.0.0a6/src/plone/distribution/browser/image.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/browser/overrides.zcml` & `plone.distribution-1.0.0a6/src/plone/distribution/browser/overrides.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-logo.png` & `plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-logo.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-overview.min.css` & `plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-overview.min.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone-overview.min.js` & `plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone-overview.min.js`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/browser/static/plone.svg` & `plone.distribution-1.0.0a6/src/plone/distribution/browser/static/plone.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/browser/templates/plone-overview.pt` & `plone.distribution-1.0.0a6/src/plone/distribution/browser/templates/plone-overview.pt`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
-<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en"
-      xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:metal="http://xml.zope.org/namespaces/metal"
+<html xmlns="http://www.w3.org/1999/xhtml"
       xmlns:i18n="http://xml.zope.org/namespaces/i18n"
+      xmlns:metal="http://xml.zope.org/namespaces/metal"
+      xmlns:tal="http://xml.zope.org/namespaces/tal"
       lang="en"
-      i18n:domain="plone">
+      xml:lang="en"
+      i18n:domain="plone"
+>
 
-<head>
-  <meta charset="utf-8"/>
-  <meta name="viewport" content="width=device-width, initial-scale=1"/>
-  <title>Welcome to Plone!</title>
-  <link
-      rel="icon"
-      type="image/svg+xml"
-      href="${string:${context/absolute_url}/++resource++plone.distribution/plone.svg}" />
-  <link rel="stylesheet"
-        type="text/css"
-        href="${string:${context/absolute_url}/++theme++barceloneta/css/barceloneta.min.css}" />
-  <link rel="stylesheet"
-        type="text/css"
-        href="${string:${context/absolute_url}/++resource++plone-admin-ui.css}" />
-  <link rel="stylesheet"
-        type="text/css"
-        href="${string:${context/absolute_url}/++resource++plone.distribution/plone-overview.min.css}" />
-  <script type="module" crossorigin
-    src="${string:${context/absolute_url}/++resource++plone.distribution/plone-overview.min.js}"></script>
-</head>
+  <head>
+    <meta charset="utf-8" />
+    <meta name="viewport"
+          content="width=device-width, initial-scale=1"
+    />
+    <title i18n:translate="">Welcome to Plone!</title>
+    <link href="${string:${context/absolute_url}/++resource++plone.distribution/plone.svg}"
+          rel="icon"
+          type="image/svg+xml"
+    />
+    <link href="${string:${context/absolute_url}/++theme++barceloneta/css/barceloneta.min.css}"
+          rel="stylesheet"
+          type="text/css"
+    />
+    <link href="${string:${context/absolute_url}/++resource++plone-admin-ui.css}"
+          rel="stylesheet"
+          type="text/css"
+    />
+    <link href="${string:${context/absolute_url}/++resource++plone.distribution/plone-overview.min.css}"
+          rel="stylesheet"
+          type="text/css"
+    />
+    <script crossorigin=""
+            src="${string:${context/absolute_url}/++resource++plone.distribution/plone-overview.min.js}"
+            type="module"
+    ></script>
+  </head>
 
 
-<body>
-  <div id="root"></div>
-</body>
+  <body>
+    <div id="root"></div>
+  </body>
 </html>
```

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/core.py` & `plone.distribution-1.0.0a6/src/plone/distribution/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from datetime import datetime
 from pathlib import Path
+from Persistence import Persistent
 from plone.distribution import BASE_DISTRIBUTIONS_PATH
 from plone.distribution.utils import schema as schema_utils
 from typing import Callable
 from typing import List
 
 import json
 
 
 DEFAULT_SCHEMA = json.load(open(BASE_DISTRIBUTIONS_PATH / "default" / "schema.json"))
 DEFAULT_IMAGE = BASE_DISTRIBUTIONS_PATH / "default" / "image.png"
 
 
 class Distribution:
-
     name: str
     title: str
     description: str
     directory: Path
     handler: Callable
     post_handler: Callable
     _schema: dict
@@ -94,7 +95,24 @@
         """Return content structure."""
         content_folder = self._content_folder
         content_profiles = self._profiles.get("content", [])
         return {
             "profiles": content_profiles,
             "json": content_folder if content_folder.exists() else None,
         }
+
+
+class SiteCreationReport(Persistent):
+    name: str
+    date: datetime
+    _answers: str
+
+    def __init__(self, name: str, date: datetime, answers: dict):
+        """Initialize the report."""
+        self.name = name
+        self.date = date
+        self._answers = tuple([(k, v) for k, v in answers.items()])
+
+    @property
+    def answers(self) -> dict:
+        """Return original answers."""
+        return dict(self._answers)
```

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/content.json` & `plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/content.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/portal.json` & `plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/portal.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/content/portlets.json` & `plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/content/portlets.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/image.png` & `plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/distributions/classic/schema.json` & `plone.distribution-1.0.0a6/src/plone/distribution/distributions/classic/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/content/portal.json` & `plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/content/portal.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999022692601068%*

 * *Differences: {'0': "{'blocks': {'b4193840-3c95-4b28-a088-f679c11e2dcb': {'plaintext': ' Volto is the frontend "*

 * *      'for Plone written in React. It exposes all these features and communicates with Plone via '*

 * *      "its mature REST API . Volto can be easily themed and is highly customizable.', 'value': {0: "*

 * *      "{'children': {2: {'text': ' is the frontend for Plone written in React. It exposes all "*

 * *      "these features and communicates with Plone via its mature '}}}}}}}"}*

```diff
@@ -345,15 +345,15 @@
                         ],
                         "type": "p"
                     }
                 ]
             },
             "b4193840-3c95-4b28-a088-f679c11e2dcb": {
                 "@type": "slate",
-                "plaintext": " Volto is the frontent for Plone written in React. It exposes all these features and communicates with Plone via its mature REST API . Volto can be easily themed and is highly customizable.",
+                "plaintext": " Volto is the frontend for Plone written in React. It exposes all these features and communicates with Plone via its mature REST API . Volto can be easily themed and is highly customizable.",
                 "value": [
                     {
                         "children": [
                             {
                                 "text": ""
                             },
                             {
@@ -364,15 +364,15 @@
                                 ],
                                 "data": {
                                     "url": "https://6.docs.plone.org/volto/index.html"
                                 },
                                 "type": "link"
                             },
                             {
-                                "text": " is the frontent for Plone written in React. It exposes all these features and communicates with Plone via its mature "
+                                "text": " is the frontend for Plone written in React. It exposes all these features and communicates with Plone via its mature "
                             },
                             {
                                 "children": [
                                     {
                                         "text": "REST API"
                                     }
                                 ],
```

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/image.png` & `plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/distributions/default/schema.json` & `plone.distribution-1.0.0a6/src/plone/distribution/distributions/default/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/exportimport/exportimport.py` & `plone.distribution-1.0.0a6/src/plone/distribution/exportimport/dist_export.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,107 +1,64 @@
-from App.config import getConfiguration
 from collective.exportimport import config
-from collective.exportimport import import_content
+from collective.exportimport.export_content import ExportContent as BaseExportView
 from logging import getLogger
-from pathlib import Path
 from plone import api
-from plone.distribution.api import distribution as dist_api
+from plone.distribution.core import Distribution
+from plone.distribution.exportimport.helpers import filter_devel_distributions
+from plone.distribution.exportimport.helpers import parse_blocks
+from plone.distribution.exportimport.helpers import remove_site_root
 from plone.distribution.exportimport.interfaces import IDistributionBlobsMarker
 from Products.Five import BrowserView
+from typing import List
 from zope.interface import alsoProvides
 
 
 logger = getLogger(__name__)
 
 
-class ImportAll(BrowserView):
-    def __call__(self, path=None):
-        request = self.request
-        if not path and not request.form.get("form.submitted", False):
-            return self.index()
-        elif path:
-            # path the config that is usually set via env-variables
-            config.CENTRAL_DIRECTORY = str(path)
-            import_content.BLOB_HOME = str(path)
-        else:
-            # Fallback to default (e.g. var/instance/import)
-            cfg = getConfiguration()
-            path = Path(cfg.clienthome) / "import"
-
-        view = api.content.get_view("import_content", self.context, request)
-        request.form["form.submitted"] = True
-
-        # Add content
-        request.form["commit"] = 500
-        view(server_file="content.json", return_json=True)
-
-        # Update the existing portal obj using the update-strategy
-        request.form["handle_existing_content"] = 2
-        view(server_file="portal.json", return_json=True)
-
-        other_imports = [
-            "relations",
-            "members",
-            "translations",
-            "localroles",
-            "ordering",
-            "defaultpages",
-            "discussion",
-            "portlets",
-            "redirects",
-        ]
-        for name in other_imports:
-            view = api.content.get_view(f"import_{name}", self.context, request)
-            importfile = path / f"{name}.json"
-            if importfile.exists():
-                results = view(jsonfile=importfile.read_text(), return_json=True)
-                logger.info(results)
-            else:
-                logger.info(f"Skipping import of {name} because no file {importfile}")
-
-        return request.response.redirect(self.context.absolute_url())
-
-
 class ExportAll(BrowserView):
     def __call__(self):
+        distribution = None
         request = self.request
         if not request.form.get("form.submitted", False):
             return self.index()
 
-        dist_name = request.form.get("distribution", False)
-        if not dist_name:
-            api.portal.show_message("Please select a target")
+        dist_name = request.form.get("distribution", "")
+        distributions = self.distributions(dist_name)
+        if not distributions:
+            api.portal.show_message("Please select a valid target")
             return self.index()
-
+        distribution = distributions[0]
         alsoProvides(self.request, IDistributionBlobsMarker)
-        distribution = dist_api.get(dist_name)
         package_path = distribution.directory
         directory = package_path / "content"
         config.CENTRAL_DIRECTORY = str(directory)
         # pass the target-dir to blob-serializer via request
         request.form["distribution_directory"] = str(directory)
 
         # Export all content
-        export_name = "export_content"
+        export_name = "dist_export_content"
         view = api.content.get_view(export_name, self.context, request)
         # small hack to get all exportable types from the view
         view.portal_type = []
         view.path = "/".join(self.context.getPhysicalPath())
         view.depth = -1
         portal_types = [
             i["value"] for i in view.portal_types() if i["value"] != "Plone Site"
         ]
         request.form["filename"] = "content.json"
         view(portal_type=portal_types, include_blobs=2, download_to_server=True)
-        logger.info("Finished {}".format(export_name))
+        logger.info(f"Finished {export_name}")
 
         portal_types = ["Plone Site"]
         request.form["filename"] = "portal.json"
+        # To handle an issue with json_body deserialization
+        request["BODY"] = {}
         view(portal_type=portal_types, include_blobs=2, download_to_server=True)
-        logger.info("Finished {}".format(export_name))
+        logger.info(f"Finished {export_name}")
 
         other_exports = [
             "relations",
             "members",
             "translations",
             "localroles",
             "ordering",
@@ -117,9 +74,48 @@
             request.form["form.submitted"] = True
             request.form["filename"] = f"{export}.json"
             export_view(download_to_server=True)
 
         logger.info("Finished export_all")
         return self.request.response.redirect(self.context.absolute_url())
 
-    def distributions(self):
-        return dist_api.get_distributions()
+    def distributions(self, name: str = "") -> List[Distribution]:
+        """Return a list of distributions."""
+        return filter_devel_distributions(name=name)
+
+
+class ExportContent(BaseExportView):
+    """Export content from a distribution."""
+
+    PORTAL_URL: str = ""
+
+    def __call__(
+        self,
+        portal_type=None,
+        path=None,
+        depth=-1,
+        include_blobs=1,
+        download_to_server=False,
+        migration=True,
+        include_revisions=False,
+    ):
+        self.PORTAL_URL = api.portal.get().absolute_url()
+        return super().__call__(
+            portal_type,
+            path,
+            depth,
+            include_blobs,
+            download_to_server,
+            migration,
+            include_revisions,
+        )
+
+    def global_dict_hook(self, item, obj):
+        """Clean up data before export."""
+        item = remove_site_root(item)
+        if item["@type"] == "Plone Site":
+            # To avoid a conflict between @id and id
+            item["@id"] = f"/{item['id']}"
+        if "blocks" in item:
+            blocks = item["blocks"]
+            item["blocks"] = parse_blocks(blocks)
+        return item
```

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/exportimport/serializer.py` & `plone.distribution-1.0.0a6/src/plone/distribution/exportimport/serializer.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/exportimport/templates/import_all.pt` & `plone.distribution-1.0.0a6/src/plone/distribution/exportimport/templates/import_all.pt`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,52 @@
 <html xmlns="http://www.w3.org/1999/xhtml"
+      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
       xmlns:metal="http://xml.zope.org/namespaces/metal"
       xmlns:tal="http://xml.zope.org/namespaces/tal"
-      xmlns:i18n="http://xml.zope.org/namespaces/i18n"
-      i18n:domain="plone.z3cform"
-      metal:use-macro="context/main_template/macros/master">
+      metal:use-macro="context/main_template/macros/master"
+      i18n:domain="plone.distribution"
+>
 
-<div metal:fill-slot="main">
+  <div metal:fill-slot="main">
     <tal:main-macro metal:define-macro="main">
 
-      <h1 class="documentFirstHeading">Import all</h1>
-
-      <p class="documentDescription">Run all imports</p>
-
-        <form action="@@import_all" tal:attributes="action request/URL" method="post" enctype="multipart/form-data">
-
-            <div class="formControls" class="form-group">
-                <input type="hidden" name="form.submitted" value="1"/>
-
-                <button class="btn btn-primary submit-widget button-field context"
-                        type="submit" name="submit" value="export">Import all
-                </button>
-            </div>
+      <h1 class="documentFirstHeading"
+          i18n:translate=""
+      >Import Distribution Data</h1>
+
+      <p class="documentDescription"
+         i18n:translate=""
+      >Run all imports</p>
+
+      <form action="@@import_all"
+            enctype="multipart/form-data"
+            method="post"
+            tal:attributes="
+              action request/URL;
+            "
+      >
+
+        <div class="form-group">
+          <input name="form.submitted"
+                 type="hidden"
+                 value="1"
+          />
+
+          <button class="btn btn-primary submit-widget button-field context"
+                  name="submit"
+                  type="submit"
+                  value="export"
+                  i18n:translate=""
+          >Import all
+          </button>
+        </div>
 
-            <div metal:use-macro="context/@@exportimport_links/links">
+        <div metal:use-macro="context/@@exportimport_links/links">
               Links to all exports and imports
-            </div>
+        </div>
 
-        </form>
+      </form>
 
     </tal:main-macro>
-</div>
+  </div>
 
 </html>
```

#### html2text {}

```diff
@@ -1,4 +1,4 @@
-****** Import all ******
+****** Import Distribution Data ******
 Run all imports
  Import all
 Links to all exports and imports
```

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/handler.py` & `plone.distribution-1.0.0a6/src/plone/distribution/handler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from plone import api
 from plone.distribution.core import Distribution
 from Products.CMFPlone.Portal import PloneSite
-from zope.component import getMultiAdapter
 from zope.globalrequest import getRequest
 
+import transaction
+
 
 def default_handler(
     distribution: Distribution, site: PloneSite, answers: dict
 ) -> PloneSite:
     """Default handler to create a new site."""
     # Process answers
     profiles = distribution.profiles
@@ -21,10 +23,13 @@
         # First process any content profiles
         content_profiles = contents["profiles"]
         for profile_id in content_profiles:
             setup_tool.runAllImportStepsFromProfile(f"profile-{profile_id}")
         # Process content import from json
         content_json_path = contents["json"]
         if content_json_path:
-            import_all = getMultiAdapter((site, getRequest()), name="import_all")
+            # If there is no savepoint most tests fail with a PosKeyError
+            transaction.savepoint(optimistic=True)
+            request = getRequest() or site.REQUEST
+            import_all = api.content.get_view("dist_import_all", site, request)
             import_all(content_json_path)
     return site
```

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/interfaces.py` & `plone.distribution-1.0.0a6/src/plone/distribution/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/registry.py` & `plone.distribution-1.0.0a6/src/plone/distribution/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         return self.lookup(name)
 
     @security.protected(ManagePortal)
     def enumerate_distributions(self) -> List[Distribution]:
         """Return all distributions registered in the Distribution Registry.
 
         This implementation returns the distributions sorted by name, but keep
-        the distribuion named default as the first item of the list.
+        the distribution named default as the first item of the list.
         """
         result = []
         distributions = sorted(self._registered.items())
         for name, distribution in distributions:
             if name == "default":
                 result.insert(0, distribution)
             else:
```

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/services/auth/login.py` & `plone.distribution-1.0.0a6/src/plone/distribution/services/auth/login.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/services/sites/add.py` & `plone.distribution-1.0.0a6/src/plone/distribution/services/sites/add.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/services/sites/configure.zcml` & `plone.distribution-1.0.0a6/src/plone/distribution/services/sites/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/services/sites/get.py` & `plone.distribution-1.0.0a6/src/plone/distribution/services/sites/get.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/testing.py` & `plone.distribution-1.0.0a6/src/plone/distribution/testing/testing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,40 @@
+from .layer import DEFAULT_ANSWERS
+from .layer import PloneDistributionFixture
 from plone.app.testing import FunctionalTesting
 from plone.app.testing import IntegrationTesting
-from plone.app.testing import PLONE_FIXTURE
 from plone.app.testing import PloneSandboxLayer
 from plone.testing.zope import WSGI_SERVER_FIXTURE
 
 
-class DistributionLayer(PloneSandboxLayer):
+CLASSIC_ANSWERS = {
+    "site_id": "classic",
+    "title": "Plone Site",
+    "description": "A Plone Site with Classic UI",
+    "default_language": "en",
+    "portal_timezone": "America/Sao_Paulo",
+    "setup_content": True,
+}
 
-    defaultBases = (PLONE_FIXTURE,)
 
-    def setUpZope(self, app, configurationContext):
-        import plone.distribution
-        import plone.volto
+class BaseFixture(PloneDistributionFixture):
+    SITES = (
+        ("default", DEFAULT_ANSWERS),
+        ("classic", CLASSIC_ANSWERS),
+    )
 
-        self.loadZCML(package=plone.distribution)
-        self.loadZCML(package=plone.volto)
 
+BASE_FIXTURE = BaseFixture()
 
-FIXTURE = DistributionLayer()
+
+class Layer(PloneSandboxLayer):
+    defaultBases = (BASE_FIXTURE,)
+
+
+FIXTURE = Layer()
 
 
 INTEGRATION_TESTING = IntegrationTesting(
     bases=(FIXTURE,),
     name="DistributionLayer:IntegrationTesting",
 )
```

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/utils/request.py` & `plone.distribution-1.0.0a6/src/plone/distribution/utils/request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/utils/schema.py` & `plone.distribution-1.0.0a6/src/plone/distribution/utils/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     tz_vocab = getUtility(IVocabularyFactory, "plone.app.vocabularies.CommonTimezones")(
         context
     )
 
     response = []
     for term in tz_vocab:
         value = term.value
-        splitted = value.split("/")
-        friendly = splitted[-1]
+        split_value = value.split("/")
+        friendly = split_value[-1]
         label = f"{friendly} ({value})"
         response.append({"label": label, "value": value})
 
     return response
 
 
 def _available_languages() -> list:
```

### Comparing `plone.distribution-1.0.0a5/src/plone/distribution/zcml.py` & `plone.distribution-1.0.0a6/src/plone/distribution/metaconfigure.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/src/plone.distribution.egg-info/PKG-INFO` & `plone.distribution-1.0.0a6/src/plone.distribution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -272,14 +272,36 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a6 (2023-06-23)
+
+
+### New features:
+
+- Improve support for testing distributions [@ericof] #24
+- Allow export only for distributions still in development [@ericof] #28
+- Create a report for Plone sites created from a distribution [@ericof] #30
+- Clean up exported content to remove references to portal.absolute_url() [@ericof] #32
+
+
+### Bug fixes:
+
+- Content language should be allowed in portal configuration [@ericof] #23
+
+
+### Internal:
+
+- Update configuration files.
+  [plone devs] 047ec50d, 55bda5c9, d7e9e748
+
+
 ## 1.0.0a5 (2023-05-18)
 
 
 ### Bug fixes:
 
 - Import did not import any steps except content and portal. [pbauer] #22
```

### Comparing `plone.distribution-1.0.0a5/src/plone.distribution.egg-info/SOURCES.txt` & `plone.distribution-1.0.0a6/src/plone.distribution.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 .editorconfig
+.flake8
 .gitignore
+.meta.toml
+.pre-commit-config.yaml
 CHANGES.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 constraints.txt
 instance.yaml
 mx.ini
 pyproject.toml
 requirements-docs.txt
 requirements.txt
 setup.py
+tox.ini
 docs/Makefile
-docs/changelog_template.jinja
 docs/conf.py
 docs/index.md
 docs/_static/favicon.ico
 docs/_static/logo.svg
 docs/_static/print.css
 docs/_static/styles.css
 docs/api/distribution.md
@@ -40,17 +43,16 @@
 src/plone/distribution/__init__.py
 src/plone/distribution/configure.zcml
 src/plone/distribution/core.py
 src/plone/distribution/distributions.zcml
 src/plone/distribution/handler.py
 src/plone/distribution/interfaces.py
 src/plone/distribution/meta.zcml
+src/plone/distribution/metaconfigure.py
 src/plone/distribution/registry.py
-src/plone/distribution/testing.py
-src/plone/distribution/zcml.py
 src/plone/distribution/api/__init__.py
 src/plone/distribution/api/distribution.py
 src/plone/distribution/api/site.py
 src/plone/distribution/browser/__init__.py
 src/plone/distribution/browser/admin.py
 src/plone/distribution/browser/configure.zcml
 src/plone/distribution/browser/image.py
@@ -70,35 +72,46 @@
 src/plone/distribution/distributions/classic/content/portlets.json
 src/plone/distribution/distributions/default/image.png
 src/plone/distribution/distributions/default/profiles.json
 src/plone/distribution/distributions/default/schema.json
 src/plone/distribution/distributions/default/content/portal.json
 src/plone/distribution/exportimport/__init__.py
 src/plone/distribution/exportimport/configure.zcml
-src/plone/distribution/exportimport/exportimport.py
+src/plone/distribution/exportimport/dist_export.py
+src/plone/distribution/exportimport/dist_import.py
+src/plone/distribution/exportimport/helpers.py
 src/plone/distribution/exportimport/interfaces.py
 src/plone/distribution/exportimport/serializer.py
 src/plone/distribution/exportimport/templates/export_all.pt
 src/plone/distribution/exportimport/templates/import_all.pt
 src/plone/distribution/services/__init__.py
 src/plone/distribution/services/configure.zcml
 src/plone/distribution/services/auth/__init__.py
 src/plone/distribution/services/auth/configure.zcml
 src/plone/distribution/services/auth/login.py
 src/plone/distribution/services/sites/__init__.py
 src/plone/distribution/services/sites/add.py
 src/plone/distribution/services/sites/configure.zcml
 src/plone/distribution/services/sites/get.py
+src/plone/distribution/testing/__init__.py
+src/plone/distribution/testing/layer.py
+src/plone/distribution/testing/testing.py
 src/plone/distribution/utils/__init__.py
 src/plone/distribution/utils/request.py
 src/plone/distribution/utils/schema.py
 tests/__init__.py
 tests/conftest.py
 tests/api/test_api_distribution.py
 tests/api/test_api_site.py
+tests/distributions/__init__.py
+tests/distributions/conftest.py
+tests/distributions/test_distributions_classic.py
+tests/distributions/test_distributions_default.py
+tests/exportimport/portal.json
+tests/exportimport/test_exportimport_helpers.py
 tests/services/__init__.py
 tests/services/conftest.py
 tests/services/test_services_site.py
 tests/utils/__init__.py
 tests/utils/test_utils_request.py
 tests/utils/test_utils_schema.py
 tests/utils/data/invalid.json
```

### Comparing `plone.distribution-1.0.0a5/tests/api/test_api_distribution.py` & `plone.distribution-1.0.0a6/tests/api/test_api_distribution.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/tests/services/test_services_site.py` & `plone.distribution-1.0.0a6/tests/services/test_services_site.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         assert distributions[0]["title"] == "Plone Site"
 
     def test_sites_get_sites(self, app):
         response = self.api_session.get("@sites")
         data = response.json()
         sites = data["sites"]
         assert isinstance(sites, list)
-        assert len(sites) == 1
+        assert len(sites) == 3
         assert sites[0]["id"] == "plone"
         assert sites[0]["needs_upgrade"] is False
 
 
 class TestServicesSitesPOST(TestServicesSite):
     @pytest.fixture(autouse=True)
     def _answers(self):
```

### Comparing `plone.distribution-1.0.0a5/tests/utils/data/invalid.json` & `plone.distribution-1.0.0a6/tests/utils/data/invalid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/tests/utils/data/valid.json` & `plone.distribution-1.0.0a6/tests/utils/data/valid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0a5/tests/utils/test_utils_request.py` & `plone.distribution-1.0.0a6/tests/utils/test_utils_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 class TestUtilsRequest:
     @pytest.mark.parametrize(
         "language,expected",
         [
             ("en-US,en;q=0.5", "en-us"),
             ("pt-BR,pt;q=0.5", "pt-br"),
             ("pt-BO,pt;q=0.5", "pt"),
+            ("pt-PT,pt;q=0.5", "pt"),
             ("en;q=0.5", "en"),
             ("es;q=0.5", "es"),
             ("de;q=0.5", "de"),
         ],
     )
     def test_extract_browser_language(self, language, expected):
         provideAdapter(BrowserLanguages, [IHTTPRequest], IUserPreferredLanguages)
```

### Comparing `plone.distribution-1.0.0a5/tests/utils/test_utils_schema.py` & `plone.distribution-1.0.0a6/tests/utils/test_utils_schema.py`

 * *Files identical despite different names*

