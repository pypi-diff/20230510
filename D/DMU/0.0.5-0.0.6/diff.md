# Comparing `tmp/DMU-0.0.5.tar.gz` & `tmp/DMU-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DMU-0.0.5.tar", last modified: Wed May  3 13:08:37 2023, max compression
+gzip compressed data, was "DMU-0.0.6.tar", last modified: Wed May 10 12:30:55 2023, max compression
```

## Comparing `DMU-0.0.5.tar` & `DMU-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 13:08:37.620279 DMU-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-03 13:08:37.604689 DMU-0.0.5/DMU/
--rw-rw-rw-   0        0        0        0 2023-05-03 13:07:59.000000 DMU-0.0.5/DMU/__init__.py
--rw-rw-rw-   0        0        0      713 2023-05-03 13:07:59.000000 DMU-0.0.5/DMU/graph_styles.py
--rw-rw-rw-   0        0        0    92377 2023-05-03 13:07:59.000000 DMU-0.0.5/DMU/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-03 13:08:37.620279 DMU-0.0.5/DMU.egg-info/
--rw-rw-rw-   0        0        0    11119 2023-05-03 13:08:37.000000 DMU-0.0.5/DMU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      209 2023-05-03 13:08:37.000000 DMU-0.0.5/DMU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 13:08:37.000000 DMU-0.0.5/DMU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-03 13:08:37.000000 DMU-0.0.5/DMU.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-03 13:08:37.000000 DMU-0.0.5/DMU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1102 2023-05-03 13:07:59.000000 DMU-0.0.5/LICENSE
--rw-rw-rw-   0        0        0    11119 2023-05-03 13:08:37.620279 DMU-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    10503 2023-05-03 13:07:59.000000 DMU-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 13:08:37.620279 DMU-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     3608 2023-05-03 13:07:59.000000 DMU-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:30:55.029269 DMU-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-10 12:30:55.029269 DMU-0.0.6/DMU/
+-rw-rw-rw-   0        0        0        0 2023-05-10 12:30:31.000000 DMU-0.0.6/DMU/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-05-10 12:30:31.000000 DMU-0.0.6/DMU/graph_styles.py
+-rw-rw-rw-   0        0        0   102783 2023-05-10 12:30:31.000000 DMU-0.0.6/DMU/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-10 12:30:55.029269 DMU-0.0.6/DMU.egg-info/
+-rw-rw-rw-   0        0        0    11119 2023-05-10 12:30:54.000000 DMU-0.0.6/DMU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2023-05-10 12:30:54.000000 DMU-0.0.6/DMU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 12:30:54.000000 DMU-0.0.6/DMU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-10 12:30:54.000000 DMU-0.0.6/DMU.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-10 12:30:54.000000 DMU-0.0.6/DMU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1102 2023-05-10 12:30:31.000000 DMU-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    11119 2023-05-10 12:30:55.029269 DMU-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    10503 2023-05-10 12:30:31.000000 DMU-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-10 12:30:55.029269 DMU-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     3608 2023-05-10 12:30:31.000000 DMU-0.0.6/setup.py
```

### Comparing `DMU-0.0.5/DMU/graph_styles.py` & `DMU-0.0.6/DMU/graph_styles.py`

 * *Files identical despite different names*

### Comparing `DMU-0.0.5/DMU/utils.py` & `DMU-0.0.6/DMU/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 import numpy as np
 from scipy import integrate
 from scipy import interpolate
 import json
 from collections import Counter
 import natsort
 import csv
+import xlrd
+import matplotlib.cm as mcm
 
 #%%        
 def AbsPowIntegrator(Data,x,y,z,WL):
     
     """
     "A function that uses a RectBivariateSpline function to determine the total absorbed power from a pabs_adv lumerical file."
     Calculating total power absorption as a power fraction:s
@@ -49,71 +51,151 @@
 
         P_tot.append(np.sum(BivarSpline))
     
     return(P_tot)
 
 #%%
 
-def bias_plotter(data,ax,**kwargs): 
+def bias_plotter(data,FIG,**kwargs): 
+    ax = FIG.ax[0]
     keys = list(data.keys())
     kwargdict = {'fwd':'fwd','f':'fwd','forward':'fwd',
                  'bwd':'rev','rev':'rev','reverse':'rev',
                  'title':'title','tit':'title',
-                 'labels':'labels','lbl':'labels'}
+                 'tool':'tool','experiment':'exp','exp':'exp'}
     
     kuniq = np.unique(list(kwargdict.keys()))
     Pkwargs = {}
     #Filtering out the function kwargs from the plot kwargs
     for key in kwargs.keys():
         if key not in kuniq:
             kwargdict[key] = key
     #Collecting kwargs
-    kw = KwargEval(kwargs, kwargdict,fwd = True, rev = True, title=None, labels=[None,None])
+    kw = KwargEval(kwargs, kwargdict,fwd = True, rev = True, title=None,tool="Nanonis",exp='2IV')
     xkey = []; ykey = []; fwdbwd = []
     
-    for k in keys:
-        if "bias" in k.lower():
-            xkey.append(k)
-            
-        if "bwd" not in k.lower() and "bias" not in k.lower():
-            ykey.append(k)
-            fwdbwd.append(0) #Note: 0  is forward, 1 is backwards
-        
-        if "bwd" in k.lower() and "bias" not in k.lower():
-            ykey.append(k)
-            fwdbwd.append(1) #Note: 0  is forward, 1 is backwards
-    
+    #Separating plot kwargs into a different dict
     for key,val in kwargs.items():
         if key not in kuniq:
             Pkwargs[key] = val
-
-    for n,i in enumerate(fwdbwd):    
-        plotkwargs = {}
-        for k,v in Pkwargs.items():
-            try: 
-                plotkwargs[k] = v[i]
-            except:
-                plotkwargs[k] = v
+            
     
-        if kw.fwd == True and i == 0:
-            if kw.labels[0] is None:
-                kw.labels[0] = "Forward"
+    if kw.tool == "Nanonis":
+        for k in keys:
+            if "bias" in k.lower():
+                xkey.append(k)
+                
+            if "bwd" not in k.lower() and "bias" not in k.lower():
+                ykey.append(k)
+                fwdbwd.append(0) #Note: 0  is forward, 1 is backwards
+            
+            if "bwd" in k.lower() and "bias" not in k.lower():
+                ykey.append(k)
+                fwdbwd.append(1) #Note: 0  is forward, 1 is backwards
+        
+        for n,i in enumerate(fwdbwd):    
+            plotkwargs = {}
+            for k,v in Pkwargs.items():
+                try: 
+                    plotkwargs[k] = v[i]
+                except:
+                    plotkwargs[k] = v
+        
+            if kw.fwd == True and i == 0:
+                ax.plot(data[xkey[0]],data[ykey[i]],label='Forward',**plotkwargs)
                 
-            ax.plot(data[xkey[0]],data[ykey[i]],label=kw.labels[0],**plotkwargs)
-            
+            if kw.rev == True and i == 1:
+                ax.plot(data[xkey[0]],data[ykey[i]],label='Backward',**plotkwargs)
+        ax.set_xlabel(xkey[0])
+        ax.set_ylabel(ykey[fwdbwd[0]])
+        ax.legend()
+        ax.set_title(kw.title)
         
-        if kw.rev == True and i == 1:
-            if kw.labels[1] is None:
-                kw.labels[1] = "Backward"
-            ax.plot(data[xkey[0]],data[ykey[i]],label=kw.labels[1],**plotkwargs)        
-    ax.set_xlabel(xkey[0])
-    ax.set_ylabel(ykey[fwdbwd[0]])
-    
-    ax.legend()
-    ax.set_title(kw.title)
+    elif kw.tool == "Keithley":
+        keys = data['col headers']
+        plotkwargs = {}
+        
+        for i,ll in enumerate(xkey):
+            for k,v in Pkwargs.items():
+                try: 
+                    plotkwargs[k] = v[i]
+                except:
+                    plotkwargs[k] = v
+                    
+        for k in keys:
+            if "voltage" in k.lower() or (k.endswith("V") == True and any(s.lower() in k.lower() for s in ["START","STOP"])==False):
+                xkey.append(k)
+            elif "current" in k.lower() or (k.endswith("I") == True and any(s.lower() in k.lower() for s in ["START","STOP"])==False):
+                ykey.append(k)
+        
+        xkey.sort(); ykey.sort()
+        
+        if "Voltage Linear Sweep" in data["Settings"]["Operation Mode"]:
+            if len(xkey) == 1 and len(ykey) == 1:
+                ax.plot(data[xkey[0]],data[ykey[0]],label=ykey[0],**plotkwargs)
+            
+            elif len(xkey) > 1 and len(ykey)>1:
+                for n,key in enumerate(xkey):
+                    ax.plot(data[xkey[n]],data[ykey[n]],label=ykey[n],**plotkwargs)
+                    
+            elif len(xkey) == 1 and len(ykey)>1:
+                for n,key in enumerate(ykey):
+                    ax.plot(data[xkey[0]],data[ykey[n]],label=ykey[n],**plotkwargs)
+                    
+            elif len(xkey) > 1 and len(ykey)==1:
+                for n,key in enumerate(xkey):
+                    ax.plot(data[xkey[n]],data[ykey[0]],label=ykey[0],**plotkwargs) 
+            ax.set_xlabel(xkey[0])
+            ax.set_ylabel(ykey[0])
+            ax.legend()
+            ax.set_title(kw.title)
+             
+        elif "Voltage List Sweep" in data["Settings"]["Operation Mode"]:
+            FIG.fig,(FIG.ax[0],FIG.ax[1]) = plt.subplots(nrows=2, sharex=True)
+            fig, ax_top, ax_bottom = [FIG.fig,FIG.ax[0],FIG.ax[1]]
+            ax_top.spines["bottom"].set_visible(False)
+            ax_bottom.spines["top"].set_visible(False)
+            ax_top.tick_params(bottom=False)
+            ax_bottom.tick_params(top=False)
+            plt.subplots_adjust(hspace=0.1)
+    
+            ax_top_r = ax_top.twinx()
+            ax_bottom_r = ax_bottom.twinx()
+            
+            axyy  = [ax_top,ax_bottom]
+            axxy  = [ax_top_r,ax_bottom_r]
+            if len(xkey) == 1 and len(ykey)>1:
+                for n,key in enumerate(ykey):
+                    axyy[n].plot(data[ykey[n]],label=ykey[n],**plotkwargs)
+                    axxy[n].plot(data[xkey[0]],label=xkey[0],**plotkwargs)
+                    axyy[n].set_ylabel(ykey[n])
+                    axxy[n].set_ylabel(xkey[0])
+                    
+            if len(xkey) > 1 and len(ykey)>1:
+                for n,key in enumerate(ykey):
+                    axyy[n].plot(data[ykey[n]],label=ykey[n],**plotkwargs)
+                    axxy[n].plot(data[xkey[n]],label=xkey[n],**plotkwargs)
+                    axyy[n].set_ylabel(ykey[n])
+                    axxy[n].set_ylabel(xkey[n])
+                #Fix colours
+            if len(Pkwargs['c'])<4:
+                Pkwargs['c'] = mcm.get_cmap("tab20",20)
+            for axis in axyy:
+                for i,line in enumerate(axis.get_lines()):
+                    line.set_color(Pkwargs['c'](i))
+            for axis in axxy:
+                for i,line in enumerate(axis.get_lines()):
+                    line.set_color(Pkwargs['c'](i+3))
+            ax_bottom.set_xlabel("index")
+            ax_top.set_xlabel("index")
+            handles1,labels = ax_top.get_legend_handles_labels()
+            handles2,labels = ax_top_r.get_legend_handles_labels()
+            fig.legend(handles=handles1+handles2,labels=['$I_{NW}$','$V_{NW}$'])
+ 
+            FIG.ax[0].set_title(kw.title)
 
 #%%
 def Single_NW_Diagram_Plotter(fig,ax,NanonisDat):
     """
     Parameters
     ----------
     ax : TYPE
@@ -853,15 +935,15 @@
     except:
         cprint(['Note that ','kw.act',' = ',str(kw.act),' does not correspond to an action!',' Skipping kwarg eval.'],mt = ['wrn','err','wrn','note'])
         
     #Check if file exists, else write an empty file:
     if os.path.isfile(kw.ddir) == False:
             jsonhandler(f = kw.ddir,d={},pt='abs',a='w')    
     DirDict = jsonhandler(f = kw.ddir,pt='abs', a='r')
-    
+    print(DirDict)
     if kw.act == 'add':
         DirDict = NewDict(DirDict) #Make sure that the add command adds in the correct format
         print(DirDict)
         root = tk.Tk()
         file_path = askdirectory(title = 'Please select a data directory to append to your data directories list!').replace('/',S_ESC)
         
         tk.Tk.withdraw(root)
@@ -1094,50 +1176,51 @@
     Goal of class: use for colourmapping profiles such that:
         - cmap types can be selected
         - The range of values before their full colour contents is selected
         - Alternatively the increment between each cmap value can be selected
         - Invoking the class allows the next value to be given (as to not rely on the for loop i)
         - Allowing for the class to be reset
     """
-    def __init__(self,**kwargs):
+    def __init__(self):
         self.cmap = None
         self.i    = 0
-
+        
         """
         kwargs:
             ==============
             cmap:  the name of the colormap you wish to use
             steps: the number of increments of the colormap between first and last values
             custom: enables custom mode where colour 1 and colour 2 (and the interp between them) can be seleced
             col1: colour 1
             col2: colour 2
             interp: value for interpolation speed (number of points between col1 and col2)
         """
         
     def set_cmap(self,**kwargs):
-        import matplotlib.cm as mcm
         kwargdict = {'cmap':'cmap','colormap':'cmap','colourmap':'cmap',
                      'steps':'steps','step':'steps','N':'steps',
                      'custom':'custom','cust':'custom',
                      'col1':'col1','color1':'col1','colour1':'col1',
                      'col2':'col2','color2':'col2','colour2':'col2',
                      'interp':'interp','interpolation':'interp'}
         kuniq = np.unique(list(kwargdict.keys()))
         kw = KwargEval(kwargs, kwargdict, cmap='viridis',steps=100,custom=False,col1=None,col2=None,interp=None)
 
         self.cmap = mcm.get_cmap(kw.cmap,kw.steps)
         self.col  = self.cmap(self.i)
+
         
     def iter_cmap(self):
         self.i += 1
         self.col  = self.cmap(self.i)
         
     def reset(self):
         self.i = 0
         
+        
 #%%
 class ezplot(object):
     """
     goal of testing:
     Plot.fig = plt.figure(num)
     Plot.add_subplot => fig.add_subplot => Plot.ax[ind] = ax_new
     """
@@ -1364,14 +1447,15 @@
                  'extension':'ext','ext':'ext','ex':'ext','e':'ext',
                  's':'sort','sort':'sort','sorting':'sort'}
     #Collecting kwargs
     kw = KwargEval(kwargs, kwargdict, pt = 'rel',ext = None, sort = None)
     
     cprint('=-=-=-=-=-=-=-=-=-=-=- Running: Get_FileList -=-=-=-=-=-=-=-=-=-=-=',mt = 'funct')
     Dpath = PathSet(path,pt=kw.pt)
+    
     #Checking that kw.sort has been selected correctly
     if kw.sort not in [None,'alphabetical','numeric']:
         cprint('sorting was not set correctly, reverting to using alphabetical sorting (no extra sorting)',mt='note')
         kw.sort = None
     
     #Filtering out the intended file types from the filenames
     #First, checking that the format for ext is correct.
@@ -1401,15 +1485,15 @@
         DList = {}
         summary = ['\nSummary:']
         for ex in kw.ext:
             NList[ex] = [file for file in os.listdir(Dpath) if file.endswith(ex)]
             if kw.sort == 'numeric':
                 NList[ex] = natsort.natsorted(NList[ex], key=lambda y: y.lower())
                 cprint([ex, ' files were sorted numerically'],fg=['g','c'],ts='b')
-            DList[ex] = [Dpath+name for name in NList[ex]]
+            DList[ex] = [Dpath+S_ESC+name for name in NList[ex]]
             
         
             DSum = len(DList[ex])
             summary.append(str(DSum) + ' ' + ex + ' files')
                        
     else:
         NList = [file for file in os.listdir(Dpath)]
@@ -2013,14 +2097,145 @@
             ent[VarI] = float(ent[VarI])
             d_dict[ent[FieldI]] = float(ent[VarI])
         except:
             d_dict[ent[FieldI]] =  ent[VarI]
     return(d_dict)
 
 #%%
+def Keithley_xls_read(directory,**kwargs):
+    if directory == None:
+        directory = os.getcwd()
+        
+    # Get a list of all the Excel files in the current directory
+    files = [f for f in os.listdir(directory) if f.endswith('.xls')]
+    
+    # Create an empty dictionary to store the data
+    data = {}
+    
+    # Loop over each file and each sheet within the file
+    for file in files:
+        filename = os.path.splitext(file)[0]
+        xls = xlrd.open_workbook(file)
+        file_data = {}
+        if 'LOG' in filename.upper():
+            # If filename contains LOG, read data as a flat dictionary
+            sheet = xls.sheet_by_index(0)
+            rows = []
+            for row_index in range(1, sheet.nrows):  # Exclude the first row
+                row_data = sheet.row_values(row_index)
+                rows.append(row_data)
+            # Extract the keys from the first row
+            keys = [str(cell_value) for cell_value in sheet.row_values(0) if cell_value != ""]
+            
+            # Convert data to a dictionary with the values in the first row as the keys
+            flat_data = {}
+            #Determine the SMU position data and create a key for this in flat_data
+            smu_ind = [i for i, item in enumerate(keys) if "SMU" in item]
+            flat_data['positions'] = {}
+            for ind in smu_ind:
+                flat_data['positions']["pos"+str(1+ind - min(smu_ind))] = {}
+                flat_data['positions']["pos"+str(1+ind - min(smu_ind))]['SMU'] = keys[ind]
+            position_indices = [i for i, header in enumerate(keys) if 'POSITION' in header]
+            for row in rows:
+                if all(x == '' for x in row) != True:
+                    if row[0] == "":
+                        for i,var in enumerate(smu_ind):
+                            if row[var] == "":
+                                flat_data['positions']["pos"+str(1+var-min(smu_ind))]['NW'] = row[var-1]
+                            else:
+                                flat_data['positions']["pos"+str(1+var-min(smu_ind))]['NW'] = row[var]
+                        
+                       
+                    elif row[0] !="": 
+                        run_key = str(int(row[0]))
+                        row_dict = {}
+                        for i, header in enumerate(keys):
+                            if i in position_indices:
+                                for j, nw_value in enumerate(row[i:i+2]):
+                                    nw_key = 'position ' + str(j+1)
+                                    row_dict[nw_key] = {'SMU': header, 'NW': nw_value}
+                            elif i > 0:
+                                row_dict[header] = row[i]
+                        flat_data[run_key] = row_dict
+            file_data = flat_data
+
+        else:
+            # Otherwise, read data as nested sheets
+            for sheet_name in xls.sheet_names():
+                sheet = xls.sheet_by_name(sheet_name)
+                
+                if sheet_name == "Settings":
+                    # Read data row by row into a list
+                    rows = []
+                    for row_index in range(sheet.nrows):  # Exclude header row
+                        row_data = sheet.row_values(row_index)
+                        rows.append(row_data)
+                    
+                    settings_data = {}
+                    for row in rows:
+                        if any("===" in s for s in row) or (all(not s.strip() for s in row)): 
+                            
+                            continue
+                
+                        if any("Run" in s for s in row):
+                            key = str(row[0])
+                            settings_data[key] = {}
+                            continue
+                        
+                        header = row[0]
+                        
+                        if len(row) > 1:
+                            values = row[1:]
+                            values = [x for x in values if x != '']
+                            if len(values) == 1:
+                                settings_data[key][header] = str(values[0])
+                            else:
+                                settings_data[key][header] = str(values)
+                                
+                    file_data[sheet_name] = settings_data   
+                    
+                else:
+                    # Read data column by column into a dictionary with the first item in each column as the key
+                    cols = {}
+                    cols["col headers"] = []
+                    for col_index in range(sheet.ncols):
+                        col_data = [x for x in sheet.col_values(col_index) if x != '']
+                        key = col_data.pop(0)
+                        if len(col_data) == 1:
+                            col_data = col_data[0]
+                        cols[key] = col_data 
+                        cols["col headers"].append(key)
+                    # Store the data in the dictionary
+                    file_data[sheet_name] = cols
+        # Store the data for the file in the top-level dictionary
+        data[filename] = file_data
+        
+    #Now we need to check the logbook run info against all included excel sheets so that we can import the correct logbook data.
+    log_keys = [x for x in data.keys() if "LOG" in x.upper()]
+    for log_key in log_keys: 
+        for lkey in data[log_key].keys():
+            for key in [key for key in data.keys() if "LOG" not in key.upper()]:
+               
+                if key == log_key:
+                    continue
+                
+                if any(lkey in s for s in data[key]):
+                    for runID in data[key].keys():
+                        if str(lkey) in str(runID):
+                            data[key][runID]['LOG'] = data[log_key][lkey]
+                            continue
+        del(data[log_key])
+    #Now we need to move the settings file into the 
+    for rkey in data.keys():
+        for runID in data[rkey]["Settings"].keys():
+            if runID in data[rkey].keys():
+                data[rkey][runID]['Settings'] = data[rkey]["Settings"][runID]
+                continue
+        del(data[rkey]["Settings"])
+    return(data)
 
 def Nanonis_dat_read(file,**kwargs):
     """
     Reads the data structure in nanonis data files, and outputs a dictionary containing the data. 
     """
     Raw   = {}
     if 'portformat' not in list(kwargs.keys()):
@@ -2085,22 +2300,25 @@
                 cdstr = "".join(cdata).lower()
                 
                 if "device" in cdstr:
                     itlist = cdstr.split(' ; ')
                     Raw['[Pre-Data]'][itlist[0]] = itlist[1]
                 
                 if "light" in cdstr:
-                    itlist = cdstr.split(' ; ')
-                    if itlist[1].lower() in ['false','fal','off','none',None,'no']:
-                        itlist[1] = False
-                    
-                    elif itlist[1].lower() in ['true','tru','on','light','yes']:
-                        itlist[1] = True
+                    try:
+                        itlist = cdstr.split(' ; ')
+                        if itlist[1].lower() in ['false','fal','off','none',None,'no']:
+                            itlist[1] = False
                         
-                    Raw['[Pre-Data]'][itlist[0]] = itlist[1]
+                        elif itlist[1].lower() in ['true','tru','on','light','yes']:
+                            itlist[1] = True
+                            
+                        Raw['[Pre-Data]'][itlist[0]] = itlist[1]
+                    except:
+                        None
                     
                 else:
                     Raw['[Pre-Data]'][cdata[0]] = {'NW':None,'bias':False,'sweep':False,'current':False,'ground':False,'pos':None}
                 
                 for item in cdata:
                     try:
                         itlist = item.split(' ; ')
```

### Comparing `DMU-0.0.5/DMU.egg-info/PKG-INFO` & `DMU-0.0.6/DMU.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DMU
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package is used to store commonly used functions on pip for the sake of easy pulling for other code.
 Home-page: https://github.com/DeltaMod/DMU
 Author: Atli Vidar Már FLodgren
 Author-email: vidar.flodgren@sljus.lu.se
 Keywords: hello world example examples
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `DMU-0.0.5/LICENSE` & `DMU-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `DMU-0.0.5/PKG-INFO` & `DMU-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DMU
-Version: 0.0.5
+Version: 0.0.6
 Summary: This package is used to store commonly used functions on pip for the sake of easy pulling for other code.
 Home-page: https://github.com/DeltaMod/DMU
 Author: Atli Vidar Már FLodgren
 Author-email: vidar.flodgren@sljus.lu.se
 Keywords: hello world example examples
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `DMU-0.0.5/README.md` & `DMU-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `DMU-0.0.5/setup.py` & `DMU-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 
 setup(
     name="DMU",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(),
     scripts=[TrgtScr],
 
     # Project uses reStructuredText, so ensure that the docutils get
     # installed or upgraded on the target machine
     install_requires=[module_filter(modules)+["docutils>=0.3"]],
```

