# Comparing `tmp/openvisuspy-0.0.22-py3-none-any.whl.zip` & `tmp/openvisuspy-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 26586 bytes, number of entries: 15
--rw-r--r--  2.0 unx      239 b- defN 23-Mar-22 17:13 openvisuspy/__init__.py
--rw-r--r--  2.0 unx     3757 b- defN 23-Apr-05 18:56 openvisuspy/app.py
--rw-r--r--  2.0 unx     6033 b- defN 23-Mar-22 18:55 openvisuspy/backend.py
--rw-r--r--  2.0 unx     7093 b- defN 23-Mar-22 00:10 openvisuspy/backend_cpp.py
--rw-r--r--  2.0 unx    11577 b- defN 23-Mar-22 19:30 openvisuspy/backend_py.py
--rw-r--r--  2.0 unx     4417 b- defN 23-Mar-22 18:06 openvisuspy/canvas.py
--rw-r--r--  2.0 unx     6655 b- defN 23-Apr-05 18:35 openvisuspy/slice.py
--rw-r--r--  2.0 unx     1498 b- defN 23-Apr-05 18:57 openvisuspy/slices.py
--rw-r--r--  2.0 unx     7249 b- defN 23-Mar-22 20:12 openvisuspy/utils.py
--rw-r--r--  2.0 unx    16458 b- defN 23-Apr-05 20:50 openvisuspy/widgets.py
--rwxrwxrwx  2.0 unx     1849 b- defN 23-Apr-05 22:36 openvisuspy-0.0.22.dist-info/LICENSE
--rw-r--r--  2.0 unx     7138 b- defN 23-Apr-05 22:36 openvisuspy-0.0.22.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-05 22:36 openvisuspy-0.0.22.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       12 b- defN 23-Apr-05 22:36 openvisuspy-0.0.22.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1200 b- defN 23-Apr-05 22:36 openvisuspy-0.0.22.dist-info/RECORD
-15 files, 75267 bytes uncompressed, 24620 bytes compressed:  67.3%
+Zip file size: 25028 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      239 b- defN 23-May-08 20:27 openvisuspy/__init__.py
+-rw-r--r--  2.0 unx     3757 b- defN 23-May-08 20:27 openvisuspy/app.py
+-rw-r--r--  2.0 unx     6033 b- defN 23-May-08 20:27 openvisuspy/backend.py
+-rw-r--r--  2.0 unx     7093 b- defN 23-May-08 20:27 openvisuspy/backend_cpp.py
+-rw-r--r--  2.0 unx    11577 b- defN 23-May-08 20:27 openvisuspy/backend_py.py
+-rw-r--r--  2.0 unx     4417 b- defN 23-May-08 20:27 openvisuspy/canvas.py
+-rw-r--r--  2.0 unx     6655 b- defN 23-May-08 20:27 openvisuspy/slice.py
+-rw-r--r--  2.0 unx     1498 b- defN 23-May-08 20:27 openvisuspy/slices.py
+-rw-r--r--  2.0 unx     7249 b- defN 23-May-08 20:27 openvisuspy/utils.py
+-rw-r--r--  2.0 unx    16756 b- defN 23-May-08 20:27 openvisuspy/widgets.py
+-rw-r--r--  2.0 unx     1849 b- defN 23-May-10 00:05 openvisuspy-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2068 b- defN 23-May-10 00:05 openvisuspy-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 00:05 openvisuspy-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-10 00:05 openvisuspy-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1195 b- defN 23-May-10 00:05 openvisuspy-1.0.1.dist-info/RECORD
+15 files, 70490 bytes uncompressed, 23072 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: openvisuspy/utils.py
 Comment: 
 
 Filename: openvisuspy/widgets.py
 Comment: 
 
-Filename: openvisuspy-0.0.22.dist-info/LICENSE
+Filename: openvisuspy-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: openvisuspy-0.0.22.dist-info/METADATA
+Filename: openvisuspy-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: openvisuspy-0.0.22.dist-info/WHEEL
+Filename: openvisuspy-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: openvisuspy-0.0.22.dist-info/top_level.txt
+Filename: openvisuspy-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: openvisuspy-0.0.22.dist-info/RECORD
+Filename: openvisuspy-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openvisuspy/widgets.py

```diff
@@ -86,16 +86,17 @@
 		self.widgets.num_views.on_change("value",lambda attr, old, new: self.setNumberOfViews(int(new))) 
  
 		# timestep
 		self.widgets.timestep = PatchSlider(Slider(title='Time', value=0, start=0, end=1, sizing_mode='stretch_width'))
 		self.widgets.timestep.on_change ("value",lambda attr, old, new: self.setTimestep(int(new)))
 
 		# timestep delta
-		self.widgets.timestep_delta=Select(title="Time delta",options=["1","2","5","10","50","100","200"], value="1",width=100)
-		self.widgets.timestep_delta.on_change("value", lambda attr, old, new: self.setTimestepDelta(int(new)))   
+		speed_options=["1x","2x","4x","8x","16x","32x","64x","128x"]
+		self.widgets.timestep_delta=Select(title="Speed",options=speed_options, value=speed_options[0],width=100)
+		self.widgets.timestep_delta.on_change("value", lambda attr, old, new: self.setTimestepDelta(self.speedFromOption(new)))   
 
 		# field
 		self.widgets.field = Select(title='Field',  options=[],value='data',width=100)
 		self.widgets.field.on_change("value",lambda attr, old, new: self.setField(new))  
   
 		# direction 
 		self.widgets.direction = Select(title='Direction', options=[('0','X'), ('1','Y'), ('2','Z')],value='2',width=100)
@@ -128,15 +129,15 @@
 		self.widgets.status_bar["response"].disabled=True
   
  		# play time
 		self.play=types.SimpleNamespace()
 		self.play.is_playing=False
 		self.widgets.play_button = Button(label="Play",width=80,sizing_mode='stretch_height')
 		self.widgets.play_button.on_click(self.togglePlay)
-		self.widgets.play_sec = Select(title="Play sec",options=["0.0", "0.01","0.1","0.2","0.1","1","2"], value="0.01",width=120)
+		self.widgets.play_sec = Select(title="Frame delay",options=["0.00","0.01","0.1","0.2","0.1","1","2"], value="0.01",width=120)
 
 		self.panel_layout=None
 		self.idle_callback=None
 
 	# start
 	def start(self):
 		for it in self.children:
@@ -326,22 +327,30 @@
 	# setTimesteps
 	def setTimesteps(self,value):
 		logger.info(f"Widgets[{self.id}]::setTimesteps start={value[0]} end={value[-1]}")
 		self.widgets.timestep.start =  value[0]
 		self.widgets.timestep.end   =  value[-1]
 		self.widgets.timestep.step  = 1
 
+	# speedFromOption
+	def speedFromOption (self,option):
+                return (int(option[:-1]))
+
+	# optionFromSpeed
+	def optionFromSpeed (self,speed):
+                return (str(speed)+"x")
+
 	# getTimestepDelta
 	def getTimestepDelta(self):
-		return int(self.widgets.timestep_delta.value)
+		return self.speedFromOption(self.widgets.timestep_delta.value)
 
 	# setTimestepDelta
 	def setTimestepDelta(self,value):
 		logger.info(f"Widgets[{self.id}]::setTimestepDelta value={value}")
-		self.widgets.timestep_delta.value=str(value)
+		self.widgets.timestep_delta.value=self.optionFromSpeed (value)
 		self.widgets.timestep.step=value
 		A=self.widgets.timestep.start
 		B=self.widgets.timestep.end
 		T=self.getTimestep()
 		T=A+value*int((T-A)/value)
 		T=min(B,max(A,T))
 		self.setTimestep(T)
@@ -558,8 +567,8 @@
 			T=self.timesteps.widgets.timestep.start
    
 		logger.info(f"Widgets[{self.id}]::playing timestep={T}")
 		
 		# I will wait for the resolution to be displayed
 		self.play.wait_render_id=[(it+1) if it is not None else None for it in render_id]
 		self.play.t1=time.time()
-		self.setTimestep(T) 
+		self.setTimestep(T)
```

## Comparing `openvisuspy-0.0.22.dist-info/LICENSE` & `openvisuspy-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openvisuspy-0.0.22.dist-info/RECORD` & `openvisuspy-1.0.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 openvisuspy/backend.py,sha256=CJ3ChI0L8P5srnpoK_bI4eyCE07lRYNacUkK77BpPic,6033
 openvisuspy/backend_cpp.py,sha256=ZukezVcj3DikB823ZvinWDb2Tlefke5CjRoSLCDjNTw,7093
 openvisuspy/backend_py.py,sha256=B-ns-tcnhhrE9AedVS6nrVICxZjkkYkqr_oa9mBd2uk,11577
 openvisuspy/canvas.py,sha256=oa42eKl7mQSRnagJ9Kz0uG8duJV0eKaaeG8fFLE6N3A,4417
 openvisuspy/slice.py,sha256=lrerqoE5fekQ0-D0KBWKk_dugRVHKFT-NavfJ3iR3-E,6655
 openvisuspy/slices.py,sha256=ijF00q4UpLMsYC1poXVjr2ZvZM2nl5OZnLh94scjWEM,1498
 openvisuspy/utils.py,sha256=DGfo09rGiKQdB6SHJiEWmOYeMTJnxRJFNUNWPUTxmVQ,7249
-openvisuspy/widgets.py,sha256=Sele_OK0boq-VhllNcqjYvDkli7BtBlc1mXvOebQeLU,16458
-openvisuspy-0.0.22.dist-info/LICENSE,sha256=6e8f7JrZAwWAqUNg-mtEFpikTHZvcDrSGPViHeAlgrw,1849
-openvisuspy-0.0.22.dist-info/METADATA,sha256=H7vOjSIpppLEqFTquhgJ7WOVIh2FKPZQlUee_eN041Y,7138
-openvisuspy-0.0.22.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-openvisuspy-0.0.22.dist-info/top_level.txt,sha256=o9WLF82UoNRuLU1MIOWVUfHBb7u7oGs9w2i6lfhRy_Y,12
-openvisuspy-0.0.22.dist-info/RECORD,,
+openvisuspy/widgets.py,sha256=OADksn13PktE8giInU-IVH9Ti8skz_S6mdLrVMkzWeQ,16756
+openvisuspy-1.0.1.dist-info/LICENSE,sha256=6e8f7JrZAwWAqUNg-mtEFpikTHZvcDrSGPViHeAlgrw,1849
+openvisuspy-1.0.1.dist-info/METADATA,sha256=tICbGsHvEsP4bSxgkGx9D5rBD__EYTtATVsNOEuVTNs,2068
+openvisuspy-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+openvisuspy-1.0.1.dist-info/top_level.txt,sha256=o9WLF82UoNRuLU1MIOWVUfHBb7u7oGs9w2i6lfhRy_Y,12
+openvisuspy-1.0.1.dist-info/RECORD,,
```

