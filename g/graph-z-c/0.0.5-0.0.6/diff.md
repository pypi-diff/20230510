# Comparing `tmp/graph_z_c-0.0.5.tar.gz` & `tmp/graph_z_c-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_z_c-0.0.5.tar", last modified: Tue May  9 13:41:03 2023, max compression
+gzip compressed data, was "graph_z_c-0.0.6.tar", last modified: Wed May 10 11:46:39 2023, max compression
```

## Comparing `graph_z_c-0.0.5.tar` & `graph_z_c-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:41:03.557340 graph_z_c-0.0.5/
--rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-09 13:41:03.557155 graph_z_c-0.0.5/PKG-INFO
--rw-r--r--   0 zelpha     (501) staff       (20)        0 2023-05-08 02:13:18.000000 graph_z_c-0.0.5/README.md
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:41:03.556443 graph_z_c-0.0.5/graph_z/
--rw-r--r--   0 zelpha     (501) staff       (20)       73 2023-05-09 13:29:04.000000 graph_z_c-0.0.5/graph_z/__init__.py
--rw-r--r--   0 zelpha     (501) staff       (20)     4697 2023-05-09 13:38:40.000000 graph_z_c-0.0.5/graph_z/graph_z.py
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:41:03.556968 graph_z_c-0.0.5/graph_z_c.egg-info/
--rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-09 13:41:03.000000 graph_z_c-0.0.5/graph_z_c.egg-info/PKG-INFO
--rw-r--r--   0 zelpha     (501) staff       (20)      189 2023-05-09 13:41:03.000000 graph_z_c-0.0.5/graph_z_c.egg-info/SOURCES.txt
--rw-r--r--   0 zelpha     (501) staff       (20)        1 2023-05-09 13:41:03.000000 graph_z_c-0.0.5/graph_z_c.egg-info/dependency_links.txt
--rw-r--r--   0 zelpha     (501) staff       (20)        8 2023-05-09 13:41:03.000000 graph_z_c-0.0.5/graph_z_c.egg-info/top_level.txt
--rw-r--r--   0 zelpha     (501) staff       (20)       38 2023-05-09 13:41:03.557389 graph_z_c-0.0.5/setup.cfg
--rw-r--r--   0 zelpha     (501) staff       (20)      174 2023-05-09 13:40:49.000000 graph_z_c-0.0.5/setup.py
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-10 11:46:39.844617 graph_z_c-0.0.6/
+-rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-10 11:46:39.844354 graph_z_c-0.0.6/PKG-INFO
+-rw-r--r--   0 zelpha     (501) staff       (20)        0 2023-05-08 02:13:18.000000 graph_z_c-0.0.6/README.md
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-10 11:46:39.842821 graph_z_c-0.0.6/graph_z/
+-rw-r--r--   0 zelpha     (501) staff       (20)       73 2023-05-09 13:29:04.000000 graph_z_c-0.0.6/graph_z/__init__.py
+-rw-r--r--   0 zelpha     (501) staff       (20)     5452 2023-05-10 11:44:56.000000 graph_z_c-0.0.6/graph_z/graph_z.py
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-10 11:46:39.844100 graph_z_c-0.0.6/graph_z_c.egg-info/
+-rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-10 11:46:39.000000 graph_z_c-0.0.6/graph_z_c.egg-info/PKG-INFO
+-rw-r--r--   0 zelpha     (501) staff       (20)      189 2023-05-10 11:46:39.000000 graph_z_c-0.0.6/graph_z_c.egg-info/SOURCES.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)        1 2023-05-10 11:46:39.000000 graph_z_c-0.0.6/graph_z_c.egg-info/dependency_links.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)        8 2023-05-10 11:46:39.000000 graph_z_c-0.0.6/graph_z_c.egg-info/top_level.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)       38 2023-05-10 11:46:39.844680 graph_z_c-0.0.6/setup.cfg
+-rw-r--r--   0 zelpha     (501) staff       (20)      174 2023-05-10 11:46:20.000000 graph_z_c-0.0.6/setup.py
```

### Comparing `graph_z_c-0.0.5/graph_z/graph_z.py` & `graph_z_c-0.0.6/graph_z/graph_z.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,28 +8,26 @@
 def get_distance(p1, p2):
     return np.sqrt(sum([(p2_coordinate - p1_coordinate) ** 2 for p1_coordinate, p2_coordinate in zip(p1, p2)]))
 
 def get_midpoint(p1, p2):
     return ((p1[0]+p2[0])/2, (p1[1]+p2[1])/2)
 
 
-
 def plot_line_segment(p1, p2, scaling_factor=1):
     L = get_distance(p1, p2)
     p2_m = ((p1[0]*(1-scaling_factor) + p2[0]*scaling_factor), (p1[1]*(1-scaling_factor) + p2[1]*scaling_factor))
     plt.arrow(p1[0], p1[1], p2_m[0], p2_m[1], head_width=0, color='black')
 
 
 
 class Vertex():
     def __init__(self, id, value, paths=None):
         self.id = id
         self.value = value
         self.paths = paths or []
-        self.circle_coordinates = (0, 0)
 
 class Graph:
     def __init__(self, vertices=[]):
         self.vertices = vertices
         self.ids = []
         self.all_paths = []
         for vertex in vertices:
@@ -48,15 +46,15 @@
         self.ids.append(vertex.id)
 
     def get_vertex(self, id):
         for vertex in self.vertices:
             if vertex.id == id:
                 return vertex
 
-    def add_path(self, id1, id2, path_cost):
+    def add_path(self, id1, id2, path_cost, message=True):
         if id1 not in self.ids or id2 not in self.ids:
             print("Vertices with the given ids do not exist in this graph")
             return None
 
         vertex1, vertex2 = self.get_vertex(id1), self.get_vertex(id2)
         existance_of_copy = False
         for i, path in enumerate(self.all_paths):
@@ -68,45 +66,59 @@
         if existance_of_copy:
             vertex1.paths[vertex1.paths.index((id2, previous_cost))] = (id2, path_cost)
             vertex2.paths[vertex2.paths.index((id1, previous_cost))] = (id1, path_cost)
         else:
             self.all_paths.append((id1, id2, path_cost))
             vertex1.paths.append((id2, path_cost))
             vertex2.paths.append((id1, path_cost))
-
-        print("Path added succesfully")
+        if message:
+            print("Path added succesfully")
 
 
     def bar_visuals(self):
         values = [vertex.value for vertex in self.vertices]
         sns.barplot(pd.DataFrame({
             'IDs': self.ids,
             'Values': values
         }), x='IDs', y='Values')
 
 
-    def plot_graph(self):
+    def plot_graph(self, show_path=True):
         fig, ax = plt.subplots()
         ax.set_aspect('equal')
 
-        n = len(self.vertices)
-        theta = np.linspace(0, 2*np.pi, n, endpoint=False)
-        x, y = np.cos(theta), np.sin(theta)
-
+        num_vertices = len(self.vertices)
+        num_circles = int(np.floor(num_vertices/4))
+        extras = num_vertices%4
+        theta = np.linspace(0, 2*np.pi, 4, endpoint=False)
+        theta_last = np.linspace(0, 2*np.pi, extras, endpoint=False)
+        x, y = np.array([]), np.array([])
+        for r in range(1, num_circles+1):
+            if r%2 != 0:
+                x = np.concatenate((x, r*np.cos(theta)))
+                y = np.concatenate((y, r*np.sin(theta)))
+            else:
+                x = np.concatenate((x, r*np.cos(theta + np.pi/4)))
+                y = np.concatenate((y, r*np.sin(theta + np.pi/4)))
+            
+        x = np.concatenate((x, (num_circles+1)*np.cos(theta_last)))
+        y = np.concatenate((y, (num_circles+1)*np.sin(theta_last)))
+                        
         # Plot the vertices
         ax.scatter(x, y)
         for i, vertex in enumerate(self.vertices):
             ax.annotate(f"{vertex.id}:{vertex.value}", (x[i], y[i]))
 
-        # Plot the edges
-        for id1, id2, cost in self.all_paths:
-            vertex1, vertex2 = self.get_vertex(id1), self.get_vertex(id2)
-            i1, i2 = self.ids.index(id1), self.ids.index(id2)
-            ax.plot([x[i1], x[i2]], [y[i1], y[i2]])
-            ax.annotate(cost, ((x[i1]+x[i2])/2, (y[i1]+y[i2])/2))
+        if show_path:
+            # Plot the edges
+            for id1, id2, cost in self.all_paths:
+                vertex1, vertex2 = self.get_vertex(id1), self.get_vertex(id2)
+                i1, i2 = self.ids.index(id1), self.ids.index(id2)
+                ax.plot([x[i1], x[i2]], [y[i1], y[i2]], color='black')
+                ax.annotate(cost, ((x[i1]+x[i2])/2, (y[i1]+y[i2])/2))
 
         plt.show()
 
     def get_detailed_dataframe(self):
         values = []
         paths = []
         for vertex in self.vertices:
@@ -132,15 +144,15 @@
         vertex = Vertex(vertex_ids[i], vertex_values[i])
         graph.add_vertex(vertex)
     
     path_costs = np.random.randint(*path_cost_range, size=num_paths)
     for i in range(num_paths):
         vertex_ids = [v.id for v in graph.vertices]  # get list of vertex IDs in the graph
         rand_id1, rand_id2 = np.random.choice(vertex_ids, size=2, replace=False)
-        graph.add_path(rand_id1, rand_id2, path_costs[i])
+        graph.add_path(rand_id1, rand_id2, path_costs[i], message=False)
     
     return graph
```

