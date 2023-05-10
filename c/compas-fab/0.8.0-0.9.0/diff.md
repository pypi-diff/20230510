# Comparing `tmp/compas_fab-0.8.0.tar.gz` & `tmp/compas_fab-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\compas_fab-0.8.0.tar", last modified: Fri Nov  1 23:29:37 2019, max compression
+gzip compressed data, was "dist\compas_fab-0.9.0.tar", last modified: Tue Nov 12 23:10:22 2019, max compression
```

## Comparing `compas_fab-0.8.0.tar` & `compas_fab-0.9.0.tar`

### file list

```diff
@@ -1,130 +1,131 @@
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/
--rw-rw-rw-   0        0        0     1714 2019-10-15 05:45:22.000000 compas_fab-0.8.0/AUTHORS.rst
--rw-rw-rw-   0        0        0     5179 2019-11-01 23:29:32.000000 compas_fab-0.8.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     2430 2019-10-14 06:33:33.000000 compas_fab-0.8.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1081 2018-09-08 09:23:03.000000 compas_fab-0.8.0/LICENSE
--rw-rw-rw-   0        0        0      379 2019-10-14 06:33:33.000000 compas_fab-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11964 2019-11-01 23:29:37.000000 compas_fab-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     4056 2019-10-14 06:33:33.000000 compas_fab-0.8.0/README.rst
--rw-rw-rw-   0        0        0      536 2019-11-01 23:29:37.000000 compas_fab-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     2468 2019-11-01 23:08:40.000000 compas_fab-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab/
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/artists/
--rw-rw-rw-   0        0        0     8826 2019-11-01 23:08:40.000000 compas_fab-0.8.0/src/compas_fab/artists/base.py
--rw-rw-rw-   0        0        0      721 2019-04-22 20:28:20.000000 compas_fab-0.8.0/src/compas_fab/artists/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/backends/
--rw-rw-rw-   0        0        0      371 2019-01-29 00:43:08.000000 compas_fab-0.8.0/src/compas_fab/backends/exceptions.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/
--rw-rw-rw-   0        0        0    16732 2019-11-01 23:08:40.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/client.py
--rw-rw-rw-   0        0        0     4763 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/direct_ur_action_client.py
--rw-rw-rw-   0        0        0      942 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/exceptions.py
--rw-rw-rw-   0        0        0    11996 2019-11-01 23:08:40.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/fileserver_loader.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/
--rw-rw-rw-   0        0        0     1748 2019-01-26 21:39:30.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/actionlib_msgs.py
--rw-rw-rw-   0        0        0     4122 2019-11-01 23:11:25.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/control_msgs.py
--rw-rw-rw-   0        0        0     3650 2019-01-26 21:39:30.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/direct_ur.py
--rw-rw-rw-   0        0        0     2942 2019-10-25 14:47:20.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/geometry_msgs.py
--rw-rw-rw-   0        0        0    21326 2019-10-20 22:31:08.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/moveit_msgs.py
--rw-rw-rw-   0        0        0      386 2019-10-14 06:33:33.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/object_recognition_msgs.py
--rw-rw-rw-   0        0        0     1274 2019-01-27 12:45:44.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/octomap_msgs.py
--rw-rw-rw-   0        0        0     1687 2019-01-26 21:39:30.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/sensor_msgs.py
--rw-rw-rw-   0        0        0     7673 2019-10-20 22:31:08.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/services.py
--rw-rw-rw-   0        0        0     4056 2019-10-14 06:33:33.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/shape_msgs.py
--rw-rw-rw-   0        0        0     1628 2019-01-26 21:39:30.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/std_msgs.py
--rw-rw-rw-   0        0        0     2916 2019-10-18 06:48:22.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/trajectory_msgs.py
--rw-rw-rw-   0        0        0      354 2019-01-27 12:25:23.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/messages/__init__.py
--rw-rw-rw-   0        0        0     3144 2019-10-14 06:33:33.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/planner_backend.py
--rw-rw-rw-   0        0        0    18251 2019-11-01 23:08:40.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/planner_backend_moveit.py
--rw-rw-rw-   0        0        0      696 2019-04-23 11:48:13.000000 compas_fab-0.8.0/src/compas_fab/backends/ros/__init__.py
--rw-rw-rw-   0        0        0     2157 2019-10-18 06:48:22.000000 compas_fab-0.8.0/src/compas_fab/backends/tasks.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/
--rw-rw-rw-   0        0        0    30665 2019-10-20 22:31:08.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/client.py
--rw-rw-rw-   0        0        0      160 2019-10-20 22:31:08.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/conftest.py
--rw-rw-rw-   0        0        0     7178 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/coordinator.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/
--rw-rw-rw-   0        0        0    70656 2018-09-08 08:08:47.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/remoteApi.dll
--rw-rw-rw-   0        0        0    88768 2018-09-08 08:08:47.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/remoteApi.dylib
--rw-rw-rw-   0        0        0   113336 2018-09-08 08:08:47.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/remoteApi.so
--rw-rw-rw-   0        0        0    71894 2019-01-26 21:37:02.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/vrep.py
--rw-rw-rw-   0        0        0    45214 2018-09-08 08:08:48.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/vrepConst.py
--rw-rw-rw-   0        0        0        0 2018-09-08 08:08:47.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/__init__.py
--rw-rw-rw-   0        0        0      569 2019-04-22 20:33:48.000000 compas_fab-0.8.0/src/compas_fab/backends/vrep/__init__.py
--rw-rw-rw-   0        0        0     1104 2019-10-18 06:48:22.000000 compas_fab-0.8.0/src/compas_fab/backends/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/blender/
--rw-rw-rw-   0        0        0      803 2019-10-14 06:33:33.000000 compas_fab-0.8.0/src/compas_fab/blender/artists.py
--rw-rw-rw-   0        0        0      767 2019-04-22 20:34:13.000000 compas_fab-0.8.0/src/compas_fab/blender/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab/data/
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/data/planning_scene/
--rw-rw-rw-   0        0        0     3184 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/planning_scene/cone.stl
--rw-rw-rw-   0        0        0      184 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/planning_scene/floor.stl
--rw-rw-rw-   0        0        0     3832 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/planning_scene/timber_beam.obj
--rw-rw-rw-   0        0        0      635 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/planning_scene/timber_structure.obj
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur5_moveit_config/
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur5_moveit_config/config/
--rw-rw-rw-   0        0        0     3761 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur5_moveit_config/config/ur5.srdf
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/
--rw-rw-rw-   0        0        0    28984 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/base.stl
--rw-rw-rw-   0        0        0    52584 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/forearm.stl
--rw-rw-rw-   0        0        0    33784 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/shoulder.stl
--rw-rw-rw-   0        0        0    58884 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/upperarm.stl
--rw-rw-rw-   0        0        0    35184 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist1.stl
--rw-rw-rw-   0        0        0    35184 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist2.stl
--rw-rw-rw-   0        0        0    22384 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist3.stl
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/
--rw-rw-rw-   0        0        0   199155 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/base.obj
--rw-rw-rw-   0        0        0  2009046 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/forearm.obj
--rw-rw-rw-   0        0        0  1341223 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/shoulder.obj
--rw-rw-rw-   0        0        0  3007971 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/upperarm.obj
--rw-rw-rw-   0        0        0  1388431 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist1.obj
--rw-rw-rw-   0        0        0  1386269 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist2.obj
--rw-rw-rw-   0        0        0   169008 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist3.obj
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/urdf/
--rw-rw-rw-   0        0        0    12061 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/urdf/ur5.urdf
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/ghpython/
--rw-rw-rw-   0        0        0      947 2019-10-14 06:33:33.000000 compas_fab-0.8.0/src/compas_fab/ghpython/artists.py
--rw-rw-rw-   0        0        0    13148 2019-10-14 06:33:33.000000 compas_fab-0.8.0/src/compas_fab/ghpython/path_planning.py
--rw-rw-rw-   0        0        0      823 2019-10-14 06:33:33.000000 compas_fab-0.8.0/src/compas_fab/ghpython/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/rhino/
--rw-rw-rw-   0        0        0     3397 2019-10-14 06:33:33.000000 compas_fab-0.8.0/src/compas_fab/rhino/artists.py
--rw-rw-rw-   0        0        0      795 2019-02-07 16:09:03.000000 compas_fab-0.8.0/src/compas_fab/rhino/install.py
--rw-rw-rw-   0        0        0      829 2019-02-07 23:32:30.000000 compas_fab-0.8.0/src/compas_fab/rhino/uninstall.py
--rw-rw-rw-   0        0        0      762 2019-04-22 20:33:32.000000 compas_fab-0.8.0/src/compas_fab/rhino/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/robots/
--rw-rw-rw-   0        0        0     5866 2019-10-20 22:31:08.000000 compas_fab-0.8.0/src/compas_fab/robots/configuration.py
--rw-rw-rw-   0        0        0      856 2019-10-30 15:38:16.000000 compas_fab-0.8.0/src/compas_fab/robots/conftest.py
--rw-rw-rw-   0        0        0    11033 2019-11-01 23:08:40.000000 compas_fab-0.8.0/src/compas_fab/robots/constraints.py
--rw-rw-rw-   0        0        0     1752 2019-04-23 11:48:13.000000 compas_fab-0.8.0/src/compas_fab/robots/path_plan.py
--rw-rw-rw-   0        0        0     9599 2019-10-20 22:31:08.000000 compas_fab-0.8.0/src/compas_fab/robots/planning_scene.py
--rw-rw-rw-   0        0        0     2892 2019-10-20 22:31:09.000000 compas_fab-0.8.0/src/compas_fab/robots/rfl.py
--rw-rw-rw-   0        0        0    56434 2019-11-01 23:08:40.000000 compas_fab-0.8.0/src/compas_fab/robots/robot.py
--rw-rw-rw-   0        0        0     5329 2019-11-01 23:08:40.000000 compas_fab-0.8.0/src/compas_fab/robots/semantics.py
--rw-rw-rw-   0        0        0     2070 2019-10-20 22:31:09.000000 compas_fab-0.8.0/src/compas_fab/robots/time_.py
--rw-rw-rw-   0        0        0     7328 2019-10-20 22:31:09.000000 compas_fab-0.8.0/src/compas_fab/robots/trajectory.py
--rw-rw-rw-   0        0        0      861 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/robots/units.py
--rw-rw-rw-   0        0        0     1786 2019-10-20 22:31:09.000000 compas_fab-0.8.0/src/compas_fab/robots/ur5.py
--rw-rw-rw-   0        0        0     1683 2019-10-25 14:47:20.000000 compas_fab-0.8.0/src/compas_fab/robots/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/sensors/
--rw-rw-rw-   0        0        0      657 2019-01-26 21:34:28.000000 compas_fab-0.8.0/src/compas_fab/sensors/base.py
--rw-rw-rw-   0        0        0    24735 2019-10-20 22:31:09.000000 compas_fab-0.8.0/src/compas_fab/sensors/baumer.py
--rw-rw-rw-   0        0        0      195 2019-10-15 05:45:22.000000 compas_fab-0.8.0/src/compas_fab/sensors/exceptions.py
--rw-rw-rw-   0        0        0      761 2019-10-15 05:45:22.000000 compas_fab-0.8.0/src/compas_fab/sensors/__init__.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab/utilities/
--rw-rw-rw-   0        0        0     1589 2019-01-26 21:34:28.000000 compas_fab-0.8.0/src/compas_fab/utilities/filesystem.py
--rw-rw-rw-   0        0        0     1402 2019-01-26 21:34:28.000000 compas_fab-0.8.0/src/compas_fab/utilities/file_io.py
--rw-rw-rw-   0        0        0     3722 2019-04-19 13:42:03.000000 compas_fab-0.8.0/src/compas_fab/utilities/numbers.py
--rw-rw-rw-   0        0        0      487 2019-01-26 21:34:28.000000 compas_fab-0.8.0/src/compas_fab/utilities/utilities.py
--rw-rw-rw-   0        0        0      896 2019-04-22 20:32:41.000000 compas_fab-0.8.0/src/compas_fab/utilities/__init__.py
--rw-rw-rw-   0        0        0     1206 2019-10-15 05:45:22.000000 compas_fab-0.8.0/src/compas_fab/__init__.py
--rw-rw-rw-   0        0        0      356 2019-11-01 23:29:32.000000 compas_fab-0.8.0/src/compas_fab/__version__.py
-drwxrwxrwx   0        0        0        0 2019-11-01 23:29:37.000000 compas_fab-0.8.0/src/compas_fab.egg-info/
--rw-rw-rw-   0        0        0        1 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-10-20 22:02:07.000000 compas_fab-0.8.0/src/compas_fab.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0    11964 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       42 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab.egg-info/requires.txt
--rw-rw-rw-   0        0        0     4594 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       11 2019-11-01 23:29:36.000000 compas_fab-0.8.0/src/compas_fab.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:22.000000 compas_fab-0.9.0/
+-rw-rw-rw-   0        0        0     1834 2019-11-07 08:05:16.000000 compas_fab-0.9.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     5605 2019-11-12 23:10:17.000000 compas_fab-0.9.0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0     2557 2019-11-07 14:00:14.000000 compas_fab-0.9.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1081 2018-09-08 09:23:03.000000 compas_fab-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0      379 2019-10-14 06:33:33.000000 compas_fab-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    12507 2019-11-12 23:10:22.000000 compas_fab-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4056 2019-10-14 06:33:33.000000 compas_fab-0.9.0/README.rst
+-rw-rw-rw-   0        0        0      666 2019-11-12 23:10:22.000000 compas_fab-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     2394 2019-11-12 21:36:35.000000 compas_fab-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/artists/
+-rw-rw-rw-   0        0        0     8826 2019-11-06 21:41:06.000000 compas_fab-0.9.0/src/compas_fab/artists/base.py
+-rw-rw-rw-   0        0        0      721 2019-04-22 20:28:20.000000 compas_fab-0.9.0/src/compas_fab/artists/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/backends/
+-rw-rw-rw-   0        0        0      371 2019-01-29 00:43:08.000000 compas_fab-0.9.0/src/compas_fab/backends/exceptions.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/
+-rw-rw-rw-   0        0        0    19401 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/client.py
+-rw-rw-rw-   0        0        0     4763 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/direct_ur_action_client.py
+-rw-rw-rw-   0        0        0      942 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/exceptions.py
+-rw-rw-rw-   0        0        0    11945 2019-11-07 08:05:16.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/fileserver_loader.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/
+-rw-rw-rw-   0        0        0     1754 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/actionlib_msgs.py
+-rw-rw-rw-   0        0        0     4122 2019-11-02 09:00:24.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/control_msgs.py
+-rw-rw-rw-   0        0        0     3626 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/direct_ur.py
+-rw-rw-rw-   0        0        0     6776 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/geometry_msgs.py
+-rw-rw-rw-   0        0        0    21326 2019-10-20 22:31:08.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/moveit_msgs.py
+-rw-rw-rw-   0        0        0      386 2019-10-14 06:33:33.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/object_recognition_msgs.py
+-rw-rw-rw-   0        0        0     1275 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/octomap_msgs.py
+-rw-rw-rw-   0        0        0     1653 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/sensor_msgs.py
+-rw-rw-rw-   0        0        0     7673 2019-10-20 22:31:08.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/services.py
+-rw-rw-rw-   0        0        0     4010 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/shape_msgs.py
+-rw-rw-rw-   0        0        0     1626 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/std_msgs.py
+-rw-rw-rw-   0        0        0     2916 2019-10-18 06:48:22.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/trajectory_msgs.py
+-rw-rw-rw-   0        0        0      691 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/messages/__init__.py
+-rw-rw-rw-   0        0        0     3144 2019-10-14 06:33:33.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/planner_backend.py
+-rw-rw-rw-   0        0        0    18251 2019-11-06 21:41:06.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/planner_backend_moveit.py
+-rw-rw-rw-   0        0        0      852 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/ros/__init__.py
+-rw-rw-rw-   0        0        0     2157 2019-10-18 06:48:22.000000 compas_fab-0.9.0/src/compas_fab/backends/tasks.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/backends/vrep/
+-rw-rw-rw-   0        0        0    30750 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/vrep/client.py
+-rw-rw-rw-   0        0        0      160 2019-10-20 22:31:08.000000 compas_fab-0.9.0/src/compas_fab/backends/vrep/conftest.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/
+-rw-rw-rw-   0        0        0    70656 2018-09-08 08:08:47.000000 compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/remoteApi.dll
+-rw-rw-rw-   0        0        0    88768 2018-09-08 08:08:47.000000 compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/remoteApi.dylib
+-rw-rw-rw-   0        0        0   113336 2018-09-08 08:08:47.000000 compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/remoteApi.so
+-rw-rw-rw-   0        0        0    71894 2019-01-26 21:37:02.000000 compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/vrep.py
+-rw-rw-rw-   0        0        0    45214 2018-09-08 08:08:48.000000 compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/vrepConst.py
+-rw-rw-rw-   0        0        0        0 2018-09-08 08:08:47.000000 compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/__init__.py
+-rw-rw-rw-   0        0        0      569 2019-04-22 20:33:48.000000 compas_fab-0.9.0/src/compas_fab/backends/vrep/__init__.py
+-rw-rw-rw-   0        0        0     1285 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/backends/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/blender/
+-rw-rw-rw-   0        0        0      773 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/blender/artists.py
+-rw-rw-rw-   0        0        0      767 2019-04-22 20:34:13.000000 compas_fab-0.9.0/src/compas_fab/blender/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/data/
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:22.000000 compas_fab-0.9.0/src/compas_fab/data/planning_scene/
+-rw-rw-rw-   0        0        0     3184 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/planning_scene/cone.stl
+-rw-rw-rw-   0        0        0      184 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/planning_scene/floor.stl
+-rw-rw-rw-   0        0        0     3832 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/planning_scene/timber_beam.obj
+-rw-rw-rw-   0        0        0      635 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/planning_scene/timber_structure.obj
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur5_moveit_config/
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:22.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur5_moveit_config/config/
+-rw-rw-rw-   0        0        0     3761 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur5_moveit_config/config/ur5.srdf
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:22.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/
+-rw-rw-rw-   0        0        0    28984 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/base.stl
+-rw-rw-rw-   0        0        0    52584 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/forearm.stl
+-rw-rw-rw-   0        0        0    33784 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/shoulder.stl
+-rw-rw-rw-   0        0        0    58884 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/upperarm.stl
+-rw-rw-rw-   0        0        0    35184 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist1.stl
+-rw-rw-rw-   0        0        0    35184 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist2.stl
+-rw-rw-rw-   0        0        0    22384 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist3.stl
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:22.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/
+-rw-rw-rw-   0        0        0   199155 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/base.obj
+-rw-rw-rw-   0        0        0  2009046 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/forearm.obj
+-rw-rw-rw-   0        0        0  1341223 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/shoulder.obj
+-rw-rw-rw-   0        0        0  3007971 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/upperarm.obj
+-rw-rw-rw-   0        0        0  1388431 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist1.obj
+-rw-rw-rw-   0        0        0  1386269 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist2.obj
+-rw-rw-rw-   0        0        0   169008 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist3.obj
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:22.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/urdf/
+-rw-rw-rw-   0        0        0    12061 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/urdf/ur5.urdf
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:22.000000 compas_fab-0.9.0/src/compas_fab/ghpython/
+-rw-rw-rw-   0        0        0      947 2019-10-14 06:33:33.000000 compas_fab-0.9.0/src/compas_fab/ghpython/artists.py
+-rw-rw-rw-   0        0        0     9531 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/ghpython/path_planning.py
+-rw-rw-rw-   0        0        0      832 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/ghpython/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:22.000000 compas_fab-0.9.0/src/compas_fab/rhino/
+-rw-rw-rw-   0        0        0     3042 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/rhino/artists.py
+-rw-rw-rw-   0        0        0      795 2019-02-07 16:09:03.000000 compas_fab-0.9.0/src/compas_fab/rhino/install.py
+-rw-rw-rw-   0        0        0      829 2019-02-07 23:32:30.000000 compas_fab-0.9.0/src/compas_fab/rhino/uninstall.py
+-rw-rw-rw-   0        0        0      762 2019-04-22 20:33:32.000000 compas_fab-0.9.0/src/compas_fab/rhino/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:22.000000 compas_fab-0.9.0/src/compas_fab/robots/
+-rw-rw-rw-   0        0        0     5866 2019-10-20 22:31:08.000000 compas_fab-0.9.0/src/compas_fab/robots/configuration.py
+-rw-rw-rw-   0        0        0      940 2019-11-07 08:05:16.000000 compas_fab-0.9.0/src/compas_fab/robots/conftest.py
+-rw-rw-rw-   0        0        0    11033 2019-11-06 21:41:06.000000 compas_fab-0.9.0/src/compas_fab/robots/constraints.py
+-rw-rw-rw-   0        0        0     2179 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/robots/inertia.py
+-rw-rw-rw-   0        0        0     1752 2019-04-23 11:48:13.000000 compas_fab-0.9.0/src/compas_fab/robots/path_plan.py
+-rw-rw-rw-   0        0        0     9599 2019-10-20 22:31:08.000000 compas_fab-0.9.0/src/compas_fab/robots/planning_scene.py
+-rw-rw-rw-   0        0        0     2892 2019-10-20 22:31:09.000000 compas_fab-0.9.0/src/compas_fab/robots/rfl.py
+-rw-rw-rw-   0        0        0    56500 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/robots/robot.py
+-rw-rw-rw-   0        0        0     5329 2019-11-06 21:40:34.000000 compas_fab-0.9.0/src/compas_fab/robots/semantics.py
+-rw-rw-rw-   0        0        0     2070 2019-10-20 22:31:09.000000 compas_fab-0.9.0/src/compas_fab/robots/time_.py
+-rw-rw-rw-   0        0        0     7328 2019-10-20 22:31:09.000000 compas_fab-0.9.0/src/compas_fab/robots/trajectory.py
+-rw-rw-rw-   0        0        0      861 2019-04-19 13:42:03.000000 compas_fab-0.9.0/src/compas_fab/robots/units.py
+-rw-rw-rw-   0        0        0     1786 2019-10-20 22:31:09.000000 compas_fab-0.9.0/src/compas_fab/robots/ur5.py
+-rw-rw-rw-   0        0        0    11356 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/robots/wrench.py
+-rw-rw-rw-   0        0        0     2101 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/robots/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:22.000000 compas_fab-0.9.0/src/compas_fab/sensors/
+-rw-rw-rw-   0        0        0      657 2019-01-26 21:34:28.000000 compas_fab-0.9.0/src/compas_fab/sensors/base.py
+-rw-rw-rw-   0        0        0    24793 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/sensors/baumer.py
+-rw-rw-rw-   0        0        0      197 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/sensors/exceptions.py
+-rw-rw-rw-   0        0        0      811 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/sensors/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:22.000000 compas_fab-0.9.0/src/compas_fab/utilities/
+-rw-rw-rw-   0        0        0     1590 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/utilities/filesystem.py
+-rw-rw-rw-   0        0        0     1411 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/utilities/file_io.py
+-rw-rw-rw-   0        0        0     3758 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/utilities/numbers.py
+-rw-rw-rw-   0        0        0      464 2019-11-06 22:53:27.000000 compas_fab-0.9.0/src/compas_fab/utilities/utilities.py
+-rw-rw-rw-   0        0        0     1057 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1381 2019-11-07 14:00:14.000000 compas_fab-0.9.0/src/compas_fab/__init__.py
+-rw-rw-rw-   0        0        0      356 2019-11-12 23:10:17.000000 compas_fab-0.9.0/src/compas_fab/__version__.py
+drwxrwxrwx   0        0        0        0 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab.egg-info/
+-rw-rw-rw-   0        0        0        1 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-11-12 23:09:25.000000 compas_fab-0.9.0/src/compas_fab.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0    12507 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     4615 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       11 2019-11-12 23:10:21.000000 compas_fab-0.9.0/src/compas_fab.egg-info/top_level.txt
```

### Comparing `compas_fab-0.8.0/AUTHORS.rst` & `compas_fab-0.9.0/AUTHORS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
             Casas, G. and
             Parascho, S. and
             Jenny, D. and
             D\"{o}rfler, K. and
             Helmreich, M. and
             Gandia, A. and
             Ma, Z. and
-            Ariza, I.
+            Ariza, I. and
+            Pacher, M.
             },
         howpublished={https://github.com/compas-dev/compas\_fab/},
         note={Gramazio Kohler Research, ETH Z\"{u}rich},
         year={2018}
     }
 
 Authors
@@ -33,7 +34,8 @@
 * Stefana Parascho <parascho@arch.ethz.ch> `@stefanaparascho <https://github.com/stefanaparascho>`_
 * David Jenny <jenny@arch.ethz.ch> `@DavidJenny <https://github.com/DavidJenny>`_
 * Kathrin Dörfler <doerfler@arch.ethz.ch> `@kathrindoerfler <https://github.com/kathrindoerfler>`_
 * Matthias Helmreich <helmreich@arch.ethz.ch> `@mhelmrei <https://github.com/mhelmrei>`_
 * Augusto Gandia <gandia@arch.ethz.ch> `@augustogandia <https://github.com/augustogandia>`_
 * Zhao Ma <ma@arch.ethz.ch> `@xarthurx <https://github.com/xarthurx>`_
 * Inés Ariza <ariza@arch.ethz.ch> `@inesariza <https://github.com/inesariza>`_
+* Matteo Pacher <pacher@arch.ethz.ch> `@matteo-pacher <https://github.com/matteo-pacher>`_
```

### Comparing `compas_fab-0.8.0/CHANGELOG.rst` & `compas_fab-0.9.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,27 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_
 and this project adheres to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
+0.9.0
+----------
+
+**Added**
+
+* Added ``load_robot`` method to ROS client to simplify loading robots from running ROS setup.
+* Added ``compas_fab.robots.Wrench``: a Wrench class representing force in free space, separated into its linear (force) and angular (torque) parts.
+* Added ``compas_fab.robots.Inertia``: a Inertia class representing spatial distribution of mass in a rigid body
+
+**Changed**
+
+* Updated to COMPAS 0.11
+
 0.8.0
 ----------
 
 **Changed**
 
 * Updated to COMPAS 0.10
 * Add better support for passive joints on IK, Cartesian and Kinematic planning
```

### Comparing `compas_fab-0.8.0/CONTRIBUTING.rst` & `compas_fab-0.9.0/CONTRIBUTING.rst`

 * *Files 6% similar despite different names*

```diff
@@ -25,25 +25,32 @@
 5. Start making your changes to the **master** branch (or branch off of it).
 6. Make sure all tests still pass:
 
 ::
 
     invoke test
 
-7. Add yourself to ``AUTHORS.rst``.
-8. Commit your changes and push your branch to GitHub.
-9. Create a `pull request <https://help.github.com/articles/about-pull-requests/>`_ through the GitHub website.
+7. Check there are no linter errors:
+
+::
+
+    invoke lint
+
+8. Add yourself to ``AUTHORS.rst``.
+9. Commit your changes and push your branch to GitHub.
+10. Create a `pull request <https://help.github.com/articles/about-pull-requests/>`_ through the GitHub website.
 
 
 During development, use `pyinvoke <http://docs.pyinvoke.org/>`_ tasks on the
 command prompt to ease recurring operations:
 
 * ``invoke clean``: Clean all generated artifacts.
 * ``invoke check``: Run various code and documentation style checks.
 * ``invoke docs``: Generate documentation.
+* ``invoke lint``: Run code linter for coding style checks.
 * ``invoke test``: Run all tests and checks in one swift command.
 * ``invoke``: Show available tasks.
 
 
 Documentation improvements
 --------------------------
```

### Comparing `compas_fab-0.8.0/LICENSE` & `compas_fab-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/PKG-INFO` & `compas_fab-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: compas_fab
-Version: 0.8.0
+Version: 0.9.0
 Summary: Robotic fabrication package for the COMPAS Framework
 Home-page: https://github.com/compas-dev/compas_fab
 Author: Gramazio Kohler Research
 Author-email: gramaziokohler@arch.ethz.ch
 License: MIT license
 Description: ============================================================
         COMPAS FAB: Robotic Fabrication for COMPAS
@@ -118,14 +118,27 @@
         =========
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_
         and this project adheres to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
         
+        0.9.0
+        ----------
+        
+        **Added**
+        
+        * Added ``load_robot`` method to ROS client to simplify loading robots from running ROS setup.
+        * Added ``compas_fab.robots.Wrench``: a Wrench class representing force in free space, separated into its linear (force) and angular (torque) parts.
+        * Added ``compas_fab.robots.Inertia``: a Inertia class representing spatial distribution of mass in a rigid body
+        
+        **Changed**
+        
+        * Updated to COMPAS 0.11
+        
         0.8.0
         ----------
         
         **Changed**
         
         * Updated to COMPAS 0.10
         * Add better support for passive joints on IK, Cartesian and Kinematic planning
```

### Comparing `compas_fab-0.8.0/README.rst` & `compas_fab-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/setup.py` & `compas_fab-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-#!/usr/bin/env python
-# -*- encoding: utf-8 -*-
-from __future__ import absolute_import, print_function
-
-import io
-import re
-from glob import glob
-from os.path import abspath, basename, dirname, join, splitext
-
-from setuptools import find_packages, setup
-
-requirements = [
-    # Until COMPAS reaches 1.0, we pin major.minor and allow patch version updates
-    'compas>=0.10,<0.11',
-    'roslibpy>=0.7',
-    'pyserial',
-]
-keywords_list = ['robotic fabrication', 'digital fabrication', 'architecture', 'robotics', 'ros']
-
-here = abspath(dirname(__file__))
-
-
-def read(*names, **kwargs):
-    return io.open(
-        join(here, *names),
-        encoding=kwargs.get('encoding', 'utf8')
-    ).read()
-
-
-about = {}
-exec(read('src', 'compas_fab', '__version__.py'), about)
-
-setup(
-    name=about['__title__'],
-    version=about['__version__'],
-    license=about['__license__'],
-    description=about['__description__'],
-    author=about['__author__'],
-    author_email=about['__author_email__'],
-    url=about['__url__'],
-    long_description='%s\n%s' % (
-        re.compile('^.. start-badges.*^.. end-badges', re.M |
-                   re.S).sub('', read('README.rst')),
-        re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
-    ),
-    packages=find_packages('src'),
-    package_dir={'': 'src'},
-    py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
-    include_package_data=True,
-    zip_safe=False,
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: Unix',
-        'Operating System :: POSIX',
-        'Operating System :: Microsoft :: Windows',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: IronPython',
-        'Topic :: Scientific/Engineering',
-    ],
-    keywords=keywords_list,
-    install_requires=requirements,
-    extras_require={},
-    entry_points={},
-)
+#!/usr/bin/env python
+# -*- encoding: utf-8 -*-
+from __future__ import absolute_import, print_function
+
+import io
+import re
+from glob import glob
+from os.path import abspath, basename, dirname, join, splitext
+
+from setuptools import find_packages, setup
+
+requirements = [
+    # Until COMPAS reaches 1.0, we pin major.minor and allow patch version updates
+    'compas>=0.11,<0.12',
+    'roslibpy>=0.7',
+    'pyserial',
+]
+keywords_list = ['robotic fabrication', 'digital fabrication', 'architecture', 'robotics', 'ros']
+
+here = abspath(dirname(__file__))
+
+
+def read(*names, **kwargs):
+    return io.open(
+        join(here, *names),
+        encoding=kwargs.get('encoding', 'utf8')
+    ).read()
+
+
+about = {}
+exec(read('src', 'compas_fab', '__version__.py'), about)
+
+setup(
+    name=about['__title__'],
+    version=about['__version__'],
+    license=about['__license__'],
+    description=about['__description__'],
+    author=about['__author__'],
+    author_email=about['__author_email__'],
+    url=about['__url__'],
+    long_description='%s\n%s' % (
+        re.compile('^.. start-badges.*^.. end-badges', re.M |
+                   re.S).sub('', read('README.rst')),
+        re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
+    ),
+    packages=find_packages('src'),
+    package_dir={'': 'src'},
+    py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
+    include_package_data=True,
+    zip_safe=False,
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'Intended Audience :: Developers',
+        'Intended Audience :: Science/Research',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: Unix',
+        'Operating System :: POSIX',
+        'Operating System :: Microsoft :: Windows',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.3',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: IronPython',
+        'Topic :: Scientific/Engineering',
+    ],
+    keywords=keywords_list,
+    install_requires=requirements,
+    extras_require={},
+    entry_points={},
+)
```

### Comparing `compas_fab-0.8.0/src/compas_fab/artists/base.py` & `compas_fab-0.9.0/src/compas_fab/artists/base.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/artists/__init__.py` & `compas_fab-0.9.0/src/compas_fab/artists/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/client.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from __future__ import print_function
 
+import os
+
+from compas.robots import RobotModel
 from compas.utilities import await_callback
 from roslibpy import Message
 from roslibpy import Ros
 from roslibpy.actionlib import ActionClient
 from roslibpy.actionlib import Goal
 
 from compas_fab.backends.ros.exceptions import RosError
+from compas_fab.backends.ros.fileserver_loader import RosFileServerLoader
 from compas_fab.backends.ros.messages import ExecuteTrajectoryFeedback
 from compas_fab.backends.ros.messages import ExecuteTrajectoryGoal
 from compas_fab.backends.ros.messages import ExecuteTrajectoryResult
 from compas_fab.backends.ros.messages import FollowJointTrajectoryFeedback
 from compas_fab.backends.ros.messages import FollowJointTrajectoryGoal
 from compas_fab.backends.ros.messages import FollowJointTrajectoryResult
 from compas_fab.backends.ros.messages import Header
 from compas_fab.backends.ros.messages import JointTrajectory as RosMsgJointTrajectory
 from compas_fab.backends.ros.messages import JointTrajectoryPoint as RosMsgJointTrajectoryPoint
 from compas_fab.backends.ros.messages import MoveItErrorCodes
 from compas_fab.backends.ros.messages import RobotTrajectory
 from compas_fab.backends.ros.messages import Time
 from compas_fab.backends.ros.planner_backend_moveit import MoveItPlanner
 from compas_fab.backends.tasks import CancellableFutureResult
+from compas_fab.robots import Robot
+from compas_fab.robots import RobotSemantics
 
 __all__ = [
     'RosClient',
 ]
 
 PLANNER_BACKENDS = {
     'moveit': MoveItPlanner
@@ -106,14 +112,67 @@
         return self
 
     def __exit__(self, *args):
         self.dispose_planner()
 
         self.close()
 
+    def load_robot(self, load_geometry=False, urdf_param_name='/robot_description', srdf_param_name='/robot_description_semantic', precision=None, local_cache_directory=None):
+        """Load an entire robot instance -including model and semantics- directly from ROS.
+
+        Parameters
+        ----------
+        load_geometry : bool, optional
+            ``True`` to load the robot's geometry, otherwise ``False`` to load only the model and semantics.
+        urdf_param_name : str, optional
+            Parameter name where the URDF is defined. If not defined, it will default to ``/robot_description``.
+        srdf_param_name : str, optional
+            Parameter name where the SRDF is defined. If not defined, it will default to ``/robot_description_semantic``.
+        precision : float
+            Defines precision for importing/loading meshes. Defaults to ``compas.PRECISION``.
+        local_cache_directory : str, optional
+            Directory where the robot description (URDF, SRDF and meshes) are stored.
+            This differs from the directory taken as parameter by the :class:`RosFileServerLoader`
+            in that it points directly to the specific robot package, not to a global workspace storage
+            for all robots. If not assigned, the robot will not be cached locally.
+
+        Examples
+        --------
+
+        >>> from compas_fab.backends import RosClient
+        >>> with RosClient() as client:
+        ...     robot = client.load_robot()
+        ...     print(robot.name)
+        ur5
+        """
+        robot_name = None
+        use_local_cache = False
+
+        if local_cache_directory is not None:
+            use_local_cache = True
+            path_parts = local_cache_directory.strip(os.path.sep).split(os.path.sep)
+            path_parts, robot_name = path_parts[:-1], path_parts[-1]
+            local_cache_directory = os.path.sep.join(path_parts)
+
+        loader = RosFileServerLoader(self, use_local_cache, local_cache_directory, precision)
+
+        if robot_name:
+            loader.robot_name = robot_name
+
+        urdf = loader.load_urdf(urdf_param_name)
+        srdf = loader.load_srdf(srdf_param_name)
+
+        model = RobotModel.from_urdf_string(urdf)
+        semantics = RobotSemantics.from_srdf_string(srdf, model)
+
+        if load_geometry:
+            model.load_geometry(loader)
+
+        return Robot(model, semantics=semantics, client=self)
+
     def inverse_kinematics(self, frame, base_link, group,
                            joint_names, joint_positions, avoid_collisions=True,
                            constraints=None, attempts=8,
                            attached_collision_meshes=None):
         kwargs = {}
         kwargs['frame'] = frame
         kwargs['base_link'] = base_link
```

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/direct_ur_action_client.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/direct_ur_action_client.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/exceptions.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/exceptions.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/fileserver_loader.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/fileserver_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 import roslibpy
 from compas.datastructures import Mesh
 from compas.datastructures import mesh_transform
 from compas.files import XML
 from compas.geometry import Transformation
 from compas.robots.resources.basic import _get_file_format
 from compas.robots.resources.basic import _mesh_import
-from compas.utilities import await_callback
 from compas.utilities import geometric_key
 
 LOGGER = logging.getLogger('compas_fab.backends.ros')
+TIMEOUT = 10
 
 __all__ = [
     'RosFileServerLoader',
 ]
 
 
 def _cache_file_exists(filename):
@@ -115,15 +115,15 @@
         if self.local_cache_enabled and self.robot_name:
             filename = self._urdf_filename
 
             if _cache_file_exists(filename):
                 return _read_file(filename)
 
         param = roslibpy.Param(self.ros, parameter_name)
-        urdf = await_callback(param.get)
+        urdf = param.get(timeout=TIMEOUT)
 
         self.robot_name = self._read_robot_name(urdf)
 
         if self.local_cache_enabled:
             # Retrieve filename again, now that robot_name
             # has been loaded from URDF
             _write_file(self._urdf_filename, urdf)
@@ -147,15 +147,15 @@
         if self.local_cache_enabled and self.robot_name:
             filename = self._srdf_filename
 
             if _cache_file_exists(filename):
                 return _read_file(filename)
 
         param = roslibpy.Param(self.ros, parameter_name)
-        srdf = await_callback(param.get)
+        srdf = param.get(timeout=TIMEOUT)
 
         if self.local_cache_enabled:
             _write_file(self._srdf_filename, srdf)
 
         return srdf
 
     def _read_robot_name(self, robot_description):
@@ -201,15 +201,15 @@
             use_local_file = _cache_file_exists(local_filename)
         else:
             _, local_filename = tempfile.mkstemp(suffix='.' + file_extension, prefix='ros_fileserver_')
 
         if not use_local_file:
             service = roslibpy.Service(self.ros, '/file_server/get_file', 'file_server/GetBinaryFile')
             request = roslibpy.ServiceRequest(dict(name=url))
-            response = await_callback(service.call, 'callback', 'errback', request)
+            response = service.call(request, timeout=TIMEOUT)
 
             file_content = binascii.a2b_base64(response.data['value'])
 
             # Just look away, we're about to do something nasty!
             # namespaces are handled differently between the CLI and CPython
             # XML parsers, so, we just get rid of it for DAE files
             if file_extension == 'dae':
```

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/messages/actionlib_msgs.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/messages/actionlib_msgs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from __future__ import absolute_import
 
 from .std_msgs import ROSmsg
 from .std_msgs import Header
 from .std_msgs import Time
 
+
 class GoalID(ROSmsg):
     """http://docs.ros.org/api/actionlib_msgs/html/msg/GoalID.html
     """
+
     def __init__(self, stamp=Time(), id=""):
         self.stamp = stamp
         self.id = id
-    
+
     @classmethod
     def from_msg(cls, msg):
         stamp = Time.from_msg(msg['stamp'])
         id = msg['id']
         return cls(stamp, id)
 
+
 class GoalStatus(ROSmsg):
     """http://docs.ros.org/api/actionlib_msgs/html/msg/GoalStatus.html
     """
 
     PENDING = 0
     ACTIVE = 1
     PREEMPTED = 2
@@ -32,15 +35,15 @@
     RECALLED = 8
     LOST = 9
 
     def __init__(self, goal_id=GoalID(), status=0, text=''):
         self.goal_id = goal_id
         self.status = status
         self.text = text
-    
+
     @classmethod
     def from_msg(cls, msg):
         goal_id = GoalID.from_msg(msg['goal_id'])
         status = msg['status']
         text = msg['text']
         return cls(goal_id, status, text)
 
@@ -48,22 +51,25 @@
     def human_readable(self):
         cls = type(self)
         for k, v in cls.__dict__.items():
             if v == self.status:
                 return k
         return ''
 
+
 class GoalStatusArray(ROSmsg):
     """http://docs.ros.org/api/actionlib_msgs/html/msg/GoalStatusArray.html
     """
+
     def __init__(self, header=Header(), status_list=[]):
         self.header = header
         self.status_list = status_list
 
+
 """
 rostopic info /follow_joint_trajectory/cancel
 Type: actionlib_msgs/GoalID
 
 rostopic info /follow_joint_trajectory/status
 Type: actionlib_msgs/GoalStatusArray
 
-"""
+"""
```

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/messages/control_msgs.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/messages/control_msgs.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/messages/direct_ur.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/messages/direct_ur.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,84 @@
 from __future__ import absolute_import
 
 
 class URmsg(object):
     """
     """
+
     def __init__(self, **kwargs):
         for k, v in kwargs.items():
             setattr(self, k, v)
 
     def __str__(self):
         result = ""
         for key, value in self.__dict__.items():
             if value:
                 result += "%s, " % value
         return result[:-2]
-    
+
     def __repr__(self):
         return self.__str__
 
 
 class Point(URmsg):
     """
     """
+
     def __init__(self, x, y, z):
-        self.x = x # [m]
-        self.y = y # [m]
-        self.z = z # [m]
+        self.x = x  # [m]
+        self.y = y  # [m]
+        self.z = z  # [m]
 
     def __str__(self):
-        return '%.6f, %.6f, %.6f' % (self.x ,self.y, self.z)
+        return '%.6f, %.6f, %.6f' % (self.x, self.y, self.z)
 
 
 class AxisAngle(URmsg):
     """
     """
+
     def __init__(self, x, y, z):
         self.x = x
         self.y = y
         self.z = z
-    
+
     def __str__(self):
-        return '%.6f, %.6f, %.6f' % (self.x ,self.y, self.z)
+        return '%.6f, %.6f, %.6f' % (self.x, self.y, self.z)
 
 
 class URPose(URmsg):
     """
     """
-    def __init__(self, position=Point(0,0,0), orientation=AxisAngle(0,0,0)):
+
+    def __init__(self, position=Point(0, 0, 0), orientation=AxisAngle(0, 0, 0)):
         self.position = position
         self.orientation = orientation
 
     @classmethod
     def from_frame(cls, frame):
         point = frame.point
         ax, ay, az = frame.axis_angle_vector
         return cls(Point(*list(point)), AxisAngle(ax, ay, az))
-    
+
     def __str__(self):
         return "p[%s, %s]" % (self.position, self.orientation)
 
 
 class URPoseTrajectoryPoint(URmsg):
     """
     """
+
     def __init__(self, pose=URPose(), acceleration=None, velocity=None, time=None, radius=None):
         self.pose = pose
-        self.acceleration = acceleration # [m/s^2]
-        self.velocity = velocity # [m/s]
-        self.time = time # [s]
-        self.radius = radius # [m]
-        
+        self.acceleration = acceleration  # [m/s^2]
+        self.velocity = velocity  # [m/s]
+        self.time = time  # [s]
+        self.radius = radius  # [m]
+
     def __str__(self):
         result = "%s" % self.pose
         if self.acceleration:
             result += ", a=%.6f" % self.acceleration
         if self.velocity:
             result += ", v=%.6f" % self.velocity
         if self.time:
@@ -82,39 +87,42 @@
             result += ", r=%.6f" % self.radius
         return result
 
 
 class URMovej(URmsg):
     """
     """
+
     def __init__(self, pose_trajectory_point=URPoseTrajectoryPoint()):
         self.pose_trajectory_point = pose_trajectory_point
 
     def __str__(self):
         return "movej(%s)" % self.pose_trajectory_point
 
 
 class URMovel(URmsg):
     """
     """
+
     def __init__(self, pose_trajectory_point=URPoseTrajectoryPoint()):
         self.pose_trajectory_point = pose_trajectory_point
 
     def __str__(self):
         return "movel(%s)" % self.pose_trajectory_point
 
 
 class URGoal(URmsg):
     """
     """
+
     def __init__(self, script_lines=[]):
         self.script = "def prog():\n\t"
-        self.script += "\n\t".join([str(line) for line in script_lines]) 
+        self.script += "\n\t".join([str(line) for line in script_lines])
         self.script += "\nend\nprog()\n\n"
-    
+
     @property
     def msg(self):
         return {"script": self.script}
 
 
 if __name__ == "__main__":
 
@@ -125,16 +133,16 @@
     f2.point /= 1000.
     frames = [f1, f2]
 
     acceleration = 0.35
     velocity = 0.17
     time = 5.
     script_lines = []
-    
-    for frame in frames:        
-        ptp = URPoseTrajectoryPoint(URPose.from_frame(frame), acceleration, velocity, time, None)
+
+    for frame in frames:
+        ptp = URPoseTrajectoryPoint(URPose.from_frame(
+            frame), acceleration, velocity, time, None)
         move = URMovej(ptp)
-        #move = Movel(ptp)
         script_lines.append(move)
 
     urgoal = URGoal(script_lines)
     print(urgoal.msg["script_lines"])
```

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/messages/moveit_msgs.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/messages/moveit_msgs.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/messages/octomap_msgs.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/messages/octomap_msgs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-
-from .std_msgs import ROSmsg
-from .std_msgs import Header
-from .std_msgs import Time
-
-from .geometry_msgs import Pose
-
-
-class Octomap(ROSmsg):
-    """http://docs.ros.org/kinetic/api/octomap_msgs/html/msg/Octomap.html"""
-
-    def __init__(self, header=None, binary=False, id='', resolution=0., data=None):
-        self.header = header or Header()  # Header
-        self.binary = binary  # Flag to denote a binary (only free/occupied) or full occupancy octree (.bt/.ot file)
-        self.id = id  # Class id of the contained octree
-        self.resolution = resolution  # Resolution (in m) of the smallest octree nodes
-        self.data = data  # binary serialization of octree, use conversions.h to read and write octrees
-
-
-class OctomapWithPose(ROSmsg):
-    """http://docs.ros.org/kinetic/api/octomap_msgs/html/msg/OctomapWithPose.html"""
-
-    def __init__(self, header=None, origin=None, octomap=None):
-        self.header = header or Header()  # Header
-        self.origin = origin or Pose()  # geometry_msgs/Pose  The pose of the octree with respect to the header frame
-        self.octomap = octomap or Octomap()  # octomap_msgs/Octomap  The actual octree msg
+from __future__ import absolute_import
+from __future__ import division
+from __future__ import print_function
+
+from .std_msgs import ROSmsg
+from .std_msgs import Header
+
+from .geometry_msgs import Pose
+
+
+class Octomap(ROSmsg):
+    """http://docs.ros.org/kinetic/api/octomap_msgs/html/msg/Octomap.html"""
+
+    def __init__(self, header=None, binary=False, id='', resolution=0., data=None):
+        self.header = header or Header()  # Header
+        self.binary = binary  # Flag to denote a binary (only free/occupied) or full occupancy octree (.bt/.ot file)
+        self.id = id  # Class id of the contained octree
+        self.resolution = resolution  # Resolution (in m) of the smallest octree nodes
+        self.data = data  # binary serialization of octree, use conversions.h to read and write octrees
+
+
+class OctomapWithPose(ROSmsg):
+    """http://docs.ros.org/kinetic/api/octomap_msgs/html/msg/OctomapWithPose.html"""
+
+    def __init__(self, header=None, origin=None, octomap=None):
+        self.header = header or Header()  # Header
+        self.origin = origin or Pose()  # geometry_msgs/Pose  The pose of the octree with respect to the header frame
+        self.octomap = octomap or Octomap()  # octomap_msgs/Octomap  The actual octree msg
```

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/messages/sensor_msgs.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/messages/sensor_msgs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import absolute_import
 
 from .std_msgs import ROSmsg
 from .std_msgs import Header
-from .std_msgs import Time
+
 
 class JointState(ROSmsg):
     """http://docs.ros.org/kinetic/api/sensor_msgs/html/msg/JointState.html
     """
 
     def __init__(self, header=None, name=None, position=None, velocity=None,
                  effort=None):
@@ -15,19 +15,19 @@
         self.position = position if position else []
         self.velocity = velocity if velocity else []
         self.effort = effort if effort else []
 
     @classmethod
     def from_name_and_position(cls, name, position):
         return cls(Header(), name, position, [], [])
-    
+
     @classmethod
     def from_configuration(cls):
         pass
-    
+
     @property
     def configuration(self):
         pass
 
     @classmethod
     def from_msg(cls, msg):
         header = Header.from_msg(msg['header'])
```

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/messages/services.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/messages/services.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/messages/shape_msgs.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/messages/shape_msgs.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,16 +73,16 @@
         return cls(msg['type'], msg['dimensions'])
 
 
 class Mesh(ROSmsg):
     """http://docs.ros.org/kinetic/api/shape_msgs/html/msg/Mesh.html
     """
     def __init__(self, triangles=None, vertices=None):
-        self.triangles = triangles if triangles else [] # shape_msgs/MeshTriangle[]
-        self.vertices = vertices if vertices else [] # geometry_msgs/Point[]
+        self.triangles = triangles or []  # shape_msgs/MeshTriangle[]
+        self.vertices = vertices or []  # geometry_msgs/Point[]
 
     @classmethod
     def from_mesh(cls, compas_mesh):
         """Construct a `Mesh` message from a :class:`compas.datastructures.Mesh`.
         """
         mesh_quads_to_triangles(compas_mesh)
         vertices, faces = compas_mesh.to_vertices_and_faces()
@@ -106,15 +106,15 @@
 
 class MeshTriangle(ROSmsg):
     """http://docs.ros.org/api/shape_msgs/html/msg/MeshTriangle.html
     """
     def __init__(self, vertex_indices=None):
         if len(vertex_indices) != 3:
             raise ValueError("Please specify 3 indices for face, %d given." % len(vertex_indices))
-        self.vertex_indices = vertex_indices if vertex_indices else [] # uint32[3]
+        self.vertex_indices = vertex_indices or []  # uint32[3]
 
     @classmethod
     def from_msg(cls, msg):
         vertex_indices = msg['vertex_indices']
         return cls(vertex_indices)
```

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/messages/std_msgs.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/messages/std_msgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     @classmethod
     def from_msg(cls, msg):
         return cls(**msg)
 
     def __str__(self):
         return str(self.msg)
-    
+
     def __repr__(self):
         return self.__str__
 
 
 class Time(ROSmsg):
     """http://docs.ros.org/kinetic/api/std_msgs/html/msg/Time.html
     """
@@ -51,12 +51,13 @@
     """
 
     def __init__(self, seq=0, stamp=Time(), frame_id='/world'):
         self.seq = seq
         self.stamp = stamp
         self.frame_id = frame_id
 
+
 class String(ROSmsg):
     """http://docs.ros.org/api/std_msgs/html/msg/String.html
     """
     def __init__(self, data=''):
         self.data = data
```

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/messages/trajectory_msgs.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/messages/trajectory_msgs.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/planner_backend.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/planner_backend.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/planner_backend_moveit.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/planner_backend_moveit.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/ros/__init__.py` & `compas_fab-0.9.0/src/compas_fab/backends/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,60 @@
 """
-*******************************************************************************
-compas_fab.backends.ros
-*******************************************************************************
+********************************************************************************
+compas_fab.backends
+********************************************************************************
 
-.. module:: compas_fab.backends.ros
+.. currentmodule:: compas_fab.backends
 
-Package with functionality to interact with `ROS <http://ros.org/>`_.
+This package contains classes backends for simulation, planning and execution.
+
+V-REP
+-----
 
 .. autosummary::
     :toctree: generated/
+    :nosignatures:
+
+    VrepClient
+
+ROS
+---
+
+.. autosummary::
+    :toctree: generated/
+    :nosignatures:
 
     RosClient
     RosFileServerLoader
+
+Long-running tasks
+------------------
+
+.. autosummary::
+    :toctree: generated/
+    :nosignatures:
+
+    FutureResult
+    CancellableFutureResult
+
+Exceptions
+----------
+
+.. autosummary::
+    :toctree: generated/
+    :nosignatures:
+
+    BackendError
     RosError
     RosValidationError
+    VrepError
 
 """
 
-from __future__ import absolute_import
-
-from .client import *
-from .exceptions import *
-from .fileserver_loader import *
-from .direct_ur_action_client import *
-from .messages import *
+from .exceptions import *               # noqa: F401,F403
+from .tasks import *                    # noqa: F401,F403
+from .ros.client import *               # noqa: F401,F403
+from .ros.exceptions import *           # noqa: F401,F403
+from .ros.fileserver_loader import *    # noqa: F401,F403
+from .vrep.client import *              # noqa: F401,F403
 
 __all__ = [name for name in dir() if not name.startswith('_')]
```

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/tasks.py` & `compas_fab-0.9.0/src/compas_fab/backends/tasks.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/vrep/client.py` & `compas_fab-0.9.0/src/compas_fab/backends/vrep/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from __future__ import print_function
 
 import logging
-import math
 import socket
 from timeit import default_timer as timer
 
-from compas.datastructures import Mesh
 from compas.geometry import Frame
 from compas.geometry import matrix_from_frame
 
 from compas_fab.backends.exceptions import BackendError
 from compas_fab.backends.vrep.remote_api import vrep
 from compas_fab.robots import Configuration
-from compas_fab.robots import Robot
 
 DEFAULT_SCALE = 1.
 DEFAULT_OP_MODE = vrep.simx_opmode_blocking
 CHILD_SCRIPT_TYPE = vrep.sim_scripttype_childscript
 LOG = logging.getLogger('compas_fab.backends.vrep.client')
 
 __all__ = [
@@ -57,17 +54,17 @@
         ...     print ('Connected: %s' % client.is_connected)
         Connected: True
 
     Note:
         For more examples, check out the :ref:`V-REP examples page <examples_vrep>`.
     """
     SUPPORTED_PLANNERS = ('bitrrt', 'bkpiece1', 'est', 'kpiece1',
-                           'lazyprmstar', 'lbkpiece1', 'lbtrrt', 'pdst',
-                           'prm', 'prrt', 'rrt', 'rrtconnect', 'rrtstar',
-                           'sbl', 'stride', 'trrt')
+                          'lazyprmstar', 'lbkpiece1', 'lbtrrt', 'pdst',
+                          'prm', 'prrt', 'rrt', 'rrtconnect', 'rrtstar',
+                          'sbl', 'stride', 'trrt')
 
     def __init__(self, host='127.0.0.1', port=19997, scale=DEFAULT_SCALE, lua_script='RFL', debug=False):
         super(VrepClient, self).__init__()
         self.client_id = None
         self.host = resolve_host(host)
         self.port = port
         self.default_timeout_in_ms = -50000000
@@ -172,15 +169,15 @@
 
         It takes a list containing one value per configurable joint. Each value
         ranges from 0 to 1, where 1 indicates the axis is blocked and cannot
         move during inverse kinematic solving. A value of 1 on any of these
         effectively removes one degree of freedom (DOF).
 
         Args:
-            robot (:class:`Robot`): Robot instance.
+            robot (:class:`compas_fab.robots.Robot`): Robot instance.
             metric_values (:obj:`list` of :obj:`float`): List containing one value
                 per configurable joint. Each value ranges from 0 to 1.
         """
         assert_robot(robot)
 
         vrep.simxCallScriptFunction(self.client_id,
                                     self.lua_script,
@@ -188,15 +185,15 @@
                                     [robot.model.attr['index']], metric_values, [],
                                     bytearray(), DEFAULT_OP_MODE)
 
     def set_robot_pose(self, robot, frame):
         """Moves the robot to a given pose, specified as a frame.
 
         Args:
-            robot (:class:`Robot`): Robot instance to move.
+            robot (:class:`compas_fab.robots.Robot`): Robot instance to move.
             frame (:class:`Frame`): Target or goal frame.
 
         Returns:
             An instance of :class:`Configuration` found for the given pose.
         """
         assert_robot(robot)
 
@@ -211,15 +208,15 @@
 
         return config
 
     def set_robot_config(self, robot, config):
         """Moves the robot to the specified configuration.
 
         Args:
-            robot (:class:`Robot`): Robot instance to move.
+            robot (:class:`compas_fab.robots.Robot`): Robot instance to move.
             config (:class:`Configuration` instance): Describes the position of the
                 robot as an instance of :class:`Configuration`.
 
         Examples:
 
             >>> from compas_fab.robots import *
             >>> with VrepClient() as client:
@@ -239,15 +236,15 @@
         self.run_child_script('moveRobotFK',
                               [], values, ['robot' + robot.name])
 
     def get_robot_config(self, robot):
         """Gets the current configuration of the specified robot.
 
         Args:
-            robot (:class:`Robot`): Robot instance.
+            robot (:class:`compas_fab.robots.Robot`): Robot instance.
 
         Examples:
 
             >>> from compas_fab.robots import *
             >>> with VrepClient() as client:
             ...     config = client.get_robot_config(rfl.Robot('A'))
 
@@ -261,37 +258,37 @@
                                                       [], [])
         return config_from_vrep(config, self.scale)
 
     def forward_kinematics(self, robot):
         """Calculates forward kinematics to get the current end-effector pose.
 
         Args:
-            robot (:class:`Robot`): Robot instance.
+            robot (:class:`compas_fab.robots.Robot`): Robot instance.
 
         Examples:
 
             >>> from compas_fab.robots import *
             >>> with VrepClient() as client:
             ...     frame = client.forward_kinematics(rfl.Robot('A'))
 
         Returns:
             An instance of :class:`Frame`.
         """
         assert_robot(robot)
 
         _res, _, pose, _, _ = self.run_child_script('getIkTipPose',
-                                                     [robot.model.attr['index']],
-                                                     [], [])
+                                                    [robot.model.attr['index']],
+                                                    [], [])
         return vrep_pose_to_frame(pose, self.scale)
 
     def inverse_kinematics(self, robot, goal_frame, metric_values=None, gantry_joint_limits=None, arm_joint_limits=None, max_trials=None, max_results=1):
         """Calculates inverse kinematics to find valid robot configurations for the specified goal frame.
 
         Args:
-            robot (:class:`Robot`): Robot instance.
+            robot (:class:`compas_fab.robots.Robot`): Robot instance.
             goal_frame (:class:`Frame`): Target or goal frame.
             metric_values (:obj:`list` of :obj:`float`): List containing one value
                 per configurable joint. Each value ranges from 0 to 1,
                 where 1 indicates the axis/joint is blocked and cannot
                 move during inverse kinematic solving.
             gantry_joint_limits (:obj:`list` of `float`): List of 6 floats defining the upper/lower limits of
                 gantry joints. Use this if you want to restrict the area in which to search for states.
@@ -353,15 +350,15 @@
 
         return final_states
 
     def pick_building_member(self, robot, building_member_mesh, pickup_frame, metric_values=None):
         """Picks up a building member and attaches it to the robot.
 
         Args:
-            robot (:class:`Robot`): Robot instance to use for pick up.
+            robot (:class:`compas_fab.robots.Robot`): Robot instance to use for pick up.
             building_member_mesh (:class:`compas.datastructures.Mesh`): Mesh
                 of the building member that will be attached to the robot.
             pickup_pose (:class:`Frame`): Pickup frame.
             metric_values (:obj:`list` of :obj:`float`): List containing one value
                 per configurable joint. Each value ranges from 0 to 1,
                 where 1 indicates the axis/joint is blocked and cannot
                 move during inverse kinematic solving.
@@ -451,15 +448,15 @@
                               gantry_joint_limits=None, arm_joint_limits=None, shallow_state_search=True, optimize_path_length=False):
         """Find a path plan to move the selected robot from its current position to one of the `goal_configs`.
 
         This function is useful when it is required to get a path plan that ends in one
         specific goal configuration.
 
         Args:
-            robot (:class:`Robot`): Robot instance to move.
+            robot (:class:`compas_fab.robots.Robot`): Robot instance to move.
             goal_configs (:obj:`list` of :class:`Configuration`): List of target or goal configurations.
             metric_values (:obj:`list` of :obj:`float`): List containing one value
                 per configurable joint. Each value ranges from 0 to 1,
                 where 1 indicates the axis/joint is blocked and cannot
                 move during inverse kinematic solving.
             collision_meshes (:obj:`list` of :class:`compas.datastructures.Mesh`): Collision meshes
                 to be taken into account when calculating the motion plan.
@@ -489,15 +486,15 @@
 
     def plan_motion(self, robot, goal_frame, metric_values=None, collision_meshes=None,
                     planner_id='rrtconnect', trials=1, resolution=0.02,
                     gantry_joint_limits=None, arm_joint_limits=None, shallow_state_search=True, optimize_path_length=False):
         """Find a path plan to move the selected robot from its current position to the `goal_frame`.
 
         Args:
-            robot (:class:`Robot`): Robot instance to move.
+            robot (:class:`compas_fab.robots.Robot`): Robot instance to move.
             goal_frame (:class:`Frame`): Target or goal frame.
             metric_values (:obj:`list` of :obj:`float`): List containing one value
                 per configurable joint. Each value ranges from 0 to 1,
                 where 1 indicates the axis/joint is blocked and cannot
                 move during inverse kinematic solving.
             collision_meshes (:obj:`list` of :class:`compas.datastructures.Mesh`): Collision meshes
                 to be taken into account when calculating the motion plan.
@@ -525,15 +522,15 @@
                                     metric_values, collision_meshes, planner_id, trials, resolution,
                                     gantry_joint_limits, arm_joint_limits, shallow_state_search, optimize_path_length)
 
     def add_building_member(self, robot, building_member_mesh):
         """Adds a building member to the 3D scene and attaches it to the robot.
 
         Args:
-            robot (:class:`Robot`): Robot instance to attach the building member to.
+            robot (:class:`compas_fab.robots.Robot`): Robot instance to attach the building member to.
             building_member_mesh (:class:`compas.datastructures.Mesh`): Mesh
                 of the building member that will be attached to the robot.
 
         Returns:
             int: Object handle (identifier) assigned to the building member.
 
         .. note::
```

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/remoteApi.dll` & `compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/remoteApi.dll`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/remoteApi.dylib` & `compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/remoteApi.dylib`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/remoteApi.so` & `compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/remoteApi.so`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/vrep.py` & `compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/vrep.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/vrep/remote_api/vrepConst.py` & `compas_fab-0.9.0/src/compas_fab/backends/vrep/remote_api/vrepConst.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/vrep/__init__.py` & `compas_fab-0.9.0/src/compas_fab/backends/vrep/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/backends/__init__.py` & `compas_fab-0.9.0/src/compas_fab/backends/ros/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,28 @@
 """
-********************************************************************************
-compas_fab.backends
-********************************************************************************
+*******************************************************************************
+compas_fab.backends.ros
+*******************************************************************************
 
-.. currentmodule:: compas_fab.backends
+.. module:: compas_fab.backends.ros
 
-This package contains classes backends for simulation, planning and execution.
-
-V-REP
------
+Package with functionality to interact with `ROS <http://ros.org/>`_.
 
 .. autosummary::
     :toctree: generated/
-    :nosignatures:
-
-    VrepClient
-
-ROS
----
-
-.. autosummary::
-    :toctree: generated/
-    :nosignatures:
 
     RosClient
     RosFileServerLoader
-
-Long-running tasks
-------------------
-
-.. autosummary::
-    :toctree: generated/
-    :nosignatures:
-
-    FutureResult
-    CancellableFutureResult
-
-Exceptions
-----------
-
-.. autosummary::
-    :toctree: generated/
-    :nosignatures:
-
-    BackendError
     RosError
     RosValidationError
-    VrepError
 
 """
 
-from .exceptions import *
-from .tasks import *
-from .ros.client import *
-from .ros.exceptions import *
-from .ros.fileserver_loader import *
-from .vrep.client import *
+from __future__ import absolute_import
+
+from .client import *                     # noqa: F401,F403
+from .exceptions import *                 # noqa: F401,F403
+from .fileserver_loader import *          # noqa: F401,F403
+from .direct_ur_action_client import *    # noqa: F401,F403
+from .messages import *                   # noqa: F401,F403
 
 __all__ = [name for name in dir() if not name.startswith('_')]
```

### Comparing `compas_fab-0.8.0/src/compas_fab/blender/artists.py` & `compas_fab-0.9.0/src/compas_fab/blender/artists.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from __future__ import absolute_import
 from __future__ import division
 from __future__ import print_function
 
-import time
-
-import compas
 from compas_blender import draw_mesh
 
 from compas_fab.artists import BaseRobotArtist
 
 try:
     import mathutils
 except ImportError:
```

### Comparing `compas_fab-0.8.0/src/compas_fab/blender/__init__.py` & `compas_fab-0.9.0/src/compas_fab/blender/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/planning_scene/cone.stl` & `compas_fab-0.9.0/src/compas_fab/data/planning_scene/cone.stl`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/planning_scene/timber_beam.obj` & `compas_fab-0.9.0/src/compas_fab/data/planning_scene/timber_beam.obj`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/planning_scene/timber_structure.obj` & `compas_fab-0.9.0/src/compas_fab/data/planning_scene/timber_structure.obj`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur5_moveit_config/config/ur5.srdf` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur5_moveit_config/config/ur5.srdf`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/base.stl` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/base.stl`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/forearm.stl` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/forearm.stl`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/shoulder.stl` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/shoulder.stl`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/upperarm.stl` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/upperarm.stl`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist1.stl` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist1.stl`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist2.stl` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist2.stl`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist3.stl` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/collision/wrist3.stl`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/base.obj` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/base.obj`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/forearm.obj` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/forearm.obj`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/shoulder.obj` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/shoulder.obj`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/upperarm.obj` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/upperarm.obj`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist1.obj` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist1.obj`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist2.obj` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist2.obj`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist3.obj` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/meshes/ur5/visual/wrist3.obj`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/data/universal_robot/ur_description/urdf/ur5.urdf` & `compas_fab-0.9.0/src/compas_fab/data/universal_robot/ur_description/urdf/ur5.urdf`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/ghpython/artists.py` & `compas_fab-0.9.0/src/compas_fab/ghpython/artists.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/ghpython/__init__.py` & `compas_fab-0.9.0/src/compas_fab/ghpython/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,10 +22,10 @@
 
     RobotArtist
 
 
 """
 
 from .artists import RobotArtist
-from .path_planning import *
+from .path_planning import *          # noqa: F401,F403
 
-__all__ = ['RobotArtist', 'PathVisualizer']
+__all__ = ['RobotArtist']
```

### Comparing `compas_fab-0.8.0/src/compas_fab/rhino/artists.py` & `compas_fab-0.9.0/src/compas_fab/rhino/artists.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from __future__ import division
 from __future__ import print_function
 
 import time
 
 import compas
 from compas.utilities import rgb_to_rgb
-import compas_rhino
 
 from compas_fab.artists import BaseRobotArtist
 
 try:
     import Rhino.Geometry
     import rhinoscriptsyntax as rs
     import scriptcontext as sc
@@ -25,15 +24,15 @@
 ]
 
 
 class RobotArtist(BaseRobotArtist):
     """Visualizer for robots inside a Rhino environment."""
 
     # TODO: Add layer (e.g. __init__(self, robot, layer=None))
-    def __init__(self, robot): #, layer=None):
+    def __init__(self, robot):
         super(RobotArtist, self).__init__(robot)
 
     def transform(self, native_mesh, transformation):
         T = xform_from_transformation(transformation)
         native_mesh.Transform(T)
 
     def draw_geometry(self, geometry, color=None):
@@ -85,24 +84,14 @@
 
         """
         if timeout:
             time.sleep(timeout)
         rs.EnableRedraw(True)
         rs.Redraw()
 
-    # def clear_layer(self):
-    #     """Clear the main layer of the artist."""
-    #     if self.layer:
-    #         compas_rhino.clear_layer(self.layer)
-    #     else:
-    #         compas_rhino.clear_current_layer()
-
-    # def clear(self):
-    #     """Clear the robot."""
-    #     self.clear_robot()
 
 # TODO: Move to compas_rhino.geometry
 def xform_from_transformation(transformation):
     """Creates a Rhino Transform instance from a :class:`Transformation`.
 
     Args:
         transformation (:class:`Transformation`): the transformation.
```

### Comparing `compas_fab-0.8.0/src/compas_fab/rhino/install.py` & `compas_fab-0.9.0/src/compas_fab/rhino/install.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/rhino/uninstall.py` & `compas_fab-0.9.0/src/compas_fab/rhino/uninstall.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/rhino/__init__.py` & `compas_fab-0.9.0/src/compas_fab/rhino/__init__.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/configuration.py` & `compas_fab-0.9.0/src/compas_fab/robots/configuration.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/conftest.py` & `compas_fab-0.9.0/src/compas_fab/robots/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import math
 import time
 
 import pytest
 from compas.datastructures import Mesh
 from compas.geometry import Frame
 from compas.geometry import Scale
+from compas.geometry import Rotation
 
 import compas_fab
 from compas_fab.backends import RosClient
 from compas_fab.robots.ur5 import Robot
 
 
 @pytest.fixture(autouse=True)
 def add_imports(doctest_namespace):
     doctest_namespace["math"] = math
     doctest_namespace["time"] = time
     doctest_namespace["Mesh"] = Mesh
     doctest_namespace["Frame"] = Frame
     doctest_namespace["Scale"] = Scale
     doctest_namespace["compas_fab"] = compas_fab
+    doctest_namespace["Rotation"] = Rotation
 
 
 @pytest.fixture(scope="session", autouse=True)
 def connect_to_ros(doctest_namespace):
     client = RosClient()
     client.run()
     robot = Robot(client)
```

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/constraints.py` & `compas_fab-0.9.0/src/compas_fab/robots/constraints.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/path_plan.py` & `compas_fab-0.9.0/src/compas_fab/robots/path_plan.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/planning_scene.py` & `compas_fab-0.9.0/src/compas_fab/robots/planning_scene.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/rfl.py` & `compas_fab-0.9.0/src/compas_fab/robots/rfl.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/robot.py` & `compas_fab-0.9.0/src/compas_fab/robots/robot.py`

 * *Files 0% similar despite different names*

```diff
@@ -788,15 +788,16 @@
         Examples
         --------
         >>> frame = Frame([0.4, 0.3, 0.4], [0, 1, 0], [0, 0, 1])
         >>> tolerance_position = 0.001
         >>> tolerances_axes = [math.radians(1)]
         >>> group = robot.main_group_name
         >>> robot.constraints_from_frame(frame, tolerance_position, tolerances_axes, group)
-        [PositionConstraint('ee_link', BoundingVolume(2, Sphere(Point(0.400, 0.300, 0.400), 0.001)), 1.0), OrientationConstraint('ee_link', [0.5, 0.5, 0.5, 0.5], [0.017453292519943295, 0.017453292519943295, 0.017453292519943295], 1.0)]
+        [PositionConstraint('ee_link', BoundingVolume(2, Sphere(Point(0.400, 0.300, 0.400), 0.001)), 1.0), \
+        OrientationConstraint('ee_link', [0.5, 0.5, 0.5, 0.5], [0.017453292519943295, 0.017453292519943295, 0.017453292519943295], 1.0)]
 
         Notes
         -----
         There are many other possibilities of how to create a position and
         orientation constraint. Checkout :class:`compas_fab.robots.PositionConstraint`
         and :class:`compas_fab.robots.OrientationConstraint`.
 
@@ -822,15 +823,20 @@
 
         Examples
         --------
         >>> configuration = Configuration.from_revolute_values([-0.042, 4.295, -4.110, -3.327, 4.755, 0.])
         >>> tolerances = [math.radians(5)] * 6
         >>> group = robot.main_group_name
         >>> robot.constraints_from_configuration(configuration, tolerances, group)
-        [JointConstraint('shoulder_pan_joint', -0.042, 0.08726646259971647, 1.0), JointConstraint('shoulder_lift_joint', 4.295, 0.08726646259971647, 1.0), JointConstraint('elbow_joint', -4.11, 0.08726646259971647, 1.0), JointConstraint('wrist_1_joint', -3.327, 0.08726646259971647, 1.0), JointConstraint('wrist_2_joint', 4.755, 0.08726646259971647, 1.0), JointConstraint('wrist_3_joint', 0.0, 0.08726646259971647, 1.0)]
+        [JointConstraint('shoulder_pan_joint', -0.042, 0.08726646259971647, 1.0), \
+        JointConstraint('shoulder_lift_joint', 4.295, 0.08726646259971647, 1.0), \
+        JointConstraint('elbow_joint', -4.11, 0.08726646259971647, 1.0), \
+        JointConstraint('wrist_1_joint', -3.327, 0.08726646259971647, 1.0), \
+        JointConstraint('wrist_2_joint', 4.755, 0.08726646259971647, 1.0), \
+        JointConstraint('wrist_3_joint', 0.0, 0.08726646259971647, 1.0)]
 
         Raises
         ------
         ValueError
             If the passed configuration does not correspond to the group.
         ValueError
             If the passed tolerances have a different length than the configuration.
```

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/semantics.py` & `compas_fab-0.9.0/src/compas_fab/robots/semantics.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/time_.py` & `compas_fab-0.9.0/src/compas_fab/robots/time_.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/trajectory.py` & `compas_fab-0.9.0/src/compas_fab/robots/trajectory.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/units.py` & `compas_fab-0.9.0/src/compas_fab/robots/units.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/ur5.py` & `compas_fab-0.9.0/src/compas_fab/robots/ur5.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/robots/__init__.py` & `compas_fab-0.9.0/src/compas_fab/robots/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     :toctree: generated/
     :nosignatures:
 
     Robot
     RobotSemantics
     Configuration
     Duration
+    Wrench
+    Inertia
 
 Path planning
 -------------
 .. autosummary::
     :toctree: generated/
     :nosignatures:
 
@@ -65,18 +67,20 @@
     :nosignatures:
 
     to_degrees
     to_radians
 
 """
 
-from .configuration import *
-from .constraints import *
-from .path_plan import *
-from .planning_scene import *
-from .units import *
-from .robot import *
-from .semantics import *
-from .time_ import *
-from .trajectory import *
+from .configuration import *          # noqa: F401,F403
+from .constraints import *            # noqa: F401,F403
+from .path_plan import *              # noqa: F401,F403
+from .planning_scene import *         # noqa: F401,F403
+from .units import *                  # noqa: F401,F403
+from .robot import *                  # noqa: F401,F403
+from .semantics import *              # noqa: F401,F403
+from .time_ import *                  # noqa: F401,F403
+from .trajectory import *             # noqa: F401,F403
+from .wrench import *                 # noqa: F401,F403
+from .inertia import *                # noqa: F401,F403
 
 __all__ = [name for name in dir() if not name.startswith('_')]
```

### Comparing `compas_fab-0.8.0/src/compas_fab/sensors/base.py` & `compas_fab-0.9.0/src/compas_fab/sensors/base.py`

 * *Files identical despite different names*

### Comparing `compas_fab-0.8.0/src/compas_fab/sensors/baumer.py` & `compas_fab-0.9.0/src/compas_fab/sensors/baumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     ...         sensor.set_measurement_type('Edge L rise')                          # doctest: +SKIP
     ...         sensor.set_precision(2)                                             # doctest: +SKIP
     ...         data = sensor.get_measurement()                                     # doctest: +SKIP
     """
     FRAME_HEAD = '{%s,%s,%s'
     FRAME_TAIL = '%s%s}'
     BROADCAST_ADDRESS = 0
-    MEASUREMENT_TYPES = ('Edge L rise', 'Edge L fall', 'Edge R rise', 'Edge R fall', 'Width', 'Center width', 'Gap', 'Center gap')
+    MEASUREMENT_TYPES = ('Edge L rise', 'Edge L fall', 'Edge R rise',
+                         'Edge R fall', 'Width', 'Center width', 'Gap', 'Center gap')
     QUALITY = {
         0: 'Valid',
         1: 'Low signal',
         2: 'No edge',
         3: 'Low signal, no edge',
         4: 'No signal'}
     ERROR_CODES = {
@@ -364,20 +365,20 @@
     ...         data = sensor.get_measurement()                                     # doctest: +SKIP
     """
 
     FRAME_HEAD = ':%s%s;%s;'
     FRAME_TAIL = '%s%s\r\n'
     BROADCAST_ADDRESS = 0
     MEASUREMENT_TYPES = {
-        'Diameter' : 28,
-        'X_center' : 29,
-        'Z_center' : 30,
-        'X_left'   : 31,
-        'X_right'  : 32,
-        'Z_top'    : 33}
+        'Diameter': 28,
+        'X_center': 29,
+        'Z_center': 30,
+        'X_left': 31,
+        'X_right': 32,
+        'Z_top': 33}
     QUALITY = {
         0: 'Valid',
         1: 'Low signal',
         2: 'No edge',
         3: 'Low signal, no edge',
         4: 'No signal'}
     ERROR_CODES = {
@@ -432,29 +433,31 @@
         return self.FRAME_TAIL % (frame, self.calculate_checksum(frame))
 
     def calculate_checksum(self, command):
         """Checks that message is complete.
 
         Note
         ----
-        See `RS-485 Protocol Structure <https://www.baumer.com/ae/en/product-overview/2d-3d-sensors/profile-sensors-/measurement-of-round-objects/oxc7-x0250-ii1250-ti/p/medias/__secure__/en_BA_RS485_Protocol_Structure.pdf?mediaPK=8799860686878>`_ for more info.
+        See `RS-485 Protocol Structure <https://www.baumer.com/ae/en/product-overview/2d-3d-sensors/profile-sensors-/measurement-of-round-objects/\
+        oxc7-x0250-ii1250-ti/p/medias/__secure__/en_BA_RS485_Protocol_Structure.pdf?mediaPK=8799860686878>`_ for more info.
         """
         return '****'
 
     def get_payload(self, result):
         """Gets payload."""
         frame_head = result[:-6]
         result_type = frame_head[3]
 
         if result_type == 'a':
             raise SensorTimeoutError('Sensor has not completed reading')
 
         if result_type == 'E':
             error_index = frame_head.split(';')
-            raise ProtocolError('Application error, Result=%s' % frame_head + 'Error type: ' + str(self.ERROR_CODES[str(error_index[1])]))
+            raise ProtocolError('Application error, Result=%s' % frame_head +
+                                'Error type: ' + str(self.ERROR_CODES[str(error_index[1])]))
 
         if result_type == 'B':
             raise ProtocolError('Sensor is busy, Result=%s' % frame_head)
 
         return result[5:-6].split(';')
 
     def send_command(self, address, command, data=None):
```

### Comparing `compas_fab-0.8.0/src/compas_fab/sensors/__init__.py` & `compas_fab-0.9.0/src/compas_fab/sensors/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -28,11 +28,11 @@
     :nosignatures:
 
     PosCon3D
     PosConCM
 
 """
 
-from .base import *
-from .baumer import *
+from .base import *         # noqa: F401,F403
+from .baumer import *       # noqa: F401,F403
 
 __all__ = [name for name in dir() if not name.startswith('_')]
```

### Comparing `compas_fab-0.8.0/src/compas_fab/utilities/filesystem.py` & `compas_fab-0.9.0/src/compas_fab/utilities/filesystem.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,22 +23,23 @@
     directory = os.path.abspath(directory)
     files = []
     extensions = [".%s" % ext for ext in extensions if ext[0] != "."]
     for item in os.listdir(directory):
         item_fullpath = os.path.join(directory, item)
         if os.path.isfile(item_fullpath):
             if len(extensions):
-                found = reduce(lambda x, y: x or y, [item.endswith(ext) for ext in extensions])
+                found = any([item.endswith(ext) for ext in extensions])
                 if not found:
                     continue
             if fullpath:
                 files.append(item_fullpath)
             else:
                 files.append(item)
     return files
 
 
 if __name__ == "__main__":
 
-    path = os.path.join(os.path.dirname(__file__), "..", "robots", "ur", "ur10", "model")
+    path = os.path.join(os.path.dirname(__file__), "..",
+                        "robots", "ur", "ur10", "model")
     os.listdir(path)
     print(list_files_in_directory(path, fullpath=True, extensions=["obj"]))
```

### Comparing `compas_fab-0.8.0/src/compas_fab/utilities/file_io.py` & `compas_fab-0.9.0/src/compas_fab/utilities/file_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,51 +6,55 @@
     'read_csv_to_dictionary',
     'write_data_to_json',
     'read_data_from_json',
     'write_data_to_pickle',
     'read_data_from_pickle'
 ]
 
+
 def read_csv_to_dictionary(csvfile, delimiter=';'):
     """Reads a csv file and returns a dictionary with the respective keys
     specified in the first row of the csv file.
     """
     data = []
     with open(csvfile, mode='r') as infile:
         reader = csv.reader(infile, delimiter=delimiter)
         for i, rows in enumerate(reader):
             data.append(rows)
         infile.close()
-    data = zip(*data) # transpose data
+    data = zip(*data)  # transpose data
     data_dict = {}
     for l in data:
         key = l[0]
         values = list(l[1:])
         data_dict.update({key: values})
     return data_dict
 
 
 def write_data_to_json(data, file):
     """Write data to json file.
     """
     with open(file, 'w') as f:
         json.dump(data, f)
 
+
 def read_data_from_json(file):
     """Read data from json file.
     """
     with open(file) as f:
         data = json.load(f)
     return data
 
+
 def write_data_to_pickle(data, file):
     """Write data to pickle file.
     """
     with open(file, 'wb') as f:
         pickle.dump(data, f)
 
+
 def read_data_from_pickle(file):
     """Read data from pickle file.
     """
     with open(file, 'rb') as f:
         data = pickle.load(f)
     return data
```

### Comparing `compas_fab-0.8.0/src/compas_fab/utilities/numbers.py` & `compas_fab-0.9.0/src/compas_fab/utilities/numbers.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,103 +15,111 @@
 
 def map_range(value, from_min, from_max, to_min, to_max):
     """Performs a linear interpolation of a value within the range of [from_min,
         from_max] to another range of [to_min, to_max].
     """
     from_range = from_max - from_min
     to_range = to_max - to_min
-    value_scaled = (value - from_min)/float(from_range)
+    value_scaled = (value - from_min) / float(from_range)
     return to_min + (value_scaled * to_range)
 
+
 def range_geometric_row(number, d, r=1.1):
     """Returns a list of numbers with a certain relation to each other.
 
     The function divides one number into a list of d numbers [n0, n1, ...], such
     that their sum is number and the relation between the numbers is defined
     with n1 = n0 / r, n2 = n1 / r, n3 = n2 / r, ...
     """
     if r <= 0:
         raise ValueError("r must be > 0")
 
-    n0 = number/((1 - (1/r)**d)/(1 - 1/r))
+    n0 = number / ((1 - (1 / r)**d) / (1 - 1 / r))
 
     numbers = [n0]
     for i in range(d - 1):
         numbers.append(numbers[-1] / r)
     return numbers
 
+
 def arange(start, stop, step):
     """Returns evenly spaced values within a given interval.
 
     The function is similar to NumPy's *arange* function.
     """
     if math.fabs(stop - (start + step)) > math.fabs(stop - start):
         raise ValueError("Please check the sign of step.")
 
-    len = int(math.ceil((stop - start)/float(step)))
-    return [start + i*step for i in range(len)]
+    len = int(math.ceil((stop - start) / float(step)))
+    return [start + i * step for i in range(len)]
+
 
 def diffs(l1, l2):
     """Returns the element-wise differences between two lists.
 
     Raises
     ------
     ValueError
         If 2 lists of different length are passed.
     """
     if len(l1) != len(l2):
         raise ValueError("Pass 2 lists of equal length.")
     return [math.fabs(a - b) for a, b in zip(l1, l2)]
 
+
 def allclose(l1, l2, tol=1e-05):
     """Returns True if two lists are element-wise equal within a tolerance.
 
     The function is similar to NumPy's *allclose* function.
     """
     for a, b in zip(l1, l2):
         if math.fabs(a - b) > tol:
             return False
     return True
 
+
 def argsort(numbers):
     """Returns the indices that would sort an array of numbers.
 
     The function is similar to NumPy's *argsort* function.
 
     Note
     ----
     For a large list of numbers reconsider using NumPy's *argsort* function,
     since this function might take too long.
     """
     return [i[0] for i in sorted(enumerate(numbers), key=lambda x:x[1])]
 
+
 def argmin(numbers):
     """Returns the index of the minimum value in numbers.
 
     The function is similar to NumPy's *argmin* function.
 
     Note
     ----
     For a large list of numbers reconsider using NumPy's *argmin* function,
     since this function might take too long.
     """
     return argsort(numbers)[0]
 
+
 def argmax(numbers):
     """Returns the index of the maximum value in numbers.
 
     The function is similar to NumPy's *argmax* function.
 
     Note
     ----
     For a large list of numbers reconsider using NumPy's *argmax* function,
     since this function might take too long.
     """
     return argsort(numbers)[-1]
 
+
 def clamp(value, min_value, max_value):
     """Clamps a value witin the bound [min_value, max_value]
 
     Returns
     -------
     float
     """
@@ -119,11 +127,11 @@
         raise ValueError("min_value must be bigger than max_value")
     return float(min(max(value, min_value), max_value))
 
 
 if __name__ == "__main__":
     print(map_range(2, 0, 10, 0, 100))
     print(arange(3, -4, -0.2))
-    print(argsort([34,1,7,2,100]))
+    print(argsort([34, 1, 7, 2, 100]))
     print(clamp(5, 1, 4))
     print(clamp(0, 1, 4))
-    print(clamp(3, 1, 4))
+    print(clamp(3, 1, 4))
```

### Comparing `compas_fab-0.8.0/src/compas_fab.egg-info/PKG-INFO` & `compas_fab-0.9.0/src/compas_fab.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: compas-fab
-Version: 0.8.0
+Version: 0.9.0
 Summary: Robotic fabrication package for the COMPAS Framework
 Home-page: https://github.com/compas-dev/compas_fab
 Author: Gramazio Kohler Research
 Author-email: gramaziokohler@arch.ethz.ch
 License: MIT license
 Description: ============================================================
         COMPAS FAB: Robotic Fabrication for COMPAS
@@ -118,14 +118,27 @@
         =========
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_
         and this project adheres to `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
         
+        0.9.0
+        ----------
+        
+        **Added**
+        
+        * Added ``load_robot`` method to ROS client to simplify loading robots from running ROS setup.
+        * Added ``compas_fab.robots.Wrench``: a Wrench class representing force in free space, separated into its linear (force) and angular (torque) parts.
+        * Added ``compas_fab.robots.Inertia``: a Inertia class representing spatial distribution of mass in a rigid body
+        
+        **Changed**
+        
+        * Updated to COMPAS 0.11
+        
         0.8.0
         ----------
         
         **Changed**
         
         * Updated to COMPAS 0.10
         * Add better support for passive joints on IK, Cartesian and Kinematic planning
```

### Comparing `compas_fab-0.8.0/src/compas_fab.egg-info/SOURCES.txt` & `compas_fab-0.9.0/src/compas_fab.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 src/compas_fab/backends/ros/messages/services.py
 src/compas_fab/backends/ros/messages/shape_msgs.py
 src/compas_fab/backends/ros/messages/std_msgs.py
 src/compas_fab/backends/ros/messages/trajectory_msgs.py
 src/compas_fab/backends/vrep/__init__.py
 src/compas_fab/backends/vrep/client.py
 src/compas_fab/backends/vrep/conftest.py
-src/compas_fab/backends/vrep/coordinator.py
 src/compas_fab/backends/vrep/remote_api/__init__.py
 src/compas_fab/backends/vrep/remote_api/remoteApi.dll
 src/compas_fab/backends/vrep/remote_api/remoteApi.dylib
 src/compas_fab/backends/vrep/remote_api/remoteApi.so
 src/compas_fab/backends/vrep/remote_api/vrep.py
 src/compas_fab/backends/vrep/remote_api/vrepConst.py
 src/compas_fab/blender/__init__.py
@@ -78,23 +77,25 @@
 src/compas_fab/rhino/artists.py
 src/compas_fab/rhino/install.py
 src/compas_fab/rhino/uninstall.py
 src/compas_fab/robots/__init__.py
 src/compas_fab/robots/configuration.py
 src/compas_fab/robots/conftest.py
 src/compas_fab/robots/constraints.py
+src/compas_fab/robots/inertia.py
 src/compas_fab/robots/path_plan.py
 src/compas_fab/robots/planning_scene.py
 src/compas_fab/robots/rfl.py
 src/compas_fab/robots/robot.py
 src/compas_fab/robots/semantics.py
 src/compas_fab/robots/time_.py
 src/compas_fab/robots/trajectory.py
 src/compas_fab/robots/units.py
 src/compas_fab/robots/ur5.py
+src/compas_fab/robots/wrench.py
 src/compas_fab/sensors/__init__.py
 src/compas_fab/sensors/base.py
 src/compas_fab/sensors/baumer.py
 src/compas_fab/sensors/exceptions.py
 src/compas_fab/utilities/__init__.py
 src/compas_fab/utilities/file_io.py
 src/compas_fab/utilities/filesystem.py
```

