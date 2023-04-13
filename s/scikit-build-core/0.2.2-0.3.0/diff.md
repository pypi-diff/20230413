# Comparing `tmp/scikit_build_core-0.2.2.tar.gz` & `tmp/scikit_build_core-0.3.0.tar.gz`

## Comparing `scikit_build_core-0.2.2.tar` & `scikit_build_core-0.3.0.tar`

### file list

```diff
@@ -1,150 +1,215 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/.gitattributes
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/.readthedocs.yml
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/noxfile.py
--rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     9753 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/changelog.md
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/conf.py
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/getting_started.md
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/index.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/_compat/importlib.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0     4013 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0     7947 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198527 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0    15158 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/src/scikit_build_core/setuptools/extension.py
--rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/conftest.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/constraints.txt
--rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_builder.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_cmake_config.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_fileapi.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_generator_default.py
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_get_requires.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_name_main.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_program_search.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     7443 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0    13859 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_settings.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_simple_pure.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_simplest_c.py
--rw-r--r--   0        0        0    10892 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/LICENSE
--rw-r--r--   0        0        0     9071 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/README.md
--rw-r--r--   0        0        0     5602 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    11754 2020-02-02 00:00:00.000000 scikit_build_core-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.gitattributes
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.packit.yaml
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.readthedocs.yml
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/noxfile.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.distro/scikit-build-core.spec
+-rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/changelog.md
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/cmakelists.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/configuration.md
+-rw-r--r--   0        0        0     9065 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/getting_started.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/index.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/metadata.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/setuptools/extension.py
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/constraints.txt
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_builder.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_fileapi.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_generator_default.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_get_requires.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_logging.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_name_main.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_program_search.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_settings.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/LICENSE
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/README.md
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12297 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/PKG-INFO
```

### Comparing `scikit_build_core-0.2.2/.pre-commit-config.yaml` & `scikit_build_core-0.3.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -25,23 +25,23 @@
     rev: v1.10.0
     hooks:
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/asottile/blacken-docs
     rev: 1.13.0
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==23.1.0]
+        additional_dependencies: [black==23.3.0]
 
   - repo: https://github.com/cheshirekow/cmake-format-precommit
     rev: v0.6.13
     hooks:
       - id: cmake-format
         exclude: ^src/scikit_build_core/resources/find_python
 
@@ -50,41 +50,57 @@
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: "^tests"
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.256
+    rev: v0.0.261
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.2.0
     hooks:
       - id: mypy
-        exclude: tests/packages/(simplest_c/src/simplest/__init__.py|.*/setup.py)
+        exclude: |
+          (?x)^(
+            tests/packages/simplest_c/src/simplest/__init__.py|
+            tests/packages/dynamic_metadata/src/dynamic/__init__.py|
+            tests/packages/.*/setup.py
+          )
         files: ^(src|tests)
         args: []
         additional_dependencies:
           - build
           - cattrs
           - cmake
           - exceptiongroup
-          - importlib_metadata
+          - hatch-fancy-pypi-readme
+          - importlib-metadata
           - importlib_resources
           - ninja
           - packaging
           - pyproject_metadata
           - pytest
           - rich
+          - setuptools-scm
           - tomli
-          - types-setuptools
-          - typing_extensions >=4; python_version<'3.11'
+          - types-setuptools>=67.6.0.5
+          - typing_extensions>=4;python_version<'3.11'
+
+  - repo: https://github.com/henryiii/check-sdist
+    rev: "v0.1.0"
+    hooks:
+      - id: check-sdist
+        args: [--inject-junk]
+        additional_dependencies:
+          - hatchling
+          - hatch-vcs
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.4
     hooks:
       - id: codespell
         exclude: ^(LICENSE$|src/scikit_build_core/resources/find_python)
```

### Comparing `scikit_build_core-0.2.2/noxfile.py` & `scikit_build_core-0.3.0/noxfile.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import argparse
 import shutil
+import sys
 from pathlib import Path
 
 import nox
 
 DIR = Path(__file__).parent.resolve()
 
 nox.options.sessions = ["lint", "pylint", "tests"]
@@ -23,46 +24,42 @@
 @nox.session(reuse_venv=True)
 def pylint(session: nox.Session) -> None:
     """
     Run PyLint.
     """
     # This needs to be installed into the package environment, and is slower
     # than a pre-commit check
-    session.install("-e.[dev,test]", "pylint")
+    session.install(
+        "-e.[dev,test]", "pylint", "hatch-fancy-pypi-readme", "setuptools-scm"
+    )
     session.run("pylint", "scikit_build_core", *session.posargs)
 
 
 @nox.session(reuse_venv=True)
 def tests(session: nox.Session) -> None:
     """
-    Run the unit and regular tests.
+    Run the unit and regular tests. Includes coverage if --cov passed.
     """
+    posargs = list(session.posargs)
     env = {"PIP_DISABLE_PIP_VERSION_CHECK": "1"}
-    extra = ["rich"]
+    extra = ["hatch-fancy-pypi-readme", "rich", "setuptools-scm"]
     # This will not work if system CMake is too old (<3.15)
     if shutil.which("cmake") is None and shutil.which("cmake3") is None:
         extra.append("cmake")
     if shutil.which("ninja") is None:
         extra.append("ninja")
+    if (3, 8) <= sys.version_info < (3, 12):
+        extra.append("numpy")
 
-    session.install("-e.[test]", *extra)
-    session.run("pytest", *session.posargs, env=env)
+    install_arg = "-e.[test,cov]" if "--cov" in posargs else "-e.[test]"
+    session.install(install_arg, *extra)
+    session.run("pytest", *posargs, env=env)
 
 
 @nox.session(reuse_venv=True)
-def coverage(session: nox.Session) -> None:
-    """
-    Run coverage and report.
-    """
-
-    session.install("-e.[test,cov]")
-    session.run("pytest", "--cov=scikit_build_core", *session.posargs)
-
-
-@nox.session
 def docs(session: nox.Session) -> None:
     """
     Build the docs. Pass "--serve" to serve.
     """
 
     parser = argparse.ArgumentParser()
     parser.add_argument("--serve", action="store_true", help="Serve after building")
@@ -100,7 +97,20 @@
 def build(session: nox.Session) -> None:
     """
     Build an SDist and wheel.
     """
 
     session.install("build")
     session.run("python", "-m", "build", **session.posargs)
+
+
+EXAMPLES = ["c", "abi3", "pybind11", "swig", "cython"]
+if not sys.platform.startswith("win") and shutil.which("gfortran"):
+    EXAMPLES.append("fortran")
+
+
+@nox.session
+@nox.parametrize("example", EXAMPLES, ids=EXAMPLES)
+def test_doc_examples(session: nox.Session, example: str) -> None:
+    session.chdir(f"docs/examples/getting_started/{example}")
+    session.install(".", "--config-settings=cmake.verbose=true")
+    session.run("python", "../test.py")
```

### Comparing `scikit_build_core-0.2.2/.github/matchers/pylint.json` & `scikit_build_core-0.3.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/.github/workflows/cd.yml` & `scikit_build_core-0.3.0/.github/workflows/cd.yml`

 * *Files 22% similar despite different names*

```diff
@@ -20,11 +20,11 @@
       - name: Build package
         run: pipx run build
 
       - uses: actions/upload-artifact@v3
         with:
           path: dist/*
 
-      - uses: pypa/gh-action-pypi-publish@v1.8.1
+      - uses: pypa/gh-action-pypi-publish@v1.8.5
         if: github.event_name == 'release' && github.event.action == 'published'
         with:
           password: ${{ secrets.pypi_password }}
```

### Comparing `scikit_build_core-0.2.2/docs/changelog.md` & `scikit_build_core-0.3.0/docs/changelog.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,60 @@
 # Changelog
 
+## Version 0.3.0
+
+This version brings two new dynamic metadata plugins (wrappers for
+`setuptools_scm` & `hatch-pypi-fancy-readme`). Third-party packages can now add
+entry-points declaring `CMAKE_PREFIX_DIR` and `CMAKE_MODULE_DIR` entries.
+Support has been added for requesting metadata without building. And
+experimental support was added for editable installs, including an option for
+automatic rebuilds.
+
+Several fixes have been added as well, like SABI support, ARM cross-compiling
+support for FindPython, scripts entries now process shebang lines, and setting a
+`build-dir` with `{wheel_tag}` was not working before. The docs have been
+started, with a quickstart for common situations, a page on configuration, and
+some info on authoring a CMakeLists.
+
+### What's Changed
+
+Features:
+
+- Support dynamic metadata by @bennyrowland in #197 and rework by @henryiii in
+  #251
+- Support modules/prefix dirs by @henryiii in #255
+- Add `get_requires_for_dynamic_metadata` by @henryiii in #235
+- Make setuptools wrapper more generic by @henryiii in #225
+- Experimental support for editable installs by @henryiii in #212, #268, and
+  #271
+
+Fixes:
+
+- CMake 3.26.0 (exactly) needs the backport too by @henryiii in #238
+- Add python library artifact for better Windows cross compiling by @henryiii in
+  #263
+- Include 3.26.1 SABI fix by @henryiii in #227
+- Restructure `get_requires` & fix some ninja paths by @henryiii in #250
+- Support script rewriting by @henryiii in #254
+- Version not a string (typing updates) by @henryiii in #231
+- `{wheel_tag}` was not working by @henryiii in #262
+- `CMAKE_PREFIX_DIR` and `CMAKE_MODULE_DIR` are passed in the init cache file to
+  remove a unused variable warning by @henryiii in #272
+- Support color printouts without Rich (pip requires `FORCE_COLOR`) by @henryiii
+  in #266
+
+Other things:
+
+- Add Fortran testing and CI by @henryiii in #86
+- Avoid internet usage in non-isolated testing by @henryiii in #247
+- Add an SDist checker & fix contents by @henryiii in #253
+- Add more setuptools types by @henryiii in #233
+- Add FedoraProject rpm spec file by @LecrisUT in #201 and #241
+- Better coverage handling by @henryiii in #270
+
 ## Version 0.2.2
 
 This release makes a small improvement to the wheel file permissions (in line
 with wheel 0.40). It also ensures the test suite will still pass in an
 environment with `SOURCE_DATE_EPOCH` already set. A few internal changes are
 paving the way to 0.3.0.
```

### Comparing `scikit_build_core-0.2.2/docs/conf.py` & `scikit_build_core-0.3.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # ones.
 extensions = [
     "myst_parser",
     "sphinx.ext.autodoc",
     "sphinx.ext.mathjax",
     "sphinx.ext.napoleon",
     "sphinx_copybutton",
+    "sphinx_inline_tabs",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = []
 
 source_suffix = [".rst", ".md"]
```

### Comparing `scikit_build_core-0.2.2/docs/index.md` & `scikit_build_core-0.3.0/docs/index.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 ```{toctree}
 :maxdepth: 2
 :titlesonly:
 :caption: Guide
 :glob:
 
 getting_started
+configuration
+cmakelists
 changelog
 ```
 
 ```{toctree}
 :maxdepth: 1
 :titlesonly:
 :caption: API docs
```

### Comparing `scikit_build_core-0.2.2/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.3.0/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.3.0/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.3.0/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.3.0/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/docs/api/scikit_build_core.rst` & `scikit_build_core-0.3.0/docs/api/scikit_build_core.rst`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 .. toctree::
    :maxdepth: 4
 
    scikit_build_core.build
    scikit_build_core.builder
    scikit_build_core.file_api
+   scikit_build_core.metadata
    scikit_build_core.resources
    scikit_build_core.settings
    scikit_build_core.setuptools
 
 Submodules
 ----------
```

### Comparing `scikit_build_core-0.2.2/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.3.0/docs/api/scikit_build_core.settings.rst`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,22 @@
    :members:
    :undoc-members:
    :show-inheritance:
 
 Submodules
 ----------
 
+scikit\_build\_core.settings.metadata module
+--------------------------------------------
+
+.. automodule:: scikit_build_core.settings.metadata
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 scikit\_build\_core.settings.skbuild\_model module
 --------------------------------------------------
 
 .. automodule:: scikit_build_core.settings.skbuild_model
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `scikit_build_core-0.2.2/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.3.0/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/_logging.py` & `scikit_build_core-0.3.0/src/scikit_build_core/_logging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
+import contextlib
 import logging
+import os
 import re
 import sys
 import typing
 from typing import Any
 
 __all__ = ["logger", "raw_logger", "ScikitBuildLogger", "rich_print"]
 
@@ -74,23 +76,66 @@
     def addHandler(self, handler: logging.Handler) -> None:
         self.logger.addHandler(handler)
 
 
 logger = ScikitBuildLogger(raw_logger)
 
 
-def _strip_rich(msg: object) -> object:
-    if isinstance(msg, str):
-        return re.sub(r"\[.*?\]", "", msg)
-    return msg
+ANY_ESCAPE = re.compile(r"\[([\w\s/]*)\]")
+
+
+_COLORS = {
+    "red": "\33[91m",
+    "green": "\33[92m",
+    "yellow": "\33[93m",
+    "blue": "\33[94m",
+    "magenta": "\33[95m",
+    "cyan": "\33[96m",
+    "bold": "\33[1m",
+    "/red": "\33[0m",
+    "/green": "\33[0m",
+    "/blue": "\33[0m",
+    "/yellow": "\33[0m",
+    "/magenta": "\33[0m",
+    "/cyan": "\33[0m",
+    "/bold": "\33[22m",
+    "reset": "\33[0m",
+}
+_NO_COLORS = {color: "" for color in _COLORS}
+
+
+def colors() -> dict[str, str]:
+    if "NO_COLOR" in os.environ:
+        return _NO_COLORS
+    # Pip reroutes sys.stdout, so FORCE_COLOR is required there
+    if os.environ.get("FORCE_COLOR", ""):
+        return _COLORS
+    # Avoid ValueError: I/O operation on closed file
+    with contextlib.suppress(ValueError):
+        # Assume sys.stderr is similar to sys.stdout
+        isatty = sys.stdout.isatty()
+        if isatty and not sys.platform.startswith("win"):
+            return _COLORS
+    return _NO_COLORS
+
+
+def _process_rich(msg: object) -> str:
+    return ANY_ESCAPE.sub(
+        lambda m: "".join(colors()[x] for x in m.group(1).split()),
+        str(msg),
+    )
 
 
 def fake_rich_print(*args: object, **kwargs: object) -> None:
-    args_2 = (_strip_rich(arg) for arg in args)
+    args_2 = tuple(_process_rich(arg) for arg in args)
+    if args != args_2:
+        args_2 = (*args_2[:-1], args_2[-1] + colors()["reset"])
     print(*args_2, **kwargs)  # type: ignore[call-overload] # noqa: T201
 
 
-try:
-    from rich import print as rich_print
-except ModuleNotFoundError:
-    if not typing.TYPE_CHECKING:
+if typing.TYPE_CHECKING:
+    rich_print = fake_rich_print
+else:
+    try:
+        from rich import print as rich_print
+    except ModuleNotFoundError:
         rich_print = fake_rich_print
```

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.3.0/src/scikit_build_core/_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/cmake.py` & `scikit_build_core-0.3.0/src/scikit_build_core/cmake.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,32 @@
                     f.write(f'set({key} {str_value} CACHE BOOL "" FORCE)\n')
                 elif isinstance(value, os.PathLike):
                     # Convert to CMake's internal path format
                     str_value = str(value).replace("\\", "/")
                     f.write(f'set({key} [===[{str_value}]===] CACHE PATH "" FORCE)\n')
                 else:
                     f.write(f'set({key} [===[{value}]===] CACHE STRING "" FORCE)\n')
+
+            if self.module_dirs:
+                # Convert to CMake's internal path format, otherwise this breaks try_compile on Windows
+                module_dirs_str = ";".join(map(str, self.module_dirs)).replace(
+                    "\\", "/"
+                )
+                f.write(
+                    f'set(CMAKE_MODULE_PATH [===[{module_dirs_str}]===] CACHE PATH "" FORCE)\n'
+                )
+
+            if self.prefix_dirs:
+                prefix_dirs_str = ";".join(map(str, self.prefix_dirs)).replace(
+                    "\\", "/"
+                )
+                f.write(
+                    f'set(CMAKE_PREFIX_PATH [===[{prefix_dirs_str}]===] CACHE PATH "" FORCE)\n'
+                )
+
         contents = self.init_cache_file.read_text(encoding="utf-8").strip()
         logger.debug(
             "{}:\n{}",
             self.init_cache_file,
             textwrap.indent(contents.strip(), "  "),
         )
 
@@ -144,35 +162,26 @@
         yield f"-S{self.source_dir}"
         yield f"-B{self.build_dir}"
 
         if self.init_cache_file.is_file():
             yield f"-C{self.init_cache_file}"
 
         if self.single_config and self.build_type:
-            yield f"-DCMAKE_BUILD_TYPE={self.build_type}"
+            yield f"-DCMAKE_BUILD_TYPE:STRING={self.build_type}"
 
         for key, value in defines.items():
             if isinstance(value, bool):
                 str_value = "ON" if value else "OFF"
                 yield f"-D{key}:BOOL={str_value}"
             elif isinstance(value, os.PathLike):
                 str_value = str(value).replace("\\", "/")
                 yield f"-D{key}:PATH={str_value}"
             else:
                 yield f"-D{key}={value}"
 
-        if self.module_dirs:
-            # Convert to CMake's internal path format, otherwise this breaks try_compile on Windows
-            module_dirs_str = ";".join(map(str, self.module_dirs)).replace("\\", "/")
-            yield f"-DCMAKE_MODULE_PATH:PATH={module_dirs_str}"
-
-        if self.prefix_dirs:
-            prefix_dirs_str = ";".join(map(str, self.prefix_dirs)).replace("\\", "/")
-            yield f"-DCMAKE_PREFIX_PATH:PATH={prefix_dirs_str}"
-
     def configure(
         self,
         *,
         defines: Mapping[str, str | os.PathLike[str] | bool] | None = None,
         cmake_args: Sequence[str] = (),
     ) -> None:
         if "CMAKE_GENERATOR" in self.env:
```

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/errors.py` & `scikit_build_core-0.3.0/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/program_search.py` & `scikit_build_core-0.3.0/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.3.0/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.3.0/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.3.0/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.3.0/src/scikit_build_core/build/_wheelfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.3.0/src/scikit_build_core/build/sdist.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import copy
 import gzip
 import io
 import os
 import tarfile
 from pathlib import Path
 
-from pyproject_metadata import StandardMetadata
-
 from .._compat import tomllib
+from ..settings.metadata import get_standard_metadata
 from ..settings.skbuild_read_settings import SettingsReader
 from ._file_processor import each_unignored_file
 from ._init import setup_logging
 
 __all__: list[str] = ["build_sdist"]
 
 
@@ -65,31 +64,31 @@
     return tar_info
 
 
 def build_sdist(
     sdist_directory: str,
     config_settings: dict[str, list[str] | str] | None = None,
 ) -> str:
-    settings_reader = SettingsReader.from_file("pyproject.toml", config_settings)
+    with Path("pyproject.toml").open("rb") as f:
+        pyproject = tomllib.load(f)
+
+    settings_reader = SettingsReader(pyproject, config_settings or {})
     settings = settings_reader.settings
     setup_logging(settings.logging.level)
 
     settings_reader.validate_may_exit()
 
     sdist_dir = Path(sdist_directory)
 
-    with Path("pyproject.toml").open("rb") as f:
-        pyproject = tomllib.load(f)
-
     reproducible = settings.sdist.reproducible
     timestamp = get_reproducible_epoch() if reproducible else None
 
+    metadata = get_standard_metadata(pyproject, settings)
     # Using deepcopy here because of a bug in pyproject-metadata
     # https://github.com/FFY00/python-pyproject-metadata/pull/49
-    metadata = StandardMetadata.from_pyproject(pyproject)
     pkg_info = bytes(copy.deepcopy(metadata).as_rfc822())
 
     srcdirname = f"{metadata.name}-{metadata.version}"
     filename = f"{srcdirname}.tar.gz"
 
     sdist_dir.mkdir(parents=True, exist_ok=True)
     with contextlib.ExitStack() as stack:
```

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.3.0/src/scikit_build_core/build/wheel.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,35 +5,41 @@
 import shutil
 import sys
 import tempfile
 from collections.abc import Sequence
 from pathlib import Path
 
 from packaging.version import Version
-from pyproject_metadata import StandardMetadata
 
 from .. import __version__
 from .._compat import tomllib
 from .._logging import logger, rich_print
 from ..builder.builder import Builder, archs_to_tags, get_archs
 from ..builder.wheel_tag import WheelTag
 from ..cmake import CMake, CMaker
+from ..resources import resources
+from ..settings.metadata import get_standard_metadata
 from ..settings.skbuild_read_settings import SettingsReader
 from ._init import setup_logging
-from ._pathutil import packages_to_file_mapping
+from ._pathutil import packages_to_file_mapping, path_to_module, scantree
+from ._scripts import process_script_dir
 from ._wheelfile import WheelWriter
 
 __all__: list[str] = ["_build_wheel_impl"]
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
-def _get_packages(*, packages: Sequence[str] | None, name: str) -> list[str]:
+def _get_packages(
+    *,
+    packages: Sequence[str] | None,
+    name: str,
+) -> list[str]:
     if packages is not None:
         return list(packages)
 
     # Auto package discovery
     packages = []
     for base_path in (Path("src"), Path(".")):
         path = base_path / name
@@ -55,28 +61,31 @@
     mapping: dict[str, str] = dataclasses.field(default_factory=dict)
 
 
 def _build_wheel_impl(
     wheel_directory: str | None,
     config_settings: dict[str, list[str] | str] | None,
     metadata_directory: str | None,
+    *,
+    editable: bool,
 ) -> WheelImplReturn:
     """
-    Build a wheel or just prepare metadata (if wheel dir is None).
+    Build a wheel or just prepare metadata (if wheel dir is None). Can be editable.
     """
+    pyproject_path = Path("pyproject.toml")
+    with pyproject_path.open("rb") as ft:
+        pyproject = tomllib.load(ft)
 
-    settings_reader = SettingsReader.from_file("pyproject.toml", config_settings)
+    settings_reader = SettingsReader(pyproject, config_settings or {})
     settings = settings_reader.settings
     setup_logging(settings.logging.level)
 
     settings_reader.validate_may_exit()
 
-    with Path("pyproject.toml").open("rb") as ft:
-        pyproject = tomllib.load(ft)
-    metadata = StandardMetadata.from_pyproject(pyproject)
+    metadata = get_standard_metadata(pyproject, settings)
 
     if metadata.version is None:
         msg = "project.version is not statically specified, must be present currently"
         raise AssertionError(msg)
 
     normalized_name = metadata.name.replace("-", "_").replace(".", "_")
 
@@ -96,16 +105,18 @@
             settings.wheel.py_api,
             expand_macos=settings.wheel.expand_macos_universal_tags,
         )
 
         # A build dir can be specified, otherwise use a temporary directory
         build_dir = (
             Path(
-                settings.build_dir.format(cache_tag=sys.implementation.cache_tag),
-                wheel_tag=str(tags),
+                settings.build_dir.format(
+                    cache_tag=sys.implementation.cache_tag,
+                    wheel_tag=str(tags),
+                )
             )
             if settings.build_dir
             else build_tmp_folder / "build"
         )
         logger.info("Build directory: {}", build_dir.resolve())
 
         wheel_dirs = {
@@ -145,23 +156,21 @@
             config=config,
         )
 
         if wheel_directory is None:
             if metadata_directory is None:
                 msg = "metadata_directory must be specified if wheel_directory is None"
                 raise AssertionError(msg)
-            with WheelWriter(
-                metadata, Path(metadata_directory), tags.as_tags_set()
-            ) as wheel:
-                dist_info_contents = wheel.dist_info_contents()
-                dist_info = Path(metadata_directory) / f"{wheel.name_ver}.dist-info"
-                dist_info.mkdir(parents=True)
-                for key, data in dist_info_contents.items():
-                    path = dist_info / key
-                    path.write_bytes(data)
+            wheel = WheelWriter(metadata, Path(metadata_directory), tags.as_tags_set())
+            dist_info_contents = wheel.dist_info_contents()
+            dist_info = Path(metadata_directory) / f"{wheel.name_ver}.dist-info"
+            dist_info.mkdir(parents=True)
+            for key, data in dist_info_contents.items():
+                path = dist_info / key
+                path.write_bytes(data)
             return WheelImplReturn(wheel_filename=dist_info.name)
 
         rich_print("[green]***[/green] [bold]Configurating CMake...")
         defines: dict[str, str] = {}
         cache_entries = {f"SKBUILD_{k.upper()}_DIR": v for k, v in wheel_dirs.items()}
         builder.configure(
             defines=defines,
@@ -190,30 +199,51 @@
         mapping = packages_to_file_mapping(
             packages=packages,
             platlib_dir=wheel_dirs["platlib"],
             include=settings.sdist.include,
             exclude=settings.sdist.exclude,
         )
 
-        for filepath, package_dir in mapping.items():
-            Path(package_dir).parent.mkdir(exist_ok=True, parents=True)
-            shutil.copyfile(filepath, package_dir)
-
-        for item in wheel_dirs["scripts"].iterdir():
-            with item.open("rb") as f:
-                content = f.read(len(b"#!python"))
-                if content.startswith(b"#!/") and content == b"#!python":
-                    logger.warning(
-                        "Files in scripts/ are not post-processed yet for shabang fixes"
-                    )
-                    break
+        if not editable:
+            for filepath, package_dir in mapping.items():
+                Path(package_dir).parent.mkdir(exist_ok=True, parents=True)
+                shutil.copyfile(filepath, package_dir)
+
+            process_script_dir(wheel_dirs["scripts"])
 
         with WheelWriter(metadata, Path(wheel_directory), tags.as_tags_set()) as wheel:
             wheel.build(wheel_dirs)
 
+            if editable:
+                modules = {
+                    path_to_module(Path(v).relative_to(wheel_dirs["platlib"])): str(
+                        Path(k).resolve()
+                    )
+                    for k, v in mapping.items()
+                }
+                installed = {
+                    path_to_module(v.relative_to(wheel_dirs["platlib"])): str(
+                        v.relative_to(wheel_dirs["platlib"])
+                    )
+                    for v in scantree(wheel_dirs["platlib"])
+                }
+                editable_py = resources / "_editable_redirect.py"
+                editable_txt = editable_py.read_text(encoding="utf-8")
+                reload_dir = os.fspath(build_dir) if settings.build_dir else None
+                editable_txt += f"\n\ninstall({modules!r}, {installed!r}, {reload_dir!r}, {settings.editable.rebuild!r}, {settings.editable.verbose!r})\n"
+
+                wheel.writestr(
+                    f"_{normalized_name}_editable.py",
+                    editable_txt.encode("utf-8"),
+                )
+                wheel.writestr(
+                    f"_{normalized_name}_editable.pth",
+                    f"import _{normalized_name}_editable\n".encode(),
+                )
+
     if metadata_directory is not None:
         dist_info_contents = wheel.dist_info_contents()
         dist_info = Path(metadata_directory)
         for key, data in dist_info_contents.items():
             path = dist_info / key
             prevous_data = path.read_bytes()
             if prevous_data != data:
```

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.3.0/src/scikit_build_core/builder/builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from collections.abc import Sequence
 from pathlib import Path
 from typing import Mapping
 
 from packaging.version import Version
 
 from .. import __version__
+from .._compat.importlib import metadata, resources
 from .._logging import logger
 from ..cmake import CMaker
 from ..resources import find_python
 from ..settings.skbuild_model import ScikitBuildSettings
 from .generator import set_environment_for_gen
 from .sysconfig import get_platform, get_python_include_dir, get_python_library
 
@@ -82,14 +83,22 @@
         cache_entries: Mapping[str, str | Path] | None = None,
         name: str | None = None,
         version: Version | None = None,
         limited_abi: bool | None = None,
     ) -> None:
         cmake_defines = dict(defines)
 
+        # Add any extra CMake modules
+        eps = metadata.entry_points(group="cmake.module")
+        self.config.module_dirs.extend(resources.files(ep.load()) for ep in eps)
+
+        # Add any extra CMake prefixes
+        eps = metadata.entry_points(group="cmake.prefix")
+        self.config.prefix_dirs.extend(resources.files(ep.load()) for ep in eps)
+
         # Add site-packages to the prefix path for CMake
         site_packages = Path(sysconfig.get_path("purelib"))
         self.config.prefix_dirs.append(site_packages)
         logger.debug("SITE_PACKAGES: {}", site_packages)
         if site_packages != DIR.parent.parent:
             self.config.prefix_dirs.append(DIR.parent.parent)
             logger.debug("Extra SITE_PACKAGES: {}", site_packages)
@@ -131,14 +140,16 @@
 
         # Modern Find Python
         for prefix in ("Python", "Python3"):
             cache_config[f"{prefix}_EXECUTABLE"] = sys.executable
             cache_config[f"{prefix}_ROOT_DIR"] = sys.prefix
             cache_config[f"{prefix}_INCLUDE_DIR"] = python_include_dir
             cache_config[f"{prefix}_FIND_REGISTRY"] = "NEVER"
+            if python_library:
+                cache_config[f"{prefix}_LIBRARY"] = python_library
 
         if limited_abi:
             cache_config["SKBUILD_SOABI"] = (
                 "" if sys.platform.startswith("win") else "abi3"
             )
         else:
             # Workaround for bug in PyPy and packaging that is not handled in CMake
```

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.3.0/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.3.0/src/scikit_build_core/builder/get_requires.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
 
+import dataclasses
 import functools
 import os
 import sys
-from collections.abc import Mapping
+from collections.abc import Generator, Mapping
 
 from packaging.tags import sys_tags
 from packaging.version import Version
 
 from .._compat import tomllib
 from .._compat.typing import Literal
 from .._logging import logger
 from ..program_search import (
     best_program,
     get_cmake_programs,
     get_make_programs,
     get_ninja_programs,
 )
 from ..resources import resources
+from ..settings._load_provider import load_provider
 from ..settings.skbuild_read_settings import SettingsReader
 
-__all__ = ["cmake_ninja_for_build_wheel"]
+__all__ = ["GetRequires"]
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
 @functools.lru_cache(maxsize=2)
@@ -34,44 +36,70 @@
 
 
 @functools.lru_cache(maxsize=2)
 def is_known_platform(platforms: frozenset[str]) -> bool:
     return any(tag.platform in platforms for tag in sys_tags())
 
 
-def cmake_ninja_for_build_wheel(
-    config_settings: Mapping[str, str | list[str]] | None = None
-) -> list[str]:
-    settings = SettingsReader.from_file("pyproject.toml", config_settings).settings
-
-    packages = []
-    cmake_min = Version(settings.cmake.minimum_version)
-    cmake = best_program(get_cmake_programs(module=False), minimum_version=cmake_min)
-    if cmake is None:
-        packages.append(f"cmake>={cmake_min}")
-    else:
+@dataclasses.dataclass
+class GetRequires:
+    config_settings: Mapping[str, list[str] | str] | None = None
+
+    def __post_init__(self) -> None:
+        self._settings = SettingsReader.from_file(
+            "pyproject.toml", self.config_settings
+        ).settings
+
+    def cmake(self) -> Generator[str, None, None]:
+        cmake_min = Version(self._settings.cmake.minimum_version)
+        cmake = best_program(
+            get_cmake_programs(module=False), minimum_version=cmake_min
+        )
+        if cmake is None:
+            yield f"cmake>={cmake_min}"
+            return
         logger.debug("Found system CMake: {} - not requiring PyPI package", cmake)
 
-    if (
-        not sys.platform.startswith("win")
-        and os.environ.get("CMAKE_GENERATOR", "Ninja") == "Ninja"
-        and not os.environ.get("CMAKE_MAKE_PROGRAM", "")
-    ):
-        ninja_min = Version(settings.ninja.minimum_version)
+    def ninja(self) -> Generator[str, None, None]:
+        # On Windows, Ninja is not default
+        if sys.platform.startswith("win") and "Ninja" not in os.environ.get(
+            "CMAKE_GENERATOR", ""
+        ):
+            return
+
+        # If something besides Windows is set, don't add ninja
+        if "Ninja" not in os.environ.get("CMAKE_GENERATOR", "Ninja"):
+            return
+
+        # If CMAKE_MAKE_PROGRAM is set, don't add anything, someone already knows what they want
+        if os.environ.get("CMAKE_MAKE_PROGRAM", ""):
+            return
+
+        ninja_min = Version(self._settings.ninja.minimum_version)
         ninja = best_program(
             get_ninja_programs(module=False), minimum_version=ninja_min
         )
-        if ninja is None:
-            if (
-                not settings.ninja.make_fallback
-                or is_known_platform(known_wheels("ninja"))
-                or not list(get_make_programs())
-            ):
-                packages.append(f"ninja>={ninja_min}")
-            else:
-                logger.debug(
-                    "Found system Make & not on known platform - not requiring PyPI package for Ninja"
-                )
-        else:
+        if ninja is not None:
             logger.debug("Found system Ninja: {} - not requiring PyPI package", ninja)
+            return
 
-    return packages
+        if (
+            self._settings.ninja.make_fallback
+            and not is_known_platform(known_wheels("ninja"))
+            and list(get_make_programs())
+        ):
+            logger.debug(
+                "Found system Make & not on known platform - not requiring PyPI package for Ninja"
+            )
+            return
+        yield f"ninja>={ninja_min}"
+
+    def dynamic_metadata(self) -> Generator[str, None, None]:
+        for dynamic_metadata in self._settings.metadata.values():
+            if "provider" in dynamic_metadata:
+                config = dynamic_metadata.copy()
+                provider = config.pop("provider")
+                provider_path = config.pop("provider-path", None)
+                module = load_provider(provider, provider_path)
+                yield from getattr(
+                    module, "get_requires_for_dynamic_metadata", lambda _: []
+                )(config)
```

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.3.0/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.3.0/src/scikit_build_core/builder/sysconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,17 @@
                     masd = masd[len(os.sep) :]
                 libdir_masd = libdir / masd
                 if libdir_masd.is_dir():
                     libdir = libdir_masd
             libpath = libdir / ldlibrary
             if Path(os.path.expandvars(libpath)).is_file():
                 return libpath
+            logger.warning("libdir/ldlibrary: {} is not a real file!", libpath)
+        else:
+            logger.warning("libdir: {} is not a directory", libdir)
 
     framework_prefix = sysconfig.get_config_var("PYTHONFRAMEWORKPREFIX")
     if framework_prefix and Path(framework_prefix).is_dir() and ldlibrary:
         libpath = Path(framework_prefix) / ldlibrary
         if libpath.is_file():
             return libpath
```

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.3.0/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.3.0/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.3.0/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.3.0/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.3.0/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files 0% similar despite different names*

```diff
@@ -494,15 +494,15 @@
       if (NAME STREQUAL "INCLUDES")
         # do some clean-up
         string (REGEX MATCHALL "(-I|-iwithsysroot)[ ]*[^ ]+" _values "${_values}")
         string (REGEX REPLACE "(-I|-iwithsysroot)[ ]*" "" _values "${_values}")
         list (REMOVE_DUPLICATES _values)
       elseif (NAME STREQUAL "SOABI")
         # clean-up: remove prefix character and suffix
-        if (_values MATCHES "^(\\.${CMAKE_SHARED_LIBRARY_SUFFIX}|\\.so|\\.pyd)$")
+        if (_values MATCHES "^(${CMAKE_SHARED_LIBRARY_SUFFIX}|\\.so|\\.pyd)$")
           set(_values "")
         else()
           string (REGEX REPLACE "^[.-](.+)(${CMAKE_SHARED_LIBRARY_SUFFIX}|\\.(so|pyd))$" "\\1" _values "${_values}")
         endif()
       endif()
     endif()
   endif()
@@ -545,15 +545,15 @@
                        ERROR_QUIET
                        OUTPUT_STRIP_TRAILING_WHITESPACE)
       if (_result)
         unset (_values)
       else()
         if (_values)
           # clean-up: remove prefix character and suffix
-          if (_values MATCHES "^(\\.${CMAKE_SHARED_LIBRARY_SUFFIX}|\\.so|\\.pyd)$")
+          if (_values MATCHES "^(${CMAKE_SHARED_LIBRARY_SUFFIX}|\\.so|\\.pyd)$")
             set(_values "")
           else()
             string (REGEX REPLACE "^[.-](.+)(${CMAKE_SHARED_LIBRARY_SUFFIX}|\\.(so|pyd))$" "\\1" _values "${_values}")
           endif()
         endif()
       endif()
 
@@ -572,24 +572,24 @@
             if (_item)
               set (_values "${_item}")
               break()
             endif()
           endforeach()
           if (_values)
             # clean-up: remove prefix character and suffix
-            if (_values MATCHES "^(\\.${CMAKE_SHARED_LIBRARY_SUFFIX}|\\.so|\\.pyd)$")
+            if (_values MATCHES "^(${CMAKE_SHARED_LIBRARY_SUFFIX}|\\.so|\\.pyd)$")
               set(_values "")
             else()
               string (REGEX REPLACE "^[.-](.+)(${CMAKE_SHARED_LIBRARY_SUFFIX}|\\.(so|pyd))$" "\\1" _values "${_values}")
             endif()
           endif()
         endif()
       endif()
     elseif (NAME STREQUAL "SOSABI")
-      execute_process (COMMAND ${_${_PYTHON_PREFIX}_INTERPRETER_LAUNCHER} "${_${_PYTHON_PREFIX}_EXECUTABLE}" -c "import sys\nimport re\nimport importlib\nsys.stdout.write(next(filter(lambda x: re.search('^\\.abi', x), importlib.machinery.EXTENSION_SUFFIXES)))"
+      execute_process (COMMAND ${_${_PYTHON_PREFIX}_INTERPRETER_LAUNCHER} "${_${_PYTHON_PREFIX}_EXECUTABLE}" -c "import sys\nimport re\nimport importlib.machinery\nsys.stdout.write(next(filter(lambda x: re.search('^\\.abi', x), importlib.machinery.EXTENSION_SUFFIXES)))"
                        RESULT_VARIABLE _result
                        OUTPUT_VARIABLE _values
                        ERROR_QUIET
                        OUTPUT_STRIP_TRAILING_WHITESPACE)
       if (_result)
         unset (_values)
       else()
```

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.3.0/src/scikit_build_core/settings/skbuild_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import dataclasses
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 
 __all__ = [
     "ScikitBuildSettings",
     "NinjaSettings",
     "CMakeSettings",
     "LoggingSettings",
     "SDistSettings",
@@ -95,25 +95,40 @@
     install_dir: str = ""
 
 
 @dataclasses.dataclass
 class BackportSettings:
     #: If CMake is less than this value, backport a copy of FindPython. Set
     #: to 0 disable this, or the empty string.
-    find_python: str = "3.26"
+    find_python: str = "3.26.1"
+
+
+@dataclasses.dataclass
+class Editable:
+    #: Select the editable mode to use. Currently only "redirect" is supported.
+    mode: str = "redirect"
+
+    #: Turn on verbose output for the editable mode rebuilds.
+    verbose: bool = True
+
+    #: Rebuild the project when the package is imported.
+    #: The build-directory must be set.
+    rebuild: bool = False
 
 
 @dataclasses.dataclass
 class ScikitBuildSettings:
     cmake: CMakeSettings = dataclasses.field(default_factory=CMakeSettings)
     ninja: NinjaSettings = dataclasses.field(default_factory=NinjaSettings)
     logging: LoggingSettings = dataclasses.field(default_factory=LoggingSettings)
     sdist: SDistSettings = dataclasses.field(default_factory=SDistSettings)
     wheel: WheelSettings = dataclasses.field(default_factory=WheelSettings)
     backport: BackportSettings = dataclasses.field(default_factory=BackportSettings)
+    metadata: Dict[str, Dict[str, Any]] = dataclasses.field(default_factory=dict)
+    editable: Editable = dataclasses.field(default_factory=Editable)
 
     #: Strictly check all config options. If False, warnings will be
     #: printed for unknown options. If True, an error will be raised.
     strict_config: bool = True
 
     #: Enable early previews of features not finalized yet.
     experimental: bool = False
```

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.3.0/src/scikit_build_core/settings/sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     else:
         yield list(inner)
 
 
 class Source(Protocol):
     def has_item(self, *fields: str, is_dict: bool) -> bool:
         """
-        Check if the source contains a chain of fields. For example, feilds =
+        Check if the source contains a chain of fields. For example, fields =
         [Field(name="a"), Field(name="b")] will check if the source contains the
         key "a.b".
         """
         ...
 
     def get_item(self, *fields: str, is_dict: bool) -> Any:
         ...
@@ -272,24 +272,26 @@
     def convert(
         cls, item: str | list[str] | dict[str, str], target: type[Any]
     ) -> object:
         raw_target = _get_target_raw_type(target)
         if raw_target == list:
             if isinstance(item, list):
                 return [cls.convert(i, _get_inner_type(target)) for i in item]
-            assert not isinstance(item, dict)
+            if isinstance(item, dict):
+                msg = f"Expected {target}, got {type(item).__name__}"
+                raise TypeError(msg)
             return [
                 cls.convert(i.strip(), _get_inner_type(target)) for i in item.split(";")
             ]
         if raw_target == dict:
             assert not isinstance(item, (str, list))
             return {k: cls.convert(v, _get_inner_type(target)) for k, v in item.items()}
-        assert not isinstance(
-            item, (list, dict)
-        ), "Can't convert list or dict to non-list/dict"
+        if isinstance(item, (list, dict)):
+            msg = f"Expected {target}, got {type(item).__name__}"
+            raise TypeError(msg)
         if raw_target is bool:
             result = item.strip().lower() not in {"0", "false", "off", "no", ""}
             return result
         if callable(raw_target):
             return raw_target(item)
         msg = f"Can't convert target {target}"
         raise AssertionError(msg)
@@ -343,17 +345,25 @@
             msg = f"{names!r} not found in configuration settings"
             raise KeyError(msg) from None
 
     @classmethod
     def convert(cls, item: Any, target: type[Any]) -> object:
         raw_target = _get_target_raw_type(target)
         if raw_target == list:
+            if not isinstance(item, list):
+                msg = f"Expected {target}, got {type(item).__name__}"
+                raise TypeError(msg)
             return [cls.convert(it, _get_inner_type(target)) for it in item]
         if raw_target == dict:
+            if not isinstance(item, dict):
+                msg = f"Expected {target}, got {type(item).__name__}"
+                raise TypeError(msg)
             return {k: cls.convert(v, _get_inner_type(target)) for k, v in item.items()}
+        if raw_target == Any:
+            return item
         if callable(raw_target):
             return raw_target(item)
         msg = f"Can't convert target {target}"
         raise AssertionError(msg)
 
     def unrecognized_options(self, options: object) -> Generator[str, None, None]:
         yield from _unrecognized_dict(self.settings, options, self.prefixes)
@@ -361,16 +371,22 @@
     def all_option_names(self, target: type[Any]) -> Iterator[str]:
         for names in _nested_dataclass_to_names(target):
             dash_names = [name.replace("_", "-") for name in names]
             yield ".".join((*self.prefixes, *dash_names))
 
 
 class SourceChain:
-    def __init__(self, *sources: Source) -> None:
+    def __init__(self, *sources: Source, prefixes: Sequence[str] = ()) -> None:
+        """
+        Combine a collection of sources into a single object that can run
+        ``convert_target(dataclass)``.  An optional list of prefixes can be
+        given that will be prepended (dot separated) to error messages.
+        """
         self.sources = sources
+        self.prefixes = prefixes
 
     def __getitem__(self, index: int) -> Source:
         return self.sources[index]
 
     def has_item(self, *fields: str, is_dict: bool) -> bool:
         return any(source.has_item(*fields, is_dict=is_dict) for source in self.sources)
 
@@ -383,34 +399,43 @@
 
     @classmethod
     def convert(cls, item: Any, target: type[T]) -> T:  # noqa: ARG003
         msg = "SourceChain cannot convert items, use the result from has_item"
         raise NotImplementedError(msg)
 
     def convert_target(self, target: type[T], *prefixes: str) -> T:
+        """
+        Given a dataclass type, create an object of that dataclass filled
+        with the values in the sources.
+        """
+
         errors = []
         prep: dict[str, Any] = {}
         for field in dataclasses.fields(target):  # type: ignore[arg-type]
             if dataclasses.is_dataclass(field.type):
                 try:
                     prep[field.name] = self.convert_target(
                         field.type, *prefixes, field.name
                     )
                 except Exception as e:
+                    name = ".".join([*self.prefixes, *prefixes, field.name])
+                    e.__notes__ = [*getattr(e, "__notes__", []), f"Field: {name}"]  # type: ignore[attr-defined]
                     errors.append(e)
                 continue
 
             is_dict = _get_target_raw_type(field.type) == dict
 
             for source in self.sources:
                 if source.has_item(*prefixes, field.name, is_dict=is_dict):
                     simple = source.get_item(*prefixes, field.name, is_dict=is_dict)
                     try:
                         tmp = source.convert(simple, field.type)
                     except Exception as e:
+                        name = ".".join([*self.prefixes, *prefixes, field.name])
+                        e.__notes__ = [*getattr(e, "__notes__", []), f"Field {name}"]  # type: ignore[attr-defined]
                         errors.append(e)
                         prep[field.name] = None
                         break
 
                     if is_dict:
                         assert isinstance(tmp, dict), f"{field.name} must be a dict"
                         prep[field.name] = {**tmp, **prep.get(field.name, {})}
@@ -428,15 +453,15 @@
             if field.default_factory is not dataclasses.MISSING:
                 prep[field.name] = field.default_factory()
                 continue
 
             errors.append(ValueError(f"Missing value for {field.name!r}"))
 
         if errors:
-            prefix_str = ".".join(prefixes)
+            prefix_str = ".".join([*self.prefixes, *prefixes])
             msg = f"Failed converting {prefix_str}"
             raise ExceptionGroup(msg, errors)
 
         return target(**prep)
 
     def unrecognized_options(self, options: object) -> Generator[str, None, None]:
         for source in self.sources:
```

### Comparing `scikit_build_core-0.2.2/src/scikit_build_core/setuptools/extension.py` & `scikit_build_core-0.3.0/src/scikit_build_core/setuptools/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import os
 import shutil
 import sys
 import sysconfig
 from pathlib import Path
+from typing import Any
 
 import setuptools
 import setuptools.command.build_ext
 from packaging.version import Version
 from setuptools.dist import Distribution
 
 from .._compat.typing import Literal
@@ -24,37 +25,39 @@
     return __all__
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # The sourcedir is relative to the setup.py directory, where the CMakeLists.txt lives
 class CMakeExtension(setuptools.Extension):
-    def __init__(self, name: str, sourcedir: str = "", **kwargs: object) -> None:
+    def __init__(self, name: str, sourcedir: str = "", **kwargs: Any) -> None:
         super().__init__(name, [], **kwargs)
         self.sourcedir = Path(sourcedir).resolve()
 
 
 class CMakeBuild(setuptools.command.build_ext.build_ext):
     def build_extension(self, ext: setuptools.Extension) -> None:
         if not isinstance(ext, CMakeExtension):
             super().build_extension(ext)
             return
 
         build_tmp_folder = Path(self.build_temp)
         build_temp = build_tmp_folder / "_skbuild"  # TODO: include python platform
 
-        dist = self.distribution  # type: ignore[attr-defined]
+        dist = self.distribution
 
-        limited_api = dist.get_command_obj("bdist_wheel").py_limited_api
+        bdist_wheel = dist.get_command_obj("bdist_wheel")
+        assert bdist_wheel is not None
+        limited_api = bdist_wheel.py_limited_api  # type: ignore[attr-defined]
         if limited_api:
             ext.py_limited_api = True
 
         # This dir doesn't exist, so Path.cwd() is needed for Python < 3.10
         # due to a Windows bug in resolve https://github.com/python/cpython/issues/82852
-        ext_fullpath = Path.cwd() / self.get_ext_fullpath(ext.name)  # type: ignore[no-untyped-call]
+        ext_fullpath = Path.cwd() / self.get_ext_fullpath(ext.name)
         extdir = ext_fullpath.parent.resolve()
 
         # TODO: this is a hack due to moving temporary paths for isolation
         if build_temp.exists():
             shutil.rmtree(build_temp)
 
         settings = SettingsReader.from_file("pyproject.toml", {}).settings
@@ -90,15 +93,15 @@
         for key, value in ext.define_macros:
             assert isinstance(value, str), "define_macros values must not be None"
             defines[key] = value
 
         builder.configure(
             defines=defines,
             name=dist.get_name(),
-            version=dist.get_version(),
+            version=Version(dist.get_version()),
             limited_abi=ext.py_limited_api,
         )
 
         # Set CMAKE_BUILD_PARALLEL_LEVEL to control the parallel build level
         # across all generators.
         build_args = []
 
@@ -129,24 +132,24 @@
     assert (
         settings.logging.level == "WARNING"
     ), "Logging is not adjustable in setuptools mode yet"
     assert (
         not settings.wheel.py_api
     ), "wheel.py_api is not supported in setuptools mode, use bdist_wheel options instead"
 
-    dist.has_ext_modules = lambda: True  # type: ignore[attr-defined]
+    dist.has_ext_modules = lambda: True  # type: ignore[method-assign]
     dist.ext_modules = (dist.ext_modules or []) + value
 
     dist.cmdclass["build_ext"] = CMakeBuild
 
 
 def cmake_source_dir(
     dist: Distribution, attr: Literal["cmake_source_dir"], value: str
 ) -> None:
     assert attr == "cmake_source_dir"
     assert Path(value).is_dir()
     assert dist.cmake_extensions is None, "Combining cmake_source_dir= and cmake_extensions= is not allowed"  # type: ignore[attr-defined]
-    name = dist.get_name().replace("-", "_")  # type: ignore[attr-defined]
+    name = dist.get_name().replace("-", "_")
 
     extensions = [CMakeExtension(name, value)]
     dist.cmake_extensions = extensions  # type: ignore[attr-defined]
     cmake_extensions(dist, "cmake_extensions", extensions)
```

### Comparing `scikit_build_core-0.2.2/tests/test_builder.py` & `scikit_build_core-0.3.0/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/test_cmake_config.py` & `scikit_build_core-0.3.0/tests/test_cmake_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,25 +18,15 @@
     yield f"-B{config.build_dir}"
 
     if init:
         cmake_init = config.build_dir / "CMakeInit.txt"
         yield f"-C{cmake_init}"
 
     if config.single_config:
-        yield f"-DCMAKE_BUILD_TYPE={config.build_type}"
-
-    if config.module_dirs:
-        yield "-DCMAKE_MODULE_PATH:PATH={}".format(
-            ";".join(str(p).replace("\\", "/") for p in config.module_dirs)
-        )
-
-    if config.prefix_dirs:
-        yield "-DCMAKE_PREFIX_PATH:PATH={}".format(
-            ";".join(str(p).replace("\\", "/") for p in config.prefix_dirs)
-        )
+        yield f"-DCMAKE_BUILD_TYPE:STRING={config.build_type}"
 
 
 @pytest.mark.configure()
 def test_init_cache(fp, tmp_path):
     fp.register([fp.program("cmake"), "--version"], stdout="3.14.0")
     fp.register([fp.program("cmake3"), "--version"], stdout="3.14.0")
```

### Comparing `scikit_build_core-0.2.2/tests/test_fileapi.py` & `scikit_build_core-0.3.0/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/test_generator_default.py` & `scikit_build_core-0.3.0/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/test_module_dir.py` & `scikit_build_core-0.3.0/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/test_name_main.py` & `scikit_build_core-0.3.0/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/test_program_search.py` & `scikit_build_core-0.3.0/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/test_pyproject_abi3.py` & `scikit_build_core-0.3.0/tests/test_pyproject_abi3.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import shutil
 import sys
+import sysconfig
 import zipfile
 from pathlib import Path
 
 import pytest
 
 from scikit_build_core.build import build_wheel
 
 DIR = Path(__file__).parent.resolve()
 ABI_PKG = DIR / "packages/abi3_pyproject_ext"
+SYSCONFIGPLAT = sysconfig.get_platform()
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.skipif(
     sys.implementation.name == "pypy", reason="pypy does not support abi3"
 )
 @pytest.mark.skipif(
-    sys.platform.startswith("win"),
-    reason="abi3 is hard to target with FindPython on Windows",
+    SYSCONFIGPLAT.startswith(("msys", "mingw")),
+    reason="abi3 FindPython on MSYS/MinGW reports not found",
 )
 def test_abi3_wheel(tmp_path, monkeypatch, virtualenv):
     dist = tmp_path / "dist"
     dist.mkdir()
     monkeypatch.chdir(ABI_PKG)
     if Path("dist").is_dir():
         shutil.rmtree("dist")
```

### Comparing `scikit_build_core-0.2.2/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.3.0/tests/test_pyproject_extra_dirs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,31 @@
-import shutil
 import sys
 import zipfile
 from pathlib import Path
 
 import pytest
 
 from scikit_build_core.build import build_wheel
 from scikit_build_core.errors import CMakeConfigError
 
-DIR = Path(__file__).parent.resolve()
-HELLO_PEP518 = DIR / "packages/filepath_pure"
-
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.skipif(
     sys.version_info < (3, 8),
     reason="Python 3.7 doesn't have a nice Path zipfile interface",
 )
-def test_pep517_wheel_extra_dirs(tmp_path, monkeypatch):
-    dist = tmp_path / "dist"
-    dist.mkdir()
-    monkeypatch.chdir(HELLO_PEP518)
+@pytest.mark.usefixtures("package_filepath_pure")
+def test_pep517_wheel_extra_dirs(monkeypatch):
     monkeypatch.setenv("SKBUILD_CMAKE_DEFINE", "SOME_DEFINE3=baz;SOME_DEFINE4=baz")
     monkeypatch.setenv("SKBUILD_CMAKE_ARGS", "-DSOME_ARGS1=baz")
 
-    if Path("dist").is_dir():
-        shutil.rmtree("dist")
+    dist = Path("dist")
     out = build_wheel(
-        str(dist),
+        "dist",
         {"cmake.define.SOME_DEFINE2": "bar", "cmake.define.SOME_DEFINE3": "bar"},
     )
     (wheel,) = dist.glob("cmake_dirs-0.0.1-*.whl")
     assert wheel == dist / out
 
     if sys.version_info >= (3, 8):
         with wheel.open("rb") as f:
@@ -59,26 +52,21 @@
 
         assert package == {"main.py"}
         assert data == {"in_data.txt"}
         assert headers == {"in_headers.h"}
         assert scripts == {"in_scripts.py"}
 
 
-def test_pep517_wheel_too_old_core(tmp_path, monkeypatch):
-    dist = tmp_path / "dist"
-    dist.mkdir()
-    monkeypatch.chdir(HELLO_PEP518)
+@pytest.mark.usefixtures("package_filepath_pure")
+def test_pep517_wheel_too_old_core(monkeypatch):
     monkeypatch.setenv("SKBUILD_CMAKE_DEFINE", "SOME_DEFINE3=baz;SOME_DEFINE4=baz")
     monkeypatch.setenv("SKBUILD_CMAKE_ARGS", "-DSOME_ARGS1=baz")
 
-    if Path("dist").is_dir():
-        shutil.rmtree("dist")
-
     with pytest.raises(CMakeConfigError):
         build_wheel(
-            str(dist),
+            "dist",
             {
                 "cmake.define.SOME_DEFINE2": "bar",
                 "cmake.define.SOME_DEFINE3": "bar",
                 "minimum-version": "99",
             },
         )
```

### Comparing `scikit_build_core-0.2.2/tests/test_pyproject_pep517.py` & `scikit_build_core-0.3.0/tests/test_pyproject_pep517.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from pathlib import Path
 
 import build.util
 import pytest
 
 from scikit_build_core.build import _file_processor, build_sdist, build_wheel
 
-DIR = Path(__file__).parent.resolve()
-HELLO_PEP518 = DIR / "packages/simple_pyproject_ext"
 ENTRYPOINTS = """\
 [one.two]
 three = four
 
 [console_scripts]
 something = other
 
@@ -35,20 +33,18 @@
 mark_hashes_different = pytest.mark.xfail(
     sys.platform.startswith("win32") or sys.platform.startswith("cygwin"),
     reason="hashes differ on Windows",
     strict=False,
 )
 
 
-def test_pep517_sdist(tmp_path, monkeypatch):
-    dist = tmp_path.resolve() / "dist"
-    monkeypatch.chdir(HELLO_PEP518)
-    if Path("dist").is_dir():
-        shutil.rmtree("dist")
-    out = build_sdist(str(dist))
+@pytest.mark.usefixtures("package_simple_pyproject_ext")
+def test_pep517_sdist():
+    dist = Path("dist")
+    out = build_sdist("dist")
 
     (sdist,) = dist.iterdir()
     assert sdist.name == "cmake-example-0.0.1.tar.gz"
     assert sdist == dist / out
 
     with tarfile.open(sdist) as f:
         file_names = set(f.getnames())
@@ -64,41 +60,29 @@
         pkg_info = f.extractfile("cmake-example-0.0.1/PKG-INFO")
         assert pkg_info
         pkg_info_contents = pkg_info.read().decode()
         assert pkg_info_contents == METADATA
 
 
 @mark_hashes_different
-def test_pep517_sdist_hash(tmp_path, monkeypatch):
+def test_pep517_sdist_hash(monkeypatch, package_simple_pyproject_ext):
     # Unset SOURCE_DATE_EPOCH in order to guarantee the hash match
     monkeypatch.delenv("SOURCE_DATE_EPOCH", raising=False)
-    dist = tmp_path.resolve() / "dist"
-    monkeypatch.chdir(HELLO_PEP518)
-    if Path("dist").is_dir():
-        shutil.rmtree("dist")
-    out = build_sdist(str(dist))
+    dist = Path("dist")
+    out = build_sdist("dist")
     sdist = dist / out
     hash = hashlib.sha256(sdist.read_bytes()).hexdigest()
-    if sys.version_info < (3, 9):
-        assert (
-            hash == "3b4af3fbe3d4505415bb1e55bb2e49902f4633d371ae7288007d90eb1488bc4d"
-        )
-    else:
-        assert (
-            hash == "d373b8458ee37b176cfd03f0f3199b30fdb034bca465b2826392a6c3af85ca4c"
-        )
+    assert hash == package_simple_pyproject_ext.sdist_hash
 
 
-def test_pep517_sdist_time_hash(tmp_path, monkeypatch):
-    dist = tmp_path.resolve() / "dist"
-    monkeypatch.chdir(HELLO_PEP518)
-    if Path("dist").is_dir():
-        shutil.rmtree("dist")
+@pytest.mark.usefixtures("package_simple_pyproject_ext")
+def test_pep517_sdist_time_hash():
+    dist = Path("dist")
 
-    out = build_sdist(str(dist))
+    out = build_sdist("dist")
     sdist = dist / out
     hash1 = hashlib.sha256(sdist.read_bytes()).hexdigest()
 
     time.sleep(2)
     Path("src/main.cpp").touch()
 
     if Path("dist").is_dir():
@@ -108,21 +92,19 @@
     sdist = dist / out
 
     hash2 = hashlib.sha256(sdist.read_bytes()).hexdigest()
 
     assert hash1 == hash2
 
 
-def test_pep517_sdist_time_hash_nonreproducable(tmp_path, monkeypatch):
-    dist = tmp_path.resolve() / "dist"
-    monkeypatch.chdir(HELLO_PEP518)
-    if Path("dist").is_dir():
-        shutil.rmtree("dist")
+@pytest.mark.usefixtures("package_simple_pyproject_ext")
+def test_pep517_sdist_time_hash_nonreproducable():
+    dist = Path("dist")
 
-    out = build_sdist(str(dist), {"sdist.reproducible": "false"})
+    out = build_sdist("dist", {"sdist.reproducible": "false"})
     sdist = dist / out
     hash1 = hashlib.sha256(sdist.read_bytes()).hexdigest()
 
     time.sleep(2)
 
     if Path("dist").is_dir():
         shutil.rmtree("dist")
@@ -133,52 +115,43 @@
     hash2 = hashlib.sha256(sdist.read_bytes()).hexdigest()
 
     assert hash1 != hash2
 
 
 @mark_hashes_different
 @pytest.mark.parametrize("reverse_order", [False, True])
-def test_pep517_sdist_time_hash_set_epoch(tmp_path, monkeypatch, reverse_order):
-    dist = tmp_path.resolve() / "dist"
-    monkeypatch.chdir(HELLO_PEP518)
-    monkeypatch.setenv("SOURCE_DATE_EPOCH", "12345")
-    if Path("dist").is_dir():
-        shutil.rmtree("dist")
+def test_pep517_sdist_time_hash_set_epoch(
+    monkeypatch, reverse_order, package_simple_pyproject_ext
+):
+    dist = Path("dist")
+    monkeypatch.setenv(
+        "SOURCE_DATE_EPOCH", package_simple_pyproject_ext.source_date_epoch
+    )
 
     _each_unignored_file = _file_processor.each_unignored_file
 
     def each_unignored_file_ordered(*args, **kwargs):
         return sorted(_each_unignored_file(*args, **kwargs), reverse=reverse_order)
 
     monkeypatch.setattr(
         _file_processor, "each_unignored_file", each_unignored_file_ordered
     )
 
     out = build_sdist(str(dist), {"sdist.reproducible": "true"})
     sdist = dist / out
     hash = hashlib.sha256(sdist.read_bytes()).hexdigest()
-    if sys.version_info < (3, 9):
-        assert (
-            hash == "99d54d3090f932f00b77f01d12d422aacb674a6a9afd6af24f7afaaab7c3082b"
-        )
-    else:
-        assert (
-            hash == "359e38eb01415440cc8f7d9ee09612d625b8906ca09cd08c9d56f3eb972b0110"
-        )
+    assert hash == package_simple_pyproject_ext.sdist_dated_hash
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
-def test_pep517_wheel(tmp_path, monkeypatch, virtualenv):
-    dist = tmp_path / "dist"
-    dist.mkdir()
-    monkeypatch.chdir(HELLO_PEP518)
-    if Path("dist").is_dir():
-        shutil.rmtree("dist")
-    out = build_wheel(str(dist))
+@pytest.mark.usefixtures("package_simple_pyproject_ext")
+def test_pep517_wheel(virtualenv):
+    dist = Path("dist")
+    out = build_wheel("dist")
     (wheel,) = dist.glob("cmake_example-0.0.1-*.whl")
     assert wheel == dist / out
 
     if sys.version_info >= (3, 8):
         with wheel.open("rb") as f:
             p = zipfile.Path(f)
             file_names = [p.name for p in p.iterdir()]
@@ -215,22 +188,18 @@
     )
     assert add.strip() == "3"
 
 
 @pytest.mark.skip(reason="Doesn't work yet")
 @pytest.mark.compile()
 @pytest.mark.configure()
-def test_pep517_wheel_time_hash(tmp_path, monkeypatch):
-    dist = tmp_path / "dist"
-    dist.mkdir()
-    monkeypatch.chdir(HELLO_PEP518)
+def test_pep517_wheel_time_hash(monkeypatch):
     monkeypatch.setenv("SOURCE_DATE_EPOCH", "12345")
-    if Path("dist").is_dir():
-        shutil.rmtree("dist")
-    out = build_wheel(str(dist))
+    dist = Path("dist")
+    out = build_wheel("dist")
     wheel = dist / out
     hash1 = hashlib.sha256(wheel.read_bytes()).hexdigest()
 
     time.sleep(2)
     Path("src/main.cpp").touch()
 
     if Path("dist").is_dir():
@@ -240,16 +209,17 @@
     wheel = dist / out
 
     hash2 = hashlib.sha256(wheel.read_bytes()).hexdigest()
 
     assert hash1 == hash2
 
 
+@pytest.mark.usefixtures("package_simple_pyproject_ext")
 def test_prepare_metdata_for_build_wheel():
-    metadata = build.util.project_wheel_metadata(HELLO_PEP518, isolated=False)
+    metadata = build.util.project_wheel_metadata(str(Path.cwd()), isolated=False)
     answer = {
         "Metadata-Version": "2.1",
         "Name": "cmake-example",
         "Version": "0.0.1",
         "Requires-Python": ">=3.7",
         "Provides-Extra": "test",
         "Requires-Dist": 'pytest>=6.0; extra == "test"',
```

### Comparing `scikit_build_core-0.2.2/tests/test_pyproject_pep518.py` & `scikit_build_core-0.3.0/tests/test_pyproject_pep518.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,52 +5,36 @@
 import tarfile
 import textwrap
 import zipfile
 from pathlib import Path
 
 import pytest
 
-DIR = Path(__file__).parent.resolve()
-HELLO_PEP518 = DIR / "packages/simple_pyproject_ext"
-
 
 @pytest.mark.isolated()
 @pytest.mark.integration()
-def test_pep518_sdist():
+def test_pep518_sdist(package_simple_pyproject_ext):
     correct_metadata = textwrap.dedent(
         """\
         Metadata-Version: 2.1
         Name: cmake-example
         Version: 0.0.1
         Requires-Python: >=3.7
         Provides-Extra: test
         Requires-Dist: pytest>=6.0; extra == "test"
         """
     )
 
-    dist = HELLO_PEP518 / "dist"
-    shutil.rmtree(dist, ignore_errors=True)
-    subprocess.run(
-        [sys.executable, "-m", "build", "--sdist"], cwd=HELLO_PEP518, check=True
-    )
-    (sdist,) = dist.iterdir()
+    subprocess.run([sys.executable, "-m", "build", "--sdist"], check=True)
+    (sdist,) = Path("dist").iterdir()
     assert sdist.name == "cmake-example-0.0.1.tar.gz"
 
     if not (sys.platform.startswith("win32") or sys.platform.startswith("cygwin")):
         hash = hashlib.sha256(sdist.read_bytes()).hexdigest()
-        if sys.version_info < (3, 9):
-            assert (
-                hash
-                == "3b4af3fbe3d4505415bb1e55bb2e49902f4633d371ae7288007d90eb1488bc4d"
-            )
-        else:
-            assert (
-                hash
-                == "d373b8458ee37b176cfd03f0f3199b30fdb034bca465b2826392a6c3af85ca4c"
-            )
+        assert hash == package_simple_pyproject_ext.sdist_hash
 
     with tarfile.open(sdist) as f:
         file_names = set(f.getnames())
         assert file_names == {
             f"cmake-example-0.0.1/{x}"
             for x in (
                 "CMakeLists.txt",
@@ -64,28 +48,26 @@
         pkg_info_contents = pkg_info.read().decode()
         assert correct_metadata == pkg_info_contents
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.integration()
+@pytest.mark.usefixtures("package_simple_pyproject_ext")
 @pytest.mark.parametrize(
     "build_args", [(), ("--wheel",)], ids=["sdist_to_wheel", "wheel_directly"]
 )
-def test_pep518_wheel(isolated, build_args, monkeypatch):
-    dist = HELLO_PEP518 / "dist"
-    shutil.rmtree(dist, ignore_errors=True)
-    monkeypatch.chdir(HELLO_PEP518)
+def test_pep518_wheel(isolated, build_args):
     isolated.install("build[virtualenv]")
     isolated.module(
         "build",
         "--config-setting=logging.level=DEBUG",
         *build_args,
     )
-    (wheel,) = dist.glob("cmake_example-0.0.1-*.whl")
+    (wheel,) = Path("dist").glob("cmake_example-0.0.1-*.whl")
 
     if sys.version_info >= (3, 8):
         with wheel.open("rb") as f:
             p = zipfile.Path(f)
             file_names = [p.name for p in p.iterdir()]
 
         assert len(file_names) == 2
@@ -107,23 +89,24 @@
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.integration()
 @pytest.mark.parametrize(
     "build_args", [(), ("--wheel",)], ids=["sdist_to_wheel", "wheel_directly"]
 )
-def test_pep518_rebuild_build_dir(isolated, monkeypatch, tmp_path, build_args):
-    dist = HELLO_PEP518 / "dist"
-    monkeypatch.chdir(HELLO_PEP518)
+@pytest.mark.usefixtures("package_simple_pyproject_ext")
+def test_pep518_rebuild_build_dir(isolated, tmp_path, build_args):
     isolated.install("build[virtualenv]")
 
     build_dir = tmp_path.joinpath("build")
     build_dir.mkdir()
     build_dir = build_dir.resolve()
 
+    dist = Path("dist")
+
     for _ in range(2):
         shutil.rmtree(dist, ignore_errors=True)
         isolated.module(
             "build",
             *build_args,
             "--config-setting=logging.level=DEBUG",
             f"--config-setting=build-dir={build_dir}",
@@ -148,15 +131,16 @@
     version = isolated.execute("import cmake_example; print(cmake_example.__version__)")
     assert version == "0.0.1"
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.integration()
+@pytest.mark.usefixtures("package_simple_pyproject_ext")
 def test_pep518_pip(isolated):
-    isolated.install("-v", HELLO_PEP518)
+    isolated.install("-v", ".")
 
     version = isolated.execute("import cmake_example; print(cmake_example.__version__)")
     assert version == "0.0.1"
 
     add = isolated.execute("import cmake_example; print(cmake_example.add(1, 2))")
     assert add == "3"
```

### Comparing `scikit_build_core-0.2.2/tests/test_settings.py` & `scikit_build_core-0.3.0/tests/test_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 from pathlib import Path
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import pytest
 
 from scikit_build_core.settings.sources import (
     ConfSource,
     EnvSource,
     SourceChain,
@@ -20,14 +20,16 @@
     three: List[str]
     four: List[int] = dataclasses.field(default_factory=list)
     five: str = "empty"
     six: Path = Path("empty")
     seven: Union[int, None] = None
     eight: Dict[str, str] = dataclasses.field(default_factory=dict)
     nine: Dict[str, int] = dataclasses.field(default_factory=dict)
+    # TOML only
+    ten: Dict[str, Any] = dataclasses.field(default_factory=dict)
 
 
 def test_empty(monkeypatch):
     monkeypatch.setenv("SKB_ZERO", "zero")
     monkeypatch.setenv("SKB_ONE", "one")
     monkeypatch.setenv("SKB_TWO", "2")
     monkeypatch.setenv("SKB_THREE", "three")
@@ -124,14 +126,15 @@
         "three": ["three"],
         "four": [4],
         "five": "five",
         "six": "six",
         "seven": 7,
         "eight": {"one": "one", "two": "two"},
         "nine": {"thing": 8},
+        "ten": {"a": {"b": 3}},
     }
 
     sources = SourceChain(
         EnvSource("SKBUILD"),
         ConfSource(settings={}),
         TOMLSource(settings=toml_settings),
     )
@@ -143,14 +146,15 @@
     assert settings.three == ["three"]
     assert settings.four == [4]
     assert settings.five == "five"
     assert settings.six == Path("six")
     assert settings.seven == 7
     assert settings.eight == {"one": "one", "two": "two"}
     assert settings.nine == {"thing": 8}
+    assert settings.ten == {"a": {"b": 3}}
 
 
 def test_all_names():
     keys = [x.name for x in dataclasses.fields(SettingChecker)]
 
     envame = [f"SKBUILD_{x.upper()}" for x in keys]
     assert list(EnvSource("SKBUILD").all_option_names(SettingChecker)) == envame
```

### Comparing `scikit_build_core-0.2.2/tests/test_setuptools_abi3.py` & `scikit_build_core-0.3.0/tests/test_setuptools_abi3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 import shutil
 import sys
+import sysconfig
 import zipfile
 from pathlib import Path
 
 import pytest
 
 from scikit_build_core.setuptools.build_meta import build_wheel
 
 pytestmark = pytest.mark.setuptools
 
 DIR = Path(__file__).parent.resolve()
 ABI_PKG = DIR / "packages/abi3_setuptools_ext"
+SYSCONFIGPLAT = sysconfig.get_platform()
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.skipif(
     sys.implementation.name == "pypy", reason="pypy does not support abi3"
 )
 @pytest.mark.skipif(
-    sys.platform.startswith("win"),
-    reason="abi3 is hard to target with FindPython on Windows",
+    SYSCONFIGPLAT.startswith(("msys", "mingw")),
+    reason="abi3 FindPython on MSYS/MinGW reports not found",
 )
 def test_abi3_wheel(tmp_path, monkeypatch, virtualenv):
     dist = tmp_path / "dist"
     dist.mkdir()
-    monkeypatch.chdir(ABI_PKG)
+
+    # create a temporary copy of the package source so we don't contaminate the
+    # main source tree with build artefacts
+    src = tmp_path / "src"
+    shutil.copytree(ABI_PKG, src)
+    monkeypatch.chdir(src)
     if Path("dist").is_dir():
         shutil.rmtree("dist")
 
     out = build_wheel(str(dist))
     (wheel,) = dist.glob("abi3_example-0.0.1-*.whl")
     assert wheel == dist / out
     assert "-cp37-abi3-" in out
@@ -37,18 +44,18 @@
     assert virtualenv.execute("print('hello')") == "hello"
 
     if sys.version_info >= (3, 8):
         with wheel.open("rb") as f:
             p = zipfile.Path(f)
             file_names = {p.name for p in p.iterdir()}
 
-        so_file = (
-            "abi3_example.abi3.dll"
-            if sys.platform.startswith("cygwin")
-            else "abi3_example.abi3.so"
-        )
-        assert so_file in file_names
+        if sys.platform.startswith("win"):
+            assert "abi3_example.pyd" in file_names
+        elif sys.platform.startswith("cygwin"):
+            assert "abi3_example.abi3.dll" in file_names
+        else:
+            assert "abi3_example.abi3.so" in file_names
 
     virtualenv.install(wheel)
 
     output = virtualenv.execute("import abi3_example; print(abi3_example.square(2))")
     assert output == "4.0"
```

### Comparing `scikit_build_core-0.2.2/tests/test_setuptools_pep517.py` & `scikit_build_core-0.3.0/tests/test_setuptools_pep517.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,37 @@
-import shutil
 import sys
 import tarfile
 import textwrap
 import zipfile
 from pathlib import Path
 
 import pytest
 
 from scikit_build_core.setuptools.build_meta import build_sdist, build_wheel
 
 pytestmark = pytest.mark.setuptools
 
-DIR = Path(__file__).parent.resolve()
-HELLO_PEP518 = DIR / "packages/simple_setuptools_ext"
 
-
-def test_pep517_sdist(tmp_path, monkeypatch):
+@pytest.mark.usefixtures("package_simple_setuptools_ext")
+def test_pep517_sdist():
     correct_metadata = textwrap.dedent(
         """\
         Metadata-Version: 2.1
         Name: cmake-example
         Version: 0.0.1
         Requires-Python: >=3.7
         Provides-Extra: test
         """
         # TODO: why is this missing?
         # Requires-Dist: pytest>=6.0; extra == "test"
     )
     metadata_set = set(correct_metadata.strip().splitlines())
 
-    dist = tmp_path / "dist"
-    dist.mkdir()
-    monkeypatch.chdir(HELLO_PEP518)
-    if Path("dist").is_dir():
-        shutil.rmtree("dist")
-
-    out = build_sdist(str(dist))
+    dist = Path("dist")
+    out = build_sdist("dist")
 
     (sdist,) = dist.iterdir()
     assert sdist.name == "cmake-example-0.0.1.tar.gz"
     assert sdist == dist / out
 
     with tarfile.open(sdist) as f:
         file_names = set(f.getnames())
@@ -65,24 +57,22 @@
         assert pkg_info
         pkg_info_contents = set(pkg_info.read().decode().strip().splitlines())
         assert metadata_set <= pkg_info_contents
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
+@pytest.mark.broken_on_urct()
+@pytest.mark.usefixtures("package_simple_setuptools_ext")
 @pytest.mark.skipif(
     sys.platform.startswith("cygwin"), reason="Cygwin fails here with ld errors"
 )
-def test_pep517_wheel(tmp_path, monkeypatch, virtualenv):
-    dist = tmp_path / "dist"
-    dist.mkdir()
-    monkeypatch.chdir(HELLO_PEP518)
-    if Path("dist").is_dir():
-        shutil.rmtree("dist")
-    out = build_wheel(str(dist))
+def test_pep517_wheel(virtualenv):
+    dist = Path("dist")
+    out = build_wheel("dist")
     (wheel,) = dist.glob("cmake_example-0.0.1-*.whl")
     assert wheel == dist / out
 
     if sys.version_info >= (3, 8):
         with wheel.open("rb") as f:
             p = zipfile.Path(f)
             file_names = [p.name for p in p.iterdir()]
```

### Comparing `scikit_build_core-0.2.2/tests/test_setuptools_pep518.py` & `scikit_build_core-0.3.0/tests/test_setuptools_pep518.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-import shutil
 import sys
 import zipfile
 from pathlib import Path
 
 import pytest
 
 pytestmark = pytest.mark.setuptools
 
-DIR = Path(__file__).parent.resolve()
-HELLO_PEP518 = DIR / "packages/simple_setuptools_ext"
-
 
 # TODO: work out why this fails on Cygwin
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.integration()
+@pytest.mark.broken_on_urct()
 @pytest.mark.skipif(
     sys.platform.startswith("cygwin"), reason="Cygwin fails here with ld errors"
 )
-def test_pep518_wheel(monkeypatch, isolated):
-    dist = HELLO_PEP518 / "dist"
-    shutil.rmtree(dist, ignore_errors=True)
-    monkeypatch.chdir(HELLO_PEP518)
+@pytest.mark.usefixtures("package_simple_setuptools_ext")
+def test_pep518_wheel(isolated):
+    dist = Path("dist")
     isolated.install("build[virtualenv]")
     isolated.module("build", "--wheel")
     (wheel,) = dist.iterdir()
     assert "cmake_example-0.0.1" in wheel.name
     assert wheel.suffix == ".whl"
 
     if sys.version_info >= (3, 8):
@@ -49,19 +45,21 @@
     add = isolated.execute("import cmake_example; print(cmake_example.add(1, 2))")
     assert add == "3"
 
 
 @pytest.mark.compile()
 @pytest.mark.configure()
 @pytest.mark.integration()
+@pytest.mark.broken_on_urct()
 @pytest.mark.skipif(
     sys.platform.startswith("cygwin"), reason="Cygwin fails here with ld errors"
 )
+@pytest.mark.usefixtures("package_simple_setuptools_ext")
 def test_pep518_pip(isolated):
-    isolated.install("-v", HELLO_PEP518)
+    isolated.install("-v", ".")
 
     version = isolated.execute(
         "import cmake_example; print(cmake_example.__version__)",
     )
     assert version == "0.0.1"
 
     add = isolated.execute(
```

### Comparing `scikit_build_core-0.2.2/tests/test_simple_pure.py` & `scikit_build_core-0.3.0/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/test_simplest_c.py` & `scikit_build_core-0.3.0/tests/test_simplest_c.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/test_skbuild_settings.py` & `scikit_build_core-0.3.0/tests/test_skbuild_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,23 @@
     assert settings.logging.level == "WARNING"
     assert settings.sdist.include == []
     assert settings.sdist.exclude == []
     assert settings.sdist.reproducible
     assert settings.wheel.packages is None
     assert settings.wheel.py_api == ""
     assert not settings.wheel.expand_macos_universal_tags
-    assert settings.backport.find_python == "3.26"
+    assert settings.backport.find_python == "3.26.1"
     assert settings.strict_config
     assert not settings.experimental
     assert settings.minimum_version is None
     assert settings.build_dir == ""
+    assert settings.metadata == {}
+    assert settings.editable.mode == "redirect"
+    assert not settings.editable.rebuild
+    assert settings.editable.verbose
 
 
 def test_skbuild_settings_envvar(tmp_path, monkeypatch):
     monkeypatch.setattr(
         scikit_build_core.settings.skbuild_read_settings, "__version__", "0.1.0"
     )
 
@@ -63,14 +67,16 @@
     monkeypatch.setenv("SKBUILD_WHEEL_EXPAND_MACOS_UNIVERSAL_TAGS", "True")
     monkeypatch.setenv("SKBUILD_BACKPORT_FIND_PYTHON", "0")
     monkeypatch.setenv("SKBUILD_STRICT_CONFIG", "0")
     monkeypatch.setenv("SKBUILD_EXPERIMENTAL", "1")
     monkeypatch.setenv("SKBUILD_MINIMUM_VERSION", "0.1")
     monkeypatch.setenv("SKBUILD_CMAKE_VERBOSE", "TRUE")
     monkeypatch.setenv("SKBUILD_BUILD_DIR", "a/b/c")
+    monkeypatch.setenv("SKBUILD_EDITABLE_REBUILD", "True")
+    monkeypatch.setenv("SKBUILD_EDITABLE_VERBOSE", "False")
 
     pyproject_toml = tmp_path / "pyproject.toml"
     pyproject_toml.write_text("", encoding="utf-8")
 
     config_settings: dict[str, list[str] | str] = {}
 
     settings_reader = SettingsReader.from_file(pyproject_toml, config_settings)
@@ -92,14 +98,18 @@
     assert settings.wheel.py_api == "cp39"
     assert settings.wheel.expand_macos_universal_tags
     assert settings.backport.find_python == "0"
     assert not settings.strict_config
     assert settings.experimental
     assert settings.minimum_version == "0.1"
     assert settings.build_dir == "a/b/c"
+    assert settings.metadata == {}
+    assert settings.editable.mode == "redirect"
+    assert settings.editable.rebuild
+    assert not settings.editable.verbose
 
 
 def test_skbuild_settings_config_settings(tmp_path, monkeypatch):
     monkeypatch.setattr(
         scikit_build_core.settings.skbuild_read_settings, "__version__", "0.1.0"
     )
 
@@ -123,14 +133,17 @@
         "wheel.py-api": "cp39",
         "wheel.expand-macos-universal-tags": "True",
         "backport.find-python": "",
         "strict-config": "false",
         "experimental": "1",
         "minimum-version": "0.1",
         "build-dir": "a/b/c",
+        "editable.mode": "redirect",
+        "editable.rebuild": "True",
+        "editable.verbose": "False",
     }
 
     settings_reader = SettingsReader.from_file(pyproject_toml, config_settings)
     settings = settings_reader.settings
     assert list(settings_reader.unrecognized_options()) == []
 
     assert settings.ninja.minimum_version == "1.2"
@@ -148,14 +161,18 @@
     assert settings.wheel.py_api == "cp39"
     assert settings.wheel.expand_macos_universal_tags
     assert settings.backport.find_python == ""
     assert not settings.strict_config
     assert settings.experimental
     assert settings.minimum_version == "0.1"
     assert settings.build_dir == "a/b/c"
+    assert settings.metadata == {}
+    assert settings.editable.mode == "redirect"
+    assert settings.editable.rebuild
+    assert not settings.editable.verbose
 
 
 def test_skbuild_settings_pyproject_toml(tmp_path, monkeypatch):
     monkeypatch.setattr(
         scikit_build_core.settings.skbuild_read_settings, "__version__", "0.1.0"
     )
     pyproject_toml = tmp_path / "pyproject.toml"
@@ -178,14 +195,18 @@
             wheel.py-api = "cp39"
             wheel.expand-macos-universal-tags = true
             backport.find-python = "3.18"
             strict-config = false
             experimental = true
             minimum-version = "0.1"
             build-dir = "a/b/c"
+            metadata.version.provider = "a"
+            editable.mode = "redirect"
+            editable.rebuild = true
+            editable.verbose = false
             """
         ),
         encoding="utf-8",
     )
 
     config_settings: dict[str, list[str] | str] = {}
 
@@ -208,14 +229,18 @@
     assert settings.wheel.py_api == "cp39"
     assert settings.wheel.expand_macos_universal_tags
     assert settings.backport.find_python == "3.18"
     assert not settings.strict_config
     assert settings.experimental
     assert settings.minimum_version == "0.1"
     assert settings.build_dir == "a/b/c"
+    assert settings.metadata == {"version": {"provider": "a"}}
+    assert settings.editable.mode == "redirect"
+    assert settings.editable.rebuild
+    assert not settings.editable.verbose
 
 
 def test_skbuild_settings_pyproject_toml_broken(tmp_path, capsys):
     pyproject_toml = tmp_path / "pyproject.toml"
     pyproject_toml.write_text(
         textwrap.dedent(
             """\
```

### Comparing `scikit_build_core-0.2.2/tests/test_wheelfile_utils.py` & `scikit_build_core-0.3.0/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.3.0/tests/packages/dynamic_metadata/src/module.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#define Py_LIMITED_API 0x03070000
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 float square(float x) { return x * x; }
 
 static PyObject *square_wrapper(PyObject *self, PyObject *args) {
   float input, result;
@@ -13,13 +12,13 @@
   return PyFloat_FromDouble(result);
 }
 
 static PyMethodDef pysimple_methods[] = {
     {"square", square_wrapper, METH_VARARGS, "Square function"},
     {NULL, NULL, 0, NULL}};
 
-static struct PyModuleDef pysimple_module = {PyModuleDef_HEAD_INIT, "pysimple",
+static struct PyModuleDef pysimple_module = {PyModuleDef_HEAD_INIT, "_module",
                                              NULL, -1, pysimple_methods};
 
-PyMODINIT_FUNC PyInit_abi3_example(void) {
+PyMODINIT_FUNC PyInit__module(void) {
   return PyModule_Create(&pysimple_module);
 }
```

### Comparing `scikit_build_core-0.2.2/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.3.0/tests/packages/simplest_c/src/module.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#define Py_LIMITED_API 0x03070000
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 
 float square(float x) { return x * x; }
 
 static PyObject *square_wrapper(PyObject *self, PyObject *args) {
   float input, result;
@@ -13,13 +12,13 @@
   return PyFloat_FromDouble(result);
 }
 
 static PyMethodDef pysimple_methods[] = {
     {"square", square_wrapper, METH_VARARGS, "Square function"},
     {NULL, NULL, 0, NULL}};
 
-static struct PyModuleDef pysimple_module = {PyModuleDef_HEAD_INIT, "pysimple",
+static struct PyModuleDef pysimple_module = {PyModuleDef_HEAD_INIT, "_module",
                                              NULL, -1, pysimple_methods};
 
-PyMODINIT_FUNC PyInit_abi3_example(void) {
+PyMODINIT_FUNC PyInit__module(void) {
   return PyModule_Create(&pysimple_module);
 }
```

### Comparing `scikit_build_core-0.2.2/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.3.0/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cmake_minimum_required(VERSION 3.15...3.25)
+cmake_minimum_required(VERSION 3.15...3.26)
 project(
   "${SKBUILD_PROJECT_NAME}"
   LANGUAGES C
   VERSION "${SKBUILD_PROJECT_VERSION}")
 
 file(TOUCH ${CMAKE_CURRENT_BINARY_DIR}/in_headers.h)
 file(TOUCH ${CMAKE_CURRENT_BINARY_DIR}/in_scripts.py)
```

### Comparing `scikit_build_core-0.2.2/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.3.0/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.3.0/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.3.0/tests/packages/simplest_c/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cmake_minimum_required(VERSION 3.15...3.25)
+cmake_minimum_required(VERSION 3.15...3.26)
 
 project(
   ${SKBUILD_PROJECT_NAME}
   LANGUAGES C
   VERSION ${SKBUILD_PROJECT_VERSION})
 
 find_package(Python COMPONENTS Interpreter Development.Module)
```

### Comparing `scikit_build_core-0.2.2/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.3.0/docs/examples/getting_started/abi3/example.c`

 * *Files 20% similar despite different names*

```diff
@@ -8,17 +8,18 @@
   if (!PyArg_ParseTuple(args, "f", &input)) {
     return NULL;
   }
   result = square(input);
   return PyFloat_FromDouble(result);
 }
 
-static PyMethodDef pysimple_methods[] = {
+static PyMethodDef example_methods[] = {
     {"square", square_wrapper, METH_VARARGS, "Square function"},
     {NULL, NULL, 0, NULL}};
 
-static struct PyModuleDef pysimple_module = {PyModuleDef_HEAD_INIT, "pysimple",
-                                             NULL, -1, pysimple_methods};
+static struct PyModuleDef example_module = {PyModuleDef_HEAD_INIT, "example",
+                                             NULL, -1, example_methods};
 
-PyMODINIT_FUNC PyInit__module(void) {
-  return PyModule_Create(&pysimple_module);
+/* name here must match extension name, with PyInit_ prefix */
+PyMODINIT_FUNC PyInit_example(void) {
+  return PyModule_Create(&example_module);
 }
```

### Comparing `scikit_build_core-0.2.2/.gitignore` & `scikit_build_core-0.3.0/.gitignore`

 * *Files 21% similar despite different names*

```diff
@@ -144,9 +144,27 @@
 # SKBuild cache dir
 _skbuild/
 
 # Any build dirs in the tests
 tests/**/build/
 /src/scikit_build_core/_version.py
 
-# VIM temp files
+# Common editor files
 *~
+*.swp
+
+# RPM spec file
+!/.distro/scikit-build-core.spec
+/.distro/*.tar.gz
+*.rpm
+
+# ruff
+.ruff_cache/
+
+# OS specific stuff
+.DS_Store
+.DS_Store?
+._*
+.Spotlight-V100
+.Trashes
+ehthumbs.db
+Thumbs.db
```

### Comparing `scikit_build_core-0.2.2/LICENSE` & `scikit_build_core-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.2.2/README.md` & `scikit_build_core-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 # scikit-build-core
 
+[![Documentation Status][rtd-badge]][rtd-link]
+
 [![Actions Status][actions-badge]][actions-link]
 [![Code style: black][black-badge]][black-link]
 [![codecov][codecov-badge]][codecov-link]
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![Conda-Forge][conda-badge]][conda-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- Not implemented yet
-[![Documentation Status][rtd-badge]][rtd-link]
 [![Gitter][gitter-badge]][gitter-link]
 -->
 
 <!-- SPHINX-START -->
 
 Features over classic Scikit-build:
 
 - Better warnings, errors, and logging
 - No warning about unused variables
 - Automatically adds Ninja and/or CMake only as required
-- No dependency on setuptools, distutils, or wheel in build mode.
-- Powerful config system, including config options support in build mode.
+- No dependency on setuptools, distutils, or wheel.
+- Powerful config system, including config options support.
 - Automatic inclusion of site-packages in `CMAKE_PREFIX_PATH`
-- FindPython is backported if running on CMake < 3.26 (configurable), supports
-  PyPY SOABI.
+- FindPython is backported if running on CMake < 3.26.1 (configurable), supports
+  PyPY SOABI & Limited API / Stable ABI.
 - Limited API / Stable ABI and pythonless tags supported via config option
 - No slow generator search, ninja/make or MSVC used by default, respects
   `CMAKE_GENERATOR`
 - SDists are reproducible by default (UNIX, Python 3.9+)
 - Support for caching between builds (opt-in by setting `build-dir`)
 - Support for writing out to extra wheel folders (scripts, headers, data)
+- Dedicated entrypoints for module and prefix directories
+- Several integrated dynamic metadata plugins (proposing standardized support
+  soon)
+- Experimental editable mode support, with optional experimental auto rebuilds
+  on import.
 
 The following limitations are present compared to classic scikit-build:
 
 - The minimum supported CMake is 3.15
 - The minimum supported Python is 3.7
 
 Some known missing features that will be developed soon:
 
-- No editable mode support
-- The docs are not written
-- Dedicated entrypoints are planned for projects wanting to support discovery
 - No support for other targets besides install
 - Wheels are not fully reproducible yet
-- Dynamic metadata support is being developed
+- Several editable mode caveats (mentioned in the docs)
 
 Other backends are also planned:
 
 - Setuptools integration highly experimental
 - The extensionlib integration is missing
 - No hatchling plugin yet
 
-The recommended interface is the PEP 517 interface. There is also a WIP
+The recommended interface is the native pyproject builder. There is also a WIP
 setuptools-based interface that is being developed to provide a transition path
 for classic scikit-build.
 
 **WARNING**: Only the pyproject-based builder should be used; the setuptools
 backend is experimental and likely to move to a separate package before being
 declared stable, and internal API is still being solidified. A future version of
 this package will support creating new build extensions.
@@ -83,26 +86,24 @@
 the minimum to get started. You can also add the `rich` (more colorful
 printouts) or `pyproject` (pre-load some dependencies) extras if you want.
 
 An example `CMakeLists.txt`:
 
 ```cmake
 cmake_minimum_required(VERSION 3.15...3.26)
+project(${SKBUILD_PROJECT_NAME} LANGUAGES C)
 
-project(${SKBUILD_PROJECT_NAME} LANGUAGES C VERSION ${SKBUILD_PROJECT_VERSION})
-
-find_package(Python COMPONENTS Interpreter Development.Module)
+find_package(Python COMPONENTS Interpreter Development.Module REQUIRED)
 
 Python_add_library(_module MODULE src/module.c WITH_SOABI)
-
 install(TARGETS _module DESTINATION ${SKBUILD_PROJECT_NAME})
 ```
 
-Scikit-build-core will backport FindPython from CMake 3.26 to older versions of
-Python, and will handle PyPy for you if you are building from PyPy. You will
+Scikit-build-core will backport FindPython from CMake 3.26.1 to older versions
+of Python, and will handle PyPy for you if you are building from PyPy. You will
 need to install everything you want into the full final path inside site-modules
 (so you will usually prefix everything by the package name).
 
 More examples are in the
 [tests/packages](https://github.com/scikit-build/scikit-build-core/tree/main/tests/packages).
 
 ## Configuration
@@ -165,32 +166,44 @@
 # original dir is still at SKBUILD_PLATLIB_DIR (also SKBUILD_DATA_DIR, etc. are
 # available)
 wheel.install-dir = "."
 
 # This will backport an internal copy of FindPython if CMake is less than this
 # value. Set to 0 or the empty string to disable. The default will be kept in
 # sync with the version of FindPython stored in scikit-build-core.
-backport.find-python = "3.26"
+backport.find-python = "3.26.1"
+
+# This is the only editable mode currently
+editable.mode = "redirect"
+
+# Enable auto rebuilds on import (experimental)
+editable.rebuild = false
+
+# Display output on stderr while rebuilding on import
+editable.verbose = true
 
 # Enable experimental features if any are available
 experimental = false
 
 # Strictly validate config options
 strict-config = true
 
 # This provides some backward compatibility if set. Defaults to the latest
 # scikit-build-core version.
 minimum-version = "0.2"  # current version
 
-# Build directory (empty will use a temporary directory). {cache_tag} is
-# available to provide a unique directory per interpreter.
+# Build directory (empty will use a temporary directory). {cache_tag} and
+# {wheel_tag} are available to provide a unique directory per interpreter.
 build-dir = ""
 
 [tool.scikit-build.cmake.define]
 # Put CMake defines in this table.
+
+[tool.scikit-build.metadata]
+# List dynamic metadata fields and hook locations in this table
 ```
 
 Most CMake environment variables should be supported, and `CMAKE_ARGS` can be
 used to set extra CMake args. `ARCHFLAGS` is used to specify macOS universal2 or
 cross-compiles, just like setuptools.
 
 ## Acknowledgements
```

### Comparing `scikit_build_core-0.2.2/pyproject.toml` & `scikit_build_core-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ]
 
 dynamic = ["version"]
 
 dependencies = [
     "exceptiongroup; python_version<'3.11'",
     "importlib_resources >=1.3; python_version<'3.9'",
+    "importlib_metadata; python_version<'3.8'",
     "packaging >=20.9",
     "tomli >=1.1; python_version<'3.11'",
     "typing_extensions >=3.10.0; python_version<'3.8'",
 ]
 # Note: for building wheels and sdists, there are also additional dependencies
 # in the pyproject extra. And cmake and possibly ninja if those are not already
 # present (user controllable)
@@ -73,14 +74,15 @@
     "rich",
 ]
 docs = [
     "furo",
     "myst_parser >=0.13",
     "sphinx >=4.0",
     "sphinx_copybutton",
+    "sphinx_inline_tabs",
 ]
 
 [project.urls]
 Homepage = "https://github.com/scikit-build/scikit-build-core"
 Examples = "https://github.com/scikit-build/scikit-build-core/tree/main/tests/packages"
 
 [project.entry-points."distutils.setup_keywords"]
@@ -97,24 +99,27 @@
 minversion = "7.0"
 addopts = ["-ra", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = [
     "error",
     "ignore:pkg_resources is deprecated as an API:DeprecationWarning",  # Caused by wheel in tests
     "ignore:Config variable '.*' is unset, Python ABI tag may be incorrect:RuntimeWarning",
+    "ignore:onerror argument is deprecated, use onexc instead:DeprecationWarning",  # Caused by wheel and Python 3.12
 ]
 log_cli_level = "info"
 testpaths = ["tests"]
 markers = [
+    "broken_on_urct: Broken for now due to lib not found",
     "compile: Compiles code",
     "configure: Configures CMake code",
+    "fortran: Fortran code",
     "integration: Full package build",
+    "isolated: Needs an isolated virtualenv",
     "setuptools: Tests setuptools integration",
     "virtualenv: Needs a virtualenv",
-    "isolated: Needs an isolated virtualenv",
 ]
 
 
 [tool.mypy]
 files = ["src", "tests"]
 mypy_path = ["$MYPY_CONFIG_FILE_DIR/src"]
 python_version = "3.7"
@@ -125,15 +130,15 @@
 disallow_untyped_defs = false
 
 [[tool.mypy.overrides]]
 module = ["scikit_build_core.*"]
 disallow_untyped_defs = true
 
 [[tool.mypy.overrides]]
-module = ["pathspec"]
+module = ["numpy", "pathspec", "setuptools_scm", "hatch_fancy_pypi_readme"]
 ignore_missing_imports = true
 
 
 [tool.pylint]
 py-version = "3.7"
 jobs = "0"
 reports.output-format = "colorized"
@@ -154,14 +159,15 @@
     "broad-except",
     "unused-argument",  # Handled by Ruff
     "redefined-builtin",  # ExceptionGroup is a builtin
 ]
 
 
 [tool.coverage]
+run.source = ["scikit_build_core"]
 report.exclude_lines = [
     'pragma: no cover',
     '\.\.\.',
     'if typing.TYPE_CHECKING:',
 ]
 
 
@@ -188,22 +194,26 @@
     "RUF",         # Ruff-specific
     "SIM",         # flake8-simplify
     "T20",         # flake8-print
     "UP",          # pyupgrade
     "YTT",         # flake8-2020
 ]
 extend-ignore = [
-    "PLR0915",
-    "PLR0912",
-    "PLR2004",
-    "PLE1205",  # Format check doesn't work with our custom logger
-    "E501",  # Line too long
+    "PLR",     # Design rules for pylint
+    "PLE1205", # Format check doesn't work with our custom logger
+    "E501",    # Line too long
+    "PT004",
 ]
 target-version = "py37"
 typing-modules = ["scikit_build_core._compat.typing"]
 src = ["src"]
 unfixable = ["T20", "F841"]
 exclude = []
 
 [tool.ruff.per-file-ignores]
 "tests/**" = ["T20"]
 "noxfile.py" = ["T20"]
+"src/scikit_build_core/resources/*.py" = ["PTH", "ARG002"]
+
+
+[tool.check-sdist]
+sdist-only = ["src/scikit_build_core/_version.py"]
```

### Comparing `scikit_build_core-0.2.2/PKG-INFO` & `scikit_build_core-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_build_core
-Version: 0.2.2
+Version: 0.3.0
 Summary: Build backend for CMake based projects
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Examples, https://github.com/scikit-build/scikit-build-core/tree/main/tests/packages
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Requires-Dist: exceptiongroup; python_version < '3.11'
+Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: importlib-resources>=1.3; python_version < '3.9'
 Requires-Dist: packaging>=20.9
 Requires-Dist: tomli>=1.1; python_version < '3.11'
 Requires-Dist: typing-extensions>=3.10.0; python_version < '3.8'
 Provides-Extra: cov
 Requires-Dist: pytest-cov[toml]; extra == 'cov'
 Provides-Extra: dev
@@ -36,14 +37,15 @@
 Requires-Dist: pytest-subprocess; extra == 'dev'
 Requires-Dist: pytest>=7.0; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
+Requires-Dist: sphinx-inline-tabs; extra == 'docs'
 Requires-Dist: sphinx>=4.0; extra == 'docs'
 Provides-Extra: pyproject
 Requires-Dist: pathspec>=0.10.1; extra == 'pyproject'
 Requires-Dist: pyproject-metadata>=0.5; extra == 'pyproject'
 Provides-Extra: rich
 Requires-Dist: rich; extra == 'rich'
 Provides-Extra: test
@@ -57,68 +59,71 @@
 Requires-Dist: pytest>=7.0; extra == 'test'
 Requires-Dist: setuptools; extra == 'test'
 Requires-Dist: wheel; extra == 'test'
 Description-Content-Type: text/markdown
 
 # scikit-build-core
 
+[![Documentation Status][rtd-badge]][rtd-link]
+
 [![Actions Status][actions-badge]][actions-link]
 [![Code style: black][black-badge]][black-link]
 [![codecov][codecov-badge]][codecov-link]
 [![GitHub Discussion][github-discussions-badge]][github-discussions-link]
 
 [![PyPI version][pypi-version]][pypi-link]
 [![Conda-Forge][conda-badge]][conda-link]
 [![PyPI platforms][pypi-platforms]][pypi-link]
 
 <!-- Not implemented yet
-[![Documentation Status][rtd-badge]][rtd-link]
 [![Gitter][gitter-badge]][gitter-link]
 -->
 
 <!-- SPHINX-START -->
 
 Features over classic Scikit-build:
 
 - Better warnings, errors, and logging
 - No warning about unused variables
 - Automatically adds Ninja and/or CMake only as required
-- No dependency on setuptools, distutils, or wheel in build mode.
-- Powerful config system, including config options support in build mode.
+- No dependency on setuptools, distutils, or wheel.
+- Powerful config system, including config options support.
 - Automatic inclusion of site-packages in `CMAKE_PREFIX_PATH`
-- FindPython is backported if running on CMake < 3.26 (configurable), supports
-  PyPY SOABI.
+- FindPython is backported if running on CMake < 3.26.1 (configurable), supports
+  PyPY SOABI & Limited API / Stable ABI.
 - Limited API / Stable ABI and pythonless tags supported via config option
 - No slow generator search, ninja/make or MSVC used by default, respects
   `CMAKE_GENERATOR`
 - SDists are reproducible by default (UNIX, Python 3.9+)
 - Support for caching between builds (opt-in by setting `build-dir`)
 - Support for writing out to extra wheel folders (scripts, headers, data)
+- Dedicated entrypoints for module and prefix directories
+- Several integrated dynamic metadata plugins (proposing standardized support
+  soon)
+- Experimental editable mode support, with optional experimental auto rebuilds
+  on import.
 
 The following limitations are present compared to classic scikit-build:
 
 - The minimum supported CMake is 3.15
 - The minimum supported Python is 3.7
 
 Some known missing features that will be developed soon:
 
-- No editable mode support
-- The docs are not written
-- Dedicated entrypoints are planned for projects wanting to support discovery
 - No support for other targets besides install
 - Wheels are not fully reproducible yet
-- Dynamic metadata support is being developed
+- Several editable mode caveats (mentioned in the docs)
 
 Other backends are also planned:
 
 - Setuptools integration highly experimental
 - The extensionlib integration is missing
 - No hatchling plugin yet
 
-The recommended interface is the PEP 517 interface. There is also a WIP
+The recommended interface is the native pyproject builder. There is also a WIP
 setuptools-based interface that is being developed to provide a transition path
 for classic scikit-build.
 
 **WARNING**: Only the pyproject-based builder should be used; the setuptools
 backend is experimental and likely to move to a separate package before being
 declared stable, and internal API is still being solidified. A future version of
 this package will support creating new build extensions.
@@ -144,26 +149,24 @@
 the minimum to get started. You can also add the `rich` (more colorful
 printouts) or `pyproject` (pre-load some dependencies) extras if you want.
 
 An example `CMakeLists.txt`:
 
 ```cmake
 cmake_minimum_required(VERSION 3.15...3.26)
+project(${SKBUILD_PROJECT_NAME} LANGUAGES C)
 
-project(${SKBUILD_PROJECT_NAME} LANGUAGES C VERSION ${SKBUILD_PROJECT_VERSION})
-
-find_package(Python COMPONENTS Interpreter Development.Module)
+find_package(Python COMPONENTS Interpreter Development.Module REQUIRED)
 
 Python_add_library(_module MODULE src/module.c WITH_SOABI)
-
 install(TARGETS _module DESTINATION ${SKBUILD_PROJECT_NAME})
 ```
 
-Scikit-build-core will backport FindPython from CMake 3.26 to older versions of
-Python, and will handle PyPy for you if you are building from PyPy. You will
+Scikit-build-core will backport FindPython from CMake 3.26.1 to older versions
+of Python, and will handle PyPy for you if you are building from PyPy. You will
 need to install everything you want into the full final path inside site-modules
 (so you will usually prefix everything by the package name).
 
 More examples are in the
 [tests/packages](https://github.com/scikit-build/scikit-build-core/tree/main/tests/packages).
 
 ## Configuration
@@ -226,32 +229,44 @@
 # original dir is still at SKBUILD_PLATLIB_DIR (also SKBUILD_DATA_DIR, etc. are
 # available)
 wheel.install-dir = "."
 
 # This will backport an internal copy of FindPython if CMake is less than this
 # value. Set to 0 or the empty string to disable. The default will be kept in
 # sync with the version of FindPython stored in scikit-build-core.
-backport.find-python = "3.26"
+backport.find-python = "3.26.1"
+
+# This is the only editable mode currently
+editable.mode = "redirect"
+
+# Enable auto rebuilds on import (experimental)
+editable.rebuild = false
+
+# Display output on stderr while rebuilding on import
+editable.verbose = true
 
 # Enable experimental features if any are available
 experimental = false
 
 # Strictly validate config options
 strict-config = true
 
 # This provides some backward compatibility if set. Defaults to the latest
 # scikit-build-core version.
 minimum-version = "0.2"  # current version
 
-# Build directory (empty will use a temporary directory). {cache_tag} is
-# available to provide a unique directory per interpreter.
+# Build directory (empty will use a temporary directory). {cache_tag} and
+# {wheel_tag} are available to provide a unique directory per interpreter.
 build-dir = ""
 
 [tool.scikit-build.cmake.define]
 # Put CMake defines in this table.
+
+[tool.scikit-build.metadata]
+# List dynamic metadata fields and hook locations in this table
 ```
 
 Most CMake environment variables should be supported, and `CMAKE_ARGS` can be
 used to set extra CMake args. `ARCHFLAGS` is used to specify macOS universal2 or
 cross-compiles, just like setuptools.
 
 ## Acknowledgements
```

