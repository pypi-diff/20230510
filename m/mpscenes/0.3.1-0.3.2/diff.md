# Comparing `tmp/mpscenes-0.3.1.tar.gz` & `tmp/mpscenes-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpscenes-0.3.1.tar", max compression
+gzip compressed data, was "mpscenes-0.3.2.tar", max compression
```

## Comparing `mpscenes-0.3.1.tar` & `mpscenes-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0       71 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/.__init__.py
--rw-r--r--   0        0        0       71 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/__init__.py
--rw-r--r--   0        0        0     1214 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/common/analytic_trajectory.py
--rw-r--r--   0        0        0     1889 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/common/component.py
--rw-r--r--   0        0        0      432 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/common/errors.py
--rw-r--r--   0        0        0      368 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/common/reference_trajectory.py
--rw-r--r--   0        0        0     3418 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/common/spline_trajectory.py
--rw-r--r--   0        0        0     7901 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/goals/dynamic_sub_goal.py
--rw-r--r--   0        0        0     3392 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/goals/goal_composition.py
--rw-r--r--   0        0        0     2154 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/goals/static_joint_space_sub_goal.py
--rw-r--r--   0        0        0     7825 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/goals/static_sub_goal.py
--rw-r--r--   0        0        0     2094 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/goals/sub_goal.py
--rw-r--r--   0        0        0      905 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/goals/sub_goal_creator.py
--rw-r--r--   0        0        0     5742 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/box_obstacle.py
--rw-r--r--   0        0        0       14 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/box_smooth.mtl
--rw-r--r--   0        0        0      836 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/box_smooth.obj
--rw-r--r--   0        0        0     2143 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/collision_obstacle.py
--rw-r--r--   0        0        0     4828 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/cylinder_obstacle.py
--rw-r--r--   0        0        0     1227 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/dynamic_box_obstacle.py
--rw-r--r--   0        0        0     1312 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/dynamic_cylinder_obstacle.py
--rw-r--r--   0        0        0     3624 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/dynamic_obstacle.py
--rw-r--r--   0        0        0     1278 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/dynamic_sphere_obstacle.py
--rw-r--r--   0        0        0     1244 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/dynamic_urdf_obstacle.py
--rw-r--r--   0        0        0      817 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/obstacleCreator.py
--rw-r--r--   0        0        0     4699 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/sphere_obstacle.py
--rw-r--r--   0        0        0      136 2023-02-22 09:25:33.252473 mpscenes-0.3.1/mpscenes/obstacles/sphere_smooth.mtl
--rw-r--r--   0        0        0   111602 2023-02-22 09:25:33.256473 mpscenes-0.3.1/mpscenes/obstacles/sphere_smooth.obj
--rw-r--r--   0        0        0     2097 2023-02-22 09:25:33.256473 mpscenes-0.3.1/mpscenes/obstacles/urdf_obstacle.py
--rw-r--r--   0        0        0      597 2023-02-22 09:25:33.256473 mpscenes-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 mpscenes-0.3.1/setup.py
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 mpscenes-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-05-10 07:27:54.952210 mpscenes-0.3.2/mpscenes/.__init__.py
+-rw-r--r--   0        0        0       71 2023-05-10 07:27:54.952210 mpscenes-0.3.2/mpscenes/__init__.py
+-rw-r--r--   0        0        0     1214 2023-05-10 07:27:54.952210 mpscenes-0.3.2/mpscenes/common/analytic_trajectory.py
+-rw-r--r--   0        0        0     1889 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/common/component.py
+-rw-r--r--   0        0        0      495 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/common/errors.py
+-rw-r--r--   0        0        0      368 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/common/reference_trajectory.py
+-rw-r--r--   0        0        0     3418 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/common/spline_trajectory.py
+-rw-r--r--   0        0        0     7901 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/dynamic_sub_goal.py
+-rw-r--r--   0        0        0     3392 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/goal_composition.py
+-rw-r--r--   0        0        0     2154 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/static_joint_space_sub_goal.py
+-rw-r--r--   0        0        0     7825 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/static_sub_goal.py
+-rw-r--r--   0        0        0     2094 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/sub_goal.py
+-rw-r--r--   0        0        0      905 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/sub_goal_creator.py
+-rw-r--r--   0        0        0     6021 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/box_obstacle.py
+-rw-r--r--   0        0        0       14 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/box_smooth.mtl
+-rw-r--r--   0        0        0      836 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/box_smooth.obj
+-rw-r--r--   0        0        0     2353 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/collision_obstacle.py
+-rw-r--r--   0        0        0     5152 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/cylinder_obstacle.py
+-rw-r--r--   0        0        0     1227 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/dynamic_box_obstacle.py
+-rw-r--r--   0        0        0     1312 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/dynamic_cylinder_obstacle.py
+-rw-r--r--   0        0        0     3624 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/dynamic_obstacle.py
+-rw-r--r--   0        0        0     1278 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/dynamic_sphere_obstacle.py
+-rw-r--r--   0        0        0     1244 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/dynamic_urdf_obstacle.py
+-rw-r--r--   0        0        0      817 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/obstacleCreator.py
+-rw-r--r--   0        0        0     4864 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/sphere_obstacle.py
+-rw-r--r--   0        0        0      136 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/sphere_smooth.mtl
+-rw-r--r--   0        0        0   111602 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/sphere_smooth.obj
+-rw-r--r--   0        0        0     2255 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/urdf_obstacle.py
+-rw-r--r--   0        0        0      597 2023-05-10 07:27:54.956210 mpscenes-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 mpscenes-0.3.2/PKG-INFO
```

### Comparing `mpscenes-0.3.1/mpscenes/common/analytic_trajectory.py` & `mpscenes-0.3.2/mpscenes/common/analytic_trajectory.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/common/component.py` & `mpscenes-0.3.2/mpscenes/common/component.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/common/spline_trajectory.py` & `mpscenes-0.3.2/mpscenes/common/spline_trajectory.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/goals/dynamic_sub_goal.py` & `mpscenes-0.3.2/mpscenes/goals/dynamic_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/goals/goal_composition.py` & `mpscenes-0.3.2/mpscenes/goals/goal_composition.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/goals/static_joint_space_sub_goal.py` & `mpscenes-0.3.2/mpscenes/goals/static_joint_space_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/goals/static_sub_goal.py` & `mpscenes-0.3.2/mpscenes/goals/static_sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/goals/sub_goal.py` & `mpscenes-0.3.2/mpscenes/goals/sub_goal.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/goals/sub_goal_creator.py` & `mpscenes-0.3.2/mpscenes/goals/sub_goal_creator.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/box_obstacle.py` & `mpscenes-0.3.2/mpscenes/obstacles/box_obstacle.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,14 +126,19 @@
 
     def movable(self):
         return self._config.movable
 
     def csv(self, file_name, samples=100):
         pass
 
+    def distance(self, position: np.ndarray) -> float:
+        pos = self.position_into_obstacle_frame(position)
+        q = np.absolute(pos) - np.array(self.size())/2.0
+        return np.linalg.norm(np.maximum(q, 0)) + np.minimum(np.maximum(q[0], np.maximum(q[1], q[2])), 0.0)
+
     def render_gym(self, viewer, rendering, **kwargs):
         if self.dimension() != 2:
             raise DimensionNotSuitableForEnv(
                 "PlanarGym only supports two dimensional obstacles"
             )
         x = self.position()
         tf = rendering.Transform(rotation=0, translation=(x[0], x[1]))
```

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/box_smooth.obj` & `mpscenes-0.3.2/mpscenes/obstacles/box_smooth.obj`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/collision_obstacle.py` & `mpscenes-0.3.2/mpscenes/obstacles/collision_obstacle.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,10 +76,17 @@
 
     def movable(self):
         return self._config.movable
 
     def update_bullet_position(self, pybullet, **kwargs):
         pass
 
+    def position_into_obstacle_frame(self, position: np.ndarray) -> np.ndarray:
+        return position - self.position()
+
+    @abstractmethod
+    def distance(self, position: np.array) -> float:
+        pass
+
     @abstractmethod
     def size(self):
         pass
```

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/cylinder_obstacle.py` & `mpscenes-0.3.2/mpscenes/obstacles/cylinder_obstacle.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,14 +114,21 @@
 
     def movable(self):
         return self._config.movable
 
     def csv(self, file_name, samples=100):
         pass
 
+    def distance(self, position) -> float:
+        pos = self.position_into_obstacle_frame(position)
+        pos[2] += self.size()[1]/2
+        d = np.absolute(np.array([np.linalg.norm(pos[0:2]), pos[2]])) - np.array(self.size())
+        return np.minimum(np.maximum(d[0], d[1]), 0.0) + np.linalg.norm(np.maximum(d, 0.0))
+
+
     def render_gym(self, viewer, rendering, **kwargs):
         pass
 
     def add_to_bullet(self, pybullet) -> int:
         if self.dimension() == 2:
             base_position = self.position().tolist() + [0.0]
         elif self.dimension() == 3:
```

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/dynamic_box_obstacle.py` & `mpscenes-0.3.2/mpscenes/obstacles/dynamic_box_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/dynamic_cylinder_obstacle.py` & `mpscenes-0.3.2/mpscenes/obstacles/dynamic_cylinder_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/dynamic_obstacle.py` & `mpscenes-0.3.2/mpscenes/obstacles/dynamic_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/dynamic_sphere_obstacle.py` & `mpscenes-0.3.2/mpscenes/obstacles/dynamic_sphere_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/dynamic_urdf_obstacle.py` & `mpscenes-0.3.2/mpscenes/obstacles/dynamic_urdf_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/obstacleCreator.py` & `mpscenes-0.3.2/mpscenes/obstacles/obstacleCreator.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/sphere_obstacle.py` & `mpscenes-0.3.2/mpscenes/obstacles/sphere_obstacle.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,18 @@
         x = self.position()[0] + (self.radius() - 0.1) * np.cos(theta)
         y = self.position()[1] + (self.radius() - 0.1) * np.sin(theta)
         with open(file_name, mode="w") as file:
             csv_writer = csv.writer(file, delimiter=",")
             for i in range(2 * samples):
                 csv_writer.writerow([x[i], y[i]])
 
+    def distance(self, position: np.ndarray) -> float:
+        pos = self.position_into_obstacle_frame(position)
+        return np.linalg.norm(pos) - self.radius()
+
     def render_gym(self, viewer, rendering, **kwargs):
         if self.dimension() != 2:
             raise DimensionNotSuitableForEnv(
                 "PlanarGym only supports two dimensional obstacles"
             )
         x = self.position(t=t)
         tf = rendering.Transform(rotation=0, translation=(x[0], x[1]))
```

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/sphere_smooth.obj` & `mpscenes-0.3.2/mpscenes/obstacles/sphere_smooth.obj`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.1/mpscenes/obstacles/urdf_obstacle.py` & `mpscenes-0.3.2/mpscenes/obstacles/urdf_obstacle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import List, Optional
 import numpy as np
 from omegaconf import OmegaConf
 
 from mpscenes.obstacles.collision_obstacle import CollisionObstacle, CollisionObstacleConfig, GeometryConfig
-from mpscenes.common.errors import ComponentIncompleteError, DimensionNotSuitableForEnv
+from mpscenes.common.errors import NoDistanceFunctionForURDFObstacle, DimensionNotSuitableForEnv
 
 
 @dataclass
 class UrdfGeometryConfig(GeometryConfig):
     pass
 
 
@@ -60,14 +60,17 @@
 
     def acceleration(self):
         return np.zeros(3)
 
     def dimension(self):
         return len(self._config.geometry.position)
 
+    def distance(self, position: np.ndarray) -> None:
+        raise NoDistanceFunctionForURDFObstacle("Cannot compute distance for urdf-obstacle.")
+
     def add_to_bullet(self, pybullet) -> int:
         if self.dimension() != 3:
             raise DimensionNotSuitableForEnv(
                 "Pybullet only supports three dimensional obstacles"
             )
         self._bullet_id = pybullet.loadURDF(
             fileName=self.urdf(),
```

### Comparing `mpscenes-0.3.1/pyproject.toml` & `mpscenes-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpscenes"
-version = "0.3.1"
+version = "0.3.2"
 description = "Generic motion planning scenes, including goals and obstacles."
 authors = ["Max <m.spahn@tudelft.nl>"]
   
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.22.0"
```

### Comparing `mpscenes-0.3.1/PKG-INFO` & `mpscenes-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpscenes
-Version: 0.3.1
+Version: 0.3.2
 Summary: Generic motion planning scenes, including goals and obstacles.
 Author: Max
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

