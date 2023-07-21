# Comparing `tmp/python-semantic-release-8.0.2.tar.gz` & `tmp/python-semantic-release-8.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-semantic-release-8.0.2.tar", last modified: Tue Jul 18 21:40:50 2023, max compression
+gzip compressed data, was "python-semantic-release-8.0.3.tar", last modified: Fri Jul 21 16:21:41 2023, max compression
```

## Comparing `python-semantic-release-8.0.2.tar` & `python-semantic-release-8.0.3.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/
--rw-r--r--   0 root         (0) root         (0)      230 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1084 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      153 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3108 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2272 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/README.rst
--rw-r--r--   0 root         (0) root         (0)     4651 2023-07-18 21:40:42.000000 python-semantic-release-8.0.2/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.645312 python-semantic-release-8.0.2/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3108 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4266 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      598 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-18 21:40:50.000000 python-semantic-release-8.0.2/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.645312 python-semantic-release-8.0.2/semantic_release/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-07-18 21:40:43.000000 python-semantic-release-8.0.2/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.649312 python-semantic-release-8.0.2/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      361 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6470 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4328 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.649312 python-semantic-release-8.0.2/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.649312 python-semantic-release-8.0.2/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3364 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     4956 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    18649 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    12975 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     3753 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.649312 python-semantic-release-8.0.2/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      884 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5713 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)     1456 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      831 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.641312 python-semantic-release-8.0.2/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.653312 python-semantic-release-8.0.2/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      465 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.653312 python-semantic-release-8.0.2/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      300 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5595 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     8285 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    10146 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     5898 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.653312 python-semantic-release-8.0.2/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      339 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14641 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7267 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3037 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14060 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.641312 python-semantic-release-8.0.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.653312 python-semantic-release-8.0.2/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)     3631 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_publish.py
--rw-r--r--   0 root         (0) root         (0)    20288 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/command_line/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      106 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    45283 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/fixtures/git_repo.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46838 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12186 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5005 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     2540 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2102 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.657312 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_github_actions_output.py
--rw-r--r--   0 root         (0) root         (0)     5768 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)     4227 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_util.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      648 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    22533 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    23987 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    13407 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 21:40:50.661312 python-semantic-release-8.0.2/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8947 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9640 2023-07-18 21:39:53.000000 python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      153 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)     4651 2023-07-21 16:21:34.000000 python-semantic-release-8.0.3/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.698726 python-semantic-release-8.0.3/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      598 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-21 16:21:41.000000 python-semantic-release-8.0.3/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.698726 python-semantic-release-8.0.3/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)     1123 2023-07-21 16:21:34.000000 python-semantic-release-8.0.3/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.702726 python-semantic-release-8.0.3/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.702726 python-semantic-release-8.0.3/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.702726 python-semantic-release-8.0.3/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    18649 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    12975 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.702726 python-semantic-release-8.0.3/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      884 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5713 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.694726 python-semantic-release-8.0.3/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.706726 python-semantic-release-8.0.3/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)      844 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.706726 python-semantic-release-8.0.3/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     8285 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    10146 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.706726 python-semantic-release-8.0.3/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14710 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7267 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3037 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    13967 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      466 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.694726 python-semantic-release-8.0.3/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.706726 python-semantic-release-8.0.3/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)     3631 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_publish.py
+-rw-r--r--   0 root         (0) root         (0)    20288 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/command_line/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    45283 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/fixtures/git_repo.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46838 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12186 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5005 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.710726 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     5768 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)     4227 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_util.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    22533 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    23987 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    13407 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-21 16:21:41.714726 python-semantic-release-8.0.3/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9248 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9675 2023-07-21 16:20:49.000000 python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_version.py
```

### Comparing `python-semantic-release-8.0.2/LICENSE` & `python-semantic-release-8.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/PKG-INFO` & `python-semantic-release-8.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.2
+Version: 8.0.3
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.2/README.rst` & `python-semantic-release-8.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/pyproject.toml` & `python-semantic-release-8.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "8.0.2"
+version = "8.0.3"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.7"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
```

### Comparing `python-semantic-release-8.0.2/python_semantic_release.egg-info/PKG-INFO` & `python-semantic-release-8.0.3/python_semantic_release.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.2
+Version: 8.0.3
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `python-semantic-release-8.0.2/python_semantic_release.egg-info/SOURCES.txt` & `python-semantic-release-8.0.3/python_semantic_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/python_semantic_release.egg-info/requires.txt` & `python-semantic-release-8.0.3/python_semantic_release.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/__init__.py` & `python-semantic-release-8.0.3/semantic_release/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,24 +10,25 @@
     ParseResultType as ParseResultType,
     ParserOptions as ParserOptions,
 )
 from semantic_release.enums import LevelBump as LevelBump
 from semantic_release.errors import (
     CommitParseError as CommitParseError,
     InvalidConfiguration as InvalidConfiguration,
+    InvalidVersion as InvalidVersion,
     SemanticReleaseBaseError as SemanticReleaseBaseError,
 )
 from semantic_release.version import (
     Version as Version,
     VersionTranslator as VersionTranslator,
     next_version as next_version,
     tags_and_versions as tags_and_versions,
 )
 
-__version__ = "8.0.2"
+__version__ = "8.0.3"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python-semantic-release-8.0.2/semantic_release/changelog/context.py` & `python-semantic-release-8.0.3/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/changelog/release_history.py` & `python-semantic-release-8.0.3/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/changelog/template.py` & `python-semantic-release-8.0.3/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/cli/commands/changelog.py` & `python-semantic-release-8.0.3/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/cli/commands/generate_config.py` & `python-semantic-release-8.0.3/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/cli/commands/main.py` & `python-semantic-release-8.0.3/semantic_release/cli/commands/main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/cli/commands/publish.py` & `python-semantic-release-8.0.3/semantic_release/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/cli/commands/version.py` & `python-semantic-release-8.0.3/semantic_release/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/cli/common.py` & `python-semantic-release-8.0.3/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/cli/config.py` & `python-semantic-release-8.0.3/semantic_release/cli/config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/cli/github_actions_output.py` & `python-semantic-release-8.0.3/semantic_release/cli/github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/cli/masking_filter.py` & `python-semantic-release-8.0.3/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/cli/util.py` & `python-semantic-release-8.0.3/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/commit_parser/__init__.py` & `python-semantic-release-8.0.3/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/commit_parser/_base.py` & `python-semantic-release-8.0.3/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/commit_parser/angular.py` & `python-semantic-release-8.0.3/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/commit_parser/emoji.py` & `python-semantic-release-8.0.3/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/commit_parser/scipy.py` & `python-semantic-release-8.0.3/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/commit_parser/tag.py` & `python-semantic-release-8.0.3/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/commit_parser/token.py` & `python-semantic-release-8.0.3/semantic_release/commit_parser/token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/commit_parser/util.py` & `python-semantic-release-8.0.3/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/const.py` & `python-semantic-release-8.0.3/semantic_release/const.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/data/templates/CHANGELOG.md.j2` & `python-semantic-release-8.0.3/semantic_release/data/templates/CHANGELOG.md.j2`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/enums.py` & `python-semantic-release-8.0.3/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/errors.py` & `python-semantic-release-8.0.3/semantic_release/errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 
 class InvalidConfiguration(SemanticReleaseBaseError):
     """
     Raised when configuration is deemed invalid
     """
 
 
+class InvalidVersion(ValueError, SemanticReleaseBaseError):
+    """
+    Raised when Version.parse attempts to parse a string containing
+    an invalid version.
+    """
+
+
 class NotAReleaseBranch(InvalidConfiguration):
     """
     Raised when semantic_release is invoked on a branch which isn't configured for
     releases
     """
```

### Comparing `python-semantic-release-8.0.2/semantic_release/helpers.py` & `python-semantic-release-8.0.3/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/hvcs/_base.py` & `python-semantic-release-8.0.3/semantic_release/hvcs/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/hvcs/gitea.py` & `python-semantic-release-8.0.3/semantic_release/hvcs/gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/hvcs/github.py` & `python-semantic-release-8.0.3/semantic_release/hvcs/github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/hvcs/gitlab.py` & `python-semantic-release-8.0.3/semantic_release/hvcs/gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/hvcs/token_auth.py` & `python-semantic-release-8.0.3/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/hvcs/util.py` & `python-semantic-release-8.0.3/semantic_release/hvcs/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/version/algorithm.py` & `python-semantic-release-8.0.3/semantic_release/version/algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     CommitParser,
     ParsedCommit,
     ParseResult,
     ParserOptions,
 )
 from semantic_release.const import DEFAULT_VERSION
 from semantic_release.enums import LevelBump
+from semantic_release.errors import InvalidVersion
 from semantic_release.version.translator import VersionTranslator
 from semantic_release.version.version import Version
 
 log = logging.getLogger(__name__)
 
 
 def tags_and_versions(
@@ -36,15 +37,15 @@
 
     Tags which are not matched by `translator` are ignored.
     """
     ts_and_vs: list[tuple[Tag, Version]] = []
     for tag in tags:
         try:
             version = translator.from_tag(tag.name)
-        except NotImplementedError as e:
+        except (NotImplementedError, InvalidVersion) as e:
             log.warning(
                 "Couldn't parse tag %s as as Version: %s",
                 tag.name,
                 str(e),
                 exc_info=log.isEnabledFor(logging.DEBUG),
             )
             continue
```

### Comparing `python-semantic-release-8.0.2/semantic_release/version/declaration.py` & `python-semantic-release-8.0.3/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/version/translator.py` & `python-semantic-release-8.0.3/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/semantic_release/version/version.py` & `python-semantic-release-8.0.3/semantic_release/version/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,26 +4,20 @@
 import re
 from functools import wraps
 from itertools import zip_longest
 from typing import Callable, Union, overload
 
 from semantic_release.const import SEMVER_REGEX
 from semantic_release.enums import LevelBump
+from semantic_release.errors import InvalidVersion
 from semantic_release.helpers import check_tag_format
 
 log = logging.getLogger(__name__)
 
 
-class InvalidVersion(ValueError):
-    """
-    Raised when Version.parse attempts to parse a string containing
-    an invalid version.
-    """
-
-
 # Very heavily inspired by semver.version:_comparator, I don't think there's
 # a cleaner way to do this
 # https://github.com/python-semver/python-semver/blob/b5317af9a7e99e6a86df98320e73be72d5adf0de/src/semver/version.py#L32
 VersionComparable = Union["Version", str]
 VersionComparator = Callable[["Version", "Version"], bool]
```

### Comparing `python-semantic-release-8.0.2/tests/command_line/test_changelog.py` & `python-semantic-release-8.0.3/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/command_line/test_generate_config.py` & `python-semantic-release-8.0.3/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/command_line/test_help.py` & `python-semantic-release-8.0.3/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/command_line/test_main.py` & `python-semantic-release-8.0.3/tests/command_line/test_main.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/command_line/test_publish.py` & `python-semantic-release-8.0.3/tests/command_line/test_publish.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/command_line/test_version.py` & `python-semantic-release-8.0.3/tests/command_line/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/fixtures/commit_parsers.py` & `python-semantic-release-8.0.3/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/fixtures/example_project.py` & `python-semantic-release-8.0.3/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/fixtures/git_repo.py` & `python-semantic-release-8.0.3/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/fixtures/scipy.py` & `python-semantic-release-8.0.3/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/scenario/test_next_version.py` & `python-semantic-release-8.0.3/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/scenario/test_release_history.py` & `python-semantic-release-8.0.3/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/scenario/test_template_render.py` & `python-semantic-release-8.0.3/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_release_notes.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/changelog/test_template.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_config.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_github_actions_output.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_github_actions_output.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_masking_filter.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_util.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/cli/test_version.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_angular.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_tag.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/commit_parser/test_token.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/commit_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test__base.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_gitea.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_github.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_algorithm.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,26 @@
                 "v1.0.0-beta.11",
                 "v1.0.0-alpha.1",
                 "v1.0.0-alpha.beta.1",
                 "v1.0.0",
             ],
         ),
         (
+            "v{version}",
+            ("0.3", "0.4"),
+            [
+                "v1.0.0-rc.1",
+                "v1.0.0-beta.2",
+                "v1.0.0-beta.11",
+                "v1.0.0-alpha.1",
+                "v1.0.0-alpha.beta.1",
+                "v1.0.0",
+            ],
+        ),
+        (
             r"(\w+--)?v{version}",
             ("v1.1.0-test-test", "test_v1.1.0"),
             [
                 "v1.0.0-rc.1",
                 "test--v1.1.0",
                 "v1.0.0-beta.2",
                 "v1.0.0-beta.11",
```

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_declaration.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_translator.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.2/tests/unit/semantic_release/version/test_version.py` & `python-semantic-release-8.0.3/tests/unit/semantic_release/version/test_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import operator
 import random
 
 import pytest
 
 from semantic_release.enums import LevelBump
-from semantic_release.version.version import InvalidVersion, Version
+from semantic_release.errors import InvalidVersion
+from semantic_release.version.version import Version
 
 random.seed(0)
 
 EXAMPLE_VERSION_STRINGS = [
     "1.0.0",
     "0.1.0",
     "0.0.1",
```

