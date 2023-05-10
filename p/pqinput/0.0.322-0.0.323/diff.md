# Comparing `tmp/pqinput-0.0.322.tar.gz` & `tmp/pqinput-0.0.323.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqinput-0.0.322.tar", last modified: Tue May  9 09:34:31 2023, max compression
+gzip compressed data, was "pqinput-0.0.323.tar", last modified: Wed May 10 12:09:28 2023, max compression
```

## Comparing `pqinput-0.0.322.tar` & `pqinput-0.0.323.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-09 09:34:31.070855 pqinput-0.0.322/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.322/LICENSE.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3939 2023-05-09 09:34:31.070855 pqinput-0.0.322/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3366 2023-05-09 09:31:18.000000 pqinput-0.0.322/README.md
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-09 09:34:31.070855 pqinput-0.0.322/pqinput/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      119 2023-05-04 15:25:36.000000 pqinput-0.0.322/pqinput/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8419 2023-05-08 12:48:15.000000 pqinput-0.0.322/pqinput/drawPES.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    14524 2023-05-09 09:31:29.000000 pqinput-0.0.322/pqinput/inpxml.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-09 09:34:31.070855 pqinput-0.0.322/pqinput.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     3939 2023-05-09 09:34:31.000000 pqinput-0.0.322/pqinput.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      226 2023-05-09 09:34:31.000000 pqinput-0.0.322/pqinput.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-09 09:34:31.000000 pqinput-0.0.322/pqinput.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-09 09:34:31.000000 pqinput-0.0.322/pqinput.egg-info/top_level.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      542 2023-05-09 09:34:13.000000 pqinput-0.0.322/pyproject.toml
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-09 09:34:31.070855 pqinput-0.0.322/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      653 2023-05-09 09:34:20.000000 pqinput-0.0.322/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 12:09:28.490713 pqinput-0.0.323/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1075 2023-02-09 10:07:34.000000 pqinput-0.0.323/LICENSE.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3887 2023-05-10 12:09:28.490713 pqinput-0.0.323/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3314 2023-05-09 09:41:50.000000 pqinput-0.0.323/README.md
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 12:09:28.490713 pqinput-0.0.323/pqinput/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      106 2023-05-09 11:00:00.000000 pqinput-0.0.323/pqinput/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8239 2023-05-09 11:18:26.000000 pqinput-0.0.323/pqinput/drawPES.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    14625 2023-05-09 14:26:11.000000 pqinput-0.0.323/pqinput/inpxml.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-10 12:09:28.490713 pqinput-0.0.323/pqinput.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     3887 2023-05-10 12:09:28.000000 pqinput-0.0.323/pqinput.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      226 2023-05-10 12:09:28.000000 pqinput-0.0.323/pqinput.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-10 12:09:28.000000 pqinput-0.0.323/pqinput.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-10 12:09:28.000000 pqinput-0.0.323/pqinput.egg-info/top_level.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      542 2023-05-10 12:09:05.000000 pqinput-0.0.323/pyproject.toml
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-10 12:09:28.490713 pqinput-0.0.323/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      653 2023-05-10 12:09:12.000000 pqinput-0.0.323/setup.py
```

### Comparing `pqinput-0.0.322/LICENSE.txt` & `pqinput-0.0.323/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pqinput-0.0.322/PKG-INFO` & `pqinput-0.0.323/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.322
+Version: 0.0.323
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
@@ -22,49 +22,49 @@
 Class with methods to write and edit *xml* structures designed as input files for quantum chemistry calculations on QDng package. 
 Requires *lxml*.
 
 
 ### Example: 
 
 In:
-    dt, steps = 20, 1000
-    propag, hamilt = 'Cheby', 'Sum'
-    Nef, conv = 20, 1e-9
-    name_T, name_V = "GridNablaSq", "GridPotential"
-    mass, pot_file = 2000, 'pot_Vg'
-    directory = 'efs_g'
-    wf_file = 'wfguess'
-    file_name='teste_dt_'
-    key = 'T'
-    nparams = {'dt':1, 'steps':int(1000), 'dir':'efs_g', 'Nef':20, 'conv':1e-11 } 
-   
-    T00 = {'head':'T', 'name':name_T, 'mass':mass, 'key':'T'}
-    V00 = {'head':'V', 'name':name_V, 'file':pot_file}
+
+    Tf = 25 # [fs]
+    dt = 0.25 # [fs]
+    steps = Tf*41.34/dt
+    Nfiles = 5e2
+    wcycle = int(steps/Nfiles)
+    mass = 1764.30
+
+    propa_params = {'dt': dt, 'steps': int(steps), 'wcycle': wcycle, 
+                'dir': 'example_directory/', 'nfile': 'norm'}
+
+    T00 = {'head':'T', 'name':'Sum', 'mass':mass, 'key':'T'}
+    V00 = {'head':'V', 'name':'Sum', 'file':'MgH/pots/pot_Sig_0'}
     m00 = {'head':'m0', 'name':'Sum', 'Opes':[T00, V00]} 
     T11 = {'head':'T', 'ref':'T'}
-    V11 = {'head':'V', 'name':name_V, 'file':pot_file}
+    V11 = {'head':'V', 'name':'Sum', 'file':'MgH/pots/pot_Sig_1'}
     m11 = {'head':'m1', 'name':'Sum', 'Opes':[T11, V11]} 
     m22 = {'head':'m2', 'name':'Sum', 'Opes':[T11, V11]} 
     m10 = {'head':'m10', 'name':'GridDipole', 'file':'mu', 'laser':'Et', 'Opes':[]} 
-  
-    Hparams = {'type':'Multistate', 'Mels':[m00, m11, m10, m22]} 
+
+    H_params = {'type':'Multistate', 'Mels':[m00, m11, m10, m22]} 
     Hsum = {'type':'Sum', 'Opes':[T00, V00, T00]} 
     wf, ef, vib =   [1, ], ['Sig0',], [1, ] # args['wf'], args['ef'], , args['vib'] #
-    WFparams = {'type':'Multistate', 'states':'1',
+    WF_params = {'type':'Multistate', 'states':'1',
              'file':["MgH/efs_{}/ef_{}".format(ef[i], vib[i]) for i in range(len(ef))], 
              'index':[wf[i] for i in range(len(wf))], 'normalize':True}
-    filteropes = [{'expeconly':{'name':'Multistate', 'states':WFparams['states'], 'unity':'False', 'header':"mu{}".format(ind)}, 
+    filter_opes = [{'expeconly':{'name':'Multistate', 'states':WF_params['states'], 'unity':'False', 'header':"mu{}".format(ind)}, 
                    'm{}'.format(ind):{'name':'GridPotential', 'file':'MgH/mu/mu_Sig0Sig1'}}
                    for ind in [2.1,] ]
     #%%
     # Initialize
     prop = InpXML()
-    prop.program('propa', nparams, WFparams)
-    prop.propagation('Cheby', Hparams)
-    prop.filter('filterpost', filteropes)
+    prop.program('propa', propa_params, WF_params)
+    prop.propagation('Cheby', H_params)
+    prop.filter('filterpost', filter_opes)
     prop.show
 
     # Editing
     prop.hamilt = 'name', 'something'
     prop.hamilt = 'm0.0/T', 'name', 'something_new'
     prop.show
```

### Comparing `pqinput-0.0.322/README.md` & `pqinput-0.0.323/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,49 +5,49 @@
 Class with methods to write and edit *xml* structures designed as input files for quantum chemistry calculations on QDng package. 
 Requires *lxml*.
 
 
 ### Example: 
 
 In:
-    dt, steps = 20, 1000
-    propag, hamilt = 'Cheby', 'Sum'
-    Nef, conv = 20, 1e-9
-    name_T, name_V = "GridNablaSq", "GridPotential"
-    mass, pot_file = 2000, 'pot_Vg'
-    directory = 'efs_g'
-    wf_file = 'wfguess'
-    file_name='teste_dt_'
-    key = 'T'
-    nparams = {'dt':1, 'steps':int(1000), 'dir':'efs_g', 'Nef':20, 'conv':1e-11 } 
-   
-    T00 = {'head':'T', 'name':name_T, 'mass':mass, 'key':'T'}
-    V00 = {'head':'V', 'name':name_V, 'file':pot_file}
+
+    Tf = 25 # [fs]
+    dt = 0.25 # [fs]
+    steps = Tf*41.34/dt
+    Nfiles = 5e2
+    wcycle = int(steps/Nfiles)
+    mass = 1764.30
+
+    propa_params = {'dt': dt, 'steps': int(steps), 'wcycle': wcycle, 
+                'dir': 'example_directory/', 'nfile': 'norm'}
+
+    T00 = {'head':'T', 'name':'Sum', 'mass':mass, 'key':'T'}
+    V00 = {'head':'V', 'name':'Sum', 'file':'MgH/pots/pot_Sig_0'}
     m00 = {'head':'m0', 'name':'Sum', 'Opes':[T00, V00]} 
     T11 = {'head':'T', 'ref':'T'}
-    V11 = {'head':'V', 'name':name_V, 'file':pot_file}
+    V11 = {'head':'V', 'name':'Sum', 'file':'MgH/pots/pot_Sig_1'}
     m11 = {'head':'m1', 'name':'Sum', 'Opes':[T11, V11]} 
     m22 = {'head':'m2', 'name':'Sum', 'Opes':[T11, V11]} 
     m10 = {'head':'m10', 'name':'GridDipole', 'file':'mu', 'laser':'Et', 'Opes':[]} 
-  
-    Hparams = {'type':'Multistate', 'Mels':[m00, m11, m10, m22]} 
+
+    H_params = {'type':'Multistate', 'Mels':[m00, m11, m10, m22]} 
     Hsum = {'type':'Sum', 'Opes':[T00, V00, T00]} 
     wf, ef, vib =   [1, ], ['Sig0',], [1, ] # args['wf'], args['ef'], , args['vib'] #
-    WFparams = {'type':'Multistate', 'states':'1',
+    WF_params = {'type':'Multistate', 'states':'1',
              'file':["MgH/efs_{}/ef_{}".format(ef[i], vib[i]) for i in range(len(ef))], 
              'index':[wf[i] for i in range(len(wf))], 'normalize':True}
-    filteropes = [{'expeconly':{'name':'Multistate', 'states':WFparams['states'], 'unity':'False', 'header':"mu{}".format(ind)}, 
+    filter_opes = [{'expeconly':{'name':'Multistate', 'states':WF_params['states'], 'unity':'False', 'header':"mu{}".format(ind)}, 
                    'm{}'.format(ind):{'name':'GridPotential', 'file':'MgH/mu/mu_Sig0Sig1'}}
                    for ind in [2.1,] ]
     #%%
     # Initialize
     prop = InpXML()
-    prop.program('propa', nparams, WFparams)
-    prop.propagation('Cheby', Hparams)
-    prop.filter('filterpost', filteropes)
+    prop.program('propa', propa_params, WF_params)
+    prop.propagation('Cheby', H_params)
+    prop.filter('filterpost', filter_opes)
     prop.show
 
     # Editing
     prop.hamilt = 'name', 'something'
     prop.hamilt = 'm0.0/T', 'name', 'something_new'
     prop.show
```

### Comparing `pqinput-0.0.322/pqinput/drawPES.py` & `pqinput-0.0.323/pqinput/drawPES.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 good way of testing if the input files addresses are working well.
 need qdio package classes
 
 example in the bottom, ''if name==main''
 
 """
 import matplotlib.pyplot as plt, re, os, numpy as np
-# from unitscvt.aunits import HEeV, redPlanck as hP, autime as sec2au, HartreeEnergy as HE
+# from unitscvt.aunits import HEeV
 HEeV =  27.211386245988034 # HartreeEnergy to eV
-sec2au = 2.418884325103622e-17 # seconds to atomic units
-f2En =  2.418884325103622e-17 # transform frequency to energy: hbar/HartreeEnergy(*omega) 
 
 from qdio.qd_file_wf import FileWF 
 from qdio.qd_file_op import FileOP 
-fwf, fop = FileWF(), FileOP() # initiate qdio classes to read potential and wavefunction files 
+fwf, fop = FileWF(), FileOP() 
+# initiate qdio classes to read potential and wavefunction files 
 
 home = '/'+ '/'.join(os.getcwd().split('/')[1:3]) + '/'
 pwdd = home + 'mntcluster/QDng/'
 
-#%%
+#%% color modification
 def lighter(color, amount=0.5):
     #https://gist.github.com/ihincks/6a420b599f43fcd7dbd79d56798c4e5a
     """
     Lightens the given color by multiplying (1-luminosity) by the given amount.
     Input can be matplotlib color string, hex string, or RGB tuple.
     
     Examples:
@@ -43,40 +42,42 @@
     try:
         c = mc.cnames[color]
     except:
         c = color
     c = np.array(colorsys.rgb_to_hls(*mc.to_rgb(c)))
     return colorsys.hls_to_rgb(c[0],1-amount * (1-c[1]),c[2])
 
-def draw_PESs(inxstc, savename=None, SIunits=True, yrange=None, xrange=None, 
+# %%
+# MAIN function
+def plotPES(self, savename=None, SIunits=True, yrange=None, xrange=None, 
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
     
-    iwave = inxstc._wavefunction.getchildren()[0].get('file')
+    iwave = self._wavefunction.getchildren()[0].get('file')
     wf, _ = fwf.read(pwdd + iwave + '.wf')
-    windx = int(re.findall('([\d]+)', inxstc._wavefunction.getchildren()[0].tag)[0])
+    windx = int(re.findall('([\d]+)', self._wavefunction.getchildren()[0].tag)[0])
 
-    children = inxstc._hamiltonian.getchildren()
+    children = self._hamiltonian.getchildren()
 
     for element in children:
         jj = re.findall('([\d]+)', element.tag)
         if jj[0] == jj[1]:
             j = int(jj[0])
-            pot = inxstc._hamiltonian.find(element.tag+'/V')
+            pot = self._hamiltonian.find(element.tag+'/V')
             filepot, offset = pot.get('file'), pot.get('offset')
             offset = (None if offset==0 else offset)
             Pot, _ = fop.read(pwdd + filepot + '.op') 
             potmin = (Pot.min() if Pot.min() < potmin else potmin)
             Pot = Pot - potmin
             
             try: x.size # check if x was defined before
@@ -90,15 +91,15 @@
             ax.plot(x, Pot*(HEeV if SIunits else 1), 
                     color=(cmap(j) if not offset else lighter(cmap(j),.5) ), 
                     linestyle=('-' if not offset else '--') ,
             label=(re.findall('([\d]+)', element.tag)[0] if not offset else '_nolegend_') )
             
             '''If the state PES has a photonic contribution'''
             if offset: 
-                homega = float(offset)*HEeV/sec2au*f2En
+                homega = float(offset)*HEeV
                 
                 '''photon energy in eV'''
                 xytxt = (x[Pot.argmin()], Pot.min()*HEeV)
                 ax.annotate((f'{homega:.3}eV' if not offsetlabel else offsetlabel[off]),
                          xy=(x[Pot.argmin()]+.05, 
                              Pot.min()*HEeV+(0 if not xytxt in previousannot else offset_overlap)),
                          xytext=(2, 2), color=lighter(cmap(j),.8), weight=600,
@@ -147,16 +148,16 @@
     ax.minorticks_on
     ax.grid(which='minor', color='#EEEEEE', linestyle=':', linewidth=0.5)
     if savename: plt.savefig(savename) 
     [plt.close() if not showfig else plt.show()]
         
     return fig, ax
 
-
 # %% if __name__==__main__
+# EXAMPLE
 if __name__=='__main__':
     import inpxml 
     mass = 12500
     propapar = {'dt': 4.138276,'steps': 1000,'wcycle': 100,'dir': 'propa_files','nfile': 'norm'}
     # Kinect energy operators
     T_CO = {'head':'T', 'name':"GridNablaSq", 'mass':mass, 'key':'T'}
     Tref = {'head':'T','ref':'T'}
@@ -188,9 +189,9 @@
     prop = inpxml.InpXML()
     prop.program('propa', propapar, WFpar)
     prop.propagation('Cheby', Hparams)
     #%%
     # prop.addfilter('filterpost', filteropes)
     # prop.show()
     #legend=['G','E','Gl','Gr',],
-    draw_PESs(prop, yrange=(0,20), xrange=(1.5,5), legend=['G','E','Gl','Gr',], offsetlabel=['wx', 'wy'] ,
+    plotPES(prop, yrange=(0,20), xrange=(1.5,5), legend=['G','E','Gl','Gr',], offsetlabel=['wx', 'wy'] ,
               showfig=True)
```

### Comparing `pqinput-0.0.322/pqinput/inpxml.py` & `pqinput-0.0.323/pqinput/inpxml.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     sub = et.SubElement(supelem, params['head'])
     dict2attr(sub, params) 
     return sub
 
 def show(xmlelem): # works for any kind of lxml element, show is just for class
     print(et.tostring(xmlelem, pretty_print=True).decode())
     
-    # Property methods
+    # %% Property methods
 def typed_property(name): # Python Cookbook 3rd: 9.21
     storage_name = '_' + name
     
     @property
     def propriety(self): # lost in translation 
         # Get the property element 
         if not hasattr(self, storage_name): raise AttributeError(f'{name} attribute not defined.')
@@ -101,19 +101,18 @@
         elif len(args)==2: key, new_value = args
         element = (getattr(self, storage_name).find(path) if path else getattr(self, storage_name))
         if element is None: 
             raise AttributeError('setter path do not point to a defined attribute.')
        
         element.set(key, str(new_value))
         # show(element)
-    
-        
         # READ MORE ABOUT XPATH AND IF ITS USEFUL
-        
+    #
     return propriety
+
 # %% 
 '''-------------------------------------------------------------------------'''
 '''                                Class                                    '''
 '''-------------------------------------------------------------------------'''
 class InpXML:
     """ InpXMl class for the creation of a qdng calculation input in xml format.
     requires the lxml.etree package
@@ -147,16 +146,18 @@
     hamilt = typed_property('hamiltonian')
     filterpost = typed_property('filterpost')
     # Defined operations and programs so far
     
     def __init__(self, qdng_params=None): # Initiate the input layout 
         self._qdng = et.Element("qdng") 
         # Root of the XML tree: self._qdng, with the tag-headline 
-
         if qdng_params: dict2attr(self._qdng, qdng_params)
+    
+    # Import method to plot PES curves from the input info
+    from drawPES import plotPES
         
     def __str__(self): # define string format for printing
         return f'{et.tostring(self._qdng, pretty_print=True).decode()}'    
     
     @property
     def show(self): # printing property
         '''Print out the full text in readable xml format
@@ -187,15 +188,16 @@
             if 'normalize' in wfp.keys() and wfp['normalize']: wfel.set('normalize', 'true')
             for ind in range(wfp['states']):
                 wfstate = et.SubElement(wfel, 'wf'+str(ind))
                 wfstate.set('file', wfp['file'][ind])
             
         elif wfp['type'] == 'Multistate':
             wfel = et.Element('wf', name=wfp['type'])
-            wfel.set('states', str(wfp['states'])) # hamiltonian define it later
+            if 'states' in wfp.keys(): wfel.set('states', str(wfp['states']))
+            # hamiltonian define states number later
             if 'normalize' in wfp.keys(): wfel.set('normalize', 'true')
             
             for ii, index in enumerate(wfp['index']):
                 wfstate = et.SubElement(wfel, 'wf'+str(index), file=str(wfp['file'][ii]))
                 if 'coeff2' in wfp.keys(): wfstate.set('coeff2', wfp['coeff2'][ii])
         else:
             raise SyntaxError('Wavefunction type not defined.')
@@ -218,17 +220,15 @@
         """
         '''MAIN PROGRAM'''
         if not ptype in ['propa','eigen']: raise SyntaxError('Program not defined.')  
         self._program = subelem(self._qdng, program_parameters, ptype )
         # Create self._program as a lxml child element of qdng
         '''WAVEFUNCTION'''
         self.define_wavefunction(wf_parameters)
-        # define wavefunction parameters
-        
-    
+        # define wavefunction parameters    
     
     # %% 
     """ Operators """
     def def_hamiltonian(self, Hp):    
         Hel = et.SubElement(self._propagation, 'hamiltonian')
         # Create a lxml element to be appended to the self.propag 
         if Hp['type'] == 'Sum': 
@@ -282,16 +282,14 @@
             raise SyntaxError('Propagator type not defined.')
         # others propagators
         try:
             self._program.append( self._wavefunction ) # append wavefunction after the propagation
         except:
             raise SyntaxError('Wavefunction was not properly defined for propa.')    
 
-
-    
     def def_filterpost(self, filter_list):
         # Define the filterpost operation, must be called after propagation
         filterpost = et.Element('filterpost')
         for dic in filter_list:
             for opes, values in dic.items():
                 for keys in values.keys():
                     values[keys] = str(values[keys])
@@ -310,54 +308,55 @@
             if not isinstance(params, list): params = [params]
             self._filterpost = self.def_filterpost(params)    
 
         
 # %% Name == Main 
 if __name__ == "__main__":
     
-    dt, steps = 20, 1000
-    propag, hamilt = 'Cheby', 'Sum'
-    Nef, conv = 20, 1e-9
-    name_T, name_V = "GridNablaSq", "GridPotential"
-    mass, pot_file = 2000, 'pot_Vg'
-    directory = 'efs_g'
-    wf_file = 'wfguess'
-    file_name='teste_dt_'
-    key = 'T'
-
-    nparams = {'dt':1, 'steps':int(1000), 'dir':'efs_g', 'Nef':20, 'conv':1e-11 } 
-   
-    T00 = {'head':'T', 'name':name_T, 'mass':mass, 'key':'T'}
-    V00 = {'head':'V', 'name':name_V, 'file':pot_file}
+    Tf = 25 # [fs]
+    dt = 0.25 # [fs]
+    steps = Tf*41.34/dt
+    Nfiles = 5e2
+    wcycle = int(steps/Nfiles)
+    mass = 1764.30
+
+    propa_params = {'dt': dt, 'steps': int(steps), 'wcycle': wcycle, 
+                'dir': 'example_directory/', 'nfile': 'norm'}
+
+    T00 = {'head':'T', 'name':'Sum', 'mass':mass, 'key':'T'}
+    V00 = {'head':'V', 'name':'Sum', 'file':'MgH/pots/pot_Sig_0'}
     m00 = {'head':'m0', 'name':'Sum', 'Opes':[T00, V00]} 
     T11 = {'head':'T', 'ref':'T'}
-    V11 = {'head':'V', 'name':name_V, 'file':pot_file}
+    V11 = {'head':'V', 'name':'Sum', 'file':'MgH/pots/pot_Sig_1'}
     m11 = {'head':'m1', 'name':'Sum', 'Opes':[T11, V11]} 
     m22 = {'head':'m2', 'name':'Sum', 'Opes':[T11, V11]} 
     m10 = {'head':'m10', 'name':'GridDipole', 'file':'mu', 'laser':'Et', 'Opes':[]} 
 
-    Hparams = {'type':'Multistate', 'Mels':[m00, m11, m10, m22]} 
+    H_params = {'type':'Multistate', 'Mels':[m00, m11, m10, m22]} 
     Hsum = {'type':'Sum', 'Opes':[T00, V00, T00]} 
     wf, ef, vib =   [1, ], ['Sig0',], [1, ] # args['wf'], args['ef'], , args['vib'] #
-    WFparams = {'type':'Multistate', 'states':'1',
+    WF_params = {'type':'Multistate', 'states':'1',
              'file':["MgH/efs_{}/ef_{}".format(ef[i], vib[i]) for i in range(len(ef))], 
              'index':[wf[i] for i in range(len(wf))], 'normalize':True}
-    filteropes = [{'expeconly':{'name':'Multistate', 'states':WFparams['states'], 'unity':'False', 'header':"mu{}".format(ind)}, 
+    filter_opes = [{'expeconly':{'name':'Multistate', 'states':WF_params['states'], 'unity':'False', 'header':"mu{}".format(ind)}, 
                    'm{}'.format(ind):{'name':'GridPotential', 'file':'MgH/mu/mu_Sig0Sig1'}}
                    for ind in [2.1,] ]
     #%%
     # Initialize
     prop = InpXML()
-    prop.program('propa', nparams, WFparams)
-    prop.propagation('Cheby', Hparams)
-    prop.filter('filterpost', filteropes)
+    prop.program('propa', propa_params, WF_params)
+    prop.propagation('Cheby', H_params)
+    prop.filter('filterpost', filter_opes)
     prop.show
 
     # Editing
     prop.hamilt = 'name', 'something'
     prop.hamilt = 'm0.0/T', 'name', 'something_new'
     prop.show
+    
+
+    prop.plotPES(showfig=True)
      
     # Writing to file
     # prop.writexml(filename='filename', txt=True)
```

### Comparing `pqinput-0.0.322/pqinput.egg-info/PKG-INFO` & `pqinput-0.0.323/pqinput.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pqinput
-Version: 0.0.322
+Version: 0.0.323
 Summary: Create input files for QDng calculations
 Home-page: https://gitlab.fysik.su.se/lucas.borges/inputxml
 Author: Lucas Borges
 Author-email: Lucas Borges <lucas.borges@fysik.su.se>
 License: MIT
 Project-URL: Homepage, https://gitlab.fysik.su.se/lucas.borges/pqinput
 Keywords: qdng
@@ -22,49 +22,49 @@
 Class with methods to write and edit *xml* structures designed as input files for quantum chemistry calculations on QDng package. 
 Requires *lxml*.
 
 
 ### Example: 
 
 In:
-    dt, steps = 20, 1000
-    propag, hamilt = 'Cheby', 'Sum'
-    Nef, conv = 20, 1e-9
-    name_T, name_V = "GridNablaSq", "GridPotential"
-    mass, pot_file = 2000, 'pot_Vg'
-    directory = 'efs_g'
-    wf_file = 'wfguess'
-    file_name='teste_dt_'
-    key = 'T'
-    nparams = {'dt':1, 'steps':int(1000), 'dir':'efs_g', 'Nef':20, 'conv':1e-11 } 
-   
-    T00 = {'head':'T', 'name':name_T, 'mass':mass, 'key':'T'}
-    V00 = {'head':'V', 'name':name_V, 'file':pot_file}
+
+    Tf = 25 # [fs]
+    dt = 0.25 # [fs]
+    steps = Tf*41.34/dt
+    Nfiles = 5e2
+    wcycle = int(steps/Nfiles)
+    mass = 1764.30
+
+    propa_params = {'dt': dt, 'steps': int(steps), 'wcycle': wcycle, 
+                'dir': 'example_directory/', 'nfile': 'norm'}
+
+    T00 = {'head':'T', 'name':'Sum', 'mass':mass, 'key':'T'}
+    V00 = {'head':'V', 'name':'Sum', 'file':'MgH/pots/pot_Sig_0'}
     m00 = {'head':'m0', 'name':'Sum', 'Opes':[T00, V00]} 
     T11 = {'head':'T', 'ref':'T'}
-    V11 = {'head':'V', 'name':name_V, 'file':pot_file}
+    V11 = {'head':'V', 'name':'Sum', 'file':'MgH/pots/pot_Sig_1'}
     m11 = {'head':'m1', 'name':'Sum', 'Opes':[T11, V11]} 
     m22 = {'head':'m2', 'name':'Sum', 'Opes':[T11, V11]} 
     m10 = {'head':'m10', 'name':'GridDipole', 'file':'mu', 'laser':'Et', 'Opes':[]} 
-  
-    Hparams = {'type':'Multistate', 'Mels':[m00, m11, m10, m22]} 
+
+    H_params = {'type':'Multistate', 'Mels':[m00, m11, m10, m22]} 
     Hsum = {'type':'Sum', 'Opes':[T00, V00, T00]} 
     wf, ef, vib =   [1, ], ['Sig0',], [1, ] # args['wf'], args['ef'], , args['vib'] #
-    WFparams = {'type':'Multistate', 'states':'1',
+    WF_params = {'type':'Multistate', 'states':'1',
              'file':["MgH/efs_{}/ef_{}".format(ef[i], vib[i]) for i in range(len(ef))], 
              'index':[wf[i] for i in range(len(wf))], 'normalize':True}
-    filteropes = [{'expeconly':{'name':'Multistate', 'states':WFparams['states'], 'unity':'False', 'header':"mu{}".format(ind)}, 
+    filter_opes = [{'expeconly':{'name':'Multistate', 'states':WF_params['states'], 'unity':'False', 'header':"mu{}".format(ind)}, 
                    'm{}'.format(ind):{'name':'GridPotential', 'file':'MgH/mu/mu_Sig0Sig1'}}
                    for ind in [2.1,] ]
     #%%
     # Initialize
     prop = InpXML()
-    prop.program('propa', nparams, WFparams)
-    prop.propagation('Cheby', Hparams)
-    prop.filter('filterpost', filteropes)
+    prop.program('propa', propa_params, WF_params)
+    prop.propagation('Cheby', H_params)
+    prop.filter('filterpost', filter_opes)
     prop.show
 
     # Editing
     prop.hamilt = 'name', 'something'
     prop.hamilt = 'm0.0/T', 'name', 'something_new'
     prop.show
```

### Comparing `pqinput-0.0.322/pyproject.toml` & `pqinput-0.0.323/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pqinput"
-version = "0.0.322"
+version = "0.0.323"
 authors = [
   { name="Lucas Borges", email="lucas.borges@fysik.su.se" },
 ]
 description = "Create input files for QDng calculations"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pqinput-0.0.322/setup.py` & `pqinput-0.0.323/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setuptools.setup(
     name = "pqinput",
-    version = "0.0.322",
+    version = "0.0.323",
     author = "Lucas Borges",
     author_email = "lucas.borges@fysik.su.se",
     description = ("additional functions for QDng calculations setups."),
     license = "MIT",
     keywords = "qdng",
     url = "https://gitlab.fysik.su.se/lucas.borges/inputxml",
     packages=setuptools.find_packages(),
```

