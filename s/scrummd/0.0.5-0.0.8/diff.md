# Comparing `tmp/scrummd-0.0.5.tar.gz` & `tmp/scrummd-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrummd-0.0.5.tar", last modified: Tue Mar 12 06:55:37 2024, max compression
+gzip compressed data, was "scrummd-0.0.8.tar", last modified: Tue Mar 26 11:09:15 2024, max compression
```

## Comparing `scrummd-0.0.5.tar` & `scrummd-0.0.8.tar`

### file list

```diff
@@ -1,175 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.262833 scrummd-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.234833 scrummd-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.242833 scrummd-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-12 06:55:23.000000 scrummd-0.0.5/.github/workflows/lint-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-12 06:55:23.000000 scrummd-0.0.5/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-12 06:55:23.000000 scrummd-0.0.5/.github/workflows/pipy-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-12 06:55:23.000000 scrummd-0.0.5/.github/workflows/test-pypi-deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-03-12 06:55:23.000000 scrummd-0.0.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.242833 scrummd-0.0.5/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-12 06:55:23.000000 scrummd-0.0.5/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-12 06:55:23.000000 scrummd-0.0.5/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    34905 2024-03-12 06:55:23.000000 scrummd-0.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-12 06:55:37.262833 scrummd-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-12 06:55:23.000000 scrummd-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/card.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/commands/commands.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/commands/sbench.rst
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/commands/sbl.rst
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/commands/scard.rst
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/commands/svalid.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/concepts.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/semver.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/source/scrummd.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial1.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.238833 scrummd-0.0.5/docs/tutorial_examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.238833 scrummd-0.0.5/docs/tutorial_examples/tutorial1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.238833 scrummd-0.0.5/docs/tutorial_examples/tutorial1/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.250833 scrummd-0.0.5/docs/tutorial_examples/tutorial1/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.250833 scrummd-0.0.5/docs/tutorial_examples/tutorial1/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1/scrum/reports/bug1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.238833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.238833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.2/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.2/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.2/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.2/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.2/scrum/reports/bug1.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.2/scrum/reports/bug2.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.2/scrum/reports/bug3.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.238833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.238833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.3/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.3/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.3/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.3/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.3/scrum/reports/bug1.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.3/scrum/reports/bug2.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.3/scrum/reports/bug3.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.238833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.4/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.4/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.4/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.4/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.4/scrum/reports/bug1.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.4/scrum/reports/bug2.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.4/scrum/reports/bug3.md
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.4/scrum/reports/bug4.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.4/scrum.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.238833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.5/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.246833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.5/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.5/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.250833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.5/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.5/scrum/reports/bug1.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.5/scrum/reports/bug2.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.5/scrum/reports/bug3.md
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.5/scrum.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.250833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.238833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.6/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.250833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.6/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.6/scrum/backlog/card1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.250833 scrummd-0.0.5/docs/tutorial_examples/tutorial1.6/scrum/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.6/scrum/reports/bug1.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.6/scrum/reports/bug2.md
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.6/scrum/reports/bug3.md
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-12 06:55:23.000000 scrummd-0.0.5/docs/tutorial_examples/tutorial1.6/scrum.toml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-12 06:55:23.000000 scrummd-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-12 06:55:23.000000 scrummd-0.0.5/readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.250833 scrummd-0.0.5/scrum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.254834 scrummd-0.0.5/scrum/backlog/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli001.md
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli002.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli003.md
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli004.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli005.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli006.md
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli007.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli008.md
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli009.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli010.md
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli011.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli012.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli013.md
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli014.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli015.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli016.md
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli017.md
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli018.md
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli019.md
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli020.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli021.md
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli022.md
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli023.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli024.md
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli025.md
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli026.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/backlog/cli027.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrum/v0-1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.254834 scrummd-0.0.5/scrummd/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-12 06:55:37.000000 scrummd-0.0.5/scrummd/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/card.py
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/sbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/sbl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/scard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/source_md.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/svalid.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-12 06:55:23.000000 scrummd-0.0.5/scrummd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.262833 scrummd-0.0.5/scrummd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-12 06:55:37.000000 scrummd-0.0.5/scrummd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-03-12 06:55:37.000000 scrummd-0.0.5/scrummd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 06:55:37.000000 scrummd-0.0.5/scrummd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-12 06:55:37.000000 scrummd-0.0.5/scrummd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-12 06:55:37.000000 scrummd-0.0.5/scrummd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-12 06:55:37.000000 scrummd-0.0.5/scrummd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 06:55:37.262833 scrummd-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.258834 scrummd-0.0.5/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.258834 scrummd-0.0.5/test/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.258834 scrummd-0.0.5/test/data/collection1/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/collection1/.meta.md
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/collection1/c1.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/collection1/c2.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/collection1/c3.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.258834 scrummd-0.0.5/test/data/collection1/embedded/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/collection1/embedded/e1.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.258834 scrummd-0.0.5/test/data/collection2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.262833 scrummd-0.0.5/test/data/collection2/.ignorethis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.262833 scrummd-0.0.5/test/data/collection2/.ignorethis/collection/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/collection2/.ignorethis/collection/i2.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/collection2/.ignorethis/i1.md
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/collection2/c4.md
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/collection2/c5.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/collection2/c6.md
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/collection3.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.242833 scrummd-0.0.5/test/data/fail_cases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.262833 scrummd-0.0.5/test/data/fail_cases/invalid/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/fail_cases/invalid/no_summary.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 06:55:37.262833 scrummd-0.0.5/test/data/fail_cases/rule_violation/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/fail_cases/rule_violation/bad_status.md
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/md1.md
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/data/md2.md
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/test_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/test_config_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/test_in_anger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/test_scard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/test_source_md.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-12 06:55:23.000000 scrummd-0.0.5/test/test_svalid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.402374 scrummd-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-03-26 11:09:01.000000 scrummd-0.0.8/.github/workflows/lint-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-26 11:09:01.000000 scrummd-0.0.8/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-26 11:09:01.000000 scrummd-0.0.8/.github/workflows/pipy-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-26 11:09:01.000000 scrummd-0.0.8/.github/workflows/test-pypi-deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-03-26 11:09:01.000000 scrummd-0.0.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.402374 scrummd-0.0.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-03-26 11:09:01.000000 scrummd-0.0.8/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-26 11:09:01.000000 scrummd-0.0.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34905 2024-03-26 11:09:01.000000 scrummd-0.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-26 11:09:15.426374 scrummd-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-26 11:09:01.000000 scrummd-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/card.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/commands/commands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/commands/sbench.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/commands/sbl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/commands/scard.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/commands/svalid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/concepts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/semver.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/source/scrummd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10879 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial1.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.402374 scrummd-0.0.8/docs/tutorial_examples/tutorial1/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1/scrum/reports/bug1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/reports/bug1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/reports/bug2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.2/scrum/reports/bug3.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.406374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/reports/bug1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/reports/bug2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.3/scrum/reports/bug3.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/reports/bug1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/reports/bug2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/reports/bug3.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum/reports/bug4.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.4/scrum.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/reports/bug1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/reports/bug2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum/reports/bug3.md
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.5/scrum.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.398374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/backlog/card1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/reports/bug1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/reports/bug2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum/reports/bug3.md
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-26 11:09:01.000000 scrummd-0.0.8/docs/tutorial_examples/tutorial1.6/scrum.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-26 11:09:01.000000 scrummd-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-26 11:09:01.000000 scrummd-0.0.8/readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.410374 scrummd-0.0.8/scrum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.418374 scrummd-0.0.8/scrum/backlog/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli001.md
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli002.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli003.md
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli004.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli005.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli006.md
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli007.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli008.md
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli009.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli010.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli011.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli012.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli013.md
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli014.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli015.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli016.md
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli017.md
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli018.md
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli019.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli020.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli021.md
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli022.md
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli023.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli024.md
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli025.md
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli026.md
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli027.md
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli028.md
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/backlog/cli029.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrum/v0-1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.418374 scrummd-0.0.8/scrummd/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6641 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/sbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/sbl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/scard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/source_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/svalid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-26 11:09:01.000000 scrummd-0.0.8/scrummd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/scrummd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-26 11:09:15.000000 scrummd-0.0.8/scrummd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 11:09:15.426374 scrummd-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.422374 scrummd-0.0.8/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.422374 scrummd-0.0.8/test/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.422374 scrummd-0.0.8/test/data/collection1/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection1/c1.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection1/c2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection1/c3.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.422374 scrummd-0.0.8/test/data/collection1/embedded/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection1/embedded/e1.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/data/collection2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/data/collection2/.ignorethis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/data/collection2/.ignorethis/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection2/.ignorethis/collection/i2.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection2/.ignorethis/i1.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection2/c4.md
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection2/c5.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection2/c6.md
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection3.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/data/collection4/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/collection4/c7.md
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/md1.md
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/data/md2.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.402374 scrummd-0.0.8/test/fail_cases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/fail_cases/collection_rule_violation/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/fail_cases/collection_rule_violation/bad_status.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/fail_cases/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/fail_cases/invalid/no_summary.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 11:09:15.426374 scrummd-0.0.8/test/fail_cases/rule_violation/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/fail_cases/rule_violation/bad_status.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_in_anger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_sbl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_scard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_source_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-26 11:09:01.000000 scrummd-0.0.8/test/test_svalid.py
```

### Comparing `scrummd-0.0.5/.github/workflows/lint-and-test.yml` & `scrummd-0.0.8/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/.github/workflows/mypy.yml` & `scrummd-0.0.8/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/.github/workflows/pipy-publish.yml` & `scrummd-0.0.8/.github/workflows/pipy-publish.yml`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/.github/workflows/test-pypi-deploy.yml` & `scrummd-0.0.8/.github/workflows/test-pypi-deploy.yml`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/.gitignore` & `scrummd-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/.vscode/launch.json` & `scrummd-0.0.8/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/LICENSE.md` & `scrummd-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/PKG-INFO` & `scrummd-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrummd
-Version: 0.0.5
+Version: 0.0.8
 Author-email: Lachlan Kingsford <lachlan@nerdygentleman.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: importlib-metadata; python_version >= "3.11"
 
 ## ScrumMD
```

### Comparing `scrummd-0.0.5/README.md` & `scrummd-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/docs/Makefile` & `scrummd-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/docs/card.rst` & `scrummd-0.0.8/docs/card.rst`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/docs/concepts.rst` & `scrummd-0.0.8/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/docs/conf.py` & `scrummd-0.0.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/docs/configuration.rst` & `scrummd-0.0.8/docs/configuration.rst`

 * *Files 24% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 
 Configuration
 ~~~~~~~~~~~~~
 
 Configuration files
 ===================
 
-.. note::
-    It is intended that additional configuration will be able to be set on a per
-    collection and per card basis. This is not implemented yet.
-
 ScrumMD is configured by a toml file. The first of the following files available
 will be read for configuration:
 
 -   ``.scrum.toml``
 -   ``scrum.toml``
 -   ``pyproject.toml``
 
 All fields in the ``[tool.scrummd]`` collection.
 
+Where fields are listed as ``[tool.scrummd.fieldname]``, they should be in
+square brackets as TOML categories/arrays.
+
 Supported fields
 ================
 
 ``[tool.scrummd]``
 ##################
 
 ``strict``
@@ -88,39 +87,84 @@
 str
 
 Description
 """""""""""
 
 Format of ``[[card]]`` fields when shown by ``scard``. Replaces ``$field`` with the field from the card.
 
-``[tools.scrummd.fields]``
-##########################
+``required``
+
+Type
+""""
 
-*field name*
-^^^^^^^^^^^^
+array of str
+
+Description
+"""""""""""
+
+List of fields that must be present in all cards.
+
+``[tools.scrummd.fields.<field name>]``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Type
 """"
 
 array of str
 
 Description
 """""""""""
 
 Limit *field name* to specific values. Each member is an array of str.
 
+``[tools.scrummd.collections.<collection name>]``
+#################################################
+
+Additional restrictions which apply only to a specific collection.
+
+``required``
 
+Type
+""""
+
+array of str
+
+Description
+"""""""""""
+
+List of fields that must be present in all cards in the collection.
+
+``[tools.scrummd.collections.<collection name>.fields.<field name>]``
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Type
+""""
+
+array of str
+
+Description
+"""""""""""
+
+Limit *field name* to specific values for all cards in the collection. Each
+member is an array of str.
 
 Example configuration file
 ==========================
 
 .. code-block:: toml
 
     [tool.scrummd]
     strict = true
     scrum_path = "scrum"
     columns = ["index", "status", "summary"]
     scard_reference_format = "$index [$status] ($assignee)"
     omit_headers = false
+    required = ["status"]
 
     [tool.scrummd.fields]
     status = ["Not Fully Defined", "Ready", "In Progress", "In Testing", "Done"]
+
+    [tool.scrummd.collections.epic]
+    required = ["cost centre", "members"]
+
+    [tool.scrummd.collections.epic.fields]
+    cost_status = ["Not Costed", "Fully Costed"]
```

### Comparing `scrummd-0.0.5/docs/index.rst` & `scrummd-0.0.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/docs/installation.rst` & `scrummd-0.0.8/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/docs/make.bat` & `scrummd-0.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/docs/semver.rst` & `scrummd-0.0.8/docs/semver.rst`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/docs/source/scrummd.rst` & `scrummd-0.0.8/docs/source/scrummd.rst`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/docs/tutorial1.rst` & `scrummd-0.0.8/docs/tutorial1.rst`

 * *Files 12% similar despite different names*

```diff
@@ -370,26 +370,47 @@
 
 We added a reference format, and expected values for the status.
 
 Now, if we go ``scard bug1``, we'll see:
 
 .. code-block:: text
 
-    $ card bug1
+    $ scard bug1
     ---
     bug1: Bug with project
     ---
     reporter: example@example.com
     severity: High
     description: Demonstrate another collection of cards
     fixed by: 
     card1 - My first Scrum card [Ready for Development]
 
 You'll see that the reference has been replaced with a more useful reference.
 
+Filters
+^^^^^^^
+
+Now you've got some bugs (sorry), you might want to see just the highest
+severity bugs. ``sbl`` has filters available with ``--include``.
+
+You can add multiple filters with multiple ``--include`` statements (all of
+which must be matched to show), and multiple values to ``include`` by separating
+them with a comma. If you were to go:
+
+.. code-block:: text
+
+    $ sbl --include severity=high
+    index, summary
+    bug3, Bad bug
+    bug1, Bug with project
+
+You can see that just high severity bugs are returned. Alternatively - you could
+go ``sbl --include severity=high,medium`` to show all medium and high bugs.
+
+
 Tags
 ^^^^
 
 Cards can be added to additional collections by 'tagging' them. If you add a
 ``tags`` field, any listed values will be created as a collection. Modify
 the following cards as follows:
```

### Comparing `scrummd-0.0.5/pyproject.toml` & `scrummd-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/readthedocs.yaml` & `scrummd-0.0.8/readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrum/backlog/cli001.md` & `scrummd-0.0.8/scrum/backlog/cli001.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrum/backlog/cli002.md` & `scrummd-0.0.8/scrum/backlog/cli002.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrum/backlog/cli004.md` & `scrummd-0.0.8/scrum/backlog/cli004.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrum/backlog/cli009.md` & `scrummd-0.0.8/scrum/backlog/cli009.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrum/backlog/cli011.md` & `scrummd-0.0.8/scrum/backlog/cli011.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrum/backlog/cli017.md` & `scrummd-0.0.8/scrum/backlog/cli017.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrum/backlog/cli021.md` & `scrummd-0.0.8/scrum/backlog/cli021.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrum/backlog/cli022.md` & `scrummd-0.0.8/scrum/backlog/cli022.md`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrum/backlog/cli023.md` & `scrummd-0.0.8/scrum/backlog/cli023.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 ---
 Summary: Equals filter
-Status: Ready
+Status: Done
 ---
 
 # Description
 
 We need to be able to filter by cards in `sbl`.
 
 For this card, the user should be able to filter by a field equalling something specific - and only have those matching cards returned.
 
 # Cucumber
 
 **GIVEN** a scrum repository
 **WHEN** `sbl --include [FIELD]=[VALUE]` is run
 **THEN** then only cards where the FIELD equals the VALUE
 
+**GIVEN** an include statement
+**WHEN** `[VALUE]` contains multiple values separated by a comma
+**THEN** then cards that match any of the values are included (OR)
+
 **GIVEN** a scrum repository
 **WHEN** `sbl` is run with multiple `--include` arguments
-**THEN** then cards that match any of the include statements are included
+**THEN** then cards that match all of the include statements are included
 
 # Clarifications
 
 -   Search is to be case insensitive
 -   Search is to trim the strings
 -   Include should be able to be specified in the config
```

### Comparing `scrummd-0.0.5/scrummd/collection.py` & `scrummd-0.0.8/scrummd/collection.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,66 @@
 from argparse import ArgumentError
 from collections import OrderedDict
+from copy import copy
+from dataclasses import dataclass
+from enum import Enum
+import itertools
 import os
 import pathlib
 from typing import Optional, Union
-from scrummd.card import Card, fromStr
+from scrummd.card import Card, from_str
 import logging
 from scrummd.config import ScrumConfig
 from scrummd.exceptions import ValidationError, DuplicateIndexError
 
 logger = logging.getLogger(__name__)
 
 Collection = dict[str, Card]
 
 
+@dataclass
+class Filter:
+    """Filter for filtering through a collection"""
+
+    class FilterMode(Enum):
+        """Types of filter"""
+
+        EQUALS = 1
+
+    field: str
+    """Field that is being tested"""
+
+    values: str | list[str]
+    """Potential values for the field"""
+
+    mode: FilterMode = FilterMode.EQUALS
+    """Mode that the filter is in"""
+
+    def apply(self, collection: Collection) -> Collection:
+        """Apply this filter to a collection
+
+        Args:
+            collection (Collection): Collection to apply the filter to
+
+        Returns:
+            Collection: The filtered collection
+        """
+        if isinstance(self.values, list):
+            values = [value.strip().lower() for value in self.values]
+        else:
+            values = [str(self.values).strip().lower()]
+
+        return {
+            card_index: card
+            for card_index, card in collection.items()
+            if not isinstance(card.get_field(self.field), list)
+            and str(card.get_field(self.field)).strip().lower() in values
+        }
+
+
 def get_collection(
     config: ScrumConfig, collection_name: Optional[str] = None
 ) -> Collection:
     """Get a collection of cards
 
     Args:
         config (ScrumConfig): ScrumMD Configuration to use
@@ -26,15 +70,15 @@
         DuplicateIndexError: A card with an index is found twice
 
     Returns:
         dict[str, Card]: A dict with the index of the card, and a card object
     """
 
     all_cards: dict[str, Card] = {}
-    collection: dict[str, Card] = {}
+
     collection_path = pathlib.Path(config.scrum_path)
     for root, _, files in os.walk(collection_path, followlinks=True):
         # So - this'll turn "scrum/backlog/special" into "backlog.special"
         path_parts = pathlib.Path(root).relative_to(collection_path).parts
         collection_from_path = ".".join(path_parts)
         # Ignore any folder starting with .
         if any([folder_name[0] == "." for folder_name in path_parts]):
@@ -44,54 +88,96 @@
             path = pathlib.Path(root, name)
             if name[0] == ".":
                 # Ignore all files that start with .
                 continue
             try:
                 with open(path, "r") as fo:
                     contents = fo.read()
-                    card = fromStr(config, contents, collection_from_path, path)
+                    card = from_str(config, contents, collection_from_path, path)
                     if card.index in all_cards:
                         raise DuplicateIndexError(card.index, path)
                     all_cards[card.index] = card
 
             except ValidationError as ex:
                 if config.strict:
                     logging.error("ValidationError (%s) reading %s", ex, path)
                     raise
                 else:
-                    logging.warn("ValidationError (%s) reading %s", ex, path)
+                    logging.warning("ValidationError (%s) reading %s", ex, path)
 
             except DuplicateIndexError as ex:
                 if config.strict:
                     raise
                 else:
-                    logging.warn("%s ignored", path)
+                    logging.warning("%s ignored", path)
 
-    if not collection_name:
-        return all_cards
+    collections: dict[str, Collection] = {}
 
+    # Get all the cards in each collection per implicit collection from folder
+    # and collections listed in the card
     for index, card in all_cards.items():
         for _collection in card.collections:
-            if _collection == collection_name or _collection.startswith(
-                collection_name + "."
+            # The partial name stuff here is because if a card is in
+            # 'collection.subcollection', it's also in 'collection' implicitly
+            # - accumulate with that lambda means that for A.B.C, it adds it to
+            # A, then A.B, then A.B.C
+            for partial_name in itertools.accumulate(
+                _collection.split("."), lambda i, j: f"{i}.{j}"
             ):
-                collection[index] = card
+                if partial_name in collections:
+                    collections[partial_name][index] = card
+                else:
+                    collections[partial_name] = {index: card}
 
-        for collection_subname, _defined_collection in card.defined_collections.items():
-            current_collection_name = (
-                index if collection_subname == "" else f"{index}.{collection_subname}"
-            )
-            if (
-                current_collection_name == collection_name
-                or current_collection_name.startswith(collection_name + ".")
-            ):
-                for card_index in _defined_collection:
-                    collection[card_index] = all_cards[card_index]
+    # Get all the collections defined in a card in the fields. Again - needs to
+    # add to parent collections too.
+    # Holy horizontal ladder, Batman!
+    for index, card in all_cards.items():
+        for defined_name, defined_collection in card.defined_collections.items():
+            for referenced_card_index in defined_collection:
+                if referenced_card_index not in all_cards:
+                    # Card not found
+                    continue
 
-    return collection
+                if defined_name in collections:
+                    collections[defined_name][referenced_card_index] = all_cards[
+                        referenced_card_index
+                    ]
+                else:
+                    collections[defined_name] = {
+                        referenced_card_index: all_cards[referenced_card_index]
+                    }
+                if index in collections:
+                    collections[index][referenced_card_index] = all_cards[
+                        referenced_card_index
+                    ]
+                else:
+                    collections[index] = {
+                        referenced_card_index: all_cards[referenced_card_index]
+                    }
+
+    # Validate that all cards in a collection are valid per its rules in config
+    for _collection_name, collection in collections.items():
+        collection_config = config.collections.get(_collection_name)
+        if not collection_config:
+            continue
+        for index, card in collection.items():
+            try:
+                card.assert_valid_rules(collection_config)
+            except ValidationError as ex:
+                if config.strict:
+                    logging.error("ValidationError (%s) reading %s", ex, path)
+                    raise
+                else:
+                    logging.warn("ValidationError (%s) reading %s", ex, path)
+
+    if not collection_name:
+        return all_cards
+
+    return collections.get(collection_name) or {}
 
 
 Groups = dict[Optional[str], Union["Groups", list[Card]]]
 
 
 def group_collection(
     config: ScrumConfig, collection: Collection, groups: list[str]
@@ -158,7 +244,23 @@
     # This is not particularly clear - if there's more groups to embed, recurse.
     return {
         key: group_collection(
             config, {c.index: c for c in group if isinstance(c, Card)}, groups[1:]
         )
         for key, group in card_groups.items()
     }
+
+
+def filter_collection(collection: Collection, filters: list[Filter]) -> Collection:
+    """Apply all filters to a collection
+
+    Args:
+        collection (Collection): Collection to apply filters to.
+        filters (list[Filter]): Filters to apply. All filters are applied.
+
+    Returns:
+        Collection: Filtered collection of cards.
+    """
+    working_collection = copy(collection)
+    for f in filters:
+        working_collection = f.apply(working_collection)
+    return working_collection
```

### Comparing `scrummd-0.0.5/scrummd/config_loader.py` & `scrummd-0.0.8/scrummd/config_loader.py`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrummd/exceptions.py` & `scrummd-0.0.8/scrummd/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,7 +31,13 @@
         super().__init__(f"Duplicate index {self.index} found in {self.path}")
 
 
 class InvalidGroupError(ValueError):
     """Called when a field is not a valid group"""
 
     pass
+
+
+class RequiredFieldNotPresentError(RuleViolationError):
+    """Called when a field required by config isn't present"""
+
+    pass
```

### Comparing `scrummd-0.0.5/scrummd/sbench.py` & `scrummd-0.0.8/scrummd/sbench.py`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrummd/sbl.py` & `scrummd-0.0.8/scrummd/sbl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,48 @@
 """Display a collection of scrum cards"""
 
 import argparse
 
-from scrummd.collection import Groups, get_collection, group_collection
+from scrummd.collection import (
+    Filter,
+    Groups,
+    get_collection,
+    group_collection,
+    filter_collection,
+)
 from scrummd.config import ScrumConfig
 from scrummd.config_loader import load_fs_config
 from scrummd.exceptions import ValidationError
 from scrummd.scard import format_field
 from scrummd.version import version_to_output
 
 VALIDATION_ERROR = 1
 
 
+def include_to_filter(source: str) -> Filter:
+    """Transform an --include argument into a Filter
+
+    Args:
+        source (str): FILTER from --include
+
+    Returns:
+        Filter: Filter object from the string
+    """
+    try:
+        field, value_str = source.split("=")
+    except ValueError:
+        raise argparse.ArgumentTypeError(
+            "Filter not in valid format. Expected format is --include key=value1[, value2]"
+        )
+
+    values = [value.strip() for value in value_str.split(",")]
+
+    return Filter(field.strip(), values, Filter.FilterMode.EQUALS)
+
+
 def create_parser() -> argparse.ArgumentParser:
     """Create an argument parser for sbl
 
     Returns:
         argparse.ArgumentParser: ArgumentParser for sbl
     """
     parser = argparse.ArgumentParser()
@@ -43,18 +70,30 @@
         help="Omit headers from output.",
     )
 
     parser.add_argument(
         "-g",
         "--group-by",
         action="append",
+        metavar="FIELD",
         help="Group by field in card. Can use multiple group-by arguments to have multiple levels of grouping.",
     )
 
     parser.add_argument(
+        "-i",
+        "--include",
+        action="append",
+        metavar="FILTER",
+        type=include_to_filter,
+        help="Only include collections that match this filter. The filter is in the format "
+        + "`key=value1[, value2, ...]`. Multiple values verify if the field is any of the values. "
+        + "Multiple --include statements must all be matched.",
+    )
+
+    parser.add_argument(
         "--version",
         action="version",
         version=version_to_output(),
     )
     parser.description = __doc__
     return parser
 
@@ -82,14 +121,17 @@
     if args.bare:
         columns = ["path"]
         omit_headers = True
 
     if not omit_headers:
         print(", ".join(columns))
 
+    if args.include:
+        collection = filter_collection(collection, args.include)
+
     if not args.group_by:
         for card in collection.values():
             values = [format_field(card.get_field(col)) for col in columns]
             print(", ".join(values))
 
     else:
         grouped = group_collection(config, collection, args.group_by)
```

### Comparing `scrummd-0.0.5/scrummd/scard.py` & `scrummd-0.0.8/scrummd/scard.py`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrummd/source_md.py` & `scrummd-0.0.8/scrummd/source_md.py`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrummd/svalid.py` & `scrummd-0.0.8/scrummd/svalid.py`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/scrummd.egg-info/PKG-INFO` & `scrummd-0.0.8/scrummd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrummd
-Version: 0.0.5
+Version: 0.0.8
 Author-email: Lachlan Kingsford <lachlan@nerdygentleman.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: importlib-metadata; python_version >= "3.11"
 
 ## ScrumMD
```

### Comparing `scrummd-0.0.5/scrummd.egg-info/SOURCES.txt` & `scrummd-0.0.8/scrummd.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 scrum/backlog/cli021.md
 scrum/backlog/cli022.md
 scrum/backlog/cli023.md
 scrum/backlog/cli024.md
 scrum/backlog/cli025.md
 scrum/backlog/cli026.md
 scrum/backlog/cli027.md
+scrum/backlog/cli028.md
+scrum/backlog/cli029.md
 scrummd/__init__.py
 scrummd/_version.py
 scrummd/card.py
 scrummd/collection.py
 scrummd/config.py
 scrummd/config_loader.py
 scrummd/const.py
@@ -103,25 +105,27 @@
 scrummd.egg-info/requires.txt
 scrummd.egg-info/top_level.txt
 test/fixtures.py
 test/test_card.py
 test/test_collection.py
 test/test_config_loader.py
 test/test_in_anger.py
+test/test_sbl.py
 test/test_scard.py
 test/test_source_md.py
 test/test_svalid.py
 test/data/collection3.md
 test/data/md1.md
 test/data/md2.md
-test/data/collection1/.meta.md
 test/data/collection1/c1.md
 test/data/collection1/c2.md
 test/data/collection1/c3.md
 test/data/collection1/embedded/e1.md
 test/data/collection2/c4.md
 test/data/collection2/c5.md
 test/data/collection2/c6.md
 test/data/collection2/.ignorethis/i1.md
 test/data/collection2/.ignorethis/collection/i2.md
-test/data/fail_cases/invalid/no_summary.md
-test/data/fail_cases/rule_violation/bad_status.md
+test/data/collection4/c7.md
+test/fail_cases/collection_rule_violation/bad_status.md
+test/fail_cases/invalid/no_summary.md
+test/fail_cases/rule_violation/bad_status.md
```

### Comparing `scrummd-0.0.5/test/test_collection.py` & `scrummd-0.0.8/test/test_collection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,28 @@
+"""Tests for `collection.py`"""
+
+from copy import copy
 import os
 import pytest
+from pathlib import Path
 
 from scrummd.config import ScrumConfig
-from scrummd.collection import get_collection, group_collection
+from scrummd.collection import (
+    Filter,
+    get_collection,
+    group_collection,
+    filter_collection,
+)
 from fixtures import data_config
+from scrummd.exceptions import RuleViolationError
+
+
+# NOTE: These almost all retrieve the same set of data. We might want to think
+# about ways we can restructure this to see more useful fail cases if something
+# was to go wrong.
 
 
 def test_get_basic_collection(data_config):
     """Test that all the cards in a basic collection are returned"""
     test_collection = get_collection(data_config, "collection1")
 
     indices = test_collection.keys()
@@ -103,7 +118,54 @@
 def test_multiple_groupbys(data_config):
     """Test that grouping when there are two fields is correct"""
     test_collection = get_collection(data_config, "collection1")
     grouped = group_collection(data_config, test_collection, ["status", "assignee"])
     assert set((card.index for card in grouped["ready"]["bob"])) == set(["c1"])
     assert set((card.index for card in grouped["ready"]["mary"])) == set(["c2"])
     assert set((card.index for card in grouped["done"]["bob"])) == set(["c3"])
+
+
+def test_collection_with_rules(data_config):
+    """Test that a card with valid collection-level rules is added"""
+    collection4 = get_collection(data_config, "collection4").values()
+    assert set((card.index for card in collection4)) == set(["c7"])
+
+
+def test_collection_with_invalid_collection_rules(data_config):
+    """Test that a card violating collection rules raises an error"""
+    config = copy(data_config)
+    config.scrum_path = "test/fail_cases/collection_rule_violation"
+    with pytest.raises(RuleViolationError):
+        get_collection(config, "collection4")
+
+
+def test_path_correctly_set(data_config):
+    """Test that the path for a card is as expected"""
+    test_collection = get_collection(data_config, "collection1")
+    assert Path(test_collection["c1"].path) == Path("test/data/collection1/c1.md")
+    assert Path(test_collection["e1"].path) == Path(
+        "test/data/collection1/embedded/e1.md"
+    )
+
+
+@pytest.mark.parametrize(
+    ["filters", "expected_card_ids"],
+    [
+        [[Filter("assignee", "Bob")], ["c1", "c3"]],
+        [[Filter("assignee", ["Bob", "Mary"])], ["c1", "c2", "c3"]],
+        [[Filter("assignee", "bob")], ["c1", "c3"]],
+        [[Filter("assignee", "bob"), Filter("status", "ready")], ["c1"]],
+        [[Filter("assignee", " bob"), Filter("status", "ready")], ["c1"]],
+    ],
+    ids=[
+        "1 field",
+        "1 field, 2 values",
+        "Check for case insensitivity",
+        "Multiple conditions",
+        "Strip whitespace",
+    ],
+)
+def test_filtering(data_config, filters, expected_card_ids):
+    """Test that filters are correctly applied"""
+    test_collection = get_collection(data_config)
+    result = filter_collection(test_collection, filters).keys()
+    assert set(result) == set(expected_card_ids)
```

### Comparing `scrummd-0.0.5/test/test_config_loader.py` & `scrummd-0.0.8/test/test_config_loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -90,7 +90,47 @@
     assert config.scrum_path == "with_config"
 
 
 def test_fields_table(temp_dir, scrum_dot_toml):
     """Test that the fields values are set from tool.scrummd.field"""
     config = load_fs_config()
     assert config.fields["status"] == ["Ready", "Progress", "Done"]
+
+
+COLLECTION_CONFIG = """
+[tool.scrummd]
+strict = true
+scrum_path = "basic_tool"
+
+[tool.scrummd.fields]
+status = ["Ready", "Progress", "Done"]
+
+[tool.scrummd.collections.epic]
+required = ["cost", "components"]
+
+[tool.scrummd.collections.epic.fields]
+status = ["Not Defined", "Started", "Done"]
+"""
+
+
+@pytest.fixture(scope="function")
+def collection_config_f(temp_dir):
+    with open(Path(temp_dir, "scrum.toml"), "w") as fo:
+        fo.write(COLLECTION_CONFIG)
+        fo.flush()
+        yield
+
+
+def test_collection_level_1(temp_dir, collection_config_f):
+    """Test that a setting in [tool.scrummd.collections.*] is set"""
+    config = load_fs_config()
+    assert config.collections["epic"].required == ["cost", "components"]
+
+
+def test_collection_level_2(temp_dir, collection_config_f):
+    """Test that a setting in [tool.scrummd.collections.*.fields] is set"""
+    config = load_fs_config()
+    assert config.collections["epic"].fields["status"] == [
+        "Not Defined",
+        "Started",
+        "Done",
+    ]
```

### Comparing `scrummd-0.0.5/test/test_in_anger.py` & `scrummd-0.0.8/test/test_in_anger.py`

 * *Files identical despite different names*

### Comparing `scrummd-0.0.5/test/test_scard.py` & `scrummd-0.0.8/test/test_scard.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from copy import copy
 from pathlib import Path
-from scrummd.card import Card, fromStr
+from scrummd.card import Card, from_str
 from scrummd.scard import output_value, format_card
 from fixtures import data_config, test_collection
 import pytest
 
 
 @pytest.fixture(scope="function")
 def test_card(data_config) -> Card:
     test_card = """
 ---
 summary: Test Card
 key: Field [[c1]]
 key 2: [[c2]][[c3]]
 ---
 """
-    card = fromStr(data_config, test_card, "collection", Path("collection/card.md"))
+    card = from_str(data_config, test_card, "collection", Path("collection/card.md"))
     return card
 
 
 def test_output_value(data_config, test_card, test_collection):
     config = copy(data_config)
     config.scard_reference_format = "[$index $assignee $status]"
     assert (
@@ -29,22 +29,23 @@
     assert (
         output_value(config, test_card.get_field("key 2"), test_collection)
         == "[c2 Mary ready][c3 Bob Done]"
     )
 
 
 @pytest.fixture()
-def sample_card():
+def sample_card(data_config):
     return Card(
         index="i",
         summary="1",
         collections=[],
         defined_collections=[],
         path="test/i.md",
         udf={"assignee": "me"},
+        _config=data_config,
     )
 
 
 @pytest.mark.parametrize(
     ["input_format", "expected"],
     [
         ["$index", "i"],
```

### Comparing `scrummd-0.0.5/test/test_source_md.py` & `scrummd-0.0.8/test/test_source_md.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     fo.close()
 
 
 def test_extract_property_from_full_file(md1_fo):
     """Test extracting property variables from an md file"""
     results = source_md.extract_fields(md1_fo.read())
     assert results["summary"] == "Summary of card"
-    assert results["status"] == "Status of card"
+    assert results["status"] == "Ready"
 
 
 def test_extract_header(md1_fo):
     """Test extracting header style variables from an md file"""
     results = source_md.extract_fields(md1_fo.read())
     assert (
         results["description"].strip()
```

### Comparing `scrummd-0.0.5/test/test_svalid.py` & `scrummd-0.0.8/test/test_svalid.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     config = copy(data_config)
     config.scrum_path = "test/data/collection1"
     assert get_exit_code(config) == ExitCode.SUCCESSFUL
 
 
 def test_invalid(data_config):
     config = copy(data_config)
-    config.scrum_path = "test/data/fail_cases/invalid"
+    config.scrum_path = "test/fail_cases/invalid"
     assert get_exit_code(config) == ExitCode.INVALID_FILE
 
 
 def test_rule_violation(data_config):
     config = copy(data_config)
-    config.scrum_path = "test/data/fail_cases/rule_violation"
+    config.scrum_path = "test/fail_cases/rule_violation"
     assert get_exit_code(config) == ExitCode.RULE_VIOLATION
```

