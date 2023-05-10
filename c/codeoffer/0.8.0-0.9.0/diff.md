# Comparing `tmp/codeoffer-0.8.0.tar.gz` & `tmp/codeoffer-0.9.0.tar.gz`

## Comparing `codeoffer-0.8.0.tar` & `codeoffer-0.9.0.tar`

### file list

```diff
@@ -1,812 +1,812 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 codeoffer-0.8.0/.idea/.gitignore
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 codeoffer-0.8.0/.idea/misc.xml
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 codeoffer-0.8.0/.idea/modules.xml
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 codeoffer-0.8.0/.idea/v1-python-library.iml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 codeoffer-0.8.0/.idea/vcs.xml
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 codeoffer-0.8.0/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 codeoffer-0.8.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/codeoffer/__init__.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 codeoffer-0.8.0/codeoffer/api.py
--rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 codeoffer-0.8.0/codeoffer/app.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 codeoffer-0.8.0/codeoffer/exceptions.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 codeoffer-0.8.0/codeoffer/oauth.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 codeoffer-0.8.0/codeoffer/user.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 codeoffer-0.8.0/codeoffer/utilities.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/.gitignore
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/pyvenv.cfg
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/_virtualenv.pth
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/_virtualenv.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/distutils-precedence.pth
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip-22.3.1.virtualenv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.virtualenv
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel-0.38.4.virtualenv
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/_distutils_hack/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/_distutils_hack/override.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/__init__.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/__main__.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/__pip-runner__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/py.typed
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/__init__.py
--rw-r--r--   0        0        0    10234 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/build_env.py
--rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cache.py
--rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/configuration.py
--rw-r--r--   0        0        0    20942 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/exceptions.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/main.py
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/pyproject.py
--rw-r--r--   0        0        0     8020 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
--rw-r--r--   0        0        0    13079 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/wheel_builder.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/__init__.py
--rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
--rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/base_command.py
--rw-r--r--   0        0        0    29381 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/command_context.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/main.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/parser.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
--rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/req_command.py
--rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/spinners.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
--rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/__init__.py
--rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/cache.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/check.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/completion.py
--rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/configuration.py
--rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/debug.py
--rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/download.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/freeze.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/hash.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/help.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/index.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/inspect.py
--rw-r--r--   0        0        0    31726 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/install.py
--rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/list.py
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/search.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/show.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
--rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/wheel.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/distributions/base.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/distributions/installed.py
--rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/index/__init__.py
--rw-r--r--   0        0        0    16503 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/index/collector.py
--rw-r--r--   0        0        0    37596 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/index/package_finder.py
--rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/index/sources.py
--rw-r--r--   0        0        0    17552 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/locations/__init__.py
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
--rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/locations/base.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/_json.py
--rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/base.py
--rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
--rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/__init__.py
--rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/candidate.py
--rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/direct_url.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/format_control.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/index.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/installation_report.py
--rw-r--r--   0        0        0    18083 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/link.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/scheme.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/search_scope.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/target_python.py
--rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/wheel.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/__init__.py
--rw-r--r--   0        0        0    12190 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/auth.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/cache.py
--rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/download.py
--rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
--rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/session.py
--rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/utils.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/__init__.py
--rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/check.py
--rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/freeze.py
--rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/prepare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
--rw-r--r--   0        0        0    27407 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/__init__.py
--rw-r--r--   0        0        0    16611 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/constructors.py
--rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/req_file.py
--rw-r--r--   0        0        0    35600 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/req_install.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/req_set.py
--rw-r--r--   0        0        0    24045 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
--rw-r--r--   0        0        0    24129 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
--rw-r--r--   0        0        0    18963 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
--rw-r--r--   0        0        0    27878 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
--rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
--rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/_log.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/compat.py
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/datetime.py
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/encoding.py
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
--rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/glibc.py
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/hashes.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
--rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/logging.py
--rw-r--r--   0        0        0    21617 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/misc.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/models.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/packaging.py
--rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
--rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
--rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/urls.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/wheel.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
--rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/git.py
--rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
--rw-r--r--   0        0        0    11728 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
--rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
--rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/__init__.py
--rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/six.py
--rw-r--r--   0        0        0    80114 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/vendor.txt
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
--rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
--rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
--rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
--rw-r--r--   0        0        0   286370 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/certifi/core.py
--rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
--rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
--rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
--rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
--rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
--rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
--rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
--rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
--rw-r--r--   0        0        0    13919 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
--rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
--rw-r--r--   0        0        0    26797 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
--rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
--rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
--rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
--rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
--rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
--rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
--rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
--rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
--rw-r--r--   0        0        0    30068 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
--rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
--rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
--rw-r--r--   0        0        0    13280 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
--rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
--rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
--rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/database.py
--rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/index.py
--rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
--rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
--rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
--rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
--rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
--rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/t32.exe
--rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
--rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/t64.exe
--rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/util.py
--rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/version.py
--rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/w32.exe
--rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
--rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/w64.exe
--rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
--rw-r--r--   0        0        0    48841 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distro/distro.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/codec.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/compat.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/core.py
--rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
--rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
--rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
--rw-r--r--   0        0        0    34557 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/version.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/__init__.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/_compat.py
--rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/build.py
--rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/check.py
--rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/meta.py
--rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py
--rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py
--rw-r--r--   0        0        0   108287 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
--rw-r--r--   0        0        0    12831 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
--rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
--rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
--rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
--rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/console.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
--rw-r--r--   0        0        0    32005 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
--rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/style.py
--rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/token.py
--rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
--rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/util.py
--rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
--rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
--rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
--rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
--rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
--rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
--rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
--rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
--rw-r--r--   0        0        0    70232 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
--rw-r--r--   0        0        0    53376 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
--rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
--rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
--rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/api.py
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/auth.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/certs.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/compat.py
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
--rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/help.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
--rw-r--r--   0        0        0    35287 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/models.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/packages.py
--rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/structures.py
--rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/utils.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
--rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
--rw-r--r--   0        0        0    17592 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
--rw-r--r--   0        0        0     5944 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
--rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
--rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
--rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
--rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
--rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
--rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/abc.py
--rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/align.py
--rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
--rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/bar.py
--rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/box.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/cells.py
--rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/color.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/columns.py
--rw-r--r--   0        0        0    95885 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/console.py
--rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
--rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/containers.py
--rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/control.py
--rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/errors.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/json.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
--rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/layout.py
--rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/live.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
--rw-r--r--   0        0        0    11471 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/logging.py
--rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/markup.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/measure.py
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/padding.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/pager.py
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/palette.py
--rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/panel.py
--rw-r--r--   0        0        0    36576 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
--rw-r--r--   0        0        0    59746 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/progress.py
--rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
--rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/region.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/repr.py
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/rule.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/scope.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/screen.py
--rw-r--r--   0        0        0    24224 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/segment.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/status.py
--rw-r--r--   0        0        0    26240 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/style.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/styled.py
--rw-r--r--   0        0        0    34697 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
--rw-r--r--   0        0        0    39515 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/table.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
--rw-r--r--   0        0        0    44666 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/text.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/theme.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/themes.py
--rw-r--r--   0        0        0    26060 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
--rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/tree.py
--rw-r--r--   0        0        0    18364 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
--rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
--rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
--rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
--rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
--rw-r--r--   0        0        0    39093 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
--rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
--rw-r--r--   0        0        0    30109 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
--rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
--rw-r--r--   0        0        0    17182 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
--rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
--rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
--rw-r--r--   0        0        0    22001 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
--rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
--rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
--rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip-22.3.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip-22.3.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip-22.3.1.dist-info/METADATA
--rw-r--r--   0        0        0    71279 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip-22.3.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip-22.3.1.dist-info/WHEEL
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip-22.3.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pip-22.3.1.dist-info/top_level.txt
--rw-r--r--   0        0        0   108568 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
--rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   132569 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    18410 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/extern/__init__.py
--rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_deprecation_warning.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_entry_points.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_imp.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_importlib.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_itertools.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_path.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_reqs.py
--rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/archive_util.py
--rw-r--r--   0        0        0    19539 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/build_meta.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/cli-32.exe
--rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/cli-64.exe
--rwxr-xr-x   0        0        0   137216 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/cli-arm64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/cli.exe
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/dep_util.py
--rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/depends.py
--rw-r--r--   0        0        0    20799 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/discovery.py
--rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/dist.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/errors.py
--rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/extension.py
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/glob.py
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/gui-32.exe
--rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/gui-64.exe
--rwxr-xr-x   0        0        0   137728 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/gui-arm64.exe
--rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/gui.exe
--rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/installer.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/launch.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/logging.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/monkey.py
--rw-r--r--   0        0        0    47724 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/msvc.py
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/namespaces.py
--rw-r--r--   0        0        0    40329 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/package_index.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/py34compat.py
--rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/sandbox.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/script (dev).tmpl
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/script.tmpl
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/unicode_utils.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/version.py
--rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/wheel.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/windows_support.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/__init__.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/_collections.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/_functools.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
--rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
--rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
--rw-r--r--   0        0        0    14789 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
--rw-r--r--   0        0        0    47369 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
--rw-r--r--   0        0        0    17973 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/cmd.py
--rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/config.py
--rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/core.py
--rw-r--r--   0        0        0    12537 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/debug.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
--rw-r--r--   0        0        0    50186 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/dist.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/errors.py
--rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/extension.py
--rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
--rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/file_util.py
--rw-r--r--   0        0        0    13713 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/filelist.py
--rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/log.py
--rw-r--r--   0        0        0    30235 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
--rw-r--r--   0        0        0    23602 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/spawn.py
--rw-r--r--   0        0        0    18858 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
--rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/text_file.py
--rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
--rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/util.py
--rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/version.py
--rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
--rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
--rw-r--r--   0        0        0    22051 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
--rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/build.py
--rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
--rw-r--r--   0        0        0    31558 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
--rw-r--r--   0        0        0    16568 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
--rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/check.py
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
--rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/config.py
--rw-r--r--   0        0        0    30221 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
--rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
--rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
--rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/register.py
--rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/__init__.py
--rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
--rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
--rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/zipp.py
--rw-r--r--   0        0        0    30130 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
--rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
--rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
--rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
--rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
--rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
--rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
--rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
--rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
--rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
--rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
--rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
--rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
--rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
--rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/__init__.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/alias.py
--rw-r--r--   0        0        0    16623 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/bdist_egg.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
--rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/build.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/build_clib.py
--rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/build_ext.py
--rw-r--r--   0        0        0    14115 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/build_py.py
--rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/develop.py
--rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/dist_info.py
--rw-r--r--   0        0        0    85662 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/easy_install.py
--rw-r--r--   0        0        0    31188 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/editable_wheel.py
--rw-r--r--   0        0        0    26795 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/egg_info.py
--rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/install.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/install_egg_info.py
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/install_lib.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/install_scripts.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/launcher manifest.xml
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/py36compat.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/register.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/rotate.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/saveopts.py
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/sdist.py
--rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/setopt.py
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/test.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/upload.py
--rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/upload_docs.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/__init__.py
--rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
--rw-r--r--   0        0        0    16319 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/expand.py
--rw-r--r--   0        0        0    19304 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
--rw-r--r--   0        0        0    25198 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/setupcfg.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
--rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
--rw-r--r--   0        0        0   269900 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
--rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools/extern/__init__.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/LICENSE
--rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/METADATA
--rw-r--r--   0        0        0    35656 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/WHEEL
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/top_level.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/__init__.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/__main__.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/_setuptools_logging.py
--rw-r--r--   0        0        0    19293 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/bdist_wheel.py
--rw-r--r--   0        0        0    16145 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/macosx_libfile.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/metadata.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/util.py
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/wheelfile.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/cli/__init__.py
--rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/cli/convert.py
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/cli/pack.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/cli/unpack.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/vendored/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
--rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py
--rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py
--rw-r--r--   0        0        0    15612 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/INSTALLER
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/METADATA
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/RECORD
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/WHEEL
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/entry_points.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/top_level.txt
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/Activate.ps1
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/activate
--rwxr-xr-x   0        0        0     1029 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/activate.bat
--rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/activate.fish
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/activate.nu
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/activate_this.py
--rwxr-xr-x   0        0        0      511 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/deactivate.bat
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/deactivate.nu
--rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/pip-3.10.exe
--rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/pip.exe
--rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/pip3.10.exe
--rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/pip3.exe
--rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/pydoc.bat
--rwxr-xr-x   0        0        0   268568 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/python.exe
--rwxr-xr-x   0        0        0   257304 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/pythonw.exe
--rwxr-xr-x   0        0        0   108418 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/wheel-3.10.exe
--rwxr-xr-x   0        0        0   108418 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/wheel.exe
--rwxr-xr-x   0        0        0   108418 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/wheel3.10.exe
--rwxr-xr-x   0        0        0   108418 2020-02-02 00:00:00.000000 codeoffer-0.8.0/venv/Scripts/wheel3.exe
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 codeoffer-0.8.0/LICENSE
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 codeoffer-0.8.0/README.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 codeoffer-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 codeoffer-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 codeoffer-0.9.0/.idea/.gitignore
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 codeoffer-0.9.0/.idea/misc.xml
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 codeoffer-0.9.0/.idea/modules.xml
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 codeoffer-0.9.0/.idea/v1-python-library.iml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 codeoffer-0.9.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 codeoffer-0.9.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 codeoffer-0.9.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/src/codeoffer/__init__.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 codeoffer-0.9.0/src/codeoffer/api.py
+-rw-r--r--   0        0        0     2107 2020-02-02 00:00:00.000000 codeoffer-0.9.0/src/codeoffer/app.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 codeoffer-0.9.0/src/codeoffer/exceptions.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 codeoffer-0.9.0/src/codeoffer/oauth.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 codeoffer-0.9.0/src/codeoffer/user.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 codeoffer-0.9.0/src/codeoffer/utilities.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/.gitignore
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/pyvenv.cfg
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/_virtualenv.pth
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/_virtualenv.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/distutils-precedence.pth
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip-22.3.1.virtualenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.virtualenv
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel-0.38.4.virtualenv
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/_distutils_hack/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/_distutils_hack/override.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/__init__.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/__main__.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/__pip-runner__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/py.typed
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/__init__.py
+-rw-r--r--   0        0        0    10234 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/build_env.py
+-rw-r--r--   0        0        0    10734 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cache.py
+-rw-r--r--   0        0        0    13529 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/configuration.py
+-rw-r--r--   0        0        0    20942 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/exceptions.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/main.py
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/pyproject.py
+-rw-r--r--   0        0        0     8020 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/self_outdated_check.py
+-rw-r--r--   0        0        0    13079 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/wheel_builder.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/__init__.py
+-rw-r--r--   0        0        0     6676 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py
+-rw-r--r--   0        0        0     7842 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/base_command.py
+-rw-r--r--   0        0        0    29381 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/command_context.py
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/main.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/main_parser.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/parser.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py
+-rw-r--r--   0        0        0    18172 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/req_command.py
+-rw-r--r--   0        0        0     5118 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/spinners.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/status_codes.py
+-rw-r--r--   0        0        0     3882 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     7582 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/cache.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/check.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/completion.py
+-rw-r--r--   0        0        0     9815 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/configuration.py
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/debug.py
+-rw-r--r--   0        0        0     5289 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/download.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/freeze.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/hash.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/help.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/index.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/inspect.py
+-rw-r--r--   0        0        0    31726 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/install.py
+-rw-r--r--   0        0        0    12343 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/list.py
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/search.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/show.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/uninstall.py
+-rw-r--r--   0        0        0     7396 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/wheel.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/distributions/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/distributions/base.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/distributions/installed.py
+-rw-r--r--   0        0        0     6494 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/distributions/sdist.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/distributions/wheel.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/index/__init__.py
+-rw-r--r--   0        0        0    16503 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/index/collector.py
+-rw-r--r--   0        0        0    37596 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/index/package_finder.py
+-rw-r--r--   0        0        0     6557 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/index/sources.py
+-rw-r--r--   0        0        0    17552 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/locations/__init__.py
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/locations/_distutils.py
+-rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/locations/base.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/__init__.py
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/_json.py
+-rw-r--r--   0        0        0    25277 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/base.py
+-rw-r--r--   0        0        0     9773 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/__init__.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py
+-rw-r--r--   0        0        0     7457 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/__init__.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/candidate.py
+-rw-r--r--   0        0        0     5877 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/direct_url.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/format_control.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/index.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/installation_report.py
+-rw-r--r--   0        0        0    18083 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/link.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/scheme.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/search_scope.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/target_python.py
+-rw-r--r--   0        0        0     3600 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/wheel.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/__init__.py
+-rw-r--r--   0        0        0    12190 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/auth.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/cache.py
+-rw-r--r--   0        0        0     6096 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/download.py
+-rw-r--r--   0        0        0     7638 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py
+-rw-r--r--   0        0        0    18443 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/session.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/utils.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/__init__.py
+-rw-r--r--   0        0        0     5109 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/check.py
+-rw-r--r--   0        0        0     9784 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/freeze.py
+-rw-r--r--   0        0        0    25091 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/prepare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/__init__.py
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/install/__init__.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py
+-rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py
+-rw-r--r--   0        0        0    27407 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/__init__.py
+-rw-r--r--   0        0        0    16611 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/constructors.py
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/req_file.py
+-rw-r--r--   0        0        0    35600 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/req_install.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/req_set.py
+-rw-r--r--   0        0        0    24045 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/__init__.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/__init__.py
+-rw-r--r--   0        0        0    24129 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py
+-rw-r--r--   0        0        0    18963 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py
+-rw-r--r--   0        0        0    27878 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py
+-rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py
+-rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/_log.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/appdirs.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/compat.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/datetime.py
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/deprecation.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/egg_link.py
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/encoding.py
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py
+-rw-r--r--   0        0        0     5122 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/filesystem.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/filetypes.py
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/glibc.py
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/hashes.py
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py
+-rw-r--r--   0        0        0    11632 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/logging.py
+-rw-r--r--   0        0        0    21617 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/misc.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/models.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/packaging.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py
+-rw-r--r--   0        0        0     9197 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/subprocess.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py
+-rw-r--r--   0        0        0     8821 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/unpacking.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/urls.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py
+-rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/wheel.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/__init__.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py
+-rw-r--r--   0        0        0    18116 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/git.py
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py
+-rw-r--r--   0        0        0    11728 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/subversion.py
+-rw-r--r--   0        0        0    22811 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/__init__.py
+-rw-r--r--   0        0        0    34549 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/six.py
+-rw-r--r--   0        0        0    80114 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/vendor.txt
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py
+-rw-r--r--   0        0        0    16416 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py
+-rw-r--r--   0        0        0     4154 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/__init__.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/certifi/__init__.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/certifi/__main__.py
+-rw-r--r--   0        0        0   286370 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/certifi/core.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py
+-rw-r--r--   0        0        0    31274 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py
+-rw-r--r--   0        0        0     9608 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py
+-rw-r--r--   0        0        0     4801 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/enums.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py
+-rw-r--r--   0        0        0    12021 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py
+-rw-r--r--   0        0        0    13566 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py
+-rw-r--r--   0        0        0    36913 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py
+-rw-r--r--   0        0        0    20735 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py
+-rw-r--r--   0        0        0    13919 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py
+-rw-r--r--   0        0        0    25796 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py
+-rw-r--r--   0        0        0    26797 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py
+-rw-r--r--   0        0        0   104562 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py
+-rw-r--r--   0        0        0    98484 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py
+-rw-r--r--   0        0        0    98196 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py
+-rw-r--r--   0        0        0   101363 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py
+-rw-r--r--   0        0        0   128035 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py
+-rw-r--r--   0        0        0   102774 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py
+-rw-r--r--   0        0        0    95372 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py
+-rw-r--r--   0        0        0     5260 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py
+-rw-r--r--   0        0        0    30068 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py
+-rw-r--r--   0        0        0     6199 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py
+-rw-r--r--   0        0        0    13288 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/__init__.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/__init__.py
+-rw-r--r--   0        0        0    13280 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py
+-rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/colorama/win32.py
+-rw-r--r--   0        0        0     6438 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py
+-rw-r--r--   0        0        0    41259 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/compat.py
+-rw-r--r--   0        0        0    51697 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/database.py
+-rw-r--r--   0        0        0    20834 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/index.py
+-rw-r--r--   0        0        0    51991 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/locators.py
+-rw-r--r--   0        0        0    14811 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/markers.py
+-rw-r--r--   0        0        0    39801 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py
+-rw-r--r--   0        0        0    10820 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/resources.py
+-rw-r--r--   0        0        0    18102 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py
+-rwxr-xr-x   0        0        0    97792 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/t32.exe
+-rwxr-xr-x   0        0        0   182784 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe
+-rwxr-xr-x   0        0        0   108032 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/t64.exe
+-rw-r--r--   0        0        0    66262 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/util.py
+-rw-r--r--   0        0        0    23513 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/version.py
+-rwxr-xr-x   0        0        0    91648 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/w32.exe
+-rwxr-xr-x   0        0        0   168448 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe
+-rwxr-xr-x   0        0        0   101888 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/w64.exe
+-rw-r--r--   0        0        0    43898 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distro/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distro/__main__.py
+-rw-r--r--   0        0        0    48841 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distro/distro.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/__init__.py
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/codec.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/compat.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/core.py
+-rw-r--r--   0        0        0    44375 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/intranges.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/package_data.py
+-rw-r--r--   0        0        0   206539 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py
+-rw-r--r--   0        0        0    34557 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/__init__.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/_compat.py
+-rw-r--r--   0        0        0     3443 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/build.py
+-rw-r--r--   0        0        0     6083 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/check.py
+-rw-r--r--   0        0        0     3994 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py
+-rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/meta.py
+-rw-r--r--   0        0        0    12721 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py
+-rw-r--r--   0        0        0    10801 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py
+-rw-r--r--   0        0        0   108287 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py
+-rw-r--r--   0        0        0    12831 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py
+-rw-r--r--   0        0        0     2655 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py
+-rw-r--r--   0        0        0     6910 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/version.py
+-rw-r--r--   0        0        0     6439 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/__main__.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/console.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/filter.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py
+-rw-r--r--   0        0        0    32005 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/style.py
+-rw-r--r--   0        0        0     6184 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/token.py
+-rw-r--r--   0        0        0    63187 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py
+-rw-r--r--   0        0        0     9110 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/util.py
+-rw-r--r--   0        0        0    40386 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py
+-rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py
+-rw-r--r--   0        0        0    35441 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py
+-rw-r--r--   0        0        0    21938 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py
+-rw-r--r--   0        0        0     5871 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py
+-rw-r--r--   0        0        0    19351 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py
+-rw-r--r--   0        0        0     7335 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py
+-rw-r--r--   0        0        0    11753 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py
+-rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py
+-rw-r--r--   0        0        0    70232 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py
+-rw-r--r--   0        0        0    53376 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py
+-rw-r--r--   0        0        0     9171 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213344 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23685 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0     5178 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/__version__.py
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py
+-rw-r--r--   0        0        0    21443 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/adapters.py
+-rw-r--r--   0        0        0     6377 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/api.py
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/auth.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/certs.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/compat.py
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/cookies.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/help.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/hooks.py
+-rw-r--r--   0        0        0    35287 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/models.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/packages.py
+-rw-r--r--   0        0        0    30180 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/sessions.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/structures.py
+-rw-r--r--   0        0        0    33240 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/utils.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py
+-rw-r--r--   0        0        0    17592 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/__init__.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/compat/collections_abc.py
+-rw-r--r--   0        0        0     5944 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/__init__.py
+-rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/__main__.py
+-rw-r--r--   0        0        0    10096 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py
+-rw-r--r--   0        0        0   140235 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_extension.py
+-rw-r--r--   0        0        0     9695 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_loop.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_pick.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py
+-rw-r--r--   0        0        0    19919 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_stack.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_timer.py
+-rw-r--r--   0        0        0    22820 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_windows.py
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/abc.py
+-rw-r--r--   0        0        0    10368 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/align.py
+-rw-r--r--   0        0        0     6820 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/ansi.py
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/bar.py
+-rw-r--r--   0        0        0     9864 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/box.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/cells.py
+-rw-r--r--   0        0        0    17957 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/color.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/columns.py
+-rw-r--r--   0        0        0    95885 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/console.py
+-rw-r--r--   0        0        0     1288 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/constrain.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/containers.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/control.py
+-rw-r--r--   0        0        0     7954 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/emoji.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/errors.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/filesize.py
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/json.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py
+-rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/layout.py
+-rw-r--r--   0        0        0    14172 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/live.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/live_render.py
+-rw-r--r--   0        0        0    11471 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/logging.py
+-rw-r--r--   0        0        0     8198 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/markup.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/measure.py
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/padding.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/pager.py
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/palette.py
+-rw-r--r--   0        0        0     8744 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/panel.py
+-rw-r--r--   0        0        0    36576 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/pretty.py
+-rw-r--r--   0        0        0    59746 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/progress.py
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py
+-rw-r--r--   0        0        0    11303 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/prompt.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/protocol.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/region.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/repr.py
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/rule.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/scope.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/screen.py
+-rw-r--r--   0        0        0    24224 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/segment.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/spinner.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/status.py
+-rw-r--r--   0        0        0    26240 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/style.py
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/styled.py
+-rw-r--r--   0        0        0    34697 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/syntax.py
+-rw-r--r--   0        0        0    39515 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/table.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py
+-rw-r--r--   0        0        0    44666 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/text.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/theme.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/themes.py
+-rw-r--r--   0        0        0    26060 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/traceback.py
+-rw-r--r--   0        0        0     9169 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/tree.py
+-rw-r--r--   0        0        0    18364 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py
+-rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/after.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/before.py
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py
+-rw-r--r--   0        0        0     7550 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py
+-rw-r--r--   0        0        0     8011 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py
+-rw-r--r--   0        0        0    10811 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/_version.py
+-rw-r--r--   0        0        0    20070 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py
+-rw-r--r--   0        0        0    39093 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py
+-rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py
+-rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py
+-rw-r--r--   0        0        0     5985 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/request.py
+-rw-r--r--   0        0        0    30109 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/response.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py
+-rw-r--r--   0        0        0    11034 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py
+-rw-r--r--   0        0        0    17182 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34448 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    17632 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    13922 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/__init__.py
+-rw-r--r--   0        0        0    34665 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/queue.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py
+-rw-r--r--   0        0        0    22001 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py
+-rw-r--r--   0        0        0    17177 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5758 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     6895 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10003 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10579 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py
+-rw-r--r--   0        0        0     4307 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip-22.3.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip-22.3.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip-22.3.1.dist-info/METADATA
+-rw-r--r--   0        0        0    71279 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip-22.3.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip-22.3.1.dist-info/WHEEL
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip-22.3.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pip-22.3.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0   108568 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/__init__.py
+-rw-r--r--   0        0        0    24701 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    13515 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15526 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   132569 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    18410 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8496 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4706 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/extern/__init__.py
+-rw-r--r--   0        0        0     8429 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_deprecation_warning.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_entry_points.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_imp.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_importlib.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_itertools.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_path.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_reqs.py
+-rw-r--r--   0        0        0     7346 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/archive_util.py
+-rw-r--r--   0        0        0    19539 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/build_meta.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/cli-32.exe
+-rwxr-xr-x   0        0        0    74752 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/cli-64.exe
+-rwxr-xr-x   0        0        0   137216 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/cli-arm64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/cli.exe
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/dep_util.py
+-rw-r--r--   0        0        0     5499 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/depends.py
+-rw-r--r--   0        0        0    20799 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/discovery.py
+-rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/dist.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/errors.py
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/extension.py
+-rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/glob.py
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/gui-32.exe
+-rwxr-xr-x   0        0        0    75264 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/gui-64.exe
+-rwxr-xr-x   0        0        0   137728 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/gui-arm64.exe
+-rwxr-xr-x   0        0        0    65536 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/gui.exe
+-rw-r--r--   0        0        0     3824 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/installer.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/launch.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/logging.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/monkey.py
+-rw-r--r--   0        0        0    47724 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/msvc.py
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/namespaces.py
+-rw-r--r--   0        0        0    40329 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/package_index.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/py34compat.py
+-rw-r--r--   0        0        0    14348 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/sandbox.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/script (dev).tmpl
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/script.tmpl
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/unicode_utils.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/version.py
+-rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/wheel.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/windows_support.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/__init__.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/_collections.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/_functools.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/_macos_compat.py
+-rw-r--r--   0        0        0    19672 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py
+-rw-r--r--   0        0        0     8603 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/archive_util.py
+-rw-r--r--   0        0        0    14789 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py
+-rw-r--r--   0        0        0    47369 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py
+-rw-r--r--   0        0        0    17973 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/cmd.py
+-rw-r--r--   0        0        0     4920 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/config.py
+-rw-r--r--   0        0        0     9451 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/core.py
+-rw-r--r--   0        0        0    12537 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/debug.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/dep_util.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/dir_util.py
+-rw-r--r--   0        0        0    50186 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/dist.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/errors.py
+-rw-r--r--   0        0        0    10270 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/extension.py
+-rw-r--r--   0        0        0    17910 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py
+-rw-r--r--   0        0        0     8226 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/file_util.py
+-rw-r--r--   0        0        0    13713 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/filelist.py
+-rw-r--r--   0        0        0     1972 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/log.py
+-rw-r--r--   0        0        0    30235 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py
+-rw-r--r--   0        0        0    23602 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/py38compat.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/py39compat.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/spawn.py
+-rw-r--r--   0        0        0    18858 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py
+-rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/text_file.py
+-rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py
+-rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/util.py
+-rw-r--r--   0        0        0    12952 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/version.py
+-rw-r--r--   0        0        0     5248 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/__init__.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py
+-rw-r--r--   0        0        0     5441 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py
+-rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py
+-rw-r--r--   0        0        0    22051 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/build.py
+-rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py
+-rw-r--r--   0        0        0    31558 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py
+-rw-r--r--   0        0        0    16568 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py
+-rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/check.py
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/clean.py
+-rw-r--r--   0        0        0    13137 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/config.py
+-rw-r--r--   0        0        0    30221 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install.py
+-rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py
+-rw-r--r--   0        0        0    11765 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/register.py
+-rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/__init__.py
+-rw-r--r--   0        0        0    15130 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py
+-rw-r--r--   0        0        0    87149 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py
+-rw-r--r--   0        0        0     8425 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/zipp.py
+-rw-r--r--   0        0        0    30130 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/__init__.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/__init__.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py
+-rw-r--r--   0        0        0    13512 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py
+-rw-r--r--   0        0        0    15517 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/__init__.py
+-rw-r--r--   0        0        0   117959 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py
+-rw-r--r--   0        0        0    16256 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0    11488 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4378 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     8493 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0     4700 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    30110 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    15699 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py
+-rw-r--r--   0        0        0     6426 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py
+-rw-r--r--   0        0        0    12936 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py
+-rw-r--r--   0        0        0   213310 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py
+-rw-r--r--   0        0        0    39129 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py
+-rw-r--r--   0        0        0    25341 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py
+-rw-r--r--   0        0        0    13402 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py
+-rw-r--r--   0        0        0    10787 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py
+-rw-r--r--   0        0        0    23668 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/alias.py
+-rw-r--r--   0        0        0    16623 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/bdist_egg.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/bdist_rpm.py
+-rw-r--r--   0        0        0     6589 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/build.py
+-rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/build_clib.py
+-rw-r--r--   0        0        0    15821 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/build_ext.py
+-rw-r--r--   0        0        0    14115 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/build_py.py
+-rw-r--r--   0        0        0     7012 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/develop.py
+-rw-r--r--   0        0        0     4800 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/dist_info.py
+-rw-r--r--   0        0        0    85662 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/easy_install.py
+-rw-r--r--   0        0        0    31188 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/editable_wheel.py
+-rw-r--r--   0        0        0    26795 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/egg_info.py
+-rw-r--r--   0        0        0     5163 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/install.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/install_egg_info.py
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/install_lib.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/install_scripts.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/launcher manifest.xml
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/py36compat.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/register.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/rotate.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/saveopts.py
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/sdist.py
+-rw-r--r--   0        0        0     5086 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/setopt.py
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/test.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/upload.py
+-rw-r--r--   0        0        0     7494 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/upload_docs.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/__init__.py
+-rw-r--r--   0        0        0    13398 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py
+-rw-r--r--   0        0        0    16319 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/expand.py
+-rw-r--r--   0        0        0    19304 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py
+-rw-r--r--   0        0        0    25198 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/setupcfg.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py
+-rw-r--r--   0        0        0    11266 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py
+-rw-r--r--   0        0        0   269900 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py
+-rw-r--r--   0        0        0     8736 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools/extern/__init__.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/LICENSE
+-rw-r--r--   0        0        0     6311 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/METADATA
+-rw-r--r--   0        0        0    35656 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/__init__.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/__main__.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/_setuptools_logging.py
+-rw-r--r--   0        0        0    19293 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/bdist_wheel.py
+-rw-r--r--   0        0        0    16145 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/macosx_libfile.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/metadata.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/util.py
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/wheelfile.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/cli/__init__.py
+-rw-r--r--   0        0        0     9427 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/cli/convert.py
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/cli/pack.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/cli/unpack.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/vendored/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/vendored/packaging/__init__.py
+-rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py
+-rw-r--r--   0        0        0    15612 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel/vendored/packaging/tags.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/METADATA
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/RECORD
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/WHEEL
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/entry_points.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/top_level.txt
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/Activate.ps1
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/activate
+-rwxr-xr-x   0        0        0     1029 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/activate.bat
+-rw-r--r--   0        0        0     3053 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/activate.fish
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/activate.nu
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/activate_this.py
+-rwxr-xr-x   0        0        0      511 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/deactivate.bat
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/deactivate.nu
+-rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/pip-3.10.exe
+-rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/pip.exe
+-rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/pip3.10.exe
+-rwxr-xr-x   0        0        0   108431 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/pip3.exe
+-rwxr-xr-x   0        0        0       24 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/pydoc.bat
+-rwxr-xr-x   0        0        0   268568 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/python.exe
+-rwxr-xr-x   0        0        0   257304 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/pythonw.exe
+-rwxr-xr-x   0        0        0   108418 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/wheel-3.10.exe
+-rwxr-xr-x   0        0        0   108418 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/wheel.exe
+-rwxr-xr-x   0        0        0   108418 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/wheel3.10.exe
+-rwxr-xr-x   0        0        0   108418 2020-02-02 00:00:00.000000 codeoffer-0.9.0/venv/Scripts/wheel3.exe
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 codeoffer-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 codeoffer-0.9.0/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 codeoffer-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 codeoffer-0.9.0/PKG-INFO
```

### Comparing `codeoffer-0.8.0/codeoffer/api.py` & `codeoffer-0.9.0/src/codeoffer/api.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/codeoffer/app.py` & `codeoffer-0.9.0/src/codeoffer/app.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/codeoffer/exceptions.py` & `codeoffer-0.9.0/src/codeoffer/exceptions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/codeoffer/oauth.py` & `codeoffer-0.9.0/src/codeoffer/oauth.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/codeoffer/user.py` & `codeoffer-0.9.0/src/codeoffer/user.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/codeoffer/utilities.py` & `codeoffer-0.9.0/src/codeoffer/utilities.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/_virtualenv.py` & `codeoffer-0.9.0/venv/Lib/site-packages/_virtualenv.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/_distutils_hack/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/_distutils_hack/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/__main__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/__main__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/__pip-runner__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/__pip-runner__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/build_env.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/build_env.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cache.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cache.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/configuration.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/configuration.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/exceptions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/pyproject.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/pyproject.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/self_outdated_check.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/self_outdated_check.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/wheel_builder.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/wheel_builder.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/autocompletion.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/base_command.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/base_command.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/cmdoptions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/command_context.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/command_context.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/main.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/main_parser.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/main_parser.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/parser.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/parser.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/progress_bars.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/req_command.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/req_command.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/cli/spinners.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/cli/spinners.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/cache.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/cache.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/check.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/check.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/completion.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/completion.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/configuration.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/configuration.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/debug.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/debug.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/download.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/download.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/freeze.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/freeze.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/hash.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/hash.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/help.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/help.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/index.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/index.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/inspect.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/install.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/install.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/list.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/list.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/search.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/search.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/show.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/show.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/uninstall.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/commands/wheel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/commands/wheel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/distributions/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/distributions/base.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/distributions/base.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/distributions/installed.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/distributions/installed.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/distributions/sdist.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/distributions/sdist.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/distributions/wheel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/distributions/wheel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/index/collector.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/index/collector.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/index/package_finder.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/index/package_finder.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/index/sources.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/index/sources.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/locations/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/locations/_distutils.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/locations/_distutils.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/locations/_sysconfig.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/locations/base.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/locations/base.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/_json.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/_json.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/base.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/base.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_dists.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/metadata/importlib/_envs.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/candidate.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/candidate.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/direct_url.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/direct_url.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/format_control.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/format_control.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/index.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/index.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/installation_report.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/installation_report.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/link.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/link.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/scheme.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/scheme.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/search_scope.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/search_scope.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/selection_prefs.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/target_python.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/target_python.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/models/wheel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/models/wheel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/auth.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/auth.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/cache.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/cache.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/download.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/download.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/lazy_wheel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/session.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/session.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/utils.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/utils.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/network/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/check.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/check.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/freeze.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/freeze.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/prepare.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/prepare.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/build_tracker.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_editable.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/metadata_legacy.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_editable.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/build/wheel_legacy.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/install/editable_legacy.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/install/legacy.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/operations/install/wheel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/constructors.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/constructors.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/req_file.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/req_file.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/req_install.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/req_install.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/req_set.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/req_set.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/req/req_uninstall.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/base.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/base.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/legacy/resolver.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/base.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/candidates.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/factory.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/found_candidates.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/provider.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/reporter.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/requirements.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/resolution/resolvelib/resolver.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/_log.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/_log.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/appdirs.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/appdirs.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/deprecation.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/direct_url_helpers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/distutils_args.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/egg_link.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/egg_link.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/encoding.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/entrypoints.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/filesystem.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/filetypes.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/filetypes.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/glibc.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/glibc.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/hashes.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/inject_securetransport.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/logging.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/logging.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/misc.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/models.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/models.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/packaging.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/packaging.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/setuptools_build.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/subprocess.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/temp_dir.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/unpacking.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/unpacking.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/urls.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/urls.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/virtualenv.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/utils/wheel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/git.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/git.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/mercurial.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/subversion.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/subversion.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_internal/vcs/versioncontrol.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/six.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/six.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/typing_extensions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/_cmd.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/adapter.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/cache.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/controller.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/filewrapper.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/heuristics.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/serialize.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/wrapper.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/file_cache.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/cachecontrol/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/certifi/cacert.pem`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/certifi/core.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/certifi/core.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/big5freq.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/big5prober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/chardistribution.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetgroupprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/charsetprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/codingstatemachine.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/cp949prober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/enums.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/enums.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/escprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/escsm.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/eucjpprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrfreq.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/euckrprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwfreq.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/euctwprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312freq.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/gb2312prober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/hebrewprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/jisfreq.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/johabfreq.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/johabprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/jpcntx.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langbulgarianmodel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langgreekmodel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langhebrewmodel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langhungarianmodel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langrussianmodel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langthaimodel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/langturkishmodel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/latin1prober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/mbcssm.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcharsetprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/sbcsgroupprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/sjisprober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/universaldetector.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/utf1632prober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/utf8prober.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/cli/chardetect.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/chardet/metadata/languages.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/colorama/win32.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/database.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/database.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/index.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/index.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/locators.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/locators.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/manifest.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/markers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/markers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/metadata.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/resources.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/resources.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/scripts.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/t32.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/t32.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/t64-arm.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/t64.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/t64.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/version.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/version.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/w32.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/w32.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/w64-arm.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/w64.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/w64.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distlib/wheel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distro/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distro/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/distro/distro.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/distro/distro.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/codec.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/codec.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/core.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/core.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/idnadata.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/intranges.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/intranges.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/idna/uts46data.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/msgpack/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/msgpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/msgpack/ext.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/msgpack/fallback.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/markers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/tags.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/utils.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/packaging/version.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/build.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/build.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/check.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/check.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/colorlog.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/dirtools.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/envbuild.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/meta.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/meta.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/wrappers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pep517/in_process/_in_process.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pkg_resources/py31compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/cmdline.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/console.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/console.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/filter.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/filter.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatter.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/modeline.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/plugin.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/regexopt.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/scanner.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/sphinxext.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/style.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/style.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/token.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/token.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/unistring.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/_mapping.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/bbcode.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/groff.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/html.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/img.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/irc.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/latex.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/other.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/pangomarkup.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/rtf.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/svg.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/formatters/terminal256.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/_mapping.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/lexers/python.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pygments/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/adapters.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/adapters.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/api.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/api.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/auth.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/auth.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/certs.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/certs.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/cookies.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/cookies.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/help.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/help.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/hooks.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/hooks.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/models.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/models.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/packages.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/packages.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/sessions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/sessions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/status_codes.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/structures.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/structures.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/requests/utils.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/requests/utils.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/providers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/reporters.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/resolvers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/resolvelib/structs.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/__main__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/__main__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_cell_widths.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_codes.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_emoji_replace.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_export_format.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_inspect.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_log_render.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_loop.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_loop.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_palettes.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_ratio.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_spinners.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_win32_console.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_windows.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_windows.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_windows_renderer.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/_wrap.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/abc.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/abc.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/align.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/align.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/ansi.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/ansi.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/bar.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/bar.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/box.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/box.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/cells.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/cells.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/color.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/color.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/color_triplet.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/columns.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/columns.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/console.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/console.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/constrain.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/constrain.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/containers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/containers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/control.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/control.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/default_styles.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/diagnose.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/emoji.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/emoji.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/errors.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/errors.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/file_proxy.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/filesize.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/filesize.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/highlighter.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/json.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/json.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/jupyter.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/layout.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/layout.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/live.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/live.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/live_render.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/live_render.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/logging.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/logging.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/markup.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/markup.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/measure.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/measure.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/padding.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/padding.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/pager.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/pager.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/palette.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/palette.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/panel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/panel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/pretty.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/pretty.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/progress.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/progress.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/prompt.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/prompt.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/protocol.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/protocol.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/repr.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/repr.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/rule.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/rule.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/scope.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/scope.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/screen.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/screen.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/segment.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/segment.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/spinner.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/spinner.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/status.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/status.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/style.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/style.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/styled.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/styled.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/syntax.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/syntax.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/table.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/table.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/terminal_theme.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/text.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/text.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/theme.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/theme.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/traceback.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/traceback.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/rich/tree.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/rich/tree.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/_asyncio.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/_utils.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/after.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/after.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/before.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/before.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/before_sleep.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/nap.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/retry.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/stop.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/tornadoweb.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tenacity/wait.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/tomli/_re.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/connection.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/exceptions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/poolmanager.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/request.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/request.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/response.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/response.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_appengine_environ.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/appengine.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/ntlmpool.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/six.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/packages/backports/makefile.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/retry.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/webencodings/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/webencodings/labels.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/webencodings/mklabels.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/webencodings/tests.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pip/_vendor/webencodings/x_user_defined.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip-22.3.1.dist-info/LICENSE.txt` & `codeoffer-0.9.0/venv/Lib/site-packages/pip-22.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip-22.3.1.dist-info/METADATA` & `codeoffer-0.9.0/venv/Lib/site-packages/pip-22.3.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pip-22.3.1.dist-info/RECORD` & `codeoffer-0.9.0/venv/Lib/site-packages/pip-22.3.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/appdirs.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/pkg_resources/extern/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/pkg_resources/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_entry_points.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_entry_points.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_imp.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_imp.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_importlib.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_importlib.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_itertools.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_itertools.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_path.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_path.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/archive_util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/archive_util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/build_meta.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/cli-32.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/cli-32.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/cli-64.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/cli-64.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/cli-arm64.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/cli-arm64.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/cli.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/cli.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/dep_util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/dep_util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/depends.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/depends.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/discovery.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/discovery.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/dist.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/dist.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/errors.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/errors.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/extension.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/glob.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/glob.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/gui-32.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/gui-32.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/gui-64.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/gui-64.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/gui-arm64.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/gui-arm64.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/gui.exe` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/gui.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/installer.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/installer.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/launch.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/launch.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/logging.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/logging.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/monkey.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/monkey.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/msvc.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/msvc.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/namespaces.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/namespaces.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/package_index.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/package_index.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/sandbox.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/sandbox.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/unicode_utils.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/unicode_utils.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/wheel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/wheel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/windows_support.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/windows_support.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/_collections.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/_collections.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/_msvccompiler.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/archive_util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/archive_util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/bcppcompiler.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/ccompiler.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/cmd.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/cmd.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/config.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/config.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/core.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/core.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/cygwinccompiler.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/dep_util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/dep_util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/dir_util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/dir_util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/dist.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/dist.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/errors.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/errors.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/extension.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/extension.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/fancy_getopt.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/file_util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/file_util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/filelist.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/filelist.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/log.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/log.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/msvc9compiler.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/msvccompiler.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/py39compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/py39compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/spawn.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/spawn.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/sysconfig.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/text_file.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/text_file.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/unixccompiler.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/version.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/version.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/versionpredicate.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/_framework_compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_dumb.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/build.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/build.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/build_py.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/build_scripts.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/check.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/check.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/clean.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/clean.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/config.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/config.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install_data.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install_headers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/py37compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/register.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/register.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/sdist.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_distutils/command/upload.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_distutils/command/upload.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/ordered_set.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/typing_extensions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/zipp.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/zipp.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_adapters.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_common.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_itertools.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/_legacy.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/abc.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/readers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/importlib_resources/simple.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/context.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/functools.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/jaraco/text/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/more.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/more_itertools/recipes.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/__about__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/markers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/requirements.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/specifiers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/packaging/version.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/actions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/common.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/core.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/exceptions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/helpers.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/results.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/testing.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/unicode.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/pyparsing/diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/alias.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/alias.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/bdist_egg.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/bdist_egg.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/bdist_rpm.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/bdist_rpm.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/build.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/build.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/build_clib.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/build_clib.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/build_ext.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/build_ext.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/build_py.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/build_py.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/develop.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/develop.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/dist_info.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/dist_info.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/easy_install.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/easy_install.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/editable_wheel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/editable_wheel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/egg_info.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/egg_info.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/install.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/install.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/install_egg_info.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/install_egg_info.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/install_lib.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/install_lib.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/install_scripts.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/install_scripts.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/launcher manifest.xml` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/launcher manifest.xml`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/py36compat.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/py36compat.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/rotate.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/rotate.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/saveopts.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/saveopts.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/sdist.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/sdist.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/setopt.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/setopt.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/test.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/test.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/command/upload_docs.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/command/upload_docs.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_apply_pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/expand.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/expand.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/pyprojecttoml.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/setupcfg.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/setupcfg.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/error_reporting.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/extra_validations.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/fastjsonschema_validations.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/config/_validate_pyproject/formats.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools/extern/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools/extern/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/LICENSE` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/METADATA` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/RECORD` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/entry_points.txt` & `codeoffer-0.9.0/venv/Lib/site-packages/setuptools-65.5.1.dist-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/_setuptools_logging.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/_setuptools_logging.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/bdist_wheel.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/bdist_wheel.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/macosx_libfile.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/macosx_libfile.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/metadata.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/metadata.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/util.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/util.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/wheelfile.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/cli/__init__.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/cli/convert.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/cli/pack.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/cli/unpack.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/vendored/packaging/_manylinux.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/vendored/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel/vendored/packaging/tags.py` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel/vendored/packaging/tags.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/LICENSE.txt` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/METADATA` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/RECORD` & `codeoffer-0.9.0/venv/Lib/site-packages/wheel-0.38.4.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/Activate.ps1` & `codeoffer-0.9.0/venv/Scripts/Activate.ps1`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/activate` & `codeoffer-0.9.0/venv/Scripts/activate`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/activate.bat` & `codeoffer-0.9.0/venv/Scripts/activate.bat`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/activate.fish` & `codeoffer-0.9.0/venv/Scripts/activate.fish`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/activate.nu` & `codeoffer-0.9.0/venv/Scripts/activate.nu`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/activate_this.py` & `codeoffer-0.9.0/venv/Scripts/activate_this.py`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/deactivate.nu` & `codeoffer-0.9.0/venv/Scripts/deactivate.nu`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/pip-3.10.exe` & `codeoffer-0.9.0/venv/Scripts/pip-3.10.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/pip.exe` & `codeoffer-0.9.0/venv/Scripts/pip.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/pip3.10.exe` & `codeoffer-0.9.0/venv/Scripts/pip3.10.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/pip3.exe` & `codeoffer-0.9.0/venv/Scripts/pip3.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/python.exe` & `codeoffer-0.9.0/venv/Scripts/python.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/pythonw.exe` & `codeoffer-0.9.0/venv/Scripts/pythonw.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/wheel-3.10.exe` & `codeoffer-0.9.0/venv/Scripts/wheel-3.10.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/wheel.exe` & `codeoffer-0.9.0/venv/Scripts/wheel.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/wheel3.10.exe` & `codeoffer-0.9.0/venv/Scripts/wheel3.10.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/venv/Scripts/wheel3.exe` & `codeoffer-0.9.0/venv/Scripts/wheel3.exe`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/LICENSE` & `codeoffer-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codeoffer-0.8.0/README.md` & `codeoffer-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 `token.get_login_link()`
 
 Right after that call the `token.wait_for_confirmation()` method, this method will wait until the user completed the login-process.
 
 To return the current logged in user you need to import the `user` class from `codeoffer`
 
 ```py
-from codeoffer import user
+
+from src.codeoffer import user
 ```
 
 Then you can return the current user by using the `get_user` method and passing the token as a parameter:
 
 ```py
 user = user.User.get_user(token)
 ```
@@ -74,27 +75,28 @@
 ```
 ```py
 for asset in assets:  
 	print(f"{asset.name}: {asset.access}")
 ```
 
 #### Complete Example
+
 ```py
-from codeoffer import oauth  
-from codeoffer import app  
-from codeoffer import user  
-      
-session = oauth.Session("10aa641e562bdd82d2f8449d")  
-token = session.create_session_token()  
-token.get_login_link()  
-token.wait_for_confirmation()  
-user = user.User.get_user(token)  
-print(f"Hey {user.username}")  
-app = app.App.by_session_token(token)  
-assets = app.get_asset_directory()  
-for asset in assets:  
-	print(f"{asset.name}: {asset.access}")
+from codeoffer import oauth
+from codeoffer import app
+from src.codeoffer import user
+
+session = oauth.Session("10aa641e562bdd82d2f8449d")
+token = session.create_session_token()
+token.get_login_link()
+token.wait_for_confirmation()
+user = user.User.get_user(token)
+print(f"Hey {user.username}")
+app = app.App.by_session_token(token)
+assets = app.get_asset_directory()
+for asset in assets:
+    print(f"{asset.name}: {asset.access}")
 ```
 
 ## License
 
 This package is licensed under the MIT License.
```

### Comparing `codeoffer-0.8.0/pyproject.toml` & `codeoffer-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "codeoffer"
-version = "0.8.0"
+version = "0.9.0"
 authors = [
   { name="CodeOffer", email="contact@codeoffer.net" },
 ]
 description = "Python API Wrapper for the public CodeOffer API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `codeoffer-0.8.0/PKG-INFO` & `codeoffer-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeoffer
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python API Wrapper for the public CodeOffer API
 Project-URL: Homepage, https://github.com/codeoffer/v1-python-library
 Project-URL: Bug Tracker, https://github.com/codeoffer/v1-python-library/issues
 Author-email: CodeOffer <contact@codeoffer.net>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -45,15 +45,16 @@
 `token.get_login_link()`
 
 Right after that call the `token.wait_for_confirmation()` method, this method will wait until the user completed the login-process.
 
 To return the current logged in user you need to import the `user` class from `codeoffer`
 
 ```py
-from codeoffer import user
+
+from src.codeoffer import user
 ```
 
 Then you can return the current user by using the `get_user` method and passing the token as a parameter:
 
 ```py
 user = user.User.get_user(token)
 ```
@@ -87,27 +88,28 @@
 ```
 ```py
 for asset in assets:  
 	print(f"{asset.name}: {asset.access}")
 ```
 
 #### Complete Example
+
 ```py
-from codeoffer import oauth  
-from codeoffer import app  
-from codeoffer import user  
-      
-session = oauth.Session("10aa641e562bdd82d2f8449d")  
-token = session.create_session_token()  
-token.get_login_link()  
-token.wait_for_confirmation()  
-user = user.User.get_user(token)  
-print(f"Hey {user.username}")  
-app = app.App.by_session_token(token)  
-assets = app.get_asset_directory()  
-for asset in assets:  
-	print(f"{asset.name}: {asset.access}")
+from codeoffer import oauth
+from codeoffer import app
+from src.codeoffer import user
+
+session = oauth.Session("10aa641e562bdd82d2f8449d")
+token = session.create_session_token()
+token.get_login_link()
+token.wait_for_confirmation()
+user = user.User.get_user(token)
+print(f"Hey {user.username}")
+app = app.App.by_session_token(token)
+assets = app.get_asset_directory()
+for asset in assets:
+    print(f"{asset.name}: {asset.access}")
 ```
 
 ## License
 
 This package is licensed under the MIT License.
```

