# Comparing `tmp/scikit_build_core-0.4.6.tar.gz` & `tmp/scikit_build_core-0.4.7.tar.gz`

## Comparing `scikit_build_core-0.4.6.tar` & `scikit_build_core-0.4.7.tar`

### file list

```diff
@@ -1,267 +1,267 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.gitattributes
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.packit.yaml
--rw-r--r--   0        0        0     3380 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.readthedocs.yml
--rw-r--r--   0        0        0     6527 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/noxfile.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.fmf/version
--rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/matchers/pylint.json
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/workflows/cd.yml
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.github/workflows/ci.yml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/packit.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/python-scikit-build-core.spec
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/plans/examples.fmf
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/plans/main.fmf.dist-git
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/plans/rpmlint.fmf
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/plans/smoke.fmf
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/tests/rpmlint.fmf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/distro/tests/smoke.fmf
--rw-r--r--   0        0        0    17544 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/changelog.md
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/cmakelists.md
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/conf.py
--rw-r--r--   0        0        0    12729 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/configuration.md
--rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/getting_started.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/index.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/man.md
--rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/migration_guide.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/main.fmf
--rwxr-xr-x   0        0        0      865 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/test.sh
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/CMakeLists.txt
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/LICENSE
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/README.md
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/pyproject.toml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/tests/test_basic.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/CMakeLists.txt
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/LICENSE
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/README.md
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/pyproject.toml
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/src/main.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/tests/test_basic.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/abi3/main.fmf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/c/main.fmf
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/cython/main.fmf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/fortran/main.fmf
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/nanobind/CMakeLists.txt
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/nanobind/example.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/nanobind/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/pybind11/main.fmf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/swig/main.fmf
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0    10814 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/metadata.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     7759 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/setuptools/build_cmake.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/src/scikit_build_core/setuptools/wrapper.py
--rw-r--r--   0        0        0     9491 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/conftest.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/constraints.txt
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_builder.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_cmake_config.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_custom_modules.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_file_processor.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_fileapi.py
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_generator_default.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_get_requires.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_name_main.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_program_search.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_settings.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_shutil.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_simple_pure.py
--rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_simplest_c.py
--rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/CMakeLists.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/setup.cfg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/setup.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/src/main.cpp
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/LICENSE
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/pyproject.toml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/_module.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/LICENSE
--rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/README.md
--rw-r--r--   0        0        0     9166 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/pyproject.toml
--rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 scikit_build_core-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.gitattributes
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.packit.yaml
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.readthedocs.yml
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/noxfile.py
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.fmf/version
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/packit.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/python-scikit-build-core.spec
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/plans/examples.fmf
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/plans/main.fmf.dist-git
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/plans/rpmlint.fmf
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/plans/smoke.fmf
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/tests/rpmlint.fmf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/distro/tests/smoke.fmf
+-rw-r--r--   0        0        0    18148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/changelog.md
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/cmakelists.md
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/conf.py
+-rw-r--r--   0        0        0    12729 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/configuration.md
+-rw-r--r--   0        0        0    10617 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/getting_started.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/index.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/man.md
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/migration_guide.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/main.fmf
+-rwxr-xr-x   0        0        0      865 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/test.sh
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/CMakeLists.txt
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/LICENSE
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/README.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/pyproject.toml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/tests/test_basic.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/CMakeLists.txt
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/LICENSE
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/README.md
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/pyproject.toml
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/src/main.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/tests/test_basic.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/abi3/main.fmf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/c/main.fmf
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/cython/main.fmf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/fortran/main.fmf
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/nanobind/CMakeLists.txt
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/nanobind/example.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/nanobind/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/pybind11/main.fmf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/swig/main.fmf
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0    10865 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     7032 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     4990 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/metadata.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0    18158 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     7825 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/setuptools/build_cmake.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/src/scikit_build_core/setuptools/wrapper.py
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/conftest.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/constraints.txt
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_builder.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_file_processor.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_fileapi.py
+-rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_generator_default.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_get_requires.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_logging.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_name_main.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_program_search.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     8248 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_settings.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_shutil.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    12743 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/CMakeLists.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/setup.cfg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/setup.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/src/main.cpp
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/LICENSE
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/pyproject.toml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/_module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/LICENSE
+-rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/README.md
+-rw-r--r--   0        0        0     9033 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0    14490 2020-02-02 00:00:00.000000 scikit_build_core-0.4.7/PKG-INFO
```

### Comparing `scikit_build_core-0.4.6/.packit.yaml` & `scikit_build_core-0.4.7/.packit.yaml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/.pre-commit-config.yaml` & `scikit_build_core-0.4.7/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -50,41 +50,42 @@
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: "^tests"
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.272
+    rev: v0.0.275
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.4.0
     hooks:
       - id: mypy
         exclude: |
           (?x)^(
             tests/packages/simplest_c/src/simplest/__init__.py|
             tests/packages/dynamic_metadata/src/dynamic/__init__.py|
             tests/packages/.*/setup.py
           )
-        files: ^(src|tests)
+        files: ^(src|tests|noxfile.py)
         args: []
         additional_dependencies:
           - build
           - cattrs
           - cmake
           - exceptiongroup
           - hatch-fancy-pypi-readme
           - importlib-metadata>=6.6.0
           - importlib-resources
           - markdown-it-py<3 # Python 3.7 compat needed for mypy check
           - ninja
+          - nox
           - packaging
           - pyproject_metadata
           - pytest
           - rich
           - setuptools-scm
           - tomli
           - types-setuptools>=67.8
```

### Comparing `scikit_build_core-0.4.6/noxfile.py` & `scikit_build_core-0.4.7/noxfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     session.install("-e.[dev,test,test-meta]", "pylint")
     session.run("pylint", "scikit_build_core", *session.posargs)
 
 
 def _run_tests(
     session: nox.Session,
     *,
-    install_args: Sequence[str],
+    install_args: Sequence[str] = (),
     run_args: Sequence[str] = (),
     extras: Sequence[str] = (),
 ) -> None:
     posargs = list(session.posargs)
     env = {"PIP_DISABLE_PIP_VERSION_CHECK": "1"}
 
     _install_args = list(install_args)
@@ -143,15 +143,15 @@
 @nox.session
 def build(session: nox.Session) -> None:
     """
     Build an SDist and wheel.
     """
 
     session.install("build")
-    session.run("python", "-m", "build", **session.posargs)
+    session.run("python", "-m", "build", *session.posargs)
 
 
 EXAMPLES = ["c", "abi3", "pybind11", "nanobind", "swig", "cython"]
 if not sys.platform.startswith("win") and shutil.which("gfortran"):
     EXAMPLES.append("fortran")
 EXAMPLES = [f"getting_started/{n}" for n in EXAMPLES]
 EXAMPLES += ["downstream/pybind11_example", "downstream/nanobind_example"]
@@ -200,15 +200,15 @@
         session.run("git", "pull", external=True)
     else:
         session.run(
             "git",
             "clone",
             args.project,
             *remaining,
-            proj_dir,
+            str(proj_dir),
             "--recurse-submodules",
             external=True,
         )
         session.chdir(proj_dir)
 
     # Read and strip requirements
     pyproject_toml = Path("pyproject.toml")
```

### Comparing `scikit_build_core-0.4.6/.github/CONTRIBUTING.md` & `scikit_build_core-0.4.7/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/.github/matchers/pylint.json` & `scikit_build_core-0.4.7/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/.github/workflows/cd.yml` & `scikit_build_core-0.4.7/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/.github/workflows/ci.yml` & `scikit_build_core-0.4.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/distro/python-scikit-build-core.spec` & `scikit_build_core-0.4.7/distro/python-scikit-build-core.spec`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 
 License:        Apache-2.0
 URL:            https://github.com/scikit-build/scikit-build-core
 Source:         %{pypi_source scikit_build_core}
 
 BuildArch:      noarch
 BuildRequires:  python3-devel
+# Testing dependences
 BuildRequires:  cmake
 BuildRequires:  ninja-build
 BuildRequires:  gcc
 BuildRequires:  gcc-c++
+BuildRequires:  git
 
 %global _description %{expand:
 A next generation Python CMake adaptor and Python API for plugins
 }
 
 %description %_description
 
@@ -32,15 +34,15 @@
 
 
 %prep
 %autosetup -n scikit_build_core-%{version}
 
 
 %generate_buildrequires
-%pyproject_buildrequires -x test
+%pyproject_buildrequires -x test,test-meta,test-numpy
 
 
 %build
 %pyproject_wheel
 
 
 %install
```

### Comparing `scikit_build_core-0.4.6/docs/changelog.md` & `scikit_build_core-0.4.7/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # Changelog
 
+## Version 0.4.7
+
+This version fixes a unused variable message in 0.4.6, along with a debug
+logging improvement, and a few test fixes, including a regression in the recent
+noxfile reworking.
+
+- fix: remove `SKBUILD_STATE` unused message when building by @henryiii in #401
+- fix: logging environment should use reprs by @henryiii in #409
+
+Tests and CI:
+
+- Support running tests with `NO_COLOR` by @henryiii in #407
+- `noxfile.py` added to mypy, two fixes by @henryiii in #408
+- Get packages of interest from `pyproject.toml` by @henryiii in #402
+- Enable more tests in the spec file by @LecrisUT in #400
+
 ## Version 0.4.6
 
 This release has one small new feature (access to `${SKBUILD_STATE}` from
 CMake), and fixes an issue when adding read-only files on Windows with Python
 3.7. Some testing and docs infrastructure updates should make it easier for
 downstream packagers to ship scikit-build-core.
```

### Comparing `scikit_build_core-0.4.6/docs/cmakelists.md` & `scikit_build_core-0.4.7/docs/cmakelists.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/conf.py` & `scikit_build_core-0.4.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/configuration.md` & `scikit_build_core-0.4.7/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/getting_started.md` & `scikit_build_core-0.4.7/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/index.md` & `scikit_build_core-0.4.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/migration_guide.md` & `scikit_build_core-0.4.7/docs/migration_guide.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.4.7/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.4.7/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.4.7/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.4.7/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.4.7/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/api/scikit_build_core.rst` & `scikit_build_core-0.4.7/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.4.7/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.4.7/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/test.sh` & `scikit_build_core-0.4.7/docs/examples/test.sh`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/CMakeLists.txt` & `scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/LICENSE` & `scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/README.md` & `scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/downstream/nanobind_example/pyproject.toml` & `scikit_build_core-0.4.7/docs/examples/downstream/nanobind_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/LICENSE` & `scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/README.md` & `scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/pyproject.toml` & `scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/downstream/pybind11_example/src/main.cpp` & `scikit_build_core-0.4.7/docs/examples/downstream/pybind11_example/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.4.7/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.4.7/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.4.7/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.4.7/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.4.7/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/_logging.py` & `scikit_build_core-0.4.7/src/scikit_build_core/_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.4.7/src/scikit_build_core/_shutil.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,19 +48,19 @@
         options = [
             os.fspath(arg) if isinstance(arg, os.PathLike) else arg for arg in args
         ]
 
         if self.env:
             if not self._prev_env:
                 type(self)._prev_env = self.env.copy()
-                msg = "\n  ".join(f"{k}={v}" for k, v in sorted(self.env.items()))
+                msg = "\n  ".join(f"{k}={v!r}" for k, v in sorted(self.env.items()))
                 logger.debug("RUNENV:\n  {}", msg)
             else:
                 msg = "\n  ".join(
-                    f"{self._key_diff(k)} {k}={self.env.get(k, '<unset>')}"
+                    f"{self._key_diff(k)} {k}={self.env.get(k, '<unset>')!r}"
                     for k in sorted(self.env.keys() | self._prev_env.keys())
                     if self._prev_env.get(k, None) != self.env.get(k, None)
                 )
                 logger.debug("RUNENV - changes since last run only:\n  {}", msg)
                 type(self)._prev_env = self.env.copy()
 
         logger.debug("RUN: {}", " ".join(options))
```

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/cmake.py` & `scikit_build_core-0.4.7/src/scikit_build_core/cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/errors.py` & `scikit_build_core-0.4.7/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/program_search.py` & `scikit_build_core-0.4.7/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.4.7/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.4.7/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.4.7/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.4.7/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.4.7/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.4.7/src/scikit_build_core/build/_pathutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.4.7/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.4.7/src/scikit_build_core/build/_wheelfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.4.7/src/scikit_build_core/build/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.4.7/src/scikit_build_core/build/wheel.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,16 +193,18 @@
                 if not path.parent.is_dir():
                     path.parent.mkdir(exist_ok=True, parents=True)
                 path.write_bytes(data)
             return WheelImplReturn(wheel_filename=dist_info.name)
 
         rich_print("[green]***[/green] [bold]Configuring CMake...")
         defines: dict[str, str] = {}
-        cache_entries = {f"SKBUILD_{k.upper()}_DIR": v for k, v in wheel_dirs.items()}
-        defines["SKBUILD_STATE"] = action
+        cache_entries: dict[str, str | Path] = {
+            f"SKBUILD_{k.upper()}_DIR": v for k, v in wheel_dirs.items()
+        }
+        cache_entries["SKBUILD_STATE"] = action
         builder.configure(
             defines=defines,
             cache_entries=cache_entries,
             name=metadata.name,
             version=metadata.version,
         )
```

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.4.7/src/scikit_build_core/builder/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,15 @@
     Returns an empty list otherwise or if ARCHFLAGS is not set.
     """
 
     if sys.platform.startswith("darwin"):
         for cmake_arg in cmake_args:
             if "CMAKE_SYSTEM_PROCESSOR" in cmake_arg:
                 return [cmake_arg.split("=")[1]]
-        archs = re.findall(r"-arch (\S+)", env.get("ARCHFLAGS", ""))
-        return archs
+        return re.findall(r"-arch (\S+)", env.get("ARCHFLAGS", ""))
     if sys.platform.startswith("win") and get_platform(env) == "win-arm64":
         return ["win_arm64"]
 
     return []
 
 
 def archs_to_tags(archs: list[str]) -> list[str]:
```

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.4.7/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.4.7/src/scikit_build_core/builder/get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.4.7/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.4.7/src/scikit_build_core/builder/sysconfig.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.4.7/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.4.7/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.4.7/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.4.7/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.4.7/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.4.7/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,19 +29,23 @@
     with Path("pyproject.toml").open("rb") as f:
         pyproject_dict = tomllib.load(f)
 
     config = load_and_validate_config(
         pyproject_dict["tool"]["hatch"]["metadata"]["hooks"]["fancy-pypi-readme"]
     )
 
+    # Version 22.3 does not have fragment support
     return {
         "readme": {
             "content-type": config.content_type,
-            "text": build_text(config.fragments, config.substitutions),
+            "text": build_text(config.fragments, config.substitutions)
+            if hasattr(config, "substitutions")
+            # pylint: disable-next=no-value-for-parameter
+            else build_text(config.fragments),  # type: ignore[call-arg]
         }
     }
 
 
 def get_requires_for_dynamic_metadata(
     _settings: dict[str, object] | None = None,
 ) -> list[str]:
-    return ["hatch-fancy-pypi-readme"]
+    return ["hatch-fancy-pypi-readme>=22.3"]
```

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.4.7/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.4.7/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.4.7/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.4.7/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.4.7/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/settings/metadata.py` & `scikit_build_core-0.4.7/src/scikit_build_core/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.4.7/src/scikit_build_core/settings/skbuild_model.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.4.7/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.4.7/src/scikit_build_core/settings/sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,16 +225,15 @@
                 cls.convert(i.strip(), _get_inner_type(target)) for i in item.split(";")
             ]
         if raw_target == dict:
             items = (i.strip().split("=") for i in item.split(";"))
             return {k: cls.convert(v, _get_inner_type(target)) for k, v in items}
 
         if raw_target is bool:
-            result = item.strip().lower() not in {"0", "false", "off", "no", ""}
-            return result
+            return item.strip().lower() not in {"0", "false", "off", "no", ""}
 
         if callable(raw_target):
             return raw_target(item)
         msg = f"Can't convert target {target}"
         raise TypeError(msg)
 
     def unrecognized_options(
@@ -335,16 +334,15 @@
         if raw_target == dict:
             assert not isinstance(item, (str, list))
             return {k: cls.convert(v, _get_inner_type(target)) for k, v in item.items()}
         if isinstance(item, (list, dict)):
             msg = f"Expected {target}, got {type(item).__name__}"
             raise TypeError(msg)
         if raw_target is bool:
-            result = item.strip().lower() not in {"0", "false", "off", "no", ""}
-            return result
+            return item.strip().lower() not in {"0", "false", "off", "no", ""}
         if callable(raw_target):
             return raw_target(item)
         msg = f"Can't convert target {target}"
         raise TypeError(msg)
 
     def unrecognized_options(self, options: object) -> Generator[str, None, None]:
         if not self.verify:
```

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/setuptools/build_cmake.py` & `scikit_build_core-0.4.7/src/scikit_build_core/setuptools/build_cmake.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import os
 import shutil
 import sys
 from pathlib import Path
+from typing import ClassVar
 
 import setuptools
 import setuptools.errors
 from packaging.version import Version
 from setuptools.dist import Distribution
 
 from .._compat.typing import Literal
@@ -44,15 +45,15 @@
     build_lib: str | None
     build_temp: str | None
     debug: bool | None
     editable_mode: bool
     parallel: int | None
     plat_name: str | None
 
-    user_options = [
+    user_options: ClassVar[list[tuple[str, str, str]]] = [
         ("build-lib=", "b", "directory for compiled extension modules"),
         ("build-temp=", "t", "directory for temporary files (build by-products)"),
         ("plat-name=", "p", "platform name to cross-compile for, if supported "),
         ("debug", "g", "compile/link with debugging information"),
         ("parallel=", "j", "number of parallel build jobs"),
         ("source-dir=", "j", "directory with CMakeLists.txt"),
         ("cmake-args=", "a", "extra arguments for CMake"),
```

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.4.7/src/scikit_build_core/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/src/scikit_build_core/setuptools/wrapper.py` & `scikit_build_core-0.4.7/src/scikit_build_core/setuptools/wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/conftest.py` & `scikit_build_core-0.4.7/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,22 @@
 if sys.version_info < (3, 8):
     import importlib_metadata as metadata
     from typing_extensions import Literal, overload
 else:
     from importlib import metadata
     from typing import Literal, overload
 
+if sys.version_info < (3, 11):
+    import tomli as tomllib
+else:
+    import tomllib
+
+
 import pytest
+from packaging.requirements import Requirement
 
 DIR = Path(__file__).parent.resolve()
 BASE = DIR.parent
 
 
 @pytest.fixture(scope="session")
 def pep518_wheelhouse(tmp_path_factory: pytest.TempPathFactory) -> Path:
@@ -297,28 +304,27 @@
         if "isolated" in getattr(item, "fixturenames", ()):
             item.add_marker(pytest.mark.virtualenv)
             item.add_marker(pytest.mark.isolated)
             item.add_marker(pytest.mark.network)
 
 
 def pytest_report_header() -> str:
-    interesting_packages = [
-        "build",
-        "packaging",
-        "pathspec",
-        "pip",
-        "pybind11",
-        "pyproject_metadata",
-        "scikit_build_core",
-        "setuptools",
-        "virtualenv",
-        "wheel",
-    ]
+    with BASE.joinpath("pyproject.toml").open("rb") as f:
+        pyproject = tomllib.load(f)
+    project = pyproject.get("project", {})
+
+    pkgs = project.get("dependencies", [])
+    pkgs += [p for ps in project.get("optional-dependencies", {}).values() for p in ps]
+    if "name" in project:
+        pkgs.append(project["name"])
+    interesting_packages = {Requirement(p).name for p in pkgs}
+    interesting_packages.add("pip")
+
     valid = []
-    for package in interesting_packages:
+    for package in sorted(interesting_packages):
         with contextlib.suppress(ModuleNotFoundError):
             valid.append(f"{package}=={metadata.version(package)}")
     reqs = " ".join(valid)
     lines = [
         f"installed packages of interest: {reqs}",
         f"sysconfig platform: {sysconfig.get_platform()}",
     ]
```

### Comparing `scikit_build_core-0.4.6/tests/test_builder.py` & `scikit_build_core-0.4.7/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_cmake_config.py` & `scikit_build_core-0.4.7/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_custom_modules.py` & `scikit_build_core-0.4.7/tests/test_custom_modules.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_dynamic_metadata.py` & `scikit_build_core-0.4.7/tests/test_dynamic_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
     assert str(metadata.version) == "0.1.0"
     assert metadata.readme == pyproject_metadata.Readme(
         "Fragment #1Fragment #2", None, "text/x-rst"
     )
 
     assert set(GetRequires().dynamic_metadata()) == {
-        "hatch-fancy-pypi-readme",
+        "hatch-fancy-pypi-readme>=22.3",
         "setuptools-scm",
     }
 
 
 @pytest.mark.usefixtures("package_dynamic_metadata")
 def test_faulty_metadata():
     with Path("faulty_project.toml").open("rb") as ft:
```

### Comparing `scikit_build_core-0.4.6/tests/test_file_processor.py` & `scikit_build_core-0.4.7/tests/test_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_fileapi.py` & `scikit_build_core-0.4.7/tests/test_fileapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     assert len(index.objects) == 4
 
     codemodel = index.reply.codemodel_v2
     assert codemodel is not None
     assert codemodel.kind == "codemodel"
     assert codemodel.version.major == 2
     assert codemodel.version.minor == 4
-    assert codemodel.configurations[0].name == ""  # noqa: PLC1901
+    assert codemodel.configurations[0].name == ""
 
     cache = index.reply.cache_v2
     assert cache is not None
 
     cmakefiles = index.reply.cmakefiles_v1
     assert cmakefiles is not None
```

### Comparing `scikit_build_core-0.4.6/tests/test_fortran.py` & `scikit_build_core-0.4.7/tests/test_fortran.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_generator_default.py` & `scikit_build_core-0.4.7/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_get_requires.py` & `scikit_build_core-0.4.7/tests/test_get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_module_dir.py` & `scikit_build_core-0.4.7/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_name_main.py` & `scikit_build_core-0.4.7/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_prepare_metadata.py` & `scikit_build_core-0.4.7/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_process_scripts.py` & `scikit_build_core-0.4.7/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_program_search.py` & `scikit_build_core-0.4.7/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_pyproject_abi3.py` & `scikit_build_core-0.4.7/tests/test_pyproject_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.4.7/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_pyproject_pep517.py` & `scikit_build_core-0.4.7/tests/test_pyproject_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_pyproject_pep518.py` & `scikit_build_core-0.4.7/tests/test_pyproject_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_pyproject_pep660.py` & `scikit_build_core-0.4.7/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_settings.py` & `scikit_build_core-0.4.7/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_setuptools_abi3.py` & `scikit_build_core-0.4.7/tests/test_setuptools_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_setuptools_pep517.py` & `scikit_build_core-0.4.7/tests/test_setuptools_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_setuptools_pep518.py` & `scikit_build_core-0.4.7/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_shutil.py` & `scikit_build_core-0.4.7/tests/test_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_simple_pure.py` & `scikit_build_core-0.4.7/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_simplest_c.py` & `scikit_build_core-0.4.7/tests/test_simplest_c.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_skbuild_settings.py` & `scikit_build_core-0.4.7/tests/test_skbuild_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/test_wheelfile_utils.py` & `scikit_build_core-0.4.7/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.4.7/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.4.7/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.4.7/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.4.7/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.4.7/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.4.7/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.4.7/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/mixed_setuptools/CMakeLists.txt` & `scikit_build_core-0.4.7/tests/packages/mixed_setuptools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/LICENSE` & `scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.4.7/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/LICENSE` & `scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/simple_pyproject_source_dir/src/main.cpp` & `scikit_build_core-0.4.7/tests/packages/simple_pyproject_source_dir/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/LICENSE` & `scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.4.7/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.4.7/tests/packages/simplest_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.4.7/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/.gitignore` & `scikit_build_core-0.4.7/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/LICENSE` & `scikit_build_core-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/README.md` & `scikit_build_core-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.4.6/pyproject.toml` & `scikit_build_core-0.4.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,43 +30,42 @@
     "Typing :: Typed",
 ]
 
 dynamic = ["version"]
 
 dependencies = [
     "exceptiongroup; python_version<'3.11'",
-    "importlib-resources >=1.3; python_version<'3.9'",
     "importlib-metadata; python_version<'3.8'",
+    "importlib-resources >=1.3; python_version<'3.9'",
     "packaging >=20.9",
     "tomli >=1.1; python_version<'3.11'",
     "typing-extensions >=3.10.0; python_version<'3.8'",
 ]
 # Note: for building wheels and sdists, there are also additional dependencies
 # in the pyproject extra. And cmake and possibly ninja if those are not already
 # present (user controllable)
 
 [project.optional-dependencies]
 pyproject = [
-    "pyproject-metadata >=0.5",
     "pathspec >=0.10.1",
+    "pyproject-metadata >=0.5",
 ]
 test = [
     "build[virtualenv]",
     "cattrs >=22.2.0",
-    "importlib-metadata; python_version<'3.8'",
     "pathspec >=0.10.1",
     "pybind11",
     "pyproject-metadata >=0.5",
     "pytest >=7.0",  # 7.2+ recommended for better tracebacks with ExceptionGroup
     "pytest-subprocess >=1.5",
     "setuptools",
     "wheel",
 ]
 test-meta = [
-    "hatch-fancy-pypi-readme",
+    "hatch-fancy-pypi-readme>=22.3",
     "setuptools-scm",
 ]
 test-numpy = [
     "numpy; python_version<'3.12' and platform_python_implementation!='PyPy'",
     "numpy~=1.21.0; python_version=='3.7' and platform_python_implementation=='PyPy' and sys_platform == 'linux'",
     "numpy~=1.24.0; python_version=='3.8' and platform_python_implementation=='PyPy'",
     "numpy~=1.25.0; python_version=='3.9' and platform_python_implementation=='PyPy'",
@@ -88,19 +87,19 @@
     "pyproject-metadata >=0.5",
     "sphinx >=4.0",
     "sphinx-copybutton",
     "sphinx-inline-tabs",
 ]
 
 [project.urls]
-Homepage = "https://github.com/scikit-build/scikit-build-core"
-Documentation = "https://scikit-build-core.readthedocs.io"
+Changelog = "https://scikit-build-core.readthedocs.io/en/latest/changelog.html"
 Discussions = "https://github.com/orgs/scikit-build/discussions"
+Documentation = "https://scikit-build-core.readthedocs.io"
+Homepage = "https://github.com/scikit-build/scikit-build-core"
 Issues = "https://github.com/scikit-build/scikit-build-core/issues"
-Changelog = "https://scikit-build-core.readthedocs.io/en/latest/changelog.html"
 
 [project.entry-points]
 "distutils.commands".build_cmake = "scikit_build_core.setuptools.build_cmake:BuildCMake"
 "distutils.setup_keywords".cmake_source_dir = "scikit_build_core.setuptools.build_cmake:cmake_source_dir"
 "distutils.setup_keywords".cmake_args = "scikit_build_core.setuptools.build_cmake:cmake_args"
 "setuptools.finalize_distribution_options".scikit_build_entry = "scikit_build_core.setuptools.build_cmake:finalize_distribution_options"
 
@@ -111,18 +110,17 @@
 
 [tool.pytest.ini_options]
 minversion = "7.0"
 addopts = ["-ra", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = [
     "error",
-    "ignore:pkg_resources is deprecated as an API:DeprecationWarning",  # Caused by wheel in tests
+    "ignore:pkg_resources is deprecated as an API:DeprecationWarning:wheel",  # Caused by wheel in tests
     "ignore:Config variable '.*' is unset, Python ABI tag may be incorrect:RuntimeWarning",
-    "ignore:onerror argument is deprecated, use onexc instead:DeprecationWarning",  # Caused by wheel and Python 3.12
-    "ignore:(ast.Str|Attribute s|ast.NameConstant|ast.Num) is deprecated:DeprecationWarning:_pytest",  # Python 3.12
+    "ignore:onerror argument is deprecated, use onexc instead:DeprecationWarning:wheel",  # Caused by wheel and Python 3.12
 ]
 log_cli_level = "info"
 testpaths = ["tests"]
 markers = [
     "broken_on_urct: Broken for now due to lib not found",
     "compile: Compiles code",
     "configure: Configures CMake code",
@@ -132,15 +130,15 @@
     "network: Needs a network connection to setup or run",
     "setuptools: Tests setuptools integration",
     "virtualenv: Needs a virtualenv",
 ]
 
 
 [tool.mypy]
-files = ["src", "tests"]
+files = ["src", "tests", "noxfile.py"]
 mypy_path = ["$MYPY_CONFIG_FILE_DIR/src"]
 python_version = "3.7"
 warn_unused_configs = true
 show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 strict = true
 disallow_untyped_defs = false
```

### Comparing `scikit_build_core-0.4.6/PKG-INFO` & `scikit_build_core-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scikit_build_core
-Version: 0.4.6
+Version: 0.4.7
 Summary: Build backend for CMake based projects
-Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
-Project-URL: Documentation, https://scikit-build-core.readthedocs.io
+Project-URL: Changelog, https://scikit-build-core.readthedocs.io/en/latest/changelog.html
 Project-URL: Discussions, https://github.com/orgs/scikit-build/discussions
+Project-URL: Documentation, https://scikit-build-core.readthedocs.io
+Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Issues, https://github.com/scikit-build/scikit-build-core/issues
-Project-URL: Changelog, https://scikit-build-core.readthedocs.io/en/latest/changelog.html
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -47,24 +47,23 @@
 Requires-Dist: sphinx>=4.0; extra == 'docs'
 Provides-Extra: pyproject
 Requires-Dist: pathspec>=0.10.1; extra == 'pyproject'
 Requires-Dist: pyproject-metadata>=0.5; extra == 'pyproject'
 Provides-Extra: test
 Requires-Dist: build[virtualenv]; extra == 'test'
 Requires-Dist: cattrs>=22.2.0; extra == 'test'
-Requires-Dist: importlib-metadata; python_version < '3.8' and extra == 'test'
 Requires-Dist: pathspec>=0.10.1; extra == 'test'
 Requires-Dist: pybind11; extra == 'test'
 Requires-Dist: pyproject-metadata>=0.5; extra == 'test'
 Requires-Dist: pytest-subprocess>=1.5; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
 Requires-Dist: setuptools; extra == 'test'
 Requires-Dist: wheel; extra == 'test'
 Provides-Extra: test-meta
-Requires-Dist: hatch-fancy-pypi-readme; extra == 'test-meta'
+Requires-Dist: hatch-fancy-pypi-readme>=22.3; extra == 'test-meta'
 Requires-Dist: setuptools-scm; extra == 'test-meta'
 Provides-Extra: test-numpy
 Requires-Dist: numpy; python_version < '3.12' and platform_python_implementation != 'PyPy' and extra == 'test-numpy'
 Requires-Dist: numpy~=1.21.0; python_version == '3.7' and platform_python_implementation == 'PyPy' and sys_platform == 'linux' and extra == 'test-numpy'
 Requires-Dist: numpy~=1.24.0; python_version == '3.8' and platform_python_implementation == 'PyPy' and extra == 'test-numpy'
 Requires-Dist: numpy~=1.25.0; python_version == '3.9' and platform_python_implementation == 'PyPy' and extra == 'test-numpy'
 Provides-Extra: wheels
```

