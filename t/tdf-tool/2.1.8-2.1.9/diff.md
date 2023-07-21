# Comparing `tmp/tdf_tool-2.1.8.tar.gz` & `tmp/tdf_tool-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdf_tool-2.1.8.tar", max compression
+gzip compressed data, was "tdf_tool-2.1.9.tar", max compression
```

## Comparing `tdf_tool-2.1.8.tar` & `tdf_tool-2.1.9.tar`

### file list

```diff
@@ -1,159 +1,159 @@
--rw-r--r--   0        0        0     1068 2023-06-21 02:31:04.044131 tdf_tool-2.1.8/LICENSE
--rw-r--r--   0        0        0     9217 2023-07-17 07:59:26.799207 tdf_tool-2.1.8/README.md
--rw-r--r--   0        0        0     1608 2023-07-21 12:10:01.958510 tdf_tool-2.1.8/pyproject.toml
--rw-r--r--   0        0        0      321 2023-07-20 10:16:56.395361 tdf_tool-2.1.8/tdf_tool/app.py
--rw-r--r--   0        0        0      973 2023-06-21 03:12:05.604731 tdf_tool-2.1.8/tdf_tool/pipeline.py
--rw-r--r--   0        0        0      424 2023-06-21 02:31:04.047403 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0     2567 2023-06-21 02:31:04.047684 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc
--rw-r--r--   0        0        0     1651 2023-07-17 08:24:09.257737 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc
--rw-r--r--   0        0        0     2668 2023-06-21 02:31:04.048055 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc
--rw-r--r--   0        0        0     1603 2023-07-17 08:24:09.271291 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc
--rw-r--r--   0        0        0      496 2023-06-21 02:31:04.048397 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/init.cpython-39.pyc
--rw-r--r--   0        0        0     3015 2023-06-21 02:31:04.048562 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc
--rw-r--r--   0        0        0     2021 2023-07-17 08:24:08.899762 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc
--rw-r--r--   0        0        0     2981 2023-06-21 02:31:04.048893 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc
--rw-r--r--   0        0        0     2218 2023-07-17 08:24:09.266984 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc
--rw-r--r--   0        0        0    36213 2023-06-21 02:31:04.049422 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc
--rw-r--r--   0        0        0    19495 2023-07-17 09:12:25.271862 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc
--rw-r--r--   0        0        0     3262 2023-06-21 02:31:04.050018 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc
--rw-r--r--   0        0        0     1964 2023-07-17 08:24:09.141480 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc
--rw-r--r--   0        0        0      817 2023-06-21 02:31:04.050452 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc
--rw-r--r--   0        0        0      595 2023-07-17 08:24:09.272692 tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc
--rw-r--r--   0        0        0     1246 2023-06-21 03:12:05.603571 tdf_tool-2.1.8/tdf_tool/pipelines/fix_header.py
--rw-r--r--   0        0        0     1212 2023-06-21 03:12:05.777495 tdf_tool-2.1.8/tdf_tool/pipelines/git.py
--rw-r--r--   0        0        0     1431 2023-06-21 03:12:05.832235 tdf_tool-2.1.8/tdf_tool/pipelines/module.py
--rw-r--r--   0        0        0     1634 2023-06-21 03:12:05.832106 tdf_tool-2.1.8/tdf_tool/pipelines/package.py
--rw-r--r--   0        0        0    26719 2023-07-21 12:09:52.162579 tdf_tool-2.1.8/tdf_tool/pipelines/router.py
--rw-r--r--   0        0        0     1659 2023-06-21 03:12:05.832050 tdf_tool-2.1.8/tdf_tool/pipelines/translate.py
--rw-r--r--   0        0        0      179 2023-07-17 07:59:32.656005 tdf_tool-2.1.8/tdf_tool/pipelines/upgrade.py
--rw-r--r--   0        0        0     1653 2023-06-21 02:31:04.052779 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc
--rw-r--r--   0        0        0     1038 2023-07-17 08:24:09.026923 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc
--rw-r--r--   0        0        0    10270 2023-06-21 02:31:04.053400 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     5123 2023-07-17 08:24:09.016694 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc
--rw-r--r--   0        0        0     1328 2023-06-21 02:31:04.054020 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/env.cpython-311.pyc
--rw-r--r--   0        0        0      873 2023-07-17 08:24:09.028816 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/env.cpython-39.pyc
--rw-r--r--   0        0        0     2480 2023-06-21 02:31:04.054546 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc
--rw-r--r--   0        0        0     1438 2023-07-17 08:24:09.151442 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc
--rw-r--r--   0        0        0     2969 2023-06-21 02:31:04.054996 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/print.cpython-311.pyc
--rw-r--r--   0        0        0     1855 2023-07-17 09:44:23.214841 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/print.cpython-39.pyc
--rw-r--r--   0        0        0     9661 2023-06-21 02:31:04.055529 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc
--rw-r--r--   0        0        0     6155 2023-07-17 08:24:09.154070 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc
--rw-r--r--   0        0        0    10739 2023-06-21 02:31:04.056124 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc
--rw-r--r--   0        0        0     5615 2023-07-17 08:24:09.024850 tdf_tool-2.1.8/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc
--rw-r--r--   0        0        0    11432 2023-06-21 02:31:04.057084 tdf_tool-2.1.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc
--rw-r--r--   0        0        0     6738 2023-07-20 11:08:20.395006 tdf_tool-2.1.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc
--rw-r--r--   0        0        0     7216 2023-06-21 02:31:04.057686 tdf_tool-2.1.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc
--rw-r--r--   0        0        0     3688 2023-07-17 08:24:08.903584 tdf_tool-2.1.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc
--rw-r--r--   0        0        0     1809 2023-07-20 07:43:35.811934 tdf_tool-2.1.8/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc
--rw-r--r--   0        0        0     1628 2023-07-20 07:43:31.587168 tdf_tool-2.1.8/tdf_tool/tools/cli/bean/deps_item.py
--rw-r--r--   0        0        0    10047 2023-07-20 11:11:23.484503 tdf_tool-2.1.8/tdf_tool/tools/cli/module_deps_rewrite.py
--rw-r--r--   0        0        0     4715 2023-06-21 03:12:05.851780 tdf_tool-2.1.8/tdf_tool/tools/cli/project_cli.py
--rw-r--r--   0        0        0     1893 2023-07-20 11:01:33.451132 tdf_tool-2.1.8/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc
--rw-r--r--   0        0        0     1833 2023-07-20 11:01:30.457179 tdf_tool-2.1.8/tdf_tool/tools/cli/utils/yaml_utils.py
--rw-r--r--   0        0        0      559 2023-06-21 03:12:05.832296 tdf_tool-2.1.8/tdf_tool/tools/cmd.py
--rw-r--r--   0        0        0     7002 2023-06-21 02:31:04.059140 tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc
--rw-r--r--   0        0        0     3359 2023-07-17 08:24:09.061860 tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc
--rw-r--r--   0        0        0     2717 2023-06-21 02:31:04.059653 tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc
--rw-r--r--   0        0        0     1465 2023-07-17 08:24:09.134281 tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc
--rw-r--r--   0        0        0     2693 2023-06-21 02:31:04.060168 tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc
--rw-r--r--   0        0        0     2732 2023-06-21 02:31:04.060423 tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc
--rw-r--r--   0        0        0     1886 2023-07-17 08:24:09.149229 tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc
--rw-r--r--   0        0        0     9155 2023-06-21 02:31:04.060789 tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc
--rw-r--r--   0        0        0     4406 2023-07-17 08:24:09.256080 tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc
--rw-r--r--   0        0        0     3983 2023-06-21 03:12:06.205956 tdf_tool-2.1.8/tdf_tool/tools/config/config.py
--rw-r--r--   0        0        0     1311 2023-06-21 03:12:06.079241 tdf_tool-2.1.8/tdf_tool/tools/config/initial_json_config.py
--rw-r--r--   0        0        0     1120 2023-06-21 03:12:06.079047 tdf_tool-2.1.8/tdf_tool/tools/config/module_json_config.py
--rw-r--r--   0        0        0     5593 2023-07-21 12:01:57.126418 tdf_tool-2.1.8/tdf_tool/tools/config/packages_config.py
--rw-r--r--   0        0        0     7704 2023-06-21 03:12:05.852079 tdf_tool-2.1.8/tdf_tool/tools/dependencies_analysis.py
--rw-r--r--   0        0        0      662 2023-06-21 03:12:05.604668 tdf_tool-2.1.8/tdf_tool/tools/env.py
--rw-r--r--   0        0        0     6312 2023-06-21 02:31:04.062376 tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc
--rw-r--r--   0        0        0     3590 2023-07-17 08:24:09.261201 tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc
--rw-r--r--   0        0        0     3174 2023-06-21 02:31:04.062688 tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc
--rw-r--r--   0        0        0     1978 2023-07-17 08:24:09.259434 tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc
--rw-r--r--   0        0        0     4314 2023-06-21 02:31:04.063007 tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc
--rw-r--r--   0        0        0     2438 2023-07-17 08:24:09.262748 tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc
--rw-r--r--   0        0        0     6437 2023-06-21 02:31:04.063372 tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc
--rw-r--r--   0        0        0     3655 2023-07-17 08:24:09.265080 tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc
--rw-r--r--   0        0        0     2422 2023-06-21 02:31:04.063692 tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc
--rw-r--r--   0        0        0     3345 2023-06-21 03:12:06.079100 tdf_tool-2.1.8/tdf_tool/tools/fix_header/fix_header_entry.py
--rw-r--r--   0        0        0     1586 2023-06-21 03:12:05.851836 tdf_tool-2.1.8/tdf_tool/tools/fix_header/fix_header_lint.py
--rw-r--r--   0        0        0     2137 2023-06-21 03:12:06.060569 tdf_tool-2.1.8/tdf_tool/tools/fix_header/fix_header_lint_tool.py
--rw-r--r--   0        0        0     4095 2023-06-21 03:12:06.060768 tdf_tool-2.1.8/tdf_tool/tools/fix_header/fix_header_replace_tool.py
--rw-r--r--   0        0        0     1159 2023-06-21 02:31:04.064465 tdf_tool-2.1.8/tdf_tool/tools/flutter_script.py
--rw-r--r--   0        0        0     7243 2023-06-21 02:31:04.064796 tdf_tool-2.1.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc
--rw-r--r--   0        0        0     4143 2023-07-17 08:24:09.136658 tdf_tool-2.1.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc
--rw-r--r--   0        0        0     7055 2023-06-21 02:31:04.065169 tdf_tool-2.1.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc
--rw-r--r--   0        0        0     3760 2023-07-17 08:24:09.064237 tdf_tool-2.1.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc
--rw-r--r--   0        0        0      593 2023-06-21 02:31:04.065493 tdf_tool-2.1.8/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc
--rw-r--r--   0        0        0     4993 2023-06-21 03:12:06.079521 tdf_tool-2.1.8/tdf_tool/tools/gitlab/gitlab_utils.py
--rw-r--r--   0        0        0     3814 2023-06-21 03:12:05.851649 tdf_tool-2.1.8/tdf_tool/tools/gitlab/python_gitlab_api.py
--rw-r--r--   0        0        0     2482 2023-06-21 02:31:04.066493 tdf_tool-2.1.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc
--rw-r--r--   0        0        0     1386 2023-07-17 08:24:09.059310 tdf_tool-2.1.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc
--rw-r--r--   0        0        0     1063 2023-06-21 03:12:06.079438 tdf_tool-2.1.8/tdf_tool/tools/module/module_tools.py
--rw-r--r--   0        0        0    11056 2023-06-21 02:31:04.067165 tdf_tool-2.1.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc
--rw-r--r--   0        0        0     5241 2023-07-17 08:24:09.269631 tdf_tool-2.1.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc
--rw-r--r--   0        0        0     9752 2023-06-21 03:12:06.540634 tdf_tool-2.1.8/tdf_tool/tools/package/seal_off_package_utils.py
--rw-r--r--   0        0        0      911 2023-06-21 02:31:04.067712 tdf_tool-2.1.8/tdf_tool/tools/platform_tools.py
--rw-r--r--   0        0        0     1112 2023-07-17 09:44:17.292892 tdf_tool-2.1.8/tdf_tool/tools/print.py
--rw-r--r--   0        0        0     7598 2023-06-21 03:12:06.261413 tdf_tool-2.1.8/tdf_tool/tools/regular_tool.py
--rw-r--r--   0        0        0     5744 2023-06-21 03:12:06.261176 tdf_tool-2.1.8/tdf_tool/tools/shell_dir.py
--rw-r--r--   0        0        0     3840 2023-06-21 02:31:04.068490 tdf_tool-2.1.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc
--rw-r--r--   0        0        0     2135 2023-07-17 08:24:09.224646 tdf_tool-2.1.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc
--rw-r--r--   0        0        0     2695 2023-06-21 02:31:04.068830 tdf_tool-2.1.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     1652 2023-07-17 08:24:09.247309 tdf_tool-2.1.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0    11711 2023-06-21 02:31:04.069307 tdf_tool-2.1.8/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     1999 2023-06-21 03:12:05.852140 tdf_tool-2.1.8/tdf_tool/tools/translate/file_util.py
--rw-r--r--   0        0        0    15484 2023-06-21 02:31:04.069828 tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     8259 2023-07-17 08:24:09.220923 tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0    26818 2023-06-21 02:31:04.070315 tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc
--rw-r--r--   0        0        0    13401 2023-07-17 08:24:09.146999 tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0    10691 2023-06-21 03:12:06.578332 tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/flutter_translate_lint.py
--rw-r--r--   0        0        0    18954 2023-06-21 03:12:07.368394 tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/flutter_translate_tools.py
--rw-r--r--   0        0        0     8395 2023-06-21 02:31:04.071283 tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc
--rw-r--r--   0        0        0     4569 2023-07-17 08:24:09.223168 tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc
--rw-r--r--   0        0        0     5228 2023-06-21 03:12:06.079172 tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py
--rw-r--r--   0        0        0      859 2023-06-21 02:31:04.071917 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc
--rw-r--r--   0        0        0     7351 2023-06-21 02:31:04.072189 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc
--rw-r--r--   0        0        0     7599 2023-06-21 02:31:04.072359 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc
--rw-r--r--   0        0        0     4190 2023-07-17 08:24:09.226607 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc
--rw-r--r--   0        0        0     3952 2023-06-21 02:31:04.072731 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc
--rw-r--r--   0        0        0     2321 2023-07-17 08:24:09.248904 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc
--rw-r--r--   0        0        0      870 2023-06-21 02:31:04.073029 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc
--rw-r--r--   0        0        0     4766 2023-06-21 02:31:04.073248 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     6219 2023-06-21 02:31:04.073438 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc
--rw-r--r--   0        0        0     2631 2023-06-21 02:31:04.073617 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc
--rw-r--r--   0        0        0     4438 2023-06-21 03:12:06.060679 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/ios_translate.py
--rw-r--r--   0        0        0     2000 2023-06-21 03:12:05.851695 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/ios_translate_lint.py
--rw-r--r--   0        0        0     5061 2023-06-21 02:31:04.074222 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc
--rw-r--r--   0        0        0     2826 2023-07-17 08:24:09.228819 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc
--rw-r--r--   0        0        0    17576 2023-06-21 02:31:04.074611 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc
--rw-r--r--   0        0        0     9280 2023-07-17 08:24:09.231738 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc
--rw-r--r--   0        0        0     7901 2023-06-21 02:31:04.075044 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc
--rw-r--r--   0        0        0     4372 2023-07-17 08:24:09.245596 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc
--rw-r--r--   0        0        0     1158 2023-06-21 02:31:04.075359 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc
--rw-r--r--   0        0        0     1002 2023-07-17 08:24:09.232973 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc
--rw-r--r--   0        0        0    10070 2023-06-21 02:31:04.075692 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc
--rw-r--r--   0        0        0     5340 2023-07-17 08:24:09.235247 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc
--rw-r--r--   0        0        0     2773 2023-06-21 02:31:04.076018 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc
--rw-r--r--   0        0        0     2663 2023-07-17 08:24:09.240527 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc
--rw-r--r--   0        0        0    11353 2023-06-21 02:31:04.076362 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc
--rw-r--r--   0        0        0     6200 2023-07-17 08:24:09.243096 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc
--rw-r--r--   0        0        0     4943 2023-06-21 02:31:04.076714 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc
--rw-r--r--   0        0        0     2661 2023-07-17 08:24:09.236832 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc
--rw-r--r--   0        0        0     3270 2023-06-21 03:12:06.079138 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py
--rw-r--r--   0        0        0    14326 2023-06-21 03:12:06.559653 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/ios_module.py
--rw-r--r--   0        0        0     5223 2023-06-21 03:12:06.225517 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py
--rw-r--r--   0        0        0     1189 2023-06-21 02:31:04.077541 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py
--rw-r--r--   0        0        0     8191 2023-06-21 03:12:06.261115 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py
--rw-r--r--   0        0        0     2337 2023-06-21 02:31:04.077863 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/location_string_temp.py
--rw-r--r--   0        0        0     8684 2023-06-21 03:12:07.158038 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/podspec.py
--rw-r--r--   0        0        0     2886 2023-06-21 03:12:06.261520 tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/string_util.py
--rw-r--r--   0        0        0     8625 2023-06-21 02:31:04.078483 tdf_tool-2.1.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc
--rw-r--r--   0        0        0     5006 2023-07-17 08:24:09.239263 tdf_tool-2.1.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc
--rw-r--r--   0        0        0     5111 2023-06-21 03:12:06.243717 tdf_tool-2.1.8/tdf_tool/tools/translate/tools/translate_tool.py
--rw-r--r--   0        0        0     1408 2023-06-21 03:12:05.851584 tdf_tool-2.1.8/tdf_tool/tools/translate/translate_lint.py
--rw-r--r--   0        0        0     1268 2023-06-21 02:31:04.079222 tdf_tool-2.1.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc
--rw-r--r--   0        0        0      854 2023-07-17 08:24:09.138752 tdf_tool-2.1.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc
--rw-r--r--   0        0        0      440 2023-06-21 03:12:05.832157 tdf_tool-2.1.8/tdf_tool/tools/vscode/vscode.py
--rw-r--r--   0        0        0    11029 2023-07-21 12:10:06.432807 tdf_tool-2.1.8/setup.py
--rw-r--r--   0        0        0    10466 2023-07-21 12:10:06.433256 tdf_tool-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-21 02:31:04.044131 tdf_tool-2.1.9/LICENSE
+-rw-r--r--   0        0        0     9217 2023-07-17 07:59:26.799207 tdf_tool-2.1.9/README.md
+-rw-r--r--   0        0        0     1608 2023-07-21 12:52:14.293685 tdf_tool-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-07-20 10:16:56.395361 tdf_tool-2.1.9/tdf_tool/app.py
+-rw-r--r--   0        0        0      973 2023-06-21 03:12:05.604731 tdf_tool-2.1.9/tdf_tool/pipeline.py
+-rw-r--r--   0        0        0      424 2023-06-21 02:31:04.047403 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0     2567 2023-06-21 02:31:04.047684 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc
+-rw-r--r--   0        0        0     1651 2023-07-17 08:24:09.257737 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc
+-rw-r--r--   0        0        0     2668 2023-06-21 02:31:04.048055 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc
+-rw-r--r--   0        0        0     1603 2023-07-17 08:24:09.271291 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc
+-rw-r--r--   0        0        0      496 2023-06-21 02:31:04.048397 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/init.cpython-39.pyc
+-rw-r--r--   0        0        0     3015 2023-06-21 02:31:04.048562 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc
+-rw-r--r--   0        0        0     2021 2023-07-17 08:24:08.899762 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc
+-rw-r--r--   0        0        0     2981 2023-06-21 02:31:04.048893 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc
+-rw-r--r--   0        0        0     2218 2023-07-17 08:24:09.266984 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc
+-rw-r--r--   0        0        0    36213 2023-06-21 02:31:04.049422 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc
+-rw-r--r--   0        0        0    19495 2023-07-17 09:12:25.271862 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc
+-rw-r--r--   0        0        0     3262 2023-06-21 02:31:04.050018 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc
+-rw-r--r--   0        0        0     1964 2023-07-17 08:24:09.141480 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc
+-rw-r--r--   0        0        0      817 2023-06-21 02:31:04.050452 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc
+-rw-r--r--   0        0        0      595 2023-07-17 08:24:09.272692 tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc
+-rw-r--r--   0        0        0     1246 2023-06-21 03:12:05.603571 tdf_tool-2.1.9/tdf_tool/pipelines/fix_header.py
+-rw-r--r--   0        0        0     1212 2023-06-21 03:12:05.777495 tdf_tool-2.1.9/tdf_tool/pipelines/git.py
+-rw-r--r--   0        0        0     1431 2023-06-21 03:12:05.832235 tdf_tool-2.1.9/tdf_tool/pipelines/module.py
+-rw-r--r--   0        0        0     1634 2023-06-21 03:12:05.832106 tdf_tool-2.1.9/tdf_tool/pipelines/package.py
+-rw-r--r--   0        0        0    26719 2023-07-21 12:09:52.162579 tdf_tool-2.1.9/tdf_tool/pipelines/router.py
+-rw-r--r--   0        0        0     1659 2023-06-21 03:12:05.832050 tdf_tool-2.1.9/tdf_tool/pipelines/translate.py
+-rw-r--r--   0        0        0      179 2023-07-17 07:59:32.656005 tdf_tool-2.1.9/tdf_tool/pipelines/upgrade.py
+-rw-r--r--   0        0        0     1653 2023-06-21 02:31:04.052779 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc
+-rw-r--r--   0        0        0     1038 2023-07-17 08:24:09.026923 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc
+-rw-r--r--   0        0        0    10270 2023-06-21 02:31:04.053400 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc
+-rw-r--r--   0        0        0     5123 2023-07-17 08:24:09.016694 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc
+-rw-r--r--   0        0        0     1328 2023-06-21 02:31:04.054020 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/env.cpython-311.pyc
+-rw-r--r--   0        0        0      873 2023-07-17 08:24:09.028816 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/env.cpython-39.pyc
+-rw-r--r--   0        0        0     2480 2023-06-21 02:31:04.054546 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     1438 2023-07-17 08:24:09.151442 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     2969 2023-06-21 02:31:04.054996 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/print.cpython-311.pyc
+-rw-r--r--   0        0        0     1855 2023-07-17 09:44:23.214841 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/print.cpython-39.pyc
+-rw-r--r--   0        0        0     9661 2023-06-21 02:31:04.055529 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     6155 2023-07-17 08:24:09.154070 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc
+-rw-r--r--   0        0        0    10739 2023-06-21 02:31:04.056124 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc
+-rw-r--r--   0        0        0     5615 2023-07-17 08:24:09.024850 tdf_tool-2.1.9/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc
+-rw-r--r--   0        0        0    11432 2023-06-21 02:31:04.057084 tdf_tool-2.1.9/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc
+-rw-r--r--   0        0        0     6738 2023-07-20 11:08:20.395006 tdf_tool-2.1.9/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc
+-rw-r--r--   0        0        0     7216 2023-06-21 02:31:04.057686 tdf_tool-2.1.9/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc
+-rw-r--r--   0        0        0     3688 2023-07-17 08:24:08.903584 tdf_tool-2.1.9/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc
+-rw-r--r--   0        0        0     1809 2023-07-20 07:43:35.811934 tdf_tool-2.1.9/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc
+-rw-r--r--   0        0        0     1628 2023-07-20 07:43:31.587168 tdf_tool-2.1.9/tdf_tool/tools/cli/bean/deps_item.py
+-rw-r--r--   0        0        0    10059 2023-07-21 12:52:04.819159 tdf_tool-2.1.9/tdf_tool/tools/cli/module_deps_rewrite.py
+-rw-r--r--   0        0        0     4715 2023-06-21 03:12:05.851780 tdf_tool-2.1.9/tdf_tool/tools/cli/project_cli.py
+-rw-r--r--   0        0        0     1893 2023-07-20 11:01:33.451132 tdf_tool-2.1.9/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     1833 2023-07-20 11:01:30.457179 tdf_tool-2.1.9/tdf_tool/tools/cli/utils/yaml_utils.py
+-rw-r--r--   0        0        0      559 2023-06-21 03:12:05.832296 tdf_tool-2.1.9/tdf_tool/tools/cmd.py
+-rw-r--r--   0        0        0     7002 2023-06-21 02:31:04.059140 tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     3359 2023-07-17 08:24:09.061860 tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc
+-rw-r--r--   0        0        0     2717 2023-06-21 02:31:04.059653 tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1465 2023-07-17 08:24:09.134281 tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc
+-rw-r--r--   0        0        0     2693 2023-06-21 02:31:04.060168 tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0        0        0     2732 2023-06-21 02:31:04.060423 tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc
+-rw-r--r--   0        0        0     1886 2023-07-17 08:24:09.149229 tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc
+-rw-r--r--   0        0        0     9155 2023-06-21 02:31:04.060789 tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc
+-rw-r--r--   0        0        0     4406 2023-07-17 08:24:09.256080 tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc
+-rw-r--r--   0        0        0     3983 2023-06-21 03:12:06.205956 tdf_tool-2.1.9/tdf_tool/tools/config/config.py
+-rw-r--r--   0        0        0     1311 2023-06-21 03:12:06.079241 tdf_tool-2.1.9/tdf_tool/tools/config/initial_json_config.py
+-rw-r--r--   0        0        0     1120 2023-06-21 03:12:06.079047 tdf_tool-2.1.9/tdf_tool/tools/config/module_json_config.py
+-rw-r--r--   0        0        0     5593 2023-07-21 12:01:57.126418 tdf_tool-2.1.9/tdf_tool/tools/config/packages_config.py
+-rw-r--r--   0        0        0     7704 2023-06-21 03:12:05.852079 tdf_tool-2.1.9/tdf_tool/tools/dependencies_analysis.py
+-rw-r--r--   0        0        0      662 2023-06-21 03:12:05.604668 tdf_tool-2.1.9/tdf_tool/tools/env.py
+-rw-r--r--   0        0        0     6312 2023-06-21 02:31:04.062376 tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc
+-rw-r--r--   0        0        0     3590 2023-07-17 08:24:09.261201 tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc
+-rw-r--r--   0        0        0     3174 2023-06-21 02:31:04.062688 tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     1978 2023-07-17 08:24:09.259434 tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc
+-rw-r--r--   0        0        0     4314 2023-06-21 02:31:04.063007 tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     2438 2023-07-17 08:24:09.262748 tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     6437 2023-06-21 02:31:04.063372 tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     3655 2023-07-17 08:24:09.265080 tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     2422 2023-06-21 02:31:04.063692 tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     3345 2023-06-21 03:12:06.079100 tdf_tool-2.1.9/tdf_tool/tools/fix_header/fix_header_entry.py
+-rw-r--r--   0        0        0     1586 2023-06-21 03:12:05.851836 tdf_tool-2.1.9/tdf_tool/tools/fix_header/fix_header_lint.py
+-rw-r--r--   0        0        0     2137 2023-06-21 03:12:06.060569 tdf_tool-2.1.9/tdf_tool/tools/fix_header/fix_header_lint_tool.py
+-rw-r--r--   0        0        0     4095 2023-06-21 03:12:06.060768 tdf_tool-2.1.9/tdf_tool/tools/fix_header/fix_header_replace_tool.py
+-rw-r--r--   0        0        0     1159 2023-06-21 02:31:04.064465 tdf_tool-2.1.9/tdf_tool/tools/flutter_script.py
+-rw-r--r--   0        0        0     7243 2023-06-21 02:31:04.064796 tdf_tool-2.1.9/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     4143 2023-07-17 08:24:09.136658 tdf_tool-2.1.9/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     7055 2023-06-21 02:31:04.065169 tdf_tool-2.1.9/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc
+-rw-r--r--   0        0        0     3760 2023-07-17 08:24:09.064237 tdf_tool-2.1.9/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc
+-rw-r--r--   0        0        0      593 2023-06-21 02:31:04.065493 tdf_tool-2.1.9/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc
+-rw-r--r--   0        0        0     4993 2023-06-21 03:12:06.079521 tdf_tool-2.1.9/tdf_tool/tools/gitlab/gitlab_utils.py
+-rw-r--r--   0        0        0     3814 2023-06-21 03:12:05.851649 tdf_tool-2.1.9/tdf_tool/tools/gitlab/python_gitlab_api.py
+-rw-r--r--   0        0        0     2482 2023-06-21 02:31:04.066493 tdf_tool-2.1.9/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     1386 2023-07-17 08:24:09.059310 tdf_tool-2.1.9/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     1063 2023-06-21 03:12:06.079438 tdf_tool-2.1.9/tdf_tool/tools/module/module_tools.py
+-rw-r--r--   0        0        0    11056 2023-06-21 02:31:04.067165 tdf_tool-2.1.9/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc
+-rw-r--r--   0        0        0     5241 2023-07-17 08:24:09.269631 tdf_tool-2.1.9/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     9752 2023-06-21 03:12:06.540634 tdf_tool-2.1.9/tdf_tool/tools/package/seal_off_package_utils.py
+-rw-r--r--   0        0        0      911 2023-06-21 02:31:04.067712 tdf_tool-2.1.9/tdf_tool/tools/platform_tools.py
+-rw-r--r--   0        0        0     1112 2023-07-17 09:44:17.292892 tdf_tool-2.1.9/tdf_tool/tools/print.py
+-rw-r--r--   0        0        0     7598 2023-06-21 03:12:06.261413 tdf_tool-2.1.9/tdf_tool/tools/regular_tool.py
+-rw-r--r--   0        0        0     5744 2023-06-21 03:12:06.261176 tdf_tool-2.1.9/tdf_tool/tools/shell_dir.py
+-rw-r--r--   0        0        0     3840 2023-06-21 02:31:04.068490 tdf_tool-2.1.9/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc
+-rw-r--r--   0        0        0     2135 2023-07-17 08:24:09.224646 tdf_tool-2.1.9/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc
+-rw-r--r--   0        0        0     2695 2023-06-21 02:31:04.068830 tdf_tool-2.1.9/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     1652 2023-07-17 08:24:09.247309 tdf_tool-2.1.9/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0    11711 2023-06-21 02:31:04.069307 tdf_tool-2.1.9/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     1999 2023-06-21 03:12:05.852140 tdf_tool-2.1.9/tdf_tool/tools/translate/file_util.py
+-rw-r--r--   0        0        0    15484 2023-06-21 02:31:04.069828 tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     8259 2023-07-17 08:24:09.220923 tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0    26818 2023-06-21 02:31:04.070315 tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc
+-rw-r--r--   0        0        0    13401 2023-07-17 08:24:09.146999 tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0    10691 2023-06-21 03:12:06.578332 tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/flutter_translate_lint.py
+-rw-r--r--   0        0        0    18954 2023-06-21 03:12:07.368394 tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/flutter_translate_tools.py
+-rw-r--r--   0        0        0     8395 2023-06-21 02:31:04.071283 tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc
+-rw-r--r--   0        0        0     4569 2023-07-17 08:24:09.223168 tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc
+-rw-r--r--   0        0        0     5228 2023-06-21 03:12:06.079172 tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py
+-rw-r--r--   0        0        0      859 2023-06-21 02:31:04.071917 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc
+-rw-r--r--   0        0        0     7351 2023-06-21 02:31:04.072189 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc
+-rw-r--r--   0        0        0     7599 2023-06-21 02:31:04.072359 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc
+-rw-r--r--   0        0        0     4190 2023-07-17 08:24:09.226607 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc
+-rw-r--r--   0        0        0     3952 2023-06-21 02:31:04.072731 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc
+-rw-r--r--   0        0        0     2321 2023-07-17 08:24:09.248904 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc
+-rw-r--r--   0        0        0      870 2023-06-21 02:31:04.073029 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc
+-rw-r--r--   0        0        0     4766 2023-06-21 02:31:04.073248 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     6219 2023-06-21 02:31:04.073438 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc
+-rw-r--r--   0        0        0     2631 2023-06-21 02:31:04.073617 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc
+-rw-r--r--   0        0        0     4438 2023-06-21 03:12:06.060679 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/ios_translate.py
+-rw-r--r--   0        0        0     2000 2023-06-21 03:12:05.851695 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/ios_translate_lint.py
+-rw-r--r--   0        0        0     5061 2023-06-21 02:31:04.074222 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     2826 2023-07-17 08:24:09.228819 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc
+-rw-r--r--   0        0        0    17576 2023-06-21 02:31:04.074611 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc
+-rw-r--r--   0        0        0     9280 2023-07-17 08:24:09.231738 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc
+-rw-r--r--   0        0        0     7901 2023-06-21 02:31:04.075044 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc
+-rw-r--r--   0        0        0     4372 2023-07-17 08:24:09.245596 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc
+-rw-r--r--   0        0        0     1158 2023-06-21 02:31:04.075359 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc
+-rw-r--r--   0        0        0     1002 2023-07-17 08:24:09.232973 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc
+-rw-r--r--   0        0        0    10070 2023-06-21 02:31:04.075692 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc
+-rw-r--r--   0        0        0     5340 2023-07-17 08:24:09.235247 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc
+-rw-r--r--   0        0        0     2773 2023-06-21 02:31:04.076018 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc
+-rw-r--r--   0        0        0     2663 2023-07-17 08:24:09.240527 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc
+-rw-r--r--   0        0        0    11353 2023-06-21 02:31:04.076362 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc
+-rw-r--r--   0        0        0     6200 2023-07-17 08:24:09.243096 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc
+-rw-r--r--   0        0        0     4943 2023-06-21 02:31:04.076714 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc
+-rw-r--r--   0        0        0     2661 2023-07-17 08:24:09.236832 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc
+-rw-r--r--   0        0        0     3270 2023-06-21 03:12:06.079138 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py
+-rw-r--r--   0        0        0    14326 2023-06-21 03:12:06.559653 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/ios_module.py
+-rw-r--r--   0        0        0     5223 2023-06-21 03:12:06.225517 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py
+-rw-r--r--   0        0        0     1189 2023-06-21 02:31:04.077541 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py
+-rw-r--r--   0        0        0     8191 2023-06-21 03:12:06.261115 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py
+-rw-r--r--   0        0        0     2337 2023-06-21 02:31:04.077863 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/location_string_temp.py
+-rw-r--r--   0        0        0     8684 2023-06-21 03:12:07.158038 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/podspec.py
+-rw-r--r--   0        0        0     2886 2023-06-21 03:12:06.261520 tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/string_util.py
+-rw-r--r--   0        0        0     8625 2023-06-21 02:31:04.078483 tdf_tool-2.1.9/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     5006 2023-07-17 08:24:09.239263 tdf_tool-2.1.9/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc
+-rw-r--r--   0        0        0     5111 2023-06-21 03:12:06.243717 tdf_tool-2.1.9/tdf_tool/tools/translate/tools/translate_tool.py
+-rw-r--r--   0        0        0     1408 2023-06-21 03:12:05.851584 tdf_tool-2.1.9/tdf_tool/tools/translate/translate_lint.py
+-rw-r--r--   0        0        0     1268 2023-06-21 02:31:04.079222 tdf_tool-2.1.9/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc
+-rw-r--r--   0        0        0      854 2023-07-17 08:24:09.138752 tdf_tool-2.1.9/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc
+-rw-r--r--   0        0        0      440 2023-06-21 03:12:05.832157 tdf_tool-2.1.9/tdf_tool/tools/vscode/vscode.py
+-rw-r--r--   0        0        0    11029 2023-07-21 12:52:17.668451 tdf_tool-2.1.9/setup.py
+-rw-r--r--   0        0        0    10466 2023-07-21 12:52:17.668891 tdf_tool-2.1.9/PKG-INFO
```

### Comparing `tdf_tool-2.1.8/LICENSE` & `tdf_tool-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/README.md` & `tdf_tool-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/pyproject.toml` & `tdf_tool-2.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 项目信息
 [tool.poetry]
 name = "tdf_tool"
-version = "2.1.8"
+version = "2.1.9"
 description = "二维火 flutter 脚手架工具"
 authors = ["Jian Xu <3386218996@qq.com>", "FanJiao Gai <gaijiaofan@2dfire.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://git.2dfire.net/app/flutter/tools/package_tools"
 repository = "https://git.2dfire.net/app/flutter/tools/package_tools.git"
 keywords = ["tdf", "tdf-tool", "tdf_tool"]
```

### Comparing `tdf_tool-2.1.8/tdf_tool/pipeline.py` & `tdf_tool-2.1.9/tdf_tool/pipeline.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/fix_header.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/fix_header.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/git.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/git.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/package.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/package.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/router.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/router.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/translate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/translate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/upgrade.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/pipelines/__pycache__/upgrade.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/fix_header.py` & `tdf_tool-2.1.9/tdf_tool/pipelines/fix_header.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/git.py` & `tdf_tool-2.1.9/tdf_tool/pipelines/git.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/module.py` & `tdf_tool-2.1.9/tdf_tool/pipelines/module.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/package.py` & `tdf_tool-2.1.9/tdf_tool/pipelines/package.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/router.py` & `tdf_tool-2.1.9/tdf_tool/pipelines/router.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/pipelines/translate.py` & `tdf_tool-2.1.9/tdf_tool/pipelines/translate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/cmd.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/cmd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/dependencies_analysis.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/env.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/env.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/env.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/env.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/platform_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/platform_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/print.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/print.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/print.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/print.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/regular_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/regular_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/shell_dir.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/__pycache__/shell_dir.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/cli/__pycache__/module_deps_rewrite.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/cli/__pycache__/project_cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/cli/__pycache__/project_cli.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/cli/bean/__pycache__/deps_item.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/cli/bean/deps_item.py` & `tdf_tool-2.1.9/tdf_tool/tools/cli/bean/deps_item.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/cli/module_deps_rewrite.py` & `tdf_tool-2.1.9/tdf_tool/tools/cli/module_deps_rewrite.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         self._writeNewDeps("./", self.moduleNameList)
         
 
     def _writeNewDeps(self, modulePath: str, deps: list[str], isShell: bool = True):
         yamlFileUtils = YamlFileUtils(modulePath)
         depsKeys = yamlFileUtils.readOverrideDepsKeys()
         # 重写的依赖不一致，则需要重写并执行pub upgrade
-        if sorted(depsKeys) != sorted(deps) and self.existDepsResult(modulePath):
+        if sorted(depsKeys) != sorted(deps) and self.existDepsResult(modulePath) is not True:
             yamlFileUtils.writeOverrideDeps(deps, isShell=isShell)
             # 依赖重写完，执行pub upgrade更新lock文件
             command = "flutter pub upgrade"
             result = subprocess.run(command, shell=True, capture_output=True, text=True, cwd=modulePath)
             print("Standard Output:", result.stdout)
             Print.debug("lock文件已更新")
```

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/cli/project_cli.py` & `tdf_tool-2.1.9/tdf_tool/tools/cli/project_cli.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/cli/utils/__pycache__/yaml_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/cli/utils/yaml_utils.py` & `tdf_tool-2.1.9/tdf_tool/tools/cli/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/cmd.py` & `tdf_tool-2.1.9/tdf_tool/tools/cmd.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/initial_json_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/json.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/module_json_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/module_json_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/packages_config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/config/__pycache__/packages_config.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/config.py` & `tdf_tool-2.1.9/tdf_tool/tools/config/config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/initial_json_config.py` & `tdf_tool-2.1.9/tdf_tool/tools/config/initial_json_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/module_json_config.py` & `tdf_tool-2.1.9/tdf_tool/tools/config/module_json_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/config/packages_config.py` & `tdf_tool-2.1.9/tdf_tool/tools/config/packages_config.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/dependencies_analysis.py` & `tdf_tool-2.1.9/tdf_tool/tools/dependencies_analysis.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/env.py` & `tdf_tool-2.1.9/tdf_tool/tools/env.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_entry.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_lint_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_replace_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/__pycache__/fix_header_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/fix_header_entry.py` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/fix_header_entry.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/fix_header_lint.py` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/fix_header_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/fix_header_lint_tool.py` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/fix_header_lint_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/fix_header/fix_header_replace_tool.py` & `tdf_tool-2.1.9/tdf_tool/tools/fix_header/fix_header_replace_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/flutter_script.py` & `tdf_tool-2.1.9/tdf_tool/tools/flutter_script.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/gitlab/__pycache__/gitlab_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/gitlab/__pycache__/python_gitlab_api.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/gitlab/__pycache__/raw_git.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/gitlab/gitlab_utils.py` & `tdf_tool-2.1.9/tdf_tool/tools/gitlab/gitlab_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/gitlab/python_gitlab_api.py` & `tdf_tool-2.1.9/tdf_tool/tools/gitlab/python_gitlab_api.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/module/__pycache__/module_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/module/__pycache__/module_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/module/module_tools.py` & `tdf_tool-2.1.9/tdf_tool/tools/module/module_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/package/__pycache__/seal_off_package_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/package/seal_off_package_utils.py` & `tdf_tool-2.1.9/tdf_tool/tools/package/seal_off_package_utils.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/platform_tools.py` & `tdf_tool-2.1.9/tdf_tool/tools/platform_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/print.py` & `tdf_tool-2.1.9/tdf_tool/tools/print.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/regular_tool.py` & `tdf_tool-2.1.9/tdf_tool/tools/regular_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/shell_dir.py` & `tdf_tool-2.1.9/tdf_tool/tools/shell_dir.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/__pycache__/file_util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/__pycache__/file_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/__pycache__/translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/__pycache__/translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/file_util.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/file_util.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/__pycache__/flutter_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/flutter_translate_lint.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/flutter_translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/flutter_translate_tools.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/flutter_translate_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/tools/__pycache__/flutter_translate_integrate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/flutter/tools/flutter_translate_integrate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/file_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_lint.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_pattern.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/ios_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/podspec.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/__pycache__/string_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/ios_translate.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/ios_translate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/ios_translate_lint.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/ios_translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/batch_pod_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_module.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_integrate.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_pattern.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/ios_translate_tools.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/location_string_temp.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/podspec.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/__pycache__/string_util.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/batch_pod_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/ios_module.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/ios_module.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/ios_translate_integrate.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/ios_translate_pattern.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/ios_translate_tools.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/location_string_temp.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/location_string_temp.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/podspec.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/podspec.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/ios/tools/string_util.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/ios/tools/string_util.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/translate/tools/__pycache__/translate_tool.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/tools/translate_tool.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/tools/translate_tool.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/translate/translate_lint.py` & `tdf_tool-2.1.9/tdf_tool/tools/translate/translate_lint.py`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/vscode/__pycache__/vscode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc` & `tdf_tool-2.1.9/tdf_tool/tools/vscode/__pycache__/vscode.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `tdf_tool-2.1.8/setup.py` & `tdf_tool-2.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'ruamel.yaml>=0.17.21,<0.18.0']
 
 entry_points = \
 {'console_scripts': ['tdf_tool = tdf_tool.app:main', 'tl = tdf_tool.app:main']}
 
 setup_kwargs = {
     'name': 'tdf-tool',
-    'version': '2.1.8',
+    'version': '2.1.9',
     'description': '二维火 flutter 脚手架工具',
     'long_description': '## 帮助文档\n\n```shell\nNAME\n    tdf_tool - 二维火 Flutter 脚手架工具，包含项目构建，依赖分析，git等功能。。\n\nSYNOPSIS\n    tdf_tool GROUP | COMMAND\n\nDESCRIPTION\n    二维火 Flutter 脚手架工具，包含项目构建，依赖分析，git等功能。。\n\nGROUPS\n    GROUP is one of the following:\n\n     module\n       模块相关工具： tdf_tool module -h 查看详情\n\n     package\n       封包工具相关：tdf_tool package -h 查看详情\n\n     translate\n       国际化相关：tdf_tool translate -h 查看详情\n\nCOMMANDS\n    COMMAND is one of the following:\n\n     git\n       tdf_tool git【git 命令】：批量操作 git 命令, 例如 tdf_tool git push\n\n     router\n       tdf_tool router：会以交互式进行路由操作，对指定的模块执行路由生成和路由注册逻辑\n\n     upgrade\n       tdf_tool upgrade：升级插件到最新版本\n        \n```\n\n\n\n## 插件安装方式\n\n安装python包\n\n```\npip3 install tdf-tool --user\n```\n\n安装并更新python包\n\n```\npip3 install --upgrade tdf-tool --user\n```\n\n安装测试环境python包\n\n```\npip3 install -i https://test.pypi.org/simple/ tdf-tool --user\n```\n\n安装并更新测试环境python包\n\n```\npip3 install --upgrade -i https://test.pypi.org/simple/ tdf-tool --user\n```\n\n\n\n## 工具使用流程说明\n\n### 1.准备工作\n\n- 确保python的bin插件目录已经被配置到环境变量中（这一步不满足的话，插件安装之后是无法识别到本插件命令的）\n\n- 在~目录下，创建.tdf_tool_config文件并配置相关必需属性如下\n\n```json\ngit_private_token=***\n```\n\ngit_private_token是gitlab的token\n\n获取途径：进入gitlab页面，点击右上角头像，选择Preferences，选择左侧列表中的AccessToken进行创建\n\n**上述步骤如果没有做，会在使用插件时，会有提示**\n\n### 2.初始化\n\n#### i.进入壳目录（确保执行命令在壳目录内）\n\n#### ii.执行tdf_tool module init\n\n- 判断当前目录是否存在tdf_cache，若不存在，则会自动创建tdf_cache\n- 自动读取当前壳模块名称，写入initial_config.json配置文件；\n- 读取当前壳分支，写入initial_config.json配置文件；\n- 交互式提示用户输入需要开发的模块名并写入initial_config.json配置文件的moduleNameList列表字段中\n- ！退出，即输入完成\n- 自动clone所有开发模块到  ```../.tdf_flutter```  隐藏目录中；\n- 将所有开发模块分支切换至与壳一致；\n- 自动分析依赖树，并**由下至上**对所有模块自动执行```flutter pub upgrade```;\n\n#### iii.开发过程中\n\n##### 1.开发模块添加\n\n- 若是有新模块需要添加入开发模块中，可直接修改initial_config.json配置文件，修改moduleNameList字段；\n- 执行tdf_tool deps更新依赖\n\n##### 2.新开发模块添加\n\n- 添加新模块后，会提示找不到模块，实际查找的是```tdf_cache```文件夹中的module_config.json文件；\n- 如果没有找到该模块，则可以执行```tdf_tool module-update```,更新远程module_config.json文件；\n- 删掉本地的module_config.json文件，重新执行命令即可，脚本会自动判断本地是否存在该配置文件，如果不存在会**下载**；\n\n<span style="color:#ff0000">请确保gitlab仓库的新开发模块master分支是一个flutter模块，如果判定不是flutter模块，则会报错（判定条件为存在pubspec.yaml文件）</span>\n\n\n\n### 3.版本控制\n\n版本控制请使用tdf_tool命令，命令详情可使用  ```tdf_tool -h```  查看，现已支持大部分命令，若有特殊命令需要执行，可以使用  ```tdf_tool <git命令>``` ，如：```tdf_tool git add .```\n\n\n\n### 4.自动打包发布\n\n暂未接入打包工具，预计下一季度进行支持；\n\n\n\n**<span style="color:#ff0000">FAQ</span>**\n\nwindows系统请使用bash命令；\n\n\n\n## 额外功能说明\n\n### 1.二维数组表达依赖树\n\n生成一个二维数组，可根据该二维数组的数据进行**并发**打tag，每一层的模块，都可以同时进行打tag发布操作，减少发布耗时；\n\n```json\n[\n\t["tdf_channel", "tdf_event", "tdf_network"], \n\t["tdf_widgets"], \n\t["tdf_smart_devices", "tdf_account_module"], \n\t["flutter_reset_module"]\n]\n```\n\n如上数据，数组中每一个节点中的模块均可同时打tag，节点之间需要由上至下的顺序进行tag操作\n\n\n\n### 2.插件更新\n\n执行 ```tdf_tool upgrade```\n\n\n\n### 3.远程模块配置文件更新\n\n执行 ```tdf_tool module module_update```\n\n\n\n## 依赖树分析原理\n\n采用有向有/无环图进行依赖树的分析\n\n数据结构采用如下：\n\n```python\nclass DependencyNode:\n    def __init__(self):\n        self.nodeName = \'\'\n        self.parent = []  # 父亲节点列表\n        self.children = []  # 子孙节点列表\n        self.delete = False\n```\n\n![dependency](./README_DIR/dependency.png)\n\n如上图1：一个正常的依赖树表示；\n\n如上图2：对图1中，依赖树所有节点去重，变换为图2有向图；\t\n\n\n\n**分析流程：**\n\n**依赖图构建**\n\n```python\n# 生成依赖图\n    def _generateDependenciesMap(self):\n        for package in self.__moduleDependenciesMap:\n            for module in moduleNameList:\n                if package == module:\n                    # 到这一步表明当前这个模块属于开发模块且在当前模块的依赖模块列表中，是当前模块的子模块\n                    self._mNodeDict[self.__moduleName].children.append(package)\n                    self._mNodeDict[package].parent.append(self.__moduleName)\n```\n\n- 共5个节点\n\n  - node构建：\n\n    - ```python\n      {\n      \t"模块1":{\n          "nodeNmae": "模块1",\n          "parent": [],\n          "children": ["模块2","模块3","模块4","模块5"],\n          "delete": False\n      \t},\n      \t"模块2":{\n          "nodeNmae": "模块2",\n          "parent": ["模块1"],\n          "children": ["模块4","模块5"],\n          "delete": False\n      \t}\n      \t"模块3":{\n          "nodeNmae": "模块3",\n          "parent": ["模块1"],\n          "children": ["模块5"],\n          "delete": False\n      \t}\n      \t"模块4":{\n          "nodeNmae": "模块4",\n          "parent": ["模块1","模块2"],\n          "children": [],\n          "delete": False\n      \t}\n      \t"模块5":{\n          "nodeNmae": "模块5",\n          "parent": ["模块1","模块2","模块3"],\n          "children": [],\n          "delete": False\n      \t}\n      }\n      ```\n\n**依赖图解析伪代码（以一维数组为例）**\n\n```python\n# 返回二维数组，用于并发打tag\n    def _generateDependenciesOrder(self):\n        resList = []\n        while 存在节点delete属性不为True:\n            \n            for：查找子节点为0的节点\n            \t设置节点delete属性为True\n              \n            for：deleteItemList = 拿到所有delete属性为true的节点\n\n            for：遍历所有节点，如果节点的子节点中包含deleteItemList的节点，则将其从子节点列表中删除\n```\n\n\n\n\n\n- **initial_config.json文件说明**\n\n  ```json\n  {\n      "featureBranch": "feature/test_dev_1", // 开发分支\n      "shellName": "flutter_reset_module",\n      // 项目需要开发的模块,可自由配置\n      "moduleNameList": [\n          "flutter_reset_module",\n          "tdf_smart_devices",\n          "tdf_widgets",\n          "tdf_channel"\n      ]\n  }\n  ```\n\n- **module_config.json文件说明**\n\n  ```json\n  {\n      "flutter_globalyun_us_module": {\n        \t"id": "11111"\n          "type": "shell",\n          "git": "git@git.2dfire.net:app/flutter/app/flutter_globalyun_us_module.git"\n      },\n      "tdf_router_anno": {\n          "type": "base",\n          "git": "git@git.2dfire.net:app/flutter/app/tdf_router_anno.git"\n      },\n  }\n  //语意\n  {\n    "模块名":{\n      "id": 项目gitlab id\n      "类型": gitlab group名\n      "git": gitlab地址\n    }\n  }\n  ```\n\n\n\n## 后续计划\n\n<span style="color:#ff0000">**问题：**</span>由于现在flutter ci 【lint】【tag】任务脚本成功率过于低，很多时候是因为项目模块的配置问题导致的，且后续会接入一键打tag工具\n\n方案：在执行统一push前，对所有模块的项目配置信息进行校验，确保数据规范；\n\n\n\n## 插件打包发布命令\n\n**插件打包命令**\n\n```\npoetry build\n```\n**插件发布命令**\n\n```\npoetry publish\n```\n\n## History\n\n### 2.1.00\n\n- 路由功能支持flutter版本3.3.10，兼容flutter版本2.2.3；\n\n### 2.0.61\n\n- Flutter国际化字符串整合；\n\n### 2.0.38\n\n- 路由生成完后增加路由相关代码format（解决windows代码生成后顺序错乱）；\n\n### 2.0.01\n\n- Cli 框架升级；\n- 代码重构；\n\n### **1.1.00（2022-4-28）**\n\n- 国际化解决输出json中包含转义字符的问题，如\\n；\n- 四类语言输出文件自动格式化\n\n### **1.0.55（2022-4-28）**\n\n- 国际化key使用中文（依照ios项目开发形式）；\n\n### **1.0.53（2022-4-28）**\n\n- 国际化流程中，兼容解决部分json解析失败问题，譬如字符串中包含"="符号；\n\n> 错误日志如：Unterminated string starting at: line 1 column 5650 (char 5649)\n\n### **1.0.50（2022-4-28）**\n\n- 国际化增加繁体字翻译；\n\n',
     'author': 'Jian Xu',
     'author_email': '3386218996@qq.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://git.2dfire.net/app/flutter/tools/package_tools',
```

### Comparing `tdf_tool-2.1.8/PKG-INFO` & `tdf_tool-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdf-tool
-Version: 2.1.8
+Version: 2.1.9
 Summary: 二维火 flutter 脚手架工具
 Home-page: https://git.2dfire.net/app/flutter/tools/package_tools
 License: MIT
 Keywords: tdf,tdf-tool,tdf_tool
 Author: Jian Xu
 Author-email: 3386218996@qq.com
 Requires-Python: >=3.9.0,<4.0.0
```

