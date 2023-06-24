# Comparing `tmp/openfractal_client-0.0.0.tar.gz` & `tmp/openfractal_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfractal_client-0.0.0.tar", last modified: Mon Jun  5 21:28:35 2023, max compression
+gzip compressed data, was "openfractal_client-0.1.0.tar", last modified: Sat Jun 24 14:25:46 2023, max compression
```

## Comparing `openfractal_client-0.0.0.tar` & `openfractal_client-0.1.0.tar`

### file list

```diff
@@ -1,38 +1,45 @@
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/.github/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)        9 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/.github/CODEOWNERS
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     5202 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/.github/CODE_OF_CONDUCT.md
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      333 2023-06-05 13:38:23.000000 openfractal_client-0.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      104 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/.github/SECURITY.md
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/.github/workflows/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1119 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/.github/workflows/code-check.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1397 2023-06-05 16:33:55.000000 openfractal_client-0.0.0/.github/workflows/doc.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1366 2023-06-05 21:23:36.000000 openfractal_client-0.0.0/.github/workflows/docker.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     3112 2023-06-05 17:37:51.000000 openfractal_client-0.0.0/.github/workflows/release.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1055 2023-06-05 16:20:43.000000 openfractal_client-0.0.0/.github/workflows/test.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      477 2023-06-05 13:35:03.000000 openfractal_client-0.0.0/.gitignore
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       32 2023-06-05 13:34:51.000000 openfractal_client-0.0.0/CHANGELOG.md
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     2607 2023-06-05 17:03:50.000000 openfractal_client-0.0.0/Dockerfile
--rw-rw-r--   0 hadim     (1000) hadim     (1000)    11315 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/LICENSE
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     3220 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/PKG-INFO
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1834 2023-06-05 21:00:45.000000 openfractal_client-0.0.0/README.md
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/docker/
--rwxrwxr-x   0 hadim     (1000) hadim     (1000)     1191 2023-06-05 20:57:48.000000 openfractal_client-0.0.0/docker/entrypoint.sh
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      695 2023-06-05 21:23:27.000000 openfractal_client-0.0.0/docker-compose.yml
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/docs/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       21 2023-06-05 13:33:33.000000 openfractal_client-0.0.0/docs/index.md
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       20 2023-04-22 12:58:40.000000 openfractal_client-0.0.0/docs/license.md
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      746 2023-06-05 13:59:38.000000 openfractal_client-0.0.0/env.yml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1690 2023-06-05 21:00:48.000000 openfractal_client-0.0.0/mkdocs.yml
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/openfractal_client/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       34 2023-06-05 13:36:33.000000 openfractal_client-0.0.0/openfractal_client/__init__.py
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      229 2023-06-05 13:36:59.000000 openfractal_client-0.0.0/openfractal_client/_version.py
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/openfractal_client.egg-info/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     3220 2023-06-05 21:28:35.000000 openfractal_client-0.0.0/openfractal_client.egg-info/PKG-INFO
--rw-rw-r--   0 hadim     (1000) hadim     (1000)      651 2023-06-05 21:28:35.000000 openfractal_client-0.0.0/openfractal_client.egg-info/SOURCES.txt
--rw-rw-r--   0 hadim     (1000) hadim     (1000)        1 2023-06-05 21:28:35.000000 openfractal_client-0.0.0/openfractal_client.egg-info/dependency_links.txt
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       19 2023-06-05 21:28:35.000000 openfractal_client-0.0.0/openfractal_client.egg-info/top_level.txt
--rw-rw-r--   0 hadim     (1000) hadim     (1000)     1885 2023-06-05 21:28:31.000000 openfractal_client-0.0.0/pyproject.toml
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       38 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/setup.cfg
-drwxrwxr-x   0 hadim     (1000) hadim     (1000)        0 2023-06-05 21:28:35.247740 openfractal_client-0.0.0/tests/
--rw-rw-r--   0 hadim     (1000) hadim     (1000)       49 2023-06-05 13:35:24.000000 openfractal_client-0.0.0/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.505146 openfractal_client-0.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.505146 openfractal_client-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/CHANGELOGS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.505146 openfractal_client-0.1.0/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/configs/manager_local.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/configs/manager_slurm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.505146 openfractal_client-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    50050 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docs/tutorials/01_submit_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    36862 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docs/tutorials/02_execute_manager.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31799 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docs/tutorials/03_export_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/openfractal_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/openfractal_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/openfractal_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/openfractal_client/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/openfractal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-24 14:25:46.000000 openfractal_client-0.1.0/openfractal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-24 14:25:46.000000 openfractal_client-0.1.0/openfractal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:25:46.000000 openfractal_client-0.1.0/openfractal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-24 14:25:46.000000 openfractal_client-0.1.0/openfractal_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-24 14:25:46.000000 openfractal_client-0.1.0/openfractal_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/tests/test_import.py
```

### Comparing `openfractal_client-0.0.0/.github/CODE_OF_CONDUCT.md` & `openfractal_client-0.1.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/.github/workflows/code-check.yml` & `openfractal_client-0.1.0/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/.github/workflows/doc.yml` & `openfractal_client-0.1.0/.github/workflows/doc.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 name: doc
 
 on:
   push:
     branches: ["main"]
-    tags: ["*"]
 
 # Prevent doc action on `main` to conflict with each others.
 concurrency:
   group: doc-${{ github.ref }}
   cancel-in-progress: true
 
 permissions:
@@ -31,27 +30,19 @@
           environment-name: openfractal
           cache-environment: true
           cache-downloads: true
 
       - name: Install library
         run: python -m pip install --no-deps .
 
-      - name: Deploy the doc
+      - name: Configure git
         run: |
-          echo "Configure git"
           git config --global user.name "${GITHUB_ACTOR}"
           git config --global user.email "${GITHUB_ACTOR}@users.noreply.github.com"
 
+      - name: Deploy the doc
+        run: |
           echo "Get the gh-pages branch"
           git fetch origin gh-pages
 
-          TAG_OR_BRANCH_NAME=${GITHUB_REF##*/}
-
-          if [ $TAG_OR_BRANCH_NAME = "main" ]; then
-            echo "Build and deploy the doc on main"
-            mike deploy --push --force main
-          else
-            echo "Build and deploy the doc on $TAG_OR_BRANCH_NAME"
-
-            mike deploy --push --force stable
-            mike deploy --push --force $TAG_OR_BRANCH_NAME
-          fi
+          echo "Build and deploy the doc on main"
+          mike deploy --push --force main
```

### Comparing `openfractal_client-0.0.0/.github/workflows/docker.yml` & `openfractal_client-0.1.0/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/.github/workflows/release.yml` & `openfractal_client-0.1.0/.github/workflows/release.yml`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     inputs:
       release-version:
         description: "A valid Semver version string"
         required: true
 
 permissions:
   contents: write
+  pull-requests: write
 
 jobs:
   release:
     # Do not release if not triggered from the default branch
     if: github.ref == format('refs/heads/{0}', github.event.repository.default_branch)
 
     runs-on: ubuntu-latest
@@ -64,26 +65,37 @@
 
           if [ "$IS_HIGHER_VERSION" != "1" ]; then
             echo "The version '$RELEASE_VERSION' is not higher than the latest version '$LATEST_VERSION'."
             echo "The release process is aborted."
             exit 1
           fi
 
+      - name: Build Changelog
+        id: github_release
+        uses: mikepenz/release-changelog-builder-action@v4
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+        with:
+          toTag: "main"
+
       - name: Configure git
         run: |
           git config --global user.name "${GITHUB_ACTOR}"
           git config --global user.email "${GITHUB_ACTOR}@users.noreply.github.com"
 
       - name: Create and push git tag
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
         run: |
           # Tag the release
           git tag -a "${{ inputs.release-version }}" -m "Release version ${{ inputs.release-version }}"
 
+          # Push the modified changelogs
+          git push origin main
+
           # Push the tags
           git push origin "${{ inputs.release-version }}"
 
       - name: Install library
         run: python -m pip install --no-deps .
 
       - name: Build the wheel and sdist
@@ -95,8 +107,17 @@
           password: ${{ secrets.PYPI_API_TOKEN }}
           packages-dir: dist/
 
       - name: Create GitHub Release
         uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
         with:
           tag_name: ${{ inputs.release-version }}
-          body: "See [CHANGELOGS.md](https://github.com/datamol-io/datamol/blob/main/CHANGELOG.md)."
+          body: ${{steps.github_release.outputs.changelog}}
+
+      - name: Deploy the doc
+        run: |
+          echo "Get the gh-pages branch"
+          git fetch origin gh-pages
+
+          echo "Build and deploy the doc on ${{ inputs.release-version }}"
+          mike deploy --push --force stable
+          mike deploy --push --force ${{ inputs.release-version }}
```

### Comparing `openfractal_client-0.0.0/.github/workflows/test.yml` & `openfractal_client-0.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/LICENSE` & `openfractal_client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.0.0/PKG-INFO` & `openfractal_client-0.1.0/openfractal_client.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openfractal_client
-Version: 0.0.0
+Name: openfractal-client
+Version: 0.1.0
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,38 +32,38 @@
 [![release](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/release.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/release.yml)
 [![docker](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/docker.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/docker.yml)
 [![code-check](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/code-check.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/code-check.yml)
 [![doc](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/doc.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/doc.yml)
 
 A Python client based on [QCPortal](https://github.com/MolSSI/QCFractal) for Open Drug Discovery (ODD) QM large scale data generation.
 
+## Documentation
+
+Visit <https://opendrugdiscovery.github.io/openfractal-client/>.
+
 ## Development lifecycle
 
 ### Setup dev environment
 
 ```bash
 micromamba create -n openfractal -f env.yml
 micromamba activate openfractal
 
-# Install the git version of QCPortal
-pip install --no-deps git+https://github.com/MolSSI/QCFractal.git@c00627258f9344b4b35a7583ee4a9cc5ff2de3e8#subdirectory=qcportal
-pip install --no-deps git+https://github.com/MolSSI/QCFractal.git@c00627258f9344b4b35a7583ee4a9cc5ff2de3e8#subdirectory=qcfractalcompute
-
 # Install openfractal-client lib
 pip install -e .
 ```
 
 ### Tests
 
 You can run tests locally with:
 
 ```bash
 pytest
 ```
 
 ## Changelogs
 
-See the latest changelogs at [CHANGELOG.md](./CHANGELOG.md).
+See the latest changelogs at [CHANGELOGS.md](./CHANGELOGS.md).
 
 ## License
 
 Under the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `openfractal_client-0.0.0/README.md` & `openfractal_client-0.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 [![release](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/release.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/release.yml)
 [![docker](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/docker.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/docker.yml)
 [![code-check](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/code-check.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/code-check.yml)
 [![doc](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/doc.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/doc.yml)
 
 A Python client based on [QCPortal](https://github.com/MolSSI/QCFractal) for Open Drug Discovery (ODD) QM large scale data generation.
 
+## Documentation
+
+Visit <https://opendrugdiscovery.github.io/openfractal-client/>.
+
 ## Development lifecycle
 
 ### Setup dev environment
 
 ```bash
 micromamba create -n openfractal -f env.yml
 micromamba activate openfractal
 
-# Install the git version of QCPortal
-pip install --no-deps git+https://github.com/MolSSI/QCFractal.git@c00627258f9344b4b35a7583ee4a9cc5ff2de3e8#subdirectory=qcportal
-pip install --no-deps git+https://github.com/MolSSI/QCFractal.git@c00627258f9344b4b35a7583ee4a9cc5ff2de3e8#subdirectory=qcfractalcompute
-
 # Install openfractal-client lib
 pip install -e .
 ```
 
 ### Tests
 
 You can run tests locally with:
 
 ```bash
 pytest
 ```
 
 ## Changelogs
 
-See the latest changelogs at [CHANGELOG.md](./CHANGELOG.md).
+See the latest changelogs at [CHANGELOGS.md](./CHANGELOGS.md).
 
 ## License
 
 Under the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `openfractal_client-0.0.0/mkdocs.yml` & `openfractal_client-0.1.0/mkdocs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 docs_dir: "docs"
 
 # Fail on warnings to detect issues with types and docstring
 strict: true
 
 nav:
   - Overview: index.md
+  - Tutorials:
+      - Submit a Dataset: tutorials/01_submit_dataset.ipynb
+      - Execute a Manager: tutorials/02_execute_manager.ipynb
+      - Export a Dataset: tutorials/03_export_dataset.ipynb
   - License: license.md
 
 theme:
   name: material
   # NOTE(hadim): to customize the material primary and secondary
   # color check `docs/assets/css/datamol-custom.css`.
   features:
```

### Comparing `openfractal_client-0.0.0/openfractal_client.egg-info/PKG-INFO` & `openfractal_client-0.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openfractal-client
-Version: 0.0.0
+Name: openfractal_client
+Version: 0.1.0
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
@@ -32,38 +32,38 @@
 [![release](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/release.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/release.yml)
 [![docker](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/docker.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/docker.yml)
 [![code-check](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/code-check.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/code-check.yml)
 [![doc](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/doc.yml/badge.svg)](https://github.com/OpenDrugDiscovery/openfractal-client/actions/workflows/doc.yml)
 
 A Python client based on [QCPortal](https://github.com/MolSSI/QCFractal) for Open Drug Discovery (ODD) QM large scale data generation.
 
+## Documentation
+
+Visit <https://opendrugdiscovery.github.io/openfractal-client/>.
+
 ## Development lifecycle
 
 ### Setup dev environment
 
 ```bash
 micromamba create -n openfractal -f env.yml
 micromamba activate openfractal
 
-# Install the git version of QCPortal
-pip install --no-deps git+https://github.com/MolSSI/QCFractal.git@c00627258f9344b4b35a7583ee4a9cc5ff2de3e8#subdirectory=qcportal
-pip install --no-deps git+https://github.com/MolSSI/QCFractal.git@c00627258f9344b4b35a7583ee4a9cc5ff2de3e8#subdirectory=qcfractalcompute
-
 # Install openfractal-client lib
 pip install -e .
 ```
 
 ### Tests
 
 You can run tests locally with:
 
 ```bash
 pytest
 ```
 
 ## Changelogs
 
-See the latest changelogs at [CHANGELOG.md](./CHANGELOG.md).
+See the latest changelogs at [CHANGELOGS.md](./CHANGELOGS.md).
 
 ## License
 
 Under the Apache-2.0 license. See [LICENSE](LICENSE).
```

### Comparing `openfractal_client-0.0.0/pyproject.toml` & `openfractal_client-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openfractal_client"
 description = "A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation."
 authors = [{ name = "Hadrien Mary", email = "hadrien@valencediscovery.com" }]
 readme = "README.md"
-# dynamic = ["version"]
-version = "0.0.0"
+dynamic = ["version"]
 requires-python = ">=3.9"
 license = { text = "Apache" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Healthcare Industry",
     "Intended Audience :: Science/Research",
@@ -26,14 +25,17 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = []
 
+[project.scripts]
+opfc = "openfractal_client.cli:app"
+
 [project.urls]
 "Source Code" = "https://github.com/OpenDrugDiscovery/openfractal-client"
 "Bug Tracker" = "https://github.com/OpenDrugDiscovery/openfractal-client/issues"
 Documentation = "https://github.com/OpenDrugDiscovery/openfractal-client"
 
 [tool.setuptools]
 include-package-data = true
```

