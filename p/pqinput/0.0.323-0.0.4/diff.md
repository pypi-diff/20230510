# Comparing `tmp/pqinput-0.0.323.tar.gz` & `tmp/pqinput-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqinput-0.0.323.tar", last modified: Wed May 10 12:09:28 2023, max compression
+gzip compressed data, was "pqinput-0.0.4.tar", last modified: Wed May 10 13:25:45 2023, max compression
```

## Comparing `pqinput-0.0.323.tar` & `pqinput-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 12:09:28.490713 pqinput-0.0.323/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.323/LICENSE.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3887 2023-05-10 12:09:28.490713 pqinput-0.0.323/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3314 2023-05-09 09:41:50.000000 pqinput-0.0.323/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 12:09:28.490713 pqinput-0.0.323/pqinput/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      106 2023-05-09 11:00:00.000000 pqinput-0.0.323/pqinput/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8239 2023-05-09 11:18:26.000000 pqinput-0.0.323/pqinput/drawPES.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    14625 2023-05-09 14:26:11.000000 pqinput-0.0.323/pqinput/inpxml.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 12:09:28.490713 pqinput-0.0.323/pqinput.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3887 2023-05-10 12:09:28.000000 pqinput-0.0.323/pqinput.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      226 2023-05-10 12:09:28.000000 pqinput-0.0.323/pqinput.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-10 12:09:28.000000 pqinput-0.0.323/pqinput.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-10 12:09:28.000000 pqinput-0.0.323/pqinput.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      542 2023-05-10 12:09:05.000000 pqinput-0.0.323/pyproject.toml
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-10 12:09:28.490713 pqinput-0.0.323/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      653 2023-05-10 12:09:12.000000 pqinput-0.0.323/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 13:25:45.898127 pqinput-0.0.4/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.4/LICENSE.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3885 2023-05-10 13:25:45.898127 pqinput-0.0.4/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3314 2023-05-09 09:41:50.000000 pqinput-0.0.4/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 13:25:45.898127 pqinput-0.0.4/pqinput/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      106 2023-05-09 11:00:00.000000 pqinput-0.0.4/pqinput/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8243 2023-05-10 13:13:23.000000 pqinput-0.0.4/pqinput/drawPES.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    14637 2023-05-10 13:19:55.000000 pqinput-0.0.4/pqinput/inpxml.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 13:25:45.898127 pqinput-0.0.4/pqinput.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3885 2023-05-10 13:25:45.000000 pqinput-0.0.4/pqinput.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      226 2023-05-10 13:25:45.000000 pqinput-0.0.4/pqinput.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-10 13:25:45.000000 pqinput-0.0.4/pqinput.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-10 13:25:45.000000 pqinput-0.0.4/pqinput.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      540 2023-05-10 13:25:01.000000 pqinput-0.0.4/pyproject.toml
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-10 13:25:45.898127 pqinput-0.0.4/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      651 2023-05-10 13:24:53.000000 pqinput-0.0.4/setup.py
```

### Comparing `pqinput-0.0.323/LICENSE.txt` & `pqinput-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.323/PKG-INFO` & `pqinput-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.323
+Version: 0.0.4
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.323/README.md` & `pqinput-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.323/pqinput/drawPES.py` & `pqinput-0.0.4/pqinput/drawPES.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,89 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Mon Feb 20 14:40:25 2023
+Created on Wed May  3 14:57:01 2023
 
 @author: lucas
 
 Draw Input file system
+"""
+import os
+import re
 
-good way of testing if the input files addresses are working well.
-need qdio package classes
-
-example in the bottom, ''if name==main''
+import matplotlib.pyplot as plt
+import numpy as np
+from unitscvt.aunits import HartreeEnergy as HE
+from unitscvt.aunits import HEeV
+from unitscvt.aunits import autime as sec2au
+from unitscvt.aunits import redPlanck as hP
+
+# from unitscvt.siconst import electronVolt as eV
+f2En = hP/HE
+from qdio.qd_file_op import FileOP
+from qdio.qd_file_wf import FileWF
 
-"""
-import matplotlib.pyplot as plt, re, os, numpy as np
-# from unitscvt.aunits import HEeV
-HEeV =  27.211386245988034 # HartreeEnergy to eV
-
-from qdio.qd_file_wf import FileWF 
-from qdio.qd_file_op import FileOP 
-fwf, fop = FileWF(), FileOP() 
-# initiate qdio classes to read potential and wavefunction files 
+fwf, fop = FileWF(), FileOP()
 
 home = '/'+ '/'.join(os.getcwd().split('/')[1:3]) + '/'
 pwdd = home + 'mntcluster/QDng/'
 
-#%% color modification
+""" pwd = os.getcwd()
+pwdd = pwd.removesuffix('Propagation_MgH')
+pwdd = pwdd + ('/' if not pwdd.endswith('/') else '') """
+
+#%%
 def lighter(color, amount=0.5):
     #https://gist.github.com/ihincks/6a420b599f43fcd7dbd79d56798c4e5a
     """
     Lightens the given color by multiplying (1-luminosity) by the given amount.
     Input can be matplotlib color string, hex string, or RGB tuple.
     
     Examples:
     >> lighten_color('g', 0.3)
     >> lighten_color('#F034A3', 0.6)
     >> lighten_color((.3,.55,.1), 0.5)
     """
-    import matplotlib.colors as mc
     import colorsys
+
+    import matplotlib.colors as mc
     try:
         c = mc.cnames[color]
     except:
         c = color
     c = np.array(colorsys.rgb_to_hls(*mc.to_rgb(c)))
     return colorsys.hls_to_rgb(c[0],1-amount * (1-c[1]),c[2])
 
-# %%
-# MAIN function
-def plotPES(self, savename=None, SIunits=True, yrange=None, xrange=None, 
+def plotPES(inxstc, savename=None, SIunits=True, yrange=None, xrange=None, 
 legend=None, showfig=None, showWF=True, offset_overlap=0.5, sizex=12/2.54, sizey=8/2.54,
 title=None, offsetlabel=None): # inx structure
     
     
     fig, ax = plt.subplots(layout='constrained', figsize=(sizex, sizey))
     plt.rcParams.update({'font.size': 10})
     
     cmap = plt.get_cmap("tab10")
     potmin = 0
     x = []
     jorder = []
     previousannot = []
     off = 0
     
-    iwave = self._wavefunction.getchildren()[0].get('file')
+    iwave = inxstc._wavefunction.getchildren()[0].get('file')
     wf, _ = fwf.read(pwdd + iwave + '.wf')
-    windx = int(re.findall('([\d]+)', self._wavefunction.getchildren()[0].tag)[0])
+    windx = int(re.findall('([\d]+)', inxstc._wavefunction.getchildren()[0].tag)[0])
+
+    children = inxstc._hamiltonian.getchildren()
 
-    children = self._hamiltonian.getchildren()
 
     for element in children:
         jj = re.findall('([\d]+)', element.tag)
         if jj[0] == jj[1]:
             j = int(jj[0])
-            pot = self._hamiltonian.find(element.tag+'/V')
+            pot = inxstc._hamiltonian.find(element.tag+'/V')
             filepot, offset = pot.get('file'), pot.get('offset')
             offset = (None if offset==0 else offset)
             Pot, _ = fop.read(pwdd + filepot + '.op') 
             potmin = (Pot.min() if Pot.min() < potmin else potmin)
             Pot = Pot - potmin
             
             try: x.size # check if x was defined before
@@ -91,15 +97,15 @@
             ax.plot(x, Pot*(HEeV if SIunits else 1), 
                     color=(cmap(j) if not offset else lighter(cmap(j),.5) ), 
                     linestyle=('-' if not offset else '--') ,
             label=(re.findall('([\d]+)', element.tag)[0] if not offset else '_nolegend_') )
             
             '''If the state PES has a photonic contribution'''
             if offset: 
-                homega = float(offset)*HEeV
+                homega = float(offset)*HEeV/sec2au*f2En
                 
                 '''photon energy in eV'''
                 xytxt = (x[Pot.argmin()], Pot.min()*HEeV)
                 ax.annotate((f'{homega:.3}eV' if not offsetlabel else offsetlabel[off]),
                          xy=(x[Pot.argmin()]+.05, 
                              Pot.min()*HEeV+(0 if not xytxt in previousannot else offset_overlap)),
                          xytext=(2, 2), color=lighter(cmap(j),.8), weight=600,
@@ -145,21 +151,20 @@
     ax.grid(which='major', color='#DDDDDD', linewidth=0.8)
     # Show the minor grid as well. Style it in very light gray as a thin,
     # dotted line.
     ax.minorticks_on
     ax.grid(which='minor', color='#EEEEEE', linestyle=':', linewidth=0.5)
     if savename: plt.savefig(savename) 
     [plt.close() if not showfig else plt.show()]
-        
+    
+    
     return fig, ax
-
-# %% if __name__==__main__
-# EXAMPLE
+# %%
 if __name__=='__main__':
-    import inpxml 
+    import pqinput.inpxml as inx
     mass = 12500
     propapar = {'dt': 4.138276,'steps': 1000,'wcycle': 100,'dir': 'propa_files','nfile': 'norm'}
     # Kinect energy operators
     T_CO = {'head':'T', 'name':"GridNablaSq", 'mass':mass, 'key':'T'}
     Tref = {'head':'T','ref':'T'}
     # Potential energy surfaces
     Vg = {'head':'V', 'name':"GridPotential", 'file':'CO/pots/pot_VSp'}
@@ -182,16 +187,16 @@
     WFpar = {'type':'Multistate', 'states':4,
              'file':["CO/efs_{}/ef_{}".format(ef[1][i], ef[0][i]) for i in range(len(ef[0]))], 
              'index':[iwf[i] for i in range(len(iwf))], 'normalize':True}
     filteropes = [{'expeconly':{'name':'Multistate', 'states':'4', 'unity':'False', 'header':"mu{}".format(ind)}, 
                    'm{}'.format(ind):{'name':'GridPotential', 'file':'CO/mu/mu'}}
                    for ind in [2.1, 2.3, 3.1] ]
     
-    prop = inpxml.InpXML()
+    prop = inx.InpXML()
     prop.program('propa', propapar, WFpar)
     prop.propagation('Cheby', Hparams)
     #%%
-    # prop.addfilter('filterpost', filteropes)
-    # prop.show()
+    
+    prop.show
     #legend=['G','E','Gl','Gr',],
     plotPES(prop, yrange=(0,20), xrange=(1.5,5), legend=['G','E','Gl','Gr',], offsetlabel=['wx', 'wy'] ,
               showfig=True)
```

### Comparing `pqinput-0.0.323/pqinput/inpxml.py` & `pqinput-0.0.4/pqinput/inpxml.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 '''TO IMPLEMENT
 make laser part functional
 '''
 # %% Imports
 from lxml import etree as et
 
+
 # %% General functions
 def etree_to_dict(t):
     if type(t) is et.ElementTree: return etree_to_dict(t.getroot())
     return {
         **t.attrib,
         **{e.tag: etree_to_dict(e) for e in t}
     }
@@ -77,14 +78,15 @@
     dict2attr(sub, params) 
     return sub
 
 def show(xmlelem): # works for any kind of lxml element, show is just for class
     print(et.tostring(xmlelem, pretty_print=True).decode())
     
     # %% Property methods
+    
 def typed_property(name): # Python Cookbook 3rd: 9.21
     storage_name = '_' + name
     
     @property
     def propriety(self): # lost in translation 
         # Get the property element 
         if not hasattr(self, storage_name): raise AttributeError(f'{name} attribute not defined.')
@@ -356,7 +358,9 @@
 
     prop.plotPES(showfig=True)
      
     # Writing to file
     # prop.writexml(filename='filename', txt=True)
         
 
+
+# %%
```

### Comparing `pqinput-0.0.323/pqinput.egg-info/PKG-INFO` & `pqinput-0.0.4/pqinput.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.323
+Version: 0.0.4
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
```

### Comparing `pqinput-0.0.323/pyproject.toml` & `pqinput-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqinput"
-version = "0.0.323"
+version = "0.0.4"
 authors = [
   { name="Lucas Borges", email="lucas.borges@fysik.su.se" },
 ]
 description = "Create input files for QDng calculations"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pqinput-0.0.323/setup.py` & `pqinput-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name = "pqinput",
-    version = "0.0.323",
+    version = "0.0.4",
     author = "Lucas Borges",
     author_email = "lucas.borges@fysik.su.se",
     description = ("additional functions for QDng calculations setups."),
     license = "MIT",
     keywords = "qdng",
     url = "https://gitlab.fysik.su.se/lucas.borges/inputxml",
     packages=setuptools.find_packages(),
```

