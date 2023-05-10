# Comparing `tmp/llwp-1.3.1.tar.gz` & `tmp/llwp-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llwp-1.3.1.tar", last modified: Thu Mar 30 19:46:24 2023, max compression
+gzip compressed data, was "llwp-1.3.2.tar", last modified: Wed May 10 08:29:59 2023, max compression
```

## Comparing `llwp-1.3.1.tar` & `llwp-1.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-30 19:46:24.266702 llwp-1.3.1/
--rw-rw-rw-   0        0        0      832 2023-03-29 17:51:04.000000 llwp-1.3.1/LICENSE
--rw-rw-rw-   0        0        0       21 2023-03-29 19:59:21.000000 llwp-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0      981 2023-03-30 19:46:24.265702 llwp-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-03-29 18:29:00.000000 llwp-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-30 19:46:24.235702 llwp-1.3.1/llwp/
--rw-rw-rw-   0        0        0   230765 2023-03-30 19:39:20.000000 llwp-1.3.1/llwp/LLWP.py
--rw-rw-rw-   0        0        0     1193 2022-09-29 19:12:05.000000 llwp-1.3.1/llwp/LLWP.svg
--rw-rw-rw-   0        0        0       20 2023-03-29 18:18:08.000000 llwp-1.3.1/llwp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-30 19:46:24.263702 llwp-1.3.1/llwp.egg-info/
--rw-rw-rw-   0        0        0      981 2023-03-30 19:46:24.000000 llwp-1.3.1/llwp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-03-30 19:46:24.000000 llwp-1.3.1/llwp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-30 19:46:24.000000 llwp-1.3.1/llwp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-03-30 19:46:24.000000 llwp-1.3.1/llwp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2023-03-30 19:46:24.000000 llwp-1.3.1/llwp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-30 19:46:24.000000 llwp-1.3.1/llwp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      807 2023-03-30 19:46:04.000000 llwp-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-30 19:46:24.266702 llwp-1.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-10 08:29:59.709115 llwp-1.3.2/
+-rw-rw-rw-   0        0        0      832 2023-04-18 13:31:13.000000 llwp-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0       21 2023-03-29 19:59:21.000000 llwp-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      981 2023-05-10 08:29:59.709115 llwp-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-03-29 18:29:00.000000 llwp-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 08:29:59.677865 llwp-1.3.2/llwp/
+-rw-rw-rw-   0        0        0   230232 2023-05-09 18:07:29.000000 llwp-1.3.2/llwp/LLWP.py
+-rw-rw-rw-   0        0        0     1193 2022-09-29 19:12:05.000000 llwp-1.3.2/llwp/LLWP.svg
+-rw-rw-rw-   0        0        0       20 2023-03-29 18:18:08.000000 llwp-1.3.2/llwp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 08:29:59.709115 llwp-1.3.2/llwp.egg-info/
+-rw-rw-rw-   0        0        0      981 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-10 08:29:59.000000 llwp-1.3.2/llwp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      807 2023-05-10 08:19:00.000000 llwp-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-10 08:29:59.709115 llwp-1.3.2/setup.cfg
```

### Comparing `llwp-1.3.1/LICENSE` & `llwp-1.3.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Copyright 2021 Luis Bonah
 
-As this programs GUI is based on PyQt5, which is GNU GPL v3 licensed, this program is also licensed under GNU GPL v3 (See the bottom paragraph).
+As this programs GUI is based on PyQt6, which is GNU GPL v3 licensed, this program is also licensed under GNU GPL v3 (See the bottom paragraph).
 
 Copyright (C) 2020
 
 	This program is free software: you can redistribute it and/or modify
 	it under the terms of the GNU General Public License as published by
 	the Free Software Foundation, either version 3 of the License, or
 	(at your option) any later version.
```

### Comparing `llwp-1.3.1/PKG-INFO` & `llwp-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llwp
-Version: 1.3.1
+Version: 1.3.2
 Summary: LLWP is a fast, efficient and easy solution for exploring and assigning spectra - relying on Loomis-Wood plots.
 Author-email: Luis Bonah <bonah@ph1.uni-koeln.de>
 Project-URL: Homepage, https://llwp.astro.uni-koeln.de/
 Keywords: LLWP,Loomis-Wood Plots,Spectroscopy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `llwp-1.3.1/llwp/LLWP.py` & `llwp-1.3.2/llwp/LLWP.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 
 # Author: Luis Bonah
 # Description: Loomis-Wood Plot Software for Assigning experimental Spectra to Quantum Numbers
 
 CREDITSSTRING = """Made by Luis Bonah
 
-As this programs GUI is based on PyQt5, which is GNU GPL v3 licensed, this program is also licensed under GNU GPL v3 (See the bottom paragraph).
+As this programs GUI is based on PyQt6, which is GNU GPL v3 licensed, this program is also licensed under GNU GPL v3 (See the bottom paragraph).
 
 pandas, matplotlib, scipy and numpy were used for this program, speeding up the development process massively.
 
 Copyright (C) 2020
 
 	This program is free software: you can redistribute it and/or modify
 	it under the terms of the GNU General Public License as published by
@@ -47,21 +47,21 @@
 import pandas as pd
 import subprocess
 import webbrowser
 import pyckett
 
 from scipy import optimize, special, signal
 
-from PyQt5.QtCore import *
-from PyQt5.QtWidgets import *
-from PyQt5.QtGui import *
+from PyQt6.QtCore import *
+from PyQt6.QtWidgets import *
+from PyQt6.QtGui import *
 
 import matplotlib
 from matplotlib import style, figure
-from matplotlib.backends.backend_qt5agg import FigureCanvas, NavigationToolbar2QT
+from matplotlib.backends.backend_qtagg import FigureCanvas, NavigationToolbar2QT
 
 import warnings
 warnings.simplefilter('ignore', np.RankWarning)
 
 QLocale.setDefault(QLocale("en_EN"))
 
 ##
@@ -125,54 +125,76 @@
 
 
 ##
 ## Main Class, Window and Widget
 ##
 class Main():
 	def __init__(self):
+		self.app = QApplication(sys.argv)
+		self.app.setStyle("Fusion")
+	
 		self.open_windows = {}
 		self.signalclass = SignalClass()
 		self.config = Config(self.signalclass.updateconfig)
 
 		self.setup_dfs()
 		self.loadoptions()
 
 	def gui(self):
 		sys.excepthook = except_hook
 		threading.excepthook = lambda args: except_hook(*args[:3])
 
-		self.app = QApplication(sys.argv)
-		self.app.setStyle("Fusion")
+		self.update_mpl_theme()
+		self.app.styleHints().colorSchemeChanged.connect(self.update_mpl_theme)
+		matplotlib.rcParams['axes.facecolor'] = '#00000000'
+		
+		matplotlib.rc('font', **self.config["plot_font_dict"])
+		self.config.register("plot_font_dict", lambda: matplotlib.rc('font', **self.config["plot_font_dict"]))
 
 		self.notificationsbox = NotificationsBox()
 		self.signalclass.notification.connect(lambda text: self.notificationsbox.add_message(text))
 
 		self.mainwindow = MainWindow()
 		self.plotwidget = PlotWidget()
 		self.plotwidget.gui()
 		self.plotwidget.create_plots()
+		
 		self.mainwindow.setCentralWidget(self.plotwidget)
 		self.mainwindow.loaddockables()
 		self.mainwindow.createmenu()
 		self.mainwindow.readstate()
 		if len(sys.argv) > 1:
-			self.loadproject(sys.argv[1])
+			project = sys.argv[1]
+			if project == "RESTART":
+				self.loadproject(llwpfile(".llwp"))
+			else:
+				self.loadproject(project)
 		self.mainwindow.show()
 
 		if self.messages:
 			main.notification("\n".join(self.messages))
-		self.change_style(self.config["layout_theme"])
 
 		self.autosavetimer = QTimer(self.app)
 		self.autosavetimer.timeout.connect(lambda: main.save_lines_lin(llwpfile(".lin"), force_noappend=True, force_lin=True, quiet=True))
 		if main.config["flag_autosave"]:
 			self.autosavetimer.start(main.config["flag_autosave"]*1000)
 		main.config.register("flag_autosave", lambda: self.autosavetimer.start(main.config["flag_autosave"]*1000) if main.config["flag_autosave"] > 0 else self.autosavetimer.stop())
 
-		sys.exit(self.app.exec_())
+		sys.exit(self.app.exec())
+
+	def update_mpl_theme(self):
+		if is_dark_theme():
+			mpl_style = 'dark_background'
+			mpl_background = 'black'
+		else:
+			mpl_style = 'default'
+			mpl_background = 'white'
+			
+		matplotlib.style.use(mpl_style)
+		matplotlib.rcParams['figure.facecolor'] = mpl_background
 
 	def setup_dfs(self):
 		self.exp_df = pd.DataFrame(columns=exp_dtypes.keys()).astype(exp_dtypes)
 		self.exp_df["filename"] = None
 		self.cat_df = pd.DataFrame(columns=cat_dtypes.keys()).astype(cat_dtypes)
 		self.cat_df["filename"] = None
 		self.lin_df = pd.DataFrame(columns=lin_dtypes.keys()).astype(lin_dtypes)
@@ -196,15 +218,15 @@
 		self.signalclass.writelog.emit(output)
 
 	def update_plot(self, dict_={}):
 		self.signalclass.updateplot.emit(dict_)
 
 	def loadoptions(self, fname=None):
 		if not fname:
-			self.config.update({key: value[0] for key, value in config_specs.items()})
+			self.config.update({key: value for key, (value, class_) in config_specs.items()})
 			fname = llwpfile(".ini")
 
 		config_parser = configparser.ConfigParser(interpolation=None)
 		config_parser.read(fname)
 
 		self.messages = []
 		for section in config_parser.sections():
@@ -223,15 +245,27 @@
 						self.config[fullkey] = value
 					except Exception as E:
 						message = f"The value for the option {fullkey} from the option file was not understood."
 						self.messages.append(message)
 						print(message)
 				else:
 					self.config[fullkey] = value
-
+		
+		# Special case changing colors for better contrast
+		for key, value in self.config.items():
+			if key in config_specs and config_specs[key][1] == Color:
+				if is_dark_theme():
+					if value in ("#000000", ):
+						self.config[key] = "#ffffff"
+						self.messages.append(f"Changed the color of '{key}' from black to white as it is otherwise invisible.")
+				else:
+					if value in ("#ffffff", ):
+						self.config[key] = "#000000"
+						self.messages.append(f"Changed the color of '{key}' from white to black as it is otherwise invisible.")
+				
 	def saveoptions(self):
 		self.mainwindow.savestate()
 		output_dict = {}
 		for key, value in self.config.items():
 			category, name = key.split("_", 1)
 			category = category.capitalize()
 			if category not in output_dict:
@@ -449,15 +483,15 @@
 		for thread in threads:
 			thread.join()
 		self.plotwidget.set_data()
 
 	@synchronized_d(locks["lin_df"])
 	def save_lines_lin(self, path = None, force_noappend=False, force_lin=False, quiet=False):
 		append = self.config["flag_appendonsave"]
-		options = {"options": QFileDialog.DontConfirmOverwrite} if append else {}
+		options = {"options": QFileDialog.Option.DontConfirmOverwrite} if append else {}
 
 		if not path:
 			path, ext = QFileDialog.getSaveFileName(None, 'Save file', '', **options)
 			if not path:
 				return
 
 		catalog = self.new_df
@@ -557,105 +591,14 @@
 			elif type == "lin":
 				return(self.lin_df)
 			elif type == "new":
 				return(self.new_df)
 			elif type == "ser":
 				return(self.ser_df)
 
-	def change_style(self, style=None):
-		styles = ["light", "dark", "custom"]
-		app = self.app
-		if style == None:
-			self.config["layout_theme"] = styles[(styles.index(self.config["layout_theme"])+1)%len(styles)]
-		elif style in styles:
-			self.config["layout_theme"] = style
-		else:
-			self.config["layout_theme"] = styles[0]
-
-		if self.config["layout_owntheme"] == {} and self.config["layout_theme"] == "custom":
-			self.config["layout_theme"] = "light"
-
-		if self.config["layout_theme"] == "light":
-			palette = app.style().standardPalette()
-			mplstyles = ("default", "white")
-
-		elif self.config["layout_theme"] == "dark" or self.config["layout_theme"] == "custom":
-			colors = {
-				"window":				QColor(53, 53, 53),
-				"windowText":			QColor(255, 255, 255),
-				"base":					QColor(35, 35, 35),
-				"alternateBase":		QColor(53, 53, 53),
-				"toolTipBase":			QColor(25, 25, 25),
-				"toolTipText":			QColor(255, 255, 255),
-				"placeholderText":		QColor(100, 100, 100),
-				"text":					QColor(255, 255, 255),
-				"button":				QColor(53, 53, 53),
-				"buttonText":			QColor(255, 255, 255),
-				"brightText":			Qt.red,
-				"light":				QColor(255, 255, 255),
-				"midlight":				QColor(200, 200, 200),
-				"mid":					QColor(150, 150, 150),
-				"dark":					QColor(50, 50, 50),
-				"shadow":				QColor(0, 0, 0),
-				"highlight":			QColor(42, 130, 218),
-				"highlightedText":		 QColor(35, 35, 35),
-				"link":					QColor(42, 130, 218),
-				"linkVisited":			QColor(42, 130, 218),
-
-				"disabledButtonText":	Qt.darkGray,
-				"disabledWindowText":	Qt.darkGray,
-				"disabledText":			Qt.darkGray,
-				"disabledLight":		QColor(53, 53, 53),
-
-				"mplstyles":			("dark_background", "black"),
-			}
-
-			if self.config["layout_theme"] == "custom":
-				colors.update(self.config["layout_owntheme"])
-
-			tmp_dict = {
-				"window":				(QPalette.Window,),
-				"windowText":			(QPalette.WindowText,),
-				"base":					(QPalette.Base,),
-				"alternateBase":		(QPalette.AlternateBase,),
-				"toolTipBase":			(QPalette.ToolTipBase,),
-				"toolTipText":			(QPalette.ToolTipText,),
-				"placeholderText":		(QPalette.PlaceholderText,),
-				"text":					(QPalette.Text,),
-				"button":				(QPalette.Button,),
-				"buttonText":			(QPalette.ButtonText,),
-				"brightText":			(QPalette.BrightText,),
-				"light":				(QPalette.Light,),
-				"midlight":				(QPalette.Midlight,),
-				"dark":					(QPalette.Dark,),
-				"mid":					(QPalette.Mid,),
-				"shadow":				(QPalette.Shadow,),
-				"highlight":			(QPalette.Highlight,),
-				"highlightedText":		(QPalette.HighlightedText,),
-				"link":					(QPalette.Link,),
-				"linkVisited":			(QPalette.LinkVisited,),
-
-				"disabledButtonText":	(QPalette.Disabled, QPalette.ButtonText),
-				"disabledWindowText":	(QPalette.Disabled, QPalette.WindowText),
-				"disabledText":			(QPalette.Disabled, QPalette.Text),
-				"disabledLight":		(QPalette.Disabled, QPalette.Light),
-			}
-
-			mplstyles = colors["mplstyles"]
-			palette = QPalette()
-			for key, values in tmp_dict.items():
-				palette.setColor(*values, colors[key])
-
-
-		app.setPalette(palette)
-		matplotlib.style.use(mplstyles[0])
-		matplotlib.rc('font', **self.config["plot_font_dict"])
-		main.config.register("plot_font_dict", lambda: matplotlib.rc('font', **self.config["plot_font_dict"]))
-		self.plotwidget.fig.patch.set_facecolor(mplstyles[1])
-		self.plotwidget.create_plots()
 
 	@synchronized_d(locks["windows"])
 	def open_window(self, window, *args):
 		if window not in self.open_windows:
 			self.open_windows[window] = window(window.__name__.lower(), *args)
 		self.open_windows[window].show()
 		self.open_windows[window].activateWindow()
@@ -674,15 +617,15 @@
 
 		self.plotwidget.set_data()
 		model.update()
 
 class MainWindow(QMainWindow):
 	def __init__(self, parent=None):
 		super().__init__(parent)
-		self.setFocusPolicy(Qt.StrongFocus)
+		self.setFocusPolicy(Qt.FocusPolicy.StrongFocus)
 		self.setWindowTitle(APP_TAG)
 		self.setAcceptDrops(True)
 		self.shortcuts()
 
 		geometry = main.config.get("windowgeometry_mainwindow")
 		if geometry:
 			self.setGeometry(*json.loads(geometry))
@@ -782,16 +725,14 @@
 				None,
 				QQ(QAction, parent=self, text="&Save Project", change=lambda x: main.saveproject(), shortcut="Ctrl+S", tooltip="Save the references to the currently opened files as a project"),
 				QQ(QAction, parent=self, text="&Load Project", change=lambda x: main.loadproject(), shortcut="Ctrl+O", tooltip="Load a project file"),
 				None,
 				QQ(QAction, parent=self, text="&Quit", change=self.close, tooltip="Close the program"),
 			),
 			"View": (
-				QQ(QAction, parent=self, text="&Change Style", tooltip="Change between light, dark and custom theme", change=lambda x: main.change_style()),
-				None,
 				QQ(QAction, "layout_mpltoolbar", parent=self, text="&MPL Toolbar", shortcut="Shift+1", tooltip="Show or hide toolbar to edit or save the plot canvas", checkable=True),
 				toggleaction_configureplots,
 				toggleaction_referenceseries,
 				toggleaction_catalog,
 				toggleaction_hover,
 				toggleaction_log,
 				None,
@@ -907,15 +848,16 @@
 		files_by_class = {key: [] for key in list(types.keys())}
 
 		for file in files:
 			if not os.path.isfile(file):
 				main.notification(f"<span style='color:#ff0000;'>ERROR</span>: The file {file} could not be found.")
 				continue
 
-			extension = os.path.splitext(file)[1]
+			path, extension = os.path.splitext(file)
+			extension = extension if extension else os.path.basename(path)
 			type = None
 			for key, value in types.items():
 				if extension in value:
 					type = key
 					break
 
 			if type == None:
@@ -987,15 +929,15 @@
 
 		for label, func in buttonsdict.items():
 			button = QQ(QPushButton, text=label, change=func, visible=main.config["flag_showmainplotcontrols"])
 			toplayout.addWidget(button)
 			main.config.register("flag_showmainplotcontrols", lambda button=button: button.setVisible(main.config["flag_showmainplotcontrols"]))
 
 		self.toplabel = QQ(QLabel, text="", wordwrap=False)
-		self.indicator = QQ(QLabel, text="Ready", textFormat=Qt.RichText)
+		self.indicator = QQ(QLabel, text="Ready", textFormat=Qt.TextFormat.RichText)
 		self.working = queue.Queue()
 		main.signalclass.setindicator.connect(self.indicator.setText)
 
 		toplayout.addWidget(self.toplabel, 1)
 		toplayout.addWidget(self.indicator)
 
 		rows_cols_elements = (
@@ -1378,15 +1320,15 @@
 
 	@synchronized_d(locks["axs"])
 	def on_range(self, xmin, xmax, index):
 		axrange = self.axs["ax"][index].get_xlim()
 		if xmax == xmin or xmax > axrange[1] or xmin < axrange[0]:
 			return
 
-		shift = (QApplication.keyboardModifiers() == Qt.ShiftModifier)
+		shift = (QApplication.keyboardModifiers() == Qt.KeyboardModifier.ShiftModifier)
 		if shift or main.config["fit_alwaysfit"]:
 			xmiddle, xuncert = self.fit_peak(xmin, xmax, index)
 			if main.config["fit_clipboard"]:
 				QApplication.clipboard().setText(str(xmiddle))
 			xpre = self.cache_positions[index]
 
 			dict_ = {
@@ -1900,16 +1842,16 @@
 			pass
 
 	def wheelEvent(self, event):
 		steps = event.angleDelta().y() // 120
 		self.set_width(2 ** -steps, absolute=False)
 
 	def change_fitcolor(self):
-		color = QColorDialog.getColor(initial=QColor(rgbt_to_trgb(main.config["color_fit"])), options=QColorDialog.ShowAlphaChannel)
-		color = Color(trgb_to_rgbt(color.name(QColor.HexArgb)))
+		color = QColorDialog.getColor(initial=QColor(rgbt_to_trgb(main.config["color_fit"])), options=QColorDialog.ColorDialogOption.ShowAlphaChannel)
+		color = Color(trgb_to_rgbt(color.name(QColor.NameFormat.HexArgb)))
 		main.config["color_fit"] = color
 
 	def plot_number(self):
 		resp, rc = QInputDialog.getText(self, 'How many plots do you want: ', 'Number:')
 		if not rc:
 			return
 		resp = resp.split("x")
@@ -1954,15 +1896,15 @@
 ## Enhanced DockWidget Class
 ##
 class EQDockWidget(QDockWidget):
 	def __init__(self, parent=None):
 		super().__init__(main.mainwindow)
 		self.setObjectName(self.__class__.__name__)
 
-		main.mainwindow.addDockWidget(2, self)
+		main.mainwindow.addDockWidget(Qt.DockWidgetArea(2), self)
 		QShortcut("Esc", self).activated.connect(self.close)
 
 class ConfigurePlotsWindow(EQDockWidget):
 	def __init__(self, parent=None):
 		super().__init__(parent)
 		self.setWindowTitle("Configure Plots")
 
@@ -1976,15 +1918,15 @@
 		binningfield = QQ(QSpinBox, "plot_bins", range=(1, None), minWidth=120)
 		[hbox1.addWidget(binninglabel), hbox1.addWidget(binningfield), hbox1.addStretch(1)]
 
 		checkbox_coupled  = QQ(QCheckBox, "plot_coupled", text="Plots are coupled")
 		checkbox_annotate = QQ(QCheckBox, "plot_annotate", text="Annotate plots")
 
 
-		[layout.addLayout(hbox1), layout.addItem(QSpacerItem(5, 5, QSizePolicy.Minimum, QSizePolicy.Expanding))]
+		[layout.addLayout(hbox1), layout.addItem(QSpacerItem(5, 5, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding))]
 		[layout.addWidget(widget) for widget in (checkbox_coupled, checkbox_annotate, )]
 
 		checkbox_scale = QQ(QComboBox, "plot_yscale", options=("Per Plot", "Global", "Custom"), change=lambda x: main.signalclass.updateplot.emit())
 		spinbox_scalemin = QQ(QDoubleSpinBox, "plot_yscale_min", range=(None, None), minWidth=120, change=lambda x: main.signalclass.updateplot.emit())
 		spinbox_scalemax = QQ(QDoubleSpinBox, "plot_yscale_max", range=(None, None), minWidth=120, change=lambda x: main.signalclass.updateplot.emit())
 		spinbox_scalecatfac = QQ(QDoubleSpinBox, "plot_expcat_factor", range=(0, None), minWidth=120, change=lambda x: main.signalclass.updateplot.emit())
 		spinbox_scalecatexp = QQ(QSpinBox, "plot_expcat_exponent", range=(None, None), prefix="*10^", minWidth=120, change=lambda x: main.signalclass.updateplot.emit())
@@ -2012,15 +1954,15 @@
 		grid.addWidget(spinbox_scalecatexp, 1, 2, 1, 2)
 		grid.addWidget(scaleMinLabel, 2, 0)
 		grid.addWidget(spinbox_scalemin, 2, 1)
 		grid.addWidget(scaleMaxLabel, 2, 2)
 		grid.addWidget(spinbox_scalemax, 2, 3)
 		grid.setColumnStretch(7, 10)
 		grid.setRowStretch(2, 10)
-		layout.addItem(QSpacerItem(5, 5, QSizePolicy.Minimum, QSizePolicy.Expanding))
+		layout.addItem(QSpacerItem(5, 5, QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Expanding))
 		layout.addLayout(grid)
 
 		layout.addStretch(1)
 
 class ReferenceSeriesWindow(EQDockWidget):
 	def __init__(self, parent=None):
 		super().__init__(parent)
@@ -2034,15 +1976,15 @@
 		self.tabs = QTabWidget()
 		layout.addWidget(self.tabs)
 
 		self.tabs.setTabsClosable(True)
 		self.tabs.setMovable(True)
 		self.tabs.setDocumentMode(True)
 
-		self.tabs.setCornerWidget(QQ(QToolButton, text="Dupl.", tooltip="Duplicate current tab", change=self.duplicate_tab), Qt.TopRightCorner)
+		self.tabs.setCornerWidget(QQ(QToolButton, text="Dupl.", tooltip="Duplicate current tab", change=self.duplicate_tab), Qt.Corner.TopRightCorner)
 		self.tabs.tabCloseRequested.connect(self.close_tab)
 		self.tabs.tabBarDoubleClicked.connect(self.renameoradd_tab)
 		self.tabs.setCurrentIndex(main.config["series_currenttab"])
 		self.tabs.currentChanged.connect(lambda x: main.config.__setitem__("series_currenttab", x))
 		main.signalclass.createdplots.connect(self.min_series)
 
 		self.set_state(main.config["series_references"])
@@ -2216,41 +2158,41 @@
 		self.setWindowTitle("Quote")
 
 		mainwidget = QGroupBox()
 		layout = QVBoxLayout()
 		self.setWidget(mainwidget)
 		mainwidget.setLayout(layout)
 
-		self.quote = QQ(QLabel, wordwrap=True, align=Qt.AlignCenter)
+		self.quote = QQ(QLabel, wordwrap=True, align=Qt.AlignmentFlag.AlignCenter)
 		self.new_quote()
 		layout.addWidget(self.quote)
 		self.setVisible(False)
 
 	def toggle(self):
 		self.new_quote()
 		self.setVisible(not self.isVisible())
 
 	def new_quote(self):
 		quotes = json.loads(quotes_str)
 		quote = quotes[random.randint(0,len(quotes)-1)]
 		self.quote.setText(quote)
-		self.quote.setSizePolicy(QSizePolicy.Minimum, QSizePolicy.Minimum)
+		self.quote.setSizePolicy(QSizePolicy.Policy.Minimum, QSizePolicy.Policy.Minimum)
 
 
 
 
 ##
 ## Enhanced Window Class
 ##
 class EQWidget(QWidget):
 	def __init__(self, id, parent=None):
 		self.id = id
+		geometry = main.config.get(f"windowgeometry_{self.id}")
 		super().__init__(parent)
 
-		geometry = main.config.get(f"windowgeometry_{self.id}")
 		if geometry:
 			if isinstance(geometry, str):
 				geometry = json.loads(geometry)
 			self.setGeometry(*geometry)
 
 		QShortcut("Esc", self).activated.connect(self.close)
 
@@ -2268,15 +2210,15 @@
 class CreditsWindow(EQWidget):
 	def __init__(self, id, parent=None):
 		super().__init__(id, parent)
 		self.setWindowTitle("Credits")
 
 		global CREDITSSTRING
 		layout = QVBoxLayout()
-		layout.addWidget(QQ(QLabel, text=CREDITSSTRING, align=Qt.AlignCenter, wordwrap=True, minHeight=300, minWidth=500))
+		layout.addWidget(QQ(QLabel, text=CREDITSSTRING, align=Qt.AlignmentFlag.AlignCenter, wordwrap=True, minHeight=300, minWidth=500))
 		self.setLayout(layout)
 
 class FileWindow(EQWidget):
 	def __init__(self, id, parent=None):
 		super().__init__(id, parent)
 		self.setWindowTitle("Files Window")
 
@@ -2364,16 +2306,16 @@
 			buttonsbox.addWidget(QQ(QToolButton, text="Reread All", change=lambda x, type=type: main.load_file(type, reread=True, do_QNs=False)))
 			buttonsbox.addWidget(QQ(QToolButton, text="Reset All", change=lambda x, type=type: self.reset_all(type)))
 			buttonsbox.addWidget(QQ(QToolButton, text="Delete All", change=lambda x, type=type: self.delete_file(type)))
 			buttonsbox.addStretch(1)
 
 			filesgrid = QGridLayout()
 
-			scrollarea.setVerticalScrollBarPolicy(Qt.ScrollBarAsNeeded)
-			scrollarea.setHorizontalScrollBarPolicy(Qt.ScrollBarAsNeeded)
+			scrollarea.setVerticalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAsNeeded)
+			scrollarea.setHorizontalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAsNeeded)
 			scrollarea.setWidgetResizable(True)
 			scrollarea.setWidget(widget)
 			widget.setLayout(filesgrid)
 
 			self.widgets[f"{type}_filesgrid"] = filesgrid
 			self.widgets[f"{type}_scrollarea"] = scrollarea
 
@@ -2516,17 +2458,17 @@
 
 	@synchronized_d(locks["axs"])
 	def change_color(self, type, file, inp=False):
 		color_input = self.widgets[type][file]["colorinput"].text()
 		if inp:
 			color = color_input
 		else:
-			color = QColorDialog.getColor(initial=QColor(rgbt_to_trgb(color_input)), options=QColorDialog.ShowAlphaChannel)
+			color = QColorDialog.getColor(initial=QColor(rgbt_to_trgb(color_input)), options=QColorDialog.ColorDialogOption.ShowAlphaChannel)
 			if color.isValid():
-				color = trgb_to_rgbt(color.name(QColor.HexArgb))
+				color = trgb_to_rgbt(color.name(QColor.NameFormat.HexArgb))
 			else:
 				return
 
 		try:
 			color = Color(color)
 		except CustomError:
 			return
@@ -2684,15 +2626,18 @@
 						self.cat_line.set(segments=segs, colors=colors)
 
 					breakpoint(ownid, self.fit_thread_id)
 
 					xs = []
 					ys = []
 					ws = []
+					exp_mean = 0
 					if len(exp_ys) and (polynomrank + len(peaks)):
+						if main.config["blendedlineswindow_autopositionpeaks"]:
+							exp_mean = exp_ys.mean()
 						p0 = []
 						bounds = [[],[]]
 
 						y0 = 4*(np.amax(exp_ys)-np.amin(exp_ys))
 						w0 = xrange[1] - xrange[0]
 						wmax = main.config["blendedlineswindow_maxfwhm"] or w0
 						for peak in peaks:
@@ -2742,22 +2687,25 @@
 						try:
 							popt, pcov = optimize.curve_fit(fitfunction, exp_xs, exp_ys, p0=p0, bounds=bounds)
 						except Exception as E:
 							popt, pcov = optimize.curve_fit(fitfunction, exp_xs, exp_ys, p0=p0, bounds=bounds)
 						perr = np.sqrt(np.diag(pcov))
 						res_xs = np.linspace(xrange[0], xrange[1], main.config["blendedlineswindow_xpoints"])
 						res_ys = fitfunction(res_xs, *popt)
+						res_exp_ys = fitfunction(exp_xs, *popt)
 					else:
 						popt = [0]*(noa*len(peaks)+polynomrank+2*fixedwidth)
 						perr = [0]*(noa*len(peaks)+polynomrank+2*fixedwidth)
 						res_xs = np.linspace(xrange[0], xrange[1], main.config["blendedlineswindow_xpoints"])
 						res_ys = res_xs*0
+						res_exp_ys = exp_xs*0
 
 					breakpoint(ownid, self.fit_thread_id)
 
+
 					self.fit_line.set_data(res_xs, res_ys)
 					self.fit_line.set_color(main.config["blendedlineswindow_color_total"])
 
 					opt_param = []
 					err_param = []
 
 					for i in range(len(peaks)):
@@ -2765,29 +2713,31 @@
 						tmp_errors = list(perr[i*noa: (i+1)*noa])
 
 						if fixedwidth:
 							tmp_params.extend(popt[-(polynomrank+now):len(popt)-polynomrank])
 							tmp_errors.extend(perr[-(polynomrank+now):len(popt)-polynomrank])
 
 						tmp_ys = fitfunction_withoutbaseline(res_xs, *tmp_params)
+						tmp_ys += exp_mean
 						self.plot_parts.append(self.ax.plot(res_xs, tmp_ys, color=main.config["blendedlineswindow_color_total"], alpha=main.config["blendedlineswindow_transparency"])[0])
 
 						opt_param.append( tmp_params )
 						err_param.append( tmp_errors )
 
 
-					self.plot_parts.append(self.ax.scatter([x[0] for x in opt_param], [x[1] for x in opt_param], color=main.config["blendedlineswindow_color_points"]))
+					self.plot_parts.append(self.ax.scatter([x[0] for x in opt_param], [x[1] + exp_mean for x in opt_param], color=main.config["blendedlineswindow_color_points"]))
 
 					if polynomrank > 0 and main.config["blendedlineswindow_showbaseline"]:
 						baseline_args = popt[-polynomrank:]
 						self.plot_parts.append(self.ax.plot(res_xs, np.polyval(baseline_args, res_xs-self.center), color=main.config["blendedlineswindow_color_baseline"])[0])
 					else:
 						baseline_args = []
 
-					self.parent.params = opt_param, err_param, profile, derivative, noa, now, self.center, baseline_args
+					rms_ys = np.sqrt(np.sum((exp_ys - res_exp_ys)**2) / len(exp_ys)) if len(exp_ys) else 0
+					self.parent.params = opt_param, err_param, profile, derivative, noa, now, self.center, baseline_args, rms_ys
 
 					breakpoint(ownid, self.fit_thread_id)
 
 					main.signalclass.blwfit.emit()
 					main.signalclass.fitindicator.emit("Ready")
 					super().update_plot()
 				except CustomError as E:
@@ -2831,15 +2781,15 @@
 		tmplayout.addWidget(QQ(QSpinBox, "blendedlineswindow_polynom", range=(-1, None), minWidth=120), row_id, 1)
 
 		tmplayout.addWidget(QQ(QCheckBox, "blendedlineswindow_showbaseline", text="Show Baseline"), row_id, 2, 1, 2)
 		tmplayout.setColumnStretch(4, 1)
 
 		layout.addLayout(tmplayout)
 
-		self.label = QQ(QLabel, text="Ready", textFormat=Qt.RichText)
+		self.label = QQ(QLabel, text="Ready", textFormat=Qt.TextFormat.RichText)
 		main.signalclass.fitindicator.connect(self.label.setText)
 		tmp_layout = QHBoxLayout()
 		layout.addLayout(tmp_layout)
 		row = (
 		  QQ(QPushButton, text="Del All", change=lambda x: self.del_peak(-1)),
 		  QQ(QPushButton, text="Update", change=lambda x: self.plotWidget.update_plot()),
 		  QQ(QPushButton, text="Save", change=lambda x: self.save_values()),
@@ -2847,15 +2797,15 @@
 		)
 
 		for widget in row:
 			tmp_layout.addWidget(widget)
 		tmp_layout.addStretch()
 
 		self.table = QTableWidget()
-		self.table.setEditTriggers(QAbstractItemView.NoEditTriggers)
+		self.table.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
 		self.table.setMinimumHeight(50)
 		layout.addWidget(self.table)
 
 		self.cid = self.plotWidget.plot_canvas.mpl_connect("button_press_event", lambda event: self.add_peak(event.xdata, event.ydata))
 		main.signalclass.blwfit.connect(self.fill_table)
 
 	def add_peak(self, x, y):
@@ -2904,21 +2854,23 @@
 			if fixedwidth:
 				tmp_params.extend(widths)
 			res_ys.append(lineshape(fun, der, x, *tmp_params))
 
 		return(np.sum(res_ys, axis=0))
 
 	def fill_table(self):
-		opt_param, err_param, function, derivative, noa, now, self.center, baseline_args = self.params
+		opt_param, err_param, function, derivative, noa, now, self.center, baseline_args, rms_ys = self.params
 		fit_values = {
 			"function": function,
 			"derivative": derivative,
 			"center": self.center,
 			"baseline": list(baseline_args),
 			"peaks": [],
+			"RMS": rms_ys,
+			"datetime": time.strftime("%d.%m.%Y %H:%M:%S", time.localtime()),
 		}
 		
 		opt_param.sort(key=lambda x: x[0])
 		table = self.table
 		table.setRowCount(0)
 		table.setColumnCount(7)
 		table.setHorizontalHeaderLabels(["Action", "Frequency", "Amplitude", "FWHM Gauss", "FWHM Lorentz", "Other QNs", "Delete"])
@@ -2938,17 +2890,26 @@
 			fit_values["peaks"].append({"values": (x, y, wg, wl), "errors": (x_error, y_error, wg_error, wl_error)})
 		self.fit_values = fit_values
 		table.resizeColumnsToContents()
 
 	def save_values(self):
 		if self.fit_values:
 			filename = llwpfile(".fit")
+			
 			with open(filename, "a+") as file:
-				file.write(json.dumps(self.fit_values))
-				file.write("\n")
+				file.seek(0)
+				previous_fits = file.read()
+				if previous_fits.strip():
+					all_fits = json.loads(previous_fits)
+					all_fits.append(self.fit_values)
+				else:
+					all_fits = [self.fit_values]
+			
+				file.truncate(0)
+				json.dump(all_fits, file, indent=2)
 			main.notification(f"Saved the fit to the file {filename}.")
 		else:
 			main.notification(f"No fit values to be saved.")
 
 	def pre_assign(self, x, error, oqns=False):
 		index = self.plotWidget.i
 
@@ -2961,15 +2922,15 @@
 		for i in range(6):
 			dict_[f"qnu{i+1}"] = pyckett.SENTINEL
 			dict_[f"qnl{i+1}"] = pyckett.SENTINEL
 
 		if oqns:
 			visible_cat_data = main.get_visible_data("cat")
 			dialog = QNsDialog(x, visible_cat_data)
-			dialog.exec_()
+			dialog.exec()
 
 			if dialog.result() == 1:
 				dict_.update(dialog.save())
 			else:
 				return
 		else:
 			reference = main.plotwidget.get_series_reference(index[1])
@@ -3003,15 +2964,15 @@
 		self.setWindowTitle("Series Finder")
 
 		layout = QVBoxLayout()
 
 		self.messageLabel = QQ(QLabel, wordwrap=True, hidden=True)
 
 		self.outputTable = QTableWidget()
-		self.outputTable.setEditTriggers(QAbstractItemView.NoEditTriggers)
+		self.outputTable.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
 
 		vertLayout = QHBoxLayout()
 		leftLayout = QGridLayout()
 		rightLayout = QVBoxLayout()
 		layout.addWidget(QQ(QLabel, wordwrap=True, text="Series Finder allows to find the strongest (unassigned) predicted transitions."))
 
 		rightLayout.addWidget(QQ(QLabel, text="Allowed Transitions"))
@@ -3192,15 +3153,15 @@
 
 		self.label = QQ(QLabel)
 		layout.addWidget(self.label)
 
 		self.noq = main.config["series_qns"]
 		self.table = QTableWidget()
 		self.cols = ["x", "y", "dist"] + [f"qn{ul}{i+1}" for ul in ("u", "l") for i in range(6)] + ["filename"]
-		self.table.setEditTriggers(QAbstractItemView.NoEditTriggers)
+		self.table.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
 		self.table.setRowCount(0)
 		self.table.setColumnCount(len(self.cols)+1)
 		self.table.setHorizontalHeaderLabels(["Y/N", "x", "log. y", "Dist"] +  [f"{ul}{i+1}" for ul in ("U", "L") for i in range(6)] + ["Filename"])
 		layout.addWidget(self.table)
 
 		buttons_layout = QHBoxLayout()
 
@@ -3416,15 +3377,15 @@
 				input_type.setCurrentIndex(len(items)-1)
 			self.change_type(key)
 
 		self.infolabel = QQ(QLabel, wordwrap=True, text="Press 'Run Peakfinder' to find peaks.")
 		layout.addWidget(self.infolabel)
 
 		self.table = QTableWidget()
-		self.table.setEditTriggers(QAbstractItemView.NoEditTriggers)
+		self.table.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
 		self.table.setHidden(True)
 		self.table.doubleClicked.connect(self.go_to)
 
 		layout.addWidget(self.table)
 
 		main.signalclass.peakfinderstart.connect(lambda: self.run_button.setEnabled(False))
 		main.signalclass.peakfinderstart.connect(lambda: self.infolabel.setText("Finding peaks ..."))
@@ -3967,16 +3928,16 @@
 			self.fig.canvas.draw()
 
 class SpectraResolverWindow(EQWidget):
 	def __init__(self, id, parent=None):
 		super().__init__(id, parent)
 		self.setWindowTitle("Spectra Resolver")
 		self.list_ = QListWidget()
-		self.list_.setDragDropMode(QAbstractItemView.InternalMove)
-		self.list_.setSelectionMode(QAbstractItemView.ExtendedSelection)
+		self.list_.setDragDropMode(QAbstractItemView.DragDropMode.InternalMove)
+		self.list_.setSelectionMode(QAbstractItemView.SelectionMode.ExtendedSelection)
 
 		self.label = QQ(QLabel, text="Ready", wordwrap=True)
 
 		self.apply_order_button = QQ(QPushButton, text="Save overlap free")
 		self.apply_order_button.clicked.connect(self.solveoverlap)
 
 		self.layout = QVBoxLayout()
@@ -4237,27 +4198,21 @@
 		self.view.setStyleSheet("background:transparent;")
 
 		layout.addWidget(self.view, 2)
 
 		self.layout = layout
 
 		QShortcut(
-			QKeySequence(QKeySequence.ZoomIn),
-			self.view,
-			activated=self.zoom_in,
-		)
-
-		QShortcut(
-			QKeySequence(QKeySequence.ZoomIn),
+			QKeySequence(Qt.Key.Key_ZoomIn),
 			self.view,
 			activated=self.zoom_in,
 		)
 
 		QShortcut(
-			QKeySequence(QKeySequence.ZoomOut),
+			QKeySequence(Qt.Key.Key_ZoomOut),
 			self.view,
 			activated=self.zoom_out,
 		)
 
 	def wheelEvent(self,event):
 		steps = event.angleDelta().y() // 120
 		tmp_funct = self.zoom_in if steps > 0 else self.zoom_out
@@ -4472,22 +4427,22 @@
 		vbox = QVBoxLayout()
 		scrollarea = QScrollArea()
 		widget = QWidget()
 		layout = QGridLayout()
 
 		self.updating = True
 
-		scrollarea.setVerticalScrollBarPolicy(Qt.ScrollBarAsNeeded)
-		scrollarea.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
+		scrollarea.setVerticalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAsNeeded)
+		scrollarea.setHorizontalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOff)
 		scrollarea.setWidgetResizable(True)
 
 		tmp_layout = QHBoxLayout()
 		tmp_layout.addWidget(QQ(QPushButton, text="Save as default", change=lambda: main.saveoptions()))
 		completer = QCompleter(main.config.keys())
-		completer.setCaseSensitivity(Qt.CaseInsensitive)
+		completer.setCaseSensitivity(Qt.CaseSensitivity.CaseInsensitive)
 		tmp_layout.addWidget(QQ(QLineEdit, placeholder="Search", completer=completer, change=lambda x: self.search(x)))
 		tmp_layout.addStretch(1)
 
 		vbox.addLayout(tmp_layout)
 		self.widgets = {}
 
 		i = 1
@@ -4743,27 +4698,28 @@
 ## Dialogs
 ##
 class QNsDialog(QDialog):
 	def __init__(self, frequency, df):
 		super().__init__()
 		QShortcut("Esc", self).activated.connect(lambda: self.predone(0))
 
+		noq = main.config["series_qns"]
 		qns = [f"qnu{i+1}" for i in range(6)]+[f"qnl{i+1}" for i in range(6)]
+		qns_visible = [f"qn{ul}{n+1}" for ul in ("u", "l") for n in range(noq)]
 		self.res = {key: pyckett.SENTINEL for key in qns}
 
 		self.setWindowTitle(f"Choose QNs for transition at {frequency}")
 		self.resize(main.config["qnsdialog_width"], main.config["qnsdialog_height"])
 		self.frequency = frequency
 
 		layout = QVBoxLayout()
 		self.setLayout(layout)
 		layout.addWidget(QQ(QLabel, wordwrap=True, text="Enter the quantum numbers in the input fields or choose one of the transitions from the table."))
 		layout.addSpacing(10)
 
-		noq = main.config["series_qns"]
 		self.sbs = {}
 		qnslayout = QGridLayout()
 		for i in range(noq):
 			widget = QQ(QSpinBox, value=0, range=(0, None))
 			qnslayout.addWidget(widget, 1, i)
 			self.sbs[f"qnu{i+1}"] = widget
 
@@ -4775,46 +4731,48 @@
 		for i in range(noq):
 			lab = QLabel(f"QN {i+1}")
 			qnslayout.addWidget(QQ(QLabel, text=f"QN{i+1}"), 0, i)
 
 		qnslayout.setColumnStretch(7, 1)
 		layout.addLayout(qnslayout)
 
-		cols = ["dist", "x", "log y"] + qns
+		tmp = ["dist", "x", "log y"]
+		cols = tmp + qns
 		table = QTableWidget()
 		table.setColumnCount(len(cols)+1)
 		table.setHorizontalHeaderLabels(["Assign"] + cols)
 		table.setRowCount(0)
-		table.setEditTriggers(QAbstractItemView.NoEditTriggers)
+		table.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
 
 		tmp_df = df.copy()
 		tmp_df["dist"] = tmp_df["x"] - frequency
 		tmp_df["log y"] = np.log10(tmp_df["y"])
 		tmp_df["absdist"] = abs(tmp_df["dist"])
 		tmp_df.sort_values(by=["absdist"], inplace=True)
 		tmp_df.reset_index(drop=True, inplace=True)
 
 		for i, row in tmp_df.head(100).iterrows():
 			currRowCount = table.rowCount()
 			table.insertRow(currRowCount)
 			for j, col in enumerate(cols):
 				val = f'{row[col]:{main.config["flag_xformatfloat"]}}'.rstrip("0").rstrip(".")
 				table.setItem(currRowCount, j+1, QTableWidgetItem(val))
-			tmpd = {key: row[key] for key in qns}
+			tmpd = {key: row[key] for key in qns_visible}
 			tmpd["xpre"] = row["x"]
 			table.setCellWidget(currRowCount, 0, QQ(QPushButton, text="Assign", change=lambda x, tmpd=tmpd: self.table_save(tmpd)))
 
+		
 		for i in range(6):
-			table.setColumnHidden(i+3, i>=noq)
-			table.setColumnHidden(i+9, i>=noq)
+			table.setColumnHidden(i+ len(tmp) + 2, i>=noq)
+			table.setColumnHidden(i+ len(tmp) + 8, i>=noq)
 
 		table.resizeColumnsToContents()
 		layout.addWidget(table)
 
-		buttons = QDialogButtonBox.Ok | QDialogButtonBox.Cancel
+		buttons = QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
 		buttonBox = QDialogButtonBox(buttons)
 		buttonBox.accepted.connect(lambda: self.selector_save(1))
 		buttonBox.rejected.connect(lambda: self.predone(0))
 		layout.addWidget(buttonBox)
 
 	def table_save(self, tmpd):
 		self.res.update(tmpd)
@@ -4868,15 +4826,15 @@
 		buttons_layout.addWidget(QQ(QPushButton, text="Cancel", change=lambda x: self.predone(0), shortcut="Esc"))
 		buttons_layout.addStretch()
 		layout.addLayout(buttons_layout)
 
 	def add_tab(self, title="Command", command=""):
 		textarea = QQ(QPlainTextEdit, value=command)
 		cursor = textarea.textCursor()
-		cursor.movePosition(QTextCursor.End)
+		cursor.movePosition(QTextCursor.MoveOperation.End)
 		textarea.setTextCursor(cursor)
 		self.tabs.addTab(textarea, title)
 
 	def close_tab(self, index):
 		tab = self.tabs.widget(index)
 		tab.deleteLater()
 		self.tabs.removeTab(index)
@@ -5005,15 +4963,15 @@
 		layout.addStretch(1)
 		plotwidgets["Transition"].setLayout(layout)
 
 		# Tab 2: List
 		layout = QVBoxLayout()
 
 		self.xsTable = QQ(QTableWidget, rowCount=0, columnCount=2, move=(0, 0))
-		self.xsTable.setEditTriggers(QAbstractItemView.NoEditTriggers)
+		self.xsTable.setEditTriggers(QAbstractItemView.EditTrigger.NoEditTriggers)
 		self.xsTable.setHorizontalHeaderLabels(["#", "Frequency"])
 		layout.addWidget(self.xsTable)
 		if self.state["list"]["xs"]:
 			self.load_xs_list(values=self.state["list"]["xs"])
 
 		button_open = QQ(QToolButton, text="Open List", change=lambda x: self.load_xs_list(temp=False))
 		button_write = QQ(QToolButton, text="Write List", change=lambda x: self.load_xs_list(temp=True))
@@ -5256,14 +5214,20 @@
 
 
 
 
 ##
 ## Miscellaneous Classes
 ##
+class FigureCanvas(FigureCanvas):
+	def __init__(self, *args, **kwargs):
+		super().__init__(*args, **kwargs)
+		self.wheelEvent = lambda event: event.ignore()
+		self.setStyleSheet('background-color: #00000000')
+
 class ProtPlot(QWidget):
 	def __init__(self, parent=None, i=None, onrange=False):
 		super().__init__(parent)
 
 		self.parent = parent
 		self.shortcuts()
 
@@ -5413,15 +5377,15 @@
 			QShortcut(keys, self.parent).activated.connect(function)
 
 	@synchronized_d(locks["axs"])
 	def on_range(self, xmin, xmax, index):
 		axrange = self.axs["ax"][index].get_xlim()
 		if xmax == xmin or xmax > axrange[1] or xmin < axrange[0]:
 			return
-		shift = (QApplication.keyboardModifiers() == Qt.ShiftModifier)
+		shift = (QApplication.keyboardModifiers() == Qt.KeyboardModifier.ShiftModifier)
 		if self.onrange == "Assign" and (shift or main.config["fit_alwaysfit"]):
 			xmiddle, xuncert = main.plotwidget.fit_peak(xmin, xmax, index)
 			xpre = main.plotwidget.self.cache_positions[index]
 
 			dict_ = {
 				"x":		xmiddle,
 				"error":	xuncert,
@@ -5448,34 +5412,34 @@
 
 class NotificationsBox(QWidget):
 	def __init__(self):
 		super().__init__()
 		self.bg_color = QColor("#a5aab3")
 		self.messages = []
 		self.setWindowFlags(
-			Qt.Window | Qt.Tool | Qt.FramelessWindowHint |
-			Qt.WindowStaysOnTopHint | Qt.X11BypassWindowManagerHint)
+			Qt.WindowType.Window | Qt.WindowType.Tool | Qt.WindowType.FramelessWindowHint |
+			Qt.WindowType.WindowStaysOnTopHint | Qt.WindowType.X11BypassWindowManagerHint)
 
-		self.setAttribute(Qt.WA_NoSystemBackground, True)
-		self.setAttribute(Qt.WA_TranslucentBackground, True)
+		self.setAttribute(Qt.WidgetAttribute.WA_NoSystemBackground, True)
+		self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground, True)
 
 		self.setMinimumHeight(80)
 		self.setMinimumWidth(300)
 		self.setMaximumWidth(300)
 
 		self.layout = QVBoxLayout()
 		self.setLayout(self.layout)
 
 		self.setStyleSheet("""
 			color: white;
 			background-color: #bf29292a;
 		""")
 
-		self._desktop = QApplication.instance().desktop()
-		startPos = QPoint(self._desktop.screenGeometry().width() - self.width() - 10, 10)
+		self._desktop = QApplication.instance().primaryScreen()
+		startPos = QPoint(self._desktop.geometry().width() - self.width() - 10, 10)
 		self.move(startPos)
 
 	def paintEvent(self, event=None):
 		painter = QPainter(self)
 
 		painter.setOpacity(0.5)
 		painter.setPen(QPen(self.bg_color))
@@ -5569,14 +5533,17 @@
 		df = self.callbacks
 		df.loc[len(df), ["id", "key", "function", "widget"]] = id, key, function, widget
 		widget.destroyed.connect(lambda x, id=id: self.unregister_widget(id))
 
 	def unregister_widget(self, id):
 		self.callbacks.drop(self.callbacks[self.callbacks["id"] == id].index, inplace=True)
 
+def is_dark_theme():
+	return(QApplication.styleHints().colorScheme() == Qt.ColorScheme.Dark)
+
 class Color(str):
 	def __new__(cls, color):
 		cls.validate_color(cls, color)
 		return super().__new__(cls, color)
 
 	def __assign__(self, color):
 		self.validate_color(color)
@@ -5614,20 +5581,20 @@
 		super().__init__()
 
 class QSpinBox(QSpinBox):
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		# AdaptiveDecimalStepType is not implemented in earlier versions of PyQt5
 		try:
-			self.setStepType(QAbstractSpinBox.AdaptiveDecimalStepType)
+			self.setStepType(QAbstractSpinBox.StepType.AdaptiveDecimalStepType)
 		except:
 			pass
 
 	def setSingleStep(self, value):
-		self.setStepType(QAbstractSpinBox.DefaultStepType)
+		self.setStepType(QAbstractSpinBox.StepType.DefaultStepType)
 		super().setSingleStep(value)
 
 	def setValue(self, value):
 		if value < -2147483647 or value > 2147483647:
 			value = 0
 		return super().setValue(value)
 
@@ -5638,20 +5605,20 @@
 
 class QDoubleSpinBox(QDoubleSpinBox):
 	def __init__(self, *args, **kwargs):
 		super().__init__(*args, **kwargs)
 		self.setDecimals(20)
 		# AdaptiveDecimalStepType is not implemented in earlier versions of PyQt5
 		try:
-			self.setStepType(QAbstractSpinBox.AdaptiveDecimalStepType)
+			self.setStepType(QAbstractSpinBox.StepType.AdaptiveDecimalStepType)
 		except:
 			pass
 
 	def setSingleStep(self, value):
-		self.setStepType(QAbstractSpinBox.DefaultStepType)
+		self.setStepType(QAbstractSpinBox.StepType.DefaultStepType)
 		super().setSingleStep(value)
 
 	def textFromValue(self, value):
 		if value and abs(np.log10(abs(value))) > 5:
 			return(f"{value:.2e}")
 		else:
 			return(f"{value:.10f}".rstrip("0").rstrip("."))
@@ -5663,22 +5630,22 @@
 		min = min if not min is None else -np.inf
 		max = max if not max is None else +np.inf
 		return super().setRange(min, max)
 
 	def validate(self, text, position):
 		try:
 			np.float64(text)
-			return(2, text, position)
+			return(QValidator.State(2), text, position)
 		except ValueError:
 			if text.strip() in ["+", "-", ""]:
-				return(1, text, position)
+				return(QValidator.State(1), text, position)
 			elif re.match(r"^[+-]?\d+\.?\d*[Ee][+-]?\d?$", text):
-				return(1, text, position)
+				return(QValidator.State(1), text, position)
 			else:
-				return(0, text, position)
+				return(QValidator.State(0), text, position)
 
 	def fixup(self, text):
 		tmp = re.search(r"[+-]?\d+\.?\d*", text)
 		if tmp:
 			return(tmp[0])
 		else:
 			return(str(0))
@@ -5699,65 +5666,65 @@
 
 		self.data = data
 		self.headers = headers if headers else data.columns
 		self.hiddencolumns = hiddencolumns
 		self.editable = editable
 
 	def data(self, index, role):
-		if role == Qt.DisplayRole or role == Qt.EditRole:
+		if role == Qt.ItemDataRole.DisplayRole or role == Qt.ItemDataRole.EditRole:
 			value = self.data.iloc[index.row(), index.column()]
 			dtype = self.data[self.data.columns[index.column()]].dtypes
 
 			if isinstance(value, str):
 				return(value)
 			elif isinstance(value, (np.integer, int)):
 				if value == pyckett.SENTINEL:
 					return("")
 				else:
-					if role == Qt.EditRole:
+					if role == Qt.ItemDataRole.EditRole:
 						return(str(value))
 					else:
 						return(f"{{:{main.config['flag_tableformatint']}}}".format(value))
 			elif np.isnan(value):
 				return("")
 			else:
-				if role == Qt.EditRole:
+				if role == Qt.ItemDataRole.EditRole:
 					return(str(value))
 				else:
 					return(f"{{:{main.config['flag_tableformatfloat']}}}".format(value))
 
 	def rowCount(self, index):
 		return(self.data.shape[0])
 
 	def columnCount(self, index):
 		return(self.data.shape[1]-len(self.hiddencolumns))
 
 	def headerData(self, section, orientation, role):
-		if role == Qt.DisplayRole:
-			if orientation == Qt.Horizontal:
+		if role == Qt.ItemDataRole.DisplayRole:
+			if orientation == Qt.Orientation.Horizontal:
 				return str(self.headers[section])
 
-			if orientation == Qt.Vertical:
+			if orientation == Qt.Orientation.Vertical:
 				if section >= len(self.data.index):
 					return ""
 				return str(self.data.index[section])
 
 	def flags(self, index):
 		if self.editable:
-			return(Qt.ItemIsEnabled | Qt.ItemIsSelectable | Qt.ItemIsEditable)
+			return(Qt.ItemFlag.ItemIsEnabled | Qt.ItemFlag.ItemIsSelectable | Qt.ItemFlag.ItemIsEditable)
 		else:
-			return(Qt.ItemIsEnabled | Qt.ItemIsSelectable)
+			return(Qt.ItemFlag.ItemIsEnabled | Qt.ItemFlag.ItemIsSelectable)
 
 	def update(self):
 		self.layoutChanged.emit()
 
 	def setData(self, index, value, role):
 		if not index.isValid():
 			return False
-		if role != Qt.EditRole:
+		if role != Qt.ItemDataRole.EditRole:
 			return False
 
 		row = index.row()
 		if row < 0 or row >= len(self.data):
 			return False
 		column = index.column()
 		if column < 0 or column >= self.data.columns.size:
@@ -5915,45 +5882,45 @@
 	if "y" not in dataframe:
 		dataframe = dataframe.loc[dataframe.drop_duplicates(("bin", "filename"), keep="last").sort_values(["x"]).index]
 	else:
 		dataframe = dataframe.loc[dataframe.sort_values("y").drop_duplicates(("bin", "filename"), keep="last").sort_values(["x"]).index]
 	return(dataframe)
 
 def csv_copypaste(self, event):
-	if event.key() == Qt.Key_C and (event.modifiers() & Qt.ControlModifier):
+	if event.key() == Qt.Key.Key_C and (event.modifiers() == Qt.KeyboardModifier.ControlModifier):
 		cells = sorted(self.selectedIndexes())
 		output = []
 		i = 0
 
 		while i < len(cells):
 			tmp = []
 			row = cells[i].row()
 			while i < len(cells) and cells[i].row() == row:
 				tmp.append(cells[i].data())
 				i += 1
 			output.append("\t".join(tmp))
 		output = "\n".join(output)
 		QApplication.clipboard().setText(output)
 
-	elif event.key() == Qt.Key_V and (event.modifiers() & Qt.ControlModifier):
-		if QAbstractItemView.NoEditTriggers == self.editTriggers():
+	elif event.key() == Qt.Key.Key_V and (event.modifiers() == Qt.KeyboardModifier.ControlModifier):
+		if QAbstractItemView.EditTrigger.NoEditTriggers == self.editTriggers():
 			return
 		cells = sorted(self.selectedIndexes())
 		if not cells:
 			return
 		text = QApplication.clipboard().text()
 		data = [row.split("\t") for row in text.split("\n")]
 		i_0, j_0 = cells[0].row(), cells[0].column()
 
 		for i, row in enumerate(data):
 			j_hidden = 0
 			for j, value in enumerate(row):
 				while self.isColumnHidden(j_0+j+j_hidden):
 					j_hidden += 1
-				self.model().setData(self.model().index(i_0+i, j_0+j+j_hidden), value, Qt.EditRole)
+				self.model().setData(self.model().index(i_0+i, j_0+j+j_hidden), value, Qt.ItemDataRole.EditRole)
 	else:
 		return False
 	return True
 
 def trgb_to_rgbt(color):
 	if len(color) == 9:
 		color = f"#{color[3:]}{color[1:3]}"
@@ -6038,15 +6005,15 @@
 def breakpoint(ownid, lastid):
 	if ownid != lastid:
 		raise CustomError()
 
 def commandline(showdialog=True):
 	if showdialog:
 		dialog = ConsoleDialog()
-		dialog.exec_()
+		dialog.exec()
 		if dialog.result() != 1:
 			return
 
 	title, command = main.config["commandlinedialog_commands"][main.config["commandlinedialog_current"]]
 	if not command.strip():
 		return
 	message = []
@@ -6064,21 +6031,20 @@
 	message.append(red_output.getvalue())
 	main.notification("\n".join(message))
 
 def send_mail_to_author():
 	webbrowser.open(f"mailto:bonah@ph1.uni-koeln.de?subject={APP_TAG}")
 
 def restart():
-	dir = os.path.dirname(os.path.realpath(__file__))
-	fname = os.path.join(dir, llwpfile(".llwp"))
+	fname = llwpfile(".llwp")
 	main.saveproject(fname)
 	main.saveoptions()
 	if not main.new_df.empty:
 		main.save_lines_lin(llwpfile(".lin"), force_noappend=True, force_lin=True)
-	os.execv(sys.executable, [sys.executable, sys.argv[0], fname])
+	os.execl(sys.executable, sys.executable, __file__, fname)
 
 def lineshape(shape, derivative, *args):
 	if shape == "Gauss":
 		x, x_0, amp, width = args
 		width = width/(2*np.sqrt(2*np.log(2)))
 		if width == 0:
 			return [0 if i!=x_0 else np.inf for i in x]
@@ -6165,16 +6131,14 @@
 }
 
 cat_dtypes = pyckett.cat_dtypes
 lin_dtypes = pyckett.lin_dtypes
 
 config_specs = {
 	# Format is: [default value, class]
-	"layout_theme":							["light", str],
-	"layout_owntheme":						[{}, dict],
 	"layout_mpltoolbar":					[False, bool],
 
 	"color_exp":							["#000000", Color],
 	"color_lin":							["#ff38fc", Color],
 	"color_cat":							["#d91e6f", Color],
 	"color_cur":							["#71eb34", Color],
 	"color_fit":							["#bc20e3", Color],
@@ -6229,17 +6193,17 @@
 	"flag_xcolumn":							[0, int],
 	"flag_ycolumn":							[1, int],
 	"flag_separator":						[9, int],
 	"flag_debug":							[False, bool],
 	"flag_alwaysshowlog":					[True, bool],
 	"flag_extensions":						[{"exp": [".csv"], "cat": [".cat"], "lin": [".lin"], "project": [".llwp"]}, dict],
 	"flag_autosetqns":						[True, bool],
-	"flag_predictionformats":				[{}, dict, True],
-	"flag_assignmentformats":				[{}, dict, True],
-	"flag_assignmentsavefmt":				[{}, dict, True],
+	"flag_predictionformats":				[{}, dict],
+	"flag_assignmentformats":				[{}, dict],
+	"flag_assignmentsavefmt":				[{}, dict],
 	"flag_loadfilesthreaded":				[True, bool],
 	"flag_shownotification":				[True, bool],
 	"flag_notificationtime":				[2000, int],
 	"flag_showmainplotcontrols":			[True, bool],
 	"flag_showmainplotwidth":				[True, bool],
 	"flag_showmainplotrowscols":			[True, bool],
 	"flag_showmainplotposition":			[True, bool],
@@ -6261,14 +6225,15 @@
 	"blendedlineswindow_polynom":			[0, int],
 	"blendedlineswindow_fixedwidth":		[False, bool],
 	"blendedlineswindow_showbaseline":		[True, bool],
 	"blendedlineswindow_xpoints":			[1000, int],
 	"blendedlineswindow_color_total":		["#3d5dff", Color],
 	"blendedlineswindow_color_points":		["#ff3352", Color],
 	"blendedlineswindow_color_baseline":	["#f6fa14", Color],
+	"blendedlineswindow_autopositionpeaks":	[True, bool],
 
 	"lineshapewindow_lineshape":			["Gauss", str],
 	"lineshapewindow_derivative":			[0, int],
 	"lineshapewindow_scaling_factor":		[1, float],
 	"lineshapewindow_scaling_exponent":		[10, int],
 	"lineshapewindow_gauss":				[1, float],
 	"lineshapewindow_lorentz":				[1, float],
```

### Comparing `llwp-1.3.1/llwp/LLWP.svg` & `llwp-1.3.2/llwp/LLWP.svg`

 * *Files identical despite different names*

### Comparing `llwp-1.3.1/llwp.egg-info/PKG-INFO` & `llwp-1.3.2/llwp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llwp
-Version: 1.3.1
+Version: 1.3.2
 Summary: LLWP is a fast, efficient and easy solution for exploring and assigning spectra - relying on Loomis-Wood plots.
 Author-email: Luis Bonah <bonah@ph1.uni-koeln.de>
 Project-URL: Homepage, https://llwp.astro.uni-koeln.de/
 Keywords: LLWP,Loomis-Wood Plots,Spectroscopy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `llwp-1.3.1/pyproject.toml` & `llwp-1.3.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llwp"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Luis Bonah", email="bonah@ph1.uni-koeln.de" },
 ]
 description = "LLWP is a fast, efficient and easy solution for exploring and assigning spectra - relying on Loomis-Wood plots."
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = ['numpy', 'pandas', 'matplotlib', 'wrapt', 'pyckett', 'scipy', 'PyQt5']
+dependencies = ['numpy', 'pandas', 'matplotlib', 'wrapt', 'pyckett', 'scipy', 'PyQt6']
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 	"Operating System :: OS Independent",
 ]
 keywords = ["LLWP", "Loomis-Wood Plots", "Spectroscopy"]
```

