# Comparing `tmp/devapps-2023.5.1.tar.gz` & `tmp/devapps-2023.5.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devapps-2023.5.1.tar", max compression
+gzip compressed data, was "devapps-2023.5.10.tar", max compression
```

## Comparing `devapps-2023.5.1.tar` & `devapps-2023.5.10.tar`

### file list

```diff
@@ -1,143 +1,143 @@
--rw-r--r--   0        0        0     1323 2022-05-05 20:54:49.110883 devapps-2023.5.1/LICENSE
--rw-r--r--   0        0        0      992 2023-05-02 12:46:04.185957 devapps-2023.5.1/README.md
--rw-r--r--   0        0        0     5914 2023-05-02 12:45:48.609953 devapps-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-22 14:30:25.715938 devapps-2023.5.1/src/ax/utils/__init__.py
--rw-r--r--   0        0        0       28 2023-03-22 14:30:25.715938 devapps-2023.5.1/src/ax/utils/ax_tree/__init__.py
--rwxr-xr-x   0        0        0    88440 2023-03-22 14:30:25.716939 devapps-2023.5.1/src/ax/utils/ax_tree/_ax_tree.so
--rw-r--r--   0        0        0    10033 2023-03-22 14:30:25.716939 devapps-2023.5.1/src/ax/utils/ax_tree/ax_tree.py
--rwxr-xr-x   0        0        0      491 2023-03-22 14:28:26.989865 devapps-2023.5.1/src/devapp/__init__.py
--rwxr-xr-x   0        0        0    19220 2023-05-02 12:43:21.727927 devapps-2023.5.1/src/devapp/app.py
--rwxr-xr-x   0        0        0        0 2023-03-22 14:28:26.990865 devapps-2023.5.1/src/devapp/app_token/__init__.py
--rwxr-xr-x   0        0        0     1201 2023-03-22 14:28:26.990865 devapps-2023.5.1/src/devapp/app_token/create_tokens.py
--rwxr-xr-x   0        0        0     2230 2023-03-22 14:28:26.990865 devapps-2023.5.1/src/devapp/app_token/read_tokens.py
--rwxr-xr-x   0        0        0      151 2023-03-22 14:28:26.990865 devapps-2023.5.1/src/devapp/app_token/verify_token
--rwxr-xr-x   0        0        0      297 2023-03-22 14:28:26.990865 devapps-2023.5.1/src/devapp/components/__init__.py
--rwxr-xr-x   0        0        0     6980 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/components/cloudfoundry.py
--rwxr-xr-x   0        0        0     5956 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/components/gitlab.py
--rwxr-xr-x   0        0        0     4828 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/components/gitlab_runner.py
--rwxr-xr-x   0        0        0      150 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/da.py
--rwxr-xr-x   0        0        0     1321 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/dev_mode.py
--rwxr-xr-x   0        0        0     1636 2023-04-30 10:26:20.741214 devapps-2023.5.1/src/devapp/gevent_patched.py
--rwxr-xr-x   0        0        0     1549 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/layer.py
--rwxr-xr-x   0        0        0      188 2023-03-22 14:28:26.991865 devapps-2023.5.1/src/devapp/lib/README.md
--rwxr-xr-x   0        0        0        0 2023-03-22 14:28:26.992865 devapps-2023.5.1/src/devapp/lib/__init__.py
--rwxr-xr-x   0        0        0   123141 2023-03-22 14:28:26.992865 devapps-2023.5.1/src/devapp/lib/sh.py
--rwxr-xr-x   0        0        0     2343 2023-03-22 14:28:26.992865 devapps-2023.5.1/src/devapp/load.py
--rwxr-xr-x   0        0        0      655 2023-03-22 14:28:26.993865 devapps-2023.5.1/src/devapp/logo
--rwxr-xr-x   0        0        0     1671 2023-03-22 14:28:26.993865 devapps-2023.5.1/src/devapp/max.py
--rw-r--r--   0        0        0     1752 2023-03-22 14:28:26.993865 devapps-2023.5.1/src/devapp/operations/resources.py
--rwxr-xr-x   0        0        0     1551 2023-03-22 14:28:26.993865 devapps-2023.5.1/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py
--rwxr-xr-x   0        0        0     6445 2023-03-22 14:28:26.993865 devapps-2023.5.1/src/devapp/plugins/dev_devapp/repo_sym_links.py
--rw-r--r--   0        0        0     3090 2023-03-22 14:28:26.994865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resource_install.py
--rw-r--r--   0        0        0     4577 2023-03-22 14:28:26.994865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resource_run.py
--rw-r--r--   0        0        0     8983 2023-03-22 14:28:26.994865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resources.py.dis
--rw-r--r--   0        0        0      671 2023-03-22 14:28:26.994865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resources_list.py
--rw-r--r--   0        0        0      879 2023-03-22 14:28:26.994865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/wait_for_port.py
--rwxr-xr-x   0        0        0     8688 2023-03-22 14:28:26.995865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/container_build.py
--rwxr-xr-x   0        0        0    10257 2023-03-22 14:28:26.995865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/container_pull.py
--rwxr-xr-x   0        0        0    28013 2023-03-22 14:28:26.995865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/fs_build.py
--rwxr-xr-x   0        0        0    13318 2023-03-22 14:28:26.995865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py
--rwxr-xr-x   0        0        0     9232 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py
--rwxr-xr-x   0        0        0    12668 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py
--rwxr-xr-x   0        0        0     8750 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/kubectl/__init__.py
--rwxr-xr-x   0        0        0     2975 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/life_cycle.py
--rw-r--r--   0        0        0     1573 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/log_view.py
--rwxr-xr-x   0        0        0    11484 2023-03-22 14:28:26.996865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/project/__init__.py
--rw-r--r--   0        0        0     9960 2023-03-22 14:28:26.997865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py
--rw-r--r--   0        0        0     4994 2023-03-22 14:28:26.997865 devapps-2023.5.1/src/devapp/plugins/ops_devapp/run.py
--rwxr-xr-x   0        0        0    28235 2023-03-22 14:28:26.997865 devapps-2023.5.1/src/devapp/run.py
--rwxr-xr-x   0        0        0    25984 2023-03-22 14:28:26.997865 devapps-2023.5.1/src/devapp/spec/build.py
--rwxr-xr-x   0        0        0     2929 2023-03-22 14:28:26.997865 devapps-2023.5.1/src/devapp/spec/find_paths_in_fs_components.py
--rwxr-xr-x   0        0        0    16176 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/fs_components.py
--rwxr-xr-x   0        0        0     1715 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/links.py
--rwxr-xr-x   0        0        0     2481 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/os_tools.py
--rwxr-xr-x   0        0        0     7913 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/templ.py
--rwxr-xr-x   0        0        0     1600 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/templates/unit
--rwxr-xr-x   0        0        0     7586 2023-03-22 14:28:26.998865 devapps-2023.5.1/src/devapp/spec/tools.py
--rwxr-xr-x   0        0        0    30671 2023-03-22 14:28:26.999865 devapps-2023.5.1/src/devapp/t
--rw-r--r--   0        0        0     3559 2023-03-22 14:28:26.999865 devapps-2023.5.1/src/devapp/testing/auto_docs.py
--rw-r--r--   0        0        0      443 2023-03-22 14:28:26.999865 devapps-2023.5.1/src/devapp/tests/test_unit_devapp.py
--rwxr-xr-x   0        0        0    13808 2023-03-22 14:28:26.999865 devapps-2023.5.1/src/devapp/third/rpl
--rwxr-xr-x   0        0        0    50010 2023-05-02 12:16:52.557397 devapps-2023.5.1/src/devapp/tools/__init__.py
--rw-r--r--   0        0        0     4025 2023-03-22 14:28:27.000865 devapps-2023.5.1/src/devapp/tools/flag.py
--rw-r--r--   0        0        0      731 2023-03-22 14:28:27.000865 devapps-2023.5.1/src/devapp/tools/http.py
--rw-r--r--   0        0        0    35701 2023-03-22 14:28:27.000865 devapps-2023.5.1/src/devapp/tools/infra/__init__.py
--rw-r--r--   0        0        0    16618 2023-03-22 14:28:27.001865 devapps-2023.5.1/src/devapp/tools/infra/actions.py
--rw-r--r--   0        0        0     3089 2023-03-22 14:28:27.001865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/000:functions.sh
--rwxr-xr-x   0        0        0      375 2023-03-22 14:28:27.001865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/001:add_sudo_user.sh
--rwxr-xr-x   0        0        0     1521 2023-03-22 14:28:27.001865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh
--rwxr-xr-x   0        0        0      448 2023-03-22 14:28:27.002865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/100:docker.sh
--rwxr-xr-x   0        0        0      324 2023-03-22 14:28:27.002865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/200:tools.sh
--rwxr-xr-x   0        0        0      760 2023-03-22 14:28:27.002865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/300:dns.sh
--rwxr-xr-x   0        0        0     4375 2023-03-22 14:28:27.002865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/500:k3s.sh
--rwxr-xr-x   0        0        0      943 2023-03-22 14:28:27.002865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/501:kind.sh
--rwxr-xr-x   0        0        0    17210 2023-03-22 14:28:27.003865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/502:k3s.sh
--rw-r--r--   0        0        0      276 2023-03-22 14:28:27.003865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/510:label_workers.sh
--rwxr-xr-x   0        0        0      661 2023-03-22 14:28:27.003865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/600:longhorn.sh
--rw-r--r--   0        0        0     1737 2023-03-22 14:28:27.003865 devapps-2023.5.1/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh
--rw-r--r--   0        0        0     4408 2023-05-02 12:43:20.050927 devapps-2023.5.1/src/devapp/tools/plugin.py
--rw-r--r--   0        0        0    25788 2023-05-02 07:07:04.676265 devapps-2023.5.1/src/devapp/tools/resource.py
--rw-r--r--   0        0        0     1861 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/tools/times.py
--rwxr-xr-x   0        0        0        0 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/utils/__init__.py
--rwxr-xr-x   0        0        0    15787 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/utils/os_.py
--rwxr-xr-x   0        0        0     1871 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/utils/py_source_env.py
--rwxr-xr-x   0        0        0     9335 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/utils/rx_tools.py
--rwxr-xr-x   0        0        0    11529 2023-03-22 14:28:27.004865 devapps-2023.5.1/src/devapp/utils/vault.py
--rwxr-xr-x   0        0        0     2107 2023-05-02 12:19:24.575457 devapps-2023.5.1/src/devapp/utils/watch_dog.py
--rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.734938 devapps-2023.5.1/src/mdvl/__init__.py
--rwxr-xr-x   0        0        0    20402 2023-05-02 08:41:56.784342 devapps-2023.5.1/src/mdvl/mdvl.py
--rwxr-xr-x   0        0        0     2317 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/mdvl/tools.py
--rwxr-xr-x   0        0        0      519 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/structlogging/__init__.py
--rwxr-xr-x   0        0        0     1559 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/structlogging/adapters.py
--rwxr-xr-x   0        0        0       88 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/structlogging/common.py
--rwxr-xr-x   0        0        0     5503 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/structlogging/config.py
--rwxr-xr-x   0        0        0     1618 2023-03-22 14:30:25.735939 devapps-2023.5.1/src/structlogging/formatters.py
--rwxr-xr-x   0        0        0     2640 2023-03-22 14:30:25.736939 devapps-2023.5.1/src/structlogging/processors.py
--rwxr-xr-x   0        0        0     5472 2023-03-22 14:30:25.736939 devapps-2023.5.1/src/structlogging/renderers.py
--rwxr-xr-x   0        0        0    11172 2023-05-02 12:28:38.054778 devapps-2023.5.1/src/structlogging/sl.py
--rw-r--r--   0        0        0     4022 2023-03-22 14:30:25.736939 devapps-2023.5.1/src/structlogging/stacktrace.py
--rwxr-xr-x   0        0        0     1355 2023-03-22 14:30:25.736939 devapps-2023.5.1/src/structlogging/tests/test_structlogging.py
--rwxr-xr-x   0        0        0      886 2023-03-22 14:30:25.736939 devapps-2023.5.1/src/theming/__init__.py
--rwxr-xr-x   0        0        0    14865 2023-05-02 11:32:09.295201 devapps-2023.5.1/src/theming/absl_color_help.py
--rwxr-xr-x   0        0        0     4345 2023-03-22 14:30:25.737939 devapps-2023.5.1/src/theming/ansi2html.py
--rwxr-xr-x   0        0        0    11888 2023-03-22 14:30:25.737939 devapps-2023.5.1/src/theming/ansi2html.sh
--rwxr-xr-x   0        0        0     3030 2023-03-22 14:30:25.737939 devapps-2023.5.1/src/theming/ansistrm.py
--rwxr-xr-x   0        0        0    10066 2023-03-22 14:30:25.737939 devapps-2023.5.1/src/theming/ax_xml.py
--rwxr-xr-x   0        0        0    10495 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/camel_snake.py
--rwxr-xr-x   0        0        0     7517 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/charting.py
--rwxr-xr-x   0        0        0     3392 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/colorhilite.py
--rwxr-xr-x   0        0        0     1113 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/filesize/README.txt
--rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/filesize/__init__.py
--rwxr-xr-x   0        0        0     2549 2023-03-22 14:30:25.738939 devapps-2023.5.1/src/theming/filesize/filesize.py
--rwxr-xr-x   0        0        0     3756 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/formatters.py
--rw-r--r--   0        0        0     3807 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/formatting/markdown.py
--rw-r--r--   0        0        0     1241 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/formatting/viz_sequence.py
--rwxr-xr-x   0        0        0     3410 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/html_tools.py
--rwxr-xr-x   0        0        0    11409 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/inflect.py
--rwxr-xr-x   0        0        0      460 2023-03-22 14:30:25.739939 devapps-2023.5.1/src/theming/msgs.py
--rwxr-xr-x   0        0        0     9864 2023-03-22 14:30:25.740939 devapps-2023.5.1/src/theming/pretty_print.py
--rwxr-xr-x   0        0        0    55699 2023-03-22 14:30:25.740939 devapps-2023.5.1/src/theming/tablepretty.py
--rwxr-xr-x   0        0        0    13998 2023-03-22 14:30:25.740939 devapps-2023.5.1/src/theming/term.py
--rwxr-xr-x   0        0        0     1468 2023-03-22 14:30:25.740939 devapps-2023.5.1/src/theming/term_struct_hilite.py
--rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.740939 devapps-2023.5.1/src/theming/test
--rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.741938 devapps-2023.5.1/src/theming/tests/__init__.py
--rwxr-xr-x   0        0        0     9454 2023-03-22 14:30:25.741938 devapps-2023.5.1/src/theming/tests/test_text_formatting.py
--rwxr-xr-x   0        0        0     1063 2023-03-22 14:30:25.741938 devapps-2023.5.1/src/theming/tracebacks.py
--rwxr-xr-x   0        0        0     3011 2023-03-22 14:30:25.741938 devapps-2023.5.1/src/theming/unicode_chars.py
--rwxr-xr-x   0        0        0    23138 2023-03-23 18:50:41.169018 devapps-2023.5.1/src/tree_builder/__init__.py
--rwxr-xr-x   0        0        0    19864 2023-03-23 18:50:41.169018 devapps-2023.5.1/src/tree_builder/arch/__init__.py.bak
--rwxr-xr-x   0        0        0     7762 2023-03-23 18:50:41.169018 devapps-2023.5.1/src/tree_builder/arch/links.py.bak
--rwxr-xr-x   0        0        0    11455 2023-03-23 18:50:41.169018 devapps-2023.5.1/src/tree_builder/arch/o.py
--rwxr-xr-x   0        0        0    19872 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/arch/old
--rwxr-xr-x   0        0        0    10911 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/arch/olinit
--rwxr-xr-x   0        0        0    11597 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/arch/oo
--rwxr-xr-x   0        0        0      154 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/arch/py2.py
--rwxr-xr-x   0        0        0     7968 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/arch/render.py.bak
--rwxr-xr-x   0        0        0     2078 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/chrome_reload.sh
--rwxr-xr-x   0        0        0     5502 2023-03-23 18:50:41.170018 devapps-2023.5.1/src/tree_builder/delivery2.py
--rwxr-xr-x   0        0        0    10773 2023-03-23 18:50:41.171018 devapps-2023.5.1/src/tree_builder/links.py
--rwxr-xr-x   0        0        0      218 2023-03-23 18:50:41.171018 devapps-2023.5.1/src/tree_builder/py3.py
--rwxr-xr-x   0        0        0     8028 2023-03-23 18:50:41.171018 devapps-2023.5.1/src/tree_builder/render.py
--rwxr-xr-x   0        0        0       21 2023-03-23 18:50:41.171018 devapps-2023.5.1/src/tree_builder/version.py
--rw-r--r--   0        0        0     3037 2023-05-02 12:46:06.858805 devapps-2023.5.1/setup.py
--rw-r--r--   0        0        0     1804 2023-05-02 12:46:06.859069 devapps-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1323 2022-05-05 20:54:49.110883 devapps-2023.5.10/LICENSE
+-rw-r--r--   0        0        0      992 2023-05-10 02:47:33.968713 devapps-2023.5.10/README.md
+-rw-r--r--   0        0        0     5914 2023-05-10 02:47:19.782710 devapps-2023.5.10/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-22 14:30:25.715938 devapps-2023.5.10/src/ax/utils/__init__.py
+-rw-r--r--   0        0        0       28 2023-03-22 14:30:25.715938 devapps-2023.5.10/src/ax/utils/ax_tree/__init__.py
+-rwxr-xr-x   0        0        0    88440 2023-03-22 14:30:25.716939 devapps-2023.5.10/src/ax/utils/ax_tree/_ax_tree.so
+-rw-r--r--   0        0        0    10033 2023-03-22 14:30:25.716939 devapps-2023.5.10/src/ax/utils/ax_tree/ax_tree.py
+-rwxr-xr-x   0        0        0      491 2023-05-02 12:47:20.238964 devapps-2023.5.10/src/devapp/__init__.py
+-rwxr-xr-x   0        0        0    19220 2023-05-02 12:47:20.238964 devapps-2023.5.10/src/devapp/app.py
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.238964 devapps-2023.5.10/src/devapp/app_token/__init__.py
+-rwxr-xr-x   0        0        0     1201 2023-05-02 12:47:20.238964 devapps-2023.5.10/src/devapp/app_token/create_tokens.py
+-rwxr-xr-x   0        0        0     2230 2023-05-02 12:47:20.238964 devapps-2023.5.10/src/devapp/app_token/read_tokens.py
+-rwxr-xr-x   0        0        0      151 2023-05-02 12:47:20.239964 devapps-2023.5.10/src/devapp/app_token/verify_token
+-rwxr-xr-x   0        0        0      297 2023-05-02 12:47:20.239964 devapps-2023.5.10/src/devapp/components/__init__.py
+-rwxr-xr-x   0        0        0     6980 2023-05-02 12:47:20.239964 devapps-2023.5.10/src/devapp/components/cloudfoundry.py
+-rwxr-xr-x   0        0        0     5956 2023-05-02 12:47:20.239964 devapps-2023.5.10/src/devapp/components/gitlab.py
+-rwxr-xr-x   0        0        0     4828 2023-05-02 12:47:20.239964 devapps-2023.5.10/src/devapp/components/gitlab_runner.py
+-rwxr-xr-x   0        0        0      150 2023-05-02 12:47:20.239964 devapps-2023.5.10/src/devapp/da.py
+-rwxr-xr-x   0        0        0     1321 2023-05-02 12:47:20.239964 devapps-2023.5.10/src/devapp/dev_mode.py
+-rwxr-xr-x   0        0        0     1636 2023-05-02 12:47:20.240964 devapps-2023.5.10/src/devapp/gevent_patched.py
+-rwxr-xr-x   0        0        0     1549 2023-05-02 12:47:20.240964 devapps-2023.5.10/src/devapp/layer.py
+-rwxr-xr-x   0        0        0      188 2023-05-02 12:47:20.240964 devapps-2023.5.10/src/devapp/lib/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.240964 devapps-2023.5.10/src/devapp/lib/__init__.py
+-rwxr-xr-x   0        0        0   123141 2023-05-02 12:47:20.241964 devapps-2023.5.10/src/devapp/lib/sh.py
+-rwxr-xr-x   0        0        0     2343 2023-05-02 12:47:20.241964 devapps-2023.5.10/src/devapp/load.py
+-rwxr-xr-x   0        0        0      655 2023-05-02 12:47:20.241964 devapps-2023.5.10/src/devapp/logo
+-rwxr-xr-x   0        0        0     1671 2023-05-02 12:47:20.241964 devapps-2023.5.10/src/devapp/max.py
+-rw-r--r--   0        0        0     1926 2023-05-05 09:54:59.157765 devapps-2023.5.10/src/devapp/operations/resources.py
+-rwxr-xr-x   0        0        0     1551 2023-05-02 12:47:20.241964 devapps-2023.5.10/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py
+-rwxr-xr-x   0        0        0     6445 2023-05-02 12:47:20.241964 devapps-2023.5.10/src/devapp/plugins/dev_devapp/repo_sym_links.py
+-rw-r--r--   0        0        0     3090 2023-05-02 12:47:20.242964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/arch/resource_install.py
+-rw-r--r--   0        0        0     4577 2023-05-02 12:47:20.242964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/arch/resource_run.py
+-rw-r--r--   0        0        0     8983 2023-05-02 12:47:20.242964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/arch/resources.py.dis
+-rw-r--r--   0        0        0      671 2023-05-02 12:47:20.242964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/arch/resources_list.py
+-rw-r--r--   0        0        0      879 2023-05-02 12:47:20.242964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/arch/wait_for_port.py
+-rwxr-xr-x   0        0        0     8688 2023-05-02 12:47:20.242964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/container_build.py
+-rwxr-xr-x   0        0        0    10257 2023-05-02 12:47:20.242964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/container_pull.py
+-rwxr-xr-x   0        0        0    28013 2023-05-02 12:47:20.243964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/fs_build.py
+-rwxr-xr-x   0        0        0    13318 2023-05-02 12:47:20.243964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py
+-rwxr-xr-x   0        0        0     9232 2023-05-02 12:47:20.243964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py
+-rwxr-xr-x   0        0        0    12668 2023-05-02 12:47:20.243964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py
+-rwxr-xr-x   0        0        0     8750 2023-05-02 12:47:20.244964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/kubectl/__init__.py
+-rwxr-xr-x   0        0        0     2975 2023-05-02 12:47:20.244964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/life_cycle.py
+-rw-r--r--   0        0        0     1573 2023-05-02 12:47:20.244964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/log_view.py
+-rwxr-xr-x   0        0        0    11773 2023-05-10 02:43:35.060661 devapps-2023.5.10/src/devapp/plugins/ops_devapp/project/__init__.py
+-rw-r--r--   0        0        0     9960 2023-05-02 12:47:20.244964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py
+-rw-r--r--   0        0        0     4994 2023-05-02 12:47:20.245964 devapps-2023.5.10/src/devapp/plugins/ops_devapp/run.py
+-rwxr-xr-x   0        0        0    28235 2023-05-02 12:47:20.245964 devapps-2023.5.10/src/devapp/run.py
+-rwxr-xr-x   0        0        0    25984 2023-05-02 12:47:20.245964 devapps-2023.5.10/src/devapp/spec/build.py
+-rwxr-xr-x   0        0        0     2929 2023-05-02 12:47:20.246964 devapps-2023.5.10/src/devapp/spec/find_paths_in_fs_components.py
+-rwxr-xr-x   0        0        0    16176 2023-05-02 12:47:20.246964 devapps-2023.5.10/src/devapp/spec/fs_components.py
+-rwxr-xr-x   0        0        0     1715 2023-05-02 12:47:20.246964 devapps-2023.5.10/src/devapp/spec/links.py
+-rwxr-xr-x   0        0        0     2481 2023-05-02 12:47:20.246964 devapps-2023.5.10/src/devapp/spec/os_tools.py
+-rwxr-xr-x   0        0        0     7913 2023-05-02 12:47:20.246964 devapps-2023.5.10/src/devapp/spec/templ.py
+-rwxr-xr-x   0        0        0     1600 2023-05-02 12:47:20.246964 devapps-2023.5.10/src/devapp/spec/templates/unit
+-rwxr-xr-x   0        0        0     7586 2023-05-02 12:47:20.247964 devapps-2023.5.10/src/devapp/spec/tools.py
+-rwxr-xr-x   0        0        0    30671 2023-05-02 12:47:20.247964 devapps-2023.5.10/src/devapp/t
+-rw-r--r--   0        0        0     3559 2023-05-02 12:47:20.247964 devapps-2023.5.10/src/devapp/testing/auto_docs.py
+-rw-r--r--   0        0        0      443 2023-05-02 12:47:20.247964 devapps-2023.5.10/src/devapp/tests/test_unit_devapp.py
+-rwxr-xr-x   0        0        0    13808 2023-05-02 12:47:20.247964 devapps-2023.5.10/src/devapp/third/rpl
+-rwxr-xr-x   0        0        0    50010 2023-05-02 12:47:20.248964 devapps-2023.5.10/src/devapp/tools/__init__.py
+-rw-r--r--   0        0        0     4025 2023-05-02 12:47:20.248964 devapps-2023.5.10/src/devapp/tools/flag.py
+-rw-r--r--   0        0        0      731 2023-05-02 12:47:20.248964 devapps-2023.5.10/src/devapp/tools/http.py
+-rw-r--r--   0        0        0    35701 2023-05-02 12:47:20.248964 devapps-2023.5.10/src/devapp/tools/infra/__init__.py
+-rw-r--r--   0        0        0    16618 2023-05-02 12:47:20.248964 devapps-2023.5.10/src/devapp/tools/infra/actions.py
+-rw-r--r--   0        0        0     3089 2023-05-02 12:47:20.249964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/000:functions.sh
+-rwxr-xr-x   0        0        0      375 2023-05-02 12:47:20.249964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/001:add_sudo_user.sh
+-rwxr-xr-x   0        0        0     1521 2023-05-02 12:47:20.249964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh
+-rwxr-xr-x   0        0        0      448 2023-05-02 12:47:20.249964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/100:docker.sh
+-rwxr-xr-x   0        0        0      324 2023-05-02 12:47:20.249964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/200:tools.sh
+-rwxr-xr-x   0        0        0      760 2023-05-02 12:47:20.249964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/300:dns.sh
+-rwxr-xr-x   0        0        0     4375 2023-05-02 12:47:20.249964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/500:k3s.sh
+-rwxr-xr-x   0        0        0      943 2023-05-02 12:47:20.249964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/501:kind.sh
+-rwxr-xr-x   0        0        0    17210 2023-05-02 12:47:20.250964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/502:k3s.sh
+-rw-r--r--   0        0        0      276 2023-05-02 12:47:20.250964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/510:label_workers.sh
+-rwxr-xr-x   0        0        0      661 2023-05-02 12:47:20.250964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/600:longhorn.sh
+-rw-r--r--   0        0        0     1737 2023-05-02 12:47:20.250964 devapps-2023.5.10/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh
+-rw-r--r--   0        0        0     4415 2023-05-03 12:55:53.147915 devapps-2023.5.10/src/devapp/tools/plugin.py
+-rw-r--r--   0        0        0    25842 2023-05-05 09:37:50.644432 devapps-2023.5.10/src/devapp/tools/resource.py
+-rw-r--r--   0        0        0     1861 2023-05-02 12:47:20.251964 devapps-2023.5.10/src/devapp/tools/times.py
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.251964 devapps-2023.5.10/src/devapp/utils/__init__.py
+-rwxr-xr-x   0        0        0    15787 2023-05-02 12:47:20.251964 devapps-2023.5.10/src/devapp/utils/os_.py
+-rwxr-xr-x   0        0        0     1871 2023-05-02 12:47:20.251964 devapps-2023.5.10/src/devapp/utils/py_source_env.py
+-rwxr-xr-x   0        0        0     9335 2023-05-02 12:47:20.252964 devapps-2023.5.10/src/devapp/utils/rx_tools.py
+-rwxr-xr-x   0        0        0    11529 2023-05-02 12:47:20.252964 devapps-2023.5.10/src/devapp/utils/vault.py
+-rwxr-xr-x   0        0        0     2107 2023-05-02 12:47:20.252964 devapps-2023.5.10/src/devapp/utils/watch_dog.py
+-rwxr-xr-x   0        0        0        0 2023-03-22 14:30:25.734938 devapps-2023.5.10/src/mdvl/__init__.py
+-rwxr-xr-x   0        0        0    20402 2023-05-02 08:41:56.784342 devapps-2023.5.10/src/mdvl/mdvl.py
+-rwxr-xr-x   0        0        0     2317 2023-03-22 14:30:25.735939 devapps-2023.5.10/src/mdvl/tools.py
+-rwxr-xr-x   0        0        0      519 2023-03-22 14:30:25.735939 devapps-2023.5.10/src/structlogging/__init__.py
+-rwxr-xr-x   0        0        0     1559 2023-03-22 14:30:25.735939 devapps-2023.5.10/src/structlogging/adapters.py
+-rwxr-xr-x   0        0        0       88 2023-03-22 14:30:25.735939 devapps-2023.5.10/src/structlogging/common.py
+-rwxr-xr-x   0        0        0     5503 2023-03-22 14:30:25.735939 devapps-2023.5.10/src/structlogging/config.py
+-rwxr-xr-x   0        0        0     1618 2023-03-22 14:30:25.735939 devapps-2023.5.10/src/structlogging/formatters.py
+-rwxr-xr-x   0        0        0     2640 2023-03-22 14:30:25.736939 devapps-2023.5.10/src/structlogging/processors.py
+-rwxr-xr-x   0        0        0     5472 2023-03-22 14:30:25.736939 devapps-2023.5.10/src/structlogging/renderers.py
+-rwxr-xr-x   0        0        0    11172 2023-05-02 12:28:38.054778 devapps-2023.5.10/src/structlogging/sl.py
+-rw-r--r--   0        0        0     4022 2023-03-22 14:30:25.736939 devapps-2023.5.10/src/structlogging/stacktrace.py
+-rwxr-xr-x   0        0        0     1355 2023-03-22 14:30:25.736939 devapps-2023.5.10/src/structlogging/tests/test_structlogging.py
+-rwxr-xr-x   0        0        0      886 2023-05-02 12:47:20.254964 devapps-2023.5.10/src/theming/__init__.py
+-rwxr-xr-x   0        0        0    14865 2023-05-02 12:47:20.254964 devapps-2023.5.10/src/theming/absl_color_help.py
+-rwxr-xr-x   0        0        0     4345 2023-05-02 12:47:20.255964 devapps-2023.5.10/src/theming/ansi2html.py
+-rwxr-xr-x   0        0        0    11888 2023-05-02 12:47:20.255964 devapps-2023.5.10/src/theming/ansi2html.sh
+-rwxr-xr-x   0        0        0     3030 2023-05-02 12:47:20.255964 devapps-2023.5.10/src/theming/ansistrm.py
+-rwxr-xr-x   0        0        0    10066 2023-05-02 12:47:20.255964 devapps-2023.5.10/src/theming/ax_xml.py
+-rwxr-xr-x   0        0        0    10495 2023-05-02 12:47:20.255964 devapps-2023.5.10/src/theming/camel_snake.py
+-rwxr-xr-x   0        0        0     7517 2023-05-02 12:47:20.256964 devapps-2023.5.10/src/theming/charting.py
+-rwxr-xr-x   0        0        0     3392 2023-05-02 12:47:20.256964 devapps-2023.5.10/src/theming/colorhilite.py
+-rwxr-xr-x   0        0        0     1113 2023-05-02 12:47:20.256964 devapps-2023.5.10/src/theming/filesize/README.txt
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.256964 devapps-2023.5.10/src/theming/filesize/__init__.py
+-rwxr-xr-x   0        0        0     2549 2023-05-02 12:47:20.256964 devapps-2023.5.10/src/theming/filesize/filesize.py
+-rwxr-xr-x   0        0        0     3756 2023-05-02 12:47:20.257964 devapps-2023.5.10/src/theming/formatters.py
+-rw-r--r--   0        0        0     3807 2023-05-02 12:47:20.257964 devapps-2023.5.10/src/theming/formatting/markdown.py
+-rw-r--r--   0        0        0     1241 2023-05-02 12:47:20.257964 devapps-2023.5.10/src/theming/formatting/viz_sequence.py
+-rwxr-xr-x   0        0        0     3410 2023-05-02 12:47:20.257964 devapps-2023.5.10/src/theming/html_tools.py
+-rwxr-xr-x   0        0        0    11409 2023-05-02 12:47:20.257964 devapps-2023.5.10/src/theming/inflect.py
+-rwxr-xr-x   0        0        0      460 2023-05-02 12:47:20.258964 devapps-2023.5.10/src/theming/msgs.py
+-rwxr-xr-x   0        0        0     9864 2023-05-02 12:47:20.258964 devapps-2023.5.10/src/theming/pretty_print.py
+-rwxr-xr-x   0        0        0    55699 2023-05-02 12:47:20.258964 devapps-2023.5.10/src/theming/tablepretty.py
+-rwxr-xr-x   0        0        0    13998 2023-05-02 12:47:20.259964 devapps-2023.5.10/src/theming/term.py
+-rwxr-xr-x   0        0        0     1468 2023-05-02 12:47:20.259964 devapps-2023.5.10/src/theming/term_struct_hilite.py
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.5.10/src/theming/test
+-rwxr-xr-x   0        0        0        0 2023-05-02 12:47:20.259964 devapps-2023.5.10/src/theming/tests/__init__.py
+-rwxr-xr-x   0        0        0     9454 2023-05-02 12:47:20.260964 devapps-2023.5.10/src/theming/tests/test_text_formatting.py
+-rwxr-xr-x   0        0        0     1063 2023-05-02 12:47:20.260964 devapps-2023.5.10/src/theming/tracebacks.py
+-rwxr-xr-x   0        0        0     3011 2023-05-02 12:47:20.260964 devapps-2023.5.10/src/theming/unicode_chars.py
+-rwxr-xr-x   0        0        0    23138 2023-03-23 18:50:41.169018 devapps-2023.5.10/src/tree_builder/__init__.py
+-rwxr-xr-x   0        0        0    19864 2023-03-23 18:50:41.169018 devapps-2023.5.10/src/tree_builder/arch/__init__.py.bak
+-rwxr-xr-x   0        0        0     7762 2023-03-23 18:50:41.169018 devapps-2023.5.10/src/tree_builder/arch/links.py.bak
+-rwxr-xr-x   0        0        0    11455 2023-03-23 18:50:41.169018 devapps-2023.5.10/src/tree_builder/arch/o.py
+-rwxr-xr-x   0        0        0    19872 2023-03-23 18:50:41.170018 devapps-2023.5.10/src/tree_builder/arch/old
+-rwxr-xr-x   0        0        0    10911 2023-03-23 18:50:41.170018 devapps-2023.5.10/src/tree_builder/arch/olinit
+-rwxr-xr-x   0        0        0    11597 2023-03-23 18:50:41.170018 devapps-2023.5.10/src/tree_builder/arch/oo
+-rwxr-xr-x   0        0        0      154 2023-03-23 18:50:41.170018 devapps-2023.5.10/src/tree_builder/arch/py2.py
+-rwxr-xr-x   0        0        0     7968 2023-03-23 18:50:41.170018 devapps-2023.5.10/src/tree_builder/arch/render.py.bak
+-rwxr-xr-x   0        0        0     2078 2023-03-23 18:50:41.170018 devapps-2023.5.10/src/tree_builder/chrome_reload.sh
+-rwxr-xr-x   0        0        0     5502 2023-03-23 18:50:41.170018 devapps-2023.5.10/src/tree_builder/delivery2.py
+-rwxr-xr-x   0        0        0    10773 2023-03-23 18:50:41.171018 devapps-2023.5.10/src/tree_builder/links.py
+-rwxr-xr-x   0        0        0      218 2023-03-23 18:50:41.171018 devapps-2023.5.10/src/tree_builder/py3.py
+-rwxr-xr-x   0        0        0     8028 2023-03-23 18:50:41.171018 devapps-2023.5.10/src/tree_builder/render.py
+-rwxr-xr-x   0        0        0       21 2023-03-23 18:50:41.171018 devapps-2023.5.10/src/tree_builder/version.py
+-rw-r--r--   0        0        0     3038 2023-05-10 02:47:36.693590 devapps-2023.5.10/setup.py
+-rw-r--r--   0        0        0     1805 2023-05-10 02:47:36.693855 devapps-2023.5.10/PKG-INFO
```

### Comparing `devapps-2023.5.1/LICENSE` & `devapps-2023.5.10/LICENSE`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/README.md` & `devapps-2023.5.10/README.md`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/pyproject.toml` & `devapps-2023.5.10/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "devapps"
-version = "2023.05.01"
+version = "2023.05.10"
 description = "Apps - End to End."
 authors = ["Gunther Klessinger <g_kle_ss_ing_er@gmx.de>"]
 license = "BSD"
 readme = "README.md"
 repository = "https://github.com/AXGKl/devapps"
 homepage = "https://axgkl.github.io/devapps"
 keywords = []
```

### Comparing `devapps-2023.5.1/src/ax/utils/ax_tree/_ax_tree.so` & `devapps-2023.5.10/src/ax/utils/ax_tree/_ax_tree.so`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/ax/utils/ax_tree/ax_tree.py` & `devapps-2023.5.10/src/ax/utils/ax_tree/ax_tree.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/app.py` & `devapps-2023.5.10/src/devapp/app.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/app_token/create_tokens.py` & `devapps-2023.5.10/src/devapp/app_token/create_tokens.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/app_token/read_tokens.py` & `devapps-2023.5.10/src/devapp/app_token/read_tokens.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/components/cloudfoundry.py` & `devapps-2023.5.10/src/devapp/components/cloudfoundry.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/components/gitlab.py` & `devapps-2023.5.10/src/devapp/components/gitlab.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/components/gitlab_runner.py` & `devapps-2023.5.10/src/devapp/components/gitlab_runner.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/dev_mode.py` & `devapps-2023.5.10/src/devapp/dev_mode.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/gevent_patched.py` & `devapps-2023.5.10/src/devapp/gevent_patched.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/layer.py` & `devapps-2023.5.10/src/devapp/layer.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/lib/sh.py` & `devapps-2023.5.10/src/devapp/lib/sh.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/load.py` & `devapps-2023.5.10/src/devapp/load.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/logo` & `devapps-2023.5.10/src/devapp/logo`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/max.py` & `devapps-2023.5.10/src/devapp/max.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/operations/resources.py` & `devapps-2023.5.10/src/devapp/operations/resources.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 from devapp.app import app
 
 
 class tool:
     conda_env = 'lctools'
 
 
-redis_pre = '''
+redis_pre = """
 test "$1" == "cli" && { shift; redis-cli "$@"; exit $?; }
 test -n "$1" && { redis-server "$@"; exit $?; }
 test -e "$host_conf_dir/redis.conf" && { redis-server "$host_conf_dir/redis.conf"; exit $?; }
 
-'''
+"""
 
 
 def redis_server(**kw):
-    m = {'cmd': ':redis-server --port %s' % offset_port(kw['rsc'].port)}
-    m['cmd_pre'] = redis_pre
+    if kw.get('cmd') == 'redis-cli':
+        m = {'cmd': ':redis-cli -p %s' % offset_port(kw['rsc'].port)}
+    else:
+        m = {'cmd': ':redis-server --port %s' % offset_port(kw['rsc'].port)}
+        m['cmd_pre'] = redis_pre
     return m
 
 
 def verify_tools(path, rsc, **kw):
     for p in rsc.provides:
         d = path + '/' + p
         if not exists(d):
@@ -39,14 +42,15 @@
     return cmd
 
 
 class rsc:
     """For services we change dir to project."""
 
     class redis_server:
+        provides = ['redis-server', 'redis-cli']
         cmd = 'redis-server'
         run = redis_server
         pkg = 'redis'
         port = 6379
         systemd = 'redis-server'
 
     class lc_tools:
```

### Comparing `devapps-2023.5.1/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py` & `devapps-2023.5.10/src/devapp/plugins/dev_devapp/personal_development_sandbox/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/dev_devapp/repo_sym_links.py` & `devapps-2023.5.10/src/devapp/plugins/dev_devapp/repo_sym_links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resource_install.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/arch/resource_install.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resource_run.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/arch/resource_run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resources.py.dis` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/arch/resources.py.dis`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/resources_list.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/arch/resources_list.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/arch/wait_for_port.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/arch/wait_for_port.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/container_build.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/container_build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/container_pull.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/container_pull.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/fs_build.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/fs_build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/infra_aws_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/infra_digital_ocean/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/infra_hetzner_cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/kubectl/__init__.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/kubectl/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/life_cycle.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/life_cycle.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/log_view.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/log_view.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/project/__init__.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/project/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 """
 Devapp Project Creation
 
 By providing the --init_at <project dir> switch we will (re-)initialize a project directory there, incl:
 
 - Installing available resources, like databases and tools within a given directory (conda_prefix)
 - Creating resource start wrappers in <project_dir>/bin
-- Creating a 
+- Creating a
 
 Privilege escalation is not required for any of these steps, your system remains unchanged, except <project_dir> and <conda_prefix>
-
 """
 # Could be done far smaller.
 from re import match
 from devapp import gevent_patched
 import hashlib
 import json
 import os
@@ -59,29 +58,30 @@
         d = False
 
     class init_create_all_units:
         n = 'If set we create unit files for ALL service type resources'
         d = False
 
     class init_create_unit_files:
-        'Valid: Entries in rsc.provides, rsc.cmd or rsc.exe (i.e. the filename of the wrapper in bin dir). Not: rsc.name.'
+        """Valid: Entries in rsc.provides, rsc.cmd or rsc.exe (i.e. the filename of the wrapper in bin dir). Not: rsc.name."""
+
         n = 'List service unit files you want to have created for systemctl --user.'
         d = []
 
     class init_resource_match:
         n = 'Install only matching resources. Examples: -irm "redis, hub" or -irm \'!mysql, !redis\' (! negates).'
         d = []
 
     class list_resources_files:
         n = 'Show available definition files.'
         d = False
 
     class add_post_process_cmd:
         n = 'Add this to all commands which have systemd service units. Intended for output redirection. Not applied when stdout is a tty.\n'
-        n += '''Example: -appc='2>&1 | rotatelogs -e -n1 "$logfile" 1M' ($logfile defined in wrapper -> use single quotes).\n'''
+        n += """Example: -appc='2>&1 | rotatelogs -e -n1 "$logfile" 1M' ($logfile defined in wrapper -> use single quotes).\n"""
         n += 'Tip: Use rotatelogs only on powers of 10 - spotted problems with 200M. Use 100M or 1G in that case.'
         d = ''
 
     class edit_matching_resource_file:
         n = 'Open resource files in $EDITOR, matching given string in their content'
         d = ''
 
@@ -205,16 +205,26 @@
     for u in list(m):
         if u.startswith('!'):
             m.remove(u)
             negates.append(u[1:])
     r = api.find_resource_defs()
     rscs = S.rscs_defined
     api.add_install_state(rscs)
-    matches = lambda r: any([_ in str(api.to_dict(r)) for _ in m])
-    rscs = [r for r in rscs if not m or matches(r)]
+    # matches = lambda r: any([_ in str(api.to_dict(r)) for _ in m])
+    def matches(rsc, m):
+        r = api.to_dict(rsc)
+        for _ in m:
+            if (
+                str(r.get('systemd')) == _
+                or str(r.get('cmd')).startswith(_)
+                or str(r.get('name')).startswith(_)
+            ):
+                return True
+
+    rscs = [r for r in rscs if not m or matches(r, m)]
     if negates:
         n = negates
         rscs = [r for r in rscs if not any([_ in str(api.to_dict(r)) for _ in n])]
     disabled.rscs = d = [
         r for r in rscs if r.disabled == True and not matches(r) and not r.installed
     ]
     if d:
@@ -296,15 +306,15 @@
         app.warn('systemd --user service seems not running', hint=T_SDU_SVD)
         # automatic installs must get an error when this happens:
         app.die('Failing the project init command, please fix systemd --user')
 
 
 # https://serverfault.com/a/1026914 - this is really relevant,
 # since RH and drives deployers crazy on first command!
-T_SDU_SVD = '''
+T_SDU_SVD = """
 We are using the systemd **user** service to manage processes. This means there is a systemd process that runs as unprivileged user. 
 The systemd user service is not used as commonly as the normal systemd process manager.
 For example Red Hat disabled the systemd user service in RHEL 7 (and thereby all distros that come from RHEL, like CentOS, Oracle Linux 7, Amazon Linux 2).
 However, RedHat has assured that running the systemd user service is supported as long as the service is re-enabled.
 
 This is how to start the `systemd --user service` for user with $UID=_UID_ (the current user):
 
@@ -345,15 +355,15 @@
 WantedBy=default.target
 
 ____________________________________________________________________________________________________
 
 Then enable and start the unit.
 
 Run `ps -fww $(pgrep -f "systemd --user")` to verify success, then try re-init the project.
-'''
+"""
 
 T_SDU_SVD = T_SDU_SVD.replace('_UID_', str(os.getuid()))
 
 
 main = lambda: run_app(run, flags=Flags)
```

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/project/devinstall/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/plugins/ops_devapp/run.py` & `devapps-2023.5.10/src/devapp/plugins/ops_devapp/run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/run.py` & `devapps-2023.5.10/src/devapp/run.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/spec/build.py` & `devapps-2023.5.10/src/devapp/spec/build.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/spec/find_paths_in_fs_components.py` & `devapps-2023.5.10/src/devapp/spec/find_paths_in_fs_components.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/spec/fs_components.py` & `devapps-2023.5.10/src/devapp/spec/fs_components.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/spec/links.py` & `devapps-2023.5.10/src/devapp/spec/links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/spec/os_tools.py` & `devapps-2023.5.10/src/devapp/spec/os_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/spec/templ.py` & `devapps-2023.5.10/src/devapp/spec/templ.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/spec/templates/unit` & `devapps-2023.5.10/src/devapp/spec/templates/unit`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/spec/tools.py` & `devapps-2023.5.10/src/devapp/spec/tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/t` & `devapps-2023.5.10/src/devapp/t`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/testing/auto_docs.py` & `devapps-2023.5.10/src/devapp/testing/auto_docs.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/third/rpl` & `devapps-2023.5.10/src/devapp/third/rpl`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/__init__.py` & `devapps-2023.5.10/src/devapp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/flag.py` & `devapps-2023.5.10/src/devapp/tools/flag.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/http.py` & `devapps-2023.5.10/src/devapp/tools/http.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/infra/__init__.py` & `devapps-2023.5.10/src/devapp/tools/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/infra/actions.py` & `devapps-2023.5.10/src/devapp/tools/infra/actions.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/infra/playbooks/000:functions.sh` & `devapps-2023.5.10/src/devapp/tools/infra/playbooks/000:functions.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh` & `devapps-2023.5.10/src/devapp/tools/infra/playbooks/1000:k_hello_world1.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/infra/playbooks/300:dns.sh` & `devapps-2023.5.10/src/devapp/tools/infra/playbooks/300:dns.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/infra/playbooks/500:k3s.sh` & `devapps-2023.5.10/src/devapp/tools/infra/playbooks/500:k3s.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/infra/playbooks/501:kind.sh` & `devapps-2023.5.10/src/devapp/tools/infra/playbooks/501:kind.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/infra/playbooks/502:k3s.sh` & `devapps-2023.5.10/src/devapp/tools/infra/playbooks/502:k3s.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/infra/playbooks/600:longhorn.sh` & `devapps-2023.5.10/src/devapp/tools/infra/playbooks/600:longhorn.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh` & `devapps-2023.5.10/src/devapp/tools/infra/playbooks/800:kube_hypermodern.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/tools/plugin.py` & `devapps-2023.5.10/src/devapp/tools/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 def get_docstr(app=None):
     if not app:
         app = sys.argv[0]
 
     D = """
 Usage: %(app)s ACTION [--flag[=value] ...]
 
-Available Plugins:
+Available Action Plugins:
 <PLUGINS>
 
 Help:
     %(app)s <action> <-h|--helpfull> [match]
 
 Note:
     - Action shortcuts understood, e.g. action "foo_bar_baz" = fbb
```

### Comparing `devapps-2023.5.1/src/devapp/tools/resource.py` & `devapps-2023.5.10/src/devapp/tools/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python
 """
 Common API for all resources
-
 """
 # FIXME Do this as state table! Its crying for that
 
 import os, sys
 import json
 import time
 from functools import partial
@@ -20,15 +19,15 @@
     exists,
     repl_dollar_var_with_env_val,
     dirname,
     write_file,
     read_file,
 )
 
-T_unit = '''
+T_unit = """
 [Unit]
 Description      = %(descr)s %(name)s
 Wants            = network-online.target
 StopWhenUnneeded = false
 
 [Service]
 Type             = simple
@@ -42,15 +41,15 @@
 TimeoutStopSec   = 5
 SyslogIdentifier = %(name)s
 
 [Install]
 WantedBy = default.target
 
 # _MATCH_ (auto created %(ctime)s) 
-'''
+"""
 unit_match = 'DevApp Unit'
 T_unit = T_unit.replace('_MATCH_', unit_match)
 
 
 class S:
     """state"""
 
@@ -97,15 +96,15 @@
     """
     Resources install location, except filesystem based ones. Env vars resolved.
 
     Aliases:
     - local|l: <project_dir>/conda
     - default|d: $HOME/miniconda3 (default path of conda)
     - current|c: Any current conda_prefix set when running.
-    
+
     Note: Installing resources outside the project keeps the project relocatable and resources reusable for other products.
     """
 
     cli = repl_dollar_var_with_env_val(FLG.conda_prefix)
     if not cli:
         cli = 'default'
     if cli in ('current', 'c'):
@@ -420,23 +419,23 @@
             if g(FLG, 'init_create_all_units'):
                 units.extend(listed(g(rsc, 'systemd', None)))
 
             has_unit = False
             if any([u for u in units if u == cmd]):
                 has_unit = True
                 n_svc = Install.write_unit_file(cmd, fn, rsc)
-                s = '''
+                s = """
 
                 case "${1:-}" in
                     start|restart|stop|status)
                         systemctl --user --no-pager $1 "%s"
                         exit $?
                         ;;
                 esac
-                '''
+                """
                 add(deindent(s % n_svc))
 
             # env['PATH'] = '%s:$PATH' % g(rsc, 'path')
             add('')
             add("H='__HOME__'")
             add('export PROJECT_ROOT="%s"' % project.root())
             add('')
@@ -537,15 +536,18 @@
                     '%(conda)s activate "%(name)s"',
                 ]
             ctx['conda'] = ctx.get('conda', 'conda')
             pth = '%(D)s/envs/%(name)s/bin/' % ctx
 
             if g(rsc, 'typ') == 'pip':
                 ctx['cmd'] = rsc.cmd
-                cmd += ['%(conda)s install -c conda-forge python; %p/pip install %%(cmd)s' % pth]
+                cmd += [
+                    '%(conda)s install -c conda-forge python; %p/pip install %%(cmd)s'
+                    % pth
+                ]
             else:
                 icmd = g(rsc, 'conda_inst', '')
                 if icmd:
                     cmd += [icmd]
                 else:
                     p = g(rsc, 'conda_pkg') or g(rsc, 'pkg') or ' '.join(rsc.provides)
                     chan = g(rsc, 'conda_chan', '')
@@ -553,15 +555,15 @@
                         chan = '-c ' + chan
                     ctx['chan'] = chan
                     ctx['pkg'] = p
                     cmd += ['%(conda)s install %(yes)s -c conda-forge %(chan)s %(pkg)s']
             cmd = ' && '.join(cmd) % ctx
             rsc.path = g(rsc, 'path') or pth
 
-            #app.info('cmd', cmd=cmd)
+            # app.info('cmd', cmd=cmd)
             # import subprocess
             # s = subprocess.run(cmd, shell=True, executable='/bin/bash')
             # will run under dash, sh, bash -> problem e.g. for conda activate
             return do(system, cmd)
 
         def base(location):
             app.warn('conda dir not found', dir=location)
```

### Comparing `devapps-2023.5.1/src/devapp/tools/times.py` & `devapps-2023.5.10/src/devapp/tools/times.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/utils/os_.py` & `devapps-2023.5.10/src/devapp/utils/os_.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/utils/py_source_env.py` & `devapps-2023.5.10/src/devapp/utils/py_source_env.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/utils/rx_tools.py` & `devapps-2023.5.10/src/devapp/utils/rx_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/utils/vault.py` & `devapps-2023.5.10/src/devapp/utils/vault.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/devapp/utils/watch_dog.py` & `devapps-2023.5.10/src/devapp/utils/watch_dog.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/mdvl/mdvl.py` & `devapps-2023.5.10/src/mdvl/mdvl.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/mdvl/tools.py` & `devapps-2023.5.10/src/mdvl/tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/structlogging/__init__.py` & `devapps-2023.5.10/src/structlogging/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/structlogging/adapters.py` & `devapps-2023.5.10/src/structlogging/adapters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/structlogging/config.py` & `devapps-2023.5.10/src/structlogging/config.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/structlogging/formatters.py` & `devapps-2023.5.10/src/structlogging/formatters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/structlogging/processors.py` & `devapps-2023.5.10/src/structlogging/processors.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/structlogging/renderers.py` & `devapps-2023.5.10/src/structlogging/renderers.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/structlogging/sl.py` & `devapps-2023.5.10/src/structlogging/sl.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/structlogging/stacktrace.py` & `devapps-2023.5.10/src/structlogging/stacktrace.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/structlogging/tests/test_structlogging.py` & `devapps-2023.5.10/src/structlogging/tests/test_structlogging.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/__init__.py` & `devapps-2023.5.10/src/theming/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/absl_color_help.py` & `devapps-2023.5.10/src/theming/absl_color_help.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/ansi2html.py` & `devapps-2023.5.10/src/theming/ansi2html.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/ansi2html.sh` & `devapps-2023.5.10/src/theming/ansi2html.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/ansistrm.py` & `devapps-2023.5.10/src/theming/ansistrm.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/ax_xml.py` & `devapps-2023.5.10/src/theming/ax_xml.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/camel_snake.py` & `devapps-2023.5.10/src/theming/camel_snake.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/charting.py` & `devapps-2023.5.10/src/theming/charting.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/colorhilite.py` & `devapps-2023.5.10/src/theming/colorhilite.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/filesize/README.txt` & `devapps-2023.5.10/src/theming/filesize/README.txt`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/filesize/filesize.py` & `devapps-2023.5.10/src/theming/filesize/filesize.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/formatters.py` & `devapps-2023.5.10/src/theming/formatters.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/formatting/markdown.py` & `devapps-2023.5.10/src/theming/formatting/markdown.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/formatting/viz_sequence.py` & `devapps-2023.5.10/src/theming/formatting/viz_sequence.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/html_tools.py` & `devapps-2023.5.10/src/theming/html_tools.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/inflect.py` & `devapps-2023.5.10/src/theming/inflect.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/pretty_print.py` & `devapps-2023.5.10/src/theming/pretty_print.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/tablepretty.py` & `devapps-2023.5.10/src/theming/tablepretty.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/term.py` & `devapps-2023.5.10/src/theming/term.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/term_struct_hilite.py` & `devapps-2023.5.10/src/theming/term_struct_hilite.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/tests/test_text_formatting.py` & `devapps-2023.5.10/src/theming/tests/test_text_formatting.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/tracebacks.py` & `devapps-2023.5.10/src/theming/tracebacks.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/theming/unicode_chars.py` & `devapps-2023.5.10/src/theming/unicode_chars.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/__init__.py` & `devapps-2023.5.10/src/tree_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/arch/__init__.py.bak` & `devapps-2023.5.10/src/tree_builder/arch/__init__.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/arch/links.py.bak` & `devapps-2023.5.10/src/tree_builder/arch/links.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/arch/o.py` & `devapps-2023.5.10/src/tree_builder/arch/o.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/arch/old` & `devapps-2023.5.10/src/tree_builder/arch/old`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/arch/olinit` & `devapps-2023.5.10/src/tree_builder/arch/olinit`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/arch/oo` & `devapps-2023.5.10/src/tree_builder/arch/oo`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/arch/render.py.bak` & `devapps-2023.5.10/src/tree_builder/arch/render.py.bak`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/chrome_reload.sh` & `devapps-2023.5.10/src/tree_builder/chrome_reload.sh`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/delivery2.py` & `devapps-2023.5.10/src/tree_builder/delivery2.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/links.py` & `devapps-2023.5.10/src/tree_builder/links.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/src/tree_builder/render.py` & `devapps-2023.5.10/src/tree_builder/render.py`

 * *Files identical despite different names*

### Comparing `devapps-2023.5.1/setup.py` & `devapps-2023.5.10/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                      'dev = devapp.tools.plugin:main',
                      'fui = interactive.cli:main',
                      'myapp = devapp.tools.plugin:main',
                      'ops = devapp.tools.plugin:main']}
 
 setup_kwargs = {
     'name': 'devapps',
-    'version': '2023.5.1',
+    'version': '2023.5.10',
     'description': 'Apps - End to End.',
     'long_description': '# devapps\n\n\n<!-- badges -->\n[![docs pages][docs pages_img]][docs pages] [![gh-ci][gh-ci_img]][gh-ci] [![pkg][pkg_img]][pkg] [![code_style][code_style_img]][code_style] \n\n[docs pages]: https://axgkl.github.io/devapps/\n[docs pages_img]: https://axgkl.github.io/devapps/img/badge_docs.svg\n[gh-ci]: https://github.com/AXGKl/devapps/actions/workflows/ci.yml\n[gh-ci_img]: https://github.com/AXGKl/devapps/actions/workflows/ci.yml/badge.svg\n[pkg]: https://pypi.com/\n[pkg_img]: https://axgkl.github.io/devapps/img/badge_pypi.svg\n[code_style]: https://pypi.org/project/axblack/\n[code_style_img]: https://axgkl.github.io/devapps/img/badge_axblack.svg\n<!-- badges -->\n\n\nEnabler repo for dev *and* ops friendly apps, in a normalized way.\n\nIncludes:\n\n- logging (structlog)\n- cli flags handling (abseil, with addons)\n- docutools (mkdocs-material)\n- project setup\n- (test) resources management, including daemons and container filesystem layers\n\nand more.\n\n\n\n\nDocumentation: https://axgkl.github.io/devapps/',
     'author': 'Gunther Klessinger',
     'author_email': 'g_kle_ss_ing_er@gmx.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://axgkl.github.io/devapps',
```

### Comparing `devapps-2023.5.1/PKG-INFO` & `devapps-2023.5.10/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devapps
-Version: 2023.5.1
+Version: 2023.5.10
 Summary: Apps - End to End.
 Home-page: https://axgkl.github.io/devapps
 License: BSD
 Author: Gunther Klessinger
 Author-email: g_kle_ss_ing_er@gmx.de
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

