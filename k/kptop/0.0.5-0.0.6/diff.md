# Comparing `tmp/kptop-0.0.5-py3-none-any.whl.zip` & `tmp/kptop-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 44315 bytes, number of entries: 20
--rw-r--r--  2.0 unx       86 b- defN 22-Dec-18 22:31 kptop_tool.py
--rw-r--r--  2.0 unx        0 b- defN 22-Dec-12 07:34 kubePtop/__init__.py
--rw-r--r--  2.0 unx     5483 b- defN 22-Dec-16 17:39 kubePtop/ascii_graph.py
--rw-r--r--  2.0 unx     7048 b- defN 22-Dec-24 07:15 kubePtop/cli.py
--rw-r--r--  2.0 unx      366 b- defN 22-Dec-16 16:41 kubePtop/colors.py
--rw-r--r--  2.0 unx      531 b- defN 22-Dec-23 13:26 kubePtop/global_attrs.py
--rw-r--r--  2.0 unx     3464 b- defN 22-Dec-16 22:55 kubePtop/helper.py
--rw-r--r--  2.0 unx     1053 b- defN 22-Dec-23 13:26 kubePtop/logging.py
--rw-r--r--  2.0 unx    52509 b- defN 22-Dec-24 08:34 kubePtop/node_metrics.py
--rw-r--r--  2.0 unx    59849 b- defN 22-Dec-23 13:26 kubePtop/node_monitor.py
--rw-r--r--  2.0 unx    53769 b- defN 22-Dec-24 08:29 kubePtop/pod_metrics.py
--rw-r--r--  2.0 unx    36839 b- defN 22-Dec-23 13:26 kubePtop/pod_monitor.py
--rw-r--r--  2.0 unx     2267 b- defN 22-Dec-23 13:26 kubePtop/read_env.py
--rw-r--r--  2.0 unx    16760 b- defN 22-Dec-23 13:26 kubePtop/session.py
--rw-r--r--  2.0 unx    35149 b- defN 22-Dec-24 08:38 kptop-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      533 b- defN 22-Dec-24 08:38 kptop-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Dec-24 08:38 kptop-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 22-Dec-24 08:38 kptop-0.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 22-Dec-24 08:38 kptop-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1548 b- defN 22-Dec-24 08:38 kptop-0.0.5.dist-info/RECORD
-20 files, 277407 bytes uncompressed, 41833 bytes compressed:  84.9%
+Zip file size: 45505 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      442 b- defN 23-May-09 23:35 kptop_tool.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-09 17:17 kubePtop/__init__.py
+-rw-r--r--  2.0 unx     5483 b- defN 23-May-09 17:17 kubePtop/ascii_graph.py
+-rw-r--r--  2.0 unx     8249 b- defN 23-May-10 04:30 kubePtop/cli.py
+-rw-r--r--  2.0 unx      366 b- defN 23-May-09 17:17 kubePtop/colors.py
+-rw-r--r--  2.0 unx      531 b- defN 23-May-09 17:17 kubePtop/global_attrs.py
+-rw-r--r--  2.0 unx     3464 b- defN 23-May-09 17:17 kubePtop/helper.py
+-rw-r--r--  2.0 unx     1053 b- defN 23-May-09 17:17 kubePtop/logging.py
+-rw-r--r--  2.0 unx    58007 b- defN 23-May-10 04:33 kubePtop/node_metrics.py
+-rw-r--r--  2.0 unx    59849 b- defN 23-May-09 17:17 kubePtop/node_monitor.py
+-rw-r--r--  2.0 unx    53769 b- defN 23-May-09 17:17 kubePtop/pod_metrics.py
+-rw-r--r--  2.0 unx    36836 b- defN 23-May-10 04:41 kubePtop/pod_monitor.py
+-rw-r--r--  2.0 unx     2267 b- defN 23-May-09 17:17 kubePtop/read_env.py
+-rw-r--r--  2.0 unx    16760 b- defN 23-May-09 17:17 kubePtop/session.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-10 04:43 kptop-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      599 b- defN 23-May-10 04:43 kptop-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 04:43 kptop-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-May-10 04:43 kptop-0.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-May-10 04:43 kptop-0.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1549 b- defN 23-May-10 04:43 kptop-0.0.6.dist-info/RECORD
+20 files, 284527 bytes uncompressed, 43023 bytes compressed:  84.9%
```

## zipnote {}

```diff
@@ -36,26 +36,26 @@
 
 Filename: kubePtop/read_env.py
 Comment: 
 
 Filename: kubePtop/session.py
 Comment: 
 
-Filename: kptop-0.0.5.dist-info/LICENSE
+Filename: kptop-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: kptop-0.0.5.dist-info/METADATA
+Filename: kptop-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: kptop-0.0.5.dist-info/WHEEL
+Filename: kptop-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: kptop-0.0.5.dist-info/entry_points.txt
+Filename: kptop-0.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: kptop-0.0.5.dist-info/top_level.txt
+Filename: kptop-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: kptop-0.0.5.dist-info/RECORD
+Filename: kptop-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kptop_tool.py

```diff
@@ -1,6 +1,20 @@
 def run():
     # It runs at the initilization
     from kubePtop.cli import Cli
 
 
-run()
+run()
+
+# from kubePtop.node_metrics import PrometheusNodeMetrics
+# from kubePtop.read_env import ReadEnv
+# env = ReadEnv()
+# env.read_env()
+# import rich
+
+# test = PrometheusNodeMetrics()
+# rich.print(test.nodeManagedK8sInfo('.*'))
+# print(test.topNode())
+# test.topNodeTable(option="cloud")
+# test.topNodeJson('ip-10-129-143-105.eu-west-1.compute.internal')
+
+
```

## kubePtop/cli.py

```diff
@@ -32,35 +32,50 @@
         self.container = None
         self.namespace = "default"
         self.all_namespaces = False
         self.debug = False
         self.dashboard = 'default'
         self.list_dashboards = False
         self.sort_by_mem_usage = False
+        self.list_option = ''
+        self.list_nodes_option = []
+        self.colorize_json = False
+        
 
         # Read CLI arguments
         self.argparse()
 
 
         if self.debug:
             GlobalAttrs.debug = True
             Logging.log.setLevel(level="DEBUG")
 
         # kptop nodes <NODE-NAME>
         if self.node:
             if self.list_dashboards:
                 node_monitor.list_dashboards()
                 exit(0)
+            
+            # kptop nodes <NODE-NAME> -o json
+            if self.list_option == 'json':
+                node_metrics.topNodeJson(node=self.node, color=self.colorize_json)
+                exit(0)
             # Check if the node found.
             node_monitor.display_dashboard(dashboard=self.dashboard, node_name=self.node)
 
+        # kptop nodes
         if self.list_nodes:
-            node_metrics.topNodeTable()
+            # kptop nodes -o json
+            if self.list_option == 'json':
+                node_metrics.topNodeJson(node=".*", color=self.colorize_json)
+                exit(0)
+            node_metrics.topNodeTable(option=self.list_option)
             exit(0)
 
+
         # kptop pods <POD-NAME>
         if self.pod:
             if self.container is None:
                 self.container = ".*"
             # Check if the pod found.
             check_pod = pod_metrics.podExists(pod=self.pod, namespace=self.namespace)
             if not check_pod.get('result'):
@@ -86,30 +101,33 @@
             exit(0)
 
         # Print help if no args are provided.
         # self.parser.print_help()
 
     def argparse(self):
         parser = argparse.ArgumentParser(description='A Python tool for Kubernetes Nodes/Pods terminal monitoring through Prometheus metrics.')
-        parser.add_argument('top', type=str, nargs='*', metavar='{pods, pod, po}  |  {nodes, node}  |  {pvcs, pvc}', help='top pods/nodes/pvcs')
+        parser.add_argument('top', type=str, nargs='*', metavar='{pods, pod, po}  |  {nodes, node}  |  {persistentvolumeclaim, pvc}', help='top pods/nodes/persistentvolumeclaim')
         parser.add_argument('-n', '--namespace', type=str, required=False, metavar='', help='Specify a Kubernetes namespace')
         parser.add_argument('-A', '--all-namespaces', required=False, action='store_true', help='All Kubernetes namespaces')
         parser.add_argument('-c', '--container', type=str, required=False, metavar='', help='Monitor a specific Pod\'s container')
         parser.add_argument('-i', '--interval', type=int, required=False, metavar='', help='Live monitoring update interval')
         parser.add_argument('-V', '--verify-prometheus', required=False, action='store_true', help='Verify Prometheus connection & exporters')
         parser.add_argument('-C', '--check-metrics', required=False, action='store_true', help='Checks the availability of the needed metrics')
         parser.add_argument('-d', '--debug', required=False, action='store_true', help='Print debug output')
         parser.add_argument('-s', '--sort-by-mem-usage', required=False, action='store_true', help='Sort top result by memory usage')
+        parser.add_argument('-o', '--option', type=str, required=False, choices=['cloud', 'json'], help='options for "kptop node||pod" (currently supported in "kptop node")')
+        parser.add_argument('-cj', '--colorize-json', required=False, action='store_true', help='Colorize Json output (with "-o json")')
+        # parser.add_argument('-q', '--query', type=str, required=False, help='options for "Run a custom query')
 
         # parser.add_argument('-D', '--dashboard', type=str, required=False, metavar='', help='Specify a dashboard')
         # parser.add_argument('-L', '--list-dashboards', required=False, action='store_true', help='List available dashboards')
 
         pod_aliases = ['pod', 'pods', 'po']
         node_aliases = ['node', 'nodes']
-        pvc_aliases = ['pvc', 'pvcs']
+        pvc_aliases = ['pvc', 'persistentvolumeclaim']
 
         results = parser.parse_args()
         self.parser = parser
 
         if results.debug:
             self.debug = True
         
@@ -156,14 +174,20 @@
         if results.namespace and results.all_namespaces:
             rich.print("[bold]ERROR -- You can only use '--all-namespaces' or '--namespace' \n")
             self.parser.print_help()
             exit(1)
 
         if results.namespace:
             self.namespace = results.namespace
+            
+        if results.option:
+            self.list_option = results.option
+            
+        if results.colorize_json:
+            self.colorize_json = results.option
 
         if results.all_namespaces:
             self.all_namespaces = results.all_namespaces
 
         if results.container:
             self.container = results.container
```

## kubePtop/node_metrics.py

```diff
@@ -1,13 +1,15 @@
 from kubePtop.session import PrometheusAPI
 from kubePtop.global_attrs import GlobalAttrs
 from kubePtop.logging import Logging
 from kubePtop.helper import Helper
 from tabulate import tabulate
 from kubePtop.colors import Bcolors
+import json
+import rich
 bcolors = Bcolors()
 import traceback
 
 
 
 helper_ = Helper()
 
@@ -188,15 +190,15 @@
         """
         output = {
             "success": False,
             "fail_reason": "",
             "result": ""
         }
         try:
-            result = self.run_query(f'node_memory_MemTotal_bytes{{{GlobalAttrs.node_exporter_node_label}="{node}"}}')
+            result = self.run_query(f'node_memory_MemTotal_bytes{{{GlobalAttrs.node_exporter_node_label}=~"{node}"}}')
             if not result.get('status') == 'success':
                 output['fail_reason'] = "could not get metric value"
                 return output
 
             if not result.get('data').get('result'):
                 output['fail_reason'] = "metric did not return any data"
                 return output
@@ -1283,81 +1285,96 @@
     #         output['fail_reason'] = e
     #         Logging.log.error(e)
     #         Logging.log.exception(traceback.format_stack())
 
     #     return output
 
 
-    def topNode(self):
+    def topNode(self, node=".*"):
         """
         """
         output = {
             "success": False,
             "fail_reason": "",
             "result": {}
         }
         try:
-            
-            memory_total_query = f'node_memory_MemTotal_bytes' # f'machine_memory_bytes'
+            memory_total_query = f'node_memory_MemTotal_bytes{{{GlobalAttrs.node_exporter_node_label}=~"{node}"}}'
             memory_total = self.run_query(memory_total_query)
             if not memory_total.get('status') == 'success':
                 output['fail_reason'] = f"could not get metric's value: {memory_total_query}"
                 return output
             if not memory_total.get('data').get('result'):
                 output['fail_reason'] =  f"Query did not return any data: {memory_total_query}"
                 return output
 
-            memory_free_query = f'node_memory_MemFree_bytes'
+            nodes_dct = {}
+            for node_ in memory_total.get('data').get('result'):
+                nodes_dct[node_.get('metric').get(GlobalAttrs.node_exporter_node_label)] = {
+                    "memory_total": int(node_.get('value')[1]),
+                    "memory_free": -1,
+                    "memory_used": -1,
+                    "cpu_cores": -1,
+                    # "cpu_used": -1, # not sure of the metrics to get the used cpu in milicores.
+                    "cpu_used_percentage": -1,
+                    "running_pods_num": -1,
+                    "cluster": "",
+                    "node_os": "",
+                    "node_arch": "",
+                    "region": "",
+                    "az": "",
+                    "instance_type": "",
+                    "cluster_env": "Unknown",
+                    "node_group_capacity_type": "",
+                    "node_group_name": "",
+                }
+
+            memory_free_query = f'node_memory_MemFree_bytes{{{GlobalAttrs.node_exporter_node_label}=~"{node}"}}'
             memory_free = self.run_query(memory_free_query)
             if not memory_free.get('status') == 'success':
                 output['fail_reason'] = f"could not get metric's value: {memory_free_query}"
                 return output
             if not memory_free.get('data').get('result'):
                 output['fail_reason'] =  f"Query did not return any data: {memory_free_query}"
                 return output
 
-            cpu_cores_query = f'machine_cpu_cores'
+            cpu_cores_query = f'machine_cpu_cores{{kubernetes_io_hostname=~"{node}"}}'
             cpu_cores = self.run_query(cpu_cores_query)
             if not cpu_cores.get('status') == 'success':
                 output['fail_reason'] = f"could not get metric's value: {cpu_cores_query}"
                 return output
             if not cpu_cores.get('data').get('result'):
                 output['fail_reason'] =  f"Query did not return any data: {cpu_cores_query}"
                 return output
 
-            cpu_used_percentage_query =  f'100 - (avg by ({GlobalAttrs.node_exporter_node_label}) (rate(node_cpu_seconds_total{{mode="idle"}}[10m])) * 100)'
+            #### Fix
+            cpu_used_percentage_query =  f'100 - (avg by ({GlobalAttrs.node_exporter_node_label}) (rate(node_cpu_seconds_total{{mode="idle", {GlobalAttrs.node_exporter_node_label}=~"{node}"}}[10m])) * 100)'
             cpu_used_percentage = self.run_query(cpu_used_percentage_query)
             if not cpu_used_percentage.get('status') == 'success':
                 output['fail_reason'] = f"could not get metric's value: {cpu_used_percentage_query}"
                 return output
             if not cpu_used_percentage.get('data').get('result'):
                 output['fail_reason'] =  f"Query did not return any data: {cpu_used_percentage_query}"
                 return output
 
-            running_pods_count_query = f'kubelet_running_pods'
+            running_pods_count_query = f'kubelet_running_pods{{instance=~"{node}"}}'
             running_pods_count = self.run_query(running_pods_count_query)
             if not running_pods_count.get('status') == 'success':
                 output['fail_reason'] = f"could not get metric's value: {running_pods_count_query}"
                 return output
             if not running_pods_count.get('data').get('result'):
                 output['fail_reason'] =  f"Query did not return any data: {running_pods_count_query}"
                 return output
-
-            
-            nodes_dct = {}
-            for node in memory_total.get('data').get('result'):
-                nodes_dct[node.get('metric').get(GlobalAttrs.node_exporter_node_label)] = {
-                    "memory_total": int(node.get('value')[1]),
-                    "memory_free": -1,
-                    "memory_used": -1,
-                    "cpu_cores": -1,
-                    # "cpu_used": -1, # not sure of the metrics to get the used cpu in milicores.
-                    "cpu_used_percentage": -1,
-                    "running_pods_num": -1,
-                }
+                
+            ## 
+            node_managed_k8s_info = self.nodeManagedK8sInfo(node=node)
+            if not node_managed_k8s_info.get('success'):
+                output['fail_reason'] = node_managed_k8s_info.get('fail_reason')
+                return output
+        
             
             for node in memory_free.get('data').get('result'):
                 nodes_dct[node.get('metric').get(GlobalAttrs.node_exporter_node_label)]['memory_free'] = int(node.get('value')[1])
                 nodes_dct[node.get('metric').get(GlobalAttrs.node_exporter_node_label)]['memory_used'] = nodes_dct[node.get('metric').get(GlobalAttrs.node_exporter_node_label)]['memory_total'] - int(node.get('value')[1])
 
             for node in cpu_cores.get('data').get('result'):
                 try:
@@ -1369,44 +1386,143 @@
                 nodes_dct[node.get('metric').get(GlobalAttrs.node_exporter_node_label)]['cpu_used_percentage'] = float(node.get('value')[1])
 
             for node in running_pods_count.get('data').get('result'):
                 try:
                     nodes_dct[node.get('metric').get('instance')]['running_pods_num'] = int(node.get('value')[1])
                 except KeyError:
                     pass # A KeyError Exception is expected as this metric returns the value for the master nodes while other metrics dont.
+                    
+            
+            for node in node_managed_k8s_info.get('result'):
+                # General Labels (match different cloud providers)
+                try:
+                    nodes_dct[node.get('metric').get('instance')]['node_arch'] = node['metric']['beta_kubernetes_io_arch']
+                    nodes_dct[node.get('metric').get('instance')]['node_os'] = node['metric']['beta_kubernetes_io_os']
+                    nodes_dct[node.get('metric').get('instance')]['cluster'] = node['metric']['cluster']
+                    nodes_dct[node.get('metric').get('instance')]['region'] = node['metric']['topology_kubernetes_io_region']
+                    nodes_dct[node.get('metric').get('instance')]['az'] = node['metric']['topology_kubernetes_io_zone']
+                    nodes_dct[node.get('metric').get('instance')]['instance_type'] = node['metric']['node_kubernetes_io_instance_type']
+                except KeyError:
+                    pass # If labels are not found, means that most probably this is a Local cluster
+                
+                # AWS Labels
+                try:
+                    nodes_dct[node.get('metric').get('instance')]['node_group_capacity_type'] = node['metric']['eks_amazonaws_com_capacityType']
+                    nodes_dct[node.get('metric').get('instance')]['node_group_name'] = node['metric']['eks_amazonaws_com_nodegroup']
+                    if nodes_dct[node.get('metric').get('instance')]['node_group_name']:
+                        nodes_dct[node.get('metric').get('instance')]['cluster_env'] = 'EKS'
+                except KeyError:
+                    pass # If labels are not found, means that it's not an EKS cluster.
+            
 
             output['result'] = nodes_dct
             output['success'] = True
 
         except(KeyError, AttributeError) as e:
             output['success']: False
             output['fail_reason'] = e
             Logging.log.error(e)
             Logging.log.exception(traceback.format_stack())
 
         return output
+    
+    def topNodeJson(self, node=".*", color=False):
+        nodes_dct = self.topNode(node=node)
+        if not nodes_dct.get('success'):
+            print(f"ERROR -- Failed to get nodes \n{nodes_dct.get('fail_reason')}")
+            exit(1)
+            
+        if color:
+            rich.print_json(data=nodes_dct.get('result'))
+        else:
+            print(json.dumps(nodes_dct.get('result'), indent=4))
 
 
-    def topNodeTable(self):
+    def topNodeTable(self, option=""):
         """
         """
         nodes_json = self.topNode()
         # import rich
         # rich.print(nodes_json)
         if not nodes_json.get('success'):
             print(f"No nodes found \n{bcolors.WARNING + str(nodes_json.get('fail_reason')) + bcolors.ENDC}")
             exit(1)
 
 
         table = [['NODE', 'MEM TOTAL', 'MEM USAGE', 'MEM FREE', 'CPU CORES', 'CPU USAGE%', 'RUNNING PODS' ]]
-        for  node, value in nodes_json.get('result').items():
-            row = [node, helper_.bytes_to_kb_mb_gb(value.get('memory_total')), helper_.bytes_to_kb_mb_gb(value.get('memory_used')), helper_.bytes_to_kb_mb_gb(value.get('memory_free')), value.get('cpu_cores'), str(round(value.get('cpu_used_percentage'))) + "%", value.get('running_pods_num')]
-            table.append(row)
+        if option == 'cloud':
+            table = [['NODE', 'MEM TOTAL', 'MEM USAGE', 'MEM FREE', 'CPU CORES', 'CPU USAGE%', 'RUNNING PODS', 'CLUSTER', 'INSTANCE TYPE', 'AZ', 'ENV', 'NG CAPACITY TYPE']]
+            
+        if option == 'cloud':
+            for  node, value in nodes_json.get('result').items():
+                row = [
+                        node,
+                        helper_.bytes_to_kb_mb_gb(value.get('memory_total')),
+                        helper_.bytes_to_kb_mb_gb(value.get('memory_used')),
+                        helper_.bytes_to_kb_mb_gb(value.get('memory_free')),
+                        value.get('cpu_cores'),
+                        str(round(value.get('cpu_used_percentage'))) + "%", 
+                        value.get('running_pods_num'),
+                        value.get('cluster'),
+                        value.get('instance_type'),
+                        # value.get('region'),
+                        value.get('az'),
+                        value.get('cluster_env'),
+                        value.get('node_group_capacity_type'),
+                        # value.get('node_group_name'),
+                    ]
+                table.append(row)
+        else:
+            for  node, value in nodes_json.get('result').items():
+                row = [
+                        node,
+                        helper_.bytes_to_kb_mb_gb(value.get('memory_total')),
+                        helper_.bytes_to_kb_mb_gb(value.get('memory_used')),
+                        helper_.bytes_to_kb_mb_gb(value.get('memory_free')),
+                        value.get('cpu_cores'),
+                        str(round(value.get('cpu_used_percentage'))) + "%", 
+                        value.get('running_pods_num'),
+                    ]
+                table.append(row)
+                
         out = tabulate(table, headers='firstrow', tablefmt='plain', showindex=False)
         print(out)
         
 
+    def nodeManagedK8sInfo(self, node):
+        """
+        INPUT:
+            - K8s node name (str)
+        Return:
+            - dct of metric (dct)
+        """
+        output = {
+            "success": False,
+            "fail_reason": "",
+            "result": {}
+        }
+        try:
+            query = f'kubelet_node_name{{kubernetes_io_hostname=~"{node}"}}'
+            result = self.run_query(query)
+            if not result.get('status') == 'success':
+                output['fail_reason'] =  f"could not get metric's value: \n{query}"
+                return output
 
-        
+            if not result.get('data').get('result'):
+                output['fail_reason'] = f"Query did not return any data: \n{query}"
+                return output
+
+            output['result'] = result.get('data').get('result')
+            output['success'] = True
+
+        except(KeyError, AttributeError) as e:
+            output['success']: False
+            output['fail_reason'] = e
+            Logging.log.error(e)
+            Logging.log.exception(traceback.format_stack())
+
+        return output 
+    
+
```

## kubePtop/pod_monitor.py

```diff
@@ -552,15 +552,15 @@
                     group_disk_io = Group(
                         Markdown("Bytes Read", justify='center'),
                         Text.from_ansi(disk_read_bytes_graph.graph + f"\n {disk_read_bytes_graph.colors_description_str}"),
                         Rule(style='#AAAAAA'),
                         Markdown("Bytes Write", justify='center'),
                         Text.from_ansi(disk_write_bytes_graph.graph + f"\n {disk_write_bytes_graph.colors_description_str}"),
                     )
-                    layout["body2_b_a"].update(Panel(group_disk_io, title="[b]Network IO", padding=(1, 1)))
+                    layout["body2_b_a"].update(Panel(group_disk_io, title="[b]Disk IO", padding=(1, 1)))
 
 
 
 
                     
                     time.sleep(GlobalAttrs.live_update_interval)
         except Exception as e:
```

## Comparing `kptop-0.0.5.dist-info/LICENSE` & `kptop-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

