# Comparing `tmp/mpscenes-0.3.2.tar.gz` & `tmp/mpscenes-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpscenes-0.3.2.tar", max compression
+gzip compressed data, was "mpscenes-0.4.0.tar", max compression
```

## Comparing `mpscenes-0.3.2.tar` & `mpscenes-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0       71 2023-05-10 07:27:54.952210 mpscenes-0.3.2/mpscenes/.__init__.py
--rw-r--r--   0        0        0       71 2023-05-10 07:27:54.952210 mpscenes-0.3.2/mpscenes/__init__.py
--rw-r--r--   0        0        0     1214 2023-05-10 07:27:54.952210 mpscenes-0.3.2/mpscenes/common/analytic_trajectory.py
--rw-r--r--   0        0        0     1889 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/common/component.py
--rw-r--r--   0        0        0      495 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/common/errors.py
--rw-r--r--   0        0        0      368 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/common/reference_trajectory.py
--rw-r--r--   0        0        0     3418 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/common/spline_trajectory.py
--rw-r--r--   0        0        0     7901 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/dynamic_sub_goal.py
--rw-r--r--   0        0        0     3392 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/goal_composition.py
--rw-r--r--   0        0        0     2154 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/static_joint_space_sub_goal.py
--rw-r--r--   0        0        0     7825 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/static_sub_goal.py
--rw-r--r--   0        0        0     2094 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/sub_goal.py
--rw-r--r--   0        0        0      905 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/goals/sub_goal_creator.py
--rw-r--r--   0        0        0     6021 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/box_obstacle.py
--rw-r--r--   0        0        0       14 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/box_smooth.mtl
--rw-r--r--   0        0        0      836 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/box_smooth.obj
--rw-r--r--   0        0        0     2353 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/collision_obstacle.py
--rw-r--r--   0        0        0     5152 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/cylinder_obstacle.py
--rw-r--r--   0        0        0     1227 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/dynamic_box_obstacle.py
--rw-r--r--   0        0        0     1312 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/dynamic_cylinder_obstacle.py
--rw-r--r--   0        0        0     3624 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/dynamic_obstacle.py
--rw-r--r--   0        0        0     1278 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/dynamic_sphere_obstacle.py
--rw-r--r--   0        0        0     1244 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/dynamic_urdf_obstacle.py
--rw-r--r--   0        0        0      817 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/obstacleCreator.py
--rw-r--r--   0        0        0     4864 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/sphere_obstacle.py
--rw-r--r--   0        0        0      136 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/sphere_smooth.mtl
--rw-r--r--   0        0        0   111602 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/sphere_smooth.obj
--rw-r--r--   0        0        0     2255 2023-05-10 07:27:54.956210 mpscenes-0.3.2/mpscenes/obstacles/urdf_obstacle.py
--rw-r--r--   0        0        0      597 2023-05-10 07:27:54.956210 mpscenes-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 mpscenes-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       71 2023-05-10 09:47:35.022060 mpscenes-0.4.0/mpscenes/.__init__.py
+-rw-r--r--   0        0        0       71 2023-05-10 09:47:35.022060 mpscenes-0.4.0/mpscenes/__init__.py
+-rw-r--r--   0        0        0     1161 2023-05-10 09:47:35.022060 mpscenes-0.4.0/mpscenes/common/analytic_trajectory.py
+-rw-r--r--   0        0        0     1684 2023-05-10 09:47:35.022060 mpscenes-0.4.0/mpscenes/common/component.py
+-rw-r--r--   0        0        0      500 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/common/errors.py
+-rw-r--r--   0        0        0      755 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/common/reference_trajectory.py
+-rw-r--r--   0        0        0     3271 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/common/spline_trajectory.py
+-rw-r--r--   0        0        0     3314 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/dynamic_sub_goal.py
+-rw-r--r--   0        0        0     2513 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/goal_composition.py
+-rw-r--r--   0        0        0     1961 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/static_joint_space_sub_goal.py
+-rw-r--r--   0        0        0     2642 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/static_sub_goal.py
+-rw-r--r--   0        0        0     1958 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/sub_goal.py
+-rw-r--r--   0        0        0      905 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/goals/sub_goal_creator.py
+-rw-r--r--   0        0        0     4045 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/box_obstacle.py
+-rw-r--r--   0        0        0       14 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/box_smooth.mtl
+-rw-r--r--   0        0        0      836 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/box_smooth.obj
+-rw-r--r--   0        0        0     2217 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/collision_obstacle.py
+-rw-r--r--   0        0        0     3747 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/cylinder_obstacle.py
+-rw-r--r--   0        0        0     1227 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/dynamic_box_obstacle.py
+-rw-r--r--   0        0        0     1312 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/dynamic_cylinder_obstacle.py
+-rw-r--r--   0        0        0     2901 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/dynamic_obstacle.py
+-rw-r--r--   0        0        0     1278 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/dynamic_sphere_obstacle.py
+-rw-r--r--   0        0        0     1244 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/dynamic_urdf_obstacle.py
+-rw-r--r--   0        0        0      817 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/obstacleCreator.py
+-rw-r--r--   0        0        0     3092 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/sphere_obstacle.py
+-rw-r--r--   0        0        0      136 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/sphere_smooth.mtl
+-rw-r--r--   0        0        0   111602 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/sphere_smooth.obj
+-rw-r--r--   0        0        0     1833 2023-05-10 09:47:35.026060 mpscenes-0.4.0/mpscenes/obstacles/urdf_obstacle.py
+-rw-r--r--   0        0        0      551 2023-05-10 09:47:35.026060 mpscenes-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 mpscenes-0.4.0/PKG-INFO
```

### Comparing `mpscenes-0.3.2/mpscenes/common/component.py` & `mpscenes-0.4.0/mpscenes/common/component.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from abc import ABC
 import yaml
 from omegaconf import OmegaConf
 
-from mpscenes.common.errors import ComponentIncompleteError, DimensionNotSuitableForEnv
+from mpscenes.common.errors import (
+    ComponentIncompleteError,
+    DimensionNotSuitableForEnv,
+)
 
 
 class MPComponent(ABC):
-
     def __init__(self, **kwargs):
-        schema = kwargs.get('schema')
-        if 'content_dict' in kwargs and 'name' in kwargs:
-            self._content_dict = kwargs.get('content_dict')
-            self._name = kwargs.get('name')
-        elif 'file_name' in kwargs:
-            with open(kwargs.get('file_name'), 'r') as stream:
+        schema = kwargs.get("schema")
+        if "content_dict" in kwargs and "name" in kwargs:
+            self._content_dict = kwargs.get("content_dict")
+            self._name = kwargs.get("name")
+        elif "file_name" in kwargs:
+            with open(kwargs.get("file_name"), "r") as stream:
                 self._content_dict = yaml.safe_load(stream)
-            self._name = self._content_dict['name']
-            del self._content_dict['name']
+            self._name = self._content_dict["name"]
+            del self._content_dict["name"]
         self._config = OmegaConf.create(self._content_dict)
         config = OmegaConf.create(self._content_dict)
         self._config = OmegaConf.merge(schema, config)
 
     def check_completeness(self):
         pass
         """
@@ -44,16 +46,7 @@
                 result[mask_entry] = getattr(self, mask_entry)(t=t)
             except TypeError as _:
                 result[mask_entry] = getattr(self, mask_entry)()
         return result
 
     def dict(self):
         return OmegaConf.to_container(self._config)
-
-    def add_to_bullet(self, pybullet, position=[0.0, 0.0, 0.0]) -> int:
-        """Adds component to pybullet instance.
-
-        Returns
-        ----------
-        int: multi_body_identifier
-        """
-        pass
```

### Comparing `mpscenes-0.3.2/mpscenes/common/spline_trajectory.py` & `mpscenes-0.4.0/mpscenes/common/spline_trajectory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,83 @@
 import numpy as np
 
 from geomdl import BSpline
 from geomdl import utilities
 import logging
 
-from mpscenes.common.reference_trajectory import ReferenceTrajectory
 from mpscenes.common.errors import TrajectoryComponentMissingError
-
+from mpscenes.common.reference_trajectory import ReferenceTrajectory
 
 
 class SplineTrajectory(ReferenceTrajectory):
     def __init__(self, n: int, **kwargs):
         super().__init__(n)
-        if "traj" not in kwargs:
-            raise TrajectoryComponentMissingError(
-                "Spline definition not complete. Missing component: traj"
-            )
-        self._trajDict = kwargs.get("traj")
-        if "degree" not in self._trajDict.keys():
+        self._config = kwargs
+        if "degree" not in self.trajectory_dictionary().keys():
             raise TrajectoryComponentMissingError(
                 "Spline definition not complete. Missing component in trajectory: degree"
             )
-        if "controlPoints" not in self._trajDict.keys():
+        if "controlPoints" not in self.trajectory_dictionary().keys():
             raise TrajectoryComponentMissingError(
                 "Spline definition not complete. Missing component in trajectory: controlPoints"
             )
-        if "duration" not in self._trajDict.keys():
+        if "duration" not in self.trajectory_dictionary().keys():
             raise TrajectoryComponentMissingError(
                 "Spline definition not complete. Missing component in trajectory: duration"
             )
         self.initialize_spline()
 
+
+
     def initialize_spline(self):
         self._traj = BSpline.Curve()
-        self._traj.degree = self._trajDict["degree"]
-        list_ctrlpts = [list(val) for val in self._trajDict["controlPoints"]]
+        self._traj.degree = self.trajectory_dictionary()["degree"]
+        list_ctrlpts = [list(val) for val in self.trajectory_dictionary()["controlPoints"]]
         self._traj.ctrlpts = list_ctrlpts
         self._traj.knotvector = utilities.generate_knot_vector(
             self._traj.degree, len(self._traj.ctrlpts)
         )
-        self._duration = self._trajDict["duration"]
+        self._duration = self.trajectory_dictionary()["duration"]
 
     def concretize(self):
         pass
 
     def shuffle(self):
-        limit_low = np.array(self._trajDict['low']['controlPoints'])
-        limit_high = np.array(self._trajDict['high']['controlPoints'])
-        self._trajDict['controlPoints'] = np.random.uniform(limit_low, limit_high, limit_low.shape).tolist()
+        limit_low = np.array(self.trajectory_dictionary()["low"]["controlPoints"])
+        limit_high = np.array(self.trajectory_dictionary()["high"]["controlPoints"])
+        self._config['traj']["controlPoints"] = np.random.uniform(
+            limit_low, limit_high, limit_low.shape
+        ).tolist()
         self.initialize_spline()
 
-    def timeReparameterize(self, t):
-        if t > self._duration:
+    def timeReparameterize(self, time_step: float) -> float:
+        if time_step > self._duration:
             return 1.0
-        return 0.5 * (1 - np.cos(np.pi * t / self._duration))
+        return 0.5 * (1 - np.cos(np.pi * time_step / self._duration))
 
-    def getScaledDerivatives(self, t):
-        t_ref = self.timeReparameterize(t)
+    def getScaledDerivatives(self, time_step: float) -> list:
+        t_ref = self.timeReparameterize(time_step)
         xds = self._traj.derivatives(t_ref, order=2)
-        x = np.array(xds[0])
+        position = np.array(xds[0])
         v_raw = np.array(xds[1])
         a_raw = np.array(xds[2])
-        v_scaling = 1 * np.pi / self._duration * np.sin(t * np.pi / self._duration)
-        a_scaling = 1 * np.pi / self._duration * np.cos(t * np.pi / self._duration)
-        v = v_scaling * v_raw / np.linalg.norm(v_raw)
+        v_scaling = (
+            1 * np.pi / self._duration * np.sin(time_step * np.pi / self._duration)
+        )
+        a_scaling = (
+            1 * np.pi / self._duration * np.cos(time_step * np.pi / self._duration)
+        )
+        velocity = v_scaling * v_raw / np.linalg.norm(v_raw)
         if np.linalg.norm(a_raw) < 1e-5:
-            logging.warn(f"Assuming zero acceleration on spline, because of large magnitude {np.linalg.norm(a_raw)}")
-            a = a_raw * 0
+            logging.warn(
+                f"Assuming zero acceleration on spline, because of large magnitude {np.linalg.norm(a_raw)}"
+            )
+            acceleration = a_raw * 0
         else:
-            a = a_scaling * a_raw / np.linalg.norm(a_raw)
+            acceleration = a_scaling * a_raw / np.linalg.norm(a_raw)
         if t_ref == 1.0:
-            v = v_raw * 0.0
-            a = a_raw * 0.0
-        return x, v, a
-
-    def evaluate(self, t):
-        x, v, a = self.getScaledDerivatives(t)
-        return [x, v, a]
-
-    def render(self):
-        # Import Matplotlib visualization module
-        from geomdl.visualization import VisMPL
-
-        # Set the visualization component of the curve
-        self._traj.vis = VisMPL.VisCurve3D()
-
-        # Plot the curve
-        self._traj.render()
-        # TODO: The programm is basically stopped here <09-12-21, mspahn> #
+            velocity = v_raw * 0.0
+            acceleration = a_raw * 0.0
+        return [position, velocity, acceleration]
+
+    def evaluate(self, time_step: float) -> list:
+        return self.getScaledDerivatives(time_step)
```

### Comparing `mpscenes-0.3.2/mpscenes/goals/goal_composition.py` & `mpscenes-0.4.0/mpscenes/goals/goal_composition.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-from mpscenes.common.component import MPComponent
-from mpscenes.goals.sub_goal import SubGoal
-from mpscenes.goals.sub_goal_creator import SubGoalCreator
-from mpscenes.common.errors import JointSpaceGoalsNotSupportedError
-
 import yaml
-import logging
 from omegaconf import OmegaConf
 
 from mpscenes.common.errors import MultiplePrimeGoalsError
+from mpscenes.common.component import MPComponent
+from mpscenes.goals.sub_goal import SubGoal
+from mpscenes.goals.sub_goal_creator import SubGoalCreator
 
 
 class GoalComposition(MPComponent):
     def __init__(self, **kwargs):
         if "content_dict" in kwargs and "name" in kwargs:
             self._content_dict = kwargs.get("content_dict")
             self._name = kwargs.get("name")
@@ -68,25 +65,7 @@
             composition_dict[sub_goal.name()] = sub_goal.dict()
         return composition_dict
 
     def shuffle(self):
         for sub_goal in self._sub_goals:
             sub_goal.shuffle()
 
-    def render_gym(self, viewer, rendering, **kwargs):
-        for sub_goal in self._sub_goals:
-            try:
-                sub_goal.render_gym(viewer, rendering, **kwargs)
-            except JointSpaceGoalsNotSupportedError as _:
-                logging.warn("Skipping visualization of joint space goal.")
-
-    def add_to_bullet(self, pybullet):
-        for sub_goal in self._sub_goals:
-            try:
-                sub_goal.add_to_bullet(
-                    pybullet, position=self.primary_goal().position()
-                )
-            except JointSpaceGoalsNotSupportedError as _:
-                print("Skipping visualization of joint space goal.")
-
-    def update_bullet_position(self, pybullet, **kwargs):
-        self.primary_goal().update_bullet_position(pybullet, **kwargs)
```

### Comparing `mpscenes-0.3.2/mpscenes/goals/static_joint_space_sub_goal.py` & `mpscenes-0.4.0/mpscenes/goals/static_joint_space_sub_goal.py`

 * *Files 10% similar despite different names*

```diff
@@ -61,13 +61,7 @@
         return np.zeros(self.dimension())
 
     def shuffle(self):
         random_pos = np.random.uniform(
             self.limit_low(), self.limit_high(), self.dimension()
         )
         self._config.desired_position = random_pos.tolist()
-
-    def render_gym(self, viewer, **kwargs):
-        raise JointSpaceGoalsNotSupportedError()
-
-    def add_to_bullet(self, pybullet, **kwargs):
-        raise JointSpaceGoalsNotSupportedError()
```

### Comparing `mpscenes-0.3.2/mpscenes/goals/sub_goal.py` & `mpscenes-0.4.0/mpscenes/goals/sub_goal.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,17 +40,14 @@
             raise MissmatchDimensionError(
                 "SubGoal: Dimension mismatch between goal and indices"
             )
 
     def is_primary_goal(self):
         return self._config.is_primary_goal
 
-    def bullet_id(self) -> int:
-        return self._bullet_id
-
     def epsilon(self):
         return self._config.epsilon
 
     def indices(self):
         return self._config.indices
 
     def dimension(self):
@@ -58,17 +55,14 @@
 
     def weight(self):
         return self._config.weight
 
     def type(self):
         return self._config.type
 
-    def update_bullet_position(self, pybullet, **kwargs):
-        pass
-
     def evaluate(self, **kwargs) -> list:
         return [
             self.position(**kwargs),
             self.velocity(**kwargs),
             self.acceleration(**kwargs)
         ]
```

### Comparing `mpscenes-0.3.2/mpscenes/goals/sub_goal_creator.py` & `mpscenes-0.4.0/mpscenes/goals/sub_goal_creator.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.2/mpscenes/obstacles/box_smooth.obj` & `mpscenes-0.4.0/mpscenes/obstacles/box_smooth.obj`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.2/mpscenes/obstacles/collision_obstacle.py` & `mpscenes-0.4.0/mpscenes/obstacles/collision_obstacle.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,17 +45,14 @@
 
 
 class CollisionObstacle(MPComponent):
 
     def type(self) -> str:
         return self._config.type
 
-    def bullet_id(self) -> int:
-        return self._bullet_id
-
     def geometry(self):
         return self._config.geometry
 
     def evaluate(self, **kwargs) -> list:
         return [
             self.position(**kwargs),
             self.velocity(**kwargs),
@@ -73,17 +70,14 @@
 
     def acceleration(self, **kwargs) -> np.ndarray:
         return np.zeros(self.dimension())
 
     def movable(self):
         return self._config.movable
 
-    def update_bullet_position(self, pybullet, **kwargs):
-        pass
-
     def position_into_obstacle_frame(self, position: np.ndarray) -> np.ndarray:
         return position - self.position()
 
     @abstractmethod
     def distance(self, position: np.array) -> float:
         pass
```

### Comparing `mpscenes-0.3.2/mpscenes/obstacles/dynamic_box_obstacle.py` & `mpscenes-0.4.0/mpscenes/obstacles/dynamic_box_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.2/mpscenes/obstacles/dynamic_cylinder_obstacle.py` & `mpscenes-0.4.0/mpscenes/obstacles/dynamic_cylinder_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.2/mpscenes/obstacles/dynamic_obstacle.py` & `mpscenes-0.4.0/mpscenes/obstacles/dynamic_obstacle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from dataclasses import dataclass
-from typing import Optional, Any
-import os
-import numpy as np
-import csv
-from omegaconf import OmegaConf
+from typing import Any
 
-from mpscenes.obstacles.collision_obstacle import CollisionObstacle, CollisionObstacleConfig
+from mpscenes.obstacles.collision_obstacle import CollisionObstacle
 from mpscenes.common.errors import MissmatchDimensionError, TrajectoryNotSupported
 from mpscenes.common.analytic_trajectory import AnalyticTrajectory
 from mpscenes.common.spline_trajectory import SplineTrajectory
-from mpscenes.common.component import MPComponent
+
 
 @dataclass
 class DynamicGeometryConfig:
     """Configuration dataclass for geometry.
 
     This configuration class holds information about position
     and radius of a dynamic sphere obstacle.
@@ -26,29 +22,29 @@
         a analytic trajectory.
     radius: float
         radius of the obstacle
     """
 
     trajectory: Any
 
+
 class DynamicObstacle(CollisionObstacle):
     def __init__(self, **kwargs):
-        schema = kwargs.get('schema')
         super().__init__(**kwargs)
-        if "controlPoints" in self.geometry()['trajectory']:
+        if "controlPoints" in self.geometry()["trajectory"]:
             self._trajectory_type = "spline"
-        elif isinstance(self.geometry()['trajectory'][0], str):
+        elif isinstance(self.geometry()["trajectory"][0], str):
             self._trajectory_type = "analytic"
         else:
             raise TrajectoryNotSupported(
                 f"Trajectory definition not supported, {self.geometry()['trajectory']}"
             )
         self.check_completeness()
         self.check_dimensionality()
-        if self.trajectory_type() == 'spline':
+        if self.trajectory_type() == "spline":
             self._traj = SplineTrajectory(
                 self.dimension(), traj=self._config.geometry.trajectory
             )
         elif self.trajectory_type() == "analytic":
             self._traj = AnalyticTrajectory(
                 self.dimension(), traj=self._config.geometry.trajectory
             )
@@ -61,19 +57,17 @@
         dim_verification = self.dimension()
         if self.dimension() != dim_verification:
             raise MissmatchDimensionError(
                 "Dynamic Obstacle: Dimension mismatch between trajectory array and dimension"
             )
 
     def dimension(self) -> int:
-        if self.trajectory_type() == 'spline':
-            return len(
-                self.geometry()["trajectory"]["controlPoints"][0]
-            )
-        if self.trajectory_type() == 'analytic':
+        if self.trajectory_type() == "spline":
+            return len(self.geometry()["trajectory"]["controlPoints"][0])
+        if self.trajectory_type() == "analytic":
             return len(self.geometry()["trajectory"])
 
     def traj(self):
         return self._traj
 
     def position(self, **kwargs):
         if "t" not in kwargs:
@@ -91,21 +85,7 @@
 
     def acceleration(self, **kwargs):
         if "t" not in kwargs:
             t = 0.0
         else:
             t = kwargs.get("t")
         return self._traj.evaluate(t)[2]
-
-    def update_bullet_position(self, pybullet, **kwargs):
-        if "t" not in kwargs:
-            t = 0.0
-        else:
-            t = kwargs.get("t")
-        pos = self.position(t=t).tolist()
-        vel = self.velocity(t=t).tolist()
-        if self.dimension() == 2:
-            pos += [0.0]
-            vel += [0.0]
-        ori = [0, 0, 0, 1]
-        pybullet.resetBasePositionAndOrientation(self.bullet_id(), pos, ori)
-        pybullet.resetBaseVelocity(self.bullet_id(), linearVelocity=vel)
```

### Comparing `mpscenes-0.3.2/mpscenes/obstacles/dynamic_sphere_obstacle.py` & `mpscenes-0.4.0/mpscenes/obstacles/dynamic_sphere_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.2/mpscenes/obstacles/dynamic_urdf_obstacle.py` & `mpscenes-0.4.0/mpscenes/obstacles/dynamic_urdf_obstacle.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.2/mpscenes/obstacles/obstacleCreator.py` & `mpscenes-0.4.0/mpscenes/obstacles/obstacleCreator.py`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.2/mpscenes/obstacles/sphere_obstacle.py` & `mpscenes-0.4.0/mpscenes/obstacles/sphere_obstacle.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import List, Optional
 import os
 import csv
 import numpy as np
 from omegaconf import OmegaConf
 
 from mpscenes.obstacles.collision_obstacle import CollisionObstacle, CollisionObstacleConfig, GeometryConfig
-from mpscenes.common.errors import DimensionNotSuitableForEnv
 
 
 @dataclass
 class SphereGeometryConfig(GeometryConfig):
     """Configuration dataclass for geometry.
 
     This configuration class holds information about position
@@ -43,15 +42,15 @@
     geometry: SphereGeometryConfig
     low: Optional[SphereGeometryConfig] = None
     high: Optional[SphereGeometryConfig] = None
 
 
 class SphereObstacle(CollisionObstacle):
     def __init__(self, **kwargs):
-        if not 'schema' in kwargs:
+        if 'schema' not in kwargs:
             schema = OmegaConf.structured(SphereObstacleConfig)
             kwargs['schema'] = schema
         super().__init__(**kwargs)
         self.check_completeness()
 
     def size(self):
         return [
@@ -90,61 +89,15 @@
         self._config.geometry.radius = float(random_radius)
 
 
     def csv(self, file_name, samples=100):
         theta = np.arange(-np.pi, np.pi + np.pi / samples, step=np.pi / samples)
         x = self.position()[0] + (self.radius() - 0.1) * np.cos(theta)
         y = self.position()[1] + (self.radius() - 0.1) * np.sin(theta)
-        with open(file_name, mode="w") as file:
+        with open(file_name, "w", encoding="utf8") as file:
             csv_writer = csv.writer(file, delimiter=",")
             for i in range(2 * samples):
                 csv_writer.writerow([x[i], y[i]])
 
     def distance(self, position: np.ndarray) -> float:
         pos = self.position_into_obstacle_frame(position)
         return np.linalg.norm(pos) - self.radius()
-
-    def render_gym(self, viewer, rendering, **kwargs):
-        if self.dimension() != 2:
-            raise DimensionNotSuitableForEnv(
-                "PlanarGym only supports two dimensional obstacles"
-            )
-        x = self.position(t=t)
-        tf = rendering.Transform(rotation=0, translation=(x[0], x[1]))
-        joint = viewer.draw_circle(self.radius())
-        joint.add_attr(tf)
-
-    def add_to_bullet(self, pybullet) -> int:
-        if self.dimension() == 2:
-            base_position = self.position().tolist() + [0.0]
-        elif self.dimension() == 3:
-            base_position = self.position().tolist()
-        else:
-            raise DimensionNotSuitableForEnv(
-                "Pybullet only supports three dimensional obstacles"
-            )
-        collision_shape = pybullet.createCollisionShape(
-            pybullet.GEOM_SPHERE, radius=self.radius()
-        )
-        visual_shape_id = -1
-        base_orientation = [0, 0, 0, 1]
-        mass = int(self.movable())
-        pybullet.setAdditionalSearchPath(
-            os.path.dirname(os.path.realpath(__file__))
-        )
-        visual_shape_id = pybullet.createVisualShape(
-            pybullet.GEOM_MESH,
-            fileName="sphere_smooth.obj",
-            rgbaColor=[1.0, 0.0, 0.0, 1.0],
-            specularColor=[1.0, 0.5, 0.5],
-            meshScale=[self.radius(), self.radius(), self.radius()],
-        )
-        assert isinstance(base_position, list)
-        assert isinstance(base_orientation, list)
-        self._bullet_id = pybullet.createMultiBody(
-            mass,
-            collision_shape,
-            visual_shape_id,
-            base_position,
-            base_orientation,
-        )
-        return self._bullet_id
```

### Comparing `mpscenes-0.3.2/mpscenes/obstacles/sphere_smooth.obj` & `mpscenes-0.4.0/mpscenes/obstacles/sphere_smooth.obj`

 * *Files identical despite different names*

### Comparing `mpscenes-0.3.2/mpscenes/obstacles/urdf_obstacle.py` & `mpscenes-0.4.0/mpscenes/obstacles/urdf_obstacle.py`

 * *Files 13% similar despite different names*

```diff
@@ -63,18 +63,7 @@
 
     def dimension(self):
         return len(self._config.geometry.position)
 
     def distance(self, position: np.ndarray) -> None:
         raise NoDistanceFunctionForURDFObstacle("Cannot compute distance for urdf-obstacle.")
 
-    def add_to_bullet(self, pybullet) -> int:
-        if self.dimension() != 3:
-            raise DimensionNotSuitableForEnv(
-                "Pybullet only supports three dimensional obstacles"
-            )
-        self._bullet_id = pybullet.loadURDF(
-            fileName=self.urdf(),
-            basePosition=self.position(),
-            globalScaling=self._config.scaling
-            )
-        return self._bullet_id
```

### Comparing `mpscenes-0.3.2/pyproject.toml` & `mpscenes-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "mpscenes"
-version = "0.3.2"
+version = "0.4.0"
 description = "Generic motion planning scenes, including goals and obstacles."
 authors = ["Max <m.spahn@tudelft.nl>"]
   
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.22.0"
 PyYAML = "^6.0"
 geomdl = "^5.3.1"
 pyquaternion = "^0.9.9"
 omegaconf = "^2.2.2"
-pybullet = {version = "^3.2.3", optional = true}
 sympy = "^1.7"
 
-[tool.poetry.extras]
-bullet = ["pybullet"]
+[tool.poetry.group.dev]
+optional = true
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pylint = "^2.12"
 pytest = "^6.2.5"
 black = "^22.6.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mpscenes-0.3.2/PKG-INFO` & `mpscenes-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: mpscenes
-Version: 0.3.2
+Version: 0.4.0
 Summary: Generic motion planning scenes, including goals and obstacles.
 Author: Max
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: bullet
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: geomdl (>=5.3.1,<6.0.0)
 Requires-Dist: numpy (>=1.22.0,<2.0.0)
 Requires-Dist: omegaconf (>=2.2.2,<3.0.0)
-Requires-Dist: pybullet (>=3.2.3,<4.0.0) ; extra == "bullet"
 Requires-Dist: pyquaternion (>=0.9.9,<0.10.0)
 Requires-Dist: sympy (>=1.7,<2.0)
```

