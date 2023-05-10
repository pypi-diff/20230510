# Comparing `tmp/rp2040-tools-0.0.7.tar.gz` & `tmp/rp2040-tools-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rp2040-tools-0.0.7.tar", last modified: Fri Jan 13 13:22:34 2023, max compression
+gzip compressed data, was "rp2040-tools-0.0.8.tar", last modified: Wed May 10 06:35:53 2023, max compression
```

## Comparing `rp2040-tools-0.0.7.tar` & `rp2040-tools-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,41 @@
-drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-01-13 13:22:34.007582 rp2040-tools-0.0.7/
--rw-r--r--   0 1zql1      (501) staff       (20)     1059 2022-12-27 05:29:31.000000 rp2040-tools-0.0.7/LICENSE.txt
--rw-r--r--   0 1zql1      (501) staff       (20)      358 2023-01-13 13:22:34.007433 rp2040-tools-0.0.7/PKG-INFO
--rw-r--r--   0 1zql1      (501) staff       (20)       37 2023-01-03 14:09:49.000000 rp2040-tools-0.0.7/README.md
-drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-01-13 13:22:34.000585 rp2040-tools-0.0.7/rp2040/
--rw-rw-r--   0 1zql1      (501) staff       (20)        0 2023-01-04 14:48:47.000000 rp2040-tools-0.0.7/rp2040/__init__.py
--rw-rw-r--   0 1zql1      (501) staff       (20)     4529 2023-01-10 05:35:56.000000 rp2040-tools-0.0.7/rp2040/base.py
-drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-01-13 13:22:34.001427 rp2040-tools-0.0.7/rp2040/message/
--rw-r--r--   0 1zql1      (501) staff       (20)        0 2023-01-05 23:32:54.000000 rp2040-tools-0.0.7/rp2040/message/__init__.py
--rw-r--r--   0 1zql1      (501) staff       (20)        0 2023-01-10 06:45:29.000000 rp2040-tools-0.0.7/rp2040/message/drive.py
--rw-r--r--   0 1zql1      (501) staff       (20)     3248 2023-01-13 03:46:06.000000 rp2040-tools-0.0.7/rp2040/message/protocol.py
-drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-01-13 13:22:34.002175 rp2040-tools-0.0.7/rp2040/oled/
--rw-rw-r--   0 1zql1      (501) staff       (20)        0 2023-01-04 14:48:47.000000 rp2040-tools-0.0.7/rp2040/oled/__init__.py
--rw-rw-r--   0 1zql1      (501) staff       (20)     4860 2023-01-03 00:41:02.000000 rp2040-tools-0.0.7/rp2040/oled/ssd1306.py
--rw-r--r--   0 1zql1      (501) staff       (20)      613 2023-01-05 23:32:33.000000 rp2040-tools-0.0.7/rp2040/pico.py
-drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-01-13 13:22:34.004725 rp2040-tools-0.0.7/rp2040/powerhouse/
--rw-r--r--   0 1zql1      (501) staff       (20)        0 2023-01-04 14:36:04.000000 rp2040-tools-0.0.7/rp2040/powerhouse/__init__.py
--rw-r--r--   0 1zql1      (501) staff       (20)     2006 2023-01-10 06:36:54.000000 rp2040-tools-0.0.7/rp2040/powerhouse/blendComposition.py
--rw-r--r--   0 1zql1      (501) staff       (20)     1599 2023-01-10 00:16:07.000000 rp2040-tools-0.0.7/rp2040/powerhouse/engine.py
--rw-r--r--   0 1zql1      (501) staff       (20)        0 2023-01-10 05:51:23.000000 rp2040-tools-0.0.7/rp2040/powerhouse/engineGroup.py
--rw-r--r--   0 1zql1      (501) staff       (20)     2333 2023-01-10 00:16:07.000000 rp2040-tools-0.0.7/rp2040/powerhouse/servo.py
--rw-r--r--   0 1zql1      (501) staff       (20)     1089 2023-01-10 06:24:19.000000 rp2040-tools-0.0.7/rp2040/powerhouse/servoGroup.py
-drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-01-13 13:22:34.006035 rp2040-tools-0.0.7/rp2040/sensor/
--rw-rw-r--   0 1zql1      (501) staff       (20)        0 2023-01-05 06:32:27.000000 rp2040-tools-0.0.7/rp2040/sensor/__init__.py
--rw-r--r--   0 1zql1      (501) staff       (20)      519 2023-01-05 05:27:51.000000 rp2040-tools-0.0.7/rp2040/sensor/hcsr04.py
--rw-rw-r--   0 1zql1      (501) staff       (20)    10930 2023-01-03 14:09:49.000000 rp2040-tools-0.0.7/rp2040/sensor/mpu6050.py
--rw-r--r--   0 1zql1      (501) staff       (20)      158 2023-01-12 15:18:43.000000 rp2040-tools-0.0.7/rp2040/zero.py
-drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-01-13 13:22:34.007154 rp2040-tools-0.0.7/rp2040_tools.egg-info/
--rw-r--r--   0 1zql1      (501) staff       (20)      358 2023-01-13 13:22:33.000000 rp2040-tools-0.0.7/rp2040_tools.egg-info/PKG-INFO
--rw-r--r--   0 1zql1      (501) staff       (20)      626 2023-01-13 13:22:33.000000 rp2040-tools-0.0.7/rp2040_tools.egg-info/SOURCES.txt
--rw-r--r--   0 1zql1      (501) staff       (20)        1 2023-01-13 13:22:33.000000 rp2040-tools-0.0.7/rp2040_tools.egg-info/dependency_links.txt
--rw-r--r--   0 1zql1      (501) staff       (20)        7 2023-01-13 13:22:33.000000 rp2040-tools-0.0.7/rp2040_tools.egg-info/top_level.txt
--rw-r--r--   0 1zql1      (501) staff       (20)       38 2023-01-13 13:22:34.007640 rp2040-tools-0.0.7/setup.cfg
--rw-r--r--   0 1zql1      (501) staff       (20)     1001 2023-01-13 13:22:33.000000 rp2040-tools-0.0.7/setup.py
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-05-10 06:35:53.687117 rp2040-tools-0.0.8/
+-rw-r--r--   0 1zql1      (501) staff       (20)     1059 2022-12-27 05:29:31.000000 rp2040-tools-0.0.8/LICENSE.txt
+-rw-r--r--   0 1zql1      (501) staff       (20)      358 2023-05-10 06:35:53.686960 rp2040-tools-0.0.8/PKG-INFO
+-rw-r--r--   0 1zql1      (501) staff       (20)       37 2023-01-03 14:09:49.000000 rp2040-tools-0.0.8/README.md
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-05-10 06:35:53.681811 rp2040-tools-0.0.8/rp2040/
+-rw-rw-r--   0 1zql1      (501) staff       (20)        0 2023-01-04 14:48:47.000000 rp2040-tools-0.0.8/rp2040/__init__.py
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-05-10 06:35:53.682278 rp2040-tools-0.0.8/rp2040/algorithm/
+-rw-r--r--   0 1zql1      (501) staff       (20)    10083 2023-05-10 06:33:24.000000 rp2040-tools-0.0.8/rp2040/algorithm/PID.py
+-rw-r--r--   0 1zql1      (501) staff       (20)        0 2023-05-10 06:29:06.000000 rp2040-tools-0.0.8/rp2040/algorithm/__init__.py
+-rw-rw-r--   0 1zql1      (501) staff       (20)     5737 2023-05-10 06:12:15.000000 rp2040-tools-0.0.8/rp2040/base.py
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-05-10 06:35:53.682388 rp2040-tools-0.0.8/rp2040/drives/
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-05-10 06:35:53.682537 rp2040-tools-0.0.8/rp2040/drives/HC/
+-rw-r--r--   0 1zql1      (501) staff       (20)    13312 2023-05-10 03:05:22.000000 rp2040-tools-0.0.8/rp2040/drives/HC/__init__.py
+-rw-r--r--   0 1zql1      (501) staff       (20)        0 2023-04-05 03:47:36.000000 rp2040-tools-0.0.8/rp2040/drives/__init__.py
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-05-10 06:35:53.683243 rp2040-tools-0.0.8/rp2040/message/
+-rw-r--r--   0 1zql1      (501) staff       (20)        0 2023-01-05 23:32:54.000000 rp2040-tools-0.0.8/rp2040/message/__init__.py
+-rw-r--r--   0 1zql1      (501) staff       (20)        0 2023-01-10 06:45:29.000000 rp2040-tools-0.0.8/rp2040/message/drive.py
+-rw-r--r--   0 1zql1      (501) staff       (20)     3248 2023-01-13 03:46:06.000000 rp2040-tools-0.0.8/rp2040/message/protocol.py
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-05-10 06:35:53.683787 rp2040-tools-0.0.8/rp2040/oled/
+-rw-rw-r--   0 1zql1      (501) staff       (20)        0 2023-01-04 14:48:47.000000 rp2040-tools-0.0.8/rp2040/oled/__init__.py
+-rw-rw-r--   0 1zql1      (501) staff       (20)     4860 2023-01-03 00:41:02.000000 rp2040-tools-0.0.8/rp2040/oled/ssd1306.py
+-rw-r--r--   0 1zql1      (501) staff       (20)      613 2023-01-05 23:32:33.000000 rp2040-tools-0.0.8/rp2040/pico.py
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-05-10 06:35:53.685174 rp2040-tools-0.0.8/rp2040/powerhouse/
+-rw-r--r--   0 1zql1      (501) staff       (20)        0 2023-01-04 14:36:04.000000 rp2040-tools-0.0.8/rp2040/powerhouse/__init__.py
+-rw-r--r--   0 1zql1      (501) staff       (20)     2006 2023-01-10 06:36:54.000000 rp2040-tools-0.0.8/rp2040/powerhouse/blendComposition.py
+-rw-r--r--   0 1zql1      (501) staff       (20)     1599 2023-01-10 00:16:07.000000 rp2040-tools-0.0.8/rp2040/powerhouse/engine.py
+-rw-r--r--   0 1zql1      (501) staff       (20)        0 2023-01-10 05:51:23.000000 rp2040-tools-0.0.8/rp2040/powerhouse/engineGroup.py
+-rw-r--r--   0 1zql1      (501) staff       (20)     2692 2023-05-10 05:14:53.000000 rp2040-tools-0.0.8/rp2040/powerhouse/servo.py
+-rw-r--r--   0 1zql1      (501) staff       (20)     1089 2023-01-10 06:24:19.000000 rp2040-tools-0.0.8/rp2040/powerhouse/servoGroup.py
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-05-10 06:35:53.685844 rp2040-tools-0.0.8/rp2040/sensor/
+-rw-rw-r--   0 1zql1      (501) staff       (20)        0 2023-01-05 06:32:27.000000 rp2040-tools-0.0.8/rp2040/sensor/__init__.py
+-rw-r--r--   0 1zql1      (501) staff       (20)      519 2023-01-05 05:27:51.000000 rp2040-tools-0.0.8/rp2040/sensor/hcsr04.py
+-rw-rw-r--   0 1zql1      (501) staff       (20)    10930 2023-01-03 14:09:49.000000 rp2040-tools-0.0.8/rp2040/sensor/mpu6050.py
+-rw-r--r--   0 1zql1      (501) staff       (20)      158 2023-01-12 15:18:43.000000 rp2040-tools-0.0.8/rp2040/zero.py
+drwxr-xr-x   0 1zql1      (501) staff       (20)        0 2023-05-10 06:35:53.686681 rp2040-tools-0.0.8/rp2040_tools.egg-info/
+-rw-r--r--   0 1zql1      (501) staff       (20)      358 2023-05-10 06:35:53.000000 rp2040-tools-0.0.8/rp2040_tools.egg-info/PKG-INFO
+-rw-r--r--   0 1zql1      (501) staff       (20)      734 2023-05-10 06:35:53.000000 rp2040-tools-0.0.8/rp2040_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 1zql1      (501) staff       (20)        1 2023-05-10 06:35:53.000000 rp2040-tools-0.0.8/rp2040_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 1zql1      (501) staff       (20)        7 2023-05-10 06:35:53.000000 rp2040-tools-0.0.8/rp2040_tools.egg-info/top_level.txt
+-rw-r--r--   0 1zql1      (501) staff       (20)       38 2023-05-10 06:35:53.687168 rp2040-tools-0.0.8/setup.cfg
+-rw-r--r--   0 1zql1      (501) staff       (20)     1001 2023-05-10 06:35:51.000000 rp2040-tools-0.0.8/setup.py
```

### Comparing `rp2040-tools-0.0.7/LICENSE.txt` & `rp2040-tools-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rp2040-tools-0.0.7/rp2040/message/protocol.py` & `rp2040-tools-0.0.8/rp2040/message/protocol.py`

 * *Files identical despite different names*

### Comparing `rp2040-tools-0.0.7/rp2040/oled/ssd1306.py` & `rp2040-tools-0.0.8/rp2040/oled/ssd1306.py`

 * *Files identical despite different names*

### Comparing `rp2040-tools-0.0.7/rp2040/pico.py` & `rp2040-tools-0.0.8/rp2040/pico.py`

 * *Files identical despite different names*

### Comparing `rp2040-tools-0.0.7/rp2040/powerhouse/blendComposition.py` & `rp2040-tools-0.0.8/rp2040/powerhouse/blendComposition.py`

 * *Files identical despite different names*

### Comparing `rp2040-tools-0.0.7/rp2040/powerhouse/engine.py` & `rp2040-tools-0.0.8/rp2040/powerhouse/engine.py`

 * *Files identical despite different names*

### Comparing `rp2040-tools-0.0.7/rp2040/powerhouse/servo.py` & `rp2040-tools-0.0.8/rp2040/powerhouse/servo.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,28 +36,28 @@
         if speed <= 0:
             self.stop()
         elif speed > 1000:
             speed = 1000
         self.pwm.duty_ns(1_500_000 - speed * 1_000)
 
 
-class SimpleServo180:
+class SimpleServo:
 
-    def __init__(self, pin, offset=0, angle_range=None):
+    def __init__(self, pin, angle, offset=0, angle_range=None):
         """
         :param pin: pin
         :param offset: 偏移量
         :param angle_range: (-90, 90) 角度范围
         """
         if angle_range is None:
-            angle_range = (-180, 180)
+            angle_range = (-angle, angle)
         self._angle = 0
-        self.__angle = 2_000_000 / 180
+        self.__angle = 2_000_000 / angle
         self.offset = offset
-        self.offset_range = (-90 - offset, 90 - offset)
+        self.offset_range = (angle_range[0] - offset, angle_range[1] - offset)
         self._range = None
         self.range(angle_range)
         self.pwm = PWM(Pin(pin))
         self.pwm.freq(50)
         self.stop()
 
     def range(self, angle_range=None):
@@ -89,10 +89,22 @@
         if angle < self._range[0]:
             angle = self._range[0]
         elif angle > self._range[1]:
             angle = self._range[1]
         self.pwm.duty_ns(int(1_500_000 + (angle + self.offset) * self.__angle))
 
 
+class SimpleServo180(SimpleServo):
+
+    def __init__(self, pin, offset=0, angle_range=None):
+        super().__init__(pin, 180, offset, angle_range)
+
+class SimpleServo270(SimpleServo):
+
+    def __init__(self, pin, offset=0, angle_range=None):
+        super().__init__(pin, 270, offset, angle_range)
+
+
 MG995D360 = SimpleServo360
 MG995D180 = SimpleServo180
 SG90180 = SimpleServo180
+TBS_K20 = SimpleServo270
```

### Comparing `rp2040-tools-0.0.7/rp2040/powerhouse/servoGroup.py` & `rp2040-tools-0.0.8/rp2040/powerhouse/servoGroup.py`

 * *Files identical despite different names*

### Comparing `rp2040-tools-0.0.7/rp2040/sensor/hcsr04.py` & `rp2040-tools-0.0.8/rp2040/sensor/hcsr04.py`

 * *Files identical despite different names*

### Comparing `rp2040-tools-0.0.7/rp2040/sensor/mpu6050.py` & `rp2040-tools-0.0.8/rp2040/sensor/mpu6050.py`

 * *Files identical despite different names*

### Comparing `rp2040-tools-0.0.7/rp2040_tools.egg-info/SOURCES.txt` & `rp2040-tools-0.0.8/rp2040_tools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 LICENSE.txt
 README.md
 setup.py
 rp2040/__init__.py
 rp2040/base.py
 rp2040/pico.py
 rp2040/zero.py
+rp2040/algorithm/PID.py
+rp2040/algorithm/__init__.py
+rp2040/drives/__init__.py
+rp2040/drives/HC/__init__.py
 rp2040/message/__init__.py
 rp2040/message/drive.py
 rp2040/message/protocol.py
 rp2040/oled/__init__.py
 rp2040/oled/ssd1306.py
 rp2040/powerhouse/__init__.py
 rp2040/powerhouse/blendComposition.py
```

### Comparing `rp2040-tools-0.0.7/setup.py` & `rp2040-tools-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rp2040-tools',  # 包名
-    version='v0.0.7',  # 版本
+    version='v0.0.8',  # 版本
     description="Some tools for RP2040",  # 包简介
     long_description=open('README.md', encoding='utf-8').read(),  # 读取文件中介绍包的详细内容
     long_description_content_type='text/markdown',
     include_package_data=True,  # 是否允许上传资源文件
     author='曾钦李',  # 作者
     author_email='1838696034@qq.com',  # 作者邮件
     maintainer='',  # 维护者
```

