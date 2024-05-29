# Comparing `tmp/greatlibrarian-0.0.8.tar.gz` & `tmp/greatlibrarian-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greatlibrarian-0.0.8.tar", max compression
+gzip compressed data, was "greatlibrarian-0.0.9.tar", max compression
```

## Comparing `greatlibrarian-0.0.8.tar` & `greatlibrarian-0.0.9.tar`

### file list

```diff
@@ -1,763 +1,763 @@
--rw-r--r--   0        0        0        2 2024-04-25 07:41:33.407779 greatlibrarian-0.0.8/greatlibrarian/Agents/__init__.py
--rw-r--r--   0        0        0       29 2024-04-25 07:41:33.239109 greatlibrarian-0.0.8/greatlibrarian/Agents/BookStore/__init__.py
--rw-r--r--   0        0        0      713 2024-04-25 07:41:33.239109 greatlibrarian-0.0.8/greatlibrarian/Agents/BookStore/checkDupli.py
--rw-r--r--   0        0        0    12525 2024-04-25 07:41:33.239109 greatlibrarian-0.0.8/greatlibrarian/Agents/BookStore/getData.py
--rw-r--r--   0        0        0      342 2024-04-25 07:41:33.240106 greatlibrarian-0.0.8/greatlibrarian/Agents/BookStore/main.py
--rw-r--r--   0        0        0     8969 2024-04-25 07:41:33.239109 greatlibrarian-0.0.8/greatlibrarian/Agents/BookStore/RawData/Area Studies/African American Studies.csv
--rw-r--r--   0        0        0      953 2024-04-25 07:41:33.405787 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/__init__.py
--rw-r--r--   0        0        0       32 2024-04-25 07:41:33.405787 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/algebra.py
--rw-r--r--   0        0        0      164 2024-04-25 07:41:33.405787 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/codeComphnExp.py
--rw-r--r--   0        0        0      118 2024-04-25 07:41:33.405787 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/codeDefeIdentify.py
--rw-r--r--   0        0        0     2828 2024-04-25 07:41:33.405787 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/codeEnv.py
--rw-r--r--   0        0        0       77 2024-04-25 07:41:33.405787 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/codeOpt.py
--rw-r--r--   0        0        0       82 2024-04-25 07:41:33.406784 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/evalPerformance.py
--rw-r--r--   0        0        0      269 2024-04-25 07:41:33.406784 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/script_test.py
--rw-r--r--   0        0        0      438 2024-04-25 07:41:33.406784 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/test_code.json
--rw-r--r--   0        0        0     3240 2024-04-25 07:41:33.406784 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/ttest.py
--rw-r--r--   0        0        0     2310 2024-04-25 07:41:33.240106 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate
--rw-r--r--   0        0        0     1323 2024-04-25 07:41:33.240106 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate.csh
--rw-r--r--   0        0        0     2513 2024-04-25 07:41:33.241102 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate.fish
--rw-r--r--   0        0        0     8834 2024-04-25 07:41:33.240106 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/Activate.ps1
--rw-r--r--   0        0        0      295 2024-04-25 07:41:33.241102 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/pip
--rw-r--r--   0        0        0      295 2024-04-25 07:41:33.241102 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/pip3
--rw-r--r--   0        0        0      295 2024-04-25 07:41:33.241102 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/pip3.8
--rw-r--r--   0        0        0       58 2024-04-25 07:41:33.241102 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/python
--rw-r--r--   0        0        0        6 2024-04-25 07:41:33.241102 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/python3
--rw-r--r--   0        0        0     3766 2024-04-25 07:41:33.242100 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0        0        0       45 2024-04-25 07:41:33.242100 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/_distutils_hack/override.py
--rw-r--r--   0        0        0      153 2024-04-25 07:41:33.242100 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/distutils-precedence.pth
--rw-r--r--   0        0        0      370 2024-04-25 07:41:33.245090 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/__init__.py
--rw-r--r--   0        0        0     1229 2024-04-25 07:41:33.245090 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1494 2024-04-25 07:41:33.245090 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      592 2024-04-25 07:41:33.245090 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10554 2024-04-25 07:41:33.246087 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    11027 2024-04-25 07:41:33.246087 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0      136 2024-04-25 07:41:33.246087 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6847 2024-04-25 07:41:33.246087 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     8059 2024-04-25 07:41:33.246087 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    30552 2024-04-25 07:41:33.247083 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      801 2024-04-25 07:41:33.247083 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2542 2024-04-25 07:41:33.247083 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4472 2024-04-25 07:41:33.248080 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    11111 2024-04-25 07:41:33.248080 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     2036 2024-04-25 07:41:33.248080 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18674 2024-04-25 07:41:33.248080 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5277 2024-04-25 07:41:33.248080 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      122 2024-04-25 07:41:33.248080 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     4014 2024-04-25 07:41:33.249076 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7803 2024-04-25 07:41:33.249076 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1736 2024-04-25 07:41:33.249076 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4255 2024-04-25 07:41:33.249076 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0    10097 2024-04-25 07:41:33.249076 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6813 2024-04-25 07:41:33.250073 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5436 2024-04-25 07:41:33.250073 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     3071 2024-04-25 07:41:33.250073 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1762 2024-04-25 07:41:33.250073 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1173 2024-04-25 07:41:33.250073 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4932 2024-04-25 07:41:33.250073 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3280 2024-04-25 07:41:33.251069 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    33296 2024-04-25 07:41:33.251069 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12708 2024-04-25 07:41:33.251069 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5871 2024-04-25 07:41:33.251069 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6608 2024-04-25 07:41:33.251069 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3999 2024-04-25 07:41:33.252067 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     7597 2024-04-25 07:41:33.252067 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0    13903 2024-04-25 07:41:33.252067 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0      879 2024-04-25 07:41:33.252067 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1260 2024-04-25 07:41:33.252067 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      752 2024-04-25 07:41:33.253063 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6644 2024-04-25 07:41:33.253063 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1198 2024-04-25 07:41:33.253063 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0    24991 2024-04-25 07:41:33.253063 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0       32 2024-04-25 07:41:33.254059 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    17009 2024-04-25 07:41:33.254059 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    38902 2024-04-25 07:41:33.254059 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6779 2024-04-25 07:41:33.254059 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    15832 2024-04-25 07:41:33.255057 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6273 2024-04-25 07:41:33.255057 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7893 2024-04-25 07:41:33.255057 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2637 2024-04-25 07:41:33.255057 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0      352 2024-04-25 07:41:33.255057 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     4407 2024-04-25 07:41:33.256053 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2679 2024-04-25 07:41:33.256053 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25979 2024-04-25 07:41:33.256053 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0      111 2024-04-25 07:41:33.256053 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1937 2024-04-25 07:41:33.256053 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8405 2024-04-25 07:41:33.257049 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7645 2024-04-25 07:41:33.257049 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0    10043 2024-04-25 07:41:33.257049 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0       65 2024-04-25 07:41:33.258047 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0     1024 2024-04-25 07:41:33.258047 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     6854 2024-04-25 07:41:33.258047 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2600 2024-04-25 07:41:33.258047 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1058 2024-04-25 07:41:33.258047 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2670 2024-04-25 07:41:33.259043 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    19126 2024-04-25 07:41:33.259043 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      769 2024-04-25 07:41:33.259043 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4775 2024-04-25 07:41:33.259043 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1958 2024-04-25 07:41:33.259043 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3968 2024-04-25 07:41:33.260040 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3692 2024-04-25 07:41:33.260040 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       52 2024-04-25 07:41:33.260040 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    16953 2024-04-25 07:41:33.260040 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2214 2024-04-25 07:41:33.260040 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6282 2024-04-25 07:41:33.260040 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7848 2024-04-25 07:41:33.261037 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18959 2024-04-25 07:41:33.261037 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4169 2024-04-25 07:41:33.261037 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1851 2024-04-25 07:41:33.262033 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.262033 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.262033 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4293 2024-04-25 07:41:33.262033 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1529 2024-04-25 07:41:33.262033 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1569 2024-04-25 07:41:33.262033 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2304 2024-04-25 07:41:33.263029 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1112 2024-04-25 07:41:33.263029 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1463 2024-04-25 07:41:33.263029 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3180 2024-04-25 07:41:33.263029 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0     5271 2024-04-25 07:41:33.263029 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0    10038 2024-04-25 07:41:33.263029 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0       53 2024-04-25 07:41:33.264026 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1401 2024-04-25 07:41:33.264026 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0     4223 2024-04-25 07:41:33.264026 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0        0        0    28145 2024-04-25 07:41:33.264026 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0    25758 2024-04-25 07:41:33.264026 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0     7161 2024-04-25 07:41:33.265023 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     2901 2024-04-25 07:41:33.265023 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    17110 2024-04-25 07:41:33.265023 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    18186 2024-04-25 07:41:33.265023 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    36730 2024-04-25 07:41:33.266020 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     2940 2024-04-25 07:41:33.266020 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24686 2024-04-25 07:41:33.267017 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.267017 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      603 2024-04-25 07:41:33.267017 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.267017 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24729 2024-04-25 07:41:33.267017 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.268012 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5361 2024-04-25 07:41:33.268012 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    19519 2024-04-25 07:41:33.268012 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    28607 2024-04-25 07:41:33.268012 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5860 2024-04-25 07:41:33.269009 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0    10162 2024-04-25 07:41:33.269009 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     2594 2024-04-25 07:41:33.269009 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5619 2024-04-25 07:41:33.269009 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11829 2024-04-25 07:41:33.269009 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0     8409 2024-04-25 07:41:33.269009 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.270007 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1053 2024-04-25 07:41:33.270007 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1717 2024-04-25 07:41:33.270007 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1947 2024-04-25 07:41:33.270007 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5542 2024-04-25 07:41:33.270007 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      253 2024-04-25 07:41:33.271002 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     5952 2024-04-25 07:41:33.271002 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3293 2024-04-25 07:41:33.271002 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     1158 2024-04-25 07:41:33.271002 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0        0        0     2190 2024-04-25 07:41:33.271002 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1205 2024-04-25 07:41:33.271002 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3148 2024-04-25 07:41:33.271002 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5275 2024-04-25 07:41:33.272000 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      743 2024-04-25 07:41:33.272000 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3198 2024-04-25 07:41:33.272000 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     4975 2024-04-25 07:41:33.272000 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      830 2024-04-25 07:41:33.272000 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    11980 2024-04-25 07:41:33.272000 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    22992 2024-04-25 07:41:33.272997 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1232 2024-04-25 07:41:33.272997 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2165 2024-04-25 07:41:33.272997 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     5857 2024-04-25 07:41:33.272997 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9460 2024-04-25 07:41:33.272997 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     7948 2024-04-25 07:41:33.272997 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     9078 2024-04-25 07:41:33.273992 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1829 2024-04-25 07:41:33.273992 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3560 2024-04-25 07:41:33.273992 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4685 2024-04-25 07:41:33.273992 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      611 2024-04-25 07:41:33.273992 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3631 2024-04-25 07:41:33.274990 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18646 2024-04-25 07:41:33.274990 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5401 2024-04-25 07:41:33.274990 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    12053 2024-04-25 07:41:33.275986 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    23516 2024-04-25 07:41:33.276104 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0    13518 2024-04-25 07:41:33.276607 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0     5072 2024-04-25 07:41:33.276607 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0      485 2024-04-25 07:41:33.276607 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1440 2024-04-25 07:41:33.276607 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5171 2024-04-25 07:41:33.276607 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1598 2024-04-25 07:41:33.277607 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      251 2024-04-25 07:41:33.277607 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5457 2024-04-25 07:41:33.277607 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1070 2024-04-25 07:41:33.277607 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0      810 2024-04-25 07:41:33.277607 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    16855 2024-04-25 07:41:33.278602 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     4057 2024-04-25 07:41:33.278602 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4384 2024-04-25 07:41:33.278602 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7283 2024-04-25 07:41:33.278602 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      805 2024-04-25 07:41:33.278602 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0       98 2024-04-25 07:41:33.279599 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      267 2024-04-25 07:41:33.279599 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   279760 2024-04-25 07:41:33.281594 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4436 2024-04-25 07:41:33.281594 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     4912 2024-04-25 07:41:33.282590 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31660 2024-04-25 07:41:33.282590 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1810 2024-04-25 07:41:33.282590 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0    10293 2024-04-25 07:41:33.282590 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     4021 2024-04-25 07:41:33.282590 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     5565 2024-04-25 07:41:33.283586 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.283586 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     3354 2024-04-25 07:41:33.283586 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0     3822 2024-04-25 07:41:33.283586 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0      561 2024-04-25 07:41:33.283586 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
--rw-r--r--   0        0        0     1909 2024-04-25 07:41:33.284583 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1768 2024-04-25 07:41:33.284583 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     4108 2024-04-25 07:41:33.284583 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12437 2024-04-25 07:41:33.284583 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     4036 2024-04-25 07:41:33.284583 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13762 2024-04-25 07:41:33.284583 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1800 2024-04-25 07:41:33.284583 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    37301 2024-04-25 07:41:33.285579 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1800 2024-04-25 07:41:33.285579 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    21019 2024-04-25 07:41:33.285579 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1806 2024-04-25 07:41:33.285579 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    14853 2024-04-25 07:41:33.286576 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    26121 2024-04-25 07:41:33.286576 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    44880 2024-04-25 07:41:33.286576 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1799 2024-04-25 07:41:33.286576 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    27293 2024-04-25 07:41:33.287572 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   109211 2024-04-25 07:41:33.288570 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0   102881 2024-04-25 07:41:33.288570 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0   102576 2024-04-25 07:41:33.289566 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   106012 2024-04-25 07:41:33.289566 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   133760 2024-04-25 07:41:33.290562 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   107154 2024-04-25 07:41:33.290562 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    99752 2024-04-25 07:41:33.291559 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5527 2024-04-25 07:41:33.291559 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     6239 2024-04-25 07:41:33.291559 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/macromanprober.py
--rw-r--r--   0        0        0     3810 2024-04-25 07:41:33.291559 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2188 2024-04-25 07:41:33.291559 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    31052 2024-04-25 07:41:33.292556 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.292556 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13912 2024-04-25 07:41:33.292556 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      418 2024-04-25 07:41:33.292556 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/resultdict.py
--rw-r--r--   0        0        0     6562 2024-04-25 07:41:33.293553 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4225 2024-04-25 07:41:33.293553 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     4112 2024-04-25 07:41:33.293553 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    15210 2024-04-25 07:41:33.293553 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8730 2024-04-25 07:41:33.293553 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2894 2024-04-25 07:41:33.293553 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      253 2024-04-25 07:41:33.294552 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0      271 2024-04-25 07:41:33.294552 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2407 2024-04-25 07:41:33.294552 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    11438 2024-04-25 07:41:33.294552 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3449 2024-04-25 07:41:33.295547 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0       76 2024-04-25 07:41:33.295547 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/__init__.py
--rw-r--r--   0        0        0     2907 2024-04-25 07:41:33.295547 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansi_test.py
--rw-r--r--   0        0        0    10788 2024-04-25 07:41:33.295547 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
--rw-r--r--   0        0        0     6845 2024-04-25 07:41:33.295547 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/initialise_test.py
--rw-r--r--   0        0        0     1923 2024-04-25 07:41:33.296543 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/isatty_test.py
--rw-r--r--   0        0        0     1138 2024-04-25 07:41:33.296543 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/utils.py
--rw-r--r--   0        0        0     3810 2024-04-25 07:41:33.296543 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/winterm_test.py
--rw-r--r--   0        0        0     6395 2024-04-25 07:41:33.296543 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     7366 2024-04-25 07:41:33.296543 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0      656 2024-04-25 07:41:33.297540 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    42254 2024-04-25 07:41:33.297540 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    52975 2024-04-25 07:41:33.297540 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    21460 2024-04-25 07:41:33.298537 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    53335 2024-04-25 07:41:33.298537 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    15095 2024-04-25 07:41:33.298537 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5361 2024-04-25 07:41:33.299533 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    40949 2024-04-25 07:41:33.299533 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    11149 2024-04-25 07:41:33.299533 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18723 2024-04-25 07:41:33.299533 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    97792 2024-04-25 07:41:33.300530 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   182784 2024-04-25 07:41:33.302523 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   108032 2024-04-25 07:41:33.303520 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    68382 2024-04-25 07:41:33.304517 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23976 2024-04-25 07:41:33.304517 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    91648 2024-04-25 07:41:33.304517 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   168448 2024-04-25 07:41:33.305513 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0   101888 2024-04-25 07:41:33.306512 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    45224 2024-04-25 07:41:33.306512 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0     1035 2024-04-25 07:41:33.306512 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       68 2024-04-25 07:41:33.306512 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    50727 2024-04-25 07:41:33.307507 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      893 2024-04-25 07:41:33.307507 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3482 2024-04-25 07:41:33.307507 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      338 2024-04-25 07:41:33.308503 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    14509 2024-04-25 07:41:33.308503 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    46510 2024-04-25 07:41:33.309500 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1955 2024-04-25 07:41:33.309500 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2024-04-25 07:41:33.309500 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   248014 2024-04-25 07:41:33.311498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1189 2024-04-25 07:41:33.311498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1129 2024-04-25 07:41:33.311498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6273 2024-04-25 07:41:33.311498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    35571 2024-04-25 07:41:33.312493 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      687 2024-04-25 07:41:33.312493 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      522 2024-04-25 07:41:33.312493 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11789 2024-04-25 07:41:33.312493 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4514 2024-04-25 07:41:33.313490 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1492 2024-04-25 07:41:33.313490 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8789 2024-04-25 07:41:33.313490 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4822 2024-04-25 07:41:33.313490 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30881 2024-04-25 07:41:33.314487 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    16184 2024-04-25 07:41:33.314487 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4336 2024-04-25 07:41:33.314487 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    15159 2024-04-25 07:41:33.315480 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0   111851 2024-04-25 07:41:33.316477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0      570 2024-04-25 07:41:33.316477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0        0        0    13532 2024-04-25 07:41:33.316477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1222 2024-04-25 07:41:33.316477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4236 2024-04-25 07:41:33.317477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     5066 2024-04-25 07:41:33.317477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2791 2024-04-25 07:41:33.317477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     7124 2024-04-25 07:41:33.317477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0      164 2024-04-25 07:41:33.317477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     6848 2024-04-25 07:41:33.318474 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     3093 2024-04-25 07:41:33.318474 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      370 2024-04-25 07:41:33.318474 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    24844 2024-04-25 07:41:33.318474 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1778 2024-04-25 07:41:33.318474 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     2037 2024-04-25 07:41:33.319470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0    32699 2024-04-25 07:41:33.319470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     3011 2024-04-25 07:41:33.319470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0     4936 2024-04-25 07:41:33.320467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     5081 2024-04-25 07:41:33.320467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3424 2024-04-25 07:41:33.320467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5276 2024-04-25 07:41:33.320467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    37498 2024-04-25 07:41:33.320467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    22637 2024-04-25 07:41:33.321463 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     5838 2024-04-25 07:41:33.321463 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19746 2024-04-25 07:41:33.321463 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5167 2024-04-25 07:41:33.322460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2295 2024-04-25 07:41:33.322460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5100 2024-04-25 07:41:33.322460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7613 2024-04-25 07:41:33.322460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4538 2024-04-25 07:41:33.322460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    12123 2024-04-25 07:41:33.322460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    32910 2024-04-25 07:41:33.323457 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0    11541 2024-04-25 07:41:33.323457 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0   100947 2024-04-25 07:41:33.324454 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    78835 2024-04-25 07:41:33.324454 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     1049 2024-04-25 07:41:33.325447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2679 2024-04-25 07:41:33.325447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3354 2024-04-25 07:41:33.325447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3148 2024-04-25 07:41:33.325447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     4943 2024-04-25 07:41:33.325447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6388 2024-04-25 07:41:33.325447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     3455 2024-04-25 07:41:33.326447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     5060 2024-04-25 07:41:33.326447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63500 2024-04-25 07:41:33.326447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0     9373 2024-04-25 07:41:33.326447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0     9500 2024-04-25 07:41:33.327443 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6633 2024-04-25 07:41:33.327443 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    13360 2024-04-25 07:41:33.327443 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   219156 2024-04-25 07:41:33.329437 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0    24325 2024-04-25 07:41:33.329437 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0     9290 2024-04-25 07:41:33.329437 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    40311 2024-04-25 07:41:33.330433 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    26152 2024-04-25 07:41:33.330433 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13733 2024-04-25 07:41:33.330433 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    11139 2024-04-25 07:41:33.330433 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     7040 2024-04-25 07:41:33.331430 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0      514 2024-04-25 07:41:33.331430 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/__init__.py
--rw-r--r--   0        0        0      146 2024-04-25 07:41:33.331430 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_compat.py
--rw-r--r--   0        0        0    12420 2024-04-25 07:41:33.331430 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_impl.py
--rw-r--r--   0        0        0      578 2024-04-25 07:41:33.331430 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
--rw-r--r--   0        0        0    11133 2024-04-25 07:41:33.332425 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
--rw-r--r--   0        0        0     5366 2024-04-25 07:41:33.332425 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      449 2024-04-25 07:41:33.332425 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1445 2024-04-25 07:41:33.332425 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    22025 2024-04-25 07:41:33.332425 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6534 2024-04-25 07:41:33.333423 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10516 2024-04-25 07:41:33.333423 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      603 2024-04-25 07:41:33.333423 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1353 2024-04-25 07:41:33.333423 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    19121 2024-04-25 07:41:33.334420 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3964 2024-04-25 07:41:33.334420 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     4010 2024-04-25 07:41:33.334420 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      766 2024-04-25 07:41:33.334420 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    36314 2024-04-25 07:41:33.334420 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      744 2024-04-25 07:41:33.334420 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30999 2024-04-25 07:41:33.335416 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4363 2024-04-25 07:41:33.335416 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     3011 2024-04-25 07:41:33.335416 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    34328 2024-04-25 07:41:33.335416 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      563 2024-04-25 07:41:33.336413 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.336413 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      162 2024-04-25 07:41:33.336413 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     6005 2024-04-25 07:41:33.336413 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1626 2024-04-25 07:41:33.336413 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    18044 2024-04-25 07:41:33.337410 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4959 2024-04-25 07:41:33.337410 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0     6267 2024-04-25 07:41:33.337410 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8781 2024-04-25 07:41:33.337410 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10547 2024-04-25 07:41:33.337410 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   143845 2024-04-25 07:41:33.338978 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1096 2024-04-25 07:41:33.338978 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2192 2024-04-25 07:41:33.339498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      275 2024-04-25 07:41:33.339498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0     9965 2024-04-25 07:41:33.339498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3319 2024-04-25 07:41:33.339498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1279 2024-04-25 07:41:33.339498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     1724 2024-04-25 07:41:33.339498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_null_file.py
--rw-r--r--   0        0        0     7372 2024-04-25 07:41:33.340504 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      440 2024-04-25 07:41:33.340504 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5630 2024-04-25 07:41:33.340504 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    20401 2024-04-25 07:41:33.340504 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      367 2024-04-25 07:41:33.340504 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      436 2024-04-25 07:41:33.340504 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    23496 2024-04-25 07:41:33.341498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1996 2024-04-25 07:41:33.341498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2839 2024-04-25 07:41:33.341498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1896 2024-04-25 07:41:33.341498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      923 2024-04-25 07:41:33.341498 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10678 2024-04-25 07:41:33.342500 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     7056 2024-04-25 07:41:33.342500 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3356 2024-04-25 07:41:33.342500 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0    10357 2024-04-25 07:41:33.342500 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4740 2024-04-25 07:41:33.342500 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    18630 2024-04-25 07:41:33.343494 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1092 2024-04-25 07:41:33.343494 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7318 2024-04-25 07:41:33.343494 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0   100737 2024-04-25 07:41:33.344490 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1325 2024-04-25 07:41:33.344490 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5664 2024-04-25 07:41:33.344490 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6855 2024-04-25 07:41:33.344490 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     8146 2024-04-25 07:41:33.344490 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0     1009 2024-04-25 07:41:33.344490 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2597 2024-04-25 07:41:33.345486 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      676 2024-04-25 07:41:33.345486 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1670 2024-04-25 07:41:33.345486 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2597 2024-04-25 07:41:33.345486 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9817 2024-04-25 07:41:33.345486 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5191 2024-04-25 07:41:33.345486 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3353 2024-04-25 07:41:33.346483 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14446 2024-04-25 07:41:33.346483 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14543 2024-04-25 07:41:33.346483 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3780 2024-04-25 07:41:33.346483 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    12192 2024-04-25 07:41:33.346483 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8442 2024-04-25 07:41:33.346483 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5456 2024-04-25 07:41:33.347480 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     5110 2024-04-25 07:41:33.347480 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      862 2024-04-25 07:41:33.347480 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3496 2024-04-25 07:41:33.347480 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0    10882 2024-04-25 07:41:33.347480 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    38445 2024-04-25 07:41:33.348477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    61545 2024-04-25 07:41:33.348477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8387 2024-04-25 07:41:33.348477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11677 2024-04-25 07:41:33.348477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1433 2024-04-25 07:41:33.349473 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      176 2024-04-25 07:41:33.349473 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4597 2024-04-25 07:41:33.349473 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4907 2024-04-25 07:41:33.349473 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2929 2024-04-25 07:41:33.349473 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1645 2024-04-25 07:41:33.349473 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24961 2024-04-25 07:41:33.350470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4510 2024-04-25 07:41:33.350470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4555 2024-04-25 07:41:33.350470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    27261 2024-04-25 07:41:33.350470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1300 2024-04-25 07:41:33.350470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    35936 2024-04-25 07:41:33.351467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    40680 2024-04-25 07:41:33.351467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3523 2024-04-25 07:41:33.351467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    46995 2024-04-25 07:41:33.351467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3739 2024-04-25 07:41:33.352463 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      107 2024-04-25 07:41:33.352463 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    26758 2024-04-25 07:41:33.352463 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9416 2024-04-25 07:41:33.352463 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    35710 2024-04-25 07:41:33.353460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0    19161 2024-04-25 07:41:33.353460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3441 2024-04-25 07:41:33.353460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     2012 2024-04-25 07:41:33.353460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1542 2024-04-25 07:41:33.354460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1425 2024-04-25 07:41:33.354460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     1966 2024-04-25 07:41:33.354460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1426 2024-04-25 07:41:33.354460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     7854 2024-04-25 07:41:33.354460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     2886 2024-04-25 07:41:33.354460 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2239 2024-04-25 07:41:33.355454 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8283 2024-04-25 07:41:33.355454 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      407 2024-04-25 07:41:33.355454 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    23324 2024-04-25 07:41:33.355454 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     3050 2024-04-25 07:41:33.355454 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      264 2024-04-25 07:41:33.356450 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0    83672 2024-04-25 07:41:33.356450 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     3435 2024-04-25 07:41:33.356450 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    11171 2024-04-25 07:41:33.357447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       66 2024-04-25 07:41:33.357447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20636 2024-04-25 07:41:33.357447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    40213 2024-04-25 07:41:33.357447 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.358442 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      993 2024-04-25 07:41:33.358442 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.358442 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    18149 2024-04-25 07:41:33.358442 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    14317 2024-04-25 07:41:33.358442 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0    11351 2024-04-25 07:41:33.359439 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4658 2024-04-25 07:41:33.359439 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17597 2024-04-25 07:41:33.359439 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    35365 2024-04-25 07:41:33.360438 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7315 2024-04-25 07:41:33.360438 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0     8540 2024-04-25 07:41:33.360438 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8836 2024-04-25 07:41:33.360438 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2538 2024-04-25 07:41:33.360438 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.361433 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.361433 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1468 2024-04-25 07:41:33.361433 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0    35742 2024-04-25 07:41:33.361433 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0    20326 2024-04-25 07:41:33.362430 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     6157 2024-04-25 07:41:33.362430 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    31511 2024-04-25 07:41:33.362430 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0     1204 2024-04-25 07:41:33.362430 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     5049 2024-04-25 07:41:33.362430 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1662 2024-04-25 07:41:33.363427 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      520 2024-04-25 07:41:33.363427 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     4134 2024-04-25 07:41:33.363427 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3617 2024-04-25 07:41:33.363427 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22621 2024-04-25 07:41:33.363427 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17672 2024-04-25 07:41:33.364423 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5917 2024-04-25 07:41:33.364423 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     7116 2024-04-25 07:41:33.364958 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10271 2024-04-25 07:41:33.364958 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14726 2024-04-25 07:41:33.364958 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5555 2024-04-25 07:41:33.365472 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0      499 2024-04-25 07:41:33.365472 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0    10930 2024-04-25 07:41:33.365472 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     7084 2024-04-25 07:41:33.365472 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1384 2024-04-25 07:41:33.365472 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6910 2024-04-25 07:41:33.366477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4624 2024-04-25 07:41:33.366477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0      290 2024-04-25 07:41:33.366477 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/py.typed
--rw-r--r--   0        0        0      128 2024-04-25 07:41:33.244093 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0        5 2024-04-25 07:41:33.243095 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1113 2024-04-25 07:41:33.243095 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     4160 2024-04-25 07:41:33.243095 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/METADATA
--rw-r--r--   0        0        0    76671 2024-04-25 07:41:33.243095 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.244093 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/REQUESTED
--rw-r--r--   0        0        0        5 2024-04-25 07:41:33.244093 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/top_level.txt
--rw-r--r--   0        0        0       97 2024-04-25 07:41:33.244093 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0   111748 2024-04-25 07:41:33.367474 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.367474 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    25276 2024-04-25 07:41:33.367474 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0        0        0      763 2024-04-25 07:41:33.367474 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      588 2024-04-25 07:41:33.368470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     1166 2024-04-25 07:41:33.368470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     2108 2024-04-25 07:41:33.368470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     1860 2024-04-25 07:41:33.368470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_typing.py
--rw-r--r--   0        0        0     9870 2024-04-25 07:41:33.368470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     5100 2024-04-25 07:41:33.368470 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    32778 2024-04-25 07:41:33.369467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    24774 2024-04-25 07:41:33.369467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     1876 2024-04-25 07:41:33.369467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16001 2024-04-25 07:41:33.369467 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0   237588 2024-04-25 07:41:33.371665 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/pyparsing.py
--rw-r--r--   0        0        0     2448 2024-04-25 07:41:33.371665 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0      112 2024-04-25 07:41:33.371665 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
--rw-r--r--   0        0        0     7938 2024-04-25 07:41:33.373659 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0      225 2024-04-25 07:41:33.373659 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0        0        0      266 2024-04-25 07:41:33.374655 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0        0        0    21250 2024-04-25 07:41:33.374655 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0        0        0     8881 2024-04-25 07:41:33.374655 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0        0        0    14925 2024-04-25 07:41:33.374655 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0        0        0    48047 2024-04-25 07:41:33.375772 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0        0        0    18385 2024-04-25 07:41:33.375772 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0        0        0      660 2024-04-25 07:41:33.375772 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0        0        0     5406 2024-04-25 07:41:33.376779 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0        0        0     4792 2024-04-25 07:41:33.376779 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0        0        0    40520 2024-04-25 07:41:33.376779 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_msi.py
--rw-r--r--   0        0        0    22373 2024-04-25 07:41:33.377770 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0        0        0    16099 2024-04-25 07:41:33.377770 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_wininst.py
--rw-r--r--   0        0        0     5740 2024-04-25 07:41:33.377770 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0        0        0     7908 2024-04-25 07:41:33.377770 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0        0        0    32208 2024-04-25 07:41:33.378771 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0        0        0    17833 2024-04-25 07:41:33.378771 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0        0        0     6507 2024-04-25 07:41:33.378771 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0        0        0     6012 2024-04-25 07:41:33.378771 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0        0        0     2677 2024-04-25 07:41:33.379763 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0        0        0    13512 2024-04-25 07:41:33.379763 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0        0        0    28171 2024-04-25 07:41:33.379763 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0        0        0     2861 2024-04-25 07:41:33.379763 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0        0        0     2715 2024-04-25 07:41:33.380764 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0        0        0     1232 2024-04-25 07:41:33.380764 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0        0        0     8666 2024-04-25 07:41:33.380764 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0        0        0     1995 2024-04-25 07:41:33.380764 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0        0        0      703 2024-04-25 07:41:33.380764 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0        0        0    12088 2024-04-25 07:41:33.381760 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0        0        0    19766 2024-04-25 07:41:33.381760 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0        0        0     7654 2024-04-25 07:41:33.381760 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0        0        0     5045 2024-04-25 07:41:33.381760 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0        0        0     9110 2024-04-25 07:41:33.381760 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0        0        0    16550 2024-04-25 07:41:33.382757 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0        0        0      144 2024-04-25 07:41:33.382757 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0        0        0     3519 2024-04-25 07:41:33.382757 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0        0        0     8264 2024-04-25 07:41:33.382757 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0        0        0    51532 2024-04-25 07:41:33.382757 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0        0        0     3716 2024-04-25 07:41:33.383754 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0        0        0    10497 2024-04-25 07:41:33.383754 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0        0        0    18261 2024-04-25 07:41:33.383754 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0        0        0     8335 2024-04-25 07:41:33.383754 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0        0        0    13615 2024-04-25 07:41:33.383754 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0        0        0     2052 2024-04-25 07:41:33.384747 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0        0        0    30633 2024-04-25 07:41:33.384747 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0        0        0    23971 2024-04-25 07:41:33.384747 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0        0        0      474 2024-04-25 07:41:33.385744 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/py35compat.py
--rw-r--r--   0        0        0      221 2024-04-25 07:41:33.385744 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0        0        0     4494 2024-04-25 07:41:33.385744 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0        0        0    22267 2024-04-25 07:41:33.385744 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0        0        0    12386 2024-04-25 07:41:33.385744 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0        0        0    14832 2024-04-25 07:41:33.386740 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0        0        0    21614 2024-04-25 07:41:33.386740 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0        0        0    12772 2024-04-25 07:41:33.386740 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0        0        0     5276 2024-04-25 07:41:33.386740 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0        0        0     2514 2024-04-25 07:41:33.387740 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_imp.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.387740 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15618 2024-04-25 07:41:33.387740 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0      763 2024-04-25 07:41:33.387740 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      588 2024-04-25 07:41:33.387740 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     1168 2024-04-25 07:41:33.388733 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_compat.py
--rw-r--r--   0        0        0     2108 2024-04-25 07:41:33.388733 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     1860 2024-04-25 07:41:33.388733 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_typing.py
--rw-r--r--   0        0        0     9863 2024-04-25 07:41:33.388733 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     5088 2024-04-25 07:41:33.388733 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    32778 2024-04-25 07:41:33.389734 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    24778 2024-04-25 07:41:33.389734 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     1876 2024-04-25 07:41:33.389734 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16003 2024-04-25 07:41:33.389734 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0   237588 2024-04-25 07:41:33.390731 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/pyparsing.py
--rw-r--r--   0        0        0     7270 2024-04-25 07:41:33.390731 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0    10356 2024-04-25 07:41:33.391724 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/build_meta.py
--rwxr-xr-x   0        0        0    65536 2024-04-25 07:41:33.392727 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli-32.exe
--rwxr-xr-x   0        0        0    74752 2024-04-25 07:41:33.393312 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli-64.exe
--rwxr-xr-x   0        0        0    65536 2024-04-25 07:41:33.393819 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0      648 2024-04-25 07:41:33.393819 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     2461 2024-04-25 07:41:33.393819 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    17079 2024-04-25 07:41:33.394824 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0      883 2024-04-25 07:41:33.394824 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0     4489 2024-04-25 07:41:33.394824 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    13579 2024-04-25 07:41:33.394824 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0     9586 2024-04-25 07:41:33.394824 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     8285 2024-04-25 07:41:33.395820 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0     1031 2024-04-25 07:41:33.395820 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    87874 2024-04-25 07:41:33.395820 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    25626 2024-04-25 07:41:33.396813 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     4873 2024-04-25 07:41:33.396813 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2252 2024-04-25 07:41:33.396813 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3995 2024-04-25 07:41:33.396813 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2688 2024-04-25 07:41:33.396813 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      643 2024-04-25 07:41:33.397814 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0     5097 2024-04-25 07:41:33.397814 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0        0        0      486 2024-04-25 07:41:33.397814 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2159 2024-04-25 07:41:33.397814 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      678 2024-04-25 07:41:33.397814 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     8114 2024-04-25 07:41:33.397814 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     5029 2024-04-25 07:41:33.397814 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0     9812 2024-04-25 07:41:33.398810 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/test.py
--rw-r--r--   0        0        0      479 2024-04-25 07:41:33.398810 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7500 2024-04-25 07:41:33.398810 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0    22705 2024-04-25 07:41:33.398810 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/config.py
--rw-r--r--   0        0        0      960 2024-04-25 07:41:33.398810 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5680 2024-04-25 07:41:33.399807 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    41467 2024-04-25 07:41:33.399807 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0      540 2024-04-25 07:41:33.399807 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/errors.py
--rw-r--r--   0        0        0     1739 2024-04-25 07:41:33.399807 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     2495 2024-04-25 07:41:33.400805 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0     5034 2024-04-25 07:41:33.400805 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/glob.py
--rwxr-xr-x   0        0        0    65536 2024-04-25 07:41:33.400805 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui-32.exe
--rwxr-xr-x   0        0        0    75264 2024-04-25 07:41:33.401800 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui-64.exe
--rwxr-xr-x   0        0        0    65536 2024-04-25 07:41:33.401800 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0     3734 2024-04-25 07:41:33.401800 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/installer.py
--rw-r--r--   0        0        0      848 2024-04-25 07:41:33.401800 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     2414 2024-04-25 07:41:33.401800 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/lib2to3_ex.py
--rw-r--r--   0        0        0     5374 2024-04-25 07:41:33.402797 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    53059 2024-04-25 07:41:33.402797 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     3145 2024-04-25 07:41:33.402797 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    42201 2024-04-25 07:41:33.403794 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0      260 2024-04-25 07:41:33.403794 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/py34compat.py
--rw-r--r--   0        0        0    14994 2024-04-25 07:41:33.403794 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      224 2024-04-25 07:41:33.403794 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      141 2024-04-25 07:41:33.403794 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0     8816 2024-04-25 07:41:33.404791 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/ssl_support.py
--rw-r--r--   0        0        0      983 2024-04-25 07:41:33.404791 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      150 2024-04-25 07:41:33.404791 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     8521 2024-04-25 07:41:33.404791 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      743 2024-04-25 07:41:33.404791 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0      241 2024-04-25 07:41:33.373659 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/dependency_links.txt
--rw-r--r--   0        0        0     2929 2024-04-25 07:41:33.373659 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/entry_points.txt
--rw-r--r--   0        0        0        5 2024-04-25 07:41:33.372662 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/INSTALLER
--rw-r--r--   0        0        0     1069 2024-04-25 07:41:33.372662 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/LICENSE
--rw-r--r--   0        0        0     4873 2024-04-25 07:41:33.372662 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/METADATA
--rw-r--r--   0        0        0    22796 2024-04-25 07:41:33.372662 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/RECORD
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.372662 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/REQUESTED
--rw-r--r--   0        0        0       44 2024-04-25 07:41:33.373659 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/top_level.txt
--rw-r--r--   0        0        0       97 2024-04-25 07:41:33.372662 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/WHEEL
--rw-r--r--   0        0        0        3 2024-04-25 07:41:33.404791 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib64
--rw-r--r--   0        0        0      116 2024-04-25 07:41:33.404791 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/pyvenv.cfg
--rw-r--r--   0        0        0      251 2024-04-25 07:41:33.405787 greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/virtualenv_runner.log
--rw-r--r--   0        0        0       81 2024-04-25 07:41:33.406784 greatlibrarian-0.0.8/greatlibrarian/Agents/PromptMarket/__init__.py
--rw-r--r--   0        0        0     3606 2024-04-25 07:41:33.406784 greatlibrarian-0.0.8/greatlibrarian/Agents/PromptMarket/getContextExamples.py
--rw-r--r--   0        0        0     2206 2024-04-25 07:41:33.406784 greatlibrarian-0.0.8/greatlibrarian/Agents/PromptMarket/main.py
--rw-r--r--   0        0        0     1602 2024-04-25 07:41:33.407779 greatlibrarian-0.0.8/greatlibrarian/Agents/PromptMarket/promptGenerator.py
--rw-r--r--   0        0        0      305 2024-04-25 07:41:33.407779 greatlibrarian-0.0.8/greatlibrarian/Agents/PromptMarket/testAPI.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.407779 greatlibrarian-0.0.8/greatlibrarian/Agents/TranslationAPI/__init__.py
--rw-r--r--   0        0        0      315 2024-04-25 07:41:33.407779 greatlibrarian-0.0.8/greatlibrarian/Agents/TranslationAPI/translationGPT.py
--rw-r--r--   0        0        0       60 2024-04-25 07:41:33.408775 greatlibrarian-0.0.8/greatlibrarian/Analyser/__init__.py
--rw-r--r--   0        0        0    22905 2024-04-25 07:41:33.408775 greatlibrarian-0.0.8/greatlibrarian/Analyser/analyse.py
--rw-r--r--   0        0        0     2276 2024-04-25 07:41:33.408775 greatlibrarian-0.0.8/greatlibrarian/Analyser/getInfo.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.411767 greatlibrarian-0.0.8/greatlibrarian/Assets/__init__.py
--rw-r--r--   0        0        0   432227 2024-04-25 07:41:33.411767 greatlibrarian-0.0.8/greatlibrarian/Assets/GreatLibrarian.pdf
--rw-r--r--   0        0        0      773 2024-04-25 07:41:33.411767 greatlibrarian-0.0.8/greatlibrarian/Assets/template.py
--rw-r--r--   0        0        0       67 2024-04-25 07:41:33.411767 greatlibrarian-0.0.8/greatlibrarian/Configs/__init__.py
--rw-r--r--   0        0        0      197 2024-04-25 07:41:33.412763 greatlibrarian-0.0.8/greatlibrarian/Configs/base.py
--rw-r--r--   0        0        0      456 2024-04-25 07:41:33.412763 greatlibrarian-0.0.8/greatlibrarian/Configs/example_config.py
--rw-r--r--   0        0        0      162 2024-04-25 07:41:33.412763 greatlibrarian-0.0.8/greatlibrarian/Core/__init__.py
--rw-r--r--   0        0        0      776 2024-04-25 07:41:33.412763 greatlibrarian-0.0.8/greatlibrarian/Core/agents.py
--rw-r--r--   0        0        0     1226 2024-04-25 07:41:33.412763 greatlibrarian-0.0.8/greatlibrarian/Core/evalMethods.py
--rw-r--r--   0        0        0      512 2024-04-25 07:41:33.413761 greatlibrarian-0.0.8/greatlibrarian/Core/finalscore.py
--rw-r--r--   0        0        0      689 2024-04-25 07:41:33.412763 greatlibrarian-0.0.8/greatlibrarian/Core/LLMs.py
--rw-r--r--   0        0        0      551 2024-04-25 07:41:33.412763 greatlibrarian-0.0.8/greatlibrarian/Core/TestCase.py
--rw-r--r--   0        0        0      126 2024-04-25 07:41:33.413761 greatlibrarian-0.0.8/greatlibrarian/EvalMethods/__init__.py
--rw-r--r--   0        0        0     3024 2024-04-25 07:41:33.413761 greatlibrarian-0.0.8/greatlibrarian/EvalMethods/blacklist.py
--rw-r--r--   0        0        0     3873 2024-04-25 07:41:33.413761 greatlibrarian-0.0.8/greatlibrarian/EvalMethods/keyword.py
--rw-r--r--   0        0        0     6078 2024-04-25 07:41:33.414757 greatlibrarian-0.0.8/greatlibrarian/EvalMethods/llmEval.py
--rw-r--r--   0        0        0     3918 2024-04-25 07:41:33.414757 greatlibrarian-0.0.8/greatlibrarian/EvalMethods/toolUsage.py
--rw-r--r--   0        0        0       38 2024-04-25 07:41:33.414757 greatlibrarian-0.0.8/greatlibrarian/FinalScore/__init__.py
--rw-r--r--   0        0        0     2223 2024-04-25 07:41:33.414757 greatlibrarian-0.0.8/greatlibrarian/FinalScore/finalscore1.py
--rw-r--r--   0        0        0      158 2024-04-25 07:41:33.414757 greatlibrarian-0.0.8/greatlibrarian/Interactor/__init__.py
--rw-r--r--   0        0        0     9019 2024-04-25 07:41:33.415753 greatlibrarian-0.0.8/greatlibrarian/Interactor/autoInteractor.py
--rw-r--r--   0        0        0        0 2024-04-25 07:41:33.415753 greatlibrarian-0.0.8/greatlibrarian/Interactor/fairnessInteractor.py
--rw-r--r--   0        0        0     5283 2024-04-25 07:41:33.415753 greatlibrarian-0.0.8/greatlibrarian/Interactor/hallucinationInteractor.py
--rw-r--r--   0        0        0     9128 2024-04-25 07:41:33.415753 greatlibrarian-0.0.8/greatlibrarian/Interactor/multiturnInteractor.py
--rw-r--r--   0        0        0      123 2024-04-25 07:41:33.416748 greatlibrarian-0.0.8/greatlibrarian/LLMs/__init__.py
--rw-r--r--   0        0        0       66 2024-04-25 07:41:33.415753 greatlibrarian-0.0.8/greatlibrarian/LLMs/APIs/__init__.py
--rw-r--r--   0        0        0     6665 2024-04-25 07:41:33.416748 greatlibrarian-0.0.8/greatlibrarian/LLMs/APIs/openai.py
--rw-r--r--   0        0        0     1556 2024-04-25 07:41:33.417746 greatlibrarian-0.0.8/greatlibrarian/LLMs/dbInteractor.py
--rw-r--r--   0        0        0      398 2024-04-25 07:41:33.416748 greatlibrarian-0.0.8/greatlibrarian/LLMs/LLMs.ini
--rw-r--r--   0        0        0       34 2024-04-25 07:41:33.416748 greatlibrarian-0.0.8/greatlibrarian/LLMs/OpenSource/__init__.py
--rw-r--r--   0        0        0     1782 2024-04-25 07:41:33.416748 greatlibrarian-0.0.8/greatlibrarian/LLMs/OpenSource/chatGLM6B.py
--rw-r--r--   0        0        0     1743 2024-04-25 07:41:33.416748 greatlibrarian-0.0.8/greatlibrarian/LLMs/OpenSource/chatglm6b_2.py
--rw-r--r--   0        0        0       30 2024-04-25 07:41:33.417746 greatlibrarian-0.0.8/greatlibrarian/Recoder/__init__.py
--rw-r--r--   0        0        0      123 2024-04-25 07:41:33.417746 greatlibrarian-0.0.8/greatlibrarian/Recoder/recoder.py
--rw-r--r--   0        0        0     1351 2024-04-25 07:41:33.420736 greatlibrarian-0.0.8/greatlibrarian/register.py
--rw-r--r--   0        0        0     3934 2024-04-25 07:41:33.421733 greatlibrarian-0.0.8/greatlibrarian/run.py
--rw-r--r--   0        0        0       76 2024-04-25 07:41:33.417746 greatlibrarian-0.0.8/greatlibrarian/Runner/__init__.py
--rw-r--r--   0        0        0    10921 2024-04-25 07:41:33.417746 greatlibrarian-0.0.8/greatlibrarian/Runner/autoRunner.py
--rw-r--r--   0        0        0     2831 2024-04-25 07:41:33.418743 greatlibrarian-0.0.8/greatlibrarian/Runner/updateRunner.py
--rw-r--r--   0        0        0       38 2024-04-25 07:41:33.418743 greatlibrarian-0.0.8/greatlibrarian/TestCase/__init__.py
--rw-r--r--   0        0        0     4943 2024-04-25 07:41:33.418743 greatlibrarian-0.0.8/greatlibrarian/TestCase/testProject.py
--rw-r--r--   0        0        0      497 2024-04-25 07:41:33.418743 greatlibrarian-0.0.8/greatlibrarian/Utils/__init__.py
--rw-r--r--   0        0        0     1622 2024-04-25 07:41:33.418743 greatlibrarian-0.0.8/greatlibrarian/Utils/clean_log.py
--rw-r--r--   0        0        0      100 2024-04-25 07:41:33.418743 greatlibrarian-0.0.8/greatlibrarian/Utils/clear_log.py
--rw-r--r--   0        0        0      586 2024-04-25 07:41:33.419740 greatlibrarian-0.0.8/greatlibrarian/Utils/extract_example.py
--rw-r--r--   0        0        0      774 2024-04-25 07:41:33.419740 greatlibrarian-0.0.8/greatlibrarian/Utils/human_evaluation.py
--rw-r--r--   0        0        0      693 2024-04-25 07:41:33.419740 greatlibrarian-0.0.8/greatlibrarian/Utils/io.py
--rw-r--r--   0        0        0    15555 2024-04-25 07:41:33.419740 greatlibrarian-0.0.8/greatlibrarian/Utils/logger.py
--rw-r--r--   0        0        0     2298 2024-04-25 07:41:33.419740 greatlibrarian-0.0.8/greatlibrarian/Utils/logsafe.py
--rw-r--r--   0        0        0      922 2024-04-25 07:41:33.419740 greatlibrarian-0.0.8/greatlibrarian/Utils/mistaken_case.py
--rw-r--r--   0        0        0      622 2024-04-25 07:41:33.420736 greatlibrarian-0.0.8/greatlibrarian/Utils/process.py
--rw-r--r--   0        0        0     1030 2024-04-25 07:41:33.420736 greatlibrarian-0.0.8/greatlibrarian/Utils/project_info.py
--rw-r--r--   0        0        0      643 2024-04-25 07:41:33.420736 greatlibrarian-0.0.8/greatlibrarian/Utils/record_testcase.py
--rw-r--r--   0        0        0      790 2024-04-25 07:41:33.420736 greatlibrarian-0.0.8/greatlibrarian/Utils/register.py
--rw-r--r--   0        0        0     5956 2024-04-25 07:41:33.420736 greatlibrarian-0.0.8/greatlibrarian/Utils/registry.py
--rw-r--r--   0        0        0      250 2024-04-25 07:41:33.420736 greatlibrarian-0.0.8/greatlibrarian/Utils/typetrans.py
--rw-r--r--   0        0        0      508 2024-04-25 07:41:33.420736 greatlibrarian-0.0.8/greatlibrarian/Utils/update_dialog.py
--rw-r--r--   0        0        0      620 2024-04-25 07:43:01.550313 greatlibrarian-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    29598 2024-04-25 07:41:33.236119 greatlibrarian-0.0.8/README.md
--rw-r--r--   0        0        0    29990 1970-01-01 00:00:00.000000 greatlibrarian-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-25 07:41:33.407779 greatlibrarian-0.0.9/greatlibrarian/Agents/__init__.py
+-rw-r--r--   0        0        0       29 2024-04-25 07:41:33.239109 greatlibrarian-0.0.9/greatlibrarian/Agents/BookStore/__init__.py
+-rw-r--r--   0        0        0      713 2024-04-25 07:41:33.239109 greatlibrarian-0.0.9/greatlibrarian/Agents/BookStore/checkDupli.py
+-rw-r--r--   0        0        0    12525 2024-04-25 07:41:33.239109 greatlibrarian-0.0.9/greatlibrarian/Agents/BookStore/getData.py
+-rw-r--r--   0        0        0      342 2024-04-25 07:41:33.240106 greatlibrarian-0.0.9/greatlibrarian/Agents/BookStore/main.py
+-rw-r--r--   0        0        0     8969 2024-04-25 07:41:33.239109 greatlibrarian-0.0.9/greatlibrarian/Agents/BookStore/RawData/Area Studies/African American Studies.csv
+-rw-r--r--   0        0        0      953 2024-04-25 07:41:33.405787 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-25 07:41:33.405787 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/algebra.py
+-rw-r--r--   0        0        0      164 2024-04-25 07:41:33.405787 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/codeComphnExp.py
+-rw-r--r--   0        0        0      118 2024-04-25 07:41:33.405787 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/codeDefeIdentify.py
+-rw-r--r--   0        0        0     2828 2024-04-25 07:41:33.405787 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/codeEnv.py
+-rw-r--r--   0        0        0       77 2024-04-25 07:41:33.405787 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/codeOpt.py
+-rw-r--r--   0        0        0       82 2024-04-25 07:41:33.406784 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/evalPerformance.py
+-rw-r--r--   0        0        0      269 2024-04-25 07:41:33.406784 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/script_test.py
+-rw-r--r--   0        0        0      438 2024-04-25 07:41:33.406784 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/test_code.json
+-rw-r--r--   0        0        0     3240 2024-04-25 07:41:33.406784 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/ttest.py
+-rw-r--r--   0        0        0     2310 2024-04-25 07:41:33.240106 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate
+-rw-r--r--   0        0        0     1323 2024-04-25 07:41:33.240106 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate.csh
+-rw-r--r--   0        0        0     2513 2024-04-25 07:41:33.241102 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate.fish
+-rw-r--r--   0        0        0     8834 2024-04-25 07:41:33.240106 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/Activate.ps1
+-rw-r--r--   0        0        0      295 2024-04-25 07:41:33.241102 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/pip
+-rw-r--r--   0        0        0      295 2024-04-25 07:41:33.241102 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/pip3
+-rw-r--r--   0        0        0      295 2024-04-25 07:41:33.241102 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/pip3.8
+-rw-r--r--   0        0        0       58 2024-04-25 07:41:33.241102 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/python
+-rw-r--r--   0        0        0        6 2024-04-25 07:41:33.241102 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/python3
+-rw-r--r--   0        0        0     3766 2024-04-25 07:41:33.242100 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       45 2024-04-25 07:41:33.242100 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0      153 2024-04-25 07:41:33.242100 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0      370 2024-04-25 07:41:33.245090 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0     1229 2024-04-25 07:41:33.245090 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1494 2024-04-25 07:41:33.245090 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      592 2024-04-25 07:41:33.245090 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10554 2024-04-25 07:41:33.246087 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    11027 2024-04-25 07:41:33.246087 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0      136 2024-04-25 07:41:33.246087 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6847 2024-04-25 07:41:33.246087 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     8059 2024-04-25 07:41:33.246087 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    30552 2024-04-25 07:41:33.247083 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      801 2024-04-25 07:41:33.247083 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2542 2024-04-25 07:41:33.247083 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4472 2024-04-25 07:41:33.248080 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    11111 2024-04-25 07:41:33.248080 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     2036 2024-04-25 07:41:33.248080 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18674 2024-04-25 07:41:33.248080 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5277 2024-04-25 07:41:33.248080 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      122 2024-04-25 07:41:33.248080 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     4014 2024-04-25 07:41:33.249076 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7803 2024-04-25 07:41:33.249076 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1736 2024-04-25 07:41:33.249076 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4255 2024-04-25 07:41:33.249076 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0    10097 2024-04-25 07:41:33.249076 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6813 2024-04-25 07:41:33.250073 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5436 2024-04-25 07:41:33.250073 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     3071 2024-04-25 07:41:33.250073 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1762 2024-04-25 07:41:33.250073 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1173 2024-04-25 07:41:33.250073 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4932 2024-04-25 07:41:33.250073 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3280 2024-04-25 07:41:33.251069 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    33296 2024-04-25 07:41:33.251069 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12708 2024-04-25 07:41:33.251069 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5871 2024-04-25 07:41:33.251069 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6608 2024-04-25 07:41:33.251069 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3999 2024-04-25 07:41:33.252067 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     7597 2024-04-25 07:41:33.252067 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0    13903 2024-04-25 07:41:33.252067 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0      879 2024-04-25 07:41:33.252067 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1260 2024-04-25 07:41:33.252067 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      752 2024-04-25 07:41:33.253063 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6644 2024-04-25 07:41:33.253063 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1198 2024-04-25 07:41:33.253063 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0    24991 2024-04-25 07:41:33.253063 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0       32 2024-04-25 07:41:33.254059 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    17009 2024-04-25 07:41:33.254059 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    38902 2024-04-25 07:41:33.254059 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     6779 2024-04-25 07:41:33.254059 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    15832 2024-04-25 07:41:33.255057 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6273 2024-04-25 07:41:33.255057 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7893 2024-04-25 07:41:33.255057 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2637 2024-04-25 07:41:33.255057 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0      352 2024-04-25 07:41:33.255057 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     4407 2024-04-25 07:41:33.256053 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2679 2024-04-25 07:41:33.256053 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25979 2024-04-25 07:41:33.256053 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0      111 2024-04-25 07:41:33.256053 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1937 2024-04-25 07:41:33.256053 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8405 2024-04-25 07:41:33.257049 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7645 2024-04-25 07:41:33.257049 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0    10043 2024-04-25 07:41:33.257049 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0       65 2024-04-25 07:41:33.258047 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0     1024 2024-04-25 07:41:33.258047 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     6854 2024-04-25 07:41:33.258047 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2600 2024-04-25 07:41:33.258047 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1058 2024-04-25 07:41:33.258047 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2670 2024-04-25 07:41:33.259043 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    19126 2024-04-25 07:41:33.259043 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      769 2024-04-25 07:41:33.259043 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4775 2024-04-25 07:41:33.259043 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1958 2024-04-25 07:41:33.259043 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     3968 2024-04-25 07:41:33.260040 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3692 2024-04-25 07:41:33.260040 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       52 2024-04-25 07:41:33.260040 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    16953 2024-04-25 07:41:33.260040 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2214 2024-04-25 07:41:33.260040 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6282 2024-04-25 07:41:33.260040 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7848 2024-04-25 07:41:33.261037 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18959 2024-04-25 07:41:33.261037 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4169 2024-04-25 07:41:33.261037 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1851 2024-04-25 07:41:33.262033 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.262033 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.262033 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4293 2024-04-25 07:41:33.262033 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1529 2024-04-25 07:41:33.262033 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1569 2024-04-25 07:41:33.262033 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2304 2024-04-25 07:41:33.263029 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1112 2024-04-25 07:41:33.263029 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1463 2024-04-25 07:41:33.263029 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3180 2024-04-25 07:41:33.263029 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0     5271 2024-04-25 07:41:33.263029 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0    10038 2024-04-25 07:41:33.263029 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0       53 2024-04-25 07:41:33.264026 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-25 07:41:33.264026 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0     4223 2024-04-25 07:41:33.264026 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0        0        0    28145 2024-04-25 07:41:33.264026 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0    25758 2024-04-25 07:41:33.264026 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0     7161 2024-04-25 07:41:33.265023 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     2901 2024-04-25 07:41:33.265023 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    17110 2024-04-25 07:41:33.265023 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    18186 2024-04-25 07:41:33.265023 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    36730 2024-04-25 07:41:33.266020 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     2940 2024-04-25 07:41:33.266020 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24686 2024-04-25 07:41:33.267017 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.267017 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      603 2024-04-25 07:41:33.267017 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.267017 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24729 2024-04-25 07:41:33.267017 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.268012 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5361 2024-04-25 07:41:33.268012 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    19519 2024-04-25 07:41:33.268012 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    28607 2024-04-25 07:41:33.268012 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5860 2024-04-25 07:41:33.269009 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0    10162 2024-04-25 07:41:33.269009 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     2594 2024-04-25 07:41:33.269009 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5619 2024-04-25 07:41:33.269009 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11829 2024-04-25 07:41:33.269009 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0     8409 2024-04-25 07:41:33.269009 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.270007 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1053 2024-04-25 07:41:33.270007 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1717 2024-04-25 07:41:33.270007 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1947 2024-04-25 07:41:33.270007 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5542 2024-04-25 07:41:33.270007 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      253 2024-04-25 07:41:33.271002 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     5952 2024-04-25 07:41:33.271002 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3293 2024-04-25 07:41:33.271002 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     1158 2024-04-25 07:41:33.271002 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0        0        0     2190 2024-04-25 07:41:33.271002 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1205 2024-04-25 07:41:33.271002 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3148 2024-04-25 07:41:33.271002 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5275 2024-04-25 07:41:33.272000 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      743 2024-04-25 07:41:33.272000 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3198 2024-04-25 07:41:33.272000 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     4975 2024-04-25 07:41:33.272000 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      830 2024-04-25 07:41:33.272000 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    11980 2024-04-25 07:41:33.272000 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    22992 2024-04-25 07:41:33.272997 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1232 2024-04-25 07:41:33.272997 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2165 2024-04-25 07:41:33.272997 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     5857 2024-04-25 07:41:33.272997 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9460 2024-04-25 07:41:33.272997 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     7948 2024-04-25 07:41:33.272997 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     9078 2024-04-25 07:41:33.273992 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1829 2024-04-25 07:41:33.273992 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3560 2024-04-25 07:41:33.273992 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4685 2024-04-25 07:41:33.273992 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      611 2024-04-25 07:41:33.273992 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3631 2024-04-25 07:41:33.274990 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18646 2024-04-25 07:41:33.274990 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5401 2024-04-25 07:41:33.274990 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    12053 2024-04-25 07:41:33.275986 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    23516 2024-04-25 07:41:33.276104 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0    13518 2024-04-25 07:41:33.276607 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0     5072 2024-04-25 07:41:33.276607 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0      485 2024-04-25 07:41:33.276607 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1440 2024-04-25 07:41:33.276607 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     5171 2024-04-25 07:41:33.276607 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1598 2024-04-25 07:41:33.277607 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      251 2024-04-25 07:41:33.277607 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5457 2024-04-25 07:41:33.277607 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1070 2024-04-25 07:41:33.277607 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0      810 2024-04-25 07:41:33.277607 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    16855 2024-04-25 07:41:33.278602 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     4057 2024-04-25 07:41:33.278602 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4384 2024-04-25 07:41:33.278602 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     7283 2024-04-25 07:41:33.278602 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      805 2024-04-25 07:41:33.278602 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0       98 2024-04-25 07:41:33.279599 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      267 2024-04-25 07:41:33.279599 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   279760 2024-04-25 07:41:33.281594 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4436 2024-04-25 07:41:33.281594 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     4912 2024-04-25 07:41:33.282590 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31660 2024-04-25 07:41:33.282590 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1810 2024-04-25 07:41:33.282590 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0    10293 2024-04-25 07:41:33.282590 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     4021 2024-04-25 07:41:33.282590 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     5565 2024-04-25 07:41:33.283586 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.283586 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     3354 2024-04-25 07:41:33.283586 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0     3822 2024-04-25 07:41:33.283586 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0      561 2024-04-25 07:41:33.283586 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachinedict.py
+-rw-r--r--   0        0        0     1909 2024-04-25 07:41:33.284583 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1768 2024-04-25 07:41:33.284583 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     4108 2024-04-25 07:41:33.284583 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12437 2024-04-25 07:41:33.284583 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     4036 2024-04-25 07:41:33.284583 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13762 2024-04-25 07:41:33.284583 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1800 2024-04-25 07:41:33.284583 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    37301 2024-04-25 07:41:33.285579 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1800 2024-04-25 07:41:33.285579 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    21019 2024-04-25 07:41:33.285579 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1806 2024-04-25 07:41:33.285579 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    14853 2024-04-25 07:41:33.286576 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    26121 2024-04-25 07:41:33.286576 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    44880 2024-04-25 07:41:33.286576 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1799 2024-04-25 07:41:33.286576 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    27293 2024-04-25 07:41:33.287572 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   109211 2024-04-25 07:41:33.288570 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0   102881 2024-04-25 07:41:33.288570 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0   102576 2024-04-25 07:41:33.289566 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   106012 2024-04-25 07:41:33.289566 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   133760 2024-04-25 07:41:33.290562 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   107154 2024-04-25 07:41:33.290562 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    99752 2024-04-25 07:41:33.291559 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5527 2024-04-25 07:41:33.291559 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     6239 2024-04-25 07:41:33.291559 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/macromanprober.py
+-rw-r--r--   0        0        0     3810 2024-04-25 07:41:33.291559 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2188 2024-04-25 07:41:33.291559 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    31052 2024-04-25 07:41:33.292556 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.292556 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13912 2024-04-25 07:41:33.292556 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      418 2024-04-25 07:41:33.292556 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/resultdict.py
+-rw-r--r--   0        0        0     6562 2024-04-25 07:41:33.293553 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4225 2024-04-25 07:41:33.293553 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     4112 2024-04-25 07:41:33.293553 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    15210 2024-04-25 07:41:33.293553 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8730 2024-04-25 07:41:33.293553 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2894 2024-04-25 07:41:33.293553 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      253 2024-04-25 07:41:33.294552 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0      271 2024-04-25 07:41:33.294552 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2407 2024-04-25 07:41:33.294552 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    11438 2024-04-25 07:41:33.294552 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3449 2024-04-25 07:41:33.295547 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0       76 2024-04-25 07:41:33.295547 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/__init__.py
+-rw-r--r--   0        0        0     2907 2024-04-25 07:41:33.295547 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansi_test.py
+-rw-r--r--   0        0        0    10788 2024-04-25 07:41:33.295547 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py
+-rw-r--r--   0        0        0     6845 2024-04-25 07:41:33.295547 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/initialise_test.py
+-rw-r--r--   0        0        0     1923 2024-04-25 07:41:33.296543 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/isatty_test.py
+-rw-r--r--   0        0        0     1138 2024-04-25 07:41:33.296543 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/utils.py
+-rw-r--r--   0        0        0     3810 2024-04-25 07:41:33.296543 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/winterm_test.py
+-rw-r--r--   0        0        0     6395 2024-04-25 07:41:33.296543 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     7366 2024-04-25 07:41:33.296543 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0      656 2024-04-25 07:41:33.297540 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    42254 2024-04-25 07:41:33.297540 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    52975 2024-04-25 07:41:33.297540 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    21460 2024-04-25 07:41:33.298537 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    53335 2024-04-25 07:41:33.298537 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    15095 2024-04-25 07:41:33.298537 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5361 2024-04-25 07:41:33.299533 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    40949 2024-04-25 07:41:33.299533 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    11149 2024-04-25 07:41:33.299533 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18723 2024-04-25 07:41:33.299533 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/scripts.py
+-rwxr-xr-x   0        0        0    97792 2024-04-25 07:41:33.300530 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t32.exe
+-rwxr-xr-x   0        0        0   182784 2024-04-25 07:41:33.302523 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rwxr-xr-x   0        0        0   108032 2024-04-25 07:41:33.303520 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    68382 2024-04-25 07:41:33.304517 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23976 2024-04-25 07:41:33.304517 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/version.py
+-rwxr-xr-x   0        0        0    91648 2024-04-25 07:41:33.304517 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w32.exe
+-rwxr-xr-x   0        0        0   168448 2024-04-25 07:41:33.305513 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rwxr-xr-x   0        0        0   101888 2024-04-25 07:41:33.306512 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    45224 2024-04-25 07:41:33.306512 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0     1035 2024-04-25 07:41:33.306512 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       68 2024-04-25 07:41:33.306512 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    50727 2024-04-25 07:41:33.307507 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0      893 2024-04-25 07:41:33.307507 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3482 2024-04-25 07:41:33.307507 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      338 2024-04-25 07:41:33.308503 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    14509 2024-04-25 07:41:33.308503 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    46510 2024-04-25 07:41:33.309500 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1955 2024-04-25 07:41:33.309500 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2024-04-25 07:41:33.309500 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   248014 2024-04-25 07:41:33.311498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1189 2024-04-25 07:41:33.311498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1129 2024-04-25 07:41:33.311498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6273 2024-04-25 07:41:33.311498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    35571 2024-04-25 07:41:33.312493 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      687 2024-04-25 07:41:33.312493 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      522 2024-04-25 07:41:33.312493 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11789 2024-04-25 07:41:33.312493 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4514 2024-04-25 07:41:33.313490 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1492 2024-04-25 07:41:33.313490 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8789 2024-04-25 07:41:33.313490 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4822 2024-04-25 07:41:33.313490 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30881 2024-04-25 07:41:33.314487 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    16184 2024-04-25 07:41:33.314487 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4336 2024-04-25 07:41:33.314487 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    15159 2024-04-25 07:41:33.315480 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   111851 2024-04-25 07:41:33.316477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0      570 2024-04-25 07:41:33.316477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/py31compat.py
+-rw-r--r--   0        0        0    13532 2024-04-25 07:41:33.316477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1222 2024-04-25 07:41:33.316477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4236 2024-04-25 07:41:33.317477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     5066 2024-04-25 07:41:33.317477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2791 2024-04-25 07:41:33.317477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     7124 2024-04-25 07:41:33.317477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0      164 2024-04-25 07:41:33.317477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     6848 2024-04-25 07:41:33.318474 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     3093 2024-04-25 07:41:33.318474 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      370 2024-04-25 07:41:33.318474 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    24844 2024-04-25 07:41:33.318474 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1778 2024-04-25 07:41:33.318474 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     2037 2024-04-25 07:41:33.319470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0    32699 2024-04-25 07:41:33.319470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     3011 2024-04-25 07:41:33.319470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0     4936 2024-04-25 07:41:33.320467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     5081 2024-04-25 07:41:33.320467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3424 2024-04-25 07:41:33.320467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5276 2024-04-25 07:41:33.320467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    37498 2024-04-25 07:41:33.320467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    22637 2024-04-25 07:41:33.321463 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     5838 2024-04-25 07:41:33.321463 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19746 2024-04-25 07:41:33.321463 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5167 2024-04-25 07:41:33.322460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2295 2024-04-25 07:41:33.322460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5100 2024-04-25 07:41:33.322460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7613 2024-04-25 07:41:33.322460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4538 2024-04-25 07:41:33.322460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    12123 2024-04-25 07:41:33.322460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    32910 2024-04-25 07:41:33.323457 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0    11541 2024-04-25 07:41:33.323457 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0   100947 2024-04-25 07:41:33.324454 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    78835 2024-04-25 07:41:33.324454 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     1049 2024-04-25 07:41:33.325447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2679 2024-04-25 07:41:33.325447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3354 2024-04-25 07:41:33.325447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3148 2024-04-25 07:41:33.325447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     4943 2024-04-25 07:41:33.325447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6388 2024-04-25 07:41:33.325447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     3455 2024-04-25 07:41:33.326447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     5060 2024-04-25 07:41:33.326447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63500 2024-04-25 07:41:33.326447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0     9373 2024-04-25 07:41:33.326447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0     9500 2024-04-25 07:41:33.327443 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6633 2024-04-25 07:41:33.327443 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    13360 2024-04-25 07:41:33.327443 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   219156 2024-04-25 07:41:33.329437 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0    24325 2024-04-25 07:41:33.329437 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0     9290 2024-04-25 07:41:33.329437 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    40311 2024-04-25 07:41:33.330433 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    26152 2024-04-25 07:41:33.330433 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13733 2024-04-25 07:41:33.330433 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    11139 2024-04-25 07:41:33.330433 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     7040 2024-04-25 07:41:33.331430 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0      514 2024-04-25 07:41:33.331430 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/__init__.py
+-rw-r--r--   0        0        0      146 2024-04-25 07:41:33.331430 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_compat.py
+-rw-r--r--   0        0        0    12420 2024-04-25 07:41:33.331430 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_impl.py
+-rw-r--r--   0        0        0      578 2024-04-25 07:41:33.331430 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py
+-rw-r--r--   0        0        0    11133 2024-04-25 07:41:33.332425 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py
+-rw-r--r--   0        0        0     5366 2024-04-25 07:41:33.332425 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      449 2024-04-25 07:41:33.332425 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1445 2024-04-25 07:41:33.332425 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    22025 2024-04-25 07:41:33.332425 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6534 2024-04-25 07:41:33.333423 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10516 2024-04-25 07:41:33.333423 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      603 2024-04-25 07:41:33.333423 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1353 2024-04-25 07:41:33.333423 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    19121 2024-04-25 07:41:33.334420 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3964 2024-04-25 07:41:33.334420 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     4010 2024-04-25 07:41:33.334420 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      766 2024-04-25 07:41:33.334420 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    36314 2024-04-25 07:41:33.334420 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      744 2024-04-25 07:41:33.334420 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30999 2024-04-25 07:41:33.335416 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4363 2024-04-25 07:41:33.335416 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     3011 2024-04-25 07:41:33.335416 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    34328 2024-04-25 07:41:33.335416 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      563 2024-04-25 07:41:33.336413 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.336413 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      162 2024-04-25 07:41:33.336413 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     6005 2024-04-25 07:41:33.336413 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1626 2024-04-25 07:41:33.336413 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    18044 2024-04-25 07:41:33.337410 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4959 2024-04-25 07:41:33.337410 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0     6267 2024-04-25 07:41:33.337410 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8781 2024-04-25 07:41:33.337410 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10547 2024-04-25 07:41:33.337410 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   143845 2024-04-25 07:41:33.338978 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1096 2024-04-25 07:41:33.338978 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2192 2024-04-25 07:41:33.339498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      275 2024-04-25 07:41:33.339498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0     9965 2024-04-25 07:41:33.339498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3319 2024-04-25 07:41:33.339498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1279 2024-04-25 07:41:33.339498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     1724 2024-04-25 07:41:33.339498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_null_file.py
+-rw-r--r--   0        0        0     7372 2024-04-25 07:41:33.340504 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      440 2024-04-25 07:41:33.340504 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5630 2024-04-25 07:41:33.340504 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    20401 2024-04-25 07:41:33.340504 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      367 2024-04-25 07:41:33.340504 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      436 2024-04-25 07:41:33.340504 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    23496 2024-04-25 07:41:33.341498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1996 2024-04-25 07:41:33.341498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2839 2024-04-25 07:41:33.341498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1896 2024-04-25 07:41:33.341498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      923 2024-04-25 07:41:33.341498 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10678 2024-04-25 07:41:33.342500 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     7056 2024-04-25 07:41:33.342500 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3356 2024-04-25 07:41:33.342500 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0    10357 2024-04-25 07:41:33.342500 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4740 2024-04-25 07:41:33.342500 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    18630 2024-04-25 07:41:33.343494 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1092 2024-04-25 07:41:33.343494 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7318 2024-04-25 07:41:33.343494 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0   100737 2024-04-25 07:41:33.344490 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1325 2024-04-25 07:41:33.344490 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5664 2024-04-25 07:41:33.344490 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6855 2024-04-25 07:41:33.344490 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     8146 2024-04-25 07:41:33.344490 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0     1009 2024-04-25 07:41:33.344490 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2597 2024-04-25 07:41:33.345486 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      676 2024-04-25 07:41:33.345486 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1670 2024-04-25 07:41:33.345486 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2597 2024-04-25 07:41:33.345486 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9817 2024-04-25 07:41:33.345486 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5191 2024-04-25 07:41:33.345486 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3353 2024-04-25 07:41:33.346483 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14446 2024-04-25 07:41:33.346483 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14543 2024-04-25 07:41:33.346483 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3780 2024-04-25 07:41:33.346483 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    12192 2024-04-25 07:41:33.346483 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8442 2024-04-25 07:41:33.346483 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5456 2024-04-25 07:41:33.347480 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     5110 2024-04-25 07:41:33.347480 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      862 2024-04-25 07:41:33.347480 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3496 2024-04-25 07:41:33.347480 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0    10882 2024-04-25 07:41:33.347480 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    38445 2024-04-25 07:41:33.348477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    61545 2024-04-25 07:41:33.348477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8387 2024-04-25 07:41:33.348477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11677 2024-04-25 07:41:33.348477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1433 2024-04-25 07:41:33.349473 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0      176 2024-04-25 07:41:33.349473 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4597 2024-04-25 07:41:33.349473 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4907 2024-04-25 07:41:33.349473 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2929 2024-04-25 07:41:33.349473 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1645 2024-04-25 07:41:33.349473 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24961 2024-04-25 07:41:33.350470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4510 2024-04-25 07:41:33.350470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4555 2024-04-25 07:41:33.350470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    27261 2024-04-25 07:41:33.350470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1300 2024-04-25 07:41:33.350470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    35936 2024-04-25 07:41:33.351467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    40680 2024-04-25 07:41:33.351467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3523 2024-04-25 07:41:33.351467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    46995 2024-04-25 07:41:33.351467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3739 2024-04-25 07:41:33.352463 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      107 2024-04-25 07:41:33.352463 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    26758 2024-04-25 07:41:33.352463 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9416 2024-04-25 07:41:33.352463 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    35710 2024-04-25 07:41:33.353460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0    19161 2024-04-25 07:41:33.353460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3441 2024-04-25 07:41:33.353460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     2012 2024-04-25 07:41:33.353460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1542 2024-04-25 07:41:33.354460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1425 2024-04-25 07:41:33.354460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     1966 2024-04-25 07:41:33.354460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1426 2024-04-25 07:41:33.354460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0     7854 2024-04-25 07:41:33.354460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     2886 2024-04-25 07:41:33.354460 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2239 2024-04-25 07:41:33.355454 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8283 2024-04-25 07:41:33.355454 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      407 2024-04-25 07:41:33.355454 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    23324 2024-04-25 07:41:33.355454 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     3050 2024-04-25 07:41:33.355454 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      264 2024-04-25 07:41:33.356450 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0    83672 2024-04-25 07:41:33.356450 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     3435 2024-04-25 07:41:33.356450 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    11171 2024-04-25 07:41:33.357447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       66 2024-04-25 07:41:33.357447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20636 2024-04-25 07:41:33.357447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    40213 2024-04-25 07:41:33.357447 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.358442 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      993 2024-04-25 07:41:33.358442 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.358442 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    18149 2024-04-25 07:41:33.358442 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    14317 2024-04-25 07:41:33.358442 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0    11351 2024-04-25 07:41:33.359439 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4658 2024-04-25 07:41:33.359439 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17597 2024-04-25 07:41:33.359439 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    35365 2024-04-25 07:41:33.360438 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7315 2024-04-25 07:41:33.360438 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0     8540 2024-04-25 07:41:33.360438 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8836 2024-04-25 07:41:33.360438 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2538 2024-04-25 07:41:33.360438 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.361433 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.361433 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1468 2024-04-25 07:41:33.361433 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0    35742 2024-04-25 07:41:33.361433 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0    20326 2024-04-25 07:41:33.362430 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     6157 2024-04-25 07:41:33.362430 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    31511 2024-04-25 07:41:33.362430 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0     1204 2024-04-25 07:41:33.362430 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     5049 2024-04-25 07:41:33.362430 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1662 2024-04-25 07:41:33.363427 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      520 2024-04-25 07:41:33.363427 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     4134 2024-04-25 07:41:33.363427 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3617 2024-04-25 07:41:33.363427 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22621 2024-04-25 07:41:33.363427 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17672 2024-04-25 07:41:33.364423 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5917 2024-04-25 07:41:33.364423 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     7116 2024-04-25 07:41:33.364958 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10271 2024-04-25 07:41:33.364958 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14726 2024-04-25 07:41:33.364958 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5555 2024-04-25 07:41:33.365472 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0      499 2024-04-25 07:41:33.365472 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0    10930 2024-04-25 07:41:33.365472 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     7084 2024-04-25 07:41:33.365472 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1384 2024-04-25 07:41:33.365472 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6910 2024-04-25 07:41:33.366477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4624 2024-04-25 07:41:33.366477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0      290 2024-04-25 07:41:33.366477 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      128 2024-04-25 07:41:33.244093 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2024-04-25 07:41:33.243095 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1113 2024-04-25 07:41:33.243095 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4160 2024-04-25 07:41:33.243095 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0    76671 2024-04-25 07:41:33.243095 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.244093 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0        5 2024-04-25 07:41:33.244093 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0       97 2024-04-25 07:41:33.244093 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0   111748 2024-04-25 07:41:33.367474 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.367474 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    25276 2024-04-25 07:41:33.367474 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/appdirs.py
+-rw-r--r--   0        0        0      763 2024-04-25 07:41:33.367474 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      588 2024-04-25 07:41:33.368470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     1166 2024-04-25 07:41:33.368470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0     2108 2024-04-25 07:41:33.368470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     1860 2024-04-25 07:41:33.368470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_typing.py
+-rw-r--r--   0        0        0     9870 2024-04-25 07:41:33.368470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     5100 2024-04-25 07:41:33.368470 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    32778 2024-04-25 07:41:33.369467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    24774 2024-04-25 07:41:33.369467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     1876 2024-04-25 07:41:33.369467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16001 2024-04-25 07:41:33.369467 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   237588 2024-04-25 07:41:33.371665 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/pyparsing.py
+-rw-r--r--   0        0        0     2448 2024-04-25 07:41:33.371665 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0      112 2024-04-25 07:41:33.371665 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/tests/data/my-test-package-source/setup.py
+-rw-r--r--   0        0        0     7938 2024-04-25 07:41:33.373659 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-25 07:41:33.373659 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_deprecation_warning.py
+-rw-r--r--   0        0        0      266 2024-04-25 07:41:33.374655 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0    21250 2024-04-25 07:41:33.374655 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8881 2024-04-25 07:41:33.374655 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    14925 2024-04-25 07:41:33.374655 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    48047 2024-04-25 07:41:33.375772 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    18385 2024-04-25 07:41:33.375772 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0      660 2024-04-25 07:41:33.375772 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     5406 2024-04-25 07:41:33.376779 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4792 2024-04-25 07:41:33.376779 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    40520 2024-04-25 07:41:33.376779 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_msi.py
+-rw-r--r--   0        0        0    22373 2024-04-25 07:41:33.377770 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0    16099 2024-04-25 07:41:33.377770 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_wininst.py
+-rw-r--r--   0        0        0     5740 2024-04-25 07:41:33.377770 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     7908 2024-04-25 07:41:33.377770 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    32208 2024-04-25 07:41:33.378771 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    17833 2024-04-25 07:41:33.378771 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     6507 2024-04-25 07:41:33.378771 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     6012 2024-04-25 07:41:33.378771 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2677 2024-04-25 07:41:33.379763 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13512 2024-04-25 07:41:33.379763 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    28171 2024-04-25 07:41:33.379763 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2861 2024-04-25 07:41:33.379763 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2715 2024-04-25 07:41:33.380764 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1232 2024-04-25 07:41:33.380764 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8666 2024-04-25 07:41:33.380764 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     1995 2024-04-25 07:41:33.380764 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      703 2024-04-25 07:41:33.380764 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    12088 2024-04-25 07:41:33.381760 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19766 2024-04-25 07:41:33.381760 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7654 2024-04-25 07:41:33.381760 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0     5045 2024-04-25 07:41:33.381760 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     9110 2024-04-25 07:41:33.381760 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    16550 2024-04-25 07:41:33.382757 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      144 2024-04-25 07:41:33.382757 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0     3519 2024-04-25 07:41:33.382757 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     8264 2024-04-25 07:41:33.382757 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    51532 2024-04-25 07:41:33.382757 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3716 2024-04-25 07:41:33.383754 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10497 2024-04-25 07:41:33.383754 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    18261 2024-04-25 07:41:33.383754 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8335 2024-04-25 07:41:33.383754 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    13615 2024-04-25 07:41:33.383754 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     2052 2024-04-25 07:41:33.384747 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    30633 2024-04-25 07:41:33.384747 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    23971 2024-04-25 07:41:33.384747 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      474 2024-04-25 07:41:33.385744 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/py35compat.py
+-rw-r--r--   0        0        0      221 2024-04-25 07:41:33.385744 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0     4494 2024-04-25 07:41:33.385744 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    22267 2024-04-25 07:41:33.385744 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12386 2024-04-25 07:41:33.385744 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    14832 2024-04-25 07:41:33.386740 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    21614 2024-04-25 07:41:33.386740 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    12772 2024-04-25 07:41:33.386740 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5276 2024-04-25 07:41:33.386740 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0     2514 2024-04-25 07:41:33.387740 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.387740 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15618 2024-04-25 07:41:33.387740 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0      763 2024-04-25 07:41:33.387740 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      588 2024-04-25 07:41:33.387740 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     1168 2024-04-25 07:41:33.388733 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_compat.py
+-rw-r--r--   0        0        0     2108 2024-04-25 07:41:33.388733 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     1860 2024-04-25 07:41:33.388733 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_typing.py
+-rw-r--r--   0        0        0     9863 2024-04-25 07:41:33.388733 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     5088 2024-04-25 07:41:33.388733 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    32778 2024-04-25 07:41:33.389734 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    24778 2024-04-25 07:41:33.389734 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     1876 2024-04-25 07:41:33.389734 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16003 2024-04-25 07:41:33.389734 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0   237588 2024-04-25 07:41:33.390731 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/pyparsing.py
+-rw-r--r--   0        0        0     7270 2024-04-25 07:41:33.390731 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    10356 2024-04-25 07:41:33.391724 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/build_meta.py
+-rwxr-xr-x   0        0        0    65536 2024-04-25 07:41:33.392727 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli-32.exe
+-rwxr-xr-x   0        0        0    74752 2024-04-25 07:41:33.393312 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli-64.exe
+-rwxr-xr-x   0        0        0    65536 2024-04-25 07:41:33.393819 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0      648 2024-04-25 07:41:33.393819 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     2461 2024-04-25 07:41:33.393819 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    17079 2024-04-25 07:41:33.394824 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0      883 2024-04-25 07:41:33.394824 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     4489 2024-04-25 07:41:33.394824 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    13579 2024-04-25 07:41:33.394824 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0     9586 2024-04-25 07:41:33.394824 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     8285 2024-04-25 07:41:33.395820 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0     1031 2024-04-25 07:41:33.395820 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    87874 2024-04-25 07:41:33.395820 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    25626 2024-04-25 07:41:33.396813 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     4873 2024-04-25 07:41:33.396813 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     2252 2024-04-25 07:41:33.396813 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     3995 2024-04-25 07:41:33.396813 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2688 2024-04-25 07:41:33.396813 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      643 2024-04-25 07:41:33.397814 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0     5097 2024-04-25 07:41:33.397814 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0        0        0      486 2024-04-25 07:41:33.397814 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2159 2024-04-25 07:41:33.397814 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      678 2024-04-25 07:41:33.397814 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     8114 2024-04-25 07:41:33.397814 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     5029 2024-04-25 07:41:33.397814 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0     9812 2024-04-25 07:41:33.398810 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/test.py
+-rw-r--r--   0        0        0      479 2024-04-25 07:41:33.398810 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7500 2024-04-25 07:41:33.398810 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0    22705 2024-04-25 07:41:33.398810 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/config.py
+-rw-r--r--   0        0        0      960 2024-04-25 07:41:33.398810 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5680 2024-04-25 07:41:33.399807 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    41467 2024-04-25 07:41:33.399807 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0      540 2024-04-25 07:41:33.399807 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     1739 2024-04-25 07:41:33.399807 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     2495 2024-04-25 07:41:33.400805 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0     5034 2024-04-25 07:41:33.400805 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/glob.py
+-rwxr-xr-x   0        0        0    65536 2024-04-25 07:41:33.400805 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui-32.exe
+-rwxr-xr-x   0        0        0    75264 2024-04-25 07:41:33.401800 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui-64.exe
+-rwxr-xr-x   0        0        0    65536 2024-04-25 07:41:33.401800 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     3734 2024-04-25 07:41:33.401800 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      848 2024-04-25 07:41:33.401800 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     2414 2024-04-25 07:41:33.401800 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/lib2to3_ex.py
+-rw-r--r--   0        0        0     5374 2024-04-25 07:41:33.402797 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    53059 2024-04-25 07:41:33.402797 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     3145 2024-04-25 07:41:33.402797 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    42201 2024-04-25 07:41:33.403794 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0      260 2024-04-25 07:41:33.403794 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/py34compat.py
+-rw-r--r--   0        0        0    14994 2024-04-25 07:41:33.403794 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      224 2024-04-25 07:41:33.403794 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      141 2024-04-25 07:41:33.403794 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0     8816 2024-04-25 07:41:33.404791 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/ssl_support.py
+-rw-r--r--   0        0        0      983 2024-04-25 07:41:33.404791 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      150 2024-04-25 07:41:33.404791 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     8521 2024-04-25 07:41:33.404791 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      743 2024-04-25 07:41:33.404791 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      241 2024-04-25 07:41:33.373659 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/dependency_links.txt
+-rw-r--r--   0        0        0     2929 2024-04-25 07:41:33.373659 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        5 2024-04-25 07:41:33.372662 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1069 2024-04-25 07:41:33.372662 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/LICENSE
+-rw-r--r--   0        0        0     4873 2024-04-25 07:41:33.372662 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/METADATA
+-rw-r--r--   0        0        0    22796 2024-04-25 07:41:33.372662 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.372662 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/REQUESTED
+-rw-r--r--   0        0        0       44 2024-04-25 07:41:33.373659 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/top_level.txt
+-rw-r--r--   0        0        0       97 2024-04-25 07:41:33.372662 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/WHEEL
+-rw-r--r--   0        0        0        3 2024-04-25 07:41:33.404791 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib64
+-rw-r--r--   0        0        0      116 2024-04-25 07:41:33.404791 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/pyvenv.cfg
+-rw-r--r--   0        0        0      251 2024-04-25 07:41:33.405787 greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/virtualenv_runner.log
+-rw-r--r--   0        0        0       81 2024-04-25 07:41:33.406784 greatlibrarian-0.0.9/greatlibrarian/Agents/PromptMarket/__init__.py
+-rw-r--r--   0        0        0     3606 2024-04-25 07:41:33.406784 greatlibrarian-0.0.9/greatlibrarian/Agents/PromptMarket/getContextExamples.py
+-rw-r--r--   0        0        0     2206 2024-04-25 07:41:33.406784 greatlibrarian-0.0.9/greatlibrarian/Agents/PromptMarket/main.py
+-rw-r--r--   0        0        0     1602 2024-04-25 07:41:33.407779 greatlibrarian-0.0.9/greatlibrarian/Agents/PromptMarket/promptGenerator.py
+-rw-r--r--   0        0        0      305 2024-04-25 07:41:33.407779 greatlibrarian-0.0.9/greatlibrarian/Agents/PromptMarket/testAPI.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.407779 greatlibrarian-0.0.9/greatlibrarian/Agents/TranslationAPI/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-25 07:41:33.407779 greatlibrarian-0.0.9/greatlibrarian/Agents/TranslationAPI/translationGPT.py
+-rw-r--r--   0        0        0       60 2024-04-25 07:41:33.408775 greatlibrarian-0.0.9/greatlibrarian/Analyser/__init__.py
+-rw-r--r--   0        0        0    22812 2024-04-26 01:09:52.498125 greatlibrarian-0.0.9/greatlibrarian/Analyser/analyse.py
+-rw-r--r--   0        0        0     2276 2024-04-25 07:41:33.408775 greatlibrarian-0.0.9/greatlibrarian/Analyser/getInfo.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.411767 greatlibrarian-0.0.9/greatlibrarian/Assets/__init__.py
+-rw-r--r--   0        0        0   432227 2024-04-25 07:41:33.411767 greatlibrarian-0.0.9/greatlibrarian/Assets/GreatLibrarian.pdf
+-rw-r--r--   0        0        0      773 2024-04-25 07:41:33.411767 greatlibrarian-0.0.9/greatlibrarian/Assets/template.py
+-rw-r--r--   0        0        0       67 2024-04-25 07:41:33.411767 greatlibrarian-0.0.9/greatlibrarian/Configs/__init__.py
+-rw-r--r--   0        0        0      197 2024-04-25 07:41:33.412763 greatlibrarian-0.0.9/greatlibrarian/Configs/base.py
+-rw-r--r--   0        0        0      456 2024-04-25 07:41:33.412763 greatlibrarian-0.0.9/greatlibrarian/Configs/example_config.py
+-rw-r--r--   0        0        0      162 2024-04-26 01:09:52.498125 greatlibrarian-0.0.9/greatlibrarian/Core/__init__.py
+-rw-r--r--   0        0        0      776 2024-04-25 07:41:33.412763 greatlibrarian-0.0.9/greatlibrarian/Core/agents.py
+-rw-r--r--   0        0        0     1226 2024-04-25 07:41:33.412763 greatlibrarian-0.0.9/greatlibrarian/Core/evalMethods.py
+-rw-r--r--   0        0        0      510 2024-04-26 01:09:52.499122 greatlibrarian-0.0.9/greatlibrarian/Core/finalscore.py
+-rw-r--r--   0        0        0      689 2024-04-25 07:41:33.412763 greatlibrarian-0.0.9/greatlibrarian/Core/LLMs.py
+-rw-r--r--   0        0        0      551 2024-04-25 07:41:33.412763 greatlibrarian-0.0.9/greatlibrarian/Core/TestCase.py
+-rw-r--r--   0        0        0      126 2024-04-25 07:41:33.413761 greatlibrarian-0.0.9/greatlibrarian/EvalMethods/__init__.py
+-rw-r--r--   0        0        0     3024 2024-04-25 07:41:33.413761 greatlibrarian-0.0.9/greatlibrarian/EvalMethods/blacklist.py
+-rw-r--r--   0        0        0     3873 2024-04-25 07:41:33.413761 greatlibrarian-0.0.9/greatlibrarian/EvalMethods/keyword.py
+-rw-r--r--   0        0        0     6078 2024-04-25 07:41:33.414757 greatlibrarian-0.0.9/greatlibrarian/EvalMethods/llmEval.py
+-rw-r--r--   0        0        0     3918 2024-04-25 07:41:33.414757 greatlibrarian-0.0.9/greatlibrarian/EvalMethods/toolUsage.py
+-rw-r--r--   0        0        0       38 2024-04-26 01:09:52.499122 greatlibrarian-0.0.9/greatlibrarian/FinalScore/__init__.py
+-rw-r--r--   0        0        0     2223 2024-04-25 07:41:33.414757 greatlibrarian-0.0.9/greatlibrarian/FinalScore/finalscore1.py
+-rw-r--r--   0        0        0      158 2024-04-25 07:41:33.414757 greatlibrarian-0.0.9/greatlibrarian/Interactor/__init__.py
+-rw-r--r--   0        0        0     9019 2024-04-25 07:41:33.415753 greatlibrarian-0.0.9/greatlibrarian/Interactor/autoInteractor.py
+-rw-r--r--   0        0        0        0 2024-04-25 07:41:33.415753 greatlibrarian-0.0.9/greatlibrarian/Interactor/fairnessInteractor.py
+-rw-r--r--   0        0        0     5283 2024-04-25 07:41:33.415753 greatlibrarian-0.0.9/greatlibrarian/Interactor/hallucinationInteractor.py
+-rw-r--r--   0        0        0     9128 2024-04-25 07:41:33.415753 greatlibrarian-0.0.9/greatlibrarian/Interactor/multiturnInteractor.py
+-rw-r--r--   0        0        0      123 2024-04-25 07:41:33.416748 greatlibrarian-0.0.9/greatlibrarian/LLMs/__init__.py
+-rw-r--r--   0        0        0       66 2024-04-25 07:41:33.415753 greatlibrarian-0.0.9/greatlibrarian/LLMs/APIs/__init__.py
+-rw-r--r--   0        0        0     6665 2024-04-25 07:41:33.416748 greatlibrarian-0.0.9/greatlibrarian/LLMs/APIs/openai.py
+-rw-r--r--   0        0        0     1556 2024-04-25 07:41:33.417746 greatlibrarian-0.0.9/greatlibrarian/LLMs/dbInteractor.py
+-rw-r--r--   0        0        0      398 2024-04-25 07:41:33.416748 greatlibrarian-0.0.9/greatlibrarian/LLMs/LLMs.ini
+-rw-r--r--   0        0        0       34 2024-04-25 07:41:33.416748 greatlibrarian-0.0.9/greatlibrarian/LLMs/OpenSource/__init__.py
+-rw-r--r--   0        0        0     1782 2024-04-25 07:41:33.416748 greatlibrarian-0.0.9/greatlibrarian/LLMs/OpenSource/chatGLM6B.py
+-rw-r--r--   0        0        0     1743 2024-04-25 07:41:33.416748 greatlibrarian-0.0.9/greatlibrarian/LLMs/OpenSource/chatglm6b_2.py
+-rw-r--r--   0        0        0       30 2024-04-25 07:41:33.417746 greatlibrarian-0.0.9/greatlibrarian/Recoder/__init__.py
+-rw-r--r--   0        0        0      123 2024-04-25 07:41:33.417746 greatlibrarian-0.0.9/greatlibrarian/Recoder/recoder.py
+-rw-r--r--   0        0        0     1351 2024-04-25 07:41:33.420736 greatlibrarian-0.0.9/greatlibrarian/register.py
+-rw-r--r--   0        0        0     3934 2024-04-25 07:41:33.421733 greatlibrarian-0.0.9/greatlibrarian/run.py
+-rw-r--r--   0        0        0       76 2024-04-25 07:41:33.417746 greatlibrarian-0.0.9/greatlibrarian/Runner/__init__.py
+-rw-r--r--   0        0        0    10921 2024-04-25 07:41:33.417746 greatlibrarian-0.0.9/greatlibrarian/Runner/autoRunner.py
+-rw-r--r--   0        0        0     2831 2024-04-25 07:41:33.418743 greatlibrarian-0.0.9/greatlibrarian/Runner/updateRunner.py
+-rw-r--r--   0        0        0       38 2024-04-25 07:41:33.418743 greatlibrarian-0.0.9/greatlibrarian/TestCase/__init__.py
+-rw-r--r--   0        0        0     4943 2024-04-25 07:41:33.418743 greatlibrarian-0.0.9/greatlibrarian/TestCase/testProject.py
+-rw-r--r--   0        0        0      497 2024-04-25 07:41:33.418743 greatlibrarian-0.0.9/greatlibrarian/Utils/__init__.py
+-rw-r--r--   0        0        0     1622 2024-04-25 07:41:33.418743 greatlibrarian-0.0.9/greatlibrarian/Utils/clean_log.py
+-rw-r--r--   0        0        0      100 2024-04-25 07:41:33.418743 greatlibrarian-0.0.9/greatlibrarian/Utils/clear_log.py
+-rw-r--r--   0        0        0      586 2024-04-25 07:41:33.419740 greatlibrarian-0.0.9/greatlibrarian/Utils/extract_example.py
+-rw-r--r--   0        0        0      774 2024-04-25 07:41:33.419740 greatlibrarian-0.0.9/greatlibrarian/Utils/human_evaluation.py
+-rw-r--r--   0        0        0      693 2024-04-25 07:41:33.419740 greatlibrarian-0.0.9/greatlibrarian/Utils/io.py
+-rw-r--r--   0        0        0    15555 2024-04-25 07:41:33.419740 greatlibrarian-0.0.9/greatlibrarian/Utils/logger.py
+-rw-r--r--   0        0        0     2298 2024-04-25 07:41:33.419740 greatlibrarian-0.0.9/greatlibrarian/Utils/logsafe.py
+-rw-r--r--   0        0        0      922 2024-04-25 07:41:33.419740 greatlibrarian-0.0.9/greatlibrarian/Utils/mistaken_case.py
+-rw-r--r--   0        0        0      622 2024-04-25 07:41:33.420736 greatlibrarian-0.0.9/greatlibrarian/Utils/process.py
+-rw-r--r--   0        0        0     1030 2024-04-25 07:41:33.420736 greatlibrarian-0.0.9/greatlibrarian/Utils/project_info.py
+-rw-r--r--   0        0        0      643 2024-04-25 07:41:33.420736 greatlibrarian-0.0.9/greatlibrarian/Utils/record_testcase.py
+-rw-r--r--   0        0        0      790 2024-04-25 07:41:33.420736 greatlibrarian-0.0.9/greatlibrarian/Utils/register.py
+-rw-r--r--   0        0        0     5956 2024-04-25 07:41:33.420736 greatlibrarian-0.0.9/greatlibrarian/Utils/registry.py
+-rw-r--r--   0        0        0      250 2024-04-25 07:41:33.420736 greatlibrarian-0.0.9/greatlibrarian/Utils/typetrans.py
+-rw-r--r--   0        0        0      508 2024-04-25 07:41:33.420736 greatlibrarian-0.0.9/greatlibrarian/Utils/update_dialog.py
+-rw-r--r--   0        0        0      620 2024-04-26 01:10:34.783740 greatlibrarian-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    29598 2024-04-25 07:41:33.236119 greatlibrarian-0.0.9/README.md
+-rw-r--r--   0        0        0    29990 1970-01-01 00:00:00.000000 greatlibrarian-0.0.9/PKG-INFO
```

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/BookStore/checkDupli.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/BookStore/checkDupli.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/BookStore/getData.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/BookStore/getData.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/BookStore/RawData/Area Studies/African American Studies.csv` & `greatlibrarian-0.0.9/greatlibrarian/Agents/BookStore/RawData/Area Studies/African American Studies.csv`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/codeEnv.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/codeEnv.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/ttest.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/ttest.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate.csh` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate.fish` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/bin/Activate.ps1` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/bin/Activate.ps1`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/_distutils_hack/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/__main__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/__pip-runner__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/build_env.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cache.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/autocompletion.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/base_command.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/cmdoptions.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/command_context.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/main.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/main_parser.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/parser.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/progress_bars.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/req_command.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/spinners.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/cache.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/check.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/completion.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/configuration.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/debug.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/download.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/freeze.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/hash.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/help.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/index.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/inspect.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/install.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/list.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/search.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/show.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/uninstall.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/wheel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/configuration.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/base.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/installed.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/sdist.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/wheel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/exceptions.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/collector.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/package_finder.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/sources.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/_distutils.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/_sysconfig.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/base.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/_json.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/base.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_compat.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_dists.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_envs.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/pkg_resources.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/candidate.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/direct_url.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/format_control.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/index.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/installation_report.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/link.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/scheme.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/search_scope.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/selection_prefs.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/target_python.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/wheel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/auth.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/cache.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/download.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/lazy_wheel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/session.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/utils.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/xmlrpc.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/build_tracker.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_editable.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_editable.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/check.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/freeze.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/editable_legacy.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/legacy.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/wheel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/prepare.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/pyproject.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/constructors.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_file.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_install.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_set.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_uninstall.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/base.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/resolver.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/base.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/self_outdated_check.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/_log.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/appdirs.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/compat.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/compatibility_tags.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/deprecation.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/direct_url_helpers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/distutils_args.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/egg_link.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/encoding.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/entrypoints.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/filesystem.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/filetypes.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/glibc.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/hashes.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/inject_securetransport.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/logging.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/misc.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/models.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/packaging.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/setuptools_build.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/subprocess.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/temp_dir.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/unpacking.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/urls.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/virtualenv.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/wheel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/bazaar.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/git.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/mercurial.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/subversion.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/versioncontrol.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/wheel_builder.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/adapter.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/cache.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/compat.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/controller.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/serialize.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/core.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/big5freq.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/big5prober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/chardistribution.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachinedict.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/codingstatemachinedict.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/cp949prober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/enums.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/escprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/escsm.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/eucjpprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrfreq.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwfreq.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312freq.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312prober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/hebrewprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/jisfreq.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/johabfreq.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/johabprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/jpcntx.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langthaimodel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/latin1prober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/macromanprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/macromanprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcssm.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/metadata/languages.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sjisprober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/universaldetector.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/utf1632prober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/utf8prober.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/ansi.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/ansitowin32.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/initialise.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansi_test.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansi_test.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/ansitowin32_test.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/initialise_test.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/initialise_test.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/isatty_test.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/isatty_test.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/utils.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/utils.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/winterm_test.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/tests/winterm_test.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/win32.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/winterm.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/compat.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/database.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/index.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/locators.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/manifest.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/markers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/metadata.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/resources.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/scripts.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t32.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t64-arm.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t64.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/util.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/version.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w32.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w64-arm.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w64.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/wheel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distro/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distro/distro.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/codec.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/core.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/idnadata.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/intranges.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/uts46data.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/exceptions.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/ext.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/fallback.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/__about__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_manylinux.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_musllinux.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_structures.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/markers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/requirements.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/specifiers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/tags.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/utils.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/version.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__main__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/android.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/api.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/macos.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/unix.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/windows.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/cmdline.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/console.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/filter.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/filters/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatter.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/groff.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/html.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/img.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/irc.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/latex.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/other.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/svg.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexer.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/python.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/modeline.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/plugin.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/regexopt.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/scanner.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/sphinxext.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/style.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/styles/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/token.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/unistring.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/util.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/actions.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/common.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/core.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/exceptions.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/helpers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/results.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/testing.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/unicode.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/util.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_impl.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_impl.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/pyproject_hooks/_in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/_internal_utils.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/adapters.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/api.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/auth.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/certs.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/compat.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/cookies.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/exceptions.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/help.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/hooks.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/models.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/packages.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/sessions.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/status_codes.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/structures.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/utils.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/providers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/reporters.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/resolvers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/structs.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/__main__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_cell_widths.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_codes.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_replace.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_export_format.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_inspect.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_log_render.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_loop.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_null_file.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_null_file.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_palettes.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_ratio.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_spinners.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_win32_console.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_windows.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_windows_renderer.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_wrap.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/abc.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/align.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/ansi.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/bar.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/box.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/cells.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/color.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/color_triplet.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/columns.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/console.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/constrain.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/containers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/control.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/default_styles.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/diagnose.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/emoji.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/errors.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/file_proxy.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/filesize.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/highlighter.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/json.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/jupyter.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/layout.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/live.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/live_render.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/logging.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/markup.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/measure.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/padding.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/pager.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/palette.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/panel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/pretty.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/progress.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/progress_bar.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/prompt.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/protocol.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/repr.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/rule.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/scope.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/screen.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/segment.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/spinner.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/status.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/style.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/styled.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/syntax.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/table.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/terminal_theme.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/text.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/theme.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/traceback.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/tree.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/six.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/_asyncio.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/_utils.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/after.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/before.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/before_sleep.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/nap.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/retry.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/stop.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/wait.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/_parser.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/_re.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/typing_extensions.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/_collections.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/connection.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/connectionpool.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/exceptions.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/fields.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/filepost.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/six.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/poolmanager.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/request.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/response.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/connection.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/proxy.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/queue.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/queue.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/request.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/response.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/retry.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/timeout.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/url.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/wait.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/labels.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/mklabels.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/tests.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/LICENSE.txt` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/METADATA` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/RECORD` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pip-23.0.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/appdirs.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_compat.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_typing.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/markers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/tags.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/utils.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/version.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/pyparsing.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/extern/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/_msvccompiler.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/archive_util.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/bcppcompiler.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/ccompiler.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/cmd.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_msi.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_msi.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_wininst.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/bdist_wininst.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_clib.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_ext.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_py.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_scripts.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/check.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/clean.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/config.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_data.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_egg_info.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_headers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_lib.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_scripts.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/py37compat.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/register.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/sdist.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/upload.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/config.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/core.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/cygwinccompiler.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dep_util.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dir_util.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dist.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/errors.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/extension.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/fancy_getopt.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/file_util.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/filelist.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/log.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/msvc9compiler.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/msvccompiler.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/spawn.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/sysconfig.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/text_file.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/unixccompiler.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/util.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/version.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/versionpredicate.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_imp.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/ordered_set.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__about__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_compat.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_compat.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_structures.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_typing.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/markers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/requirements.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/specifiers.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/tags.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/utils.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/version.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/pyparsing.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/_vendor/pyparsing.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/archive_util.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/build_meta.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli-32.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli-64.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/alias.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/bdist_egg.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/bdist_rpm.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_clib.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_ext.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_py.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/develop.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/dist_info.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/easy_install.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/egg_info.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_egg_info.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_lib.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_scripts.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/py36compat.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/rotate.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/saveopts.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/sdist.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/setopt.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/test.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/upload_docs.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/config.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/config.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/dep_util.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/depends.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/dist.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/errors.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/extension.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/extern/__init__.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/glob.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui-32.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui-64.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui.exe` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/installer.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/launch.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/lib2to3_ex.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/lib2to3_ex.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/monkey.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/msvc.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/namespaces.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/package_index.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/sandbox.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/ssl_support.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/ssl_support.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/unicode_utils.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/wheel.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/windows_support.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/entry_points.txt` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/LICENSE` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/METADATA` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/RECORD` & `greatlibrarian-0.0.9/greatlibrarian/Agents/CodeRunner/VirEnv/lib/python3.8/site-packages/setuptools-56.0.0.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/PromptMarket/getContextExamples.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/PromptMarket/getContextExamples.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/PromptMarket/main.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/PromptMarket/main.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Agents/PromptMarket/promptGenerator.py` & `greatlibrarian-0.0.9/greatlibrarian/Agents/PromptMarket/promptGenerator.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Analyser/analyse.py` & `greatlibrarian-0.0.9/greatlibrarian/Analyser/analyse.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,14 +518,8 @@
 
             multiline_latex = match.replace('\n', '\\\\')
 
             input_str = input_str.replace('$$' + match + '$$', r'\begin{equation}' + multiline_latex + r'\end{equation}')
 
         input_str = re.sub(pattern, '', input_str)
         
-        return input_str
-
-
-
-    
-        text = re.sub(r"([#$%&~_^\\{}])", r"\\\1", text)
-        return text
+        return input_str
```

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Analyser/getInfo.py` & `greatlibrarian-0.0.9/greatlibrarian/Analyser/getInfo.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Assets/GreatLibrarian.pdf` & `greatlibrarian-0.0.9/greatlibrarian/Assets/GreatLibrarian.pdf`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Assets/template.py` & `greatlibrarian-0.0.9/greatlibrarian/Assets/template.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Core/agents.py` & `greatlibrarian-0.0.9/greatlibrarian/Core/agents.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Core/evalMethods.py` & `greatlibrarian-0.0.9/greatlibrarian/Core/evalMethods.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Core/LLMs.py` & `greatlibrarian-0.0.9/greatlibrarian/Core/LLMs.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Core/TestCase.py` & `greatlibrarian-0.0.9/greatlibrarian/Core/TestCase.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/EvalMethods/blacklist.py` & `greatlibrarian-0.0.9/greatlibrarian/EvalMethods/blacklist.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/EvalMethods/keyword.py` & `greatlibrarian-0.0.9/greatlibrarian/EvalMethods/keyword.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/EvalMethods/llmEval.py` & `greatlibrarian-0.0.9/greatlibrarian/EvalMethods/llmEval.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/EvalMethods/toolUsage.py` & `greatlibrarian-0.0.9/greatlibrarian/EvalMethods/toolUsage.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/FinalScore/finalscore1.py` & `greatlibrarian-0.0.9/greatlibrarian/FinalScore/finalscore1.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Interactor/autoInteractor.py` & `greatlibrarian-0.0.9/greatlibrarian/Interactor/autoInteractor.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Interactor/hallucinationInteractor.py` & `greatlibrarian-0.0.9/greatlibrarian/Interactor/hallucinationInteractor.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Interactor/multiturnInteractor.py` & `greatlibrarian-0.0.9/greatlibrarian/Interactor/multiturnInteractor.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/LLMs/APIs/openai.py` & `greatlibrarian-0.0.9/greatlibrarian/LLMs/APIs/openai.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/LLMs/dbInteractor.py` & `greatlibrarian-0.0.9/greatlibrarian/LLMs/dbInteractor.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/LLMs/OpenSource/chatGLM6B.py` & `greatlibrarian-0.0.9/greatlibrarian/LLMs/OpenSource/chatGLM6B.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/LLMs/OpenSource/chatglm6b_2.py` & `greatlibrarian-0.0.9/greatlibrarian/LLMs/OpenSource/chatglm6b_2.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/register.py` & `greatlibrarian-0.0.9/greatlibrarian/register.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/run.py` & `greatlibrarian-0.0.9/greatlibrarian/run.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Runner/autoRunner.py` & `greatlibrarian-0.0.9/greatlibrarian/Runner/autoRunner.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Runner/updateRunner.py` & `greatlibrarian-0.0.9/greatlibrarian/Runner/updateRunner.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/TestCase/testProject.py` & `greatlibrarian-0.0.9/greatlibrarian/TestCase/testProject.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/clean_log.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/clean_log.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/extract_example.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/extract_example.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/human_evaluation.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/human_evaluation.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/io.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/io.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/logger.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/logger.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/logsafe.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/logsafe.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/mistaken_case.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/mistaken_case.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/process.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/process.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/project_info.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/project_info.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/record_testcase.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/record_testcase.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/register.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/register.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/greatlibrarian/Utils/registry.py` & `greatlibrarian-0.0.9/greatlibrarian/Utils/registry.py`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/pyproject.toml` & `greatlibrarian-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "greatlibrarian"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["dmj <ggxxding@163.com>"]
 readme = "README.md"
 repository = "https://github.com/JerryMazeyu/GreatLibrarian"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `greatlibrarian-0.0.8/README.md` & `greatlibrarian-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `greatlibrarian-0.0.8/PKG-INFO` & `greatlibrarian-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greatlibrarian
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Home-page: https://github.com/JerryMazeyu/GreatLibrarian
 Author: dmj
 Author-email: ggxxding@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

