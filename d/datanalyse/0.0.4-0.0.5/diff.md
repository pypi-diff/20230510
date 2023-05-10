# Comparing `tmp/datanalyse-0.0.4.tar.gz` & `tmp/datanalyse-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datanalyse-0.0.4.tar", last modified: Mon May  8 20:32:43 2023, max compression
+gzip compressed data, was "datanalyse-0.0.5.tar", last modified: Wed May 10 08:48:10 2023, max compression
```

## Comparing `datanalyse-0.0.4.tar` & `datanalyse-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     1078 2023-05-06 19:06:32.333418 datanalyse-0.0.4/LICENSE
--rw-r--r--   0        0        0      459 2023-05-06 20:17:48.271205 datanalyse-0.0.4/README.md
--rw-r--r--   0        0        0      685 2023-05-08 20:32:43.119241 datanalyse-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 18:40:19.058776 datanalyse-0.0.4/src/datanalyse/__init__.py
--rw-r--r--   0        0        0        0 2023-05-06 12:49:40.254042 datanalyse-0.0.4/src/datanalyse/dataelement/__init__.py
--rw-r--r--   0        0        0     8724 2023-05-06 19:27:23.414206 datanalyse-0.0.4/src/datanalyse/dataelement/dataelement.py
--rw-r--r--   0        0        0     3492 2023-05-08 19:59:39.673710 datanalyse-0.0.4/src/datanalyse/dataelement/dfmanipulation.py
--rw-r--r--   0        0        0    32084 2023-05-08 20:31:46.831458 datanalyse-0.0.4/src/datanalyse/dataelement/formate.py
--rw-r--r--   0        0        0      362 2023-05-08 19:59:45.459719 datanalyse-0.0.4/src/datanalyse/dataelement/stoffwerte.py
--rw-r--r--   0        0        0        0 2023-05-08 18:40:19.069280 datanalyse-0.0.4/src/datanalyse/diagramme/__init__.py
--rw-r--r--   0        0        0     4753 2023-05-08 20:30:15.275768 datanalyse-0.0.4/src/datanalyse/diagramme/balken.py
--rw-r--r--   0        0        0     2863 2023-05-08 19:59:19.452792 datanalyse-0.0.4/src/datanalyse/diagramme/diagramm.py
--rw-r--r--   0        0        0     4224 2023-05-08 19:59:23.694912 datanalyse-0.0.4/src/datanalyse/diagramme/globalbewertung.py
--rw-r--r--   0        0        0     1102 2023-05-08 19:59:25.417764 datanalyse-0.0.4/src/datanalyse/diagramme/matplotlib_parameter.py
--rw-r--r--   0        0        0     3115 2023-05-08 20:30:59.493810 datanalyse-0.0.4/src/datanalyse/diagramme/zeitreihe.py
--rw-r--r--   0        0        0      703 2023-04-28 12:58:07.459695 datanalyse-0.0.4/src/datanalyse/pfade.py
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 datanalyse-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-08 10:35:18.120135 datanalyse-0.0.5/LICENSE
+-rw-r--r--   0        0        0      459 2023-05-08 11:21:31.284922 datanalyse-0.0.5/README.md
+-rw-r--r--   0        0        0      664 2023-05-10 08:48:10.438077 datanalyse-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 13:28:09.975326 datanalyse-0.0.5/src/datanalyse/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 21:03:10.188371 datanalyse-0.0.5/src/datanalyse/dataelement/__init__.py
+-rw-r--r--   0        0        0     8844 2023-05-10 07:45:44.270328 datanalyse-0.0.5/src/datanalyse/dataelement/dataelement.py
+-rw-r--r--   0        0        0     3492 2023-05-08 20:06:25.263720 datanalyse-0.0.5/src/datanalyse/dataelement/dfmanipulation.py
+-rw-r--r--   0        0        0    32051 2023-05-10 07:45:44.276278 datanalyse-0.0.5/src/datanalyse/dataelement/formate.py
+-rw-r--r--   0        0        0      362 2023-05-08 20:06:25.269023 datanalyse-0.0.5/src/datanalyse/dataelement/stoffwerte.py
+-rw-r--r--   0        0        0        0 2022-11-21 14:15:44.602999 datanalyse-0.0.5/src/datanalyse/diagramme/__init__.py
+-rw-r--r--   0        0        0     4753 2023-05-10 07:45:44.282229 datanalyse-0.0.5/src/datanalyse/diagramme/balken.py
+-rw-r--r--   0        0        0     2863 2023-05-08 20:06:25.272554 datanalyse-0.0.5/src/datanalyse/diagramme/diagramm.py
+-rw-r--r--   0        0        0     4224 2023-05-08 20:06:25.274579 datanalyse-0.0.5/src/datanalyse/diagramme/globalbewertung.py
+-rw-r--r--   0        0        0     1102 2023-05-08 20:06:25.278540 datanalyse-0.0.5/src/datanalyse/diagramme/matplotlib_parameter.py
+-rw-r--r--   0        0        0     3115 2023-05-10 07:45:44.288184 datanalyse-0.0.5/src/datanalyse/diagramme/zeitreihe.py
+-rw-r--r--   0        0        0      703 2023-05-08 10:35:18.138208 datanalyse-0.0.5/src/datanalyse/pfade.py
+-rw-r--r--   0        0        0   149819 2023-05-10 07:45:44.296614 datanalyse-0.0.5/tests/Ahlborn.xlsx
+-rw-r--r--   0        0        0      376 2023-05-10 08:29:38.906242 datanalyse-0.0.5/tests/test_dataelement.py
+-rw-r--r--   0        0        0     1011 1970-01-01 00:00:00.000000 datanalyse-0.0.5/PKG-INFO
```

### Comparing `datanalyse-0.0.4/LICENSE` & `datanalyse-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.4/pyproject.toml` & `datanalyse-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [project]
 name = "datanalyse"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "Maximilian Beyer", email = "maximilian.beyer@tu-dresden.de" },
 ]
 description = "A data analysis package."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "pandas>=2.0.1",
     "matplotlib>=3.7.1",
-    "black>=23.3.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/MakusuB/datanalyse"
 "Bug Tracker" = "https://github.com/MakusuB/datanalyse/issues"
 
 [build-system]
```

### Comparing `datanalyse-0.0.4/src/datanalyse/dataelement/dataelement.py` & `datanalyse-0.0.5/src/datanalyse/dataelement/dataelement.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
         oberelement=None,
         unterelemente: list = [],
     ):
         """
         Objekt, welches die Daten einer Datei / eines Versuchs / einer Versuchsreihe beinhaltet.
         Ein Dataelement kann wiederum aus mehreren Unterelementen bestehen und/oder zu einem Oberelement dazugehören.
         :param pfad: Pfad zur Datei / zum Versuch(sreihen)ordner (als pathlib-Objekt)
-        :param daten: Daten (als Dataframe-Objekt, optional)
+        :param daten: Daten (als Dataframe-Objekt, optional)        
+        :param name: Name des Dataelements (optional), entspricht falls nicht angegeben dem Datei-/Ordnernamen
         :param oberelement: Zuweisung des Objekts zu einem übergeordneten Dataelement (optional)
         :param unterelemente: Liste mit allen zum Objekt gehörenden untergeordneten Dataelementen (optional)
         """
 
         # übergebene statische Attribute:
         self.pfad = pfad
         self.daten = daten
@@ -103,15 +104,15 @@
                 "AttributeError in der Funktion lese_daten_unformatiert_ein",
             )
 
     def lese_daten_formatiert_ein(self, format_dict: dict):
         if self.elementtyp == "datei":
             for key in format_dict.keys():
                 if key in self.name:
-                    self.daten = format_dict[key](Dataelement=self)
+                    self.daten = format_dict[key](dataelement=self)
                     break
         else:
             print(
                 datetime.now(),
                 "Fehler in",
                 self.name + ":",
                 "Typ Ordner kann keine Rohdaten einlesen.",
```

### Comparing `datanalyse-0.0.4/src/datanalyse/dataelement/dfmanipulation.py` & `datanalyse-0.0.5/src/datanalyse/dataelement/dfmanipulation.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.4/src/datanalyse/dataelement/formate.py` & `datanalyse-0.0.5/src/datanalyse/dataelement/formate.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 # from .dataelement import Dataelement - does not work in vsc
 # from src.datanalyse.dataelement.dataelement import Dataelement - does not work in vsc
 from .dataelement import Dataelement
 from . import dfmanipulation as dfm
 
 
 def wincontrol_standard(
-    datenelement: Dataelement,
+    dataelement: Dataelement,
     dropna_spalten=True,
     dropna_zeilen=True,
     rolling_zeitschritt=None,
     resample_zeitschritt="1min",
     nur_ergebniszeile=False,
 ):
     """
     Standard-Einlese-Formatierung für xlsx-Daten aus einer WinControl-Tabelle
-    :param datenelement: Dataelement
+    :param dataelement: Dataelement
     :param dropna_spalten: drop alle leeren Spalten
     :param dropna_zeilen: drop alle Zeilen mit teilweise leerem Inhalt
     :param rolling_zeitschritt: Es wird über die Höhe des Zeitschritts der gleitende Mittelwert gebildet
     :param resample_zeitschritt: Resampling aller Daten dient der Umrechnung auf eine gemeinsame Zeitschrittweite, es werden alle zur Zeitschrittweite gehörenden Werte gemittelt
     :param nur_ergebniszeile:
     :return: formatiertes Dataelement
     """
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         parse_dates=[
             ["Datum", "Zeit"]
         ],  # Datum und Zeit werden zum Zeitstempel kombiniert
     )
 
     # Zeitstempel wird als Index gesetzt
@@ -75,33 +75,33 @@
     )
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
 def wincontrol_csv(
-    datenelement: Dataelement,
+    dataelement: Dataelement,
     dropna_spalten=True,
     dropna_zeilen=True,
     rolling_zeitschritt=None,
     resample_zeitschritt="1min",
     nur_ergebniszeile=False,
 ):
     """
     Standard-Einlese-Formatierung für csv-Daten aus einer WinControl-Tabelle
-    :param datenelement: Dataelement
+    :param dataelement: Dataelement
     :param dropna_spalten: drop alle leeren Spalten
     :param dropna_zeilen: drop alle Zeilen mit teilweise leerem Inhalt
     :param rolling_zeitschritt: Es wird über die Höhe des Zeitschritts der gleitende Mittelwert gebildet
     :param resample_zeitschritt: Resampling aller Daten dient der Umrechnung auf eine gemeinsame Zeitschrittweite, es werden alle zur Zeitschrittweite gehörenden Werte gemittelt
     :param nur_ergebniszeile:
     :return: formatiertes Dataelement
     """
     df = pd.read_csv(
-        datenelement.pfad,
+        dataelement.pfad,
         sep=";",
         decimal=",",
         encoding="ANSI",
         index_col=0,
         header=2,
         skiprows=[3, 4, 5, 6],
         parse_dates=[[0, 1]],
@@ -127,30 +127,30 @@
         df, rolling_zeitschritt, resample_zeitschritt, nur_ergebniszeile
     )
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
-def mothership(datenelement: Dataelement):
+def mothership(dataelement: Dataelement):
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         header=4,
         index_col=0,
     )
 
     # Überspring die ersten beiden Zeilen, da leer bzw. 0
     df = df.iloc[2:]
 
     # Konvertiere Zeitstempel-String im Index zu echtem Zeitstempel
     df.index = pd.to_datetime(df.index)
 
     # Das Datum der Messung wird aus dem Dateinamen entnommen
-    messdatum = pd.to_datetime(str(datenelement.pfad.name)[37:47], format="%d_%m_%Y")
+    messdatum = pd.to_datetime(str(dataelement.pfad.name)[37:47], format="%d_%m_%Y")
     # ersetze Datum im Zeitstempel durch das Datum der Speicherzeit
     df.index = df.index.map(
         lambda x: x.replace(
             year=messdatum.year, month=messdatum.month, day=messdatum.day
         )
     )
 
@@ -161,17 +161,17 @@
     # Lösche Sollwerte, da keine sinnvollen Werte enthalten
     df.drop(labels="Sollwert aller Wände", axis=1, inplace=True)
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
-def klimaanlage(datenelement: Dataelement):
+def klimaanlage(dataelement: Dataelement):
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         header=9,
         index_col="Name",  # Die Zeitstempel stehen in Excel unter der Spalte "Name"
     )
 
     # Überspring die ersten 4 Zeilen, da leer bzw. 0
     df = df.iloc[4:]
@@ -211,21 +211,21 @@
     # Resampling der Daten
     df = df.resample("1min").mean()
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
-def umbuzoo_standard(datenelement: Dataelement):
+def umbuzoo_standard(dataelement: Dataelement):
     pass
 
 
-def umbuzoo_person(datenelement: Dataelement):
+def umbuzoo_person(dataelement: Dataelement):
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         header=None,
         index_col=None,
         skiprows=8,  # 8 Zeilen unnützer Informationen werden direkt beim Einlesen übersprungen
     )
 
     # Spalten entfernen, die komplett leer sind (Abstandsspalten des ursprünglichen Files)
@@ -279,17 +279,17 @@
         df, ["Geschlecht"], ["männlich", "weiblich", "divers"], [1, 0, -1]
     )  # V2.0
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
-def umbuzoo_abschluss_viessmann(datenelement: Dataelement):
+def umbuzoo_abschluss_viessmann(dataelement: Dataelement):
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         header=None,
         index_col=None,
         skiprows=8,  # 8 Zeilen unnützer Informationen werden direkt beim Einlesen übersprungen
     )
 
     # Spalten entfernen, die komplett leer sind (Abstandsspalten des ursprünglichen Files)
@@ -356,17 +356,17 @@
         [2, 1, 0, -1, -2],
     )
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
-def umbuzoo_klimaraum(datenelement: Dataelement):
+def umbuzoo_klimaraum(dataelement: Dataelement):
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         header=None,
         index_col=None,
         skiprows=8,  # 8 Zeilen unnützer Informationen werden direkt beim Einlesen übersprungen
     )
 
     # Spalten entfernen, die komplett leer sind (Abstandsspalten des ursprünglichen Files)
@@ -443,17 +443,17 @@
         df, ["Luftqualität"], ["1", "2", "3", "4", "5"], range(-2, 3)
     )
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
-def umbuzoo_klimaraum_hybrid(datenelement: Dataelement):
+def umbuzoo_klimaraum_hybrid(dataelement: Dataelement):
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         header=None,
         index_col=None,
         skiprows=8,  # 8 Zeilen unnützer Informationen werden direkt beim Einlesen übersprungen
     )
 
     # Spalten entfernen, die komplett leer sind (Abstandsspalten des ursprünglichen Files)
@@ -566,17 +566,17 @@
         df, ["Luftqualität", "Störgeräusche"], ["1", "2", "3", "4", "5"], range(1, 6)
     )
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
-def umbuzoo_klimaraum_viessmann(datenelement: Dataelement):
+def umbuzoo_klimaraum_viessmann(dataelement: Dataelement):
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         header=None,
         index_col=None,
         skiprows=8,  # 8 Zeilen unnützer Informationen werden direkt beim Einlesen übersprungen
     )
 
     # Spalten entfernen, die komplett leer sind (Abstandsspalten des ursprünglichen Files)
@@ -661,17 +661,17 @@
         df, ["Luftqualität"], ["1", "2", "3", "4", "5"], range(-2, 3)
     )
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
-def versuchsleitung_normhybr(datenelement: Dataelement):
+def versuchsleitung_normhybr(dataelement: Dataelement):
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         header=0,
         index_col=0,
         nrows=9,  # Verwende nur die ersten 9 Zeilen
         usecols="A:H",  # Verwende nur diese Spalten (G/H enthält ggf. Bemerkungen)
     )
 
@@ -680,15 +680,15 @@
         columns={"Unnamed: 6": "Kommentar", "Unnamed: 7": "Kommentar"}, inplace=True
     )
 
     # Entferne leere Spalten (es verbleibt nur die Kommentarspalte, in der auch etwas steht)
     df.dropna(how="all", axis=1, inplace=True)
 
     # Konvertiere Uhrzeit mit dem Messdatum (Erhalt aus dem Änderungsdatum der Datei) zu echtem Zeitstempel
-    messdatum = datetime.utcfromtimestamp(datenelement.pfad.stat().st_mtime)
+    messdatum = datetime.utcfromtimestamp(dataelement.pfad.stat().st_mtime)
     df.index = df.index.map(lambda x: datetime.combine(messdatum, x))
 
     # Phasenspalte aufräumen, sodass nur noch Zeilen mit den Phasen-Startzeitpunkten enthalten sind
     df = df[df["Phase"].str.contains("Phase")]
 
     # Spalte mit Reihenfolge der Deckentemperaturen ergänzen durch Vergleich des letzten mit erstem Sollwert
     if df["Deckentemp. (°C)"][-1] > df["Deckentemp. (°C)"][0]:
@@ -696,59 +696,59 @@
     else:
         df = df.assign(Rang="absteigend")
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
-def versuchsleitung_halbraum(datenelement: Dataelement):
+def versuchsleitung_halbraum(dataelement: Dataelement):
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         header=9,
         index_col=1,
         nrows=7,  # Verwende nur die ersten 8 Zeilen
         usecols="B:G",  # Verwende nur diese 5 Spalten
     )
     df.drop(
         index=["hh:mm"], inplace=True
     )  # Löschen der ersten Zeile, da nur Einheiten enthalten
 
     # Konvertiere Uhrzeit mit dem Messdatum (Erhalt aus dem Änderungsdatum der Datei) zu echtem Zeitstempel
-    messdatum = datetime.utcfromtimestamp(datenelement.pfad.stat().st_mtime)
+    messdatum = datetime.utcfromtimestamp(dataelement.pfad.stat().st_mtime)
     df.index = df.index.map(lambda x: datetime.combine(messdatum, x))
 
     # 1 Minuten addiert, da die erste Umfrage einer Phase genau die relevante für die Phase DAVOR ist
     df.index = df.index + pd.DateOffset(minutes=1)
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
-def versuchsleitung_viessmann(datenelement: Dataelement):
+def versuchsleitung_viessmann(dataelement: Dataelement):
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         header=0,
         index_col=0,
         nrows=6,  # Verwende nur die ersten 8 Zeilen
     )
 
     # Konvertiere Uhrzeit mit dem Messdatum (Erhalt aus dem Änderungsdatum der Datei) zu echtem Zeitstempel
-    messdatum_raw = datenelement.name[:10].replace("_", "-")
+    messdatum_raw = dataelement.name[:10].replace("_", "-")
     messdatum = pd.to_datetime(messdatum_raw)
     df.index = df.index.map(lambda x: datetime.combine(messdatum, x))
 
     # Übergebe das fertige Dataframe zurück
     return df
 
 
-def versuchsleitung_standard(datenelement: Dataelement):
+def versuchsleitung_standard(dataelement: Dataelement):
     df = pd.read_excel(
-        datenelement.pfad,
+        dataelement.pfad,
         sheet_name=0,
         header=0,
         index_col=0,
         parse_dates=[["Datum", "Uhrzeit"]],
     )  # Verhindert Verwechslung von Tag und Monat beim Einlesen des Datums
 
     # Übergebe das fertige Dataframe zurück
```

### Comparing `datanalyse-0.0.4/src/datanalyse/diagramme/balken.py` & `datanalyse-0.0.5/src/datanalyse/diagramme/balken.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.4/src/datanalyse/diagramme/diagramm.py` & `datanalyse-0.0.5/src/datanalyse/diagramme/diagramm.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.4/src/datanalyse/diagramme/globalbewertung.py` & `datanalyse-0.0.5/src/datanalyse/diagramme/globalbewertung.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.4/src/datanalyse/diagramme/matplotlib_parameter.py` & `datanalyse-0.0.5/src/datanalyse/diagramme/matplotlib_parameter.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.4/src/datanalyse/diagramme/zeitreihe.py` & `datanalyse-0.0.5/src/datanalyse/diagramme/zeitreihe.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.4/src/datanalyse/pfade.py` & `datanalyse-0.0.5/src/datanalyse/pfade.py`

 * *Files identical despite different names*

### Comparing `datanalyse-0.0.4/PKG-INFO` & `datanalyse-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: datanalyse
-Version: 0.0.4
+Version: 0.0.5
 Summary: A data analysis package.
 Author-Email: Maximilian Beyer <maximilian.beyer@tu-dresden.de>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/MakusuB/datanalyse
 Project-URL: Bug tracker, https://github.com/MakusuB/datanalyse/issues
 Requires-Python: >=3.11
 Requires-Dist: pandas>=2.0.1
 Requires-Dist: matplotlib>=3.7.1
-Requires-Dist: black>=23.3.0
 Description-Content-Type: text/markdown
 
 # datanalyse
 
 The package name datanalyse is a suitcase word for data and analyse - mainly of experimental data from the Combined Energy Lab at TU Dresden, but perhaps useful for others as well. However, due to its absolute alpha status, I cannot recommend it to anybody in the world but me.
 
 It is more or less a tool-kit for my daily work as an experimentalist and data scientist and makes use of the fantastic packages pandas, pathlib and matplotlib.
```

