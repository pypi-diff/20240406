# Comparing `tmp/python-semantic-release-9.4.0.tar.gz` & `tmp/python-semantic-release-9.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-semantic-release-9.4.0.tar", last modified: Sun Mar 31 20:43:57 2024, max compression
+gzip compressed data, was "python-semantic-release-9.4.1.tar", last modified: Sat Apr  6 19:50:33 2024, max compression
```

## Comparing `python-semantic-release-9.4.0.tar` & `python-semantic-release-9.4.1.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.848466 python-semantic-release-9.4.0/
--rw-r--r--   0 root         (0) root         (0)      230 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1083 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      225 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5281 2024-03-31 20:43:57.848466 python-semantic-release-9.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2673 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.820466 python-semantic-release-9.4.0/docs/
--rw-r--r--   0 root         (0) root         (0)     6984 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)     9656 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/algorithm.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.820466 python-semantic-release-9.4.0/docs/automatic-releases/
--rw-r--r--   0 root         (0) root         (0)     1284 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/automatic-releases/cronjobs.rst
--rw-r--r--   0 root         (0) root         (0)     4046 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/automatic-releases/github-actions.rst
--rw-r--r--   0 root         (0) root         (0)      738 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/automatic-releases/index.rst
--rw-r--r--   0 root         (0) root         (0)     2268 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/automatic-releases/travis.rst
--rw-r--r--   0 root         (0) root         (0)    15332 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/changelog_templates.rst
--rw-r--r--   0 root         (0) root         (0)    13275 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/commands.rst
--rw-r--r--   0 root         (0) root         (0)    15380 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/commit-parsing.rst
--rw-r--r--   0 root         (0) root         (0)     2288 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)    23320 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/configuration.rst
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/contributing.rst
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/contributors.rst
--rw-r--r--   0 root         (0) root         (0)     3501 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/github-action.rst
--rw-r--r--   0 root         (0) root         (0)     6814 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)     6735 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)    21218 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/migrating_from_v7.rst
--rw-r--r--   0 root         (0) root         (0)     8866 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/multibranch_releases.rst
--rw-r--r--   0 root         (0) root         (0)     2403 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/strict_mode.rst
--rw-r--r--   0 root         (0) root         (0)     1452 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/docs/troubleshooting.rst
--rw-r--r--   0 root         (0) root         (0)     9689 2024-03-31 20:43:51.000000 python-semantic-release-9.4.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.844466 python-semantic-release-9.4.0/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5281 2024-03-31 20:43:57.000000 python-semantic-release-9.4.0/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5538 2024-03-31 20:43:57.000000 python-semantic-release-9.4.0/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 20:43:57.000000 python-semantic-release-9.4.0/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2024-03-31 20:43:57.000000 python-semantic-release-9.4.0/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      613 2024-03-31 20:43:57.000000 python-semantic-release-9.4.0/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-03-31 20:43:57.000000 python-semantic-release-9.4.0/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.824466 python-semantic-release-9.4.0/semantic_release/
--rw-r--r--   0 root         (0) root         (0)      870 2024-03-31 20:43:51.000000 python-semantic-release-9.4.0/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.824466 python-semantic-release-9.4.0/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      262 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      986 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6675 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4640 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.824466 python-semantic-release-9.4.0/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      419 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.828466 python-semantic-release-9.4.0/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4087 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     3443 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/commands/cli_context.py
--rw-r--r--   0 root         (0) root         (0)     1699 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     2900 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1703 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    22111 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)     1439 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    16070 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2102 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     3071 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     3755 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.828466 python-semantic-release-9.4.0/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      615 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2609 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4393 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5777 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3194 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1505 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      730 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.812466 python-semantic-release-9.4.0/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.828466 python-semantic-release-9.4.0/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1066 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)     1001 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     5581 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.832466 python-semantic-release-9.4.0/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      379 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5635 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     4626 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/hvcs/bitbucket.py
--rw-r--r--   0 root         (0) root         (0)     9146 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    10710 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     6154 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      663 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2886 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.832466 python-semantic-release-9.4.0/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      270 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16854 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7357 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3050 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14175 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-31 20:43:57.848466 python-semantic-release-9.4.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.832466 python-semantic-release-9.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.832466 python-semantic-release-9.4.0/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2983 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)    11474 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1759 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)     6566 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     5255 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    28853 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/command_line/test_version.py
--rw-r--r--   0 root         (0) root         (0)     1107 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     8953 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.836466 python-semantic-release-9.4.0/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      197 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      912 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)    11562 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    13280 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/git_repo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.836466 python-semantic-release-9.4.0/tests/fixtures/repos/
--rw-r--r--   0 root         (0) root         (0)      142 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/repos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.836466 python-semantic-release-9.4.0/tests/fixtures/repos/git_flow/
--rw-r--r--   0 root         (0) root         (0)      140 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/repos/git_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21042 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
--rw-r--r--   0 root         (0) root         (0)    21711 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.836466 python-semantic-release-9.4.0/tests/fixtures/repos/github_flow/
--rw-r--r--   0 root         (0) root         (0)       71 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/repos/github_flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15712 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/repos/github_flow/repo_w_release_channels.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.836466 python-semantic-release-9.4.0/tests/fixtures/repos/trunk_based_dev/
--rw-r--r--   0 root         (0) root         (0)      199 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/repos/trunk_based_dev/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10463 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
--rw-r--r--   0 root         (0) root         (0)    13604 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
--rw-r--r--   0 root         (0) root         (0)    10698 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
--rw-r--r--   0 root         (0) root         (0)     4494 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.840466 python-semantic-release-9.4.0/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)   127286 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12845 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     5074 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.840466 python-semantic-release-9.4.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.840466 python-semantic-release-9.4.0/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.840466 python-semantic-release-9.4.0/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6225 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     3563 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2116 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.840466 python-semantic-release-9.4.0/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5468 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     1842 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     6361 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     4219 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/cli/test_util.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.844466 python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5952 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2483 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2096 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      648 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)      836 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.844466 python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1357 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)     5363 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test_bitbucket.py
--rw-r--r--   0 root         (0) root         (0)    22326 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    26340 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    13318 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      966 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test_util.py
--rw-r--r--   0 root         (0) root         (0)     4507 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/test_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 20:43:57.844466 python-semantic-release-9.4.0/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9605 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3874 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2951 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9714 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/unit/semantic_release/version/test_version.py
--rw-r--r--   0 root         (0) root         (0)     6070 2024-03-31 20:42:39.000000 python-semantic-release-9.4.0/tests/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.068435 python-semantic-release-9.4.1/
+-rw-r--r--   0 root         (0) root         (0)      230 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      225 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5281 2024-04-06 19:50:33.068435 python-semantic-release-9.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2673 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.040435 python-semantic-release-9.4.1/docs/
+-rw-r--r--   0 root         (0) root         (0)     6984 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)     9656 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/algorithm.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.040435 python-semantic-release-9.4.1/docs/automatic-releases/
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/automatic-releases/cronjobs.rst
+-rw-r--r--   0 root         (0) root         (0)     4046 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/automatic-releases/github-actions.rst
+-rw-r--r--   0 root         (0) root         (0)      738 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/automatic-releases/index.rst
+-rw-r--r--   0 root         (0) root         (0)     2268 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/automatic-releases/travis.rst
+-rw-r--r--   0 root         (0) root         (0)    15332 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/changelog_templates.rst
+-rw-r--r--   0 root         (0) root         (0)    13275 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/commands.rst
+-rw-r--r--   0 root         (0) root         (0)    15380 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/commit-parsing.rst
+-rw-r--r--   0 root         (0) root         (0)     2288 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)    23320 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/configuration.rst
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/contributors.rst
+-rw-r--r--   0 root         (0) root         (0)     3501 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/github-action.rst
+-rw-r--r--   0 root         (0) root         (0)     6814 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)     6735 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)    21218 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/migrating_from_v7.rst
+-rw-r--r--   0 root         (0) root         (0)     8866 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/multibranch_releases.rst
+-rw-r--r--   0 root         (0) root         (0)     2403 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/strict_mode.rst
+-rw-r--r--   0 root         (0) root         (0)     1452 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/docs/troubleshooting.rst
+-rw-r--r--   0 root         (0) root         (0)     9689 2024-04-06 19:50:26.000000 python-semantic-release-9.4.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.064435 python-semantic-release-9.4.1/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5281 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5538 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      613 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-06 19:50:33.000000 python-semantic-release-9.4.1/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.044435 python-semantic-release-9.4.1/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)      870 2024-04-06 19:50:26.000000 python-semantic-release-9.4.1/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.044435 python-semantic-release-9.4.1/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      986 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6675 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4640 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.044435 python-semantic-release-9.4.1/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.048435 python-semantic-release-9.4.1/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/cli_context.py
+-rw-r--r--   0 root         (0) root         (0)     1699 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     2900 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1703 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    22111 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)     1439 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    16070 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2110 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.048435 python-semantic-release-9.4.1/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      615 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2609 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4393 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5777 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3194 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      730 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.032435 python-semantic-release-9.4.1/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.048435 python-semantic-release-9.4.1/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5581 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.052435 python-semantic-release-9.4.1/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      379 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5635 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4626 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)     9146 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    10710 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     6154 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      663 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2886 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.052435 python-semantic-release-9.4.1/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16854 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3050 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14175 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 19:50:33.068435 python-semantic-release-9.4.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.052435 python-semantic-release-9.4.1/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.052435 python-semantic-release-9.4.1/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)    11474 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1759 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     6566 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     5255 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    28853 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/command_line/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     8953 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.056435 python-semantic-release-9.4.1/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      197 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      912 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)    11562 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    13280 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/git_repo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.056435 python-semantic-release-9.4.1/tests/fixtures/repos/
+-rw-r--r--   0 root         (0) root         (0)      142 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.056435 python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21042 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py
+-rw-r--r--   0 root         (0) root         (0)    21711 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.056435 python-semantic-release-9.4.1/tests/fixtures/repos/github_flow/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/github_flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15712 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/github_flow/repo_w_release_channels.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.056435 python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py
+-rw-r--r--   0 root         (0) root         (0)    10698 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.060435 python-semantic-release-9.4.1/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   127286 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12845 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     5074 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.060435 python-semantic-release-9.4.1/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.060435 python-semantic-release-9.4.1/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.060435 python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6225 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.060435 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5468 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     6361 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4219 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_util.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.064435 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5952 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      648 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      836 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.064435 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1357 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)     5363 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_bitbucket.py
+-rw-r--r--   0 root         (0) root         (0)    22326 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    26340 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    13318 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      966 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_util.py
+-rw-r--r--   0 root         (0) root         (0)     4507 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/test_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 19:50:33.064435 python-semantic-release-9.4.1/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9605 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3874 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9714 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     6070 2024-04-06 19:49:10.000000 python-semantic-release-9.4.1/tests/util.py
```

### Comparing `python-semantic-release-9.4.0/LICENSE` & `python-semantic-release-9.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/PKG-INFO` & `python-semantic-release-9.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.4.0
+Version: 9.4.1
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
@@ -49,17 +49,17 @@
 Requires-Dist: pytest-clarity~=1.0; extra == "test"
 Requires-Dist: responses~=0.25.0; extra == "test"
 Requires-Dist: requests-mock~=1.10; extra == "test"
 Requires-Dist: types-pytest-lazy-fixture~=0.6.3; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pre-commit~=3.5; extra == "dev"
 Requires-Dist: tox~=4.11; extra == "dev"
-Requires-Dist: ruff==0.3.4; extra == "dev"
+Requires-Dist: ruff==0.3.5; extra == "dev"
 Provides-Extra: mypy
-Requires-Dist: mypy==1.8.0; extra == "mypy"
+Requires-Dist: mypy==1.9.0; extra == "mypy"
 Requires-Dist: types-requests~=2.31.0; extra == "mypy"
 
 Python Semantic Release
 ***********************
 
 |Ruff| |Test Status| |PyPI Version| |conda-forge version| |Read the Docs Status| |Pre-Commit Enabled|
```

### Comparing `python-semantic-release-9.4.0/README.rst` & `python-semantic-release-9.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/Makefile` & `python-semantic-release-9.4.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/algorithm.rst` & `python-semantic-release-9.4.1/docs/algorithm.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/automatic-releases/cronjobs.rst` & `python-semantic-release-9.4.1/docs/automatic-releases/cronjobs.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/automatic-releases/github-actions.rst` & `python-semantic-release-9.4.1/docs/automatic-releases/github-actions.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/automatic-releases/index.rst` & `python-semantic-release-9.4.1/docs/automatic-releases/index.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/automatic-releases/travis.rst` & `python-semantic-release-9.4.1/docs/automatic-releases/travis.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/changelog_templates.rst` & `python-semantic-release-9.4.1/docs/changelog_templates.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/commands.rst` & `python-semantic-release-9.4.1/docs/commands.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/commit-parsing.rst` & `python-semantic-release-9.4.1/docs/commit-parsing.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/conf.py` & `python-semantic-release-9.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/configuration.rst` & `python-semantic-release-9.4.1/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/github-action.rst` & `python-semantic-release-9.4.1/docs/github-action.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/index.rst` & `python-semantic-release-9.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/make.bat` & `python-semantic-release-9.4.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/migrating_from_v7.rst` & `python-semantic-release-9.4.1/docs/migrating_from_v7.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/multibranch_releases.rst` & `python-semantic-release-9.4.1/docs/multibranch_releases.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/strict_mode.rst` & `python-semantic-release-9.4.1/docs/strict_mode.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/docs/troubleshooting.rst` & `python-semantic-release-9.4.1/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/pyproject.toml` & `python-semantic-release-9.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools ~= 69.0", "wheel ~= 0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "9.4.0"
+version = "9.4.1"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.8",
@@ -67,18 +67,18 @@
   "responses ~= 0.25.0",
   "requests-mock ~= 1.10",
   "types-pytest-lazy-fixture ~= 0.6.3",
 ]
 dev = [
   "pre-commit ~= 3.5",
   "tox ~= 4.11",
-  "ruff == 0.3.4"
+  "ruff == 0.3.5"
 ]
 mypy = [
-  "mypy == 1.8.0",
+  "mypy == 1.9.0",
   "types-requests ~= 2.31.0"
 ]
 
 [tool.pytest.ini_options]
 env = [
   "PYTHONHASHSEED = 123456"
 ]
```

### Comparing `python-semantic-release-9.4.0/python_semantic_release.egg-info/PKG-INFO` & `python-semantic-release-9.4.1/python_semantic_release.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 9.4.0
+Version: 9.4.1
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: changelog, https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md
 Project-URL: documentation, https://python-semantic-release.readthedocs.io
 Project-URL: homepage, https://python-semantic-release.readthedocs.io
 Project-URL: issues, https://github.com/python-semantic-release/python-semantic-release/issues
@@ -49,17 +49,17 @@
 Requires-Dist: pytest-clarity~=1.0; extra == "test"
 Requires-Dist: responses~=0.25.0; extra == "test"
 Requires-Dist: requests-mock~=1.10; extra == "test"
 Requires-Dist: types-pytest-lazy-fixture~=0.6.3; extra == "test"
 Provides-Extra: dev
 Requires-Dist: pre-commit~=3.5; extra == "dev"
 Requires-Dist: tox~=4.11; extra == "dev"
-Requires-Dist: ruff==0.3.4; extra == "dev"
+Requires-Dist: ruff==0.3.5; extra == "dev"
 Provides-Extra: mypy
-Requires-Dist: mypy==1.8.0; extra == "mypy"
+Requires-Dist: mypy==1.9.0; extra == "mypy"
 Requires-Dist: types-requests~=2.31.0; extra == "mypy"
 
 Python Semantic Release
 ***********************
 
 |Ruff| |Test Status| |PyPI Version| |conda-forge version| |Read the Docs Status| |Pre-Commit Enabled|
```

### Comparing `python-semantic-release-9.4.0/python_semantic_release.egg-info/SOURCES.txt` & `python-semantic-release-9.4.1/python_semantic_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/python_semantic_release.egg-info/requires.txt` & `python-semantic-release-9.4.1/python_semantic_release.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 pydantic~=2.0
 rich~=12.5
 shellingham~=1.5
 
 [dev]
 pre-commit~=3.5
 tox~=4.11
-ruff==0.3.4
+ruff==0.3.5
 
 [docs]
 Sphinx~=6.0
 sphinxcontrib-apidoc==0.5.0
 sphinx-autobuild==2024.2.4
 furo~=2023.3
 
 [mypy]
-mypy==1.8.0
+mypy==1.9.0
 types-requests~=2.31.0
 
 [test]
 coverage[toml]~=7.0
 pytest~=7.0
 pytest-env~=1.0
 pytest-xdist~=3.0
```

### Comparing `python-semantic-release-9.4.0/semantic_release/__init__.py` & `python-semantic-release-9.4.1/semantic_release/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from semantic_release.version import (
     Version,
     VersionTranslator,
     next_version,
     tags_and_versions,
 )
 
-__version__ = "9.4.0"
+__version__ = "9.4.1"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python-semantic-release-9.4.0/semantic_release/changelog/context.py` & `python-semantic-release-9.4.1/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/changelog/release_history.py` & `python-semantic-release-9.4.1/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/changelog/template.py` & `python-semantic-release-9.4.1/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/cli/commands/changelog.py` & `python-semantic-release-9.4.1/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/cli/commands/cli_context.py` & `python-semantic-release-9.4.1/semantic_release/cli/commands/cli_context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/cli/commands/generate_config.py` & `python-semantic-release-9.4.1/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/cli/commands/main.py` & `python-semantic-release-9.4.1/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/cli/commands/publish.py` & `python-semantic-release-9.4.1/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/cli/commands/version.py` & `python-semantic-release-9.4.1/semantic_release/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/cli/common.py` & `python-semantic-release-9.4.1/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/cli/config.py` & `python-semantic-release-9.4.1/semantic_release/cli/config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/cli/github_actions_output.py` & `python-semantic-release-9.4.1/semantic_release/cli/github_actions_output.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,16 @@
             )
 
         outputs = {
             "released": str(self.released).lower(),
             "version": str(self.version),
             "tag": self.tag,
         }
-        return "\n".join(f"{key}={value!s}" for key, value in outputs.items())
+
+        return str.join("", [f"{key}={value!s}\n" for key, value in outputs.items()])
 
     def write_if_possible(self, filename: str | None = None) -> None:
         output_file = filename or os.getenv(self.OUTPUT_ENV_VAR)
         if not output_file:
             log.info("not writing GitHub Actions output, as no file specified")
             return
```

### Comparing `python-semantic-release-9.4.0/semantic_release/cli/masking_filter.py` & `python-semantic-release-9.4.1/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/cli/util.py` & `python-semantic-release-9.4.1/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/commit_parser/__init__.py` & `python-semantic-release-9.4.1/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/commit_parser/_base.py` & `python-semantic-release-9.4.1/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/commit_parser/angular.py` & `python-semantic-release-9.4.1/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/commit_parser/emoji.py` & `python-semantic-release-9.4.1/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/commit_parser/scipy.py` & `python-semantic-release-9.4.1/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/commit_parser/tag.py` & `python-semantic-release-9.4.1/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/commit_parser/token.py` & `python-semantic-release-9.4.1/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/commit_parser/util.py` & `python-semantic-release-9.4.1/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/const.py` & `python-semantic-release-9.4.1/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/data/templates/CHANGELOG.md.j2` & `python-semantic-release-9.4.1/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/enums.py` & `python-semantic-release-9.4.1/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/errors.py` & `python-semantic-release-9.4.1/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/helpers.py` & `python-semantic-release-9.4.1/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/hvcs/_base.py` & `python-semantic-release-9.4.1/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/hvcs/bitbucket.py` & `python-semantic-release-9.4.1/semantic_release/hvcs/bitbucket.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/hvcs/gitea.py` & `python-semantic-release-9.4.1/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/hvcs/github.py` & `python-semantic-release-9.4.1/semantic_release/hvcs/github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/hvcs/gitlab.py` & `python-semantic-release-9.4.1/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/hvcs/token_auth.py` & `python-semantic-release-9.4.1/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/hvcs/util.py` & `python-semantic-release-9.4.1/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/version/algorithm.py` & `python-semantic-release-9.4.1/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/version/declaration.py` & `python-semantic-release-9.4.1/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/version/translator.py` & `python-semantic-release-9.4.1/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/semantic_release/version/version.py` & `python-semantic-release-9.4.1/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/command_line/conftest.py` & `python-semantic-release-9.4.1/tests/command_line/conftest.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/command_line/test_changelog.py` & `python-semantic-release-9.4.1/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/command_line/test_generate_config.py` & `python-semantic-release-9.4.1/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/command_line/test_help.py` & `python-semantic-release-9.4.1/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/command_line/test_main.py` & `python-semantic-release-9.4.1/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/command_line/test_publish.py` & `python-semantic-release-9.4.1/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/command_line/test_version.py` & `python-semantic-release-9.4.1/tests/command_line/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/conftest.py` & `python-semantic-release-9.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/const.py` & `python-semantic-release-9.4.1/tests/const.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/fixtures/commit_parsers.py` & `python-semantic-release-9.4.1/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/fixtures/example_project.py` & `python-semantic-release-9.4.1/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/fixtures/git_repo.py` & `python-semantic-release-9.4.1/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py` & `python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/repo_w_2_release_channels.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py` & `python-semantic-release-9.4.1/tests/fixtures/repos/git_flow/repo_w_3_release_channels.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/fixtures/repos/github_flow/repo_w_release_channels.py` & `python-semantic-release-9.4.1/tests/fixtures/repos/github_flow/repo_w_release_channels.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py` & `python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_no_tags.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py` & `python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_prereleases.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py` & `python-semantic-release-9.4.1/tests/fixtures/repos/trunk_based_dev/repo_w_tags.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/fixtures/scipy.py` & `python-semantic-release-9.4.1/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/scenario/test_next_version.py` & `python-semantic-release-9.4.1/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/scenario/test_release_history.py` & `python-semantic-release-9.4.1/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/scenario/test_template_render.py` & `python-semantic-release-9.4.1/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/changelog/test_release_notes.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/changelog/test_template.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/cli/test_config.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/cli/test_masking_filter.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/cli/test_util.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/cli/test_version.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/test_angular.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/test_tag.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/test_token.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/commit_parser/test_util.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/commit_parser/test_util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test__base.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test_bitbucket.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_bitbucket.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test_gitea.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test_github.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/test_helpers.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/test_helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/version/test_algorithm.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/version/test_declaration.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/version/test_translator.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/unit/semantic_release/version/test_version.py` & `python-semantic-release-9.4.1/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-9.4.0/tests/util.py` & `python-semantic-release-9.4.1/tests/util.py`

 * *Files identical despite different names*

