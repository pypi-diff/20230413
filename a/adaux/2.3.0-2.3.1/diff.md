# Comparing `tmp/adaux-2.3.0.tar.gz` & `tmp/adaux-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaux-2.3.0.tar", last modified: Wed Apr 12 21:34:40 2023, max compression
+gzip compressed data, was "adaux-2.3.1.tar", last modified: Wed Apr 12 23:48:21 2023, max compression
```

## Comparing `adaux-2.3.0.tar` & `adaux-2.3.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.981871 adaux-2.3.0/
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-10 20:31:51.000000 adaux-2.3.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-12 21:34:40.981871 adaux-2.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-12 21:34:40.985871 adaux-2.3.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.797864 adaux-2.3.0/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.857867 adaux-2.3.0/source/adaux/
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-12 15:47:50.000000 adaux-2.3.0/source/adaux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_base_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    14762 2023-04-12 21:29:55.000000 adaux-2.3.0/source/adaux/_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14469 2023-04-12 21:20:17.000000 adaux-2.3.0/source/adaux/_cli_mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.909868 adaux-2.3.0/source/adaux/_components/
--rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_00_extra_level.py
--rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_01_file_io_support.py
--rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_02_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_03_meta.py
--rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_04_monotonic_version.py
--rw-rw-rw-   0 root         (0) root         (0)     6665 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_05_project.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_06_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_07_package.py
--rw-rw-rw-   0 root         (0) root         (0)     3686 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_08_pip.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_09_gitignore.py
--rw-rw-rw-   0 root         (0) root         (0)     4135 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_10_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)     5813 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_11_precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     6494 2023-04-12 21:27:08.000000 adaux-2.3.0/source/adaux/_components/_12_pylint.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_13_executable.py
--rw-rw-rw-   0 root         (0) root         (0)     2305 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_14_mypy.py
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_15_pytest.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_16_coverage.py
--rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_17_docs.py
--rw-rw-rw-   0 root         (0) root         (0)    19733 2023-04-12 21:20:17.000000 adaux-2.3.0/source/adaux/_components/_18_payload.py
--rw-rw-rw-   0 root         (0) root         (0)    15938 2023-04-12 20:52:41.000000 adaux-2.3.0/source/adaux/_components/_19_docker.py
--rw-rw-rw-   0 root         (0) root         (0)    11985 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_20_ci.py
--rw-rw-rw-   0 root         (0) root         (0)     3637 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_98_sentinel.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_99_all.py
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12836 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_components/_aux_ci.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.917869 adaux-2.3.0/source/adaux/_components/_payload/
--rw-rw-rw-   0 root         (0) root         (0)      683 2023-04-12 15:47:50.000000 adaux-2.3.0/source/adaux/_components/_payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_docker.py
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-04-11 12:28:10.000000 adaux-2.3.0/source/adaux/_components/_payload/_docker_build.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_docker_compose.py
--rw-rw-rw-   0 root         (0) root         (0)    15703 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_docker_executors.py
--rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-11 12:28:10.000000 adaux-2.3.0/source/adaux/_components/_payload/_docker_run.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_python.py
--rw-rw-rw-   0 root         (0) root         (0)     1358 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_components/_payload/_with_dependency.py
--rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-10 20:31:51.000000 adaux-2.3.0/source/adaux/_create_badge.py
--rw-rw-rw-   0 root         (0) root         (0)    14742 2023-04-11 12:31:50.000000 adaux-2.3.0/source/adaux/_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     7090 2023-04-12 09:55:20.000000 adaux-2.3.0/source/adaux/_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_proto_namespace.py
--rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_tick.py
--rw-rw-rw-   0 root         (0) root         (0)     3388 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_todo.py
--rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_util.py
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.921869 adaux-2.3.0/source/adaux/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.921869 adaux-2.3.0/source/adaux/src/CI/
--rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/CI/00-main.yml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/CI/01-rules.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.921869 adaux-2.3.0/source/adaux/src/CI/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/CI/jinja-snippets/coverage.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/CI/jinja-snippets/tags.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.925869 adaux-2.3.0/source/adaux/src/docker/
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/comp-helper.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.805865 adaux-2.3.0/source/adaux/src/docker/services/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.925869 adaux-2.3.0/source/adaux/src/docker/services/ansible-deploy/
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.929869 adaux-2.3.0/source/adaux/src/docker/services/docs/
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.933869 adaux-2.3.0/source/adaux/src/docker/services/gitlab-release-run/
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.937869 adaux-2.3.0/source/adaux/src/docker/services/image/
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/image/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.941870 adaux-2.3.0/source/adaux/src/docker/services/image-pytest/
--rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.957870 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.957870 adaux-2.3.0/source/adaux/src/docker/services/pkg-gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.957870 adaux-2.3.0/source/adaux/src/docker/services/pkg-pypi/
--rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.961870 adaux-2.3.0/source/adaux/src/docker/services/pre-commit/
--rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.961870 adaux-2.3.0/source/adaux/src/docker/services/pycov/
--rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.965870 adaux-2.3.0/source/adaux/src/docker/services/pytest/
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.965870 adaux-2.3.0/source/adaux/src/docker/services/pytest-standalone/
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.969870 adaux-2.3.0/source/adaux/src/docker/services/python-deps/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.969870 adaux-2.3.0/source/adaux/src/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/default_conf.py.jinja2
--rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/postprocess_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.969870 adaux-2.3.0/source/adaux/src/docs/static/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/static/git-link-color.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.973871 adaux-2.3.0/source/adaux/src/docs/user/
--rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/user/conf.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/user/gitignore
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/docs/user/index.rst.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-12 15:47:50.000000 adaux-2.3.0/source/adaux/src/gitignore
--rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/install-dev.sh.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.973871 adaux-2.3.0/source/adaux/src/license/
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/license/Apache-2.0.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/license/BSD-3_clause.txt.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/license/MIT.txt.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.809865 adaux-2.3.0/source/adaux/src/payload/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.977871 adaux-2.3.0/source/adaux/src/payload/python/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.977871 adaux-2.3.0/source/adaux/src/payload/python/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     2601 2023-04-12 21:33:51.000000 adaux-2.3.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
--rw-rw-rw-   0 root         (0) root         (0)     3117 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/payload/python/functions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.977871 adaux-2.3.0/source/adaux/src/pip/
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/pip/pip.conf.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.981871 adaux-2.3.0/source/adaux/src/pre-commit/
--rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/pre-commit/config.yaml.jinja2
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/pre-commit/mypy.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.981871 adaux-2.3.0/source/adaux/src/root/
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/root/_setup.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/root/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/root/setup.cfg.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.981871 adaux-2.3.0/source/adaux/src/root/source/
--rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/root/source/gitignore.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-10 20:31:52.000000 adaux-2.3.0/source/adaux/src/temp-combination
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 21:34:40.869867 adaux-2.3.0/source/adaux.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5236 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 21:33:50.000000 adaux-2.3.0/source/adaux.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      203 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-12 21:34:40.000000 adaux-2.3.0/source/adaux.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.537555 adaux-2.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-04-10 20:31:51.000000 adaux-2.3.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-12 23:48:21.537555 adaux-2.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      974 2023-04-12 23:48:21.541556 adaux-2.3.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      144 2022-07-30 13:12:02.000000 adaux-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.441552 adaux-2.3.1/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.473553 adaux-2.3.1/source/adaux/
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-04-12 22:22:11.000000 adaux-2.3.1/source/adaux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_base_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14627 2023-04-12 22:22:11.000000 adaux-2.3.1/source/adaux/_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14469 2023-04-12 21:20:17.000000 adaux-2.3.1/source/adaux/_cli_mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.493554 adaux-2.3.1/source/adaux/_components/
+-rw-rw-rw-   0 root         (0) root         (0)      261 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_00_extra_level.py
+-rw-rw-rw-   0 root         (0) root         (0)     4879 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_01_file_io_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_02_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3208 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_03_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_04_monotonic_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6665 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_05_project.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_06_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     1192 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_07_package.py
+-rw-rw-rw-   0 root         (0) root         (0)     3686 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_08_pip.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_09_gitignore.py
+-rw-rw-rw-   0 root         (0) root         (0)     4135 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_10_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5813 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_11_precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6494 2023-04-12 21:27:08.000000 adaux-2.3.1/source/adaux/_components/_12_pylint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_13_executable.py
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_14_mypy.py
+-rw-rw-rw-   0 root         (0) root         (0)     3025 2023-04-12 23:18:12.000000 adaux-2.3.1/source/adaux/_components/_15_pytest.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_16_coverage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2801 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_17_docs.py
+-rw-rw-rw-   0 root         (0) root         (0)    20343 2023-04-12 23:43:59.000000 adaux-2.3.1/source/adaux/_components/_18_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)    15938 2023-04-12 23:43:59.000000 adaux-2.3.1/source/adaux/_components/_19_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)    11985 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_20_ci.py
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_98_sentinel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_99_all.py
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12836 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_components/_aux_ci.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.501554 adaux-2.3.1/source/adaux/_components/_payload/
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-04-12 15:47:50.000000 adaux-2.3.1/source/adaux/_components/_payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_payload/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_payload/_docker.py
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2023-04-11 12:28:10.000000 adaux-2.3.1/source/adaux/_components/_payload/_docker_build.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_payload/_docker_compose.py
+-rw-rw-rw-   0 root         (0) root         (0)    15814 2023-04-12 23:05:47.000000 adaux-2.3.1/source/adaux/_components/_payload/_docker_executors.py
+-rw-rw-rw-   0 root         (0) root         (0)      490 2023-04-11 12:28:10.000000 adaux-2.3.1/source/adaux/_components/_payload/_docker_run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_payload/_python.py
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_components/_payload/_with_dependency.py
+-rwxrwxrwx   0 root         (0) root         (0)     1629 2023-04-10 20:31:51.000000 adaux-2.3.1/source/adaux/_create_badge.py
+-rw-rw-rw-   0 root         (0) root         (0)    14742 2023-04-11 12:31:50.000000 adaux-2.3.1/source/adaux/_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     7090 2023-04-12 09:55:20.000000 adaux-2.3.1/source/adaux/_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     1245 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/_proto_namespace.py
+-rw-rw-rw-   0 root         (0) root         (0)     2464 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/_tick.py
+-rw-rw-rw-   0 root         (0) root         (0)     3388 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/_todo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/_util.py
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.501554 adaux-2.3.1/source/adaux/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.505554 adaux-2.3.1/source/adaux/src/CI/
+-rw-rw-rw-   0 root         (0) root         (0)     2316 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/CI/00-main.yml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/CI/01-rules.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.505554 adaux-2.3.1/source/adaux/src/CI/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/CI/jinja-snippets/coverage.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       94 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/CI/jinja-snippets/tags.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.505554 adaux-2.3.1/source/adaux/src/docker/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/comp-helper.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.457553 adaux-2.3.1/source/adaux/src/docker/services/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.505554 adaux-2.3.1/source/adaux/src/docker/services/ansible-deploy/
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.509554 adaux-2.3.1/source/adaux/src/docker/services/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/docs/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/docs/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.509554 adaux-2.3.1/source/adaux/src/docker/services/gitlab-release-run/
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.509554 adaux-2.3.1/source/adaux/src/docker/services/image/
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/image/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      407 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/image/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.513554 adaux-2.3.1/source/adaux/src/docker/services/image-pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      617 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/image-pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.517555 adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/apt_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/apt_install_root.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/base_arg.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/extra_script.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      437 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      326 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/pip_install.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/platform.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/pytest_command.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/sdist_untar.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.517555 adaux-2.3.1/source/adaux/src/docker/services/pkg-gitlab/
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.521555 adaux-2.3.1/source/adaux/src/docker/services/pkg-pypi/
+-rw-rw-rw-   0 root         (0) root         (0)      485 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/pkg-pypi/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.521555 adaux-2.3.1/source/adaux/src/docker/services/pre-commit/
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      599 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.521555 adaux-2.3.1/source/adaux/src/docker/services/pycov/
+-rw-rw-rw-   0 root         (0) root         (0)      482 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/pycov/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.521555 adaux-2.3.1/source/adaux/src/docker/services/pytest/
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/pytest/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/pytest/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.525555 adaux-2.3.1/source/adaux/src/docker/services/pytest-standalone/
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      409 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/pytest-standalone/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.525555 adaux-2.3.1/source/adaux/src/docker/services/python-deps/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      211 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docker/services/python-deps/docker-compose.yml.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.525555 adaux-2.3.1/source/adaux/src/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4843 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docs/default_conf.py.jinja2
+-rwxrwxrwx   0 root         (0) root         (0)     1873 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docs/postprocess_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.529555 adaux-2.3.1/source/adaux/src/docs/static/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docs/static/git-link-color.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.529555 adaux-2.3.1/source/adaux/src/docs/user/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docs/user/conf.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docs/user/gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/docs/user/index.rst.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-04-12 15:47:50.000000 adaux-2.3.1/source/adaux/src/gitignore
+-rwxrwxrwx   0 root         (0) root         (0)      410 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/install-dev.sh.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.533555 adaux-2.3.1/source/adaux/src/license/
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/license/Apache-2.0.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1495 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/license/BSD-3_clause.txt.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/license/MIT.txt.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.457553 adaux-2.3.1/source/adaux/src/payload/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.533555 adaux-2.3.1/source/adaux/src/payload/python/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.533555 adaux-2.3.1/source/adaux/src/payload/python/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-04-12 23:47:45.000000 adaux-2.3.1/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2023-04-12 23:05:47.000000 adaux-2.3.1/source/adaux/src/payload/python/functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.533555 adaux-2.3.1/source/adaux/src/pip/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/pip/pip.conf.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.537555 adaux-2.3.1/source/adaux/src/pre-commit/
+-rwxrwxrwx   0 root         (0) root         (0)     1680 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/pre-commit/add_copy_right.py.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     5098 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/pre-commit/config.yaml.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/pre-commit/mypy.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.537555 adaux-2.3.1/source/adaux/src/root/
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/root/_setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/root/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      487 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/root/setup.cfg.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.537555 adaux-2.3.1/source/adaux/src/root/source/
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/root/source/gitignore.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-10 20:31:52.000000 adaux-2.3.1/source/adaux/src/temp-combination
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 23:48:21.477553 adaux-2.3.1/source/adaux.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2023-04-12 23:48:20.000000 adaux-2.3.1/source/adaux.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5236 2023-04-12 23:48:21.000000 adaux-2.3.1/source/adaux.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 23:48:21.000000 adaux-2.3.1/source/adaux.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-12 23:48:21.000000 adaux-2.3.1/source/adaux.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 23:47:44.000000 adaux-2.3.1/source/adaux.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      203 2023-04-12 23:48:21.000000 adaux-2.3.1/source/adaux.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-12 23:48:21.000000 adaux-2.3.1/source/adaux.egg-info/top_level.txt
```

### Comparing `adaux-2.3.0/LICENSE.txt` & `adaux-2.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/setup.cfg` & `adaux-2.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_base_parser.py` & `adaux-2.3.1/source/adaux/_base_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_cli.py` & `adaux-2.3.1/source/adaux/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,21 +376,14 @@
     is_flag=True,
     default=False,
     help="show what payloads would run, without running them",
 )
 @click.option(
     "-l", "--show-all", is_flag=True, default=False, help="show all available payloads"
 )
-@click.option(
-    "-p",
-    "--plantuml",
-    is_flag=True,
-    default=False,
-    help="generate a png with the dependency graph",
-)
 def run(  # pylint: disable=too-many-arguments
     ctx: click.Context,
     payload_names: tp.Tuple[str, ...],
     force: bool,
     dry: bool,
     show_all: bool,
 ) -> None:
```

### Comparing `adaux-2.3.0/source/adaux/_cli_mixin.py` & `adaux-2.3.1/source/adaux/_cli_mixin.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_01_file_io_support.py` & `adaux-2.3.1/source/adaux/_components/_01_file_io_support.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_02_base.py` & `adaux-2.3.1/source/adaux/_components/_02_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_03_meta.py` & `adaux-2.3.1/source/adaux/_components/_03_meta.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_04_monotonic_version.py` & `adaux-2.3.1/source/adaux/_components/_04_monotonic_version.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_05_project.py` & `adaux-2.3.1/source/adaux/_components/_05_project.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_06_dependency.py` & `adaux-2.3.1/source/adaux/_components/_06_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_07_package.py` & `adaux-2.3.1/source/adaux/_components/_07_package.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_08_pip.py` & `adaux-2.3.1/source/adaux/_components/_08_pip.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_09_gitignore.py` & `adaux-2.3.1/source/adaux/_components/_09_gitignore.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_10_gitlab.py` & `adaux-2.3.1/source/adaux/_components/_10_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_11_precommit.py` & `adaux-2.3.1/source/adaux/_components/_11_precommit.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_12_pylint.py` & `adaux-2.3.1/source/adaux/_components/_12_pylint.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_13_executable.py` & `adaux-2.3.1/source/adaux/_components/_13_executable.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_14_mypy.py` & `adaux-2.3.1/source/adaux/_components/_14_mypy.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_15_pytest.py` & `adaux-2.3.1/source/adaux/_components/_15_pytest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,25 @@
     def templated(self, negative_default: bool = False) -> None:
         super().templated(negative_default)
         data = self.auxcon.pytest = _ProtoNamespace()
         self.auxcon.dependencies.test.append(self.versions.pytest)
         data.markers = _ProtoNamespace({"merge_only": "run test only on merge request"})
         data.addopts = '--strict-markers -m "not merge_only"'
 
+    def update_to_template(self, tpl: _ProtoNamespace, full: _ProtoNamespace) -> None:
+        super().update_to_template(tpl, full)
+        self.auxf.setdefault("pytest", _ProtoNamespace())
+        data = self.auxf.pytest
+        if "markers" not in data:
+            data.setdefault("markers", tpl.pytest.markers)
+            self._print(f"added pytest.markers: {data.markers}", fg="green")
+        if "addopts" not in data:
+            data.setdefault("addopts", tpl.pytest.addopts)
+            self._print(f"added pytest.markers: {data.addopts}", fg="green")
+
     def demodata(self) -> None:
         super().demodata()
         data = self.auxcon.pytest
         data.asyncio_mode = "strict"
 
     def formatted(self) -> None:
         super().formatted()
```

### Comparing `adaux-2.3.0/source/adaux/_components/_17_docs.py` & `adaux-2.3.1/source/adaux/_components/_17_docs.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_18_payload.py` & `adaux-2.3.1/source/adaux/_components/_18_payload.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,16 +308,29 @@
             assert isinstance(res, Payload)
             lookup.update({key: res}, flavor=flavor, unique=True)
             return res
 
         for flavor in self.payload_types():
             for key, val in data[flavor].items():
                 create_payload(val, flavor)
+
         data.lookup = lookup
         for val in lookup.level("with_dependency").values():
+            # promote potential lvl=0 to lvl=1
+            orig_deps = val.deps
+            val.deps = tuple(lookup[x.name] for x in orig_deps)
+            for dep1, dep2 in zip(orig_deps, val.deps):
+                if dep1 is not dep2:
+                    logger.info(
+                        "%s upgraded deps %s (%s -> %s)",
+                        val.name,
+                        dep1.name,
+                        dep1.flavor,
+                        dep2.flavor,
+                    )
             val.hydrate()
         for val in lookup.level("docker_build").values():
             val.hydrate()
 
     def payload_run(self, *payloads: Payload, force: bool, dry: bool = False) -> bool:
         # pylint: disable=import-outside-toplevel
         from ._aux_ci import JobManager, CommonJob
@@ -348,23 +361,24 @@
                         return True, "--force"
                     return True, f"missing {self.payload.executor.tag}"
 
                 return super().is_included(env)
 
         jman = JobManager(env=dict(verbose=True))
 
-        def demo(*pld: Payload) -> tp.List[PayloadJob]:
+        def payloads2jobman(*pld: Payload) -> tp.List[PayloadJob]:
             jobs = []
             for pl in pld:
                 if isinstance(pl, WithDependencyPayload):
-                    parents = demo(*pl.deps)
+                    parents = payloads2jobman(*pl.deps)
                     name = pl.payload.name
                     if name in jman.jobs:
                         x = jman.jobs[name]
                     else:
+                        print(name, [(x.name, x.payload.flavor) for x in parents])
                         x = jman.add_job(
                             PayloadJob,
                             payload=pl.payload,
                             force=force,
                             name=pl.payload.name,
                             parents=parents,
                         )
@@ -376,15 +390,15 @@
                     else:
                         x = jman.add_job(
                             PayloadJob, payload=pl, force=force, name=pl.name
                         )
                     jobs.append(x)
             return jobs  # type: ignore
 
-        demo(*payloads)
+        payloads2jobman(*payloads)
 
         if dry:
             jman.prune_unincluded(show=True)
         else:
             jman.run_pipeline(show=True)
             jman.show_result()
```

### Comparing `adaux-2.3.0/source/adaux/_components/_19_docker.py` & `adaux-2.3.1/source/adaux/_components/_19_docker.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         data.setdefault("python", _ProtoNamespace())
         data.python["check-release-notes"] = _ProtoNamespace()
 
         if self.is_enabled("pre-commit"):
             data.setdefault("with_dependency", _ProtoNamespace())
             run = "pre-commit"
             build = f"build-{run}"
-            data.with_dependency[run] = dict(variant={"all": dict(cmd="--all")})
             data.with_dependency[build] = dict(deps=["build-python-deps"])
+            data.with_dependency[run] = dict(variant={"all": dict(cmd="--all")})
 
         if self.is_enabled("pytest"):
             data.setdefault("with_dependency", _ProtoNamespace())
             run = "pytest"
             build = f"build-{run}"
             data.with_dependency[build] = dict(deps=["build-python-deps"])
             data.with_dependency[run] = dict()
```

### Comparing `adaux-2.3.0/source/adaux/_components/_20_ci.py` & `adaux-2.3.1/source/adaux/_components/_20_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_98_sentinel.py` & `adaux-2.3.1/source/adaux/_components/_98_sentinel.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_99_all.py` & `adaux-2.3.1/source/adaux/_components/_99_all.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_aux_ci.py` & `adaux-2.3.1/source/adaux/_components/_aux_ci.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_payload/__init__.py` & `adaux-2.3.1/source/adaux/_components/_payload/__init__.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_payload/_base.py` & `adaux-2.3.1/source/adaux/_components/_payload/_base.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_payload/_docker.py` & `adaux-2.3.1/source/adaux/_components/_payload/_docker.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_payload/_docker_build.py` & `adaux-2.3.1/source/adaux/_components/_payload/_docker_build.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_payload/_docker_executors.py` & `adaux-2.3.1/source/adaux/_components/_payload/_docker_executors.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,31 +88,32 @@
             # download other images which are not a direct dependency (cross-repo)
             for image_tag in self.images:
                 image_remote_tag = (
                     f"{self.registry_host}/{self._remove_namespace_local(image_tag)}"
                 )
                 check_and_pull_if_not_existent(image_remote_tag, image_tag)
 
-        # build
-        cmd = [
-            "docker",
-            "--log-level",
-            "ERROR",
-            "compose",
-            "-p",
-            self.slug,
-            "-f",
-            "devops/docker/compose.yml",
-            "build",
-            self.service,
-        ]
-        subprocess_run(cmd, check=True)
+        if not exists_locally(self.local_tag):
+            # build
+            cmd = [
+                "docker",
+                "--log-level",
+                "ERROR",
+                "compose",
+                "-p",
+                self.slug,
+                "-f",
+                "devops/docker/compose.yml",
+                "build",
+                self.service,
+            ]
+            subprocess_run(cmd, check=True)
 
-        # upload
-        tag_image(self.use_tag, local_tag)
+            # upload
+            tag_image(self.use_tag, local_tag)
         if self.remote_exists():
             upload_to_remote(local_tag, remote_tag)
             logger.info("uploaded %s to %s", local_tag, remote_tag)
 
     @functools.cached_property
     def tag(self) -> str:
         hasher = hashlib.md5()
```

### Comparing `adaux-2.3.0/source/adaux/_components/_payload/_python.py` & `adaux-2.3.1/source/adaux/_components/_payload/_python.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_components/_payload/_with_dependency.py` & `adaux-2.3.1/source/adaux/_components/_payload/_with_dependency.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_create_badge.py` & `adaux-2.3.1/source/adaux/_create_badge.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_gitlab.py` & `adaux-2.3.1/source/adaux/_gitlab.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_parser.py` & `adaux-2.3.1/source/adaux/_parser.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_proto_namespace.py` & `adaux-2.3.1/source/adaux/_proto_namespace.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_tick.py` & `adaux-2.3.1/source/adaux/_tick.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_todo.py` & `adaux-2.3.1/source/adaux/_todo.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/_util.py` & `adaux-2.3.1/source/adaux/_util.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/CI/00-main.yml.jinja2` & `adaux-2.3.1/source/adaux/src/CI/00-main.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/CI/01-rules.yml.jinja2` & `adaux-2.3.1/source/adaux/src/CI/01-rules.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/ansible-deploy/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/ansible-deploy/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/docs/Dockerfile.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/docs/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/gitlab-release-run/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/image/Dockerfile.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/image/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/image-pytest/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/jinja-snippets/docker-build.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/pkg-gitlab/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/pre-commit/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/pre-commit/docker-compose.yml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/pytest-standalone/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2` & `adaux-2.3.1/source/adaux/src/docker/services/python-deps/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docs/default_conf.py.jinja2` & `adaux-2.3.1/source/adaux/src/docs/default_conf.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/docs/postprocess_html.py` & `adaux-2.3.1/source/adaux/src/docs/postprocess_html.py`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/license/Apache-2.0.txt.jinja2` & `adaux-2.3.1/source/adaux/src/license/Apache-2.0.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/license/BSD-3_clause.txt.jinja2` & `adaux-2.3.1/source/adaux/src/license/BSD-3_clause.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/license/MIT.txt.jinja2` & `adaux-2.3.1/source/adaux/src/license/MIT.txt.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc` & `adaux-2.3.1/source/adaux/src/payload/python/__pycache__/functions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Apr 10 20:31:52 2023 UTC, .py size: 3117 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3872 3464 2d0c 0000  o.......8r4d-...
+00000000: 6f0d 0d0a 0000 0000 4b39 3764 e60b 0000  o.......K97d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 b800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6402 6403 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6404 6c04 6d06 5a06 0100 6402  ..d.d.l.m.Z...d.
 00000060: 6405 6c04 6d07 5a07 0100 6402 6406 6c08  d.l.m.Z...d.d.l.
 00000070: 6d09 5a09 0100 6407 6509 6408 6401 6604  m.Z...d.e.d.d.f.
@@ -73,91 +73,87 @@
 00000480: da03 7275 6e29 0572 0700 0000 720e 0000  ..run).r....r...
 00000490: 0072 0f00 0000 da0b 6465 7363 7269 7074  .r......descript
 000004a0: 696f 6e72 1d00 0000 7218 0000 0072 1800  ionr....r....r..
 000004b0: 0000 7219 0000 00da 0e67 6974 6c61 625f  ..r......gitlab_
 000004c0: 7265 6c65 6173 651f 0000 0073 0e00 0000  release....s....
 000004d0: 0801 0801 0801 0a01 0a01 0c01 0c01 7221  ..............r!
 000004e0: 0000 00da 0464 6570 73da 0474 6167 7363  .....deps..tagsc
-000004f0: 0300 0000 0000 0000 0000 0000 0700 0000  ................
-00000500: 0600 0000 4300 0000 7392 0000 0074 007c  ....C...s....t.|
-00000510: 0274 0183 0272 087c 0267 017d 0274 027c  .t...r.|.g.}.t.|
-00000520: 0183 0164 016b 0372 1b74 0364 027c 029b  ...d.k.r.t.d.|..
-00000530: 0064 0374 027c 0183 019b 0064 049d 0583  .d.t.|.....d....
-00000540: 0182 0164 057d 037c 0244 005d 277d 047c  ...d.}.|.D.]'}.|
-00000550: 046a 047c 006a 056a 067c 006a 076a 0864  .j.|.j.j.|.j.j.d
-00000560: 068d 027d 047c 0164 0719 006a 09a0 0a7c  ...}.|.d...j...|
-00000570: 04a1 015c 027d 057d 067c 037c 056b 0372  ...\.}.}.|.|.k.r
-00000580: 417c 057d 0374 0b64 087c 0583 0201 0074  A|.}.t.d.|.....t
-00000590: 0b64 097c 0683 0201 0071 1f64 0053 0029  .d.|.....q.d.S.)
-000005a0: 0a4e e901 0000 007a 0c74 6167 206a 6f62  .N.....z.tag job
-000005b0: 2066 6f72 20fa 2720 7368 6f75 6c64 2068   for .' should h
-000005c0: 6176 6520 6578 6163 746c 7920 3120 6465  ave exactly 1 de
-000005d0: 7065 6e64 656e 6379 2c20 6e6f 7420 fa01  pendency, not ..
-000005e0: 21da 0029 0272 0f00 0000 da06 6272 616e  !..).r......bran
-000005f0: 6368 7201 0000 00da 0875 706c 6f61 6465  chr......uploade
-00000600: 64fa 0820 2020 2d3e 2074 6f29 0cda 0a69  d..   -> to)...i
-00000610: 7369 6e73 7461 6e63 65da 0373 7472 da03  sinstance..str..
-00000620: 6c65 6e72 1000 0000 da06 666f 726d 6174  lenr......format
-00000630: 720d 0000 0072 0f00 0000 da06 6769 746c  r....r......gitl
-00000640: 6162 da0e 6375 7272 656e 745f 6272 616e  ab..current_bran
-00000650: 6368 da08 6578 6563 7574 6f72 da0e 7461  ch..executor..ta
-00000660: 675f 616e 645f 7570 6c6f 6164 7216 0000  g_and_uploadr...
-00000670: 0029 0772 0700 0000 7222 0000 0072 2300  .).r....r"...r#.
-00000680: 0000 5a0e 6c61 7374 5f6c 6f63 616c 5f74  ..Z.last_local_t
-00000690: 6167 da03 7461 67da 096c 6f63 616c 5f74  ag..tag..local_t
-000006a0: 6167 da0b 7265 6c65 6173 655f 7461 6772  ag..release_tagr
-000006b0: 1800 0000 7218 0000 0072 1900 0000 7233  ....r....r....r3
-000006c0: 0000 0029 0000 0073 1e00 0000 0a05 0601  ...)...s........
-000006d0: 0c02 0201 1401 04ff 0403 0801 1601 1401  ................
-000006e0: 0801 0401 0a01 0c01 04fa 7233 0000 0072  ..........r3...r
-000006f0: 3500 0000 6303 0000 0000 0000 0000 0000  5...c...........
-00000700: 0004 0000 0008 0000 0043 0000 0073 a400  .........C...s..
-00000710: 0000 7400 7c01 8301 6401 6b03 7213 7401  ..t.|...d.k.r.t.
-00000720: 6402 7c02 9b00 6403 7400 7c01 8301 9b00  d.|...d.t.|.....
-00000730: 6404 9d05 8301 8201 7c02 6a02 7c00 6a03  d.......|.j.|.j.
-00000740: 6a04 7c00 6a05 6a06 6405 8d02 7d02 7c01  j.|.j.j.d...}.|.
-00000750: 6406 1900 6a07 a008 a100 7d03 7409 7c03  d...j.....}.t.|.
-00000760: 7c02 8302 0100 740a 6407 6408 6409 740b  |.....t.d.d.d.t.
-00000770: 6a0c 640a 1900 640b 740b 6a0c 640c 1900  j.d...d.t.j.d...
-00000780: 640d 6707 8301 0100 740d 7c03 7c02 8302  d.g.....t.|.|...
-00000790: 0100 740a 6700 640e a201 8301 0100 740e  ..t.g.d.......t.
-000007a0: 640f 7c03 8302 0100 740e 6410 7c02 8302  d.|.....t.d.|...
-000007b0: 0100 6400 5300 2911 4e72 2400 0000 7a16  ..d.S.).Nr$...z.
-000007c0: 696d 672d 646f 636b 6572 6875 6220 6a6f  img-dockerhub jo
-000007d0: 6220 666f 7220 7225 0000 0072 2600 0000  b for r%...r&...
-000007e0: 2902 720f 0000 00da 0e63 695f 6164 6175  ).r......ci_adau
-000007f0: 785f 696d 6167 6572 0100 0000 da06 646f  x_imager......do
-00000800: 636b 6572 da05 6c6f 6769 6e7a 022d 755a  cker..loginz.-uZ
-00000810: 1244 4f43 4b45 5248 5542 5f55 5345 524e  .DOCKERHUB_USERN
-00000820: 414d 457a 022d 705a 1244 4f43 4b45 5248  AMEz.-pZ.DOCKERH
-00000830: 5542 5f50 4153 5357 4f52 44fa 0964 6f63  UB_PASSWORD..doc
-00000840: 6b65 722e 696f 2903 7237 0000 005a 066c  ker.io).r7...Z.l
-00000850: 6f67 6f75 7472 3900 0000 7229 0000 0072  ogoutr9...r)...r
-00000860: 2a00 0000 290f 722d 0000 0072 1000 0000  *...).r-...r....
-00000870: 722e 0000 0072 0d00 0000 720f 0000 00da  r....r....r.....
-00000880: 0876 6572 7369 6f6e 7372 3600 0000 7231  .versionsr6...r1
-00000890: 0000 00da 1470 756c 6c5f 6966 5f6e 6f74  .....pull_if_not
-000008a0: 5f65 7869 7374 656e 7472 0400 0000 7203  _existentr....r.
-000008b0: 0000 0072 1b00 0000 721c 0000 0072 0500  ...r....r....r..
-000008c0: 0000 7216 0000 0029 0472 0700 0000 7222  ..r....).r....r"
-000008d0: 0000 0072 3500 0000 7234 0000 0072 1800  ...r5...r4...r..
-000008e0: 0000 7218 0000 0072 1900 0000 da0d 696d  ..r....r......im
-000008f0: 675f 646f 636b 6572 6875 623f 0000 0073  g_dockerhub?...s
-00000900: 2e00 0000 0c05 0201 1401 04ff 0403 0c01  ................
-00000910: 06ff 0e03 0a01 0201 0202 0201 0201 0801  ................
-00000920: 0201 0801 0201 02f9 04ff 0a0b 0c01 0a01  ................
-00000930: 0e01 723c 0000 0029 1272 1b00 0000 7212  ..r<...).r....r.
-00000940: 0000 00da 0674 7970 696e 67da 0274 705a  .....typing..tpZ
-00000950: 265f 636f 6d70 6f6e 656e 7473 2e5f 7061  &_components._pa
-00000960: 796c 6f61 642e 5f64 6f63 6b65 725f 6578  yload._docker_ex
-00000970: 6563 7574 6f72 7372 0300 0000 7204 0000  ecutorsr....r...
-00000980: 0072 0500 0000 da10 5f70 726f 746f 5f6e  .r......_proto_n
-00000990: 616d 6573 7061 6365 7206 0000 0072 1a00  amespacer....r..
-000009a0: 0000 7221 0000 00da 0341 6e79 da05 556e  ..r!.....Any..Un
-000009b0: 696f 6e72 2c00 0000 da08 5365 7175 656e  ionr,.....Sequen
-000009c0: 6365 7233 0000 0072 3c00 0000 7218 0000  cer3...r<...r...
-000009d0: 0072 1800 0000 7218 0000 0072 1900 0000  .r....r....r....
-000009e0: da08 3c6d 6f64 756c 653e 0100 0000 7336  ..<module>....s6
-000009f0: 0000 0008 0108 0108 010c 020c 010c 010c  ................
-00000a00: 0112 0312 1302 0a02 0102 ff04 0202 fe12  ................
-00000a10: 0302 fd02 040a fc02 1602 0102 ff04 0202  ................
-00000a20: fe02 0302 fd02 040e fc                   .........
+000004f0: 0300 0000 0000 0000 0000 0000 0800 0000  ................
+00000500: 0600 0000 4300 0000 7372 0000 0074 007c  ....C...sr...t.|
+00000510: 0274 0183 0272 087c 0267 017d 0264 017d  .t...r.|.g.}.d.}
+00000520: 037c 0144 005d 2a7d 047c 0244 005d 257d  .|.D.]*}.|.D.]%}
+00000530: 057c 056a 027c 006a 036a 047c 006a 056a  .|.j.|.j.j.|.j.j
+00000540: 0664 028d 027d 057c 046a 07a0 087c 05a1  .d...}.|.j...|..
+00000550: 015c 027d 067d 077c 037c 066b 0372 307c  .\.}.}.|.|.k.r0|
+00000560: 067d 0374 0964 037c 0683 0201 0074 0964  .}.t.d.|.....t.d
+00000570: 047c 0783 0201 0071 1071 0c64 0053 0029  .|.....q.q.d.S.)
+00000580: 054e da00 2902 720f 0000 00da 0662 7261  .N..).r......bra
+00000590: 6e63 68da 0875 706c 6f61 6465 64fa 0820  nch..uploaded.. 
+000005a0: 2020 2d3e 2074 6f29 0ada 0a69 7369 6e73    -> to)...isins
+000005b0: 7461 6e63 65da 0373 7472 da06 666f 726d  tance..str..form
+000005c0: 6174 720d 0000 0072 0f00 0000 da06 6769  atr....r......gi
+000005d0: 746c 6162 da0e 6375 7272 656e 745f 6272  tlab..current_br
+000005e0: 616e 6368 da08 6578 6563 7574 6f72 da0e  anch..executor..
+000005f0: 7461 675f 616e 645f 7570 6c6f 6164 7216  tag_and_uploadr.
+00000600: 0000 0029 0872 0700 0000 7222 0000 0072  ...).r....r"...r
+00000610: 2300 0000 5a0e 6c61 7374 5f6c 6f63 616c  #...Z.last_local
+00000620: 5f74 6167 da03 6465 70da 0374 6167 da09  _tag..dep..tag..
+00000630: 6c6f 6361 6c5f 7461 67da 0b72 656c 6561  local_tag..relea
+00000640: 7365 5f74 6167 7218 0000 0072 1800 0000  se_tagr....r....
+00000650: 7219 0000 0072 3000 0000 2900 0000 731e  r....r0...)...s.
+00000660: 0000 000a 0506 0104 0208 0108 0104 010c  ................
+00000670: 0106 ff10 0308 0104 010a 010c 0102 f804  ................
+00000680: ff72 3000 0000 7232 0000 0063 0300 0000  .r0...r2...c....
+00000690: 0000 0000 0000 0000 0400 0000 0800 0000  ................
+000006a0: 4300 0000 73a4 0000 0074 007c 0183 0164  C...s....t.|...d
+000006b0: 016b 0372 1374 0164 027c 029b 0064 0374  .k.r.t.d.|...d.t
+000006c0: 007c 0183 019b 0064 049d 0583 0182 017c  .|.....d.......|
+000006d0: 026a 027c 006a 036a 047c 006a 056a 0664  .j.|.j.j.|.j.j.d
+000006e0: 058d 027d 027c 0164 0619 006a 07a0 08a1  ...}.|.d...j....
+000006f0: 007d 0374 097c 037c 0283 0201 0074 0a64  .}.t.|.|.....t.d
+00000700: 0764 0864 0974 0b6a 0c64 0a19 0064 0b74  .d.d.t.j.d...d.t
+00000710: 0b6a 0c64 0c19 0064 0d67 0783 0101 0074  .j.d...d.g.....t
+00000720: 0d7c 037c 0283 0201 0074 0a67 0064 0ea2  .|.|.....t.g.d..
+00000730: 0183 0101 0074 0e64 0f7c 0383 0201 0074  .....t.d.|.....t
+00000740: 0e64 107c 0283 0201 0064 0053 0029 114e  .d.|.....d.S.).N
+00000750: e901 0000 007a 1669 6d67 2d64 6f63 6b65  .....z.img-docke
+00000760: 7268 7562 206a 6f62 2066 6f72 207a 2720  rhub job for z' 
+00000770: 7368 6f75 6c64 2068 6176 6520 6578 6163  should have exac
+00000780: 746c 7920 3120 6465 7065 6e64 656e 6379  tly 1 dependency
+00000790: 2c20 6e6f 7420 fa01 2129 0272 0f00 0000  , not ..!).r....
+000007a0: da0e 6369 5f61 6461 7578 5f69 6d61 6765  ..ci_adaux_image
+000007b0: 7201 0000 00da 0664 6f63 6b65 72da 056c  r......docker..l
+000007c0: 6f67 696e 7a02 2d75 5a12 444f 434b 4552  oginz.-uZ.DOCKER
+000007d0: 4855 425f 5553 4552 4e41 4d45 7a02 2d70  HUB_USERNAMEz.-p
+000007e0: 5a12 444f 434b 4552 4855 425f 5041 5353  Z.DOCKERHUB_PASS
+000007f0: 574f 5244 fa09 646f 636b 6572 2e69 6f29  WORD..docker.io)
+00000800: 0372 3600 0000 5a06 6c6f 676f 7574 7238  .r6...Z.logoutr8
+00000810: 0000 0072 2600 0000 7227 0000 0029 0fda  ...r&...r'...)..
+00000820: 036c 656e 7210 0000 0072 2a00 0000 720d  .lenr....r*...r.
+00000830: 0000 0072 0f00 0000 da08 7665 7273 696f  ...r......versio
+00000840: 6e73 7235 0000 0072 2d00 0000 da14 7075  nsr5...r-.....pu
+00000850: 6c6c 5f69 665f 6e6f 745f 6578 6973 7465  ll_if_not_existe
+00000860: 6e74 7204 0000 0072 0300 0000 721b 0000  ntr....r....r...
+00000870: 0072 1c00 0000 7205 0000 0072 1600 0000  .r....r....r....
+00000880: 2904 7207 0000 0072 2200 0000 7232 0000  ).r....r"...r2..
+00000890: 0072 3100 0000 7218 0000 0072 1800 0000  .r1...r....r....
+000008a0: 7219 0000 00da 0d69 6d67 5f64 6f63 6b65  r......img_docke
+000008b0: 7268 7562 3e00 0000 732e 0000 000c 0502  rhub>...s.......
+000008c0: 0114 0104 ff04 030c 0106 ff0e 030a 0102  ................
+000008d0: 0102 0202 0102 0108 0102 0108 0102 0102  ................
+000008e0: f904 ff0a 0b0c 010a 010e 0172 3c00 0000  ...........r<...
+000008f0: 2912 721b 0000 0072 1200 0000 da06 7479  ).r....r......ty
+00000900: 7069 6e67 da02 7470 5a26 5f63 6f6d 706f  ping..tpZ&_compo
+00000910: 6e65 6e74 732e 5f70 6179 6c6f 6164 2e5f  nents._payload._
+00000920: 646f 636b 6572 5f65 7865 6375 746f 7273  docker_executors
+00000930: 7203 0000 0072 0400 0000 7205 0000 00da  r....r....r.....
+00000940: 105f 7072 6f74 6f5f 6e61 6d65 7370 6163  ._proto_namespac
+00000950: 6572 0600 0000 721a 0000 0072 2100 0000  er....r....r!...
+00000960: da03 416e 79da 0555 6e69 6f6e 7229 0000  ..Any..Unionr)..
+00000970: 00da 0853 6571 7565 6e63 6572 3000 0000  ...Sequencer0...
+00000980: 723c 0000 0072 1800 0000 7218 0000 0072  r<...r....r....r
+00000990: 1800 0000 7219 0000 00da 083c 6d6f 6475  ....r......<modu
+000009a0: 6c65 3e01 0000 0073 3600 0000 0801 0801  le>....s6.......
+000009b0: 0801 0c02 0c01 0c01 0c01 1203 1213 020a  ................
+000009c0: 0201 02ff 0402 02fe 1203 02fd 0204 0afc  ................
+000009d0: 0215 0201 02ff 0402 02fe 0203 02fd 0204  ................
+000009e0: 0efc                                     ..
```

### Comparing `adaux-2.3.0/source/adaux/src/payload/python/functions.py` & `adaux-2.3.1/source/adaux/src/payload/python/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,26 +42,25 @@
     aux: _ProtoNamespace,  # pylint: disable=unused-argument
     deps: tp.Any,
     tags: tp.Union[str, tp.Sequence[str]],  # pylint: disable=redefined-outer-name
 ) -> None:
     if isinstance(tags, str):
         tags = [tags]
 
-    if len(deps) != 1:
-        raise RuntimeError(
-            f"tag job for {tags} should have exactly 1 dependency, not {len(deps)}!"
-        )
     last_local_tag = ""
-    for tag in tags:  # pylint: disable=redefined-outer-name
-        tag = tag.format(version=aux.project.version, branch=aux.gitlab.current_branch)
-        local_tag, release_tag = deps[0].executor.tag_and_upload(tag)
-        if last_local_tag != local_tag:
-            last_local_tag = local_tag
-            print("uploaded", local_tag)
-        print("   -> to", release_tag)
+    for dep in deps:
+        for tag in tags:  # pylint: disable=redefined-outer-name
+            tag = tag.format(
+                version=aux.project.version, branch=aux.gitlab.current_branch
+            )
+            local_tag, release_tag = dep.executor.tag_and_upload(tag)
+            if last_local_tag != local_tag:
+                last_local_tag = local_tag
+                print("uploaded", local_tag)
+            print("   -> to", release_tag)
 
 
 def img_dockerhub(
     aux: _ProtoNamespace,
     deps: tp.Any,
     release_tag: str,
 ) -> None:
```

### Comparing `adaux-2.3.0/source/adaux/src/pre-commit/add_copy_right.py.jinja2` & `adaux-2.3.1/source/adaux/src/pre-commit/add_copy_right.py.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux/src/pre-commit/config.yaml.jinja2` & `adaux-2.3.1/source/adaux/src/pre-commit/config.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `adaux-2.3.0/source/adaux.egg-info/SOURCES.txt` & `adaux-2.3.1/source/adaux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

